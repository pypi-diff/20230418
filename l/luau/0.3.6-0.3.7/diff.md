# Comparing `tmp/luau-0.3.6.tar.gz` & `tmp/luau-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luau-0.3.6.tar", last modified: Tue Apr 18 01:11:01 2023, max compression
+gzip compressed data, was "luau-0.3.7.tar", last modified: Tue Apr 18 16:26:58 2023, max compression
```

## Comparing `luau-0.3.6.tar` & `luau-0.3.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 01:11:01.946844 luau-0.3.6/
--rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.3.6/LICENSE
--rw-rw-rw-   0        0        0      405 2023-04-18 01:11:01.946844 luau-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.3.6/README.md
--rw-rw-rw-   0        0        0      512 2023-04-18 01:10:37.000000 luau-0.3.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 01:11:01.947843 luau-0.3.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-18 01:11:01.900362 luau-0.3.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-18 01:11:01.910996 luau-0.3.6/src/luau/
--rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.3.6/src/luau/__init__.py
--rw-rw-rw-   0        0        0     5709 2023-04-15 01:24:18.000000 luau-0.3.6/src/luau/convert.py
--rw-rw-rw-   0        0        0     2515 2023-04-14 03:02:52.000000 luau-0.3.6/src/luau/path.py
-drwxrwxrwx   0        0        0        0 2023-04-18 01:11:01.944850 luau-0.3.6/src/luau/roblox/
--rw-rw-rw-   0        0        0      937 2023-04-18 01:10:33.000000 luau-0.3.6/src/luau/roblox/__init__.py
--rw-rw-rw-   0        0        0      810 2023-04-15 00:17:07.000000 luau-0.3.6/src/luau/roblox/rojo.py
--rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.3.6/src/luau/roblox/tool.py
--rw-rw-rw-   0        0        0      863 2023-04-14 22:00:20.000000 luau-0.3.6/src/luau/roblox/util.py
--rw-rw-rw-   0        0        0     2849 2023-04-15 00:38:19.000000 luau-0.3.6/src/luau/roblox/wally.py
-drwxrwxrwx   0        0        0        0 2023-04-18 01:11:01.937923 luau-0.3.6/src/luau.egg-info/
--rw-rw-rw-   0        0        0      405 2023-04-18 01:11:01.000000 luau-0.3.6/src/luau.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-04-18 01:11:01.000000 luau-0.3.6/src/luau.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 01:11:01.000000 luau-0.3.6/src/luau.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-18 01:11:01.000000 luau-0.3.6/src/luau.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-18 01:11:01.000000 luau-0.3.6/src/luau.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 16:26:58.830150 luau-0.3.7/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.3.7/LICENSE
+-rw-rw-rw-   0        0        0      405 2023-04-18 16:26:58.829154 luau-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.3.7/README.md
+-rw-rw-rw-   0        0        0      512 2023-04-18 16:26:04.000000 luau-0.3.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 16:26:58.830150 luau-0.3.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 16:26:58.674054 luau-0.3.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 16:26:58.770310 luau-0.3.7/src/luau/
+-rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.3.7/src/luau/__init__.py
+-rw-rw-rw-   0        0        0     5709 2023-04-15 01:24:18.000000 luau-0.3.7/src/luau/convert.py
+-rw-rw-rw-   0        0        0     2627 2023-04-18 16:26:04.000000 luau-0.3.7/src/luau/path.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:26:58.812201 luau-0.3.7/src/luau/roblox/
+-rw-rw-rw-   0        0        0      937 2023-04-18 01:10:33.000000 luau-0.3.7/src/luau/roblox/__init__.py
+-rw-rw-rw-   0        0        0     1807 2023-04-18 16:23:30.000000 luau-0.3.7/src/luau/roblox/rojo.py
+-rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.3.7/src/luau/roblox/tool.py
+-rw-rw-rw-   0        0        0      863 2023-04-14 22:00:20.000000 luau-0.3.7/src/luau/roblox/util.py
+-rw-rw-rw-   0        0        0     2849 2023-04-15 00:38:19.000000 luau-0.3.7/src/luau/roblox/wally.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:26:58.797240 luau-0.3.7/src/luau.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-04-18 16:26:58.000000 luau-0.3.7/src/luau.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-04-18 16:26:58.000000 luau-0.3.7/src/luau.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 16:26:58.000000 luau-0.3.7/src/luau.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-18 16:26:58.000000 luau-0.3.7/src/luau.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-18 16:26:58.000000 luau-0.3.7/src/luau.egg-info/top_level.txt
```

### Comparing `luau-0.3.6/LICENSE` & `luau-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `luau-0.3.6/pyproject.toml` & `luau-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "luau"
-version = "0.3.6"
+version = "0.3.7"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"dpath~=2.1.5",
 	"toml~=0.10.2",
 	"types-toml~=0.10.8.6"
```

### Comparing `luau-0.3.6/src/luau/__init__.py` & `luau-0.3.7/src/luau/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.6/src/luau/convert.py` & `luau-0.3.7/src/luau/convert.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.6/src/luau/path.py` & `luau-0.3.7/src/luau/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import shutil
 from typing import Literal
 
 def set_language_ext(path: str, desired_ext: Literal["luau", "lua"]) -> str:
 	base, ext = os.path.splitext(path)
 	return base + "." + desired_ext
 
 def get_alt_ext_path(path: str) -> str:
@@ -66,14 +67,18 @@
 	no_domain_path = filter_domain(build_path)
 	base, ext = os.path.splitext(no_domain_path)
 	return base+"."+domain+ext
 
 def remove_all_path_variants(path: str, domain: str=""):
 	alt_ext_path = get_alt_ext_path(path)
 
+	base_path = strip_full_ext(path)
+	if os.path.exists(base_path):
+		shutil.rmtree(base_path)
+
 	if os.path.exists(path):
 		os.remove(path)
 
 	if os.path.exists(alt_ext_path):
 		os.remove(alt_ext_path)
 
 	if get_domain_ext(path) != None:
```

### Comparing `luau-0.3.6/src/luau/roblox/__init__.py` & `luau-0.3.7/src/luau/roblox/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.6/src/luau/roblox/tool.py` & `luau-0.3.7/src/luau/roblox/tool.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.6/src/luau/roblox/util.py` & `luau-0.3.7/src/luau/roblox/util.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.6/src/luau/roblox/wally.py` & `luau-0.3.7/src/luau/roblox/wally.py`

 * *Files identical despite different names*

