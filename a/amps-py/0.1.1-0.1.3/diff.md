# Comparing `tmp/amps-py-0.1.1.tar.gz` & `tmp/amps-py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amps-py-0.1.1.tar", last modified: Tue Aug  9 21:07:51 2022, max compression
+gzip compressed data, was "amps-py-0.1.3.tar", last modified: Tue Apr 18 03:12:22 2023, max compression
```

## Comparing `amps-py-0.1.1.tar` & `amps-py-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2022-08-09 21:07:51.652582 amps-py-0.1.1/
--rw-r--r--   0 abhayram   (501) staff       (20)     1074 2022-05-20 22:16:05.000000 amps-py-0.1.1/LICENSE
--rw-r--r--   0 abhayram   (501) staff       (20)      828 2022-08-09 21:07:51.652716 amps-py-0.1.1/PKG-INFO
--rw-r--r--   0 abhayram   (501) staff       (20)      314 2022-05-23 03:14:45.000000 amps-py-0.1.1/README.md
--rw-r--r--   0 abhayram   (501) staff       (20)       84 2022-05-20 22:16:05.000000 amps-py-0.1.1/pyproject.toml
--rw-r--r--   0 abhayram   (501) staff       (20)      638 2022-08-09 21:07:51.653266 amps-py-0.1.1/setup.cfg
-drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2022-08-09 21:07:51.648950 amps-py-0.1.1/src/
-drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2022-08-09 21:07:51.650672 amps-py-0.1.1/src/amps/
--rw-r--r--   0 abhayram   (501) staff       (20)    32806 2022-08-09 21:07:05.000000 amps-py-0.1.1/src/amps/__init__.py
-drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2022-08-09 21:07:51.652374 amps-py-0.1.1/src/amps_py.egg-info/
--rw-r--r--   0 abhayram   (501) staff       (20)      828 2022-08-09 21:07:51.000000 amps-py-0.1.1/src/amps_py.egg-info/PKG-INFO
--rw-r--r--   0 abhayram   (501) staff       (20)      203 2022-08-09 21:07:51.000000 amps-py-0.1.1/src/amps_py.egg-info/SOURCES.txt
--rw-r--r--   0 abhayram   (501) staff       (20)        1 2022-08-09 21:07:51.000000 amps-py-0.1.1/src/amps_py.egg-info/dependency_links.txt
--rw-r--r--   0 abhayram   (501) staff       (20)        5 2022-08-09 21:07:51.000000 amps-py-0.1.1/src/amps_py.egg-info/top_level.txt
+drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2023-04-18 03:12:22.435683 amps-py-0.1.3/
+-rw-r--r--   0 abhayram   (501) staff       (20)     1074 2023-04-13 22:49:51.000000 amps-py-0.1.3/LICENSE
+-rw-r--r--   0 abhayram   (501) staff       (20)      828 2023-04-18 03:12:22.435774 amps-py-0.1.3/PKG-INFO
+-rw-r--r--   0 abhayram   (501) staff       (20)      314 2023-04-13 22:49:51.000000 amps-py-0.1.3/README.md
+-rw-r--r--   0 abhayram   (501) staff       (20)       84 2023-04-13 22:49:51.000000 amps-py-0.1.3/pyproject.toml
+-rw-r--r--   0 abhayram   (501) staff       (20)      638 2023-04-18 03:12:22.436124 amps-py-0.1.3/setup.cfg
+drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2023-04-18 03:12:22.433386 amps-py-0.1.3/src/
+drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2023-04-18 03:12:22.434273 amps-py-0.1.3/src/amps/
+-rw-r--r--   0 abhayram   (501) staff       (20)    35433 2023-04-17 04:58:50.000000 amps-py-0.1.3/src/amps/__init__.py
+drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2023-04-18 03:12:22.435512 amps-py-0.1.3/src/amps_py.egg-info/
+-rw-r--r--   0 abhayram   (501) staff       (20)      828 2023-04-18 03:12:22.000000 amps-py-0.1.3/src/amps_py.egg-info/PKG-INFO
+-rw-r--r--   0 abhayram   (501) staff       (20)      203 2023-04-18 03:12:22.000000 amps-py-0.1.3/src/amps_py.egg-info/SOURCES.txt
+-rw-r--r--   0 abhayram   (501) staff       (20)        1 2023-04-18 03:12:22.000000 amps-py-0.1.3/src/amps_py.egg-info/dependency_links.txt
+-rw-r--r--   0 abhayram   (501) staff       (20)        5 2023-04-18 03:12:22.000000 amps-py-0.1.3/src/amps_py.egg-info/top_level.txt
```

### Comparing `amps-py-0.1.1/LICENSE` & `amps-py-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `amps-py-0.1.1/PKG-INFO` & `amps-py-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amps-py
-Version: 0.1.1
+Version: 0.1.3
 Summary: Package for Interfacing with AMPS from Agile Data Inc.
 Home-page: https://mftlabs.github.io/amps-py
 Author: Abhay Ram
 Author-email: abhayram@hub4edi.com
 Project-URL: Bug Tracker, https://github.com/mftlabs/amps-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `amps-py-0.1.1/setup.cfg` & `amps-py-0.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = amps-py
-version = 0.1.1
+version = 0.1.3
 author = Abhay Ram
 author_email = abhayram@hub4edi.com
 description = Package for Interfacing with AMPS from Agile Data Inc.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://mftlabs.github.io/amps-py
 project_urls =
```

### Comparing `amps-py-0.1.1/src/amps/__init__.py` & `amps-py-0.1.3/src/amps/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from erlport.erlang import cast, call
-from erlport.erlterms import Atom
+from erlport.erlterms import Atom, Map, List
 import traceback
 import os
 import json
 import uuid
 
 
 class Util:
@@ -12,14 +12,27 @@
 
     """
     def get_id():
         """Utility method that returns a unique ID in the format used by AMPS.
         """
         return uuid.UUID(str(uuid.uuid4())).hex
 
+    @staticmethod
+    def unravel_erlport_object(result):
+        if isinstance(result, List):
+            return [Util.unravel_erlport_object(x) for x in result]
+        elif isinstance(result, Map):
+            return {k.decode(): Util.unravel_erlport_object(v) for k, v in result.items()}
+        elif isinstance(result, Atom):
+            return result.decode()
+        elif isinstance(result, bytes):
+            return result.decode()
+        else:
+            return result
+
 
 class Logger:
     """The `Logger` class from AMPS is a utility class for logging events back to AMPS. This class should not be used directly, but rather instances of this class within Actions, Endpoints, and Services should be used.
 
     Usage:
     ```
     from amps import Action
@@ -122,14 +135,65 @@
                 # Perform Action Logic Here
                 self.logger.error("Something major went wrong.")
         ```
         """
         self.log("error", message)
 
 
+class DB:
+    def __init__(self, env):
+        self.env = env
+
+    def find(self, collection, clauses):
+        coll = bytes(collection, "utf-8")
+        collection = call(Atom(b'Elixir.AmpsUtil'), Atom(
+            b'index'), [bytes(self.env, "utf-8"), coll])
+        clauses = Map(clauses)
+        result = call(Atom(b'Elixir.Amps.PyService'),
+                      Atom(b'find'), [collection, clauses])
+        return Util.unravel_erlport_object(result)
+
+    def find_one(self, collection, clauses):
+        coll = bytes(collection, "utf-8")
+        collection = call(Atom(b'Elixir.AmpsUtil'), Atom(
+            b'index'), [bytes(self.env, "utf-8"), coll])
+        clauses = Map(clauses)
+        result = call(Atom(b'Elixir.Amps.PyService'),
+                      Atom(b'find_one'), [collection, clauses])
+        return Util.unravel_erlport_object(result)
+
+    def create(self, collection, body):
+        coll = bytes(collection, "utf-8")
+        collection = call(Atom(b'Elixir.AmpsUtil'), Atom(
+            b'index'), [bytes(self.env, "utf-8"), coll])
+        body = Map(body)
+        result = call(Atom(b'Elixir.Amps.PyService'),
+                      Atom(b'create'), [collection, body])
+        return Util.unravel_erlport_object(result)
+
+    def update(self, collection, body, id):
+        coll = bytes(collection, "utf-8")
+        id = bytes(id, "utf-8")
+        collection = call(Atom(b'Elixir.AmpsUtil'), Atom(
+            b'index'), [bytes(self.env, "utf-8"), coll])
+        body = Map(body)
+        result = call(Atom(b'Elixir.Amps.PyService'),
+                      Atom(b'update'), [collection, body, id])
+        return Util.unravel_erlport_object(result)
+
+    def delete(self, collection, id):
+        coll = bytes(collection, "utf-8")
+        id = bytes(id, "utf-8")
+        collection = call(Atom(b'Elixir.AmpsUtil'), Atom(
+            b'index'), [bytes(self.env, "utf-8"), coll])
+        result = call(Atom(b'Elixir.Amps.PyService'),
+                      Atom(b'delete'), [collection, id])
+        return Util.unravel_erlport_object(result)
+
+
 class Action:
     """The `Action` class from AMPS provides a base class for actions that must be extended in a custom action. Actions can be performed by overriding the `Action.action` callback exposed by the class.
 
     Attributes:
         msg (dict): The msg attribute contains a python of the dictionary and the message with all of its metadata. Message data can be accessed from the msg attribute, either using the "data" key for inline data, or the "fpath" key for a path to the file containing the data.
         parms (dict): The parms attribute contains all the parameters of the configured action including any extra parameters you may have specified under the "parms" key.
         sysparms (dict): The sysparms attribute contains all useful system configuration parameters for use in actions. Currently, sysparms only contains the AMPS temporary directory under the "tempdir" key.
@@ -156,14 +220,16 @@
 
     def __init__(self, msgdata):
         msgdata = json.loads(msgdata)
         self.msg = msgdata["msg"]
         self.parms = msgdata["parms"]
         self.sysparms = msgdata["sysparms"]
         self.extra = self.parms["parms"]
+        self.env = self.parms["env"]
+        self.db = DB(self.env)
         if self.parms["use_provider"]:
             self.provider = self.parms["provider"]
         if self.msg.get("sid"):
             self.logger = Logger(sid=self.msg["sid"])
         else:
             self.logger = Logger()
```

### Comparing `amps-py-0.1.1/src/amps_py.egg-info/PKG-INFO` & `amps-py-0.1.3/src/amps_py.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amps-py
-Version: 0.1.1
+Version: 0.1.3
 Summary: Package for Interfacing with AMPS from Agile Data Inc.
 Home-page: https://mftlabs.github.io/amps-py
 Author: Abhay Ram
 Author-email: abhayram@hub4edi.com
 Project-URL: Bug Tracker, https://github.com/mftlabs/amps-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

