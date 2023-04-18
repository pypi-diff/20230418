# Comparing `tmp/alia-0.1.8.tar.gz` & `tmp/alia-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alia-0.1.8.tar", last modified: Wed Apr 12 19:03:17 2023, max compression
+gzip compressed data, was "alia-0.1.9.tar", last modified: Tue Apr 18 16:52:30 2023, max compression
```

## Comparing `alia-0.1.8.tar` & `alia-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-12 19:03:17.708780 alia-0.1.8/
--rw-r--r--   0 aliavictor   (502) staff       (20)     1066 2023-03-23 20:16:29.000000 alia-0.1.8/LICENSE
--rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-12 19:03:17.708439 alia-0.1.8/PKG-INFO
--rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 19:00:09.000000 alia-0.1.8/README.md
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-12 19:03:17.705915 alia-0.1.8/alia/
--rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 18:58:43.000000 alia-0.1.8/alia/__init__.py
--rw-r--r--   0 aliavictor   (502) staff       (20)    14246 2023-03-23 19:42:40.000000 alia-0.1.8/alia/colors.py
--rw-r--r--   0 aliavictor   (502) staff       (20)     5598 2023-04-05 19:22:12.000000 alia-0.1.8/alia/df_tools.py
--rw-r--r--   0 aliavictor   (502) staff       (20)    25979 2023-04-12 19:02:55.000000 alia-0.1.8/alia/tools.py
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-12 19:03:17.707835 alia-0.1.8/alia.egg-info/
--rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-12 19:03:17.000000 alia-0.1.8/alia.egg-info/PKG-INFO
--rw-r--r--   0 aliavictor   (502) staff       (20)      228 2023-04-12 19:03:17.000000 alia-0.1.8/alia.egg-info/SOURCES.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)        1 2023-04-12 19:03:17.000000 alia-0.1.8/alia.egg-info/dependency_links.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)       74 2023-04-12 19:03:17.000000 alia-0.1.8/alia.egg-info/requires.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)        5 2023-04-12 19:03:17.000000 alia-0.1.8/alia.egg-info/top_level.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)       38 2023-04-12 19:03:17.708866 alia-0.1.8/setup.cfg
--rw-r--r--   0 aliavictor   (502) staff       (20)      884 2023-04-12 19:02:55.000000 alia-0.1.8/setup.py
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-18 16:52:30.117637 alia-0.1.9/
+-rw-r--r--   0 aliavictor   (502) staff       (20)     1066 2023-03-23 20:16:29.000000 alia-0.1.9/LICENSE
+-rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-18 16:52:30.117315 alia-0.1.9/PKG-INFO
+-rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 19:00:09.000000 alia-0.1.9/README.md
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-18 16:52:30.114095 alia-0.1.9/alia/
+-rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 18:58:43.000000 alia-0.1.9/alia/__init__.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)    14246 2023-03-23 19:42:40.000000 alia-0.1.9/alia/colors.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)     5598 2023-04-05 19:22:12.000000 alia-0.1.9/alia/df_tools.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)    26066 2023-04-18 16:51:02.000000 alia-0.1.9/alia/tools.py
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-18 16:52:30.116850 alia-0.1.9/alia.egg-info/
+-rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-18 16:52:30.000000 alia-0.1.9/alia.egg-info/PKG-INFO
+-rw-r--r--   0 aliavictor   (502) staff       (20)      228 2023-04-18 16:52:30.000000 alia-0.1.9/alia.egg-info/SOURCES.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)        1 2023-04-18 16:52:30.000000 alia-0.1.9/alia.egg-info/dependency_links.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)       74 2023-04-18 16:52:30.000000 alia-0.1.9/alia.egg-info/requires.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)        5 2023-04-18 16:52:30.000000 alia-0.1.9/alia.egg-info/top_level.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)       38 2023-04-18 16:52:30.117719 alia-0.1.9/setup.cfg
+-rw-r--r--   0 aliavictor   (502) staff       (20)      884 2023-04-18 16:51:49.000000 alia-0.1.9/setup.py
```

### Comparing `alia-0.1.8/LICENSE` & `alia-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alia-0.1.8/PKG-INFO` & `alia-0.1.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alia
-Version: 0.1.8
+Version: 0.1.9
 Summary: A collection of random helper tools to make life easier
 Home-page: https://github.com/aliavictor/alia
 Author: Alia
 Author-email: alia.jo.victor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alia-0.1.8/alia/colors.py` & `alia-0.1.9/alia/colors.py`

 * *Files identical despite different names*

### Comparing `alia-0.1.8/alia/df_tools.py` & `alia-0.1.9/alia/df_tools.py`

 * *Files identical despite different names*

### Comparing `alia-0.1.8/alia/tools.py` & `alia-0.1.9/alia/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,27 +20,28 @@
 
     Returns:
         Nothing."""
     pyperclip.copy(string)
     green("Copied to clipboard", ts=False)
 
 
-def save_obj(obj, filename):
+def save_obj(obj, filename, mode="wb"):
     """Saves an object to a file by pickling it.
 
     Args:
         obj (any type): Object to save
         filename (str): Filename to save the object as
+        mode (str): Which file mode to use ('wb' by default, 'a' to append)
 
     Returns:
         Nothing."""
     if ".pkl" not in filename:
         filename = f"{filename.strip()}.pkl"
 
-    with open(filename, "wb") as f:
+    with open(filename, mode) as f:
         pickle.dump(obj, f)
 
     green(f"Object saved as {filename}", ts=False)
 
 
 def load_obj(filename):
     """Loads a saved pickled object.
```

### Comparing `alia-0.1.8/alia.egg-info/PKG-INFO` & `alia-0.1.9/alia.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alia
-Version: 0.1.8
+Version: 0.1.9
 Summary: A collection of random helper tools to make life easier
 Home-page: https://github.com/aliavictor/alia
 Author: Alia
 Author-email: alia.jo.victor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alia-0.1.8/setup.py` & `alia-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="alia",
-    version="0.1.8",
+    version="0.1.9",
     description="A collection of random helper tools to make life easier",
     author="Alia",
     author_email="alia.jo.victor@gmail.com",
     url="https://github.com/aliavictor/alia",
     packages=find_packages(),
     install_requires=[
         # i.e. 'numpy>=1.18.0'
```

