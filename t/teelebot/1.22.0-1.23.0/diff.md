# Comparing `tmp/teelebot-1.22.0-py3-none-any.whl.zip` & `tmp/teelebot-1.23.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 50060 bytes, number of entries: 18
--rw-rw-rw-  2.0 fat     3966 b- defN 22-Dec-22 03:24 teelebot/__init__.py
+Zip file size: 50456 bytes, number of entries: 18
+-rw-rw-rw-  2.0 fat     3990 b- defN 23-Apr-11 12:57 teelebot/__init__.py
 -rw-rw-rw-  2.0 fat      163 b- defN 21-Sep-11 03:28 teelebot/__main__.py
 -rw-rw-rw-  2.0 fat     7352 b- defN 21-Sep-11 03:28 teelebot/buffer.py
--rw-rw-rw-  2.0 fat    18917 b- defN 21-Oct-02 23:43 teelebot/handler.py
+-rw-rw-rw-  2.0 fat    19293 b- defN 23-Apr-11 13:11 teelebot/handler.py
 -rw-rw-rw-  2.0 fat     1808 b- defN 21-Sep-11 03:28 teelebot/logger.py
 -rw-rw-rw-  2.0 fat      619 b- defN 22-Aug-14 05:17 teelebot/polling.py
--rw-rw-rw-  2.0 fat     4156 b- defN 22-Dec-24 12:06 teelebot/request.py
+-rw-rw-rw-  2.0 fat     4304 b- defN 23-Apr-11 13:55 teelebot/request.py
 -rw-rw-rw-  2.0 fat     3876 b- defN 21-Sep-11 03:28 teelebot/schedule.py
--rw-rw-rw-  2.0 fat   125013 b- defN 23-Feb-14 05:18 teelebot/teelebot.py
--rw-rw-rw-  2.0 fat      478 b- defN 23-Feb-14 05:05 teelebot/version.py
+-rw-rw-rw-  2.0 fat   125830 b- defN 23-Apr-18 02:19 teelebot/teelebot.py
+-rw-rw-rw-  2.0 fat      478 b- defN 23-Apr-18 02:19 teelebot/version.py
 -rw-rw-rw-  2.0 fat     2665 b- defN 22-Aug-14 10:03 teelebot/webhook.py
--rw-rw-rw-  2.0 fat    35823 b- defN 23-Feb-14 05:44 teelebot-1.22.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    14660 b- defN 23-Feb-14 05:44 teelebot-1.22.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Feb-14 05:44 teelebot-1.22.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       43 b- defN 23-Feb-14 05:44 teelebot-1.22.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-Feb-14 05:44 teelebot-1.22.0.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Feb-14 05:44 teelebot-1.22.0.dist-info/zip-safe
-?rw-rw-r--  2.0 fat     1420 b- defN 23-Feb-14 05:44 teelebot-1.22.0.dist-info/RECORD
-18 files, 221062 bytes uncompressed, 47758 bytes compressed:  78.4%
+-rw-rw-rw-  2.0 fat    35823 b- defN 23-Apr-18 02:32 teelebot-1.23.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    14712 b- defN 23-Apr-18 02:32 teelebot-1.23.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-18 02:32 teelebot-1.23.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       43 b- defN 23-Apr-18 02:32 teelebot-1.23.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-18 02:32 teelebot-1.23.0.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-18 02:32 teelebot-1.23.0.dist-info/zip-safe
+-rw-rw-r--  2.0 fat     1420 b- defN 23-Apr-18 02:32 teelebot-1.23.0.dist-info/RECORD
+18 files, 222479 bytes uncompressed, 48154 bytes compressed:  78.4%
```

## zipnote {}

```diff
@@ -27,29 +27,29 @@
 
 Filename: teelebot/version.py
 Comment: 
 
 Filename: teelebot/webhook.py
 Comment: 
 
-Filename: teelebot-1.22.0.dist-info/LICENSE
+Filename: teelebot-1.23.0.dist-info/LICENSE
 Comment: 
 
-Filename: teelebot-1.22.0.dist-info/METADATA
+Filename: teelebot-1.23.0.dist-info/METADATA
 Comment: 
 
-Filename: teelebot-1.22.0.dist-info/WHEEL
+Filename: teelebot-1.23.0.dist-info/WHEEL
 Comment: 
 
-Filename: teelebot-1.22.0.dist-info/entry_points.txt
+Filename: teelebot-1.23.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: teelebot-1.22.0.dist-info/top_level.txt
+Filename: teelebot-1.23.0.dist-info/top_level.txt
 Comment: 
 
-Filename: teelebot-1.22.0.dist-info/zip-safe
+Filename: teelebot-1.23.0.dist-info/zip-safe
 Comment: 
 
-Filename: teelebot-1.22.0.dist-info/RECORD
+Filename: teelebot-1.23.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## teelebot/__init__.py

```diff
@@ -1,11 +1,11 @@
 # -*- coding:utf-8 -*-
 """
 @creation date: 2019-08-23
-@last modification: 2022-08-14
+@last modification: 2023-04-11
 """
 import os
 import requests
 import urllib3
 
 from .polling import _runUpdates
 from .webhook import _runWebhook
@@ -30,17 +30,17 @@
         "    __            __     __          __  " + "\n" + \
         "   / /____  ___  / /__  / /_  ____  / /_ " + "\n" + \
         "  / __/ _ \/ _ \/ / _ \/ __ \/ __ \/ __/ " + "\n" + \
         " / /_/  __/  __/ /  __/ /_/ / /_/ / /_   " + "\n" + \
         " \__/\___/\___/_/\___/_.___/\____/\__/   " + "\n"
     )
     print(" * Self-checking...", end="\r")
-    req = requests.post(url=bot._url + "getWebhookInfo", verify=False)
+    req = requests.post(url=bot._url + "getWebhookInfo", verify=False, proxies=bot._proxies)
     if not req.json().get("ok"):
-        if (req.json().get("error_code") == 401 and
+        if (req.json().get("error_code") == 401 and \
             req.json().get("description") == "Unauthorized"):
             print("\nif you already logout the bot from the cloud Bot API server,please wait at least 10 minutes and try again.")
         else:
             print("\nfailed to get running mode!")
         os._exit(0)
 
     status = req.json().get("result")
```

## teelebot/handler.py

```diff
@@ -1,11 +1,11 @@
 # -*- coding:utf-8 -*-
 '''
 @creation date: 2019-08-23
-@last modification: 2021-10-03
+@last modification: 2023-04-11
 '''
 import configparser
 import argparse
 import os
 import sys
 import shutil
 import requests
@@ -94,15 +94,16 @@
                 "webhook = False" + "\n",
                 "self_signed = False" + "\n",
                 "cert_key = " + "\n",
                 "cert_pub = " + "\n",
                 "server_address = " + "\n",
                 "server_port = " + "\n",
                 "local_address = " + "\n",
-                "local_port = "
+                "local_port = " + "\n",
+                "proxy = "
             ])
             print("the configuration file has been created automatically.")
             print("configuration file path: " + str(config_dir))
         if not args.key or not args.root:
             print("please modify the relevant parameters and restart the teelebot.")
             os._exit(0)
         # else:
@@ -340,14 +341,23 @@
         config["webhook"] = True
     elif config["webhook"] == "False":
         config["webhook"] = False
     else:
         print("The webhook field value in the configuration file is wrong.")
         os._exit(0)
 
+    if "proxy" in config.keys():
+        if str(config["proxy"]).strip() == "" or str(config["proxy"]).strip() == None:
+            config["proxies"] = {"all": None}
+        else:
+            config["proxies"] = {"all": str(config["proxy"]).strip()}
+        config.pop("proxy")
+    else:
+        config["proxies"] = {"all": None}
+
     config["author"] = __author__
     config["version"] = __version__
     config["plugin_dir"] = plugin_dir
     config["plugin_bridge"], config["non_plugin_list"] = _bridge(config["plugin_dir"])
     config["plugin_info"] = _plugin_info(
         config["plugin_bridge"].keys(), config["plugin_dir"])
     config["non_plugin_info"] = _plugin_info(
```

## teelebot/request.py

```diff
@@ -1,41 +1,44 @@
 # -*- coding:utf-8 -*-
 '''
 @creation date: 2019-11-15
-@last modification: 2021-09-11
+@last modification: 2023-04-11
 '''
 import os
 
 import requests
 import inspect
 from .logger import _logger
 from traceback import extract_stack
 
-
 class _Request(object):
     """
     接口请求类
     """
-    def __init__(self, thread_pool_size, url, debug=False):
+    def __init__(self, thread_pool_size, url, debug=False, proxies={"all": None}):
         self.__url = url
         self.__debug = debug
+        self.__proxies = proxies
         self.__session = self.__connection_session(
             pool_connections=thread_pool_size,
             pool_maxsize=thread_pool_size * 2
         )
 
     def __del__(self):
         self.__session.close()
 
     def __connection_session(self, pool_connections=10, pool_maxsize=10, max_retries=5):
         """
         连接池
         """
         session = requests.Session()
         session.verify = False
+        session.trust_env = False
+        session.proxies.update(self.__proxies)
+        
 
         adapter = requests.adapters.HTTPAdapter(pool_connections=pool_connections,
                                                 pool_maxsize=pool_maxsize, max_retries=max_retries)
         session.mount('http://', adapter)
         session.mount('https://', adapter)
 
         return session
```

## teelebot/teelebot.py

```diff
@@ -1,14 +1,14 @@
 # -*- coding:utf-8 -*-
 """
 @description:基于Telegram Bot Api 的机器人框架
 @creation date: 2019-08-13
-@last modification: 2023-02-14
+@last modification: 2023-04-18
 @author: Pluto (github:plutobell)
-@version: 1.22.0
+@version: 1.23.0
 """
 import inspect
 import time
 import sys
 import os
 import json
 import string
@@ -34,14 +34,16 @@
     def __init__(self, key=""):
         config = _config()
 
         if key != "":
             self._key = key
         elif key == "":
             self._key = config["key"]
+        
+        self._proxies = config["proxies"]
 
         self._cloud_api_server = config["cloud_api_server"]
         self._local_api_server = config["local_api_server"]
         if self._local_api_server != "False":
             self._basic_url = config["local_api_server"]
         else:
             self._basic_url = self._cloud_api_server
@@ -96,15 +98,15 @@
         self.__start_time = int(time.time())
         self.__response_times = 0
         self.__response_chats = []
         self.__response_users = []
 
         thread_pool_size = round(int(self._pool_size) * 2 / 3)
         schedule_queue_size = int(self._pool_size) - thread_pool_size
-        self.request = _Request(thread_pool_size, self._url, self._debug)
+        self.request = _Request(thread_pool_size, self._url, self._debug, self._proxies)
         self.schedule = _Schedule(schedule_queue_size)
         self.buffer = _Buffer(int(self._buffer_size) * 1024 * 1024,
             self.__plugin_bridge.keys(), self.__plugin_dir)
 
         self.__thread_pool = ThreadPoolExecutor(
             max_workers=thread_pool_size)
         self.__timer_thread_pool = ThreadPoolExecutor(
@@ -845,34 +847,62 @@
             addr += "&message_thread_id=" + str(message_thread_id)
 
         if file_data is None:
             return self.request.post(addr)
         else:
             return self.request.postFile(addr, file_data)
 
-    def sendAnimation(self, chat_id, animation, caption=None, parse_mode="Text", reply_to_message_id=None,
-        reply_markup=None, allow_sending_without_reply=None, caption_entities=None,
-        protect_content=None, message_thread_id=None, has_spoiler=None):
+
+    def sendAnimation(self, chat_id, animation, message_thread_id=None, duration=None,
+        width=None, height=None, thumbnail=None, caption=None, parse_mode=None,
+        caption_entities=None, has_spoiler=None, disable_notification=None,
+        protect_content=None, reply_to_message_id=None, allow_sending_without_reply=None,
+        reply_markup=None):
         """
-        发送动画 gif/mp4
+        使用此方法发送动画文件（GIF或H.264/MPEG-4 AVC视频，无声音）
+        目前，机器人可以发送大小为50MB的动画文件，这个限制在未来可能会被改变
         """
         command = inspect.stack()[0].function
+        file_data = {}
         if animation[:7] == "http://" or animation[:7] == "https:/":
             file_data = None
             addr = command + "?chat_id=" + str(chat_id) + "&animation=" + animation
         elif type(animation) == bytes:
             file_data = {"animation": animation}
             addr = command + "?chat_id=" + str(chat_id)
         elif type(animation) == str and '.' not in animation:
             file_data = None
             addr = command + "?chat_id=" + str(chat_id) + "&animation=" + animation
         else:
             file_data = {"animation": open(animation, 'rb')}
             addr = command + "?chat_id=" + str(chat_id)
 
+        if thumbnail[:7] == "http://" or thumbnail[:7] == "https:/":
+            addr += "&thumbnail=" + thumbnail
+        elif type(thumbnail) == bytes:
+            if file_data is None:
+                file_data = {"thumbnail": thumbnail}
+            else:
+                file_data["thumbnail"] = thumbnail
+        elif type(thumbnail) == str and '.' not in thumbnail:
+            addr += "&thumbnail=" + thumbnail
+        else:
+            if file_data is None:
+                file_data = {"thumbnail": open(thumbnail, 'rb')}
+            else:
+                file_data["thumbnail"] = open(thumbnail, 'rb')
+
+        if duration is not None:
+            addr += "&duration=" + quote(duration)
+        if width is not None:
+            addr += "&width=" + quote(width)
+        if height is not None:
+            addr += "&height=" + quote(height)
+        if disable_notification is not None:
+            addr += "&disable_notification=" + quote(disable_notification)
         if caption is not None:
             addr += "&caption=" + quote(caption)
         if parse_mode in ("Markdown", "MarkdownV2", "HTML"):
             addr += "&parse_mode" + parse_mode
         if reply_to_message_id is not None:
             addr += "&reply_to_message_id=" + str(reply_to_message_id)
         if reply_markup is not None:
@@ -889,34 +919,57 @@
             addr += "&has_spoiler=" + str(has_spoiler)
 
         if file_data is None:
             return self.request.post(addr)
         else:
             self.request.postFile(addr, file_data)
 
-    def sendAudio(self, chat_id, audio, caption=None, parse_mode="Text", title=None, reply_to_message_id=None,
-        reply_markup=None, allow_sending_without_reply=None, caption_entities=None,
-        protect_content=None, message_thread_id=None):
+    def sendAudio(self, chat_id, audio, message_thread_id=None, caption=None,
+        parse_mode=None, caption_entities=None, duration=None, performer=None, title=None,
+        thumbnail=None, disable_notification=None, protect_content=None,
+        reply_to_message_id=None, allow_sending_without_reply=None, reply_markup=None):
         """
-        发送音频 mp3
+        使用此方法发送音频文件
         """
         command = inspect.stack()[0].function
+        file_data = {}
         if audio[:7] == "http://" or audio[:7] == "https:/":
             file_data = None
             addr = command + "?chat_id=" + str(chat_id) + "&audio=" + audio
         elif type(audio) == bytes:
             file_data = {"audio": audio}
             addr = command + "?chat_id=" + str(chat_id)
         elif type(audio) == str and '.' not in audio:
             file_data = None
             addr = command + "?chat_id=" + str(chat_id) + "&audio=" + audio
         else:
             file_data = {"audio": open(audio, 'rb')}
             addr = command + "?chat_id=" + str(chat_id)
 
+        if thumbnail[:7] == "http://" or thumbnail[:7] == "https:/":
+            addr += "&thumbnail=" + thumbnail
+        elif type(thumbnail) == bytes:
+            if file_data is None:
+                file_data = {"thumbnail": thumbnail}
+            else:
+                file_data["thumbnail"] = thumbnail
+        elif type(thumbnail) == str and '.' not in thumbnail:
+            addr += "&thumbnail=" + thumbnail
+        else:
+            if file_data is None:
+                file_data = {"thumbnail": open(thumbnail, 'rb')}
+            else:
+                file_data["thumbnail"] = open(thumbnail, 'rb')
+
+        if duration is not None:
+            addr += "&duration=" + quote(duration)
+        if performer is not None:
+            addr += "&performer=" + quote(performer)
+        if disable_notification is not None:
+            addr += "&disable_notification=" + quote(disable_notification)
         if caption is not None:
             addr += "&caption=" + quote(caption)
         if parse_mode in ("Markdown", "MarkdownV2", "HTML"):
             addr += "&parse_mode" + parse_mode
         if title is not None:
             addr += "&title=" + title
         if reply_to_message_id is not None:
@@ -977,34 +1030,62 @@
             addr += "&has_spoiler=" + str(has_spoiler)
 
         if file_data is None:
             return self.request.post(addr)
         else:
             return self.request.postFile(addr, file_data)
 
-    def sendVideo(self, chat_id, video, caption=None, parse_mode="Text", reply_to_message_id=None,
-        reply_markup=None, allow_sending_without_reply=None, caption_entities=None,
-        protect_content=None, message_thread_id=None, has_spoiler=None):
+    def sendVideo(self, chat_id, video, message_thread_id=None, duration=None, width=None,
+        height=None, thumbnail=None, caption=None, parse_mode=None, caption_entities=None,
+        has_spoiler=None, supports_streaming=None, disable_notification=None,
+        protect_content=None, reply_to_message_id=None, allow_sending_without_reply=None,
+        reply_markup=None):
         """
         发送视频
         """
         command = inspect.stack()[0].function
+        file_data = {}
         if video[:7] == "http://" or video[:7] == "https:/":
             file_data = None
             addr = command + "?chat_id=" + str(chat_id) + "&video=" + video
         elif type(video) == bytes:
             file_data = {"video": video}
             addr = command + "?chat_id=" + str(chat_id)
         elif type(video) == str and '.' not in video:
             file_data = None
             addr = command + "?chat_id=" + str(chat_id) + "&video=" + video
         else:
             file_data = {"video": open(video, 'rb')}
             addr = command + "?chat_id=" + str(chat_id)
 
+        if thumbnail[:7] == "http://" or thumbnail[:7] == "https:/":
+            addr += "&thumbnail=" + thumbnail
+        elif type(thumbnail) == bytes:
+            if file_data is None:
+                file_data = {"thumbnail": thumbnail}
+            else:
+                file_data["thumbnail"] = thumbnail
+        elif type(thumbnail) == str and '.' not in thumbnail:
+            addr += "&thumbnail=" + thumbnail
+        else:
+            if file_data is None:
+                file_data = {"thumbnail": open(thumbnail, 'rb')}
+            else:
+                file_data["thumbnail"] = open(thumbnail, 'rb')
+
+        if duration is not None:
+            addr += "&duration=" + quote(duration)
+        if width is not None:
+            addr += "&width=" + quote(width)
+        if height is not None:
+            addr += "&height=" + quote(height)
+        if disable_notification is not None:
+            addr += "&disable_notification=" + quote(disable_notification)
+        if supports_streaming is not None:
+            addr += "&supports_streaming=" + quote(supports_streaming)
         if caption is not None:
             addr += "&caption=" + quote(caption)
         if parse_mode in ("Markdown", "MarkdownV2", "HTML"):
             addr += "&parse_mode=" + parse_mode
         if reply_to_message_id is not None:
             addr += "&reply_to_message_id=" + str(reply_to_message_id)
         if reply_markup is not None:
@@ -1021,39 +1102,57 @@
             addr += "&has_spoiler=" + str(has_spoiler)
 
         if file_data is None:
             return self.request.post(addr)
         else:
             return self.request.postFile(addr, file_data)
 
-    def sendVideoNote(self, chat_id, video_note, caption=None, parse_mode="Text",
-        reply_to_message_id=None, reply_markup=None,allow_sending_without_reply=None,
-        protect_content=None, message_thread_id=None):
+    def sendVideoNote(self, chat_id, video_note, message_thread_id=None, duration=None,
+        length=None, thumbnail=None, disable_notification=None, protect_content=None,
+        reply_to_message_id=None, allow_sending_without_reply=None, reply_markup=None):
         """
         发送圆形或方形视频？
         """
         command = inspect.stack()[0].function
+        file_data = {}
         char_id_str = str(chat_id)
         if video_note[:7] == "http://" or video_note[:7] == "https:/":
             file_data = None
             addr = command + "?chat_id=" + char_id_str + "&video_note=" + video_note
         elif type(video_note) == bytes:
             file_data = {"video_note": video_note}
             addr = command + "?chat_id=" + char_id_str
         elif type(video_note) == str and '.' not in video_note:
             file_data = None
             addr = command + "?chat_id=" + char_id_str + "&video_note=" + video_note
         else:
             file_data = {"video_note": open(video_note, 'rb')}
             addr = command + "?chat_id=" + char_id_str
 
-        if caption is not None:
-            addr += "&caption=" + quote(caption)
-        if parse_mode in ("Markdown", "MarkdownV2", "HTML"):
-            addr += "&parse_mode=" + parse_mode
+        if thumbnail[:7] == "http://" or thumbnail[:7] == "https:/":
+            addr += "&thumbnail=" + thumbnail
+        elif type(thumbnail) == bytes:
+            if file_data is None:
+                file_data = {"thumbnail": thumbnail}
+            else:
+                file_data["thumbnail"] = thumbnail
+        elif type(thumbnail) == str and '.' not in thumbnail:
+            addr += "&thumbnail=" + thumbnail
+        else:
+            if file_data is None:
+                file_data = {"thumbnail": open(thumbnail, 'rb')}
+            else:
+                file_data["thumbnail"] = open(thumbnail, 'rb')
+
+        if duration is not None:
+            addr += "&duration=" + quote(duration)
+        if length is not None:
+            addr += "&length=" + quote(length)
+        if disable_notification is not None:
+            addr += "&disable_notification=" + quote(disable_notification)
         if reply_to_message_id is not None:
             addr += "&reply_to_message_id=" + str(reply_to_message_id)
         if reply_markup is not None:
             addr += "&reply_markup=" + json.dumps(reply_markup)
         if allow_sending_without_reply is not None:
             addr += "&allow_sending_without_reply=" + str(allow_sending_without_reply)
         if protect_content is not None:
@@ -1118,35 +1217,54 @@
         if protect_content is not None:
             addr += "&protect_content=" + str(protect_content)
         if message_thread_id is not None:
             addr += "&message_thread_id=" + str(message_thread_id)
 
         return self.request.postJson(addr, medias)
 
-    def sendDocument(self, chat_id, document, caption=None, parse_mode="Text",
-        reply_to_message_id=None, reply_markup=None, disable_content_type_detection=None,
-        allow_sending_without_reply=None, caption_entities=None,
-        protect_content=None, message_thread_id=None):
+    def sendDocument(self, chat_id, document, message_thread_id=None, thumbnail=None,
+        caption=None, parse_mode=None, caption_entities=None,
+        disable_content_type_detection=None, disable_notification=None,
+        protect_content=None, reply_to_message_id=None, allow_sending_without_reply=None,
+        reply_markup=None):
         """
         发送文件
         """
         command = inspect.stack()[0].function
+        file_data = {}
         if document[:7] == "http://" or document[:7] == "https:/":
             file_data = None
             addr = command + "?chat_id=" + str(chat_id) + "&document=" + document
         elif type(document) == bytes:
             file_data = {"document": document}
             addr = command + "?chat_id=" + str(chat_id)
         elif type(document) == str and '.' not in document:
             file_data = None
             addr = command + "?chat_id=" + str(chat_id) + "&document=" + document
         else:
             file_data = {"document": open(document, 'rb')}
             addr = command + "?chat_id=" + str(chat_id)
 
+        if thumbnail[:7] == "http://" or thumbnail[:7] == "https:/":
+            addr += "&thumbnail=" + thumbnail
+        elif type(thumbnail) == bytes:
+            if file_data is None:
+                file_data = {"thumbnail": thumbnail}
+            else:
+                file_data["thumbnail"] = thumbnail
+        elif type(thumbnail) == str and '.' not in thumbnail:
+            addr += "&thumbnail=" + thumbnail
+        else:
+            if file_data is None:
+                file_data = {"thumbnail": open(thumbnail, 'rb')}
+            else:
+                file_data["thumbnail"] = open(thumbnail, 'rb')
+
+        if disable_notification is not None:
+            addr += "&disable_notification=" + quote(disable_notification)
         if caption is not None:
             addr += "&caption=" + quote(caption)
         if parse_mode in ("Markdown", "MarkdownV2", "HTML"):
             addr += "&parse_mode=" + parse_mode
         if reply_to_message_id is not None:
             addr += "&reply_to_message_id=" + str(reply_to_message_id)
         if reply_markup is not None:
@@ -1840,64 +1958,14 @@
         为一个超级群组设置贴纸集
         """
         command = inspect.stack()[0].function
         addr = command + "?chat_id=" + str(chat_id) + "&sticker_set_name=" + str(sticker_set_name)
 
         return self.request.post(addr)
 
-    def addStickerToSet(self, user_id, name, emojis,
-        png_sticker=None, tgs_sticker=None, mask_position=None):
-        """
-        使用此方法在机器人创建的集合中添加一个新贴纸。
-        必须使用png标签或tgs标签中的一个字段。
-        动画贴纸只能添加到动画贴纸组中。
-        动画贴纸组最多可以有50个贴纸。
-        静态贴纸组最多可以有120个贴纸。
-        """
-        command = inspect.stack()[0].function
-        addr = command + "?user_id=" + str(user_id) + "&name=" + str(name) \
-            + "&emoji=" + str(emoji)
-
-        if png_sticker is not None and tgs_sticker is not None:
-            return False
-        elif png_sticker is None and tgs_sticker is None:
-            return False
-        else:
-            if png_sticker is not None:
-                if png_sticker[:7] == "http://" or png_sticker[:7] == "https:/":
-                    file_data = None
-                    addr = command + "?chat_id=" + str(chat_id) + "&png_sticker=" + png_sticker
-                elif type(png_sticker) == bytes:
-                    file_data = {"png_sticker": png_sticker}
-                    addr = command + "?chat_id=" + str(chat_id)
-                elif type(png_sticker) == str and '.' not in png_sticker:
-                    file_data = None
-                    addr = command + "?chat_id=" + str(chat_id) + "&png_sticker=" + png_sticker
-                else:
-                    file_data = {"png_sticker": open(png_sticker, 'rb')}
-                    addr = command + "?chat_id=" + str(chat_id)
-            elif tgs_sticker is not None:
-                if tgs_sticker[:7] == "http://" or tgs_sticker[:7] == "https:/":
-                    file_data = None
-                    addr = command + "?chat_id=" + str(chat_id) + "&tgs_sticker=" + tgs_sticker
-                elif type(png_sticker) == bytes:
-                    file_data = {"tgs_sticker": tgs_sticker}
-                    addr = command + "?chat_id=" + str(chat_id)
-                elif type(tgs_sticker) == str and '.' not in tgs_sticker:
-                    file_data = None
-                    addr = command + "?chat_id=" + str(chat_id) + "&tgs_sticker=" + tgs_sticker
-                else:
-                    file_data = {"tgs_sticker": open(tgs_sticker, 'rb')}
-                    addr = command + "?chat_id=" + str(chat_id)
-
-            if file_data is None:
-                return self.request.post(addr)
-            else:
-                return self.request.postFile(addr, file_data)
-
     def deleteChatStickerSet(self, chat_id):
         """
         删除超级群组的贴纸集
         """
         command = inspect.stack()[0].function
         addr = command + "?chat_id=" + str(chat_id)
 
@@ -2028,14 +2096,62 @@
             data["language_code"] = str(language_code)
 
         if len(data) != 0:
             return self.request.postJson(addr, data)
         else:
             return self.request.post(addr)
 
+    def setMyDescription(self, description="", language_code=None):
+        """
+        使用此方法改变机器人的描述
+        """
+        command = inspect.stack()[0].function
+        addr = command + "?description=" + str(description)
+        
+        if language_code is not None:
+            addr += "&language_code=" + str(language_code)
+        
+        return self.request.post(addr)
+
+    def getMyDescription(self, language_code=None):
+        """
+        使用此方法来获得当前的机器人描述
+        """
+        command = inspect.stack()[0].function
+        addr = command
+
+        if language_code is not None:
+            addr += "?language_code=" + str(language_code)
+        
+        return self.request.post(addr)
+
+    def setMyShortDescription(self, short_description="", language_code=None):
+        """
+        使用这种方法来改变机器人的简短描述
+        """
+        command = inspect.stack()[0].function
+        addr = command + "?short_description=" + str(short_description)
+        
+        if language_code is not None:
+            addr += "&language_code=" + str(language_code)
+        
+        return self.request.post(addr)
+
+    def getMyShortDescription(self, language_code=None):
+        """
+        使用此方法获得当前的机器人简短描述
+        """
+        command = inspect.stack()[0].function
+        addr = command
+
+        if language_code is not None:
+            addr += "?&language_code=" + str(language_code)
+        
+        return self.request.post(addr)
+
     def setChatMenuButton(self, chat_id=None, menu_button=None):
         """
         使用此方法在私人聊天中更改机器人的菜单按钮或默认菜单按钮
 
         menu_button传入格式示例：
             menu_button = {
                 "type": "web_app",  # 类型只能是 default | command | web_app
@@ -2543,15 +2659,15 @@
         data["web_app_query_id"] = str(web_app_query_id)
         data["result"] = result
         
         return self.request.postJson(addr, data)
     
 
     # Stickers
-    def sendSticker(self, chat_id, sticker, disable_notification=None,
+    def sendSticker(self, chat_id, sticker, emoji=None, disable_notification=None,
         reply_to_message_id=None, reply_markup=None, allow_sending_without_reply=None,
         protect_content=None, message_thread_id=None):
         """
         使用此方法发送静态、webp或动画、tgs贴纸
         """
         command = inspect.stack()[0].function
 
@@ -2564,14 +2680,16 @@
         elif type(sticker) == str and '.' not in sticker:
             file_data = None
             addr = command + "?chat_id=" + str(chat_id) + "&sticker=" + sticker
         else:
             file_data = {"sticker": open(sticker, 'rb')}
             addr = command + "?chat_id=" + str(chat_id)
 
+        if emoji is not None:
+            addr += "&emoji=" + str(emoji)
         if disable_notification is not None:
             addr += "&disable_notification=" + str(disable_notification)
         if reply_to_message_id is not None:
             addr += "&reply_to_message_id=" + str(reply_to_message_id)
         if reply_markup is not None:
             addr += "&reply_markup=" + json.dumps(reply_markup)
         if allow_sending_without_reply is not None:
@@ -2603,175 +2721,56 @@
         command = inspect.stack()[0].function
         addr = command
         data = {}
         data["custom_emoji_ids"] = custom_emoji_ids
 
         return self.request.postJson(addr, data)
 
-
-    def uploadStickerFile(self, user_id, name, title, emojis,
-        png_sticker=None, tgs_sticker=None, contains_masks=None,
-        mask_position=None):
+    def uploadStickerFile(self, user_id, sticker, sticker_format):
         """
-        使用此方法可以上传带有标签的.PNG文件
-        以供以后在createNewStickerSet和addStickerToSet方法中使用
-        （可以多次使用）
+        使用此方法上传一个带有贴纸的文件
+        以便以后在createNewStickerSet和addStickerToSet方法中使用（该文件可以多次使用）
+        成功时返回上传的文件
         """
         command = inspect.stack()[0].function
+        addr = command + "?user_id=" + str(user_id)
+        addr += "&sticker_format=" + str(sticker_format)
+        
+        return self.request.postFile(addr, sticker)
 
-        user_id_str = str(user_id)
-        if png_sticker[:7] == "http://" or png_sticker[:7] == "https:/":
-            file_data = None
-            addr = command + "?user_id=" + user_id_str + "&png_sticker=" + png_sticker
-        elif type(png_sticker) == bytes:
-            file_data = {"png_sticker": png_sticker}
-            addr = command + "?user_id=" + user_id_str
-        elif type(png_sticker) == str and '.' not in png_sticker:
-            file_data = None
-            addr = command + "?user_id=" + user_id_str + "&png_sticker=" + png_sticker
-        else:
-            file_data = {"png_sticker": open(png_sticker, 'rb')}
-            addr = command + "?user_id=" + user_id_str
-
-        if file_data is None:
-            return self.request.post(addr)
-        else:
-            return self.request.postFile(addr, file_data)
-
-    def createNewStickerSet(self, user_id, name, title, emojis,
-        png_sticker=None, tgs_sticker=None, webm_sticker=None,
-        contains_masks=None, sticker_type=None, mask_position=None):
+    def createNewStickerSet(self, user_id, name, title, stickers, sticker_format,
+            sticker_type=None, needs_repainting=None):
         """
         使用此方法可以创建用户拥有的新贴纸集
         机器人将能够编辑由此创建的贴纸集
-        png_sticker、webm_sticker和tgs_sticker字段不能同时存在，有且只有一个
-
-        参数contains_masks已从方法createNewStickerSet的文档中删除,
-        为了向后兼容，该参数仍然有效，但新的应用请使用参数sticker_type代替。
         """
         command = inspect.stack()[0].function
         addr = command + "?user_id=" + str(user_id)
         addr += "&name=" + str(name)
         addr += "&title=" + str(title)
-        addr += "&emojis=" + str(emojis)
+        addr += "&sticker_format=" + str(sticker_format)
 
-        if png_sticker is None and tgs_sticker is None and webm_sticker is None:
-            return False
-        elif png_sticker is not None and tgs_sticker is not None \
-            and webm_sticker is not None:
-            return False
-        else:
-            if png_sticker is not None:
-                if png_sticker[:7] == "http://" or png_sticker[:7] == "https:/":
-                    file_data = None
-                    addr += "&png_sticker=" + png_sticker
-                elif type(png_sticker) == bytes:
-                    file_data = {"png_sticker": png_sticker}
-                elif type(png_sticker) == str and '.' not in png_sticker:
-                    file_data = None
-                    addr += "&png_sticker=" + png_sticker
-                else:
-                    file_data = {"png_sticker": open(png_sticker, 'rb')}
-            elif tgs_sticker is not None:
-                if tgs_sticker[:7] == "http://" or tgs_sticker[:7] == "https:/":
-                    file_data = None
-                    addr += "&tgs_sticker=" + tgs_sticker
-                elif type(tgs_sticker) == bytes:
-                    file_data = {"tgs_sticker": tgs_sticker}
-                elif type(tgs_sticker) == str and '.' not in tgs_sticker:
-                    file_data = None
-                    addr += "&tgs_sticker=" + tgs_sticker
-                else:
-                    file_data = {"tgs_sticker": open(tgs_sticker, 'rb')}
-            elif webm_sticker is not None:
-                if webm_sticker[:7] == "http://" or webm_sticker[:7] == "https:/":
-                    file_data = None
-                    addr += "&webm_sticker=" + webm_sticker
-                elif type(webm_sticker) == bytes:
-                    file_data = {"webm_sticker": webm_sticker}
-                elif type(webm_sticker) == str and '.' not in webm_sticker:
-                    file_data = None
-                    addr += "&webm_sticker=" + webm_sticker
-                else:
-                    file_data = {"webm_sticker": open(webms_sticker, 'rb')}
+        if sticker_type is not None:
+            addr += "&sticker_type=" + str(sticker_type)
+        if needs_repainting is not None:
+            addr += "&needs_repainting=" + str(needs_repainting)
 
-            if (contains_masks is not None) and (sticker_type is None):
-                sticker_type = contains_masks
-            if sticker_type is not None:
-                addr += "&sticker_type=" + str(sticker_type)
-                if mask_position is not None:
-                    addr += "&mask_position=" + json.dumps(mask_position)
-                else:
-                    return False
-
-            if file_data is None:
-                return self.request.post(addr)
-            else:
-                return self.request.postFile(addr, file_data)
+        return self.request.postJson(addr, stickers)
 
-    def addStickerToSet(self, user_id, name, emojis, png_sticker=None,
-        tgs_sticker=None, webm_sticker=None, smask_position=None):
+    def addStickerToSet(self, user_id, name, sticker):
         """
         使用此方法可以将新标签添加到由机器人创建的集合中
-        png_sticker、webm_sticker和tgs_sticker字段不能同时存在，有且只有一个
         可以将动画贴纸添加到动画贴纸集中，并且只能添加到它们
         动画贴纸集最多可以包含50个贴纸。 静态贴纸集最多可包含120个贴纸
         """
         command = inspect.stack()[0].function
         addr = command + "?user_id=" + str(user_id)
         addr += "&name=" + str(name)
-        addr += "&emojis=" + str(emojis)
 
-        if png_sticker is None and tgs_sticker is None and webm_sticker is None:
-            return False
-        elif png_sticker is not None and tgs_sticker is not None \
-            and webm_sticker is not None:
-            return False
-        else:
-            if png_sticker is not None:
-                if png_sticker[:7] == "http://" or png_sticker[:7] == "https:/":
-                    file_data = None
-                    addr += "&png_sticker=" + png_sticker
-                elif type(png_sticker) == bytes:
-                    file_data = {"png_sticker": png_sticker}
-                elif type(png_sticker) == str and '.' not in png_sticker:
-                    file_data = None
-                    addr += "&png_sticker=" + png_sticker
-                else:
-                    file_data = {"png_sticker": open(png_sticker, 'rb')}
-            elif tgs_sticker is not None:
-                if tgs_sticker[:7] == "http://" or tgs_sticker[:7] == "https:/":
-                    file_data = None
-                    addr += "&tgs_sticker=" + tgs_sticker
-                elif type(tgs_sticker) == bytes:
-                    file_data = {"tgs_sticker": tgs_sticker}
-                elif type(tgs_sticker) == str and '.' not in tgs_sticker:
-                    file_data = None
-                    addr += "&tgs_sticker=" + tgs_sticker
-                else:
-                    file_data = {"tgs_sticker": open(tgs_sticker, 'rb')}
-            elif webm_sticker is not None:
-                if webm_sticker[:7] == "http://" or webm_sticker[:7] == "https:/":
-                    file_data = None
-                    addr += "&webm_sticker=" + webm_sticker
-                elif type(webm_sticker) == bytes:
-                    file_data = {"webm_sticker": webm_sticker}
-                elif type(webm_sticker) == str and '.' not in webm_sticker:
-                    file_data = None
-                    addr += "&webm_sticker=" + webm_sticker
-                else:
-                    file_data = {"webm_sticker": open(webms_sticker, 'rb')}
-
-            if mask_position is not None:
-                addr += "&mask_position=" + json.dumps(mask_position)
-
-            if file_data is None:
-                return self.request.post(addr)
-            else:
-                return self.request.postFile(addr, file_data)
+        return self.request.postJson(addr, sticker)
 
     def setStickerPositionInSet(self, sticker, position):
         """
         使用此方法将机器人创建的一组贴纸移动到特定位置
         """
         command = inspect.stack()[0].function
         addr = command + "?sticker=" + str(sticker)
@@ -2784,39 +2783,104 @@
         使用此方法从机器人创建的集合中删除贴纸
         """
         command = inspect.stack()[0].function
         addr = command + "?sticker=" + str(sticker)
 
         return self.request.post(addr)
 
-    def setStickerSetThumb(self, name, user_id, thumb=None):
+    def setStickerSetThumbnail(self, name, user_id, thumbnail=None):
         """
         使用此方法设置贴纸集的缩略图
         只能为动画贴纸集设置动画缩略图
         """
         command = inspect.stack()[0].function
         addr = command + "?name=" + str(name)
         addr += "&user_id=" + str(user_id)
 
-        if thumb is not None:
-            if thumb[:7] == "http://" or thumb[:7] == "https:/":
+        if thumbnail is not None:
+            if thumbnail[:7] == "http://" or thumbnail[:7] == "https:/":
                 file_data = None
-                addr += "&thumb=" + thumb
-            elif type(thumb) == bytes:
-                file_data = {"thumb": thumb}
-            elif type(thumb) == str and '.' not in thumb:
+                addr += "&thumbnail=" + thumbnail
+            elif type(thumbnail) == bytes:
+                file_data = {"thumbnail": thumbnail}
+            elif type(thumbnail) == str and '.' not in thumbnail:
                 file_data = None
-                addr += "&thumb=" + thumb
+                addr += "&thumbnail=" + thumbnail
             else:
-                file_data = {"thumb": open(thumb, 'rb')}
+                file_data = {"thumbnail": open(thumbnail, 'rb')}
 
         if file_data is None:
             return self.request.post(addr)
         else:
             return self.request.postFile(addr, file_data)
+        
+    def setCustomEmojiStickerSetThumbnail(self, name, custom_emoji_id=""):
+        """
+        使用此方法来设置自定义表情贴纸集的缩略图
+        """
+        command = inspect.stack()[0].function
+        addr = command + "?name=" + str(name)
+        addr += "&custom_emoji_id=" + str(custom_emoji_id)
+
+        return self.request.post(addr)
+    
+    def setStickerSetTitle(self, name, title):
+        """
+        使用此方法来设置已创建的贴纸集的标题
+        """
+        command = inspect.stack()[0].function
+        addr = command + "?name=" + str(name)
+        addr += "&custom_emoji_id=" + str(title)
+
+        return self.request.post(addr)
+    
+    def deleteStickerSet(self, name):
+        """
+        使用此方法删除一个由机器人创建的贴纸集
+        """
+        command = inspect.stack()[0].function
+        addr = command + "?name=" + str(name)
+
+        return self.request.post(addr)
+    
+    def setStickerEmojiList(self, sticker, emoji_list):
+        """
+        使用这个方法来改变分配给普通或自定义表情贴纸的表情符号列表
+        该贴纸必须属于由机器人创建的贴纸集
+        """
+        command = inspect.stack()[0].function
+        addr = command + "?sticker=" + str(sticker)
+
+        return self.request.postJson(addr, emoji_list)
+    
+    def setStickerKeywords(self, sticker, keywords=None):
+        """
+        使用这种方法来改变分配给普通或自定义表情符号贴纸的搜索关键词
+        该贴纸必须属于由机器人创建的贴纸集
+        """
+        command = inspect.stack()[0].function
+        addr = command + "?sticker=" + str(sticker)
+
+        if keywords is not None:
+            return self.request.postJson(addr, keywords)
+        else:
+            return self.request.post(addr)
+        
+    def setStickerMaskPosition(self, sticker, mask_position=None):
+        """
+        使用这个方法来改变一个面具贴纸的面具位置
+        该贴纸必须属于一个由机器人创建的贴纸集
+        """
+        command = inspect.stack()[0].function
+        addr = command + "?sticker=" + str(sticker)
+
+        if mask_position is not None:
+            return self.request.postJson(addr, mask_position)
+        else:
+            return self.request.post(addr)
 
     # Payments
     def sendInvoice(self, chat_id, title, description, payload, provider_token,
                     currency, prices, start_parameter=None, provider_data=None, photo_url=None,
                     photo_size=None, photo_width=None, photo_height=None,
                     need_name=None, need_phone_number=None, need_email=None,
                     need_shipping_address=None, send_phone_number_to_provider=None,
```

## teelebot/version.py

```diff
@@ -1,15 +1,15 @@
 # -*- coding:utf-8 -*-
 """
 @description:基于Telegram Bot Api 的机器人框架
 @creation date: 2019-11-15
-@last modification: 2023-02-14
+@last modification: 2023-04-18
 @author: Pluto (github:plutobell)
-@version: 1.22.0
+@version: 1.23.0
 """
 
-__version__ = "1.22.0"
+__version__ = "1.23.0"
 __author__ = "Pluto"
 __email__ = "hi@ojoll.com"
 __blog__ = "https://ojoll.com"
 __github__ = "https://github.com/plutobell/teelebot"
 __description__ = "teelebot is a robot framework based on Telegram Bot API, with plug-in system, easy to extend."
```

## Comparing `teelebot-1.22.0.dist-info/LICENSE` & `teelebot-1.23.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `teelebot-1.22.0.dist-info/METADATA` & `teelebot-1.23.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teelebot
-Version: 1.22.0
+Version: 1.23.0
 Summary: teelebot is a robot framework based on Telegram Bot API, with plug-in system, easy to extend.
 Home-page: https://ojoll.com
 Author: Pluto
 Author-email: hi@ojoll.com
 License: GPLv3
 Keywords: teelebot telegram bot telegram bot api telegram
 Classifier: Programming Language :: Python :: 3
@@ -239,29 +239,30 @@
 
 **完整的配置文件**如下所示:
 
 ```python
 [config]
 key=bot key
 plugin_dir=your plugin dir
-pool_size=40 //the thread pool size, default 40, range(1, 101)
-buffer_size=16 //the buffer area size, default 16(MB)
+pool_size=40 # the thread pool size, default 40, range(1, 101)
+buffer_size=16 # the buffer area size, default 16(MB)
 webhook=False
-self_signed=False //Optional while webhook is False
-cert_key=your private cert path //Optional while webhook is False
-cert_pub=your public cert path //Optional while webhook is False
-server_ip=your server ip address //Optional while webhook is False
-server_port=your server port //Optional while webhook is False
-local_address=webhook local address //Optional while webhook is False
-local_port=webhook local port //Optional while webhook is False
+self_signed=False # Optional while webhook is False
+cert_key=your private cert path # Optional while webhook is False
+cert_pub=your public cert path # Optional while webhook is False
+server_ip=your server ip address # Optional while webhook is False
+server_port=your server port # Optional while webhook is False
+local_address=webhook local address # Optional while webhook is False
+local_port=webhook local port # Optional while webhook is False
 root_id=your user id
 debug=False
 drop_pending_updates=False
-local_api_server=local api server address //[Optional]
-updates_chat_member=False //[Optional]
+local_api_server=local api server address # [Optional]
+updates_chat_member=False # [Optional]
+proxy = socks5h://user:pass@host:port # [Optional]
 ```
 
 **在 `1.13.0` 及以上版本，支持自动生成配置文件。（默认为Polling模式）**
 
 1.在命令行未指定配置文件路径的情况下，会在默认配置文件路径下不存在配置文件时自动生成配置文件 `config.cfg`。
 
 * 在Linux下，会自动在用户目录下创建文件夹 `.teelebot` ，并生成配置文件 `config.cfg`
```

## Comparing `teelebot-1.22.0.dist-info/RECORD` & `teelebot-1.23.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-teelebot/__init__.py,sha256=YDmd03P5OPlxBmNGG2-wKzeZ9tVTBISBLw6Xi8E8u74,3966
+teelebot/__init__.py,sha256=EldJeJVnSdTl8FRjC4QCHJ9trFjt_9W_W_XeHHkkgvg,3990
 teelebot/__main__.py,sha256=SRKzFAyri9IQ-2Ox_xM3h_o9KrU4Qb2SikEGl-fhun8,163
 teelebot/buffer.py,sha256=YFYDSt7wQzko4Fuzg16PdwyjpXLpvBIK_ZHenv5gD4s,7352
-teelebot/handler.py,sha256=ItcfaBRNz5fENhmJpIBNmDSHEQyVQY_jdYgXWbYTUgE,18917
+teelebot/handler.py,sha256=GQPNT3IUvzdrQpF5_VKbjO_tXqpVhgtTjAR0IgimdRo,19293
 teelebot/logger.py,sha256=WALHg4p9zKuBTuI9ciND-8z-dZ04kVIwgdBmQx2lk0M,1808
 teelebot/polling.py,sha256=KyfGkXHUpPBkDzB2bQRZ8btJm0EOOXoTFZpRZS0b4nM,619
-teelebot/request.py,sha256=cgZXT4ep3aZJvUleBAwHTCgqNhHyqOTmDw8JfvS2xyo,4156
+teelebot/request.py,sha256=WntfQMyHqjGFtiekGx6O-YOZV9Ljqayvr0D1hsruNs8,4304
 teelebot/schedule.py,sha256=K5eecKJD-M9h_ZXqXMlgXlo3Bq8h6unqmTWt37LZhXg,3876
-teelebot/teelebot.py,sha256=epE2RM5YKaptDCwuqBZlUxQBQ1XB9Xy3ejax3x3t1ZM,125013
-teelebot/version.py,sha256=24AAn7OXpBeveIoAe0GRh_WFAXb_vH4iejFn_hCPfx0,478
+teelebot/teelebot.py,sha256=SSw0sHnQfZepuLYrNocFSYnN6lb2Tz0KatDQSyE1h24,125830
+teelebot/version.py,sha256=q5rHZe7sqob66__s95ZKKO37SUR1jiRT4oNgrSyxvLI,478
 teelebot/webhook.py,sha256=LQ51F722XOJW1mdErKw-rA9AhotGJnsvR8RStDotpVM,2665
-teelebot-1.22.0.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
-teelebot-1.22.0.dist-info/METADATA,sha256=nbqeDRFixy_mva45iVoCRjWLDg7NKg2YnN1IoxFqVFk,14660
-teelebot-1.22.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-teelebot-1.22.0.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
-teelebot-1.22.0.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
-teelebot-1.22.0.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-teelebot-1.22.0.dist-info/RECORD,,
+teelebot-1.23.0.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
+teelebot-1.23.0.dist-info/METADATA,sha256=8VE1PQz7gMDhyjbaYOo5NJWd57xPES9ddIGLSnf3bJQ,14712
+teelebot-1.23.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+teelebot-1.23.0.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
+teelebot-1.23.0.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
+teelebot-1.23.0.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+teelebot-1.23.0.dist-info/RECORD,,
```

