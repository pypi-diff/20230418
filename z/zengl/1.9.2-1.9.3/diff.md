# Comparing `tmp/zengl-1.9.2.tar.gz` & `tmp/zengl-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zengl-1.9.2.tar", last modified: Mon Aug 15 13:24:25 2022, max compression
+gzip compressed data, was "zengl-1.9.3.tar", last modified: Wed Nov  9 14:12:05 2022, max compression
```

## Comparing `zengl-1.9.2.tar` & `zengl-1.9.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 13:24:25.553571 zengl-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-08-15 13:24:15.000000 zengl-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-08-15 13:24:15.000000 zengl-1.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9533 2022-08-15 13:24:25.553571 zengl-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8589 2022-08-15 13:24:15.000000 zengl-1.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    17530 2022-08-15 13:24:15.000000 zengl-1.9.2/_zengl.py
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-08-15 13:24:15.000000 zengl-1.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-15 13:24:25.553571 zengl-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2240 2022-08-15 13:24:15.000000 zengl-1.9.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)   104612 2022-08-15 13:24:15.000000 zengl-1.9.2/zengl.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 13:24:25.553571 zengl-1.9.2/zengl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9533 2022-08-15 13:24:25.000000 zengl-1.9.2/zengl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-08-15 13:24:25.000000 zengl-1.9.2/zengl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-15 13:24:25.000000 zengl-1.9.2/zengl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-08-15 13:24:25.000000 zengl-1.9.2/zengl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-15 13:24:25.000000 zengl-1.9.2/zengl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35953 2022-08-15 13:24:15.000000 zengl-1.9.2/zengl.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     8364 2022-08-15 13:24:15.000000 zengl-1.9.2/zengl.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 14:12:05.697829 zengl-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-11-09 14:11:58.000000 zengl-1.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-11-09 14:11:58.000000 zengl-1.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     9117 2022-11-09 14:12:05.697829 zengl-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8173 2022-11-09 14:11:58.000000 zengl-1.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)    17530 2022-11-09 14:11:58.000000 zengl-1.9.3/_zengl.py
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-11-09 14:11:58.000000 zengl-1.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-09 14:12:05.697829 zengl-1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2314 2022-11-09 14:11:58.000000 zengl-1.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 14:12:05.697829 zengl-1.9.3/zengl-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)     8364 2022-11-09 14:11:58.000000 zengl-1.9.3/zengl-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)   104612 2022-11-09 14:11:58.000000 zengl-1.9.3/zengl.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 14:12:05.697829 zengl-1.9.3/zengl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     9117 2022-11-09 14:12:05.000000 zengl-1.9.3/zengl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2022-11-09 14:12:05.000000 zengl-1.9.3/zengl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-09 14:12:05.000000 zengl-1.9.3/zengl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2022-11-09 14:12:05.000000 zengl-1.9.3/zengl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-09 14:12:05.000000 zengl-1.9.3/zengl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    35953 2022-11-09 14:11:58.000000 zengl-1.9.3/zengl.hpp
```

### Comparing `zengl-1.9.2/LICENSE` & `zengl-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zengl-1.9.2/PKG-INFO` & `zengl-1.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zengl
-Version: 1.9.2
+Version: 1.9.3
 Summary: Compact Python OpenGL rendering library
 Home-page: https://github.com/szabolcsdombi/zengl/
 Author: Szabolcs Dombi
 Author-email: cprogrammer1994@gmail.com
 License: MIT
 Project-URL: Documentation, https://zengl.readthedocs.io/
 Project-URL: Source, https://github.com/szabolcsdombi/zengl/
@@ -217,21 +217,7 @@
 [![linting_04](https://github.com/szabolcsdombi/zengl-example-images/raw/examples/linting/linting_04.png)](#typehints)
 
 [![linting_05](https://github.com/szabolcsdombi/zengl-example-images/raw/examples/linting/linting_05.png)](#typehints)
 
 [![linting_06](https://github.com/szabolcsdombi/zengl-example-images/raw/examples/linting/linting_06.png)](#typehints)
 
 [![linting_07](https://github.com/szabolcsdombi/zengl-example-images/raw/examples/linting/linting_07.png)](#typehints)
-
-**Not Working?**
-
-It is a known issue that at the moment on linux with venv the pyi file is not distributed properly.
-
-To fix this issue please download the [zengl.pyi](https://github.com/szabolcsdombi/zengl/raw/main/zengl.pyi) file
-and place it either in you project's root or next to the zengl binary.
-To locate the installation just inspect `zengl.__file__`.
-
-```py
->>> import zengl
->>> zengl.__file__
-'...'
-```
```

### Comparing `zengl-1.9.2/README.md` & `zengl-1.9.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -192,21 +192,7 @@
 [![linting_04](https://github.com/szabolcsdombi/zengl-example-images/raw/examples/linting/linting_04.png)](#typehints)
 
 [![linting_05](https://github.com/szabolcsdombi/zengl-example-images/raw/examples/linting/linting_05.png)](#typehints)
 
 [![linting_06](https://github.com/szabolcsdombi/zengl-example-images/raw/examples/linting/linting_06.png)](#typehints)
 
 [![linting_07](https://github.com/szabolcsdombi/zengl-example-images/raw/examples/linting/linting_07.png)](#typehints)
-
-**Not Working?**
-
-It is a known issue that at the moment on linux with venv the pyi file is not distributed properly.
-
-To fix this issue please download the [zengl.pyi](https://github.com/szabolcsdombi/zengl/raw/main/zengl.pyi) file
-and place it either in you project's root or next to the zengl binary.
-To locate the installation just inspect `zengl.__file__`.
-
-```py
->>> import zengl
->>> zengl.__file__
-'...'
-```
```

### Comparing `zengl-1.9.2/_zengl.py` & `zengl-1.9.3/_zengl.py`

 * *Files identical despite different names*

### Comparing `zengl-1.9.2/setup.py` & `zengl-1.9.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,18 +18,20 @@
 )
 
 with open('README.md') as readme:
     long_description = readme.read()
 
 setup(
     name='zengl',
-    version='1.9.2',
+    version='1.9.3',
     ext_modules=[ext],
     py_modules=['_zengl'],
-    data_files=[('.', ['zengl.pyi'])],
+    packages=['zengl-stubs'],
+    package_data={'zengl-stubs': ['__init__.pyi']},
+    include_package_data=True,
     license='MIT',
     python_requires='>=3.6',
     platforms=['any'],
     description='Compact Python OpenGL rendering library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Szabolcs Dombi',
```

### Comparing `zengl-1.9.2/zengl.cpp` & `zengl-1.9.3/zengl.cpp`

 * *Files identical despite different names*

### Comparing `zengl-1.9.2/zengl.egg-info/PKG-INFO` & `zengl-1.9.3/zengl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zengl
-Version: 1.9.2
+Version: 1.9.3
 Summary: Compact Python OpenGL rendering library
 Home-page: https://github.com/szabolcsdombi/zengl/
 Author: Szabolcs Dombi
 Author-email: cprogrammer1994@gmail.com
 License: MIT
 Project-URL: Documentation, https://zengl.readthedocs.io/
 Project-URL: Source, https://github.com/szabolcsdombi/zengl/
@@ -217,21 +217,7 @@
 [![linting_04](https://github.com/szabolcsdombi/zengl-example-images/raw/examples/linting/linting_04.png)](#typehints)
 
 [![linting_05](https://github.com/szabolcsdombi/zengl-example-images/raw/examples/linting/linting_05.png)](#typehints)
 
 [![linting_06](https://github.com/szabolcsdombi/zengl-example-images/raw/examples/linting/linting_06.png)](#typehints)
 
 [![linting_07](https://github.com/szabolcsdombi/zengl-example-images/raw/examples/linting/linting_07.png)](#typehints)
-
-**Not Working?**
-
-It is a known issue that at the moment on linux with venv the pyi file is not distributed properly.
-
-To fix this issue please download the [zengl.pyi](https://github.com/szabolcsdombi/zengl/raw/main/zengl.pyi) file
-and place it either in you project's root or next to the zengl binary.
-To locate the installation just inspect `zengl.__file__`.
-
-```py
->>> import zengl
->>> zengl.__file__
-'...'
-```
```

### Comparing `zengl-1.9.2/zengl.hpp` & `zengl-1.9.3/zengl.hpp`

 * *Files identical despite different names*

### Comparing `zengl-1.9.2/zengl.pyi` & `zengl-1.9.3/zengl-stubs/__init__.pyi`

 * *Files identical despite different names*

