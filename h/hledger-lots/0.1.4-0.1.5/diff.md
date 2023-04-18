# Comparing `tmp/hledger_lots-0.1.4.tar.gz` & `tmp/hledger_lots-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hledger_lots-0.1.4.tar", last modified: Mon Apr 17 20:53:21 2023, max compression
+gzip compressed data, was "hledger_lots-0.1.5.tar", last modified: Tue Apr 18 19:32:28 2023, max compression
```

## Comparing `hledger_lots-0.1.4.tar` & `hledger_lots-0.1.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-17 20:53:21.214704 hledger_lots-0.1.4/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5073 2023-04-17 20:53:21.214704 hledger_lots-0.1.4/PKG-INFO
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-17 20:53:21.203704 hledger_lots-0.1.4/docs/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4733 2023-04-17 20:48:23.000000 hledger_lots-0.1.4/docs/README.md
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-17 20:53:21.205704 hledger_lots-0.1.4/hledger_lots/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/hledger_lots/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       85 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/hledger_lots/__main__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3001 2023-04-17 20:48:23.000000 hledger_lots-0.1.4/hledger_lots/avg.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2525 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/hledger_lots/avg_info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1393 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/hledger_lots/checks.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)    12828 2023-04-17 20:48:23.000000 hledger_lots-0.1.4/hledger_lots/cli.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3776 2023-04-17 20:48:23.000000 hledger_lots-0.1.4/hledger_lots/fifo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3040 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/hledger_lots/fifo_info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      969 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/hledger_lots/files.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1709 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/hledger_lots/hl.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4313 2023-04-17 20:48:23.000000 hledger_lots-0.1.4/hledger_lots/info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2780 2023-04-17 20:48:23.000000 hledger_lots-0.1.4/hledger_lots/lib.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3770 2023-04-17 20:48:23.000000 hledger_lots-0.1.4/hledger_lots/prices_yahoo.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-17 20:53:21.207704 hledger_lots-0.1.4/hledger_lots.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5073 2023-04-17 20:53:21.000000 hledger_lots-0.1.4/hledger_lots.egg-info/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1003 2023-04-17 20:53:21.000000 hledger_lots-0.1.4/hledger_lots.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-04-17 20:53:21.000000 hledger_lots-0.1.4/hledger_lots.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-04-17 20:53:21.000000 hledger_lots-0.1.4/hledger_lots.egg-info/entry_points.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       33 2023-04-17 20:53:21.000000 hledger_lots-0.1.4/hledger_lots.egg-info/requires.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       53 2023-04-17 20:53:21.000000 hledger_lots-0.1.4/hledger_lots.egg-info/top_level.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1174 2023-04-17 20:49:44.000000 hledger_lots-0.1.4/pyproject.toml
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-04-17 20:53:21.214704 hledger_lots-0.1.4/setup.cfg
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-17 20:53:21.210704 hledger_lots-0.1.4/tests/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-03-30 00:36:22.000000 hledger_lots-0.1.4/tests/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5566 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/tests/lots_data.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      192 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/tests/test__main__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4601 2023-04-17 20:48:23.000000 hledger_lots-0.1.4/tests/test_avg.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3241 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/tests/test_checks.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2612 2023-04-17 20:48:23.000000 hledger_lots-0.1.4/tests/test_fifo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2305 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/tests/test_files.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/tests/test_hl.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/tests/test_info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2136 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/tests/test_lib.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-17 20:53:21.202704 hledger_lots-0.1.4/venv/
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-17 20:53:21.214704 hledger_lots-0.1.4/venv/bin/
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2html.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2html4.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2html5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2latex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2man.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2odt.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2s5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2xetex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2xml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rstpep2html.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:32:28.822543 hledger_lots-0.1.5/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5073 2023-04-18 19:32:28.822543 hledger_lots-0.1.5/PKG-INFO
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:32:28.815543 hledger_lots-0.1.5/docs/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4733 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/docs/README.md
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:32:28.818543 hledger_lots-0.1.5/hledger_lots/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       85 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/__main__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3001 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/avg.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2525 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/avg_info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1393 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/checks.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)    12828 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/cli.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3776 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/fifo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3040 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/fifo_info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      969 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/files.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1709 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/hl.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4313 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2780 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/lib.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3770 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/prices_yahoo.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:32:28.819543 hledger_lots-0.1.5/hledger_lots.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5073 2023-04-18 19:32:28.000000 hledger_lots-0.1.5/hledger_lots.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1003 2023-04-18 19:32:28.000000 hledger_lots-0.1.5/hledger_lots.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-04-18 19:32:28.000000 hledger_lots-0.1.5/hledger_lots.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-04-18 19:32:28.000000 hledger_lots-0.1.5/hledger_lots.egg-info/entry_points.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       66 2023-04-18 19:32:28.000000 hledger_lots-0.1.5/hledger_lots.egg-info/requires.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       34 2023-04-18 19:32:28.000000 hledger_lots-0.1.5/hledger_lots.egg-info/top_level.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1234 2023-04-18 19:27:41.000000 hledger_lots-0.1.5/pyproject.toml
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-04-18 19:32:28.822543 hledger_lots-0.1.5/setup.cfg
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:32:28.820543 hledger_lots-0.1.5/tests/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/tests/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5566 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/tests/lots_data.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      192 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/tests/test__main__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4601 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/tests/test_avg.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3241 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/tests/test_checks.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2612 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/tests/test_fifo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2305 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/tests/test_files.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/tests/test_hl.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/tests/test_info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2136 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/tests/test_lib.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:32:28.814543 hledger_lots-0.1.5/venv/
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:32:28.822543 hledger_lots-0.1.5/venv/bin/
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2html.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2html4.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2html5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2latex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2man.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2odt.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2s5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2xml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rstpep2html.py
```

### Comparing `hledger_lots-0.1.4/PKG-INFO` & `hledger_lots-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hledger_lots
-Version: 0.1.4
+Version: 0.1.5
 License: MIT License
 Project-URL: homepage, https://github.com/edkedk99/hledger-lots
 Project-URL: documentation, https://edkedk99.github.io/hledger-lots/
 Project-URL: repository, https://github.com/edkedk99/hledger-lots
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `hledger_lots-0.1.4/docs/README.md` & `hledger_lots-0.1.5/docs/README.md`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/hledger_lots/avg.py` & `hledger_lots-0.1.5/hledger_lots/avg.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/hledger_lots/avg_info.py` & `hledger_lots-0.1.5/hledger_lots/avg_info.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/hledger_lots/checks.py` & `hledger_lots-0.1.5/hledger_lots/checks.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/hledger_lots/cli.py` & `hledger_lots-0.1.5/hledger_lots/cli.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/hledger_lots/fifo.py` & `hledger_lots-0.1.5/hledger_lots/fifo.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/hledger_lots/fifo_info.py` & `hledger_lots-0.1.5/hledger_lots/fifo_info.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/hledger_lots/files.py` & `hledger_lots-0.1.5/hledger_lots/files.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/hledger_lots/hl.py` & `hledger_lots-0.1.5/hledger_lots/hl.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/hledger_lots/info.py` & `hledger_lots-0.1.5/hledger_lots/info.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/hledger_lots/lib.py` & `hledger_lots-0.1.5/hledger_lots/lib.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/hledger_lots/prices_yahoo.py` & `hledger_lots-0.1.5/hledger_lots/prices_yahoo.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/hledger_lots.egg-info/PKG-INFO` & `hledger_lots-0.1.5/hledger_lots.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hledger-lots
-Version: 0.1.4
+Version: 0.1.5
 License: MIT License
 Project-URL: homepage, https://github.com/edkedk99/hledger-lots
 Project-URL: documentation, https://edkedk99.github.io/hledger-lots/
 Project-URL: repository, https://github.com/edkedk99/hledger-lots
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `hledger_lots-0.1.4/hledger_lots.egg-info/SOURCES.txt` & `hledger_lots-0.1.5/hledger_lots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/pyproject.toml` & `hledger_lots-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -22,23 +22,26 @@
 keyword = ["hledger","PTA", "investments", "accounting", "lots"]
 classifiers = [""]
 author = "Eduardo"
 author_email = "edkedk99@hotmail.com"
 
 [project]
 name = "hledger_lots"
-version = "0.1.4"
+version = "0.1.5"
 readme= "docs/README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 dependencies = [
 	     "click",
 	     "rich_click",
 	     "tabulate",
-	     "pyxirr"
+	     "pyxirr",
+	     "yfinance",
+	     "requests",
+	     "requests-cache"
 ]
 
 [project.urls]
 homepage = "https://github.com/edkedk99/hledger-lots"
 documentation = "https://edkedk99.github.io/hledger-lots/"
 repository = "https://github.com/edkedk99/hledger-lots"
 # changelog = ""
```

### Comparing `hledger_lots-0.1.4/tests/lots_data.py` & `hledger_lots-0.1.5/tests/lots_data.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/tests/test_avg.py` & `hledger_lots-0.1.5/tests/test_avg.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/tests/test_checks.py` & `hledger_lots-0.1.5/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/tests/test_fifo.py` & `hledger_lots-0.1.5/tests/test_fifo.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/tests/test_files.py` & `hledger_lots-0.1.5/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/tests/test_hl.py` & `hledger_lots-0.1.5/tests/test_hl.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/tests/test_info.py` & `hledger_lots-0.1.5/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/tests/test_lib.py` & `hledger_lots-0.1.5/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/venv/bin/rst2html.py` & `hledger_lots-0.1.5/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/venv/bin/rst2html4.py` & `hledger_lots-0.1.5/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/venv/bin/rst2html5.py` & `hledger_lots-0.1.5/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/venv/bin/rst2latex.py` & `hledger_lots-0.1.5/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/venv/bin/rst2man.py` & `hledger_lots-0.1.5/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/venv/bin/rst2odt.py` & `hledger_lots-0.1.5/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/venv/bin/rst2odt_prepstyles.py` & `hledger_lots-0.1.5/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/venv/bin/rst2pseudoxml.py` & `hledger_lots-0.1.5/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/venv/bin/rst2s5.py` & `hledger_lots-0.1.5/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/venv/bin/rst2xetex.py` & `hledger_lots-0.1.5/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/venv/bin/rst2xml.py` & `hledger_lots-0.1.5/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.4/venv/bin/rstpep2html.py` & `hledger_lots-0.1.5/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

