# Comparing `tmp/yopass_api-0.0.5.tar.gz` & `tmp/yopass_api-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yopass_api-0.0.5.tar", max compression
+gzip compressed data, was "yopass_api-0.0.6.tar", max compression
```

## Comparing `yopass_api-0.0.5.tar` & `yopass_api-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1096 2023-04-17 04:26:33.237964 yopass_api-0.0.5/LICENSE
--rw-r--r--   0        0        0     1039 2023-04-17 19:48:01.884801 yopass_api-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1018 2023-04-17 19:35:57.769174 yopass_api-0.0.5/README.md
--rw-r--r--   0        0        0       27 2023-04-17 04:26:33.238965 yopass_api-0.0.5/yopass_api/__init__.py
--rw-r--r--   0        0        0     5048 2023-04-17 17:57:13.344021 yopass_api-0.0.5/yopass_api/yopass_api.py
--rw-r--r--   0        0        0     2071 1970-01-01 00:00:00.000000 yopass_api-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-04-17 04:26:33.237964 yopass_api-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1039 2023-04-17 21:59:48.753648 yopass_api-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1082 2023-04-17 20:24:20.186363 yopass_api-0.0.6/README.md
+-rw-r--r--   0        0        0       27 2023-04-17 04:26:33.238965 yopass_api-0.0.6/yopass_api/__init__.py
+-rw-r--r--   0        0        0     5138 2023-04-17 21:55:38.544258 yopass_api-0.0.6/yopass_api/yopass_api.py
+-rw-r--r--   0        0        0     2134 1970-01-01 00:00:00.000000 yopass_api-0.0.6/PKG-INFO
```

### Comparing `yopass_api-0.0.5/LICENSE` & `yopass_api-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yopass_api-0.0.5/pyproject.toml` & `yopass_api-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yopass-api"
-version = "0.0.5"
+version = "0.0.6"
 description = "This module will allow you to use Python and Yopass in automation projects"
 license = "MIT"
 authors = ["Sergey Ilyashevich <silyashevich@gmail.com>"]
 maintainers = ["Sergey Ilyashevich <silyashevich@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/silyashevich/yopass_api"
 repository = "https://github.com/silyashevich/yopass_api"
```

### Comparing `yopass_api-0.0.5/README.md` & `yopass_api-0.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-[![codecov](https://codecov.io/github/silyashevich/yopass_api/branch/main/graph/badge.svg?token=YDY235VL6Q)](https://codecov.io/github/silyashevich/yopass_api)
-
 # yopass_api
 
+[![codecov](https://codecov.io/github/silyashevich/yopass_api/branch/main/graph/badge.svg?token=YDY235VL6Q)](https://codecov.io/github/silyashevich/yopass_api)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/yopass_api)
+
 This is a module to work with a (the) [Yopass](https://github.com/jhaals/yopass) backend created by [Johan Haals](https://github.com/jhaals).
 This module will allow you to use Python and self-hosted Yopass in automation projects.
 
 ## Installing
 
 ```py
 pip install yopass_api
```

### Comparing `yopass_api-0.0.5/yopass_api/yopass_api.py` & `yopass_api-0.0.6/yopass_api/yopass_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,13 +159,16 @@
         try:
             response = requests.get(
                 urljoin(self._api, f"/secret/{secret_id}"),
                 headers=headers,
                 timeout=self.timeout,
             )
             response.raise_for_status()
+        except requests.exceptions.RequestException as _:
+            return ""
+        try:
             secret = pgpy.PGPMessage.from_blob(response.json()["message"]).decrypt(
                 passphrase=password
             )
             return secret.message
-        except requests.exceptions.RequestException as _:
+        except pgpy.errors.PGPDecryptionError as _:
             return ""
```

### Comparing `yopass_api-0.0.5/PKG-INFO` & `yopass_api-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yopass-api
-Version: 0.0.5
+Version: 0.0.6
 Summary: This module will allow you to use Python and Yopass in automation projects
 Home-page: https://github.com/silyashevich/yopass_api
 License: MIT
 Keywords: api,cryptography,yopass
 Author: Sergey Ilyashevich
 Author-email: silyashevich@gmail.com
 Maintainer: Sergey Ilyashevich
@@ -21,18 +21,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Security :: Cryptography
 Requires-Dist: pgpy (>=0.6.0,<0.7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/silyashevich/yopass_api
 Description-Content-Type: text/markdown
 
-[![codecov](https://codecov.io/github/silyashevich/yopass_api/branch/main/graph/badge.svg?token=YDY235VL6Q)](https://codecov.io/github/silyashevich/yopass_api)
-
 # yopass_api
 
+[![codecov](https://codecov.io/github/silyashevich/yopass_api/branch/main/graph/badge.svg?token=YDY235VL6Q)](https://codecov.io/github/silyashevich/yopass_api)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/yopass_api)
+
 This is a module to work with a (the) [Yopass](https://github.com/jhaals/yopass) backend created by [Johan Haals](https://github.com/jhaals).
 This module will allow you to use Python and self-hosted Yopass in automation projects.
 
 ## Installing
 
 ```py
 pip install yopass_api
```

