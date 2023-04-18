# Comparing `tmp/streamlit-component-dropfilltextarea-0.1.0.tar.gz` & `tmp/streamlit-component-dropfilltextarea-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-component-dropfilltextarea-0.1.0.tar", last modified: Tue Apr 18 10:53:15 2023, max compression
+gzip compressed data, was "streamlit-component-dropfilltextarea-0.1.1.tar", last modified: Tue Apr 18 11:04:40 2023, max compression
```

## Comparing `streamlit-component-dropfilltextarea-0.1.0.tar` & `streamlit-component-dropfilltextarea-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,26 @@
-drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-04-18 10:53:15.603323 streamlit-component-dropfilltextarea-0.1.0/
--rwxrwxrwx   0 frank     (1000) frank     (1000)     1069 2023-04-17 12:15:35.000000 streamlit-component-dropfilltextarea-0.1.0/LICENSE
--rwxrwxrwx   0 frank     (1000) frank     (1000)       94 2023-04-17 12:38:47.000000 streamlit-component-dropfilltextarea-0.1.0/MANIFEST.in
--rw-rw-r--   0 frank     (1000) frank     (1000)     1345 2023-04-18 10:53:15.599323 streamlit-component-dropfilltextarea-0.1.0/PKG-INFO
--rwxrwxrwx   0 frank     (1000) frank     (1000)      836 2023-04-18 10:53:06.000000 streamlit-component-dropfilltextarea-0.1.0/README.md
--rw-rw-r--   0 frank     (1000) frank     (1000)       38 2023-04-18 10:53:15.603323 streamlit-component-dropfilltextarea-0.1.0/setup.cfg
--rwxrwxrwx   0 frank     (1000) frank     (1000)      904 2023-04-18 10:53:12.000000 streamlit-component-dropfilltextarea-0.1.0/setup.py
-drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-04-18 10:53:15.595323 streamlit-component-dropfilltextarea-0.1.0/src/
-drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-04-18 10:53:15.599323 streamlit-component-dropfilltextarea-0.1.0/src/st_dropfill_textarea/
--rwxrwxrwx   0 frank     (1000) frank     (1000)     2514 2023-04-18 10:21:06.000000 streamlit-component-dropfilltextarea-0.1.0/src/st_dropfill_textarea/__init__.py
-drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-04-18 10:53:15.599323 streamlit-component-dropfilltextarea-0.1.0/src/streamlit_component_dropfilltextarea.egg-info/
--rw-rw-r--   0 frank     (1000) frank     (1000)     1345 2023-04-18 10:53:15.000000 streamlit-component-dropfilltextarea-0.1.0/src/streamlit_component_dropfilltextarea.egg-info/PKG-INFO
--rw-rw-r--   0 frank     (1000) frank     (1000)      394 2023-04-18 10:53:15.000000 streamlit-component-dropfilltextarea-0.1.0/src/streamlit_component_dropfilltextarea.egg-info/SOURCES.txt
--rw-rw-r--   0 frank     (1000) frank     (1000)        1 2023-04-18 10:53:15.000000 streamlit-component-dropfilltextarea-0.1.0/src/streamlit_component_dropfilltextarea.egg-info/dependency_links.txt
--rw-rw-r--   0 frank     (1000) frank     (1000)       22 2023-04-18 10:53:15.000000 streamlit-component-dropfilltextarea-0.1.0/src/streamlit_component_dropfilltextarea.egg-info/requires.txt
--rw-rw-r--   0 frank     (1000) frank     (1000)       21 2023-04-18 10:53:15.000000 streamlit-component-dropfilltextarea-0.1.0/src/streamlit_component_dropfilltextarea.egg-info/top_level.txt
+drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-04-18 11:04:40.628941 streamlit-component-dropfilltextarea-0.1.1/
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     1069 2023-04-17 12:15:35.000000 streamlit-component-dropfilltextarea-0.1.1/LICENSE
+-rwxrwxrwx   0 frank     (1000) frank     (1000)       93 2023-04-18 11:03:01.000000 streamlit-component-dropfilltextarea-0.1.1/MANIFEST.in
+-rw-rw-r--   0 frank     (1000) frank     (1000)     1345 2023-04-18 11:04:40.628941 streamlit-component-dropfilltextarea-0.1.1/PKG-INFO
+-rwxrwxrwx   0 frank     (1000) frank     (1000)      836 2023-04-18 10:53:06.000000 streamlit-component-dropfilltextarea-0.1.1/README.md
+-rw-rw-r--   0 frank     (1000) frank     (1000)       38 2023-04-18 11:04:40.628941 streamlit-component-dropfilltextarea-0.1.1/setup.cfg
+-rwxrwxrwx   0 frank     (1000) frank     (1000)      904 2023-04-18 10:58:02.000000 streamlit-component-dropfilltextarea-0.1.1/setup.py
+drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-04-18 11:04:40.608941 streamlit-component-dropfilltextarea-0.1.1/src/
+drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-04-18 11:04:40.612941 streamlit-component-dropfilltextarea-0.1.1/src/st_dropfill_textarea/
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     2514 2023-04-18 10:21:06.000000 streamlit-component-dropfilltextarea-0.1.1/src/st_dropfill_textarea/__init__.py
+drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-04-18 11:04:40.604941 streamlit-component-dropfilltextarea-0.1.1/src/st_dropfill_textarea/frontend/
+drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-04-18 11:04:40.612941 streamlit-component-dropfilltextarea-0.1.1/src/st_dropfill_textarea/frontend/dist/
+drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-04-18 11:04:40.612941 streamlit-component-dropfilltextarea-0.1.1/src/st_dropfill_textarea/frontend/dist/css/
+-rw-rw-r--   0 frank     (1000) frank     (1000)      600 2023-04-18 10:14:17.000000 streamlit-component-dropfilltextarea-0.1.1/src/st_dropfill_textarea/frontend/dist/css/app.a458ce97.css
+-rw-rw-r--   0 frank     (1000) frank     (1000)      725 2023-04-18 10:14:17.000000 streamlit-component-dropfilltextarea-0.1.1/src/st_dropfill_textarea/frontend/dist/index.html
+drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-04-18 11:04:40.616941 streamlit-component-dropfilltextarea-0.1.1/src/st_dropfill_textarea/frontend/dist/js/
+-rw-rw-r--   0 frank     (1000) frank     (1000)     7676 2023-04-18 10:14:17.000000 streamlit-component-dropfilltextarea-0.1.1/src/st_dropfill_textarea/frontend/dist/js/app.338e43a2.js
+-rw-rw-r--   0 frank     (1000) frank     (1000)    28746 2023-04-18 10:14:17.000000 streamlit-component-dropfilltextarea-0.1.1/src/st_dropfill_textarea/frontend/dist/js/app.338e43a2.js.map
+-rw-rw-r--   0 frank     (1000) frank     (1000)   865876 2023-04-18 10:14:17.000000 streamlit-component-dropfilltextarea-0.1.1/src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js
+-rw-rw-r--   0 frank     (1000) frank     (1000)  3348860 2023-04-18 10:14:17.000000 streamlit-component-dropfilltextarea-0.1.1/src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js.map
+drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-04-18 11:04:40.628941 streamlit-component-dropfilltextarea-0.1.1/src/streamlit_component_dropfilltextarea.egg-info/
+-rw-rw-r--   0 frank     (1000) frank     (1000)     1345 2023-04-18 11:04:40.000000 streamlit-component-dropfilltextarea-0.1.1/src/streamlit_component_dropfilltextarea.egg-info/PKG-INFO
+-rw-rw-r--   0 frank     (1000) frank     (1000)      764 2023-04-18 11:04:40.000000 streamlit-component-dropfilltextarea-0.1.1/src/streamlit_component_dropfilltextarea.egg-info/SOURCES.txt
+-rw-rw-r--   0 frank     (1000) frank     (1000)        1 2023-04-18 11:04:40.000000 streamlit-component-dropfilltextarea-0.1.1/src/streamlit_component_dropfilltextarea.egg-info/dependency_links.txt
+-rw-rw-r--   0 frank     (1000) frank     (1000)       22 2023-04-18 11:04:40.000000 streamlit-component-dropfilltextarea-0.1.1/src/streamlit_component_dropfilltextarea.egg-info/requires.txt
+-rw-rw-r--   0 frank     (1000) frank     (1000)       21 2023-04-18 11:04:40.000000 streamlit-component-dropfilltextarea-0.1.1/src/streamlit_component_dropfilltextarea.egg-info/top_level.txt
```

### Comparing `streamlit-component-dropfilltextarea-0.1.0/LICENSE` & `streamlit-component-dropfilltextarea-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-component-dropfilltextarea-0.1.0/PKG-INFO` & `streamlit-component-dropfilltextarea-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-component-dropfilltextarea
-Version: 0.1.0
+Version: 0.1.1
 Summary: Streamlit's DropFillTextarea lets users drag and drop files onto a text area, filling in text quickly. It populates text areas with pre-existing files, reducing manual input, while offering layout customization. Ideal for simplifying workflows for both developers and users.
 Author: Jiayi Chen
 Author-email: chenjiayi_344@hotmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-component-dropfilltextarea-0.1.0/README.md` & `streamlit-component-dropfilltextarea-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-component-dropfilltextarea-0.1.0/setup.py` & `streamlit-component-dropfilltextarea-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-component-dropfilltextarea",
-    version="0.1.0",
+    version="0.1.1",
     author="Jiayi Chen",
     author_email="chenjiayi_344@hotmail.com",
     description="Streamlit's DropFillTextarea lets users drag and drop files onto a text area, filling in text quickly. It populates text areas with pre-existing files, reducing manual input, while offering layout customization. Ideal for simplifying workflows for both developers and users.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
```

### Comparing `streamlit-component-dropfilltextarea-0.1.0/src/st_dropfill_textarea/__init__.py` & `streamlit-component-dropfilltextarea-0.1.1/src/st_dropfill_textarea/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-component-dropfilltextarea-0.1.0/src/streamlit_component_dropfilltextarea.egg-info/PKG-INFO` & `streamlit-component-dropfilltextarea-0.1.1/src/streamlit_component_dropfilltextarea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-component-dropfilltextarea
-Version: 0.1.0
+Version: 0.1.1
 Summary: Streamlit's DropFillTextarea lets users drag and drop files onto a text area, filling in text quickly. It populates text areas with pre-existing files, reducing manual input, while offering layout customization. Ideal for simplifying workflows for both developers and users.
 Author: Jiayi Chen
 Author-email: chenjiayi_344@hotmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

