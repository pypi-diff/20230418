# Comparing `tmp/iamai-3.14.4.post1.tar.gz` & `tmp/iamai-3.14.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamai-3.14.4.post1.tar", max compression
+gzip compressed data, was "iamai-3.14.5.tar", max compression
```

## Comparing `iamai-3.14.4.post1.tar` & `iamai-3.14.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-04-18 16:13:08.028408 iamai-3.14.4.post1/LICENSE
--rw-r--r--   0        0        0     9617 2023-04-18 16:13:08.028408 iamai-3.14.4.post1/README.md
--rw-r--r--   0        0        0      543 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/__init__.py
--rw-r--r--   0        0        0     4432 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/adapter/__init__.py
--rw-r--r--   0        0        0     1211 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/adapter/http_server_test_adapter.py
--rw-r--r--   0        0        0     1059 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/adapter/test.py
--rw-r--r--   0        0        0     7955 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/adapter/utils.py
--rw-r--r--   0        0        0    34820 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/bot.py
--rw-r--r--   0        0        0     1970 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/config.py
--rw-r--r--   0        0        0     1907 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/event.py
--rw-r--r--   0        0        0     1088 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/exceptions.py
--rw-r--r--   0        0        0      689 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/log.py
--rw-r--r--   0        0        0    13843 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/message.py
--rw-r--r--   0        0        0     3503 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/plugin.py
--rw-r--r--   0        0        0     1052 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/typing.py
--rw-r--r--   0        0        0     5529 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/utils.py
--rw-r--r--   0        0        0     2317 2023-04-18 16:13:08.040408 iamai-3.14.4.post1/pyproject.toml
--rw-r--r--   0        0        0    10918 1970-01-01 00:00:00.000000 iamai-3.14.4.post1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-18 16:22:36.618502 iamai-3.14.5/LICENSE
+-rw-r--r--   0        0        0     9629 2023-04-18 16:22:36.618502 iamai-3.14.5/README.md
+-rw-r--r--   0        0        0      543 2023-04-18 16:22:36.626502 iamai-3.14.5/iamai/__init__.py
+-rw-r--r--   0        0        0     4432 2023-04-18 16:22:36.626502 iamai-3.14.5/iamai/adapter/__init__.py
+-rw-r--r--   0        0        0     1211 2023-04-18 16:22:36.626502 iamai-3.14.5/iamai/adapter/http_server_test_adapter.py
+-rw-r--r--   0        0        0     1059 2023-04-18 16:22:36.626502 iamai-3.14.5/iamai/adapter/test.py
+-rw-r--r--   0        0        0     7955 2023-04-18 16:22:36.626502 iamai-3.14.5/iamai/adapter/utils.py
+-rw-r--r--   0        0        0    34820 2023-04-18 16:22:36.626502 iamai-3.14.5/iamai/bot.py
+-rw-r--r--   0        0        0     1970 2023-04-18 16:22:36.626502 iamai-3.14.5/iamai/config.py
+-rw-r--r--   0        0        0     1907 2023-04-18 16:22:36.626502 iamai-3.14.5/iamai/event.py
+-rw-r--r--   0        0        0     1088 2023-04-18 16:22:36.626502 iamai-3.14.5/iamai/exceptions.py
+-rw-r--r--   0        0        0      689 2023-04-18 16:22:36.626502 iamai-3.14.5/iamai/log.py
+-rw-r--r--   0        0        0    13843 2023-04-18 16:22:36.626502 iamai-3.14.5/iamai/message.py
+-rw-r--r--   0        0        0     3503 2023-04-18 16:22:36.626502 iamai-3.14.5/iamai/plugin.py
+-rw-r--r--   0        0        0     1052 2023-04-18 16:22:36.626502 iamai-3.14.5/iamai/typing.py
+-rw-r--r--   0        0        0     5529 2023-04-18 16:22:36.626502 iamai-3.14.5/iamai/utils.py
+-rw-r--r--   0        0        0     2311 2023-04-18 16:22:36.630502 iamai-3.14.5/pyproject.toml
+-rw-r--r--   0        0        0    10924 1970-01-01 00:00:00.000000 iamai-3.14.5/PKG-INFO
```

### Comparing `iamai-3.14.4.post1/LICENSE` & `iamai-3.14.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4.post1/README.md` & `iamai-3.14.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -190,13 +190,13 @@
 ## ✨ Project Activity
 
 ![Alt](https://repobeats.axiom.co/api/embed/cc9b8bded331c406e68cc0c7c294ef04122d6da2.svg "Repobeats analytics image")
 
 ## 👨‍🚀 Contributors
 
 <a href="https://github.com/retrofor/iamai/graphs/contributors">
-  <img src="https://contrib.rocks/image?repo=retrofor/iamai" />
+  <img width="150" src="https://contrib.rocks/image?repo=retrofor/iamai" />
 </a>
 
 ## 📄 License
 
 [MIT](https://github.com/retrofor/iamai/blob/main/LICENSE) © 2023-PRESENT [简律纯](https://github.com/HsiangNianian)
```

### Comparing `iamai-3.14.4.post1/iamai/__init__.py` & `iamai-3.14.5/iamai/__init__.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4.post1/iamai/adapter/__init__.py` & `iamai-3.14.5/iamai/adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4.post1/iamai/adapter/http_server_test_adapter.py` & `iamai-3.14.5/iamai/adapter/http_server_test_adapter.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4.post1/iamai/adapter/test.py` & `iamai-3.14.5/iamai/adapter/test.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4.post1/iamai/adapter/utils.py` & `iamai-3.14.5/iamai/adapter/utils.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4.post1/iamai/bot.py` & `iamai-3.14.5/iamai/bot.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4.post1/iamai/config.py` & `iamai-3.14.5/iamai/config.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4.post1/iamai/event.py` & `iamai-3.14.5/iamai/event.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4.post1/iamai/exceptions.py` & `iamai-3.14.5/iamai/exceptions.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4.post1/iamai/log.py` & `iamai-3.14.5/iamai/log.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4.post1/iamai/message.py` & `iamai-3.14.5/iamai/message.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4.post1/iamai/plugin.py` & `iamai-3.14.5/iamai/plugin.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4.post1/iamai/typing.py` & `iamai-3.14.5/iamai/typing.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4.post1/iamai/utils.py` & `iamai-3.14.5/iamai/utils.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4.post1/pyproject.toml` & `iamai-3.14.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamai"
-version = "3.14.4.post1"
+version = "3.14.5"
 description = "bot framework."
 authors = ["简律纯 <admin@jyunko.cn>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://retrofor.space/"
 repository = "https://github.com/retrofor/iamai"
 documentation = "https://iamai.retrofor.space/"
```

### Comparing `iamai-3.14.4.post1/PKG-INFO` & `iamai-3.14.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamai
-Version: 3.14.4.post1
+Version: 3.14.5
 Summary: bot framework.
 Home-page: https://retrofor.space/
 License: MIT
 Keywords: bot,qq,qqbot,mirai,coolq
 Author: 简律纯
 Author-email: admin@jyunko.cn
 Requires-Python: >=3.8,<4.0
@@ -225,14 +225,14 @@
 ## ✨ Project Activity
 
 ![Alt](https://repobeats.axiom.co/api/embed/cc9b8bded331c406e68cc0c7c294ef04122d6da2.svg "Repobeats analytics image")
 
 ## 👨‍🚀 Contributors
 
 <a href="https://github.com/retrofor/iamai/graphs/contributors">
-  <img src="https://contrib.rocks/image?repo=retrofor/iamai" />
+  <img width="150" src="https://contrib.rocks/image?repo=retrofor/iamai" />
 </a>
 
 ## 📄 License
 
 [MIT](https://github.com/retrofor/iamai/blob/main/LICENSE) © 2023-PRESENT [简律纯](https://github.com/HsiangNianian)
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: iamai Version: 3.14.4.post1 Summary: bot framework.
-Home-page: https://retrofor.space/ License: MIT Keywords:
-bot,qq,qqbot,mirai,coolq Author: ç®å¾çº¯ Author-email: admin@jyunko.cn
-Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 5 - Production/
-Stable Classifier: Framework :: Robot Framework Classifier: Framework :: Robot
-Framework :: Library Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3 Provides-Extra: all Provides-Extra:
-apscheduler Provides-Extra: cqhttp Provides-Extra: dingtalk Provides-Extra:
-hot-reload Requires-Dist: aiohttp (>=3.8.0,<4.0.0) Requires-Dist: loguru
-(>=0.6.0,<0.7.0) Requires-Dist: pydantic (>=1.10.0,<2.0.0) Requires-Dist: tomli
-(>=2.0.0,<3.0.0) ; python_version < "3.11" Requires-Dist: typing-extensions
-(>=4.4.0,<5.0.0) Project-URL: Documentation, https://iamai.retrofor.space/
-Project-URL: Repository, https://github.com/retrofor/iamai Description-Content-
-Type: text/markdown
+Metadata-Version: 2.1 Name: iamai Version: 3.14.5 Summary: bot framework. Home-
+page: https://retrofor.space/ License: MIT Keywords: bot,qq,qqbot,mirai,coolq
+Author: ç®å¾çº¯ Author-email: admin@jyunko.cn Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable Classifier: Framework
+:: Robot Framework Classifier: Framework :: Robot Framework :: Library
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3 Provides-Extra: all Provides-Extra: apscheduler Provides-Extra:
+cqhttp Provides-Extra: dingtalk Provides-Extra: hot-reload Requires-Dist:
+aiohttp (>=3.8.0,<4.0.0) Requires-Dist: loguru (>=0.6.0,<0.7.0) Requires-Dist:
+pydantic (>=1.10.0,<2.0.0) Requires-Dist: tomli (>=2.0.0,<3.0.0) ;
+python_version < "3.11" Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
+Project-URL: Documentation, https://iamai.retrofor.space/ Project-URL:
+Repository, https://github.com/retrofor/iamai Description-Content-Type: text/
+markdown
                    [https://iamai.retrofor.space/retro.png]
                               ****** iamai ******
                                [Discord] [QQç¾¤]
                       ç®ä½ä¸­æ ã«ã»ãã íêµ­ì´
             Cross-platform robot framework, mainly used for ML/DL.
                              [Website] [Website]
                                [pypi] [python]
```

