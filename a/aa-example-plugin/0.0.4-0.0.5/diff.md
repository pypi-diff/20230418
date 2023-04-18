# Comparing `tmp/aa_example_plugin-0.0.4.tar.gz` & `tmp/aa_example_plugin-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_example_plugin-0.0.4.tar", last modified: Sat Nov 26 12:30:38 2022, max compression
+gzip compressed data, was "aa_example_plugin-0.0.5.tar", last modified: Tue Apr 18 16:04:49 2023, max compression
```

## Comparing `aa_example_plugin-0.0.4.tar` & `aa_example_plugin-0.0.5.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 12:30:38.189022 aa_example_plugin-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2022-11-26 12:30:18.000000 aa_example_plugin-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2022-11-26 12:30:18.000000 aa_example_plugin-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2022-11-26 12:30:38.189022 aa_example_plugin-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2022-11-26 12:30:18.000000 aa_example_plugin-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 12:30:38.189022 aa_example_plugin-0.0.4/aa_example_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2022-11-26 12:30:38.000000 aa_example_plugin-0.0.4/aa_example_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      692 2022-11-26 12:30:38.000000 aa_example_plugin-0.0.4/aa_example_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-26 12:30:38.000000 aa_example_plugin-0.0.4/aa_example_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-26 12:30:37.000000 aa_example_plugin-0.0.4/aa_example_plugin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-11-26 12:30:38.000000 aa_example_plugin-0.0.4/aa_example_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-11-26 12:30:38.000000 aa_example_plugin-0.0.4/aa_example_plugin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 12:30:38.189022 aa_example_plugin-0.0.4/example/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2022-11-26 12:30:18.000000 aa_example_plugin-0.0.4/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-11-26 12:30:18.000000 aa_example_plugin-0.0.4/example/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2022-11-26 12:30:18.000000 aa_example_plugin-0.0.4/example/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2022-11-26 12:30:18.000000 aa_example_plugin-0.0.4/example/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2022-11-26 12:30:18.000000 aa_example_plugin-0.0.4/example/auth_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 12:30:38.189022 aa_example_plugin-0.0.4/example/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2022-11-26 12:30:18.000000 aa_example_plugin-0.0.4/example/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-26 12:30:18.000000 aa_example_plugin-0.0.4/example/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2022-11-26 12:30:18.000000 aa_example_plugin-0.0.4/example/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 12:30:38.185022 aa_example_plugin-0.0.4/example/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 12:30:38.189022 aa_example_plugin-0.0.4/example/static/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-26 12:30:18.000000 aa_example_plugin-0.0.4/example/static/example/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      244 2022-11-26 12:30:18.000000 aa_example_plugin-0.0.4/example/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 12:30:38.185022 aa_example_plugin-0.0.4/example/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 12:30:38.189022 aa_example_plugin-0.0.4/example/templates/example/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2022-11-26 12:30:18.000000 aa_example_plugin-0.0.4/example/templates/example/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      478 2022-11-26 12:30:18.000000 aa_example_plugin-0.0.4/example/templates/example/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 12:30:38.189022 aa_example_plugin-0.0.4/example/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2022-11-26 12:30:18.000000 aa_example_plugin-0.0.4/example/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2022-11-26 12:30:18.000000 aa_example_plugin-0.0.4/example/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2022-11-26 12:30:18.000000 aa_example_plugin-0.0.4/example/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2022-11-26 12:30:18.000000 aa_example_plugin-0.0.4/example/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-11-26 12:30:18.000000 aa_example_plugin-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2022-11-26 12:30:38.193022 aa_example_plugin-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:04:49.773968 aa_example_plugin-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-18 16:04:29.000000 aa_example_plugin-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-18 16:04:29.000000 aa_example_plugin-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-04-18 16:04:49.773968 aa_example_plugin-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-04-18 16:04:29.000000 aa_example_plugin-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:04:49.769967 aa_example_plugin-0.0.5/aa_example_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-04-18 16:04:49.000000 aa_example_plugin-0.0.5/aa_example_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-18 16:04:49.000000 aa_example_plugin-0.0.5/aa_example_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:04:49.000000 aa_example_plugin-0.0.5/aa_example_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:04:49.000000 aa_example_plugin-0.0.5/aa_example_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 16:04:49.000000 aa_example_plugin-0.0.5/aa_example_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 16:04:49.000000 aa_example_plugin-0.0.5/aa_example_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:04:49.773968 aa_example_plugin-0.0.5/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-18 16:04:29.000000 aa_example_plugin-0.0.5/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 16:04:29.000000 aa_example_plugin-0.0.5/example/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-18 16:04:29.000000 aa_example_plugin-0.0.5/example/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-18 16:04:29.000000 aa_example_plugin-0.0.5/example/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-18 16:04:29.000000 aa_example_plugin-0.0.5/example/auth_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:04:49.773968 aa_example_plugin-0.0.5/example/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:04:29.000000 aa_example_plugin-0.0.5/example/locale/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:04:49.773968 aa_example_plugin-0.0.5/example/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-18 16:04:29.000000 aa_example_plugin-0.0.5/example/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:04:29.000000 aa_example_plugin-0.0.5/example/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-18 16:04:29.000000 aa_example_plugin-0.0.5/example/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:04:49.765967 aa_example_plugin-0.0.5/example/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:04:49.773968 aa_example_plugin-0.0.5/example/static/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:04:29.000000 aa_example_plugin-0.0.5/example/static/example/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-18 16:04:29.000000 aa_example_plugin-0.0.5/example/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:04:49.765967 aa_example_plugin-0.0.5/example/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:04:49.773968 aa_example_plugin-0.0.5/example/templates/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-18 16:04:29.000000 aa_example_plugin-0.0.5/example/templates/example/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-18 16:04:29.000000 aa_example_plugin-0.0.5/example/templates/example/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:04:49.773968 aa_example_plugin-0.0.5/example/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 16:04:29.000000 aa_example_plugin-0.0.5/example/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-18 16:04:29.000000 aa_example_plugin-0.0.5/example/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-18 16:04:29.000000 aa_example_plugin-0.0.5/example/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-18 16:04:29.000000 aa_example_plugin-0.0.5/example/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-18 16:04:29.000000 aa_example_plugin-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-18 16:04:49.777968 aa_example_plugin-0.0.5/setup.cfg
```

### Comparing `aa_example_plugin-0.0.4/LICENSE` & `aa_example_plugin-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_example_plugin-0.0.4/PKG-INFO` & `aa_example_plugin-0.0.5/aa_example_plugin.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aa_example_plugin
-Version: 0.0.4
+Name: aa-example-plugin
+Version: 0.0.5
 Summary: Example Plugin for Alliance Auth (GitHub Version)
 Home-page: https://github.com/ppfeufer/aa-example-plugin
 Author: Peter Pfeufer
 Author-email: development@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: development@ppfeufer.de
 License: GPL-3.0
@@ -27,48 +27,66 @@
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Example Plugin App for Alliance Auth (GitHub Version)
 
 This is an example plugin app for [Alliance Auth](https://gitlab.com/allianceauth/allianceauth)
-(AA) that can be used as starting point to develop custom plugins.
+(AA) that can be used as a starting point to develop custom plugins.
 
 ![License](https://img.shields.io/badge/license-GPLv3-green)
 ![python](https://img.shields.io/badge/python-3.8-informational)
 ![django](https://img.shields.io/badge/django-3.2-informational)
 ![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
 
 _(These badges are examples, you can and should replace them with your own)_
 
 For the GitLab version of this example app, please have a look over here, Erik
 Kalkoken was so friendly to provide it » [Alliance Auth Example App (GitLab Version)](https://gitlab.com/ErikKalkoken/allianceauth-example-plugin)
 
 
+---
+
+<!-- TOC -->
+* [Example Plugin App for Alliance Auth (GitHub Version)](#example-plugin-app-for-alliance-auth-github-version)
+  * [Features](#features)
+  * [How to Use It](#how-to-use-it)
+    * [Cloning From Repo](#cloning-from-repo)
+    * [Renaming the App](#renaming-the-app)
+  * [Clearing Migrations](#clearing-migrations)
+  * [Writing Unit Tests](#writing-unit-tests)
+  * [Installing Into Your Dev AA](#installing-into-your-dev-aa)
+  * [Installing Into Production AA](#installing-into-production-aa)
+  * [Contribute](#contribute)
+<!-- TOC -->
+
+---
+
+
 ## Features
 
 - The plugin can be installed, upgraded (and removed) into an existing AA
   installation using PyInstaller.
 - It has its own menu item in the sidebar.
 - It has one view that shows a panel and some text
 
 
 ## How to Use It
 
-To use this example as basis for your own development just fork this repo and then
+To use this example as a basis for your own development, just fork this repo and then
 clone it on your dev machine.
 
 You then should rename the app, and then you can install it into your AA dev
 installation.
 
 
 ### Cloning From Repo
 
-For this app we are assuming that you have all your AA projects, your virtual
-environment and your AA installation under one top folder (e.g. aa-dev).
+For this app, we're assuming that you have all your AA projects, your virtual
+environment, and your AA installation under one top folder (e.g. aa-dev).
 
 This should look something like this:
 
 ```text
 aa-dev
 |- venv/
 |- myauth/
@@ -98,17 +116,17 @@
 
 Here is an overview of the places that you need to edit to adopt the name.
 
 Easiest is to just find & replace `example` with your new app name in all files
 listed below.
 
 One small warning about picking names: Python is a bit particular about what special
-characters are allowed for names of modules and packages. To avoid any pitfalls I
-would therefore recommend to use only normal characters (a-z) in your app's name
-unless you know exactly what you are doing.
+characters are allowed for names of modules and packages. To avoid any pitfalls, I
+would therefore recommend using only normal characters (a-z) in your app's name
+unless you know exactly what you're doing.
 
 | Location                                 | Description                                                                            |
 |------------------------------------------|----------------------------------------------------------------------------------------|
 | `./example/`                             | Folder name                                                                            |
 | `./example/static/example/`              | Folder name                                                                            |
 | `./example/templates/example/`           | Folder name                                                                            |
 | `./setup.cfg`                            | Update module name for version import, update package name, update title, author, etc. |
@@ -128,16 +146,16 @@
 | `./tox.ini`                              | App name                                                                               |
 | `./.isort.cfg`                           | App name for `import_heading_firstparty`                                               |
 | `./Makefile`                             | App name and package name                                                              |
 
 
 ## Clearing Migrations
 
-Instead of renaming your app in the migrations it's easier to just recreate them
-later in the process. For this to work you need to delete the old migration files in
+Instead of renaming your app in the migrations, it's easier to just recreate them
+later in the process. For this to work, you need to delete the old migration files in
 your `migrations` folder.
 
 ```bash
 rm your-app-name/migrations/0001_initial.py
 rm -rf your-app-name/migrations/_pycache
 ```
 
@@ -146,59 +164,59 @@
 
 Write your unit tests in `your-app-name/tests/` and make sure that you use a "test_"
 prefix for files with your unit tests.
 
 
 ## Installing Into Your Dev AA
 
-Once you have cloned or copied all files into place and finished renaming the app
-you are ready to install it to your dev AA instance.
+Once you've cloned or copied all files into place and finished renaming the app,
+you're ready to install it to your dev AA instance.
 
-Make sure you are in your venv. Then install it with pip in editable mode:
+Make sure you're in your venv. Then install it with pip in editable mode:
 
 ```bash
 pip install -e aa-your-app-name
 ```
 
 First add your app to the Django project by adding the name of your app to
 INSTALLED_APPS in `settings/local.py`.
 
-Next we will create new migrations for your app:
+Next, we will create new migrations for your app:
 
 ```bash
 python manage.py makemigrations
 ```
 
 Then run a check to see if everything is set up correctly.
 
 ```bash
 python manage.py check
 ```
 
-In case they are errors make sure to fix them before proceeding.
+In case they're errors make sure to fix them before proceeding.
 
-Next perform migrations to add your model to the database:
+Next, perform migrations to add your model to the database:
 
 ```bash
 python manage.py migrate
 ```
 
 Finally, restart your AA server and that's it.
 
 
 ## Installing Into Production AA
 
-To install your plugin into a production AA run this command within the virtual
+To install your plugin into a production AA, run this command within the virtual
 Python environment of your AA installation:
 
 ```bash
 pip install git+https://github.com/YourName/aa-your-app-name
 ```
 
-Alternatively you can create a package file and manually upload it to your
+Alternatively, you can create a package file and manually upload it to your
 production AA:
 
 ```bash
 pip install build
 python -m build
 ```
 
@@ -212,11 +230,11 @@
 
 Then add your app to `INSTALLED_APPS` in `settings/local.py`, run migrations and
 restart your allianceserver.
 
 
 ## Contribute
 
-If you made a new app for AA please consider sharing it with the rest of the
-community. For any questions on how to share your app please contact the AA devs on
+If you've made a new app for AA, please consider sharing it with the rest of the
+community. For any questions on how to share your app, please contact the AA devs on
 their Discord. You find the current community creations
 [here](https://gitlab.com/allianceauth/community-creations).
```

### Comparing `aa_example_plugin-0.0.4/README.md` & `aa_example_plugin-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,62 @@
 # Example Plugin App for Alliance Auth (GitHub Version)
 
 This is an example plugin app for [Alliance Auth](https://gitlab.com/allianceauth/allianceauth)
-(AA) that can be used as starting point to develop custom plugins.
+(AA) that can be used as a starting point to develop custom plugins.
 
 ![License](https://img.shields.io/badge/license-GPLv3-green)
 ![python](https://img.shields.io/badge/python-3.8-informational)
 ![django](https://img.shields.io/badge/django-3.2-informational)
 ![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
 
 _(These badges are examples, you can and should replace them with your own)_
 
 For the GitLab version of this example app, please have a look over here, Erik
 Kalkoken was so friendly to provide it » [Alliance Auth Example App (GitLab Version)](https://gitlab.com/ErikKalkoken/allianceauth-example-plugin)
 
 
+---
+
+<!-- TOC -->
+* [Example Plugin App for Alliance Auth (GitHub Version)](#example-plugin-app-for-alliance-auth-github-version)
+  * [Features](#features)
+  * [How to Use It](#how-to-use-it)
+    * [Cloning From Repo](#cloning-from-repo)
+    * [Renaming the App](#renaming-the-app)
+  * [Clearing Migrations](#clearing-migrations)
+  * [Writing Unit Tests](#writing-unit-tests)
+  * [Installing Into Your Dev AA](#installing-into-your-dev-aa)
+  * [Installing Into Production AA](#installing-into-production-aa)
+  * [Contribute](#contribute)
+<!-- TOC -->
+
+---
+
+
 ## Features
 
 - The plugin can be installed, upgraded (and removed) into an existing AA
   installation using PyInstaller.
 - It has its own menu item in the sidebar.
 - It has one view that shows a panel and some text
 
 
 ## How to Use It
 
-To use this example as basis for your own development just fork this repo and then
+To use this example as a basis for your own development, just fork this repo and then
 clone it on your dev machine.
 
 You then should rename the app, and then you can install it into your AA dev
 installation.
 
 
 ### Cloning From Repo
 
-For this app we are assuming that you have all your AA projects, your virtual
-environment and your AA installation under one top folder (e.g. aa-dev).
+For this app, we're assuming that you have all your AA projects, your virtual
+environment, and your AA installation under one top folder (e.g. aa-dev).
 
 This should look something like this:
 
 ```text
 aa-dev
 |- venv/
 |- myauth/
@@ -68,17 +86,17 @@
 
 Here is an overview of the places that you need to edit to adopt the name.
 
 Easiest is to just find & replace `example` with your new app name in all files
 listed below.
 
 One small warning about picking names: Python is a bit particular about what special
-characters are allowed for names of modules and packages. To avoid any pitfalls I
-would therefore recommend to use only normal characters (a-z) in your app's name
-unless you know exactly what you are doing.
+characters are allowed for names of modules and packages. To avoid any pitfalls, I
+would therefore recommend using only normal characters (a-z) in your app's name
+unless you know exactly what you're doing.
 
 | Location                                 | Description                                                                            |
 |------------------------------------------|----------------------------------------------------------------------------------------|
 | `./example/`                             | Folder name                                                                            |
 | `./example/static/example/`              | Folder name                                                                            |
 | `./example/templates/example/`           | Folder name                                                                            |
 | `./setup.cfg`                            | Update module name for version import, update package name, update title, author, etc. |
@@ -98,16 +116,16 @@
 | `./tox.ini`                              | App name                                                                               |
 | `./.isort.cfg`                           | App name for `import_heading_firstparty`                                               |
 | `./Makefile`                             | App name and package name                                                              |
 
 
 ## Clearing Migrations
 
-Instead of renaming your app in the migrations it's easier to just recreate them
-later in the process. For this to work you need to delete the old migration files in
+Instead of renaming your app in the migrations, it's easier to just recreate them
+later in the process. For this to work, you need to delete the old migration files in
 your `migrations` folder.
 
 ```bash
 rm your-app-name/migrations/0001_initial.py
 rm -rf your-app-name/migrations/_pycache
 ```
 
@@ -116,59 +134,59 @@
 
 Write your unit tests in `your-app-name/tests/` and make sure that you use a "test_"
 prefix for files with your unit tests.
 
 
 ## Installing Into Your Dev AA
 
-Once you have cloned or copied all files into place and finished renaming the app
-you are ready to install it to your dev AA instance.
+Once you've cloned or copied all files into place and finished renaming the app,
+you're ready to install it to your dev AA instance.
 
-Make sure you are in your venv. Then install it with pip in editable mode:
+Make sure you're in your venv. Then install it with pip in editable mode:
 
 ```bash
 pip install -e aa-your-app-name
 ```
 
 First add your app to the Django project by adding the name of your app to
 INSTALLED_APPS in `settings/local.py`.
 
-Next we will create new migrations for your app:
+Next, we will create new migrations for your app:
 
 ```bash
 python manage.py makemigrations
 ```
 
 Then run a check to see if everything is set up correctly.
 
 ```bash
 python manage.py check
 ```
 
-In case they are errors make sure to fix them before proceeding.
+In case they're errors make sure to fix them before proceeding.
 
-Next perform migrations to add your model to the database:
+Next, perform migrations to add your model to the database:
 
 ```bash
 python manage.py migrate
 ```
 
 Finally, restart your AA server and that's it.
 
 
 ## Installing Into Production AA
 
-To install your plugin into a production AA run this command within the virtual
+To install your plugin into a production AA, run this command within the virtual
 Python environment of your AA installation:
 
 ```bash
 pip install git+https://github.com/YourName/aa-your-app-name
 ```
 
-Alternatively you can create a package file and manually upload it to your
+Alternatively, you can create a package file and manually upload it to your
 production AA:
 
 ```bash
 pip install build
 python -m build
 ```
 
@@ -182,11 +200,11 @@
 
 Then add your app to `INSTALLED_APPS` in `settings/local.py`, run migrations and
 restart your allianceserver.
 
 
 ## Contribute
 
-If you made a new app for AA please consider sharing it with the rest of the
-community. For any questions on how to share your app please contact the AA devs on
+If you've made a new app for AA, please consider sharing it with the rest of the
+community. For any questions on how to share your app, please contact the AA devs on
 their Discord. You find the current community creations
 [here](https://gitlab.com/allianceauth/community-creations).
```

### Comparing `aa_example_plugin-0.0.4/aa_example_plugin.egg-info/PKG-INFO` & `aa_example_plugin-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aa-example-plugin
-Version: 0.0.4
+Name: aa_example_plugin
+Version: 0.0.5
 Summary: Example Plugin for Alliance Auth (GitHub Version)
 Home-page: https://github.com/ppfeufer/aa-example-plugin
 Author: Peter Pfeufer
 Author-email: development@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: development@ppfeufer.de
 License: GPL-3.0
@@ -27,48 +27,66 @@
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Example Plugin App for Alliance Auth (GitHub Version)
 
 This is an example plugin app for [Alliance Auth](https://gitlab.com/allianceauth/allianceauth)
-(AA) that can be used as starting point to develop custom plugins.
+(AA) that can be used as a starting point to develop custom plugins.
 
 ![License](https://img.shields.io/badge/license-GPLv3-green)
 ![python](https://img.shields.io/badge/python-3.8-informational)
 ![django](https://img.shields.io/badge/django-3.2-informational)
 ![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
 
 _(These badges are examples, you can and should replace them with your own)_
 
 For the GitLab version of this example app, please have a look over here, Erik
 Kalkoken was so friendly to provide it » [Alliance Auth Example App (GitLab Version)](https://gitlab.com/ErikKalkoken/allianceauth-example-plugin)
 
 
+---
+
+<!-- TOC -->
+* [Example Plugin App for Alliance Auth (GitHub Version)](#example-plugin-app-for-alliance-auth-github-version)
+  * [Features](#features)
+  * [How to Use It](#how-to-use-it)
+    * [Cloning From Repo](#cloning-from-repo)
+    * [Renaming the App](#renaming-the-app)
+  * [Clearing Migrations](#clearing-migrations)
+  * [Writing Unit Tests](#writing-unit-tests)
+  * [Installing Into Your Dev AA](#installing-into-your-dev-aa)
+  * [Installing Into Production AA](#installing-into-production-aa)
+  * [Contribute](#contribute)
+<!-- TOC -->
+
+---
+
+
 ## Features
 
 - The plugin can be installed, upgraded (and removed) into an existing AA
   installation using PyInstaller.
 - It has its own menu item in the sidebar.
 - It has one view that shows a panel and some text
 
 
 ## How to Use It
 
-To use this example as basis for your own development just fork this repo and then
+To use this example as a basis for your own development, just fork this repo and then
 clone it on your dev machine.
 
 You then should rename the app, and then you can install it into your AA dev
 installation.
 
 
 ### Cloning From Repo
 
-For this app we are assuming that you have all your AA projects, your virtual
-environment and your AA installation under one top folder (e.g. aa-dev).
+For this app, we're assuming that you have all your AA projects, your virtual
+environment, and your AA installation under one top folder (e.g. aa-dev).
 
 This should look something like this:
 
 ```text
 aa-dev
 |- venv/
 |- myauth/
@@ -98,17 +116,17 @@
 
 Here is an overview of the places that you need to edit to adopt the name.
 
 Easiest is to just find & replace `example` with your new app name in all files
 listed below.
 
 One small warning about picking names: Python is a bit particular about what special
-characters are allowed for names of modules and packages. To avoid any pitfalls I
-would therefore recommend to use only normal characters (a-z) in your app's name
-unless you know exactly what you are doing.
+characters are allowed for names of modules and packages. To avoid any pitfalls, I
+would therefore recommend using only normal characters (a-z) in your app's name
+unless you know exactly what you're doing.
 
 | Location                                 | Description                                                                            |
 |------------------------------------------|----------------------------------------------------------------------------------------|
 | `./example/`                             | Folder name                                                                            |
 | `./example/static/example/`              | Folder name                                                                            |
 | `./example/templates/example/`           | Folder name                                                                            |
 | `./setup.cfg`                            | Update module name for version import, update package name, update title, author, etc. |
@@ -128,16 +146,16 @@
 | `./tox.ini`                              | App name                                                                               |
 | `./.isort.cfg`                           | App name for `import_heading_firstparty`                                               |
 | `./Makefile`                             | App name and package name                                                              |
 
 
 ## Clearing Migrations
 
-Instead of renaming your app in the migrations it's easier to just recreate them
-later in the process. For this to work you need to delete the old migration files in
+Instead of renaming your app in the migrations, it's easier to just recreate them
+later in the process. For this to work, you need to delete the old migration files in
 your `migrations` folder.
 
 ```bash
 rm your-app-name/migrations/0001_initial.py
 rm -rf your-app-name/migrations/_pycache
 ```
 
@@ -146,59 +164,59 @@
 
 Write your unit tests in `your-app-name/tests/` and make sure that you use a "test_"
 prefix for files with your unit tests.
 
 
 ## Installing Into Your Dev AA
 
-Once you have cloned or copied all files into place and finished renaming the app
-you are ready to install it to your dev AA instance.
+Once you've cloned or copied all files into place and finished renaming the app,
+you're ready to install it to your dev AA instance.
 
-Make sure you are in your venv. Then install it with pip in editable mode:
+Make sure you're in your venv. Then install it with pip in editable mode:
 
 ```bash
 pip install -e aa-your-app-name
 ```
 
 First add your app to the Django project by adding the name of your app to
 INSTALLED_APPS in `settings/local.py`.
 
-Next we will create new migrations for your app:
+Next, we will create new migrations for your app:
 
 ```bash
 python manage.py makemigrations
 ```
 
 Then run a check to see if everything is set up correctly.
 
 ```bash
 python manage.py check
 ```
 
-In case they are errors make sure to fix them before proceeding.
+In case they're errors make sure to fix them before proceeding.
 
-Next perform migrations to add your model to the database:
+Next, perform migrations to add your model to the database:
 
 ```bash
 python manage.py migrate
 ```
 
 Finally, restart your AA server and that's it.
 
 
 ## Installing Into Production AA
 
-To install your plugin into a production AA run this command within the virtual
+To install your plugin into a production AA, run this command within the virtual
 Python environment of your AA installation:
 
 ```bash
 pip install git+https://github.com/YourName/aa-your-app-name
 ```
 
-Alternatively you can create a package file and manually upload it to your
+Alternatively, you can create a package file and manually upload it to your
 production AA:
 
 ```bash
 pip install build
 python -m build
 ```
 
@@ -212,11 +230,11 @@
 
 Then add your app to `INSTALLED_APPS` in `settings/local.py`, run migrations and
 restart your allianceserver.
 
 
 ## Contribute
 
-If you made a new app for AA please consider sharing it with the rest of the
-community. For any questions on how to share your app please contact the AA devs on
+If you've made a new app for AA, please consider sharing it with the rest of the
+community. For any questions on how to share your app, please contact the AA devs on
 their Discord. You find the current community creations
 [here](https://gitlab.com/allianceauth/community-creations).
```

### Comparing `aa_example_plugin-0.0.4/aa_example_plugin.egg-info/SOURCES.txt` & `aa_example_plugin-0.0.5/aa_example_plugin.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 example/app_settings.py
 example/apps.py
 example/auth_hooks.py
 example/models.py
 example/tasks.py
 example/urls.py
 example/views.py
+example/locale/.gitkeep
 example/migrations/0001_initial.py
 example/migrations/__init__.py
 example/static/example/.gitkeep
 example/templates/example/base.html
 example/templates/example/index.html
 example/tests/__init__.py
 example/tests/test_example.py
```

### Comparing `aa_example_plugin-0.0.4/example/auth_hooks.py` & `aa_example_plugin-0.0.5/example/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_example_plugin-0.0.4/example/migrations/0001_initial.py` & `aa_example_plugin-0.0.5/example/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_example_plugin-0.0.4/setup.cfg` & `aa_example_plugin-0.0.5/setup.cfg`

 * *Files identical despite different names*

