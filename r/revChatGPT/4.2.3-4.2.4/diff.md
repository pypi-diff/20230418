# Comparing `tmp/revChatGPT-4.2.3.tar.gz` & `tmp/revChatGPT-4.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-4.2.3.tar", last modified: Sun Apr 16 15:13:25 2023, max compression
+gzip compressed data, was "revChatGPT-4.2.4.tar", last modified: Tue Apr 18 02:36:58 2023, max compression
```

## Comparing `revChatGPT-4.2.3.tar` & `revChatGPT-4.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:13:25.220344 revChatGPT-4.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-16 15:12:53.000000 revChatGPT-4.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-04-16 15:13:25.220344 revChatGPT-4.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-04-16 15:13:25.000000 revChatGPT-4.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-16 15:13:25.224344 revChatGPT-4.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-16 15:12:53.000000 revChatGPT-4.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:13:25.220344 revChatGPT-4.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:13:25.220344 revChatGPT-4.2.3/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    47267 2023-04-16 15:12:53.000000 revChatGPT-4.2.3/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23198 2023-04-16 15:12:53.000000 revChatGPT-4.2.3/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-16 15:12:53.000000 revChatGPT-4.2.3/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-16 15:12:53.000000 revChatGPT-4.2.3/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:13:25.220344 revChatGPT-4.2.3/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-16 15:12:53.000000 revChatGPT-4.2.3/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-16 15:12:53.000000 revChatGPT-4.2.3/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-16 15:12:53.000000 revChatGPT-4.2.3/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:13:25.220344 revChatGPT-4.2.3/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-04-16 15:13:25.000000 revChatGPT-4.2.3/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-16 15:13:25.000000 revChatGPT-4.2.3/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 15:13:25.000000 revChatGPT-4.2.3/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-16 15:13:25.000000 revChatGPT-4.2.3/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-16 15:13:25.000000 revChatGPT-4.2.3/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:36:58.286491 revChatGPT-4.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-18 02:36:29.000000 revChatGPT-4.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-04-18 02:36:58.286491 revChatGPT-4.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-04-18 02:36:58.000000 revChatGPT-4.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-18 02:36:58.286491 revChatGPT-4.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-18 02:36:29.000000 revChatGPT-4.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:36:58.282492 revChatGPT-4.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:36:58.286491 revChatGPT-4.2.4/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    47267 2023-04-18 02:36:29.000000 revChatGPT-4.2.4/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-04-18 02:36:29.000000 revChatGPT-4.2.4/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-18 02:36:29.000000 revChatGPT-4.2.4/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-18 02:36:29.000000 revChatGPT-4.2.4/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:36:58.286491 revChatGPT-4.2.4/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-18 02:36:29.000000 revChatGPT-4.2.4/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-18 02:36:29.000000 revChatGPT-4.2.4/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-18 02:36:29.000000 revChatGPT-4.2.4/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:36:58.286491 revChatGPT-4.2.4/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-04-18 02:36:58.000000 revChatGPT-4.2.4/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-18 02:36:58.000000 revChatGPT-4.2.4/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 02:36:58.000000 revChatGPT-4.2.4/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-18 02:36:58.000000 revChatGPT-4.2.4/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 02:36:58.000000 revChatGPT-4.2.4/src/revChatGPT.egg-info/top_level.txt
```

### Comparing `revChatGPT-4.2.3/LICENSE` & `revChatGPT-4.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.3/PKG-INFO` & `revChatGPT-4.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 4.2.3
+Version: 4.2.4
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -26,14 +26,16 @@
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
 
+[![](https://github.com/acheong08/ChatGPT/blob/main/docs/view.gif?raw=true)](https://pypi.python.org/pypi/revChatGPT)
+
 > ## Support my work
 >
 > Make a pull request and fix my bad code.
 >
 > [![support](https://ko-fi.com/img/githubbutton_sm.svg)](https://www.youtube.com/watch?v=dQw4w9WgXcQ)
 
 > #### Discord Server: https://discord.gg/9K2BvbXEHT
```

### Comparing `revChatGPT-4.2.3/README.md` & `revChatGPT-4.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
 
+[![](https://github.com/acheong08/ChatGPT/blob/main/docs/view.gif?raw=true)](https://pypi.python.org/pypi/revChatGPT)
+
 > ## Support my work
 >
 > Make a pull request and fix my bad code.
 >
 > [![support](https://ko-fi.com/img/githubbutton_sm.svg)](https://www.youtube.com/watch?v=dQw4w9WgXcQ)
 
 > #### Discord Server: https://discord.gg/9K2BvbXEHT
```

### Comparing `revChatGPT-4.2.3/setup.py` & `revChatGPT-4.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="4.2.3",
+    version="4.2.4",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-4.2.3/src/revChatGPT/V1.py` & `revChatGPT-4.2.4/src/revChatGPT/V1.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,17 +67,17 @@
             return out
 
         return wrapper
 
     return decorator
 
 
-BASE_URL = environ.get("CHATGPT_BASE_URL") or "https://chat.gateway.do/api/"
+BASE_URL = environ.get("CHATGPT_BASE_URL") or "https://ai.fakeopen.com/api/"
 
-bcolors = t.colors()
+bcolors = t.Colors()
 
 
 class Chatbot:
     """
     Chatbot class for ChatGPT
     """
```

### Comparing `revChatGPT-4.2.3/src/revChatGPT/V3.py` & `revChatGPT-4.2.4/src/revChatGPT/V3.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
             timeout=kwargs.get("timeout", self.timeout),
             stream=True,
         )
         if response.status_code != 200:
             raise t.APIConnectionError(
                 f"{response.status_code} {response.reason} {response.text}",
             )
-        response_role: str = None
+        response_role: str or None = None
         full_response: str = ""
         for line in response.iter_lines():
             if not line:
                 continue
             # Remove "data: "
             line = line.decode("utf-8")[6:]
             if line == "[DONE]":
@@ -367,15 +367,15 @@
             del data["aclient"]
             json.dump(
                 data,
                 f,
                 indent=2,
             )
 
-    def load(self, file: str, *keys_: str) -> None:
+    def load(self, file: Path, *keys_: str) -> None:
         """
         Load the Chatbot configuration from a JSON file
         """
         with open(file, encoding="utf-8") as f:
             # load json, if session is in keys, load proxies
             loaded_config = json.load(f)
             keys = get_filtered_keys_from_object(self, *keys_)
```

### Comparing `revChatGPT-4.2.3/src/revChatGPT/__init__.py` & `revChatGPT-4.2.4/src/revChatGPT/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 The __init__ file does not a main file
 
 You can import the following module to use:
 revChatGPT.V0
 revChatGPT.V1
 revChatGPT.V3
 """
-__version__ = "4.2.1"
+__version__ = "4.2.2"
 __all__ = ()
 
 # Available Python Version Verify
 from . import typings as t
 from platform import python_version_tuple
 from platform import python_version
 from warnings import warn
```

### Comparing `revChatGPT-4.2.3/src/revChatGPT/__main__.py` & `revChatGPT-4.2.4/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.3/src/revChatGPT/config/enable_internet.json` & `revChatGPT-4.2.4/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.3/src/revChatGPT/typings.py` & `revChatGPT-4.2.4/src/revChatGPT/typings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from os import getenv
 from platform import python_version_tuple
-
 Any = object()
 
 SUPPORT_ADD_NOTES = [int(each) for each in python_version_tuple()][0] >= 3 and [
     int(each) for each in python_version_tuple()
 ][1] >= 11
 del python_version_tuple
 
@@ -24,15 +23,15 @@
 
 
 class MetaNotAllowInstance(type):
     """
     Metaclass that do not allow classes to be instantiated
     """
 
-    def __call__(self, *args: Any, **kwds: Any) -> Any:
+    def __call__(cls, *args: Any, **kwargs: Any) -> Any:
         error = ActionNotAllowedError("This class is not allowed to be instantiated")
         raise error
 
 
 class ActionError(ChatbotError):
     def __init__(self, *args: object) -> None:
         if SUPPORT_ADD_NOTES:
@@ -42,15 +41,15 @@
         super().__init__(*args)
 
 
 class ActionNotAllowedError(ActionError):
     """
     Subclass of ActionError
 
-    An object that throws an error because the execution of an unallowed operation is blocked
+    An object that throws an error because the execution of an unalloyed operation is blocked
     """
 
     pass
 
 
 class ActionRefuseError(ActionError):
     pass
@@ -76,15 +75,15 @@
     2: Rate limit error
     3: Invalid request error
     4: Expired access token error
     5: Invalid access token error
     6: Prohibited concurrent query error
     """
 
-    def __init__(self, source: str, message: str, code: int = 0, *args) -> None:
+    def __init__(self, source: str, message: str, code: int = 0, *args: object) -> None:
         self.source: str = source
         self.message: str = message
         self.code: int = code
         super().__init__(*args)
 
     def __str__(self) -> str:
         return f"{self.source}: {self.message} (code: {self.code})"
@@ -174,15 +173,15 @@
     EXPIRED_ACCESS_TOKEN_ERROR = 4
     INVALID_ACCESS_TOKEN_ERROR = 5
     PROHIBITED_CONCURRENT_QUERY_ERROR = 6
     AUTHENTICATION_ERROR = 7
     CLOUDFLARE_ERROR = 8
 
 
-class colors:
+class Colors:
     """
     Colors for printing
     """
 
     HEADER = "\033[95m"
     OKBLUE = "\033[94m"
     OKCYAN = "\033[96m"
```

### Comparing `revChatGPT-4.2.3/src/revChatGPT/utils.py` & `revChatGPT-4.2.4/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.3/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-4.2.4/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 4.2.3
+Version: 4.2.4
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -26,14 +26,16 @@
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
 
+[![](https://github.com/acheong08/ChatGPT/blob/main/docs/view.gif?raw=true)](https://pypi.python.org/pypi/revChatGPT)
+
 > ## Support my work
 >
 > Make a pull request and fix my bad code.
 >
 > [![support](https://ko-fi.com/img/githubbutton_sm.svg)](https://www.youtube.com/watch?v=dQw4w9WgXcQ)
 
 > #### Discord Server: https://discord.gg/9K2BvbXEHT
```

