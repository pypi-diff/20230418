# Comparing `tmp/chatgptdevfriendly-0.0.11.tar.gz` & `tmp/chatgptdevfriendly-0.0.111.tar.gz`

## Comparing `chatgptdevfriendly-0.0.11.tar` & `chatgptdevfriendly-0.0.111.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    59016 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.11/printed_metrics.png
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.11/requirements.txt
--rw-r--r--   0        0        0    43746 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.11/response_times.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.11/src/chatgptdevfriendly/__init__.py
--rw-r--r--   0        0        0     8636 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.11/src/chatgptdevfriendly/main.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.11/tests/test_main.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.11/LICENSE.txt
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.11/README.md
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.11/pyproject.toml
--rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.11/PKG-INFO
+-rw-r--r--   0        0        0    59016 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.111/printed_metrics.png
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.111/requirements.txt
+-rw-r--r--   0        0        0    43746 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.111/response_times.png
+-rw-r--r--   0        0        0     8636 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.111/src/chatgptdevfriendly/V1.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.111/src/chatgptdevfriendly/__init__.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.111/tests/test_main.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.111/LICENSE.txt
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.111/README.md
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.111/pyproject.toml
+-rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.111/PKG-INFO
```

### Comparing `chatgptdevfriendly-0.0.11/printed_metrics.png` & `chatgptdevfriendly-0.0.111/printed_metrics.png`

 * *Files identical despite different names*

### Comparing `chatgptdevfriendly-0.0.11/response_times.png` & `chatgptdevfriendly-0.0.111/response_times.png`

 * *Files identical despite different names*

### Comparing `chatgptdevfriendly-0.0.11/src/chatgptdevfriendly/main.py` & `chatgptdevfriendly-0.0.111/src/chatgptdevfriendly/V1.py`

 * *Files identical despite different names*

### Comparing `chatgptdevfriendly-0.0.11/tests/test_main.py` & `chatgptdevfriendly-0.0.111/tests/test_main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 api_key = "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"
 model_name = "gpt-3.5-turbo"
 
-from src.chatgptdevfriendly.main import ChatGptSmartClient
+from chatgptdevfriendly.V1 import ChatGptSmartClient
 
 
 chatgptsmtclient = ChatGptSmartClient(api_key=api_key, model=model_name, log_info=True)
 
 for _ in range(10):
     chatgptsmtclient.query("List the top 10 upcoming startups in India?")
     chatgptsmtclient.query("Ok thanks, can you giv me the valuation of these startups in tabuar format")
```

### Comparing `chatgptdevfriendly-0.0.11/LICENSE.txt` & `chatgptdevfriendly-0.0.111/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chatgptdevfriendly-0.0.11/README.md` & `chatgptdevfriendly-0.0.111/README.md`

 * *Files identical despite different names*

### Comparing `chatgptdevfriendly-0.0.11/pyproject.toml` & `chatgptdevfriendly-0.0.111/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["hatchling", "openai>=0.27.3", "matplotlib>=3.7.1"]
+requires = ["hatchling", "openai==0.27.3", "matplotlib==3.7.1"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ChatGPTDevFriendly"
-version = "0.0.11"
+version = "0.0.111"
 authors = [
   { name="Srinivas Kumar R", email="srinivas1996kumar@gmail.com" },
 ]
 description = "A wrapper package which takes care of API call robustness to ensure developers quickly and easily develop CHatGPT based applications."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `chatgptdevfriendly-0.0.11/PKG-INFO` & `chatgptdevfriendly-0.0.111/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatGPTDevFriendly
-Version: 0.0.11
+Version: 0.0.111
 Summary: A wrapper package which takes care of API call robustness to ensure developers quickly and easily develop CHatGPT based applications.
 Project-URL: Homepage, https://github.com/codeastra2/ChatGPTDevFriendly
 Author-email: Srinivas Kumar R <srinivas1996kumar@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

