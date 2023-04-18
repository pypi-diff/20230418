# Comparing `tmp/vfbLib-0.4.4.tar.gz` & `tmp/vfbLib-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vfbLib-0.4.4.tar", last modified: Wed Mar 15 17:05:54 2023, max compression
+gzip compressed data, was "vfbLib-0.4.5.tar", last modified: Tue Apr 18 17:39:50 2023, max compression
```

## Comparing `vfbLib-0.4.4.tar` & `vfbLib-0.4.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-15 17:05:54.639565 vfbLib-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (116)     3396 2023-03-15 17:05:42.000000 vfbLib-0.4.4/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (116)       14 2023-03-15 17:05:42.000000 vfbLib-0.4.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-15 17:05:54.631564 vfbLib-0.4.4/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-15 17:05:54.635564 vfbLib-0.4.4/Lib/vfbLib/
--rw-r--r--   0 runner    (1001) docker     (116)     3872 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4289 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (116)     7137 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/constants.py
--rw-r--r--   0 runner    (1001) docker     (116)     1678 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/diff.py
--rw-r--r--   0 runner    (1001) docker     (116)      221 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-15 17:05:54.635564 vfbLib-0.4.4/Lib/vfbLib/parsers/
--rw-r--r--   0 runner    (1001) docker     (116)     5532 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3425 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/parsers/bitmap.py
--rw-r--r--   0 runner    (1001) docker     (116)     1083 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/parsers/cmap.py
--rw-r--r--   0 runner    (1001) docker     (116)    16680 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/parsers/glyph.py
--rw-r--r--   0 runner    (1001) docker     (116)     2048 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/parsers/guides.py
--rw-r--r--   0 runner    (1001) docker     (116)     1610 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/parsers/header.py
--rw-r--r--   0 runner    (1001) docker     (116)     2686 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/parsers/mm.py
--rw-r--r--   0 runner    (1001) docker     (116)     1986 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/parsers/numeric.py
--rw-r--r--   0 runner    (1001) docker     (116)      664 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/parsers/options.py
--rw-r--r--   0 runner    (1001) docker     (116)     1765 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/parsers/ps.py
--rw-r--r--   0 runner    (1001) docker     (116)     2471 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/parsers/text.py
--rw-r--r--   0 runner    (1001) docker     (116)     8258 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/parsers/truetype.py
--rw-r--r--   0 runner    (1001) docker     (116)     1865 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/parsers/value.py
--rw-r--r--   0 runner    (1001) docker     (116)     1355 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/truetype.py
--rw-r--r--   0 runner    (1001) docker     (116)     2396 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-15 17:05:54.639565 vfbLib-0.4.4/Lib/vfbLib/ufo/
--rw-r--r--   0 runner    (1001) docker     (116)    28157 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/ufo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1455 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/ufo/designspace.py
--rw-r--r--   0 runner    (1001) docker     (116)     2169 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/ufo/glyph.py
--rw-r--r--   0 runner    (1001) docker     (116)     5141 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/ufo/groups.py
--rw-r--r--   0 runner    (1001) docker     (116)     2469 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/ufo/guides.py
--rw-r--r--   0 runner    (1001) docker     (116)     4138 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/ufo/helpers.py
--rw-r--r--   0 runner    (1001) docker     (116)    11362 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/ufo/info.py
--rw-r--r--   0 runner    (1001) docker     (116)     2334 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/ufo/kerning.py
--rw-r--r--   0 runner    (1001) docker     (116)    10617 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/ufo/paths.py
--rw-r--r--   0 runner    (1001) docker     (116)     6454 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/ufo/pshints.py
--rw-r--r--   0 runner    (1001) docker     (116)      375 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/ufo/time.py
--rw-r--r--   0 runner    (1001) docker     (116)     5125 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/ufo/tth.py
--rw-r--r--   0 runner    (1001) docker     (116)     1504 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/ufo/typing.py
--rw-r--r--   0 runner    (1001) docker     (116)     1726 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/ufo/vfb2ufo.py
--rw-r--r--   0 runner    (1001) docker     (116)       44 2023-03-15 17:05:42.000000 vfbLib-0.4.4/Lib/vfbLib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-15 17:05:54.635564 vfbLib-0.4.4/Lib/vfbLib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3990 2023-03-15 17:05:54.000000 vfbLib-0.4.4/Lib/vfbLib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1202 2023-03-15 17:05:54.000000 vfbLib-0.4.4/Lib/vfbLib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-15 17:05:54.000000 vfbLib-0.4.4/Lib/vfbLib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      165 2023-03-15 17:05:54.000000 vfbLib-0.4.4/Lib/vfbLib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-15 17:05:54.000000 vfbLib-0.4.4/Lib/vfbLib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       54 2023-03-15 17:05:54.000000 vfbLib-0.4.4/Lib/vfbLib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2023-03-15 17:05:54.000000 vfbLib-0.4.4/Lib/vfbLib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     3990 2023-03-15 17:05:54.639565 vfbLib-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      899 2023-03-15 17:05:42.000000 vfbLib-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      151 2023-03-15 17:05:42.000000 vfbLib-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)     1208 2023-03-15 17:05:54.639565 vfbLib-0.4.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (116)      202 2023-03-15 17:05:42.000000 vfbLib-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:39:50.342136 vfbLib-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-18 17:39:41.000000 vfbLib-0.4.5/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 17:39:41.000000 vfbLib-0.4.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:39:50.334136 vfbLib-0.4.5/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:39:50.334136 vfbLib-0.4.5/Lib/vfbLib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:39:50.338136 vfbLib-0.4.5/Lib/vfbLib/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/parsers/bitmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/parsers/cmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16680 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/parsers/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/parsers/guides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/parsers/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/parsers/mm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/parsers/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/parsers/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/parsers/ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/parsers/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/parsers/truetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/parsers/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/truetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:39:50.342136 vfbLib-0.4.5/Lib/vfbLib/ufo/
+-rw-r--r--   0 runner    (1001) docker     (123)    28171 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/ufo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/ufo/designspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/ufo/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/ufo/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/ufo/guides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/ufo/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/ufo/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/ufo/kerning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10617 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/ufo/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/ufo/pshints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/ufo/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/ufo/tth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/ufo/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/ufo/vfb2ufo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 17:39:41.000000 vfbLib-0.4.5/Lib/vfbLib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:39:50.338136 vfbLib-0.4.5/Lib/vfbLib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-04-18 17:39:50.000000 vfbLib-0.4.5/Lib/vfbLib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-18 17:39:50.000000 vfbLib-0.4.5/Lib/vfbLib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:39:50.000000 vfbLib-0.4.5/Lib/vfbLib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-18 17:39:50.000000 vfbLib-0.4.5/Lib/vfbLib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:39:50.000000 vfbLib-0.4.5/Lib/vfbLib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-18 17:39:50.000000 vfbLib-0.4.5/Lib/vfbLib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 17:39:50.000000 vfbLib-0.4.5/Lib/vfbLib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-04-18 17:39:50.342136 vfbLib-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-18 17:39:41.000000 vfbLib-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 17:39:41.000000 vfbLib-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-18 17:39:50.342136 vfbLib-0.4.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-04-18 17:39:41.000000 vfbLib-0.4.5/setup.py
```

### Comparing `vfbLib-0.4.4/DESCRIPTION.md` & `vfbLib-0.4.5/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/__init__.py` & `vfbLib-0.4.5/Lib/vfbLib/__init__.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/cmdline.py` & `vfbLib-0.4.5/Lib/vfbLib/cmdline.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/constants.py` & `vfbLib-0.4.5/Lib/vfbLib/constants.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/diff.py` & `vfbLib-0.4.5/Lib/vfbLib/diff.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/parsers/__init__.py` & `vfbLib-0.4.5/Lib/vfbLib/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/parsers/bitmap.py` & `vfbLib-0.4.5/Lib/vfbLib/parsers/bitmap.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/parsers/cmap.py` & `vfbLib-0.4.5/Lib/vfbLib/parsers/cmap.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/parsers/glyph.py` & `vfbLib-0.4.5/Lib/vfbLib/parsers/glyph.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/parsers/guides.py` & `vfbLib-0.4.5/Lib/vfbLib/parsers/guides.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/parsers/header.py` & `vfbLib-0.4.5/Lib/vfbLib/parsers/header.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/parsers/mm.py` & `vfbLib-0.4.5/Lib/vfbLib/parsers/mm.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/parsers/numeric.py` & `vfbLib-0.4.5/Lib/vfbLib/parsers/numeric.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/parsers/options.py` & `vfbLib-0.4.5/Lib/vfbLib/parsers/options.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/parsers/ps.py` & `vfbLib-0.4.5/Lib/vfbLib/parsers/ps.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/parsers/text.py` & `vfbLib-0.4.5/Lib/vfbLib/parsers/text.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/parsers/truetype.py` & `vfbLib-0.4.5/Lib/vfbLib/parsers/truetype.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/parsers/value.py` & `vfbLib-0.4.5/Lib/vfbLib/parsers/value.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/truetype.py` & `vfbLib-0.4.5/Lib/vfbLib/truetype.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/typing.py` & `vfbLib-0.4.5/Lib/vfbLib/typing.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/ufo/__init__.py` & `vfbLib-0.4.5/Lib/vfbLib/ufo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         self.build()
 
     def add_axis_mappings(self, data: List[Tuple[float, float]]) -> None:
         if not self.axis_mappings_count:
             raise ValueError(
                 "If axis mappings are present, axis mappings count must be set before parsing them."
             )
-        for i in range(4):
+        for i in range(self.axis_count):
             # Get the number of mappings for the current axis
             n = self.axis_mappings_count[i]
             if n > 0:
                 # Use only n mappings out of 10 for the current axis
                 mappings = data[:n]
                 axis = self.axes[i]
                 axis.map = [(u, round(d * 1000)) for u, d in mappings]
```

### Comparing `vfbLib-0.4.4/Lib/vfbLib/ufo/designspace.py` & `vfbLib-0.4.5/Lib/vfbLib/ufo/designspace.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/ufo/glyph.py` & `vfbLib-0.4.5/Lib/vfbLib/ufo/glyph.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/ufo/groups.py` & `vfbLib-0.4.5/Lib/vfbLib/ufo/groups.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/ufo/guides.py` & `vfbLib-0.4.5/Lib/vfbLib/ufo/guides.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/ufo/helpers.py` & `vfbLib-0.4.5/Lib/vfbLib/ufo/helpers.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/ufo/info.py` & `vfbLib-0.4.5/Lib/vfbLib/ufo/info.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/ufo/kerning.py` & `vfbLib-0.4.5/Lib/vfbLib/ufo/kerning.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/ufo/paths.py` & `vfbLib-0.4.5/Lib/vfbLib/ufo/paths.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/ufo/pshints.py` & `vfbLib-0.4.5/Lib/vfbLib/ufo/pshints.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/ufo/tth.py` & `vfbLib-0.4.5/Lib/vfbLib/ufo/tth.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/ufo/typing.py` & `vfbLib-0.4.5/Lib/vfbLib/ufo/typing.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib/ufo/vfb2ufo.py` & `vfbLib-0.4.5/Lib/vfbLib/ufo/vfb2ufo.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/Lib/vfbLib.egg-info/PKG-INFO` & `vfbLib-0.4.5/Lib/vfbLib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vfbLib
-Version: 0.4.4
+Version: 0.4.5
 Summary: Tools for converting FontLab Studio 5 (VFB) files.
 Home-page: https://pypi.org/project/vfblib/
 Author: Jens Kutilek
 License: MIT
 Project-URL: Source, https://github.com/LucasFonts/vfbLib
 Project-URL: Tracker, https://github.com/LucasFonts/vfbLib/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vfbLib-0.4.4/Lib/vfbLib.egg-info/SOURCES.txt` & `vfbLib-0.4.5/Lib/vfbLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/PKG-INFO` & `vfbLib-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vfbLib
-Version: 0.4.4
+Version: 0.4.5
 Summary: Tools for converting FontLab Studio 5 (VFB) files.
 Home-page: https://pypi.org/project/vfblib/
 Author: Jens Kutilek
 License: MIT
 Project-URL: Source, https://github.com/LucasFonts/vfbLib
 Project-URL: Tracker, https://github.com/LucasFonts/vfbLib/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vfbLib-0.4.4/README.md` & `vfbLib-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.4/setup.cfg` & `vfbLib-0.4.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vfbLib
-version = 0.4.4
+version = 0.4.5
 description = Tools for converting FontLab Studio 5 (VFB) files.
 long_description = file: DESCRIPTION.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://pypi.org/project/vfblib/
 author = Jens Kutilek
 license = MIT
 license_file = LICENSE
```

