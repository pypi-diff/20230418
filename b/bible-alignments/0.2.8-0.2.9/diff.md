# Comparing `tmp/bible_alignments-0.2.8.tar.gz` & `tmp/bible_alignments-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bible_alignments-0.2.8.tar", max compression
+gzip compressed data, was "bible_alignments-0.2.9.tar", max compression
```

## Comparing `bible_alignments-0.2.8.tar` & `bible_alignments-0.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    20131 2023-02-22 04:20:29.147219 bible_alignments-0.2.8/LICENSE
--rw-r--r--   0        0        0      900 2023-03-01 18:19:16.168100 bible_alignments-0.2.8/README.md
--rw-r--r--   0        0        0     1726 2023-04-18 18:30:15.213448 bible_alignments-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      554 2023-02-22 04:20:29.528825 bible_alignments-0.2.8/src/.github/actions/run-checks/action.yml
--rw-r--r--   0        0        0     2033 2023-02-22 04:20:29.529037 bible_alignments-0.2.8/src/.github/actions/setup-poetry-env/action.yml
--rw-r--r--   0        0        0      975 2023-02-22 04:20:29.529247 bible_alignments-0.2.8/src/.github/workflows/on-merge-to-main.yml
--rw-r--r--   0        0        0      949 2023-02-22 04:20:29.529364 bible_alignments-0.2.8/src/.github/workflows/on-pull-request.yml
--rw-r--r--   0        0        0     1964 2023-02-22 04:20:29.529486 bible_alignments-0.2.8/src/.github/workflows/on-release-main.yml
--rw-r--r--   0        0        0      351 2023-02-22 04:20:29.529608 bible_alignments-0.2.8/src/.github/workflows/validate-codecov-config.yml
--rw-r--r--   0        0        0    16557 2023-02-28 20:36:24.715176 bible_alignments-0.2.8/src/01-Exploration.ipynb
--rw-r--r--   0        0        0      149 2023-04-18 14:05:38.099337 bible_alignments-0.2.8/src/__init__.py
--rw-r--r--   0        0        0     4810 2023-03-16 20:46:04.251808 bible_alignments-0.2.8/src/catalog.py
--rw-r--r--   0        0        0      247 2023-02-24 04:25:33.130530 bible_alignments-0.2.8/src/config.py
--rw-r--r--   0        0        0        0 2023-02-22 04:20:29.529807 bible_alignments-0.2.8/src/format/__init__.py
--rw-r--r--   0        0        0     5829 2023-02-22 04:20:29.529962 bible_alignments-0.2.8/src/format/grapecity.py
--rw-r--r--   0        0        0     2134 2023-04-12 01:30:26.702000 bible_alignments-0.2.8/src/gcsource.py
--rw-r--r--   0        0        0     2193 2023-04-12 01:30:54.463000 bible_alignments-0.2.8/src/gctarget.py
--rw-r--r--   0        0        0     5705 2023-04-18 12:59:07.522414 bible_alignments-0.2.8/src/grapecity.py
--rw-r--r--   0        0        0     2086 1970-01-01 00:00:00.000000 bible_alignments-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    20131 2023-02-22 04:20:29.147219 bible_alignments-0.2.9/LICENSE
+-rw-r--r--   0        0        0      900 2023-03-01 18:19:16.168100 bible_alignments-0.2.9/README.md
+-rw-r--r--   0        0        0      554 2023-02-22 04:20:29.528825 bible_alignments-0.2.9/bible_alignments/.github/actions/run-checks/action.yml
+-rw-r--r--   0        0        0     2033 2023-02-22 04:20:29.529037 bible_alignments-0.2.9/bible_alignments/.github/actions/setup-poetry-env/action.yml
+-rw-r--r--   0        0        0      975 2023-02-22 04:20:29.529246 bible_alignments-0.2.9/bible_alignments/.github/workflows/on-merge-to-main.yml
+-rw-r--r--   0        0        0      949 2023-02-22 04:20:29.529365 bible_alignments-0.2.9/bible_alignments/.github/workflows/on-pull-request.yml
+-rw-r--r--   0        0        0     1964 2023-02-22 04:20:29.529486 bible_alignments-0.2.9/bible_alignments/.github/workflows/on-release-main.yml
+-rw-r--r--   0        0        0      351 2023-02-22 04:20:29.529608 bible_alignments-0.2.9/bible_alignments/.github/workflows/validate-codecov-config.yml
+-rw-r--r--   0        0        0    16557 2023-02-28 20:36:24.715176 bible_alignments-0.2.9/bible_alignments/01-Exploration.ipynb
+-rw-r--r--   0        0        0      149 2023-04-18 14:05:38.099337 bible_alignments-0.2.9/bible_alignments/__init__.py
+-rw-r--r--   0        0        0     4810 2023-03-16 20:46:04.251808 bible_alignments-0.2.9/bible_alignments/catalog.py
+-rw-r--r--   0        0        0      247 2023-02-24 04:25:33.130530 bible_alignments-0.2.9/bible_alignments/config.py
+-rw-r--r--   0        0        0        0 2023-02-22 04:20:29.529807 bible_alignments-0.2.9/bible_alignments/format/__init__.py
+-rw-r--r--   0        0        0     5829 2023-02-22 04:20:29.529962 bible_alignments-0.2.9/bible_alignments/format/grapecity.py
+-rw-r--r--   0        0        0     2134 2023-04-12 01:30:26.702000 bible_alignments-0.2.9/bible_alignments/gcsource.py
+-rw-r--r--   0        0        0     2193 2023-04-12 01:30:54.463000 bible_alignments-0.2.9/bible_alignments/gctarget.py
+-rw-r--r--   0        0        0     5705 2023-04-18 12:59:07.522414 bible_alignments-0.2.9/bible_alignments/grapecity.py
+-rw-r--r--   0        0        0     1713 2023-04-18 20:44:28.409167 bible_alignments-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     2086 1970-01-01 00:00:00.000000 bible_alignments-0.2.9/PKG-INFO
```

### Comparing `bible_alignments-0.2.8/LICENSE` & `bible_alignments-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.8/README.md` & `bible_alignments-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.8/pyproject.toml` & `bible_alignments-0.2.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "bible-alignments"
-version = "0.2.8"
+version = "0.2.9"
 description = "Word-level alignments for Bibles, including both automatic alignments and manually corrected alignments."
 authors = ["Sean Boisen <sean.boisen@clear.bible>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["Bible", "alignment", "Bible alignment"]
 repository = "https://github.com/Clear-Bible/Alignments"
 #documentation = "https://sboisen.github.io/alignments/"
 packages = [
-  {include = "src"},
-  {include = "src/*.py"},
+  {include = "bible_alignments"},
 ]
 # need more here
 classifiers = [
     "Development Status :: 4 - Beta",
     "Operating System :: OS Independent",
     "Intended Audience :: Religion",
     "License :: OSI Approved :: MIT License",
```

### Comparing `bible_alignments-0.2.8/src/.github/actions/run-checks/action.yml` & `bible_alignments-0.2.9/bible_alignments/.github/actions/run-checks/action.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.8/src/.github/actions/setup-poetry-env/action.yml` & `bible_alignments-0.2.9/bible_alignments/.github/actions/setup-poetry-env/action.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.8/src/.github/workflows/on-merge-to-main.yml` & `bible_alignments-0.2.9/bible_alignments/.github/workflows/on-merge-to-main.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.8/src/.github/workflows/on-pull-request.yml` & `bible_alignments-0.2.9/bible_alignments/.github/workflows/on-pull-request.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.8/src/.github/workflows/on-release-main.yml` & `bible_alignments-0.2.9/bible_alignments/.github/workflows/on-release-main.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.8/src/01-Exploration.ipynb` & `bible_alignments-0.2.9/bible_alignments/01-Exploration.ipynb`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.8/src/catalog.py` & `bible_alignments-0.2.9/bible_alignments/catalog.py`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.8/src/format/grapecity.py` & `bible_alignments-0.2.9/bible_alignments/format/grapecity.py`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.8/src/gcsource.py` & `bible_alignments-0.2.9/bible_alignments/gcsource.py`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.8/src/gctarget.py` & `bible_alignments-0.2.9/bible_alignments/gctarget.py`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.8/src/grapecity.py` & `bible_alignments-0.2.9/bible_alignments/grapecity.py`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.8/PKG-INFO` & `bible_alignments-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bible-alignments
-Version: 0.2.8
+Version: 0.2.9
 Summary: Word-level alignments for Bibles, including both automatic alignments and manually corrected alignments.
 Home-page: https://github.com/Clear-Bible/Alignments
 License: MIT
 Keywords: Bible,alignment,Bible alignment
 Author: Sean Boisen
 Author-email: sean.boisen@clear.bible
 Requires-Python: >=3.7,<4.0
```

