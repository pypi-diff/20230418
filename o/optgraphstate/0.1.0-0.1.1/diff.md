# Comparing `tmp/optgraphstate-0.1.0-py3-none-any.whl.zip` & `tmp/optgraphstate-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 23265 bytes, number of entries: 9
--rw-r--r--  2.0 unx    66979 b- defN 23-Apr-17 06:42 optgraphstate/__init__.py
--rw-r--r--  2.0 unx    14822 b- defN 23-Apr-17 06:24 optgraphstate/graph_tools.py
+Zip file size: 23399 bytes, number of entries: 9
+-rw-r--r--  2.0 unx    67049 b- defN 23-Apr-18 10:31 optgraphstate/__init__.py
+-rw-r--r--  2.0 unx    14819 b- defN 23-Apr-18 10:28 optgraphstate/graph_tools.py
 -rw-r--r--  2.0 unx      686 b- defN 23-Apr-06 04:55 optgraphstate/utils.py
--rw-r--r--  2.0 unx     8900 b- defN 23-Apr-17 05:33 optgraphstate/visualization.py
--rw-r--r--  2.0 unx     1070 b- defN 23-Apr-17 11:19 optgraphstate-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1692 b- defN 23-Apr-17 11:19 optgraphstate-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 11:19 optgraphstate-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-17 11:19 optgraphstate-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      750 b- defN 23-Apr-17 11:19 optgraphstate-0.1.0.dist-info/RECORD
-9 files, 95005 bytes uncompressed, 21971 bytes compressed:  76.9%
+-rw-r--r--  2.0 unx     8936 b- defN 23-Apr-17 12:41 optgraphstate/visualization.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-Apr-18 10:35 optgraphstate-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1881 b- defN 23-Apr-18 10:35 optgraphstate-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 10:35 optgraphstate-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-18 10:35 optgraphstate-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      750 b- defN 23-Apr-18 10:35 optgraphstate-0.1.1.dist-info/RECORD
+9 files, 95297 bytes uncompressed, 22105 bytes compressed:  76.8%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: optgraphstate/utils.py
 Comment: 
 
 Filename: optgraphstate/visualization.py
 Comment: 
 
-Filename: optgraphstate-0.1.0.dist-info/LICENSE
+Filename: optgraphstate-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: optgraphstate-0.1.0.dist-info/METADATA
+Filename: optgraphstate-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: optgraphstate-0.1.0.dist-info/WHEEL
+Filename: optgraphstate-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: optgraphstate-0.1.0.dist-info/top_level.txt
+Filename: optgraphstate-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: optgraphstate-0.1.0.dist-info/RECORD
+Filename: optgraphstate-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## optgraphstate/__init__.py

```diff
@@ -1,8 +1,10 @@
 """
+**Version 0.1.1**
+
 **OptGraphState** is a python package that implements the graph-theoretical
 strategy to optimize the fusion-based generation of any graph state.
 The package has the following features:
 
 - Finding a resource-efficient method of generating a given graph state through
 type-II fusions from multiple basic resource states, which are three-qubit
 linear graph states.
@@ -1730,14 +1732,16 @@
 
         return fig, ax
 
     def copy(self):
         """
         Return a **shallow** copy of this object.
 
+        Use `copy.deepcopy()` to get a deep copy.
+
         Returns
         -------
         copy : GraphState
             Copied instance of itself.
         """
 
         copy = GraphState(graph=self.graph,
```

## optgraphstate/graph_tools.py

```diff
@@ -79,15 +79,15 @@
     elif shape == 'rhg':
         assert len(prms) == 3
         g = _get_rhg_lattice(*prms)
         # g['size'] = tuple(prms)
 
     elif shape == 'repeater':
         assert len(prms) == 1
-        g, _ = get_sample_graph('complete', 2 * prms[0])
+        g = get_sample_graph('complete', 2 * prms[0])
         vcount = g.vcount()
         for v in range(vcount):
             new_v = g.add_vertex()
             g.add_edge(v, new_v)
         # g['m'] = prms[0]
 
     elif shape == 'parity_encoding':
```

## optgraphstate/visualization.py

```diff
@@ -110,15 +110,15 @@
 
         visual_style.update(kwargs)
         _plot_base(graph, ax=ax, layout=layout, **visual_style)
 
     plt.tight_layout()
 
     if save is not None:
-        plt.savefig(save)
+        plt.savefig(save, transparent=True)
 
     return fig, ax
 
 
 def plot_fusion_network(network,
                         ax=None,
                         layout='auto',
@@ -270,10 +270,10 @@
             'LL': '-'}
         for eid, line in enumerate(lines):
             line.set(linestyle=edge_style[network.es[eid]['kind']])
 
     plt.tight_layout()
 
     if save is not None:
-        plt.savefig(save)
+        plt.savefig(save, transparent=True)
 
     return fig, ax
```

## Comparing `optgraphstate-0.1.0.dist-info/LICENSE` & `optgraphstate-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `optgraphstate-0.1.0.dist-info/METADATA` & `optgraphstate-0.1.1.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: optgraphstate
-Version: 0.1.0
+Version: 0.1.1
 Summary: Graph-theoretical optimization of fusion-based graph state generation
 Home-page: https://github.com/seokhyung-lee/OptGraphState
 Author: Seok-Hyung Lee
 Author-email: sh.lee1524@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OptGraphState
 
+**Version 0.1.1**
+
 *Graph-theoretical optimization of fusion-based graph state generation.*
 
 **OptGraphState** is a python package that implements the graph-theoretical strategy to optimize the fusion-based
 generation of any graph state. The package has the following features:
 
 - Finding a resource-efficient method of generating a given graph state through type-II fusions from multiple basic
   resource states, which are three-qubit linear graph states.
@@ -26,11 +28,22 @@
   states.
 - Visualizing the original graph (of the graph state you want to generate), unraveled graphs, and fusion networks. An
   unraveled graph is a simplified graph where the corresponding graph state is equivalent to the desired graph state up
   to fusions and single-qubit Clifford operations. A fusion network is a graph that instructs the fusions between basic
   resource states required to generate the desired graph state.
 - Various predefined sample graphs for input.
 
+## Installation
+
+`pip install optgraphstate`
+
+## Manuals
+
 Tutorials: https://github.com/seokhyung-lee/OptGraphState/raw/main/tutorials.pdf
 
 API reference: https://seokhyung-lee.github.io/OptGraphState
 
+## License
+
+OptGraphState is distributed under the MIT license. Please see the LICENSE file for more details.
+
+
```

## Comparing `optgraphstate-0.1.0.dist-info/RECORD` & `optgraphstate-0.1.1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-optgraphstate/__init__.py,sha256=L4B12WQLIMbBfJI64JnLjp1R2aW1WoXHy41efJ0yTNM,66979
-optgraphstate/graph_tools.py,sha256=5RYhjFXSnRvwGkpDB0onUythBtXWf5OWJGlQgwVLbcU,14822
+optgraphstate/__init__.py,sha256=HK-MWS9owZPXYepHgTfxuq7E8-dvqo0huocygbV8jsc,67049
+optgraphstate/graph_tools.py,sha256=foGOoB5jUwToLVSP5iuhn00fk-uokV_cZVdrWWR3uy8,14819
 optgraphstate/utils.py,sha256=11ak92ZwuPQl6DVVEI45mS_gjS-QKZONObwuRvRpmpE,686
-optgraphstate/visualization.py,sha256=ac3bit3ALq9j6R5qzfpUyObfuU2HlEfwkAsLxnLYtQI,8900
-optgraphstate-0.1.0.dist-info/LICENSE,sha256=rB8sqYvzli01OnnAHmeXktkq7ye_YYJjOWP25yuN8VY,1070
-optgraphstate-0.1.0.dist-info/METADATA,sha256=R3rSvZONm4GuE9mzT0_zvguHlfWJRyqN0BxV-PucZOo,1692
-optgraphstate-0.1.0.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-optgraphstate-0.1.0.dist-info/top_level.txt,sha256=Rj9Sk6j_-PrVy4Gk6bDHLQEpm37egogxHKxd9xLk0A0,14
-optgraphstate-0.1.0.dist-info/RECORD,,
+optgraphstate/visualization.py,sha256=GILVTwwmpr6VFO5CW3mu7vkPPbcBK-pPohHCzaEsywY,8936
+optgraphstate-0.1.1.dist-info/LICENSE,sha256=rB8sqYvzli01OnnAHmeXktkq7ye_YYJjOWP25yuN8VY,1070
+optgraphstate-0.1.1.dist-info/METADATA,sha256=CSsTR64ATx3T20PGdLyxz2kq4kt8uVyAscFCZtNhyV4,1881
+optgraphstate-0.1.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+optgraphstate-0.1.1.dist-info/top_level.txt,sha256=Rj9Sk6j_-PrVy4Gk6bDHLQEpm37egogxHKxd9xLk0A0,14
+optgraphstate-0.1.1.dist-info/RECORD,,
```

