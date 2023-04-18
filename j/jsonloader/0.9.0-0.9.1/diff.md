# Comparing `tmp/jsonloader-0.9.0.tar.gz` & `tmp/jsonloader-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonloader-0.9.0.tar", last modified: Sun Mar 19 17:00:49 2023, max compression
+gzip compressed data, was "jsonloader-0.9.1.tar", last modified: Tue Apr 18 16:07:13 2023, max compression
```

## Comparing `jsonloader-0.9.0.tar` & `jsonloader-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-03-19 17:00:49.150528 jsonloader-0.9.0/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1080 2022-02-20 15:14:23.000000 jsonloader-0.9.0/LICENSE
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     4558 2023-03-19 17:00:49.150528 jsonloader-0.9.0/PKG-INFO
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     3876 2023-03-19 16:44:21.000000 jsonloader-0.9.0/README.md
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-03-19 17:00:49.150528 jsonloader-0.9.0/jsonloader/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      453 2023-03-19 16:49:15.000000 jsonloader-0.9.0/jsonloader/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    13280 2023-03-19 16:48:37.000000 jsonloader-0.9.0/jsonloader/jsonloader.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1481 2022-03-13 19:57:15.000000 jsonloader-0.9.0/jsonloader/jsonloader2.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-03-19 17:00:49.150528 jsonloader-0.9.0/jsonloader.egg-info/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     4558 2023-03-19 17:00:49.000000 jsonloader-0.9.0/jsonloader.egg-info/PKG-INFO
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      309 2023-03-19 17:00:49.000000 jsonloader-0.9.0/jsonloader.egg-info/SOURCES.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)        1 2023-03-19 17:00:49.000000 jsonloader-0.9.0/jsonloader.egg-info/dependency_links.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      132 2023-03-19 17:00:49.000000 jsonloader-0.9.0/jsonloader.egg-info/requires.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)       11 2023-03-19 17:00:49.000000 jsonloader-0.9.0/jsonloader.egg-info/top_level.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      149 2022-03-13 20:55:23.000000 jsonloader-0.9.0/pyproject.toml
--rw-rw-r--   0 laumas    (1000) laumas    (1000)       38 2023-03-19 17:00:49.150528 jsonloader-0.9.0/setup.cfg
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1654 2023-03-19 16:43:43.000000 jsonloader-0.9.0/setup.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-03-19 17:00:49.150528 jsonloader-0.9.0/tests/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     8018 2023-03-19 16:45:44.000000 jsonloader-0.9.0/tests/test_jsonloader.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-04-18 16:07:13.266924 jsonloader-0.9.1/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1080 2022-02-20 15:14:23.000000 jsonloader-0.9.1/LICENSE
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     4558 2023-04-18 16:07:13.266924 jsonloader-0.9.1/PKG-INFO
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     3876 2023-03-19 16:44:21.000000 jsonloader-0.9.1/README.md
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-04-18 16:07:13.266924 jsonloader-0.9.1/jsonloader/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      453 2023-03-19 16:49:15.000000 jsonloader-0.9.1/jsonloader/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    13280 2023-03-19 16:48:37.000000 jsonloader-0.9.1/jsonloader/jsonloader.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1481 2022-03-13 19:57:15.000000 jsonloader-0.9.1/jsonloader/jsonloader2.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-04-18 16:07:13.266924 jsonloader-0.9.1/jsonloader.egg-info/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     4558 2023-04-18 16:07:13.000000 jsonloader-0.9.1/jsonloader.egg-info/PKG-INFO
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      309 2023-04-18 16:07:13.000000 jsonloader-0.9.1/jsonloader.egg-info/SOURCES.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)        1 2023-04-18 16:07:13.000000 jsonloader-0.9.1/jsonloader.egg-info/dependency_links.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      139 2023-04-18 16:07:13.000000 jsonloader-0.9.1/jsonloader.egg-info/requires.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)       11 2023-04-18 16:07:13.000000 jsonloader-0.9.1/jsonloader.egg-info/top_level.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      149 2022-03-13 20:55:23.000000 jsonloader-0.9.1/pyproject.toml
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)       38 2023-04-18 16:07:13.266924 jsonloader-0.9.1/setup.cfg
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1662 2023-04-18 15:44:37.000000 jsonloader-0.9.1/setup.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-04-18 16:07:13.266924 jsonloader-0.9.1/tests/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     8018 2023-03-19 16:45:44.000000 jsonloader-0.9.1/tests/test_jsonloader.py
```

### Comparing `jsonloader-0.9.0/LICENSE` & `jsonloader-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonloader-0.9.0/PKG-INFO` & `jsonloader-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonloader
-Version: 0.9.0
+Version: 0.9.1
 Summary: No more boilerplate to check and build a Python object from JSON.
 Home-page: https://github.com/OhMajesticLama/jsonloader
 Author-email: ohmajesticlama@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jsonloader-0.9.0/README.md` & `jsonloader-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `jsonloader-0.9.0/jsonloader/jsonloader.py` & `jsonloader-0.9.1/jsonloader/jsonloader.py`

 * *Files identical despite different names*

### Comparing `jsonloader-0.9.0/jsonloader/jsonloader2.py` & `jsonloader-0.9.1/jsonloader/jsonloader2.py`

 * *Files identical despite different names*

### Comparing `jsonloader-0.9.0/jsonloader.egg-info/PKG-INFO` & `jsonloader-0.9.1/jsonloader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonloader
-Version: 0.9.0
+Version: 0.9.1
 Summary: No more boilerplate to check and build a Python object from JSON.
 Home-page: https://github.com/OhMajesticLama/jsonloader
 Author-email: ohmajesticlama@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jsonloader-0.9.0/setup.py` & `jsonloader-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 
     readme_path = os.path.join(os.path.dirname(__file__), 'README.md')
     with open(readme_path, "r") as fh:
         long_description = fh.read()
 
     setuptools.setup(
         name="jsonloader",
-        version="0.9.0",
+        version="0.9.1",
         author_email="ohmajesticlama@gmail.com",
         description=description_short,
         long_description=long_description,
         long_description_content_type='text/markdown',
         url="https://github.com/OhMajesticLama/jsonloader",
         packages=setuptools.find_packages(),
         python_requires=">=3.8.10",
         install_requires=[
-            'typeguard >= 3.0.1'
+            'typeguard >= 3.0.1, <4.0.0'
             ],
         extras_require={
             'dev': [
                 'pytest >= 7.0.1',
                 'mypy >= 0.931',
                 'coverage >= 6.3',
                 'build >= 0.7.0',
```

### Comparing `jsonloader-0.9.0/tests/test_jsonloader.py` & `jsonloader-0.9.1/tests/test_jsonloader.py`

 * *Files identical despite different names*

