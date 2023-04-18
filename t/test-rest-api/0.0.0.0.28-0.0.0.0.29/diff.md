# Comparing `tmp/test_rest_api-0.0.0.0.28.tar.gz` & `tmp/test_rest_api-0.0.0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_rest_api-0.0.0.0.28.tar", last modified: Tue Apr 18 06:20:55 2023, max compression
+gzip compressed data, was "test_rest_api-0.0.0.0.29.tar", last modified: Tue Apr 18 08:16:46 2023, max compression
```

## Comparing `test_rest_api-0.0.0.0.28.tar` & `test_rest_api-0.0.0.0.29.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 06:20:55.739021 test_rest_api-0.0.0.0.28/
--rw-r--r--   0 trjose     (501) staff       (20)     1067 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.28/LICENSE
--rw-r--r--   0 trjose     (501) staff       (20)    64005 2023-04-18 06:20:55.738514 test_rest_api-0.0.0.0.28/PKG-INFO
--rw-r--r--   0 trjose     (501) staff       (20)    62282 2023-04-14 16:15:06.000000 test_rest_api-0.0.0.0.28/README.md
--rw-r--r--   0 trjose     (501) staff       (20)       38 2023-04-18 06:20:55.739166 test_rest_api-0.0.0.0.28/setup.cfg
--rw-r--r--   0 trjose     (501) staff       (20)     2893 2023-04-18 06:20:41.000000 test_rest_api-0.0.0.0.28/setup.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 06:20:55.714803 test_rest_api-0.0.0.0.28/test_rest_api/
--rw-r--r--   0 trjose     (501) staff       (20)      202 2023-04-15 11:23:49.000000 test_rest_api-0.0.0.0.28/test_rest_api/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1608 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.28/test_rest_api/__main__.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 06:20:55.719340 test_rest_api-0.0.0.0.28/test_rest_api/global_variables/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.28/test_rest_api/global_variables/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1161 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.28/test_rest_api/global_variables/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)     2716 2023-04-15 03:04:30.000000 test_rest_api-0.0.0.0.28/test_rest_api/global_variables/global_variables.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 06:20:55.721577 test_rest_api-0.0.0.0.28/test_rest_api/reporting/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-25 09:45:47.000000 test_rest_api-0.0.0.0.28/test_rest_api/reporting/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)    35371 2023-04-15 11:11:29.000000 test_rest_api-0.0.0.0.28/test_rest_api/reporting/html.py
--rw-r--r--   0 trjose     (501) staff       (20)     5418 2023-04-15 11:11:54.000000 test_rest_api-0.0.0.0.28/test_rest_api/reporting/report.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 06:20:55.726044 test_rest_api-0.0.0.0.28/test_rest_api/rest_api/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:34:23.000000 test_rest_api-0.0.0.0.28/test_rest_api/rest_api/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      173 2023-04-17 11:45:13.000000 test_rest_api-0.0.0.0.28/test_rest_api/rest_api/dot_dict.py
--rw-r--r--   0 trjose     (501) staff       (20)     1824 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.28/test_rest_api/rest_api/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      423 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.28/test_rest_api/rest_api/method.py
--rw-r--r--   0 trjose     (501) staff       (20)      332 2023-04-17 12:21:54.000000 test_rest_api-0.0.0.0.28/test_rest_api/rest_api/response.py
--rw-r--r--   0 trjose     (501) staff       (20)     6174 2023-04-17 12:21:45.000000 test_rest_api-0.0.0.0.28/test_rest_api/rest_api/rest_api.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 06:20:55.730567 test_rest_api-0.0.0.0.28/test_rest_api/testing/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:03:23.000000 test_rest_api-0.0.0.0.28/test_rest_api/testing/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     3047 2023-04-16 09:12:15.000000 test_rest_api-0.0.0.0.28/test_rest_api/testing/bug.py
--rw-r--r--   0 trjose     (501) staff       (20)    15201 2023-04-17 07:04:10.000000 test_rest_api-0.0.0.0.28/test_rest_api/testing/decorator.py
--rw-r--r--   0 trjose     (501) staff       (20)      863 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.28/test_rest_api/testing/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)    13772 2023-04-15 07:27:16.000000 test_rest_api-0.0.0.0.28/test_rest_api/testing/runner.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 06:20:55.737241 test_rest_api-0.0.0.0.28/test_rest_api/utils/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.28/test_rest_api/utils/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      943 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.28/test_rest_api/utils/aiohttp_session.py
--rw-r--r--   0 trjose     (501) staff       (20)      546 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.28/test_rest_api/utils/colors.py
--rw-r--r--   0 trjose     (501) staff       (20)      247 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.28/test_rest_api/utils/decorator_hints.py
--rw-r--r--   0 trjose     (501) staff       (20)     2027 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.28/test_rest_api/utils/error_msg.py
--rw-r--r--   0 trjose     (501) staff       (20)     1130 2023-04-16 06:45:29.000000 test_rest_api-0.0.0.0.28/test_rest_api/utils/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      606 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.28/test_rest_api/utils/logger.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 06:20:55.717810 test_rest_api-0.0.0.0.28/test_rest_api.egg-info/
--rw-r--r--   0 trjose     (501) staff       (20)    64005 2023-04-18 06:20:55.000000 test_rest_api-0.0.0.0.28/test_rest_api.egg-info/PKG-INFO
--rw-r--r--   0 trjose     (501) staff       (20)     1112 2023-04-18 06:20:55.000000 test_rest_api-0.0.0.0.28/test_rest_api.egg-info/SOURCES.txt
--rw-r--r--   0 trjose     (501) staff       (20)        1 2023-04-18 06:20:55.000000 test_rest_api-0.0.0.0.28/test_rest_api.egg-info/dependency_links.txt
--rw-r--r--   0 trjose     (501) staff       (20)       29 2023-04-18 06:20:55.000000 test_rest_api-0.0.0.0.28/test_rest_api.egg-info/requires.txt
--rw-r--r--   0 trjose     (501) staff       (20)       14 2023-04-18 06:20:55.000000 test_rest_api-0.0.0.0.28/test_rest_api.egg-info/top_level.txt
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 08:16:46.918579 test_rest_api-0.0.0.0.29/
+-rw-r--r--   0 trjose     (501) staff       (20)     1067 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.29/LICENSE
+-rw-r--r--   0 trjose     (501) staff       (20)    64005 2023-04-18 08:16:46.918271 test_rest_api-0.0.0.0.29/PKG-INFO
+-rw-r--r--   0 trjose     (501) staff       (20)    62282 2023-04-14 16:15:06.000000 test_rest_api-0.0.0.0.29/README.md
+-rw-r--r--   0 trjose     (501) staff       (20)       38 2023-04-18 08:16:46.918686 test_rest_api-0.0.0.0.29/setup.cfg
+-rw-r--r--   0 trjose     (501) staff       (20)     2893 2023-04-18 08:15:30.000000 test_rest_api-0.0.0.0.29/setup.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 08:16:46.900650 test_rest_api-0.0.0.0.29/test_rest_api/
+-rw-r--r--   0 trjose     (501) staff       (20)      202 2023-04-15 11:23:49.000000 test_rest_api-0.0.0.0.29/test_rest_api/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1608 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.29/test_rest_api/__main__.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 08:16:46.905697 test_rest_api-0.0.0.0.29/test_rest_api/global_variables/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.29/test_rest_api/global_variables/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1161 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.29/test_rest_api/global_variables/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2716 2023-04-15 03:04:30.000000 test_rest_api-0.0.0.0.29/test_rest_api/global_variables/global_variables.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 08:16:46.907986 test_rest_api-0.0.0.0.29/test_rest_api/reporting/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-25 09:45:47.000000 test_rest_api-0.0.0.0.29/test_rest_api/reporting/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)    35371 2023-04-15 11:11:29.000000 test_rest_api-0.0.0.0.29/test_rest_api/reporting/html.py
+-rw-r--r--   0 trjose     (501) staff       (20)     5418 2023-04-15 11:11:54.000000 test_rest_api-0.0.0.0.29/test_rest_api/reporting/report.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 08:16:46.911323 test_rest_api-0.0.0.0.29/test_rest_api/rest_api/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:34:23.000000 test_rest_api-0.0.0.0.29/test_rest_api/rest_api/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      173 2023-04-17 11:45:13.000000 test_rest_api-0.0.0.0.29/test_rest_api/rest_api/dot_dict.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1824 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.29/test_rest_api/rest_api/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      423 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.29/test_rest_api/rest_api/method.py
+-rw-r--r--   0 trjose     (501) staff       (20)      332 2023-04-17 12:21:54.000000 test_rest_api-0.0.0.0.29/test_rest_api/rest_api/response.py
+-rw-r--r--   0 trjose     (501) staff       (20)     6174 2023-04-17 12:21:45.000000 test_rest_api-0.0.0.0.29/test_rest_api/rest_api/rest_api.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 08:16:46.913642 test_rest_api-0.0.0.0.29/test_rest_api/testing/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:03:23.000000 test_rest_api-0.0.0.0.29/test_rest_api/testing/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     3047 2023-04-16 09:12:15.000000 test_rest_api-0.0.0.0.29/test_rest_api/testing/bug.py
+-rw-r--r--   0 trjose     (501) staff       (20)    15318 2023-04-18 08:14:24.000000 test_rest_api-0.0.0.0.29/test_rest_api/testing/decorator.py
+-rw-r--r--   0 trjose     (501) staff       (20)      863 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.29/test_rest_api/testing/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)    13772 2023-04-15 07:27:16.000000 test_rest_api-0.0.0.0.29/test_rest_api/testing/runner.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 08:16:46.917619 test_rest_api-0.0.0.0.29/test_rest_api/utils/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.29/test_rest_api/utils/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      943 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.29/test_rest_api/utils/aiohttp_session.py
+-rw-r--r--   0 trjose     (501) staff       (20)      546 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.29/test_rest_api/utils/colors.py
+-rw-r--r--   0 trjose     (501) staff       (20)      247 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.29/test_rest_api/utils/decorator_hints.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2027 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.29/test_rest_api/utils/error_msg.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1130 2023-04-16 06:45:29.000000 test_rest_api-0.0.0.0.29/test_rest_api/utils/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      606 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.29/test_rest_api/utils/logger.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 08:16:46.903929 test_rest_api-0.0.0.0.29/test_rest_api.egg-info/
+-rw-r--r--   0 trjose     (501) staff       (20)    64005 2023-04-18 08:16:46.000000 test_rest_api-0.0.0.0.29/test_rest_api.egg-info/PKG-INFO
+-rw-r--r--   0 trjose     (501) staff       (20)     1112 2023-04-18 08:16:46.000000 test_rest_api-0.0.0.0.29/test_rest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 trjose     (501) staff       (20)        1 2023-04-18 08:16:46.000000 test_rest_api-0.0.0.0.29/test_rest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 trjose     (501) staff       (20)       29 2023-04-18 08:16:46.000000 test_rest_api-0.0.0.0.29/test_rest_api.egg-info/requires.txt
+-rw-r--r--   0 trjose     (501) staff       (20)       14 2023-04-18 08:16:46.000000 test_rest_api-0.0.0.0.29/test_rest_api.egg-info/top_level.txt
```

### Comparing `test_rest_api-0.0.0.0.28/LICENSE` & `test_rest_api-0.0.0.0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.28/PKG-INFO` & `test_rest_api-0.0.0.0.29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_rest_api
-Version: 0.0.0.0.28
+Version: 0.0.0.0.29
 Summary: Asynchronous Test Framework #HighPerformance #EasyToLearn #FastToCode #AsyncTests
 Home-page: https://github.com/troymjose/test_rest_api
 Author: Troy M Jose
 Author-email: 
 Project-URL: Source, https://github.com/troymjose/test_rest_api
 Project-URL: Tracker, https://github.com/troymjose/test_rest_api/issues
 Keywords: test,unittest,restapi,testframework,asyncio,async,asynchronous,testingframework,rest,api,python,python3,testing,unittesting,automation,automationtest,automationtesting,restapitest,restapitesting,restapiunittest,restapiunittesting,restapiautomation,restapiautomationtest,restapiautomationtesting,apitest,apitesting,apiunittest,apiunittesting,apiautomation,apiautomationtest,apiautomationtesting
```

### Comparing `test_rest_api-0.0.0.0.28/README.md` & `test_rest_api-0.0.0.0.29/README.md`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.28/setup.py` & `test_rest_api-0.0.0.0.29/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Get README.md details
 with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
     long_description = '\n' + f.read()
 
 # Setup
 setup(name='test_rest_api',
-      version='0.0.0.0.28',
+      version='0.0.0.0.29',
       author='Troy M Jose',
       author_email='',
       url='https://github.com/troymjose/test_rest_api',
       bugtrack_url='https://github.com/troymjose/test_rest_api/issues',
       project_urls={
           'Source': 'https://github.com/troymjose/test_rest_api',
           'Tracker': 'https://github.com/troymjose/test_rest_api/issues',
```

### Comparing `test_rest_api-0.0.0.0.28/test_rest_api/__main__.py` & `test_rest_api-0.0.0.0.29/test_rest_api/__main__.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.28/test_rest_api/global_variables/exception.py` & `test_rest_api-0.0.0.0.29/test_rest_api/global_variables/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.28/test_rest_api/global_variables/global_variables.py` & `test_rest_api-0.0.0.0.29/test_rest_api/global_variables/global_variables.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.28/test_rest_api/reporting/html.py` & `test_rest_api-0.0.0.0.29/test_rest_api/reporting/html.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.28/test_rest_api/reporting/report.py` & `test_rest_api-0.0.0.0.29/test_rest_api/reporting/report.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.28/test_rest_api/rest_api/exception.py` & `test_rest_api-0.0.0.0.29/test_rest_api/rest_api/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.28/test_rest_api/rest_api/rest_api.py` & `test_rest_api-0.0.0.0.29/test_rest_api/rest_api/rest_api.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.28/test_rest_api/testing/bug.py` & `test_rest_api-0.0.0.0.29/test_rest_api/testing/bug.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.28/test_rest_api/testing/decorator.py` & `test_rest_api-0.0.0.0.29/test_rest_api/testing/decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,129 +71,130 @@
                         test_rest_api_logger.info(
                             f"{colors.YELLOW}{'ERROR' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
                         # Update the error type for reporting
                         error_type = ErrorType.REST_API
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
                         # Format the traceback (Remove unwanted info)
-                        start_res = re.search(r'test_rest_api/testing/decorator.py", line (.*?), in inner',
+                        start_res = re.search(r'test_rest_api(.*?)testing(.*?)decorator.py", line (.*?), in inner',
                                               traceback_data)
                         end_res = re.search(r'raise RestApiCreationException', traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 89:end_res.end()]
+                        traceback_data = traceback_data[start_res.start() + 103:end_res.end()]
                         traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
-                        if re.search(r'test_rest_api/rest_api/rest_api.py", line (.*?), in __call__', traceback_data):
+                        if re.search(r'test_rest_api(.*?)rest_api(.*?)rest_api.py", line (.*?), in __call__',
+                                     traceback_data):
                             traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
                             traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
                         # Update the test status and details
                         status, details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
                     except RestApiSendException as exc:
                         # Log the result
                         test_rest_api_logger.info(
                             f"{colors.YELLOW}{'ERROR' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
                         # Update the error type for reporting
                         error_type = ErrorType.REST_API
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
                         # Format the traceback (Remove unwanted info)
-                        start_res = re.search(r'test_rest_api/testing/decorator.py", line (.*?), in inner',
+                        start_res = re.search(r'test_rest_api(.*?)testing(.*?)decorator.py", line (.*?), in inner',
                                               traceback_data)
                         end_res = re.search(r'raise RestApiSendException', traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 89:end_res.end()]
+                        traceback_data = traceback_data[start_res.start() + 103:end_res.end()]
                         traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
                         traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
                         # Update the test status and details
                         status, details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
                     except BugCreationException as exc:
                         # Log the result
                         test_rest_api_logger.info(
                             f"{colors.YELLOW}{'ERROR' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
                         # Update the error type for reporting
                         error_type = ErrorType.BUG
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
                         # Format the traceback (Remove unwanted info)
-                        start_res = re.search(r'test_rest_api/testing/decorator.py", line (.*?), in inner',
+                        start_res = re.search(r'test_rest_api(.*?)testing(.*?)decorator.py", line (.*?), in inner',
                                               traceback_data)
                         end_res = re.search(r'raise test_rest_api_exception', traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 89:end_res.end()]
+                        traceback_data = traceback_data[start_res.start() + 103:end_res.end()]
                         traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
                         # Update the test status and details
                         status, details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
                     except GlobalVariablesException as exc:
                         # Log the result
                         test_rest_api_logger.info(
                             f"{colors.YELLOW}{'ERROR' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
                         # Update the error type for reporting
                         error_type = ErrorType.GLOBAL_VARIABLES
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
                         # Format the traceback (Remove unwanted info)
-                        start_res = re.search(r'test_rest_api/testing/decorator.py", line (.*?), in inner',
+                        start_res = re.search(r'test_rest_api(.*?)testing(.*?)decorator.py", line (.*?), in inner',
                                               traceback_data)
                         end_res = re.search(r'raise test_rest_api_exception', traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 89:end_res.end()]
+                        traceback_data = traceback_data[start_res.start() + 103:end_res.end()]
                         traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
                         # Update the test status and details
                         status, details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
                     except Bug as exc:
                         # Log the result
                         test_rest_api_logger.info(
                             f"{colors.LIGHT_RED}{'FAIL' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
                         # Update the bug priority for reporting
                         bug_priority = exc.priority
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
                         # Format the traceback (Remove unwanted info)
-                        start_res = re.search(r'test_rest_api/testing/decorator.py", line (.*?), in inner',
+                        start_res = re.search(r'test_rest_api(.*?)testing(.*?)decorator.py", line (.*?), in inner',
                                               traceback_data)
                         end_res = re.search(r'raise Bug', traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 89:end_res.end()]
+                        traceback_data = traceback_data[start_res.start() + 103:end_res.end()]
                         # Update the test status and details
                         status, details = TestStatus.FAIL, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
                     except AssertionError as exc:
                         # Log the result
                         test_rest_api_logger.info(
                             f"{colors.LIGHT_RED}{'FAIL' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
                         # Update the bug priority for reporting
                         bug_priority = exc.args[0].priority if exc.args and isinstance(exc.args[0],
                                                                                        Bug) else Bug.PRIORITY.LOW
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
                         # Format the traceback (Remove unwanted info)
-                        start_res = re.search(r'test_rest_api/testing/decorator.py", line (.*?), in inner',
+                        start_res = re.search(r'test_rest_api(.*?)testing(.*?)decorator.py", line (.*?), in inner',
                                               traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 89:]
+                        traceback_data = traceback_data[start_res.start() + 103:]
                         # Update the test status and details
                         status, details = TestStatus.FAIL, f'\nTRACEBACKS\n----------\n{traceback_data}'
                     except AttributeError as exc:
                         # Log the result
                         test_rest_api_logger.info(
                             f"{colors.YELLOW}{'ERROR' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
                         # Update the error type for reporting
                         error_type = ErrorType.UNEXPECTED
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
                         # Format the traceback (Remove unwanted info)
-                        start_res = re.search(r'test_rest_api/testing/decorator.py", line (.*?), in inner',
+                        start_res = re.search(r'test_rest_api(.*?)testing(.*?)decorator.py", line (.*?), in inner',
                                               traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 89:]
+                        traceback_data = traceback_data[start_res.start() + 103:]
                         # Update the test status and details
                         status, details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}\n\n{"Tip: This may be due to not using await keyword in function calls"}'
                     except Exception as exc:
                         # Log the result
                         test_rest_api_logger.info(
                             f"{colors.YELLOW}{'ERROR' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
                         # Update the error type for reporting
                         error_type = ErrorType.UNEXPECTED
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
                         # Format the traceback (Remove unwanted info)
-                        start_res = re.search(r'test_rest_api/testing/decorator.py", line (.*?), in inner',
+                        start_res = re.search(r'test_rest_api(.*?)testing(.*?)decorator.py", line (.*?), in inner',
                                               traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 89:]
+                        traceback_data = traceback_data[start_res.start() + 103:]
                         # Update the test status and details
                         status, details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
                     finally:
                         # Get standard out messages from all the print() statements
                         stdout_data = string_io.getvalue()
                         # Update the test logs
                         logs = f'Started the test\n{stdout_data}'
```

### Comparing `test_rest_api-0.0.0.0.28/test_rest_api/testing/exception.py` & `test_rest_api-0.0.0.0.29/test_rest_api/testing/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.28/test_rest_api/testing/runner.py` & `test_rest_api-0.0.0.0.29/test_rest_api/testing/runner.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.28/test_rest_api/utils/aiohttp_session.py` & `test_rest_api-0.0.0.0.29/test_rest_api/utils/aiohttp_session.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.28/test_rest_api/utils/colors.py` & `test_rest_api-0.0.0.0.29/test_rest_api/utils/colors.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.28/test_rest_api/utils/error_msg.py` & `test_rest_api-0.0.0.0.29/test_rest_api/utils/error_msg.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.28/test_rest_api/utils/exception.py` & `test_rest_api-0.0.0.0.29/test_rest_api/utils/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.28/test_rest_api/utils/logger.py` & `test_rest_api-0.0.0.0.29/test_rest_api/utils/logger.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.28/test_rest_api.egg-info/PKG-INFO` & `test_rest_api-0.0.0.0.29/test_rest_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-rest-api
-Version: 0.0.0.0.28
+Version: 0.0.0.0.29
 Summary: Asynchronous Test Framework #HighPerformance #EasyToLearn #FastToCode #AsyncTests
 Home-page: https://github.com/troymjose/test_rest_api
 Author: Troy M Jose
 Author-email: 
 Project-URL: Source, https://github.com/troymjose/test_rest_api
 Project-URL: Tracker, https://github.com/troymjose/test_rest_api/issues
 Keywords: test,unittest,restapi,testframework,asyncio,async,asynchronous,testingframework,rest,api,python,python3,testing,unittesting,automation,automationtest,automationtesting,restapitest,restapitesting,restapiunittest,restapiunittesting,restapiautomation,restapiautomationtest,restapiautomationtesting,apitest,apitesting,apiunittest,apiunittesting,apiautomation,apiautomationtest,apiautomationtesting
```

### Comparing `test_rest_api-0.0.0.0.28/test_rest_api.egg-info/SOURCES.txt` & `test_rest_api-0.0.0.0.29/test_rest_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

