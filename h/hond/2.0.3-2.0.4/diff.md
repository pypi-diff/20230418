# Comparing `tmp/hond-2.0.3.tar.gz` & `tmp/hond-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hond-2.0.3.tar", last modified: Mon Apr 17 21:13:51 2023, max compression
+gzip compressed data, was "hond-2.0.4.tar", last modified: Mon Apr 17 23:39:38 2023, max compression
```

## Comparing `hond-2.0.3.tar` & `hond-2.0.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:13:51.270404 hond-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-17 21:13:17.000000 hond-2.0.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:13:51.262404 hond-2.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-17 21:13:17.000000 hond-2.0.3/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-17 21:13:17.000000 hond-2.0.3/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:13:51.262404 hond-2.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-17 21:13:17.000000 hond-2.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-17 21:13:17.000000 hond-2.0.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:13:51.266404 hond-2.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-17 21:13:17.000000 hond-2.0.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-17 21:13:17.000000 hond-2.0.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-17 21:13:17.000000 hond-2.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-17 21:13:17.000000 hond-2.0.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-17 21:13:17.000000 hond-2.0.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-17 21:13:17.000000 hond-2.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-17 21:13:17.000000 hond-2.0.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-17 21:13:17.000000 hond-2.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-17 21:13:17.000000 hond-2.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-17 21:13:51.270404 hond-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-17 21:13:17.000000 hond-2.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:13:51.266404 hond-2.0.3/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 21:13:17.000000 hond-2.0.3/cache/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:13:51.266404 hond-2.0.3/chart/
--rw-r--r--   0 runner    (1001) docker     (123)    16006 2023-04-17 21:13:17.000000 hond-2.0.3/chart/chart.excalidraw
--rw-r--r--   0 runner    (1001) docker     (123)    74544 2023-04-17 21:13:17.000000 hond-2.0.3/chart/chart.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:13:51.266404 hond-2.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-17 21:13:17.000000 hond-2.0.3/examples/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-17 21:13:17.000000 hond-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-17 21:13:17.000000 hond-2.0.3/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-17 21:13:51.270404 hond-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-17 21:13:17.000000 hond-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:13:51.258404 hond-2.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:13:51.266404 hond-2.0.3/src/hond/
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-17 21:13:17.000000 hond-2.0.3/src/hond/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:13:51.266404 hond-2.0.3/src/hond/driver/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-17 21:13:17.000000 hond-2.0.3/src/hond/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-04-17 21:13:17.000000 hond-2.0.3/src/hond/driver/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-17 21:13:17.000000 hond-2.0.3/src/hond/hond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-17 21:13:17.000000 hond-2.0.3/src/hond/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-17 21:13:17.000000 hond-2.0.3/src/hond/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-17 21:13:17.000000 hond-2.0.3/src/hond/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:13:51.266404 hond-2.0.3/src/hond.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-17 21:13:51.000000 hond-2.0.3/src/hond.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-17 21:13:51.000000 hond-2.0.3/src/hond.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 21:13:51.000000 hond-2.0.3/src/hond.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 21:13:50.000000 hond-2.0.3/src/hond.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-17 21:13:51.000000 hond-2.0.3/src/hond.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 21:13:51.000000 hond-2.0.3/src/hond.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:13:51.266404 hond-2.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-17 21:13:17.000000 hond-2.0.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:13:51.270404 hond-2.0.3/tests/datastore/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-17 21:13:17.000000 hond-2.0.3/tests/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-17 21:13:17.000000 hond-2.0.3/tests/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-17 21:13:17.000000 hond-2.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:39:38.807843 hond-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-17 23:39:03.000000 hond-2.0.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:39:38.803843 hond-2.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-17 23:39:03.000000 hond-2.0.4/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-17 23:39:03.000000 hond-2.0.4/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:39:38.803843 hond-2.0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-17 23:39:03.000000 hond-2.0.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-17 23:39:03.000000 hond-2.0.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:39:38.803843 hond-2.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-17 23:39:03.000000 hond-2.0.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-17 23:39:03.000000 hond-2.0.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-17 23:39:03.000000 hond-2.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-17 23:39:03.000000 hond-2.0.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-17 23:39:03.000000 hond-2.0.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-17 23:39:03.000000 hond-2.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-17 23:39:03.000000 hond-2.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-17 23:39:03.000000 hond-2.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-17 23:39:03.000000 hond-2.0.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-17 23:39:38.807843 hond-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-17 23:39:03.000000 hond-2.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:39:38.803843 hond-2.0.4/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 23:39:03.000000 hond-2.0.4/cache/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:39:38.803843 hond-2.0.4/chart/
+-rw-r--r--   0 runner    (1001) docker     (123)    15993 2023-04-17 23:39:03.000000 hond-2.0.4/chart/chart.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (123)    75254 2023-04-17 23:39:03.000000 hond-2.0.4/chart/chart.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:39:38.803843 hond-2.0.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-17 23:39:03.000000 hond-2.0.4/examples/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-17 23:39:03.000000 hond-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-17 23:39:03.000000 hond-2.0.4/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-17 23:39:38.811843 hond-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-17 23:39:03.000000 hond-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:39:38.795843 hond-2.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:39:38.807843 hond-2.0.4/src/hond/
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-17 23:39:03.000000 hond-2.0.4/src/hond/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:39:38.807843 hond-2.0.4/src/hond/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-17 23:39:03.000000 hond-2.0.4/src/hond/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-04-17 23:39:03.000000 hond-2.0.4/src/hond/driver/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-17 23:39:03.000000 hond-2.0.4/src/hond/hond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-17 23:39:03.000000 hond-2.0.4/src/hond/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-17 23:39:03.000000 hond-2.0.4/src/hond/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-17 23:39:03.000000 hond-2.0.4/src/hond/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:39:38.807843 hond-2.0.4/src/hond.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-17 23:39:38.000000 hond-2.0.4/src/hond.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-17 23:39:38.000000 hond-2.0.4/src/hond.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:39:38.000000 hond-2.0.4/src/hond.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:39:38.000000 hond-2.0.4/src/hond.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-17 23:39:38.000000 hond-2.0.4/src/hond.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 23:39:38.000000 hond-2.0.4/src/hond.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:39:38.807843 hond-2.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-17 23:39:03.000000 hond-2.0.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:39:38.807843 hond-2.0.4/tests/datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-17 23:39:03.000000 hond-2.0.4/tests/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-17 23:39:03.000000 hond-2.0.4/tests/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-17 23:39:03.000000 hond-2.0.4/tox.ini
```

### Comparing `hond-2.0.3/.coveragerc` & `hond-2.0.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/.github/workflows/release.yml` & `hond-2.0.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/.gitignore` & `hond-2.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/CODE_OF_CONDUCT.md` & `hond-2.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/CONTRIBUTING.rst` & `hond-2.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/LICENSE.txt` & `hond-2.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/Makefile` & `hond-2.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/PKG-INFO` & `hond-2.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hond
-Version: 2.0.3
+Version: 2.0.4
 Summary: Metrics Ingestion and Alerting Reimagined.
 Home-page: https://github.com/uptimedog/hond/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/uptimedog/hond/
 Project-URL: Source, https://github.com/uptimedog/hond/
```

### Comparing `hond-2.0.3/README.rst` & `hond-2.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/chart/chart.excalidraw` & `hond-2.0.4/chart/chart.excalidraw`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991582491582491%*

 * *Differences: {"'elements'": "{14: {'x': -57.002355381084385, 'width': 628.125, 'height': 96, 'version': 227, "*

 * *               "'versionNonce': 2033313643, 'boundElements': [], 'updated': 1681774566990, "*

 * *               "'fontFamily': 3, 'baseline': 92, 'lineHeight': 1.2}}"}*

```diff
@@ -587,44 +587,44 @@
             "width": 169.76873656726355,
             "x": -195.32485267610008,
             "y": -123.13950094062196
         },
         {
             "angle": 0,
             "backgroundColor": "transparent",
-            "baseline": 94,
-            "boundElements": null,
+            "baseline": 92,
+            "boundElements": [],
             "containerId": null,
             "fillStyle": "hachure",
-            "fontFamily": 1,
+            "fontFamily": 3,
             "fontSize": 16,
             "groupIds": [],
-            "height": 100,
+            "height": 96,
             "id": "g21nsMk7w7rR29CSLWzKy",
             "isDeleted": false,
-            "lineHeight": 1.25,
+            "lineHeight": 1.2,
             "link": null,
             "locked": false,
             "opacity": 100,
             "originalText": "            m{hond.xxx.cpu>=20}[30s]\n            m{hond.xxx.cpu<20}[30s]\n            m{hond.xxx.cpu==nul}[30s]\n            m{hond.xxx.cpu==nul}[30s] and m{hond.xxx.mem==nul}[30s]\n            m{hond.xxx.cpu==nul}[30s] or m{hond.xxx.mem==nul}[30s]",
             "roughness": 1,
             "roundness": null,
             "seed": 1460590525,
             "strokeColor": "#000000",
             "strokeStyle": "solid",
             "strokeWidth": 1,
             "text": "            m{hond.xxx.cpu>=20}[30s]\n            m{hond.xxx.cpu<20}[30s]\n            m{hond.xxx.cpu==nul}[30s]\n            m{hond.xxx.cpu==nul}[30s] and m{hond.xxx.mem==nul}[30s]\n            m{hond.xxx.cpu==nul}[30s] or m{hond.xxx.mem==nul}[30s]",
             "textAlign": "left",
             "type": "text",
-            "updated": 1681678784298,
-            "version": 192,
-            "versionNonce": 490408883,
+            "updated": 1681774566990,
+            "version": 227,
+            "versionNonce": 2033313643,
             "verticalAlign": "top",
-            "width": 559.8236694335938,
-            "x": -20.858312412334385,
+            "width": 628.125,
+            "x": -57.002355381084385,
             "y": -13.502798702787686
         }
     ],
     "files": {},
     "source": "https://excalidraw.com",
     "type": "excalidraw",
     "version": 2
```

### Comparing `hond-2.0.3/examples/basic.py` & `hond-2.0.4/examples/basic.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/setup.cfg` & `hond-2.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/setup.py` & `hond-2.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/src/hond/__init__.py` & `hond-2.0.4/src/hond/__init__.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/src/hond/driver/__init__.py` & `hond-2.0.4/src/hond/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/src/hond/driver/elasticsearch.py` & `hond-2.0.4/src/hond/driver/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/src/hond/hond.py` & `hond-2.0.4/src/hond/hond.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/src/hond/logger.py` & `hond-2.0.4/src/hond/logger.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/src/hond/metric.py` & `hond-2.0.4/src/hond/metric.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/src/hond/trigger.py` & `hond-2.0.4/src/hond/trigger.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/src/hond.egg-info/PKG-INFO` & `hond-2.0.4/src/hond.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hond
-Version: 2.0.3
+Version: 2.0.4
 Summary: Metrics Ingestion and Alerting Reimagined.
 Home-page: https://github.com/uptimedog/hond/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/uptimedog/hond/
 Project-URL: Source, https://github.com/uptimedog/hond/
```

### Comparing `hond-2.0.3/src/hond.egg-info/SOURCES.txt` & `hond-2.0.4/src/hond.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/tests/__init__.py` & `hond-2.0.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/tests/datastore/__init__.py` & `hond-2.0.4/tests/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/tests/test_metric.py` & `hond-2.0.4/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.3/tox.ini` & `hond-2.0.4/tox.ini`

 * *Files identical despite different names*

