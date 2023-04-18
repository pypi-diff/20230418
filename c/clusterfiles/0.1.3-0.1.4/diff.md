# Comparing `tmp/clusterfiles-0.1.3.tar.gz` & `tmp/clusterfiles-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clusterfiles-0.1.3.tar", last modified: Tue Apr 18 14:50:34 2023, max compression
+gzip compressed data, was "clusterfiles-0.1.4.tar", last modified: Tue Apr 18 15:35:53 2023, max compression
```

## Comparing `clusterfiles-0.1.3.tar` & `clusterfiles-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 14:50:34.717558 clusterfiles-0.1.3/
--rw-rw-rw-   0        0        0     1065 2023-04-17 19:44:09.000000 clusterfiles-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      613 2023-04-18 14:50:34.717558 clusterfiles-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       82 2023-04-17 19:41:27.000000 clusterfiles-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 14:50:34.692696 clusterfiles-0.1.3/clusterfiles.egg-info/
--rw-rw-rw-   0        0        0      613 2023-04-18 14:50:34.000000 clusterfiles-0.1.3/clusterfiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      527 2023-04-18 14:50:34.000000 clusterfiles-0.1.3/clusterfiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 14:50:34.000000 clusterfiles-0.1.3/clusterfiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-04-18 14:50:34.000000 clusterfiles-0.1.3/clusterfiles.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-18 14:50:34.000000 clusterfiles-0.1.3/clusterfiles.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-18 14:50:34.692696 clusterfiles-0.1.3/clusterman/
--rw-rw-rw-   0        0        0       25 2023-04-17 20:06:18.000000 clusterfiles-0.1.3/clusterman/__init__.py
--rw-rw-rw-   0        0        0      107 2023-04-17 19:31:46.000000 clusterfiles-0.1.3/clusterman/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 14:50:34.692696 clusterfiles-0.1.3/clusterman/cli/
--rw-rw-rw-   0        0        0        0 2023-04-17 15:50:28.000000 clusterfiles-0.1.3/clusterman/cli/__init__.py
--rw-rw-rw-   0        0        0     1716 2023-04-18 13:08:15.000000 clusterfiles-0.1.3/clusterman/cli/app.py
--rw-rw-rw-   0        0        0     2343 2023-04-18 13:15:06.000000 clusterfiles-0.1.3/clusterman/cli/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-18 14:50:34.715567 clusterfiles-0.1.3/clusterman/main/
--rw-rw-rw-   0        0        0        0 2023-04-17 14:13:30.000000 clusterfiles-0.1.3/clusterman/main/__init__.py
--rw-rw-rw-   0        0        0     6057 2023-04-18 12:00:02.000000 clusterfiles-0.1.3/clusterman/main/ampq.py
--rw-rw-rw-   0        0        0    17516 2023-04-18 13:29:42.000000 clusterfiles-0.1.3/clusterman/main/controller.py
--rw-rw-rw-   0        0        0     3030 2023-04-17 19:55:11.000000 clusterfiles-0.1.3/clusterman/main/mainline.py
--rw-rw-rw-   0        0        0     6403 2023-04-17 17:33:52.000000 clusterfiles-0.1.3/clusterman/main/orm.py
--rw-rw-rw-   0        0        0     6585 2023-04-18 13:28:42.000000 clusterfiles-0.1.3/clusterman/main/processing.py
--rw-rw-rw-   0        0        0     2584 2023-04-17 19:37:59.000000 clusterfiles-0.1.3/clusterman/main/runner.py
--rw-rw-rw-   0        0        0       88 2022-11-14 15:30:25.000000 clusterfiles-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      776 2023-04-18 14:50:34.719560 clusterfiles-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 15:35:53.891598 clusterfiles-0.1.4/
+-rw-rw-rw-   0        0        0     1065 2023-04-17 19:44:09.000000 clusterfiles-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      613 2023-04-18 15:35:53.891598 clusterfiles-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       82 2023-04-17 19:41:27.000000 clusterfiles-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 15:35:53.869348 clusterfiles-0.1.4/clusterfiles.egg-info/
+-rw-rw-rw-   0        0        0      613 2023-04-18 15:35:53.000000 clusterfiles-0.1.4/clusterfiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2023-04-18 15:35:53.000000 clusterfiles-0.1.4/clusterfiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 15:35:53.000000 clusterfiles-0.1.4/clusterfiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-04-18 15:35:53.000000 clusterfiles-0.1.4/clusterfiles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-18 15:35:53.000000 clusterfiles-0.1.4/clusterfiles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 15:35:53.869348 clusterfiles-0.1.4/clusterman/
+-rw-rw-rw-   0        0        0       25 2023-04-18 15:35:24.000000 clusterfiles-0.1.4/clusterman/__init__.py
+-rw-rw-rw-   0        0        0      107 2023-04-17 19:31:46.000000 clusterfiles-0.1.4/clusterman/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:35:53.869348 clusterfiles-0.1.4/clusterman/cli/
+-rw-rw-rw-   0        0        0        0 2023-04-17 15:50:28.000000 clusterfiles-0.1.4/clusterman/cli/__init__.py
+-rw-rw-rw-   0        0        0     1716 2023-04-18 13:08:15.000000 clusterfiles-0.1.4/clusterman/cli/app.py
+-rw-rw-rw-   0        0        0     2343 2023-04-18 13:15:06.000000 clusterfiles-0.1.4/clusterman/cli/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:35:53.891598 clusterfiles-0.1.4/clusterman/main/
+-rw-rw-rw-   0        0        0        0 2023-04-17 14:13:30.000000 clusterfiles-0.1.4/clusterman/main/__init__.py
+-rw-rw-rw-   0        0        0     6057 2023-04-18 12:00:02.000000 clusterfiles-0.1.4/clusterman/main/ampq.py
+-rw-rw-rw-   0        0        0    17516 2023-04-18 13:29:42.000000 clusterfiles-0.1.4/clusterman/main/controller.py
+-rw-rw-rw-   0        0        0     3030 2023-04-17 19:55:11.000000 clusterfiles-0.1.4/clusterman/main/mainline.py
+-rw-rw-rw-   0        0        0     6405 2023-04-18 15:34:57.000000 clusterfiles-0.1.4/clusterman/main/orm.py
+-rw-rw-rw-   0        0        0     6585 2023-04-18 13:28:42.000000 clusterfiles-0.1.4/clusterman/main/processing.py
+-rw-rw-rw-   0        0        0     2584 2023-04-17 19:37:59.000000 clusterfiles-0.1.4/clusterman/main/runner.py
+-rw-rw-rw-   0        0        0       88 2022-11-14 15:30:25.000000 clusterfiles-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      776 2023-04-18 15:35:53.891598 clusterfiles-0.1.4/setup.cfg
```

### Comparing `clusterfiles-0.1.3/LICENSE` & `clusterfiles-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clusterfiles-0.1.3/PKG-INFO` & `clusterfiles-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clusterfiles
-Version: 0.1.3
+Version: 0.1.4
 Summary: Cluster file management for Python
 Home-page: https://github.com/dfo-meds/clusterman
 Author: Erin Turnbull
 Author-email: erin.a.turnbull@gmail.com
 Project-URL: Bug Tracker, https://github.com/dfo-meds/clusterman/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `clusterfiles-0.1.3/clusterfiles.egg-info/PKG-INFO` & `clusterfiles-0.1.4/clusterfiles.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clusterfiles
-Version: 0.1.3
+Version: 0.1.4
 Summary: Cluster file management for Python
 Home-page: https://github.com/dfo-meds/clusterman
 Author: Erin Turnbull
 Author-email: erin.a.turnbull@gmail.com
 Project-URL: Bug Tracker, https://github.com/dfo-meds/clusterman/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `clusterfiles-0.1.3/clusterfiles.egg-info/SOURCES.txt` & `clusterfiles-0.1.4/clusterfiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clusterfiles-0.1.3/clusterman/cli/app.py` & `clusterfiles-0.1.4/clusterman/cli/app.py`

 * *Files identical despite different names*

### Comparing `clusterfiles-0.1.3/clusterman/cli/cli.py` & `clusterfiles-0.1.4/clusterman/cli/cli.py`

 * *Files identical despite different names*

### Comparing `clusterfiles-0.1.3/clusterman/main/ampq.py` & `clusterfiles-0.1.4/clusterman/main/ampq.py`

 * *Files identical despite different names*

### Comparing `clusterfiles-0.1.3/clusterman/main/controller.py` & `clusterfiles-0.1.4/clusterman/main/controller.py`

 * *Files identical despite different names*

### Comparing `clusterfiles-0.1.3/clusterman/main/mainline.py` & `clusterfiles-0.1.4/clusterman/main/mainline.py`

 * *Files identical despite different names*

### Comparing `clusterfiles-0.1.3/clusterman/main/orm.py` & `clusterfiles-0.1.4/clusterman/main/orm.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,10 +185,10 @@
         gate = datetime.datetime.utcnow() + datetime.timedelta(seconds=lock_time)
         st = (
             db.update(LocalObject)
             .values({
                 "locked_by": None,
                 "locked_since": None
             })
-            .where(QueueItem.locked_since < gate)
+            .where(LocalObject.locked_since < gate)
         )
         db.session.execute(st)
```

### Comparing `clusterfiles-0.1.3/clusterman/main/processing.py` & `clusterfiles-0.1.4/clusterman/main/processing.py`

 * *Files identical despite different names*

### Comparing `clusterfiles-0.1.3/clusterman/main/runner.py` & `clusterfiles-0.1.4/clusterman/main/runner.py`

 * *Files identical despite different names*

### Comparing `clusterfiles-0.1.3/setup.cfg` & `clusterfiles-0.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6c75 7374 6572 6669 6c65 730d   = clusterfiles.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e33  .version = 0.1.3
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e34  .version = 0.1.4
 00000030: 0d0a 6175 7468 6f72 203d 2045 7269 6e20  ..author = Erin 
 00000040: 5475 726e 6275 6c6c 0d0a 6175 7468 6f72  Turnbull..author
 00000050: 5f65 6d61 696c 203d 2065 7269 6e2e 612e  _email = erin.a.
 00000060: 7475 726e 6275 6c6c 4067 6d61 696c 2e63  turnbull@gmail.c
 00000070: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000080: 3d20 436c 7573 7465 7220 6669 6c65 206d  = Cluster file m
 00000090: 616e 6167 656d 656e 7420 666f 7220 5079  anagement for Py
```

