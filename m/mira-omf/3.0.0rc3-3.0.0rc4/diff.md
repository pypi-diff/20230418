# Comparing `tmp/mira-omf-3.0.0rc3.tar.gz` & `tmp/mira_omf-3.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mira-omf-3.0.0rc3.tar", max compression
+gzip compressed data, was "mira_omf-3.0.0rc4.tar", max compression
```

## Comparing `mira-omf-3.0.0rc3.tar` & `mira_omf-3.0.0rc4.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1122 2023-03-23 18:03:51.811570 mira-omf-3.0.0rc3/LICENSE
--rw-r--r--   0        0        0     1684 2023-03-28 18:51:42.937154 mira-omf-3.0.0rc3/omf/__init__.py
--rw-r--r--   0        0        0     6754 2023-03-23 18:03:52.423966 mira-omf-3.0.0rc3/omf/base.py
--rw-r--r--   0        0        0     8561 2023-03-23 18:03:52.423966 mira-omf-3.0.0rc3/omf/data.py
--rw-r--r--   0        0        0      111 2023-03-23 18:03:52.424966 mira-omf-3.0.0rc3/omf/fileio/__init__.py
--rw-r--r--   0        0        0     5973 2023-03-23 18:03:52.424966 mira-omf-3.0.0rc3/omf/fileio/fileio.py
--rw-r--r--   0        0        0    35136 2023-03-23 18:03:52.425967 mira-omf-3.0.0rc3/omf/fileio/geoh5.py
--rw-r--r--   0        0        0     1123 2023-03-23 18:03:52.425967 mira-omf-3.0.0rc3/omf/fileio/utils.py
--rw-r--r--   0        0        0     1760 2023-03-23 18:03:52.425967 mira-omf-3.0.0rc3/omf/lineset.py
--rw-r--r--   0        0        0     1411 2023-03-23 18:03:52.425967 mira-omf-3.0.0rc3/omf/pointset.py
--rw-r--r--   0        0        0        0 2023-03-23 18:03:52.426966 mira-omf-3.0.0rc3/omf/scripts/__init__.py
--rw-r--r--   0        0        0     1171 2023-03-28 18:51:42.937154 mira-omf-3.0.0rc3/omf/scripts/geoh5_to_omf.py
--rw-r--r--   0        0        0     1180 2023-03-28 18:51:42.937154 mira-omf-3.0.0rc3/omf/scripts/omf_to_geoh5.py
--rw-r--r--   0        0        0     3682 2023-03-23 18:03:52.427966 mira-omf-3.0.0rc3/omf/serializers.py
--rw-r--r--   0        0        0     3736 2023-03-23 18:03:52.428162 mira-omf-3.0.0rc3/omf/surface.py
--rw-r--r--   0        0        0      675 2023-03-23 18:03:52.428162 mira-omf-3.0.0rc3/omf/texture.py
--rw-r--r--   0        0        0     2409 2023-03-23 18:03:52.429187 mira-omf-3.0.0rc3/omf/volume.py
--rw-r--r--   0        0        0     1731 2023-03-28 18:51:42.938154 mira-omf-3.0.0rc3/pyproject.toml
--rw-r--r--   0        0        0     2802 2023-03-28 18:51:42.936154 mira-omf-3.0.0rc3/README.rst
--rw-r--r--   0        0        0     3809 2023-03-28 18:52:48.428439 mira-omf-3.0.0rc3/setup.py
--rw-r--r--   0        0        0     3983 2023-03-28 18:52:48.428439 mira-omf-3.0.0rc3/PKG-INFO
+-rw-r--r--   0        0        0     1122 2023-03-23 18:03:51.811570 mira_omf-3.0.0rc4/LICENSE
+-rw-r--r--   0        0        0     1684 2023-04-18 20:37:26.576078 mira_omf-3.0.0rc4/omf/__init__.py
+-rw-r--r--   0        0        0     6754 2023-03-23 18:03:52.423966 mira_omf-3.0.0rc4/omf/base.py
+-rw-r--r--   0        0        0     8561 2023-03-23 18:03:52.423966 mira_omf-3.0.0rc4/omf/data.py
+-rw-r--r--   0        0        0      111 2023-03-23 18:03:52.424966 mira_omf-3.0.0rc4/omf/fileio/__init__.py
+-rw-r--r--   0        0        0     5973 2023-03-23 18:03:52.424966 mira_omf-3.0.0rc4/omf/fileio/fileio.py
+-rw-r--r--   0        0        0    35299 2023-04-18 20:37:26.577078 mira_omf-3.0.0rc4/omf/fileio/geoh5.py
+-rw-r--r--   0        0        0     1123 2023-03-23 18:03:52.425967 mira_omf-3.0.0rc4/omf/fileio/utils.py
+-rw-r--r--   0        0        0     1760 2023-03-23 18:03:52.425967 mira_omf-3.0.0rc4/omf/lineset.py
+-rw-r--r--   0        0        0     1411 2023-03-23 18:03:52.425967 mira_omf-3.0.0rc4/omf/pointset.py
+-rw-r--r--   0        0        0        0 2023-03-23 18:03:52.426966 mira_omf-3.0.0rc4/omf/scripts/__init__.py
+-rw-r--r--   0        0        0     1171 2023-03-28 18:51:42.937154 mira_omf-3.0.0rc4/omf/scripts/geoh5_to_omf.py
+-rw-r--r--   0        0        0     1180 2023-03-28 18:51:42.937154 mira_omf-3.0.0rc4/omf/scripts/omf_to_geoh5.py
+-rw-r--r--   0        0        0     3682 2023-03-23 18:03:52.427966 mira_omf-3.0.0rc4/omf/serializers.py
+-rw-r--r--   0        0        0     3736 2023-03-23 18:03:52.428162 mira_omf-3.0.0rc4/omf/surface.py
+-rw-r--r--   0        0        0      675 2023-03-23 18:03:52.428162 mira_omf-3.0.0rc4/omf/texture.py
+-rw-r--r--   0        0        0     2409 2023-03-23 18:03:52.429187 mira_omf-3.0.0rc4/omf/volume.py
+-rw-r--r--   0        0        0     1731 2023-04-18 20:37:26.578079 mira_omf-3.0.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     2802 2023-04-18 20:37:26.576078 mira_omf-3.0.0rc4/README.rst
+-rw-r--r--   0        0        0     3983 1970-01-01 00:00:00.000000 mira_omf-3.0.0rc4/PKG-INFO
```

### Comparing `mira-omf-3.0.0rc3/LICENSE` & `mira_omf-3.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `mira-omf-3.0.0rc3/omf/__init__.py` & `mira_omf-3.0.0rc4/omf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from .fileio import GeoH5Writer, OMFReader, OMFWriter
 from .lineset import LineSetElement, LineSetGeometry
 from .pointset import PointSetElement, PointSetGeometry
 from .surface import SurfaceElement, SurfaceGeometry, SurfaceGridGeometry
 from .texture import ImageTexture
 from .volume import VolumeElement, VolumeGridGeometry
 
-__version__ = "3.0.0-rc.3"
+__version__ = "3.0.0-rc.4"
 __author__ = "Global Mining Standards and Guidelines Group"
 __license__ = "MIT License"
 __copyright__ = "Copyright 2017 Global Mining Standards and Guidelines Group"
 
 
 def _create_logger():
     error_handler = logging.StreamHandler(sys.stderr)
```

### Comparing `mira-omf-3.0.0rc3/omf/base.py` & `mira_omf-3.0.0rc4/omf/base.py`

 * *Files identical despite different names*

### Comparing `mira-omf-3.0.0rc3/omf/data.py` & `mira_omf-3.0.0rc4/omf/data.py`

 * *Files identical despite different names*

### Comparing `mira-omf-3.0.0rc3/omf/fileio/fileio.py` & `mira_omf-3.0.0rc4/omf/fileio/fileio.py`

 * *Files identical despite different names*

### Comparing `mira-omf-3.0.0rc3/omf/fileio/geoh5.py` & `mira_omf-3.0.0rc4/omf/fileio/geoh5.py`

 * *Files 1% similar despite different names*

```diff
@@ -489,23 +489,26 @@
         return kwargs
 
     @staticmethod
     def collect_omf_attributes(element, **kwargs) -> dict:
         if not element.legends:
             return kwargs
 
-        value_map = {
-            count + 1: str(val) for count, val in enumerate(element.legends[0].values)
-        }
-        color_map = np.vstack(
-            [
-                np.r_[count + 1, val, 1.0]
-                for count, val in enumerate(element.legends[1].values)
-            ]
-        )
+        for legend in element.legends:
+            if isinstance(legend.values, StringArray):
+                value_map = {
+                    count + 1: str(val) for count, val in enumerate(legend.values)
+                }
+            else:
+                color_map = np.vstack(
+                    [
+                        np.r_[count + 1, val, 1.0]
+                        for count, val in enumerate(legend.values)
+                    ]
+                )
         kwargs["value_map"] = value_map
         kwargs["type"] = "referenced"
         kwargs["color_map"] = color_map
 
         return kwargs
 
     @staticmethod
```

### Comparing `mira-omf-3.0.0rc3/omf/fileio/utils.py` & `mira_omf-3.0.0rc4/omf/fileio/utils.py`

 * *Files identical despite different names*

### Comparing `mira-omf-3.0.0rc3/omf/lineset.py` & `mira_omf-3.0.0rc4/omf/lineset.py`

 * *Files identical despite different names*

### Comparing `mira-omf-3.0.0rc3/omf/pointset.py` & `mira_omf-3.0.0rc4/omf/pointset.py`

 * *Files identical despite different names*

### Comparing `mira-omf-3.0.0rc3/omf/scripts/geoh5_to_omf.py` & `mira_omf-3.0.0rc4/omf/scripts/geoh5_to_omf.py`

 * *Files identical despite different names*

### Comparing `mira-omf-3.0.0rc3/omf/scripts/omf_to_geoh5.py` & `mira_omf-3.0.0rc4/omf/scripts/omf_to_geoh5.py`

 * *Files identical despite different names*

### Comparing `mira-omf-3.0.0rc3/omf/serializers.py` & `mira_omf-3.0.0rc4/omf/serializers.py`

 * *Files identical despite different names*

### Comparing `mira-omf-3.0.0rc3/omf/surface.py` & `mira_omf-3.0.0rc4/omf/surface.py`

 * *Files identical despite different names*

### Comparing `mira-omf-3.0.0rc3/omf/texture.py` & `mira_omf-3.0.0rc4/omf/texture.py`

 * *Files identical despite different names*

### Comparing `mira-omf-3.0.0rc3/omf/volume.py` & `mira_omf-3.0.0rc4/omf/volume.py`

 * *Files identical despite different names*

### Comparing `mira-omf-3.0.0rc3/pyproject.toml` & `mira_omf-3.0.0rc4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mira-omf"
-version = "3.0.0-rc.3"
+version = "3.0.0-rc.4"
 description = "API Library for Open Mining Format"
 authors = [
     "Mira Geoscience <dominiquef@mirageoscience.com>",
     "Global Mining Standards and Guidelines Group <it@seequent.com>",
 ]
 repository = "https://github.com/MiraGeoscience/omf"
 homepage = "http://www.globalminingstandards.org/"
```

### Comparing `mira-omf-3.0.0rc3/README.rst` & `mira_omf-3.0.0rc4/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     :alt: MIT license
 
 .. image:: https://github.com/MiraGeoscience/omf/actions/workflows/pytest-windows.yml/badge.svg
     :target: https://github.com/MiraGeoscience/omf/actions/workflows/pytest-windows.yml
     :alt: pytest
 
 
-Version: 3.0.0-rc.3
+Version: 3.0.0-rc.4
 
 API library for Open Mining Format, a new standard for mining data backed by
 the `Global Mining Standards & Guidelines Group <http://www.globalminingstandards.org/>`_.
 
 .. warning::
     **Pre-Release Notice**
```

### Comparing `mira-omf-3.0.0rc3/PKG-INFO` & `mira_omf-3.0.0rc4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: mira-omf
-Version: 3.0.0rc3
+Version: 3.0.0rc4
 Summary: API Library for Open Mining Format
 Home-page: http://www.globalminingstandards.org/
 Keywords: geology,geophysics,earth sciences
 Author: Mira Geoscience
 Author-email: dominiquef@mirageoscience.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: geoh5py (>=0.5.0)
 Requires-Dist: numpy (>=1.7,<2.0)
 Requires-Dist: properties (>=0.6.0,<0.7.0)
 Requires-Dist: pypng (>=0.20220715,<0.20220716)
@@ -46,15 +46,15 @@
     :alt: MIT license
 
 .. image:: https://github.com/MiraGeoscience/omf/actions/workflows/pytest-windows.yml/badge.svg
     :target: https://github.com/MiraGeoscience/omf/actions/workflows/pytest-windows.yml
     :alt: pytest
 
 
-Version: 3.0.0-rc.3
+Version: 3.0.0-rc.4
 
 API library for Open Mining Format, a new standard for mining data backed by
 the `Global Mining Standards & Guidelines Group <http://www.globalminingstandards.org/>`_.
 
 .. warning::
     **Pre-Release Notice**
```

