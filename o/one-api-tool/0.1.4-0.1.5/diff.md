# Comparing `tmp/one-api-tool-0.1.4.tar.gz` & `tmp/one-api-tool-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.1.4.tar", last modified: Tue Apr 18 03:35:55 2023, max compression
+gzip compressed data, was "one-api-tool-0.1.5.tar", last modified: Tue Apr 18 03:58:31 2023, max compression
```

## Comparing `one-api-tool-0.1.4.tar` & `one-api-tool-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-18 03:35:55.044484 one-api-tool-0.1.4/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.1.4/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     2233 2023-04-18 03:35:55.044333 one-api-tool-0.1.4/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     1677 2023-04-17 13:05:41.000000 one-api-tool-0.1.4/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-18 03:35:55.043735 one-api-tool-0.1.4/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     2233 2023-04-18 03:35:55.000000 one-api-tool-0.1.4/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      242 2023-04-18 03:35:55.000000 one-api-tool-0.1.4/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-18 03:35:55.000000 one-api-tool-0.1.4/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       60 2023-04-18 03:35:55.000000 one-api-tool-0.1.4/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-04-18 03:35:55.000000 one-api-tool-0.1.4/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-18 03:35:55.044143 one-api-tool-0.1.4/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       47 2023-04-17 12:21:51.000000 one-api-tool-0.1.4/oneapi/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     9385 2023-04-18 03:35:48.000000 one-api-tool-0.1.4/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-18 03:35:55.044534 one-api-tool-0.1.4/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      908 2023-04-18 03:29:23.000000 one-api-tool-0.1.4/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-18 03:58:31.246862 one-api-tool-0.1.5/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.1.5/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-18 03:58:31.246714 one-api-tool-0.1.5/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1697 2023-04-18 03:55:54.000000 one-api-tool-0.1.5/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-18 03:58:31.246282 one-api-tool-0.1.5/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-18 03:58:31.000000 one-api-tool-0.1.5/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      242 2023-04-18 03:58:31.000000 one-api-tool-0.1.5/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-18 03:58:31.000000 one-api-tool-0.1.5/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       60 2023-04-18 03:58:31.000000 one-api-tool-0.1.5/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-04-18 03:58:31.000000 one-api-tool-0.1.5/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-18 03:58:31.246520 one-api-tool-0.1.5/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       47 2023-04-17 12:21:51.000000 one-api-tool-0.1.5/oneapi/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     9405 2023-04-18 03:56:28.000000 one-api-tool-0.1.5/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-18 03:58:31.246908 one-api-tool-0.1.5/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      908 2023-04-18 03:58:28.000000 one-api-tool-0.1.5/setup.py
```

### Comparing `one-api-tool-0.1.4/LICENSE` & `one-api-tool-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.1.4/PKG-INFO` & `one-api-tool-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.1.4
+Version: 0.1.5
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -36,24 +36,24 @@
 }
 ```
 Antropic config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
     "api": "https://api.anthropic.com",
-    "api_type": "anthropic"
+    "api_type": "claude"
 }
 ```
 `api_key` OpenAI API key is availalle on the [website](https://platform.openai.com/account/api-keys), Clade API key here [website](https://console.anthropic.com/account/keys)
 
 `api` The base api used to send requests, you may also specify to a proxy url like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard, the form of API is usually:  https://{your origization}.openai.azure.com/
 
-`api_type` fixed value for "open_ai", "azure" or "anthropic"
+`api_type` Currently supported: "open_ai", "azure" or "claude".
 
-init OneAPITool object from a local config file:
+Initialize the `OneAPITool` object from a local configuration file.:
 ```python
 from oneapi import OneAPITool
 res = OneAPITool.from_config_file("your_config_file.json").simple_chat("Hello AI!")
 print(res)
 ```
 ### 2. (Not recommended) Writing the configuration directly into the code
 ```python
```

### Comparing `one-api-tool-0.1.4/README.md` & `one-api-tool-0.1.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -24,24 +24,24 @@
 }
 ```
 Antropic config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
     "api": "https://api.anthropic.com",
-    "api_type": "anthropic"
+    "api_type": "claude"
 }
 ```
 `api_key` OpenAI API key is availalle on the [website](https://platform.openai.com/account/api-keys), Clade API key here [website](https://console.anthropic.com/account/keys)
 
 `api` The base api used to send requests, you may also specify to a proxy url like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard, the form of API is usually:  https://{your origization}.openai.azure.com/
 
-`api_type` fixed value for "open_ai", "azure" or "anthropic"
+`api_type` Currently supported: "open_ai", "azure" or "claude".
 
-init OneAPITool object from a local config file:
+Initialize the `OneAPITool` object from a local configuration file.:
 ```python
 from oneapi import OneAPITool
 res = OneAPITool.from_config_file("your_config_file.json").simple_chat("Hello AI!")
 print(res)
 ```
 ### 2. (Not recommended) Writing the configuration directly into the code
 ```python
```

### Comparing `one-api-tool-0.1.4/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.1.5/one_api_tool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.1.4
+Version: 0.1.5
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -36,24 +36,24 @@
 }
 ```
 Antropic config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
     "api": "https://api.anthropic.com",
-    "api_type": "anthropic"
+    "api_type": "claude"
 }
 ```
 `api_key` OpenAI API key is availalle on the [website](https://platform.openai.com/account/api-keys), Clade API key here [website](https://console.anthropic.com/account/keys)
 
 `api` The base api used to send requests, you may also specify to a proxy url like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard, the form of API is usually:  https://{your origization}.openai.azure.com/
 
-`api_type` fixed value for "open_ai", "azure" or "anthropic"
+`api_type` Currently supported: "open_ai", "azure" or "claude".
 
-init OneAPITool object from a local config file:
+Initialize the `OneAPITool` object from a local configuration file.:
 ```python
 from oneapi import OneAPITool
 res = OneAPITool.from_config_file("your_config_file.json").simple_chat("Hello AI!")
 print(res)
 ```
 ### 2. (Not recommended) Writing the configuration directly into the code
 ```python
```

### Comparing `one-api-tool-0.1.4/oneapi/one_api.py` & `one-api-tool-0.1.5/oneapi/one_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,14 +86,15 @@
     top_k: int = -1
     stream: bool = True
     stop_sequences: Optional[Sequence[str]] = [anthropic.HUMAN_PROMPT]
 
 
 class AbstractAPITool(ABC):
 
+    @abstractmethod
     def simple_chat(args):
         raise NotImplementedError
         
 
 class OpenAITool(AbstractAPITool):
 
     def __init__(self,method : AbstrctMethod) -> None:
```

### Comparing `one-api-tool-0.1.4/setup.py` & `one-api-tool-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
```

