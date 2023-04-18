# Comparing `tmp/drb-driver-http-1.2.0.tar.gz` & `tmp/drb-driver-http-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-http-1.2.0.tar", last modified: Fri Mar 31 09:43:09 2023, max compression
+gzip compressed data, was "drb-driver-http-1.2.1.tar", last modified: Tue Apr 18 08:20:51 2023, max compression
```

## Comparing `drb-driver-http-1.2.0.tar` & `drb-driver-http-1.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 09:43:09.985265 drb-driver-http-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 16:25:52.000000 drb-driver-http-1.2.0/LICENCE.txt
--rw-r--r--   0 root         (0) root         (0)     3844 2023-03-31 09:43:09.985265 drb-driver-http-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3391 2022-12-16 13:11:50.000000 drb-driver-http-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 09:43:09.961265 drb-driver-http-1.2.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 09:43:09.961265 drb-driver-http-1.2.0/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 09:43:09.989266 drb-driver-http-1.2.0/drb/drivers/http/
--rw-rw-rw-   0 root         (0) root         (0)      261 2022-12-16 13:11:50.000000 drb-driver-http-1.2.0/drb/drivers/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-03-31 09:43:09.989266 drb-driver-http-1.2.0/drb/drivers/http/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    14391 2023-03-31 09:29:41.000000 drb-driver-http-1.2.0/drb/drivers/http/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 09:43:09.965265 drb-driver-http-1.2.0/drb/drivers/http/oauth2/
--rw-rw-rw-   0 root         (0) root         (0)     1438 2022-12-16 13:11:50.000000 drb-driver-http-1.2.0/drb/drivers/http/oauth2/HTTPOAuth2.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-16 13:11:50.000000 drb-driver-http-1.2.0/drb/drivers/http/oauth2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3706 2022-12-19 13:27:28.000000 drb-driver-http-1.2.0/drb/drivers/http/oauth2/oauth2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 09:43:09.965265 drb-driver-http-1.2.0/drb/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)      311 2022-12-19 13:27:28.000000 drb-driver-http-1.2.0/drb/exceptions/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 09:43:09.961265 drb-driver-http-1.2.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 09:43:09.969265 drb-driver-http-1.2.0/drb/topics/http/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-16 13:11:50.000000 drb-driver-http-1.2.0/drb/topics/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-03-31 09:42:27.000000 drb-driver-http-1.2.0/drb/topics/http/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 09:43:09.969265 drb-driver-http-1.2.0/drb_driver_http.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3844 2023-03-31 09:43:09.000000 drb-driver-http-1.2.0/drb_driver_http.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      850 2023-03-31 09:43:09.000000 drb-driver-http-1.2.0/drb_driver_http.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 09:43:09.000000 drb-driver-http-1.2.0/drb_driver_http.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-03-31 09:43:09.000000 drb-driver-http-1.2.0/drb_driver_http.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 09:43:09.000000 drb-driver-http-1.2.0/drb_driver_http.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       27 2023-03-31 09:43:09.000000 drb-driver-http-1.2.0/drb_driver_http.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-31 09:43:09.000000 drb-driver-http-1.2.0/drb_driver_http.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-03-31 09:29:41.000000 drb-driver-http-1.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-03-31 09:29:41.000000 drb-driver-http-1.2.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-03-31 09:43:09.989266 drb-driver-http-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-03-31 09:29:41.000000 drb-driver-http-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 09:43:09.985265 drb-driver-http-1.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1520 2023-03-31 09:29:41.000000 drb-driver-http-1.2.0/tests/test_drb_http_basic_auth.py
--rw-rw-rw-   0 root         (0) root         (0)     3191 2023-03-31 09:29:41.000000 drb-driver-http-1.2.0/tests/test_drb_http_bearer.py
--rw-rw-rw-   0 root         (0) root         (0)      395 2022-12-16 13:11:50.000000 drb-driver-http-1.2.0/tests/test_drb_http_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1010 2023-03-31 09:29:41.000000 drb-driver-http-1.2.0/tests/test_drb_http_keyring.py
--rw-rw-rw-   0 root         (0) root         (0)     1463 2023-03-31 09:29:41.000000 drb-driver-http-1.2.0/tests/test_drb_http_signature.py
--rw-rw-rw-   0 root         (0) root         (0)     1755 2023-03-31 09:29:41.000000 drb-driver-http-1.2.0/tests/test_drb_https_signature.py
--rw-rw-rw-   0 root         (0) root         (0)     7409 2023-03-31 09:29:41.000000 drb-driver-http-1.2.0/tests/test_drb_impl_http.py
--rw-rw-rw-   0 root         (0) root         (0)    83607 2022-12-16 13:11:50.000000 drb-driver-http-1.2.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:20:51.578053 drb-driver-http-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 16:25:52.000000 drb-driver-http-1.2.1/LICENCE.txt
+-rw-r--r--   0 root         (0) root         (0)     3844 2023-04-18 08:20:51.578053 drb-driver-http-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3391 2022-12-16 13:11:50.000000 drb-driver-http-1.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:20:51.462051 drb-driver-http-1.2.1/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:20:51.458051 drb-driver-http-1.2.1/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:20:51.582053 drb-driver-http-1.2.1/drb/drivers/http/
+-rw-rw-rw-   0 root         (0) root         (0)      261 2022-12-16 13:11:50.000000 drb-driver-http-1.2.1/drb/drivers/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-04-18 08:20:51.582053 drb-driver-http-1.2.1/drb/drivers/http/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    14305 2023-04-14 09:23:27.000000 drb-driver-http-1.2.1/drb/drivers/http/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:20:51.486051 drb-driver-http-1.2.1/drb/drivers/http/oauth2/
+-rw-rw-rw-   0 root         (0) root         (0)     1438 2022-12-16 13:11:50.000000 drb-driver-http-1.2.1/drb/drivers/http/oauth2/HTTPOAuth2.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-16 13:11:50.000000 drb-driver-http-1.2.1/drb/drivers/http/oauth2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3706 2022-12-19 13:27:28.000000 drb-driver-http-1.2.1/drb/drivers/http/oauth2/oauth2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:20:51.486051 drb-driver-http-1.2.1/drb/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)      311 2022-12-19 13:27:28.000000 drb-driver-http-1.2.1/drb/exceptions/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:20:51.462051 drb-driver-http-1.2.1/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:20:51.490051 drb-driver-http-1.2.1/drb/topics/http/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-16 13:11:50.000000 drb-driver-http-1.2.1/drb/topics/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-04-18 08:20:07.000000 drb-driver-http-1.2.1/drb/topics/http/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:20:51.490051 drb-driver-http-1.2.1/drb_driver_http.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3844 2023-04-18 08:20:51.000000 drb-driver-http-1.2.1/drb_driver_http.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      850 2023-04-18 08:20:51.000000 drb-driver-http-1.2.1/drb_driver_http.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 08:20:51.000000 drb-driver-http-1.2.1/drb_driver_http.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-18 08:20:51.000000 drb-driver-http-1.2.1/drb_driver_http.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 08:20:51.000000 drb-driver-http-1.2.1/drb_driver_http.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-04-18 08:20:51.000000 drb-driver-http-1.2.1/drb_driver_http.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-18 08:20:51.000000 drb-driver-http-1.2.1/drb_driver_http.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-03-31 09:29:41.000000 drb-driver-http-1.2.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-03-31 09:29:41.000000 drb-driver-http-1.2.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-04-18 08:20:51.582053 drb-driver-http-1.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      141 2023-03-31 09:29:41.000000 drb-driver-http-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:20:51.578053 drb-driver-http-1.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1520 2023-03-31 09:29:41.000000 drb-driver-http-1.2.1/tests/test_drb_http_basic_auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     3191 2023-03-31 09:29:41.000000 drb-driver-http-1.2.1/tests/test_drb_http_bearer.py
+-rw-rw-rw-   0 root         (0) root         (0)      395 2022-12-16 13:11:50.000000 drb-driver-http-1.2.1/tests/test_drb_http_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-04-14 08:39:12.000000 drb-driver-http-1.2.1/tests/test_drb_http_keyring.py
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2023-03-31 09:29:41.000000 drb-driver-http-1.2.1/tests/test_drb_http_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     1755 2023-03-31 09:29:41.000000 drb-driver-http-1.2.1/tests/test_drb_https_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     7409 2023-03-31 09:29:41.000000 drb-driver-http-1.2.1/tests/test_drb_impl_http.py
+-rw-rw-rw-   0 root         (0) root         (0)    83607 2022-12-16 13:11:50.000000 drb-driver-http-1.2.1/versioneer.py
```

### Comparing `drb-driver-http-1.2.0/LICENCE.txt` & `drb-driver-http-1.2.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `drb-driver-http-1.2.0/PKG-INFO` & `drb-driver-http-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-driver-http
-Version: 1.2.0
+Version: 1.2.1
 Summary: DRB Http driver
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Project-URL: Documentation, http://drb-python.gitlab.io/impl/http
 Project-URL: Source, https://gitlab.com/drb-python/impl/http
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `drb-driver-http-1.2.0/README.md` & `drb-driver-http-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `drb-driver-http-1.2.0/drb/drivers/http/http.py` & `drb-driver-http-1.2.1/drb/drivers/http/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,26 +275,25 @@
     @deprecated(version='1.2.0',
                 reason='Only bracket browse should be use')
     def children(self) -> List[DrbNode]:
         return self._children
 
     @property
     def auth(self) -> AuthBase:
-        if self._auth is not None:
-            if isinstance(self._auth, HTTPBasicAuth):
-                credential = keyring.get_credential(
-                    self.path.path,
-                    self._auth.username
+        if self._auth is None:
+            credential = keyring.get_credential(
+                service_name=self.path.path,
+                username=None
+            )
+            if credential is not None:
+                self._auth = HTTPBasicAuth(
+                    credential.username,
+                    credential.password
                 )
-                if credential is not None:
-                    return HTTPBasicAuth(
-                        credential.username,
-                        credential.password
-                    )
-            return self._auth
+        return self._auth
 
     def __setitem__(self, key, value):
         raise NotImplementedError
 
     def __delitem__(self, key):
         raise NotImplementedError
```

### Comparing `drb-driver-http-1.2.0/drb/drivers/http/oauth2/HTTPOAuth2.py` & `drb-driver-http-1.2.1/drb/drivers/http/oauth2/HTTPOAuth2.py`

 * *Files identical despite different names*

### Comparing `drb-driver-http-1.2.0/drb/drivers/http/oauth2/oauth2.py` & `drb-driver-http-1.2.1/drb/drivers/http/oauth2/oauth2.py`

 * *Files identical despite different names*

### Comparing `drb-driver-http-1.2.0/drb_driver_http.egg-info/PKG-INFO` & `drb-driver-http-1.2.1/drb_driver_http.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-driver-http
-Version: 1.2.0
+Version: 1.2.1
 Summary: DRB Http driver
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Project-URL: Documentation, http://drb-python.gitlab.io/impl/http
 Project-URL: Source, https://gitlab.com/drb-python/impl/http
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `drb-driver-http-1.2.0/drb_driver_http.egg-info/SOURCES.txt` & `drb-driver-http-1.2.1/drb_driver_http.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drb-driver-http-1.2.0/setup.cfg` & `drb-driver-http-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `drb-driver-http-1.2.0/tests/test_drb_http_basic_auth.py` & `drb-driver-http-1.2.1/tests/test_drb_http_basic_auth.py`

 * *Files identical despite different names*

### Comparing `drb-driver-http-1.2.0/tests/test_drb_http_bearer.py` & `drb-driver-http-1.2.1/tests/test_drb_http_bearer.py`

 * *Files identical despite different names*

### Comparing `drb-driver-http-1.2.0/tests/test_drb_http_keyring.py` & `drb-driver-http-1.2.1/tests/test_drb_http_keyring.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import unittest
 import io
 from unittest.mock import patch
 from multiprocessing import Process
 
 from keyring.credentials import SimpleCredential
-from requests.auth import HTTPBasicAuth
 
 from drb.drivers.http import DrbHttpNode
 from tests.utility import start_auth_serve, PORT, PATH
 
 process = Process(target=start_auth_serve)
 
 
-def my_credential(usr, pwd):
+def my_credential(service_name, username):
     return SimpleCredential('user', 'pwd123456')
 
 
 class TestBitwardenKeyring(unittest.TestCase):
     url_ok = 'http://localhost:' + PORT + PATH + 'test.txt'
 
     @classmethod
@@ -25,11 +24,11 @@
 
     @classmethod
     def tearDownClass(cls) -> None:
         process.kill()
 
     @patch(target="keyring.get_credential", new=my_credential)
     def test_keyring_auth(self):
-        node = DrbHttpNode(path=self.url_ok, auth=HTTPBasicAuth('usr', 'pwd'))
+        node = DrbHttpNode(path=self.url_ok)
 
         self.assertEqual('{"path": "/resources/test.txt"}',
                          node.get_impl(io.BytesIO).getvalue().decode())
```

### Comparing `drb-driver-http-1.2.0/tests/test_drb_http_signature.py` & `drb-driver-http-1.2.1/tests/test_drb_http_signature.py`

 * *Files identical despite different names*

### Comparing `drb-driver-http-1.2.0/tests/test_drb_https_signature.py` & `drb-driver-http-1.2.1/tests/test_drb_https_signature.py`

 * *Files identical despite different names*

### Comparing `drb-driver-http-1.2.0/tests/test_drb_impl_http.py` & `drb-driver-http-1.2.1/tests/test_drb_impl_http.py`

 * *Files identical despite different names*

### Comparing `drb-driver-http-1.2.0/versioneer.py` & `drb-driver-http-1.2.1/versioneer.py`

 * *Files identical despite different names*

