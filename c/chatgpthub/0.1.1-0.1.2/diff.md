# Comparing `tmp/chatgpthub-0.1.1.tar.gz` & `tmp/chatgpthub-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpthub-0.1.1.tar", last modified: Tue Apr  4 15:59:40 2023, max compression
+gzip compressed data, was "chatgpthub-0.1.2.tar", last modified: Tue Apr 18 21:17:38 2023, max compression
```

## Comparing `chatgpthub-0.1.1.tar` & `chatgpthub-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxrwxr-x   0 kadir     (1000) kadir     (1000)        0 2023-04-04 15:59:40.500087 chatgpthub-0.1.1/
--rw-rw-r--   0 kadir     (1000) kadir     (1000)    11357 2023-03-31 14:44:11.000000 chatgpthub-0.1.1/LICENSE
--rw-rw-r--   0 kadir     (1000) kadir     (1000)       25 2023-03-31 14:44:11.000000 chatgpthub-0.1.1/MANIFEST.in
--rw-rw-r--   0 kadir     (1000) kadir     (1000)     2456 2023-04-04 15:59:40.500087 chatgpthub-0.1.1/PKG-INFO
--rw-rw-r--   0 kadir     (1000) kadir     (1000)     1401 2023-04-04 12:39:48.000000 chatgpthub-0.1.1/README.md
-drwxrwxr-x   0 kadir     (1000) kadir     (1000)        0 2023-04-04 15:59:40.496087 chatgpthub-0.1.1/chatgpthub/
--rw-rw-r--   0 kadir     (1000) kadir     (1000)      277 2023-04-04 15:59:32.000000 chatgpthub-0.1.1/chatgpthub/__init__.py
--rw-rw-r--   0 kadir     (1000) kadir     (1000)     4367 2023-04-04 15:59:32.000000 chatgpthub-0.1.1/chatgpthub/generate.py
--rw-rw-r--   0 kadir     (1000) kadir     (1000)     1908 2023-04-04 15:59:32.000000 chatgpthub-0.1.1/chatgpthub/load_tools.py
-drwxrwxr-x   0 kadir     (1000) kadir     (1000)        0 2023-04-04 15:59:40.500087 chatgpthub-0.1.1/chatgpthub/templates/
--rw-rw-r--   0 kadir     (1000) kadir     (1000)      175 2023-04-04 15:59:32.000000 chatgpthub-0.1.1/chatgpthub/templates/__init__.py
--rw-rw-r--   0 kadir     (1000) kadir     (1000)      706 2023-04-04 15:49:35.000000 chatgpthub-0.1.1/chatgpthub/templates/create_template.py
--rw-rw-r--   0 kadir     (1000) kadir     (1000)     1714 2023-03-31 18:38:29.000000 chatgpthub-0.1.1/chatgpthub/templates/translate_template.py
-drwxrwxr-x   0 kadir     (1000) kadir     (1000)        0 2023-04-04 15:59:40.500087 chatgpthub-0.1.1/chatgpthub/tools/
--rw-rw-r--   0 kadir     (1000) kadir     (1000)      116 2023-04-04 15:59:32.000000 chatgpthub-0.1.1/chatgpthub/tools/__init__.py
--rw-rw-r--   0 kadir     (1000) kadir     (1000)      453 2023-04-04 15:37:12.000000 chatgpthub-0.1.1/chatgpthub/tools/load_file.py
--rw-rw-r--   0 kadir     (1000) kadir     (1000)      842 2023-03-31 18:38:29.000000 chatgpthub-0.1.1/chatgpthub/tools/prompt_layer.py
-drwxrwxr-x   0 kadir     (1000) kadir     (1000)        0 2023-04-04 15:59:40.500087 chatgpthub-0.1.1/chatgpthub/utils/
--rw-rw-r--   0 kadir     (1000) kadir     (1000)       77 2023-04-04 15:50:14.000000 chatgpthub-0.1.1/chatgpthub/utils/__init__.py
--rw-rw-r--   0 kadir     (1000) kadir     (1000)      210 2023-03-31 18:38:29.000000 chatgpthub-0.1.1/chatgpthub/utils/key_utils.py
-drwxrwxr-x   0 kadir     (1000) kadir     (1000)        0 2023-04-04 15:59:40.496087 chatgpthub-0.1.1/chatgpthub.egg-info/
--rw-rw-r--   0 kadir     (1000) kadir     (1000)     2456 2023-04-04 15:59:40.000000 chatgpthub-0.1.1/chatgpthub.egg-info/PKG-INFO
--rw-rw-r--   0 kadir     (1000) kadir     (1000)      587 2023-04-04 15:59:40.000000 chatgpthub-0.1.1/chatgpthub.egg-info/SOURCES.txt
--rw-rw-r--   0 kadir     (1000) kadir     (1000)        1 2023-04-04 15:59:40.000000 chatgpthub-0.1.1/chatgpthub.egg-info/dependency_links.txt
--rw-rw-r--   0 kadir     (1000) kadir     (1000)       80 2023-04-04 15:59:40.000000 chatgpthub-0.1.1/chatgpthub.egg-info/requires.txt
--rw-rw-r--   0 kadir     (1000) kadir     (1000)       11 2023-04-04 15:59:40.000000 chatgpthub-0.1.1/chatgpthub.egg-info/top_level.txt
--rw-rw-r--   0 kadir     (1000) kadir     (1000)       78 2023-03-31 14:44:11.000000 chatgpthub-0.1.1/pyproject.toml
--rw-rw-r--   0 kadir     (1000) kadir     (1000)      117 2023-04-04 15:37:56.000000 chatgpthub-0.1.1/requirements.txt
--rw-rw-r--   0 kadir     (1000) kadir     (1000)      359 2023-04-04 15:59:40.500087 chatgpthub-0.1.1/setup.cfg
--rw-rw-r--   0 kadir     (1000) kadir     (1000)     1903 2023-04-03 22:58:49.000000 chatgpthub-0.1.1/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-18 21:17:38.068272 chatgpthub-0.1.2/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-18 20:56:22.000000 chatgpthub-0.1.2/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       25 2023-04-18 20:56:22.000000 chatgpthub-0.1.2/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2456 2023-04-18 21:17:38.068272 chatgpthub-0.1.2/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1401 2023-04-18 20:56:22.000000 chatgpthub-0.1.2/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-18 21:17:38.064939 chatgpthub-0.1.2/chatgpthub/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      277 2023-04-18 21:16:54.000000 chatgpthub-0.1.2/chatgpthub/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4367 2023-04-18 20:56:22.000000 chatgpthub-0.1.2/chatgpthub/generate.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-18 21:17:38.068272 chatgpthub-0.1.2/chatgpthub/templates/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      175 2023-04-18 20:56:22.000000 chatgpthub-0.1.2/chatgpthub/templates/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      706 2023-04-18 20:56:22.000000 chatgpthub-0.1.2/chatgpthub/templates/create_template.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      453 2023-04-18 21:09:31.000000 chatgpthub-0.1.2/chatgpthub/templates/csv_template.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1714 2023-04-18 20:56:22.000000 chatgpthub-0.1.2/chatgpthub/templates/translate_template.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-18 21:17:38.068272 chatgpthub-0.1.2/chatgpthub/tools/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      116 2023-04-18 20:56:22.000000 chatgpthub-0.1.2/chatgpthub/tools/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      842 2023-04-18 20:56:22.000000 chatgpthub-0.1.2/chatgpthub/tools/prompt_layer.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-18 21:17:38.068272 chatgpthub-0.1.2/chatgpthub/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       77 2023-04-18 20:56:22.000000 chatgpthub-0.1.2/chatgpthub/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      210 2023-04-18 20:56:22.000000 chatgpthub-0.1.2/chatgpthub/utils/key_utils.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-18 21:17:38.064939 chatgpthub-0.1.2/chatgpthub.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2456 2023-04-18 21:17:37.000000 chatgpthub-0.1.2/chatgpthub.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      569 2023-04-18 21:17:38.000000 chatgpthub-0.1.2/chatgpthub.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-18 21:17:37.000000 chatgpthub-0.1.2/chatgpthub.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-18 21:17:37.000000 chatgpthub-0.1.2/chatgpthub.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       11 2023-04-18 21:17:37.000000 chatgpthub-0.1.2/chatgpthub.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       78 2023-04-18 20:56:22.000000 chatgpthub-0.1.2/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      117 2023-04-18 20:56:22.000000 chatgpthub-0.1.2/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      359 2023-04-18 21:17:38.068272 chatgpthub-0.1.2/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1903 2023-04-18 20:56:22.000000 chatgpthub-0.1.2/setup.py
```

### Comparing `chatgpthub-0.1.1/LICENSE` & `chatgpthub-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpthub-0.1.1/PKG-INFO` & `chatgpthub-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpthub
-Version: 0.1.1
+Version: 0.1.2
 Summary: ChatGptHub: Gpt Chatbot Library with LangChain Support
 Home-page: https://github.com/kadirnar/chatgpthub
 Author: kadirnar
 License: Apache-2.0
 Keywords: chatgpt,chatbot,gpt-3,gpt-3.5-turbo,text-generation,language-model,language-modeling
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chatgpthub Version: 0.1.1 Summary: ChatGptHub: Gpt
+Metadata-Version: 2.1 Name: chatgpthub Version: 0.1.2 Summary: ChatGptHub: Gpt
 Chatbot Library with LangChain Support Home-page: https://github.com/kadirnar/
 chatgpthub Author: kadirnar License: Apache-2.0 Keywords: chatgpt,chatbot,gpt-
 3,gpt-3.5-turbo,text-generation,language-model,language-modeling Classifier:
 Development Status :: 5 - Production/Stable Classifier: Operating System :: OS
 Independent Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

### Comparing `chatgpthub-0.1.1/README.md` & `chatgpthub-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `chatgpthub-0.1.1/chatgpthub/generate.py` & `chatgpthub-0.1.2/chatgpthub/generate.py`

 * *Files identical despite different names*

### Comparing `chatgpthub-0.1.1/chatgpthub/templates/create_template.py` & `chatgpthub-0.1.2/chatgpthub/templates/create_template.py`

 * *Files identical despite different names*

### Comparing `chatgpthub-0.1.1/chatgpthub/templates/translate_template.py` & `chatgpthub-0.1.2/chatgpthub/templates/translate_template.py`

 * *Files identical despite different names*

### Comparing `chatgpthub-0.1.1/chatgpthub/tools/prompt_layer.py` & `chatgpthub-0.1.2/chatgpthub/tools/prompt_layer.py`

 * *Files identical despite different names*

### Comparing `chatgpthub-0.1.1/chatgpthub.egg-info/PKG-INFO` & `chatgpthub-0.1.2/chatgpthub.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpthub
-Version: 0.1.1
+Version: 0.1.2
 Summary: ChatGptHub: Gpt Chatbot Library with LangChain Support
 Home-page: https://github.com/kadirnar/chatgpthub
 Author: kadirnar
 License: Apache-2.0
 Keywords: chatgpt,chatbot,gpt-3,gpt-3.5-turbo,text-generation,language-model,language-modeling
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chatgpthub Version: 0.1.1 Summary: ChatGptHub: Gpt
+Metadata-Version: 2.1 Name: chatgpthub Version: 0.1.2 Summary: ChatGptHub: Gpt
 Chatbot Library with LangChain Support Home-page: https://github.com/kadirnar/
 chatgpthub Author: kadirnar License: Apache-2.0 Keywords: chatgpt,chatbot,gpt-
 3,gpt-3.5-turbo,text-generation,language-model,language-modeling Classifier:
 Development Status :: 5 - Production/Stable Classifier: Operating System :: OS
 Independent Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

### Comparing `chatgpthub-0.1.1/chatgpthub.egg-info/SOURCES.txt` & `chatgpthub-0.1.2/chatgpthub.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 chatgpthub/__init__.py
 chatgpthub/generate.py
-chatgpthub/load_tools.py
 chatgpthub.egg-info/PKG-INFO
 chatgpthub.egg-info/SOURCES.txt
 chatgpthub.egg-info/dependency_links.txt
 chatgpthub.egg-info/requires.txt
 chatgpthub.egg-info/top_level.txt
 chatgpthub/templates/__init__.py
 chatgpthub/templates/create_template.py
+chatgpthub/templates/csv_template.py
 chatgpthub/templates/translate_template.py
 chatgpthub/tools/__init__.py
-chatgpthub/tools/load_file.py
 chatgpthub/tools/prompt_layer.py
 chatgpthub/utils/__init__.py
 chatgpthub/utils/key_utils.py
```

### Comparing `chatgpthub-0.1.1/setup.py` & `chatgpthub-0.1.2/setup.py`

 * *Files identical despite different names*

