# Comparing `tmp/pyllms-0.1.5.tar.gz` & `tmp/pyllms-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllms-0.1.5.tar", last modified: Tue Apr 18 04:18:14 2023, max compression
+gzip compressed data, was "pyllms-0.1.7.tar", last modified: Tue Apr 18 08:36:36 2023, max compression
```

## Comparing `pyllms-0.1.5.tar` & `pyllms-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-18 04:18:14.371912 pyllms-0.1.5/
--rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.1.5/LICENSE
--rw-r--r--   0 prelovac   (502) staff       (20)    14437 2023-04-18 04:18:14.371638 pyllms-0.1.5/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)    13196 2023-04-18 04:17:49.000000 pyllms-0.1.5/README.md
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-18 04:18:14.368809 pyllms-0.1.5/llms/
--rw-r--r--   0 prelovac   (502) staff       (20)      295 2023-04-13 02:24:28.000000 pyllms-0.1.5/llms/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)    17070 2023-04-18 01:40:10.000000 pyllms-0.1.5/llms/llms.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-18 04:18:14.370067 pyllms-0.1.5/llms/providers/
--rw-r--r--   0 prelovac   (502) staff       (20)      107 2023-04-09 20:11:29.000000 pyllms-0.1.5/llms/providers/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2333 2023-04-13 21:39:49.000000 pyllms-0.1.5/llms/providers/ai21.py
--rw-r--r--   0 prelovac   (502) staff       (20)     4087 2023-04-17 15:37:12.000000 pyllms-0.1.5/llms/providers/anthropic.py
--rw-r--r--   0 prelovac   (502) staff       (20)     3569 2023-04-13 21:35:11.000000 pyllms-0.1.5/llms/providers/openai.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-18 04:18:14.371301 pyllms-0.1.5/pyllms.egg-info/
--rw-r--r--   0 prelovac   (502) staff       (20)    14437 2023-04-18 04:18:14.000000 pyllms-0.1.5/pyllms.egg-info/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)      308 2023-04-18 04:18:14.000000 pyllms-0.1.5/pyllms.egg-info/SOURCES.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-18 04:18:14.000000 pyllms-0.1.5/pyllms.egg-info/dependency_links.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       60 2023-04-18 04:18:14.000000 pyllms-0.1.5/pyllms.egg-info/requires.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-04-18 04:18:14.000000 pyllms-0.1.5/pyllms.egg-info/top_level.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-18 04:18:14.371986 pyllms-0.1.5/setup.cfg
--rw-r--r--   0 prelovac   (502) staff       (20)     1760 2023-04-18 04:18:04.000000 pyllms-0.1.5/setup.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-18 08:36:36.512801 pyllms-0.1.7/
+-rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.1.7/LICENSE
+-rw-r--r--   0 prelovac   (502) staff       (20)    14594 2023-04-18 08:36:36.512506 pyllms-0.1.7/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)    13353 2023-04-18 08:36:22.000000 pyllms-0.1.7/README.md
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-18 08:36:36.509925 pyllms-0.1.7/llms/
+-rw-r--r--   0 prelovac   (502) staff       (20)      295 2023-04-13 02:24:28.000000 pyllms-0.1.7/llms/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)    17345 2023-04-18 08:26:54.000000 pyllms-0.1.7/llms/llms.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-18 08:36:36.511015 pyllms-0.1.7/llms/providers/
+-rw-r--r--   0 prelovac   (502) staff       (20)      107 2023-04-09 20:11:29.000000 pyllms-0.1.7/llms/providers/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2333 2023-04-13 21:39:49.000000 pyllms-0.1.7/llms/providers/ai21.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     4237 2023-04-18 08:34:19.000000 pyllms-0.1.7/llms/providers/anthropic.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     3719 2023-04-18 08:32:10.000000 pyllms-0.1.7/llms/providers/openai.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-18 08:36:36.512169 pyllms-0.1.7/pyllms.egg-info/
+-rw-r--r--   0 prelovac   (502) staff       (20)    14594 2023-04-18 08:36:36.000000 pyllms-0.1.7/pyllms.egg-info/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)      308 2023-04-18 08:36:36.000000 pyllms-0.1.7/pyllms.egg-info/SOURCES.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-18 08:36:36.000000 pyllms-0.1.7/pyllms.egg-info/dependency_links.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       69 2023-04-18 08:36:36.000000 pyllms-0.1.7/pyllms.egg-info/requires.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-04-18 08:36:36.000000 pyllms-0.1.7/pyllms.egg-info/top_level.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-18 08:36:36.512888 pyllms-0.1.7/setup.cfg
+-rw-r--r--   0 prelovac   (502) staff       (20)     1780 2023-04-18 08:35:05.000000 pyllms-0.1.7/setup.py
```

### Comparing `pyllms-0.1.5/LICENSE` & `pyllms-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllms-0.1.5/PKG-INFO` & `pyllms-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllms
-Version: 0.1.5
+Version: 0.1.7
 Summary: Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21), with a built-in model performance benchmark.
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
 Project-URL: Documentation, https://github.com/kagisearch/pyllms
 Project-URL: Source Code, https://github.com/kagisearch/pyllms
 Project-URL: Issue Tracker, https://github.com/kagisearch/pyllms/issues
 Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21
@@ -140,15 +140,23 @@
 
 Tip: if you are testing this in python3 CLI, run it with -u parameter to disable buffering:
 
 ```
 python3 -u
 ```
 
-## Benchmarks
+## Other methods
+
+You can count tokens using the model's tokenizer:
+
+```
+count=model.count_tokens('the quick brown fox jumped over the lazy dog')
+```
+
+## Model Benchmarks
 
 Models are appearing like mushrooms after rain and everyone is interested in three things:
 
 1) Quality
 2) Speed
 3) Cost
```

### Comparing `pyllms-0.1.5/README.md` & `pyllms-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,23 @@
 
 Tip: if you are testing this in python3 CLI, run it with -u parameter to disable buffering:
 
 ```
 python3 -u
 ```
 
-## Benchmarks
+## Other methods
+
+You can count tokens using the model's tokenizer:
+
+```
+count=model.count_tokens('the quick brown fox jumped over the lazy dog')
+```
+
+## Model Benchmarks
 
 Models are appearing like mushrooms after rain and everyone is interested in three things:
 
 1) Quality
 2) Speed
 3) Cost
```

### Comparing `pyllms-0.1.5/llms/llms.py` & `pyllms-0.1.7/llms/llms.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,24 @@
                 model_info_list.append(model_info)
 
         sorted_list = sorted(
             model_info_list, key=lambda x: x["cost"]["prompt"] + x["cost"]["completion"]
         )
         return sorted_list
 
+    def count_tokens(self, content):
+
+        results = []
+        for provider in self._providers:
+            results.append(provider.count_tokens(content))
+        if len(self._providers)>1 :
+            return results
+        else:
+            return results[0]
+        
     def complete(self, prompt, history=None, system_message=None, **kwargs):
         def _generate(provider):
            
             response = provider.complete(prompt, history, **kwargs)
     
             formatted_cost = format(response["meta"]["cost"], '.5f')
             formatted_latency = round(response["meta"]["latency"], 2)
```

### Comparing `pyllms-0.1.5/llms/providers/ai21.py` & `pyllms-0.1.7/llms/providers/ai21.py`

 * *Files identical despite different names*

### Comparing `pyllms-0.1.5/llms/providers/anthropic.py` & `pyllms-0.1.7/llms/providers/anthropic.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,19 @@
         if model is None:
             model = "claude-instant-v1"
         self.model = model
 
     def __str__(self):
         return f"{self.__class__.__name__} ({self.model})"
 
+    def count_tokens(self, content:str):
+        raise ValueError(
+                "Count tokens is currently not supported with AI21"
+            )
+
     def complete(self,
                  prompt: str,
                  history: Optional[List[tuple]] = None,
                  temperature: float = 0,
                  max_tokens: int = 300,
                  **kwargs
                  ):
```

### Comparing `pyllms-0.1.5/llms/providers/openai.py` & `pyllms-0.1.7/llms/providers/openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import itertools
 import openai
+import tiktoken
 import time
 from typing import List, Optional
 
 
 class OpenAIProvider:
     # cost is per million tokens
     MODEL_INFO = {
@@ -16,14 +17,18 @@
         if model is None:
             model = "gpt-3.5-turbo"
         self.model = model
 
     def __str__(self):
         return f"{self.__class__.__name__} ({self.model})"
 
+    def count_tokens(self, content:str):
+        enc=tiktoken.encoding_for_model(self.model)
+        return len(enc.encode(content))
+
     def complete(self,
                  prompt: str,
                  history: Optional[List[tuple]] = None,
                  system_message: str = None,
                  temperature: float = 0,
                  **kwargs):
         start_time = time.time()
```

### Comparing `pyllms-0.1.5/pyllms.egg-info/PKG-INFO` & `pyllms-0.1.7/pyllms.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllms
-Version: 0.1.5
+Version: 0.1.7
 Summary: Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21), with a built-in model performance benchmark.
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
 Project-URL: Documentation, https://github.com/kagisearch/pyllms
 Project-URL: Source Code, https://github.com/kagisearch/pyllms
 Project-URL: Issue Tracker, https://github.com/kagisearch/pyllms/issues
 Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21
@@ -140,15 +140,23 @@
 
 Tip: if you are testing this in python3 CLI, run it with -u parameter to disable buffering:
 
 ```
 python3 -u
 ```
 
-## Benchmarks
+## Other methods
+
+You can count tokens using the model's tokenizer:
+
+```
+count=model.count_tokens('the quick brown fox jumped over the lazy dog')
+```
+
+## Model Benchmarks
 
 Models are appearing like mushrooms after rain and everyone is interested in three things:
 
 1) Quality
 2) Speed
 3) Cost
```

### Comparing `pyllms-0.1.5/setup.py` & `pyllms-0.1.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 _project_homepage = "https://github.com/kagisearch/pyllms"
 
 setup(
     name="pyllms",
-    version="0.1.5",
+    version="0.1.7",
     description="Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21), with a built-in model performance benchmark.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Vladimir Prelovac",
     author_email="vlad@kagi.com",
     packages=find_packages(),
     install_requires=[
         "openai",
+        "tiktoken",
         "anthropic",
         "ai21",
         "huggingface_hub",
         "markdown2",
         "prettytable",
     ],
     classifiers=[
```

