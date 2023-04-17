# Comparing `tmp/telegram_bottools-0.1.2.tar.gz` & `tmp/telegram_bottools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_bottools-0.1.2.tar", max compression
+gzip compressed data, was "telegram_bottools-0.1.3.tar", max compression
```

## Comparing `telegram_bottools-0.1.2.tar` & `telegram_bottools-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      472 2023-04-17 21:59:33.128358 telegram_bottools-0.1.2/README.md
--rw-r--r--   0        0        0      383 2023-04-17 22:03:53.531996 telegram_bottools-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-17 21:59:34.629363 telegram_bottools-0.1.2/telegram_bottools/__init__.py
--rw-r--r--   0        0        0     1760 2023-04-17 21:59:34.632511 telegram_bottools-0.1.2/telegram_bottools/telegram_bottools.py
--rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 telegram_bottools-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      477 2023-04-17 22:16:18.604212 telegram_bottools-0.1.3/README.md
+-rw-r--r--   0        0        0      383 2023-04-17 22:22:48.766392 telegram_bottools-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-17 21:59:34.629363 telegram_bottools-0.1.3/telegram_bottools/__init__.py
+-rw-r--r--   0        0        0     1760 2023-04-17 21:59:34.632511 telegram_bottools-0.1.3/telegram_bottools/telegram_bottools.py
+-rw-r--r--   0        0        0      873 1970-01-01 00:00:00.000000 telegram_bottools-0.1.3/PKG-INFO
```

### Comparing `telegram_bottools-0.1.2/telegram_bottools/telegram_bottools.py` & `telegram_bottools-0.1.3/telegram_bottools/telegram_bottools.py`

 * *Files identical despite different names*

### Comparing `telegram_bottools-0.1.2/PKG-INFO` & `telegram_bottools-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: telegram-bottools
-Version: 0.1.2
+Version: 0.1.3
 Summary: Telegram Bot Tools
 Author: Ricardo Merces
 Author-email: ricardo.merces@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.28,<3.0)
 Requires-Dist: urllib3 (>=1.26,<2.0)
 Description-Content-Type: text/markdown
 
 # Create Telegram Bot
 Telegram -> BotFather -> Type `/newbot`
+
 https://core.telegram.org/bots/tutorial#creating-your-command
 
 # Get Chat ID
-https://api.telegram.org/bot<token>getUpdates
+https://api.telegram.org/botXXXX:YYYYY/getUpdates
 
 # Install
 ```
 pip install telegram-bottools
 ```
 
 # Config
```

