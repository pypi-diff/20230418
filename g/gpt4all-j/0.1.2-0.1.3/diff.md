# Comparing `tmp/gpt4all-j-0.1.2.tar.gz` & `tmp/gpt4all-j-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4all-j-0.1.2.tar", last modified: Mon Apr 17 22:26:30 2023, max compression
+gzip compressed data, was "gpt4all-j-0.1.3.tar", last modified: Tue Apr 18 13:19:55 2023, max compression
```

## Comparing `gpt4all-j-0.1.2.tar` & `gpt4all-j-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 22:26:30.342463 gpt4all-j-0.1.2/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2161 2023-04-17 22:26:30.342463 gpt4all-j-0.1.2/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1138 2023-04-17 22:04:59.000000 gpt4all-j-0.1.2/README.md
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 22:26:30.332463 gpt4all-j-0.1.2/gpt4all_j.egg-info/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2161 2023-04-17 22:26:30.000000 gpt4all-j-0.1.2/gpt4all_j.egg-info/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      383 2023-04-17 22:26:30.000000 gpt4all-j-0.1.2/gpt4all_j.egg-info/SOURCES.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-17 22:26:30.000000 gpt4all-j-0.1.2/gpt4all_j.egg-info/dependency_links.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-17 22:26:30.000000 gpt4all-j-0.1.2/gpt4all_j.egg-info/not-zip-safe
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-04-17 22:26:30.000000 gpt4all-j-0.1.2/gpt4all_j.egg-info/top_level.txt
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 22:26:30.332463 gpt4all-j-0.1.2/gpt4allj/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       55 2023-04-17 19:06:48.000000 gpt4all-j-0.1.2/gpt4allj/__init__.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 22:26:30.342463 gpt4all-j-0.1.2/gpt4allj/lib/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   304128 2023-04-17 17:56:24.000000 gpt4all-j-0.1.2/gpt4allj/lib/ggml.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   896000 2023-04-17 17:56:27.000000 gpt4all-j-0.1.2/gpt4allj/lib/gptj.dll
--rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   400954 2023-04-17 21:58:27.000000 gpt4all-j-0.1.2/gpt4allj/lib/libggml.dylib
--rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   169848 2023-04-17 17:54:20.000000 gpt4all-j-0.1.2/gpt4allj/lib/libggml.so
--rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   365898 2023-04-17 21:58:27.000000 gpt4all-j-0.1.2/gpt4allj/lib/libgptj.dylib
--rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   268536 2023-04-17 17:53:22.000000 gpt4all-j-0.1.2/gpt4allj/lib/libgptj.so
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1455 2023-04-17 22:16:48.000000 gpt4all-j-0.1.2/gpt4allj/lib.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1338 2023-04-17 19:12:58.000000 gpt4all-j-0.1.2/gpt4allj/model.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-04-17 22:26:30.342463 gpt4all-j-0.1.2/setup.cfg
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      908 2023-04-17 22:18:29.000000 gpt4all-j-0.1.2/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-18 13:19:55.823923 gpt4all-j-0.1.3/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2195 2023-04-18 13:19:55.823923 gpt4all-j-0.1.3/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1164 2023-04-18 13:10:57.000000 gpt4all-j-0.1.3/README.md
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-18 13:19:55.803923 gpt4all-j-0.1.3/gpt4all_j.egg-info/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2195 2023-04-18 13:19:55.000000 gpt4all-j-0.1.3/gpt4all_j.egg-info/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      383 2023-04-18 13:19:55.000000 gpt4all-j-0.1.3/gpt4all_j.egg-info/SOURCES.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-18 13:19:55.000000 gpt4all-j-0.1.3/gpt4all_j.egg-info/dependency_links.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-18 13:19:55.000000 gpt4all-j-0.1.3/gpt4all_j.egg-info/not-zip-safe
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-04-18 13:19:55.000000 gpt4all-j-0.1.3/gpt4all_j.egg-info/top_level.txt
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-18 13:19:55.803923 gpt4all-j-0.1.3/gpt4allj/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       55 2023-04-17 19:06:48.000000 gpt4all-j-0.1.3/gpt4allj/__init__.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-18 13:19:55.823923 gpt4all-j-0.1.3/gpt4allj/lib/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   304128 2023-04-17 17:56:24.000000 gpt4all-j-0.1.3/gpt4allj/lib/ggml.dll
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   896000 2023-04-17 17:56:27.000000 gpt4all-j-0.1.3/gpt4allj/lib/gptj.dll
+-rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   400954 2023-04-17 21:58:27.000000 gpt4all-j-0.1.3/gpt4allj/lib/libggml.dylib
+-rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   169848 2023-04-17 17:54:20.000000 gpt4all-j-0.1.3/gpt4allj/lib/libggml.so
+-rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   365898 2023-04-17 21:58:27.000000 gpt4all-j-0.1.3/gpt4allj/lib/libgptj.dylib
+-rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   268536 2023-04-17 17:53:22.000000 gpt4all-j-0.1.3/gpt4allj/lib/libgptj.so
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1455 2023-04-18 12:53:57.000000 gpt4all-j-0.1.3/gpt4allj/lib.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1412 2023-04-18 13:01:45.000000 gpt4all-j-0.1.3/gpt4allj/model.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-04-18 13:19:55.823923 gpt4all-j-0.1.3/setup.cfg
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      908 2023-04-18 13:14:15.000000 gpt4all-j-0.1.3/setup.py
```

### Comparing `gpt4all-j-0.1.2/PKG-INFO` & `gpt4all-j-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4all-j
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python bindings for the C++ port of GPT4All-J model.
 Home-page: UNKNOWN
 License: MIT
 Description: # [GPT4All-J](https://github.com/marella/gpt4all-j)
         
         Python bindings for the [C++ port][gptj.cpp] of GPT4All-J model.
         
@@ -33,15 +33,16 @@
         ```py
         model.generate(prompt,
                        seed=-1,
                        n_threads=-1,
                        n_predict=200,
                        top_k=40,
                        top_p=0.9,
-                       temp=0.9)
+                       temp=0.9,
+                       n_batch=8)
         ```
         
         ### C++ Library
         
         To build the C++ library from source, please see [gptj.cpp][gptj.cpp]. Once you have built the shared libraries, you can use them as:
         
         ```py
```

### Comparing `gpt4all-j-0.1.2/README.md` & `gpt4all-j-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 ```py
 model.generate(prompt,
                seed=-1,
                n_threads=-1,
                n_predict=200,
                top_k=40,
                top_p=0.9,
-               temp=0.9)
+               temp=0.9,
+               n_batch=8)
 ```
 
 ### C++ Library
 
 To build the C++ library from source, please see [gptj.cpp][gptj.cpp]. Once you have built the shared libraries, you can use them as:
 
 ```py
```

### Comparing `gpt4all-j-0.1.2/gpt4all_j.egg-info/PKG-INFO` & `gpt4all-j-0.1.3/gpt4all_j.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4all-j
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python bindings for the C++ port of GPT4All-J model.
 Home-page: UNKNOWN
 License: MIT
 Description: # [GPT4All-J](https://github.com/marella/gpt4all-j)
         
         Python bindings for the [C++ port][gptj.cpp] of GPT4All-J model.
         
@@ -33,15 +33,16 @@
         ```py
         model.generate(prompt,
                        seed=-1,
                        n_threads=-1,
                        n_predict=200,
                        top_k=40,
                        top_p=0.9,
-                       temp=0.9)
+                       temp=0.9,
+                       n_batch=8)
         ```
         
         ### C++ Library
         
         To build the C++ library from source, please see [gptj.cpp][gptj.cpp]. Once you have built the shared libraries, you can use them as:
         
         ```py
```

### Comparing `gpt4all-j-0.1.2/gpt4allj/lib/ggml.dll` & `gpt4all-j-0.1.3/gpt4allj/lib/ggml.dll`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.1.2/gpt4allj/lib/gptj.dll` & `gpt4all-j-0.1.3/gpt4allj/lib/gptj.dll`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.1.2/gpt4allj/lib/libggml.dylib` & `gpt4all-j-0.1.3/gpt4allj/lib/libggml.dylib`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.1.2/gpt4allj/lib/libggml.so` & `gpt4all-j-0.1.3/gpt4allj/lib/libggml.so`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.1.2/gpt4allj/lib/libgptj.dylib` & `gpt4all-j-0.1.3/gpt4allj/lib/libgptj.dylib`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.1.2/gpt4allj/lib/libgptj.so` & `gpt4all-j-0.1.3/gpt4allj/lib/libgptj.so`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.1.2/gpt4allj/lib.py` & `gpt4all-j-0.1.3/gpt4allj/lib.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 class gptj_params(Structure):
     _fields_ = [
         ('seed', c_int32),
         ('n_threads', c_int32),
         ('n_predict', c_int32),
         ('top_k', c_int32),
-        ('n_batch', c_int32),
         ('top_p', c_float),
         ('temp', c_float),
+        ('n_batch', c_int32),
     ]
 
 
 def find_library(name):
     if sys.platform.startswith('linux'):
         name = f'lib{name}.so'
     elif sys.platform.startswith('win32'):
```

### Comparing `gpt4all-j-0.1.2/gpt4allj/model.py` & `gpt4all-j-0.1.3/gpt4allj/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,22 +16,24 @@
                  prompt,
                  seed=-1,
                  n_threads=-1,
                  n_predict=200,
                  top_k=40,
                  top_p=0.9,
                  temp=0.9,
+                 n_batch=8,
                  response_buffer_size=10000):
         prompt = prompt.encode()
         params = gptj_params(seed=seed,
                              n_threads=n_threads,
                              n_predict=n_predict,
                              top_k=top_k,
                              top_p=top_p,
-                             temp=temp)
+                             temp=temp,
+                             n_batch=n_batch)
         response = create_string_buffer(response_buffer_size)
         status = self._lib.gptj_generate(self._ctx, prompt, params, response)
         if not status:
             raise RuntimeError(f'Failed to generate response for "{prompt}"')
         return response.value.decode()
 
     def __del__(self):
```

### Comparing `gpt4all-j-0.1.2/setup.py` & `gpt4all-j-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as f:
     long_description = f.read()
 
 name = 'gpt4all-j'
 
 setup(
     name=name,
-    version='0.1.2',
+    version='0.1.3',
     description='Python bindings for the C++ port of GPT4All-J model.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     packages=find_packages(),
     package_data={'gpt4allj': ['**/*.so', '**/*.dll', '**/*.dylib']},
     install_requires=[],
```

