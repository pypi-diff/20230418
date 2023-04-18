# Comparing `tmp/prelude-sdk-0.9.97.tar.gz` & `tmp/prelude-sdk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-sdk-0.9.97.tar", last modified: Thu Apr 13 13:53:41 2023, max compression
+gzip compressed data, was "prelude-sdk-1.0.0.tar", last modified: Tue Apr 18 19:09:01 2023, max compression
```

## Comparing `prelude-sdk-0.9.97.tar` & `prelude-sdk-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:53:41.074432 prelude-sdk-0.9.97/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-0.9.97/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)     1140 2023-04-13 13:53:41.074494 prelude-sdk-0.9.97/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-0.9.97/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:53:41.069660 prelude-sdk-0.9.97/prelude_sdk/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-0.9.97/prelude_sdk/__init__.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:53:41.071733 prelude-sdk-0.9.97/prelude_sdk/controllers/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-0.9.97/prelude_sdk/controllers/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     3363 2023-04-07 19:23:14.000000 prelude-sdk-0.9.97/prelude_sdk/controllers/build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     6538 2023-04-13 13:44:46.000000 prelude-sdk-0.9.97/prelude_sdk/controllers/detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     4663 2023-04-13 13:44:46.000000 prelude-sdk-0.9.97/prelude_sdk/controllers/iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     1353 2023-04-11 22:16:02.000000 prelude-sdk-0.9.97/prelude_sdk/controllers/partner_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      540 2023-04-07 19:23:14.000000 prelude-sdk-0.9.97/prelude_sdk/controllers/probe_controller.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:53:41.072236 prelude-sdk-0.9.97/prelude_sdk/models/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-0.9.97/prelude_sdk/models/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2816 2023-04-07 19:23:14.000000 prelude-sdk-0.9.97/prelude_sdk/models/account.py
--rw-r--r--   0 pack       (501) staff       (20)     2609 2023-04-08 00:28:18.000000 prelude-sdk-0.9.97/prelude_sdk/models/codes.py
--rw-r--r--   0 pack       (501) staff       (20)      867 2023-03-09 20:15:21.000000 prelude-sdk-0.9.97/prelude_sdk/spinner.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:53:41.070470 prelude-sdk-0.9.97/prelude_sdk.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)     1140 2023-04-13 13:53:41.000000 prelude-sdk-0.9.97/prelude_sdk.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      796 2023-04-13 13:53:41.000000 prelude-sdk-0.9.97/prelude_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-04-13 13:53:41.000000 prelude-sdk-0.9.97/prelude_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)        9 2023-04-13 13:53:41.000000 prelude-sdk-0.9.97/prelude_sdk.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       18 2023-04-13 13:53:41.000000 prelude-sdk-0.9.97/prelude_sdk.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-0.9.97/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      533 2023-04-13 13:53:41.074722 prelude-sdk-0.9.97/setup.cfg
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:53:41.074123 prelude-sdk-0.9.97/tests/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-0.9.97/tests/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1101 2023-04-11 22:16:02.000000 prelude-sdk-0.9.97/tests/conftest.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:53:41.074344 prelude-sdk-0.9.97/tests/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-0.9.97/tests/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2658 2023-04-11 22:16:02.000000 prelude-sdk-0.9.97/tests/test_build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     4386 2023-04-11 22:16:02.000000 prelude-sdk-0.9.97/tests/test_detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3885 2023-04-13 13:44:46.000000 prelude-sdk-0.9.97/tests/test_iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-0.9.97/tests/test_probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-18 19:09:01.496272 prelude-sdk-1.0.0/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.0.0/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-04-18 19:09:01.496329 prelude-sdk-1.0.0/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.0.0/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-18 19:09:01.491630 prelude-sdk-1.0.0/prelude_sdk/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.0.0/prelude_sdk/__init__.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-18 19:09:01.494059 prelude-sdk-1.0.0/prelude_sdk/controllers/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.0.0/prelude_sdk/controllers/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     3363 2023-04-07 19:23:14.000000 prelude-sdk-1.0.0/prelude_sdk/controllers/build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     6594 2023-04-18 17:04:09.000000 prelude-sdk-1.0.0/prelude_sdk/controllers/detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     4663 2023-04-13 13:44:46.000000 prelude-sdk-1.0.0/prelude_sdk/controllers/iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     1353 2023-04-11 22:16:02.000000 prelude-sdk-1.0.0/prelude_sdk/controllers/partner_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      540 2023-04-07 19:23:14.000000 prelude-sdk-1.0.0/prelude_sdk/controllers/probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-18 19:09:01.494564 prelude-sdk-1.0.0/prelude_sdk/models/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.0.0/prelude_sdk/models/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2816 2023-04-07 19:23:14.000000 prelude-sdk-1.0.0/prelude_sdk/models/account.py
+-rw-r--r--   0 pack       (501) staff       (20)     2609 2023-04-08 00:28:18.000000 prelude-sdk-1.0.0/prelude_sdk/models/codes.py
+-rw-r--r--   0 pack       (501) staff       (20)      867 2023-03-09 20:15:21.000000 prelude-sdk-1.0.0/prelude_sdk/spinner.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-18 19:09:01.492569 prelude-sdk-1.0.0/prelude_sdk.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-04-18 19:09:01.000000 prelude-sdk-1.0.0/prelude_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      796 2023-04-18 19:09:01.000000 prelude-sdk-1.0.0/prelude_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-04-18 19:09:01.000000 prelude-sdk-1.0.0/prelude_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)        9 2023-04-18 19:09:01.000000 prelude-sdk-1.0.0/prelude_sdk.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       18 2023-04-18 19:09:01.000000 prelude-sdk-1.0.0/prelude_sdk.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.0.0/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      532 2023-04-18 19:09:01.496538 prelude-sdk-1.0.0/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-18 19:09:01.495991 prelude-sdk-1.0.0/tests/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.0.0/tests/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1101 2023-04-11 22:16:02.000000 prelude-sdk-1.0.0/tests/conftest.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-18 19:09:01.496196 prelude-sdk-1.0.0/tests/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.0.0/tests/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2658 2023-04-11 22:16:02.000000 prelude-sdk-1.0.0/tests/test_build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     4402 2023-04-18 17:04:09.000000 prelude-sdk-1.0.0/tests/test_detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3885 2023-04-13 13:44:46.000000 prelude-sdk-1.0.0/tests/test_iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-1.0.0/tests/test_probe_controller.py
```

### Comparing `prelude-sdk-0.9.97/LICENSE` & `prelude-sdk-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-sdk-0.9.97/PKG-INFO` & `prelude-sdk-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 0.9.97
+Version: 1.0.0
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-0.9.97/README.md` & `prelude-sdk-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `prelude-sdk-0.9.97/prelude_sdk/controllers/build_controller.py` & `prelude-sdk-1.0.0/prelude_sdk/controllers/build_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-0.9.97/prelude_sdk/controllers/detect_controller.py` & `prelude-sdk-1.0.0/prelude_sdk/controllers/detect_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,20 +105,21 @@
                 json=dict(code=run_code, tags=tags),
                 timeout=10
             )
             if res.status_code != 200:
                 raise Exception(res.text)
 
     @verify_credentials
-    def disable_test(self, ident):
+    def disable_test(self, ident: str, tags: str):
         """ Disable a test so endpoints will stop running it """
         with Spinner():
             res = requests.delete(
                 f'{self.account.hq}/detect/queue/{ident}',
                 headers=self.account.headers,
+                params=dict(tags=tags),
                 timeout=10
             )
             if res.status_code != 200:
                 raise Exception(res.text)
 
     @verify_credentials
     def social_stats(self, ident: str, days: int = 30):
```

### Comparing `prelude-sdk-0.9.97/prelude_sdk/controllers/iam_controller.py` & `prelude-sdk-1.0.0/prelude_sdk/controllers/iam_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-0.9.97/prelude_sdk/controllers/partner_controller.py` & `prelude-sdk-1.0.0/prelude_sdk/controllers/partner_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-0.9.97/prelude_sdk/controllers/probe_controller.py` & `prelude-sdk-1.0.0/prelude_sdk/controllers/probe_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-0.9.97/prelude_sdk/models/account.py` & `prelude-sdk-1.0.0/prelude_sdk/models/account.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-0.9.97/prelude_sdk/models/codes.py` & `prelude-sdk-1.0.0/prelude_sdk/models/codes.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-0.9.97/prelude_sdk/spinner.py` & `prelude-sdk-1.0.0/prelude_sdk/spinner.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-0.9.97/prelude_sdk.egg-info/PKG-INFO` & `prelude-sdk-1.0.0/prelude_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 0.9.97
+Version: 1.0.0
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-0.9.97/prelude_sdk.egg-info/SOURCES.txt` & `prelude-sdk-1.0.0/prelude_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-sdk-0.9.97/setup.cfg` & `prelude-sdk-1.0.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-sdk
-version = 0.9.97
+version = 1.0.0
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers =
```

### Comparing `prelude-sdk-0.9.97/tests/conftest.py` & `prelude-sdk-1.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-0.9.97/tests/test_build_controller.py` & `prelude-sdk-1.0.0/tests/test_build_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-0.9.97/tests/test_detect_controller.py` & `prelude-sdk-1.0.0/tests/test_detect_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             describe_activity = unwrap(self.detect.describe_activity)(self.detect, filters={'endpoint_id': pytest.endpoint_id})
             assert len(describe_activity) == 2
         finally:
             os.remove(pytest.probe)
 
     def test_disable_test(self, unwrap):
         """Test disable_test method"""
-        unwrap(self.detect.disable_test)(self.detect, ident=pytest.test_id)
+        unwrap(self.detect.disable_test)(self.detect, ident=pytest.test_id, tags=self.tags)
         res = unwrap(self.detect.list_queue)(self.detect)
         assert len([test for test in res if test['test'] == pytest.test_id]) == 0
 
     def test_social_stats(self, unwrap):
         """Test social_stats method"""
         res = unwrap(self.detect.social_stats)(self.detect, ident=pytest.test_id)
         assert len(res.values()) >= 1
```

### Comparing `prelude-sdk-0.9.97/tests/test_iam_controller.py` & `prelude-sdk-1.0.0/tests/test_iam_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-0.9.97/tests/test_probe_controller.py` & `prelude-sdk-1.0.0/tests/test_probe_controller.py`

 * *Files identical despite different names*

