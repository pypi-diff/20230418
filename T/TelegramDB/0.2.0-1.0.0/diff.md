# Comparing `tmp/TelegramDB-0.2.0.tar.gz` & `tmp/TelegramDB-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TelegramDB-0.2.0.tar", last modified: Sun Jan 23 16:23:19 2022, max compression
+gzip compressed data, was "TelegramDB-1.0.0.tar", last modified: Tue Apr 18 14:54:39 2023, max compression
```

## Comparing `TelegramDB-0.2.0.tar` & `TelegramDB-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-01-23 16:23:19.626603 TelegramDB-0.2.0/
--rw-rw-rw-   0        0        0     3254 2022-01-23 16:23:19.624607 TelegramDB-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1884 2022-01-23 16:16:48.000000 TelegramDB-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2022-01-23 16:23:19.617653 TelegramDB-0.2.0/TelegramDB.egg-info/
--rw-rw-rw-   0        0        0     3254 2022-01-23 16:23:19.000000 TelegramDB-0.2.0/TelegramDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2022-01-23 16:23:19.000000 TelegramDB-0.2.0/TelegramDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-23 16:23:19.000000 TelegramDB-0.2.0/TelegramDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2022-01-23 16:23:19.000000 TelegramDB-0.2.0/TelegramDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2022-01-23 16:23:19.000000 TelegramDB-0.2.0/TelegramDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-01-23 16:23:19.626603 TelegramDB-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1257 2022-01-23 16:23:19.000000 TelegramDB-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-01-23 16:23:19.618623 TelegramDB-0.2.0/telegram/
--rw-rw-rw-   0        0        0      188 2022-01-22 15:46:39.000000 TelegramDB-0.2.0/telegram/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-23 16:23:19.623611 TelegramDB-0.2.0/telegramdb/
--rw-rw-rw-   0        0        0      791 2022-01-22 15:47:28.000000 TelegramDB-0.2.0/telegramdb/__init__.py
--rw-rw-rw-   0        0        0      762 2022-01-23 16:23:19.000000 TelegramDB-0.2.0/telegramdb/constants.py
--rw-rw-rw-   0        0        0    16358 2022-01-22 15:52:43.000000 TelegramDB-0.2.0/telegramdb/database.py
--rw-rw-rw-   0        0        0     1691 2022-01-22 15:46:39.000000 TelegramDB-0.2.0/telegramdb/exceptions.py
+drwxrwxr-x   0 dell      (1000) dell      (1000)        0 2023-04-18 14:54:39.560257 TelegramDB-1.0.0/
+-rw-rw-r--   0 dell      (1000) dell      (1000)     3063 2023-04-18 14:54:39.560257 TelegramDB-1.0.0/PKG-INFO
+-rw-rw-r--   0 dell      (1000) dell      (1000)     1724 2023-04-18 08:40:36.000000 TelegramDB-1.0.0/README.md
+drwxrwxr-x   0 dell      (1000) dell      (1000)        0 2023-04-18 14:54:39.560257 TelegramDB-1.0.0/TelegramDB.egg-info/
+-rw-rw-r--   0 dell      (1000) dell      (1000)     3063 2023-04-18 14:54:38.000000 TelegramDB-1.0.0/TelegramDB.egg-info/PKG-INFO
+-rw-rw-r--   0 dell      (1000) dell      (1000)      282 2023-04-18 14:54:38.000000 TelegramDB-1.0.0/TelegramDB.egg-info/SOURCES.txt
+-rw-rw-r--   0 dell      (1000) dell      (1000)        1 2023-04-18 14:54:38.000000 TelegramDB-1.0.0/TelegramDB.egg-info/dependency_links.txt
+-rw-rw-r--   0 dell      (1000) dell      (1000)       71 2023-04-18 14:54:38.000000 TelegramDB-1.0.0/TelegramDB.egg-info/requires.txt
+-rw-rw-r--   0 dell      (1000) dell      (1000)       11 2023-04-18 14:54:38.000000 TelegramDB-1.0.0/TelegramDB.egg-info/top_level.txt
+-rw-rw-r--   0 dell      (1000) dell      (1000)       38 2023-04-18 14:54:39.560257 TelegramDB-1.0.0/setup.cfg
+-rw-rw-r--   0 dell      (1000) dell      (1000)     1223 2023-04-18 14:21:35.000000 TelegramDB-1.0.0/setup.py
+drwxrwxr-x   0 dell      (1000) dell      (1000)        0 2023-04-18 14:54:39.560257 TelegramDB-1.0.0/telegramdb/
+-rw-rw-r--   0 dell      (1000) dell      (1000)      772 2023-04-18 14:21:19.000000 TelegramDB-1.0.0/telegramdb/__init__.py
+-rw-rw-r--   0 dell      (1000) dell      (1000)      744 2023-04-18 14:21:19.000000 TelegramDB-1.0.0/telegramdb/constants.py
+-rw-rw-r--   0 dell      (1000) dell      (1000)    15951 2023-04-18 14:50:50.000000 TelegramDB-1.0.0/telegramdb/database.py
+-rw-rw-r--   0 dell      (1000) dell      (1000)     1649 2023-04-18 14:21:19.000000 TelegramDB-1.0.0/telegramdb/exceptions.py
```

### Comparing `TelegramDB-0.2.0/PKG-INFO` & `TelegramDB-1.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,78 +1,77 @@
-Metadata-Version: 2.1
-Name: TelegramDB
-Version: 0.2.0
-Summary: A library that uses your telegram account as a database for your project.
-Home-page: https://github.com/AnimeKaizoku/TelegramDB
-Author: Anony
-Author-email: contact@anonyindian.me
-License: GPLv3
-Description: # TelegramDB
-        A library which uses your telegram account as a database for your projects.
-        
-        **Documentation**: [telegramdb.readthedocs.io](https://telegramdb.readthedocs.io/) 
-        
-        [![pypi](https://img.shields.io/pypi/v/telegramdb.svg)](https://pypi.org/project/TelegramDB)
-        [![pyversion](https://img.shields.io/pypi/pyversions/telegramdb.svg)](https://pypi.org/project/TelegramDB)
-        [![downlaods](https://img.shields.io/pypi/dm/TelegramDB)](https://pypistats.org/packages/telegramdb)
-        [![docs](https://readthedocs.org/projects/telegramdb/badge/?version=stable)](https://telegramdb.readthedocs.io/en/latest/)
-        [![license](https://img.shields.io/pypi/l/telegramdb.svg)](https://www.gnu.org/licenses/gpl-3.0.en.html)
-        
-        ## Basic Usage
-        ```python
-        from os import getenv
-        from pyrogram import Client
-        from telegramdb import TelegramDB, DataPack, Member
-        
-        client = Client("session_name", getenv("API_ID"), getenv("API_HASH"))
-        client.start()
-        SESSION = TelegramDB(client, getenv("DB_CHAT_ID"))
-        
-        class TestData(DataPack):
-            __datapack_name__ = "test"
-        
-            id = Member(int, is_primary=True)
-            name = Member(str)
-        
-            def __init__(self, id):
-                self.id = id
-        
-        SESSION.prepare_datapack(TestData)
-        
-        test = TestData(777000)
-        test.name = "Telegram"
-        SESSION.commit(test)
-        ```
-        
-        ## Installation
-        You can install this library by using standard pip command.
-        ```bash
-        pip install TelegramDB
-        ```
-        
-        ## Requirements
-        - Python 3.6 or higher
-        - A telegram client
-        
-        ## Contributing
-        Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-        
-        Please make sure to update examples as appropriate.
-        
-        ## License
-        [![GPLv3](https://www.gnu.org/graphics/gplv3-127x51.png)](https://www.gnu.org/licenses/gpl-3.0.en.html)
-        <br>Licensed Under <a href="https://www.gnu.org/licenses/gpl-3.0.en.html">GNU General Public License v3</a>
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: TelegramDB
+Version: 1.0.0
+Summary: A library that uses your telegram account as a database for your project.
+Home-page: https://github.com/AnimeKaizoku/TelegramDB
+Author: Anony
+Author-email: contact@anonyindian.me
+License: GPLv3
+Description: # TelegramDB
+        A library which uses your telegram account as a database for your projects.
+        
+        **Documentation**: [telegramdb.readthedocs.io](https://telegramdb.readthedocs.io/) 
+        
+        [![pypi](https://img.shields.io/pypi/v/telegramdb.svg)](https://pypi.org/project/TelegramDB)
+        [![pyversion](https://img.shields.io/pypi/pyversions/telegramdb.svg)](https://pypi.org/project/TelegramDB)
+        [![downlaods](https://img.shields.io/pypi/dm/telegramdb)](https://pypistats.org/packages/telegramdb)
+        [![docs](https://readthedocs.org/projects/telegramdb/badge/?version=stable)](https://telegramdb.readthedocs.io/en/latest/)
+        
+        ## Basic Usage
+        ```python
+        from os import getenv
+        from pyrogram import Client
+        from telegramdb import TelegramDB, DataPack, Member
+        
+        client = Client("session_name", getenv("API_ID"), getenv("API_HASH"))
+        client.start()
+        SESSION = TelegramDB(client, getenv("DB_CHAT_ID"))
+        
+        class TestData(DataPack):
+            __datapack_name__ = "test"
+        
+            id = Member(int, is_primary=True)
+            name = Member(str)
+        
+            def __init__(self, id):
+                self.id = id
+        
+        SESSION.prepare_datapack(TestData)
+        
+        test = TestData(777000)
+        test.name = "Telegram"
+        SESSION.commit(test)
+        ```
+        
+        ## Installation
+        You can install this library by using standard pip command.
+        ```bash
+        pip install TelegramDB
+        ```
+        
+        ## Requirements
+        - Python 3.6 or higher
+        - A telegram client
+        
+        ## Contributing
+        Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+        
+        Please make sure to update examples as appropriate.
+        
+        ## License
+        [![GPLv3](https://www.gnu.org/graphics/gplv3-127x51.png)](https://www.gnu.org/licenses/gpl-3.0.en.html)
+        <br>Licensed Under <a href="https://www.gnu.org/licenses/gpl-3.0.en.html">GNU General Public License v3</a>
+        
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

### Comparing `TelegramDB-0.2.0/README.md` & `TelegramDB-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,54 @@
-# TelegramDB
-A library which uses your telegram account as a database for your projects.
-
-**Documentation**: [telegramdb.readthedocs.io](https://telegramdb.readthedocs.io/) 
-
-[![pypi](https://img.shields.io/pypi/v/telegramdb.svg)](https://pypi.org/project/TelegramDB)
-[![pyversion](https://img.shields.io/pypi/pyversions/telegramdb.svg)](https://pypi.org/project/TelegramDB)
-[![downlaods](https://img.shields.io/pypi/dm/TelegramDB)](https://pypistats.org/packages/telegramdb)
-[![docs](https://readthedocs.org/projects/telegramdb/badge/?version=stable)](https://telegramdb.readthedocs.io/en/latest/)
-[![license](https://img.shields.io/pypi/l/telegramdb.svg)](https://www.gnu.org/licenses/gpl-3.0.en.html)
-
-## Basic Usage
-```python
-from os import getenv
-from pyrogram import Client
-from telegramdb import TelegramDB, DataPack, Member
-
-client = Client("session_name", getenv("API_ID"), getenv("API_HASH"))
-client.start()
-SESSION = TelegramDB(client, getenv("DB_CHAT_ID"))
-
-class TestData(DataPack):
-    __datapack_name__ = "test"
-
-    id = Member(int, is_primary=True)
-    name = Member(str)
-
-    def __init__(self, id):
-        self.id = id
-
-SESSION.prepare_datapack(TestData)
-
-test = TestData(777000)
-test.name = "Telegram"
-SESSION.commit(test)
-```
-
-## Installation
-You can install this library by using standard pip command.
-```bash
-pip install TelegramDB
-```
-
-## Requirements
-- Python 3.6 or higher
-- A telegram client
-
-## Contributing
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-
-Please make sure to update examples as appropriate.
-
-## License
-[![GPLv3](https://www.gnu.org/graphics/gplv3-127x51.png)](https://www.gnu.org/licenses/gpl-3.0.en.html)
-<br>Licensed Under <a href="https://www.gnu.org/licenses/gpl-3.0.en.html">GNU General Public License v3</a>
+# TelegramDB
+A library which uses your telegram account as a database for your projects.
+
+**Documentation**: [telegramdb.readthedocs.io](https://telegramdb.readthedocs.io/) 
+
+[![pypi](https://img.shields.io/pypi/v/telegramdb.svg)](https://pypi.org/project/TelegramDB)
+[![pyversion](https://img.shields.io/pypi/pyversions/telegramdb.svg)](https://pypi.org/project/TelegramDB)
+[![downlaods](https://img.shields.io/pypi/dm/telegramdb)](https://pypistats.org/packages/telegramdb)
+[![docs](https://readthedocs.org/projects/telegramdb/badge/?version=stable)](https://telegramdb.readthedocs.io/en/latest/)
+
+## Basic Usage
+```python
+from os import getenv
+from pyrogram import Client
+from telegramdb import TelegramDB, DataPack, Member
+
+client = Client("session_name", getenv("API_ID"), getenv("API_HASH"))
+client.start()
+SESSION = TelegramDB(client, getenv("DB_CHAT_ID"))
+
+class TestData(DataPack):
+    __datapack_name__ = "test"
+
+    id = Member(int, is_primary=True)
+    name = Member(str)
+
+    def __init__(self, id):
+        self.id = id
+
+SESSION.prepare_datapack(TestData)
+
+test = TestData(777000)
+test.name = "Telegram"
+SESSION.commit(test)
+```
+
+## Installation
+You can install this library by using standard pip command.
+```bash
+pip install TelegramDB
+```
+
+## Requirements
+- Python 3.6 or higher
+- A telegram client
+
+## Contributing
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+Please make sure to update examples as appropriate.
+
+## License
+[![GPLv3](https://www.gnu.org/graphics/gplv3-127x51.png)](https://www.gnu.org/licenses/gpl-3.0.en.html)
+<br>Licensed Under <a href="https://www.gnu.org/licenses/gpl-3.0.en.html">GNU General Public License v3</a>
```

### Comparing `TelegramDB-0.2.0/TelegramDB.egg-info/PKG-INFO` & `TelegramDB-1.0.0/TelegramDB.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,78 +1,77 @@
-Metadata-Version: 2.1
-Name: TelegramDB
-Version: 0.2.0
-Summary: A library that uses your telegram account as a database for your project.
-Home-page: https://github.com/AnimeKaizoku/TelegramDB
-Author: Anony
-Author-email: contact@anonyindian.me
-License: GPLv3
-Description: # TelegramDB
-        A library which uses your telegram account as a database for your projects.
-        
-        **Documentation**: [telegramdb.readthedocs.io](https://telegramdb.readthedocs.io/) 
-        
-        [![pypi](https://img.shields.io/pypi/v/telegramdb.svg)](https://pypi.org/project/TelegramDB)
-        [![pyversion](https://img.shields.io/pypi/pyversions/telegramdb.svg)](https://pypi.org/project/TelegramDB)
-        [![downlaods](https://img.shields.io/pypi/dm/TelegramDB)](https://pypistats.org/packages/telegramdb)
-        [![docs](https://readthedocs.org/projects/telegramdb/badge/?version=stable)](https://telegramdb.readthedocs.io/en/latest/)
-        [![license](https://img.shields.io/pypi/l/telegramdb.svg)](https://www.gnu.org/licenses/gpl-3.0.en.html)
-        
-        ## Basic Usage
-        ```python
-        from os import getenv
-        from pyrogram import Client
-        from telegramdb import TelegramDB, DataPack, Member
-        
-        client = Client("session_name", getenv("API_ID"), getenv("API_HASH"))
-        client.start()
-        SESSION = TelegramDB(client, getenv("DB_CHAT_ID"))
-        
-        class TestData(DataPack):
-            __datapack_name__ = "test"
-        
-            id = Member(int, is_primary=True)
-            name = Member(str)
-        
-            def __init__(self, id):
-                self.id = id
-        
-        SESSION.prepare_datapack(TestData)
-        
-        test = TestData(777000)
-        test.name = "Telegram"
-        SESSION.commit(test)
-        ```
-        
-        ## Installation
-        You can install this library by using standard pip command.
-        ```bash
-        pip install TelegramDB
-        ```
-        
-        ## Requirements
-        - Python 3.6 or higher
-        - A telegram client
-        
-        ## Contributing
-        Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-        
-        Please make sure to update examples as appropriate.
-        
-        ## License
-        [![GPLv3](https://www.gnu.org/graphics/gplv3-127x51.png)](https://www.gnu.org/licenses/gpl-3.0.en.html)
-        <br>Licensed Under <a href="https://www.gnu.org/licenses/gpl-3.0.en.html">GNU General Public License v3</a>
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: TelegramDB
+Version: 1.0.0
+Summary: A library that uses your telegram account as a database for your project.
+Home-page: https://github.com/AnimeKaizoku/TelegramDB
+Author: Anony
+Author-email: contact@anonyindian.me
+License: GPLv3
+Description: # TelegramDB
+        A library which uses your telegram account as a database for your projects.
+        
+        **Documentation**: [telegramdb.readthedocs.io](https://telegramdb.readthedocs.io/) 
+        
+        [![pypi](https://img.shields.io/pypi/v/telegramdb.svg)](https://pypi.org/project/TelegramDB)
+        [![pyversion](https://img.shields.io/pypi/pyversions/telegramdb.svg)](https://pypi.org/project/TelegramDB)
+        [![downlaods](https://img.shields.io/pypi/dm/telegramdb)](https://pypistats.org/packages/telegramdb)
+        [![docs](https://readthedocs.org/projects/telegramdb/badge/?version=stable)](https://telegramdb.readthedocs.io/en/latest/)
+        
+        ## Basic Usage
+        ```python
+        from os import getenv
+        from pyrogram import Client
+        from telegramdb import TelegramDB, DataPack, Member
+        
+        client = Client("session_name", getenv("API_ID"), getenv("API_HASH"))
+        client.start()
+        SESSION = TelegramDB(client, getenv("DB_CHAT_ID"))
+        
+        class TestData(DataPack):
+            __datapack_name__ = "test"
+        
+            id = Member(int, is_primary=True)
+            name = Member(str)
+        
+            def __init__(self, id):
+                self.id = id
+        
+        SESSION.prepare_datapack(TestData)
+        
+        test = TestData(777000)
+        test.name = "Telegram"
+        SESSION.commit(test)
+        ```
+        
+        ## Installation
+        You can install this library by using standard pip command.
+        ```bash
+        pip install TelegramDB
+        ```
+        
+        ## Requirements
+        - Python 3.6 or higher
+        - A telegram client
+        
+        ## Contributing
+        Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+        
+        Please make sure to update examples as appropriate.
+        
+        ## License
+        [![GPLv3](https://www.gnu.org/graphics/gplv3-127x51.png)](https://www.gnu.org/licenses/gpl-3.0.en.html)
+        <br>Licensed Under <a href="https://www.gnu.org/licenses/gpl-3.0.en.html">GNU General Public License v3</a>
+        
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

### Comparing `TelegramDB-0.2.0/setup.py` & `TelegramDB-1.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import setuptools
-
-with open('requirements.txt') as f:
-    dependencies = [l.strip() for l in f]
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name='TelegramDB',
-    version='0.2.0',
-    description='A library that uses your telegram account as a database for your project.',
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    license='GPLv3',
-    author='Anony',
-    author_email='contact@anonyindian.me',
-    url='https://github.com/AnimeKaizoku/TelegramDB',
-    packages=setuptools.find_packages(),
-    classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Typing :: Typed'
-    ],
-    install_requires=dependencies,
-    python_requires='>=3.6'
+import setuptools
+
+with open('requirements.txt') as f:
+    dependencies = [l.strip() for l in f]
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name='TelegramDB',
+    version='1.0.0',
+    description='A library that uses your telegram account as a database for your project.',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    license='GPLv3',
+    author='Anony',
+    author_email='contact@anonyindian.me',
+    url='https://github.com/AnimeKaizoku/TelegramDB',
+    packages=setuptools.find_packages(),
+    classifiers=[
+        'Development Status :: 4 - Beta',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: Implementation :: CPython',
+        'Typing :: Typed'
+    ],
+    install_requires=dependencies,
+    python_requires='>=3.6'
 )
```

### Comparing `TelegramDB-0.2.0/telegramdb/__init__.py` & `TelegramDB-1.0.0/telegramdb/constants.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-# TelegramDB
-# Copyright (C) 2022
-# Anony <github.com/anonyindian>
-
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-from .constants import *
-from .database import *
-
-__version__ = VERSION
+# TelegramDB
+# Copyright (C) 2023
+# Anony <github.com/anonyindian>
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+DP_NAME_SEPARATOR = '::'
+
+VERSION = "1.0.0"
```

### Comparing `TelegramDB-0.2.0/telegramdb/constants.py` & `TelegramDB-1.0.0/telegramdb/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-# TelegramDB
-# Copyright (C) 2022
-# Anony <github.com/anonyindian>
-
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-DP_NAME_SEPARATOR = '::'
-
-VERSION = "0.2.0"
+# TelegramDB
+# Copyright (C) 2023
+# Anony <github.com/anonyindian>
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+from .constants import *
+from .database import *
+
+__version__ = VERSION
```

### Comparing `TelegramDB-0.2.0/telegramdb/database.py` & `TelegramDB-1.0.0/telegramdb/database.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,404 +1,404 @@
-# TelegramDB
-# Copyright (C) 2022
-# Anony <github.com/anonyindian>
-
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-import inspect, asyncio, nest_asyncio
-from logging import Logger, getLogger
-from ast import literal_eval
-from telethon import TelegramClient
-from pyrogram import Client
-from typing import Union, List
-from .constants import DP_NAME_SEPARATOR, VERSION
-from .exceptions import InvalidClient, InvalidDataPack, ReservedCharacter
-
-nest_asyncio.apply()
-
-class Member:
-    """
-    Member of a :class:`DataPack`.
-
-    Parameters:
-        _ (:obj:`type`): Datatype of the member. 
-        is_primary (:obj:`bool`): Whether the member is a primary key or not.
-
-    Example:
-        .. code-block:: python
-
-            from telegramdb import Member
-            
-            # user_id of type int as a primary key
-            user_id = Member(int, is_primary=True)
-            
-            # text of type str
-            text = Member(str)
-    """
-    def __init__(self, _:type, is_primary:bool=False):
-        self.is_primary = is_primary
-        return
-
-class DataPack:
-    """
-    Object that contains all the data in a database.
-
-    Note:
-        Members are added as attributes in an inherited class of this object. 
-
-    Attributes:
-        __datapack_name__ (:obj:`str`): Name of the :class:`DataPack`.
-
-    Example:
-        .. code-block:: python
-
-            from telegramdb import DataPack, Member
-            class TestData(DataPack):
-                __datapack_name__ = "test"
-
-                id = Member(int, is_primary=True)
-                name = Member(str)
-
-                def __init__(self, id):
-                    self.id = id
-    """
-    __datapack_name__:str
-
-    def __get_dict__(self):
-        __dict_to_return = dict(self.__dict__)
-        if '__datapack_name__' in __dict_to_return:
-            __dict_to_return.pop('__datapack_name__')
-        return __dict_to_return
-    
-    def __query_data__(self):
-        return f"{self.__datapack_name__} - {self.__get_dict__()}"
-
-class TelegramDB:
-    """
-    Main object which initialises the telegram database session.
-
-    Parameters:
-        telegram_client (:class:`pyrogram.Client` | :class:`telethon.TelegramClient`): Telegram client which will be used to save database queries on telegram.
-        chat_id (:obj:`int` | :obj:`str`): Unique identifier for the target chat or username of the target channel (in the format ``@channelusername``).
-        debug (:obj:`bool`, Optional): Database queries will be debugged if it is set to ``True``.
-        logger (:class:`logging.Logger`, Optional): Logger which will be used for debugging.
-    
-    Example:
-        .. code-block:: python
-
-            from telegramdb import TelegramDB
-            from pyrogram import Client
-
-            client = Client(
-                "my_account",
-                api_id=12345,
-                api_hash="0123456789abcdef0123456789abcdef"
-            )
-            chat_id = 777000
-            SESSION = TelegramDB(client, chat_id)
-    """
-    __datapacks__:dict = {str:{"id":int, "data":str}}
-    __dp_cache__:dict = {}  
-    def __init__(self, telegram_client: Union[Client, TelegramClient], chat_id: Union[int, str]=None, debug: bool=False, logger: Logger=None):
-        print(f"""
-    TelegramDB v{VERSION} Copyright (C) 2022 anonyindian
-    This program comes with ABSOLUTELY NO WARRANTY.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions.
-            """)
-        self.debug = debug
-        self.__telegram_client__ = telegram_client
-        self.__loop__ = asyncio.get_event_loop()
-
-        if chat_id:
-            self.__chat_id__ = chat_id
-            self.__get_datapacks__()
-        else:
-            self.__make_chat__()
-
-        if debug:
-            if not logger:
-                self.LOGGER = getLogger()
-            else:
-                self.LOGGER = logger
-    
-    def prepare_datapack(self, datapack_class: DataPack):
-        """
-        Use this method to initialise the :class:`DataPack` with primary key member.
-
-        Parameters:
-            datapack_class (:class:`DataPack`): `DataPack` to be initialised with the primary key.
-        
-        Returns:
-            :obj:`None`
-        """
-        for i in inspect.getmembers(datapack_class):
-            if not i[0].startswith('_') and not inspect.ismethod(i[1]):
-                if isinstance(i[1], Member) and i[1].is_primary:
-                    if self.debug:
-                        self.LOGGER.info(f"Initialised {datapack_class} with primary key '{i[0]}'")
-                    self.__dp_cache__[datapack_class] = i[0]
-    
-    def commit(self, datapack: DataPack):
-        """
-        Use this method to save the data on telegram database.
-
-        Parameters:
-            datapack (:class:`DataPack`): Subclass of the `DataPack` of the data to be saved on telegram.
-
-        Returns:
-            :obj:`None`
-        """
-        if DP_NAME_SEPARATOR in datapack.__datapack_name__:
-            raise ReservedCharacter(datapack.__datapack_name__)
-        datapack = self.__fill_datapack(datapack)
-        self.__publish_data__(datapack, self.__format_datapack__(datapack))
-    
-    def __publish_data__(self, datapack: DataPack, data:str):
-        """
-        This is method is used to publish the committed data on telegram database chat.
-
-        Parameters:
-            datapack (:class:`DataPack`): Subclass of the `DataPack` of the data to be published on telegram database.
-            data (:obj:`str`): Formatted string of the data to be published on telegram database.
-
-        Returns:
-            :obj:`None`
-        """
-        client = self.__telegram_client__
-        if client:
-            msg_id = 0
-            if datapack.__datapack_name__ in self.__datapacks__:
-                msg_id:int = self.__datapacks__[datapack.__datapack_name__]["id"]
-            if isinstance(client, Client):
-                if msg_id == 0:
-                    async def publish():
-                        nonlocal msg_id
-                        msg_id = (await client.send_message(chat_id=self.__chat_id__, text=data)).message_id
-                    self.__loop__.run_until_complete(publish())
-                    self.__commit_success__ = True
-                else:
-                    self.__get_data_from_cache(datapack)
-                    if self.__format_datapack__(datapack) == data:
-                        self.__commit_success__ = False
-                        if self.debug:
-                            self.LOGGER.warning(f"Exact values already stored: {datapack.__query_data__()}")
-                    else:
-                        try:
-                            self.__loop__.run_until_complete(client.edit_message_text(chat_id=self.__chat_id__, message_id=msg_id, text=data))
-                            self.__commit_success__ = True
-                        except:
-                            self.__commit_success__ = False
-                            if self.debug:
-                                self.LOGGER.warning(f"Failed to update: {datapack.__query_data__()}")
-                        
-            elif isinstance(client, TelegramClient):
-                if msg_id == 0:
-                    async def publish():
-                        nonlocal msg_id
-                        msg_id = (await client.send_message(entity=self.__chat_id__, message=data, parse_mode=None)).id
-                    self.__loop__.run_until_complete(publish())
-                    self.__commit_success__ = True
-                else:
-                    self.__get_data_from_cache(datapack)
-                    if self.__format_datapack__(datapack) == data:
-                        self.__commit_success__ = False
-                        if self.debug:
-                            self.LOGGER.warning(f"Exact values already stored: {datapack.__query_data__()}")
-                    else:
-                        try:
-                            self.__loop__.run_until_complete(client.edit_message(entity=self.__chat_id__, message=msg_id, text=data, parse_mode=None))
-                            self.__commit_success__ = True
-                        except:
-                            self.__commit_success__ = False
-                            if self.debug:
-                                self.LOGGER.warning(f"Failed to update: {datapack.__query_data__()}")
-            else:
-                raise InvalidClient()
-            if self.debug and self.__commit_success__:
-                self.LOGGER.info(datapack.__query_data__())
-            self.__datapacks__[datapack.__datapack_name__] = {"id": msg_id, "data":datapack.__get_dict__()}
-    
-    def get(self, datapack: DataPack):
-        """
-        Use this method to get the data from telegram database.
-
-        Parameters:
-            datapack (:obj:`DataPack`): Object of the `DataPack` of the data to be retrieved from telegram database.
-
-        Returns:
-            :obj:`bool`
-        """
-        return self.__get_data_from_cache(self.__fill_datapack(datapack))
-
-    def __get_data_from_cache(self, datapack: DataPack):
-        """
-        This method fills data in the provided :obj:`DataPack` from the cache.
-
-        Parameters:
-            datapack (:obj:`DataPack`): Object of the `DataPack` of the data to be retrieved from telegram database.
-
-        Returns:
-            :obj:`bool`
-        """
-        if datapack.__datapack_name__ in self.__datapacks__:
-            data = self.__datapacks__[datapack.__datapack_name__]["data"]
-            for attribute in data:
-                setattr(datapack, attribute, data[attribute])
-            return True
-        return False
-
-    def get_all(self):
-        """
-        Use this method to get all data from telegram database.
-
-        Returns:
-            A list containing elements of object :class:`DataPack`
-        """
-        datapacks: List[DataPack] = []
-        for __datapack_name__ in self.__datapacks__:
-            data = self.__datapacks__[__datapack_name__]["data"]
-            obj = DataPack()
-            obj.__datapack_name__ = str(__datapack_name__).split(DP_NAME_SEPARATOR)[0]
-            for key in data:
-                setattr(obj, key, data[key])
-            datapacks.append(obj)
-        return datapacks
-
-    def delete(self, datapack: DataPack):
-        """
-        Use this method to delete data from telegram database.
-
-        Parameters:
-            datapack (:obj:`DataPack`): Object of the `DataPack` of the data to be retrieved from telegram database.
-
-        Returns:
-            :obj:`bool`
-        """
-        datapack = self.__fill_datapack(datapack)
-        if not datapack.__datapack_name__ in self.__datapacks__:
-            return False
-        msg_id = int(self.__datapacks__[datapack.__datapack_name__]["id"])
-        del self.__datapacks__[datapack.__datapack_name__]
-        return self.__unpublish_data__(msg_id)
-
-    def __unpublish_data__(self, msg_id: int):
-        """
-        This method is used to delete message storage of the data from telegram database.
-
-        Parameters:
-            msg_id (:obj:`int`): message id of the stored datapack to be deleted.
-
-        Returns:
-            :obj:`bool`
-        """
-        client = self.__telegram_client__
-        if client:
-            if isinstance(client, Client):
-                return self.__loop__.run_until_complete(client.delete_messages(chat_id=self.__chat_id__, message_ids=msg_id))
-            elif isinstance(client, TelegramClient):
-                try:
-                    self.__loop__.run_until_complete(client.delete_messages(entity=self.__chat_id__, message_ids=msg_id))
-                    return True
-                except:
-                    return False
-            else:
-                raise InvalidClient()
-        return False            
-
-    def __format_datapack__(self, datapack: DataPack):
-        """
-        This method is used to format the :class:`DataPack` in a string which will be published on telegram database chat.
-
-        Parameters:
-            datapack (:class:`DataPack`): Subclass of the `DataPack` of the data to be published on telegram database.
-
-        Returns:
-            :obj:`str`
-        """
-        query = f"#{datapack.__datapack_name__}"
-        query += f"\n{datapack.__get_dict__()}"
-        return query
-
-    def __get_datapacks__(self):
-        """
-        This method is used to load the existing data from the telegram database chat.
-
-        Returns:
-            :obj:`None`
-        """
-        if isinstance(self.__telegram_client__, Client):
-            from pyrogram.types import Message
-            for message in self.__telegram_client__.iter_history(self.__chat_id__):
-                message: Message = message
-                if not message.text:
-                    continue
-                try:
-                    text = message.text.markdown.split("\n", 1)
-                    self.__datapacks__[text[0][1:]] = {"id":message.message_id, "data":literal_eval(text[1])}
-                except:
-                    raise InvalidDataPack(message.message_id)
-                
-        elif isinstance(self.__telegram_client__, TelegramClient):
-            from telethon.tl.types import Message
-            for message in self.__telegram_client__.iter_messages(self.__chat_id__):
-                message: Message = message
-                if not message.message:
-                    continue
-                try:
-                    text = message.message.split("\n", 1)
-                    self.__datapacks__[text[0][1:]] = {"id":message.id, "data":literal_eval(text[1])}
-                except:
-                    raise InvalidDataPack(message.id)
-            # raise UnsupportedClient("telethon")
-        else:
-            raise InvalidClient()
-    
-    def __make_chat__(self):
-        """
-        This method is used to make the telegram database chat if not provided.
-
-        Returns:
-            :obj:`None`
-        """
-        if isinstance(self.__telegram_client__, Client):
-            chat = self.__telegram_client__.create_channel("Telegram DB")
-            self.__chat_id__ = chat.id
-        elif isinstance(self.__telegram_client__, TelegramClient):
-            from telethon import functions
-            with self.__telegram_client__ as client:
-                async def make_chat():    
-                    result = await client(functions.channels.CreateChannelRequest(
-                        title='Telegram DB',
-                        about="Channel to store DataPacks",
-                        broadcast=True,
-                    ))
-                    self.__chat_id__ = result.__dict__["chats"][0].__dict__["id"]
-                self.__loop__.run_until_complete(make_chat())
-        else:
-            raise InvalidClient()
-    
-    def __fill_datapack(self, datapack: DataPack):
-        """
-        This method is used to append the primary key in default name of the datapack, separated by `DP_NAME_SEPARATOR`. 
-
-        Parameters:
-            datapack (:class:`DataPack`): Subclass of the `DataPack` of the data to be published on telegram database.
-
-        Returns:
-            :class:`DataPack`
-        """
-        for dp in self.__dp_cache__:
-            if isinstance(datapack, dp):
-                datapack.__datapack_name__ += f"{DP_NAME_SEPARATOR}" + str(getattr(datapack, self.__dp_cache__[dp]))
-                break
+# TelegramDB
+# Copyright (C) 2023
+# Anony <github.com/anonyindian>
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+import inspect, asyncio, nest_asyncio
+from logging import Logger, getLogger
+from ast import literal_eval
+from telethon import TelegramClient
+from pyrogram import Client
+from typing import Union, List
+from .constants import DP_NAME_SEPARATOR, VERSION
+from .exceptions import InvalidClient, InvalidDataPack, ReservedCharacter
+
+nest_asyncio.apply()
+
+class Member:
+    """
+    Member of a :class:`DataPack`.
+
+    Parameters:
+        _ (:obj:`type`): Datatype of the member. 
+        is_primary (:obj:`bool`): Whether the member is a primary key or not.
+
+    Example:
+        .. code-block:: python
+
+            from telegramdb import Member
+            
+            # user_id of type int as a primary key
+            user_id = Member(int, is_primary=True)
+            
+            # text of type str
+            text = Member(str)
+    """
+    def __init__(self, _:type, is_primary:bool=False):
+        self.is_primary = is_primary
+        return
+
+class DataPack:
+    """
+    Object that contains all the data in a database.
+
+    Note:
+        Members are added as attributes in an inherited class of this object. 
+
+    Attributes:
+        __datapack_name__ (:obj:`str`): Name of the :class:`DataPack`.
+
+    Example:
+        .. code-block:: python
+
+            from telegramdb import DataPack, Member
+            class TestData(DataPack):
+                __datapack_name__ = "test"
+
+                id = Member(int, is_primary=True)
+                name = Member(str)
+
+                def __init__(self, id):
+                    self.id = id
+    """
+    __datapack_name__:str
+
+    def __get_dict__(self):
+        __dict_to_return = dict(self.__dict__)
+        if '__datapack_name__' in __dict_to_return:
+            __dict_to_return.pop('__datapack_name__')
+        return __dict_to_return
+    
+    def __query_data__(self):
+        return f"{self.__datapack_name__} - {self.__get_dict__()}"
+
+class TelegramDB:
+    """
+    Main object which initialises the telegram database session.
+
+    Parameters:
+        telegram_client (:class:`pyrogram.Client` | :class:`telethon.TelegramClient`): Telegram client which will be used to save database queries on telegram.
+        chat_id (:obj:`int` | :obj:`str`): Unique identifier for the target chat or username of the target channel (in the format ``@channelusername``).
+        debug (:obj:`bool`, Optional): Database queries will be debugged if it is set to ``True``.
+        logger (:class:`logging.Logger`, Optional): Logger which will be used for debugging.
+    
+    Example:
+        .. code-block:: python
+
+            from telegramdb import TelegramDB
+            from pyrogram import Client
+
+            client = Client(
+                "my_account",
+                api_id=12345,
+                api_hash="0123456789abcdef0123456789abcdef"
+            )
+            chat_id = 777000
+            SESSION = TelegramDB(client, chat_id)
+    """
+    __datapacks__:dict = {str:{"id":int, "data":str}}
+    __dp_cache__:dict = {}  
+    def __init__(self, telegram_client: Union[Client, TelegramClient], chat_id: Union[int, str]=None, debug: bool=False, logger: Logger=None):
+        print(f"""
+    TelegramDB v{VERSION} Copyright (C) 2023 anonyindian
+    This program comes with ABSOLUTELY NO WARRANTY.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions.
+            """)
+        self.debug = debug
+        self.__telegram_client__ = telegram_client
+        self.__loop__ = asyncio.get_event_loop()
+
+        if chat_id:
+            self.__chat_id__ = chat_id
+            self.__get_datapacks__()
+        else:
+            self.__make_chat__()
+
+        if debug:
+            if not logger:
+                self.LOGGER = getLogger()
+            else:
+                self.LOGGER = logger
+    
+    def prepare_datapack(self, datapack_class: DataPack):
+        """
+        Use this method to initialise the :class:`DataPack` with primary key member.
+
+        Parameters:
+            datapack_class (:class:`DataPack`): `DataPack` to be initialised with the primary key.
+        
+        Returns:
+            :obj:`None`
+        """
+        for i in inspect.getmembers(datapack_class):
+            if not i[0].startswith('_') and not inspect.ismethod(i[1]):
+                if isinstance(i[1], Member) and i[1].is_primary:
+                    if self.debug:
+                        self.LOGGER.info(f"Initialised {datapack_class} with primary key '{i[0]}'")
+                    self.__dp_cache__[datapack_class] = i[0]
+    
+    def commit(self, datapack: DataPack):
+        """
+        Use this method to save the data on telegram database.
+
+        Parameters:
+            datapack (:class:`DataPack`): Subclass of the `DataPack` of the data to be saved on telegram.
+
+        Returns:
+            :obj:`None`
+        """
+        if DP_NAME_SEPARATOR in datapack.__datapack_name__:
+            raise ReservedCharacter(datapack.__datapack_name__)
+        datapack = self.__fill_datapack(datapack)
+        self.__publish_data__(datapack, self.__format_datapack__(datapack))
+    
+    def __publish_data__(self, datapack: DataPack, data:str):
+        """
+        This is method is used to publish the committed data on telegram database chat.
+
+        Parameters:
+            datapack (:class:`DataPack`): Subclass of the `DataPack` of the data to be published on telegram database.
+            data (:obj:`str`): Formatted string of the data to be published on telegram database.
+
+        Returns:
+            :obj:`None`
+        """
+        client = self.__telegram_client__
+        if client:
+            msg_id = 0
+            if datapack.__datapack_name__ in self.__datapacks__:
+                msg_id:int = self.__datapacks__[datapack.__datapack_name__]["id"]
+            if isinstance(client, Client):
+                if msg_id == 0:
+                    async def publish():
+                        nonlocal msg_id
+                        msg_id = (await client.send_message(chat_id=self.__chat_id__, text=data)).id
+                    self.__loop__.run_until_complete(publish())
+                    self.__commit_success__ = True
+                else:
+                    self.__get_data_from_cache(datapack)
+                    if self.__format_datapack__(datapack) == data:
+                        self.__commit_success__ = False
+                        if self.debug:
+                            self.LOGGER.warning(f"Exact values already stored: {datapack.__query_data__()}")
+                    else:
+                        try:
+                            self.__loop__.run_until_complete(client.edit_message_text(chat_id=self.__chat_id__, message_id=msg_id, text=data))
+                            self.__commit_success__ = True
+                        except:
+                            self.__commit_success__ = False
+                            if self.debug:
+                                self.LOGGER.warning(f"Failed to update: {datapack.__query_data__()}")
+                        
+            elif isinstance(client, TelegramClient):
+                if msg_id == 0:
+                    async def publish():
+                        nonlocal msg_id
+                        msg_id = (await client.send_message(entity=self.__chat_id__, message=data, parse_mode=None)).id
+                    self.__loop__.run_until_complete(publish())
+                    self.__commit_success__ = True
+                else:
+                    self.__get_data_from_cache(datapack)
+                    if self.__format_datapack__(datapack) == data:
+                        self.__commit_success__ = False
+                        if self.debug:
+                            self.LOGGER.warning(f"Exact values already stored: {datapack.__query_data__()}")
+                    else:
+                        try:
+                            self.__loop__.run_until_complete(client.edit_message(entity=self.__chat_id__, message=msg_id, text=data, parse_mode=None))
+                            self.__commit_success__ = True
+                        except:
+                            self.__commit_success__ = False
+                            if self.debug:
+                                self.LOGGER.warning(f"Failed to update: {datapack.__query_data__()}")
+            else:
+                raise InvalidClient()
+            if self.debug and self.__commit_success__:
+                self.LOGGER.info(datapack.__query_data__())
+            self.__datapacks__[datapack.__datapack_name__] = {"id": msg_id, "data":datapack.__get_dict__()}
+    
+    def get(self, datapack: DataPack):
+        """
+        Use this method to get the data from telegram database.
+
+        Parameters:
+            datapack (:obj:`DataPack`): Object of the `DataPack` of the data to be retrieved from telegram database.
+
+        Returns:
+            :obj:`bool`
+        """
+        return self.__get_data_from_cache(self.__fill_datapack(datapack))
+
+    def __get_data_from_cache(self, datapack: DataPack):
+        """
+        This method fills data in the provided :obj:`DataPack` from the cache.
+
+        Parameters:
+            datapack (:obj:`DataPack`): Object of the `DataPack` of the data to be retrieved from telegram database.
+
+        Returns:
+            :obj:`bool`
+        """
+        if datapack.__datapack_name__ in self.__datapacks__:
+            data = self.__datapacks__[datapack.__datapack_name__]["data"]
+            for attribute in data:
+                setattr(datapack, attribute, data[attribute])
+            return True
+        return False
+
+    def get_all(self):
+        """
+        Use this method to get all data from telegram database.
+
+        Returns:
+            A list containing elements of object :class:`DataPack`
+        """
+        datapacks: List[DataPack] = []
+        for __datapack_name__ in self.__datapacks__:
+            data = self.__datapacks__[__datapack_name__]["data"]
+            obj = DataPack()
+            obj.__datapack_name__ = str(__datapack_name__).split(DP_NAME_SEPARATOR)[0]
+            for key in data:
+                setattr(obj, key, data[key])
+            datapacks.append(obj)
+        return datapacks
+
+    def delete(self, datapack: DataPack):
+        """
+        Use this method to delete data from telegram database.
+
+        Parameters:
+            datapack (:obj:`DataPack`): Object of the `DataPack` of the data to be retrieved from telegram database.
+
+        Returns:
+            :obj:`bool`
+        """
+        datapack = self.__fill_datapack(datapack)
+        if not datapack.__datapack_name__ in self.__datapacks__:
+            return False
+        msg_id = int(self.__datapacks__[datapack.__datapack_name__]["id"])
+        del self.__datapacks__[datapack.__datapack_name__]
+        return self.__unpublish_data__(msg_id)
+
+    def __unpublish_data__(self, msg_id: int):
+        """
+        This method is used to delete message storage of the data from telegram database.
+
+        Parameters:
+            msg_id (:obj:`int`): message id of the stored datapack to be deleted.
+
+        Returns:
+            :obj:`bool`
+        """
+        client = self.__telegram_client__
+        if client:
+            if isinstance(client, Client):
+                return self.__loop__.run_until_complete(client.delete_messages(chat_id=self.__chat_id__, message_ids=msg_id))
+            elif isinstance(client, TelegramClient):
+                try:
+                    self.__loop__.run_until_complete(client.delete_messages(entity=self.__chat_id__, message_ids=msg_id))
+                    return True
+                except:
+                    return False
+            else:
+                raise InvalidClient()
+        return False            
+
+    def __format_datapack__(self, datapack: DataPack):
+        """
+        This method is used to format the :class:`DataPack` in a string which will be published on telegram database chat.
+
+        Parameters:
+            datapack (:class:`DataPack`): Subclass of the `DataPack` of the data to be published on telegram database.
+
+        Returns:
+            :obj:`str`
+        """
+        query = f"#{datapack.__datapack_name__}"
+        query += f"\n{datapack.__get_dict__()}"
+        return query
+
+    def __get_datapacks__(self):
+        """
+        This method is used to load the existing data from the telegram database chat.
+
+        Returns:
+            :obj:`None`
+        """
+        if isinstance(self.__telegram_client__, Client):
+            from pyrogram.types import Message
+            for message in self.__telegram_client__.get_chat_history(self.__chat_id__):
+                message: Message = message
+                if not message.text:
+                    continue
+                try:
+                    text = message.text.markdown.split("\n", 1)
+                    self.__datapacks__[text[0][1:]] = {"id":message.message_id, "data":literal_eval(text[1])}
+                except:
+                    raise InvalidDataPack(message.message_id)
+                
+        elif isinstance(self.__telegram_client__, TelegramClient):
+            from telethon.tl.types import Message
+            for message in self.__telegram_client__.iter_messages(self.__chat_id__):
+                message: Message = message
+                if not message.message:
+                    continue
+                try:
+                    text = message.message.split("\n", 1)
+                    self.__datapacks__[text[0][1:]] = {"id":message.id, "data":literal_eval(text[1])}
+                except:
+                    raise InvalidDataPack(message.id)
+            # raise UnsupportedClient("telethon")
+        else:
+            raise InvalidClient()
+    
+    def __make_chat__(self):
+        """
+        This method is used to make the telegram database chat if not provided.
+
+        Returns:
+            :obj:`None`
+        """
+        if isinstance(self.__telegram_client__, Client):
+            chat = self.__telegram_client__.create_channel("Telegram DB")
+            self.__chat_id__ = chat.id
+        elif isinstance(self.__telegram_client__, TelegramClient):
+            from telethon import functions
+            with self.__telegram_client__ as client:
+                async def make_chat():    
+                    result = await client(functions.channels.CreateChannelRequest(
+                        title='Telegram DB',
+                        about="Channel to store DataPacks",
+                        broadcast=True,
+                    ))
+                    self.__chat_id__ = result.__dict__["chats"][0].__dict__["id"]
+                self.__loop__.run_until_complete(make_chat())
+        else:
+            raise InvalidClient()
+    
+    def __fill_datapack(self, datapack: DataPack):
+        """
+        This method is used to append the primary key in default name of the datapack, separated by `DP_NAME_SEPARATOR`. 
+
+        Parameters:
+            datapack (:class:`DataPack`): Subclass of the `DataPack` of the data to be published on telegram database.
+
+        Returns:
+            :class:`DataPack`
+        """
+        for dp in self.__dp_cache__:
+            if isinstance(datapack, dp):
+                datapack.__datapack_name__ += f"{DP_NAME_SEPARATOR}" + str(getattr(datapack, self.__dp_cache__[dp]))
+                break
         return datapack
```

### Comparing `TelegramDB-0.2.0/telegramdb/exceptions.py` & `TelegramDB-1.0.0/telegramdb/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# TelegramDB
-# Copyright (C) 2022
-# Anony <github.com/anonyindian>
-
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-from . import DP_NAME_SEPARATOR
-
-class GeneralException(Exception):
-    def __init__(self, message: str):
-        super().__init__(message)
-
-class ReservedCharacter(GeneralException):
-    def __init__(self, name:str = None):
-        super().__init__(f"Reserved Characters: '{DP_NAME_SEPARATOR}' can not be used in the datapack name: '{name}'")
-
-class InvalidDataPack(GeneralException):
-    def __init__(self, message_id: int=None):
-        msg = "Invalid DataPack"
-        if message_id:
-            msg += f": Found an invalid DataPack at message id '{message_id}' of the database chat"
-        super().__init__(msg)
-
-class UnsupportedClient(GeneralException):
-    def __init__(self, message=None):
-        msg = "Unsupported Client"
-        if message:
-            msg += f": {msg}"
-        super().__init__(msg)
-
-class InvalidClient(GeneralException):
-    def __init__(self):
+# TelegramDB
+# Copyright (C) 2023
+# Anony <github.com/anonyindian>
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+from . import DP_NAME_SEPARATOR
+
+class GeneralException(Exception):
+    def __init__(self, message: str):
+        super().__init__(message)
+
+class ReservedCharacter(GeneralException):
+    def __init__(self, name:str = None):
+        super().__init__(f"Reserved Characters: '{DP_NAME_SEPARATOR}' can not be used in the datapack name: '{name}'")
+
+class InvalidDataPack(GeneralException):
+    def __init__(self, message_id: int=None):
+        msg = "Invalid DataPack"
+        if message_id:
+            msg += f": Found an invalid DataPack at message id '{message_id}' of the database chat"
+        super().__init__(msg)
+
+class UnsupportedClient(GeneralException):
+    def __init__(self, message=None):
+        msg = "Unsupported Client"
+        if message:
+            msg += f": {msg}"
+        super().__init__(msg)
+
+class InvalidClient(GeneralException):
+    def __init__(self):
         super().__init__("Invalid Client: provided client not valid")
```

