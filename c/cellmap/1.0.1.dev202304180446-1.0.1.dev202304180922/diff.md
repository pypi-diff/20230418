# Comparing `tmp/cellmap-1.0.1.dev202304180446-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304180922-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1388586 bytes, number of entries: 6
+Zip file size: 1389868 bytes, number of entries: 6
 -rw-r--r--  2.0 unx  4446947 b- defN 80-Jan-01 00:00 cellmap/CellMap_view_3D.html
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    55277 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304180446.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304180446.dist-info/WHEEL
-?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304180446.dist-info/RECORD
-6 files, 4504641 bytes uncompressed, 1387700 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx    60852 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304180922.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304180922.dist-info/WHEEL
+?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304180922.dist-info/RECORD
+6 files, 4510216 bytes uncompressed, 1388982 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304180446.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304180922.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304180446.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304180922.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304180446.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304180922.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -1,14 +1,15 @@
 from adjustText import adjust_text
 import anndata
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
 from matplotlib import patheffects as PathEffects
 import matplotlib.cm
+import networkx as nx
 import scipy
 import sklearn.preprocessing
 import sklearn.neighbors
 import matplotlib.colors
 import pandas as pd
 import logging
 import scanpy
@@ -1249,8 +1250,103 @@
         X2 = data_pos[:,idx][triangles[:,id_y]]
         V1 = data_vel[:,idx][triangles[:,id_x]]
         V2 = data_vel[:,idx][triangles[:,id_y]]
         weight = np.sum(0.5*(V1+V2)*(X2-X1),axis=1)
         min_weight = np.percentile(np.abs(weight),5)
         graph_[tuple(triangles[weight>min_weight][:,[id_x,id_y]].T[::-1])] = 1
         graph_[tuple(triangles[weight<-min_weight][:,[id_y,id_x]].T[::-1])] = 1
-    return scipy.sparse.coo_matrix(graph_)
+    return scipy.sparse.coo_matrix(graph_)
+
+
+
+def view_trajectory(
+    adata,
+    source_cluster,
+    target_clusters,
+    n_cells = 50,
+    register = 10,
+    basis = 'umap',
+    potential_key = 'potential',
+    cluster_key = 'clusters',
+    graph_method = 'Delauney',
+    n_neighbors = 10,
+    contribution_rate_pca = 0.95,
+    cutedge_vol  = None,
+    cutedge_length = None,
+):
+
+    # kwargs_arg = check_arguments(adata, verbose = True, exp_key=exp_key, vkey = vkey, basis=basis, graph_method=graph_method)
+    # exp_key,vkey,basis = kwargs_arg['exp_key'],kwargs_arg['vkey'],kwargs_arg['basis']
+
+    basis_key = 'X_%s' % basis
+    data_pos = adata.obsm[basis_key]
+
+    ## Compute graph and edge velocities
+    if graph_method == 'Delauney':
+        tri_,idx_tri = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
+        source, target = np.ravel(tri_.triangles[idx_tri][:,[0,1,2]]),np.ravel(tri_.triangles[idx_tri][:,[1,2,0]])
+    elif graph_method == 'knn':
+        pca = sklearn.decomposition.PCA()
+        exp_HD_pca = pca.fit_transform(data_pos)
+        n_pca = np.min(np.arange(len(pca.explained_variance_ratio_))[np.cumsum(pca.explained_variance_ratio_)>contribution_rate_pca])
+        knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
+        knn.fit(exp_HD_pca[:,:n_pca])
+        distances, indices = knn.kneighbors(exp_HD_pca[:,:n_pca])
+        distances, indices = distances[:,1:], indices[:,1:]
+        source = np.ravel(np.repeat(np.arange(data_pos.shape[0]).reshape((-1, 1)),n_neighbors,axis=1))
+        target = np.ravel(indices)
+
+    G = nx.DiGraph()
+
+    def cost(data_pos,s,t,g,reg):
+        return np.exp(-g*reg)*np.linalg.norm(data_pos[s]-data_pos[t])
+    grad_ = adata.obs[potential_key][source].values - adata.obs[potential_key][target].values
+    G.add_weighted_edges_from([(int(s),int(t),cost(data_pos,int(s),int(t),g,register)) for s,t,g in np.vstack((source[grad_>0],target[grad_>0],grad_[grad_>0])).T])
+    G.add_weighted_edges_from([(int(t),int(s),cost(data_pos,int(s),int(t),-g,register)) for s,t,g in np.vstack((source[grad_>0],target[grad_>0],grad_[grad_>0])).T])
+    G.add_weighted_edges_from([(int(t),int(s),cost(data_pos,int(s),int(t),-g,register)) for s,t,g in np.vstack((source[grad_<0],target[grad_<0],grad_[grad_<0])).T])
+    G.add_weighted_edges_from([(int(s),int(t),cost(data_pos,int(s),int(t),g,register)) for s,t,g in np.vstack((source[grad_<0],target[grad_<0],grad_[grad_<0])).T])
+    
+    cmap_ = plt.get_cmap("tab10")
+    figsize = (10,8)
+    fig,ax = plt.subplots(figsize=figsize)
+    ax.triplot(tri_,color='gray',zorder=0,alpha=0.2,lw=1)
+    clusters_ = adata.obs[cluster_key]
+    idx_ = clusters_ == source_cluster
+    ax.scatter(data_pos[idx_,0],data_pos[idx_,1],color=cmap_(0),zorder=10,marker='o',alpha=0.2,s=5,label=source_cluster+' (source)')
+    for i_trg_ in range(len(target_clusters)):
+        idx_ = clusters_ == target_clusters[i_trg_]
+        ax.scatter(data_pos[idx_,0],data_pos[idx_,1],color=cmap_(i_trg_+1),zorder=10,marker='o',alpha=0.2,s=5,label=target_clusters[i_trg_]+' (target)')
+    leg = ax.legend(bbox_to_anchor=(1.05, 1), loc='upper left', borderaxespad=0, fontsize=12,markerscale=3)
+    for lh in leg.legendHandles: lh.set_alpha(1)
+
+    data_src_ = data_pos[adata.obs[cluster_key].values == source_cluster]
+    center_src_ = np.mean(data_src_,axis=0)
+    centrality_src_ = np.linalg.norm(data_src_-center_src_,axis=1)
+    src_set_all_ = np.arange(adata.shape[0])[adata.obs[cluster_key].values == source_cluster][np.argsort(centrality_src_)]
+    n_src_ = sum(adata.obs[cluster_key].values == source_cluster)
+    for i_trg_ in range(len(target_clusters)):
+        target_cluster = target_clusters[i_trg_]
+        n_cells_ = np.min([n_cells,sum(adata.obs[cluster_key].values == source_cluster),sum(adata.obs[cluster_key].values == target_cluster)])
+        data_trg_ = data_pos[adata.obs[cluster_key].values == target_cluster]
+        center_trg_ = np.mean(data_trg_,axis=0)
+        centrality_trg_ = np.linalg.norm(data_trg_-center_trg_,axis=1)
+        n_trg_ = sum(adata.obs[cluster_key].values == target_cluster)
+        idx_trg_ = np.arange(0,n_src_,int(n_trg_/n_cells_))[:n_cells_]
+        trg_set_ = np.arange(adata.shape[0])[adata.obs[cluster_key].values == target_cluster][np.argsort(centrality_trg_)][idx_trg_]
+        idx_src_ = np.arange(0,n_src_,int(n_src_/n_cells_))[:n_cells_]
+        src_set_ = src_set_all_[idx_src_]
+
+        pathes,edges,weights,dists  = [],[],[],[]
+        for src_,trg_ in np.vstack((src_set_,trg_set_)).T:
+            path = nx.dijkstra_path(G, source=src_, target=trg_, weight='weight')
+            pathes.append(path)
+            edges.append(np.array([[path[i], path[i+1]] for i in range(len(path)-1)]))
+            weights.append((sum([G[path[i]][path[i+1]]['weight'] for i in range(len(path)-1)]))/sum([np.linalg.norm(data_pos[path[i]]-data_pos[path[i+1]]) for i in range(len(path)-1)]))
+            dists.append(sum([np.linalg.norm(data_pos[path[i]]-data_pos[path[i+1]]) for i in range(len(path)-1)]))
+        
+        ax.scatter(data_pos[src_set_,0],data_pos[src_set_,1],color=cmap_(0),zorder=20,marker='o',s=20)
+        ax.scatter(data_pos[trg_set_,0],data_pos[trg_set_,1],color=cmap_(i_trg_+1),zorder=20,marker='o',s=20)
+        for i in range(n_cells_):
+            src_,trg_ = src_set_[i],trg_set_[i]
+            for s,t in edges[i]:
+                ax.plot([data_pos[s,0],data_pos[t,0]],[data_pos[s,1],data_pos[t,1]],color=cmap_(i_trg_+1),zorder=10)
+    ax.axis('off')
```

## Comparing `cellmap-1.0.1.dev202304180446.dist-info/METADATA` & `cellmap-1.0.1.dev202304180922.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304180446
+Version: 1.0.1.dev202304180922
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

