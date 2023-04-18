# Comparing `tmp/Flask Boilerplate Creator-0.0.3.tar.gz` & `tmp/Flask Boilerplate Creator-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask Boilerplate Creator-0.0.3.tar", last modified: Fri Apr  7 04:52:19 2023, max compression
+gzip compressed data, was "Flask Boilerplate Creator-0.0.4.tar", last modified: Tue Apr 18 08:18:55 2023, max compression
```

## Comparing `Flask Boilerplate Creator-0.0.3.tar` & `Flask Boilerplate Creator-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 04:52:19.166823 Flask Boilerplate Creator-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-04-07 04:52:19.141228 Flask Boilerplate Creator-0.0.3/Flask_Boilerplate_Creator.egg-info/
--rw-rw-rw-   0        0        0     1868 2023-04-07 04:52:18.000000 Flask Boilerplate Creator-0.0.3/Flask_Boilerplate_Creator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-04-07 04:52:18.000000 Flask Boilerplate Creator-0.0.3/Flask_Boilerplate_Creator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 04:52:18.000000 Flask Boilerplate Creator-0.0.3/Flask_Boilerplate_Creator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-04-07 04:52:18.000000 Flask Boilerplate Creator-0.0.3/Flask_Boilerplate_Creator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1093 2023-04-07 04:02:55.000000 Flask Boilerplate Creator-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1868 2023-04-07 04:52:19.158708 Flask Boilerplate Creator-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1181 2023-04-07 04:25:06.000000 Flask Boilerplate Creator-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 04:52:19.155826 Flask Boilerplate Creator-0.0.3/flask-boilerplate-creator/
--rw-rw-rw-   0        0        0     8764 2023-04-07 04:50:30.000000 Flask Boilerplate Creator-0.0.3/flask-boilerplate-creator/__init__.py
--rw-rw-rw-   0        0        0       59 2023-04-07 02:54:15.000000 Flask Boilerplate Creator-0.0.3/flask-boilerplate-creator/__main__.py
--rw-rw-rw-   0        0        0       42 2023-04-07 04:52:19.167819 Flask Boilerplate Creator-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      895 2023-04-07 04:50:23.000000 Flask Boilerplate Creator-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:18:55.702993 Flask Boilerplate Creator-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-04-18 08:18:55.684758 Flask Boilerplate Creator-0.0.4/Flask_Boilerplate_Creator.egg-info/
+-rw-rw-rw-   0        0        0     1868 2023-04-18 08:18:55.000000 Flask Boilerplate Creator-0.0.4/Flask_Boilerplate_Creator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-04-18 08:18:55.000000 Flask Boilerplate Creator-0.0.4/Flask_Boilerplate_Creator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 08:18:55.000000 Flask Boilerplate Creator-0.0.4/Flask_Boilerplate_Creator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-04-18 08:18:55.000000 Flask Boilerplate Creator-0.0.4/Flask_Boilerplate_Creator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1093 2023-04-07 04:02:55.000000 Flask Boilerplate Creator-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1868 2023-04-18 08:18:55.700206 Flask Boilerplate Creator-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1181 2023-04-07 04:25:06.000000 Flask Boilerplate Creator-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 08:18:55.698177 Flask Boilerplate Creator-0.0.4/flask-boilerplate-creator/
+-rw-rw-rw-   0        0        0     8767 2023-04-18 08:17:04.000000 Flask Boilerplate Creator-0.0.4/flask-boilerplate-creator/__init__.py
+-rw-rw-rw-   0        0        0       59 2023-04-07 02:54:15.000000 Flask Boilerplate Creator-0.0.4/flask-boilerplate-creator/__main__.py
+-rw-rw-rw-   0        0        0       42 2023-04-18 08:18:55.702993 Flask Boilerplate Creator-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      895 2023-04-18 08:17:16.000000 Flask Boilerplate Creator-0.0.4/setup.py
```

### Comparing `Flask Boilerplate Creator-0.0.3/Flask_Boilerplate_Creator.egg-info/PKG-INFO` & `Flask Boilerplate Creator-0.0.4/Flask_Boilerplate_Creator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Boilerplate-Creator
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create boilerplate structure of flask web application
 Home-page: https://github.com/hakiKhuva/flask-boilerplate-creator
 Author: Harkishan Khuva
 Author-email: hakitechy@gmail.com
 License: MIT
 Keywords: fbc,flask-boilerplate-creator,flask boilerplate creator
 Platform: UNKNOWN
```

### Comparing `Flask Boilerplate Creator-0.0.3/LICENSE` & `Flask Boilerplate Creator-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask Boilerplate Creator-0.0.3/PKG-INFO` & `Flask Boilerplate Creator-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask Boilerplate Creator
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create boilerplate structure of flask web application
 Home-page: https://github.com/hakiKhuva/flask-boilerplate-creator
 Author: Harkishan Khuva
 Author-email: hakitechy@gmail.com
 License: MIT
 Keywords: fbc,flask-boilerplate-creator,flask boilerplate creator
 Platform: UNKNOWN
```

### Comparing `Flask Boilerplate Creator-0.0.3/README.md` & `Flask Boilerplate Creator-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Flask Boilerplate Creator-0.0.3/flask-boilerplate-creator/__init__.py` & `Flask Boilerplate Creator-0.0.4/flask-boilerplate-creator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Generate boilerplate structure for flask web app
 
 author: Harkishan Khuva <harkishankhuva.pythonanywhere.com>
-created date: 07/04/2023 IST
-version: 0.0.3
+created date: 18/04/2023 IST
+version: 0.0.4
 """
 
 # :: IMPORTS
 import os
 import sys
 import shutil
 import typing
@@ -70,15 +70,15 @@
 
 # DATA TO BE INSERTED INTO FILES
 FILES_INPUT = {
     os.path.join("app","__init__.py"): (
         "from flask import Flask\n"
         "# from flask_migrate import Migrate # uncomment if need\n"
         "# from flask_session import Session # uncomment if need\n\n"
-        "# from .models import db # uncomment if need\n"
+        "# from .models.db import db # uncomment if need\n"
         "from .settings import APP_SETTINGS\n\n"
         "# migrate = Migrate() # uncomment if need \n"
         "# session = Session() # uncomment if need \n\n"
         "def create_app():\n"
         "    app = Flask(__name__)\n"
         "    app.config.update(APP_SETTINGS)\n\n"
         "    # db.init_app(app) # uncomment is need \n"
```

### Comparing `Flask Boilerplate Creator-0.0.3/setup.py` & `Flask Boilerplate Creator-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="Flask Boilerplate Creator",
-    version="0.0.3",
+    version="0.0.4",
     description="Create boilerplate structure of flask web application",
     author="Harkishan Khuva",
     author_email="hakitechy@gmail.com",
     license="MIT",
     keywords=["fbc", "flask-boilerplate-creator", "flask boilerplate creator"],
     packages=["fbc"],
     package_dir={
```

