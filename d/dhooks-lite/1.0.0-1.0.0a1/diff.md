# Comparing `tmp/dhooks_lite-1.0.0.tar.gz` & `tmp/dhooks_lite-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhooks_lite-1.0.0.tar", last modified: Tue Apr 18 16:00:21 2023, max compression
+gzip compressed data, was "dhooks_lite-1.0.0a1.tar", last modified: Tue Apr 18 15:42:42 2023, max compression
```

## Comparing `dhooks_lite-1.0.0.tar` & `dhooks_lite-1.0.0a1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:00:21.626310 dhooks_lite-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-04-18 14:51:45.000000 dhooks_lite-1.0.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-18 14:51:45.000000 dhooks_lite-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6321 2023-04-18 16:00:21.622310 dhooks_lite-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5215 2023-04-18 15:55:09.000000 dhooks_lite-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:00:21.622310 dhooks_lite-1.0.0/dhooks_lite/
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-04-18 14:51:45.000000 dhooks_lite-1.0.0/dhooks_lite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8414 2023-04-18 14:51:45.000000 dhooks_lite-1.0.0/dhooks_lite/client.py
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-04-18 15:55:09.000000 dhooks_lite-1.0.0/dhooks_lite/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    10896 2023-04-18 15:49:20.000000 dhooks_lite-1.0.0/dhooks_lite/embed.py
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-04-18 14:51:45.000000 dhooks_lite-1.0.0/dhooks_lite/serializers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:00:21.622310 dhooks_lite-1.0.0/dhooks_lite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6321 2023-04-18 16:00:21.000000 dhooks_lite-1.0.0/dhooks_lite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-04-18 16:00:21.000000 dhooks_lite-1.0.0/dhooks_lite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 16:00:21.000000 dhooks_lite-1.0.0/dhooks_lite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-18 16:00:21.000000 dhooks_lite-1.0.0/dhooks_lite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-18 16:00:21.000000 dhooks_lite-1.0.0/dhooks_lite.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 16:00:21.626310 dhooks_lite-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1703 2023-04-18 15:55:09.000000 dhooks_lite-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:42:42.233715 dhooks_lite-1.0.0a1/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-04-18 14:51:45.000000 dhooks_lite-1.0.0a1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-18 14:51:45.000000 dhooks_lite-1.0.0a1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6360 2023-04-18 15:42:42.233715 dhooks_lite-1.0.0a1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5180 2023-04-18 15:23:27.000000 dhooks_lite-1.0.0a1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:42:42.229715 dhooks_lite-1.0.0a1/dhooks_lite/
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-04-18 14:51:45.000000 dhooks_lite-1.0.0a1/dhooks_lite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8414 2023-04-18 14:51:45.000000 dhooks_lite-1.0.0a1/dhooks_lite/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-04-18 15:23:27.000000 dhooks_lite-1.0.0a1/dhooks_lite/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    10914 2023-04-18 14:51:45.000000 dhooks_lite-1.0.0a1/dhooks_lite/embed.py
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-04-18 14:51:45.000000 dhooks_lite-1.0.0a1/dhooks_lite/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:42:42.229715 dhooks_lite-1.0.0a1/dhooks_lite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6360 2023-04-18 15:42:42.000000 dhooks_lite-1.0.0a1/dhooks_lite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-04-18 15:42:42.000000 dhooks_lite-1.0.0a1/dhooks_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 15:42:42.000000 dhooks_lite-1.0.0a1/dhooks_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-18 15:42:42.000000 dhooks_lite-1.0.0a1/dhooks_lite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-18 15:42:42.000000 dhooks_lite-1.0.0a1/dhooks_lite.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 15:42:42.233715 dhooks_lite-1.0.0a1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1795 2023-04-18 15:23:27.000000 dhooks_lite-1.0.0a1/setup.py
```

### Comparing `dhooks_lite-1.0.0/LICENSE` & `dhooks_lite-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `dhooks_lite-1.0.0/PKG-INFO` & `dhooks_lite-1.0.0a1/dhooks_lite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
-Name: dhooks_lite
-Version: 1.0.0
+Name: dhooks-lite
+Version: 1.0.0a1
 Summary: Another simple class wrapper for interacting with Discord webhooks in Python 3
-Home-page: https://gitlab.com/ErikKalkoken/dhooks-lite
+Home-page: https://github.com/ErikKalkoken/dhooks-lite
 Author: Erik Kalkoken
 Author-email: kalkoken87@gmail.com
 License: MIT
 Keywords: discord,webhooks,discordwebhooks,discordhooks
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Natural Language :: English
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -53,15 +54,14 @@
 
 This library aims to differentiate itself from similar libraries with the following properties:
 
 - is fully tested
 - simple to use (only one way of doing things, same name of attributes and objects as in the [official Discord documentation](https://discordapp.com/developers/docs/resources/webhook#execute-webhook))
 - has logging
 - requests are automatically retried and have sensible timeouts
-- works with older Python versions
 
 ## Functionality
 
 This library provides following functionality:
 
 - Posting messages in Discord channels via webhooks (synchronous calls only)
 - Attaching Embeds to messages
```

### Comparing `dhooks_lite-1.0.0/README.md` & `dhooks_lite-1.0.0a1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 This library aims to differentiate itself from similar libraries with the following properties:
 
 - is fully tested
 - simple to use (only one way of doing things, same name of attributes and objects as in the [official Discord documentation](https://discordapp.com/developers/docs/resources/webhook#execute-webhook))
 - has logging
 - requests are automatically retried and have sensible timeouts
-- works with older Python versions
 
 ## Functionality
 
 This library provides following functionality:
 
 - Posting messages in Discord channels via webhooks (synchronous calls only)
 - Attaching Embeds to messages
```

### Comparing `dhooks_lite-1.0.0/dhooks_lite/client.py` & `dhooks_lite-1.0.0a1/dhooks_lite/client.py`

 * *Files identical despite different names*

### Comparing `dhooks_lite-1.0.0/dhooks_lite/embed.py` & `dhooks_lite-1.0.0a1/dhooks_lite/embed.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                     if isinstance(value, _EmbedObject):
                         arr[key[1:]] = value.asdict()
                     else:
                         arr[key[1:]] = value
         return arr
 
     @classmethod
-    def from_dict(cls, obj_dict: dict):
+    def from_dict(cls, obj_dict: dict) -> "_EmbedObject":
         """creates a new object from the given dict"""
         args = dict()
         for param_name, param_type in get_type_hints(cls.__init__).items():
             if param_name in obj_dict and param_name != "return":
                 if hasattr(param_type, "__origin__") and param_type.__origin__ == Union:
                     param_type = param_type.__args__[0]
                 try:
```

### Comparing `dhooks_lite-1.0.0/dhooks_lite.egg-info/PKG-INFO` & `dhooks_lite-1.0.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
-Name: dhooks-lite
-Version: 1.0.0
+Name: dhooks_lite
+Version: 1.0.0a1
 Summary: Another simple class wrapper for interacting with Discord webhooks in Python 3
-Home-page: https://gitlab.com/ErikKalkoken/dhooks-lite
+Home-page: https://github.com/ErikKalkoken/dhooks-lite
 Author: Erik Kalkoken
 Author-email: kalkoken87@gmail.com
 License: MIT
 Keywords: discord,webhooks,discordwebhooks,discordhooks
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Natural Language :: English
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -53,15 +54,14 @@
 
 This library aims to differentiate itself from similar libraries with the following properties:
 
 - is fully tested
 - simple to use (only one way of doing things, same name of attributes and objects as in the [official Discord documentation](https://discordapp.com/developers/docs/resources/webhook#execute-webhook))
 - has logging
 - requests are automatically retried and have sensible timeouts
-- works with older Python versions
 
 ## Functionality
 
 This library provides following functionality:
 
 - Posting messages in Discord channels via webhooks (synchronous calls only)
 - Attaching Embeds to messages
```

### Comparing `dhooks_lite-1.0.0/setup.py` & `dhooks_lite-1.0.0a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,39 +7,40 @@
     long_description = f.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="dhooks_lite",
-    version="1.0.0",
+    version="1.0.0a1",
     packages=find_packages(),
     include_package_data=True,
     license="MIT",
     description=(
         "Another simple class wrapper for interacting with "
         "Discord webhooks in Python 3"
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["discord", "webhooks", "discordwebhooks", "discordhooks"],
-    url="https://gitlab.com/ErikKalkoken/dhooks-lite",
+    url="https://github.com/ErikKalkoken/dhooks-lite",
     author="Erik Kalkoken",
     author_email="kalkoken87@gmail.com",
     classifiers=[
         "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: MIT License",  # example license
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: Implementation :: CPython",
         "Natural Language :: English",
         "Topic :: Communications :: Chat",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     python_requires=">=3.6",
     install_requires=["requests"],
```

