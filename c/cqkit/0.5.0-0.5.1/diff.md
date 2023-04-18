# Comparing `tmp/cqkit-0.5.0.tar.gz` & `tmp/cqkit-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cqkit-0.5.0.tar", last modified: Thu Jan 12 03:51:26 2023, max compression
+gzip compressed data, was "cqkit-0.5.1.tar", last modified: Tue Apr 18 12:10:18 2023, max compression
```

## Comparing `cqkit-0.5.0.tar` & `cqkit-0.5.1.tar`

### file list

```diff
@@ -1,23 +1,32 @@
-drwxr-xr-x   0 michaelgale   (501) staff       (20)        0 2023-01-12 03:51:26.399667 cqkit-0.5.0/
--rw-r--r--   0 michaelgale   (501) staff       (20)     1079 2022-01-27 00:34:16.000000 cqkit-0.5.0/LICENSE
--rw-r--r--   0 michaelgale   (501) staff       (20)        0 2021-12-14 13:03:14.000000 cqkit-0.5.0/MANIFEST.in
--rw-r--r--   0 michaelgale   (501) staff       (20)    23003 2023-01-12 03:51:26.399229 cqkit-0.5.0/PKG-INFO
--rw-r--r--   0 michaelgale   (501) staff       (20)    22143 2023-01-12 03:50:16.000000 cqkit-0.5.0/README.md
-drwxr-xr-x   0 michaelgale   (501) staff       (20)        0 2023-01-12 03:51:26.396696 cqkit-0.5.0/cqkit/
--rw-r--r--   0 michaelgale   (501) staff       (20)      957 2023-01-12 03:33:25.000000 cqkit-0.5.0/cqkit/__init__.py
--rw-r--r--   0 michaelgale   (501) staff       (20)     6352 2023-01-12 03:36:26.000000 cqkit-0.5.0/cqkit/cq_discrete.py
--rw-r--r--   0 michaelgale   (501) staff       (20)     6598 2022-01-27 00:40:28.000000 cqkit-0.5.0/cqkit/cq_fasteners.py
--rw-r--r--   0 michaelgale   (501) staff       (20)    20952 2022-01-27 00:57:31.000000 cqkit-0.5.0/cqkit/cq_files.py
--rw-r--r--   0 michaelgale   (501) staff       (20)    32853 2022-01-17 19:07:56.000000 cqkit-0.5.0/cqkit/cq_geometry.py
--rw-r--r--   0 michaelgale   (501) staff       (20)    10466 2022-01-27 00:34:18.000000 cqkit-0.5.0/cqkit/cq_pprint.py
--rw-r--r--   0 michaelgale   (501) staff       (20)     9954 2022-01-27 00:34:18.000000 cqkit-0.5.0/cqkit/cq_ribbon.py
--rw-r--r--   0 michaelgale   (501) staff       (20)    26608 2022-01-27 00:34:18.000000 cqkit-0.5.0/cqkit/cq_selectors.py
--rw-r--r--   0 michaelgale   (501) staff       (20)    10405 2022-01-27 00:34:18.000000 cqkit-0.5.0/cqkit/cq_xsection.py
--rw-r--r--   0 michaelgale   (501) staff       (20)     7300 2021-06-27 15:57:14.000000 cqkit-0.5.0/cqkit/refdim.py
-drwxr-xr-x   0 michaelgale   (501) staff       (20)        0 2023-01-12 03:51:26.398610 cqkit-0.5.0/cqkit.egg-info/
--rw-r--r--   0 michaelgale   (501) staff       (20)    23003 2023-01-12 03:51:26.000000 cqkit-0.5.0/cqkit.egg-info/PKG-INFO
--rw-r--r--   0 michaelgale   (501) staff       (20)      351 2023-01-12 03:51:26.000000 cqkit-0.5.0/cqkit.egg-info/SOURCES.txt
--rw-r--r--   0 michaelgale   (501) staff       (20)        1 2023-01-12 03:51:26.000000 cqkit-0.5.0/cqkit.egg-info/dependency_links.txt
--rw-r--r--   0 michaelgale   (501) staff       (20)        6 2023-01-12 03:51:26.000000 cqkit-0.5.0/cqkit.egg-info/top_level.txt
--rw-r--r--   0 michaelgale   (501) staff       (20)       38 2023-01-12 03:51:26.399787 cqkit-0.5.0/setup.cfg
--rw-r--r--   0 michaelgale   (501) staff       (20)     2581 2023-01-12 03:38:03.000000 cqkit-0.5.0/setup.py
+drwxr-xr-x   0 michaelgale   (501) staff       (20)        0 2023-04-18 12:10:18.534388 cqkit-0.5.1/
+-rw-r--r--   0 michaelgale   (501) staff       (20)     1079 2022-01-27 00:34:16.000000 cqkit-0.5.1/LICENSE
+-rw-r--r--   0 michaelgale   (501) staff       (20)        0 2021-12-14 13:03:14.000000 cqkit-0.5.1/MANIFEST.in
+-rw-r--r--   0 michaelgale   (501) staff       (20)    23006 2023-04-18 12:10:18.533686 cqkit-0.5.1/PKG-INFO
+-rw-r--r--   0 michaelgale   (501) staff       (20)    22148 2023-01-17 14:55:19.000000 cqkit-0.5.1/README.md
+drwxr-xr-x   0 michaelgale   (501) staff       (20)        0 2023-04-18 12:10:18.526770 cqkit-0.5.1/cqkit/
+-rw-r--r--   0 michaelgale   (501) staff       (20)      957 2023-04-18 12:05:05.000000 cqkit-0.5.1/cqkit/__init__.py
+-rw-r--r--   0 michaelgale   (501) staff       (20)     6387 2023-01-17 18:28:37.000000 cqkit-0.5.1/cqkit/cq_discrete.py
+-rw-r--r--   0 michaelgale   (501) staff       (20)     6598 2022-01-27 00:40:28.000000 cqkit-0.5.1/cqkit/cq_fasteners.py
+-rw-r--r--   0 michaelgale   (501) staff       (20)    21031 2023-01-17 18:27:53.000000 cqkit-0.5.1/cqkit/cq_files.py
+-rw-r--r--   0 michaelgale   (501) staff       (20)    32853 2022-01-17 19:07:56.000000 cqkit-0.5.1/cqkit/cq_geometry.py
+-rw-r--r--   0 michaelgale   (501) staff       (20)    10466 2022-01-27 00:34:18.000000 cqkit-0.5.1/cqkit/cq_pprint.py
+-rw-r--r--   0 michaelgale   (501) staff       (20)     9954 2022-01-27 00:34:18.000000 cqkit-0.5.1/cqkit/cq_ribbon.py
+-rw-r--r--   0 michaelgale   (501) staff       (20)    26608 2022-01-27 00:34:18.000000 cqkit-0.5.1/cqkit/cq_selectors.py
+-rw-r--r--   0 michaelgale   (501) staff       (20)    10405 2022-01-27 00:34:18.000000 cqkit-0.5.1/cqkit/cq_xsection.py
+-rw-r--r--   0 michaelgale   (501) staff       (20)     7300 2021-06-27 15:57:14.000000 cqkit-0.5.1/cqkit/refdim.py
+drwxr-xr-x   0 michaelgale   (501) staff       (20)        0 2023-04-18 12:10:18.528493 cqkit-0.5.1/cqkit.egg-info/
+-rw-r--r--   0 michaelgale   (501) staff       (20)    23006 2023-04-18 12:10:18.000000 cqkit-0.5.1/cqkit.egg-info/PKG-INFO
+-rw-r--r--   0 michaelgale   (501) staff       (20)      530 2023-04-18 12:10:18.000000 cqkit-0.5.1/cqkit.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelgale   (501) staff       (20)        1 2023-04-18 12:10:18.000000 cqkit-0.5.1/cqkit.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelgale   (501) staff       (20)        6 2023-04-18 12:10:18.000000 cqkit-0.5.1/cqkit.egg-info/top_level.txt
+-rw-r--r--   0 michaelgale   (501) staff       (20)       38 2023-04-18 12:10:18.534555 cqkit-0.5.1/setup.cfg
+-rw-r--r--   0 michaelgale   (501) staff       (20)     2622 2023-04-18 12:05:31.000000 cqkit-0.5.1/setup.py
+drwxr-xr-x   0 michaelgale   (501) staff       (20)        0 2023-04-18 12:10:18.532960 cqkit-0.5.1/tests/
+-rw-r--r--   0 michaelgale   (501) staff       (20)     1276 2022-01-27 00:57:31.000000 cqkit-0.5.1/tests/test_discrete.py
+-rw-r--r--   0 michaelgale   (501) staff       (20)     2059 2022-01-27 00:57:31.000000 cqkit-0.5.1/tests/test_fasteners.py
+-rw-r--r--   0 michaelgale   (501) staff       (20)     3919 2022-01-27 00:57:31.000000 cqkit-0.5.1/tests/test_files.py
+-rw-r--r--   0 michaelgale   (501) staff       (20)     4591 2022-01-27 00:34:18.000000 cqkit-0.5.1/tests/test_geometry.py
+-rw-r--r--   0 michaelgale   (501) staff       (20)     1076 2022-01-27 00:34:18.000000 cqkit-0.5.1/tests/test_pprint.py
+-rw-r--r--   0 michaelgale   (501) staff       (20)     1044 2022-01-27 00:57:31.000000 cqkit-0.5.1/tests/test_ribbon.py
+-rw-r--r--   0 michaelgale   (501) staff       (20)     6398 2022-01-27 00:57:31.000000 cqkit-0.5.1/tests/test_selectors.py
+-rw-r--r--   0 michaelgale   (501) staff       (20)     3248 2022-01-27 00:57:31.000000 cqkit-0.5.1/tests/test_xsection.py
```

### Comparing `cqkit-0.5.0/LICENSE` & `cqkit-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cqkit-0.5.0/PKG-INFO` & `cqkit-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cqkit
-Version: 0.5.0
+Version: 0.5.1
 Summary: A python library of CadQuery tools and helpers for building 3D CAD models.
 Home-page: https://github.com/michaelgale/cq-kit
 Author: Michael Gale
 Author-email: michael@fxbricks.com
 License: MIT
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -430,21 +430,22 @@
   - Others TBD
 - Documentation (possibly with sphinx, but in this README as a minimum)
 - Deployment notes
 
 
 ## Releases
 
-v.0.4.0 - First release on PyPI
-v.0.5.0 - Update requires python v.3.8+ and OCP v.7.6+ CadQuery 2.1+
+- v.0.4.0 - First release on PyPI
+- v.0.5.0 - Update requires python v.3.8+ and OCP v.7.6+ CadQuery 2.1+
+
 
 ## Authors
 
 **CQ-Kit** was written by [Michael Gale](https://github.com/michaelgale)
 
 ## Changelog
 
 - v.0.2.0 - Added cq_discrete with discretize_edge() and triangle_mesh_solid()
 - v.0.3.1 - Added import_iges_file()
 - v.0.4.0 - PyPI packaging
 - v.0.5.0 - Update to support newer versions of CadQuery and OCP, minimum python 3.8+
-- 
+-
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: cqkit Version: 0.5.0 Summary: A python library of
+Metadata-Version: 2.1 Name: cqkit Version: 0.5.1 Summary: A python library of
 CadQuery tools and helpers for building 3D CAD models. Home-page: https://
 github.com/michaelgale/cq-kit Author: Michael Gale Author-email:
-michael@fxbricks.com License: MIT Classifier: Development Status :: 3 - Alpha
+michael@fxbricks.com License: MIT Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.8 Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.8 Description-Content-Type: text/markdown License-
 File: LICENSE ![CQ-Kit Logo](./images/logo.png) # CQ-Kit ![https://pypi.org/
 project/cqkit/](https://img.shields.io/pypi/v/cqkit.svg) ![python version]
 (https://img.shields.io/static/
@@ -277,14 +277,14 @@
 vertex es = SharedVerticesWithObjectSelector(Vector(1, 2, 1)) ``` | [./images/
 commonvertface.png] | | --- | ```python # selects all edges which have any of
 its end points common with any vertex # belonging to a specified face face1 =
 solid.faces(FlatFaceSelector(1.0)).val() es = SharedVerticesWithObjectSelector
 (face1) ``` ## To Do - More modules/functionality for the package extracted
 from previous work in different places - Solids: solid construction classes -
 Others TBD - Documentation (possibly with sphinx, but in this README as a
-minimum) - Deployment notes ## Releases v.0.4.0 - First release on PyPI v.0.5.0
-- Update requires python v.3.8+ and OCP v.7.6+ CadQuery 2.1+ ## Authors **CQ-
-Kit** was written by [Michael Gale](https://github.com/michaelgale) ##
+minimum) - Deployment notes ## Releases - v.0.4.0 - First release on PyPI -
+v.0.5.0 - Update requires python v.3.8+ and OCP v.7.6+ CadQuery 2.1+ ## Authors
+**CQ-Kit** was written by [Michael Gale](https://github.com/michaelgale) ##
 Changelog - v.0.2.0 - Added cq_discrete with discretize_edge() and
 triangle_mesh_solid() - v.0.3.1 - Added import_iges_file() - v.0.4.0 - PyPI
 packaging - v.0.5.0 - Update to support newer versions of CadQuery and OCP,
 minimum python 3.8+ -
```

### Comparing `cqkit-0.5.0/README.md` & `cqkit-0.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -412,13 +412,14 @@
   - Others TBD
 - Documentation (possibly with sphinx, but in this README as a minimum)
 - Deployment notes
 
 
 ## Releases
 
-v.0.4.0 - First release on PyPI
-v.0.5.0 - Update requires python v.3.8+ and OCP v.7.6+ CadQuery 2.1+
+- v.0.4.0 - First release on PyPI
+- v.0.5.0 - Update requires python v.3.8+ and OCP v.7.6+ CadQuery 2.1+
+
 
 ## Authors
 
 **CQ-Kit** was written by [Michael Gale](https://github.com/michaelgale)
```

#### html2text {}

```diff
@@ -269,10 +269,10 @@
 vertex es = SharedVerticesWithObjectSelector(Vector(1, 2, 1)) ``` | [./images/
 commonvertface.png] | | --- | ```python # selects all edges which have any of
 its end points common with any vertex # belonging to a specified face face1 =
 solid.faces(FlatFaceSelector(1.0)).val() es = SharedVerticesWithObjectSelector
 (face1) ``` ## To Do - More modules/functionality for the package extracted
 from previous work in different places - Solids: solid construction classes -
 Others TBD - Documentation (possibly with sphinx, but in this README as a
-minimum) - Deployment notes ## Releases v.0.4.0 - First release on PyPI v.0.5.0
-- Update requires python v.3.8+ and OCP v.7.6+ CadQuery 2.1+ ## Authors **CQ-
-Kit** was written by [Michael Gale](https://github.com/michaelgale)
+minimum) - Deployment notes ## Releases - v.0.4.0 - First release on PyPI -
+v.0.5.0 - Update requires python v.3.8+ and OCP v.7.6+ CadQuery 2.1+ ## Authors
+**CQ-Kit** was written by [Michael Gale](https://github.com/michaelgale)
```

### Comparing `cqkit-0.5.0/cqkit/__init__.py` & `cqkit-0.5.1/cqkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """cq-kit - A python library of CadQuery tools and helpers for building 3D CAD models."""
 
 import os
 
 # fmt: off
 __project__ = 'cqkit'
-__version__ = '0.5.0'
+__version__ = '0.5.1'
 # fmt: on
 
 VERSION = __project__ + "-" + __version__
 
 script_dir = os.path.dirname(__file__)
```

### Comparing `cqkit-0.5.0/cqkit/cq_discrete.py` & `cqkit-0.5.1/cqkit/cq_discrete.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 # Discrete Geometry Utilities
 
 try:
     from OCC.Core.BRep import BRep_Tool
     from OCC.Core.BRepAdaptor import BRepAdaptor_Curve
     from OCC.Core.BRepLProp import BRepLProp_CLProps
     from OCC.Core.BRepMesh import BRepMesh_IncrementalMesh
-    from OCC.Core.GCPnts import GCPnts_AbscissaPoint, GCPnts_QuasiUniformAbscissa
+    from OCC.Core.GCPnts import (GCPnts_AbscissaPoint,
+                                 GCPnts_QuasiUniformAbscissa)
     from OCC.Core.gp import gp_Dir
     from OCC.Core.TopAbs import TopAbs_FACE, TopAbs_VERTEX
     from OCC.Core.TopExp import TopExp_Explorer
     from OCC.Core.TopLoc import TopLoc_Location
     from OCC.Core.TopoDS import TopoDS_Face, TopoDS_Iterator, TopoDS_Vertex
 
 except:
```

### Comparing `cqkit-0.5.0/cqkit/cq_fasteners.py` & `cqkit-0.5.1/cqkit/cq_fasteners.py`

 * *Files identical despite different names*

### Comparing `cqkit-0.5.0/cqkit/cq_files.py` & `cqkit-0.5.1/cqkit/cq_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,35 +38,30 @@
 # under the hood. A better way of assigning OCCT_VERSION could
 # be done as well.
 
 try:
     from OCC.Core.BRepMesh import BRepMesh_IncrementalMesh
     from OCC.Core.IGESControl import *
     from OCC.Core.Interface import *
-    from OCC.Core.STEPControl import (
-        STEPControl_AsIs,
-        STEPControl_ManifoldSolidBrep,
-        STEPControl_Writer,
-    )
+    from OCC.Core.STEPControl import (STEPControl_AsIs,
+                                      STEPControl_ManifoldSolidBrep,
+                                      STEPControl_Writer)
     from OCC.Core.StlAPI import StlAPI_Writer
     from OCC.Extend.DataExchange import *
 
     OCCT_VERSION = "6.9"
 except:
     import OCP.IFSelect
-
     # from OCP.Extend.DataExchange import *
     from OCP.BRepMesh import BRepMesh_IncrementalMesh
     from OCP.IGESControl import *
     from OCP.Interface import *
-    from OCP.STEPControl import (
-        STEPControl_AsIs,
-        STEPControl_ManifoldSolidBrep,
-        STEPControl_Writer,
-    )
+    from OCP.STEPControl import (STEPControl_AsIs,
+                                 STEPControl_ManifoldSolidBrep,
+                                 STEPControl_Writer)
     from OCP.StlAPI import StlAPI_Writer
 
     Interface_Static_SetIVal = Interface_Static.SetIVal_s
     Interface_Static_SetCVal = Interface_Static.SetCVal_s
     OCCT_VERSION = "7.5"
```

### Comparing `cqkit-0.5.0/cqkit/cq_geometry.py` & `cqkit-0.5.1/cqkit/cq_geometry.py`

 * *Files identical despite different names*

### Comparing `cqkit-0.5.0/cqkit/cq_pprint.py` & `cqkit-0.5.1/cqkit/cq_pprint.py`

 * *Files identical despite different names*

### Comparing `cqkit-0.5.0/cqkit/cq_ribbon.py` & `cqkit-0.5.1/cqkit/cq_ribbon.py`

 * *Files identical despite different names*

### Comparing `cqkit-0.5.0/cqkit/cq_selectors.py` & `cqkit-0.5.1/cqkit/cq_selectors.py`

 * *Files identical despite different names*

### Comparing `cqkit-0.5.0/cqkit/cq_xsection.py` & `cqkit-0.5.1/cqkit/cq_xsection.py`

 * *Files identical despite different names*

### Comparing `cqkit-0.5.0/cqkit/refdim.py` & `cqkit-0.5.1/cqkit/refdim.py`

 * *Files identical despite different names*

### Comparing `cqkit-0.5.0/cqkit.egg-info/PKG-INFO` & `cqkit-0.5.1/cqkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cqkit
-Version: 0.5.0
+Version: 0.5.1
 Summary: A python library of CadQuery tools and helpers for building 3D CAD models.
 Home-page: https://github.com/michaelgale/cq-kit
 Author: Michael Gale
 Author-email: michael@fxbricks.com
 License: MIT
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -430,21 +430,22 @@
   - Others TBD
 - Documentation (possibly with sphinx, but in this README as a minimum)
 - Deployment notes
 
 
 ## Releases
 
-v.0.4.0 - First release on PyPI
-v.0.5.0 - Update requires python v.3.8+ and OCP v.7.6+ CadQuery 2.1+
+- v.0.4.0 - First release on PyPI
+- v.0.5.0 - Update requires python v.3.8+ and OCP v.7.6+ CadQuery 2.1+
+
 
 ## Authors
 
 **CQ-Kit** was written by [Michael Gale](https://github.com/michaelgale)
 
 ## Changelog
 
 - v.0.2.0 - Added cq_discrete with discretize_edge() and triangle_mesh_solid()
 - v.0.3.1 - Added import_iges_file()
 - v.0.4.0 - PyPI packaging
 - v.0.5.0 - Update to support newer versions of CadQuery and OCP, minimum python 3.8+
-- 
+-
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: cqkit Version: 0.5.0 Summary: A python library of
+Metadata-Version: 2.1 Name: cqkit Version: 0.5.1 Summary: A python library of
 CadQuery tools and helpers for building 3D CAD models. Home-page: https://
 github.com/michaelgale/cq-kit Author: Michael Gale Author-email:
-michael@fxbricks.com License: MIT Classifier: Development Status :: 3 - Alpha
+michael@fxbricks.com License: MIT Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.8 Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.8 Description-Content-Type: text/markdown License-
 File: LICENSE ![CQ-Kit Logo](./images/logo.png) # CQ-Kit ![https://pypi.org/
 project/cqkit/](https://img.shields.io/pypi/v/cqkit.svg) ![python version]
 (https://img.shields.io/static/
@@ -277,14 +277,14 @@
 vertex es = SharedVerticesWithObjectSelector(Vector(1, 2, 1)) ``` | [./images/
 commonvertface.png] | | --- | ```python # selects all edges which have any of
 its end points common with any vertex # belonging to a specified face face1 =
 solid.faces(FlatFaceSelector(1.0)).val() es = SharedVerticesWithObjectSelector
 (face1) ``` ## To Do - More modules/functionality for the package extracted
 from previous work in different places - Solids: solid construction classes -
 Others TBD - Documentation (possibly with sphinx, but in this README as a
-minimum) - Deployment notes ## Releases v.0.4.0 - First release on PyPI v.0.5.0
-- Update requires python v.3.8+ and OCP v.7.6+ CadQuery 2.1+ ## Authors **CQ-
-Kit** was written by [Michael Gale](https://github.com/michaelgale) ##
+minimum) - Deployment notes ## Releases - v.0.4.0 - First release on PyPI -
+v.0.5.0 - Update requires python v.3.8+ and OCP v.7.6+ CadQuery 2.1+ ## Authors
+**CQ-Kit** was written by [Michael Gale](https://github.com/michaelgale) ##
 Changelog - v.0.2.0 - Added cq_discrete with discretize_edge() and
 triangle_mesh_solid() - v.0.3.1 - Added import_iges_file() - v.0.4.0 - PyPI
 packaging - v.0.5.0 - Update to support newer versions of CadQuery and OCP,
 minimum python 3.8+ -
```

### Comparing `cqkit-0.5.0/setup.py` & `cqkit-0.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,39 +5,39 @@
 import os.path
 import sys
 
 import setuptools
 
 PACKAGE_NAME = "cqkit"
 
-loc = os.path.abspath(os.path.dirname(__file__))
+# loc = os.path.abspath(os.path.dirname(__file__))
 
-with open(loc + "/requirements.txt") as f:
-    requirements = f.read().splitlines()
+# with open(loc + "/requirements.txt") as f:
+#     requirements = f.read().splitlines()
 
 required = []
 dependency_links = []
-# do not add to required lines pointing to git repositories
-EGG_MARK = "#egg="
-for line in requirements:
-    if (
-        line.startswith("-e git:")
-        or line.startswith("-e git+")
-        or line.startswith("git:")
-        or line.startswith("git+")
-    ):
-        if EGG_MARK in line:
-            package_name = line[line.find(EGG_MARK) + len(EGG_MARK) :]
-            required.append(package_name)
-            dependency_links.append(line)
-        else:
-            print("Dependency to a git repository should have the format:")
-            print("git+ssh://git@github.com/xxxxx/xxxxxx#egg=package_name")
-    else:
-        required.append(line)
+# # do not add to required lines pointing to git repositories
+# EGG_MARK = "#egg="
+# for line in requirements:
+#     if (
+#         line.startswith("-e git:")
+#         or line.startswith("-e git+")
+#         or line.startswith("git:")
+#         or line.startswith("git+")
+#     ):
+#         if EGG_MARK in line:
+#             package_name = line[line.find(EGG_MARK) + len(EGG_MARK) :]
+#             required.append(package_name)
+#             dependency_links.append(line)
+#         else:
+#             print("Dependency to a git repository should have the format:")
+#             print("git+ssh://git@github.com/xxxxx/xxxxxx#egg=package_name")
+#     else:
+#         required.append(line)
 
 
 def read_package_variable(key, filename="__init__.py"):
     """Read the value of a variable from the package without importing."""
     module_path = os.path.join(PACKAGE_NAME, filename)
     with open(module_path) as module:
         for line in module:
@@ -67,15 +67,15 @@
     author_email="michael@fxbricks.com",
     python_requires=">=3.8",
     packages=setuptools.find_packages(),
     long_description=build_description(),
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.8",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
     ],
     install_requires=required,
```

