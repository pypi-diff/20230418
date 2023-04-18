# Comparing `tmp/gen3config-1.0.0.tar.gz` & `tmp/gen3config-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3config-1.0.0.tar", last modified: Fri Jun 10 19:57:46 2022, max compression
+gzip compressed data, was "gen3config-1.1.0.tar", last modified: Tue Apr 18 18:30:36 2023, max compression
```

## Comparing `gen3config-1.0.0.tar` & `gen3config-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-06-10 19:57:46.954502 gen3config-1.0.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-06-10 19:56:54.000000 gen3config-1.0.0/CHANGELOG.md
--rw-rw-r--   0 travis    (2000) travis    (2000)    11358 2022-06-10 19:56:54.000000 gen3config-1.0.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      107 2022-06-10 19:56:54.000000 gen3config-1.0.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      558 2022-06-10 19:56:54.000000 gen3config-1.0.0/NOTICE
--rw-rw-r--   0 travis    (2000) travis    (2000)      198 2022-06-10 19:57:46.954502 gen3config-1.0.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      240 2022-06-10 19:56:54.000000 gen3config-1.0.0/Pipfile
--rw-rw-r--   0 travis    (2000) travis    (2000)    21885 2022-06-10 19:56:54.000000 gen3config-1.0.0/Pipfile.lock
--rw-rw-r--   0 travis    (2000) travis    (2000)     2864 2022-06-10 19:56:54.000000 gen3config-1.0.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-06-10 19:57:46.950504 gen3config-1.0.0/gen3config/
--rw-rw-r--   0 travis    (2000) travis    (2000)       37 2022-06-10 19:56:54.000000 gen3config-1.0.0/gen3config/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13371 2022-06-10 19:56:54.000000 gen3config-1.0.0/gen3config/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       25 2022-06-10 19:56:54.000000 gen3config-1.0.0/gen3config/errors.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-06-10 19:57:46.954502 gen3config-1.0.0/gen3config.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      198 2022-06-10 19:57:46.000000 gen3config-1.0.0/gen3config.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      370 2022-06-10 19:57:46.000000 gen3config-1.0.0/gen3config.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-06-10 19:57:46.000000 gen3config-1.0.0/gen3config.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       68 2022-06-10 19:57:46.000000 gen3config-1.0.0/gen3config.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       17 2022-06-10 19:57:46.000000 gen3config-1.0.0/gen3config.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2022-06-10 19:57:46.954502 gen3config-1.0.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1196 2022-06-10 19:57:29.000000 gen3config-1.0.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-06-10 19:57:46.954502 gen3config-1.0.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-06-10 19:56:54.000000 gen3config-1.0.0/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2022-06-10 19:56:54.000000 gen3config-1.0.0/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6748 2022-06-10 19:56:54.000000 gen3config-1.0.0/tests/test_config.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-18 18:30:36.482219 gen3config-1.1.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-18 18:29:52.000000 gen3config-1.1.0/CHANGELOG.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11358 2023-04-18 18:29:52.000000 gen3config-1.1.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      107 2023-04-18 18:29:52.000000 gen3config-1.1.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      558 2023-04-18 18:29:52.000000 gen3config-1.1.0/NOTICE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      198 2023-04-18 18:30:36.482219 gen3config-1.1.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2864 2023-04-18 18:29:52.000000 gen3config-1.1.0/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-18 18:30:36.478217 gen3config-1.1.0/gen3config/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       37 2023-04-18 18:29:52.000000 gen3config-1.1.0/gen3config/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13371 2023-04-18 18:29:52.000000 gen3config-1.1.0/gen3config/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       25 2023-04-18 18:29:52.000000 gen3config-1.1.0/gen3config/errors.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-18 18:30:36.482219 gen3config-1.1.0/gen3config.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      198 2023-04-18 18:30:36.000000 gen3config-1.1.0/gen3config.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      364 2023-04-18 18:30:36.000000 gen3config-1.1.0/gen3config.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-18 18:30:36.000000 gen3config-1.1.0/gen3config.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       41 2023-04-18 18:30:36.000000 gen3config-1.1.0/gen3config.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       17 2023-04-18 18:30:36.000000 gen3config-1.1.0/gen3config.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      556 2023-04-18 18:29:52.000000 gen3config-1.1.0/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-04-18 18:30:36.482219 gen3config-1.1.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2023-04-18 18:30:21.000000 gen3config-1.1.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-18 18:30:36.482219 gen3config-1.1.0/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-18 18:29:52.000000 gen3config-1.1.0/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-04-18 18:29:52.000000 gen3config-1.1.0/tests/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6748 2023-04-18 18:29:52.000000 gen3config-1.1.0/tests/test_config.py
```

### Comparing `gen3config-1.0.0/LICENSE` & `gen3config-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3config-1.0.0/NOTICE` & `gen3config-1.1.0/NOTICE`

 * *Files identical despite different names*

### Comparing `gen3config-1.0.0/README.md` & `gen3config-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gen3config-1.0.0/gen3config/config.py` & `gen3config-1.1.0/gen3config/config.py`

 * *Files identical despite different names*

### Comparing `gen3config-1.0.0/setup.py` & `gen3config-1.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,20 +22,20 @@
             "distribution; please either download the source from PyPI, or check out "
             "from GitHub and make sure that the git CLI is available."
         )
 
 
 setup(
     name="gen3config",
-    version='1.0.0',
+    version='1.1.0',
     description="Gen3 Configuration Library",
     url="https://github.com/uc-cdis/gen3config",
     license="Apache",
     packages=find_packages(),
     install_requires=[
-        "cdiserrors~=1.0",
-        "cdislogging~=1.0",
-        "jinja2~=3.0.0",
-        "PyYAML~=5.1",
-        "six~=1.0",
+        "cdiserrors",
+        "cdislogging",
+        "jinja2",
+        "PyYAML",
+        "six",
     ],
 )
```

### Comparing `gen3config-1.0.0/tests/test_config.py` & `gen3config-1.1.0/tests/test_config.py`

 * *Files identical despite different names*

