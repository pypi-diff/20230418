# Comparing `tmp/ansys_materials_manager-0.1.0.tar.gz` & `tmp/ansys_materials_manager-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_materials_manager-0.1.0.tar", max compression
+gzip compressed data, was "ansys_materials_manager-0.2.0.tar", max compression
```

## Comparing `ansys_materials_manager-0.1.0.tar` & `ansys_materials_manager-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1089 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/LICENSE
--rw-r--r--   0        0        0     6335 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/README.rst
--rw-r--r--   0        0        0     2119 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      368 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/__init__.py
--rw-r--r--   0        0        0      512 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/_common/__init__.py
--rw-r--r--   0        0        0     2111 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/_common/_base.py
--rw-r--r--   0        0        0      480 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/_common/_exceptions.py
--rw-r--r--   0        0        0      189 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/_common/_packages.py
--rw-r--r--   0        0        0     3974 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/_common/constant.py
--rw-r--r--   0        0        0     6199 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/_common/piecewise_linear.py
--rw-r--r--   0        0        0     6052 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/_common/polynomial.py
--rw-r--r--   0        0        0        0 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/_fluent/__init__.py
--rw-r--r--   0        0        0     2981 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/_fluent/ideal_gas.py
--rw-r--r--   0        0        0      334 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/_fluent/simple_properties.py
--rw-r--r--   0        0        0        0 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/_mapdl/__init__.py
--rw-r--r--   0        0        0    14912 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/_mapdl/anisotropic_elasticity.py
--rw-r--r--   0        0        0     2033 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/_mapdl/simple_properties.py
--rw-r--r--   0        0        0        0 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/py.typed
--rw-r--r--   0        0        0     2967 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/material.py
--rw-r--r--   0        0        0     3070 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/material_manager.py
--rw-r--r--   0        0        0     1495 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/serialize.py
--rw-r--r--   0        0        0        0 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/util/__init__.py
--rw-r--r--   0        0        0     2972 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/util/common.py
--rw-r--r--   0        0        0        0 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/util/mapdl/__init__.py
--rw-r--r--   0        0        0     1073 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/util/mapdl/mapdl_reader.py
--rw-r--r--   0        0        0     6565 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/util/mapdl/mpdata_parser.py
--rw-r--r--   0        0        0     3217 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/util/mapdl/tbdata_parser.py
--rw-r--r--   0        0        0      117 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/util/matml/__init__.py
--rw-r--r--   0        0        0     8146 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/util/matml/matml_from_material.py
--rw-r--r--   0        0        0     7378 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/util/matml/matml_parser.py
--rw-r--r--   0        0        0     2993 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/util/matml/matml_property_map.py
--rw-r--r--   0        0        0     3081 2023-04-11 10:48:11.897282 ansys_materials_manager-0.1.0/src/ansys/materials/manager/util/matml/matml_to_material.py
--rw-r--r--   0        0        0     7955 1970-01-01 00:00:00.000000 ansys_materials_manager-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-18 16:17:46.452172 ansys_materials_manager-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6343 2023-04-18 16:17:46.452172 ansys_materials_manager-0.2.0/README.rst
+-rw-r--r--   0        0        0     2119 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      368 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/__init__.py
+-rw-r--r--   0        0        0      512 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/__init__.py
+-rw-r--r--   0        0        0     2111 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/_base.py
+-rw-r--r--   0        0        0      480 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/_exceptions.py
+-rw-r--r--   0        0        0      189 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/_packages.py
+-rw-r--r--   0        0        0     3974 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/constant.py
+-rw-r--r--   0        0        0     6199 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/piecewise_linear.py
+-rw-r--r--   0        0        0     6052 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/polynomial.py
+-rw-r--r--   0        0        0        0 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_fluent/__init__.py
+-rw-r--r--   0        0        0     2981 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_fluent/ideal_gas.py
+-rw-r--r--   0        0        0      334 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_fluent/simple_properties.py
+-rw-r--r--   0        0        0        0 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_mapdl/__init__.py
+-rw-r--r--   0        0        0    14912 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_mapdl/anisotropic_elasticity.py
+-rw-r--r--   0        0        0     2033 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_mapdl/simple_properties.py
+-rw-r--r--   0        0        0        0 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/py.typed
+-rw-r--r--   0        0        0     2967 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/material.py
+-rw-r--r--   0        0        0     3070 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/material_manager.py
+-rw-r--r--   0        0        0     1495 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/serialize.py
+-rw-r--r--   0        0        0        0 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/__init__.py
+-rw-r--r--   0        0        0     2972 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/common.py
+-rw-r--r--   0        0        0        0 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/mapdl/__init__.py
+-rw-r--r--   0        0        0     1073 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/mapdl/mapdl_reader.py
+-rw-r--r--   0        0        0     6565 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/mapdl/mpdata_parser.py
+-rw-r--r--   0        0        0     3217 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/mapdl/tbdata_parser.py
+-rw-r--r--   0        0        0      117 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/matml/__init__.py
+-rw-r--r--   0        0        0     9013 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/matml/matml_from_material.py
+-rw-r--r--   0        0        0     7378 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/matml/matml_parser.py
+-rw-r--r--   0        0        0     2993 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/matml/matml_property_map.py
+-rw-r--r--   0        0        0     3081 2023-04-18 16:17:46.456172 ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/matml/matml_to_material.py
+-rw-r--r--   0        0        0     7963 1970-01-01 00:00:00.000000 ansys_materials_manager-0.2.0/PKG-INFO
```

### Comparing `ansys_materials_manager-0.1.0/LICENSE` & `ansys_materials_manager-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.1.0/README.rst` & `ansys_materials_manager-0.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
 
 .. |python| image:: https://img.shields.io/badge/Python-%3E%3D3.10-blue
    :target: https://pypi.org/project/pymaterials-manager/
    :alt: Python
 
-.. |pypi| image:: https://img.shields.io/pypi/v/pymaterials-manager.svg?logo=python&logoColor=white
-   :target: https://pypi.org/project/pymaterials-manager
+.. |pypi| image:: https://img.shields.io/pypi/v/ansys-materials-manager.svg?logo=python&logoColor=white
+   :target: https://pypi.org/project/ansys-materials-manager
    :alt: PyPI
 
 .. |codecov| image:: https://codecov.io/gh/pyansys/pymaterials-manager/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/pyansys/pymaterials-manager
    :alt: Codecov
 
 .. |GH-CI| image:: https://github.com/pyansys/pymaterials-manager/actions/workflows/ci_cd.yml/badge.svg
```

### Comparing `ansys_materials_manager-0.1.0/pyproject.toml` & `ansys_materials_manager-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 # Check https://python-poetry.org/docs/pyproject/ for all available sections
 name = "ansys-materials-manager"
-version = "0.1.0"
+version = "0.2.0"
 description = "Python package to unify material management across the ansys portfolio"
 license = "MIT"
 authors = ["ANSYS, Inc. <ansys.support@ansys.com>"]
 maintainers = ["PyAnsys developers <pyansys.core@ansys.com>"]
 readme = "README.rst"
 repository = "https://github.com/pyansys/pymaterials-manager"
 documentation = "https://manager.materials.docs.pyansys.com"
@@ -32,15 +32,15 @@
 
 # Documentation dependencies
 ansys-sphinx-theme = {version = "==0.9.7", optional = true}
 importlib-metadata = {version = "^6.3", python = "<3.7"}
 numpydoc = {version = "==1.5.0", optional = true}
 Sphinx = {version = "==5.1.1", optional = true}
 sphinx-autoapi = {version = "==2.0.1", optional = true}
-sphinx-copybutton = {version = "==0.5.1", optional = true}
+sphinx-copybutton = {version = "==0.5.2", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 coolprop = "^6.4.1"
 ansys-mapdl-core = "^0.64.1"
 ansys-fluent-core = "^0.12.5"
 twine = "^4.0.2"
```

### Comparing `ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/__init__.py` & `ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/_common/_base.py` & `ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/_base.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/_common/constant.py` & `ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/constant.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/_common/piecewise_linear.py` & `ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/piecewise_linear.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/_common/polynomial.py` & `ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_common/polynomial.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/_fluent/ideal_gas.py` & `ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_fluent/ideal_gas.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/_mapdl/anisotropic_elasticity.py` & `ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_mapdl/anisotropic_elasticity.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.1.0/src/ansys/materials/manager/_models/_mapdl/simple_properties.py` & `ansys_materials_manager-0.2.0/src/ansys/materials/manager/_models/_mapdl/simple_properties.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.1.0/src/ansys/materials/manager/material.py` & `ansys_materials_manager-0.2.0/src/ansys/materials/manager/material.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.1.0/src/ansys/materials/manager/material_manager.py` & `ansys_materials_manager-0.2.0/src/ansys/materials/manager/material_manager.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.1.0/src/ansys/materials/manager/serialize.py` & `ansys_materials_manager-0.2.0/src/ansys/materials/manager/serialize.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.1.0/src/ansys/materials/manager/util/common.py` & `ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/common.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.1.0/src/ansys/materials/manager/util/mapdl/mapdl_reader.py` & `ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/mapdl/mapdl_reader.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.1.0/src/ansys/materials/manager/util/mapdl/mpdata_parser.py` & `ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/mapdl/mpdata_parser.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.1.0/src/ansys/materials/manager/util/mapdl/tbdata_parser.py` & `ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/mapdl/tbdata_parser.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.1.0/src/ansys/materials/manager/util/matml/matml_from_material.py` & `ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/matml/matml_from_material.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Provides the ``MatmlWriter`` class."""
 import os
-from typing import Dict, Sequence, Union
+from typing import BinaryIO, Dict, Sequence, Union
 import xml.etree.ElementTree as ET
 
 from ansys.materials.manager.material import Material
 
 from .matml_parser import (
     BULKDATA_KEY,
     MATERIALS_ELEMENT_KEY,
@@ -155,29 +155,15 @@
         for mat in self._materials:
             mat_element = ET.SubElement(materials_element, "Material")
             name_element = ET.SubElement(mat_element, "Name")
             name_element.text = mat.name
             transfer_element = ET.SubElement(mat_element, "DataTransferID")
             transfer_element.text = mat.uuid
 
-    def export(self, path: _PATH_TYPE, **kwargs):
-        """
-        Write a Matml (engineering data xml file from scratch).
-
-        Parameters
-        ----------
-        path :
-            File path.
-        materials :
-            list of materials.
-
-        Keyword arguments
-        -----------------
-        indent - add an indent to format the XML output (python 3.9+). Defaults to false.
-        """
+    def _to_etree(self) -> ET.ElementTree:
         root = ET.Element(ROOT_ELEMENT)
         tree = ET.ElementTree(root)
 
         root.attrib["version"] = VERSION
         root.attrib["versiondate"] = VERSION_DATE
         notes_element = ET.SubElement(root, "Notes")
         notes_element.text = "Engineering data xml file generated by pyMaterials."
@@ -189,15 +175,55 @@
 
         # add metadata to the XML tree
         metadata_element = ET.SubElement(matml_doc_element, METADATA_KEY)
         self._add_metadata(metadata_element)
 
         # add transfer id to the XML tree
         self._add_transfer_ids(root)
+        return tree
+
+    def _indent(self, tree) -> None:
+        if hasattr(ET, "indent"):
+            ET.indent(tree)
+        else:
+            print(f"ElementTree does not have `indent`. Python 3.9+ required!")
+
+    def write(self, buffer: BinaryIO, **kwargs) -> None:
+        """
+        Write a Matml (engineering data xml format) representation of materials to buffer.
+
+        Parameters
+        ----------
+        buffer:
+            buffer to write to
+        **kwargs : bool, optional
+            Optional keyword arguments.
+            indent : bool, optional
+                Whether to add an indent to format the XML output(python 3.9+).
+                Defaults to ``false``.
+        """
+        tree = self._to_etree()
+
+        if kwargs.get("indent", False):
+            self._indent(tree)
+        buffer.write(ET.tostring(tree.getroot()))
+
+    def export(self, path: _PATH_TYPE, **kwargs) -> None:
+        """
+        Write a Matml (engineering data xml format) representation of materials to file.
+
+        Parameters
+        ----------
+        path:
+            File path
+        **kwargs : bool, optional
+            Optional keyword arguments.
+            indent : bool, optional
+                Whether to add an indent to format the XML output(python 3.9+).
+                Defaults to ``false``.
+        """
+        tree = self._to_etree()
 
         print(f"write xml to {path}")
         if kwargs.get("indent", False):
-            if hasattr(ET, "indent"):
-                ET.indent(tree)
-            else:
-                print(f"ElementTree does not have `indent`. Python 3.9+ required!")
+            self._indent(tree)
         tree.write(path)
```

### Comparing `ansys_materials_manager-0.1.0/src/ansys/materials/manager/util/matml/matml_parser.py` & `ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/matml/matml_parser.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.1.0/src/ansys/materials/manager/util/matml/matml_property_map.py` & `ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/matml/matml_property_map.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.1.0/src/ansys/materials/manager/util/matml/matml_to_material.py` & `ansys_materials_manager-0.2.0/src/ansys/materials/manager/util/matml/matml_to_material.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.1.0/PKG-INFO` & `ansys_materials_manager-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-materials-manager
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python package to unify material management across the ansys portfolio
 Home-page: https://github.com/pyansys/pymaterials-manager
 License: MIT
 Author: ANSYS, Inc.
 Author-email: ansys.support@ansys.com
 Maintainer: PyAnsys developers
 Maintainer-email: pyansys.core@ansys.com
@@ -24,15 +24,15 @@
 Requires-Dist: ansys-sphinx-theme (==0.9.7) ; extra == "doc"
 Requires-Dist: importlib-metadata (>=6.3,<7.0) ; python_version < "3.7"
 Requires-Dist: numpy (>=1.24.2,<2.0.0) ; python_full_version > "3.8.0"
 Requires-Dist: numpydoc (==1.5.0) ; extra == "doc"
 Requires-Dist: pandas (>=2.0,<3.0) ; python_full_version > "3.8.0"
 Requires-Dist: scipy (>=1.9.3,<2.0.0) ; python_full_version > "3.8.0"
 Requires-Dist: sphinx-autoapi (==2.0.1) ; extra == "doc"
-Requires-Dist: sphinx-copybutton (==0.5.1) ; extra == "doc"
+Requires-Dist: sphinx-copybutton (==0.5.2) ; extra == "doc"
 Project-URL: Documentation, https://manager.materials.docs.pyansys.com
 Project-URL: Repository, https://github.com/pyansys/pymaterials-manager
 Description-Content-Type: text/x-rst
 
 PyMaterials Manager
 ===================
 |pyansys| |python| |pypi| |GH-CI| |codecov| |MIT| |black|
@@ -41,16 +41,16 @@
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
 
 .. |python| image:: https://img.shields.io/badge/Python-%3E%3D3.10-blue
    :target: https://pypi.org/project/pymaterials-manager/
    :alt: Python
 
-.. |pypi| image:: https://img.shields.io/pypi/v/pymaterials-manager.svg?logo=python&logoColor=white
-   :target: https://pypi.org/project/pymaterials-manager
+.. |pypi| image:: https://img.shields.io/pypi/v/ansys-materials-manager.svg?logo=python&logoColor=white
+   :target: https://pypi.org/project/ansys-materials-manager
    :alt: PyPI
 
 .. |codecov| image:: https://codecov.io/gh/pyansys/pymaterials-manager/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/pyansys/pymaterials-manager
    :alt: Codecov
 
 .. |GH-CI| image:: https://github.com/pyansys/pymaterials-manager/actions/workflows/ci_cd.yml/badge.svg
```

