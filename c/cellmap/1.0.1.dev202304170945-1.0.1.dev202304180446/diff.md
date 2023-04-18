# Comparing `tmp/cellmap-1.0.1.dev202304170945-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304180446-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1388592 bytes, number of entries: 6
+Zip file size: 1388586 bytes, number of entries: 6
 -rw-r--r--  2.0 unx  4446947 b- defN 80-Jan-01 00:00 cellmap/CellMap_view_3D.html
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    54856 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304170945.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304170945.dist-info/WHEEL
-?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304170945.dist-info/RECORD
-6 files, 4504220 bytes uncompressed, 1387706 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx    55277 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304180446.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304180446.dist-info/WHEEL
+?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304180446.dist-info/RECORD
+6 files, 4504641 bytes uncompressed, 1387700 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304170945.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304180446.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304170945.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304180446.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304170945.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304180446.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -1,7 +1,8 @@
+from adjustText import adjust_text
 import anndata
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
 from matplotlib import patheffects as PathEffects
 import matplotlib.cm
 import scipy
@@ -332,19 +333,16 @@
             idx_s = source == i
             idx_t = target == i
             ex_s = -(exp_LD[source[idx_s]]-exp_LD[target[idx_s]])/np.linalg.norm(exp_LD[source[idx_s]]-exp_LD[target[idx_s]],ord=2)
             ex_t = -(exp_LD[target[idx_t]]-exp_LD[source[idx_t]])/np.linalg.norm(exp_LD[target[idx_t]]-exp_LD[source[idx_t]],ord=2)
             edge_vel = edge_velocity(exp_LD,vel_LD,source,target,normalization=False)
             vel_potential[i] = 2*np.linalg.norm(edge_vel)*(np.sum((adata.obs[potential_key][source[idx_s]].values-adata.obs[potential_key][target[idx_s]].values)*ex_s.T,axis=1) + \
                                 np.sum((adata.obs[potential_key][target[idx_t]].values-adata.obs[potential_key][source[idx_t]].values)*ex_t.T,axis=1))
-            # vel_rotation[i] = 2*(np.sum((adata.obs[rotation_key][source[idx_s]].values-adata.obs[rotation_key][target[idx_s]].values)*ex_s.T,axis=1) + \
-            #                     np.sum((adata.obs[rotation_key][target[idx_t]].values-adata.obs[rotation_key][source[idx_t]].values)*ex_t.T,axis=1))
         adata.obsm[pot_vkey_] = vel_potential
         adata.obsm[rot_vkey_] = adata.obsm[vel_2d_key_]-vel_potential
-        # adata.obsm[rot_vkey_] = vel_rotation
     elif graph_method == 'knn':
         knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
         knn.fit(exp_LD)
         distances, indices = knn.kneighbors(exp_LD)
         distances, indices = distances[:,1:], indices[:,1:]
         for i in range(adata.shape[0]):
             ex_s = (exp_LD[indices[i]]-exp_LD[i])/np.linalg.norm(exp_LD[indices[i]]-exp_LD[i],ord=2)
@@ -619,22 +617,39 @@
     fontsize = 18,
     legend_fontsize = 18,
     **kwargs
     ):
     
     kwargs_arg = check_arguments(adata, basis = basis)
     basis = kwargs_arg['basis']
+    basis_key = 'X_%s' % basis
+    data_pos = adata.obsm[basis_key]
+    cluster = adata.obs[cluster_key]
     
     fig,ax = plt.subplots(1,3,figsize=figsize,tight_layout=True)
     scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=vkey, title='RNA velocity',ax=ax[0],color=cluster_key,
-                                     show=False,density=density,alpha=alpha,fontsize=fontsize,legend_fontsize=legend_fontsize, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
+                                     show=False,density=density,alpha=alpha,fontsize=fontsize,legend_fontsize=0, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
+    # texts = []
+    # for c in np.unique(cluster):
+    #     txt = ax[0].text(np.mean(data_pos[cluster == c],axis=0)[0],np.mean(data_pos[cluster == c],axis=0)[1],c,fontsize=legend_fontsize,ha='center', va='center',fontweight='bold',zorder=20)
+    #     txt.set_path_effects([PathEffects.withStroke(linewidth=5, foreground='w')])
+    #     texts.append(txt)
+    # adjust_text(texts)
     scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=potential_vkey, title='Potential flow',ax=ax[1],color=cluster_key,
-                                     show=False,density=density,alpha=alpha,fontsize=fontsize,legend_fontsize=legend_fontsize, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
+                                     show=False,density=density,alpha=alpha,fontsize=fontsize,legend_fontsize=0, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
     scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=rotation_vkey, title='Rotational flow',ax=ax[2],color=cluster_key,
-                                     show=False,density=density,alpha=alpha,fontsize=fontsize,legend_fontsize=legend_fontsize, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
+                                     show=False,density=density,alpha=alpha,fontsize=fontsize,legend_fontsize=0, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
+    for i in range(3):
+        texts = []
+        for c in np.unique(cluster):
+            txt = ax[i].text(np.mean(data_pos[cluster == c],axis=0)[0],np.mean(data_pos[cluster == c],axis=0)[1],c,fontsize=legend_fontsize,ha='center', va='center',fontweight='bold',zorder=20)
+            txt.set_path_effects([PathEffects.withStroke(linewidth=5, foreground='w')])
+            texts.append(txt)
+        # adjust_text(texts)
+
 
 def view_stream_line(
     adata,
     basis = 'umap',
     contour_key = 'stream_line',
     cluster_key = 'clusters',
     potential_key = 'potential',
@@ -803,16 +818,16 @@
                         texts.append(txt)
 
 def view_3D(
     adata,
     basis = 'umap',
     potential_key = 'potential',
     cluster_key ='clusters',
-    cutedge_vol  = 1,
-    cutedge_length = 1,
+    cutedge_vol  = None,
+    cutedge_length = None,
     show_cells = False,
     show_shadow = True,
     shadow_alpha = 0.2,
     title = 'Landscape',
     bgcolor = "white",
     gridcolor = "gray",
     edges_color='lightgray',
@@ -895,28 +910,28 @@
         
         annotations = [dict(
             showarrow=False,
             x=np.percentile(x[clstr == np.unique(clstr)[i]],50),
             y=np.percentile(y[clstr == np.unique(clstr)[i]],50),
             z=np.percentile(z[clstr == np.unique(clstr)[i]],50),
             text="<b>%s<b>" % str(np.unique(clstr)[i]),
-            font=dict(size=14,color='rgba(0,0,0,1)'),bgcolor="rgba(255,255,255,0.7)") for i in range(len(np.unique(clstr)))]#,color="rgba%s" % str(tuple(np.array(cmap_clstr(i+1))*255))
+            font=dict(size=14,color='rgba(0,0,0,1)'),bgcolor="rgba(255,255,255,0.7)") for i in range(len(np.unique(clstr)))]
         layout = go.Layout(
             title = title,
             width=1500,
             height=1000,
             margin=dict(l=0,r=0, b=0,t=50),
             scene_camera=camera,
             scene=dict(annotations=annotations,xaxis_title=basis+"_1",yaxis_title=basis+"_2",zaxis_title=potential_key,
                      xaxis = dict(backgroundcolor=bgcolor,gridcolor=gridcolor),
                      yaxis = dict(backgroundcolor=bgcolor,gridcolor=gridcolor),
                      zaxis = dict(backgroundcolor=bgcolor,gridcolor=gridcolor),
             ),
             meta=dict(),
-            scene_aspectratio=dict(x=1.2, y=1.2, z=1.2),
+            scene_aspectratio=dict(x=1.0, y=1.0, z=0.5),
         )
         data = [surf]
         if show_cells: data.append(cells)
         if show_shadow: data.append(shadow)
         fig = go.Figure(data=data, layout=layout)
         #                  )
     else:
@@ -950,15 +965,15 @@
             scene_camera=camera,
             scene=dict(xaxis_title=basis+"_1",yaxis_title=basis+"_2",zaxis_title=potential_key,
                      xaxis = dict(backgroundcolor=bgcolor,gridcolor=gridcolor),
                      yaxis = dict(backgroundcolor=bgcolor,gridcolor=gridcolor),
                      zaxis = dict(backgroundcolor=bgcolor,gridcolor=gridcolor),
             ),
             meta=dict(),
-            scene_aspectratio=dict(x=1.2, y=1.2, z=1.2),
+            scene_aspectratio=dict(x=1.0, y=1.0, z=0.5),
         )
         data = [surf]
         if show_cells: data.append(cells)
         if show_shadow: data.append(shadow)
         fig = go.Figure(data=data, layout=layout)
     fig.show()
     
@@ -1002,16 +1017,14 @@
         texts = []
         if cluster_key in adata.obs.keys():
             cluster = adata.obs[cluster_key]
             for c in np.unique(cluster):
                 txt = ax.text(np.mean(data_pos[cluster == c],axis=0)[0],np.mean(data_pos[cluster == c],axis=0)[1],np.mean(adata.obs[potential_key][cluster == c]),c,fontsize=15,ha='center', va='center',fontweight='bold',zorder=1000)
                 txt.set_path_effects([PathEffects.withStroke(linewidth=5, foreground='w')])
                 texts.append(txt)
-        # from adjustText import adjust_text
-        # adjust_text(texts)
     ax.view_init(elev=elev, azim=azim)
 
 
 def view_surface_3D_cluster(
     adata,
     basis = 'umap',
     potential_key = 'potential',
```

## Comparing `cellmap-1.0.1.dev202304170945.dist-info/METADATA` & `cellmap-1.0.1.dev202304180446.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304170945
+Version: 1.0.1.dev202304180446
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

