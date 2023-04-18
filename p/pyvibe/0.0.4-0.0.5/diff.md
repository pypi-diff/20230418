# Comparing `tmp/pyvibe-0.0.4.tar.gz` & `tmp/pyvibe-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvibe-0.0.4.tar", last modified: Mon Apr 17 17:31:39 2023, max compression
+gzip compressed data, was "pyvibe-0.0.5.tar", last modified: Tue Apr 18 00:45:02 2023, max compression
```

## Comparing `pyvibe-0.0.4.tar` & `pyvibe-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:39.293241 pyvibe-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-17 17:31:24.000000 pyvibe-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-17 17:31:39.293241 pyvibe-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-04-17 17:31:24.000000 pyvibe-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-17 17:31:24.000000 pyvibe-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 17:31:39.293241 pyvibe-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:39.289241 pyvibe-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:39.289241 pyvibe-0.0.4/src/pyvibe/
--rw-r--r--   0 runner    (1001) docker     (123)   110451 2023-04-17 17:31:24.000000 pyvibe-0.0.4/src/pyvibe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-17 17:31:24.000000 pyvibe-0.0.4/src/pyvibe/component_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:39.293241 pyvibe-0.0.4/src/pyvibe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-17 17:31:39.000000 pyvibe-0.0.4/src/pyvibe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-17 17:31:39.000000 pyvibe-0.0.4/src/pyvibe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:31:39.000000 pyvibe-0.0.4/src/pyvibe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 17:31:39.000000 pyvibe-0.0.4/src/pyvibe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:45:02.785133 pyvibe-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-18 00:44:51.000000 pyvibe-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-18 00:45:02.785133 pyvibe-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-04-18 00:44:51.000000 pyvibe-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-18 00:44:51.000000 pyvibe-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 00:45:02.785133 pyvibe-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:45:02.781133 pyvibe-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:45:02.785133 pyvibe-0.0.5/src/pyvibe/
+-rw-r--r--   0 runner    (1001) docker     (123)   110449 2023-04-18 00:44:51.000000 pyvibe-0.0.5/src/pyvibe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-18 00:44:51.000000 pyvibe-0.0.5/src/pyvibe/component_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:45:02.785133 pyvibe-0.0.5/src/pyvibe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-18 00:45:02.000000 pyvibe-0.0.5/src/pyvibe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-18 00:45:02.000000 pyvibe-0.0.5/src/pyvibe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 00:45:02.000000 pyvibe-0.0.5/src/pyvibe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 00:45:02.000000 pyvibe-0.0.5/src/pyvibe.egg-info/top_level.txt
```

### Comparing `pyvibe-0.0.4/LICENSE` & `pyvibe-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvibe-0.0.4/PKG-INFO` & `pyvibe-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvibe
-Version: 0.0.4
+Version: 0.0.5
 Summary: Easily create styled web pages with Python
 Author-email: Zain Hoda <zain@pycob.com>
 Project-URL: Homepage, https://github.com/pycob/pyvibe
 Project-URL: Bug Tracker, https://github.com/pycob/pyvibe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyvibe Version: 0.0.4 Summary: Easily create styled
+Metadata-Version: 2.1 Name: pyvibe Version: 0.0.5 Summary: Easily create styled
 web pages with Python Author-email: Zain Hoda
 pycob.com> Project-URL: Homepage, https://github.com/pycob/pyvibe Project-URL:
 Bug Tracker, https://github.com/pycob/pyvibe/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # PyVibe https://
 www.pyvibe.com/ | [Examples](https://www.pyvibe.com/gallery.html) | [Use With
```

### Comparing `pyvibe-0.0.4/README.md` & `pyvibe-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyvibe-0.0.4/src/pyvibe/__init__.py` & `pyvibe-0.0.5/src/pyvibe/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -464,15 +464,15 @@
     return '''<div class="mx-auto my-10 max-w-3xl">
     <div class="flex h-11 w-full items-center justify-start space-x-1.5 rounded-t-lg bg-gray-900 px-3">
         <span class="h-3 w-3 rounded-full bg-red-400"></span>
         <span class="h-3 w-3 rounded-full bg-yellow-400"></span>
         <span class="h-3 w-3 rounded-full bg-green-400"></span>
         <code class="pl-5 text-lime-500">''' + self.header + '''</code>
     </div>
-    <div class="w-full border-t-0 bg-gray-700 pb-5 rounded-b-lg whitespace-nowrap overflow-x-scroll p-2">
+    <div class="w-full border-t-0 bg-gray-700 pb-5 rounded-b-lg whitespace-nowrap overflow-x-auto p-2">
         <code class="text-gray-500">''' + self.prefix + '''</code>
         <code class="text-white" style="white-space: break-spaces">''' + self.value + '''</code>
     </div>
 </div>'''
 
 class CodeeditorComponent(Component):
   """You don't normally need to invoke this constructor directly. Instead, use the `.add_codeeditor` method of the parent component.
```

### Comparing `pyvibe-0.0.4/src/pyvibe.egg-info/PKG-INFO` & `pyvibe-0.0.5/src/pyvibe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvibe
-Version: 0.0.4
+Version: 0.0.5
 Summary: Easily create styled web pages with Python
 Author-email: Zain Hoda <zain@pycob.com>
 Project-URL: Homepage, https://github.com/pycob/pyvibe
 Project-URL: Bug Tracker, https://github.com/pycob/pyvibe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyvibe Version: 0.0.4 Summary: Easily create styled
+Metadata-Version: 2.1 Name: pyvibe Version: 0.0.5 Summary: Easily create styled
 web pages with Python Author-email: Zain Hoda
 pycob.com> Project-URL: Homepage, https://github.com/pycob/pyvibe Project-URL:
 Bug Tracker, https://github.com/pycob/pyvibe/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # PyVibe https://
 www.pyvibe.com/ | [Examples](https://www.pyvibe.com/gallery.html) | [Use With
```

