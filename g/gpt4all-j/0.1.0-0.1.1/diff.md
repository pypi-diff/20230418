# Comparing `tmp/gpt4all-j-0.1.0.tar.gz` & `tmp/gpt4all-j-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4all-j-0.1.0.tar", last modified: Mon Apr 17 20:50:01 2023, max compression
+gzip compressed data, was "gpt4all-j-0.1.1.tar", last modified: Mon Apr 17 22:06:16 2023, max compression
```

## Comparing `gpt4all-j-0.1.0.tar` & `gpt4all-j-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 20:50:01.112452 gpt4all-j-0.1.0/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2218 2023-04-17 20:50:01.112452 gpt4all-j-0.1.0/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1195 2023-04-17 20:47:51.000000 gpt4all-j-0.1.0/README.md
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 20:50:01.092452 gpt4all-j-0.1.0/gpt4all_j.egg-info/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2218 2023-04-17 20:50:00.000000 gpt4all-j-0.1.0/gpt4all_j.egg-info/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      329 2023-04-17 20:50:01.000000 gpt4all-j-0.1.0/gpt4all_j.egg-info/SOURCES.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-17 20:50:00.000000 gpt4all-j-0.1.0/gpt4all_j.egg-info/dependency_links.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-17 20:50:00.000000 gpt4all-j-0.1.0/gpt4all_j.egg-info/not-zip-safe
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-04-17 20:50:00.000000 gpt4all-j-0.1.0/gpt4all_j.egg-info/top_level.txt
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 20:50:01.092452 gpt4all-j-0.1.0/gpt4allj/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       55 2023-04-17 19:06:48.000000 gpt4all-j-0.1.0/gpt4allj/__init__.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 20:50:01.112452 gpt4all-j-0.1.0/gpt4allj/lib/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   304128 2023-04-17 17:56:24.000000 gpt4all-j-0.1.0/gpt4allj/lib/ggml.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   896000 2023-04-17 17:56:27.000000 gpt4all-j-0.1.0/gpt4allj/lib/gptj.dll
--rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   169848 2023-04-17 17:54:20.000000 gpt4all-j-0.1.0/gpt4allj/lib/libggml.so
--rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   268536 2023-04-17 17:53:22.000000 gpt4all-j-0.1.0/gpt4allj/lib/libgptj.so
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1372 2023-04-17 19:15:23.000000 gpt4all-j-0.1.0/gpt4allj/lib.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1338 2023-04-17 19:12:58.000000 gpt4all-j-0.1.0/gpt4allj/model.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-04-17 20:50:01.112452 gpt4all-j-0.1.0/setup.cfg
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      894 2023-04-17 20:47:02.000000 gpt4all-j-0.1.0/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 22:06:16.472461 gpt4all-j-0.1.1/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2161 2023-04-17 22:06:16.472461 gpt4all-j-0.1.1/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1138 2023-04-17 22:04:59.000000 gpt4all-j-0.1.1/README.md
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 22:06:16.462461 gpt4all-j-0.1.1/gpt4all_j.egg-info/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2161 2023-04-17 22:06:16.000000 gpt4all-j-0.1.1/gpt4all_j.egg-info/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      383 2023-04-17 22:06:16.000000 gpt4all-j-0.1.1/gpt4all_j.egg-info/SOURCES.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-17 22:06:16.000000 gpt4all-j-0.1.1/gpt4all_j.egg-info/dependency_links.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-17 22:06:16.000000 gpt4all-j-0.1.1/gpt4all_j.egg-info/not-zip-safe
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-04-17 22:06:16.000000 gpt4all-j-0.1.1/gpt4all_j.egg-info/top_level.txt
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 22:06:16.462461 gpt4all-j-0.1.1/gpt4allj/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       55 2023-04-17 19:06:48.000000 gpt4all-j-0.1.1/gpt4allj/__init__.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 22:06:16.472461 gpt4all-j-0.1.1/gpt4allj/lib/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   304128 2023-04-17 17:56:24.000000 gpt4all-j-0.1.1/gpt4allj/lib/ggml.dll
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   896000 2023-04-17 17:56:27.000000 gpt4all-j-0.1.1/gpt4allj/lib/gptj.dll
+-rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   400954 2023-04-17 21:58:27.000000 gpt4all-j-0.1.1/gpt4allj/lib/libggml.dylib
+-rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   169848 2023-04-17 17:54:20.000000 gpt4all-j-0.1.1/gpt4allj/lib/libggml.so
+-rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   365898 2023-04-17 21:58:27.000000 gpt4all-j-0.1.1/gpt4allj/lib/libgptj.dylib
+-rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   268536 2023-04-17 17:53:22.000000 gpt4all-j-0.1.1/gpt4allj/lib/libgptj.so
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1450 2023-04-17 21:58:27.000000 gpt4all-j-0.1.1/gpt4allj/lib.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1338 2023-04-17 19:12:58.000000 gpt4all-j-0.1.1/gpt4allj/model.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-04-17 22:06:16.482461 gpt4all-j-0.1.1/setup.cfg
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      908 2023-04-17 21:59:45.000000 gpt4all-j-0.1.1/setup.py
```

### Comparing `gpt4all-j-0.1.0/PKG-INFO` & `gpt4all-j-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4all-j
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python bindings for the C++ port of GPT4All-J model.
 Home-page: UNKNOWN
 License: MIT
 Description: # [GPT4All-J](https://github.com/marella/gpt4all-j)
         
         Python bindings for the [C++ port][gptj.cpp] of GPT4All-J model.
         
@@ -36,17 +36,17 @@
                        n_threads=-1,
                        n_predict=200,
                        top_k=40,
                        top_p=0.9,
                        temp=0.9)
         ```
         
-        ### macOS
+        ### C++ Library
         
-        macOS isn't supported out of the box yet but you can use it with Docker or try building the C++ library from source [here][gptj.cpp]. Once you have built the shared libraries, you can use them as:
+        To build the C++ library from source, please see [gptj.cpp][gptj.cpp]. Once you have built the shared libraries, you can use them as:
         
         ```py
         from gpt4allj import Model, load_library
         
         lib = load_library('/path/to/libgptj.so', '/path/to/libggml.so')
         
         model = Model('/path/to/ggml-gpt4all-j.bin', lib=lib)
```

### Comparing `gpt4all-j-0.1.0/README.md` & `gpt4all-j-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,17 +30,17 @@
                n_threads=-1,
                n_predict=200,
                top_k=40,
                top_p=0.9,
                temp=0.9)
 ```
 
-### macOS
+### C++ Library
 
-macOS isn't supported out of the box yet but you can use it with Docker or try building the C++ library from source [here][gptj.cpp]. Once you have built the shared libraries, you can use them as:
+To build the C++ library from source, please see [gptj.cpp][gptj.cpp]. Once you have built the shared libraries, you can use them as:
 
 ```py
 from gpt4allj import Model, load_library
 
 lib = load_library('/path/to/libgptj.so', '/path/to/libggml.so')
 
 model = Model('/path/to/ggml-gpt4all-j.bin', lib=lib)
```

### Comparing `gpt4all-j-0.1.0/gpt4all_j.egg-info/PKG-INFO` & `gpt4all-j-0.1.1/gpt4all_j.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4all-j
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python bindings for the C++ port of GPT4All-J model.
 Home-page: UNKNOWN
 License: MIT
 Description: # [GPT4All-J](https://github.com/marella/gpt4all-j)
         
         Python bindings for the [C++ port][gptj.cpp] of GPT4All-J model.
         
@@ -36,17 +36,17 @@
                        n_threads=-1,
                        n_predict=200,
                        top_k=40,
                        top_p=0.9,
                        temp=0.9)
         ```
         
-        ### macOS
+        ### C++ Library
         
-        macOS isn't supported out of the box yet but you can use it with Docker or try building the C++ library from source [here][gptj.cpp]. Once you have built the shared libraries, you can use them as:
+        To build the C++ library from source, please see [gptj.cpp][gptj.cpp]. Once you have built the shared libraries, you can use them as:
         
         ```py
         from gpt4allj import Model, load_library
         
         lib = load_library('/path/to/libgptj.so', '/path/to/libggml.so')
         
         model = Model('/path/to/ggml-gpt4all-j.bin', lib=lib)
```

### Comparing `gpt4all-j-0.1.0/gpt4allj/lib/ggml.dll` & `gpt4all-j-0.1.1/gpt4allj/lib/ggml.dll`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.1.0/gpt4allj/lib/gptj.dll` & `gpt4all-j-0.1.1/gpt4allj/lib/gptj.dll`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.1.0/gpt4allj/lib/libggml.so` & `gpt4all-j-0.1.1/gpt4allj/lib/libggml.so`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.1.0/gpt4allj/lib/libgptj.so` & `gpt4all-j-0.1.1/gpt4allj/lib/libgptj.so`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.1.0/gpt4allj/lib.py` & `gpt4all-j-0.1.1/gpt4allj/lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 
 
 def find_library(name):
     if sys.platform.startswith('linux'):
         name = f'lib{name}.so'
     elif sys.platform.startswith('win32'):
         name = f'{name}.dll'
+    elif sys.platform.startswith('darwin'):
+        name = f'lib{name}.dylib'
     else:
         raise OSError('The current platform is not supported. ' +
                       'Please try building the C++ library from source.')
     return Path(__file__).parent.resolve() / 'lib' / name
 
 
 def load_library(gptj=None, ggml=None):
```

### Comparing `gpt4all-j-0.1.0/gpt4allj/model.py` & `gpt4all-j-0.1.1/gpt4allj/model.py`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.1.0/setup.py` & `gpt4all-j-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 with open('README.md') as f:
     long_description = f.read()
 
 name = 'gpt4all-j'
 
 setup(
     name=name,
-    version='0.1.0',
+    version='0.1.1',
     description='Python bindings for the C++ port of GPT4All-J model.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     packages=find_packages(),
-    package_data={'gpt4allj': ['**/*.so', '**/*.dll']},
+    package_data={'gpt4allj': ['**/*.so', '**/*.dll', '**/*.dylib']},
     install_requires=[],
     zip_safe=False,
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

