# Comparing `tmp/fig2sketch-0.2.5.tar.gz` & `tmp/fig2sketch-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fig2sketch-0.2.5.tar", last modified: Tue Apr 18 09:39:28 2023, max compression
+gzip compressed data, was "fig2sketch-0.2.6.tar", last modified: Tue Apr 18 13:57:01 2023, max compression
```

## Comparing `fig2sketch-0.2.5.tar` & `fig2sketch-0.2.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:28.387962 fig2sketch-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-18 09:39:28.387962 fig2sketch-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 09:39:28.387962 fig2sketch-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:28.383962 fig2sketch-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:28.387962 fig2sketch-0.2.5/src/converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/artboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/document.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/font.py
--rw-r--r--   0 runner    (1001) docker     (123)    34002 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/font_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/positioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/prototype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/shape_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/shape_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/slice.py
--rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/converter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:28.387962 fig2sketch-0.2.5/src/fig2sketch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-18 09:39:28.000000 fig2sketch-0.2.5/src/fig2sketch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-18 09:39:28.000000 fig2sketch-0.2.5/src/fig2sketch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:39:28.000000 fig2sketch-0.2.5/src/fig2sketch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 09:39:28.000000 fig2sketch-0.2.5/src/fig2sketch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-18 09:39:28.000000 fig2sketch-0.2.5/src/fig2sketch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 09:39:28.000000 fig2sketch-0.2.5/src/fig2sketch.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     3382 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/fig2sketch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:28.387962 fig2sketch-0.2.5/src/figformat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/figformat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/figformat/decodefig.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/figformat/fig2tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/figformat/kiwi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/figformat/vector_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:28.387962 fig2sketch-0.2.5/src/sketchformat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/layer_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/layer_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/layer_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/prototype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:28.387962 fig2sketch-0.2.5/src/sketchformat/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/serialize/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/serialize/orjson.py
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-18 09:39:19.000000 fig2sketch-0.2.5/src/sketchformat/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:01.052606 fig2sketch-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-18 13:57:01.052606 fig2sketch-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 13:57:01.052606 fig2sketch-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:01.044606 fig2sketch-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:01.048606 fig2sketch-0.2.6/src/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/artboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34002 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/font_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/positioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/prototype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/shape_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/shape_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:01.048606 fig2sketch-0.2.6/src/fig2sketch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-18 13:57:01.000000 fig2sketch-0.2.6/src/fig2sketch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-18 13:57:01.000000 fig2sketch-0.2.6/src/fig2sketch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:57:01.000000 fig2sketch-0.2.6/src/fig2sketch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 13:57:01.000000 fig2sketch-0.2.6/src/fig2sketch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-18 13:57:01.000000 fig2sketch-0.2.6/src/fig2sketch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 13:57:01.000000 fig2sketch-0.2.6/src/fig2sketch.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3382 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/fig2sketch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:01.048606 fig2sketch-0.2.6/src/figformat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/figformat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/figformat/decodefig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/figformat/fig2tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/figformat/kiwi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/figformat/vector_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:01.052606 fig2sketch-0.2.6/src/sketchformat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/layer_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/layer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/layer_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/prototype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:01.052606 fig2sketch-0.2.6/src/sketchformat/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/serialize/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/serialize/orjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/text.py
```

### Comparing `fig2sketch-0.2.5/LICENSE` & `fig2sketch-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/PKG-INFO` & `fig2sketch-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fig2sketch
-Version: 0.2.5
+Version: 0.2.6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: fast
 Provides-Extra: dev
 License-File: LICENSE
 
 # .fig to Sketch converter
```

### Comparing `fig2sketch-0.2.5/README.md` & `fig2sketch-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/pyproject.toml` & `fig2sketch-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/converter/artboard.py` & `fig2sketch-0.2.6/src/converter/artboard.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/converter/base.py` & `fig2sketch-0.2.6/src/converter/base.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/converter/component.py` & `fig2sketch-0.2.6/src/converter/component.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/converter/context.py` & `fig2sketch-0.2.6/src/converter/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             font_file, font_name = font.get_webfont(*font_descriptor)
         except:
             logging.warning(f"Could not download font {font_descriptor}")
             font_file = None
             if fig_font_name["postscript"]:
                 font_name = fig_font_name["postscript"]
             else:
-                font_name = f"{fig_font_name['family']}-{fig_font_name['subfamily']}"
+                font_name = f"{fig_font_name['family']}-{fig_font_name['style']}"
 
         self._used_fonts[font_descriptor] = (font_file, font_name)
         return font_name
 
     def used_fonts(self) -> Dict[Tuple[str, str], Tuple[IO[bytes], str]]:
         return self._used_fonts
```

### Comparing `fig2sketch-0.2.5/src/converter/convert.py` & `fig2sketch-0.2.6/src/converter/convert.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/converter/document.py` & `fig2sketch-0.2.6/src/converter/document.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/converter/font.py` & `fig2sketch-0.2.6/src/converter/font.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/converter/font_features.py` & `fig2sketch-0.2.6/src/converter/font_features.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/converter/group.py` & `fig2sketch-0.2.6/src/converter/group.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/converter/instance.py` & `fig2sketch-0.2.6/src/converter/instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
 
 
 def find_refs(node, ref_id):
     """Find all usages of a property in a symbol, recursively"""
     refs = [
         (ref, node.get("overrideKey", node["guid"]))
         for ref in node.get("componentPropRefs", [])
-        if ref["defID"] == ref_id and not ref["isDeleted"]
+        if ref["defID"] == ref_id and not ref.get("isDeleted", False)
     ]
 
     for ch in node.get("children", []):
         refs += find_refs(ch, ref_id)
 
     return refs
```

### Comparing `fig2sketch-0.2.5/src/converter/meta.py` & `fig2sketch-0.2.6/src/converter/meta.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/converter/page.py` & `fig2sketch-0.2.6/src/converter/page.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/converter/positioning.py` & `fig2sketch-0.2.6/src/converter/positioning.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/converter/prototype.py` & `fig2sketch-0.2.6/src/converter/prototype.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/converter/rectangle.py` & `fig2sketch-0.2.6/src/converter/rectangle.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/converter/shape_group.py` & `fig2sketch-0.2.6/src/converter/shape_group.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/converter/shape_path.py` & `fig2sketch-0.2.6/src/converter/shape_path.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/converter/style.py` & `fig2sketch-0.2.6/src/converter/style.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/converter/symbol.py` & `fig2sketch-0.2.6/src/converter/symbol.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,18 +40,15 @@
         )
 
     # Use better names for variants if possible
     try:
         parent = context.fig_node(fig_symbol["parent"]["guid"])
         if parent and parent.get("isStateGroup", False):
             master.name = symbol_variant_name(parent, fig_symbol)
-        elif "=" in fig_symbol["name"]:
-            import pdb
 
-            pdb.set_trace()
     except Exception as e:
         print(e)
 
     return master
 
 
 def move_to_symbols_page(fig_symbol, sketch_symbol):
```

### Comparing `fig2sketch-0.2.5/src/converter/text.py` & `fig2sketch-0.2.6/src/converter/text.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/converter/tree.py` & `fig2sketch-0.2.6/src/converter/tree.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/converter/user.py` & `fig2sketch-0.2.6/src/converter/user.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/converter/utils.py` & `fig2sketch-0.2.6/src/converter/utils.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/fig2sketch.egg-info/PKG-INFO` & `fig2sketch-0.2.6/src/fig2sketch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fig2sketch
-Version: 0.2.5
+Version: 0.2.6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: fast
 Provides-Extra: dev
 License-File: LICENSE
 
 # .fig to Sketch converter
```

### Comparing `fig2sketch-0.2.5/src/fig2sketch.egg-info/SOURCES.txt` & `fig2sketch-0.2.6/src/fig2sketch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/fig2sketch.py` & `fig2sketch-0.2.6/src/fig2sketch.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/figformat/decodefig.py` & `fig2sketch-0.2.6/src/figformat/decodefig.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/figformat/fig2tree.py` & `fig2sketch-0.2.6/src/figformat/fig2tree.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/figformat/kiwi.py` & `fig2sketch-0.2.6/src/figformat/kiwi.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/figformat/vector_network.py` & `fig2sketch-0.2.6/src/figformat/vector_network.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/sketchformat/common.py` & `fig2sketch-0.2.6/src/sketchformat/common.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/sketchformat/document.py` & `fig2sketch-0.2.6/src/sketchformat/document.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/sketchformat/layer_common.py` & `fig2sketch-0.2.6/src/sketchformat/layer_common.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/sketchformat/layer_group.py` & `fig2sketch-0.2.6/src/sketchformat/layer_group.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/sketchformat/layer_shape.py` & `fig2sketch-0.2.6/src/sketchformat/layer_shape.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/sketchformat/prototype.py` & `fig2sketch-0.2.6/src/sketchformat/prototype.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/sketchformat/serialize/json.py` & `fig2sketch-0.2.6/src/sketchformat/serialize/json.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/sketchformat/serialize/orjson.py` & `fig2sketch-0.2.6/src/sketchformat/serialize/orjson.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/sketchformat/style.py` & `fig2sketch-0.2.6/src/sketchformat/style.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.5/src/sketchformat/text.py` & `fig2sketch-0.2.6/src/sketchformat/text.py`

 * *Files identical despite different names*

