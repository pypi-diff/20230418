# Comparing `tmp/fieldfitter-0.2.0.tar.gz` & `tmp/fieldfitter-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fieldfitter-0.2.0.tar", last modified: Tue Jul 26 04:22:00 2022, max compression
+gzip compressed data, was "fieldfitter-0.3.0.tar", last modified: Mon Apr 17 23:36:03 2023, max compression
```

## Comparing `fieldfitter-0.2.0.tar` & `fieldfitter-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-07-26 04:22:00.490279 fieldfitter-0.2.0/
--rw-r--r--   0 hsor001  (1210695619) 1403514002      594 2022-07-26 04:17:45.000000 fieldfitter-0.2.0/LICENSE
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1902 2022-07-26 04:22:00.490045 fieldfitter-0.2.0/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      504 2022-07-26 04:18:37.000000 fieldfitter-0.2.0/README.rst
--rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2022-07-26 04:22:00.490366 fieldfitter-0.2.0/setup.cfg
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1466 2022-07-26 04:21:46.000000 fieldfitter-0.2.0/setup.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-07-26 04:22:00.487041 fieldfitter-0.2.0/src/
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-07-26 04:22:00.488174 fieldfitter-0.2.0/src/fieldfitter/
--rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2022-06-16 07:45:22.000000 fieldfitter-0.2.0/src/fieldfitter/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    51496 2022-07-26 04:16:16.000000 fieldfitter-0.2.0/src/fieldfitter/fitter.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-07-26 04:22:00.489717 fieldfitter-0.2.0/src/fieldfitter.egg-info/
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1902 2022-07-26 04:22:00.000000 fieldfitter-0.2.0/src/fieldfitter.egg-info/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      313 2022-07-26 04:22:00.000000 fieldfitter-0.2.0/src/fieldfitter.egg-info/SOURCES.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2022-07-26 04:22:00.000000 fieldfitter-0.2.0/src/fieldfitter.egg-info/dependency_links.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2022-06-16 07:46:42.000000 fieldfitter-0.2.0/src/fieldfitter.egg-info/not-zip-safe
--rw-r--r--   0 hsor001  (1210695619) 1403514002       41 2022-07-26 04:22:00.000000 fieldfitter-0.2.0/src/fieldfitter.egg-info/requires.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002       12 2022-07-26 04:22:00.000000 fieldfitter-0.2.0/src/fieldfitter.egg-info/top_level.txt
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-17 23:36:03.962102 fieldfitter-0.3.0/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      594 2022-07-26 04:17:45.000000 fieldfitter-0.3.0/LICENSE
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1882 2023-04-17 23:36:03.961857 fieldfitter-0.3.0/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      494 2023-04-17 23:35:19.000000 fieldfitter-0.3.0/README.rst
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2023-04-17 23:36:03.962184 fieldfitter-0.3.0/setup.cfg
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1436 2023-04-17 23:35:24.000000 fieldfitter-0.3.0/setup.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-17 23:36:03.958108 fieldfitter-0.3.0/src/
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-17 23:36:03.959448 fieldfitter-0.3.0/src/fieldfitter/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2022-06-16 07:45:22.000000 fieldfitter-0.3.0/src/fieldfitter/__init__.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    51525 2023-04-17 23:35:19.000000 fieldfitter-0.3.0/src/fieldfitter/fitter.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-17 23:36:03.961506 fieldfitter-0.3.0/src/fieldfitter.egg-info/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1882 2023-04-17 23:36:03.000000 fieldfitter-0.3.0/src/fieldfitter.egg-info/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      313 2023-04-17 23:36:03.000000 fieldfitter-0.3.0/src/fieldfitter.egg-info/SOURCES.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-17 23:36:03.000000 fieldfitter-0.3.0/src/fieldfitter.egg-info/dependency_links.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2022-06-16 07:46:42.000000 fieldfitter-0.3.0/src/fieldfitter.egg-info/not-zip-safe
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       25 2023-04-17 23:36:03.000000 fieldfitter-0.3.0/src/fieldfitter.egg-info/requires.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       12 2023-04-17 23:36:03.000000 fieldfitter-0.3.0/src/fieldfitter.egg-info/top_level.txt
```

### Comparing `fieldfitter-0.2.0/LICENSE` & `fieldfitter-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fieldfitter-0.2.0/PKG-INFO` & `fieldfitter-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: fieldfitter
-Version: 0.2.0
-Summary: Scaffold/model field fitting library using OpenCMISS-Zinc.
+Version: 0.3.0
+Summary: Scaffold/model field fitting library using Zinc.
 Home-page: https://github.com/ABI-Software/fieldfitter
 Author: Auckland Bioengineering Institute
 Author-email: r.christie@auckland.ac.nz
 License: Apache Software License
 Description: Field Fitter
         ============
         
-        Scaffold/model field fitting library using OpenCMISS-Zinc.
+        Scaffold/model field fitting library using Zinc.
         
         Takes as input a Zinc model file and a Zinc data file.
         Model requires a model coordinates field, and data a data coordinates field
         which are in the same aligned/fitted configuration.
         
         Additional fields defined on the data may be defined and fitted to a continuous field
         on the model or a subgroup of it. The fitted field is defined using the
```

### Comparing `fieldfitter-0.2.0/setup.py` & `fieldfitter-0.3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 
 
 readme = readfile("README.rst", True)
 # For requirements not hosted on PyPi place listings
 # into the 'requirements.txt' file.
 requires = [
     # minimal requirements listing
-    "opencmiss.utils >= 0.3",
-    "opencmiss.zinc >= 3.7"
+    "cmlibs.utils",
+    "cmlibs.zinc"
 ]
 readme.extend(['', 'License', '=======', '', '::', ''])
 source_license = readfile("LICENSE")
 
 setup(
     name="fieldfitter",
-    version="0.2.0",
-    description="Scaffold/model field fitting library using OpenCMISS-Zinc.",
+    version="0.3.0",
+    description="Scaffold/model field fitting library using Zinc.",
     long_description="\n".join(readme) + source_license,
     long_description_content_type="text/x-rst",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python",
         "Topic :: Scientific/Engineering :: Medical Science Apps."
     ],
```

### Comparing `fieldfitter-0.2.0/src/fieldfitter/fitter.py` & `fieldfitter-0.3.0/src/fieldfitter/fitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 Class for fitting fields on geometrically aligned scaffolds.
 """
 
 import json
 import sys
 from timeit import default_timer as timer
 
-from opencmiss.utils.zinc.field import getGroupList, findOrCreateFieldStoredMeshLocation, getUniqueFieldName, \
+from cmlibs.utils.zinc.field import getGroupList, findOrCreateFieldStoredMeshLocation, getUniqueFieldName, \
     orphanFieldByName
-from opencmiss.utils.zinc.finiteelement import getMaximumNodeIdentifier
-from opencmiss.utils.zinc.general import ChangeManager
-from opencmiss.zinc.context import Context
-from opencmiss.zinc.field import Field, FieldFindMeshLocation, FieldFiniteElement
-from opencmiss.zinc.node import Node
-from opencmiss.zinc.optimisation import Optimisation
-from opencmiss.zinc.result import RESULT_OK, RESULT_WARNING_PART_DONE
+from cmlibs.utils.zinc.finiteelement import getMaximumNodeIdentifier
+from cmlibs.utils.zinc.general import ChangeManager
+from cmlibs.zinc.context import Context
+from cmlibs.zinc.field import Field, FieldFindMeshLocation, FieldFiniteElement
+from cmlibs.zinc.node import Node
+from cmlibs.zinc.optimisation import Optimisation
+from cmlibs.zinc.result import RESULT_OK, RESULT_WARNING_PART_DONE
 
 
 class Fitter:
     """
     Class for fitting fields on geometrically aligned scaffolds.
     """
 
@@ -902,17 +902,21 @@
         timesequence = self._getFieldTimesequence(field)
         if timesequence:
             timeCount = timesequence.getNumberOfTimes()
         else:
             timeCount = 1
 
         objectiveFormat = "{:12e}"
+
+        time = None
         start_epoch = None
+        fit_start_epoch = None
         if diagnostic_level_1:
             fit_start_epoch = timer()
+
         fieldcache = self._fieldmodule.createFieldcache()
         for timeIndex in range(1, timeCount + 1):
             if diagnostic_level_1:
                 start_epoch = timer()
             if timesequence:
                 time = timesequence.getTime(timeIndex)
                 optimisation.setAttributeReal(Optimisation.ATTRIBUTE_FIELD_PARAMETERS_TIME, time)
```

### Comparing `fieldfitter-0.2.0/src/fieldfitter.egg-info/PKG-INFO` & `fieldfitter-0.3.0/src/fieldfitter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: fieldfitter
-Version: 0.2.0
-Summary: Scaffold/model field fitting library using OpenCMISS-Zinc.
+Version: 0.3.0
+Summary: Scaffold/model field fitting library using Zinc.
 Home-page: https://github.com/ABI-Software/fieldfitter
 Author: Auckland Bioengineering Institute
 Author-email: r.christie@auckland.ac.nz
 License: Apache Software License
 Description: Field Fitter
         ============
         
-        Scaffold/model field fitting library using OpenCMISS-Zinc.
+        Scaffold/model field fitting library using Zinc.
         
         Takes as input a Zinc model file and a Zinc data file.
         Model requires a model coordinates field, and data a data coordinates field
         which are in the same aligned/fitted configuration.
         
         Additional fields defined on the data may be defined and fitted to a continuous field
         on the model or a subgroup of it. The fitted field is defined using the
```

