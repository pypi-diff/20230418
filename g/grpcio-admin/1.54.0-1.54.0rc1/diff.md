# Comparing `tmp/grpcio-admin-1.54.0.tar.gz` & `tmp/grpcio-admin-1.54.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-admin-1.54.0.tar", last modified: Thu Apr 13 00:49:34 2023, max compression
+gzip compressed data, was "grpcio-admin-1.54.0rc1.tar", last modified: Fri Mar 31 21:34:26 2023, max compression
```

## Comparing `grpcio-admin-1.54.0.tar` & `grpcio-admin-1.54.0rc1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:49:34.447562 grpcio-admin-1.54.0/
--rw-r--r--   0 root         (0) root         (0)       95 2023-04-13 00:42:03.000000 grpcio-admin-1.54.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1315 2023-04-13 00:49:34.447562 grpcio-admin-1.54.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      865 2023-04-13 00:42:03.000000 grpcio-admin-1.54.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:49:34.447562 grpcio-admin-1.54.0/grpc_admin/
--rw-r--r--   0 root         (0) root         (0)     1621 2023-04-13 00:42:03.000000 grpcio-admin-1.54.0/grpc_admin/__init__.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-04-13 00:42:03.000000 grpcio-admin-1.54.0/grpc_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:49:34.447562 grpcio-admin-1.54.0/grpcio_admin.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1315 2023-04-13 00:49:34.000000 grpcio-admin-1.54.0/grpcio_admin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      274 2023-04-13 00:49:34.000000 grpcio-admin-1.54.0/grpcio_admin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 00:49:34.000000 grpcio-admin-1.54.0/grpcio_admin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-13 00:49:34.000000 grpcio-admin-1.54.0/grpcio_admin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-13 00:49:34.000000 grpcio-admin-1.54.0/grpcio_admin.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 00:49:34.447562 grpcio-admin-1.54.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2159 2023-04-13 00:42:03.000000 grpcio-admin-1.54.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 21:34:26.416456 grpcio-admin-1.54.0rc1/
+-rw-r--r--   0 root         (0) root         (0)       95 2023-03-31 21:09:23.000000 grpcio-admin-1.54.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-03-31 21:34:26.412455 grpcio-admin-1.54.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      865 2023-03-31 21:09:23.000000 grpcio-admin-1.54.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 21:34:26.412455 grpcio-admin-1.54.0rc1/grpc_admin/
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-03-31 21:09:23.000000 grpcio-admin-1.54.0rc1/grpc_admin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-03-31 21:09:23.000000 grpcio-admin-1.54.0rc1/grpc_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 21:34:26.412455 grpcio-admin-1.54.0rc1/grpcio_admin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-03-31 21:34:26.000000 grpcio-admin-1.54.0rc1/grpcio_admin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      274 2023-03-31 21:34:26.000000 grpcio-admin-1.54.0rc1/grpcio_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 21:34:26.000000 grpcio-admin-1.54.0rc1/grpcio_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-03-31 21:34:26.000000 grpcio-admin-1.54.0rc1/grpcio_admin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-03-31 21:34:26.000000 grpcio-admin-1.54.0rc1/grpcio_admin.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 21:34:26.416456 grpcio-admin-1.54.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2159 2023-03-31 21:09:23.000000 grpcio-admin-1.54.0rc1/setup.py
```

### Comparing `grpcio-admin-1.54.0/PKG-INFO` & `grpcio-admin-1.54.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-admin
-Version: 1.54.0
+Version: 1.54.0rc1
 Summary: a collection of admin services
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `grpcio-admin-1.54.0/README.rst` & `grpcio-admin-1.54.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `grpcio-admin-1.54.0/grpc_admin/__init__.py` & `grpcio-admin-1.54.0rc1/grpc_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-admin-1.54.0/grpc_version.py` & `grpcio-admin-1.54.0rc1/grpc_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # AUTO-GENERATED FROM `$REPO_ROOT/templates/src/python/grpcio_admin/grpc_version.py.template`!!!
 
-VERSION = '1.54.0'
+VERSION = '1.54.0rc1'
```

### Comparing `grpcio-admin-1.54.0/grpcio_admin.egg-info/PKG-INFO` & `grpcio-admin-1.54.0rc1/grpcio_admin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-admin
-Version: 1.54.0
+Version: 1.54.0rc1
 Summary: a collection of admin services
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `grpcio-admin-1.54.0/setup.py` & `grpcio-admin-1.54.0rc1/setup.py`

 * *Files identical despite different names*

