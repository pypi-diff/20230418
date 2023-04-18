# Comparing `tmp/google-cloud-network-management-1.8.1.tar.gz` & `tmp/google-cloud-network-management-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-network-management-1.8.1.tar", last modified: Mon Mar 27 14:57:12 2023, max compression
+gzip compressed data, was "google-cloud-network-management-1.8.2.tar", last modified: Tue Apr 18 13:54:20 2023, max compression
```

## Comparing `google-cloud-network-management-1.8.1.tar` & `google-cloud-network-management-1.8.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:12.050427 google-cloud-network-management-1.8.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4733 2023-03-27 14:57:12.050427 google-cloud-network-management-1.8.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3784 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:12.042427 google-cloud-network-management-1.8.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:12.042427 google-cloud-network-management-1.8.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:12.042427 google-cloud-network-management-1.8.1/google/cloud/network_management/
--rw-rw-r--   0 root         (0)     1003     2621 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/google/cloud/network_management/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/google/cloud/network_management/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       92 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/google/cloud/network_management/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:12.042427 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/
--rw-rw-r--   0 root         (0)     1003     2370 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3205 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       92 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:12.046427 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:12.046427 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/reachability_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/reachability_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    41915 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/reachability_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    51661 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/reachability_service/client.py
--rw-rw-r--   0 root         (0)     1003     6105 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/reachability_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:12.046427 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/reachability_service/transports/
--rw-rw-r--   0 root         (0)     1003     1478 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/reachability_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8803 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/reachability_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    21371 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/reachability_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    21772 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/reachability_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    42143 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/reachability_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:12.046427 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/types/
--rw-rw-r--   0 root         (0)     1003     2042 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    12928 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/types/connectivity_test.py
--rw-rw-r--   0 root         (0)     1003     8907 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/types/reachability.py
--rw-rw-r--   0 root         (0)     1003    51873 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/google/cloud/network_management_v1/types/trace.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:12.046427 google-cloud-network-management-1.8.1/google_cloud_network_management.egg-info/
--rw-r--r--   0 root         (0)     1003     4733 2023-03-27 14:57:11.000000 google-cloud-network-management-1.8.1/google_cloud_network_management.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1980 2023-03-27 14:57:12.000000 google-cloud-network-management-1.8.1/google_cloud_network_management.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:57:11.000000 google-cloud-network-management-1.8.1/google_cloud_network_management.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:57:11.000000 google-cloud-network-management-1.8.1/google_cloud_network_management.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:57:11.000000 google-cloud-network-management-1.8.1/google_cloud_network_management.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 14:57:11.000000 google-cloud-network-management-1.8.1/google_cloud_network_management.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:57:11.000000 google-cloud-network-management-1.8.1/google_cloud_network_management.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 14:57:12.050427 google-cloud-network-management-1.8.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2971 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:12.046427 google-cloud-network-management-1.8.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:12.046427 google-cloud-network-management-1.8.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:12.050427 google-cloud-network-management-1.8.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:12.050427 google-cloud-network-management-1.8.1/tests/unit/gapic/network_management_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/tests/unit/gapic/network_management_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   216829 2023-03-27 14:54:37.000000 google-cloud-network-management-1.8.1/tests/unit/gapic/network_management_v1/test_reachability_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.864801 google-cloud-network-management-1.8.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4733 2023-04-18 13:54:20.864801 google-cloud-network-management-1.8.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3784 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.856801 google-cloud-network-management-1.8.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.856801 google-cloud-network-management-1.8.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.856801 google-cloud-network-management-1.8.2/google/cloud/network_management/
+-rw-rw-r--   0 root         (0)     1003     2621 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       92 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.856801 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/
+-rw-rw-r--   0 root         (0)     1003     2370 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3205 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       92 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.860801 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.860801 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    41915 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    51661 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6105 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.860801 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1478 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8803 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    21371 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    21772 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    42143 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.860801 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2042 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12903 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/types/connectivity_test.py
+-rw-rw-r--   0 root         (0)     1003     8907 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/types/reachability.py
+-rw-rw-r--   0 root         (0)     1003    51873 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/types/trace.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.860801 google-cloud-network-management-1.8.2/google_cloud_network_management.egg-info/
+-rw-r--r--   0 root         (0)     1003     4733 2023-04-18 13:54:20.000000 google-cloud-network-management-1.8.2/google_cloud_network_management.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1980 2023-04-18 13:54:20.000000 google-cloud-network-management-1.8.2/google_cloud_network_management.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-18 13:54:20.000000 google-cloud-network-management-1.8.2/google_cloud_network_management.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-04-18 13:54:20.000000 google-cloud-network-management-1.8.2/google_cloud_network_management.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-18 13:54:20.000000 google-cloud-network-management-1.8.2/google_cloud_network_management.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-04-18 13:54:20.000000 google-cloud-network-management-1.8.2/google_cloud_network_management.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-04-18 13:54:20.000000 google-cloud-network-management-1.8.2/google_cloud_network_management.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-04-18 13:54:20.864801 google-cloud-network-management-1.8.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2971 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.860801 google-cloud-network-management-1.8.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.860801 google-cloud-network-management-1.8.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.864801 google-cloud-network-management-1.8.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.864801 google-cloud-network-management-1.8.2/tests/unit/gapic/network_management_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/tests/unit/gapic/network_management_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   216829 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/tests/unit/gapic/network_management_v1/test_reachability_service.py
```

### Comparing `google-cloud-network-management-1.8.1/LICENSE` & `google-cloud-network-management-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/MANIFEST.in` & `google-cloud-network-management-1.8.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/PKG-INFO` & `google-cloud-network-management-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-network-management
-Version: 1.8.1
+Version: 1.8.2
 Summary: Google Cloud Network Management API client library
 Home-page: https://github.com/googleapis/python-network-management
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-network-management-1.8.1/README.rst` & `google-cloud-network-management-1.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/google/cloud/network_management/__init__.py` & `google-cloud-network-management-1.8.2/google/cloud/network_management/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/google/cloud/network_management/gapic_version.py` & `google-cloud-network-management-1.8.2/google/cloud/network_management/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.1"  # {x-release-please-version}
+__version__ = "1.8.2"  # {x-release-please-version}
```

### Comparing `google-cloud-network-management-1.8.1/google/cloud/network_management_v1/__init__.py` & `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/google/cloud/network_management_v1/gapic_metadata.json` & `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/google/cloud/network_management_v1/gapic_version.py` & `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.1"  # {x-release-please-version}
+__version__ = "1.8.2"  # {x-release-please-version}
```

### Comparing `google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/__init__.py` & `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/reachability_service/__init__.py` & `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/reachability_service/async_client.py` & `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/reachability_service/client.py` & `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/reachability_service/pagers.py` & `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/reachability_service/transports/__init__.py` & `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/reachability_service/transports/base.py` & `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/reachability_service/transports/grpc.py` & `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/reachability_service/transports/grpc_asyncio.py` & `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/google/cloud/network_management_v1/services/reachability_service/transports/rest.py` & `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/google/cloud/network_management_v1/types/__init__.py` & `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/google/cloud/network_management_v1/types/connectivity_test.py` & `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/types/connectivity_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,16 +201,16 @@
             the source.
         project_id (str):
             Project ID where the endpoint is located.
             The Project ID can be derived from the URI if
             you provide a VM instance or network URI.
             The following are two cases where you must
             provide the project ID: 1. Only the IP address
-            is specified, and the IP address is within a GCP
-            project.
+            is specified, and the IP address is within a
+            Google Cloud project.
             2. When you are using Shared VPC and the IP
             address that you provide is from the service
             project. In this case, the network that the IP
             address resides in is defined in the host
             project.
     """
 
@@ -218,22 +218,21 @@
         r"""The type definition of an endpoint's network. Use one of the
         following choices:
 
         Values:
             NETWORK_TYPE_UNSPECIFIED (0):
                 Default type if unspecified.
             GCP_NETWORK (1):
-                A network hosted within Google Cloud
-                Platform. To receive more detailed output,
-                specify the URI for the source or destination
-                network.
+                A network hosted within Google Cloud.
+                To receive more detailed output, specify the URI
+                for the source or destination network.
             NON_GCP_NETWORK (2):
-                A network hosted outside of Google Cloud
-                Platform. This can be an on-premises network, or
-                a network hosted by another cloud provider.
+                A network hosted outside of Google Cloud.
+                This can be an on-premises network, or a network
+                hosted by another cloud provider.
         """
         NETWORK_TYPE_UNSPECIFIED = 0
         GCP_NETWORK = 1
         NON_GCP_NETWORK = 2
 
     ip_address: str = proto.Field(
         proto.STRING,
```

### Comparing `google-cloud-network-management-1.8.1/google/cloud/network_management_v1/types/reachability.py` & `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/types/reachability.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/google/cloud/network_management_v1/types/trace.py` & `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/types/trace.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/google_cloud_network_management.egg-info/PKG-INFO` & `google-cloud-network-management-1.8.2/google_cloud_network_management.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-network-management
-Version: 1.8.1
+Version: 1.8.2
 Summary: Google Cloud Network Management API client library
 Home-page: https://github.com/googleapis/python-network-management
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-network-management-1.8.1/google_cloud_network_management.egg-info/SOURCES.txt` & `google-cloud-network-management-1.8.2/google_cloud_network_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/setup.py` & `google-cloud-network-management-1.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/tests/__init__.py` & `google-cloud-network-management-1.8.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/tests/unit/__init__.py` & `google-cloud-network-management-1.8.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/tests/unit/gapic/__init__.py` & `google-cloud-network-management-1.8.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/tests/unit/gapic/network_management_v1/__init__.py` & `google-cloud-network-management-1.8.2/tests/unit/gapic/network_management_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.1/tests/unit/gapic/network_management_v1/test_reachability_service.py` & `google-cloud-network-management-1.8.2/tests/unit/gapic/network_management_v1/test_reachability_service.py`

 * *Files identical despite different names*

