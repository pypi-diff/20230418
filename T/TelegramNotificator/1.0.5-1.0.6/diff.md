# Comparing `tmp/TelegramNotificator-1.0.5.tar.gz` & `tmp/TelegramNotificator-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TelegramNotificator-1.0.5.tar", last modified: Sun Apr 16 21:56:25 2023, max compression
+gzip compressed data, was "TelegramNotificator-1.0.6.tar", last modified: Mon Apr 17 22:23:54 2023, max compression
```

## Comparing `TelegramNotificator-1.0.5.tar` & `TelegramNotificator-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 21:56:25.980579 TelegramNotificator-1.0.5/
--rw-rw-rw-   0        0        0     1063 2023-04-15 02:05:41.000000 TelegramNotificator-1.0.5/LICENCE
--rw-rw-rw-   0        0        0      786 2023-04-16 21:56:25.980579 TelegramNotificator-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      654 2023-04-15 03:09:06.000000 TelegramNotificator-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 21:56:25.913580 TelegramNotificator-1.0.5/TelegramNotificator.egg-info/
--rw-rw-rw-   0        0        0      786 2023-04-16 21:56:25.000000 TelegramNotificator-1.0.5/TelegramNotificator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-04-16 21:56:25.000000 TelegramNotificator-1.0.5/TelegramNotificator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 21:56:25.000000 TelegramNotificator-1.0.5/TelegramNotificator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-16 21:56:25.000000 TelegramNotificator-1.0.5/TelegramNotificator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-16 21:56:25.000000 TelegramNotificator-1.0.5/TelegramNotificator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 21:56:25.981580 TelegramNotificator-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      996 2023-04-16 21:56:22.000000 TelegramNotificator-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 21:56:25.947580 TelegramNotificator-1.0.5/telegram_notificator/
--rw-rw-rw-   0        0        0      523 2023-04-15 02:58:12.000000 TelegramNotificator-1.0.5/telegram_notificator/__init__.py
--rw-rw-rw-   0        0        0      524 2023-04-15 02:58:43.000000 TelegramNotificator-1.0.5/telegram_notificator/telegram_notificator.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:23:54.598052 TelegramNotificator-1.0.6/
+-rw-rw-rw-   0        0        0     1063 2023-04-15 02:05:41.000000 TelegramNotificator-1.0.6/LICENCE
+-rw-rw-rw-   0        0        0      786 2023-04-17 22:23:54.594529 TelegramNotificator-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      654 2023-04-15 03:09:06.000000 TelegramNotificator-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 22:23:54.588529 TelegramNotificator-1.0.6/TelegramNotificator.egg-info/
+-rw-rw-rw-   0        0        0      786 2023-04-17 22:23:54.000000 TelegramNotificator-1.0.6/TelegramNotificator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-04-17 22:23:54.000000 TelegramNotificator-1.0.6/TelegramNotificator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 22:23:54.000000 TelegramNotificator-1.0.6/TelegramNotificator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-17 22:23:54.000000 TelegramNotificator-1.0.6/TelegramNotificator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-17 22:23:54.000000 TelegramNotificator-1.0.6/TelegramNotificator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 22:23:54.598052 TelegramNotificator-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      996 2023-04-17 22:19:52.000000 TelegramNotificator-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:23:54.591529 TelegramNotificator-1.0.6/telegram_notificator/
+-rw-rw-rw-   0        0        0      523 2023-04-15 02:58:12.000000 TelegramNotificator-1.0.6/telegram_notificator/__init__.py
```

### Comparing `TelegramNotificator-1.0.5/LICENCE` & `TelegramNotificator-1.0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `TelegramNotificator-1.0.5/PKG-INFO` & `TelegramNotificator-1.0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TelegramNotificator
-Version: 1.0.5
+Version: 1.0.6
 Summary: A basic telegram notifications sender.
 Home-page: https://github.com/errais2000/telegram_notificator
 Author: Cryptoroid
 Author-email: 
 License: MIT
 Keywords: telegram,message,notification,alert,send message,telegram message,telegram bot
 Classifier: Development Status :: 1 - Planning
```

### Comparing `TelegramNotificator-1.0.5/README.md` & `TelegramNotificator-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `TelegramNotificator-1.0.5/TelegramNotificator.egg-info/PKG-INFO` & `TelegramNotificator-1.0.6/TelegramNotificator.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TelegramNotificator
-Version: 1.0.5
+Version: 1.0.6
 Summary: A basic telegram notifications sender.
 Home-page: https://github.com/errais2000/telegram_notificator
 Author: Cryptoroid
 Author-email: 
 License: MIT
 Keywords: telegram,message,notification,alert,send message,telegram message,telegram bot
 Classifier: Development Status :: 1 - Planning
```

### Comparing `TelegramNotificator-1.0.5/setup.py` & `TelegramNotificator-1.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 # Setting up
 setup(
     name="TelegramNotificator",
-    version='1.0.5',
+    version='1.0.6',
     author="Cryptoroid",
     author_email="",
     license='MIT',
     description='A basic telegram notifications sender.',
     long_description_content_type="text/markdown",
     long_description='Send telegram notifications or alerts from your python programs.',
     url='https://github.com/errais2000/telegram_notificator',
```

### Comparing `TelegramNotificator-1.0.5/telegram_notificator/__init__.py` & `TelegramNotificator-1.0.6/telegram_notificator/__init__.py`

 * *Files identical despite different names*

