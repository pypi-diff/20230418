# Comparing `tmp/userdatamodel-2.4.0.tar.gz` & `tmp/userdatamodel-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/userdatamodel-2.4.0.tar", last modified: Tue Nov 23 18:47:11 2021, max compression
+gzip compressed data, was "userdatamodel-2.4.3.tar", last modified: Tue Apr 18 19:11:00 2023, max compression
```

## Comparing `userdatamodel-2.4.0.tar` & `userdatamodel-2.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-23 18:47:11.000000 userdatamodel-2.4.0/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-23 18:47:11.000000 userdatamodel-2.4.0/bin/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      992 2021-11-23 18:46:45.000000 userdatamodel-2.4.0/bin/userdatamodel-init
--rw-rw-r--   0 travis    (2000) travis    (2000)      558 2021-11-23 18:46:45.000000 userdatamodel-2.4.0/NOTICE
--rw-rw-r--   0 travis    (2000) travis    (2000)      836 2021-11-23 18:46:55.000000 userdatamodel-2.4.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-23 18:47:11.000000 userdatamodel-2.4.0/userdatamodel.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      400 2021-11-23 18:47:11.000000 userdatamodel-2.4.0/userdatamodel.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      181 2021-11-23 18:47:11.000000 userdatamodel-2.4.0/userdatamodel.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)       30 2021-11-23 18:47:11.000000 userdatamodel-2.4.0/userdatamodel.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2021-11-23 18:47:11.000000 userdatamodel-2.4.0/userdatamodel.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-11-23 18:47:11.000000 userdatamodel-2.4.0/userdatamodel.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       51 2021-11-23 18:46:45.000000 userdatamodel-2.4.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      974 2021-11-23 18:46:45.000000 userdatamodel-2.4.0/Pipfile.lock
--rw-rw-r--   0 travis    (2000) travis    (2000)      181 2021-11-23 18:47:11.000000 userdatamodel-2.4.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      206 2021-11-23 18:46:45.000000 userdatamodel-2.4.0/Pipfile
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-11-23 18:47:11.000000 userdatamodel-2.4.0/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-23 18:47:11.000000 userdatamodel-2.4.0/userdatamodel/
--rw-rw-r--   0 travis    (2000) travis    (2000)      435 2021-11-23 18:46:45.000000 userdatamodel-2.4.0/userdatamodel/init_defaults.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19609 2021-11-23 18:46:45.000000 userdatamodel-2.4.0/userdatamodel/user.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      375 2021-11-23 18:46:45.000000 userdatamodel-2.4.0/userdatamodel/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       84 2021-11-23 18:46:45.000000 userdatamodel-2.4.0/userdatamodel/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6905 2021-11-23 18:46:45.000000 userdatamodel-2.4.0/userdatamodel/driver.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       68 2021-11-23 18:46:45.000000 userdatamodel-2.4.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2021-11-23 18:46:45.000000 userdatamodel-2.4.0/LICENSE
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-18 19:11:00.330649 userdatamodel-2.4.3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2023-04-18 19:10:21.000000 userdatamodel-2.4.3/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       68 2023-04-18 19:10:21.000000 userdatamodel-2.4.3/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      558 2023-04-18 19:10:21.000000 userdatamodel-2.4.3/NOTICE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-04-18 19:11:00.330649 userdatamodel-2.4.3/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      206 2023-04-18 19:10:21.000000 userdatamodel-2.4.3/Pipfile
+-rw-rw-r--   0 travis    (2000) travis    (2000)      974 2023-04-18 19:10:21.000000 userdatamodel-2.4.3/Pipfile.lock
+-rw-rw-r--   0 travis    (2000) travis    (2000)       51 2023-04-18 19:10:21.000000 userdatamodel-2.4.3/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-18 19:11:00.326646 userdatamodel-2.4.3/bin/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      992 2023-04-18 19:10:21.000000 userdatamodel-2.4.3/bin/userdatamodel-init
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-04-18 19:11:00.330649 userdatamodel-2.4.3/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      836 2023-04-18 19:10:44.000000 userdatamodel-2.4.3/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-18 19:11:00.326646 userdatamodel-2.4.3/userdatamodel/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       84 2023-04-18 19:10:21.000000 userdatamodel-2.4.3/userdatamodel/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6905 2023-04-18 19:10:21.000000 userdatamodel-2.4.3/userdatamodel/driver.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      435 2023-04-18 19:10:21.000000 userdatamodel-2.4.3/userdatamodel/init_defaults.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      375 2023-04-18 19:10:21.000000 userdatamodel-2.4.3/userdatamodel/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19609 2023-04-18 19:10:21.000000 userdatamodel-2.4.3/userdatamodel/user.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-18 19:11:00.330649 userdatamodel-2.4.3/userdatamodel.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-04-18 19:11:00.000000 userdatamodel-2.4.3/userdatamodel.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      400 2023-04-18 19:11:00.000000 userdatamodel-2.4.3/userdatamodel.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-18 19:11:00.000000 userdatamodel-2.4.3/userdatamodel.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       30 2023-04-18 19:11:00.000000 userdatamodel-2.4.3/userdatamodel.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-04-18 19:11:00.000000 userdatamodel-2.4.3/userdatamodel.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `userdatamodel-2.4.0/bin/userdatamodel-init` & `userdatamodel-2.4.3/bin/userdatamodel-init`

 * *Files identical despite different names*

### Comparing `userdatamodel-2.4.0/NOTICE` & `userdatamodel-2.4.3/NOTICE`

 * *Files identical despite different names*

### Comparing `userdatamodel-2.4.0/setup.py` & `userdatamodel-2.4.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,12 +16,12 @@
             "distribution; please either download the source from PyPI, or check out "
             "from GitHub and make sure that the git CLI is available."
         )
 
 
 setup(
     name="userdatamodel",
-    version='2.4.0',
+    version='2.4.3',
     packages=find_packages(),
-    install_requires=["sqlalchemy~=1.3.3", "cdislogging"],
+    install_requires=["sqlalchemy>=1.3.3", "cdislogging"],
     scripts=["bin/userdatamodel-init"],
 )
```

### Comparing `userdatamodel-2.4.0/Pipfile.lock` & `userdatamodel-2.4.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `userdatamodel-2.4.0/userdatamodel/user.py` & `userdatamodel-2.4.3/userdatamodel/user.py`

 * *Files identical despite different names*

### Comparing `userdatamodel-2.4.0/userdatamodel/driver.py` & `userdatamodel-2.4.3/userdatamodel/driver.py`

 * *Files identical despite different names*

### Comparing `userdatamodel-2.4.0/LICENSE` & `userdatamodel-2.4.3/LICENSE`

 * *Files identical despite different names*

