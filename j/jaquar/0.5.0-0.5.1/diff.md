# Comparing `tmp/jaquar-0.5.0.tar.gz` & `tmp/jaquar-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jaquar-0.5.0.tar", last modified: Tue Apr 18 08:26:58 2023, max compression
+gzip compressed data, was "dist\jaquar-0.5.1.tar", last modified: Tue Apr 18 08:39:58 2023, max compression
```

## Comparing `jaquar-0.5.0.tar` & `jaquar-0.5.1.tar`

### file list

```diff
@@ -1,34 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 08:26:58.000000 jaquar-0.5.0/
-drwxrwxrwx   0        0        0        0 2023-04-18 08:26:58.000000 jaquar-0.5.0/jaquar/
--rw-rw-rw-   0        0        0     3634 2023-04-18 08:21:35.000000 jaquar-0.5.0/jaquar/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:26:58.000000 jaquar-0.5.0/jaquar/config/
--rw-rw-rw-   0        0        0      359 2023-04-17 22:48:29.000000 jaquar-0.5.0/jaquar/config/settings.py
--rw-rw-rw-   0        0        0      275 2023-04-17 23:55:51.000000 jaquar-0.5.0/jaquar/config/urls.py
--rw-rw-rw-   0        0        0        0 2023-04-17 21:11:17.000000 jaquar-0.5.0/jaquar/config/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:26:58.000000 jaquar-0.5.0/jaquar/db/
-drwxrwxrwx   0        0        0        0 2023-04-18 08:26:58.000000 jaquar-0.5.0/jaquar/db/migrations/
--rw-rw-rw-   0        0        0        2 2023-04-17 23:14:35.000000 jaquar-0.5.0/jaquar/db/migrations/migration.py
--rw-rw-rw-   0        0        0        0 2023-04-17 21:35:25.000000 jaquar-0.5.0/jaquar/db/migrations/__init__.py
--rw-rw-rw-   0        0        0      498 2023-04-17 21:43:43.000000 jaquar-0.5.0/jaquar/db/schema.py
--rw-rw-rw-   0        0        0        0 2023-04-17 21:35:07.000000 jaquar-0.5.0/jaquar/db/__init__.py
--rw-rw-rw-   0        0        0     2556 2023-04-18 08:01:12.000000 jaquar-0.5.0/jaquar/jq.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:26:58.000000 jaquar-0.5.0/jaquar/models/
--rw-rw-rw-   0        0        0      994 2023-04-18 06:13:22.000000 jaquar-0.5.0/jaquar/models/models.py
--rw-rw-rw-   0        0        0        0 2023-04-18 06:06:34.000000 jaquar-0.5.0/jaquar/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:26:58.000000 jaquar-0.5.0/jaquar/views/
--rw-rw-rw-   0        0        0       37 2023-04-17 22:14:58.000000 jaquar-0.5.0/jaquar/views/about.py
--rw-rw-rw-   0        0        0       53 2023-04-17 22:14:25.000000 jaquar-0.5.0/jaquar/views/contact.py
--rw-rw-rw-   0        0        0     1290 2023-04-17 23:55:42.000000 jaquar-0.5.0/jaquar/views/home.py
--rw-rw-rw-   0        0        0        0 2023-04-17 21:11:21.000000 jaquar-0.5.0/jaquar/views/__init__.py
--rw-rw-rw-   0        0        0       43 2023-04-18 08:14:51.000000 jaquar-0.5.0/jaquar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:26:58.000000 jaquar-0.5.0/jaquar.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-18 08:26:57.000000 jaquar-0.5.0/jaquar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-18 08:26:57.000000 jaquar-0.5.0/jaquar.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      234 2023-04-18 08:26:57.000000 jaquar-0.5.0/jaquar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-04-18 08:26:57.000000 jaquar-0.5.0/jaquar.egg-info/requires.txt
--rw-rw-rw-   0        0        0      573 2023-04-18 08:26:57.000000 jaquar-0.5.0/jaquar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 08:26:57.000000 jaquar-0.5.0/jaquar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       99 2023-04-18 06:04:11.000000 jaquar-0.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0      234 2023-04-18 08:26:58.000000 jaquar-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-04-18 08:26:58.000000 jaquar-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      473 2023-04-18 08:26:20.000000 jaquar-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:39:58.000000 jaquar-0.5.1/
+drwxrwxrwx   0        0        0        0 2023-04-18 08:39:58.000000 jaquar-0.5.1/jaquar/
+-rw-rw-rw-   0        0        0     3744 2023-04-18 08:39:17.000000 jaquar-0.5.1/jaquar/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:39:58.000000 jaquar-0.5.1/jaquar/templates/
+drwxrwxrwx   0        0        0        0 2023-04-18 08:39:58.000000 jaquar-0.5.1/jaquar/templates/static/
+drwxrwxrwx   0        0        0        0 2023-04-18 08:39:58.000000 jaquar-0.5.1/jaquar/templates/static/css/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:36:39.000000 jaquar-0.5.1/jaquar/templates/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-04-18 08:39:58.000000 jaquar-0.5.1/jaquar/templates/static/js/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:36:27.000000 jaquar-0.5.1/jaquar/templates/static/js/scripts.js
+-rw-rw-rw-   0        0        0       43 2023-04-18 08:14:51.000000 jaquar-0.5.1/jaquar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:39:58.000000 jaquar-0.5.1/jaquar.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-18 08:39:57.000000 jaquar-0.5.1/jaquar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-18 08:39:57.000000 jaquar-0.5.1/jaquar.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      234 2023-04-18 08:39:57.000000 jaquar-0.5.1/jaquar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-04-18 08:39:57.000000 jaquar-0.5.1/jaquar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      311 2023-04-18 08:39:57.000000 jaquar-0.5.1/jaquar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 08:39:57.000000 jaquar-0.5.1/jaquar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       99 2023-04-18 06:04:11.000000 jaquar-0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      234 2023-04-18 08:39:58.000000 jaquar-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-04-18 08:39:58.000000 jaquar-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      473 2023-04-18 08:39:56.000000 jaquar-0.5.1/setup.py
```

### Comparing `jaquar-0.5.0/jaquar/cli.py` & `jaquar-0.5.1/jaquar/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,31 +32,32 @@
     os.makedirs(os.path.join(project_name, 'static', 'img'))
     os.makedirs(os.path.join(project_name, 'templates'))
     os.makedirs(os.path.join(project_name, 'views'))
     os.makedirs(os.path.join(project_name, 'tests'))
 
     
     # Copy files from template directory to project directory
-    shutil.copy('templates/cli.py', os.path.join(project_name, 'cli.py'))
+    shutil.copy('templates/jq.py', os.path.join(project_name, 'jq.py'))
     shutil.copy('templates/__init__.py', os.path.join(project_name, '__init__.py'))
     shutil.copy('templates/config/__init__.py', os.path.join(project_name, 'config', '__init__.py'))
     shutil.copy('templates/config/urls.py', os.path.join(project_name, 'config', 'urls.py'))
+    shutil.copy('templates/config/settings.py', os.path.join(project_name, 'config', 'settings.py'))
     shutil.copy('templates/models/__init__.py', os.path.join(project_name, 'models', '__init__.py'))
     shutil.copy('templates/models/model.py', os.path.join(project_name, 'models', 'model.py'))
     shutil.copy('templates/db/__init__.py', os.path.join(project_name, 'db', '__init__.py'))
     shutil.copy('templates/db/migrations/__init__.py', os.path.join(project_name, 'db', 'migrations', '__init__.py'))
     shutil.copy('templates/db/migrations/alembic.ini', os.path.join(project_name, 'db', 'migrations', 'alembic.ini'))
     shutil.copy('templates/views/__init__.py', os.path.join(project_name, 'views', '__init__.py'))
     shutil.copy('templates/views/index.py', os.path.join(project_name, 'views', 'index.py'))
-    shutil.copy('templates/templates/index.html', os.path.join(project_name, 'templates', 'index.html'))
-    shutil.copy('templates/tests/__init__.py', os.path.join(project_name, 'tests', '__init__.py'))
+    shutil.copy('templates/templates/index.html.jq', os.path.join(project_name, 'templates', 'index.html.jq'))
+    # shutil.copy('templates/tests/__init__.py', os.path.join(project_name, 'tests', '__init__.py'))
     shutil.copy('templates/tests/test_index.py', os.path.join(project_name, 'tests', 'test_index.py'))
     shutil.copy('templates/static/css/style.css', os.path.join(project_name, 'static', 'css', 'style.css'))
     shutil.copy('templates/static/js/script.js', os.path.join(project_name, 'static', 'js', 'script.js'))
-    shutil.copy('templates/static/img/logo.png', os.path.join(project_name, 'static', 'img', 'logo.png'))
+    # shutil.copy('templates/static/img/logo.png', os.path.join(project_name, 'static', 'img', 'logo.png'))
 
     
 
     
     # Render README and manage.py templates and write to file
     template = env.get_template('README.md')
     with open(os.path.join(project_name, 'README.md'), 'w') as f:
```

