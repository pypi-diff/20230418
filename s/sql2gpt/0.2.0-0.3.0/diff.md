# Comparing `tmp/sql2gpt-0.2.0.tar.gz` & `tmp/sql2gpt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql2gpt-0.2.0.tar", last modified: Mon Apr 17 23:32:20 2023, max compression
+gzip compressed data, was "sql2gpt-0.3.0.tar", last modified: Mon Apr 17 23:35:40 2023, max compression
```

## Comparing `sql2gpt-0.2.0.tar` & `sql2gpt-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 chandler   (501) staff       (20)        0 2023-04-17 23:32:20.649179 sql2gpt-0.2.0/
--rw-r--r--   0 chandler   (501) staff       (20)       41 2023-04-17 21:09:51.000000 sql2gpt-0.2.0/.gitignore
--rw-r--r--   0 chandler   (501) staff       (20)       70 2023-04-17 20:53:03.000000 sql2gpt-0.2.0/.gptignore
-drwxr-xr-x   0 chandler   (501) staff       (20)        0 2023-04-17 23:32:20.645461 sql2gpt-0.2.0/.vscode/
--rw-r--r--   0 chandler   (501) staff       (20)       26 2023-04-17 18:18:45.000000 sql2gpt-0.2.0/.vscode/settings.json
--rw-r--r--   0 chandler   (501) staff       (20)     1114 2023-04-17 18:45:16.000000 sql2gpt-0.2.0/LICENSE
--rw-r--r--   0 chandler   (501) staff       (20)     2900 2023-04-17 23:32:20.649009 sql2gpt-0.2.0/PKG-INFO
--rw-r--r--   0 chandler   (501) staff       (20)      372 2023-04-17 21:12:13.000000 sql2gpt-0.2.0/Pipfile
--rw-r--r--   0 chandler   (501) staff       (20)    29622 2023-04-17 21:12:22.000000 sql2gpt-0.2.0/Pipfile.lock
--rw-r--r--   0 chandler   (501) staff       (20)     2334 2023-04-17 20:51:02.000000 sql2gpt-0.2.0/README.md
--rw-r--r--   0 chandler   (501) staff       (20)     1046 2023-04-17 18:28:17.000000 sql2gpt-0.2.0/config.py
--rw-r--r--   0 chandler   (501) staff       (20)      796 2023-04-17 23:31:34.000000 sql2gpt-0.2.0/pyproject.toml
--rw-r--r--   0 chandler   (501) staff       (20)       38 2023-04-17 23:32:20.649223 sql2gpt-0.2.0/setup.cfg
-drwxr-xr-x   0 chandler   (501) staff       (20)        0 2023-04-17 23:32:20.646402 sql2gpt-0.2.0/sql2gpt.egg-info/
--rw-r--r--   0 chandler   (501) staff       (20)     2900 2023-04-17 23:32:20.000000 sql2gpt-0.2.0/sql2gpt.egg-info/PKG-INFO
--rw-r--r--   0 chandler   (501) staff       (20)      345 2023-04-17 23:32:20.000000 sql2gpt-0.2.0/sql2gpt.egg-info/SOURCES.txt
--rw-r--r--   0 chandler   (501) staff       (20)        1 2023-04-17 23:32:20.000000 sql2gpt-0.2.0/sql2gpt.egg-info/dependency_links.txt
--rw-r--r--   0 chandler   (501) staff       (20)       41 2023-04-17 23:32:20.000000 sql2gpt-0.2.0/sql2gpt.egg-info/entry_points.txt
--rw-r--r--   0 chandler   (501) staff       (20)       44 2023-04-17 23:32:20.000000 sql2gpt-0.2.0/sql2gpt.egg-info/requires.txt
--rw-r--r--   0 chandler   (501) staff       (20)        6 2023-04-17 23:32:20.000000 sql2gpt-0.2.0/sql2gpt.egg-info/top_level.txt
--rw-r--r--   0 chandler   (501) staff       (20)     2175 2023-04-17 23:31:07.000000 sql2gpt-0.2.0/sql2gpt.py
-drwxr-xr-x   0 chandler   (501) staff       (20)        0 2023-04-17 23:32:20.647782 sql2gpt-0.2.0/tapes/
--rw-r--r--   0 chandler   (501) staff       (20)   475895 2023-04-17 20:49:47.000000 sql2gpt-0.2.0/tapes/demo.gif
--rw-r--r--   0 chandler   (501) staff       (20)      322 2023-04-17 20:46:44.000000 sql2gpt-0.2.0/tapes/demo.tape
--rw-r--r--   0 chandler   (501) staff       (20)      454 2023-04-17 18:24:03.000000 sql2gpt-0.2.0/util.py
+drwxr-xr-x   0 chandler   (501) staff       (20)        0 2023-04-17 23:35:40.695152 sql2gpt-0.3.0/
+-rw-r--r--   0 chandler   (501) staff       (20)       41 2023-04-17 21:09:51.000000 sql2gpt-0.3.0/.gitignore
+-rw-r--r--   0 chandler   (501) staff       (20)       70 2023-04-17 20:53:03.000000 sql2gpt-0.3.0/.gptignore
+drwxr-xr-x   0 chandler   (501) staff       (20)        0 2023-04-17 23:35:40.692460 sql2gpt-0.3.0/.vscode/
+-rw-r--r--   0 chandler   (501) staff       (20)       26 2023-04-17 18:18:45.000000 sql2gpt-0.3.0/.vscode/settings.json
+-rw-r--r--   0 chandler   (501) staff       (20)     1114 2023-04-17 18:45:16.000000 sql2gpt-0.3.0/LICENSE
+-rw-r--r--   0 chandler   (501) staff       (20)     2900 2023-04-17 23:35:40.695004 sql2gpt-0.3.0/PKG-INFO
+-rw-r--r--   0 chandler   (501) staff       (20)      372 2023-04-17 21:12:13.000000 sql2gpt-0.3.0/Pipfile
+-rw-r--r--   0 chandler   (501) staff       (20)    29622 2023-04-17 21:12:22.000000 sql2gpt-0.3.0/Pipfile.lock
+-rw-r--r--   0 chandler   (501) staff       (20)     2334 2023-04-17 20:51:02.000000 sql2gpt-0.3.0/README.md
+-rw-r--r--   0 chandler   (501) staff       (20)     1046 2023-04-17 18:28:17.000000 sql2gpt-0.3.0/config.py
+-rw-r--r--   0 chandler   (501) staff       (20)      796 2023-04-17 23:35:28.000000 sql2gpt-0.3.0/pyproject.toml
+-rw-r--r--   0 chandler   (501) staff       (20)       38 2023-04-17 23:35:40.695199 sql2gpt-0.3.0/setup.cfg
+drwxr-xr-x   0 chandler   (501) staff       (20)        0 2023-04-17 23:35:40.693343 sql2gpt-0.3.0/sql2gpt.egg-info/
+-rw-r--r--   0 chandler   (501) staff       (20)     2900 2023-04-17 23:35:40.000000 sql2gpt-0.3.0/sql2gpt.egg-info/PKG-INFO
+-rw-r--r--   0 chandler   (501) staff       (20)      345 2023-04-17 23:35:40.000000 sql2gpt-0.3.0/sql2gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 chandler   (501) staff       (20)        1 2023-04-17 23:35:40.000000 sql2gpt-0.3.0/sql2gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 chandler   (501) staff       (20)       41 2023-04-17 23:35:40.000000 sql2gpt-0.3.0/sql2gpt.egg-info/entry_points.txt
+-rw-r--r--   0 chandler   (501) staff       (20)       44 2023-04-17 23:35:40.000000 sql2gpt-0.3.0/sql2gpt.egg-info/requires.txt
+-rw-r--r--   0 chandler   (501) staff       (20)        6 2023-04-17 23:35:40.000000 sql2gpt-0.3.0/sql2gpt.egg-info/top_level.txt
+-rw-r--r--   0 chandler   (501) staff       (20)     2175 2023-04-17 23:31:07.000000 sql2gpt-0.3.0/sql2gpt.py
+drwxr-xr-x   0 chandler   (501) staff       (20)        0 2023-04-17 23:35:40.694682 sql2gpt-0.3.0/tapes/
+-rw-r--r--   0 chandler   (501) staff       (20)   475895 2023-04-17 20:49:47.000000 sql2gpt-0.3.0/tapes/demo.gif
+-rw-r--r--   0 chandler   (501) staff       (20)      322 2023-04-17 20:46:44.000000 sql2gpt-0.3.0/tapes/demo.tape
+-rw-r--r--   0 chandler   (501) staff       (20)      454 2023-04-17 18:24:03.000000 sql2gpt-0.3.0/util.py
```

### Comparing `sql2gpt-0.2.0/LICENSE` & `sql2gpt-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sql2gpt-0.2.0/PKG-INFO` & `sql2gpt-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: sql2gpt
-Version: 0.2.0
+Version: 0.3.0
 Summary: A tool to extract SQL database schema and generate ChatGPT prompts
 Author-email: Your Name <your.email@example.com>
 License: MIT
 Project-URL: Source, https://github.com/chand1012/sql2gpt
 Keywords: sql,chatgpt,database,schema
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SQL2GPT
 
 SQL2GPT is a Python-based tool that extracts the schema of a SQL database and generates a prompt for ChatGPT, a large language model by OpenAI. The goal of this project is to enable users to interact with ChatGPT to generate code or ask questions related to the given database schema.
```

### Comparing `sql2gpt-0.2.0/Pipfile.lock` & `sql2gpt-0.3.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `sql2gpt-0.2.0/README.md` & `sql2gpt-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sql2gpt-0.2.0/config.py` & `sql2gpt-0.3.0/config.py`

 * *Files identical despite different names*

### Comparing `sql2gpt-0.2.0/pyproject.toml` & `sql2gpt-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 requires-python = ">=3.11"
 keywords = ["sql", "chatgpt", "database", "schema"]
 license = { text = "MIT" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.10",
 ]
 dependencies = ["sqlalchemy", "psycopg2-binary", "mysqlclient", "fire"]
-version = "0.2.0"
+version = "0.3.0"
 
 [project.urls]
 Source = "https://github.com/chand1012/sql2gpt"
 
 [project.scripts]
 sql2gpt = "sql2gpt:main"
```

### Comparing `sql2gpt-0.2.0/sql2gpt.egg-info/PKG-INFO` & `sql2gpt-0.3.0/sql2gpt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: sql2gpt
-Version: 0.2.0
+Version: 0.3.0
 Summary: A tool to extract SQL database schema and generate ChatGPT prompts
 Author-email: Your Name <your.email@example.com>
 License: MIT
 Project-URL: Source, https://github.com/chand1012/sql2gpt
 Keywords: sql,chatgpt,database,schema
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SQL2GPT
 
 SQL2GPT is a Python-based tool that extracts the schema of a SQL database and generates a prompt for ChatGPT, a large language model by OpenAI. The goal of this project is to enable users to interact with ChatGPT to generate code or ask questions related to the given database schema.
```

### Comparing `sql2gpt-0.2.0/sql2gpt.py` & `sql2gpt-0.3.0/sql2gpt.py`

 * *Files identical despite different names*

### Comparing `sql2gpt-0.2.0/tapes/demo.gif` & `sql2gpt-0.3.0/tapes/demo.gif`

 * *Files identical despite different names*

