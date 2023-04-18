# Comparing `tmp/strangeworks-rigetti-0.2.8.tar.gz` & `tmp/strangeworks-rigetti-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks-rigetti-0.2.8.tar", max compression
+gzip compressed data, was "strangeworks-rigetti-0.2.9.tar", max compression
```

## Comparing `strangeworks-rigetti-0.2.8.tar` & `strangeworks-rigetti-0.2.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      466 2022-05-13 22:38:36.891576 strangeworks-rigetti-0.2.8/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2022-05-13 22:38:36.891576 strangeworks-rigetti-0.2.8/LICENSE
--rw-r--r--   0        0        0      551 2022-05-13 22:38:48.555712 strangeworks-rigetti-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      273 2022-05-13 22:38:36.891576 strangeworks-rigetti-0.2.8/strangeworks/rigetti/__init__.py
--rw-r--r--   0        0        0     1985 2022-05-13 22:38:36.891576 strangeworks-rigetti-0.2.8/strangeworks/rigetti/compiler.py
--rw-r--r--   0        0        0     2487 2022-05-13 22:38:36.891576 strangeworks-rigetti-0.2.8/strangeworks/rigetti/program.py
--rw-r--r--   0        0        0     2497 2022-05-13 22:38:36.891576 strangeworks-rigetti-0.2.8/strangeworks/rigetti/qc.py
--rw-r--r--   0        0        0     1551 2022-05-13 22:38:36.891576 strangeworks-rigetti-0.2.8/strangeworks/rigetti/strange.py
--rw-r--r--   0        0        0     1162 2022-05-13 22:38:50.169631 strangeworks-rigetti-0.2.8/setup.py
--rw-r--r--   0        0        0     1014 2022-05-13 22:38:50.169992 strangeworks-rigetti-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      466 2022-05-16 14:44:19.107226 strangeworks-rigetti-0.2.9/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2022-05-16 14:44:19.107226 strangeworks-rigetti-0.2.9/LICENSE
+-rw-r--r--   0        0        0      551 2022-05-16 14:44:28.735440 strangeworks-rigetti-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      273 2022-05-16 14:44:19.107226 strangeworks-rigetti-0.2.9/strangeworks/rigetti/__init__.py
+-rw-r--r--   0        0        0     1985 2022-05-16 14:44:19.107226 strangeworks-rigetti-0.2.9/strangeworks/rigetti/compiler.py
+-rw-r--r--   0        0        0     2487 2022-05-16 14:44:19.107226 strangeworks-rigetti-0.2.9/strangeworks/rigetti/program.py
+-rw-r--r--   0        0        0     2739 2022-05-16 14:44:19.107226 strangeworks-rigetti-0.2.9/strangeworks/rigetti/qc.py
+-rw-r--r--   0        0        0     1551 2022-05-16 14:44:19.107226 strangeworks-rigetti-0.2.9/strangeworks/rigetti/strange.py
+-rw-r--r--   0        0        0     1162 2022-05-16 14:44:30.764455 strangeworks-rigetti-0.2.9/setup.py
+-rw-r--r--   0        0        0     1014 2022-05-16 14:44:30.764762 strangeworks-rigetti-0.2.9/PKG-INFO
```

### Comparing `strangeworks-rigetti-0.2.8/LICENSE` & `strangeworks-rigetti-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks-rigetti-0.2.8/pyproject.toml` & `strangeworks-rigetti-0.2.9/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strangeworks-rigetti"
-version = "0.2.8"
+version = "0.2.9"
 description = "Strangeworks Rigetti SDK extension"
 readme = "DESCRIPTION.md"
 authors = ["Strange Devs <hello@strangeworks.com>"]
 license = "Apache-2.0"
 packages = [
     {include = "strangeworks"},
 ]
```

### Comparing `strangeworks-rigetti-0.2.8/strangeworks/rigetti/compiler.py` & `strangeworks-rigetti-0.2.9/strangeworks/rigetti/compiler.py`

 * *Files identical despite different names*

### Comparing `strangeworks-rigetti-0.2.8/strangeworks/rigetti/program.py` & `strangeworks-rigetti-0.2.9/strangeworks/rigetti/program.py`

 * *Files identical despite different names*

### Comparing `strangeworks-rigetti-0.2.8/strangeworks/rigetti/qc.py` & `strangeworks-rigetti-0.2.9/strangeworks/rigetti/qc.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import strangeworks
 from strangeworks.rigetti.program import (
     CompiledProgram,
     encrypted_program_to_json,
     program_to_json,
 )
 from strangeworks.rigetti.compiler import StrangeworksCompiler
+import base64
+import pickle
 
 
 class QuantumComputer(QuantumComputer):
     def __init__(self, ogc: QuantumComputer, as_qvm: bool):
         self.as_qvm = "True" if as_qvm else "False"
         super().__init__(
             name=ogc.name,
@@ -62,7 +64,12 @@
             "version": pyquil.pyquil_version,
         }
 
     def __serialize_program(self, p: Program) -> dict:
         d = program_to_json(p)
         d["as_qvm"] = self.as_qvm
         return d
+
+    def __read_response(self, response: dict) -> QAMExecutionResult:
+        pickled_res = response["pickled_result"]
+        pickle_bytes = base64.b64decode(pickled_res)
+        return pickle.loads(pickle_bytes)
```

### Comparing `strangeworks-rigetti-0.2.8/strangeworks/rigetti/strange.py` & `strangeworks-rigetti-0.2.9/strangeworks/rigetti/strange.py`

 * *Files identical despite different names*

### Comparing `strangeworks-rigetti-0.2.8/setup.py` & `strangeworks-rigetti-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pyquil>=3.1,<3.2', 'strangeworks>=0.2.0,<0.3.0']
 
 setup_kwargs = {
     'name': 'strangeworks-rigetti',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'Strangeworks Rigetti SDK extension',
     'long_description': '| ⚠️    | This SDK is currently in pre-release alpha state and subject to change. To get more info or access to test features check out the [Strangeworks Backstage Pass Program](https://strangeworks.com/backstage). |\n|---------------|:------------------------|\n# Strangeworks Rigetti Extension\n\n Strangeworks Python SDK extension for Rigetti.\n\n\n \n For more information on using the SDK check out the [Strangeworks documentation](https://docs.strangeworks.com/).\n',
     'author': 'Strange Devs',
     'author_email': 'hello@strangeworks.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `strangeworks-rigetti-0.2.8/PKG-INFO` & `strangeworks-rigetti-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-rigetti
-Version: 0.2.8
+Version: 0.2.9
 Summary: Strangeworks Rigetti SDK extension
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

