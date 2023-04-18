# Comparing `tmp/nonebot_plugin_sdgpt-0.2.6.tar.gz` & `tmp/nonebot_plugin_sdgpt-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sdgpt-0.2.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_sdgpt-0.2.7.tar", max compression
```

## Comparing `nonebot_plugin_sdgpt-0.2.6.tar` & `nonebot_plugin_sdgpt-0.2.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot_plugin_sdgpt-0.2.6/LICENSE
--rw-r--r--   0        0        0     9513 2023-04-15 12:01:31.983393 nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/__init__.py
--rw-r--r--   0        0        0     6527 2023-04-16 02:11:34.504831 nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/bot.py
--rw-r--r--   0        0        0     6540 2023-04-16 01:58:27.689226 nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/config.py
--rw-r--r--   0        0        0     5386 2023-04-15 06:18:07.002772 nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/configspec.ini
--rw-r--r--   0        0        0      242 2023-04-15 04:34:57.487801 nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/lib/base.py
--rw-r--r--   0        0        0     3028 2023-04-15 05:33:13.203719 nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/lib/check.py
--rw-r--r--   0        0        0      487 2023-04-13 00:23:27.760154 nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/lib/cons.py
--rw-r--r--   0        0        0     2003 2023-04-11 23:52:10.103729 nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/lib/logger.py
--rw-r--r--   0        0        0     6369 2023-04-16 02:08:54.526672 nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/lib/test.py
--rw-r--r--   0        0        0     2393 2023-04-15 11:40:17.448644 nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/lib/utils.py
--rw-r--r--   0        0        0     1206 2023-04-18 02:39:12.264217 nonebot_plugin_sdgpt-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1066 2023-04-15 04:38:37.455109 nonebot_plugin_sdgpt-0.2.6/README.md
--rw-r--r--   0        0        0     2417 1970-01-01 00:00:00.000000 nonebot_plugin_sdgpt-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot_plugin_sdgpt-0.2.7/LICENSE
+-rw-r--r--   0        0        0     9513 2023-04-15 12:01:31.983393 nonebot_plugin_sdgpt-0.2.7/nonebot_plugin_SDGPT/__init__.py
+-rw-r--r--   0        0        0     6527 2023-04-16 02:11:34.504831 nonebot_plugin_sdgpt-0.2.7/nonebot_plugin_SDGPT/bot.py
+-rw-r--r--   0        0        0     6591 2023-04-18 02:58:18.734254 nonebot_plugin_sdgpt-0.2.7/nonebot_plugin_SDGPT/config.py
+-rw-r--r--   0        0        0     5386 2023-04-15 06:18:07.002772 nonebot_plugin_sdgpt-0.2.7/nonebot_plugin_SDGPT/configspec.ini
+-rw-r--r--   0        0        0      242 2023-04-15 04:34:57.487801 nonebot_plugin_sdgpt-0.2.7/nonebot_plugin_SDGPT/lib/base.py
+-rw-r--r--   0        0        0     3028 2023-04-15 05:33:13.203719 nonebot_plugin_sdgpt-0.2.7/nonebot_plugin_SDGPT/lib/check.py
+-rw-r--r--   0        0        0      487 2023-04-13 00:23:27.760154 nonebot_plugin_sdgpt-0.2.7/nonebot_plugin_SDGPT/lib/cons.py
+-rw-r--r--   0        0        0     2003 2023-04-11 23:52:10.103729 nonebot_plugin_sdgpt-0.2.7/nonebot_plugin_SDGPT/lib/logger.py
+-rw-r--r--   0        0        0     6369 2023-04-16 02:08:54.526672 nonebot_plugin_sdgpt-0.2.7/nonebot_plugin_SDGPT/lib/test.py
+-rw-r--r--   0        0        0     2393 2023-04-15 11:40:17.448644 nonebot_plugin_sdgpt-0.2.7/nonebot_plugin_SDGPT/lib/utils.py
+-rw-r--r--   0        0        0     1206 2023-04-18 03:02:52.244410 nonebot_plugin_sdgpt-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1066 2023-04-15 04:38:37.455109 nonebot_plugin_sdgpt-0.2.7/README.md
+-rw-r--r--   0        0        0     2417 1970-01-01 00:00:00.000000 nonebot_plugin_sdgpt-0.2.7/PKG-INFO
```

### Comparing `nonebot_plugin_sdgpt-0.2.6/LICENSE` & `nonebot_plugin_sdgpt-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/__init__.py` & `nonebot_plugin_sdgpt-0.2.7/nonebot_plugin_SDGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/bot.py` & `nonebot_plugin_sdgpt-0.2.7/nonebot_plugin_SDGPT/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/config.py` & `nonebot_plugin_sdgpt-0.2.7/nonebot_plugin_SDGPT/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,27 +108,28 @@
 
 async def load_poe(DIR, outData):
     if not DIR['token'] or DIR['token'] == '':
         warn('配置检查', f'你设定的 Poe 的 token 为空，跳过载入')
         return ''
     else:
         add = ''
-        bot = poe.Client(token=DIR['token'])
-        bots = bot.bot_names
         proxy = Proxy(DIR)
         model = Model(DIR)
         models = ['Sage',
                   'GPT-4',
                   'Claude+',
                   'Claude-instant',
                   'ChatGPT',
                   'Dragonfly']
         if proxy:
-            bot.proxy = proxy
             add += f',代理: {proxy}'
+            bot = poe.Client(token=DIR['token'], proxy=proxy)
+        else:
+            bot = poe.Client(token=DIR['token'])
+        bots = bot.bot_names
         if model:
             models = list(bots.values())
             if model in models:
                 outData['cfg']['runtime']['poe_model'] = model
                 outData['cfg']['runtime']['poe_models'] = {value: key for key, value in bots.items()}
                 add += f',模型: {model}'
         suc('poe', f'Poe: 已加载{add}')
```

### Comparing `nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/configspec.ini` & `nonebot_plugin_sdgpt-0.2.7/nonebot_plugin_SDGPT/configspec.ini`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/lib/check.py` & `nonebot_plugin_sdgpt-0.2.7/nonebot_plugin_SDGPT/lib/check.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/lib/logger.py` & `nonebot_plugin_sdgpt-0.2.7/nonebot_plugin_SDGPT/lib/logger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/lib/test.py` & `nonebot_plugin_sdgpt-0.2.7/nonebot_plugin_SDGPT/lib/test.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.6/nonebot_plugin_SDGPT/lib/utils.py` & `nonebot_plugin_sdgpt-0.2.7/nonebot_plugin_SDGPT/lib/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.6/pyproject.toml` & `nonebot_plugin_sdgpt-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-SDGPT"
-version = "0.2.6"
+version = "0.2.7"
 description = "ChatBot for NoneBot : 链接 ChatGPT / Bing / Poe / Stable-Diffusion : ChatGPT Bing poe聊天, gpt解析自然语言转Stable-Diffusion生成图像"
 license = "MIT"
 authors = ["F_thx <thx1140093097@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/thx114/SDGPT"
 repository = "https://github.com/thx114/SDGPT"
 documentation = "https://github.com/thx114/SDGPTreadme"
```

### Comparing `nonebot_plugin_sdgpt-0.2.6/README.md` & `nonebot_plugin_sdgpt-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.6/PKG-INFO` & `nonebot_plugin_sdgpt-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sdgpt
-Version: 0.2.6
+Version: 0.2.7
 Summary: ChatBot for NoneBot : 链接 ChatGPT / Bing / Poe / Stable-Diffusion : ChatGPT Bing poe聊天, gpt解析自然语言转Stable-Diffusion生成图像
 Home-page: https://github.com/thx114/SDGPT
 License: MIT
 Keywords: nonebot,nonebot2,chatgpt,new bing,Stable-Diffusion
 Author: F_thx
 Author-email: thx1140093097@gmail.com
 Requires-Python: >=3.8,<4.0
```

