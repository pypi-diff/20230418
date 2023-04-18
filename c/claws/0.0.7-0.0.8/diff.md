# Comparing `tmp/claws-0.0.7.tar.gz` & `tmp/claws-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claws-0.0.7.tar", last modified: Fri Mar 31 12:32:58 2023, max compression
+gzip compressed data, was "claws-0.0.8.tar", last modified: Tue Apr 18 11:37:23 2023, max compression
```

## Comparing `claws-0.0.7.tar` & `claws-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-03-31 12:32:58.112124 claws-0.0.7/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 claws-0.0.7/LICENSE.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     4386 2023-03-31 12:32:58.112124 claws-0.0.7/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     2550 2023-03-31 10:24:28.000000 claws-0.0.7/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     1055 2023-03-31 12:32:23.000000 claws-0.0.7/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)     1026 2023-03-31 12:32:58.112124 claws-0.0.7/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-03-31 12:32:58.112124 claws-0.0.7/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-03-31 12:32:58.112124 claws-0.0.7/src/claws/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-03-30 09:13:54.000000 claws-0.0.7/src/claws/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     9772 2023-03-31 12:31:08.000000 claws-0.0.7/src/claws/aws_utils.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-03-31 12:32:58.112124 claws-0.0.7/src/claws.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     4386 2023-03-31 12:32:58.000000 claws-0.0.7/src/claws.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      278 2023-03-31 12:32:58.000000 claws-0.0.7/src/claws.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-03-31 12:32:58.000000 claws-0.0.7/src/claws.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      170 2023-03-31 12:32:58.000000 claws-0.0.7/src/claws.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        6 2023-03-31 12:32:58.000000 claws-0.0.7/src/claws.egg-info/top_level.txt
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-03-31 12:32:58.112124 claws-0.0.7/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)     8596 2023-03-30 10:45:09.000000 claws-0.0.7/tests/test_aws_utils.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-18 11:37:23.665636 claws-0.0.8/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 claws-0.0.8/LICENSE.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4386 2023-04-18 11:37:23.665636 claws-0.0.8/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2550 2023-03-31 10:24:28.000000 claws-0.0.8/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1055 2023-04-18 11:37:04.000000 claws-0.0.8/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1026 2023-04-18 11:37:23.665636 claws-0.0.8/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-18 11:37:23.665636 claws-0.0.8/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-18 11:37:23.665636 claws-0.0.8/src/claws/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-03-30 09:13:54.000000 claws-0.0.8/src/claws/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10173 2023-04-18 11:35:52.000000 claws-0.0.8/src/claws/aws_utils.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-18 11:37:23.665636 claws-0.0.8/src/claws.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4386 2023-04-18 11:37:23.000000 claws-0.0.8/src/claws.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      278 2023-04-18 11:37:23.000000 claws-0.0.8/src/claws.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-04-18 11:37:23.000000 claws-0.0.8/src/claws.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      170 2023-04-18 11:37:23.000000 claws-0.0.8/src/claws.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        6 2023-04-18 11:37:23.000000 claws-0.0.8/src/claws.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-18 11:37:23.665636 claws-0.0.8/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8596 2023-03-30 10:45:09.000000 claws-0.0.8/tests/test_aws_utils.py
```

### Comparing `claws-0.0.7/LICENSE.md` & `claws-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `claws-0.0.7/PKG-INFO` & `claws-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claws
-Version: 0.0.7
+Version: 0.0.8
 Summary: The Crossref Labs AWS tooling system.
 Home-page: https://gitlab.com/crossref/labs/distrunner
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
```

### Comparing `claws-0.0.7/README.md` & `claws-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `claws-0.0.7/pyproject.toml` & `claws-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "claws"
-version = "0.0.7"
+version = "0.0.8"
 description = "The Crossref Labs AWS tooling system."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.md"}
 keywords = ["distributed computing"]
 authors = [
   {email = "meve@crossref.org"},
```

### Comparing `claws-0.0.7/setup.cfg` & `claws-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = claws
-version = 0.0.7
+version = 0.0.8
 description = The Crossref Labs AWS tooling system.
 url = https://gitlab.com/crossref/labs/distrunner
 author = Martin Paul Eve
 author_email = meve@crossref.org
 license = MIT
 classifiers = 
 	Intended Audience :: Developers
```

### Comparing `claws-0.0.7/src/claws/aws_utils.py` & `claws-0.0.8/src/claws/aws_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,18 +48,23 @@
         self._session = boto3.Session(
             aws_access_key_id=self._aws_access_key_id,
             aws_secret_access_key=self._aws_secret_access_key,
             aws_session_token=self._aws_session_token,
         )
 
         self._s3_client = (
-            self._session.client("s3", config=self.config)
+            self._session.client(
+                "s3",
+                config=(self.config if self._unsigned else self.signed_config),
+            )
             if not self._endpoint_url
             else boto3.client(
-                "s3", endpoint_url=self._endpoint_url, config=self.config
+                "s3",
+                endpoint_url=self._endpoint_url,
+                config=(self.config if self._unsigned else self.signed_config),
             )
         )
 
         self._cloudwatch_client = (
             self._session.client(
                 "cloudwatch",
                 config=self.signed_config,
@@ -82,18 +87,23 @@
                 "logs",
                 endpoint_url=self._endpoint_url,
                 config=self.signed_config,
             )
         )
 
         self._resource = (
-            self._session.resource("s3", config=self.config)
+            self._session.resource(
+                "s3",
+                config=(self.config if self._unsigned else self.signed_config),
+            )
             if not self._endpoint_url
             else self._session.resource(
-                "s3", endpoint_url=self._endpoint_url, config=self.config
+                "s3",
+                endpoint_url=self._endpoint_url,
+                config=(self.config if self._unsigned else self.signed_config),
             )
         )
 
         if self._bucket_name != "":
             self._bucket = self._resource.Bucket(self._bucket_name)
 
         self._done_init = True
@@ -101,14 +111,15 @@
     def __init__(
         self,
         endpoint_url: str = None,
         bucket: str = "",
         aws_access_key_id=None,
         aws_secret_access_key=None,
         aws_session_token=None,
+        unsigned: bool = True,
     ):
         self._done_init = False
         self._endpoint_url = endpoint_url
         self.config = None
         self._s3_client = None
         self._cloudwatch_client = None
         self._log_client = None
@@ -116,14 +127,15 @@
         self._resource = None
         self._bucket = None
         self._bucket_name = bucket
         self._instrumentation = None
         self._aws_access_key_id = aws_access_key_id
         self._aws_secret_access_key = aws_secret_access_key
         self._aws_session_token = aws_session_token
+        self._unsigned = unsigned
 
     @property
     def instrumentation(self):
         """
         Return the instrumentation/logging class
         :return: an Instrumentation class
         """
```

### Comparing `claws-0.0.7/src/claws.egg-info/PKG-INFO` & `claws-0.0.8/src/claws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claws
-Version: 0.0.7
+Version: 0.0.8
 Summary: The Crossref Labs AWS tooling system.
 Home-page: https://gitlab.com/crossref/labs/distrunner
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
```

### Comparing `claws-0.0.7/tests/test_aws_utils.py` & `claws-0.0.8/tests/test_aws_utils.py`

 * *Files identical despite different names*

