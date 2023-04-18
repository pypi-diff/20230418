# Comparing `tmp/dhooks_lite-0.6.1.tar.gz` & `tmp/dhooks_lite-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dhooks_lite-0.6.1.tar", last modified: Mon Jan  4 00:30:31 2021, max compression
+gzip compressed data, was "dhooks_lite-1.0.0a1.tar", last modified: Tue Apr 18 15:42:42 2023, max compression
```

## Comparing `dhooks_lite-0.6.1.tar` & `dhooks_lite-1.0.0a1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 erik997   (1000) erik997   (1000)        0 2021-01-04 00:30:31.000000 dhooks_lite-0.6.1/
--rw-r--r--   0 erik997   (1000) erik997   (1000)     1070 2021-01-02 21:58:30.000000 dhooks_lite-0.6.1/LICENSE
--rw-r--r--   0 erik997   (1000) erik997   (1000)       98 2021-01-02 22:13:46.000000 dhooks_lite-0.6.1/MANIFEST.in
--rw-r--r--   0 erik997   (1000) erik997   (1000)     6918 2021-01-04 00:30:31.000000 dhooks_lite-0.6.1/PKG-INFO
--rw-r--r--   0 erik997   (1000) erik997   (1000)     4672 2021-01-02 22:16:42.000000 dhooks_lite-0.6.1/README.md
-drwxr-xr-x   0 erik997   (1000) erik997   (1000)        0 2021-01-04 00:30:31.000000 dhooks_lite-0.6.1/dhooks_lite/
--rw-r--r--   0 erik997   (1000) erik997   (1000)      148 2021-01-02 22:13:47.000000 dhooks_lite-0.6.1/dhooks_lite/__init__.py
--rw-r--r--   0 erik997   (1000) erik997   (1000)     8192 2021-01-03 00:43:37.000000 dhooks_lite-0.6.1/dhooks_lite/client.py
--rw-r--r--   0 erik997   (1000) erik997   (1000)      108 2021-01-04 00:27:22.000000 dhooks_lite-0.6.1/dhooks_lite/constants.py
--rw-r--r--   0 erik997   (1000) erik997   (1000)    10438 2021-01-02 22:13:47.000000 dhooks_lite-0.6.1/dhooks_lite/embed.py
--rw-r--r--   0 erik997   (1000) erik997   (1000)      344 2021-01-02 21:58:30.000000 dhooks_lite-0.6.1/dhooks_lite/serializers.py
-drwxr-xr-x   0 erik997   (1000) erik997   (1000)        0 2021-01-04 00:30:31.000000 dhooks_lite-0.6.1/dhooks_lite.egg-info/
--rw-r--r--   0 erik997   (1000) erik997   (1000)     6918 2021-01-04 00:30:31.000000 dhooks_lite-0.6.1/dhooks_lite.egg-info/PKG-INFO
--rw-r--r--   0 erik997   (1000) erik997   (1000)      331 2021-01-04 00:30:31.000000 dhooks_lite-0.6.1/dhooks_lite.egg-info/SOURCES.txt
--rw-r--r--   0 erik997   (1000) erik997   (1000)        1 2021-01-04 00:30:31.000000 dhooks_lite-0.6.1/dhooks_lite.egg-info/dependency_links.txt
--rw-r--r--   0 erik997   (1000) erik997   (1000)        9 2021-01-04 00:30:31.000000 dhooks_lite-0.6.1/dhooks_lite.egg-info/requires.txt
--rw-r--r--   0 erik997   (1000) erik997   (1000)       18 2021-01-04 00:30:31.000000 dhooks_lite-0.6.1/dhooks_lite.egg-info/top_level.txt
--rw-r--r--   0 erik997   (1000) erik997   (1000)       38 2021-01-04 00:30:31.000000 dhooks_lite-0.6.1/setup.cfg
--rw-r--r--   0 erik997   (1000) erik997   (1000)     1695 2021-01-04 00:27:14.000000 dhooks_lite-0.6.1/setup.py
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

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dhooks_lite-0.6.1/LICENSE` & `dhooks_lite-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `dhooks_lite-0.6.1/PKG-INFO` & `dhooks_lite-1.0.0a1/dhooks_lite.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,171 +1,175 @@
 Metadata-Version: 2.1
-Name: dhooks_lite
-Version: 0.6.1
+Name: dhooks-lite
+Version: 1.0.0a1
 Summary: Another simple class wrapper for interacting with Discord webhooks in Python 3
 Home-page: https://github.com/ErikKalkoken/dhooks-lite
 Author: Erik Kalkoken
 Author-email: kalkoken87@gmail.com
 License: MIT
-Description: # dhooks-lite
-        
-        ![version](https://img.shields.io/pypi/v/dhooks-lite)
-        ![python](https://img.shields.io/pypi/pyversions/dhooks-lite)
-        ![license](https://img.shields.io/github/license/ErikKalkoken/dhooks-lite)
-        ![build](https://api.travis-ci.org/ErikKalkoken/dhooks-lite.svg?branch=master)
-        [![codecov](https://codecov.io/gh/ErikKalkoken/dhooks-lite/branch/master/graph/badge.svg)](https://codecov.io/gh/ErikKalkoken/dhooks-lite)
-        [![Documentation Status](https://readthedocs.org/projects/dhooks-lite/badge/?version=latest)](https://dhooks-lite.readthedocs.io/en/latest/?badge=latest)
-        [![Downloads](https://pepy.tech/badge/dhooks-lite)](https://pepy.tech/project/dhooks-lite)
-        
-        ## Contents
-        
-        - [Overview](#Overview)
-        - [Functionality](#functionality)
-        - [Examples](#examples)
-        - [Installation](#installation)
-        - [Documentation](#documentation)
-        - [Contribution](#contribution)
-        - [Change Log](CHANGELOG.md)
-        
-        ## Overview
-        
-        **dhooks-lite** is a library with a set of classes for interacting with Discord webhooks written in Python 3.
-        
-        This library aims to differentiate itself from similar libraries with the following properties:
-        
-        - is fully tested
-        - simple to use (only one way of doing things, same name of attributes and objects as in the [official Discord documentation](https://discordapp.com/developers/docs/resources/webhook#execute-webhook))
-        - has logging
-        - requests are automatically retried and have sensible timeouts
-        
-        ## Functionality
-        
-        This library provides following functionality:
-        
-        - Posting messages in Discord channels via webhooks (synchronous calls only)
-        - Attaching Embeds to messages
-        - Retrieve send reports and from Discord
-        - Retrieve HTTP status and headers from Discord, e.g. for implementing rate limit handling
-        
-        ## Examples
-        
-        Here are some examples on how to use dhooks-lite in your Python scripts.
-        
-        Note that you also find the source code of all examples in the `/examples` folder of this repo.
-        
-        ### Hello World
-        
-        Minimal example for posting a message.
-        
-        ```python
-        from dhooks_lite import Webhook
-        
-        hook = Webhook(DISCORD_WEBHOOK_URL)
-        hook.execute('Hello, World!')
-        ```
-        
-        ![example1](https://i.imgur.com/t3mxMAJ.png)
-        
-        ### Posting with custom avatar
-        
-        In this example we are setting username and avatar.
-        
-        ```python
-        from dhooks_lite import Webhook
-        
-        hook = Webhook(
-            DISCORD_WEBHOOK_URL,
-            username='Bruce Wayne',
-            avatar_url='https://i.imgur.com/thK8erv.png'
-        )
-        hook.execute('I am Batman!')
-        ```
-        
-        ![example2](https://i.imgur.com/mseg2Yx.png)
-        
-        ### Complete example with embeds
-        
-        Finally, here is an example for posting a message with two embeds and using all available features (shortened):
-        
-        ```python
-        import datetime
-        from dhooks_lite import Webhook, Embed, Footer, Image, Thumbnail, Author, Field
-        
-        hook = Webhook(DISCORD_WEBHOOK_URL)
-        e1 = Embed(
-            description='Only a few years ago, scientists stumbled upon an electrical current of cosmic proportions.(...)',
-            title='Universe\'s highest electric current found',
-            url='https://www.newscientist.com/article/mg21028174-900-universes-highest-electric-current-found/',
-            timestamp=datetime.datetime.utcnow(),
-            color=0x5CDBF0,
-            footer=Footer(
-                'Science Department',
-                'https://i.imgur.com/Bgsv04h.png'
-            ),
-            image=Image('https://i.imgur.com/eis1Y0P.jpg'),
-            thumbnail=Thumbnail('https://i.imgur.com/2A4k28x.jpg'),
-            author=Author(
-                'John Scientist',
-                url='https://en.wikipedia.org/wiki/Albert_Einstein',
-                icon_url='https://i.imgur.com/1JoHDw1.png'
-            ),
-            fields=[
-                Field('1st Measurement', 'Failed'),
-                Field('2nd Measurement', 'Succeeded')
-            ]
-        )
-        e2 = Embed(description="TOP SECRET - Do not distribute!")
-        
-        hook.execute(
-            'Checkout this new report from the science department:',
-            username='Bruce Wayne',
-            avatar_url='https://i.imgur.com/thK8erv.png',
-            embeds=[e1, e2],
-            wait_for_response=True
-        )
-        ```
-        
-        ![example2](https://i.imgur.com/RoWBh2n.png)
-        
-        ## Installation
-        
-        You can install this library directly from PyPI:
-        
-        ```bash
-        pip install dhooks-lite
-        ```
-        
-        ## Documentation
-        
-        For a full documentation of all classes please see the official docs [here](https://dhooks-lite.readthedocs.io/en/latest/).
-        
-        ## Contribution
-        
-        We welcome any contribution!
-        
-        If you found a bug or have a feature request please raise an issue.
-        
-        If you want to help further improve this library please feel free to issue a merge request. Please adhere to the following requirements in your change:
-        
-        - Code should be compliant with [PEP8](https://www.python.org/dev/peps/pep-0008/)
-        - Full overage by unit tests
-        - All classes should be immutable
-        - All classes and their public methods must have docstring documentation
-        - All changes must be documented in the Change Log
-        
 Keywords: discord,webhooks,discordwebhooks,discordhooks
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Natural Language :: English
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: ~=3.6
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# dhooks-lite
+
+[![release](https://img.shields.io/pypi/v/dhooks-lite?label=release)](https://pypi.org/project/dhooks-lite/)
+[![python](https://img.shields.io/pypi/pyversions/dhooks-lite)](https://pypi.org/project/dhooks-lite/)
+[![pipeline status](https://gitlab.com/ErikKalkoken/dhooks-lite/badges/master/pipeline.svg)](https://gitlab.com/ErikKalkoken/dhooks-lite/-/commits/master)
+[![codecov](https://codecov.io/gl/ErikKalkoken/dhooks-lite/branch/master/graph/badge.svg?token=9YNL3HEJ5D)](https://codecov.io/gl/ErikKalkoken/dhooks-lite)
+[![Documentation Status](https://readthedocs.org/projects/dhooks-lite/badge/?version=latest)](https://dhooks-lite.readthedocs.io/en/latest/?badge=latest)
+[![license](https://img.shields.io/badge/license-MIT-green)](https://gitlab.com/ErikKalkoken/dhooks-lite/-/blob/master/LICENSE)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![chat](https://img.shields.io/discord/790364535294132234)](https://discord.gg/zmh52wnfvM)
+
+## Contents
+
+- [Overview](#overview)
+- [Functionality](#functionality)
+- [Examples](#examples)
+- [Installation](#installation)
+- [Documentation](#documentation)
+- [Contribution](#contribution)
+- [Change Log](CHANGELOG.md)
+
+## Overview
+
+**dhooks-lite** is a library with a set of classes for interacting with Discord webhooks written in Python 3.
+
+This library aims to differentiate itself from similar libraries with the following properties:
+
+- is fully tested
+- simple to use (only one way of doing things, same name of attributes and objects as in the [official Discord documentation](https://discordapp.com/developers/docs/resources/webhook#execute-webhook))
+- has logging
+- requests are automatically retried and have sensible timeouts
+
+## Functionality
+
+This library provides following functionality:
+
+- Posting messages in Discord channels via webhooks (synchronous calls only)
+- Attaching Embeds to messages
+- Retrieve send reports and from Discord
+- Retrieve HTTP status and headers from Discord, e.g. for implementing rate limit handling
+
+## Examples
+
+Here are some examples on how to use dhooks-lite in your Python scripts.
+
+Note that you also find the source code of all examples in the `/examples` folder of this repo.
+
+### Hello World
+
+Minimal example for posting a message.
+
+```python
+from dhooks_lite import Webhook
+
+hook = Webhook(DISCORD_WEBHOOK_URL)
+hook.execute('Hello, World!')
+```
+
+![example1](https://i.imgur.com/t3mxMAJ.png)
+
+### Posting with custom avatar
+
+In this example we are setting username and avatar.
+
+```python
+from dhooks_lite import Webhook
+
+hook = Webhook(
+    DISCORD_WEBHOOK_URL,
+    username='Bruce Wayne',
+    avatar_url='https://i.imgur.com/thK8erv.png'
+)
+hook.execute('I am Batman!')
+```
+
+![example2](https://i.imgur.com/mseg2Yx.png)
+
+### Complete example with embeds
+
+Finally, here is an example for posting a message with two embeds and using all available features (shortened):
+
+```python
+import datetime
+from dhooks_lite import Webhook, Embed, Footer, Image, Thumbnail, Author, Field
+
+hook = Webhook(DISCORD_WEBHOOK_URL)
+e1 = Embed(
+    description='Only a few years ago, scientists stumbled upon an electrical current of cosmic proportions.(...)',
+    title='Universe\'s highest electric current found',
+    url='https://www.newscientist.com/article/mg21028174-900-universes-highest-electric-current-found/',
+    timestamp=datetime.datetime.utcnow(),
+    color=0x5CDBF0,
+    footer=Footer(
+        'Science Department',
+        'https://i.imgur.com/Bgsv04h.png'
+    ),
+    image=Image('https://i.imgur.com/eis1Y0P.jpg'),
+    thumbnail=Thumbnail('https://i.imgur.com/2A4k28x.jpg'),
+    author=Author(
+        'John Scientist',
+        url='https://en.wikipedia.org/wiki/Albert_Einstein',
+        icon_url='https://i.imgur.com/1JoHDw1.png'
+    ),
+    fields=[
+        Field('1st Measurement', 'Failed'),
+        Field('2nd Measurement', 'Succeeded')
+    ]
+)
+e2 = Embed(description="TOP SECRET - Do not distribute!")
+
+hook.execute(
+    'Checkout this new report from the science department:',
+    username='Bruce Wayne',
+    avatar_url='https://i.imgur.com/thK8erv.png',
+    embeds=[e1, e2],
+    wait_for_response=True
+)
+```
+
+![example2](https://i.imgur.com/RoWBh2n.png)
+
+## Installation
+
+You can install this library directly from PyPI:
+
+```bash
+pip install dhooks-lite
+```
+
+## Documentation
+
+For a full documentation of all classes please see the official docs [here](https://dhooks-lite.readthedocs.io/en/latest/).
+
+## Contribution
+
+We welcome any contribution!
+
+If you found a bug or have a feature request please raise an issue.
+
+If you want to help further improve this library please feel free to issue a merge request. Please adhere to the following requirements in your change:
+
+- Code should be compliant with [PEP8](https://www.python.org/dev/peps/pep-0008/)
+- Full overage by unit tests
+- All classes should be immutable
+- All classes and their public methods must have docstring documentation
+- All changes must be documented in the Change Log
```

### Comparing `dhooks_lite-0.6.1/README.md` & `dhooks_lite-1.0.0a1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # dhooks-lite
 
-![version](https://img.shields.io/pypi/v/dhooks-lite)
-![python](https://img.shields.io/pypi/pyversions/dhooks-lite)
-![license](https://img.shields.io/github/license/ErikKalkoken/dhooks-lite)
-![build](https://api.travis-ci.org/ErikKalkoken/dhooks-lite.svg?branch=master)
-[![codecov](https://codecov.io/gh/ErikKalkoken/dhooks-lite/branch/master/graph/badge.svg)](https://codecov.io/gh/ErikKalkoken/dhooks-lite)
+[![release](https://img.shields.io/pypi/v/dhooks-lite?label=release)](https://pypi.org/project/dhooks-lite/)
+[![python](https://img.shields.io/pypi/pyversions/dhooks-lite)](https://pypi.org/project/dhooks-lite/)
+[![pipeline status](https://gitlab.com/ErikKalkoken/dhooks-lite/badges/master/pipeline.svg)](https://gitlab.com/ErikKalkoken/dhooks-lite/-/commits/master)
+[![codecov](https://codecov.io/gl/ErikKalkoken/dhooks-lite/branch/master/graph/badge.svg?token=9YNL3HEJ5D)](https://codecov.io/gl/ErikKalkoken/dhooks-lite)
 [![Documentation Status](https://readthedocs.org/projects/dhooks-lite/badge/?version=latest)](https://dhooks-lite.readthedocs.io/en/latest/?badge=latest)
-[![Downloads](https://pepy.tech/badge/dhooks-lite)](https://pepy.tech/project/dhooks-lite)
+[![license](https://img.shields.io/badge/license-MIT-green)](https://gitlab.com/ErikKalkoken/dhooks-lite/-/blob/master/LICENSE)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![chat](https://img.shields.io/discord/790364535294132234)](https://discord.gg/zmh52wnfvM)
 
 ## Contents
 
-- [Overview](#Overview)
+- [Overview](#overview)
 - [Functionality](#functionality)
 - [Examples](#examples)
 - [Installation](#installation)
 - [Documentation](#documentation)
 - [Contribution](#contribution)
 - [Change Log](CHANGELOG.md)
```

### Comparing `dhooks_lite-0.6.1/dhooks_lite/client.py` & `dhooks_lite-1.0.0a1/dhooks_lite/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dhooks_lite.embed import Embed
 import json
 import logging
 import requests
 from time import sleep
-from typing import List
+from typing import List, Optional
 
 from .constants import APP_NAME, APP_VERSION, HOMEPAGE_URL
 from .serializers import JsonDateTimeEncoder
 
 
 logger = logging.getLogger(__name__)
 
@@ -19,15 +19,17 @@
 HTTP_SERVICE_UNAVAILABLE = 503
 HTTP_GATEWAY_TIMEOUT = 504
 
 
 class WebhookResponse:
     """response from a Discord Webhook"""
 
-    def __init__(self, headers: dict, status_code: int, content: dict = None) -> None:
+    def __init__(
+        self, headers: dict, status_code: int, content: Optional[dict] = None
+    ) -> None:
         self._headers = dict(headers)
         self._status_code = int(status_code)
         self._content = dict(content) if content else None
 
     @property
     def headers(self) -> dict:
         """response headers"""
@@ -35,15 +37,15 @@
 
     @property
     def status_code(self) -> int:
         """HTTP status code of the response"""
         return self._status_code
 
     @property
-    def content(self) -> dict:
+    def content(self) -> Optional[dict]:
         """content of the response, e.g. send report
 
         will be empty if not waited for response from Discord
         """
         return self._content
 
     @property
@@ -86,17 +88,17 @@
     """A Discord Webhook"""
 
     MAX_CHARACTERS = 2000
 
     def __init__(
         self,
         url: str,
-        username: str = None,
-        avatar_url: str = None,
-        user_agent: UserAgent = None,
+        username: Optional[str] = None,
+        avatar_url: Optional[str] = None,
+        user_agent: Optional[UserAgent] = None,
     ) -> None:
         """Initialize a Webhook object
 
         Args:
             url: Discord webhook url
             username: Override default user name of the webhook
             avatar_url: Override default avatar icon of the webhook with image URL
@@ -114,37 +116,37 @@
         return f"{type(self).__name__}(url='{self.url}'')"
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
-    def username(self) -> str:
+    def username(self) -> Optional[str]:
         return self._username
 
     @property
-    def avatar_url(self) -> str:
+    def avatar_url(self) -> Optional[str]:
         return self._avatar_url
 
     @property
     def user_agent(self) -> UserAgent:
         return (
             self._user_agent
             if self._user_agent
             else UserAgent(APP_NAME, HOMEPAGE_URL, APP_VERSION)
         )
 
     def execute(
         self,
-        content: str = None,
-        embeds: List[Embed] = None,
-        tts: bool = None,
-        username: str = None,
-        avatar_url: str = None,
-        wait_for_response: bool = False,
+        content: Optional[str] = None,
+        embeds: Optional[List[Embed]] = None,
+        tts: Optional[bool] = None,
+        username: Optional[str] = None,
+        avatar_url: Optional[str] = None,
+        wait_for_response: Optional[bool] = False,
         max_retries: int = MAX_RETRIES,
     ) -> WebhookResponse:
         """Posts a message to this webhook
 
         Args:
             content: Text of this message
             embeds:List of Embed objects to be attached to this message
@@ -218,49 +220,49 @@
 
         try:
             content_returned = r.json()
         except ValueError:
             content_returned = None
 
         response = WebhookResponse(
-            headers=r.headers, status_code=r.status_code, content=content_returned
+            headers=dict(r.headers), status_code=r.status_code, content=content_returned
         )
         return response
 
-    def _set_content(self, payload: dict, content: str) -> None:
+    def _set_content(self, payload: dict, content: Optional[str]) -> None:
         if content:
             content = str(content)
             if len(content) > self.MAX_CHARACTERS:
                 raise ValueError("content exceeds {}".format(self.MAX_CHARACTERS))
             payload["content"] = content
 
-    def _set_embeds(self, payload: dict, embeds: list) -> None:
+    def _set_embeds(self, payload: dict, embeds: Optional[list]) -> None:
         if embeds:
             if not isinstance(embeds, list):
                 raise TypeError("embeds must be of type list")
 
             for embed in embeds:
                 if type(embed).__name__ != "Embed":
                     raise TypeError("embeds elements must be of type Embed")
 
             payload["embeds"] = [x.asdict() for x in embeds]
 
-    def _set_username(self, payload: dict, username: str) -> None:
+    def _set_username(self, payload: dict, username: Optional[str]) -> None:
         if not username and self._username:
             username = self._username
 
         if username:
             payload["username"] = str(username)
 
-    def _set_avatar_url(self, payload: dict, avatar_url: str) -> None:
+    def _set_avatar_url(self, payload: dict, avatar_url: Optional[str]) -> None:
         if not avatar_url and self._avatar_url:
             avatar_url = self._avatar_url
 
         if avatar_url:
             payload["avatar_url"] = str(avatar_url)
 
-    def _set_tts(self, payload: dict, tts: bool) -> None:
-        if tts:
+    def _set_tts(self, payload: dict, tts: Optional[bool]) -> None:
+        if tts is not None:
             if not isinstance(tts, bool):
                 raise TypeError("tts must be of type bool")
 
             payload["tts"] = tts
```

### Comparing `dhooks_lite-0.6.1/dhooks_lite.egg-info/PKG-INFO` & `dhooks_lite-1.0.0a1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,171 +1,175 @@
 Metadata-Version: 2.1
-Name: dhooks-lite
-Version: 0.6.1
+Name: dhooks_lite
+Version: 1.0.0a1
 Summary: Another simple class wrapper for interacting with Discord webhooks in Python 3
 Home-page: https://github.com/ErikKalkoken/dhooks-lite
 Author: Erik Kalkoken
 Author-email: kalkoken87@gmail.com
 License: MIT
-Description: # dhooks-lite
-        
-        ![version](https://img.shields.io/pypi/v/dhooks-lite)
-        ![python](https://img.shields.io/pypi/pyversions/dhooks-lite)
-        ![license](https://img.shields.io/github/license/ErikKalkoken/dhooks-lite)
-        ![build](https://api.travis-ci.org/ErikKalkoken/dhooks-lite.svg?branch=master)
-        [![codecov](https://codecov.io/gh/ErikKalkoken/dhooks-lite/branch/master/graph/badge.svg)](https://codecov.io/gh/ErikKalkoken/dhooks-lite)
-        [![Documentation Status](https://readthedocs.org/projects/dhooks-lite/badge/?version=latest)](https://dhooks-lite.readthedocs.io/en/latest/?badge=latest)
-        [![Downloads](https://pepy.tech/badge/dhooks-lite)](https://pepy.tech/project/dhooks-lite)
-        
-        ## Contents
-        
-        - [Overview](#Overview)
-        - [Functionality](#functionality)
-        - [Examples](#examples)
-        - [Installation](#installation)
-        - [Documentation](#documentation)
-        - [Contribution](#contribution)
-        - [Change Log](CHANGELOG.md)
-        
-        ## Overview
-        
-        **dhooks-lite** is a library with a set of classes for interacting with Discord webhooks written in Python 3.
-        
-        This library aims to differentiate itself from similar libraries with the following properties:
-        
-        - is fully tested
-        - simple to use (only one way of doing things, same name of attributes and objects as in the [official Discord documentation](https://discordapp.com/developers/docs/resources/webhook#execute-webhook))
-        - has logging
-        - requests are automatically retried and have sensible timeouts
-        
-        ## Functionality
-        
-        This library provides following functionality:
-        
-        - Posting messages in Discord channels via webhooks (synchronous calls only)
-        - Attaching Embeds to messages
-        - Retrieve send reports and from Discord
-        - Retrieve HTTP status and headers from Discord, e.g. for implementing rate limit handling
-        
-        ## Examples
-        
-        Here are some examples on how to use dhooks-lite in your Python scripts.
-        
-        Note that you also find the source code of all examples in the `/examples` folder of this repo.
-        
-        ### Hello World
-        
-        Minimal example for posting a message.
-        
-        ```python
-        from dhooks_lite import Webhook
-        
-        hook = Webhook(DISCORD_WEBHOOK_URL)
-        hook.execute('Hello, World!')
-        ```
-        
-        ![example1](https://i.imgur.com/t3mxMAJ.png)
-        
-        ### Posting with custom avatar
-        
-        In this example we are setting username and avatar.
-        
-        ```python
-        from dhooks_lite import Webhook
-        
-        hook = Webhook(
-            DISCORD_WEBHOOK_URL,
-            username='Bruce Wayne',
-            avatar_url='https://i.imgur.com/thK8erv.png'
-        )
-        hook.execute('I am Batman!')
-        ```
-        
-        ![example2](https://i.imgur.com/mseg2Yx.png)
-        
-        ### Complete example with embeds
-        
-        Finally, here is an example for posting a message with two embeds and using all available features (shortened):
-        
-        ```python
-        import datetime
-        from dhooks_lite import Webhook, Embed, Footer, Image, Thumbnail, Author, Field
-        
-        hook = Webhook(DISCORD_WEBHOOK_URL)
-        e1 = Embed(
-            description='Only a few years ago, scientists stumbled upon an electrical current of cosmic proportions.(...)',
-            title='Universe\'s highest electric current found',
-            url='https://www.newscientist.com/article/mg21028174-900-universes-highest-electric-current-found/',
-            timestamp=datetime.datetime.utcnow(),
-            color=0x5CDBF0,
-            footer=Footer(
-                'Science Department',
-                'https://i.imgur.com/Bgsv04h.png'
-            ),
-            image=Image('https://i.imgur.com/eis1Y0P.jpg'),
-            thumbnail=Thumbnail('https://i.imgur.com/2A4k28x.jpg'),
-            author=Author(
-                'John Scientist',
-                url='https://en.wikipedia.org/wiki/Albert_Einstein',
-                icon_url='https://i.imgur.com/1JoHDw1.png'
-            ),
-            fields=[
-                Field('1st Measurement', 'Failed'),
-                Field('2nd Measurement', 'Succeeded')
-            ]
-        )
-        e2 = Embed(description="TOP SECRET - Do not distribute!")
-        
-        hook.execute(
-            'Checkout this new report from the science department:',
-            username='Bruce Wayne',
-            avatar_url='https://i.imgur.com/thK8erv.png',
-            embeds=[e1, e2],
-            wait_for_response=True
-        )
-        ```
-        
-        ![example2](https://i.imgur.com/RoWBh2n.png)
-        
-        ## Installation
-        
-        You can install this library directly from PyPI:
-        
-        ```bash
-        pip install dhooks-lite
-        ```
-        
-        ## Documentation
-        
-        For a full documentation of all classes please see the official docs [here](https://dhooks-lite.readthedocs.io/en/latest/).
-        
-        ## Contribution
-        
-        We welcome any contribution!
-        
-        If you found a bug or have a feature request please raise an issue.
-        
-        If you want to help further improve this library please feel free to issue a merge request. Please adhere to the following requirements in your change:
-        
-        - Code should be compliant with [PEP8](https://www.python.org/dev/peps/pep-0008/)
-        - Full overage by unit tests
-        - All classes should be immutable
-        - All classes and their public methods must have docstring documentation
-        - All changes must be documented in the Change Log
-        
 Keywords: discord,webhooks,discordwebhooks,discordhooks
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Natural Language :: English
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: ~=3.6
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# dhooks-lite
+
+[![release](https://img.shields.io/pypi/v/dhooks-lite?label=release)](https://pypi.org/project/dhooks-lite/)
+[![python](https://img.shields.io/pypi/pyversions/dhooks-lite)](https://pypi.org/project/dhooks-lite/)
+[![pipeline status](https://gitlab.com/ErikKalkoken/dhooks-lite/badges/master/pipeline.svg)](https://gitlab.com/ErikKalkoken/dhooks-lite/-/commits/master)
+[![codecov](https://codecov.io/gl/ErikKalkoken/dhooks-lite/branch/master/graph/badge.svg?token=9YNL3HEJ5D)](https://codecov.io/gl/ErikKalkoken/dhooks-lite)
+[![Documentation Status](https://readthedocs.org/projects/dhooks-lite/badge/?version=latest)](https://dhooks-lite.readthedocs.io/en/latest/?badge=latest)
+[![license](https://img.shields.io/badge/license-MIT-green)](https://gitlab.com/ErikKalkoken/dhooks-lite/-/blob/master/LICENSE)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![chat](https://img.shields.io/discord/790364535294132234)](https://discord.gg/zmh52wnfvM)
+
+## Contents
+
+- [Overview](#overview)
+- [Functionality](#functionality)
+- [Examples](#examples)
+- [Installation](#installation)
+- [Documentation](#documentation)
+- [Contribution](#contribution)
+- [Change Log](CHANGELOG.md)
+
+## Overview
+
+**dhooks-lite** is a library with a set of classes for interacting with Discord webhooks written in Python 3.
+
+This library aims to differentiate itself from similar libraries with the following properties:
+
+- is fully tested
+- simple to use (only one way of doing things, same name of attributes and objects as in the [official Discord documentation](https://discordapp.com/developers/docs/resources/webhook#execute-webhook))
+- has logging
+- requests are automatically retried and have sensible timeouts
+
+## Functionality
+
+This library provides following functionality:
+
+- Posting messages in Discord channels via webhooks (synchronous calls only)
+- Attaching Embeds to messages
+- Retrieve send reports and from Discord
+- Retrieve HTTP status and headers from Discord, e.g. for implementing rate limit handling
+
+## Examples
+
+Here are some examples on how to use dhooks-lite in your Python scripts.
+
+Note that you also find the source code of all examples in the `/examples` folder of this repo.
+
+### Hello World
+
+Minimal example for posting a message.
+
+```python
+from dhooks_lite import Webhook
+
+hook = Webhook(DISCORD_WEBHOOK_URL)
+hook.execute('Hello, World!')
+```
+
+![example1](https://i.imgur.com/t3mxMAJ.png)
+
+### Posting with custom avatar
+
+In this example we are setting username and avatar.
+
+```python
+from dhooks_lite import Webhook
+
+hook = Webhook(
+    DISCORD_WEBHOOK_URL,
+    username='Bruce Wayne',
+    avatar_url='https://i.imgur.com/thK8erv.png'
+)
+hook.execute('I am Batman!')
+```
+
+![example2](https://i.imgur.com/mseg2Yx.png)
+
+### Complete example with embeds
+
+Finally, here is an example for posting a message with two embeds and using all available features (shortened):
+
+```python
+import datetime
+from dhooks_lite import Webhook, Embed, Footer, Image, Thumbnail, Author, Field
+
+hook = Webhook(DISCORD_WEBHOOK_URL)
+e1 = Embed(
+    description='Only a few years ago, scientists stumbled upon an electrical current of cosmic proportions.(...)',
+    title='Universe\'s highest electric current found',
+    url='https://www.newscientist.com/article/mg21028174-900-universes-highest-electric-current-found/',
+    timestamp=datetime.datetime.utcnow(),
+    color=0x5CDBF0,
+    footer=Footer(
+        'Science Department',
+        'https://i.imgur.com/Bgsv04h.png'
+    ),
+    image=Image('https://i.imgur.com/eis1Y0P.jpg'),
+    thumbnail=Thumbnail('https://i.imgur.com/2A4k28x.jpg'),
+    author=Author(
+        'John Scientist',
+        url='https://en.wikipedia.org/wiki/Albert_Einstein',
+        icon_url='https://i.imgur.com/1JoHDw1.png'
+    ),
+    fields=[
+        Field('1st Measurement', 'Failed'),
+        Field('2nd Measurement', 'Succeeded')
+    ]
+)
+e2 = Embed(description="TOP SECRET - Do not distribute!")
+
+hook.execute(
+    'Checkout this new report from the science department:',
+    username='Bruce Wayne',
+    avatar_url='https://i.imgur.com/thK8erv.png',
+    embeds=[e1, e2],
+    wait_for_response=True
+)
+```
+
+![example2](https://i.imgur.com/RoWBh2n.png)
+
+## Installation
+
+You can install this library directly from PyPI:
+
+```bash
+pip install dhooks-lite
+```
+
+## Documentation
+
+For a full documentation of all classes please see the official docs [here](https://dhooks-lite.readthedocs.io/en/latest/).
+
+## Contribution
+
+We welcome any contribution!
+
+If you found a bug or have a feature request please raise an issue.
+
+If you want to help further improve this library please feel free to issue a merge request. Please adhere to the following requirements in your change:
+
+- Code should be compliant with [PEP8](https://www.python.org/dev/peps/pep-0008/)
+- Full overage by unit tests
+- All classes should be immutable
+- All classes and their public methods must have docstring documentation
+- All changes must be documented in the Change Log
```

### Comparing `dhooks_lite-0.6.1/setup.py` & `dhooks_lite-1.0.0a1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import os
 from setuptools import find_packages, setup
 
-
 # read the contents of your README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="dhooks_lite",
-    version="0.6.1",
+    version="1.0.0a1",
     packages=find_packages(),
     include_package_data=True,
     license="MIT",
     description=(
         "Another simple class wrapper for interacting with "
         "Discord webhooks in Python 3"
     ),
@@ -31,16 +30,18 @@
         "License :: OSI Approved :: MIT License",  # example license
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: CPython",
         "Natural Language :: English",
         "Topic :: Communications :: Chat",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
-    python_requires="~=3.6",
+    python_requires=">=3.6",
     install_requires=["requests"],
 )
```

