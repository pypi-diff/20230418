# Comparing `tmp/aistore-1.2.0.tar.gz` & `tmp/aistore-1.2.1.tar.gz`

## Comparing `aistore-1.2.0.tar` & `aistore-1.2.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/client.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/common_requirements
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/botocore_patch/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/botocore_patch/__init__.py
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/botocore_patch/botocore.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/botocore_patch/botocore_requirements
--rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/pytorch/README.md
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/pytorch/__init__.py
--rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/pytorch/aisio.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/pytorch/dataset.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/pytorch/dev_requirements
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/pytorch/utils.py
--rw-r--r--   0        0        0     5511 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/README.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/__init__.py
--rw-r--r--   0        0        0    26239 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/bucket.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/client.py
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/cluster.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/const.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/errors.py
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/etl.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/etl_const.py
--rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/etl_templates.py
--rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/job.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/list_object_flag.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/namespace.py
--rw-r--r--   0        0        0     8204 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/object.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/object_attributes.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/object_iterator.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/object_reader.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/request_client.py
--rw-r--r--   0        0        0    10384 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/types.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/utils.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/multiobj/__init__.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/multiobj/object_collection.py
--rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/multiobj/object_group.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/multiobj/object_names.py
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/multiobj/object_range.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/multiobj/object_template.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 aistore-1.2.0/LICENSE
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 aistore-1.2.0/.gitignore
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 aistore-1.2.0/README.md
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 aistore-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 aistore-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/client.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/common_requirements
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/botocore_patch/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/botocore_patch/__init__.py
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/botocore_patch/botocore.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/botocore_patch/botocore_requirements
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/pytorch/README.md
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/pytorch/__init__.py
+-rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/pytorch/aisio.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/pytorch/dataset.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/pytorch/dev_requirements
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/pytorch/utils.py
+-rw-r--r--   0        0        0     5511 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/README.md
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/__init__.py
+-rw-r--r--   0        0        0    26239 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/bucket.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/client.py
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/cluster.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/const.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/errors.py
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/etl.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/etl_const.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/etl_templates.py
+-rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/job.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/list_object_flag.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/namespace.py
+-rw-r--r--   0        0        0     8204 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/object.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/object_attributes.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/object_iterator.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/object_reader.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/request_client.py
+-rw-r--r--   0        0        0    10384 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/types.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/utils.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/multiobj/__init__.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/multiobj/object_collection.py
+-rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/multiobj/object_group.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/multiobj/object_names.py
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/multiobj/object_range.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/multiobj/object_template.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 aistore-1.2.1/LICENSE
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 aistore-1.2.1/.gitignore
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 aistore-1.2.1/README.md
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 aistore-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 aistore-1.2.1/PKG-INFO
```

### Comparing `aistore-1.2.0/aistore/botocore_patch/README.md` & `aistore-1.2.1/aistore/botocore_patch/README.md`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/botocore_patch/botocore.py` & `aistore-1.2.1/aistore/botocore_patch/botocore.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/pytorch/README.md` & `aistore-1.2.1/aistore/pytorch/README.md`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/pytorch/aisio.py` & `aistore-1.2.1/aistore/pytorch/aisio.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/pytorch/dataset.py` & `aistore-1.2.1/aistore/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/pytorch/utils.py` & `aistore-1.2.1/aistore/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/README.md` & `aistore-1.2.1/aistore/sdk/README.md`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/bucket.py` & `aistore-1.2.1/aistore/sdk/bucket.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/client.py` & `aistore-1.2.1/aistore/sdk/client.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/cluster.py` & `aistore-1.2.1/aistore/sdk/cluster.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/const.py` & `aistore-1.2.1/aistore/sdk/const.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/errors.py` & `aistore-1.2.1/aistore/sdk/errors.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/etl.py` & `aistore-1.2.1/aistore/sdk/etl.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/etl_const.py` & `aistore-1.2.1/aistore/sdk/etl_const.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/etl_templates.py` & `aistore-1.2.1/aistore/sdk/etl_templates.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/job.py` & `aistore-1.2.1/aistore/sdk/job.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/list_object_flag.py` & `aistore-1.2.1/aistore/sdk/list_object_flag.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/object.py` & `aistore-1.2.1/aistore/sdk/object.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/object_attributes.py` & `aistore-1.2.1/aistore/sdk/object_attributes.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/object_iterator.py` & `aistore-1.2.1/aistore/sdk/object_iterator.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/object_reader.py` & `aistore-1.2.1/aistore/sdk/object_reader.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/request_client.py` & `aistore-1.2.1/aistore/sdk/request_client.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/types.py` & `aistore-1.2.1/aistore/sdk/types.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/utils.py` & `aistore-1.2.1/aistore/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/multiobj/object_collection.py` & `aistore-1.2.1/aistore/sdk/multiobj/object_collection.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/multiobj/object_group.py` & `aistore-1.2.1/aistore/sdk/multiobj/object_group.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/multiobj/object_names.py` & `aistore-1.2.1/aistore/sdk/multiobj/object_names.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/multiobj/object_range.py` & `aistore-1.2.1/aistore/sdk/multiobj/object_range.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/aistore/sdk/multiobj/object_template.py` & `aistore-1.2.1/aistore/sdk/multiobj/object_template.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/LICENSE` & `aistore-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/.gitignore` & `aistore-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aistore-1.2.0/pyproject.toml` & `aistore-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [tool.pytest.ini_options]
 markers = [
     "etl: marks tests as using etl and therefore requiring k8s cluster",
 ]
 
 [project]
 name = "aistore"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="AIStore Team", email="ais@exchange.nvidia.com" },
 ]
 description = "A (growing) set of client-side APIs to access and utilize clusters, buckets, and objects on AIStore."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT License"}
```

### Comparing `aistore-1.2.0/PKG-INFO` & `aistore-1.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aistore
-Version: 1.2.0
+Version: 1.2.1
 Summary: A (growing) set of client-side APIs to access and utilize clusters, buckets, and objects on AIStore.
 Project-URL: Homepage, https://aiatscale.org
 Project-URL: Download, https://github.com/NVIDIA/aistore/tags
 Project-URL: Documentation, https://aiatscale.org/docs/
 Project-URL: Release notes, https://github.com/NVIDIA/aistore/releases/
 Project-URL: Source, https://github.com/NVIDIA/aistore/
 Author-email: AIStore Team <ais@exchange.nvidia.com>
@@ -29,20 +29,20 @@
 Provides-Extra: pytorch
 Requires-Dist: torch; extra == 'pytorch'
 Requires-Dist: torchdata; extra == 'pytorch'
 Description-Content-Type: text/markdown
 
 ## AIS Python Components
 
-This directory includes the AIStore Python package containing the SDK, PyTorch integration, and Botocore patch. 
-See the README files in each directory in `aistore` for usage details.
+This package contains the AIStore Python SDK, PyTorch integration, and Botocore patch. 
+See the README files in each module for usage details:
 
-- [SDK](aistore/sdk/README.md)
-- [PyTorch](aistore/pytorch/README.md)
-- [Botocore](aistore/botocore_patch/README.md)
+- [SDK](https://github.com/NVIDIA/aistore/blob/master/python/aistore/sdk/README.md)
+- [PyTorch](https://github.com/NVIDIA/aistore/blob/master/python/aistore/pytorch/README.md)
+- [Botocore](https://github.com/NVIDIA/aistore/blob/master/python/aistore/botocore_patch/README.md)
 
 ## References
 
 * [AIStore GitHub](https://github.com/NVIDIA/aistore)
 * [Documentation](https://aiatscale.org/docs)
 * [AIStore pip package](https://pypi.org/project/aistore/)
 * [Videos and demos](https://github.com/NVIDIA/aistore/blob/master/docs/videos.md)
```

