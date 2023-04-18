# Comparing `tmp/one-api-tool-0.1.3.tar.gz` & `tmp/one-api-tool-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.1.3.tar", last modified: Mon Apr 17 13:07:47 2023, max compression
+gzip compressed data, was "one-api-tool-0.1.4.tar", last modified: Tue Apr 18 03:35:55 2023, max compression
```

## Comparing `one-api-tool-0.1.3.tar` & `one-api-tool-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-17 13:07:47.831086 one-api-tool-0.1.3/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.1.3/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     2233 2023-04-17 13:07:47.830935 one-api-tool-0.1.3/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     1677 2023-04-17 13:05:41.000000 one-api-tool-0.1.3/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-17 13:07:47.830332 one-api-tool-0.1.3/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     2233 2023-04-17 13:07:47.000000 one-api-tool-0.1.3/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      242 2023-04-17 13:07:47.000000 one-api-tool-0.1.3/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-17 13:07:47.000000 one-api-tool-0.1.3/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       60 2023-04-17 13:07:47.000000 one-api-tool-0.1.3/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-04-17 13:07:47.000000 one-api-tool-0.1.3/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-17 13:07:47.830732 one-api-tool-0.1.3/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       47 2023-04-17 12:21:51.000000 one-api-tool-0.1.3/oneapi/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     9312 2023-04-17 13:06:43.000000 one-api-tool-0.1.3/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-17 13:07:47.831130 one-api-tool-0.1.3/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      908 2023-04-17 13:07:46.000000 one-api-tool-0.1.3/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-18 03:35:55.044484 one-api-tool-0.1.4/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.1.4/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2233 2023-04-18 03:35:55.044333 one-api-tool-0.1.4/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1677 2023-04-17 13:05:41.000000 one-api-tool-0.1.4/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-18 03:35:55.043735 one-api-tool-0.1.4/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2233 2023-04-18 03:35:55.000000 one-api-tool-0.1.4/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      242 2023-04-18 03:35:55.000000 one-api-tool-0.1.4/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-18 03:35:55.000000 one-api-tool-0.1.4/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       60 2023-04-18 03:35:55.000000 one-api-tool-0.1.4/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-04-18 03:35:55.000000 one-api-tool-0.1.4/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-18 03:35:55.044143 one-api-tool-0.1.4/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       47 2023-04-17 12:21:51.000000 one-api-tool-0.1.4/oneapi/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     9385 2023-04-18 03:35:48.000000 one-api-tool-0.1.4/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-18 03:35:55.044534 one-api-tool-0.1.4/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      908 2023-04-18 03:29:23.000000 one-api-tool-0.1.4/setup.py
```

### Comparing `one-api-tool-0.1.3/LICENSE` & `one-api-tool-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.1.3/PKG-INFO` & `one-api-tool-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.1.3
+Version: 0.1.4
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.1.3/README.md` & `one-api-tool-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.1.3/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.1.4/one_api_tool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.1.3
+Version: 0.1.4
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.1.3/oneapi/one_api.py` & `one-api-tool-0.1.4/oneapi/one_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # -*- coding: utf-8 -*-
 import json
-from typing import List
-from typing import Optional, Sequence
+from typing import Optional, Sequence, List
 import openai
 import anthropic
 from pydantic import BaseModel
 from abc import ABC, ABCMeta, abstractmethod
 
 
 CLAUDE_TEMPLATE = "\n\nHuman: {prompt}\n\nAssistant: "
@@ -32,17 +31,17 @@
     method_chat = "/v1/complete"
     method_commpletions = ""
 
 class AzureMethod(AbstrctMethod):
     api_key: str
     api_base: str # Your Azure OpenAI resource's endpoint value.
     api_type: str = "azure"
-    api_version = "2023-03-15-preview"
-    deployment_name = "gpt-35-turbo" # The deployment name you chose when you deployed the ChatGPT or GPT-4 model
-    method_chat = f"/openai/deployments/{deployment_name}/chat/completions?api-version={api_version}" # used for http requests
+    api_version = "2023-03-15-preview" # Official API version, usually there is no need to modify this field.
+    deployment_name = "gpt-35-turbo" # The deployment name you chose when you deployed the ChatGPT or GPT-4 model, used for raw http requests
+    method_chat = f"/openai/deployments/{deployment_name}/chat/completions?api-version={api_version}" # used for raw http requests
     method_list_models :str = "" 
     method_model_info :str = ""
     method_commpletions :str = ""
 
 class OpenAIMethod(AbstrctMethod):
     api_key: str
     api_base: str = "https://api.openai.com/v1"
@@ -106,15 +105,15 @@
             openai.api_version = self.method.api_version
         else:
             openai.api_key = self.method.api_key
             openai.api_base = self.method.api_base
 
     def simple_chat(self, args: OpenAIDecodingArguments):
         """
-        https://learn.microsoft.com/zh-cn/azure/cognitive-services/openai/how-to/chatgpt?pivots=programming-language-chat-completions
+        https://learn.microsoft.com/en-us/azure/cognitive-services/openai/how-to/chatgpt?pivots=programming-language-chat-completions
         https://platform.openai.com/docs/api-reference/chat
         """
 
         data = args.dict()
         completion = openai.ChatCompletion.create(**data)
         if data.get("stream", False):
             # create variables to collect the stream of chunks
@@ -192,33 +191,33 @@
         self.tool = tool
 
     @classmethod
     def from_config_file(cls, config_file):
         config = cls.load_json(config_file)
         api_type = config.get("api_type")
 
-        if api_type == "anthropic":
+        if api_type == "claude":
             return cls(ClaudeAITool(ClaudeMethod(api_key=config["api_key"], api_base=config["api"])))
         elif api_type == "azure":
             return cls(OpenAITool(AzureMethod(api_key=config["api_key"], api_base=config["api"])))
         elif api_type == "open_ai":
             return cls(OpenAITool(OpenAIMethod(api_key=config["api_key"], api_base=config["api"])))
         else:
-            raise AssertionError(f"Couldn\'t find API type in config file: {config_file}. Please specify \"api_type\" as \"anthropic\", \"azure\", or \"open_ai\".")
+            raise AssertionError(f"Couldn\'t find API type in config file: {config_file}. Please specify \"api_type\" as \"claude\", \"azure\", or \"open_ai\".")
 
     @classmethod
     def from_config(cls, api_key, api, api_type):
-        if api_type == "anthropic":
+        if api_type == "claude":
             return cls(ClaudeAITool(ClaudeMethod(api_key=api_key, api_base=api)))
         elif api_type == "azure":
             return cls(OpenAITool(AzureMethod(api_key=api_key, api_base=api)))
         elif api_type == "open_ai":
             return cls(OpenAITool(OpenAIMethod(api_key=api_key, api_base=api)))
         else:
-            raise AssertionError(f"Couldn\'t find API type: {api_type}. Please specify \"api_type\" as \"anthropic\", \"azure\", or \"open_ai\".")
+            raise AssertionError(f"Couldn\'t find API type: {api_type}. Please specify \"api_type\" as \"claude\", \"azure\", or \"open_ai\".")
 
 
     @staticmethod
     def load_json(file_path):
         with open(file_path, "r") as f:
             return json.load(f)
```

### Comparing `one-api-tool-0.1.3/setup.py` & `one-api-tool-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.1.3",
+    version="0.1.4",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
```

