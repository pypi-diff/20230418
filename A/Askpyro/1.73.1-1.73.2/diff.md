# Comparing `tmp/Askpyro-1.73.1.tar.gz` & `tmp/Askpyro-1.73.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Askpyro-1.73.1.tar", last modified: Mon Apr 17 15:04:53 2023, max compression
+gzip compressed data, was "Askpyro-1.73.2.tar", last modified: Tue Apr 18 13:20:55 2023, max compression
```

## Comparing `Askpyro-1.73.1.tar` & `Askpyro-1.73.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:04:53.742693 Askpyro-1.73.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:04:53.738693 Askpyro-1.73.1/Askpyro.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3766 2023-04-17 15:04:53.000000 Askpyro-1.73.1/Askpyro.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      423 2023-04-17 15:04:53.000000 Askpyro-1.73.1/Askpyro.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 15:04:53.000000 Askpyro-1.73.1/Askpyro.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 14:50:05.000000 Askpyro-1.73.1/Askpyro.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-17 15:04:53.000000 Askpyro-1.73.1/Askpyro.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-17 14:49:34.000000 Askpyro-1.73.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3766 2023-04-17 15:04:53.742693 Askpyro-1.73.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1934 2023-04-17 14:49:34.000000 Askpyro-1.73.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:04:53.738693 Askpyro-1.73.1/askpyro/
--rw-r--r--   0 root         (0) root         (0)      242 2023-04-17 14:49:34.000000 Askpyro-1.73.1/askpyro/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5553 2023-04-17 14:49:34.000000 Askpyro-1.73.1/askpyro/conversation.py
--rw-r--r--   0 root         (0) root         (0)      842 2023-04-17 14:49:34.000000 Askpyro-1.73.1/askpyro/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:04:53.738693 Askpyro-1.73.1/askpyro/helpers/
--rw-r--r--   0 root         (0) root         (0)      893 2023-04-17 14:49:34.000000 Askpyro-1.73.1/askpyro/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3208 2023-04-17 14:49:34.000000 Askpyro-1.73.1/askpyro/helpers/helpers.py
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-17 14:49:34.000000 Askpyro-1.73.1/askpyro/helpers/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:04:53.742693 Askpyro-1.73.1/examples/
--rw-r--r--   0 root         (0) root         (0)      161 2023-04-17 14:49:34.000000 Askpyro-1.73.1/examples/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1442 2023-04-17 14:49:34.000000 Askpyro-1.73.1/examples/buttons.py
--rw-r--r--   0 root         (0) root         (0)      450 2023-04-17 14:49:34.000000 Askpyro-1.73.1/examples/callback.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-04-17 14:49:34.000000 Askpyro-1.73.1/examples/filters.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-04-17 14:49:34.000000 Askpyro-1.73.1/examples/start.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 15:04:53.742693 Askpyro-1.73.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3115 2023-04-17 15:04:48.000000 Askpyro-1.73.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:20:55.801741 Askpyro-1.73.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:20:55.797741 Askpyro-1.73.2/Askpyro.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4057 2023-04-18 13:20:55.000000 Askpyro-1.73.2/Askpyro.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      443 2023-04-18 13:20:55.000000 Askpyro-1.73.2/Askpyro.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 13:20:55.000000 Askpyro-1.73.2/Askpyro.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 13:20:55.000000 Askpyro-1.73.2/Askpyro.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-18 13:20:55.000000 Askpyro-1.73.2/Askpyro.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-18 13:20:36.000000 Askpyro-1.73.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4057 2023-04-18 13:20:55.801741 Askpyro-1.73.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2212 2023-04-18 13:20:36.000000 Askpyro-1.73.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:20:55.797741 Askpyro-1.73.2/askpyro/
+-rw-r--r--   0 root         (0) root         (0)      242 2023-04-18 13:20:36.000000 Askpyro-1.73.2/askpyro/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5532 2023-04-18 13:20:36.000000 Askpyro-1.73.2/askpyro/conversation.py
+-rw-r--r--   0 root         (0) root         (0)      824 2023-04-18 13:20:36.000000 Askpyro-1.73.2/askpyro/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:20:55.797741 Askpyro-1.73.2/askpyro/helpers/
+-rw-r--r--   0 root         (0) root         (0)      893 2023-04-18 13:20:36.000000 Askpyro-1.73.2/askpyro/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3208 2023-04-18 13:20:36.000000 Askpyro-1.73.2/askpyro/helpers/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-18 13:20:36.000000 Askpyro-1.73.2/askpyro/helpers/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:20:55.797741 Askpyro-1.73.2/examples/
+-rw-r--r--   0 root         (0) root         (0)      161 2023-04-18 13:20:36.000000 Askpyro-1.73.2/examples/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-04-18 13:20:36.000000 Askpyro-1.73.2/examples/buttons.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-04-18 13:20:36.000000 Askpyro-1.73.2/examples/callback.py
+-rw-r--r--   0 root         (0) root         (0)     1775 2023-04-18 13:20:36.000000 Askpyro-1.73.2/examples/captcha.py
+-rw-r--r--   0 root         (0) root         (0)      502 2023-04-18 13:20:36.000000 Askpyro-1.73.2/examples/filters.py
+-rw-r--r--   0 root         (0) root         (0)      444 2023-04-18 13:20:36.000000 Askpyro-1.73.2/examples/start.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 13:20:55.801741 Askpyro-1.73.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3199 2023-04-18 13:20:36.000000 Askpyro-1.73.2/setup.py
```

### Comparing `Askpyro-1.73.1/Askpyro.egg-info/PKG-INFO` & `Askpyro-1.73.2/Askpyro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: Askpyro
-Version: 1.73.1
+Version: 1.73.2
 Summary: Easy conversation handler for pyrogram
 Home-page: https://github.com/Abishnoi69
 Author: Abishnoi
 Author-email: abishnoi@askpyro.org
 License: LGPLv3
 Download-URL: https://github.com/Abishnoi69/Askpyro/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Askpyro/issues
 Project-URL: Community, https://t.me/AbishnoiMF
 Project-URL: Source, https://github.com/Abishnoi69/Askpyro
 Project-URL: Documentation, https://github.com/Abishnoi69/askpyro/wiki
-Keywords: telegram chat messenger mtproto api client library python
+Keywords: telegram chat messenger mtproto api client library python conversation
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -36,15 +36,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## ᴀsᴋ-ᴘʏʀᴏ
 
-> sᴛᴀʀᴛ ᴀsᴋ-ᴄʟɪᴇɴᴛ ᴡɪᴛʜ @ᴀᴘᴘ[ᴘʏʀᴏɢʀᴀᴍ ᴄʟɪᴇɴᴛ]
+> sᴛᴀʀᴛ ᴀsᴋ-ᴄʟɪᴇɴᴛ ᴡɪᴛʜ @ᴀᴘᴘ [ᴘʏʀᴏɢʀᴀᴍ ᴄʟɪᴇɴᴛ]
 ```python
   from askpyro import Askclient
   from pyrogram import Client ,filters
   
   app = Client("my_account")
   read = Askclient(app)
 
@@ -63,45 +63,47 @@
 
 ```python
 pip3 install askpyro
 ```
 
 <details>
 <summary><h3>
+- <b> ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ ɪɴ ᴘʏʀᴏɢʀᴀᴍ </b>
+</h3></summary>
+<a href="https://github.com/Abishnoi69/Askpyro/wiki/Conversation"><img src="https://img.shields.io/badge/ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ-903022f?logo=github"></a>
+</details>
+
+<details>
+<summary><h3>
 - <b> ᴡɪᴋɪ / ʜᴏᴡ ᴛᴏ ᴜsᴇ </b>
 </h3></summary>
-<a href="https://github.com/Abishnoi69/askpyro/wiki"><img src="https://img.shields.io/badge/ᴡɪᴋɪ-90302f?logo=github"></a>
+<a href="https://github.com/Abishnoi69/askpyro/wiki"><img src="https://img.shields.io/badge/ᴡɪᴋɪ-1589F0?logo=github"></a>
 </details>
 
 <details>
 <summary><h3>
 - <b> ᴇxᴀᴍᴘʟᴇ </b>
 </h3></summary>
-<a href="https://github.com/Abishnoi69/askpyro/tree/main/examples"><img src="https://img.shields.io/badge/ᴇxᴀᴍᴘʟᴇs-90302f?logo=github"></a>
+<a href="https://github.com/Abishnoi69/askpyro/tree/main/examples"><img src="https://img.shields.io/badge/ᴇxᴀᴍᴘʟᴇs-c5f015?logo=github"></a>
 </details>
 
-
-
 <details>
 <summary><h3>
 - <b> ᴛᴇʟᴇɢʀᴀᴍ ɢʀᴏᴜᴘ </b>
 </h3></summary>
 <a href="https://telegram.me/AbishnoiMF"><img src="https://img.shields.io/badge/-Support%20Group-blue.svg?style=for-the-badge&logo=Telegram"></a>
 </details>
 
-
-
 <details>
 <summary><h3>
 - <b>ᴄʀᴇᴅɪᴛs</b>
 </h3></summary>
 
 ➥ [𝐀𝖻𝗂𝗌𝗁𝗇𝗈𝗂] ↬ <a href="https://github.com/Abishnoi69" alt="Abishnoi69"> <img src="https://img.shields.io/badge/ᴀʙɪsʜɴᴏɪ-90302f?logo=github" /></a>  
 
 ➥ [𝐏ʏʀᴏɢʀᴀᴍ] ↬ <a href="https://github.com/pyrogram" alt="Pyrogram"> <img src="https://img.shields.io/badge/Pyrogram-90302f?logo=github" /></a>  
   
 ➥ [𝐒ᴘɪᴅᴇʀ] ↬ <a href="https://github.com/Surendra9123" alt="Surendra9123"> <img src="https://img.shields.io/badge/SPiDER-90302f?logo=github" /></a>  
-
 ━━━━━━━━━━━━━━━━━━━━
 </details>
```

#### html2text {}

```diff
@@ -1,43 +1,46 @@
-Metadata-Version: 2.1 Name: Askpyro Version: 1.73.1 Summary: Easy conversation
+Metadata-Version: 2.1 Name: Askpyro Version: 1.73.2 Summary: Easy conversation
 handler for pyrogram Home-page: https://github.com/Abishnoi69 Author: Abishnoi
 Author-email: abishnoi@askpyro.org License: LGPLv3 Download-URL: https://
 github.com/Abishnoi69/Askpyro/releases/latest Project-URL: Tracker, https://
 github.com/Abishnoi69/Askpyro/issues Project-URL: Community, https://t.me/
 AbishnoiMF Project-URL: Source, https://github.com/Abishnoi69/Askpyro Project-
 URL: Documentation, https://github.com/Abishnoi69/askpyro/wiki Keywords:
-telegram chat messenger mtproto api client library python Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Developers Classifier: Natural Language :: English Classifier:
-License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: Implementation
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+telegram chat messenger mtproto api client library python conversation
+Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers Classifier: Natural Language ::
+English Classifier: License :: OSI Approved :: GNU Lesser General Public
+License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python ::
+Implementation Classifier: Programming Language :: Python :: Implementation ::
+CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet Classifier: Topic :: Communications Classifier:
 Topic :: Communications :: Chat Classifier: Topic :: Software Development ::
 Libraries Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Topic :: Software Development :: Libraries :: Application
 Frameworks Requires-Python: ~=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE ## á´sá´-á´ÊÊá´ > sá´á´Êá´ á´sá´-
-á´ÊÉªá´É´á´ á´¡Éªá´Ê @á´á´á´[á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´]
+á´ÊÉªá´É´á´ á´¡Éªá´Ê @á´á´á´ [á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´]
 ```python from askpyro import Askclient from pyrogram import Client ,filters
 app = Client("my_account") read = Askclient(app) @app.on_message
 (filters.command("start")) async def start_pm(c: app, m: Message): answer =
 await read.ask(m, text) if answer.text: print(answer.text) await answer.reply
 ("Éª É¢á´á´ á´É´sá´¡á´Ê..") app.run() ``` ### ÉªÉ´sá´á´ÊÊÉªÉ´É¢
 ```python pip3 install askpyro ```
+**** - á´á´É´á´ á´Êsá´á´Éªá´É´ ÉªÉ´ á´ÊÊá´É¢Êá´á´ ****
+[https://img.shields.io/badge/á´á´É´á´ á´Êsá´á´Éªá´É´-
+903022f?logo=github]
 **** - á´¡Éªá´Éª / Êá´á´¡ á´á´ á´sá´ ****
-[https://img.shields.io/badge/á´¡Éªá´Éª-90302f?logo=github]
+[https://img.shields.io/badge/á´¡Éªá´Éª-1589F0?logo=github]
 **** - á´xá´á´á´Êá´ ****
-[https://img.shields.io/badge/á´xá´á´á´Êá´s-90302f?logo=github]
+[https://img.shields.io/badge/á´xá´á´á´Êá´s-c5f015?logo=github]
 **** - á´á´Êá´É¢Êá´á´ É¢Êá´á´á´ ****
 [https://img.shields.io/badge/-Support%20Group-blue.svg?style=for-the-
 badge&logo=Telegram]
 **** - á´Êá´á´Éªá´s ****
 â¥ [ðð»ðððððð] â¬ [https://img.shields.io/badge/
 á´ÊÉªsÊÉ´á´Éª-90302f?logo=github] â¥ [ðÊÊá´É¢Êá´á´] â¬ [https://
 img.shields.io/badge/Pyrogram-90302f?logo=github] â¥ [ðá´Éªá´á´Ê] â¬
```

### Comparing `Askpyro-1.73.1/LICENSE` & `Askpyro-1.73.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Askpyro-1.73.1/PKG-INFO` & `Askpyro-1.73.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: Askpyro
-Version: 1.73.1
+Version: 1.73.2
 Summary: Easy conversation handler for pyrogram
 Home-page: https://github.com/Abishnoi69
 Author: Abishnoi
 Author-email: abishnoi@askpyro.org
 License: LGPLv3
 Download-URL: https://github.com/Abishnoi69/Askpyro/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Askpyro/issues
 Project-URL: Community, https://t.me/AbishnoiMF
 Project-URL: Source, https://github.com/Abishnoi69/Askpyro
 Project-URL: Documentation, https://github.com/Abishnoi69/askpyro/wiki
-Keywords: telegram chat messenger mtproto api client library python
+Keywords: telegram chat messenger mtproto api client library python conversation
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -36,15 +36,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## ᴀsᴋ-ᴘʏʀᴏ
 
-> sᴛᴀʀᴛ ᴀsᴋ-ᴄʟɪᴇɴᴛ ᴡɪᴛʜ @ᴀᴘᴘ[ᴘʏʀᴏɢʀᴀᴍ ᴄʟɪᴇɴᴛ]
+> sᴛᴀʀᴛ ᴀsᴋ-ᴄʟɪᴇɴᴛ ᴡɪᴛʜ @ᴀᴘᴘ [ᴘʏʀᴏɢʀᴀᴍ ᴄʟɪᴇɴᴛ]
 ```python
   from askpyro import Askclient
   from pyrogram import Client ,filters
   
   app = Client("my_account")
   read = Askclient(app)
 
@@ -63,45 +63,47 @@
 
 ```python
 pip3 install askpyro
 ```
 
 <details>
 <summary><h3>
+- <b> ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ ɪɴ ᴘʏʀᴏɢʀᴀᴍ </b>
+</h3></summary>
+<a href="https://github.com/Abishnoi69/Askpyro/wiki/Conversation"><img src="https://img.shields.io/badge/ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ-903022f?logo=github"></a>
+</details>
+
+<details>
+<summary><h3>
 - <b> ᴡɪᴋɪ / ʜᴏᴡ ᴛᴏ ᴜsᴇ </b>
 </h3></summary>
-<a href="https://github.com/Abishnoi69/askpyro/wiki"><img src="https://img.shields.io/badge/ᴡɪᴋɪ-90302f?logo=github"></a>
+<a href="https://github.com/Abishnoi69/askpyro/wiki"><img src="https://img.shields.io/badge/ᴡɪᴋɪ-1589F0?logo=github"></a>
 </details>
 
 <details>
 <summary><h3>
 - <b> ᴇxᴀᴍᴘʟᴇ </b>
 </h3></summary>
-<a href="https://github.com/Abishnoi69/askpyro/tree/main/examples"><img src="https://img.shields.io/badge/ᴇxᴀᴍᴘʟᴇs-90302f?logo=github"></a>
+<a href="https://github.com/Abishnoi69/askpyro/tree/main/examples"><img src="https://img.shields.io/badge/ᴇxᴀᴍᴘʟᴇs-c5f015?logo=github"></a>
 </details>
 
-
-
 <details>
 <summary><h3>
 - <b> ᴛᴇʟᴇɢʀᴀᴍ ɢʀᴏᴜᴘ </b>
 </h3></summary>
 <a href="https://telegram.me/AbishnoiMF"><img src="https://img.shields.io/badge/-Support%20Group-blue.svg?style=for-the-badge&logo=Telegram"></a>
 </details>
 
-
-
 <details>
 <summary><h3>
 - <b>ᴄʀᴇᴅɪᴛs</b>
 </h3></summary>
 
 ➥ [𝐀𝖻𝗂𝗌𝗁𝗇𝗈𝗂] ↬ <a href="https://github.com/Abishnoi69" alt="Abishnoi69"> <img src="https://img.shields.io/badge/ᴀʙɪsʜɴᴏɪ-90302f?logo=github" /></a>  
 
 ➥ [𝐏ʏʀᴏɢʀᴀᴍ] ↬ <a href="https://github.com/pyrogram" alt="Pyrogram"> <img src="https://img.shields.io/badge/Pyrogram-90302f?logo=github" /></a>  
   
 ➥ [𝐒ᴘɪᴅᴇʀ] ↬ <a href="https://github.com/Surendra9123" alt="Surendra9123"> <img src="https://img.shields.io/badge/SPiDER-90302f?logo=github" /></a>  
-
 ━━━━━━━━━━━━━━━━━━━━
 </details>
```

#### html2text {}

```diff
@@ -1,43 +1,46 @@
-Metadata-Version: 2.1 Name: Askpyro Version: 1.73.1 Summary: Easy conversation
+Metadata-Version: 2.1 Name: Askpyro Version: 1.73.2 Summary: Easy conversation
 handler for pyrogram Home-page: https://github.com/Abishnoi69 Author: Abishnoi
 Author-email: abishnoi@askpyro.org License: LGPLv3 Download-URL: https://
 github.com/Abishnoi69/Askpyro/releases/latest Project-URL: Tracker, https://
 github.com/Abishnoi69/Askpyro/issues Project-URL: Community, https://t.me/
 AbishnoiMF Project-URL: Source, https://github.com/Abishnoi69/Askpyro Project-
 URL: Documentation, https://github.com/Abishnoi69/askpyro/wiki Keywords:
-telegram chat messenger mtproto api client library python Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Developers Classifier: Natural Language :: English Classifier:
-License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: Implementation
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+telegram chat messenger mtproto api client library python conversation
+Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers Classifier: Natural Language ::
+English Classifier: License :: OSI Approved :: GNU Lesser General Public
+License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python ::
+Implementation Classifier: Programming Language :: Python :: Implementation ::
+CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet Classifier: Topic :: Communications Classifier:
 Topic :: Communications :: Chat Classifier: Topic :: Software Development ::
 Libraries Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Topic :: Software Development :: Libraries :: Application
 Frameworks Requires-Python: ~=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE ## á´sá´-á´ÊÊá´ > sá´á´Êá´ á´sá´-
-á´ÊÉªá´É´á´ á´¡Éªá´Ê @á´á´á´[á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´]
+á´ÊÉªá´É´á´ á´¡Éªá´Ê @á´á´á´ [á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´]
 ```python from askpyro import Askclient from pyrogram import Client ,filters
 app = Client("my_account") read = Askclient(app) @app.on_message
 (filters.command("start")) async def start_pm(c: app, m: Message): answer =
 await read.ask(m, text) if answer.text: print(answer.text) await answer.reply
 ("Éª É¢á´á´ á´É´sá´¡á´Ê..") app.run() ``` ### ÉªÉ´sá´á´ÊÊÉªÉ´É¢
 ```python pip3 install askpyro ```
+**** - á´á´É´á´ á´Êsá´á´Éªá´É´ ÉªÉ´ á´ÊÊá´É¢Êá´á´ ****
+[https://img.shields.io/badge/á´á´É´á´ á´Êsá´á´Éªá´É´-
+903022f?logo=github]
 **** - á´¡Éªá´Éª / Êá´á´¡ á´á´ á´sá´ ****
-[https://img.shields.io/badge/á´¡Éªá´Éª-90302f?logo=github]
+[https://img.shields.io/badge/á´¡Éªá´Éª-1589F0?logo=github]
 **** - á´xá´á´á´Êá´ ****
-[https://img.shields.io/badge/á´xá´á´á´Êá´s-90302f?logo=github]
+[https://img.shields.io/badge/á´xá´á´á´Êá´s-c5f015?logo=github]
 **** - á´á´Êá´É¢Êá´á´ É¢Êá´á´á´ ****
 [https://img.shields.io/badge/-Support%20Group-blue.svg?style=for-the-
 badge&logo=Telegram]
 **** - á´Êá´á´Éªá´s ****
 â¥ [ðð»ðððððð] â¬ [https://img.shields.io/badge/
 á´ÊÉªsÊÉ´á´Éª-90302f?logo=github] â¥ [ðÊÊá´É¢Êá´á´] â¬ [https://
 img.shields.io/badge/Pyrogram-90302f?logo=github] â¥ [ðá´Éªá´á´Ê] â¬
```

### Comparing `Askpyro-1.73.1/README.md` & `Askpyro-1.73.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ## ᴀsᴋ-ᴘʏʀᴏ
 
-> sᴛᴀʀᴛ ᴀsᴋ-ᴄʟɪᴇɴᴛ ᴡɪᴛʜ @ᴀᴘᴘ[ᴘʏʀᴏɢʀᴀᴍ ᴄʟɪᴇɴᴛ]
+> sᴛᴀʀᴛ ᴀsᴋ-ᴄʟɪᴇɴᴛ ᴡɪᴛʜ @ᴀᴘᴘ [ᴘʏʀᴏɢʀᴀᴍ ᴄʟɪᴇɴᴛ]
 ```python
   from askpyro import Askclient
   from pyrogram import Client ,filters
   
   app = Client("my_account")
   read = Askclient(app)
 
@@ -23,43 +23,45 @@
 
 ```python
 pip3 install askpyro
 ```
 
 <details>
 <summary><h3>
+- <b> ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ ɪɴ ᴘʏʀᴏɢʀᴀᴍ </b>
+</h3></summary>
+<a href="https://github.com/Abishnoi69/Askpyro/wiki/Conversation"><img src="https://img.shields.io/badge/ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ-903022f?logo=github"></a>
+</details>
+
+<details>
+<summary><h3>
 - <b> ᴡɪᴋɪ / ʜᴏᴡ ᴛᴏ ᴜsᴇ </b>
 </h3></summary>
-<a href="https://github.com/Abishnoi69/askpyro/wiki"><img src="https://img.shields.io/badge/ᴡɪᴋɪ-90302f?logo=github"></a>
+<a href="https://github.com/Abishnoi69/askpyro/wiki"><img src="https://img.shields.io/badge/ᴡɪᴋɪ-1589F0?logo=github"></a>
 </details>
 
 <details>
 <summary><h3>
 - <b> ᴇxᴀᴍᴘʟᴇ </b>
 </h3></summary>
-<a href="https://github.com/Abishnoi69/askpyro/tree/main/examples"><img src="https://img.shields.io/badge/ᴇxᴀᴍᴘʟᴇs-90302f?logo=github"></a>
+<a href="https://github.com/Abishnoi69/askpyro/tree/main/examples"><img src="https://img.shields.io/badge/ᴇxᴀᴍᴘʟᴇs-c5f015?logo=github"></a>
 </details>
 
-
-
 <details>
 <summary><h3>
 - <b> ᴛᴇʟᴇɢʀᴀᴍ ɢʀᴏᴜᴘ </b>
 </h3></summary>
 <a href="https://telegram.me/AbishnoiMF"><img src="https://img.shields.io/badge/-Support%20Group-blue.svg?style=for-the-badge&logo=Telegram"></a>
 </details>
 
-
-
 <details>
 <summary><h3>
 - <b>ᴄʀᴇᴅɪᴛs</b>
 </h3></summary>
 
 ➥ [𝐀𝖻𝗂𝗌𝗁𝗇𝗈𝗂] ↬ <a href="https://github.com/Abishnoi69" alt="Abishnoi69"> <img src="https://img.shields.io/badge/ᴀʙɪsʜɴᴏɪ-90302f?logo=github" /></a>  
 
 ➥ [𝐏ʏʀᴏɢʀᴀᴍ] ↬ <a href="https://github.com/pyrogram" alt="Pyrogram"> <img src="https://img.shields.io/badge/Pyrogram-90302f?logo=github" /></a>  
   
 ➥ [𝐒ᴘɪᴅᴇʀ] ↬ <a href="https://github.com/Surendra9123" alt="Surendra9123"> <img src="https://img.shields.io/badge/SPiDER-90302f?logo=github" /></a>  
-
 ━━━━━━━━━━━━━━━━━━━━
 </details>
```

#### html2text {}

```diff
@@ -1,18 +1,21 @@
 ## á´sá´-á´ÊÊá´ > sá´á´Êá´ á´sá´-á´ÊÉªá´É´á´ á´¡Éªá´Ê
-@á´á´á´[á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´] ```python from askpyro import
+@á´á´á´ [á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´] ```python from askpyro import
 Askclient from pyrogram import Client ,filters app = Client("my_account") read
 = Askclient(app) @app.on_message(filters.command("start")) async def start_pm
 (c: app, m: Message): answer = await read.ask(m, text) if answer.text: print
 (answer.text) await answer.reply("Éª É¢á´á´ á´É´sá´¡á´Ê..") app.run() ```
 ### ÉªÉ´sá´á´ÊÊÉªÉ´É¢ ```python pip3 install askpyro ```
+**** - á´á´É´á´ á´Êsá´á´Éªá´É´ ÉªÉ´ á´ÊÊá´É¢Êá´á´ ****
+[https://img.shields.io/badge/á´á´É´á´ á´Êsá´á´Éªá´É´-
+903022f?logo=github]
 **** - á´¡Éªá´Éª / Êá´á´¡ á´á´ á´sá´ ****
-[https://img.shields.io/badge/á´¡Éªá´Éª-90302f?logo=github]
+[https://img.shields.io/badge/á´¡Éªá´Éª-1589F0?logo=github]
 **** - á´xá´á´á´Êá´ ****
-[https://img.shields.io/badge/á´xá´á´á´Êá´s-90302f?logo=github]
+[https://img.shields.io/badge/á´xá´á´á´Êá´s-c5f015?logo=github]
 **** - á´á´Êá´É¢Êá´á´ É¢Êá´á´á´ ****
 [https://img.shields.io/badge/-Support%20Group-blue.svg?style=for-the-
 badge&logo=Telegram]
 **** - á´Êá´á´Éªá´s ****
 â¥ [ðð»ðððððð] â¬ [https://img.shields.io/badge/
 á´ÊÉªsÊÉ´á´Éª-90302f?logo=github] â¥ [ðÊÊá´É¢Êá´á´] â¬ [https://
 img.shields.io/badge/Pyrogram-90302f?logo=github] â¥ [ðá´Éªá´á´Ê] â¬
```

### Comparing `Askpyro-1.73.1/askpyro/conversation.py` & `Askpyro-1.73.2/askpyro/conversation.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,22 +35,22 @@
       self.placeholder : str = placeholder
       self.msg_limit : int = msg_limit
       self.delete_msg : bool = clear
 
   async def ask(self,
                 msg : Message or CallbackQuery,
                 text : str,
-                alert : bool = False,
+                cb : bool = False,
                 filter : Filter = False
                 ):
-     if not isinstance(alert,bool):
-        print("Parameter alert must be Boolean (True or False)")
+     if not isinstance(cb,bool):
+        print("Parameter cb must be Boolean (True or False)")
         return errors.basic
-     if (alert and (not isinstance(msg,CallbackQuery))) or ((not alert) and (not isinstance(msg,Message))):
-        if alert:
+     if (cb and (not isinstance(msg,CallbackQuery))) or ((not cb) and (not isinstance(msg,Message))):
+        if cb:
          print("Parameter msg must be CallbackQuery object")
          return errors.basic
         else:
          print("Parameter msg must be Message object")
          return errors.basic      
      if not isinstance(text,str):
         print("Parameter text must be str")
@@ -66,15 +66,15 @@
              else:
                  anonymous = True
                  user_id = msg.sender_chat.id
          except Exception as e:
              logging.info(e)
              user_id = None
          if user_id:
-             if alert:
+             if cb:
                  uv = await self.client.send_message(chat_id=msg.message.chat.id,
                                                      text=text,
                                                      reply_markup=ForceReply(
                                                                              selective = True,
                                                                              placeholder = self.placeholder
                                                                             )
                                                      )
```

### Comparing `Askpyro-1.73.1/askpyro/errors.py` & `Askpyro-1.73.2/askpyro/errors.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from pyrogram.types import ForceReply
 import asyncio
 import logging
 
 class errors:
    class timeout:
-     code,text,cancel,unknown,alert,basic = 101,None,False,False,False,False 
+     code,text,cancel,unknown,cb,basic = 101,None,False,False,False,False 
      timeout = error = "[100] Time Out ..!"
    class cancel:
-     code,text,timeout,unknown,alert,basic = 102,None,False,False,False,False 
+     code,text,timeout,unknown,cb,basic = 102,None,False,False,False,False 
      cancel = error = "[102] Listening cancelled...!"
    class unknown:
-     code,text,timeout,cancel,alert,basic = 103,None,False,False,False,False 
+     code,text,timeout,cancel,cb,basic = 103,None,False,False,False,False 
      error = unknown = "[103] Unknown Error...!"
-   class alert:
+   class cb:
      code,text,timeout,cancel,unknown,basic = 104,None,False,False,False,False 
-     error = alert = "[104] Expected a callback query...!"
+     error = cb = "[104] Expected a callback query...!"
    class basic:
       error = basic = "Parameter type Invalid check again...!"
-      code,text,timeout,cancel,alert,unknown = 105,None,False,False,False,False
+      code,text,timeout,cancel,cb,unknown = 105,None,False,False,False,False
```

### Comparing `Askpyro-1.73.1/askpyro/helpers/__init__.py` & `Askpyro-1.73.2/askpyro/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `Askpyro-1.73.1/askpyro/helpers/helpers.py` & `Askpyro-1.73.2/askpyro/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `Askpyro-1.73.1/askpyro/helpers/parser.py` & `Askpyro-1.73.2/askpyro/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `Askpyro-1.73.1/examples/buttons.py` & `Askpyro-1.73.2/examples/buttons.py`

 * *Files identical despite different names*

### Comparing `Askpyro-1.73.1/setup.py` & `Askpyro-1.73.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Askpyro.  If not, see <http://www.gnu.org/licenses/>.
 
+# ===================================================================
+
 import re
 from sys import argv
 import setuptools
 
 
 
 with open("README.md", encoding="utf8") as readme:
@@ -30,15 +32,15 @@
     with open(file, encoding="utf-8") as r:
         return [i.strip() for i in r]
 """
 
 setuptools.setup(
     name="Askpyro",
     packages=setuptools.find_packages(),
-    version="1.73.1",
+    version="1.73.2",
     description="Easy conversation handler for pyrogram",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Abishnoi69",
     download_url="https://github.com/Abishnoi69/Askpyro/releases/latest",
     author="Abishnoi",
     author_email="abishnoi@askpyro.org",
@@ -62,15 +64,15 @@
         "Topic :: Internet",
         "Topic :: Communications",
         "Topic :: Communications :: Chat",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Libraries :: Application Frameworks"
     ],
-    keywords="telegram chat messenger mtproto api client library python",
+    keywords="telegram chat messenger mtproto api client library python conversation",
     project_urls={
         "Tracker": "https://github.com/Abishnoi69/Askpyro/issues",
         "Community": "https://t.me/AbishnoiMF",
         "Source": "https://github.com/Abishnoi69/Askpyro",
         "Documentation": "https://github.com/Abishnoi69/askpyro/wiki",
     },
     python_requires="~=3.7",
```

