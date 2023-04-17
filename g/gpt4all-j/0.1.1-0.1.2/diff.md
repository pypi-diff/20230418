# Comparing `tmp/gpt4all-j-0.1.1.tar.gz` & `tmp/gpt4all-j-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4all-j-0.1.1.tar", last modified: Mon Apr 17 22:06:16 2023, max compression
+gzip compressed data, was "gpt4all-j-0.1.2.tar", last modified: Mon Apr 17 22:26:30 2023, max compression
```

## Comparing `gpt4all-j-0.1.1.tar` & `gpt4all-j-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 22:06:16.472461 gpt4all-j-0.1.1/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2161 2023-04-17 22:06:16.472461 gpt4all-j-0.1.1/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1138 2023-04-17 22:04:59.000000 gpt4all-j-0.1.1/README.md
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 22:06:16.462461 gpt4all-j-0.1.1/gpt4all_j.egg-info/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2161 2023-04-17 22:06:16.000000 gpt4all-j-0.1.1/gpt4all_j.egg-info/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      383 2023-04-17 22:06:16.000000 gpt4all-j-0.1.1/gpt4all_j.egg-info/SOURCES.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-17 22:06:16.000000 gpt4all-j-0.1.1/gpt4all_j.egg-info/dependency_links.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-17 22:06:16.000000 gpt4all-j-0.1.1/gpt4all_j.egg-info/not-zip-safe
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-04-17 22:06:16.000000 gpt4all-j-0.1.1/gpt4all_j.egg-info/top_level.txt
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 22:06:16.462461 gpt4all-j-0.1.1/gpt4allj/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       55 2023-04-17 19:06:48.000000 gpt4all-j-0.1.1/gpt4allj/__init__.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 22:06:16.472461 gpt4all-j-0.1.1/gpt4allj/lib/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   304128 2023-04-17 17:56:24.000000 gpt4all-j-0.1.1/gpt4allj/lib/ggml.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   896000 2023-04-17 17:56:27.000000 gpt4all-j-0.1.1/gpt4allj/lib/gptj.dll
--rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   400954 2023-04-17 21:58:27.000000 gpt4all-j-0.1.1/gpt4allj/lib/libggml.dylib
--rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   169848 2023-04-17 17:54:20.000000 gpt4all-j-0.1.1/gpt4allj/lib/libggml.so
--rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   365898 2023-04-17 21:58:27.000000 gpt4all-j-0.1.1/gpt4allj/lib/libgptj.dylib
--rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   268536 2023-04-17 17:53:22.000000 gpt4all-j-0.1.1/gpt4allj/lib/libgptj.so
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1450 2023-04-17 21:58:27.000000 gpt4all-j-0.1.1/gpt4allj/lib.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1338 2023-04-17 19:12:58.000000 gpt4all-j-0.1.1/gpt4allj/model.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-04-17 22:06:16.482461 gpt4all-j-0.1.1/setup.cfg
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      908 2023-04-17 21:59:45.000000 gpt4all-j-0.1.1/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 22:26:30.342463 gpt4all-j-0.1.2/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2161 2023-04-17 22:26:30.342463 gpt4all-j-0.1.2/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1138 2023-04-17 22:04:59.000000 gpt4all-j-0.1.2/README.md
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 22:26:30.332463 gpt4all-j-0.1.2/gpt4all_j.egg-info/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2161 2023-04-17 22:26:30.000000 gpt4all-j-0.1.2/gpt4all_j.egg-info/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      383 2023-04-17 22:26:30.000000 gpt4all-j-0.1.2/gpt4all_j.egg-info/SOURCES.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-17 22:26:30.000000 gpt4all-j-0.1.2/gpt4all_j.egg-info/dependency_links.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-17 22:26:30.000000 gpt4all-j-0.1.2/gpt4all_j.egg-info/not-zip-safe
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-04-17 22:26:30.000000 gpt4all-j-0.1.2/gpt4all_j.egg-info/top_level.txt
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 22:26:30.332463 gpt4all-j-0.1.2/gpt4allj/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       55 2023-04-17 19:06:48.000000 gpt4all-j-0.1.2/gpt4allj/__init__.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 22:26:30.342463 gpt4all-j-0.1.2/gpt4allj/lib/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   304128 2023-04-17 17:56:24.000000 gpt4all-j-0.1.2/gpt4allj/lib/ggml.dll
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   896000 2023-04-17 17:56:27.000000 gpt4all-j-0.1.2/gpt4allj/lib/gptj.dll
+-rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   400954 2023-04-17 21:58:27.000000 gpt4all-j-0.1.2/gpt4allj/lib/libggml.dylib
+-rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   169848 2023-04-17 17:54:20.000000 gpt4all-j-0.1.2/gpt4allj/lib/libggml.so
+-rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   365898 2023-04-17 21:58:27.000000 gpt4all-j-0.1.2/gpt4allj/lib/libgptj.dylib
+-rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   268536 2023-04-17 17:53:22.000000 gpt4all-j-0.1.2/gpt4allj/lib/libgptj.so
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1455 2023-04-17 22:16:48.000000 gpt4all-j-0.1.2/gpt4allj/lib.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1338 2023-04-17 19:12:58.000000 gpt4all-j-0.1.2/gpt4allj/model.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-04-17 22:26:30.342463 gpt4all-j-0.1.2/setup.cfg
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      908 2023-04-17 22:18:29.000000 gpt4all-j-0.1.2/setup.py
```

### Comparing `gpt4all-j-0.1.1/PKG-INFO` & `gpt4all-j-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4all-j
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python bindings for the C++ port of GPT4All-J model.
 Home-page: UNKNOWN
 License: MIT
 Description: # [GPT4All-J](https://github.com/marella/gpt4all-j)
         
         Python bindings for the [C++ port][gptj.cpp] of GPT4All-J model.
```

### Comparing `gpt4all-j-0.1.1/README.md` & `gpt4all-j-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.1.1/gpt4all_j.egg-info/PKG-INFO` & `gpt4all-j-0.1.2/gpt4all_j.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4all-j
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python bindings for the C++ port of GPT4All-J model.
 Home-page: UNKNOWN
 License: MIT
 Description: # [GPT4All-J](https://github.com/marella/gpt4all-j)
         
         Python bindings for the [C++ port][gptj.cpp] of GPT4All-J model.
```

### Comparing `gpt4all-j-0.1.1/gpt4allj/lib/ggml.dll` & `gpt4all-j-0.1.2/gpt4allj/lib/ggml.dll`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.1.1/gpt4allj/lib/gptj.dll` & `gpt4all-j-0.1.2/gpt4allj/lib/gptj.dll`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.1.1/gpt4allj/lib/libggml.dylib` & `gpt4all-j-0.1.2/gpt4allj/lib/libggml.dylib`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.1.1/gpt4allj/lib/libggml.so` & `gpt4all-j-0.1.2/gpt4allj/lib/libggml.so`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.1.1/gpt4allj/lib/libgptj.dylib` & `gpt4all-j-0.1.2/gpt4allj/lib/libgptj.dylib`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.1.1/gpt4allj/lib/libgptj.so` & `gpt4all-j-0.1.2/gpt4allj/lib/libgptj.so`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.1.1/gpt4allj/lib.py` & `gpt4all-j-0.1.2/gpt4allj/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     elif sys.platform.startswith('win32'):
         name = f'{name}.dll'
     elif sys.platform.startswith('darwin'):
         name = f'lib{name}.dylib'
     else:
         raise OSError('The current platform is not supported. ' +
                       'Please try building the C++ library from source.')
-    return Path(__file__).parent.resolve() / 'lib' / name
+    return str(Path(__file__).parent.resolve() / 'lib' / name)
 
 
 def load_library(gptj=None, ggml=None):
     if gptj is None:
         gptj = find_library('gptj')
     if ggml is None:
         ggml = find_library('ggml')
```

### Comparing `gpt4all-j-0.1.1/gpt4allj/model.py` & `gpt4all-j-0.1.2/gpt4allj/model.py`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.1.1/setup.py` & `gpt4all-j-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as f:
     long_description = f.read()
 
 name = 'gpt4all-j'
 
 setup(
     name=name,
-    version='0.1.1',
+    version='0.1.2',
     description='Python bindings for the C++ port of GPT4All-J model.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     packages=find_packages(),
     package_data={'gpt4allj': ['**/*.so', '**/*.dll', '**/*.dylib']},
     install_requires=[],
```

