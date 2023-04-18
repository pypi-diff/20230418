# Comparing `tmp/emojito-0.1.0.post1.tar.gz` & `tmp/emojito-0.1.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emojito-0.1.0.post1.tar", max compression
+gzip compressed data, was "emojito-0.1.0.post2.tar", max compression
```

## Comparing `emojito-0.1.0.post1.tar` & `emojito-0.1.0.post2.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     1129 2022-12-13 02:48:50.130795 emojito-0.1.0.post1/README.md
--rw-r--r--   0        0        0     2538 2022-12-13 02:32:22.472374 emojito-0.1.0.post1/emojito/__init__.py
--rw-r--r--   0        0        0      455 2022-12-13 02:52:15.947734 emojito-0.1.0.post1/pyproject.toml
--rw-r--r--   0        0        0     1884 1970-01-01 00:00:00.000000 emojito-0.1.0.post1/setup.py
--rw-r--r--   0        0        0     1816 1970-01-01 00:00:00.000000 emojito-0.1.0.post1/PKG-INFO
+-rw-r--r--   0        0        0     1129 2022-12-13 02:48:50.130795 emojito-0.1.0.post2/README.md
+-rw-r--r--   0        0        0     2538 2022-12-13 02:32:22.472374 emojito-0.1.0.post2/emojito/__init__.py
+-rw-r--r--   0        0        0      453 2023-04-18 01:40:23.250585 emojito-0.1.0.post2/pyproject.toml
+-rw-r--r--   0        0        0     1812 1970-01-01 00:00:00.000000 emojito-0.1.0.post2/PKG-INFO
```

### Comparing `emojito-0.1.0.post1/README.md` & `emojito-0.1.0.post2/README.md`

 * *Files identical despite different names*

### Comparing `emojito-0.1.0.post1/emojito/__init__.py` & `emojito-0.1.0.post2/emojito/__init__.py`

 * *Files identical despite different names*

### Comparing `emojito-0.1.0.post1/PKG-INFO` & `emojito-0.1.0.post2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: emojito
-Version: 0.1.0.post1
+Version: 0.1.0.post2
 Summary: Define your own shortnames to be replaced with emojis or other content.
-Home-page: https://gitlab.com/deepadmax/emojito
+Home-page: https://gitlab.com/emojito/emojito
 License: GPL-3.0-or-later
 Author: Maximillian Strand
 Author-email: maxi@millian.se
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
-Project-URL: Repository, https://gitlab.com/deepadmax/emojito
+Project-URL: Repository, https://gitlab.com/emojito/emojito
 Description-Content-Type: text/markdown
 
 # Emojito
 
 There are many packages that provide shortnames for emojis. This package allows you to provide your own shortnames and with what to replace them.
 
 ## Features
```

