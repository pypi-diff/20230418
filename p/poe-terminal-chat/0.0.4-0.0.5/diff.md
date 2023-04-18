# Comparing `tmp/poe_terminal_chat-0.0.4.tar.gz` & `tmp/poe_terminal_chat-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poe_terminal_chat-0.0.4.tar", last modified: Tue Apr 18 09:06:37 2023, max compression
+gzip compressed data, was "poe_terminal_chat-0.0.5.tar", last modified: Tue Apr 18 09:09:46 2023, max compression
```

## Comparing `poe_terminal_chat-0.0.4.tar` & `poe_terminal_chat-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 09:06:37.289263 poe_terminal_chat-0.0.4/
--rw-rw-rw-   0        0        0     1087 2023-04-15 14:49:57.000000 poe_terminal_chat-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      211 2023-04-18 09:06:37.288262 poe_terminal_chat-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      643 2023-04-15 16:02:30.000000 poe_terminal_chat-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 09:06:37.277262 poe_terminal_chat-0.0.4/poe_terminal_chat/
--rw-rw-rw-   0        0        0        0 2023-04-15 12:08:35.000000 poe_terminal_chat-0.0.4/poe_terminal_chat/__init__.py
--rw-rw-rw-   0        0        0     1886 2023-04-18 08:55:59.000000 poe_terminal_chat-0.0.4/poe_terminal_chat/command_line.py
--rw-rw-rw-   0        0        0     1310 2023-04-18 08:56:03.000000 poe_terminal_chat-0.0.4/poe_terminal_chat/poeterminal.py
--rw-rw-rw-   0        0        0     2121 2023-04-18 08:53:44.000000 poe_terminal_chat-0.0.4/poe_terminal_chat/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:06:37.287262 poe_terminal_chat-0.0.4/poe_terminal_chat.egg-info/
--rw-rw-rw-   0        0        0      211 2023-04-18 09:06:37.000000 poe_terminal_chat-0.0.4/poe_terminal_chat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-04-18 09:06:37.000000 poe_terminal_chat-0.0.4/poe_terminal_chat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 09:06:37.000000 poe_terminal_chat-0.0.4/poe_terminal_chat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-04-18 09:06:37.000000 poe_terminal_chat-0.0.4/poe_terminal_chat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       54 2023-04-18 09:06:37.000000 poe_terminal_chat-0.0.4/poe_terminal_chat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-18 09:06:37.000000 poe_terminal_chat-0.0.4/poe_terminal_chat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 09:06:37.289263 poe_terminal_chat-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      686 2023-04-18 09:06:31.000000 poe_terminal_chat-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:09:46.529961 poe_terminal_chat-0.0.5/
+-rw-rw-rw-   0        0        0     1087 2023-04-15 14:49:57.000000 poe_terminal_chat-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      307 2023-04-18 09:09:46.528960 poe_terminal_chat-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      643 2023-04-15 16:02:30.000000 poe_terminal_chat-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 09:09:46.517960 poe_terminal_chat-0.0.5/poe_terminal_chat/
+-rw-rw-rw-   0        0        0        0 2023-04-15 12:08:35.000000 poe_terminal_chat-0.0.5/poe_terminal_chat/__init__.py
+-rw-rw-rw-   0        0        0     1886 2023-04-18 08:55:59.000000 poe_terminal_chat-0.0.5/poe_terminal_chat/command_line.py
+-rw-rw-rw-   0        0        0     1310 2023-04-18 08:56:03.000000 poe_terminal_chat-0.0.5/poe_terminal_chat/poeterminal.py
+-rw-rw-rw-   0        0        0     2121 2023-04-18 08:53:44.000000 poe_terminal_chat-0.0.5/poe_terminal_chat/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:09:46.527961 poe_terminal_chat-0.0.5/poe_terminal_chat.egg-info/
+-rw-rw-rw-   0        0        0      307 2023-04-18 09:09:46.000000 poe_terminal_chat-0.0.5/poe_terminal_chat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-04-18 09:09:46.000000 poe_terminal_chat-0.0.5/poe_terminal_chat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 09:09:46.000000 poe_terminal_chat-0.0.5/poe_terminal_chat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-04-18 09:09:46.000000 poe_terminal_chat-0.0.5/poe_terminal_chat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       54 2023-04-18 09:09:46.000000 poe_terminal_chat-0.0.5/poe_terminal_chat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-18 09:09:46.000000 poe_terminal_chat-0.0.5/poe_terminal_chat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 09:09:46.529961 poe_terminal_chat-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-04-18 09:08:35.000000 poe_terminal_chat-0.0.5/setup.py
```

### Comparing `poe_terminal_chat-0.0.4/LICENSE` & `poe_terminal_chat-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `poe_terminal_chat-0.0.4/README.md` & `poe_terminal_chat-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `poe_terminal_chat-0.0.4/poe_terminal_chat/command_line.py` & `poe_terminal_chat-0.0.5/poe_terminal_chat/command_line.py`

 * *Files identical despite different names*

### Comparing `poe_terminal_chat-0.0.4/poe_terminal_chat/poeterminal.py` & `poe_terminal_chat-0.0.5/poe_terminal_chat/poeterminal.py`

 * *Files identical despite different names*

### Comparing `poe_terminal_chat-0.0.4/poe_terminal_chat/utils.py` & `poe_terminal_chat-0.0.5/poe_terminal_chat/utils.py`

 * *Files identical despite different names*

### Comparing `poe_terminal_chat-0.0.4/setup.py` & `poe_terminal_chat-0.0.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
         name="poe_terminal_chat",
-        version="0.0.4",
-        descrption="poe(a third part AI assistant) terminal chat, can have accesses of chatgpt and claude",
+        version="0.0.5",
+        description="poe(a third part AI assistant) terminal chat, can have accesses of chatgpt and claude",
         url="https://github.com/Mushrr/poe_terminal_chat",
         author="Mushr",
         author_email="huangxingjiegkd@163.com",
         license="MIT",
         packages=["poe_terminal_chat"],
         entry_points = {
             'console_scripts': ['poechat=poe_terminal_chat.command_line:main']
```

