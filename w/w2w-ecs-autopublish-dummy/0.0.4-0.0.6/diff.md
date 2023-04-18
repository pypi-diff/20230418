# Comparing `tmp/w2w_ecs_autopublish_dummy-0.0.4.tar.gz` & `tmp/w2w_ecs_autopublish_dummy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w2w_ecs_autopublish_dummy-0.0.4.tar", last modified: Tue Apr 18 09:02:51 2023, max compression
+gzip compressed data, was "w2w_ecs_autopublish_dummy-0.0.6.tar", last modified: Tue Apr 18 09:56:58 2023, max compression
```

## Comparing `w2w_ecs_autopublish_dummy-0.0.4.tar` & `w2w_ecs_autopublish_dummy-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 09:02:51.668206 w2w_ecs_autopublish_dummy-0.0.4/
--rw-r--r--   0 root         (0) root         (0)      472 2023-04-18 09:02:51.668206 w2w_ecs_autopublish_dummy-0.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-04-18 08:59:45.000000 w2w_ecs_autopublish_dummy-0.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 09:02:51.668206 w2w_ecs_autopublish_dummy-0.0.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 09:02:51.667206 w2w_ecs_autopublish_dummy-0.0.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)      290 2023-04-18 08:49:33.000000 w2w_ecs_autopublish_dummy-0.0.4/tests/test_main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 09:02:51.667206 w2w_ecs_autopublish_dummy-0.0.4/w2w_ecs_autopublish_dummy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 08:49:33.000000 w2w_ecs_autopublish_dummy-0.0.4/w2w_ecs_autopublish_dummy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-04-18 08:49:33.000000 w2w_ecs_autopublish_dummy-0.0.4/w2w_ecs_autopublish_dummy/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 09:02:51.668206 w2w_ecs_autopublish_dummy-0.0.4/w2w_ecs_autopublish_dummy.egg-info/
--rw-r--r--   0 root         (0) root         (0)      472 2023-04-18 09:02:51.000000 w2w_ecs_autopublish_dummy-0.0.4/w2w_ecs_autopublish_dummy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      353 2023-04-18 09:02:51.000000 w2w_ecs_autopublish_dummy-0.0.4/w2w_ecs_autopublish_dummy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 09:02:51.000000 w2w_ecs_autopublish_dummy-0.0.4/w2w_ecs_autopublish_dummy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-04-18 09:02:51.000000 w2w_ecs_autopublish_dummy-0.0.4/w2w_ecs_autopublish_dummy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-18 09:02:51.000000 w2w_ecs_autopublish_dummy-0.0.4/w2w_ecs_autopublish_dummy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 09:56:58.203410 w2w_ecs_autopublish_dummy-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-04-18 09:56:58.203410 w2w_ecs_autopublish_dummy-0.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      688 2023-04-18 09:28:39.000000 w2w_ecs_autopublish_dummy-0.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 09:56:58.203410 w2w_ecs_autopublish_dummy-0.0.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 09:56:58.202410 w2w_ecs_autopublish_dummy-0.0.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      309 2023-04-18 09:28:39.000000 w2w_ecs_autopublish_dummy-0.0.6/tests/test_main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 09:56:58.202410 w2w_ecs_autopublish_dummy-0.0.6/w2w_ecs_autopublish_dummy/
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-04-18 09:28:39.000000 w2w_ecs_autopublish_dummy-0.0.6/w2w_ecs_autopublish_dummy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-18 09:28:39.000000 w2w_ecs_autopublish_dummy-0.0.6/w2w_ecs_autopublish_dummy/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 09:56:58.203410 w2w_ecs_autopublish_dummy-0.0.6/w2w_ecs_autopublish_dummy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-04-18 09:56:58.000000 w2w_ecs_autopublish_dummy-0.0.6/w2w_ecs_autopublish_dummy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      353 2023-04-18 09:56:58.000000 w2w_ecs_autopublish_dummy-0.0.6/w2w_ecs_autopublish_dummy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 09:56:58.000000 w2w_ecs_autopublish_dummy-0.0.6/w2w_ecs_autopublish_dummy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2023-04-18 09:56:58.000000 w2w_ecs_autopublish_dummy-0.0.6/w2w_ecs_autopublish_dummy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-18 09:56:58.000000 w2w_ecs_autopublish_dummy-0.0.6/w2w_ecs_autopublish_dummy.egg-info/top_level.txt
```

### Comparing `w2w_ecs_autopublish_dummy-0.0.4/pyproject.toml` & `w2w_ecs_autopublish_dummy-0.0.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "w2w_ecs_autopublish_dummy"
-version = "0.0.4"
+version = "0.0.6"
 authors = [
     { name = "Oriol Tintó", email = "oriol.tinto@lmu.de" },
 ]
 description = "A test to try PYPI package publishing using CI."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = []
 [project.scripts]
-autopublished = "AutoPublishTest.main:main"
+autopublished = "w2w_ecs_autopublish_dummy.main:launcher"
 
 [project.urls]
-"Homepage" = "https://gitlab.physik.uni-muenchen.de/Oriol.Tinto/autopublishtest"
+"Homepage" = "https://gitlab.physik.uni-muenchen.de/Oriol.Tinto/w2w_ecs_autopublish_dummy"
```

