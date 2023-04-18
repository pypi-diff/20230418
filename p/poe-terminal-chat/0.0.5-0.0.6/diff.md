# Comparing `tmp/poe_terminal_chat-0.0.5.tar.gz` & `tmp/poe_terminal_chat-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poe_terminal_chat-0.0.5.tar", last modified: Tue Apr 18 09:09:46 2023, max compression
+gzip compressed data, was "poe_terminal_chat-0.0.6.tar", last modified: Tue Apr 18 09:37:06 2023, max compression
```

## Comparing `poe_terminal_chat-0.0.5.tar` & `poe_terminal_chat-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 09:09:46.529961 poe_terminal_chat-0.0.5/
--rw-rw-rw-   0        0        0     1087 2023-04-15 14:49:57.000000 poe_terminal_chat-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      307 2023-04-18 09:09:46.528960 poe_terminal_chat-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      643 2023-04-15 16:02:30.000000 poe_terminal_chat-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 09:09:46.517960 poe_terminal_chat-0.0.5/poe_terminal_chat/
--rw-rw-rw-   0        0        0        0 2023-04-15 12:08:35.000000 poe_terminal_chat-0.0.5/poe_terminal_chat/__init__.py
--rw-rw-rw-   0        0        0     1886 2023-04-18 08:55:59.000000 poe_terminal_chat-0.0.5/poe_terminal_chat/command_line.py
--rw-rw-rw-   0        0        0     1310 2023-04-18 08:56:03.000000 poe_terminal_chat-0.0.5/poe_terminal_chat/poeterminal.py
--rw-rw-rw-   0        0        0     2121 2023-04-18 08:53:44.000000 poe_terminal_chat-0.0.5/poe_terminal_chat/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:09:46.527961 poe_terminal_chat-0.0.5/poe_terminal_chat.egg-info/
--rw-rw-rw-   0        0        0      307 2023-04-18 09:09:46.000000 poe_terminal_chat-0.0.5/poe_terminal_chat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-04-18 09:09:46.000000 poe_terminal_chat-0.0.5/poe_terminal_chat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 09:09:46.000000 poe_terminal_chat-0.0.5/poe_terminal_chat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-04-18 09:09:46.000000 poe_terminal_chat-0.0.5/poe_terminal_chat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       54 2023-04-18 09:09:46.000000 poe_terminal_chat-0.0.5/poe_terminal_chat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-18 09:09:46.000000 poe_terminal_chat-0.0.5/poe_terminal_chat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 09:09:46.529961 poe_terminal_chat-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-04-18 09:08:35.000000 poe_terminal_chat-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:37:06.248234 poe_terminal_chat-0.0.6/
+-rw-rw-rw-   0        0        0     1087 2023-04-15 14:49:57.000000 poe_terminal_chat-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      307 2023-04-18 09:37:06.247232 poe_terminal_chat-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2023-04-18 09:12:29.000000 poe_terminal_chat-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 09:37:06.231233 poe_terminal_chat-0.0.6/poe_terminal_chat/
+-rw-rw-rw-   0        0        0        0 2023-04-15 12:08:35.000000 poe_terminal_chat-0.0.6/poe_terminal_chat/__init__.py
+-rw-rw-rw-   0        0        0     1886 2023-04-18 08:55:59.000000 poe_terminal_chat-0.0.6/poe_terminal_chat/command_line.py
+-rw-rw-rw-   0        0        0     1322 2023-04-18 09:36:42.000000 poe_terminal_chat-0.0.6/poe_terminal_chat/poeterminal.py
+-rw-rw-rw-   0        0        0     2119 2023-04-18 09:36:35.000000 poe_terminal_chat-0.0.6/poe_terminal_chat/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:37:06.245233 poe_terminal_chat-0.0.6/poe_terminal_chat.egg-info/
+-rw-rw-rw-   0        0        0      307 2023-04-18 09:37:06.000000 poe_terminal_chat-0.0.6/poe_terminal_chat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-04-18 09:37:06.000000 poe_terminal_chat-0.0.6/poe_terminal_chat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 09:37:06.000000 poe_terminal_chat-0.0.6/poe_terminal_chat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-04-18 09:37:06.000000 poe_terminal_chat-0.0.6/poe_terminal_chat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       54 2023-04-18 09:37:06.000000 poe_terminal_chat-0.0.6/poe_terminal_chat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-18 09:37:06.000000 poe_terminal_chat-0.0.6/poe_terminal_chat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 09:37:06.248234 poe_terminal_chat-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-04-18 09:36:58.000000 poe_terminal_chat-0.0.6/setup.py
```

### Comparing `poe_terminal_chat-0.0.5/LICENSE` & `poe_terminal_chat-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `poe_terminal_chat-0.0.5/README.md` & `poe_terminal_chat-0.0.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ```
 more information about pipx installation [pipx](https://github.com/pypa/pipx#install-pipx)
 
 #### 2. install poe_terminal_chat
 
 ```shell
 
-pipx install poe_terminal_chat==0.0.2
+pipx install poe_terminal_chat
 ```
 
 #### 3. get poe token & set proxy server
 
 open [poe](https://poe.com), inspect this site, you will find token in cookies
 
 ```shell
```

### Comparing `poe_terminal_chat-0.0.5/poe_terminal_chat/command_line.py` & `poe_terminal_chat-0.0.6/poe_terminal_chat/command_line.py`

 * *Files identical despite different names*

### Comparing `poe_terminal_chat-0.0.5/poe_terminal_chat/poeterminal.py` & `poe_terminal_chat-0.0.6/poe_terminal_chat/poeterminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,11 +27,11 @@
                 question += tmp
             if question == "":
                 break
             print("\n😊> ", end='')
             try:
                 self.single_chat(question, with_chat_break=False)
             except:
-                print("好像网络出了点问题，重新发一下吧~🙌", end='')
+                print("好像网络出了点问题，重新发一下吧~🙌", end='', flush=True)
             print("\n")
         print(f"Hope this journey with {self.bot_name} can help you!")
         return
```

### Comparing `poe_terminal_chat-0.0.5/poe_terminal_chat/utils.py` & `poe_terminal_chat-0.0.6/poe_terminal_chat/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,8 +60,7 @@
                 prompt=prompt,
                 intro_message=intro_message
                 )
         print("Create Bot successfully!")
     except:
         print("Create Bot failed!")
         exit(0)
-
```

### Comparing `poe_terminal_chat-0.0.5/setup.py` & `poe_terminal_chat-0.0.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
         name="poe_terminal_chat",
-        version="0.0.5",
+        version="0.0.6",
         description="poe(a third part AI assistant) terminal chat, can have accesses of chatgpt and claude",
         url="https://github.com/Mushrr/poe_terminal_chat",
         author="Mushr",
         author_email="huangxingjiegkd@163.com",
         license="MIT",
         packages=["poe_terminal_chat"],
         entry_points = {
```

