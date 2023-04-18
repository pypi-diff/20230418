# Comparing `tmp/test_rest_api-0.0.0.0.27.tar.gz` & `tmp/test_rest_api-0.0.0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_rest_api-0.0.0.0.27.tar", last modified: Tue Apr 11 07:20:02 2023, max compression
+gzip compressed data, was "test_rest_api-0.0.0.0.28.tar", last modified: Tue Apr 18 06:20:55 2023, max compression
```

## Comparing `test_rest_api-0.0.0.0.27.tar` & `test_rest_api-0.0.0.0.28.tar`

### file list

```diff
@@ -1,47 +1,44 @@
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-11 07:20:02.226214 test_rest_api-0.0.0.0.27/
--rw-r--r--   0 trjose     (501) staff       (20)     1067 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.27/LICENSE
--rw-r--r--   0 trjose     (501) staff       (20)    64368 2023-04-11 07:20:02.225214 test_rest_api-0.0.0.0.27/PKG-INFO
--rw-r--r--   0 trjose     (501) staff       (20)    62645 2023-04-09 10:36:09.000000 test_rest_api-0.0.0.0.27/README.md
--rw-r--r--   0 trjose     (501) staff       (20)       38 2023-04-11 07:20:02.226532 test_rest_api-0.0.0.0.27/setup.cfg
--rw-r--r--   0 trjose     (501) staff       (20)     2917 2023-04-11 07:19:21.000000 test_rest_api-0.0.0.0.27/setup.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-11 07:20:02.199678 test_rest_api-0.0.0.0.27/test_rest_api/
--rw-r--r--   0 trjose     (501) staff       (20)      236 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.27/test_rest_api/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1608 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.27/test_rest_api/__main__.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-11 07:20:02.203755 test_rest_api-0.0.0.0.27/test_rest_api/global_variables/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.27/test_rest_api/global_variables/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1161 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.27/test_rest_api/global_variables/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)     2716 2023-04-08 13:00:44.000000 test_rest_api-0.0.0.0.27/test_rest_api/global_variables/global_variables.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-11 07:20:02.205268 test_rest_api-0.0.0.0.27/test_rest_api/logger/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.27/test_rest_api/logger/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1237 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.27/test_rest_api/logger/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      850 2023-04-09 11:31:24.000000 test_rest_api-0.0.0.0.27/test_rest_api/logger/logger.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-11 07:20:02.207582 test_rest_api-0.0.0.0.27/test_rest_api/reporting/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-25 09:45:47.000000 test_rest_api-0.0.0.0.27/test_rest_api/reporting/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)    34587 2023-04-07 17:27:51.000000 test_rest_api-0.0.0.0.27/test_rest_api/reporting/html.py
--rw-r--r--   0 trjose     (501) staff       (20)     5404 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.27/test_rest_api/reporting/report.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-11 07:20:02.212992 test_rest_api-0.0.0.0.27/test_rest_api/rest_api/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:34:23.000000 test_rest_api-0.0.0.0.27/test_rest_api/rest_api/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1824 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.27/test_rest_api/rest_api/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      423 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.27/test_rest_api/rest_api/method.py
--rw-r--r--   0 trjose     (501) staff       (20)      332 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.27/test_rest_api/rest_api/response.py
--rw-r--r--   0 trjose     (501) staff       (20)     6226 2023-04-09 11:13:23.000000 test_rest_api-0.0.0.0.27/test_rest_api/rest_api/rest_api.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-11 07:20:02.217184 test_rest_api-0.0.0.0.27/test_rest_api/testing/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:03:23.000000 test_rest_api-0.0.0.0.27/test_rest_api/testing/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     3904 2023-04-09 10:39:13.000000 test_rest_api-0.0.0.0.27/test_rest_api/testing/bug.py
--rw-r--r--   0 trjose     (501) staff       (20)    14788 2023-04-08 13:49:13.000000 test_rest_api-0.0.0.0.27/test_rest_api/testing/decorator.py
--rw-r--r--   0 trjose     (501) staff       (20)      863 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.27/test_rest_api/testing/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)    13772 2023-04-07 17:27:51.000000 test_rest_api-0.0.0.0.27/test_rest_api/testing/runner.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-11 07:20:02.223390 test_rest_api-0.0.0.0.27/test_rest_api/utils/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.27/test_rest_api/utils/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      943 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.27/test_rest_api/utils/aiohttp_session.py
--rw-r--r--   0 trjose     (501) staff       (20)      546 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.27/test_rest_api/utils/colors.py
--rw-r--r--   0 trjose     (501) staff       (20)      247 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.27/test_rest_api/utils/decorator_hints.py
--rw-r--r--   0 trjose     (501) staff       (20)     2027 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.27/test_rest_api/utils/error_msg.py
--rw-r--r--   0 trjose     (501) staff       (20)     1127 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.27/test_rest_api/utils/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      606 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.27/test_rest_api/utils/logger.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-11 07:20:02.202379 test_rest_api-0.0.0.0.27/test_rest_api.egg-info/
--rw-r--r--   0 trjose     (501) staff       (20)    64368 2023-04-11 07:20:02.000000 test_rest_api-0.0.0.0.27/test_rest_api.egg-info/PKG-INFO
--rw-r--r--   0 trjose     (501) staff       (20)     1175 2023-04-11 07:20:02.000000 test_rest_api-0.0.0.0.27/test_rest_api.egg-info/SOURCES.txt
--rw-r--r--   0 trjose     (501) staff       (20)        1 2023-04-11 07:20:02.000000 test_rest_api-0.0.0.0.27/test_rest_api.egg-info/dependency_links.txt
--rw-r--r--   0 trjose     (501) staff       (20)       29 2023-04-11 07:20:02.000000 test_rest_api-0.0.0.0.27/test_rest_api.egg-info/requires.txt
--rw-r--r--   0 trjose     (501) staff       (20)       14 2023-04-11 07:20:02.000000 test_rest_api-0.0.0.0.27/test_rest_api.egg-info/top_level.txt
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 06:20:55.739021 test_rest_api-0.0.0.0.28/
+-rw-r--r--   0 trjose     (501) staff       (20)     1067 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.28/LICENSE
+-rw-r--r--   0 trjose     (501) staff       (20)    64005 2023-04-18 06:20:55.738514 test_rest_api-0.0.0.0.28/PKG-INFO
+-rw-r--r--   0 trjose     (501) staff       (20)    62282 2023-04-14 16:15:06.000000 test_rest_api-0.0.0.0.28/README.md
+-rw-r--r--   0 trjose     (501) staff       (20)       38 2023-04-18 06:20:55.739166 test_rest_api-0.0.0.0.28/setup.cfg
+-rw-r--r--   0 trjose     (501) staff       (20)     2893 2023-04-18 06:20:41.000000 test_rest_api-0.0.0.0.28/setup.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 06:20:55.714803 test_rest_api-0.0.0.0.28/test_rest_api/
+-rw-r--r--   0 trjose     (501) staff       (20)      202 2023-04-15 11:23:49.000000 test_rest_api-0.0.0.0.28/test_rest_api/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1608 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.28/test_rest_api/__main__.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 06:20:55.719340 test_rest_api-0.0.0.0.28/test_rest_api/global_variables/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.28/test_rest_api/global_variables/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1161 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.28/test_rest_api/global_variables/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2716 2023-04-15 03:04:30.000000 test_rest_api-0.0.0.0.28/test_rest_api/global_variables/global_variables.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 06:20:55.721577 test_rest_api-0.0.0.0.28/test_rest_api/reporting/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-25 09:45:47.000000 test_rest_api-0.0.0.0.28/test_rest_api/reporting/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)    35371 2023-04-15 11:11:29.000000 test_rest_api-0.0.0.0.28/test_rest_api/reporting/html.py
+-rw-r--r--   0 trjose     (501) staff       (20)     5418 2023-04-15 11:11:54.000000 test_rest_api-0.0.0.0.28/test_rest_api/reporting/report.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 06:20:55.726044 test_rest_api-0.0.0.0.28/test_rest_api/rest_api/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:34:23.000000 test_rest_api-0.0.0.0.28/test_rest_api/rest_api/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      173 2023-04-17 11:45:13.000000 test_rest_api-0.0.0.0.28/test_rest_api/rest_api/dot_dict.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1824 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.28/test_rest_api/rest_api/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      423 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.28/test_rest_api/rest_api/method.py
+-rw-r--r--   0 trjose     (501) staff       (20)      332 2023-04-17 12:21:54.000000 test_rest_api-0.0.0.0.28/test_rest_api/rest_api/response.py
+-rw-r--r--   0 trjose     (501) staff       (20)     6174 2023-04-17 12:21:45.000000 test_rest_api-0.0.0.0.28/test_rest_api/rest_api/rest_api.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 06:20:55.730567 test_rest_api-0.0.0.0.28/test_rest_api/testing/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:03:23.000000 test_rest_api-0.0.0.0.28/test_rest_api/testing/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     3047 2023-04-16 09:12:15.000000 test_rest_api-0.0.0.0.28/test_rest_api/testing/bug.py
+-rw-r--r--   0 trjose     (501) staff       (20)    15201 2023-04-17 07:04:10.000000 test_rest_api-0.0.0.0.28/test_rest_api/testing/decorator.py
+-rw-r--r--   0 trjose     (501) staff       (20)      863 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.28/test_rest_api/testing/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)    13772 2023-04-15 07:27:16.000000 test_rest_api-0.0.0.0.28/test_rest_api/testing/runner.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 06:20:55.737241 test_rest_api-0.0.0.0.28/test_rest_api/utils/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.28/test_rest_api/utils/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      943 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.28/test_rest_api/utils/aiohttp_session.py
+-rw-r--r--   0 trjose     (501) staff       (20)      546 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.28/test_rest_api/utils/colors.py
+-rw-r--r--   0 trjose     (501) staff       (20)      247 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.28/test_rest_api/utils/decorator_hints.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2027 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.28/test_rest_api/utils/error_msg.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1130 2023-04-16 06:45:29.000000 test_rest_api-0.0.0.0.28/test_rest_api/utils/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      606 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.28/test_rest_api/utils/logger.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 06:20:55.717810 test_rest_api-0.0.0.0.28/test_rest_api.egg-info/
+-rw-r--r--   0 trjose     (501) staff       (20)    64005 2023-04-18 06:20:55.000000 test_rest_api-0.0.0.0.28/test_rest_api.egg-info/PKG-INFO
+-rw-r--r--   0 trjose     (501) staff       (20)     1112 2023-04-18 06:20:55.000000 test_rest_api-0.0.0.0.28/test_rest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 trjose     (501) staff       (20)        1 2023-04-18 06:20:55.000000 test_rest_api-0.0.0.0.28/test_rest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 trjose     (501) staff       (20)       29 2023-04-18 06:20:55.000000 test_rest_api-0.0.0.0.28/test_rest_api.egg-info/requires.txt
+-rw-r--r--   0 trjose     (501) staff       (20)       14 2023-04-18 06:20:55.000000 test_rest_api-0.0.0.0.28/test_rest_api.egg-info/top_level.txt
```

### Comparing `test_rest_api-0.0.0.0.27/LICENSE` & `test_rest_api-0.0.0.0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.27/PKG-INFO` & `test_rest_api-0.0.0.0.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_rest_api
-Version: 0.0.0.0.27
+Version: 0.0.0.0.28
 Summary: Asynchronous Test Framework #HighPerformance #EasyToLearn #FastToCode #AsyncTests
 Home-page: https://github.com/troymjose/test_rest_api
 Author: Troy M Jose
 Author-email: 
 Project-URL: Source, https://github.com/troymjose/test_rest_api
 Project-URL: Tracker, https://github.com/troymjose/test_rest_api/issues
 Keywords: test,unittest,restapi,testframework,asyncio,async,asynchronous,testingframework,rest,api,python,python3,testing,unittesting,automation,automationtest,automationtesting,restapitest,restapitesting,restapiunittest,restapiunittesting,restapiautomation,restapiautomationtest,restapiautomationtesting,apitest,apitesting,apiunittest,apiunittesting,apiautomation,apiautomationtest,apiautomationtesting
@@ -166,27 +166,24 @@
 - Tests like login, logout etc. are __perfect candidates__ for #ALL
 
 <h4 id="5-project-structure">5. Project structure</h4>
 
 - - -
 
 ```
-my_project
-│── __init__.py                   # Python module
+.
 ├── api                           # Store all your rest api files
-│   │── __init__.py               # Python module
 │   ├── auth                      # Custom structure for subfolders & files
 │   │   ├── login.py              # Python file to store rest_api code
 │   │   │   ├── def user_login()  # Python function to create rest_api
 │   │   │   ├── def admin_login()
 │   │   │   └── ...    
 │   │   └── ...
 │   └── ...
 ├── testsuite                     # Root testsuite folder
-│   │── __init__.py               # Python module
 │   ├── auth                      # Custom structure for subfolders & files
 │   │   ├── login.py              # Python file as testsuite to store tests
 │   │   │   ├── async def t001()  # Python async function as testcases
 │   │   │   ├── async def t002()
 │   │   │   └── ...    
 │   │   └── ...
 │   └── ...
@@ -277,17 +274,15 @@
     - Mandatory: False
     - Data Type: bool
     - Expected: True or False. Provide False, to run tests sequentially
     - Default: True
 - __execution_order__
     - Mandatory: False
     - Data Type: str
-    - Expected: Custom text for ordering. This will work only when is_async = False. Execution order '14' will run
-      before '2' even though the number 2 is less than 14. This is because execution_order uses alphabetic string
-      ordering & not number ordering
+    - Expected: Custom text for ordering. This will work only when is_async = False
     - Default: 'zzzzz'
 
 <h4 id="3-my-first-logger">3. My first logger</h4>
 
 - - -
 
 ```python
```

### Comparing `test_rest_api-0.0.0.0.27/README.md` & `test_rest_api-0.0.0.0.28/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -135,27 +135,24 @@
 - Tests like login, logout etc. are __perfect candidates__ for #ALL
 
 <h4 id="5-project-structure">5. Project structure</h4>
 
 - - -
 
 ```
-my_project
-│── __init__.py                   # Python module
+.
 ├── api                           # Store all your rest api files
-│   │── __init__.py               # Python module
 │   ├── auth                      # Custom structure for subfolders & files
 │   │   ├── login.py              # Python file to store rest_api code
 │   │   │   ├── def user_login()  # Python function to create rest_api
 │   │   │   ├── def admin_login()
 │   │   │   └── ...    
 │   │   └── ...
 │   └── ...
 ├── testsuite                     # Root testsuite folder
-│   │── __init__.py               # Python module
 │   ├── auth                      # Custom structure for subfolders & files
 │   │   ├── login.py              # Python file as testsuite to store tests
 │   │   │   ├── async def t001()  # Python async function as testcases
 │   │   │   ├── async def t002()
 │   │   │   └── ...    
 │   │   └── ...
 │   └── ...
@@ -246,17 +243,15 @@
     - Mandatory: False
     - Data Type: bool
     - Expected: True or False. Provide False, to run tests sequentially
     - Default: True
 - __execution_order__
     - Mandatory: False
     - Data Type: str
-    - Expected: Custom text for ordering. This will work only when is_async = False. Execution order '14' will run
-      before '2' even though the number 2 is less than 14. This is because execution_order uses alphabetic string
-      ordering & not number ordering
+    - Expected: Custom text for ordering. This will work only when is_async = False
     - Default: 'zzzzz'
 
 <h4 id="3-my-first-logger">3. My first logger</h4>
 
 - - -
 
 ```python
```

### Comparing `test_rest_api-0.0.0.0.27/setup.py` & `test_rest_api-0.0.0.0.28/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Get README.md details
 with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
     long_description = '\n' + f.read()
 
 # Setup
 setup(name='test_rest_api',
-      version='0.0.0.0.27',
+      version='0.0.0.0.28',
       author='Troy M Jose',
       author_email='',
       url='https://github.com/troymjose/test_rest_api',
       bugtrack_url='https://github.com/troymjose/test_rest_api/issues',
       project_urls={
           'Source': 'https://github.com/troymjose/test_rest_api',
           'Tracker': 'https://github.com/troymjose/test_rest_api/issues',
@@ -30,15 +30,15 @@
       description='Asynchronous Test Framework #HighPerformance #EasyToLearn #FastToCode #AsyncTests',
       keywords=['test', 'unittest', 'restapi', 'testframework', 'asyncio', 'async', 'asynchronous',
                 'testingframework', 'rest', 'api', 'python', 'python3', 'testing', 'unittesting', 'automation',
                 'automationtest', 'automationtesting',
                 'restapitest', 'restapitesting', 'restapiunittest', 'restapiunittesting', 'restapiautomation',
                 'restapiautomationtest', 'restapiautomationtesting', 'apitest', 'apitesting', 'apiunittest',
                 'apiunittesting', 'apiautomation', 'apiautomationtest', 'apiautomationtesting'],
-      packages=['test_rest_api', 'test_rest_api.global_variables', 'test_rest_api.logger', 'test_rest_api.reporting',
+      packages=['test_rest_api', 'test_rest_api.global_variables', 'test_rest_api.reporting',
                 'test_rest_api.rest_api', 'test_rest_api.testing', 'test_rest_api.utils'],
       install_requires=['aiohttp', 'Jinja2', 'python-dotenv'],
       long_description_content_type='text/markdown',
       long_description=long_description,
       classifiers=['Programming Language :: Python :: 3.8',
                    'Programming Language :: Python :: 3.9',
                    'Programming Language :: Python :: 3.10',
```

### Comparing `test_rest_api-0.0.0.0.27/test_rest_api/__main__.py` & `test_rest_api-0.0.0.0.28/test_rest_api/__main__.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.27/test_rest_api/global_variables/exception.py` & `test_rest_api-0.0.0.0.28/test_rest_api/global_variables/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.27/test_rest_api/global_variables/global_variables.py` & `test_rest_api-0.0.0.0.28/test_rest_api/global_variables/global_variables.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.27/test_rest_api/reporting/html.py` & `test_rest_api-0.0.0.0.28/test_rest_api/reporting/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -504,14 +504,26 @@
                           >{{ sync_test.error_type.replace('_', ' ').title() }}</span
                         >
                       </td>
                     </tr>
                   </tbody>
                 </table>
                 <div class="card">
+                  <div class="card-header">
+                    Logs
+                  </div>
+                  <div class="card-body">
+                    <pre>{{ sync_test.logs }}</pre>
+                  </div>
+                </div>
+                <br />
+                <div class="card">
+                  <div class="card-header">
+                    Details
+                  </div>
                   <div class="card-body">
                     <pre>{{ sync_test.details }}</pre>
                   </div>
                 </div>
               </div>
             </div>
           </div>
@@ -689,14 +701,26 @@
                           >{{ async_test.error_type.replace('_', ' ').title() }}</span
                         >
                       </td>
                     </tr>
                   </tbody>
                 </table>
                 <div class="card">
+                  <div class="card-header">
+                    Logs
+                  </div>
+                  <div class="card-body">
+                    <pre>{{ async_test.logs }}</pre>
+                  </div>
+                </div>
+                <br />
+                <div class="card">
+                  <div class="card-header">
+                    Details
+                  </div>
                   <div class="card-body">
                     <pre>{{ async_test.details }}</pre>
                   </div>
                 </div>
               </div>
             </div>
           </div>
@@ -924,8 +948,8 @@
         $(
           "#asyncTestResultAccordion .accordion-item .accordion-collapse"
         ).collapse("hide");
       });
     </script>
   </body>
 </html>
-"""
+"""
```

#### html2text {}

```diff
@@ -61,14 +61,18 @@
 Testsuite    {{ sync_test.testsuite }}
 Tags         {{ '#' + '#'.join(sync_test.tags) if sync_test.tags else '#ALL' }}
 Start        {{ sync_test.start }}
 End          {{ sync_test.end }}
 Duration     {{ sync_test.duration }}
 Bug Priority {{ sync_test.bug_priority }}
 Error Type   {{ sync_test.error_type.replace('_', ' ').title() }}
+Logs
+{{ sync_test.logs }}
+
+Details
 {{ sync_test.details }}
 {% endfor %}
 {% endif %} {% if summary.tests.async_tests > 0 %}
 
 
 
   Asynchronous Tests
@@ -88,14 +92,18 @@
 Tags         {{ '#' + '#'.join(async_test.tags) if async_test.tags else '#ALL'
              }}
 Start        {{ async_test.start }}
 End          {{ async_test.end }}
 Duration     {{ async_test.duration }}
 Bug Priority {{ async_test.bug_priority }}
 Error Type   {{ async_test.error_type.replace('_', ' ').title() }}
+Logs
+{{ async_test.logs }}
+
+Details
 {{ async_test.details }}
 {% endfor %}
 {% endif %}
```

### Comparing `test_rest_api-0.0.0.0.27/test_rest_api/reporting/report.py` & `test_rest_api-0.0.0.0.28/test_rest_api/reporting/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 class ReportTestResult:
     name: str
     desc: str
     is_async: bool
     testsuite: str
     status: str
     details: str
+    logs: str
     tags: tuple
     start: str
     end: str
     duration: str
     bug_priority: str
     error_type: str
```

### Comparing `test_rest_api-0.0.0.0.27/test_rest_api/rest_api/exception.py` & `test_rest_api-0.0.0.0.28/test_rest_api/rest_api/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.27/test_rest_api/rest_api/rest_api.py` & `test_rest_api-0.0.0.0.28/test_rest_api/rest_api/rest_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,19 +79,20 @@
         self.parameters = parameters
         self.headers = headers
         self.body = body
         # Aiohttp variables
         self._session = AioHttpSession()
 
     def __str__(self):
-        return f"""Rest Api Info
-          Url:        {self.url}
-          Headers:    {self.headers}
-          Parameters: {self.parameters}
-          Body:       {self.body}"""
+        return f"""
+Url:        {self.url}
+Headers:    {self.headers}
+Parameters: {self.parameters}
+Body:       {self.body}
+"""
 
     async def send(self, method: str):
         """
         Send the rest api by providing the request method
         """
         try:
             # Check if method is of type string
```

### Comparing `test_rest_api-0.0.0.0.27/test_rest_api/testing/decorator.py` & `test_rest_api-0.0.0.0.28/test_rest_api/testing/decorator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import re
 import traceback
 import functools
+from io import StringIO
 from itertools import count
 from datetime import datetime
 from time import perf_counter_ns
+from contextlib import redirect_stdout
 from inspect import iscoroutinefunction
-from .bug import BugException
+from .bug import Bug
 from ..utils.colors import colors
 from .exception import BugCreationException
-from ..logger.exception import LoggerException
 from ..utils.logger import test_rest_api_logger
 from ..global_variables.exception import GlobalVariablesException
 from ..reporting.report import report, ReportTestResult, TestStatus, ErrorType
 from ..rest_api.exception import RestApiCreationException, RestApiSendException
 
 # Iter for creating id for testcase name
 iter_test_name = count(start=1)
@@ -28,16 +29,16 @@
             testcase_name: str = f'{name} ({testsuite})' if name else f'{func.__name__} ({testsuite})'
             # Add unique id to the name (Users can provide same name for multiple testcases)
             testcase_name += f" [{next(iter_test_name)}]"
             # Start the stopwatch / counter
             timer_start = perf_counter_ns()
             # Get the start date time of the test
             start = datetime.now().strftime('%Y-%m-%d %H-%M-%S')
-            # Initialise test status and test details
-            test_status, test_details = TestStatus.SKIP, 'Testcase is skipped'
+            # Initialise test status, test details and test logs
+            status, details, logs = TestStatus.SKIP, 'Testcase is skipped', 'No data to display'
             # Initialise bug priority and error type which will be used for reporting
             bug_priority, error_type = '', ''
             # Initialise skip as false
             skip = False
             # Get the runner test tags
             from test_rest_api import runner
             # If we have any runner test tags
@@ -45,170 +46,182 @@
                 # Check if the tag is #ALL (This will run for all tag cases, eg: login api)
                 if 'ALL' not in tags:
                     # Check if any of the runner test tag is present in the current test else skip the test
                     if not any(test_tag in tags for test_tag in runner.test_tags):
                         skip = True
             if not skip:
                 # Initialise test status and test details
-                test_status, test_details = TestStatus.DISABLE, 'Testcase is disabled'
+                status, details = TestStatus.DISABLE, 'Testcase is disabled'
                 # Only execute enabled testcases
                 if enabled:
+                    # In-memory file-like object
+                    string_io = StringIO()
                     try:
-                        # Call the async test function
-                        result = await func(*args, **kwargs)
+                        # Redirect standard output to string_io
+                        # In python, print() function prints values to standard out
+                        with redirect_stdout(string_io):
+                            # Call the async test function
+                            await func(*args, **kwargs)
                         # Log the result
                         test_rest_api_logger.info(
                             f"{colors.LIGHT_GREEN}{'PASS' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
                         # Update the test status and details
-                        test_status, test_details = TestStatus.PASS, f'Success !\n\n{str(result) if result else ""}'
+                        status, details = TestStatus.PASS, 'Success'
                     except RestApiCreationException as exc:
                         # Log the result
                         test_rest_api_logger.info(
                             f"{colors.YELLOW}{'ERROR' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
                         # Update the error type for reporting
                         error_type = ErrorType.REST_API
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
                         # Format the traceback (Remove unwanted info)
                         start_res = re.search(r'test_rest_api/testing/decorator.py", line (.*?), in inner',
                                               traceback_data)
                         end_res = re.search(r'raise RestApiCreationException', traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 98:end_res.end()]
+                        traceback_data = traceback_data[start_res.start() + 89:end_res.end()]
                         traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
                         if re.search(r'test_rest_api/rest_api/rest_api.py", line (.*?), in __call__', traceback_data):
                             traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
                             traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
                         # Update the test status and details
-                        test_status, test_details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
+                        status, details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
                     except RestApiSendException as exc:
                         # Log the result
                         test_rest_api_logger.info(
                             f"{colors.YELLOW}{'ERROR' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
                         # Update the error type for reporting
                         error_type = ErrorType.REST_API
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
                         # Format the traceback (Remove unwanted info)
                         start_res = re.search(r'test_rest_api/testing/decorator.py", line (.*?), in inner',
                                               traceback_data)
                         end_res = re.search(r'raise RestApiSendException', traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 98:end_res.end()]
+                        traceback_data = traceback_data[start_res.start() + 89:end_res.end()]
                         traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
                         traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
                         # Update the test status and details
-                        test_status, test_details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
+                        status, details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
                     except BugCreationException as exc:
                         # Log the result
                         test_rest_api_logger.info(
                             f"{colors.YELLOW}{'ERROR' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
                         # Update the error type for reporting
                         error_type = ErrorType.BUG
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
                         # Format the traceback (Remove unwanted info)
                         start_res = re.search(r'test_rest_api/testing/decorator.py", line (.*?), in inner',
                                               traceback_data)
-                        end_res = re.search(r'raise BugCreationException', traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 98:end_res.end()]
+                        end_res = re.search(r'raise test_rest_api_exception', traceback_data)
+                        traceback_data = traceback_data[start_res.start() + 89:end_res.end()]
                         traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
-                        if re.search(r'test_rest_api/testing/bug.py", line (.*?), in __call__', traceback_data):
-                            traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
-                            traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
                         # Update the test status and details
-                        test_status, test_details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
+                        status, details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
                     except GlobalVariablesException as exc:
                         # Log the result
                         test_rest_api_logger.info(
                             f"{colors.YELLOW}{'ERROR' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
                         # Update the error type for reporting
                         error_type = ErrorType.GLOBAL_VARIABLES
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
                         # Format the traceback (Remove unwanted info)
                         start_res = re.search(r'test_rest_api/testing/decorator.py", line (.*?), in inner',
                                               traceback_data)
                         end_res = re.search(r'raise test_rest_api_exception', traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 98:end_res.end()]
+                        traceback_data = traceback_data[start_res.start() + 89:end_res.end()]
                         traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
                         # Update the test status and details
-                        test_status, test_details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
-                    except LoggerException as exc:
+                        status, details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
+                    except Bug as exc:
                         # Log the result
                         test_rest_api_logger.info(
-                            f"{colors.YELLOW}{'ERROR' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
-                        # Update the error type for reporting
-                        error_type = ErrorType.LOGGER
+                            f"{colors.LIGHT_RED}{'FAIL' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
+                        # Update the bug priority for reporting
+                        bug_priority = exc.priority
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
                         # Format the traceback (Remove unwanted info)
                         start_res = re.search(r'test_rest_api/testing/decorator.py", line (.*?), in inner',
                                               traceback_data)
-                        end_res = re.search(r'raise test_rest_api_exception', traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 98:end_res.end()]
-                        traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
+                        end_res = re.search(r'raise Bug', traceback_data)
+                        traceback_data = traceback_data[start_res.start() + 89:end_res.end()]
                         # Update the test status and details
-                        test_status, test_details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
-                    except BugException as exc:
+                        status, details = TestStatus.FAIL, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
+                    except AssertionError as exc:
                         # Log the result
                         test_rest_api_logger.info(
                             f"{colors.LIGHT_RED}{'FAIL' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
                         # Update the bug priority for reporting
-                        bug_priority = exc.priority
+                        bug_priority = exc.args[0].priority if exc.args and isinstance(exc.args[0],
+                                                                                       Bug) else Bug.PRIORITY.LOW
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
                         # Format the traceback (Remove unwanted info)
                         start_res = re.search(r'test_rest_api/testing/decorator.py", line (.*?), in inner',
                                               traceback_data)
-                        end_res = re.search(r'raise BugException', traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 98:end_res.end()]
-                        traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
-                        traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
+                        traceback_data = traceback_data[start_res.start() + 89:]
                         # Update the test status and details
-                        test_status, test_details = TestStatus.FAIL, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
+                        status, details = TestStatus.FAIL, f'\nTRACEBACKS\n----------\n{traceback_data}'
                     except AttributeError as exc:
                         # Log the result
                         test_rest_api_logger.info(
                             f"{colors.YELLOW}{'ERROR' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
                         # Update the error type for reporting
                         error_type = ErrorType.UNEXPECTED
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
                         # Format the traceback (Remove unwanted info)
                         start_res = re.search(r'test_rest_api/testing/decorator.py", line (.*?), in inner',
                                               traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 98:]
+                        traceback_data = traceback_data[start_res.start() + 89:]
                         # Update the test status and details
-                        test_status, test_details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}\n\n{"Tip: This may be due to not using await keyword in function calls"}'
+                        status, details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}\n\n{"Tip: This may be due to not using await keyword in function calls"}'
                     except Exception as exc:
                         # Log the result
                         test_rest_api_logger.info(
                             f"{colors.YELLOW}{'ERROR' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
                         # Update the error type for reporting
                         error_type = ErrorType.UNEXPECTED
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
                         # Format the traceback (Remove unwanted info)
                         start_res = re.search(r'test_rest_api/testing/decorator.py", line (.*?), in inner',
                                               traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 98:]
+                        traceback_data = traceback_data[start_res.start() + 89:]
                         # Update the test status and details
-                        test_status, test_details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
+                        status, details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
+                    finally:
+                        # Get standard out messages from all the print() statements
+                        stdout_data = string_io.getvalue()
+                        # Update the test logs
+                        logs = f'Started the test\n{stdout_data}'
+                        # Dynamic log msg for different test status
+                        if status == TestStatus.PASS:
+                            logs += 'Completed the test'
+                        elif status == TestStatus.FAIL:
+                            logs += 'Bug!\nTest exited without ending'
+                        elif status == TestStatus.ERROR:
+                            logs += 'Error in code\nTest exited without ending'
             # Set the end time of the test
             end = datetime.now().strftime('%Y-%m-%d %H-%M-%S')
             # Stop the stopwatch / counter
             timer_stop = perf_counter_ns()
             # Calculate the time duration of the test in seconds (note: duration is in nanoseconds)
             duration = f'{(timer_stop - timer_start) / 1000000000} seconds'
             # Create Report test result object instance
             test_result = ReportTestResult(name=testcase_name,
                                            desc=desc,
                                            is_async=is_async,
                                            testsuite=testsuite,
-                                           status=test_status,
-                                           details=test_details,
+                                           status=status,
+                                           details=details,
+                                           logs=logs,
                                            tags=tags,
                                            start=start,
                                            end=end,
                                            duration=duration,
                                            bug_priority=bug_priority,
                                            error_type=error_type)
             # Add the test result to the report
```

### Comparing `test_rest_api-0.0.0.0.27/test_rest_api/testing/exception.py` & `test_rest_api-0.0.0.0.28/test_rest_api/testing/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.27/test_rest_api/testing/runner.py` & `test_rest_api-0.0.0.0.28/test_rest_api/testing/runner.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.27/test_rest_api/utils/aiohttp_session.py` & `test_rest_api-0.0.0.0.28/test_rest_api/utils/aiohttp_session.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.27/test_rest_api/utils/colors.py` & `test_rest_api-0.0.0.0.28/test_rest_api/utils/colors.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.27/test_rest_api/utils/error_msg.py` & `test_rest_api-0.0.0.0.28/test_rest_api/utils/error_msg.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.27/test_rest_api/utils/exception.py` & `test_rest_api-0.0.0.0.28/test_rest_api/utils/exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ERROR MESSAGE
 -------------
 {error_msg.strip() if error_msg.strip() else _no_data_to_display}
 """
 
 
 @decorated_func_param_hints
-def catch_exc(test_rest_api_exception: TestRestApiException):
+def catch_exc(*, test_rest_api_exception: TestRestApiException):
     """
     Decorator used for catching python code exceptions for functions
     Example: Function calls with empty params, invalid params etc
 
     Developers can raise python Exceptions inside function body which will be auto converted to TestRestApiExceptions
     """
```

### Comparing `test_rest_api-0.0.0.0.27/test_rest_api/utils/logger.py` & `test_rest_api-0.0.0.0.28/test_rest_api/utils/logger.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.27/test_rest_api.egg-info/PKG-INFO` & `test_rest_api-0.0.0.0.28/test_rest_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-rest-api
-Version: 0.0.0.0.27
+Version: 0.0.0.0.28
 Summary: Asynchronous Test Framework #HighPerformance #EasyToLearn #FastToCode #AsyncTests
 Home-page: https://github.com/troymjose/test_rest_api
 Author: Troy M Jose
 Author-email: 
 Project-URL: Source, https://github.com/troymjose/test_rest_api
 Project-URL: Tracker, https://github.com/troymjose/test_rest_api/issues
 Keywords: test,unittest,restapi,testframework,asyncio,async,asynchronous,testingframework,rest,api,python,python3,testing,unittesting,automation,automationtest,automationtesting,restapitest,restapitesting,restapiunittest,restapiunittesting,restapiautomation,restapiautomationtest,restapiautomationtesting,apitest,apitesting,apiunittest,apiunittesting,apiautomation,apiautomationtest,apiautomationtesting
@@ -166,27 +166,24 @@
 - Tests like login, logout etc. are __perfect candidates__ for #ALL
 
 <h4 id="5-project-structure">5. Project structure</h4>
 
 - - -
 
 ```
-my_project
-│── __init__.py                   # Python module
+.
 ├── api                           # Store all your rest api files
-│   │── __init__.py               # Python module
 │   ├── auth                      # Custom structure for subfolders & files
 │   │   ├── login.py              # Python file to store rest_api code
 │   │   │   ├── def user_login()  # Python function to create rest_api
 │   │   │   ├── def admin_login()
 │   │   │   └── ...    
 │   │   └── ...
 │   └── ...
 ├── testsuite                     # Root testsuite folder
-│   │── __init__.py               # Python module
 │   ├── auth                      # Custom structure for subfolders & files
 │   │   ├── login.py              # Python file as testsuite to store tests
 │   │   │   ├── async def t001()  # Python async function as testcases
 │   │   │   ├── async def t002()
 │   │   │   └── ...    
 │   │   └── ...
 │   └── ...
@@ -277,17 +274,15 @@
     - Mandatory: False
     - Data Type: bool
     - Expected: True or False. Provide False, to run tests sequentially
     - Default: True
 - __execution_order__
     - Mandatory: False
     - Data Type: str
-    - Expected: Custom text for ordering. This will work only when is_async = False. Execution order '14' will run
-      before '2' even though the number 2 is less than 14. This is because execution_order uses alphabetic string
-      ordering & not number ordering
+    - Expected: Custom text for ordering. This will work only when is_async = False
     - Default: 'zzzzz'
 
 <h4 id="3-my-first-logger">3. My first logger</h4>
 
 - - -
 
 ```python
```

### Comparing `test_rest_api-0.0.0.0.27/test_rest_api.egg-info/SOURCES.txt` & `test_rest_api-0.0.0.0.28/test_rest_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,19 @@
 test_rest_api.egg-info/SOURCES.txt
 test_rest_api.egg-info/dependency_links.txt
 test_rest_api.egg-info/requires.txt
 test_rest_api.egg-info/top_level.txt
 test_rest_api/global_variables/__init__.py
 test_rest_api/global_variables/exception.py
 test_rest_api/global_variables/global_variables.py
-test_rest_api/logger/__init__.py
-test_rest_api/logger/exception.py
-test_rest_api/logger/logger.py
 test_rest_api/reporting/__init__.py
 test_rest_api/reporting/html.py
 test_rest_api/reporting/report.py
 test_rest_api/rest_api/__init__.py
+test_rest_api/rest_api/dot_dict.py
 test_rest_api/rest_api/exception.py
 test_rest_api/rest_api/method.py
 test_rest_api/rest_api/response.py
 test_rest_api/rest_api/rest_api.py
 test_rest_api/testing/__init__.py
 test_rest_api/testing/bug.py
 test_rest_api/testing/decorator.py
```

