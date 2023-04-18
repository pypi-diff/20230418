# Comparing `tmp/iamai-3.14.4.tar.gz` & `tmp/iamai-3.14.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamai-3.14.4.tar", max compression
+gzip compressed data, was "iamai-3.14.4.post1.tar", max compression
```

## Comparing `iamai-3.14.4.tar` & `iamai-3.14.4.post1.tar`

### file list

```diff
@@ -1,25 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-04-05 06:03:03.797478 iamai-3.14.4/LICENSE
--rw-r--r--   0        0        0     9133 2023-04-05 06:03:03.797478 iamai-3.14.4/README.md
--rw-r--r--   0        0        0      543 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/__init__.py
--rw-r--r--   0        0        0     4432 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/__init__.py
--rw-r--r--   0        0        0     5157 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     9165 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0       44 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/github/__init.py
--rw-r--r--   0        0        0      924 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/github/config.py
--rw-r--r--   0        0        0        0 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/github/event.py
--rw-r--r--   0        0        0        0 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/github/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/github/message.py
--rw-r--r--   0        0        0     1210 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/http_server_test_adapter.py
--rw-r--r--   0        0        0     1059 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/test.py
--rw-r--r--   0        0        0     7954 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/utils.py
--rw-r--r--   0        0        0    34568 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/bot.py
--rw-r--r--   0        0        0     1968 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/config.py
--rw-r--r--   0        0        0     1906 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/event.py
--rw-r--r--   0        0        0     1088 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/exceptions.py
--rw-r--r--   0        0        0      429 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/log.py
--rw-r--r--   0        0        0    13843 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/message.py
--rw-r--r--   0        0        0     3503 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/plugin.py
--rw-r--r--   0        0        0     1052 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/typing.py
--rw-r--r--   0        0        0     5529 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/utils.py
--rw-r--r--   0        0        0     2311 2023-04-05 06:03:03.809478 iamai-3.14.4/pyproject.toml
--rw-r--r--   0        0        0    10428 1970-01-01 00:00:00.000000 iamai-3.14.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-18 16:13:08.028408 iamai-3.14.4.post1/LICENSE
+-rw-r--r--   0        0        0     9617 2023-04-18 16:13:08.028408 iamai-3.14.4.post1/README.md
+-rw-r--r--   0        0        0      543 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/__init__.py
+-rw-r--r--   0        0        0     4432 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/adapter/__init__.py
+-rw-r--r--   0        0        0     1211 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/adapter/http_server_test_adapter.py
+-rw-r--r--   0        0        0     1059 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/adapter/test.py
+-rw-r--r--   0        0        0     7955 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/adapter/utils.py
+-rw-r--r--   0        0        0    34820 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/bot.py
+-rw-r--r--   0        0        0     1970 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/config.py
+-rw-r--r--   0        0        0     1907 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/event.py
+-rw-r--r--   0        0        0     1088 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/exceptions.py
+-rw-r--r--   0        0        0      689 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/log.py
+-rw-r--r--   0        0        0    13843 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/message.py
+-rw-r--r--   0        0        0     3503 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/plugin.py
+-rw-r--r--   0        0        0     1052 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/typing.py
+-rw-r--r--   0        0        0     5529 2023-04-18 16:13:08.036408 iamai-3.14.4.post1/iamai/utils.py
+-rw-r--r--   0        0        0     2317 2023-04-18 16:13:08.040408 iamai-3.14.4.post1/pyproject.toml
+-rw-r--r--   0        0        0    10918 1970-01-01 00:00:00.000000 iamai-3.14.4.post1/PKG-INFO
```

### Comparing `iamai-3.14.4/LICENSE` & `iamai-3.14.4.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4/README.md` & `iamai-3.14.4.post1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,58 +11,64 @@
   <a href="/README_jp.md">にほんご</a>
   <a href="/README_ko.md">한국어</a>
 </p>
 <p align="center">
   Cross-platform robot framework, mainly used for ML/DL.
 </p>
 <p align="center">
-    <img src="https://img.shields.io/badge/docs-20230309-green?style=flat-square" alt="Website" href="https://iamai.retrofor.space" target="_blank"/>
-    <img src="https://img.shields.io/badge/playgroud-live-green?style=flat-square" alt="Website" href="https://playground.retrofor.space/iamai" target="_blank"/>
+<a style="text-decoration:none" href="https://iamai.retrofor.space" target="_blank">
+    <img src="https://img.shields.io/badge/docs-iamai.retrofor.space-yellow?style=flat-square" alt="Website">
+</a>
+  <a style="text-decoration:none" href="https://playground.retrofor.space/iamai" target="_blank">
+    <img src="https://img.shields.io/badge/playgroud-Under construction-cyan?style=flat-square" alt="Website">
+    </a>
   <br>
   <a href="https://pypi.python.org/pypi/iamai">
     <img src="https://img.shields.io/pypi/v/iamai?style=flat-square" alt="pypi">
   </a>
   <img src="https://img.shields.io/badge/python-3.8+-blue?style=flat-square" alt="python">
   <br>
   <img src="https://results.pre-commit.ci/badge/github/retrofor/iamai/main.svg">
   <br>
     <a style="text-decoration:none" href="https://www.codacy.com/gh/retrofor/iamai/dashboard?utm_source=github.com&utm_medium=referral&utm_content=retrofor/iamai&utm_campaign=Badge_Gradee" target="_blank">
     <img src="https://app.codacy.com/project/badge/Grade/f3611d85db764236b65fac956bdb53df" alt="Codacy Badge" />
   </a>
+    <img src="https://img.shields.io/badge/code_style-black-000000.svg?style=flat-square" alt="Codacy Badge" />
 </p>
 <p align="center">
 </p>
 <p align="center">
 <!-- onebot -->
   <a style="text-decoration:none" href="https://onebot.dev" target="_blank">
     <img src="https://img.shields.io/badge/-Onebot%2011-000020?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAHAAAABwCAMAAADxPgR5AAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAAAxQTFRF////29vbr6+vAAAAk1hCcwAAAAR0Uk5T////AEAqqfQAAAKcSURBVHja7NrbctswDATQXfD//zlpO7FlmwAWIOnOtNaTM5JwDMa8E+PNFz7g3waJ24fviyDPgfhz8fHP39cBcBL9KoJbQUxjA2iYqHL3FAnvzhL4GtVNUcoSZe6eSHizBcK5LL7dBr2AUZlev1ARRHCljzRALIEog6H3U6bCIyqIZdAT0eBuJYaGiJaHSjmkYIZd+qSGWAQnIaz2OArVnX6vrItQvbhZJtVGB5qX9wKqCMkb9W7aexfCO/rwQRBzsDIsYx4AOz0nhAtWu7bqkEQBO0Pr+Ftjt5fFCUEbm0Sbgdu8WSgJ5NgH2iu46R/o1UcBXJsFusWF/QUaz3RwJMEgngfaGGdSxJkE/Yg4lOBryBiMwvAhZrVMUUvwqU7F05b5WLaUIN4M4hRocQQRnEedgsn7TZB3UCpRrIJwQfqvGwsg18EnI2uSVNC8t+0QmMXogvbPg/xk+Mnw/6kW/rraUlvqgmFreAA09xW5t0AFlHrQZ3CsgvZm0FbHNKyBmheBKIF2cCA8A600aHPmFtRB1XvMsJAiza7LpPog0UJwccKdzw8rdf8MyN2ePYF896LC5hTzdZqxb6VNXInaupARLDNBWgI8spq4T0Qb5H4vWfPmHo8OyB1ito+AysNNz0oglj1U955sjUN9d41LnrX2D/u7eRwxyOaOpfyevCWbTgDEoilsOnu7zsKhjRCsnD/QzhdkYLBLXjiK4f3UWmcx2M7PO21CKVTH84638NTplt6JIQH0ZwCNuiWAfvuLhdrcOYPVO9eW3A67l7hZtgaY9GZo9AFc6cryjoeFBIWeU+npnk/nLE0OxCHL1eQsc1IciehjpJv5mqCsjeopaH6r15/MrxNnVhu7tmcslay2gO2Z1QfcfX0JMACG41/u0RrI9QAAAABJRU5ErkJggg==&logoColor=white" alt="onebotv11" />
+    </a>
     <!-- github -->
-    <img src="https://img.shields.io/badge/-github-181717?style=flat-square&logo=github&logoColor=white">
+    <!-- <img src="https://img.shields.io/badge/-github-181717?style=flat-square&logo=github&logoColor=white"> -->
     <!-- discord -->
-    <img src="https://img.shields.io/badge/-Discord-5865F2?style=flat-square&logo=Discord&logoColor=white">
-    <br>
+    <!-- <img src="https://img.shields.io/badge/-Discord-5865F2?style=flat-square&logo=Discord&logoColor=white"> -->
+    <!-- <br> -->
     <!-- bilibili live -->
-    <img src="https://img.shields.io/badge/-BiliBili Live-00A1D6?style=flat-square&logo=Bilibili&logoColor=white">
+    <!-- <img src="https://img.shields.io/badge/-BiliBili Live-00A1D6?style=flat-square&logo=Bilibili&logoColor=white"> -->
     <!-- mirai-api-http -->
     <img src="https://img.shields.io/badge/-Mirai%20api%20http%202.3+-00B8AA?style=flat-square">
     <!-- dingtalk -->
     <img src="https://img.shields.io/badge/-DingTalk-blue?style=flat-square">
     <!-- qqzone -->
-    <img src="https://img.shields.io/badge/-QQ%20Zone-FECC00?style=flat-square&logo=Tencent QQ&logoColor=black">
-    <br>
+    <!-- <img src="https://img.shields.io/badge/-QQ%20Zone-FECC00?style=flat-square&logo=Tencent QQ&logoColor=black"> -->
+    <!-- <br> -->
     <!-- minecraft -->
-    <img src="https://img.shields.io/badge/-Minecraft Server-62B47A?style=flat-square&logo=Minecraft&logoColor=white">
+    <!-- <img src="https://img.shields.io/badge/-Minecraft Server-62B47A?style=flat-square&logo=Minecraft&logoColor=white"> -->
     <!-- twitter -->
-    <img src="https://img.shields.io/badge/-Twitter-1DA1F2?style=flat-square&logo=twitter&logoColor=white">
+    <!-- <img src="https://img.shields.io/badge/-Twitter-1DA1F2?style=flat-square&logo=twitter&logoColor=white"> -->
     <!-- console -->
     <img src="https://img.shields.io/badge/-Console-4EAA25?style=flat-square&logo=GNU bash&logoColor=white">
     <!-- wechat -->
-    <img src="https://img.shields.io/badge/-Wechat-07C160?style=flat-square&logo=wechat&logoColor=white">
+    <!-- <img src="https://img.shields.io/badge/-Wechat-07C160?style=flat-square&logo=wechat&logoColor=white"> -->
     <!-- tg -->
-    <img src="https://img.shields.io/badge/-Telegram-26A5E4?style=flat-square&logo=telegram&logoColor=white">
+    <!-- <img src="https://img.shields.io/badge/-Telegram-26A5E4?style=flat-square&logo=telegram&logoColor=white"> -->
   </a>
 </p>
 <p align="center">
 </p>
 <p align="center">
   <img src="https://img.shields.io/github/forks/retrofor/iamai?style=social" >
   <img src="https://img.shields.io/github/stars/retrofor/iamai?style=social" >
@@ -81,34 +87,49 @@
 ## 🚀 Features
 
 - 🎪 **Interactive [docs](https://iamai.retrofor.space) &amp; [demos](https://iamai.retrofor.space/demos)**
 - 🕶 **Seamless migration**: Works for **both** [Rasa]() and [GPT]() and more...
 - ⚡ **Fully tree shakeable**: Only take what you want, [bundle size](https://iamai.retrofor.space/export-size)
 - 🔩 **Flexible**: Configurable event filters and targets
 - 🔌 **Optional [Add-ons](https://iamai.retrofor.space/add-ons)**: [Apscheduler](https://iamai.retrofor.space/add-ons/apscheduler), etc.
-- 👍 **Cross-platform**: [Onebot](https://iamai.retrofor.space/adapters/onebot), [Wechat](https://iamai.retrofor.space/adapters/wechat), [Twitter](https://iamai.retrofor.space/adapters/twitter), [Bilibili](https://iamai.retrofor.space/adapters/bilibili), [Github](https://iamai.retrofor.space/adapters/github), etc.
+- 👍 **Cross-platform**: [cqhttp](https://iamai.retrofor.space/guide/cqhttp-adapter.html), [dingtalk](https://iamai.retrofor.space/guide/dingtalk-adapter.html), [Mirai](https://iamai.retrofor.space/guide/mirai-adapter.html) etc.
 
 <p align="center"><img width="512" src="https://iamai.retrofor.space/icons/retro_plus.png"></p>
 
 ## ⬇️ Install
 
+### FrameWork
+
 - STABLE VERSION
 
   ```sh
   pip install iamai
   ```
 
 or you can also install for TEST.
 
 - TEST VERSION
 
   ```sh
-  pip install -i https://test.pypi.org/simple/ iamai
+  git clone https://github.com/retrofor/iamai.git
+  cd iamai
+  poetry install --no-dev  # 推荐
+  pip install .  # 不推荐
   ```
 
+### Adapters
+
+iamai itself is just a chatbot framework and additional protocol adapters are required to support specific protocols. You can use pip to install the protocol adapter:
+
+```py
+pip install iamai-adapter-cqhttp
+pip install iamai-adapter-mirai
+pip install iamai-adapter-dingtalk
+```
+
 ## ❗ Usage
 
 firstly, you need to load an adapter.
 
 ```python
 from iamai import Bot
 
@@ -116,15 +137,15 @@
 bot.load_adapters("iamai.adapter.cqhttp")
 
 bot.run()
 ```
 
 then, you need load the transformer and use your models.
 
-**transformer(Use from the 🤗/transformers library)**
+### transformer(Use from the 🤗/transformers library)
 
 ```python
 from transformers import AutoModelWithLMHead, AutoTokenizer
 # load models
 model = AutoModelWithLMHead.from_pretrained("gpt2")
 # load tokenizer
 tokenizer = AutoTokenizer.from_pretrained("gpt2")
@@ -138,15 +159,15 @@
 
 You can use pre-built optimizers to speed up the model inference process, or you can write your own optimizer. However, it's important to note that the transformer model optimizer is a special type of optimizer that is designed specifically for optimizing parameters in transformer models, thereby improving their performance.
 
 To write a transformer model optimizer, you need to have an understanding of how optimizers work and be familiar with the structure of transformer models.
 
 The principle of optimizers can be referred to in the paper [&#34;Attention Is All You Need&#34;](https://arxiv.org/abs/1706.03762), and the structure of transformer models can be referred to in the paper [&#34;Transformer: A Novel Neural Network Architecture for Language Understanding&#34;](https://ai.googleblog.com/2017/08/transformer-novel-neural-network.html?m=1). The implementation of optimizers can be referred to in the [AdamW optimizer](https://huggingface.co/transformers/v3.0.2/main_classes/optimizer_schedules.html) in the Hugging Face Transformers library.
 
-**Use the Inference API**
+### Use the Inference API
 
 ```python
 import requests
 
 API_URL = "https://api-inference.huggingface.co/models/xxx/xxxxx"
 headers = {"Authorization": "Bearer xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"}
 
@@ -160,16 +181,15 @@
 ```
 
 ## 👀 See the docs
 
 > choices below.
 
 - [https://iamai.retrofor.space](https://iamai.retrofor.space) _(recommend)_
-- [https://iamai-docs-git-main-retrofor.vercel.app](https://iamai-docs-git-main-retrofor.vercel.app)
-- ~~[https://iamai-docs-retrofor.vercel.app/](https://iamai-docs-retrofor.vercel.app/)~~
+- [retrofor.github.io/iamai](https://retrofor.github.io/iamai)
 
 ## ✨ Project Activity
 
 ![Alt](https://repobeats.axiom.co/api/embed/cc9b8bded331c406e68cc0c7c294ef04122d6da2.svg "Repobeats analytics image")
 
 ## 👨‍🚀 Contributors
```

#### html2text {}

```diff
@@ -2,57 +2,50 @@
                               ****** iamai ******
                                [Discord] [QQç¾¤]
                       ç®ä½ä¸­æ ã«ã»ãã íêµ­ì´
             Cross-platform robot framework, mainly used for ML/DL.
                              [Website] [Website]
                                [pypi] [python]
      [https://results.pre-commit.ci/badge/github/retrofor/iamai/main.svg]
-                                [Codacy_Badge]
-     [onebotv11]__[https://img.shields.io/badge/-github-181717?style=flat-
- square&logo=github&logoColor=white]__[https://img.shields.io/badge/-Discord-
-            5865F2?style=flat-square&logo=Discord&logoColor=white]_
-       _[https://img.shields.io/badge/-BiliBili_Live-00A1D6?style=flat-
-    square&logo=Bilibili&logoColor=white]__[https://img.shields.io/badge/-
- Mirai%20api%20http%202.3+-00B8AA?style=flat-square]__[https://img.shields.io/
-   badge/-DingTalk-blue?style=flat-square]__[https://img.shields.io/badge/-
-     QQ%20Zone-FECC00?style=flat-square&logo=Tencent_QQ&logoColor=black]_
-      _[https://img.shields.io/badge/-Minecraft_Server-62B47A?style=flat-
-square&logo=Minecraft&logoColor=white]__[https://img.shields.io/badge/-Twitter-
-       1DA1F2?style=flat-square&logo=twitter&logoColor=white]__[https://
-        img.shields.io/badge/-Console-4EAA25?style=flat-square&logo=GNU
-bash&logoColor=white]__[https://img.shields.io/badge/-Wechat-07C160?style=flat-
- square&logo=wechat&logoColor=white]__[https://img.shields.io/badge/-Telegram-
-            26A5E4?style=flat-square&logo=telegram&logoColor=white]
+                         [Codacy_Badge] [Codacy Badge]
+ [onebotv11]         [https://img.shields.io/badge/-Mirai%20api%20http%202.3+-
+      00B8AA?style=flat-square]  [https://img.shields.io/badge/-DingTalk-
+    blue?style=flat-square]         [https://img.shields.io/badge/-Console-
+          4EAA25?style=flat-square&logo=GNU bash&logoColor=white]
   [https://img.shields.io/github/forks/retrofor/iamai?style=social] [https://
            img.shields.io/github/stars/retrofor/iamai?style=social]
 [https://img.shields.io/github/watchers/retrofor/iamai?style=social] [https://
         img.shields.io/github/search/retrofor/iamai/goto?style=social]
 [https://img.shields.io/github/repo-size/retrofor/iamai?style=social] [https://
        img.shields.io/github/languages/top/retrofor/iamai?style=social]
 ## ð Introduction A Cross-platform robot framework, mainly used for machine
 learning. ## ð Features - ðª **Interactive [docs](https://
 iamai.retrofor.space) & [demos](https://iamai.retrofor.space/demos)** - ð¶
 **Seamless migration**: Works for **both** [Rasa]() and [GPT]() and more... -
 â¡ **Fully tree shakeable**: Only take what you want, [bundle size](https://
 iamai.retrofor.space/export-size) - ð© **Flexible**: Configurable event
 filters and targets - ð **Optional [Add-ons](https://iamai.retrofor.space/
 add-ons)**: [Apscheduler](https://iamai.retrofor.space/add-ons/apscheduler),
-etc. - ð **Cross-platform**: [Onebot](https://iamai.retrofor.space/adapters/
-onebot), [Wechat](https://iamai.retrofor.space/adapters/wechat), [Twitter]
-(https://iamai.retrofor.space/adapters/twitter), [Bilibili](https://
-iamai.retrofor.space/adapters/bilibili), [Github](https://iamai.retrofor.space/
-adapters/github), etc.
+etc. - ð **Cross-platform**: [cqhttp](https://iamai.retrofor.space/guide/
+cqhttp-adapter.html), [dingtalk](https://iamai.retrofor.space/guide/dingtalk-
+adapter.html), [Mirai](https://iamai.retrofor.space/guide/mirai-adapter.html)
+etc.
               [https://iamai.retrofor.space/icons/retro_plus.png]
-## â¬ï¸ Install - STABLE VERSION ```sh pip install iamai ``` or you can also
-install for TEST. - TEST VERSION ```sh pip install -i https://test.pypi.org/
-simple/ iamai ``` ## â Usage firstly, you need to load an adapter. ```python
-from iamai import Bot bot = Bot() bot.load_adapters("iamai.adapter.cqhttp")
-bot.run() ``` then, you need load the transformer and use your models.
-**transformer(Use from the ð¤/transformers library)** ```python from
-transformers import AutoModelWithLMHead, AutoTokenizer # load models model =
+## â¬ï¸ Install ### FrameWork - STABLE VERSION ```sh pip install iamai ``` or
+you can also install for TEST. - TEST VERSION ```sh git clone https://
+github.com/retrofor/iamai.git cd iamai poetry install --no-dev # æ¨è pip
+install . # ä¸æ¨è ``` ### Adapters iamai itself is just a chatbot framework
+and additional protocol adapters are required to support specific protocols.
+You can use pip to install the protocol adapter: ```py pip install iamai-
+adapter-cqhttp pip install iamai-adapter-mirai pip install iamai-adapter-
+dingtalk ``` ## â Usage firstly, you need to load an adapter. ```python from
+iamai import Bot bot = Bot() bot.load_adapters("iamai.adapter.cqhttp") bot.run
+() ``` then, you need load the transformer and use your models. ### transformer
+(Use from the ð¤/transformers library) ```python from transformers import
+AutoModelWithLMHead, AutoTokenizer # load models model =
 AutoModelWithLMHead.from_pretrained("gpt2") # load tokenizer tokenizer =
 AutoTokenizer.from_pretrained("gpt2") # transfor the text to token input_ids =
 tokenizer.encode("Hello, my name is IamAI!", add_special_tokens=True) # input
 the token to the models outputs = model.generate(input_ids) # get the text
 generated generated_text = tokenizer.decode(outputs[0]) ``` You can use pre-
 built optimizers to speed up the model inference process, or you can write your
 own optimizer. However, it's important to note that the transformer model
@@ -63,22 +56,20 @@
 transformer models. The principle of optimizers can be referred to in the paper
 ["Attention Is All You Need"](https://arxiv.org/abs/1706.03762), and the
 structure of transformer models can be referred to in the paper ["Transformer:
 A Novel Neural Network Architecture for Language Understanding"](https://
 ai.googleblog.com/2017/08/transformer-novel-neural-network.html?m=1). The
 implementation of optimizers can be referred to in the [AdamW optimizer](https:
 //huggingface.co/transformers/v3.0.2/main_classes/optimizer_schedules.html) in
-the Hugging Face Transformers library. **Use the Inference API** ```python
+the Hugging Face Transformers library. ### Use the Inference API ```python
 import requests API_URL = "https://api-inference.huggingface.co/models/xxx/
 xxxxx" headers = {"Authorization": "Bearer
 xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"} def query(payload): response =
 requests.post(API_URL, headers=headers, json=payload) return response.json()
 output = query({ "inputs": "xxx", }) ``` ## ð See the docs > choices below.
 - [https://iamai.retrofor.space](https://iamai.retrofor.space) _(recommend)_ -
-[https://iamai-docs-git-main-retrofor.vercel.app](https://iamai-docs-git-main-
-retrofor.vercel.app) - ~~[https://iamai-docs-retrofor.vercel.app/](https://
-iamai-docs-retrofor.vercel.app/)~~ ## â¨ Project Activity ![Alt](https://
-repobeats.axiom.co/api/embed/cc9b8bded331c406e68cc0c7c294ef04122d6da2.svg
-"Repobeats analytics image") ## ð¨âð Contributors [https://
-contrib.rocks/image?repo=retrofor/iamai] ## ð License [MIT](https://
-github.com/retrofor/iamai/blob/main/LICENSE) Â© 2023-PRESENT [ç®å¾çº¯](https:
-//github.com/HsiangNianian)
+[retrofor.github.io/iamai](https://retrofor.github.io/iamai) ## â¨ Project
+Activity ![Alt](https://repobeats.axiom.co/api/embed/
+cc9b8bded331c406e68cc0c7c294ef04122d6da2.svg "Repobeats analytics image") ##
+ð¨âð Contributors [https://contrib.rocks/image?repo=retrofor/iamai] ##
+ð License [MIT](https://github.com/retrofor/iamai/blob/main/LICENSE) Â©
+2023-PRESENT [ç®å¾çº¯](https://github.com/HsiangNianian)
```

### Comparing `iamai-3.14.4/iamai/__init__.py` & `iamai-3.14.4.post1/iamai/__init__.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4/iamai/adapter/__init__.py` & `iamai-3.14.4.post1/iamai/adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4/iamai/adapter/http_server_test_adapter.py` & `iamai-3.14.4.post1/iamai/adapter/http_server_test_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """HTTP 服务端适配器示例。
 
 这里是一个最简单可以直接使用的 HTTP 服务端适配器示例。
 """
 from typing import TYPE_CHECKING, Union
 
 from aiohttp import web
+
 from iamai.event import Event
 from iamai.adapter.utils import HttpServerAdapter
 from iamai.message import Message, MessageSegment
 
 if TYPE_CHECKING:
     from iamai.message import T_Message, T_MessageSegment
```

### Comparing `iamai-3.14.4/iamai/adapter/test.py` & `iamai-3.14.4.post1/iamai/adapter/test.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4/iamai/adapter/utils.py` & `iamai-3.14.4.post1/iamai/adapter/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 import asyncio
 from typing import Union, Literal
 from abc import ABCMeta, abstractmethod
 
 import aiohttp
 from aiohttp import web
+
 from iamai.adapter import Adapter
 from iamai.typing import T_Event, T_Config
 from iamai.log import logger, error_or_exception
 
 
 class PollingAdapter(Adapter[T_Event, T_Config], metaclass=ABCMeta):
     """轮询式适配器示例。"""
```

### Comparing `iamai-3.14.4/iamai/bot.py` & `iamai-3.14.4.post1/iamai/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 import asyncio
 import threading
 from pathlib import Path
 from itertools import chain
 from collections import defaultdict
 from typing import Any, Dict, List, Type, Union, Callable, Optional, Awaitable
 
+from pydantic import ValidationError, create_model
+
 from iamai.adapter import Adapter
 from iamai.plugin import Plugin, PluginLoadType
 from iamai.log import logger, error_or_exception
-from pydantic import ValidationError, create_model
 from iamai.typing import T_Event, T_BotHook, T_EventHook, T_AdapterHook
 from iamai.config import MainConfig, ConfigModel, PluginConfig, AdapterConfig
 from iamai.exceptions import (
     SkipException,
     StopException,
     GetEventTimeout,
     LoadModuleError,
@@ -79,15 +80,16 @@
     _config_file: Optional[str]  # 配置文件
     _config_dict: Optional[Dict[str, Any]]  # 配置字典
     _hot_reload: bool  # 热重载
 
     _extend_plugins: List[
         Union[Type[Plugin], str, Path]
     ]  # 使用 load_plugins() 方法程序化加载的插件列表
-    _extend_plugin_dirs: List[Path]  # 使用 load_plugins_from_dirs() 方法程序化加载的插件路径列表
+    # 使用 load_plugins_from_dirs() 方法程序化加载的插件路径列表
+    _extend_plugin_dirs: List[Path]
     _extend_adapters: List[str]  # 使用 load_adapter() 方法程序化加载的适配器列表
     _bot_run_hooks: List[T_BotHook]
     _bot_exit_hooks: List[T_BotHook]
     _adapter_startup_hooks: List[T_AdapterHook]
     _adapter_run_hooks: List[T_AdapterHook]
     _adapter_shutdown_hooks: List[T_AdapterHook]
     _event_preprocessor_hooks: List[T_EventHook]
@@ -182,15 +184,15 @@
         # 加载插件和适配器
         self._load_plugins_from_dirs(*self.config.bot.plugin_dirs)
         self._load_plugins(*self.config.bot.plugins)
         self._load_adapters(*self.config.bot.adapters)
         self._update_config()
 
         # 启动 iamai
-        logger.warning("Running iamai...")
+        logger.info("Running iamai...")
 
         hot_reload_task = None
         if self._hot_reload:
             hot_reload_task = asyncio.create_task(self._run_hot_reload())
 
         for _hook_func in self._bot_run_hooks:
             await _hook_func(self)
@@ -257,15 +259,15 @@
         except ImportError:
             logger.warning(
                 'Hot reload needs to install "watchfiles", '
                 'try "pip install watchfiles"'
             )
             return
 
-        logger.success("Hot reload is working!")
+        logger.warning("Hot reload is working!")
         async for changes in awatch(
             *map(
                 lambda x: x.resolve(),
                 set(self._extend_plugin_dirs)
                 .union(self.config.bot.plugin_dirs)
                 .union(
                     {Path(self._config_file)}
@@ -349,15 +351,19 @@
             "Config",
             plugin=update_config(self.plugins, "PluginConfig", PluginConfig),
             adapter=update_config(self.adapters, "AdapterConfig", AdapterConfig),
             __base__=MainConfig,
         )(**self._raw_config_dict)
         # 更新 log 级别
         logger.remove()
-        logger.add(sys.stderr, level=self.config.bot.log.level)
+        logger.add(
+            sys.stderr,
+            level=self.config.bot.log.level,
+            format="<magenta>{time:YYYY-MM-DD HH:mm:ss.SSS}</magenta> <level>[{level}]</level> > <cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> - <level>{message}</level>",
+        )
 
     def _reload_config_dict(self):
         """重新加载配置文件。"""
         self._raw_config_dict = {}
         if self._config_dict is not None:
             self._raw_config_dict = self._config_dict
         elif self._config_file is not None:
@@ -677,18 +683,19 @@
     def _load_plugins_from_dirs(self, *dirs: Path):
         """从目录中加载插件，以 `_` 开头的模块中的插件不会被导入。路径可以是相对路径或绝对路径。
 
         Args:
             *dirs: 储存包含插件的模块的模块路径。
                 例如：`pathlib.Path("path/of/plugins/")` 。
         """
-        dirs = list(map(lambda x: str(x.resolve()), dirs)) # type: ignore
+        dirs = list(map(lambda x: str(x.resolve()), dirs))  # type: ignore  maybe remove?
         logger.warning(f'Loading plugins from dirs "{", ".join(map(str, dirs))}"')
-        self._module_path_finder.path.extend(dirs) # type: ignore
-        for plugin_class, module in get_classes_from_dir(dirs, Plugin): # type: ignore
+        self._module_path_finder.path.extend(dirs)  # type: ignore
+        # type: ignore
+        for plugin_class, module in get_classes_from_dir(dirs, Plugin):
             self._load_plugin_class(plugin_class, PluginLoadType.DIR, module.__file__)
 
     def load_plugins_from_dirs(self, *dirs: Path):
         """从目录中加载插件，以 `_` 开头的模块中的插件不会被导入。路径可以是相对路径或绝对路径。
 
         Args:
             *dirs: 储存包含插件的模块的模块路径。
@@ -722,15 +729,15 @@
                         raise LoadModuleError(
                             f"Can not find Adapter class in the {adapter_} module"
                         )
                     elif len(adapter_classes) > 1:
                         raise LoadModuleError(
                             f"More then one Adapter class in the {adapter_} module"
                         )
-                    adapter_object = adapter_classes[0][0](self) # type: ignore
+                    adapter_object = adapter_classes[0][0](self)  # type: ignore
                 else:
                     raise LoadModuleError(
                         f"Type error: {adapter_} can not be loaded as adapter"
                     )
             except Exception as e:
                 error_or_exception(
                     f'Load adapter "{adapter_}" failed:',
```

### Comparing `iamai-3.14.4/iamai/config.py` & `iamai-3.14.4.post1/iamai/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,17 +60,19 @@
 class PluginConfig(ConfigModel):
     """插件配置。"""
 
 
 class AdapterConfig(ConfigModel):
     """适配器配置。"""
 
+
 class DebugConfig(ConfigModel):
     """是否打印事件配置。"""
 
+
 class MainConfig(ConfigModel):
     """iamai 配置。
 
     Attributes:
         bot: iamai 的主要配置。
     """
```

### Comparing `iamai-3.14.4/iamai/event.py` & `iamai-3.14.4.post1/iamai/event.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """iamai 事件。
 
 事件类的基类。适配器开发者应实现此事件类基类的子类。
 """
 from abc import ABC
 from typing import Any, Generic, Optional
 
+from pydantic import BaseModel, PrivateAttr
+
 from iamai.message import Message
 from iamai.typing import T_Adapter
 from iamai.utils import DataclassEncoder
-from pydantic import BaseModel, PrivateAttr
 
 __all__ = ["Event"]
 
 
 class Event(ABC, BaseModel, Generic[T_Adapter]):
     """事件类的基类。
```

### Comparing `iamai-3.14.4/iamai/exceptions.py` & `iamai-3.14.4.post1/iamai/exceptions.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4/iamai/message.py` & `iamai-3.14.4.post1/iamai/message.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4/iamai/plugin.py` & `iamai-3.14.4.post1/iamai/plugin.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4/iamai/typing.py` & `iamai-3.14.4.post1/iamai/typing.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4/iamai/utils.py` & `iamai-3.14.4.post1/iamai/utils.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.4/pyproject.toml` & `iamai-3.14.4.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamai"
-version = "3.14.4"
+version = "3.14.4.post1"
 description = "bot framework."
 authors = ["简律纯 <admin@jyunko.cn>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://retrofor.space/"
 repository = "https://github.com/retrofor/iamai"
 documentation = "https://iamai.retrofor.space/"
```

### Comparing `iamai-3.14.4/PKG-INFO` & `iamai-3.14.4.post1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamai
-Version: 3.14.4
+Version: 3.14.4.post1
 Summary: bot framework.
 Home-page: https://retrofor.space/
 License: MIT
 Keywords: bot,qq,qqbot,mirai,coolq
 Author: 简律纯
 Author-email: admin@jyunko.cn
 Requires-Python: >=3.8,<4.0
@@ -46,58 +46,64 @@
   <a href="/README_jp.md">にほんご</a>
   <a href="/README_ko.md">한국어</a>
 </p>
 <p align="center">
   Cross-platform robot framework, mainly used for ML/DL.
 </p>
 <p align="center">
-    <img src="https://img.shields.io/badge/docs-20230309-green?style=flat-square" alt="Website" href="https://iamai.retrofor.space" target="_blank"/>
-    <img src="https://img.shields.io/badge/playgroud-live-green?style=flat-square" alt="Website" href="https://playground.retrofor.space/iamai" target="_blank"/>
+<a style="text-decoration:none" href="https://iamai.retrofor.space" target="_blank">
+    <img src="https://img.shields.io/badge/docs-iamai.retrofor.space-yellow?style=flat-square" alt="Website">
+</a>
+  <a style="text-decoration:none" href="https://playground.retrofor.space/iamai" target="_blank">
+    <img src="https://img.shields.io/badge/playgroud-Under construction-cyan?style=flat-square" alt="Website">
+    </a>
   <br>
   <a href="https://pypi.python.org/pypi/iamai">
     <img src="https://img.shields.io/pypi/v/iamai?style=flat-square" alt="pypi">
   </a>
   <img src="https://img.shields.io/badge/python-3.8+-blue?style=flat-square" alt="python">
   <br>
   <img src="https://results.pre-commit.ci/badge/github/retrofor/iamai/main.svg">
   <br>
     <a style="text-decoration:none" href="https://www.codacy.com/gh/retrofor/iamai/dashboard?utm_source=github.com&utm_medium=referral&utm_content=retrofor/iamai&utm_campaign=Badge_Gradee" target="_blank">
     <img src="https://app.codacy.com/project/badge/Grade/f3611d85db764236b65fac956bdb53df" alt="Codacy Badge" />
   </a>
+    <img src="https://img.shields.io/badge/code_style-black-000000.svg?style=flat-square" alt="Codacy Badge" />
 </p>
 <p align="center">
 </p>
 <p align="center">
 <!-- onebot -->
   <a style="text-decoration:none" href="https://onebot.dev" target="_blank">
     <img src="https://img.shields.io/badge/-Onebot%2011-000020?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAHAAAABwCAMAAADxPgR5AAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAAAxQTFRF////29vbr6+vAAAAk1hCcwAAAAR0Uk5T////AEAqqfQAAAKcSURBVHja7NrbctswDATQXfD//zlpO7FlmwAWIOnOtNaTM5JwDMa8E+PNFz7g3waJ24fviyDPgfhz8fHP39cBcBL9KoJbQUxjA2iYqHL3FAnvzhL4GtVNUcoSZe6eSHizBcK5LL7dBr2AUZlev1ARRHCljzRALIEog6H3U6bCIyqIZdAT0eBuJYaGiJaHSjmkYIZd+qSGWAQnIaz2OArVnX6vrItQvbhZJtVGB5qX9wKqCMkb9W7aexfCO/rwQRBzsDIsYx4AOz0nhAtWu7bqkEQBO0Pr+Ftjt5fFCUEbm0Sbgdu8WSgJ5NgH2iu46R/o1UcBXJsFusWF/QUaz3RwJMEgngfaGGdSxJkE/Yg4lOBryBiMwvAhZrVMUUvwqU7F05b5WLaUIN4M4hRocQQRnEedgsn7TZB3UCpRrIJwQfqvGwsg18EnI2uSVNC8t+0QmMXogvbPg/xk+Mnw/6kW/rraUlvqgmFreAA09xW5t0AFlHrQZ3CsgvZm0FbHNKyBmheBKIF2cCA8A600aHPmFtRB1XvMsJAiza7LpPog0UJwccKdzw8rdf8MyN2ePYF896LC5hTzdZqxb6VNXInaupARLDNBWgI8spq4T0Qb5H4vWfPmHo8OyB1ito+AysNNz0oglj1U955sjUN9d41LnrX2D/u7eRwxyOaOpfyevCWbTgDEoilsOnu7zsKhjRCsnD/QzhdkYLBLXjiK4f3UWmcx2M7PO21CKVTH84638NTplt6JIQH0ZwCNuiWAfvuLhdrcOYPVO9eW3A67l7hZtgaY9GZo9AFc6cryjoeFBIWeU+npnk/nLE0OxCHL1eQsc1IciehjpJv5mqCsjeopaH6r15/MrxNnVhu7tmcslay2gO2Z1QfcfX0JMACG41/u0RrI9QAAAABJRU5ErkJggg==&logoColor=white" alt="onebotv11" />
+    </a>
     <!-- github -->
-    <img src="https://img.shields.io/badge/-github-181717?style=flat-square&logo=github&logoColor=white">
+    <!-- <img src="https://img.shields.io/badge/-github-181717?style=flat-square&logo=github&logoColor=white"> -->
     <!-- discord -->
-    <img src="https://img.shields.io/badge/-Discord-5865F2?style=flat-square&logo=Discord&logoColor=white">
-    <br>
+    <!-- <img src="https://img.shields.io/badge/-Discord-5865F2?style=flat-square&logo=Discord&logoColor=white"> -->
+    <!-- <br> -->
     <!-- bilibili live -->
-    <img src="https://img.shields.io/badge/-BiliBili Live-00A1D6?style=flat-square&logo=Bilibili&logoColor=white">
+    <!-- <img src="https://img.shields.io/badge/-BiliBili Live-00A1D6?style=flat-square&logo=Bilibili&logoColor=white"> -->
     <!-- mirai-api-http -->
     <img src="https://img.shields.io/badge/-Mirai%20api%20http%202.3+-00B8AA?style=flat-square">
     <!-- dingtalk -->
     <img src="https://img.shields.io/badge/-DingTalk-blue?style=flat-square">
     <!-- qqzone -->
-    <img src="https://img.shields.io/badge/-QQ%20Zone-FECC00?style=flat-square&logo=Tencent QQ&logoColor=black">
-    <br>
+    <!-- <img src="https://img.shields.io/badge/-QQ%20Zone-FECC00?style=flat-square&logo=Tencent QQ&logoColor=black"> -->
+    <!-- <br> -->
     <!-- minecraft -->
-    <img src="https://img.shields.io/badge/-Minecraft Server-62B47A?style=flat-square&logo=Minecraft&logoColor=white">
+    <!-- <img src="https://img.shields.io/badge/-Minecraft Server-62B47A?style=flat-square&logo=Minecraft&logoColor=white"> -->
     <!-- twitter -->
-    <img src="https://img.shields.io/badge/-Twitter-1DA1F2?style=flat-square&logo=twitter&logoColor=white">
+    <!-- <img src="https://img.shields.io/badge/-Twitter-1DA1F2?style=flat-square&logo=twitter&logoColor=white"> -->
     <!-- console -->
     <img src="https://img.shields.io/badge/-Console-4EAA25?style=flat-square&logo=GNU bash&logoColor=white">
     <!-- wechat -->
-    <img src="https://img.shields.io/badge/-Wechat-07C160?style=flat-square&logo=wechat&logoColor=white">
+    <!-- <img src="https://img.shields.io/badge/-Wechat-07C160?style=flat-square&logo=wechat&logoColor=white"> -->
     <!-- tg -->
-    <img src="https://img.shields.io/badge/-Telegram-26A5E4?style=flat-square&logo=telegram&logoColor=white">
+    <!-- <img src="https://img.shields.io/badge/-Telegram-26A5E4?style=flat-square&logo=telegram&logoColor=white"> -->
   </a>
 </p>
 <p align="center">
 </p>
 <p align="center">
   <img src="https://img.shields.io/github/forks/retrofor/iamai?style=social" >
   <img src="https://img.shields.io/github/stars/retrofor/iamai?style=social" >
@@ -116,34 +122,49 @@
 ## 🚀 Features
 
 - 🎪 **Interactive [docs](https://iamai.retrofor.space) &amp; [demos](https://iamai.retrofor.space/demos)**
 - 🕶 **Seamless migration**: Works for **both** [Rasa]() and [GPT]() and more...
 - ⚡ **Fully tree shakeable**: Only take what you want, [bundle size](https://iamai.retrofor.space/export-size)
 - 🔩 **Flexible**: Configurable event filters and targets
 - 🔌 **Optional [Add-ons](https://iamai.retrofor.space/add-ons)**: [Apscheduler](https://iamai.retrofor.space/add-ons/apscheduler), etc.
-- 👍 **Cross-platform**: [Onebot](https://iamai.retrofor.space/adapters/onebot), [Wechat](https://iamai.retrofor.space/adapters/wechat), [Twitter](https://iamai.retrofor.space/adapters/twitter), [Bilibili](https://iamai.retrofor.space/adapters/bilibili), [Github](https://iamai.retrofor.space/adapters/github), etc.
+- 👍 **Cross-platform**: [cqhttp](https://iamai.retrofor.space/guide/cqhttp-adapter.html), [dingtalk](https://iamai.retrofor.space/guide/dingtalk-adapter.html), [Mirai](https://iamai.retrofor.space/guide/mirai-adapter.html) etc.
 
 <p align="center"><img width="512" src="https://iamai.retrofor.space/icons/retro_plus.png"></p>
 
 ## ⬇️ Install
 
+### FrameWork
+
 - STABLE VERSION
 
   ```sh
   pip install iamai
   ```
 
 or you can also install for TEST.
 
 - TEST VERSION
 
   ```sh
-  pip install -i https://test.pypi.org/simple/ iamai
+  git clone https://github.com/retrofor/iamai.git
+  cd iamai
+  poetry install --no-dev  # 推荐
+  pip install .  # 不推荐
   ```
 
+### Adapters
+
+iamai itself is just a chatbot framework and additional protocol adapters are required to support specific protocols. You can use pip to install the protocol adapter:
+
+```py
+pip install iamai-adapter-cqhttp
+pip install iamai-adapter-mirai
+pip install iamai-adapter-dingtalk
+```
+
 ## ❗ Usage
 
 firstly, you need to load an adapter.
 
 ```python
 from iamai import Bot
 
@@ -151,15 +172,15 @@
 bot.load_adapters("iamai.adapter.cqhttp")
 
 bot.run()
 ```
 
 then, you need load the transformer and use your models.
 
-**transformer(Use from the 🤗/transformers library)**
+### transformer(Use from the 🤗/transformers library)
 
 ```python
 from transformers import AutoModelWithLMHead, AutoTokenizer
 # load models
 model = AutoModelWithLMHead.from_pretrained("gpt2")
 # load tokenizer
 tokenizer = AutoTokenizer.from_pretrained("gpt2")
@@ -173,15 +194,15 @@
 
 You can use pre-built optimizers to speed up the model inference process, or you can write your own optimizer. However, it's important to note that the transformer model optimizer is a special type of optimizer that is designed specifically for optimizing parameters in transformer models, thereby improving their performance.
 
 To write a transformer model optimizer, you need to have an understanding of how optimizers work and be familiar with the structure of transformer models.
 
 The principle of optimizers can be referred to in the paper [&#34;Attention Is All You Need&#34;](https://arxiv.org/abs/1706.03762), and the structure of transformer models can be referred to in the paper [&#34;Transformer: A Novel Neural Network Architecture for Language Understanding&#34;](https://ai.googleblog.com/2017/08/transformer-novel-neural-network.html?m=1). The implementation of optimizers can be referred to in the [AdamW optimizer](https://huggingface.co/transformers/v3.0.2/main_classes/optimizer_schedules.html) in the Hugging Face Transformers library.
 
-**Use the Inference API**
+### Use the Inference API
 
 ```python
 import requests
 
 API_URL = "https://api-inference.huggingface.co/models/xxx/xxxxx"
 headers = {"Authorization": "Bearer xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"}
 
@@ -195,16 +216,15 @@
 ```
 
 ## 👀 See the docs
 
 > choices below.
 
 - [https://iamai.retrofor.space](https://iamai.retrofor.space) _(recommend)_
-- [https://iamai-docs-git-main-retrofor.vercel.app](https://iamai-docs-git-main-retrofor.vercel.app)
-- ~~[https://iamai-docs-retrofor.vercel.app/](https://iamai-docs-retrofor.vercel.app/)~~
+- [retrofor.github.io/iamai](https://retrofor.github.io/iamai)
 
 ## ✨ Project Activity
 
 ![Alt](https://repobeats.axiom.co/api/embed/cc9b8bded331c406e68cc0c7c294ef04122d6da2.svg "Repobeats analytics image")
 
 ## 👨‍🚀 Contributors
```

#### html2text {}

```diff
@@ -1,76 +1,69 @@
-Metadata-Version: 2.1 Name: iamai Version: 3.14.4 Summary: bot framework. Home-
-page: https://retrofor.space/ License: MIT Keywords: bot,qq,qqbot,mirai,coolq
-Author: ç®å¾çº¯ Author-email: admin@jyunko.cn Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 5 - Production/Stable Classifier: Framework
-:: Robot Framework Classifier: Framework :: Robot Framework :: Library
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3 Provides-Extra: all Provides-Extra: apscheduler Provides-Extra:
-cqhttp Provides-Extra: dingtalk Provides-Extra: hot-reload Requires-Dist:
-aiohttp (>=3.8.0,<4.0.0) Requires-Dist: loguru (>=0.6.0,<0.7.0) Requires-Dist:
-pydantic (>=1.10.0,<2.0.0) Requires-Dist: tomli (>=2.0.0,<3.0.0) ;
-python_version < "3.11" Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
-Project-URL: Documentation, https://iamai.retrofor.space/ Project-URL:
-Repository, https://github.com/retrofor/iamai Description-Content-Type: text/
-markdown
+Metadata-Version: 2.1 Name: iamai Version: 3.14.4.post1 Summary: bot framework.
+Home-page: https://retrofor.space/ License: MIT Keywords:
+bot,qq,qqbot,mirai,coolq Author: ç®å¾çº¯ Author-email: admin@jyunko.cn
+Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 5 - Production/
+Stable Classifier: Framework :: Robot Framework Classifier: Framework :: Robot
+Framework :: Library Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3 Provides-Extra: all Provides-Extra:
+apscheduler Provides-Extra: cqhttp Provides-Extra: dingtalk Provides-Extra:
+hot-reload Requires-Dist: aiohttp (>=3.8.0,<4.0.0) Requires-Dist: loguru
+(>=0.6.0,<0.7.0) Requires-Dist: pydantic (>=1.10.0,<2.0.0) Requires-Dist: tomli
+(>=2.0.0,<3.0.0) ; python_version < "3.11" Requires-Dist: typing-extensions
+(>=4.4.0,<5.0.0) Project-URL: Documentation, https://iamai.retrofor.space/
+Project-URL: Repository, https://github.com/retrofor/iamai Description-Content-
+Type: text/markdown
                    [https://iamai.retrofor.space/retro.png]
                               ****** iamai ******
                                [Discord] [QQç¾¤]
                       ç®ä½ä¸­æ ã«ã»ãã íêµ­ì´
             Cross-platform robot framework, mainly used for ML/DL.
                              [Website] [Website]
                                [pypi] [python]
      [https://results.pre-commit.ci/badge/github/retrofor/iamai/main.svg]
-                                [Codacy_Badge]
-     [onebotv11]__[https://img.shields.io/badge/-github-181717?style=flat-
- square&logo=github&logoColor=white]__[https://img.shields.io/badge/-Discord-
-            5865F2?style=flat-square&logo=Discord&logoColor=white]_
-       _[https://img.shields.io/badge/-BiliBili_Live-00A1D6?style=flat-
-    square&logo=Bilibili&logoColor=white]__[https://img.shields.io/badge/-
- Mirai%20api%20http%202.3+-00B8AA?style=flat-square]__[https://img.shields.io/
-   badge/-DingTalk-blue?style=flat-square]__[https://img.shields.io/badge/-
-     QQ%20Zone-FECC00?style=flat-square&logo=Tencent_QQ&logoColor=black]_
-      _[https://img.shields.io/badge/-Minecraft_Server-62B47A?style=flat-
-square&logo=Minecraft&logoColor=white]__[https://img.shields.io/badge/-Twitter-
-       1DA1F2?style=flat-square&logo=twitter&logoColor=white]__[https://
-        img.shields.io/badge/-Console-4EAA25?style=flat-square&logo=GNU
-bash&logoColor=white]__[https://img.shields.io/badge/-Wechat-07C160?style=flat-
- square&logo=wechat&logoColor=white]__[https://img.shields.io/badge/-Telegram-
-            26A5E4?style=flat-square&logo=telegram&logoColor=white]
+                         [Codacy_Badge] [Codacy Badge]
+ [onebotv11]         [https://img.shields.io/badge/-Mirai%20api%20http%202.3+-
+      00B8AA?style=flat-square]  [https://img.shields.io/badge/-DingTalk-
+    blue?style=flat-square]         [https://img.shields.io/badge/-Console-
+          4EAA25?style=flat-square&logo=GNU bash&logoColor=white]
   [https://img.shields.io/github/forks/retrofor/iamai?style=social] [https://
            img.shields.io/github/stars/retrofor/iamai?style=social]
 [https://img.shields.io/github/watchers/retrofor/iamai?style=social] [https://
         img.shields.io/github/search/retrofor/iamai/goto?style=social]
 [https://img.shields.io/github/repo-size/retrofor/iamai?style=social] [https://
        img.shields.io/github/languages/top/retrofor/iamai?style=social]
 ## ð Introduction A Cross-platform robot framework, mainly used for machine
 learning. ## ð Features - ðª **Interactive [docs](https://
 iamai.retrofor.space) & [demos](https://iamai.retrofor.space/demos)** - ð¶
 **Seamless migration**: Works for **both** [Rasa]() and [GPT]() and more... -
 â¡ **Fully tree shakeable**: Only take what you want, [bundle size](https://
 iamai.retrofor.space/export-size) - ð© **Flexible**: Configurable event
 filters and targets - ð **Optional [Add-ons](https://iamai.retrofor.space/
 add-ons)**: [Apscheduler](https://iamai.retrofor.space/add-ons/apscheduler),
-etc. - ð **Cross-platform**: [Onebot](https://iamai.retrofor.space/adapters/
-onebot), [Wechat](https://iamai.retrofor.space/adapters/wechat), [Twitter]
-(https://iamai.retrofor.space/adapters/twitter), [Bilibili](https://
-iamai.retrofor.space/adapters/bilibili), [Github](https://iamai.retrofor.space/
-adapters/github), etc.
+etc. - ð **Cross-platform**: [cqhttp](https://iamai.retrofor.space/guide/
+cqhttp-adapter.html), [dingtalk](https://iamai.retrofor.space/guide/dingtalk-
+adapter.html), [Mirai](https://iamai.retrofor.space/guide/mirai-adapter.html)
+etc.
               [https://iamai.retrofor.space/icons/retro_plus.png]
-## â¬ï¸ Install - STABLE VERSION ```sh pip install iamai ``` or you can also
-install for TEST. - TEST VERSION ```sh pip install -i https://test.pypi.org/
-simple/ iamai ``` ## â Usage firstly, you need to load an adapter. ```python
-from iamai import Bot bot = Bot() bot.load_adapters("iamai.adapter.cqhttp")
-bot.run() ``` then, you need load the transformer and use your models.
-**transformer(Use from the ð¤/transformers library)** ```python from
-transformers import AutoModelWithLMHead, AutoTokenizer # load models model =
+## â¬ï¸ Install ### FrameWork - STABLE VERSION ```sh pip install iamai ``` or
+you can also install for TEST. - TEST VERSION ```sh git clone https://
+github.com/retrofor/iamai.git cd iamai poetry install --no-dev # æ¨è pip
+install . # ä¸æ¨è ``` ### Adapters iamai itself is just a chatbot framework
+and additional protocol adapters are required to support specific protocols.
+You can use pip to install the protocol adapter: ```py pip install iamai-
+adapter-cqhttp pip install iamai-adapter-mirai pip install iamai-adapter-
+dingtalk ``` ## â Usage firstly, you need to load an adapter. ```python from
+iamai import Bot bot = Bot() bot.load_adapters("iamai.adapter.cqhttp") bot.run
+() ``` then, you need load the transformer and use your models. ### transformer
+(Use from the ð¤/transformers library) ```python from transformers import
+AutoModelWithLMHead, AutoTokenizer # load models model =
 AutoModelWithLMHead.from_pretrained("gpt2") # load tokenizer tokenizer =
 AutoTokenizer.from_pretrained("gpt2") # transfor the text to token input_ids =
 tokenizer.encode("Hello, my name is IamAI!", add_special_tokens=True) # input
 the token to the models outputs = model.generate(input_ids) # get the text
 generated generated_text = tokenizer.decode(outputs[0]) ``` You can use pre-
 built optimizers to speed up the model inference process, or you can write your
 own optimizer. However, it's important to note that the transformer model
@@ -81,22 +74,20 @@
 transformer models. The principle of optimizers can be referred to in the paper
 ["Attention Is All You Need"](https://arxiv.org/abs/1706.03762), and the
 structure of transformer models can be referred to in the paper ["Transformer:
 A Novel Neural Network Architecture for Language Understanding"](https://
 ai.googleblog.com/2017/08/transformer-novel-neural-network.html?m=1). The
 implementation of optimizers can be referred to in the [AdamW optimizer](https:
 //huggingface.co/transformers/v3.0.2/main_classes/optimizer_schedules.html) in
-the Hugging Face Transformers library. **Use the Inference API** ```python
+the Hugging Face Transformers library. ### Use the Inference API ```python
 import requests API_URL = "https://api-inference.huggingface.co/models/xxx/
 xxxxx" headers = {"Authorization": "Bearer
 xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"} def query(payload): response =
 requests.post(API_URL, headers=headers, json=payload) return response.json()
 output = query({ "inputs": "xxx", }) ``` ## ð See the docs > choices below.
 - [https://iamai.retrofor.space](https://iamai.retrofor.space) _(recommend)_ -
-[https://iamai-docs-git-main-retrofor.vercel.app](https://iamai-docs-git-main-
-retrofor.vercel.app) - ~~[https://iamai-docs-retrofor.vercel.app/](https://
-iamai-docs-retrofor.vercel.app/)~~ ## â¨ Project Activity ![Alt](https://
-repobeats.axiom.co/api/embed/cc9b8bded331c406e68cc0c7c294ef04122d6da2.svg
-"Repobeats analytics image") ## ð¨âð Contributors [https://
-contrib.rocks/image?repo=retrofor/iamai] ## ð License [MIT](https://
-github.com/retrofor/iamai/blob/main/LICENSE) Â© 2023-PRESENT [ç®å¾çº¯](https:
-//github.com/HsiangNianian)
+[retrofor.github.io/iamai](https://retrofor.github.io/iamai) ## â¨ Project
+Activity ![Alt](https://repobeats.axiom.co/api/embed/
+cc9b8bded331c406e68cc0c7c294ef04122d6da2.svg "Repobeats analytics image") ##
+ð¨âð Contributors [https://contrib.rocks/image?repo=retrofor/iamai] ##
+ð License [MIT](https://github.com/retrofor/iamai/blob/main/LICENSE) Â©
+2023-PRESENT [ç®å¾çº¯](https://github.com/HsiangNianian)
```

