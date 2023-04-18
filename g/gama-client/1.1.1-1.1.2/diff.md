# Comparing `tmp/gama_client-1.1.1.tar.gz` & `tmp/gama_client-1.1.2.tar.gz`

## Comparing `gama_client-1.1.1.tar` & `gama_client-1.1.2.tar`

### file list

```diff
@@ -1,12 +1,9 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 gama_client-1.1.1/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gama_client-1.1.1/examples/__init__.py
--rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 gama_client-1.1.1/examples/sequential_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gama_client-1.1.1/gama_client/__init__.py
--rw-r--r--   0        0        0    16230 2020-02-02 00:00:00.000000 gama_client-1.1.1/gama_client/base_client.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 gama_client-1.1.1/gama_client/command_types.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 gama_client-1.1.1/gama_client/message_types.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 gama_client-1.1.1/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 gama_client-1.1.1/LICENSE
--rw-r--r--   0        0        0     7981 2020-02-02 00:00:00.000000 gama_client-1.1.1/README.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 gama_client-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 gama_client-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gama_client-1.1.2/gama_client/__init__.py
+-rw-r--r--   0        0        0    16421 2020-02-02 00:00:00.000000 gama_client-1.1.2/gama_client/base_client.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 gama_client-1.1.2/gama_client/command_types.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 gama_client-1.1.2/gama_client/message_types.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 gama_client-1.1.2/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 gama_client-1.1.2/LICENSE
+-rw-r--r--   0        0        0     8995 2020-02-02 00:00:00.000000 gama_client-1.1.2/README.md
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 gama_client-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0    10660 2020-02-02 00:00:00.000000 gama_client-1.1.2/PKG-INFO
```

### Comparing `gama_client-1.1.1/gama_client/base_client.py` & `gama_client-1.1.2/gama_client/base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
                 except Exception as js_ex:
                     print("Unable to unpack gama-server messages as a json. Error:", js_ex, "Message received:", mess)
             except Exception as sock_ex:
                 print("Error while waiting for a message from gama-server. Exiting", sock_ex)
                 sys.exit(-1)
 
     async def load(self, file_path: str, experiment_name: str, console: bool = None, status: bool = None,
-                   dialog: bool = None, parameters: List[Dict] = None, until: str = "", socket_id: str = "",
+                   dialog: bool = None, runtime: bool = None, parameters: List[Dict] = None, until: str = "", socket_id: str = "",
                    additional_data: Dict = None):
         """Sends a command to load the experiment **experiment_name** from the file **file_path** (on the server side).
 
         **Note**
             The parameters must follow this format: ::
 
                 {
@@ -98,14 +98,15 @@
 
         :param file_path: The path of the file containing the experiment to run
         :param experiment_name: The name of the experiment to run
         :param socket_id: The socket that will be linked to the experiment, if empty uses current connection
         :param console: True if you want gama-server to redirect the simulation's console outputs
         :param status: True if you want gama-server to redirect the simulation's status changes
         :param dialog: True if you want gama-server to redirect the simulation's dialogs
+        :param runtime: True if you want gama-server to redirect the simulation's runtime errors
         :param parameters: A list of dictionaries, each dictionary representing the initial value of an experiment parameter.
             They will be set at the initialization phase of the experiment.
         :param until: A string representing an ending condition to stop an experiment run by gama-server.
             It must be expressed in the gaml language.
         :param additional_data: A dictionary containing any additional data you want to send to gama server. Those will
             be sent back with the command's answer. (for example an id for the client's internal use)
 
@@ -122,14 +123,16 @@
             cmd["socket_id"] = socket_id
         if console is not None:
             cmd["console"] = console
         if status is not None:
             cmd["status"] = status
         if dialog is not None:
             cmd["dialog"] = dialog
+        if runtime is not None:
+            cmd["runtime"] = runtime
         if parameters:
             cmd["parameters"] = parameters
         if until and until != '':
             cmd["until"] = until
         if additional_data:
             cmd.update(additional_data)
```

### Comparing `gama_client-1.1.1/gama_client/message_types.py` & `gama_client-1.1.2/gama_client/message_types.py`

 * *Files identical despite different names*

### Comparing `gama_client-1.1.1/.gitignore` & `gama_client-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gama_client-1.1.1/LICENSE` & `gama_client-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gama_client-1.1.1/README.md` & `gama_client-1.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Gama client
- Gama-client is a python wrapper for interacting with the headless mode (called gama-server) of the multi-agent modeling platform [gama](https://gama-platform.org/). The latest release is compatible with gama 1.9.0.
+ Gama-client is a python wrapper for interacting with the headless mode (called gama-server) of the multi-agent modeling platform [gama](https://gama-platform.org/). The latest release is compatible with gama 1.9.1.
 This wrapper will take care of the connection with gama-server and of sending properly formatted requests to gama-server. It is made to fit the asynchronous nature of gama-server and thus makes it possible to handle multiple simulations at the same time, but the counterpart is that the users will still have to manage what to do with the received messages (command confirmation, simulation output, errors etc.) by themselves. We provide a working example that shows the architecture you can deploy if you still want to have a sequential execution.
 
 # Installation
 In your python environment, install the gama-client package with the command:
 
 ```
 pip install gama-client
@@ -142,7 +142,34 @@
 ```
 
 
 ## Example code
 A complete working example is given in the `examples` directory, you just have to change the values of the variables `MY_SERVER_URL`, `MY_SERVER_PORT`, `GAML_FILE_PATH_ON_SERVER`, `EXPERIMENT_NAME` and `MY_EXP_INIT_PARAMETERS` to the one corresponding to your own gama-server and experiment to try it.
  
  
+# To generate a new release (for contributors only)
+## Upload the new files to pypi
+For reference: this documentation is based on this [tutorial](https://packaging.python.org/en/latest/tutorials/packaging-projects/#generating-distribution-archives). Please check it out for more details about tools to install and/or context.
+
+* increment the version number in `pyproject.toml`
+* commit your changes to github
+* make sure you installed the required tools by running
+```
+python -m pip install --upgrade build
+```
+```
+python -m pip install --upgrade twine
+```
+* in the project's folder, to build the library, run
+```
+python -m build
+```
+* then, to upload the generated files, run
+```
+python -m twine upload --repository pypi dist/*
+```
+* on github, go to releases
+* click on create a new release
+* in tag, create a new tag with the new release number
+* add a description of the changes
+* in binaries, upload the two .whl files generated by the `build` command
+* click on `publish release`
```

### Comparing `gama_client-1.1.1/pyproject.toml` & `gama_client-1.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "gama_client"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Baptiste Lesquoy", email="baptistelesquoy@protonmail.com" },
 ]
-description = "A Gama client wrapper in python to interact with Gama server"
+description = "A python library to interact with Gama server"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "websockets~=10.3",
 ]
 [project.urls]
 "Homepage" = "https://github.com/gama-platform/Gama-client-python"
 "Bug Tracker" = "https://github.com/gama-platform/Gama-client-python/issues"
+[tool.hatch.build]
+include = [
+  "gama_client/*.py",
+]
+exclude = [
+]
```

### Comparing `gama_client-1.1.1/PKG-INFO` & `gama_client-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gama_client
-Version: 1.1.1
-Summary: A Gama client wrapper in python to interact with Gama server
+Version: 1.1.2
+Summary: A python library to interact with Gama server
 Project-URL: Homepage, https://github.com/gama-platform/Gama-client-python
 Project-URL: Bug Tracker, https://github.com/gama-platform/Gama-client-python/issues
 Author-email: Baptiste Lesquoy <baptistelesquoy@protonmail.com>
 License: MIT License
         
         Copyright (c) 2022 Baptiste Lesquoy
         
@@ -31,15 +31,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: websockets~=10.3
 Description-Content-Type: text/markdown
 
 # Gama client
- Gama-client is a python wrapper for interacting with the headless mode (called gama-server) of the multi-agent modeling platform [gama](https://gama-platform.org/). The latest release is compatible with gama 1.9.0.
+ Gama-client is a python wrapper for interacting with the headless mode (called gama-server) of the multi-agent modeling platform [gama](https://gama-platform.org/). The latest release is compatible with gama 1.9.1.
 This wrapper will take care of the connection with gama-server and of sending properly formatted requests to gama-server. It is made to fit the asynchronous nature of gama-server and thus makes it possible to handle multiple simulations at the same time, but the counterpart is that the users will still have to manage what to do with the received messages (command confirmation, simulation output, errors etc.) by themselves. We provide a working example that shows the architecture you can deploy if you still want to have a sequential execution.
 
 # Installation
 In your python environment, install the gama-client package with the command:
 
 ```
 pip install gama-client
@@ -178,7 +178,34 @@
 ```
 
 
 ## Example code
 A complete working example is given in the `examples` directory, you just have to change the values of the variables `MY_SERVER_URL`, `MY_SERVER_PORT`, `GAML_FILE_PATH_ON_SERVER`, `EXPERIMENT_NAME` and `MY_EXP_INIT_PARAMETERS` to the one corresponding to your own gama-server and experiment to try it.
  
  
+# To generate a new release (for contributors only)
+## Upload the new files to pypi
+For reference: this documentation is based on this [tutorial](https://packaging.python.org/en/latest/tutorials/packaging-projects/#generating-distribution-archives). Please check it out for more details about tools to install and/or context.
+
+* increment the version number in `pyproject.toml`
+* commit your changes to github
+* make sure you installed the required tools by running
+```
+python -m pip install --upgrade build
+```
+```
+python -m pip install --upgrade twine
+```
+* in the project's folder, to build the library, run
+```
+python -m build
+```
+* then, to upload the generated files, run
+```
+python -m twine upload --repository pypi dist/*
+```
+* on github, go to releases
+* click on create a new release
+* in tag, create a new tag with the new release number
+* add a description of the changes
+* in binaries, upload the two .whl files generated by the `build` command
+* click on `publish release`
```

