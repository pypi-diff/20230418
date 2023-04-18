# Comparing `tmp/Mongeasy-0.1.4.tar.gz` & `tmp/Mongeasy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mongeasy-0.1.4.tar", last modified: Mon Apr 17 11:55:24 2023, max compression
+gzip compressed data, was "Mongeasy-0.1.5.tar", last modified: Tue Apr 18 16:45:56 2023, max compression
```

## Comparing `Mongeasy-0.1.4.tar` & `Mongeasy-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 11:55:24.691588 Mongeasy-0.1.4/
--rw-rw-rw-   0        0        0     1096 2023-04-17 10:50:01.000000 Mongeasy-0.1.4/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-17 11:55:24.671556 Mongeasy-0.1.4/Mongeasy.egg-info/
--rw-rw-rw-   0        0        0     6982 2023-04-17 11:55:24.000000 Mongeasy-0.1.4/Mongeasy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-04-17 11:55:24.000000 Mongeasy-0.1.4/Mongeasy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 11:55:24.000000 Mongeasy-0.1.4/Mongeasy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-17 11:55:24.000000 Mongeasy-0.1.4/Mongeasy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-17 11:55:24.000000 Mongeasy-0.1.4/Mongeasy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-17 11:55:24.000000 Mongeasy-0.1.4/Mongeasy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6982 2023-04-17 11:55:24.691588 Mongeasy-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     6179 2023-04-17 10:49:55.000000 Mongeasy-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 11:55:24.688588 Mongeasy-0.1.4/mongeasy/
--rw-rw-rw-   0        0        0     2035 2023-04-17 11:55:11.000000 Mongeasy-0.1.4/mongeasy/__init__.py
--rw-rw-rw-   0        0        0     2775 2023-03-03 13:34:30.000000 Mongeasy-0.1.4/mongeasy/base_dict.py
--rw-rw-rw-   0        0        0    11368 2023-04-17 11:54:55.000000 Mongeasy-0.1.4/mongeasy/document.py
--rw-rw-rw-   0        0        0     2919 2023-04-17 08:03:57.000000 Mongeasy-0.1.4/mongeasy/dynamics.py
--rw-rw-rw-   0        0        0     1851 2023-03-09 08:28:25.000000 Mongeasy-0.1.4/mongeasy/exceptions.py
--rw-rw-rw-   0        0        0       20 2023-04-17 07:50:37.000000 Mongeasy-0.1.4/mongeasy/mongeasy.py
--rw-rw-rw-   0        0        0     4963 2023-04-17 10:49:05.000000 Mongeasy-0.1.4/mongeasy/resultlist.py
--rw-rw-rw-   0        0        0     1865 2023-04-17 08:02:18.000000 Mongeasy-0.1.4/mongeasy/utils.py
--rw-rw-rw-   0        0        0       91 2023-04-17 11:07:53.000000 Mongeasy-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0     1057 2023-04-17 11:55:24.693588 Mongeasy-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1076 2023-04-17 11:55:02.000000 Mongeasy-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 11:55:24.690589 Mongeasy-0.1.4/tests/
--rw-rw-rw-   0        0        0       39 2023-04-17 07:50:37.000000 Mongeasy-0.1.4/tests/__init__.py
--rw-rw-rw-   0        0        0     9850 2023-04-17 09:38:19.000000 Mongeasy-0.1.4/tests/test_mongeasy.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:45:56.783573 Mongeasy-0.1.5/
+-rw-rw-rw-   0        0        0     1096 2023-04-17 10:50:01.000000 Mongeasy-0.1.5/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-18 16:45:56.760436 Mongeasy-0.1.5/Mongeasy.egg-info/
+-rw-rw-rw-   0        0        0     8057 2023-04-18 16:45:56.000000 Mongeasy-0.1.5/Mongeasy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-04-18 16:45:56.000000 Mongeasy-0.1.5/Mongeasy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 16:45:56.000000 Mongeasy-0.1.5/Mongeasy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-18 16:45:56.000000 Mongeasy-0.1.5/Mongeasy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-04-18 16:45:56.000000 Mongeasy-0.1.5/Mongeasy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-18 16:45:56.000000 Mongeasy-0.1.5/Mongeasy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8057 2023-04-18 16:45:56.783573 Mongeasy-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7254 2023-04-18 16:45:19.000000 Mongeasy-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 16:45:56.774957 Mongeasy-0.1.5/mongeasy/
+-rw-rw-rw-   0        0        0     2035 2023-04-18 15:29:50.000000 Mongeasy-0.1.5/mongeasy/__init__.py
+-rw-rw-rw-   0        0        0     2775 2023-03-03 13:34:30.000000 Mongeasy-0.1.5/mongeasy/base_dict.py
+-rw-rw-rw-   0        0        0    11368 2023-04-17 11:54:55.000000 Mongeasy-0.1.5/mongeasy/document.py
+-rw-rw-rw-   0        0        0     2643 2023-04-18 15:29:29.000000 Mongeasy-0.1.5/mongeasy/dynamics.py
+-rw-rw-rw-   0        0        0     1851 2023-03-09 08:28:25.000000 Mongeasy-0.1.5/mongeasy/exceptions.py
+-rw-rw-rw-   0        0        0       20 2023-04-17 07:50:37.000000 Mongeasy-0.1.5/mongeasy/mongeasy.py
+-rw-rw-rw-   0        0        0     4963 2023-04-17 10:49:05.000000 Mongeasy-0.1.5/mongeasy/resultlist.py
+-rw-rw-rw-   0        0        0     1865 2023-04-17 08:02:18.000000 Mongeasy-0.1.5/mongeasy/utils.py
+-rw-rw-rw-   0        0        0       91 2023-04-17 11:07:53.000000 Mongeasy-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1057 2023-04-18 16:45:56.784573 Mongeasy-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1076 2023-04-18 16:45:23.000000 Mongeasy-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:45:56.782573 Mongeasy-0.1.5/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-17 07:50:37.000000 Mongeasy-0.1.5/tests/__init__.py
+-rw-rw-rw-   0        0        0     9850 2023-04-17 09:38:19.000000 Mongeasy-0.1.5/tests/test_mongeasy.py
```

### Comparing `Mongeasy-0.1.4/LICENSE` & `Mongeasy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.4/Mongeasy.egg-info/PKG-INFO` & `Mongeasy-0.1.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: Mongeasy
-Version: 0.1.4
-Summary: Easy to use wrapper around pymongo for easy access to MongoDB.
-Home-page: https://github.com/artheadsweden/mongeasy
-Author: Joakim Wassberg
-Author-email: joakim.wassberg@arthead.se
-License: MIT
-Project-URL: Bug Tracker, https://github.com/artheadsweden/mongeasy/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Mongeasy
 
 Mongeasy is a easy to use library to be used for simple access to a MongoDB database, without any need for schemas or validation. Just store the data as it is used in your application.
 
 ### Connection
 Connection to the database is handled automtically for you if you have the conenction information in a configfile or set as environment variables.
 
@@ -187,14 +167,48 @@
 
 User = create_document_class('User', 'users')
 
 # Create a unique index on the name field
 User.create_index('name', unique=True)
 ```
 
+### Other uses
+When you create the document class you have an option to pass additional bases classes. You can use this feature to add functionality to the generated class.
+
+This can also be useful if you want to use Mongeasy with for example flask-login.
+
+```python
+from flask import Flask
+from flask_login import UserMixin, LoginManager
+from mongeasy import create_document_class
+from bson import ObjectId
+
+login_manager = LoginManager()
+# Create User class with mongeasy and UserMixin from flask_login as a base class
+User = create_document_class('User', 'users', base_classes=(UserMixin,))
+def get_id(self):
+    return str(self._id)
+# Add get_id method to User class
+User.get_id = get_id
+
+
+def create_app():
+    app = Flask(__name__)
+   # Define the user loader function for Flask-Login
+    @login_manager.user_loader
+    def load_user(user_id):
+        # Load the user object from the database using the user_id
+        user_id = ObjectId(user_id)
+        user = User.find(_id=user_id).first()
+        return user
+
+    return app
+
+```
+
 ### ResultList
 All queries that can return more than one document will return a `ResultList` object. This object can be used to get the first or last document in the list, or None if no document is found.
 
 
 ```python
 from mongeasy import create_document_class
 
@@ -213,19 +227,19 @@
 * `first` - Get the first document in the list or None if no document is found
 * `last` - Get the last document in the list or None if no document is found
 * `first_or_none` - Get the first document in the list or None if no document is found, same as first
 * `last_or_none` - Get the last document in the list or None if no document is found, same as last
 * `map` - Apply a given function to each element in the list and return a new ResultList containing the results
 * `filter` - Filter the list using a given function and return a new ResultList containing the results
 * `reduce` - Apply a given function to each element in the list and return a single value
-* 'group_by` - Group the list by a given key and return a dict with the results grouped by the key
+* `group_by` - Group the list by a given key and return a dict with the results grouped by the key
 * `random` - Get a random document from the list or None if no document is found
 
 
 ### Contributing
 Contributions are welcome. Please create a pull request with your changes.
 
 ### Issues
 If you find any issues please create an issue on the github page.
 
 ### License
-This project is licensed under the MIT License - see the LICENSE file for details
+This project is licensed under the MIT License - see the LICENSE file for details
```

### Comparing `Mongeasy-0.1.4/PKG-INFO` & `Mongeasy-0.1.5/Mongeasy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mongeasy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Easy to use wrapper around pymongo for easy access to MongoDB.
 Home-page: https://github.com/artheadsweden/mongeasy
 Author: Joakim Wassberg
 Author-email: joakim.wassberg@arthead.se
 License: MIT
 Project-URL: Bug Tracker, https://github.com/artheadsweden/mongeasy/issues
 Classifier: Development Status :: 4 - Beta
@@ -187,14 +187,48 @@
 
 User = create_document_class('User', 'users')
 
 # Create a unique index on the name field
 User.create_index('name', unique=True)
 ```
 
+### Other uses
+When you create the document class you have an option to pass additional bases classes. You can use this feature to add functionality to the generated class.
+
+This can also be useful if you want to use Mongeasy with for example flask-login.
+
+```python
+from flask import Flask
+from flask_login import UserMixin, LoginManager
+from mongeasy import create_document_class
+from bson import ObjectId
+
+login_manager = LoginManager()
+# Create User class with mongeasy and UserMixin from flask_login as a base class
+User = create_document_class('User', 'users', base_classes=(UserMixin,))
+def get_id(self):
+    return str(self._id)
+# Add get_id method to User class
+User.get_id = get_id
+
+
+def create_app():
+    app = Flask(__name__)
+   # Define the user loader function for Flask-Login
+    @login_manager.user_loader
+    def load_user(user_id):
+        # Load the user object from the database using the user_id
+        user_id = ObjectId(user_id)
+        user = User.find(_id=user_id).first()
+        return user
+
+    return app
+
+```
+
 ### ResultList
 All queries that can return more than one document will return a `ResultList` object. This object can be used to get the first or last document in the list, or None if no document is found.
 
 
 ```python
 from mongeasy import create_document_class
 
@@ -213,15 +247,15 @@
 * `first` - Get the first document in the list or None if no document is found
 * `last` - Get the last document in the list or None if no document is found
 * `first_or_none` - Get the first document in the list or None if no document is found, same as first
 * `last_or_none` - Get the last document in the list or None if no document is found, same as last
 * `map` - Apply a given function to each element in the list and return a new ResultList containing the results
 * `filter` - Filter the list using a given function and return a new ResultList containing the results
 * `reduce` - Apply a given function to each element in the list and return a single value
-* 'group_by` - Group the list by a given key and return a dict with the results grouped by the key
+* `group_by` - Group the list by a given key and return a dict with the results grouped by the key
 * `random` - Get a random document from the list or None if no document is found
 
 
 ### Contributing
 Contributions are welcome. Please create a pull request with your changes.
 
 ### Issues
```

### Comparing `Mongeasy-0.1.4/mongeasy/__init__.py` & `Mongeasy-0.1.5/mongeasy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Mongeasy."""
 
 __author__ = """Joakim Wassberg"""
 __email__ = 'joakim.wassberg@arthead.se'
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 
 import os
 import configparser
 import pymongo
 from mongeasy.exceptions import MongEasyDBConnectionError
 from mongeasy.dynamics import create_document_class
```

### Comparing `Mongeasy-0.1.4/mongeasy/base_dict.py` & `Mongeasy-0.1.5/mongeasy/base_dict.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.4/mongeasy/document.py` & `Mongeasy-0.1.5/mongeasy/document.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.4/mongeasy/dynamics.py` & `Mongeasy-0.1.5/mongeasy/dynamics.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,24 +20,21 @@
 import inspect
 from typing import Union
 from .utils import pascal_to_snake
 from .document import Document
 from .exceptions import MongEasyValidationException, MongEasyFieldError
 
 
-def create_document_class(class_name: str, collection_name: str = None, schema: Union[dict, None] = None, base_classes: tuple = ()):
+def create_document_class(class_name: str, collection_name: str = None, base_classes: tuple = ()):
     """
     Dynamically create a document class and register it in the calling module's namespace.
     Args:
         class_name (str): Name of the class to create.
         collection_name (str, optional): Name of the collection. Defaults to None. 
             If None, the collection name will be the snake_case version of the class name with an 's' appended.
-        schema (Union[dict, BaseModel, None], optional): _description_. An optinal schema to be used. 
-            This can either be in Mongeasy format or Pydantic.  Defaults to None.
-            If None this docuemnt will be schemaless.
         base_classes (tuple, optional): Optional base classes to be added to the document class. Defaults to ().
 
     Returns:
         _type_: The newly created document class.
     """
     # Get the calling module
     frame = inspect.currentframe().f_back
```

### Comparing `Mongeasy-0.1.4/mongeasy/exceptions.py` & `Mongeasy-0.1.5/mongeasy/exceptions.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.4/mongeasy/resultlist.py` & `Mongeasy-0.1.5/mongeasy/resultlist.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.4/mongeasy/utils.py` & `Mongeasy-0.1.5/mongeasy/utils.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.4/setup.cfg` & `Mongeasy-0.1.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6f6e 6765 6173 790d 0a76 6572   = mongeasy..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e34 0d0a 6175  sion = 0.1.4..au
+00000020: 7369 6f6e 203d 2030 2e31 2e35 0d0a 6175  sion = 0.1.5..au
 00000030: 7468 6f72 203d 204a 6f61 6b69 6d20 5761  thor = Joakim Wa
 00000040: 7373 6265 7267 0d0a 6175 7468 6f72 5f65  ssberg..author_e
 00000050: 6d61 696c 203d 206a 6f61 6b69 6d2e 7761  mail = joakim.wa
 00000060: 7373 6265 7267 4061 7274 6865 6164 2e73  ssberg@arthead.s
 00000070: 650d 0a64 6573 6372 6970 7469 6f6e 203d  e..description =
 00000080: 2045 6173 7920 746f 2075 7365 2077 7261   Easy to use wra
 00000090: 7070 6572 2061 726f 756e 6420 7079 6d6f  pper around pymo
```

### Comparing `Mongeasy-0.1.4/setup.py` & `Mongeasy-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     readme = f.read()
 
 with open("LICENSE", encoding="utf8") as f:
     license = f.read()
 
 setup(
     name="Mongeasy",
-    version="0.1.4",
+    version="0.1.5",
     author="Joakim Wassberg",
     author_email="joakim.wassberg@arthead.se",
     description="Easy to use wrapper around pymongo for easy access to MongoDB.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/artheadsweden/mongeasy",
     license="MIT",
```

### Comparing `Mongeasy-0.1.4/tests/test_mongeasy.py` & `Mongeasy-0.1.5/tests/test_mongeasy.py`

 * *Files identical despite different names*

