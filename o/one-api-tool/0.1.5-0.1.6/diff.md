# Comparing `tmp/one-api-tool-0.1.5.tar.gz` & `tmp/one-api-tool-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.1.5.tar", last modified: Tue Apr 18 03:58:31 2023, max compression
+gzip compressed data, was "one-api-tool-0.1.6.tar", last modified: Tue Apr 18 12:10:42 2023, max compression
```

## Comparing `one-api-tool-0.1.5.tar` & `one-api-tool-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-18 03:58:31.246862 one-api-tool-0.1.5/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.1.5/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-18 03:58:31.246714 one-api-tool-0.1.5/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     1697 2023-04-18 03:55:54.000000 one-api-tool-0.1.5/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-18 03:58:31.246282 one-api-tool-0.1.5/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-18 03:58:31.000000 one-api-tool-0.1.5/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      242 2023-04-18 03:58:31.000000 one-api-tool-0.1.5/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-18 03:58:31.000000 one-api-tool-0.1.5/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       60 2023-04-18 03:58:31.000000 one-api-tool-0.1.5/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-04-18 03:58:31.000000 one-api-tool-0.1.5/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-18 03:58:31.246520 one-api-tool-0.1.5/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       47 2023-04-17 12:21:51.000000 one-api-tool-0.1.5/oneapi/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     9405 2023-04-18 03:56:28.000000 one-api-tool-0.1.5/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-18 03:58:31.246908 one-api-tool-0.1.5/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      908 2023-04-18 03:58:28.000000 one-api-tool-0.1.5/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-18 12:10:42.411072 one-api-tool-0.1.6/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.1.6/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-18 12:10:42.410894 one-api-tool-0.1.6/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1697 2023-04-18 03:55:54.000000 one-api-tool-0.1.6/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-18 12:10:42.409936 one-api-tool-0.1.6/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-18 12:10:42.000000 one-api-tool-0.1.6/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      242 2023-04-18 12:10:42.000000 one-api-tool-0.1.6/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-18 12:10:42.000000 one-api-tool-0.1.6/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       60 2023-04-18 12:10:42.000000 one-api-tool-0.1.6/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-04-18 12:10:42.000000 one-api-tool-0.1.6/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-18 12:10:42.410448 one-api-tool-0.1.6/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       47 2023-04-17 12:21:51.000000 one-api-tool-0.1.6/oneapi/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     9422 2023-04-18 12:06:13.000000 one-api-tool-0.1.6/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-18 12:10:42.411127 one-api-tool-0.1.6/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      908 2023-04-18 12:07:46.000000 one-api-tool-0.1.6/setup.py
```

### Comparing `one-api-tool-0.1.5/LICENSE` & `one-api-tool-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.1.5/PKG-INFO` & `one-api-tool-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.1.5
+Version: 0.1.6
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.1.5/README.md` & `one-api-tool-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.1.5/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.1.6/one_api_tool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.1.5
+Version: 0.1.6
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.1.5/oneapi/one_api.py` & `one-api-tool-0.1.6/oneapi/one_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,33 +52,34 @@
     method_commpletions = "completions"
 
 class OpenAIDecodingArguments(BaseModel):
     messages: List[ChatGPTMessage] 
     model: str = "gpt-3.5-turbo"
     max_tokens: int = 2048
     temperature: float = 1
-    top_p: float = 1.0
+    top_p: float = 1
     n: int = 1
     stream: bool = False
     stop: Optional[Sequence[str]] = None
-    presence_penalty: float = 1.0
-    frequency_penalty: float = 1.0
+    presence_penalty: float = 0
+    frequency_penalty: float = 0
     user: Optional[str] = ""
 
 class AzureDecodingArguments(BaseModel):
     messages: List[ChatGPTMessage] 
     engine: str = "gpt-35-turbo" # The deployment name you chose when you deployed the ChatGPT or GPT-4 model
     max_tokens: int = 2048
     temperature: float = 1
-    top_p: float = 1.0
+    top_p: float = 1
     n: int = 1
     stream: bool = False
     stop: Optional[Sequence[str]] = None
-    presence_penalty: float = 1.0
-    frequency_penalty: float = 1.0
+    presence_penalty: float = 0
+    frequency_penalty: float = 0
+    user: Optional[str] = ""
 
 
 class ClaudeDecodingArguments(BaseModel):
     prompt: str
     model: str = "claude-instant-v1"
     max_tokens_to_sample: int = 2048
     temperature: float = 1
```

### Comparing `one-api-tool-0.1.5/setup.py` & `one-api-tool-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
```

