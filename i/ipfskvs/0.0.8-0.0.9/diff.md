# Comparing `tmp/ipfskvs-0.0.8.tar.gz` & `tmp/ipfskvs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfskvs-0.0.8.tar", last modified: Mon Apr 17 19:17:36 2023, max compression
+gzip compressed data, was "ipfskvs-0.0.9.tar", last modified: Mon Apr 17 20:39:52 2023, max compression
```

## Comparing `ipfskvs-0.0.8.tar` & `ipfskvs-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 19:17:36.076885 ipfskvs-0.0.8/
--rw-r--r--   0 nate       (501) staff       (20)     1211 2023-04-12 01:55:42.000000 ipfskvs-0.0.8/LICENSE
--rw-r--r--   0 nate       (501) staff       (20)     3282 2023-04-17 19:17:36.076781 ipfskvs-0.0.8/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)     1392 2023-04-17 15:48:04.000000 ipfskvs-0.0.8/README.md
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 19:17:36.076650 ipfskvs-0.0.8/ipfskvs.egg-info/
--rw-r--r--   0 nate       (501) staff       (20)     3282 2023-04-17 19:17:36.000000 ipfskvs-0.0.8/ipfskvs.egg-info/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)      195 2023-04-17 19:17:36.000000 ipfskvs-0.0.8/ipfskvs.egg-info/SOURCES.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-17 19:17:36.000000 ipfskvs-0.0.8/ipfskvs.egg-info/dependency_links.txt
--rw-r--r--   0 nate       (501) staff       (20)       50 2023-04-17 19:17:36.000000 ipfskvs-0.0.8/ipfskvs.egg-info/requires.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-17 19:17:36.000000 ipfskvs-0.0.8/ipfskvs.egg-info/top_level.txt
--rw-r--r--   0 nate       (501) staff       (20)      638 2023-04-17 19:16:25.000000 ipfskvs-0.0.8/pyproject.toml
--rw-r--r--   0 nate       (501) staff       (20)       38 2023-04-17 19:17:36.076913 ipfskvs-0.0.8/setup.cfg
--rw-r--r--   0 nate       (501) staff       (20)      886 2023-04-17 19:16:21.000000 ipfskvs-0.0.8/setup.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 20:39:52.300344 ipfskvs-0.0.9/
+-rw-r--r--   0 nate       (501) staff       (20)     1211 2023-04-12 01:55:42.000000 ipfskvs-0.0.9/LICENSE
+-rw-r--r--   0 nate       (501) staff       (20)     3243 2023-04-17 20:39:52.300230 ipfskvs-0.0.9/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)     1353 2023-04-17 19:42:03.000000 ipfskvs-0.0.9/README.md
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 20:39:52.300101 ipfskvs-0.0.9/ipfskvs.egg-info/
+-rw-r--r--   0 nate       (501) staff       (20)     3243 2023-04-17 20:39:52.000000 ipfskvs-0.0.9/ipfskvs.egg-info/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)      195 2023-04-17 20:39:52.000000 ipfskvs-0.0.9/ipfskvs.egg-info/SOURCES.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-17 20:39:52.000000 ipfskvs-0.0.9/ipfskvs.egg-info/dependency_links.txt
+-rw-r--r--   0 nate       (501) staff       (20)       50 2023-04-17 20:39:52.000000 ipfskvs-0.0.9/ipfskvs.egg-info/requires.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-17 20:39:52.000000 ipfskvs-0.0.9/ipfskvs.egg-info/top_level.txt
+-rw-r--r--   0 nate       (501) staff       (20)      638 2023-04-17 20:34:56.000000 ipfskvs-0.0.9/pyproject.toml
+-rw-r--r--   0 nate       (501) staff       (20)       38 2023-04-17 20:39:52.300377 ipfskvs-0.0.9/setup.cfg
+-rw-r--r--   0 nate       (501) staff       (20)      886 2023-04-17 20:36:37.000000 ipfskvs-0.0.9/setup.py
```

### Comparing `ipfskvs-0.0.8/LICENSE` & `ipfskvs-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfskvs-0.0.8/PKG-INFO` & `ipfskvs-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfskvs
-Version: 0.0.8
+Version: 0.0.9
 Summary: IPFS python client
 Home-page: https://github.com/nanoswap/ipfskvs
 Author: Nathaniel Schultz
 Author-email: Nathaniel Schultz <nate@nanoswap.finance>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
@@ -35,45 +35,51 @@
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ipfs (interplanetary filesystem) kvs (key value store)
 
-Documentation: https://ipfs-kvs.readthedocs.io/
+## Installation
 
-## Build docs
+```
+pip install ipfskvs
+```
+
+## Documentation
+
+https://ipfs-kvs.readthedocs.io/
+
+### Build docs locally
 `mkdocs serve`
 
-## Run tests
+## Tests
 To only run tests: `pytest`  
 To run all checks: `nox`
 
-Note: before running tests:
-   - Generate the pb2.py files used for testing
-   - Make sure your local ipfs daemon is running
+### Before running tests:
 
-## Regenerate pb2.py files
+ - Regenerate pb2.py files:  
 ```
 cd protobuf;
 protoc --python_out=../proto --proto_path=protobuf protobuf/sample.proto
 ```
 
-## Run the ipfs daemon
+ - Ipfs setup: https://docs.ipfs.tech/install/  
+
+ - Run the ipfs daemon:
 ```
 ipfs daemon --api /ip4/0.0.0.0/tcp/5001
 ```
 Check the status of your node at:
   - http://localhost:5001/webui
   - https://webui.ipfs.io/#/status
 
-### ipfs setup
-https://docs.ipfs.tech/install/
 
-### ipfs troubleshooting
+## IPFS troubleshooting
 
 Set the log level, send the logs to a file, and search the file for relevant messages
 ```
 export IPFS_LOGGING=<debug|info|error>
 ipfs daemon --debug 2>&1 | tee ipfs.log
 cat ipfs.log | grep test_directory
 ```
```

### Comparing `ipfskvs-0.0.8/README.md` & `ipfskvs-0.0.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 # ipfs (interplanetary filesystem) kvs (key value store)
 
-Documentation: https://ipfs-kvs.readthedocs.io/
+## Installation
 
-## Build docs
+```
+pip install ipfskvs
+```
+
+## Documentation
+
+https://ipfs-kvs.readthedocs.io/
+
+### Build docs locally
 `mkdocs serve`
 
-## Run tests
+## Tests
 To only run tests: `pytest`  
 To run all checks: `nox`
 
-Note: before running tests:
-   - Generate the pb2.py files used for testing
-   - Make sure your local ipfs daemon is running
+### Before running tests:
 
-## Regenerate pb2.py files
+ - Regenerate pb2.py files:  
 ```
 cd protobuf;
 protoc --python_out=../proto --proto_path=protobuf protobuf/sample.proto
 ```
 
-## Run the ipfs daemon
+ - Ipfs setup: https://docs.ipfs.tech/install/  
+
+ - Run the ipfs daemon:
 ```
 ipfs daemon --api /ip4/0.0.0.0/tcp/5001
 ```
 Check the status of your node at:
   - http://localhost:5001/webui
   - https://webui.ipfs.io/#/status
 
-### ipfs setup
-https://docs.ipfs.tech/install/
 
-### ipfs troubleshooting
+## IPFS troubleshooting
 
 Set the log level, send the logs to a file, and search the file for relevant messages
 ```
 export IPFS_LOGGING=<debug|info|error>
 ipfs daemon --debug 2>&1 | tee ipfs.log
 cat ipfs.log | grep test_directory
 ```
```

### Comparing `ipfskvs-0.0.8/ipfskvs.egg-info/PKG-INFO` & `ipfskvs-0.0.9/ipfskvs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfskvs
-Version: 0.0.8
+Version: 0.0.9
 Summary: IPFS python client
 Home-page: https://github.com/nanoswap/ipfskvs
 Author: Nathaniel Schultz
 Author-email: Nathaniel Schultz <nate@nanoswap.finance>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
@@ -35,45 +35,51 @@
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ipfs (interplanetary filesystem) kvs (key value store)
 
-Documentation: https://ipfs-kvs.readthedocs.io/
+## Installation
 
-## Build docs
+```
+pip install ipfskvs
+```
+
+## Documentation
+
+https://ipfs-kvs.readthedocs.io/
+
+### Build docs locally
 `mkdocs serve`
 
-## Run tests
+## Tests
 To only run tests: `pytest`  
 To run all checks: `nox`
 
-Note: before running tests:
-   - Generate the pb2.py files used for testing
-   - Make sure your local ipfs daemon is running
+### Before running tests:
 
-## Regenerate pb2.py files
+ - Regenerate pb2.py files:  
 ```
 cd protobuf;
 protoc --python_out=../proto --proto_path=protobuf protobuf/sample.proto
 ```
 
-## Run the ipfs daemon
+ - Ipfs setup: https://docs.ipfs.tech/install/  
+
+ - Run the ipfs daemon:
 ```
 ipfs daemon --api /ip4/0.0.0.0/tcp/5001
 ```
 Check the status of your node at:
   - http://localhost:5001/webui
   - https://webui.ipfs.io/#/status
 
-### ipfs setup
-https://docs.ipfs.tech/install/
 
-### ipfs troubleshooting
+## IPFS troubleshooting
 
 Set the log level, send the logs to a file, and search the file for relevant messages
 ```
 export IPFS_LOGGING=<debug|info|error>
 ipfs daemon --debug 2>&1 | tee ipfs.log
 cat ipfs.log | grep test_directory
 ```
```

### Comparing `ipfskvs-0.0.8/pyproject.toml` & `ipfskvs-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 source = ["ipfskvs", "*/site-packages"]
 
 [tool.coverage.report]
 show_missing = true
 
 [project]
 name = "ipfskvs"
-version = "0.0.8"
+version = "0.0.9"
 description = "IPFS python client"
 urls = {'Bug Tracker' = 'https://github.com/nanoswap/ipfskvs/issues'}
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: The Unlicense (Unlicense)'
 ]
 authors = [{'name' = 'Nathaniel Schultz', 'email' = 'nate@nanoswap.finance'}]
```

### Comparing `ipfskvs-0.0.8/setup.py` & `ipfskvs-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     """Convert README.md to a string."""
     with open(filename, "r", encoding="utf-8") as f:
         return f.read()
 
 
 setup(
     name="ipfskvs",
-    version="0.0.8",
+    version="0.0.9",
     author="Nathaniel Schultz",
     author_email="nate@nanoswap.finance",
     description="IPFS Key Value Store",
     long_description=load_long_description("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/nanoswap/ipfskvs",
     project_urls={
```

