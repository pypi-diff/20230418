# Comparing `tmp/generic-crawler-sdk-0.1.8.tar.gz` & `tmp/generic-crawler-sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generic-crawler-sdk-0.1.8.tar", last modified: Fri Mar 24 16:10:34 2023, max compression
+gzip compressed data, was "generic-crawler-sdk-0.1.9.tar", last modified: Fri Mar 24 16:25:09 2023, max compression
```

## Comparing `generic-crawler-sdk-0.1.8.tar` & `generic-crawler-sdk-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)        0 2023-03-24 16:10:34.025033 generic-crawler-sdk-0.1.8/
--rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)        0 2022-07-25 09:38:29.000000 generic-crawler-sdk-0.1.8/LICENSE.txt
--rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)    11478 2023-03-24 16:10:34.024738 generic-crawler-sdk-0.1.8/PKG-INFO
--rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)    11050 2022-09-20 09:15:03.000000 generic-crawler-sdk-0.1.8/README.md
-drwxr-xr-x   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)        0 2023-03-24 16:10:34.022166 generic-crawler-sdk-0.1.8/generic_crawler/
--rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)        0 2022-06-03 16:39:50.000000 generic-crawler-sdk-0.1.8/generic_crawler/__init__.py
--rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)     2307 2023-03-13 21:10:34.000000 generic-crawler-sdk-0.1.8/generic_crawler/actions.py
--rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)      303 2022-08-15 11:22:00.000000 generic-crawler-sdk-0.1.8/generic_crawler/config.py
--rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)     3683 2023-03-24 16:10:15.000000 generic-crawler-sdk-0.1.8/generic_crawler/core.py
--rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)      781 2023-03-13 23:26:36.000000 generic-crawler-sdk-0.1.8/generic_crawler/sample.py
-drwxr-xr-x   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)        0 2023-03-24 16:10:34.024403 generic-crawler-sdk-0.1.8/generic_crawler_sdk.egg-info/
--rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)    11478 2023-03-24 16:10:33.000000 generic-crawler-sdk-0.1.8/generic_crawler_sdk.egg-info/PKG-INFO
--rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)      432 2023-03-24 16:10:33.000000 generic-crawler-sdk-0.1.8/generic_crawler_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)        1 2023-03-24 16:10:33.000000 generic-crawler-sdk-0.1.8/generic_crawler_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)        1 2022-06-06 20:03:49.000000 generic-crawler-sdk-0.1.8/generic_crawler_sdk.egg-info/not-zip-safe
--rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)      866 2023-03-24 16:10:33.000000 generic-crawler-sdk-0.1.8/generic_crawler_sdk.egg-info/requires.txt
--rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)       16 2023-03-24 16:10:33.000000 generic-crawler-sdk-0.1.8/generic_crawler_sdk.egg-info/top_level.txt
--rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)      214 2022-06-03 17:13:04.000000 generic-crawler-sdk-0.1.8/pyproject.toml
--rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)       38 2023-03-24 16:10:34.025081 generic-crawler-sdk-0.1.8/setup.cfg
--rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)     1154 2023-03-24 16:10:24.000000 generic-crawler-sdk-0.1.8/setup.py
+drwxr-xr-x   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)        0 2023-03-24 16:25:09.746238 generic-crawler-sdk-0.1.9/
+-rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)        0 2022-07-25 09:38:29.000000 generic-crawler-sdk-0.1.9/LICENSE.txt
+-rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)    11478 2023-03-24 16:25:09.745829 generic-crawler-sdk-0.1.9/PKG-INFO
+-rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)    11050 2022-09-20 09:15:03.000000 generic-crawler-sdk-0.1.9/README.md
+drwxr-xr-x   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)        0 2023-03-24 16:25:09.738143 generic-crawler-sdk-0.1.9/generic_crawler/
+-rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)        0 2022-06-03 16:39:50.000000 generic-crawler-sdk-0.1.9/generic_crawler/__init__.py
+-rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)     2307 2023-03-13 21:10:34.000000 generic-crawler-sdk-0.1.9/generic_crawler/actions.py
+-rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)      303 2022-08-15 11:22:00.000000 generic-crawler-sdk-0.1.9/generic_crawler/config.py
+-rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)     3727 2023-03-24 16:24:59.000000 generic-crawler-sdk-0.1.9/generic_crawler/core.py
+-rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)      781 2023-03-13 23:26:36.000000 generic-crawler-sdk-0.1.9/generic_crawler/sample.py
+drwxr-xr-x   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)        0 2023-03-24 16:25:09.745065 generic-crawler-sdk-0.1.9/generic_crawler_sdk.egg-info/
+-rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)    11478 2023-03-24 16:25:09.000000 generic-crawler-sdk-0.1.9/generic_crawler_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)      432 2023-03-24 16:25:09.000000 generic-crawler-sdk-0.1.9/generic_crawler_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)        1 2023-03-24 16:25:09.000000 generic-crawler-sdk-0.1.9/generic_crawler_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)        1 2022-06-06 20:03:49.000000 generic-crawler-sdk-0.1.9/generic_crawler_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)      866 2023-03-24 16:25:09.000000 generic-crawler-sdk-0.1.9/generic_crawler_sdk.egg-info/requires.txt
+-rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)       16 2023-03-24 16:25:09.000000 generic-crawler-sdk-0.1.9/generic_crawler_sdk.egg-info/top_level.txt
+-rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)      214 2022-06-03 17:13:04.000000 generic-crawler-sdk-0.1.9/pyproject.toml
+-rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)       38 2023-03-24 16:25:09.746282 generic-crawler-sdk-0.1.9/setup.cfg
+-rw-r--r--   0 tcudikel (1513964352) TURKCELL\Domain Users (1530679350)     1154 2023-03-24 16:25:02.000000 generic-crawler-sdk-0.1.9/setup.py
```

### Comparing `generic-crawler-sdk-0.1.8/PKG-INFO` & `generic-crawler-sdk-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generic-crawler-sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: Generic Crawler SDK
 Home-page: UNKNOWN
 Author: Umut Alihan Dikel
 Author-email: alihan.dikel@turkcell.com.tr
 License: UNKNOWN
 Keywords: generic_crawler
 Platform: UNKNOWN
```

### Comparing `generic-crawler-sdk-0.1.8/README.md` & `generic-crawler-sdk-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `generic-crawler-sdk-0.1.8/generic_crawler/actions.py` & `generic-crawler-sdk-0.1.9/generic_crawler/actions.py`

 * *Files identical despite different names*

### Comparing `generic-crawler-sdk-0.1.8/generic_crawler/core.py` & `generic-crawler-sdk-0.1.9/generic_crawler/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,16 +86,17 @@
 
 
 class FileHandler:
     def __init__(self):
         pass
 
     def write_to_local_filesystem(self, local_file_path, content):
+        bcontent = content.encode('utf-8')
         with open(f"{local_file_path}", 'wb') as f:
-            f.write(content)
+            f.write(bcontent)
         logger.success(f"file saved into: {local_file_path}")
 
     def upload_to_bucket(self):
         raise NotImplementedError
```

### Comparing `generic-crawler-sdk-0.1.8/generic_crawler/sample.py` & `generic-crawler-sdk-0.1.9/generic_crawler/sample.py`

 * *Files identical despite different names*

### Comparing `generic-crawler-sdk-0.1.8/generic_crawler_sdk.egg-info/PKG-INFO` & `generic-crawler-sdk-0.1.9/generic_crawler_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generic-crawler-sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: Generic Crawler SDK
 Home-page: UNKNOWN
 Author: Umut Alihan Dikel
 Author-email: alihan.dikel@turkcell.com.tr
 License: UNKNOWN
 Keywords: generic_crawler
 Platform: UNKNOWN
```

### Comparing `generic-crawler-sdk-0.1.8/generic_crawler_sdk.egg-info/requires.txt` & `generic-crawler-sdk-0.1.9/generic_crawler_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `generic-crawler-sdk-0.1.8/setup.py` & `generic-crawler-sdk-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 
 setuptools.setup(
     name="generic-crawler-sdk",
-    version="0.1.8",
+    version="0.1.9",
     author="Umut Alihan Dikel",
     author_email="alihan.dikel@turkcell.com.tr",
     description="Generic Crawler SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=None,
     packages=["generic_crawler"],
```

