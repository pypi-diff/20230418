# Comparing `tmp/tencentcloud-sdk-python-tan-3.0.874.tar.gz` & `tmp/tencentcloud-sdk-python-tan-3.0.875.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tan-3.0.874.tar", last modified: Mon Apr 17 00:45:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tan-3.0.875.tar", last modified: Tue Apr 18 00:54:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tan-3.0.874.tar` & `tencentcloud-sdk-python-tan-3.0.875.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:45:57.000000 tencentcloud-sdk-python-tan-3.0.874/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-17 00:45:57.000000 tencentcloud-sdk-python-tan-3.0.874/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:45:57.000000 tencentcloud-sdk-python-tan-3.0.874/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:45:57.000000 tencentcloud-sdk-python-tan-3.0.874/tencentcloud/tan/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:45:57.000000 tencentcloud-sdk-python-tan-3.0.874/tencentcloud/tan/v20220420/
--rw-r--r--   0 root         (0) root         (0)     1892 2023-04-17 00:45:57.000000 tencentcloud-sdk-python-tan-3.0.874/tencentcloud/tan/v20220420/tan_client.py
--rw-r--r--   0 root         (0) root         (0)     2281 2023-04-17 00:45:57.000000 tencentcloud-sdk-python-tan-3.0.874/tencentcloud/tan/v20220420/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:45:57.000000 tencentcloud-sdk-python-tan-3.0.874/tencentcloud/tan/v20220420/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2285 2023-04-17 00:45:57.000000 tencentcloud-sdk-python-tan-3.0.874/tencentcloud/tan/v20220420/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:45:57.000000 tencentcloud-sdk-python-tan-3.0.874/tencentcloud/tan/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-17 00:45:57.000000 tencentcloud-sdk-python-tan-3.0.874/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:45:57.000000 tencentcloud-sdk-python-tan-3.0.874/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-17 00:45:57.000000 tencentcloud-sdk-python-tan-3.0.874/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-17 00:45:57.000000 tencentcloud-sdk-python-tan-3.0.874/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:45:57.000000 tencentcloud-sdk-python-tan-3.0.874/tencentcloud_sdk_python_tan.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 00:45:57.000000 tencentcloud-sdk-python-tan-3.0.874/tencentcloud_sdk_python_tan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-17 00:45:57.000000 tencentcloud-sdk-python-tan-3.0.874/tencentcloud_sdk_python_tan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:45:57.000000 tencentcloud-sdk-python-tan-3.0.874/tencentcloud_sdk_python_tan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-17 00:45:57.000000 tencentcloud-sdk-python-tan-3.0.874/tencentcloud_sdk_python_tan.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:54:07.000000 tencentcloud-sdk-python-tan-3.0.875/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-18 00:54:07.000000 tencentcloud-sdk-python-tan-3.0.875/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:54:07.000000 tencentcloud-sdk-python-tan-3.0.875/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:54:07.000000 tencentcloud-sdk-python-tan-3.0.875/tencentcloud/tan/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:54:07.000000 tencentcloud-sdk-python-tan-3.0.875/tencentcloud/tan/v20220420/
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-04-18 00:54:07.000000 tencentcloud-sdk-python-tan-3.0.875/tencentcloud/tan/v20220420/tan_client.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-04-18 00:54:07.000000 tencentcloud-sdk-python-tan-3.0.875/tencentcloud/tan/v20220420/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:54:07.000000 tencentcloud-sdk-python-tan-3.0.875/tencentcloud/tan/v20220420/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2285 2023-04-18 00:54:07.000000 tencentcloud-sdk-python-tan-3.0.875/tencentcloud/tan/v20220420/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:54:07.000000 tencentcloud-sdk-python-tan-3.0.875/tencentcloud/tan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-18 00:54:07.000000 tencentcloud-sdk-python-tan-3.0.875/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 00:54:07.000000 tencentcloud-sdk-python-tan-3.0.875/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-18 00:54:07.000000 tencentcloud-sdk-python-tan-3.0.875/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-18 00:54:07.000000 tencentcloud-sdk-python-tan-3.0.875/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:54:07.000000 tencentcloud-sdk-python-tan-3.0.875/tencentcloud_sdk_python_tan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 00:54:07.000000 tencentcloud-sdk-python-tan-3.0.875/tencentcloud_sdk_python_tan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-18 00:54:07.000000 tencentcloud-sdk-python-tan-3.0.875/tencentcloud_sdk_python_tan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 00:54:07.000000 tencentcloud-sdk-python-tan-3.0.875/tencentcloud_sdk_python_tan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 00:54:07.000000 tencentcloud-sdk-python-tan-3.0.875/tencentcloud_sdk_python_tan.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tan-3.0.874/README.rst` & `tencentcloud-sdk-python-tan-3.0.875/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tan-3.0.874/tencentcloud/tan/v20220420/tan_client.py` & `tencentcloud-sdk-python-tan-3.0.875/tencentcloud/tan/v20220420/tan_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tan-3.0.874/tencentcloud/tan/v20220420/errorcodes.py` & `tencentcloud-sdk-python-tan-3.0.875/tencentcloud/tan/v20220420/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tan-3.0.874/tencentcloud/tan/v20220420/models.py` & `tencentcloud-sdk-python-tan-3.0.875/tencentcloud/tan/v20220420/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tan-3.0.874/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tan-3.0.875/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.874'
+__version__ = '3.0.875'
```

### Comparing `tencentcloud-sdk-python-tan-3.0.874/PKG-INFO` & `tencentcloud-sdk-python-tan-3.0.875/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tan
-Version: 3.0.874
+Version: 3.0.875
 Summary: Tencent Cloud Tan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tan-3.0.874/setup.py` & `tencentcloud-sdk-python-tan-3.0.875/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tan-3.0.874/tencentcloud_sdk_python_tan.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tan-3.0.875/tencentcloud_sdk_python_tan.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tan
-Version: 3.0.874
+Version: 3.0.875
 Summary: Tencent Cloud Tan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

