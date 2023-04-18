# Comparing `tmp/pytmt-0.4.2.tar.gz` & `tmp/pytmt-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytmt-0.4.2.tar", last modified: Tue Jan 24 22:46:54 2023, max compression
+gzip compressed data, was "pytmt-0.4.3.tar", last modified: Tue Apr 18 17:15:46 2023, max compression
```

## Comparing `pytmt-0.4.2.tar` & `pytmt-0.4.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 edwardlau   (501) staff       (20)        0 2023-01-24 22:46:54.899428 pytmt-0.4.2/
--rw-r--r--   0 edwardlau   (501) staff       (20)     1086 2020-06-03 17:42:10.000000 pytmt-0.4.2/LICENSE.md
--rw-r--r--   0 edwardlau   (501) staff       (20)      172 2020-06-03 19:07:44.000000 pytmt-0.4.2/MANIFEST.in
--rw-r--r--   0 edwardlau   (501) staff       (20)     2007 2023-01-24 22:46:54.899162 pytmt-0.4.2/PKG-INFO
--rw-r--r--   0 edwardlau   (501) staff       (20)     1091 2022-10-22 03:29:52.000000 pytmt-0.4.2/README.md
--rw-r--r--   0 edwardlau   (501) staff       (20)      231 2020-06-03 15:26:33.000000 pytmt-0.4.2/pyproject.toml
-drwxr-xr-x   0 edwardlau   (501) staff       (20)        0 2023-01-24 22:46:54.764794 pytmt-0.4.2/pytmt/
--rw-r--r--   0 edwardlau   (501) staff       (20)      115 2022-10-18 04:45:18.000000 pytmt-0.4.2/pytmt/__init__.py
--rw-r--r--   0 edwardlau   (501) staff       (20)      134 2020-06-03 15:45:41.000000 pytmt-0.4.2/pytmt/__main__.py
--rw-r--r--   0 edwardlau   (501) staff       (20)     1887 2022-10-28 14:58:50.000000 pytmt-0.4.2/pytmt/correct_matrix.py
--rw-r--r--   0 edwardlau   (501) staff       (20)     2061 2022-10-28 15:02:34.000000 pytmt-0.4.2/pytmt/get_spec.py
--rw-r--r--   0 edwardlau   (501) staff       (20)      941 2022-10-29 14:51:20.000000 pytmt-0.4.2/pytmt/logger.py
--rw-r--r--   0 edwardlau   (501) staff       (20)    18914 2023-01-24 22:46:14.000000 pytmt-0.4.2/pytmt/main.py
--rw-r--r--   0 edwardlau   (501) staff       (20)     6242 2022-10-29 14:50:40.000000 pytmt-0.4.2/pytmt/protein_group.py
--rw-r--r--   0 edwardlau   (501) staff       (20)     1287 2022-10-28 04:12:25.000000 pytmt-0.4.2/pytmt/quantify_spec.py
--rw-r--r--   0 edwardlau   (501) staff       (20)     1797 2022-10-18 04:31:14.000000 pytmt-0.4.2/pytmt/tmt_reporters.py
-drwxr-xr-x   0 edwardlau   (501) staff       (20)        0 2023-01-24 22:46:54.766665 pytmt-0.4.2/pytmt.egg-info/
--rw-r--r--   0 edwardlau   (501) staff       (20)     2007 2023-01-24 22:46:54.000000 pytmt-0.4.2/pytmt.egg-info/PKG-INFO
--rw-r--r--   0 edwardlau   (501) staff       (20)      571 2023-01-24 22:46:54.000000 pytmt-0.4.2/pytmt.egg-info/SOURCES.txt
--rw-r--r--   0 edwardlau   (501) staff       (20)        1 2023-01-24 22:46:54.000000 pytmt-0.4.2/pytmt.egg-info/dependency_links.txt
--rw-r--r--   0 edwardlau   (501) staff       (20)       47 2023-01-24 22:46:54.000000 pytmt-0.4.2/pytmt.egg-info/entry_points.txt
--rw-r--r--   0 edwardlau   (501) staff       (20)       48 2023-01-24 22:46:54.000000 pytmt-0.4.2/pytmt.egg-info/requires.txt
--rw-r--r--   0 edwardlau   (501) staff       (20)       12 2023-01-24 22:46:54.000000 pytmt-0.4.2/pytmt.egg-info/top_level.txt
--rw-r--r--   0 edwardlau   (501) staff       (20)       38 2023-01-24 22:46:54.899529 pytmt-0.4.2/setup.cfg
--rw-r--r--   0 edwardlau   (501) staff       (20)     2330 2023-01-24 22:46:40.000000 pytmt-0.4.2/setup.py
-drwxr-xr-x   0 edwardlau   (501) staff       (20)        0 2023-01-24 22:46:54.767121 pytmt-0.4.2/tests/
--rw-r--r--   0 edwardlau   (501) staff       (20)        0 2020-06-02 21:32:45.000000 pytmt-0.4.2/tests/__init__.py
-drwxr-xr-x   0 edwardlau   (501) staff       (20)        0 2023-01-24 22:46:54.758901 pytmt-0.4.2/tests/data/
-drwxr-xr-x   0 edwardlau   (501) staff       (20)        0 2023-01-24 22:46:54.887826 pytmt-0.4.2/tests/data/percolator/
--rw-r--r--   0 edwardlau   (501) staff       (20)     6148 2020-06-03 17:07:53.000000 pytmt-0.4.2/tests/data/percolator/.DS_Store
--rw-r--r--   0 edwardlau   (501) staff       (20) 79458335 2020-06-03 16:21:42.000000 pytmt-0.4.2/tests/data/percolator/percolator.target.mzid
--rw-r--r--   0 edwardlau   (501) staff       (20)  5855095 2020-06-03 16:18:05.000000 pytmt-0.4.2/tests/data/percolator/percolator.target.psms.txt
--rw-r--r--   0 edwardlau   (501) staff       (20)     2747 2020-06-03 16:56:07.000000 pytmt-0.4.2/tests/test_tmt.py
+drwxr-xr-x   0 edwardlau   (501) staff       (20)        0 2023-04-18 17:15:46.381664 pytmt-0.4.3/
+-rw-r--r--   0 edwardlau   (501) staff       (20)     1086 2020-06-03 17:42:10.000000 pytmt-0.4.3/LICENSE.md
+-rw-r--r--   0 edwardlau   (501) staff       (20)      172 2020-06-03 19:07:44.000000 pytmt-0.4.3/MANIFEST.in
+-rw-r--r--   0 edwardlau   (501) staff       (20)     2007 2023-04-18 17:15:46.381392 pytmt-0.4.3/PKG-INFO
+-rw-r--r--   0 edwardlau   (501) staff       (20)     1091 2023-04-18 17:13:10.000000 pytmt-0.4.3/README.md
+-rw-r--r--   0 edwardlau   (501) staff       (20)      231 2020-06-03 15:26:33.000000 pytmt-0.4.3/pyproject.toml
+drwxr-xr-x   0 edwardlau   (501) staff       (20)        0 2023-04-18 17:15:46.233729 pytmt-0.4.3/pytmt/
+-rw-r--r--   0 edwardlau   (501) staff       (20)      115 2023-04-18 17:12:52.000000 pytmt-0.4.3/pytmt/__init__.py
+-rw-r--r--   0 edwardlau   (501) staff       (20)      134 2020-06-03 15:45:41.000000 pytmt-0.4.3/pytmt/__main__.py
+-rw-r--r--   0 edwardlau   (501) staff       (20)     1887 2022-10-28 14:58:50.000000 pytmt-0.4.3/pytmt/correct_matrix.py
+-rw-r--r--   0 edwardlau   (501) staff       (20)     2061 2022-10-28 15:02:34.000000 pytmt-0.4.3/pytmt/get_spec.py
+-rw-r--r--   0 edwardlau   (501) staff       (20)      941 2022-10-29 14:51:20.000000 pytmt-0.4.3/pytmt/logger.py
+-rw-r--r--   0 edwardlau   (501) staff       (20)    18914 2023-01-24 22:46:14.000000 pytmt-0.4.3/pytmt/main.py
+-rw-r--r--   0 edwardlau   (501) staff       (20)     6242 2022-10-29 14:50:40.000000 pytmt-0.4.3/pytmt/protein_group.py
+-rw-r--r--   0 edwardlau   (501) staff       (20)     1287 2022-10-28 04:12:25.000000 pytmt-0.4.3/pytmt/quantify_spec.py
+-rw-r--r--   0 edwardlau   (501) staff       (20)     1797 2023-04-18 17:09:20.000000 pytmt-0.4.3/pytmt/tmt_reporters.py
+drwxr-xr-x   0 edwardlau   (501) staff       (20)        0 2023-04-18 17:15:46.235212 pytmt-0.4.3/pytmt.egg-info/
+-rw-r--r--   0 edwardlau   (501) staff       (20)     2007 2023-04-18 17:15:45.000000 pytmt-0.4.3/pytmt.egg-info/PKG-INFO
+-rw-r--r--   0 edwardlau   (501) staff       (20)      571 2023-04-18 17:15:45.000000 pytmt-0.4.3/pytmt.egg-info/SOURCES.txt
+-rw-r--r--   0 edwardlau   (501) staff       (20)        1 2023-04-18 17:15:45.000000 pytmt-0.4.3/pytmt.egg-info/dependency_links.txt
+-rw-r--r--   0 edwardlau   (501) staff       (20)       47 2023-04-18 17:15:45.000000 pytmt-0.4.3/pytmt.egg-info/entry_points.txt
+-rw-r--r--   0 edwardlau   (501) staff       (20)       48 2023-04-18 17:15:45.000000 pytmt-0.4.3/pytmt.egg-info/requires.txt
+-rw-r--r--   0 edwardlau   (501) staff       (20)       12 2023-04-18 17:15:45.000000 pytmt-0.4.3/pytmt.egg-info/top_level.txt
+-rw-r--r--   0 edwardlau   (501) staff       (20)       38 2023-04-18 17:15:46.381771 pytmt-0.4.3/setup.cfg
+-rw-r--r--   0 edwardlau   (501) staff       (20)     2330 2023-04-18 17:13:06.000000 pytmt-0.4.3/setup.py
+drwxr-xr-x   0 edwardlau   (501) staff       (20)        0 2023-04-18 17:15:46.235653 pytmt-0.4.3/tests/
+-rw-r--r--   0 edwardlau   (501) staff       (20)        0 2020-06-02 21:32:45.000000 pytmt-0.4.3/tests/__init__.py
+drwxr-xr-x   0 edwardlau   (501) staff       (20)        0 2023-04-18 17:15:46.226969 pytmt-0.4.3/tests/data/
+drwxr-xr-x   0 edwardlau   (501) staff       (20)        0 2023-04-18 17:15:46.369289 pytmt-0.4.3/tests/data/percolator/
+-rw-r--r--   0 edwardlau   (501) staff       (20)     6148 2020-06-03 17:07:53.000000 pytmt-0.4.3/tests/data/percolator/.DS_Store
+-rw-r--r--   0 edwardlau   (501) staff       (20) 79458335 2020-06-03 16:21:42.000000 pytmt-0.4.3/tests/data/percolator/percolator.target.mzid
+-rw-r--r--   0 edwardlau   (501) staff       (20)  5855095 2020-06-03 16:18:05.000000 pytmt-0.4.3/tests/data/percolator/percolator.target.psms.txt
+-rw-r--r--   0 edwardlau   (501) staff       (20)     2747 2020-06-03 16:56:07.000000 pytmt-0.4.3/tests/test_tmt.py
```

### Comparing `pytmt-0.4.2/LICENSE.md` & `pytmt-0.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pytmt-0.4.2/PKG-INFO` & `pytmt-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmt
-Version: 0.4.2
+Version: 0.4.3
 Summary: pytmt returns ms2 tmt quantification values from Crux Percolator output
 Home-page: https://github.com/ed-lau/pytmt
 Author: Edward Lau
 Author-email: edward.lau@cuanschutz.edu
 License: UNKNOWN
 Project-URL: Source, https://github.com/ed-lau/pytmt
 Project-URL: Lau Lab Colorado, https://laulab.net
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# pyTMT v0.4.1
+# pyTMT v0.4.3
 
 pyTMT returns ms2 tandem mass tag quantification values from Crux/Percolator output.
 
 See the [Documentations](https://lau-lab.github.io/pytmt/) for more information.
 
 ## Getting Started
```

### Comparing `pytmt-0.4.2/README.md` & `pytmt-0.4.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pyTMT v0.4.1
+# pyTMT v0.4.3
 
 pyTMT returns ms2 tandem mass tag quantification values from Crux/Percolator output.
 
 See the [Documentations](https://lau-lab.github.io/pytmt/) for more information.
 
 ## Getting Started
```

### Comparing `pytmt-0.4.2/pytmt/correct_matrix.py` & `pytmt-0.4.3/pytmt/correct_matrix.py`

 * *Files identical despite different names*

### Comparing `pytmt-0.4.2/pytmt/get_spec.py` & `pytmt-0.4.3/pytmt/get_spec.py`

 * *Files identical despite different names*

### Comparing `pytmt-0.4.2/pytmt/logger.py` & `pytmt-0.4.3/pytmt/logger.py`

 * *Files identical despite different names*

### Comparing `pytmt-0.4.2/pytmt/main.py` & `pytmt-0.4.3/pytmt/main.py`

 * *Files identical despite different names*

### Comparing `pytmt-0.4.2/pytmt/protein_group.py` & `pytmt-0.4.3/pytmt/protein_group.py`

 * *Files identical despite different names*

### Comparing `pytmt-0.4.2/pytmt/quantify_spec.py` & `pytmt-0.4.3/pytmt/quantify_spec.py`

 * *Files identical despite different names*

### Comparing `pytmt-0.4.2/pytmt/tmt_reporters.py` & `pytmt-0.4.3/pytmt/tmt_reporters.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
                  130.134825,  # 130N
                  130.141145,  # 130C
                  131.138180,  # 131N
                  131.144500,  # 131C (11-plex)
                  132.141535,  # 132N (Pro)
                  132.147855,  # 132C (Pro)
                  133.144890,  # 133N (Pro)
-                 133.141210,  # 133C (Pro)
+                 133.151210,  # 133C (Pro)
                  134.148245,  # 134N (Pro)
                  134,154565,  # 134C (Pro-18)
                  135.151600,  # 135N (Pro-18)
                  ]
 
 def get_reporters(plex):
     """
```

### Comparing `pytmt-0.4.2/pytmt.egg-info/PKG-INFO` & `pytmt-0.4.3/pytmt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmt
-Version: 0.4.2
+Version: 0.4.3
 Summary: pytmt returns ms2 tmt quantification values from Crux Percolator output
 Home-page: https://github.com/ed-lau/pytmt
 Author: Edward Lau
 Author-email: edward.lau@cuanschutz.edu
 License: UNKNOWN
 Project-URL: Source, https://github.com/ed-lau/pytmt
 Project-URL: Lau Lab Colorado, https://laulab.net
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# pyTMT v0.4.1
+# pyTMT v0.4.3
 
 pyTMT returns ms2 tandem mass tag quantification values from Crux/Percolator output.
 
 See the [Documentations](https://lau-lab.github.io/pytmt/) for more information.
 
 ## Getting Started
```

### Comparing `pytmt-0.4.2/pytmt.egg-info/SOURCES.txt` & `pytmt-0.4.3/pytmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytmt-0.4.2/setup.py` & `pytmt-0.4.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='pytmt',
-    version='0.4.2',
+    version='0.4.3',
     description='pytmt returns ms2 tmt quantification values from Crux Percolator output',
 
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     url='https://github.com/ed-lau/pytmt',
```

### Comparing `pytmt-0.4.2/tests/data/percolator/.DS_Store` & `pytmt-0.4.3/tests/data/percolator/.DS_Store`

 * *Files identical despite different names*

### Comparing `pytmt-0.4.2/tests/data/percolator/percolator.target.mzid` & `pytmt-0.4.3/tests/data/percolator/percolator.target.mzid`

 * *Files identical despite different names*

### Comparing `pytmt-0.4.2/tests/data/percolator/percolator.target.psms.txt` & `pytmt-0.4.3/tests/data/percolator/percolator.target.psms.txt`

 * *Files identical despite different names*

### Comparing `pytmt-0.4.2/tests/test_tmt.py` & `pytmt-0.4.3/tests/test_tmt.py`

 * *Files identical despite different names*

