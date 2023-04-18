# Comparing `tmp/nonebot_plugin_sdgpt-0.2.5.tar.gz` & `tmp/nonebot_plugin_sdgpt-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sdgpt-0.2.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_sdgpt-0.2.6.tar", max compression
```

## Comparing `nonebot_plugin_sdgpt-0.2.5.tar` & `nonebot_plugin_sdgpt-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot_plugin_sdgpt-0.2.5/LICENSE
--rw-r--r--   0        0        0     9513 2023-04-15 12:01:31.983393 nonebot_plugin_sdgpt-0.2.5/nonebot_plugin_SDGPT/__init__.py
--rw-r--r--   0        0        0     6288 2023-04-15 11:16:16.354928 nonebot_plugin_sdgpt-0.2.5/nonebot_plugin_SDGPT/bot.py
--rw-r--r--   0        0        0     6542 2023-04-15 05:42:39.006444 nonebot_plugin_sdgpt-0.2.5/nonebot_plugin_SDGPT/config.py
--rw-r--r--   0        0        0     5386 2023-04-15 06:18:07.002772 nonebot_plugin_sdgpt-0.2.5/nonebot_plugin_SDGPT/configspec.ini
--rw-r--r--   0        0        0      242 2023-04-15 04:34:57.487801 nonebot_plugin_sdgpt-0.2.5/nonebot_plugin_SDGPT/lib/base.py
--rw-r--r--   0        0        0     3028 2023-04-15 05:33:13.203719 nonebot_plugin_sdgpt-0.2.5/nonebot_plugin_SDGPT/lib/check.py
--rw-r--r--   0        0        0      487 2023-04-13 00:23:27.760154 nonebot_plugin_sdgpt-0.2.5/nonebot_plugin_SDGPT/lib/cons.py
--rw-r--r--   0        0        0     2003 2023-04-11 23:52:10.103729 nonebot_plugin_sdgpt-0.2.5/nonebot_plugin_SDGPT/lib/logger.py
--rw-r--r--   0        0        0      125 2023-04-15 05:54:10.530836 nonebot_plugin_sdgpt-0.2.5/nonebot_plugin_SDGPT/lib/test.py
--rw-r--r--   0        0        0     2393 2023-04-15 11:40:17.448644 nonebot_plugin_sdgpt-0.2.5/nonebot_plugin_SDGPT/lib/utils.py
--rw-r--r--   0        0        0     1187 2023-04-15 12:02:52.235575 nonebot_plugin_sdgpt-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1066 2023-04-15 04:38:37.455109 nonebot_plugin_sdgpt-0.2.5/README.md
--rw-r--r--   0        0        0     2360 1970-01-01 00:00:00.000000 nonebot_plugin_sdgpt-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot_plugin_sdgpt-0.2.6/LICENSE
+-rw-r--r--   0        0        0     9513 2023-04-15 12:01:31.983393 nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/__init__.py
+-rw-r--r--   0        0        0     6527 2023-04-16 02:11:34.504831 nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/bot.py
+-rw-r--r--   0        0        0     6540 2023-04-16 01:58:27.689226 nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/config.py
+-rw-r--r--   0        0        0     5386 2023-04-15 06:18:07.002772 nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/configspec.ini
+-rw-r--r--   0        0        0      242 2023-04-15 04:34:57.487801 nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/lib/base.py
+-rw-r--r--   0        0        0     3028 2023-04-15 05:33:13.203719 nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/lib/check.py
+-rw-r--r--   0        0        0      487 2023-04-13 00:23:27.760154 nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/lib/cons.py
+-rw-r--r--   0        0        0     2003 2023-04-11 23:52:10.103729 nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/lib/logger.py
+-rw-r--r--   0        0        0     6369 2023-04-16 02:08:54.526672 nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/lib/test.py
+-rw-r--r--   0        0        0     2393 2023-04-15 11:40:17.448644 nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/lib/utils.py
+-rw-r--r--   0        0        0     1206 2023-04-18 02:39:12.264217 nonebot_plugin_sdgpt-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1066 2023-04-15 04:38:37.455109 nonebot_plugin_sdgpt-0.2.6/README.md
+-rw-r--r--   0        0        0     2417 1970-01-01 00:00:00.000000 nonebot_plugin_sdgpt-0.2.6/PKG-INFO
```

### Comparing `nonebot_plugin_sdgpt-0.2.5/LICENSE` & `nonebot_plugin_sdgpt-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.5/nonebot_plugin_SDGPT/__init__.py` & `nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.5/nonebot_plugin_SDGPT/bot.py` & `nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,19 @@
         switchModel(chatgpt, 'chatgpt-api', config['runtime']['chatgpt_api_model'])
         out = await chatgpt_api.ask_async(message)
         return out
     if bot == 'bing':
         async with L_bing:
             if len(prompt) > 1: message = promptBase + message
             out = await bing.ask(message, conversation_style=config['runtime']['bing_model'])
+            if out['tiem']['messages'][-1]['author'] != 'bot':
+                bot.reset()
+                out = await bing.ask(message, conversation_style=config['runtime']['bing_model'])
             out = out['item']['messages'][-1]['text']
+            out = re.sub(r'\[\^\d\^]','',out)
             return out
     if bot == 'poe':
         async with L_poe:
             if len(prompt) > 1: message = promptBase + message
             for chunk in poe.send_message(config['runtime']['poe_models'][config['runtime']['poe_model']], message):
                 pass
             out = chunk["text"]
```

### Comparing `nonebot_plugin_sdgpt-0.2.5/nonebot_plugin_SDGPT/config.py` & `nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,14 @@
         return ''
     else:
         add = ''
         try:
             with open(DIR['cookies_file_path'], 'r') as f:
                 cookies = json.load(f)
                 bot = Bing(cookies=cookies)
-
             proxy = Proxy(DIR)
             model = Model(DIR)
             if proxy:
                 bot.proxy = proxy
                 add += f',代理: {proxy}'
             if model:
                 outData['cfg']['runtime']['bing_model'] = model
```

### Comparing `nonebot_plugin_sdgpt-0.2.5/nonebot_plugin_SDGPT/configspec.ini` & `nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/configspec.ini`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.5/nonebot_plugin_SDGPT/lib/check.py` & `nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/lib/check.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.5/nonebot_plugin_SDGPT/lib/logger.py` & `nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/lib/logger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.5/nonebot_plugin_SDGPT/lib/utils.py` & `nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/lib/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.5/pyproject.toml` & `nonebot_plugin_sdgpt-0.2.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-SDGPT"
-version = "0.2.5"
+version = "0.2.6"
 description = "ChatBot for NoneBot : 链接 ChatGPT / Bing / Poe / Stable-Diffusion : ChatGPT Bing poe聊天, gpt解析自然语言转Stable-Diffusion生成图像"
 license = "MIT"
 authors = ["F_thx <thx1140093097@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/thx114/SDGPT"
 repository = "https://github.com/thx114/SDGPT"
 documentation = "https://github.com/thx114/SDGPTreadme"
@@ -16,23 +16,23 @@
 ]
 
 [tool.poetry.dependencies]
 
 python = "^3.8"
 nonebot2 = "^2.0.0-beta.1"
 python-dotenv = "*"
-revChatGPT = "*"
-EdgeGPT = "*"
+revChatGPT = "^4.2.3"
+EdgeGPT = "^0.1.25.1"
 webuiapi = "*"
 nonebot-plugin-guild-patch ="*"
 nonebot-adapter-onebot = { version = "^2.0.0-beta.1", optional = true }
 websockets = "^10.0"
 aiofiles = "*"
 configobj = "*"
-poe-api = "*"
+poe-api = "^0.2.12"
 
 
 [tool.poetry.extras]
 onebot = ["nonebot-adapter-onebot"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `nonebot_plugin_sdgpt-0.2.5/README.md` & `nonebot_plugin_sdgpt-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.5/PKG-INFO` & `nonebot_plugin_sdgpt-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sdgpt
-Version: 0.2.5
+Version: 0.2.6
 Summary: ChatBot for NoneBot : 链接 ChatGPT / Bing / Poe / Stable-Diffusion : ChatGPT Bing poe聊天, gpt解析自然语言转Stable-Diffusion生成图像
 Home-page: https://github.com/thx114/SDGPT
 License: MIT
 Keywords: nonebot,nonebot2,chatgpt,new bing,Stable-Diffusion
 Author: F_thx
 Author-email: thx1140093097@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: onebot
-Requires-Dist: EdgeGPT
+Requires-Dist: EdgeGPT (>=0.1.25.1,<0.2.0.0)
 Requires-Dist: aiofiles
 Requires-Dist: configobj
 Requires-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1,<3.0.0) ; extra == "onebot"
 Requires-Dist: nonebot-plugin-guild-patch
 Requires-Dist: nonebot2 (>=2.0.0-beta.1,<3.0.0)
-Requires-Dist: poe-api
+Requires-Dist: poe-api (>=0.2.12,<0.3.0)
 Requires-Dist: python-dotenv
-Requires-Dist: revChatGPT
+Requires-Dist: revChatGPT (>=4.2.3,<5.0.0)
 Requires-Dist: websockets (>=10.0,<11.0)
 Requires-Dist: webuiapi
 Project-URL: Documentation, https://github.com/thx114/SDGPTreadme
 Project-URL: Repository, https://github.com/thx114/SDGPT
 Description-Content-Type: text/markdown
 
 # SDGPT
```

