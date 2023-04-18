# Comparing `tmp/mongoclass-1.1.tar.gz` & `tmp/mongoclass-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongoclass-1.1.tar", last modified: Tue Jan 10 08:51:14 2023, max compression
+gzip compressed data, was "mongoclass-1.2.tar", last modified: Tue Apr 18 14:45:01 2023, max compression
```

## Comparing `mongoclass-1.1.tar` & `mongoclass-1.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-01-10 08:51:14.613750 mongoclass-1.1/
--rw-rw-rw-   0        0        0     1093 2022-10-28 01:48:28.000000 mongoclass-1.1/LICENSE
--rw-rw-rw-   0        0        0     3408 2023-01-10 08:51:14.614748 mongoclass-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2973 2022-10-28 01:48:28.000000 mongoclass-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-01-10 08:51:14.600749 mongoclass-1.1/mongoclass/
--rw-rw-rw-   0        0        0       58 2022-10-28 01:48:28.000000 mongoclass-1.1/mongoclass/__init__.py
--rw-rw-rw-   0        0        0    23922 2023-01-10 08:48:28.000000 mongoclass-1.1/mongoclass/client.py
--rw-rw-rw-   0        0        0     2015 2022-10-28 01:48:58.000000 mongoclass-1.1/mongoclass/cursor.py
-drwxrwxrwx   0        0        0        0 2023-01-10 08:51:14.612748 mongoclass-1.1/mongoclass.egg-info/
--rw-rw-rw-   0        0        0     3408 2023-01-10 08:51:14.000000 mongoclass-1.1/mongoclass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-01-10 08:51:14.000000 mongoclass-1.1/mongoclass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-10 08:51:14.000000 mongoclass-1.1/mongoclass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-01-10 08:51:14.000000 mongoclass-1.1/mongoclass.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-01-10 08:51:14.000000 mongoclass-1.1/mongoclass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-01-10 08:51:14.616753 mongoclass-1.1/setup.cfg
--rw-rw-rw-   0        0        0      769 2023-01-10 08:50:10.000000 mongoclass-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 14:45:01.541619 mongoclass-1.2/
+-rw-rw-rw-   0        0        0     1093 2022-10-28 01:48:28.000000 mongoclass-1.2/LICENSE
+-rw-rw-rw-   0        0        0     3408 2023-04-18 14:45:01.542616 mongoclass-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2973 2022-10-28 01:48:28.000000 mongoclass-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 14:45:01.501618 mongoclass-1.2/mongoclass/
+-rw-rw-rw-   0        0        0       58 2022-10-28 01:48:28.000000 mongoclass-1.2/mongoclass/__init__.py
+-rw-rw-rw-   0        0        0     5420 2023-04-18 14:44:13.000000 mongoclass-1.2/mongoclass/cache.py
+-rw-rw-rw-   0        0        0    24024 2023-04-18 14:44:13.000000 mongoclass-1.2/mongoclass/client.py
+-rw-rw-rw-   0        0        0     2015 2022-10-28 01:48:58.000000 mongoclass-1.2/mongoclass/cursor.py
+drwxrwxrwx   0        0        0        0 2023-04-18 14:45:01.539616 mongoclass-1.2/mongoclass.egg-info/
+-rw-rw-rw-   0        0        0     3408 2023-04-18 14:45:01.000000 mongoclass-1.2/mongoclass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-04-18 14:45:01.000000 mongoclass-1.2/mongoclass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 14:45:01.000000 mongoclass-1.2/mongoclass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-18 14:45:01.000000 mongoclass-1.2/mongoclass.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-18 14:45:01.000000 mongoclass-1.2/mongoclass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-18 14:45:01.550619 mongoclass-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      769 2023-04-18 14:44:29.000000 mongoclass-1.2/setup.py
```

### Comparing `mongoclass-1.1/LICENSE` & `mongoclass-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mongoclass-1.1/PKG-INFO` & `mongoclass-1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mongoclass
-Version: 1.1
+Version: 1.2
 Summary: A basic ORM like interface for mongodb in python that uses dataclasses.
 Home-page: https://github.com/bossauh/mongoclass
-Download-URL: https://github.com/bossauh/mongoclass/archive/refs/tags/v_11.tar.gz
+Download-URL: https://github.com/bossauh/mongoclass/archive/refs/tags/v_12.tar.gz
 Author: Philippe Mathew
 Author-email: philmattdev@gmail.com
 License: MIT
 Keywords: pymongo,orm
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mongoclass-1.1/README.md` & `mongoclass-1.2/README.md`

 * *Files identical despite different names*

### Comparing `mongoclass-1.1/mongoclass/client.py` & `mongoclass-1.2/mongoclass/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,14 +155,17 @@
             def wrapper(cls):
 
                 collection_name = collection or cls.__name__.lower()
 
                 @functools.wraps(cls, updated=())
                 class Inner(cls):
 
+                    COLLECTION_NAME = collection_name
+                    DATABASE_NAME = db.name
+
                     # pylint:disable=no-self-argument
                     def __init__(this, *args, **kwargs) -> None:
 
                         # MongodDB Attributes
                         this._mongodb_collection = collection_name
                         this._mongodb_db = db
                         this._mongodb_id = kwargs.pop("_mongodb_id", None)
```

### Comparing `mongoclass-1.1/mongoclass/cursor.py` & `mongoclass-1.2/mongoclass/cursor.py`

 * *Files identical despite different names*

### Comparing `mongoclass-1.1/mongoclass.egg-info/PKG-INFO` & `mongoclass-1.2/mongoclass.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mongoclass
-Version: 1.1
+Version: 1.2
 Summary: A basic ORM like interface for mongodb in python that uses dataclasses.
 Home-page: https://github.com/bossauh/mongoclass
-Download-URL: https://github.com/bossauh/mongoclass/archive/refs/tags/v_11.tar.gz
+Download-URL: https://github.com/bossauh/mongoclass/archive/refs/tags/v_12.tar.gz
 Author: Philippe Mathew
 Author-email: philmattdev@gmail.com
 License: MIT
 Keywords: pymongo,orm
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mongoclass-1.1/setup.py` & `mongoclass-1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 install_requires = ["dnspython==2.2.1", "mongita==1.1.1"]
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="mongoclass",
     packages=["mongoclass"],
-    version="1.1",
+    version="1.2",
     license="MIT",
     description="A basic ORM like interface for mongodb in python that uses dataclasses.",
     author="Philippe Mathew",
     author_email="philmattdev@gmail.com",
     url="https://github.com/bossauh/mongoclass",
-    download_url="https://github.com/bossauh/mongoclass/archive/refs/tags/v_11.tar.gz",
+    download_url="https://github.com/bossauh/mongoclass/archive/refs/tags/v_12.tar.gz",
     keywords=["pymongo", "orm"],
     install_requires=install_requires,
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

