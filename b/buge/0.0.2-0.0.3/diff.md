# Comparing `tmp/buge-0.0.2.tar.gz` & `tmp/buge-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buge-0.0.2.tar", last modified: Sat Apr 15 16:04:45 2023, max compression
+gzip compressed data, was "buge-0.0.3.tar", last modified: Tue Apr 18 02:32:29 2023, max compression
```

## Comparing `buge-0.0.2.tar` & `buge-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-15 16:04:45.847038 buge-0.0.2/
--rw-r--r--   0 damonpickett   (501) staff       (20)     1073 2023-04-14 22:43:18.000000 buge-0.0.2/LICENSE
--rw-r--r--   0 damonpickett   (501) staff       (20)       25 2023-04-14 22:43:29.000000 buge-0.0.2/MANIFEST.in
--rw-r--r--   0 damonpickett   (501) staff       (20)      637 2023-04-15 16:04:45.847084 buge-0.0.2/PKG-INFO
--rw-r--r--   0 damonpickett   (501) staff       (20)        0 2023-04-14 22:43:42.000000 buge-0.0.2/README.md
-drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-15 16:04:45.846087 buge-0.0.2/buge/
--rw-r--r--   0 damonpickett   (501) staff       (20)     1949 2023-04-15 05:23:59.000000 buge-0.0.2/buge/main.py
-drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-15 16:04:45.846940 buge-0.0.2/buge.egg-info/
--rw-r--r--   0 damonpickett   (501) staff       (20)      637 2023-04-15 16:04:45.000000 buge-0.0.2/buge.egg-info/PKG-INFO
--rw-r--r--   0 damonpickett   (501) staff       (20)      246 2023-04-15 16:04:45.000000 buge-0.0.2/buge.egg-info/SOURCES.txt
--rw-r--r--   0 damonpickett   (501) staff       (20)        1 2023-04-15 16:04:45.000000 buge-0.0.2/buge.egg-info/dependency_links.txt
--rw-r--r--   0 damonpickett   (501) staff       (20)       40 2023-04-15 16:04:45.000000 buge-0.0.2/buge.egg-info/entry_points.txt
--rw-r--r--   0 damonpickett   (501) staff       (20)       26 2023-04-15 16:04:45.000000 buge-0.0.2/buge.egg-info/requires.txt
--rw-r--r--   0 damonpickett   (501) staff       (20)        5 2023-04-15 16:04:45.000000 buge-0.0.2/buge.egg-info/top_level.txt
--rw-r--r--   0 damonpickett   (501) staff       (20)      644 2023-04-15 16:04:12.000000 buge-0.0.2/pyproject.toml
--rw-r--r--   0 damonpickett   (501) staff       (20)      784 2023-04-15 16:04:45.847332 buge-0.0.2/setup.cfg
--rw-r--r--   0 damonpickett   (501) staff       (20)       37 2023-04-13 22:46:26.000000 buge-0.0.2/setup.py
+drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-18 02:32:29.912489 buge-0.0.3/
+-rw-r--r--   0 damonpickett   (501) staff       (20)     1073 2023-04-14 22:43:18.000000 buge-0.0.3/LICENSE
+-rw-r--r--   0 damonpickett   (501) staff       (20)       25 2023-04-14 22:43:29.000000 buge-0.0.3/MANIFEST.in
+-rw-r--r--   0 damonpickett   (501) staff       (20)      637 2023-04-18 02:32:29.912531 buge-0.0.3/PKG-INFO
+-rw-r--r--   0 damonpickett   (501) staff       (20)        0 2023-04-14 22:43:42.000000 buge-0.0.3/README.md
+drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-18 02:32:29.911628 buge-0.0.3/buge/
+-rw-r--r--   0 damonpickett   (501) staff       (20)     2028 2023-04-18 02:30:28.000000 buge-0.0.3/buge/main.py
+drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-18 02:32:29.912393 buge-0.0.3/buge.egg-info/
+-rw-r--r--   0 damonpickett   (501) staff       (20)      637 2023-04-18 02:32:29.000000 buge-0.0.3/buge.egg-info/PKG-INFO
+-rw-r--r--   0 damonpickett   (501) staff       (20)      246 2023-04-18 02:32:29.000000 buge-0.0.3/buge.egg-info/SOURCES.txt
+-rw-r--r--   0 damonpickett   (501) staff       (20)        1 2023-04-18 02:32:29.000000 buge-0.0.3/buge.egg-info/dependency_links.txt
+-rw-r--r--   0 damonpickett   (501) staff       (20)       40 2023-04-18 02:32:29.000000 buge-0.0.3/buge.egg-info/entry_points.txt
+-rw-r--r--   0 damonpickett   (501) staff       (20)       26 2023-04-18 02:32:29.000000 buge-0.0.3/buge.egg-info/requires.txt
+-rw-r--r--   0 damonpickett   (501) staff       (20)        5 2023-04-18 02:32:29.000000 buge-0.0.3/buge.egg-info/top_level.txt
+-rw-r--r--   0 damonpickett   (501) staff       (20)      644 2023-04-18 02:30:40.000000 buge-0.0.3/pyproject.toml
+-rw-r--r--   0 damonpickett   (501) staff       (20)      784 2023-04-18 02:32:29.912764 buge-0.0.3/setup.cfg
+-rw-r--r--   0 damonpickett   (501) staff       (20)       37 2023-04-13 22:46:26.000000 buge-0.0.3/setup.py
```

### Comparing `buge-0.0.2/LICENSE` & `buge-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `buge-0.0.2/PKG-INFO` & `buge-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buge
-Version: 0.0.2
+Version: 0.0.3
 Summary: buge is a command-line application that uses the OpenAI API to diagnose bugs when programming.
 Home-page: https://github.com/damonpickett/buge
 Author: Damon Pickett
 Author-email: Damon Pickett <damon.pickett@gmail.com>
 Project-URL: Homepage, https://github.com/damonpickett/buge
 Project-URL: Bug Tracker, https://github.com/damonpickett/buge/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `buge-0.0.2/buge/main.py` & `buge-0.0.3/buge/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,16 @@
     # Check if OPENAI_API_KEY is set in the environment
     if not os.getenv("OPENAI_API_KEY"):
 
         # Prompt user for OPENAI_API_KEY value
         openai_api_key = input("Please enter your OpenAI API key: ")
 
         # Write value to .env file
-        with open(".env", "w") as f:
+        env_file_path = os.path.join(os.path.dirname(__file__), ".env")
+        with open(env_file_path, "w") as f:
             f.write(f"OPENAI_API_KEY={openai_api_key}")
         
         load_dotenv()
 
     openai.api_key = os.getenv("OPENAI_API_KEY")
 
     error_message = input("Please paste your error code here: ")
```

### Comparing `buge-0.0.2/buge.egg-info/PKG-INFO` & `buge-0.0.3/buge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buge
-Version: 0.0.2
+Version: 0.0.3
 Summary: buge is a command-line application that uses the OpenAI API to diagnose bugs when programming.
 Home-page: https://github.com/damonpickett/buge
 Author: Damon Pickett
 Author-email: Damon Pickett <damon.pickett@gmail.com>
 Project-URL: Homepage, https://github.com/damonpickett/buge
 Project-URL: Bug Tracker, https://github.com/damonpickett/buge/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `buge-0.0.2/pyproject.toml` & `buge-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "buge"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Damon Pickett", email="damon.pickett@gmail.com" },
 ]
 description = "buge is a command-line application that uses the OpenAI API to diagnose bugs when programming."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `buge-0.0.2/setup.cfg` & `buge-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = buge
-version = 0.0.2
+version = 0.0.3
 author = Damon Pickett
 author_email = damon.pickett@gmail.com
 description = buge is a command-line application that uses the OpenAI API to diagnose bugs when programming.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/damonpickett/buge
 classifiers =
```

