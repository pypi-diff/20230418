# Comparing `tmp/luau-0.3.5.tar.gz` & `tmp/luau-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luau-0.3.5.tar", last modified: Tue Apr 18 01:09:15 2023, max compression
+gzip compressed data, was "luau-0.3.6.tar", last modified: Tue Apr 18 01:11:01 2023, max compression
```

## Comparing `luau-0.3.5.tar` & `luau-0.3.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 01:09:15.010832 luau-0.3.5/
--rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.3.5/LICENSE
--rw-rw-rw-   0        0        0      405 2023-04-18 01:09:15.010196 luau-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.3.5/README.md
--rw-rw-rw-   0        0        0      512 2023-04-18 01:08:42.000000 luau-0.3.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 01:09:15.011651 luau-0.3.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-18 01:09:14.885715 luau-0.3.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-18 01:09:14.933185 luau-0.3.5/src/luau/
--rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.3.5/src/luau/__init__.py
--rw-rw-rw-   0        0        0     5709 2023-04-15 01:24:18.000000 luau-0.3.5/src/luau/convert.py
--rw-rw-rw-   0        0        0     2515 2023-04-14 03:02:52.000000 luau-0.3.5/src/luau/path.py
-drwxrwxrwx   0        0        0        0 2023-04-18 01:09:15.008178 luau-0.3.5/src/luau/roblox/
--rw-rw-rw-   0        0        0      910 2023-04-18 01:08:32.000000 luau-0.3.5/src/luau/roblox/__init__.py
--rw-rw-rw-   0        0        0      810 2023-04-15 00:17:07.000000 luau-0.3.5/src/luau/roblox/rojo.py
--rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.3.5/src/luau/roblox/tool.py
--rw-rw-rw-   0        0        0      863 2023-04-14 22:00:20.000000 luau-0.3.5/src/luau/roblox/util.py
--rw-rw-rw-   0        0        0     2849 2023-04-15 00:38:19.000000 luau-0.3.5/src/luau/roblox/wally.py
-drwxrwxrwx   0        0        0        0 2023-04-18 01:09:14.967217 luau-0.3.5/src/luau.egg-info/
--rw-rw-rw-   0        0        0      405 2023-04-18 01:09:14.000000 luau-0.3.5/src/luau.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-04-18 01:09:14.000000 luau-0.3.5/src/luau.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 01:09:14.000000 luau-0.3.5/src/luau.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-18 01:09:14.000000 luau-0.3.5/src/luau.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-18 01:09:14.000000 luau-0.3.5/src/luau.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 01:11:01.946844 luau-0.3.6/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0      405 2023-04-18 01:11:01.946844 luau-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.3.6/README.md
+-rw-rw-rw-   0        0        0      512 2023-04-18 01:10:37.000000 luau-0.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 01:11:01.947843 luau-0.3.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 01:11:01.900362 luau-0.3.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 01:11:01.910996 luau-0.3.6/src/luau/
+-rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.3.6/src/luau/__init__.py
+-rw-rw-rw-   0        0        0     5709 2023-04-15 01:24:18.000000 luau-0.3.6/src/luau/convert.py
+-rw-rw-rw-   0        0        0     2515 2023-04-14 03:02:52.000000 luau-0.3.6/src/luau/path.py
+drwxrwxrwx   0        0        0        0 2023-04-18 01:11:01.944850 luau-0.3.6/src/luau/roblox/
+-rw-rw-rw-   0        0        0      937 2023-04-18 01:10:33.000000 luau-0.3.6/src/luau/roblox/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-04-15 00:17:07.000000 luau-0.3.6/src/luau/roblox/rojo.py
+-rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.3.6/src/luau/roblox/tool.py
+-rw-rw-rw-   0        0        0      863 2023-04-14 22:00:20.000000 luau-0.3.6/src/luau/roblox/util.py
+-rw-rw-rw-   0        0        0     2849 2023-04-15 00:38:19.000000 luau-0.3.6/src/luau/roblox/wally.py
+drwxrwxrwx   0        0        0        0 2023-04-18 01:11:01.937923 luau-0.3.6/src/luau.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-04-18 01:11:01.000000 luau-0.3.6/src/luau.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-04-18 01:11:01.000000 luau-0.3.6/src/luau.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 01:11:01.000000 luau-0.3.6/src/luau.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-18 01:11:01.000000 luau-0.3.6/src/luau.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-18 01:11:01.000000 luau-0.3.6/src/luau.egg-info/top_level.txt
```

### Comparing `luau-0.3.5/LICENSE` & `luau-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `luau-0.3.5/pyproject.toml` & `luau-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "luau"
-version = "0.3.5"
+version = "0.3.6"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"dpath~=2.1.5",
 	"toml~=0.10.2",
 	"types-toml~=0.10.8.6"
```

### Comparing `luau-0.3.5/src/luau/__init__.py` & `luau-0.3.6/src/luau/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.5/src/luau/convert.py` & `luau-0.3.6/src/luau/convert.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.5/src/luau/path.py` & `luau-0.3.6/src/luau/path.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.5/src/luau/roblox/__init__.py` & `luau-0.3.6/src/luau/roblox/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 	if not os.path.exists(dir_name):
 		os.makedirs(dir_name)
 	elif os.path.exists(build_path):
 		os.remove(build_path)
 
 	if write_as_directory:
 		full_dir_path = build_path.split(".")[0]
-		os.makedirs(full_dir_path)
 		full_ext = ".".join(build_path.split(".")[1:])
-		dir_path = build_path.replace(full_ext, "")
-		init_file_path = dir_path+"/init."+full_ext
+		final_dir_path = (dir_name+"/"+file_name).replace(full_ext, "")
+		os.makedirs(final_dir_path)
+		init_file_path = final_dir_path+"/init."+full_ext
 		out_file = open(init_file_path, "w")
 		out_file.write(content)
 		out_file.close()
 		format(init_file_path)
 
 	else:
 		out_file = open(build_path, "w")
```

### Comparing `luau-0.3.5/src/luau/roblox/rojo.py` & `luau-0.3.6/src/luau/roblox/rojo.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.5/src/luau/roblox/tool.py` & `luau-0.3.6/src/luau/roblox/tool.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.5/src/luau/roblox/util.py` & `luau-0.3.6/src/luau/roblox/util.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.5/src/luau/roblox/wally.py` & `luau-0.3.6/src/luau/roblox/wally.py`

 * *Files identical despite different names*

