# Comparing `tmp/garpix-auth-2.3.0.tar.gz` & `tmp/garpix-auth-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix-auth-2.3.0.tar", last modified: Mon Oct 18 14:34:39 2021, max compression
+gzip compressed data, was "garpix-auth-2.4.0.tar", last modified: Tue Apr 18 18:54:29 2023, max compression
```

## Comparing `garpix-auth-2.3.0.tar` & `garpix-auth-2.4.0.tar`

### file list

```diff
@@ -1,41 +1,62 @@
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-10-18 14:34:39.308266 garpix-auth-2.3.0/
--rw-r--r--   0 crusat     (501) staff       (20)       63 2021-10-18 14:34:38.000000 garpix-auth-2.3.0/MANIFEST.in
--rw-r--r--   0 crusat     (501) staff       (20)      645 2021-10-18 14:34:39.307021 garpix-auth-2.3.0/PKG-INFO
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-10-18 14:34:39.293916 garpix-auth-2.3.0/garpix_auth/
--rw-r--r--   0 crusat     (501) staff       (20)       63 2021-02-24 18:16:12.000000 garpix-auth-2.3.0/garpix_auth/MANIFEST.in
--rw-r--r--   0 crusat     (501) staff       (20)     3261 2021-05-29 18:35:14.000000 garpix-auth-2.3.0/garpix_auth/README.rst
--rw-r--r--   0 crusat     (501) staff       (20)        0 2021-02-24 18:16:12.000000 garpix-auth-2.3.0/garpix_auth/__init__.py
--rw-r--r--   0 crusat     (501) staff       (20)       96 2021-02-24 18:16:12.000000 garpix-auth-2.3.0/garpix_auth/apps.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-10-18 14:34:39.295134 garpix-auth-2.3.0/garpix_auth/forms/
--rw-r--r--   0 crusat     (501) staff       (20)       35 2021-06-16 18:31:18.000000 garpix-auth-2.3.0/garpix_auth/forms/__init__.py
--rw-r--r--   0 crusat     (501) staff       (20)      833 2021-06-16 18:31:18.000000 garpix-auth-2.3.0/garpix_auth/forms/login.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-10-18 14:34:39.296519 garpix-auth-2.3.0/garpix_auth/models/
--rw-r--r--   0 crusat     (501) staff       (20)      151 2021-10-07 20:43:00.000000 garpix-auth-2.3.0/garpix_auth/models/__init__.py
--rw-r--r--   0 crusat     (501) staff       (20)      880 2021-10-07 20:16:50.000000 garpix-auth-2.3.0/garpix_auth/models/access_token.py
--rw-r--r--   0 crusat     (501) staff       (20)      672 2021-10-07 20:43:00.000000 garpix-auth-2.3.0/garpix_auth/models/backend.py
--rw-r--r--   0 crusat     (501) staff       (20)      884 2021-10-07 20:16:50.000000 garpix-auth-2.3.0/garpix_auth/models/refresh_token.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-10-18 14:34:39.306531 garpix-auth-2.3.0/garpix_auth/rest/
--rw-r--r--   0 crusat     (501) staff       (20)     1277 2021-02-24 18:16:12.000000 garpix-auth-2.3.0/garpix_auth/rest/auth_token_serializer.py
--rw-r--r--   0 crusat     (501) staff       (20)     1609 2021-10-18 14:29:57.000000 garpix-auth-2.3.0/garpix_auth/rest/authentication.py
--rw-r--r--   0 crusat     (501) staff       (20)     1180 2021-10-07 21:12:40.000000 garpix-auth-2.3.0/garpix_auth/rest/logout_view.py
--rw-r--r--   0 crusat     (501) staff       (20)     1349 2021-10-07 21:10:03.000000 garpix-auth-2.3.0/garpix_auth/rest/obtain_auth_token.py
--rw-r--r--   0 crusat     (501) staff       (20)      219 2021-08-18 18:06:31.000000 garpix-auth-2.3.0/garpix_auth/rest/refresh_token_serializer.py
--rw-r--r--   0 crusat     (501) staff       (20)     1693 2021-10-07 21:09:28.000000 garpix-auth-2.3.0/garpix_auth/rest/refresh_token_view.py
--rw-r--r--   0 crusat     (501) staff       (20)      226 2021-10-07 20:55:44.000000 garpix-auth-2.3.0/garpix_auth/rest/utils.py
--rw-r--r--   0 crusat     (501) staff       (20)      938 2021-02-24 18:16:12.000000 garpix-auth-2.3.0/garpix_auth/settings.py
--rw-r--r--   0 crusat     (501) staff       (20)     1212 2021-10-18 14:33:44.000000 garpix-auth-2.3.0/garpix_auth/setup.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-10-18 14:34:39.306851 garpix-auth-2.3.0/garpix_auth/tests/
--rw-r--r--   0 crusat     (501) staff       (20)       89 2021-08-18 18:23:55.000000 garpix-auth-2.3.0/garpix_auth/tests/__init__.py
--rw-r--r--   0 crusat     (501) staff       (20)     6704 2021-10-07 21:11:56.000000 garpix-auth-2.3.0/garpix_auth/tests/test_api.py
--rw-r--r--   0 crusat     (501) staff       (20)     1277 2021-06-16 18:31:18.000000 garpix-auth-2.3.0/garpix_auth/tests/test_views.py
--rw-r--r--   0 crusat     (501) staff       (20)      405 2021-08-18 14:43:22.000000 garpix-auth-2.3.0/garpix_auth/urls.py
--rw-r--r--   0 crusat     (501) staff       (20)     1330 2021-06-16 18:31:18.000000 garpix-auth-2.3.0/garpix_auth/views.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-10-18 14:34:39.294936 garpix-auth-2.3.0/garpix_auth.egg-info/
--rw-r--r--   0 crusat     (501) staff       (20)      645 2021-10-18 14:34:39.000000 garpix-auth-2.3.0/garpix_auth.egg-info/PKG-INFO
--rw-r--r--   0 crusat     (501) staff       (20)      943 2021-10-18 14:34:39.000000 garpix-auth-2.3.0/garpix_auth.egg-info/SOURCES.txt
--rw-r--r--   0 crusat     (501) staff       (20)        1 2021-10-18 14:34:39.000000 garpix-auth-2.3.0/garpix_auth.egg-info/dependency_links.txt
--rw-r--r--   0 crusat     (501) staff       (20)        1 2021-10-18 14:34:39.000000 garpix-auth-2.3.0/garpix_auth.egg-info/not-zip-safe
--rw-r--r--   0 crusat     (501) staff       (20)      139 2021-10-18 14:34:39.000000 garpix-auth-2.3.0/garpix_auth.egg-info/requires.txt
--rw-r--r--   0 crusat     (501) staff       (20)       12 2021-10-18 14:34:39.000000 garpix-auth-2.3.0/garpix_auth.egg-info/top_level.txt
--rw-r--r--   0 crusat     (501) staff       (20)       38 2021-10-18 14:34:39.308314 garpix-auth-2.3.0/setup.cfg
--rw-r--r--   0 crusat     (501) staff       (20)     1212 2021-10-18 14:34:38.000000 garpix-auth-2.3.0/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 18:54:29.124585 garpix-auth-2.4.0/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2023-04-18 18:54:29.000000 garpix-auth-2.4.0/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      570 2023-04-18 18:54:29.124457 garpix-auth-2.4.0/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 18:54:29.120281 garpix-auth-2.4.0/garpix_auth/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2022-11-07 06:15:16.000000 garpix-auth-2.4.0/garpix_auth/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3261 2022-11-07 06:15:16.000000 garpix-auth-2.4.0/garpix_auth/README.rst
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-11-07 06:15:16.000000 garpix-auth-2.4.0/garpix_auth/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 18:54:29.121312 garpix-auth-2.4.0/garpix_auth/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      165 2022-11-07 06:17:48.000000 garpix-auth-2.4.0/garpix_auth/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      394 2022-11-07 06:17:48.000000 garpix-auth-2.4.0/garpix_auth/__pycache__/apps.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      551 2022-11-07 06:17:57.000000 garpix-auth-2.4.0/garpix_auth/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2058 2023-04-18 09:10:59.000000 garpix-auth-2.4.0/garpix_auth/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       96 2022-11-07 06:15:16.000000 garpix-auth-2.4.0/garpix_auth/apps.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 18:54:29.121514 garpix-auth-2.4.0/garpix_auth/forms/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       35 2022-11-07 06:15:16.000000 garpix-auth-2.4.0/garpix_auth/forms/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 18:54:29.121720 garpix-auth-2.4.0/garpix_auth/forms/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      210 2022-11-07 06:17:57.000000 garpix-auth-2.4.0/garpix_auth/forms/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1075 2023-04-18 08:33:37.000000 garpix-auth-2.4.0/garpix_auth/forms/__pycache__/login.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      833 2023-04-18 08:23:48.000000 garpix-auth-2.4.0/garpix_auth/forms/login.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 18:54:29.122124 garpix-auth-2.4.0/garpix_auth/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      151 2022-11-07 06:15:16.000000 garpix-auth-2.4.0/garpix_auth/models/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 18:54:29.122529 garpix-auth-2.4.0/garpix_auth/models/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      329 2022-11-07 06:17:48.000000 garpix-auth-2.4.0/garpix_auth/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1586 2023-04-18 08:33:36.000000 garpix-auth-2.4.0/garpix_auth/models/__pycache__/access_token.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1040 2022-11-07 06:17:48.000000 garpix-auth-2.4.0/garpix_auth/models/__pycache__/backend.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1595 2023-04-18 08:33:36.000000 garpix-auth-2.4.0/garpix_auth/models/__pycache__/refresh_token.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      880 2022-11-07 07:45:42.000000 garpix-auth-2.4.0/garpix_auth/models/access_token.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      672 2022-11-07 06:15:16.000000 garpix-auth-2.4.0/garpix_auth/models/backend.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      884 2022-11-07 07:45:42.000000 garpix-auth-2.4.0/garpix_auth/models/refresh_token.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 18:54:29.123245 garpix-auth-2.4.0/garpix_auth/rest/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 18:54:29.123985 garpix-auth-2.4.0/garpix_auth/rest/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1218 2022-11-07 06:17:57.000000 garpix-auth-2.4.0/garpix_auth/rest/__pycache__/auth_token_serializer.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1620 2022-11-07 06:17:57.000000 garpix-auth-2.4.0/garpix_auth/rest/__pycache__/authentication.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1396 2022-11-07 06:17:57.000000 garpix-auth-2.4.0/garpix_auth/rest/__pycache__/logout_view.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1586 2023-04-18 09:09:39.000000 garpix-auth-2.4.0/garpix_auth/rest/__pycache__/obtain_auth_token.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      562 2022-11-07 06:17:57.000000 garpix-auth-2.4.0/garpix_auth/rest/__pycache__/refresh_token_serializer.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1839 2022-11-07 06:17:57.000000 garpix-auth-2.4.0/garpix_auth/rest/__pycache__/refresh_token_view.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      521 2023-04-18 18:54:28.000000 garpix-auth-2.4.0/garpix_auth/rest/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1277 2022-11-07 06:15:16.000000 garpix-auth-2.4.0/garpix_auth/rest/auth_token_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1609 2022-11-07 06:15:16.000000 garpix-auth-2.4.0/garpix_auth/rest/authentication.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1180 2022-11-07 06:15:16.000000 garpix-auth-2.4.0/garpix_auth/rest/logout_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1349 2023-04-18 09:09:38.000000 garpix-auth-2.4.0/garpix_auth/rest/obtain_auth_token.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      219 2022-11-07 06:15:16.000000 garpix-auth-2.4.0/garpix_auth/rest/refresh_token_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1693 2022-11-07 06:15:16.000000 garpix-auth-2.4.0/garpix_auth/rest/refresh_token_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      328 2023-04-18 18:54:06.000000 garpix-auth-2.4.0/garpix_auth/rest/utils.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      938 2022-11-07 06:15:16.000000 garpix-auth-2.4.0/garpix_auth/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1212 2023-04-18 18:54:06.000000 garpix-auth-2.4.0/garpix_auth/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 18:54:29.124293 garpix-auth-2.4.0/garpix_auth/tests/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       89 2022-11-07 06:15:16.000000 garpix-auth-2.4.0/garpix_auth/tests/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6704 2022-11-07 06:15:16.000000 garpix-auth-2.4.0/garpix_auth/tests/test_api.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1277 2022-11-07 06:15:16.000000 garpix-auth-2.4.0/garpix_auth/tests/test_views.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      405 2022-11-07 06:15:16.000000 garpix-auth-2.4.0/garpix_auth/urls.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1330 2023-04-18 09:10:58.000000 garpix-auth-2.4.0/garpix_auth/views.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 18:54:29.120895 garpix-auth-2.4.0/garpix_auth.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      570 2023-04-18 18:54:29.000000 garpix-auth-2.4.0/garpix_auth.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1882 2023-04-18 18:54:29.000000 garpix-auth-2.4.0/garpix_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-04-18 18:54:29.000000 garpix-auth-2.4.0/garpix_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-04-18 18:54:29.000000 garpix-auth-2.4.0/garpix_auth.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      139 2023-04-18 18:54:29.000000 garpix-auth-2.4.0/garpix_auth.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       12 2023-04-18 18:54:29.000000 garpix-auth-2.4.0/garpix_auth.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-04-18 18:54:29.124625 garpix-auth-2.4.0/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1212 2023-04-18 18:54:29.000000 garpix-auth-2.4.0/setup.py
```

### Comparing `garpix-auth-2.3.0/PKG-INFO` & `garpix-auth-2.4.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: garpix-auth
-Version: 2.3.0
-Summary: UNKNOWN
-Home-page: UNKNOWN
+Version: 2.4.0
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
```

### Comparing `garpix-auth-2.3.0/garpix_auth/README.rst` & `garpix-auth-2.4.0/garpix_auth/README.rst`

 * *Files identical despite different names*

### Comparing `garpix-auth-2.3.0/garpix_auth/forms/login.py` & `garpix-auth-2.4.0/garpix_auth/forms/login.py`

 * *Files identical despite different names*

### Comparing `garpix-auth-2.3.0/garpix_auth/models/access_token.py` & `garpix-auth-2.4.0/garpix_auth/models/access_token.py`

 * *Files identical despite different names*

### Comparing `garpix-auth-2.3.0/garpix_auth/models/backend.py` & `garpix-auth-2.4.0/garpix_auth/models/backend.py`

 * *Files identical despite different names*

### Comparing `garpix-auth-2.3.0/garpix_auth/models/refresh_token.py` & `garpix-auth-2.4.0/garpix_auth/models/refresh_token.py`

 * *Files identical despite different names*

### Comparing `garpix-auth-2.3.0/garpix_auth/rest/auth_token_serializer.py` & `garpix-auth-2.4.0/garpix_auth/rest/auth_token_serializer.py`

 * *Files identical despite different names*

### Comparing `garpix-auth-2.3.0/garpix_auth/rest/authentication.py` & `garpix-auth-2.4.0/garpix_auth/rest/authentication.py`

 * *Files identical despite different names*

### Comparing `garpix-auth-2.3.0/garpix_auth/rest/logout_view.py` & `garpix-auth-2.4.0/garpix_auth/rest/logout_view.py`

 * *Files identical despite different names*

### Comparing `garpix-auth-2.3.0/garpix_auth/rest/obtain_auth_token.py` & `garpix-auth-2.4.0/garpix_auth/rest/obtain_auth_token.py`

 * *Files identical despite different names*

### Comparing `garpix-auth-2.3.0/garpix_auth/rest/refresh_token_view.py` & `garpix-auth-2.4.0/garpix_auth/rest/refresh_token_view.py`

 * *Files identical despite different names*

### Comparing `garpix-auth-2.3.0/garpix_auth/settings.py` & `garpix-auth-2.4.0/garpix_auth/settings.py`

 * *Files identical despite different names*

### Comparing `garpix-auth-2.3.0/garpix_auth/setup.py` & `garpix-auth-2.4.0/garpix_auth/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_auth')
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix-auth',
-    version='2.3.0',
+    version='2.4.0',
     description='',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
     packages=find_packages(exclude=['testproject', 'testproject.*']),
     classifiers=[
         'Development Status :: 4 - Beta',
```

### Comparing `garpix-auth-2.3.0/garpix_auth/tests/test_api.py` & `garpix-auth-2.4.0/garpix_auth/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `garpix-auth-2.3.0/garpix_auth/tests/test_views.py` & `garpix-auth-2.4.0/garpix_auth/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `garpix-auth-2.3.0/garpix_auth/views.py` & `garpix-auth-2.4.0/garpix_auth/views.py`

 * *Files identical despite different names*

### Comparing `garpix-auth-2.3.0/garpix_auth.egg-info/PKG-INFO` & `garpix-auth-2.4.0/garpix_auth.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: garpix-auth
-Version: 2.3.0
-Summary: UNKNOWN
-Home-page: UNKNOWN
+Version: 2.4.0
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
```

### Comparing `garpix-auth-2.3.0/setup.py` & `garpix-auth-2.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_auth')
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix-auth',
-    version='2.3.0',
+    version='2.4.0',
     description='',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
     packages=find_packages(exclude=['testproject', 'testproject.*']),
     classifiers=[
         'Development Status :: 4 - Beta',
```

