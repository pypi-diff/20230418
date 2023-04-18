# Comparing `tmp/executor-http-0.1.0.tar.gz` & `tmp/executor-http-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "executor-http-0.1.0.tar", last modified: Tue Apr 18 12:17:12 2023, max compression
+gzip compressed data, was "executor-http-0.1.1.tar", last modified: Tue Apr 18 14:17:32 2023, max compression
```

## Comparing `executor-http-0.1.0.tar` & `executor-http-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:17:12.491994 executor-http-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-18 12:16:56.000000 executor-http-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-18 12:17:12.491994 executor-http-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-18 12:16:56.000000 executor-http-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:17:12.491994 executor-http-0.1.0/executor_http.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-18 12:17:12.000000 executor-http-0.1.0/executor_http.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-18 12:17:12.000000 executor-http-0.1.0/executor_http.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 12:17:12.000000 executor-http-0.1.0/executor_http.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 12:17:12.000000 executor-http-0.1.0/executor_http.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-18 12:17:12.000000 executor-http-0.1.0/executor_http.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 12:17:12.000000 executor-http-0.1.0/executor_http.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 12:17:12.491994 executor-http-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-18 12:16:56.000000 executor-http-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:17:32.484866 executor-http-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-18 14:17:14.000000 executor-http-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-18 14:17:32.484866 executor-http-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-18 14:17:14.000000 executor-http-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:17:32.480865 executor-http-0.1.1/executor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:17:32.480865 executor-http-0.1.1/executor/http/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:17:32.484866 executor-http-0.1.1/executor/http/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:17:32.484866 executor-http-0.1.1/executor/http/server/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/routers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/routers/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/routers/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/routers/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/routers/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/routers/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:17:32.484866 executor-http-0.1.1/executor/http/server/user_db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/user_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/user_db/crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/user_db/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/user_db/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/user_db/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/user_db/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:17:32.484866 executor-http-0.1.1/executor/http/server/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/utils/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-18 14:17:14.000000 executor-http-0.1.1/executor/http/server/utils/oauth2cookie.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:17:32.484866 executor-http-0.1.1/executor_http.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-18 14:17:32.000000 executor-http-0.1.1/executor_http.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-18 14:17:32.000000 executor-http-0.1.1/executor_http.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:17:32.000000 executor-http-0.1.1/executor_http.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:17:32.000000 executor-http-0.1.1/executor_http.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-18 14:17:32.000000 executor-http-0.1.1/executor_http.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 14:17:32.000000 executor-http-0.1.1/executor_http.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 14:17:32.484866 executor-http-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-18 14:17:14.000000 executor-http-0.1.1/setup.py
```

### Comparing `executor-http-0.1.0/LICENSE` & `executor-http-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `executor-http-0.1.0/PKG-INFO` & `executor-http-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: executor-http
-Version: 0.1.0
+Version: 0.1.1
 Summary: HTTP Server and Client for executor.
 Home-page: https://github.com/Nanguage/executor-http
 Author: Weize Xu
 Author-email: vet.xwz@gmail.com
 License: MIT
 Keywords: Job Management,Web,HTTP
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `executor-http-0.1.0/README.md` & `executor-http-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `executor-http-0.1.0/executor_http.egg-info/PKG-INFO` & `executor-http-0.1.1/executor_http.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: executor-http
-Version: 0.1.0
+Version: 0.1.1
 Summary: HTTP Server and Client for executor.
 Home-page: https://github.com/Nanguage/executor-http
 Author: Weize Xu
 Author-email: vet.xwz@gmail.com
 License: MIT
 Keywords: Job Management,Web,HTTP
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `executor-http-0.1.0/setup.py` & `executor-http-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     author_email='vet.xwz@gmail.com',
     version=get_version(),
     license='MIT',
     description='HTTP Server and Client for executor.',
     long_description=get_long_description(),
     keywords=keywords,
     url=URL,
-    packages=find_namespace_packages(include=["executor/*"]),
+    packages=find_namespace_packages(include=["executor.*"]),
     include_package_data=True,
     zip_safe=False,
     classifiers=classifiers,
     install_requires=get_install_requires(),
     extras_require={
         'dev': requires_dev,
         'dask': requires_dask,
```

