# Comparing `tmp/twitch-dl-2.1.1.tar.gz` & `tmp/twitch-dl-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch-dl-2.1.1.tar", last modified: Sun Nov 20 14:47:33 2022, max compression
+gzip compressed data, was "twitch-dl-2.1.2.tar", last modified: Tue Apr 18 05:12:34 2023, max compression
```

## Comparing `twitch-dl-2.1.1.tar` & `twitch-dl-2.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2022-11-20 14:47:33.643497 twitch-dl-2.1.1/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      721 2022-11-20 14:47:33.643497 twitch-dl-2.1.1/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1627 2022-08-18 08:06:46.000000 twitch-dl-2.1.1/README.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2022-11-20 14:47:33.643497 twitch-dl-2.1.1/setup.cfg
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1128 2022-11-20 14:46:29.000000 twitch-dl-2.1.1/setup.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2022-11-20 14:47:33.643497 twitch-dl-2.1.1/twitch_dl.egg-info/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      721 2022-11-20 14:47:33.000000 twitch-dl-2.1.1/twitch_dl.egg-info/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      584 2022-11-20 14:47:33.000000 twitch-dl-2.1.1/twitch_dl.egg-info/SOURCES.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2022-11-20 14:47:33.000000 twitch-dl-2.1.1/twitch_dl.egg-info/dependency_links.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       53 2022-11-20 14:47:33.000000 twitch-dl-2.1.1/twitch_dl.egg-info/entry_points.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       40 2022-11-20 14:47:33.000000 twitch-dl-2.1.1/twitch_dl.egg-info/requires.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2022-11-20 14:47:33.000000 twitch-dl-2.1.1/twitch_dl.egg-info/top_level.txt
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2022-11-20 14:47:33.643497 twitch-dl-2.1.1/twitchdl/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       68 2022-11-20 14:46:50.000000 twitch-dl-2.1.1/twitchdl/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       42 2020-11-04 07:52:52.000000 twitch-dl-2.1.1/twitchdl/__main__.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2022-11-20 14:47:33.643497 twitch-dl-2.1.1/twitchdl/commands/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      198 2022-11-20 08:22:41.000000 twitch-dl-2.1.1/twitchdl/commands/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2702 2022-11-20 14:35:33.000000 twitch-dl-2.1.1/twitchdl/commands/clips.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    12820 2022-11-20 14:32:36.000000 twitch-dl-2.1.1/twitchdl/commands/download.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      182 2022-08-09 07:04:30.000000 twitch-dl-2.1.1/twitchdl/commands/env.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2592 2022-11-20 14:35:33.000000 twitch-dl-2.1.1/twitchdl/commands/info.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1892 2022-11-20 14:35:33.000000 twitch-dl-2.1.1/twitchdl/commands/videos.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10603 2022-11-20 14:32:36.000000 twitch-dl-2.1.1/twitchdl/console.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      882 2022-08-20 11:25:04.000000 twitch-dl-2.1.1/twitchdl/download.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      113 2020-04-09 20:48:04.000000 twitch-dl-2.1.1/twitchdl/exceptions.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3892 2022-11-20 14:35:42.000000 twitch-dl-2.1.1/twitchdl/http.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4374 2022-09-10 06:24:28.000000 twitch-dl-2.1.1/twitchdl/output.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4435 2022-08-18 08:06:46.000000 twitch-dl-2.1.1/twitchdl/progress.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9434 2022-11-20 14:35:49.000000 twitch-dl-2.1.1/twitchdl/twitch.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2938 2022-11-20 14:32:36.000000 twitch-dl-2.1.1/twitchdl/utils.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-04-18 05:12:34.095268 twitch-dl-2.1.2/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      721 2023-04-18 05:12:34.095268 twitch-dl-2.1.2/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1627 2022-08-18 08:06:46.000000 twitch-dl-2.1.2/README.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2023-04-18 05:12:34.095268 twitch-dl-2.1.2/setup.cfg
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1128 2023-04-18 05:08:35.000000 twitch-dl-2.1.2/setup.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-04-18 05:12:34.095268 twitch-dl-2.1.2/twitch_dl.egg-info/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      721 2023-04-18 05:12:33.000000 twitch-dl-2.1.2/twitch_dl.egg-info/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      584 2023-04-18 05:12:34.000000 twitch-dl-2.1.2/twitch_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2023-04-18 05:12:33.000000 twitch-dl-2.1.2/twitch_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       53 2023-04-18 05:12:33.000000 twitch-dl-2.1.2/twitch_dl.egg-info/entry_points.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       40 2023-04-18 05:12:33.000000 twitch-dl-2.1.2/twitch_dl.egg-info/requires.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2023-04-18 05:12:33.000000 twitch-dl-2.1.2/twitch_dl.egg-info/top_level.txt
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-04-18 05:12:34.095268 twitch-dl-2.1.2/twitchdl/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       68 2023-04-18 05:08:41.000000 twitch-dl-2.1.2/twitchdl/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       42 2020-11-04 07:52:52.000000 twitch-dl-2.1.2/twitchdl/__main__.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-04-18 05:12:34.095268 twitch-dl-2.1.2/twitchdl/commands/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      198 2022-11-20 08:22:41.000000 twitch-dl-2.1.2/twitchdl/commands/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2702 2022-11-20 14:35:33.000000 twitch-dl-2.1.2/twitchdl/commands/clips.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    12820 2022-11-20 14:32:36.000000 twitch-dl-2.1.2/twitchdl/commands/download.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      182 2022-08-09 07:04:30.000000 twitch-dl-2.1.2/twitchdl/commands/env.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2592 2022-11-20 14:35:33.000000 twitch-dl-2.1.2/twitchdl/commands/info.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1892 2022-11-20 14:35:33.000000 twitch-dl-2.1.2/twitchdl/commands/videos.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10603 2022-11-20 14:32:36.000000 twitch-dl-2.1.2/twitchdl/console.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      882 2022-08-20 11:25:04.000000 twitch-dl-2.1.2/twitchdl/download.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      113 2020-04-09 20:48:04.000000 twitch-dl-2.1.2/twitchdl/exceptions.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3892 2022-11-20 14:35:42.000000 twitch-dl-2.1.2/twitchdl/http.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4374 2022-09-10 06:24:28.000000 twitch-dl-2.1.2/twitchdl/output.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4435 2022-08-18 08:06:46.000000 twitch-dl-2.1.2/twitchdl/progress.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9434 2023-04-18 05:05:03.000000 twitch-dl-2.1.2/twitchdl/twitch.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2938 2022-11-20 14:32:36.000000 twitch-dl-2.1.2/twitchdl/utils.py
```

### Comparing `twitch-dl-2.1.1/PKG-INFO` & `twitch-dl-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: twitch-dl
-Version: 2.1.1
+Version: 2.1.2
 Summary: Twitch downloader
 Home-page: https://github.com/ihabunek/twitch-dl/
 Author: Ivan Habunek
 Author-email: ivan@habunek.com
 License: GPLv3
 Project-URL: Documentation, https://twitch-dl.bezdomni.net/
 Description: Quickly download videos from twitch.tv.
```

### Comparing `twitch-dl-2.1.1/README.md` & `twitch-dl-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.1/setup.py` & `twitch-dl-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Works simliarly to youtube-dl but downloads multiple VODs in parallel which
 makes it faster.
 """
 
 setup(
     name="twitch-dl",
-    version="2.1.1",
+    version="2.1.2",
     description="Twitch downloader",
     long_description=long_description.strip(),
     author="Ivan Habunek",
     author_email="ivan@habunek.com",
     url="https://github.com/ihabunek/twitch-dl/",
     project_urls={
         "Documentation": "https://twitch-dl.bezdomni.net/"
```

### Comparing `twitch-dl-2.1.1/twitch_dl.egg-info/PKG-INFO` & `twitch-dl-2.1.2/twitch_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: twitch-dl
-Version: 2.1.1
+Version: 2.1.2
 Summary: Twitch downloader
 Home-page: https://github.com/ihabunek/twitch-dl/
 Author: Ivan Habunek
 Author-email: ivan@habunek.com
 License: GPLv3
 Project-URL: Documentation, https://twitch-dl.bezdomni.net/
 Description: Quickly download videos from twitch.tv.
```

### Comparing `twitch-dl-2.1.1/twitch_dl.egg-info/SOURCES.txt` & `twitch-dl-2.1.2/twitch_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.1/twitchdl/commands/clips.py` & `twitch-dl-2.1.2/twitchdl/commands/clips.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.1/twitchdl/commands/download.py` & `twitch-dl-2.1.2/twitchdl/commands/download.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.1/twitchdl/commands/info.py` & `twitch-dl-2.1.2/twitchdl/commands/info.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.1/twitchdl/commands/videos.py` & `twitch-dl-2.1.2/twitchdl/commands/videos.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.1/twitchdl/console.py` & `twitch-dl-2.1.2/twitchdl/console.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.1/twitchdl/download.py` & `twitch-dl-2.1.2/twitchdl/download.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.1/twitchdl/http.py` & `twitch-dl-2.1.2/twitchdl/http.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.1/twitchdl/output.py` & `twitch-dl-2.1.2/twitchdl/output.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.1/twitchdl/progress.py` & `twitch-dl-2.1.2/twitchdl/progress.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.1/twitchdl/twitch.py` & `twitch-dl-2.1.2/twitchdl/twitch.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,15 +331,15 @@
         raise
 
 
 def get_playlists(video_id, access_token):
     """
     For a given video return a playlist which contains possible video qualities.
     """
-    url = "http://usher.twitch.tv/vod/{}".format(video_id)
+    url = "http://usher.ttvnw.net/vod/{}".format(video_id)
 
     response = httpx.get(url, params={
         "nauth": access_token['value'],
         "nauthsig": access_token['signature'],
         "allow_audio_only": "true",
         "allow_source": "true",
         "player": "twitchweb",
```

### Comparing `twitch-dl-2.1.1/twitchdl/utils.py` & `twitch-dl-2.1.2/twitchdl/utils.py`

 * *Files identical despite different names*

