# Comparing `tmp/fig2sketch-0.2.4.tar.gz` & `tmp/fig2sketch-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fig2sketch-0.2.4.tar", last modified: Mon Apr 17 09:36:10 2023, max compression
+gzip compressed data, was "fig2sketch-0.2.5.tar", last modified: Tue Apr 18 09:39:28 2023, max compression
```

## Comparing `fig2sketch-0.2.4.tar` & `fig2sketch-0.2.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:36:10.313639 fig2sketch-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-17 09:36:10.313639 fig2sketch-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 09:36:10.313639 fig2sketch-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:36:10.305639 fig2sketch-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:36:10.309639 fig2sketch-0.2.4/src/converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/artboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/document.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/font.py
--rw-r--r--   0 runner    (1001) docker     (123)    34002 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/font_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/positioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/prototype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/shape_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/shape_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/slice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:36:10.309639 fig2sketch-0.2.4/src/fig2sketch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-17 09:36:10.000000 fig2sketch-0.2.4/src/fig2sketch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-17 09:36:10.000000 fig2sketch-0.2.4/src/fig2sketch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:36:10.000000 fig2sketch-0.2.4/src/fig2sketch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-17 09:36:10.000000 fig2sketch-0.2.4/src/fig2sketch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-17 09:36:10.000000 fig2sketch-0.2.4/src/fig2sketch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-17 09:36:10.000000 fig2sketch-0.2.4/src/fig2sketch.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     3382 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/fig2sketch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:36:10.309639 fig2sketch-0.2.4/src/figformat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/figformat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/figformat/decodefig.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/figformat/fig2tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/figformat/kiwi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/figformat/vector_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:36:10.313639 fig2sketch-0.2.4/src/sketchformat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/layer_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/layer_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/layer_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/prototype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:36:10.313639 fig2sketch-0.2.4/src/sketchformat/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/serialize/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/serialize/orjson.py
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:28.387962 fig2sketch-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-18 09:39:28.387962 fig2sketch-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 09:39:28.387962 fig2sketch-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:28.383962 fig2sketch-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:28.387962 fig2sketch-0.2.5/src/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/artboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34002 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/font_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/positioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/prototype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/shape_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/shape_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:28.387962 fig2sketch-0.2.5/src/fig2sketch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-18 09:39:28.000000 fig2sketch-0.2.5/src/fig2sketch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-18 09:39:28.000000 fig2sketch-0.2.5/src/fig2sketch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:39:28.000000 fig2sketch-0.2.5/src/fig2sketch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 09:39:28.000000 fig2sketch-0.2.5/src/fig2sketch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-18 09:39:28.000000 fig2sketch-0.2.5/src/fig2sketch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 09:39:28.000000 fig2sketch-0.2.5/src/fig2sketch.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3382 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/fig2sketch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:28.387962 fig2sketch-0.2.5/src/figformat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/figformat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/figformat/decodefig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/figformat/fig2tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/figformat/kiwi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/figformat/vector_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:28.387962 fig2sketch-0.2.5/src/sketchformat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/layer_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/layer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/layer_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/prototype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:28.387962 fig2sketch-0.2.5/src/sketchformat/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/serialize/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/serialize/orjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/text.py
```

### Comparing `fig2sketch-0.2.4/LICENSE` & `fig2sketch-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/PKG-INFO` & `fig2sketch-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fig2sketch
-Version: 0.2.4
+Version: 0.2.5
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: fast
 Provides-Extra: dev
 License-File: LICENSE
 
 # .fig to Sketch converter
```

### Comparing `fig2sketch-0.2.4/README.md` & `fig2sketch-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/pyproject.toml` & `fig2sketch-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/converter/artboard.py` & `fig2sketch-0.2.5/src/converter/artboard.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/converter/base.py` & `fig2sketch-0.2.5/src/converter/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,19 @@
 def base_styled(fig_node: dict) -> _BaseStyled:
     obj: _BaseShape = {
         **base_layer(fig_node),  # type: ignore
         **masking(fig_node),  # type: ignore
         "style": process_styles(fig_node),
     }
 
-    if obj["hasClippingMask"] and obj["clippingMaskMode"] == 0:
+    if (
+        obj["hasClippingMask"]
+        and obj["clippingMaskMode"] == ClippingMaskMode.OUTLINE
+        and not fig_node.get("f2sForceOutline")
+    ):
         # Outline mask behave differently in fig files and Sketch in regard to fill/stroke colors
         # Remove fill
         obj["style"].fills = []
         # TODO: If we have stroke, we should remove it and enlarge ourselves to occupy that space
         # which is quite tricky in things like shapePaths. This should be pretty rare in practice
 
     return obj
@@ -209,19 +213,21 @@
     "MAX": 4,  # Fixed right + width
     "STRETCH": 2,  # Fixed left and right
     "SCALE": 7,  # All free
     # 'FIXED_MIN': 0, # Unused?
     # 'FIXED_MAX': 0, # Unused?
 }
 
-
 # Vertical constraints are equivalent to horizontal ones, with a 3 bit shift
+VERTICAL_CONSTRAINT = {k: v << 3 for k, v in HORIZONTAL_CONSTRAINT.items()}
+
+
 def resizing_constraint(fig_node: dict) -> int:
     h = HORIZONTAL_CONSTRAINT[fig_node["horizontalConstraint"]]
-    v = HORIZONTAL_CONSTRAINT[fig_node["verticalConstraint"]] << 3
+    v = VERTICAL_CONSTRAINT[fig_node["verticalConstraint"]]
     return h + v
 
 
 CLIPPING_MODE = {
     "ALPHA": ClippingMaskMode.ALPHA,
     "OUTLINE": ClippingMaskMode.OUTLINE,
 }
```

### Comparing `fig2sketch-0.2.4/src/converter/component.py` & `fig2sketch-0.2.5/src/converter/component.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/converter/context.py` & `fig2sketch-0.2.5/src/converter/context.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/converter/convert.py` & `fig2sketch-0.2.5/src/converter/convert.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/converter/document.py` & `fig2sketch-0.2.5/src/converter/document.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/converter/font.py` & `fig2sketch-0.2.5/src/converter/font.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/converter/font_features.py` & `fig2sketch-0.2.5/src/converter/font_features.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/converter/group.py` & `fig2sketch-0.2.5/src/converter/group.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/converter/instance.py` & `fig2sketch-0.2.5/src/converter/instance.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/converter/meta.py` & `fig2sketch-0.2.5/src/converter/meta.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/converter/page.py` & `fig2sketch-0.2.5/src/converter/page.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/converter/positioning.py` & `fig2sketch-0.2.5/src/converter/positioning.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,19 +10,26 @@
 
     def __add__(self, other):
         return Vector(self[0] + other[0], self[1] + other[1])
 
     def __sub__(self, other):
         return Vector(self[0] - other[0], self[1] - other[1])
 
+    def length(self) -> float:
+        return (self[0] ** 2 + self[1] ** 2) ** 0.5
+
 
 class Matrix(list):
     def __init__(self, m: Sequence[Sequence[float]]):
         super().__init__(m)
 
+    @staticmethod
+    def scale(x: float, y: float) -> "Matrix":
+        return Matrix([[x, 0, 0], [0, y, 0], [0, 0, 1]])
+
     def dot(self, v: Vector) -> Vector:
         return Vector(
             self[0][2] + self[0][0] * v[0] + self[0][1] * v[1],
             self[1][2] + self[1][0] * v[0] + self[1][1] * v[1],
         )
 
     def dot2(self, v: Vector) -> Vector:
@@ -46,14 +53,35 @@
                     (self[0][2] * self[1][0] - self[0][0] * self[1][2])
                     / (self[0][0] * self[1][1] - self[0][1] * self[1][0]),
                 ],
                 [0, 0, 1],
             ]
         )
 
+    def __mul__(self, m):
+        return Matrix(
+            [
+                [
+                    self[0][0] * m[0][0] + self[0][1] * m[1][0] + self[0][2] * m[2][0],
+                    self[0][0] * m[0][1] + self[0][1] * m[1][1] + self[0][2] * m[2][1],
+                    self[0][0] * m[0][2] + self[0][1] * m[1][2] + self[0][2] * m[2][2],
+                ],
+                [
+                    self[1][0] * m[0][0] + self[1][1] * m[1][0] + self[1][2] * m[2][0],
+                    self[1][0] * m[0][1] + self[1][1] * m[1][1] + self[1][2] * m[2][1],
+                    self[1][0] * m[0][2] + self[1][1] * m[1][2] + self[1][2] * m[2][2],
+                ],
+                [
+                    self[2][0] * m[0][0] + self[2][1] * m[1][0] + self[2][2] * m[2][0],
+                    self[2][0] * m[0][1] + self[2][1] * m[1][1] + self[2][2] * m[2][1],
+                    self[2][0] * m[0][2] + self[2][1] * m[1][2] + self[2][2] * m[2][2],
+                ],
+            ]
+        )
+
 
 class _Positioning(TypedDict):
     frame: Rect
     rotation: float
     isFlippedHorizontal: bool
     isFlippedVertical: bool
```

### Comparing `fig2sketch-0.2.4/src/converter/prototype.py` & `fig2sketch-0.2.5/src/converter/prototype.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/converter/rectangle.py` & `fig2sketch-0.2.5/src/converter/rectangle.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,12 +36,13 @@
 def make_background_rect(fig: dict, frame: Rect, name: str) -> Rectangle:
     radius, corners = convert_corners(fig)
     return Rectangle(
         do_objectID=utils.gen_object_id(fig["guid"], name.encode()),
         name=name,
         frame=Rect(height=frame.height, width=frame.width, x=0, y=0),
         style=Style(do_objectID=utils.gen_object_id(fig["guid"], f"{name}_style".encode())),
-        resizingConstraint=10,
+        resizingConstraint=base.HORIZONTAL_CONSTRAINT["STRETCH"]
+        + base.VERTICAL_CONSTRAINT["STRETCH"],
         rotation=0,
         fixedRadius=radius,
         corners=corners,
     )
```

### Comparing `fig2sketch-0.2.4/src/converter/shape_group.py` & `fig2sketch-0.2.5/src/converter/shape_group.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/converter/shape_path.py` & `fig2sketch-0.2.5/src/converter/shape_path.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/converter/style.py` & `fig2sketch-0.2.5/src/converter/style.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import copy
 import dataclasses
 import math
 from .positioning import Vector, Matrix
 from converter import utils
 from sketchformat.style import *
 from typing import List, TypedDict
+from .errors import Fig2SketchNodeChanged
 
 BORDER_POSITION = {
     "CENTER": BorderPosition.CENTER,
     "INSIDE": BorderPosition.INSIDE,
     "OUTSIDE": BorderPosition.OUTSIDE,
 }
 
@@ -65,20 +67,16 @@
             if "strokeCap" in fig_node
             else BorderOptions.__dict__["lineCapStyle"],
             lineJoinStyle=LINE_JOIN_STYLE[fig_node["strokeJoin"]]
             if "strokeJoin" in fig_node
             else BorderOptions.__dict__["lineCapStyle"],
             dashPattern=fig_node.get("dashPattern", []),
         ),
-        borders=[convert_border(fig_node, b) for b in fig_node["strokePaints"]]
-        if "strokePaints" in fig_node
-        else [],
-        fills=[convert_fill(fig_node, f) for f in fig_node["fillPaints"]]
-        if "fillPaints" in fig_node
-        else [],
+        borders=[convert_border(fig_node, b) for b in fig_node.get("strokePaints", [])],
+        fills=[convert_fill(fig_node, f) for f in fig_node.get("fillPaints", [])],
         **convert_effects(fig_node),
         contextSettings=context_settings(fig_node),
     )
     return sketch_style
 
 
 def convert_border(fig_node: dict, fig_border: dict) -> Border:
@@ -100,18 +98,17 @@
             # Solid color backgrounds do not support specifying the opacity
             # Instead, it must be set in the color itself
             return Fill.Color(
                 convert_color(fig_fill["color"], fig_fill["opacity"]),
                 isEnabled=fig_fill["visible"],
             )
         case {"type": "IMAGE"}:
-            if "transform" in fig_fill and fig_fill["transform"] != Matrix(
-                [[1, 0, 0], [0, 1, 0], [0, 0, 1]]
-            ):
-                utils.log_conversion_warning("STY004", fig_node)
+            if is_cropped_image(fig_fill):
+                # Extract images to a separate layer and retrigger conversion
+                convert_crop_image_to_mask(fig_node)
 
             if "paintFilter" in fig_fill:
                 utils.log_conversion_warning("STY005", fig_node)
 
             return Fill.Image(
                 f'images/{fig_fill["image"]["filename"]}',
                 patternFillType=PATTERN_FILL_TYPE[fig_fill["imageScaleMode"]],
@@ -123,14 +120,100 @@
             return Fill.Gradient(
                 convert_gradient(fig_node, fig_fill),
                 isEnabled=fig_fill["visible"],
                 opacity=fig_fill.get("opacity", 1),
             )
 
 
+def is_cropped_image(fig_fill: dict) -> bool:
+    return (
+        fig_fill.get("type") == "IMAGE"
+        and "transform" in fig_fill
+        and fig_fill["transform"] != Matrix([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
+    )
+
+
+def convert_crop_image_to_mask(fig_node: dict) -> None:
+    content = copy.deepcopy(fig_node)
+    cropped_images = []
+    other_fills = []
+    for idx, fill in enumerate(content.get("fillPaints", [])):
+        if is_cropped_image(fill):
+            image_layer = cropped_image_layer(fig_node, fill)
+            image_layer["guid"] = fig_node["guid"] + (1, idx)
+            cropped_images.append(image_layer)
+        else:
+            other_fills.append(fill)
+
+    content["fillPaints"] = other_fills
+    content["transform"] = Matrix([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
+
+    old = copy.copy(fig_node)
+    fig_node.clear()
+    fig_node.update(
+        {
+            "type": "FRAME",
+            "name": f'{old["name"]} (crop group)',
+            "guid": old["guid"] + (0, 0),
+            "size": old["size"],
+            "transform": old["transform"],
+            "locked": old["locked"],
+            "visible": old["visible"],
+            "horizontalConstraint": old["horizontalConstraint"],
+            "verticalConstraint": old["verticalConstraint"],
+            "blendMode": old["blendMode"],
+            "opacity": old["opacity"],
+            "resizeToFit": True,
+            "children": [
+                {
+                    **content,
+                    "mask": True,
+                    "maskType": "OUTLINE",
+                    "f2sForceOutline": True,
+                },
+                *cropped_images,
+            ],
+        }
+    )
+    raise Fig2SketchNodeChanged
+
+
+def cropped_image_layer(fig_node: dict, fill: dict) -> dict:
+    invmat = fill["transform"].inv()
+
+    iw = fill["originalImageWidth"]
+    ih = fill["originalImageHeight"]
+    image_scale = Matrix.scale(1.0 / iw, 1.0 / ih)
+    layer_scale = Matrix.scale(fig_node["size"]["x"], fig_node["size"]["y"])
+
+    transform = layer_scale * invmat * image_scale
+
+    height = transform.dot2([0, ih]).length()
+    width = transform.dot2([iw, 0]).length()
+
+    normalize_scale = Matrix.scale(iw / width, ih / height)
+
+    image_layer = {
+        "type": "RECTANGLE",
+        "name": f'{fig_node["name"]} (cropped image)',
+        "size": {"x": width, "y": height},
+        "transform": transform * normalize_scale,
+        "locked": fig_node["locked"],
+        "visible": fig_node["visible"],
+        "horizontalConstraint": fig_node["horizontalConstraint"],
+        "verticalConstraint": fig_node["verticalConstraint"],
+        "blendMode": fig_node["blendMode"],
+        "opacity": fig_node["opacity"],
+        "fillPaints": [fill],
+    }
+    del image_layer["fillPaints"][0]["transform"]
+
+    return image_layer
+
+
 def convert_color(color: dict, opacity: Optional[float] = None) -> Color:
     return Color(
         red=color["r"],
         green=color["g"],
         blue=color["b"],
         alpha=color["a"] if opacity is None else opacity,
     )
```

### Comparing `fig2sketch-0.2.4/src/converter/symbol.py` & `fig2sketch-0.2.5/src/converter/symbol.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/converter/text.py` & `fig2sketch-0.2.5/src/converter/text.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/converter/tree.py` & `fig2sketch-0.2.5/src/converter/tree.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/converter/user.py` & `fig2sketch-0.2.5/src/converter/user.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/converter/utils.py` & `fig2sketch-0.2.5/src/converter/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,27 +50,28 @@
                 "rectangleTopLeftCornerRadius",
                 "rectangleTopLeftCornerRadius",
             ]
         ]
     )
 
 
+# Commented messages are no longer used, but we keep them for referencing past errors
 WARNING_MESSAGES = {
     "TXT001": "is missing the glyphs property. If the text has unicode characters, it may not convert the format properly",
     "TXT002": "has multiple text fill colors. Only the first one will be converted",
     "TXT003": "has a non-solid text color (gradient or image) which is not supported by Sketch",
     "TXT004": "contains a 'TITLE' transformation. Sketch does not support this text transformation, so no transformation is applied",
     "TXT005": "contains a LIST style with list markers. This style will be ignored",
     "TXT006": "uses OpenType features not supported by Sketch: {features}. They will be ignored",
     "SHP001": "contains a line with at least one 'Reversed triangle' end. This type of marker does not exist in Sketch. It has been converted to a 'Line' type marker",
     "SHP002": "does not have any points. It will be skipped",
     "STY001": "contains a layer blur and a background blur. Only one will be converted",
     "STY002": "contains a DIAMOND gradient, which is not supported. It is converted to a RADIAL gradient",
     "STY003": "contains a fill with a non-standard blend mode, which is not supported at the fill level (us the layer blend mode instead). It will be ignored",
-    "STY004": "has a cropped image background, which is not supported yet. It will be set to stretch",
+    # "STY004": "has a cropped image background, which is not supported yet. It will be set to stretch",
     "STY005": "contains a image fill property, which is not supported. The extra properties will be ignored",
     "SYM001": "references an invalid symbol. It will be converted to an empty placeholder group",
     "SYM002": "overrides unsupported properties: {props}. The override will be ignored",
     "SYM003": "overrides unsupported properties: {props}. The instance will be detached",
     "SYM004": "contains an override of an unknown node {node_ref}. The override will be ignored",
     "ART001": "has at least one corner radius which is not supported by sketch artboards. The corner radius will be ignored",
     "ART002": "is being converted to an artboard. However, artboard rotations are not supported. Rotation will be ignored",
```

### Comparing `fig2sketch-0.2.4/src/fig2sketch.egg-info/PKG-INFO` & `fig2sketch-0.2.5/src/fig2sketch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fig2sketch
-Version: 0.2.4
+Version: 0.2.5
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: fast
 Provides-Extra: dev
 License-File: LICENSE
 
 # .fig to Sketch converter
```

### Comparing `fig2sketch-0.2.4/src/fig2sketch.egg-info/SOURCES.txt` & `fig2sketch-0.2.5/src/fig2sketch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/fig2sketch.py` & `fig2sketch-0.2.5/src/fig2sketch.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/figformat/decodefig.py` & `fig2sketch-0.2.5/src/figformat/decodefig.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/figformat/fig2tree.py` & `fig2sketch-0.2.5/src/figformat/fig2tree.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/figformat/kiwi.py` & `fig2sketch-0.2.5/src/figformat/kiwi.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/figformat/vector_network.py` & `fig2sketch-0.2.5/src/figformat/vector_network.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/sketchformat/common.py` & `fig2sketch-0.2.5/src/sketchformat/common.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/sketchformat/document.py` & `fig2sketch-0.2.5/src/sketchformat/document.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/sketchformat/layer_common.py` & `fig2sketch-0.2.5/src/sketchformat/layer_common.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/sketchformat/layer_group.py` & `fig2sketch-0.2.5/src/sketchformat/layer_group.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/sketchformat/layer_shape.py` & `fig2sketch-0.2.5/src/sketchformat/layer_shape.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/sketchformat/prototype.py` & `fig2sketch-0.2.5/src/sketchformat/prototype.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/sketchformat/serialize/json.py` & `fig2sketch-0.2.5/src/sketchformat/serialize/json.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/sketchformat/serialize/orjson.py` & `fig2sketch-0.2.5/src/sketchformat/serialize/orjson.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/sketchformat/style.py` & `fig2sketch-0.2.5/src/sketchformat/style.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.4/src/sketchformat/text.py` & `fig2sketch-0.2.5/src/sketchformat/text.py`

 * *Files identical despite different names*

