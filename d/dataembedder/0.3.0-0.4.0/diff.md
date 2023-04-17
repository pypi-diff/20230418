# Comparing `tmp/dataembedder-0.3.0.tar.gz` & `tmp/dataembedder-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataembedder-0.3.0.tar", last modified: Thu Feb  9 03:28:54 2023, max compression
+gzip compressed data, was "dataembedder-0.4.0.tar", last modified: Mon Apr 17 23:19:08 2023, max compression
```

## Comparing `dataembedder-0.3.0.tar` & `dataembedder-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-02-09 03:28:54.266552 dataembedder-0.3.0/
--rw-r--r--   0 hsor001  (1210695619) 1403514002      594 2022-07-26 04:05:51.000000 dataembedder-0.3.0/LICENSE
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1461 2023-02-09 03:28:54.266330 dataembedder-0.3.0/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002       94 2022-07-26 04:04:06.000000 dataembedder-0.3.0/README.rst
--rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2023-02-09 03:28:54.266655 dataembedder-0.3.0/setup.cfg
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1506 2023-02-09 03:28:26.000000 dataembedder-0.3.0/setup.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-02-09 03:28:54.262691 dataembedder-0.3.0/src/
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-02-09 03:28:54.263806 dataembedder-0.3.0/src/dataembedder/
--rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2021-11-01 11:07:44.000000 dataembedder-0.3.0/src/dataembedder/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    51784 2023-02-09 03:28:26.000000 dataembedder-0.3.0/src/dataembedder/dataembedder.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-02-09 03:28:54.265982 dataembedder-0.3.0/src/dataembedder.egg-info/
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1461 2023-02-09 03:28:54.000000 dataembedder-0.3.0/src/dataembedder.egg-info/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      327 2023-02-09 03:28:54.000000 dataembedder-0.3.0/src/dataembedder.egg-info/SOURCES.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-02-09 03:28:54.000000 dataembedder-0.3.0/src/dataembedder.egg-info/dependency_links.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2021-10-20 02:01:40.000000 dataembedder-0.3.0/src/dataembedder.egg-info/not-zip-safe
--rw-r--r--   0 hsor001  (1210695619) 1403514002       42 2023-02-09 03:28:54.000000 dataembedder-0.3.0/src/dataembedder.egg-info/requires.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002       13 2023-02-09 03:28:54.000000 dataembedder-0.3.0/src/dataembedder.egg-info/top_level.txt
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-17 23:19:08.493484 dataembedder-0.4.0/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      594 2022-07-26 04:05:51.000000 dataembedder-0.4.0/LICENSE
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1251 2023-04-17 23:19:08.493262 dataembedder-0.4.0/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       83 2023-04-17 23:06:27.000000 dataembedder-0.4.0/README.rst
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2023-04-17 23:19:08.493571 dataembedder-0.4.0/setup.cfg
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1475 2023-04-17 23:18:46.000000 dataembedder-0.4.0/setup.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-17 23:19:08.489351 dataembedder-0.4.0/src/
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-17 23:19:08.490852 dataembedder-0.4.0/src/dataembedder/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2021-11-01 11:07:44.000000 dataembedder-0.4.0/src/dataembedder/__init__.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    51763 2023-04-17 23:06:27.000000 dataembedder-0.4.0/src/dataembedder/dataembedder.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-17 23:19:08.492951 dataembedder-0.4.0/src/dataembedder.egg-info/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1251 2023-04-17 23:19:08.000000 dataembedder-0.4.0/src/dataembedder.egg-info/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      327 2023-04-17 23:19:08.000000 dataembedder-0.4.0/src/dataembedder.egg-info/SOURCES.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-17 23:19:08.000000 dataembedder-0.4.0/src/dataembedder.egg-info/dependency_links.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2021-10-20 02:01:40.000000 dataembedder-0.4.0/src/dataembedder.egg-info/not-zip-safe
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       25 2023-04-17 23:19:08.000000 dataembedder-0.4.0/src/dataembedder.egg-info/requires.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       13 2023-04-17 23:19:08.000000 dataembedder-0.4.0/src/dataembedder.egg-info/top_level.txt
```

### Comparing `dataembedder-0.3.0/LICENSE` & `dataembedder-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataembedder-0.3.0/PKG-INFO` & `dataembedder-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 Metadata-Version: 2.1
 Name: dataembedder
-Version: 0.3.0
-Summary: Python library for embedding data and models in anatomical scaffolds using OpenCMISS-Zinc
+Version: 0.4.0
+Summary: Python library for embedding data and models in anatomical scaffolds using Zinc
 Home-page: https://github.com/ABI-Software/dataembedder
 Author: Auckland Bioengineering Institute
 Author-email: r.christie@auckland.ac.nz
 License: Apache Software License
-Description: Data Embedder
-        =============
-        
-        Embeds data and meshes in a host scaffold using OpenCMISS-Zinc.
-        
-        
-        
-        License
-        =======
-        
-        ::
-        
-           Copyright 2022 University of Auckland
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Data Embedder
+=============
+
+Embeds data and meshes in a host scaffold using Zinc.
+
+
+License
+=======
+
+::
+
+   Copyright 2022 University of Auckland
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+
+
```

### Comparing `dataembedder-0.3.0/setup.py` & `dataembedder-0.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 
 
 readme = readfile("README.rst", split=True)
 # For requirements not hosted on PyPi place listings
 # into the 'requirements.txt' file.
 requires = [
     # minimal requirements listing
-    "opencmiss.utils >= 0.3",
-    "opencmiss.zinc >= 3.10"
+    "cmlibs.utils",
+    "cmlibs.zinc"
 ]
 readme.extend(['', 'License', '=======', '', '::', ''])
 source_license = readfile("LICENSE")
 
 setup(
     name="dataembedder",
-    version="0.3.0",
-    description="Python library for embedding data and models in anatomical scaffolds using OpenCMISS-Zinc",
+    version="0.4.0",
+    description="Python library for embedding data and models in anatomical scaffolds using Zinc",
     long_description="\n".join(readme) + source_license,
     long_description_content_type="text/x-rst",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python",
         "Topic :: Scientific/Engineering :: Medical Science Apps."
     ],
```

### Comparing `dataembedder-0.3.0/src/dataembedder/dataembedder.py` & `dataembedder-0.4.0/src/dataembedder/dataembedder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Main class for fitting scaffolds.
 """
 
 import json
 import sys
-from opencmiss.utils.zinc.field import get_group_list, get_unique_field_name
-from opencmiss.utils.zinc.general import ChangeManager, HierarchicalChangeManager
-from opencmiss.zinc.context import Context
-from opencmiss.zinc.element import Mesh, MeshGroup
-from opencmiss.zinc.field import Field, FieldFindMeshLocation, FieldFiniteElement, FieldGroup
-from opencmiss.zinc.region import Region
-from opencmiss.zinc.result import RESULT_ERROR_NOT_FOUND, RESULT_OK, RESULT_WARNING_PART_DONE
+from cmlibs.utils.zinc.field import get_group_list, get_unique_field_name
+from cmlibs.utils.zinc.general import ChangeManager, HierarchicalChangeManager
+from cmlibs.zinc.context import Context
+from cmlibs.zinc.element import Mesh, MeshGroup
+from cmlibs.zinc.field import Field, FieldFindMeshLocation, FieldFiniteElement, FieldGroup
+from cmlibs.zinc.region import Region
+from cmlibs.zinc.result import RESULT_ERROR_NOT_FOUND, RESULT_OK, RESULT_WARNING_PART_DONE
 
 
 class DataEmbedder:
 
     _embedToken = "embed"
     _dimensionToken = "dimension"
     _sizeToken = "size"
```

### Comparing `dataembedder-0.3.0/src/dataembedder.egg-info/PKG-INFO` & `dataembedder-0.4.0/src/dataembedder.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 Metadata-Version: 2.1
 Name: dataembedder
-Version: 0.3.0
-Summary: Python library for embedding data and models in anatomical scaffolds using OpenCMISS-Zinc
+Version: 0.4.0
+Summary: Python library for embedding data and models in anatomical scaffolds using Zinc
 Home-page: https://github.com/ABI-Software/dataembedder
 Author: Auckland Bioengineering Institute
 Author-email: r.christie@auckland.ac.nz
 License: Apache Software License
-Description: Data Embedder
-        =============
-        
-        Embeds data and meshes in a host scaffold using OpenCMISS-Zinc.
-        
-        
-        
-        License
-        =======
-        
-        ::
-        
-           Copyright 2022 University of Auckland
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Data Embedder
+=============
+
+Embeds data and meshes in a host scaffold using Zinc.
+
+
+License
+=======
+
+::
+
+   Copyright 2022 University of Auckland
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+
+
```

