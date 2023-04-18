# Comparing `tmp/eltetrado-1.5.8.tar.gz` & `tmp/eltetrado-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eltetrado-1.5.8.tar", last modified: Fri Jan 20 08:38:09 2023, max compression
+gzip compressed data, was "eltetrado-1.5.9.tar", last modified: Fri Jan 20 14:05:03 2023, max compression
```

## Comparing `eltetrado-1.5.8.tar` & `eltetrado-1.5.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-01-20 08:38:09.761440 eltetrado-1.5.8/
--rw-rw-r--   0 tzok      (1000) tzok      (1000)     1068 2020-03-03 11:56:04.000000 eltetrado-1.5.8/LICENSE
--rw-r--r--   0 tzok      (1000) tzok      (1000)       62 2022-05-05 10:39:21.000000 eltetrado-1.5.8/MANIFEST.in
--rw-r--r--   0 tzok      (1000) tzok      (1000)    49689 2023-01-20 08:38:09.764773 eltetrado-1.5.8/PKG-INFO
--rw-r--r--   0 tzok      (1000) tzok      (1000)    48950 2022-10-14 14:42:14.000000 eltetrado-1.5.8/README.md
-drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-01-20 08:38:09.754773 eltetrado-1.5.8/bin/
--rw-r--r--   0 tzok      (1000) tzok      (1000)       75 2022-05-05 10:39:21.000000 eltetrado-1.5.8/bin/eltetrado
--rw-r--r--   0 tzok      (1000) tzok      (1000)       76 2022-05-05 10:39:21.000000 eltetrado-1.5.8/bin/has_tetrad
--rw-r--r--   0 tzok      (1000) tzok      (1000)      100 2022-07-26 10:07:55.000000 eltetrado-1.5.8/pyproject.toml
--rw-r--r--   0 tzok      (1000) tzok      (1000)     1091 2023-01-20 08:38:09.764773 eltetrado-1.5.8/setup.cfg
--rw-r--r--   0 tzok      (1000) tzok      (1000)       38 2022-07-28 16:53:54.000000 eltetrado-1.5.8/setup.py
-drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-01-20 08:38:09.748106 eltetrado-1.5.8/src/
-drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-01-20 08:38:09.758106 eltetrado-1.5.8/src/eltetrado/
--rw-r--r--   0 tzok      (1000) tzok      (1000)        6 2023-01-20 08:37:50.000000 eltetrado-1.5.8/src/eltetrado/VERSION
--rw-r--r--   0 tzok      (1000) tzok      (1000)        0 2021-11-16 14:21:52.000000 eltetrado-1.5.8/src/eltetrado/__init__.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)    52155 2022-12-21 17:02:46.000000 eltetrado-1.5.8/src/eltetrado/analysis.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)     8078 2022-11-30 12:50:24.000000 eltetrado-1.5.8/src/eltetrado/cli.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)     5821 2022-11-30 12:50:24.000000 eltetrado-1.5.8/src/eltetrado/dto.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)     5870 2022-08-25 14:17:27.000000 eltetrado-1.5.8/src/eltetrado/model.py
--rwxr-xr-x   0 tzok      (1000) tzok      (1000)     2380 2022-05-05 10:39:21.000000 eltetrado-1.5.8/src/eltetrado/quadraw.R
-drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-01-20 08:38:09.761440 eltetrado-1.5.8/src/eltetrado.egg-info/
--rw-r--r--   0 tzok      (1000) tzok      (1000)    49689 2023-01-20 08:38:09.000000 eltetrado-1.5.8/src/eltetrado.egg-info/PKG-INFO
--rw-r--r--   0 tzok      (1000) tzok      (1000)      479 2023-01-20 08:38:09.000000 eltetrado-1.5.8/src/eltetrado.egg-info/SOURCES.txt
--rw-r--r--   0 tzok      (1000) tzok      (1000)        1 2023-01-20 08:38:09.000000 eltetrado-1.5.8/src/eltetrado.egg-info/dependency_links.txt
--rw-r--r--   0 tzok      (1000) tzok      (1000)      100 2023-01-20 08:38:09.000000 eltetrado-1.5.8/src/eltetrado.egg-info/entry_points.txt
--rw-r--r--   0 tzok      (1000) tzok      (1000)       28 2023-01-20 08:38:09.000000 eltetrado-1.5.8/src/eltetrado.egg-info/requires.txt
--rw-r--r--   0 tzok      (1000) tzok      (1000)       10 2023-01-20 08:38:09.000000 eltetrado-1.5.8/src/eltetrado.egg-info/top_level.txt
+drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-01-20 14:05:03.139725 eltetrado-1.5.9/
+-rw-rw-r--   0 tzok      (1000) tzok      (1000)     1068 2020-03-03 11:56:04.000000 eltetrado-1.5.9/LICENSE
+-rw-r--r--   0 tzok      (1000) tzok      (1000)       62 2022-05-05 10:39:21.000000 eltetrado-1.5.9/MANIFEST.in
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    49689 2023-01-20 14:05:03.139725 eltetrado-1.5.9/PKG-INFO
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    48950 2022-10-14 14:42:14.000000 eltetrado-1.5.9/README.md
+drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-01-20 14:05:03.136392 eltetrado-1.5.9/bin/
+-rw-r--r--   0 tzok      (1000) tzok      (1000)       75 2022-05-05 10:39:21.000000 eltetrado-1.5.9/bin/eltetrado
+-rw-r--r--   0 tzok      (1000) tzok      (1000)       76 2022-05-05 10:39:21.000000 eltetrado-1.5.9/bin/has_tetrad
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      100 2022-07-26 10:07:55.000000 eltetrado-1.5.9/pyproject.toml
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     1091 2023-01-20 14:05:03.139725 eltetrado-1.5.9/setup.cfg
+-rw-r--r--   0 tzok      (1000) tzok      (1000)       38 2022-07-28 16:53:54.000000 eltetrado-1.5.9/setup.py
+drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-01-20 14:05:03.133058 eltetrado-1.5.9/src/
+drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-01-20 14:05:03.136392 eltetrado-1.5.9/src/eltetrado/
+-rw-r--r--   0 tzok      (1000) tzok      (1000)        6 2023-01-20 14:04:26.000000 eltetrado-1.5.9/src/eltetrado/VERSION
+-rw-r--r--   0 tzok      (1000) tzok      (1000)        0 2021-11-16 14:21:52.000000 eltetrado-1.5.9/src/eltetrado/__init__.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    52155 2022-12-21 17:02:46.000000 eltetrado-1.5.9/src/eltetrado/analysis.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     8078 2022-11-30 12:50:24.000000 eltetrado-1.5.9/src/eltetrado/cli.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     5974 2023-01-20 14:04:26.000000 eltetrado-1.5.9/src/eltetrado/dto.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     5870 2022-08-25 14:17:27.000000 eltetrado-1.5.9/src/eltetrado/model.py
+-rwxr-xr-x   0 tzok      (1000) tzok      (1000)     2380 2022-05-05 10:39:21.000000 eltetrado-1.5.9/src/eltetrado/quadraw.R
+drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-01-20 14:05:03.139725 eltetrado-1.5.9/src/eltetrado.egg-info/
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    49689 2023-01-20 14:05:03.000000 eltetrado-1.5.9/src/eltetrado.egg-info/PKG-INFO
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      479 2023-01-20 14:05:03.000000 eltetrado-1.5.9/src/eltetrado.egg-info/SOURCES.txt
+-rw-r--r--   0 tzok      (1000) tzok      (1000)        1 2023-01-20 14:05:03.000000 eltetrado-1.5.9/src/eltetrado.egg-info/dependency_links.txt
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      100 2023-01-20 14:05:03.000000 eltetrado-1.5.9/src/eltetrado.egg-info/entry_points.txt
+-rw-r--r--   0 tzok      (1000) tzok      (1000)       28 2023-01-20 14:05:03.000000 eltetrado-1.5.9/src/eltetrado.egg-info/requires.txt
+-rw-r--r--   0 tzok      (1000) tzok      (1000)       10 2023-01-20 14:05:03.000000 eltetrado-1.5.9/src/eltetrado.egg-info/top_level.txt
```

### Comparing `eltetrado-1.5.8/LICENSE` & `eltetrado-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eltetrado-1.5.8/PKG-INFO` & `eltetrado-1.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eltetrado
-Version: 1.5.8
+Version: 1.5.9
 Summary: Find and classify tetrads and quadruplexes in DNA/RNA 3D structure
 Home-page: https://github.com/tzok/eltetrado
 Author: Tomasz Żok
 Author-email: tomasz.zok@cs.put.poznan.pl
 Project-URL: Bug Tracker, https://github.com/tzok/eltetrado/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `eltetrado-1.5.8/README.md` & `eltetrado-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `eltetrado-1.5.8/setup.cfg` & `eltetrado-1.5.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `eltetrado-1.5.8/src/eltetrado/analysis.py` & `eltetrado-1.5.9/src/eltetrado/analysis.py`

 * *Files identical despite different names*

### Comparing `eltetrado-1.5.8/src/eltetrado/cli.py` & `eltetrado-1.5.9/src/eltetrado/cli.py`

 * *Files identical despite different names*

### Comparing `eltetrado-1.5.8/src/eltetrado/dto.py` & `eltetrado-1.5.9/src/eltetrado/dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,17 +213,21 @@
             ],
         )
         for q in helix.quadruplexes
     ]
 
 
 def convert_helices(analysis: Analysis) -> List[HelixDTO]:
+    """
+    NOTE: there is an "if" which will prevent single-tetrad helices from serialization; this is on purpose
+    """
     return [
         HelixDTO(convert_quadruplexes(h), convert_tetrad_pairs(h))
         for h in analysis.helices
+        if len(h.tetrads) > 1
     ]
 
 
 def convert_dot_bracket(analysis: Analysis) -> TwoLineDotBracketDTO:
     return TwoLineDotBracketDTO(analysis.sequence, analysis.line1, analysis.line2)
```

### Comparing `eltetrado-1.5.8/src/eltetrado/model.py` & `eltetrado-1.5.9/src/eltetrado/model.py`

 * *Files identical despite different names*

### Comparing `eltetrado-1.5.8/src/eltetrado/quadraw.R` & `eltetrado-1.5.9/src/eltetrado/quadraw.R`

 * *Files identical despite different names*

### Comparing `eltetrado-1.5.8/src/eltetrado.egg-info/PKG-INFO` & `eltetrado-1.5.9/src/eltetrado.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eltetrado
-Version: 1.5.8
+Version: 1.5.9
 Summary: Find and classify tetrads and quadruplexes in DNA/RNA 3D structure
 Home-page: https://github.com/tzok/eltetrado
 Author: Tomasz Żok
 Author-email: tomasz.zok@cs.put.poznan.pl
 Project-URL: Bug Tracker, https://github.com/tzok/eltetrado/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

