# Comparing `tmp/kscope-0.4.1.tar.gz` & `tmp/kscope-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kscope-0.4.1.tar", last modified: Wed Mar 22 00:05:51 2023, max compression
+gzip compressed data, was "kscope-0.5.0.tar", last modified: Tue Apr 18 20:33:18 2023, max compression
```

## Comparing `kscope-0.4.1.tar` & `kscope-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 jsiva    (11746) jsiva    (11828)        0 2023-03-22 00:05:51.872585 kscope-0.4.1/
--rw-rw-r--   0 jsiva    (11746) jsiva    (11828)     1073 2023-03-22 00:05:12.000000 kscope-0.4.1/LICENSE
--rw-rw-r--   0 jsiva    (11746) jsiva    (11828)     5231 2023-03-22 00:05:51.872585 kscope-0.4.1/PKG-INFO
--rw-rw-r--   0 jsiva    (11746) jsiva    (11828)     4282 2023-03-22 00:05:12.000000 kscope-0.4.1/README.md
-drwxrwxr-x   0 jsiva    (11746) jsiva    (11828)        0 2023-03-22 00:05:51.872585 kscope-0.4.1/kscope/
--rw-rw-r--   0 jsiva    (11746) jsiva    (11828)      181 2023-03-22 00:05:12.000000 kscope-0.4.1/kscope/__init__.py
--rw-rw-r--   0 jsiva    (11746) jsiva    (11828)      513 2023-03-22 00:05:12.000000 kscope-0.4.1/kscope/hooks.py
--rw-rw-r--   0 jsiva    (11746) jsiva    (11828)     8862 2023-03-22 00:05:12.000000 kscope-0.4.1/kscope/kaleidoscope_sdk.py
--rw-rw-r--   0 jsiva    (11746) jsiva    (11828)     1526 2023-03-22 00:05:12.000000 kscope-0.4.1/kscope/utils.py
-drwxrwxr-x   0 jsiva    (11746) jsiva    (11828)        0 2023-03-22 00:05:51.872585 kscope-0.4.1/kscope.egg-info/
--rw-rw-r--   0 jsiva    (11746) jsiva    (11828)     5231 2023-03-22 00:05:51.000000 kscope-0.4.1/kscope.egg-info/PKG-INFO
--rw-rw-r--   0 jsiva    (11746) jsiva    (11828)      253 2023-03-22 00:05:51.000000 kscope-0.4.1/kscope.egg-info/SOURCES.txt
--rw-rw-r--   0 jsiva    (11746) jsiva    (11828)        1 2023-03-22 00:05:51.000000 kscope-0.4.1/kscope.egg-info/dependency_links.txt
--rw-rw-r--   0 jsiva    (11746) jsiva    (11828)      134 2023-03-22 00:05:51.000000 kscope-0.4.1/kscope.egg-info/requires.txt
--rw-rw-r--   0 jsiva    (11746) jsiva    (11828)        7 2023-03-22 00:05:51.000000 kscope-0.4.1/kscope.egg-info/top_level.txt
--rw-rw-r--   0 jsiva    (11746) jsiva    (11828)       38 2023-03-22 00:05:51.872585 kscope-0.4.1/setup.cfg
--rw-rw-r--   0 jsiva    (11746) jsiva    (11828)     1427 2023-03-22 00:05:12.000000 kscope-0.4.1/setup.py
+drwxrwxr-x   0 coatsworth  (1000) coatsworth  (1000)        0 2023-04-18 20:33:18.631625 kscope-0.5.0/
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     1073 2023-04-18 20:33:06.000000 kscope-0.5.0/LICENSE
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     5225 2023-04-18 20:33:18.631625 kscope-0.5.0/PKG-INFO
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     4276 2023-04-18 20:33:06.000000 kscope-0.5.0/README.md
+drwxrwxr-x   0 coatsworth  (1000) coatsworth  (1000)        0 2023-04-18 20:33:18.631625 kscope-0.5.0/kscope/
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)      181 2023-04-18 20:33:06.000000 kscope-0.5.0/kscope/__init__.py
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)      513 2023-04-18 20:33:06.000000 kscope-0.5.0/kscope/hooks.py
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     8971 2023-04-18 20:33:06.000000 kscope-0.5.0/kscope/kaleidoscope_sdk.py
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     1526 2023-04-18 20:33:06.000000 kscope-0.5.0/kscope/utils.py
+drwxrwxr-x   0 coatsworth  (1000) coatsworth  (1000)        0 2023-04-18 20:33:18.631625 kscope-0.5.0/kscope.egg-info/
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     5225 2023-04-18 20:33:18.000000 kscope-0.5.0/kscope.egg-info/PKG-INFO
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)      253 2023-04-18 20:33:18.000000 kscope-0.5.0/kscope.egg-info/SOURCES.txt
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)        1 2023-04-18 20:33:18.000000 kscope-0.5.0/kscope.egg-info/dependency_links.txt
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)      134 2023-04-18 20:33:18.000000 kscope-0.5.0/kscope.egg-info/requires.txt
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)        7 2023-04-18 20:33:18.000000 kscope-0.5.0/kscope.egg-info/top_level.txt
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)       38 2023-04-18 20:33:18.631625 kscope-0.5.0/setup.cfg
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     1427 2023-04-18 20:33:06.000000 kscope-0.5.0/setup.py
```

### Comparing `kscope-0.4.1/LICENSE` & `kscope-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kscope-0.4.1/PKG-INFO` & `kscope-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kscope
-Version: 0.4.1
+Version: 0.5.0
 Summary: A user toolkit for analyzing and interfacing with Large Language Models (LLMs)
 Home-page: https://github.com/VectorInstitute/kaleidoscope-sdk
 Author: ['Vector AI Engineering']
 Author-email: ai_engineering@vectorinstitute.ai
 License: MIT
 Keywords: python nlp machine-learning deep-learning distributed-computing neural-networks tensor llm
 Classifier: Development Status :: 3 - Alpha
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![kaleiodsciope-logo](https://user-images.githubusercontent.com/72175053/226011498-dbdfa2dc-f09d-4fbf-a1db-8b6deccb3fec.png)
+![Kaleidoscope](https://user-images.githubusercontent.com/72175053/229659396-2a61cd69-eafa-4a96-8e1c-d93519a8f617.png)
 -----------------
 # Kaleidoscope-SDK
 ![PyPI](https://img.shields.io/pypi/v/kscope)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kscope)
 ![GitHub](https://img.shields.io/github/license/VectorInstitute/kaleidoscope-sdk)
 ![DOI](https://img.shields.io/badge/DOI-in--progress-blue)
 [![Documentation](https://img.shields.io/badge/api-reference-lightgrey.svg)](https://kaleidoscope-sdk.readthedocs.io/en/latest/)
```

### Comparing `kscope-0.4.1/README.md` & `kscope-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![kaleiodsciope-logo](https://user-images.githubusercontent.com/72175053/226011498-dbdfa2dc-f09d-4fbf-a1db-8b6deccb3fec.png)
+![Kaleidoscope](https://user-images.githubusercontent.com/72175053/229659396-2a61cd69-eafa-4a96-8e1c-d93519a8f617.png)
 -----------------
 # Kaleidoscope-SDK
 ![PyPI](https://img.shields.io/pypi/v/kscope)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kscope)
 ![GitHub](https://img.shields.io/github/license/VectorInstitute/kaleidoscope-sdk)
 ![DOI](https://img.shields.io/badge/DOI-in--progress-blue)
 [![Documentation](https://img.shields.io/badge/api-reference-lightgrey.svg)](https://kaleidoscope-sdk.readthedocs.io/en/latest/)
```

### Comparing `kscope-0.4.1/kscope/hooks.py` & `kscope-0.5.0/kscope/hooks.py`

 * *Files identical despite different names*

### Comparing `kscope-0.4.1/kscope/kaleidoscope_sdk.py` & `kscope-0.5.0/kscope/kaleidoscope_sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -223,15 +223,16 @@
     def is_active(self):
         """Checks if the model instance is active"""
         return self.state == "ACTIVE"
 
     def generate(self, prompts: Union[str, List[str]], generation_config: Dict = {}):
         """Generates text from the model instance
 
-        :param prompts: (str or List[str]) Single prompt or list of prompts to generate from
+        :param prompts: (str or List[str]) Single prompt or list of prompts to generate from. 
+        Supports upto 8 prompts in a single request.
         :param kwargs: (dict) Additional arguments to pass to the model
         """
         if isinstance(prompts, str):
             prompts = [prompts]
         generation_response = self._session.generate(
             self.id, prompts, generation_config
         )
@@ -242,15 +243,16 @@
     def get_activations(
         self,
         prompts: Union[str, List[str]],
         module_names: List[str],
         generation_config: Dict = {},
     ):
         """Gets activations from the model instance
-        :param prompts: (str or List[str]) Single prompt or list of prompts to generate from
+        :param prompts: (str or List[str]) Single prompt or list of prompts to generate from.
+        Supports upto 8 prompts in a single request.
         :param module_names: (List[str]) The layer to get activations from
         """
         if isinstance(prompts, str):
             prompts = [prompts]
         activations_response = self._session.get_activations(
             self.id, prompts, module_names, generation_config
         )
```

### Comparing `kscope-0.4.1/kscope/utils.py` & `kscope-0.5.0/kscope/utils.py`

 * *Files identical despite different names*

### Comparing `kscope-0.4.1/kscope.egg-info/PKG-INFO` & `kscope-0.5.0/kscope.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kscope
-Version: 0.4.1
+Version: 0.5.0
 Summary: A user toolkit for analyzing and interfacing with Large Language Models (LLMs)
 Home-page: https://github.com/VectorInstitute/kaleidoscope-sdk
 Author: ['Vector AI Engineering']
 Author-email: ai_engineering@vectorinstitute.ai
 License: MIT
 Keywords: python nlp machine-learning deep-learning distributed-computing neural-networks tensor llm
 Classifier: Development Status :: 3 - Alpha
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![kaleiodsciope-logo](https://user-images.githubusercontent.com/72175053/226011498-dbdfa2dc-f09d-4fbf-a1db-8b6deccb3fec.png)
+![Kaleidoscope](https://user-images.githubusercontent.com/72175053/229659396-2a61cd69-eafa-4a96-8e1c-d93519a8f617.png)
 -----------------
 # Kaleidoscope-SDK
 ![PyPI](https://img.shields.io/pypi/v/kscope)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kscope)
 ![GitHub](https://img.shields.io/github/license/VectorInstitute/kaleidoscope-sdk)
 ![DOI](https://img.shields.io/badge/DOI-in--progress-blue)
 [![Documentation](https://img.shields.io/badge/api-reference-lightgrey.svg)](https://kaleidoscope-sdk.readthedocs.io/en/latest/)
```

### Comparing `kscope-0.4.1/setup.py` & `kscope-0.5.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="kscope",
-    version="0.4.1",
+    version="0.5.0",
     description="A user toolkit for analyzing and interfacing with Large Language Models (LLMs)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="python nlp machine-learning deep-learning distributed-computing neural-networks tensor llm",
     requires_python=">=3.7",
     url="https://github.com/VectorInstitute/kaleidoscope-sdk",
     author=["Vector AI Engineering"],
```

