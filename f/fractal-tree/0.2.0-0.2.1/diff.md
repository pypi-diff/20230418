# Comparing `tmp/fractal-tree-0.2.0.tar.gz` & `tmp/fractal-tree-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal-tree-0.2.0.tar", last modified: Sat Mar 25 16:44:26 2023, max compression
+gzip compressed data, was "fractal-tree-0.2.1.tar", last modified: Tue Apr 18 06:38:39 2023, max compression
```

## Comparing `fractal-tree-0.2.0.tar` & `fractal-tree-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:44:26.390590 fractal-tree-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-03-25 16:44:02.000000 fractal-tree-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-25 16:44:02.000000 fractal-tree-0.2.0/LICENSE_fsahli
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-03-25 16:44:26.390590 fractal-tree-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-03-25 16:44:02.000000 fractal-tree-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-03-25 16:44:02.000000 fractal-tree-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 16:44:26.390590 fractal-tree-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:44:26.390590 fractal-tree-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:44:26.390590 fractal-tree-0.2.0/src/fractal_tree/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-25 16:44:02.000000 fractal-tree-0.2.0/src/fractal_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-03-25 16:44:02.000000 fractal-tree-0.2.0/src/fractal_tree/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-03-25 16:44:02.000000 fractal-tree-0.2.0/src/fractal_tree/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-03-25 16:44:02.000000 fractal-tree-0.2.0/src/fractal_tree/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-03-25 16:44:02.000000 fractal-tree-0.2.0/src/fractal_tree/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:44:26.390590 fractal-tree-0.2.0/src/fractal_tree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-03-25 16:44:26.000000 fractal-tree-0.2.0/src/fractal_tree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-25 16:44:26.000000 fractal-tree-0.2.0/src/fractal_tree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 16:44:26.000000 fractal-tree-0.2.0/src/fractal_tree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-25 16:44:26.000000 fractal-tree-0.2.0/src/fractal_tree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-25 16:44:26.000000 fractal-tree-0.2.0/src/fractal_tree.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:44:26.390590 fractal-tree-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-25 16:44:02.000000 fractal-tree-0.2.0/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:38:39.913709 fractal-tree-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-18 06:38:15.000000 fractal-tree-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-18 06:38:15.000000 fractal-tree-0.2.1/LICENSE_fsahli
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-18 06:38:39.913709 fractal-tree-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-18 06:38:15.000000 fractal-tree-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-18 06:38:15.000000 fractal-tree-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 06:38:39.913709 fractal-tree-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:38:39.909710 fractal-tree-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:38:39.913709 fractal-tree-0.2.1/src/fractal_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-18 06:38:15.000000 fractal-tree-0.2.1/src/fractal_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-04-18 06:38:15.000000 fractal-tree-0.2.1/src/fractal_tree/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-04-18 06:38:15.000000 fractal-tree-0.2.1/src/fractal_tree/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11200 2023-04-18 06:38:15.000000 fractal-tree-0.2.1/src/fractal_tree/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-18 06:38:15.000000 fractal-tree-0.2.1/src/fractal_tree/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:38:39.913709 fractal-tree-0.2.1/src/fractal_tree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-18 06:38:39.000000 fractal-tree-0.2.1/src/fractal_tree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-18 06:38:39.000000 fractal-tree-0.2.1/src/fractal_tree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 06:38:39.000000 fractal-tree-0.2.1/src/fractal_tree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-18 06:38:39.000000 fractal-tree-0.2.1/src/fractal_tree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 06:38:39.000000 fractal-tree-0.2.1/src/fractal_tree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:38:39.913709 fractal-tree-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-18 06:38:15.000000 fractal-tree-0.2.1/tests/test_integration.py
```

### Comparing `fractal-tree-0.2.0/LICENSE` & `fractal-tree-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal-tree-0.2.0/LICENSE_fsahli` & `fractal-tree-0.2.1/LICENSE_fsahli`

 * *Files identical despite different names*

### Comparing `fractal-tree-0.2.0/PKG-INFO` & `fractal-tree-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-tree
-Version: 0.2.0
+Version: 0.2.1
 Summary: Create a fractal tree over a surface discretized by triangles
 Author: Francisco Sahli Costabal
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: Copyright 2023 Henrik Finsberg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -52,18 +52,18 @@
 
 msh = meshio.read("sphere.obj")
 mesh = Mesh(verts=msh.points, connectivity=msh.cells[0].data)
 param = FractalTreeParameters(
     filename="sphere-line",
     N_it=10,
 )
-branches, nodes = generate_fractal_tree(mesh, param)
+results = generate_fractal_tree(mesh, param)
 ```
 
-For a more elaborate example you can checkout the [gmsh example](https://github.com/finsberg/fractal-tree/examples/demo_gmsh.html).
+For a more elaborate example you can checkout the [gmsh example](https://finsberg.github.io/fractal-tree/examples/demo_gmsh.html).
 
 
 ## License
 MIT
 
 ## Need help or having issues
 Please submit an [issue](https://github.com/finsberg/fractal-tree/issues)
```

### Comparing `fractal-tree-0.2.0/README.md` & `fractal-tree-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 
 msh = meshio.read("sphere.obj")
 mesh = Mesh(verts=msh.points, connectivity=msh.cells[0].data)
 param = FractalTreeParameters(
     filename="sphere-line",
     N_it=10,
 )
-branches, nodes = generate_fractal_tree(mesh, param)
+results = generate_fractal_tree(mesh, param)
 ```
 
-For a more elaborate example you can checkout the [gmsh example](https://github.com/finsberg/fractal-tree/examples/demo_gmsh.html).
+For a more elaborate example you can checkout the [gmsh example](https://finsberg.github.io/fractal-tree/examples/demo_gmsh.html).
 
 
 ## License
 MIT
 
 ## Need help or having issues
 Please submit an [issue](https://github.com/finsberg/fractal-tree/issues)
```

### Comparing `fractal-tree-0.2.0/pyproject.toml` & `fractal-tree-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system] # Require setuptool version due to https://github.com/pypa/setuptools/issues/2938
 requires = ["setuptools>=61.0.0", "wheel"]
 
 [project]
 name = "fractal-tree"
-version = "0.2.0"
+version = "0.2.1"
 description = "Create a fractal tree over a surface discretized by triangles"
 authors = [{name = "Francisco Sahli Costabal" },{name = "Henrik Finsberg", email = "henriknf@simula.no"}]
 license = {file = "LICENSE"}
 readme = "README.md"
 dependencies = [
     "numpy",
     "scipy",
@@ -18,14 +18,15 @@
 test = [
     "pytest",
     "pytest-cov",
     "meshio",
 ]
 demo = [
     "meshio",
+    "fenics-pulse",
     "cardiac-geometries[gmsh]",
 ]
 dev = [
     "pdbpp",
     "ipython",
     "bump2version",
     "pre-commit",
```

### Comparing `fractal-tree-0.2.0/src/fractal_tree/__init__.py` & `fractal-tree-0.2.1/src/fractal_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal-tree-0.2.0/src/fractal_tree/branch.py` & `fractal-tree-0.2.1/src/fractal_tree/branch.py`

 * *Files identical despite different names*

### Comparing `fractal-tree-0.2.0/src/fractal_tree/mesh.py` & `fractal-tree-0.2.1/src/fractal_tree/mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,14 +115,15 @@
 
         """
         # Get the closest point
         node = self.tree.query(point)[1]
 
         # Get triangles connected to that node
         triangles = self.node_to_tri[node]
+
         if len(triangles) == 0:
             raise InvalidNodeError(
                 f"node {node} with point {point} not connected to triangles, check your mesh"
             )
 
         # Compute the vertex normal as the avergage of the triangle normals.
         vertex_normal = np.sum(self.normals[triangles], axis=0)
```

### Comparing `fractal-tree-0.2.0/src/fractal_tree/tree.py` & `fractal-tree-0.2.1/src/fractal_tree/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,32 +113,31 @@
 
     branches_to_grow = new_branches_to_grow
     return branches, nodes, lines, branches_to_grow, lines, last_branch
 
 
 def save_tree(
     filename: Union[Path, str],
-    nodes: Nodes,
+    nodes: np.ndarray,
+    end_nodes: list[int],
     lines: list[tuple[int, int]],
     save_paraview: bool = True,
 ):
     if save_paraview:
         logger.info("Finished growing, writing paraview file")
-        xyz = np.zeros((len(nodes.nodes), 3))
-        for i in range(len(nodes.nodes)):
-            xyz[i, :] = nodes.nodes[i]
-        write_line_VTU(xyz, lines, Path(filename).with_suffix(".vtu"))
+
+        write_line_VTU(nodes, lines, Path(filename).with_suffix(".vtu"))
     name = Path(filename).name
     np.savetxt(
         Path(filename).with_name(name + "_lines").with_suffix(".txt"), lines, fmt="%d"
     )
-    np.savetxt(Path(filename).with_name(name + "_xyz").with_suffix(".txt"), xyz)
+    np.savetxt(Path(filename).with_name(name + "_xyz").with_suffix(".txt"), nodes)
     np.savetxt(
         Path(filename).with_name(name + "_endnodes").with_suffix(".txt"),
-        nodes.end_nodes,
+        end_nodes,
         fmt="%d",
     )
 
 
 @dataclass
 class FractalTreeParameters:
     """Class to specify the parameters of the fractal tree.
@@ -218,15 +217,17 @@
 
     def as_dict(self):
         return {k: v for k, v in self.__dict__.items()}
 
 
 class FractalTreeResult(NamedTuple):
     branches: dict[int, Branch]
-    nodes: Nodes
+    nodes: np.ndarray
+    end_nodes: list[int]
+    lines: list[tuple[int, int]]
 
 
 def node_direction(src: np.ndarray, target: Optional[np.ndarray] = None) -> np.ndarray:
     """Return the direction from src to target.
 
     Parameters
     ----------
@@ -315,16 +316,20 @@
         )
 
     for _ in tqdm.tqdm(range(parameters.N_it)):
         branches, nodes, lines, branches_to_grow, lines, last_branch = run_generation(
             branches_to_grow, parameters, branches, last_branch, mesh, nodes, lines
         )
 
+    xyz = np.array(nodes.nodes)
+
     if parameters.save:
         save_tree(
             filename=parameters.filename,
-            nodes=nodes,
+            nodes=xyz,
+            end_nodes=nodes.end_nodes,
             lines=lines,
             save_paraview=parameters.save_paraview,
         )
-
-    return FractalTreeResult(branches, nodes)
+    return FractalTreeResult(
+        branches=branches, nodes=xyz, end_nodes=nodes.end_nodes, lines=lines
+    )
```

### Comparing `fractal-tree-0.2.0/src/fractal_tree/viz.py` & `fractal-tree-0.2.1/src/fractal_tree/viz.py`

 * *Files identical despite different names*

### Comparing `fractal-tree-0.2.0/src/fractal_tree.egg-info/PKG-INFO` & `fractal-tree-0.2.1/src/fractal_tree.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-tree
-Version: 0.2.0
+Version: 0.2.1
 Summary: Create a fractal tree over a surface discretized by triangles
 Author: Francisco Sahli Costabal
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: Copyright 2023 Henrik Finsberg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -52,18 +52,18 @@
 
 msh = meshio.read("sphere.obj")
 mesh = Mesh(verts=msh.points, connectivity=msh.cells[0].data)
 param = FractalTreeParameters(
     filename="sphere-line",
     N_it=10,
 )
-branches, nodes = generate_fractal_tree(mesh, param)
+results = generate_fractal_tree(mesh, param)
 ```
 
-For a more elaborate example you can checkout the [gmsh example](https://github.com/finsberg/fractal-tree/examples/demo_gmsh.html).
+For a more elaborate example you can checkout the [gmsh example](https://finsberg.github.io/fractal-tree/examples/demo_gmsh.html).
 
 
 ## License
 MIT
 
 ## Need help or having issues
 Please submit an [issue](https://github.com/finsberg/fractal-tree/issues)
```

### Comparing `fractal-tree-0.2.0/tests/test_integration.py` & `fractal-tree-0.2.1/tests/test_integration.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,27 +26,27 @@
 
     # Read Mesh
     fname = here / ".." / "examples" / "sphere.obj"
     msh = meshio.read(fname)
     mesh = Mesh(verts=msh.points, connectivity=msh.cells[0].data)
 
     np.random.seed(1234)
-    branches, nodes = generate_fractal_tree(mesh, param)
+    results = generate_fractal_tree(mesh, param)
 
-    assert len(branches) == 893
-    assert len(nodes.nodes) == 5822
-    assert np.allclose(nodes.nodes[0], [-1, 0, 0])
-    assert np.allclose(nodes.nodes[2], [-0.9990874, 0.0, 0.01975606])
-    assert branches[0].nodes == [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
-    assert branches[0].triangles == [
+    assert len(results.branches) == 893
+    assert len(results.nodes) == 5822
+    assert np.allclose(results.nodes[0], [-1, 0, 0])
+    assert np.allclose(results.nodes[2], [-0.9990874, 0.0, 0.01975606])
+    assert results.branches[0].nodes == [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
+    assert results.branches[0].triangles == [
         3122,
         3122,
         3122,
         3122,
         3122,
         3122,
         3122,
         614,
         614,
         614,
     ]
-    assert branches[0].tri == 614
+    assert results.branches[0].tri == 614
```

