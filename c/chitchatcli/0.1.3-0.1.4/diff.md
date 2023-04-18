# Comparing `tmp/chitchatcli-0.1.3.tar.gz` & `tmp/chitchatcli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chitchatcli-0.1.3.tar", last modified: Tue Apr 18 21:17:21 2023, max compression
+gzip compressed data, was "chitchatcli-0.1.4.tar", last modified: Tue Apr 18 21:20:20 2023, max compression
```

## Comparing `chitchatcli-0.1.3.tar` & `chitchatcli-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-18 21:17:21.421870 chitchatcli-0.1.3/
--rw-r--r--   0 ben        (501) staff       (20)     1064 2023-04-18 20:24:23.000000 chitchatcli-0.1.3/LICENSE.txt
--rw-r--r--   0 ben        (501) staff       (20)     1935 2023-04-18 21:17:21.421105 chitchatcli-0.1.3/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     1501 2023-04-18 20:58:00.000000 chitchatcli-0.1.3/README.md
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-18 21:17:21.391123 chitchatcli-0.1.3/chitchatcli/
--rw-r--r--   0 ben        (501) staff       (20)        0 2023-04-18 21:15:52.000000 chitchatcli-0.1.3/chitchatcli/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     6639 2023-04-18 21:16:48.000000 chitchatcli-0.1.3/chitchatcli/__main__.py
--rw-r--r--   0 ben        (501) staff       (20)      836 2023-04-18 21:14:56.000000 chitchatcli-0.1.3/chitchatcli/globalvaribles.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-18 21:17:21.419457 chitchatcli-0.1.3/chitchatcli/utilis/
--rw-r--r--   0 ben        (501) staff       (20)        0 2023-04-18 20:59:05.000000 chitchatcli-0.1.3/chitchatcli/utilis/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     7812 2023-04-18 21:16:48.000000 chitchatcli-0.1.3/chitchatcli/utilis/apicalls.py
--rw-r--r--   0 ben        (501) staff       (20)     1017 2023-04-18 21:16:48.000000 chitchatcli-0.1.3/chitchatcli/utilis/event.py
--rw-r--r--   0 ben        (501) staff       (20)     3457 2023-04-18 21:16:48.000000 chitchatcli-0.1.3/chitchatcli/utilis/helper_functions.py
--rw-r--r--   0 ben        (501) staff       (20)     2786 2023-04-18 21:16:48.000000 chitchatcli-0.1.3/chitchatcli/utilis/process.py
--rw-r--r--   0 ben        (501) staff       (20)    18393 2023-04-18 21:16:48.000000 chitchatcli-0.1.3/chitchatcli/utilis/screen_functions.py
--rw-r--r--   0 ben        (501) staff       (20)     1068 2023-04-18 18:42:12.000000 chitchatcli-0.1.3/chitchatcli/utilis/storage.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-18 21:17:21.404020 chitchatcli-0.1.3/chitchatcli.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     1935 2023-04-18 21:17:21.000000 chitchatcli-0.1.3/chitchatcli.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      510 2023-04-18 21:17:21.000000 chitchatcli-0.1.3/chitchatcli.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2023-04-18 21:17:21.000000 chitchatcli-0.1.3/chitchatcli.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       74 2023-04-18 21:17:21.000000 chitchatcli-0.1.3/chitchatcli.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)       12 2023-04-18 21:17:21.000000 chitchatcli-0.1.3/chitchatcli.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)       38 2023-04-18 21:17:21.422197 chitchatcli-0.1.3/setup.cfg
--rw-r--r--   0 ben        (501) staff       (20)      888 2023-04-18 21:17:08.000000 chitchatcli-0.1.3/setup.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-18 21:20:20.003026 chitchatcli-0.1.4/
+-rw-r--r--   0 ben        (501) staff       (20)     1064 2023-04-18 20:24:23.000000 chitchatcli-0.1.4/LICENSE.txt
+-rw-r--r--   0 ben        (501) staff       (20)     1935 2023-04-18 21:20:20.002349 chitchatcli-0.1.4/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     1501 2023-04-18 20:58:00.000000 chitchatcli-0.1.4/README.md
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-18 21:20:19.978675 chitchatcli-0.1.4/chitchatcli/
+-rw-r--r--   0 ben        (501) staff       (20)        0 2023-04-18 21:15:52.000000 chitchatcli-0.1.4/chitchatcli/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     6639 2023-04-18 21:16:48.000000 chitchatcli-0.1.4/chitchatcli/__main__.py
+-rw-r--r--   0 ben        (501) staff       (20)      836 2023-04-18 21:14:56.000000 chitchatcli-0.1.4/chitchatcli/globalvaribles.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-18 21:20:20.001258 chitchatcli-0.1.4/chitchatcli/utilis/
+-rw-r--r--   0 ben        (501) staff       (20)        0 2023-04-18 20:59:05.000000 chitchatcli-0.1.4/chitchatcli/utilis/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     7824 2023-04-18 21:19:33.000000 chitchatcli-0.1.4/chitchatcli/utilis/apicalls.py
+-rw-r--r--   0 ben        (501) staff       (20)     1017 2023-04-18 21:16:48.000000 chitchatcli-0.1.4/chitchatcli/utilis/event.py
+-rw-r--r--   0 ben        (501) staff       (20)     3457 2023-04-18 21:16:48.000000 chitchatcli-0.1.4/chitchatcli/utilis/helper_functions.py
+-rw-r--r--   0 ben        (501) staff       (20)     2786 2023-04-18 21:16:48.000000 chitchatcli-0.1.4/chitchatcli/utilis/process.py
+-rw-r--r--   0 ben        (501) staff       (20)    18393 2023-04-18 21:16:48.000000 chitchatcli-0.1.4/chitchatcli/utilis/screen_functions.py
+-rw-r--r--   0 ben        (501) staff       (20)     1068 2023-04-18 18:42:12.000000 chitchatcli-0.1.4/chitchatcli/utilis/storage.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-18 21:20:19.984136 chitchatcli-0.1.4/chitchatcli.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     1935 2023-04-18 21:20:19.000000 chitchatcli-0.1.4/chitchatcli.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      510 2023-04-18 21:20:19.000000 chitchatcli-0.1.4/chitchatcli.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2023-04-18 21:20:19.000000 chitchatcli-0.1.4/chitchatcli.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)       74 2023-04-18 21:20:19.000000 chitchatcli-0.1.4/chitchatcli.egg-info/requires.txt
+-rw-r--r--   0 ben        (501) staff       (20)       12 2023-04-18 21:20:19.000000 chitchatcli-0.1.4/chitchatcli.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)       38 2023-04-18 21:20:20.005168 chitchatcli-0.1.4/setup.cfg
+-rw-r--r--   0 ben        (501) staff       (20)      888 2023-04-18 21:20:10.000000 chitchatcli-0.1.4/setup.py
```

### Comparing `chitchatcli-0.1.3/LICENSE.txt` & `chitchatcli-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chitchatcli-0.1.3/PKG-INFO` & `chitchatcli-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chitchatcli
-Version: 0.1.3
+Version: 0.1.4
 Summary: A command line chatting software designed for developers to communicate with each other.
 Author: Benjamin Eruvieru
 Author-email: benjamineruvieru@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `chitchatcli-0.1.3/README.md` & `chitchatcli-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `chitchatcli-0.1.3/chitchatcli/__main__.py` & `chitchatcli-0.1.4/chitchatcli/__main__.py`

 * *Files identical despite different names*

### Comparing `chitchatcli-0.1.3/chitchatcli/globalvaribles.py` & `chitchatcli-0.1.4/chitchatcli/globalvaribles.py`

 * *Files identical despite different names*

### Comparing `chitchatcli-0.1.3/chitchatcli/utilis/apicalls.py` & `chitchatcli-0.1.4/chitchatcli/utilis/apicalls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 from chitchatcli.globalvaribles import globalstate
 from chitchatcli.utilis.helper_functions import showError, homepage, log, renderSearchUser
 from chitchatcli.utilis.storage import storage
-from globalvaribles import globalstate
+from chitchatcli.globalvaribles import globalstate
 from chitchatcli.utilis.helper_functions import showError, homepage, log, renderMessage
 from chitchatcli.utilis.storage import storage
 from chitchatcli.utilis.event import connectToSocket
 import curses
 import time
 from chitchatcli.utilis import screen_functions
```

### Comparing `chitchatcli-0.1.3/chitchatcli/utilis/event.py` & `chitchatcli-0.1.4/chitchatcli/utilis/event.py`

 * *Files identical despite different names*

### Comparing `chitchatcli-0.1.3/chitchatcli/utilis/helper_functions.py` & `chitchatcli-0.1.4/chitchatcli/utilis/helper_functions.py`

 * *Files identical despite different names*

### Comparing `chitchatcli-0.1.3/chitchatcli/utilis/process.py` & `chitchatcli-0.1.4/chitchatcli/utilis/process.py`

 * *Files identical despite different names*

### Comparing `chitchatcli-0.1.3/chitchatcli/utilis/screen_functions.py` & `chitchatcli-0.1.4/chitchatcli/utilis/screen_functions.py`

 * *Files identical despite different names*

### Comparing `chitchatcli-0.1.3/chitchatcli/utilis/storage.py` & `chitchatcli-0.1.4/chitchatcli/utilis/storage.py`

 * *Files identical despite different names*

### Comparing `chitchatcli-0.1.3/chitchatcli.egg-info/PKG-INFO` & `chitchatcli-0.1.4/chitchatcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chitchatcli
-Version: 0.1.3
+Version: 0.1.4
 Summary: A command line chatting software designed for developers to communicate with each other.
 Author: Benjamin Eruvieru
 Author-email: benjamineruvieru@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `chitchatcli-0.1.3/setup.py` & `chitchatcli-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setup(
     name="chitchatcli",
-    version="0.1.3",
+    version="0.1.4",
     author="Benjamin Eruvieru",
     author_email="benjamineruvieru@gmail.com",
     description="A command line chatting software designed for developers to communicate with each other.",
     packages=find_packages(),
     long_description_content_type="text/markdown",
     long_description=long_description,
     install_requires=["python-socketio[client]",
```

