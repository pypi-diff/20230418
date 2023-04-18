# Comparing `tmp/streamlit-chat-animated-0.0.3.0.tar.gz` & `tmp/streamlit-chat-animated-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-chat-animated-0.0.3.0.tar", last modified: Tue Apr 18 03:35:26 2023, max compression
+gzip compressed data, was "streamlit-chat-animated-0.0.3.1.tar", last modified: Tue Apr 18 03:39:26 2023, max compression
```

## Comparing `streamlit-chat-animated-0.0.3.0.tar` & `streamlit-chat-animated-0.0.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-18 03:35:26.111854 streamlit-chat-animated-0.0.3.0/
--rw-r--r--   0 systemd    (501) staff       (20)     1064 2023-04-05 09:19:37.000000 streamlit-chat-animated-0.0.3.0/LICENSE
--rw-r--r--   0 systemd    (501) staff       (20)       59 2023-04-05 18:23:33.000000 streamlit-chat-animated-0.0.3.0/MANIFEST.in
--rw-r--r--   0 systemd    (501) staff       (20)     1261 2023-04-18 03:35:26.111535 streamlit-chat-animated-0.0.3.0/PKG-INFO
--rw-r--r--   0 systemd    (501) staff       (20)      729 2023-04-05 21:42:26.000000 streamlit-chat-animated-0.0.3.0/README.md
--rw-r--r--   0 systemd    (501) staff       (20)       38 2023-04-18 03:35:26.111971 streamlit-chat-animated-0.0.3.0/setup.cfg
--rw-r--r--   0 systemd    (501) staff       (20)      945 2023-04-18 03:34:58.000000 streamlit-chat-animated-0.0.3.0/setup.py
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-18 03:35:26.100811 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/
--rw-r--r--   0 systemd    (501) staff       (20)     7120 2023-04-18 03:34:47.000000 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/__init__.py
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-18 03:35:26.098597 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-18 03:35:26.105605 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/
--rw-r--r--   0 systemd    (501) staff       (20)      859 2023-04-18 03:35:14.000000 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/asset-manifest.json
--rw-r--r--   0 systemd    (501) staff       (20)   197459 2023-04-18 03:35:08.000000 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/bootstrap.min.css
--rw-r--r--   0 systemd    (501) staff       (20)   646432 2023-04-18 03:35:08.000000 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/bootstrap.min.css.map
--rw-r--r--   0 systemd    (501) staff       (20)     2101 2023-04-18 03:35:14.000000 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/index.html
--rw-r--r--   0 systemd    (501) staff       (20)      564 2023-04-18 03:35:14.000000 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/precache-manifest.230db9bd95594a43c51ef55435bd1bb4.js
--rw-r--r--   0 systemd    (501) staff       (20)     1183 2023-04-18 03:35:14.000000 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/service-worker.js
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-18 03:35:26.098882 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/static/
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-18 03:35:26.111016 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/static/js/
--rw-r--r--   0 systemd    (501) staff       (20)   490881 2023-04-18 03:35:14.000000 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js
--rw-r--r--   0 systemd    (501) staff       (20)     1653 2023-04-18 03:35:14.000000 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.LICENSE.txt
--rw-r--r--   0 systemd    (501) staff       (20)  1704293 2023-04-18 03:35:14.000000 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.map
--rw-r--r--   0 systemd    (501) staff       (20)     3315 2023-04-18 03:35:14.000000 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/static/js/main.6ecc478f.chunk.js
--rw-r--r--   0 systemd    (501) staff       (20)     9426 2023-04-18 03:35:14.000000 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/static/js/main.6ecc478f.chunk.js.map
--rw-r--r--   0 systemd    (501) staff       (20)     1598 2023-04-18 03:35:14.000000 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0 systemd    (501) staff       (20)     8317 2023-04-18 03:35:14.000000 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js.map
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-18 03:35:26.102475 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated.egg-info/
--rw-r--r--   0 systemd    (501) staff       (20)     1261 2023-04-18 03:35:26.000000 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated.egg-info/PKG-INFO
--rw-r--r--   0 systemd    (501) staff       (20)     1208 2023-04-18 03:35:26.000000 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated.egg-info/SOURCES.txt
--rw-r--r--   0 systemd    (501) staff       (20)        1 2023-04-18 03:35:26.000000 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated.egg-info/dependency_links.txt
--rw-r--r--   0 systemd    (501) staff       (20)       16 2023-04-18 03:35:26.000000 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated.egg-info/requires.txt
--rw-r--r--   0 systemd    (501) staff       (20)       24 2023-04-18 03:35:26.000000 streamlit-chat-animated-0.0.3.0/streamlit_chat_animated.egg-info/top_level.txt
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-18 03:39:26.801768 streamlit-chat-animated-0.0.3.1/
+-rw-r--r--   0 systemd    (501) staff       (20)     1064 2023-04-05 09:19:37.000000 streamlit-chat-animated-0.0.3.1/LICENSE
+-rw-r--r--   0 systemd    (501) staff       (20)       59 2023-04-05 18:23:33.000000 streamlit-chat-animated-0.0.3.1/MANIFEST.in
+-rw-r--r--   0 systemd    (501) staff       (20)     1261 2023-04-18 03:39:26.801478 streamlit-chat-animated-0.0.3.1/PKG-INFO
+-rw-r--r--   0 systemd    (501) staff       (20)      729 2023-04-05 21:42:26.000000 streamlit-chat-animated-0.0.3.1/README.md
+-rw-r--r--   0 systemd    (501) staff       (20)       38 2023-04-18 03:39:26.801874 streamlit-chat-animated-0.0.3.1/setup.cfg
+-rw-r--r--   0 systemd    (501) staff       (20)      945 2023-04-18 03:39:12.000000 streamlit-chat-animated-0.0.3.1/setup.py
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-18 03:39:26.790342 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/
+-rw-r--r--   0 systemd    (501) staff       (20)     7095 2023-04-18 03:38:04.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/__init__.py
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-18 03:39:26.788615 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-18 03:39:26.795562 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/
+-rw-r--r--   0 systemd    (501) staff       (20)      859 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/asset-manifest.json
+-rw-r--r--   0 systemd    (501) staff       (20)   197459 2023-04-18 03:38:14.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/bootstrap.min.css
+-rw-r--r--   0 systemd    (501) staff       (20)   646432 2023-04-18 03:38:14.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/bootstrap.min.css.map
+-rw-r--r--   0 systemd    (501) staff       (20)     2101 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/index.html
+-rw-r--r--   0 systemd    (501) staff       (20)      564 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/precache-manifest.230db9bd95594a43c51ef55435bd1bb4.js
+-rw-r--r--   0 systemd    (501) staff       (20)     1183 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/service-worker.js
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-18 03:39:26.788890 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-18 03:39:26.800998 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/
+-rw-r--r--   0 systemd    (501) staff       (20)   490881 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js
+-rw-r--r--   0 systemd    (501) staff       (20)     1653 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.LICENSE.txt
+-rw-r--r--   0 systemd    (501) staff       (20)  1704293 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.map
+-rw-r--r--   0 systemd    (501) staff       (20)     3315 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/main.6ecc478f.chunk.js
+-rw-r--r--   0 systemd    (501) staff       (20)     9426 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/main.6ecc478f.chunk.js.map
+-rw-r--r--   0 systemd    (501) staff       (20)     1598 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0 systemd    (501) staff       (20)     8317 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js.map
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-18 03:39:26.791879 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated.egg-info/
+-rw-r--r--   0 systemd    (501) staff       (20)     1261 2023-04-18 03:39:26.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated.egg-info/PKG-INFO
+-rw-r--r--   0 systemd    (501) staff       (20)     1208 2023-04-18 03:39:26.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated.egg-info/SOURCES.txt
+-rw-r--r--   0 systemd    (501) staff       (20)        1 2023-04-18 03:39:26.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated.egg-info/dependency_links.txt
+-rw-r--r--   0 systemd    (501) staff       (20)       16 2023-04-18 03:39:26.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated.egg-info/requires.txt
+-rw-r--r--   0 systemd    (501) staff       (20)       24 2023-04-18 03:39:26.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated.egg-info/top_level.txt
```

### Comparing `streamlit-chat-animated-0.0.3.0/LICENSE` & `streamlit-chat-animated-0.0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.0/PKG-INFO` & `streamlit-chat-animated-0.0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chat-animated
-Version: 0.0.3.0
+Version: 0.0.3.1
 Summary: A streamlit component, to make chatbots with animated text
 Home-page: UNKNOWN
 Author: Yash Pravin Pawar, Yash Vardhan Kapil, Darin Manley
 Author-email: darin.j.manley@gmail.com
 License: UNKNOWN
 Keywords: chat streamlit streamlit-component animated text
 Platform: UNKNOWN
```

### Comparing `streamlit-chat-animated-0.0.3.0/README.md` & `streamlit-chat-animated-0.0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.0/setup.py` & `streamlit-chat-animated-0.0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setuptools.setup(
     name="streamlit-chat-animated",
-    version="0.0.3.0",
+    version="0.0.3.1",
     author="Yash Pravin Pawar, Yash Vardhan Kapil, Darin Manley",
     author_email="darin.j.manley@gmail.com",
     description="A streamlit component, to make chatbots with animated text",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/__init__.py` & `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,17 +79,15 @@
         An optional key that uniquely identifies this component. If this is
      False, and the component's arguments are changed, the component will
         be re-mounted in the Streamlit frontend and lose its current state.
 
     Returns: False
     """
 
-
-
-    _streamlit_chat(message=str(mess['message']).replace("\n", ""), isUser=mess['isUser'], animated=mess['animated'])
+    _streamlit_chat(message=str(message).replace("\n", ""), isUser=is_user, animated=animated)
 
 
 if not _RELEASE:
     import streamlit as st  
     # testing
     long_message = """A chatbot or chatterbot is a software application used to conduct an on-line chat conversation via text or text-to-speech, in lieu of providing direct contact with a live human agent. 
     Designed to convincingly simulate the way a human would behave as a conversational partner, chatbot systems.
```

### Comparing `streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/asset-manifest.json` & `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/bootstrap.min.css` & `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/bootstrap.min.css.map` & `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/index.html` & `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/precache-manifest.230db9bd95594a43c51ef55435bd1bb4.js` & `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/precache-manifest.230db9bd95594a43c51ef55435bd1bb4.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/service-worker.js` & `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js` & `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.LICENSE.txt` & `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.map` & `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/static/js/main.6ecc478f.chunk.js` & `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/main.6ecc478f.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/static/js/main.6ecc478f.chunk.js.map` & `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/main.6ecc478f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js` & `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.0/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.0/streamlit_chat_animated.egg-info/PKG-INFO` & `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chat-animated
-Version: 0.0.3.0
+Version: 0.0.3.1
 Summary: A streamlit component, to make chatbots with animated text
 Home-page: UNKNOWN
 Author: Yash Pravin Pawar, Yash Vardhan Kapil, Darin Manley
 Author-email: darin.j.manley@gmail.com
 License: UNKNOWN
 Keywords: chat streamlit streamlit-component animated text
 Platform: UNKNOWN
```

### Comparing `streamlit-chat-animated-0.0.3.0/streamlit_chat_animated.egg-info/SOURCES.txt` & `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated.egg-info/SOURCES.txt`

 * *Files identical despite different names*

