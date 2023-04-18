# Comparing `tmp/jaquar-0.5.1.tar.gz` & `tmp/jaquar-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jaquar-0.5.1.tar", last modified: Tue Apr 18 08:39:58 2023, max compression
+gzip compressed data, was "dist\jaquar-0.5.2.tar", last modified: Tue Apr 18 08:46:27 2023, max compression
```

## Comparing `jaquar-0.5.1.tar` & `jaquar-0.5.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 08:39:58.000000 jaquar-0.5.1/
-drwxrwxrwx   0        0        0        0 2023-04-18 08:39:58.000000 jaquar-0.5.1/jaquar/
--rw-rw-rw-   0        0        0     3744 2023-04-18 08:39:17.000000 jaquar-0.5.1/jaquar/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:39:58.000000 jaquar-0.5.1/jaquar/templates/
-drwxrwxrwx   0        0        0        0 2023-04-18 08:39:58.000000 jaquar-0.5.1/jaquar/templates/static/
-drwxrwxrwx   0        0        0        0 2023-04-18 08:39:58.000000 jaquar-0.5.1/jaquar/templates/static/css/
--rw-rw-rw-   0        0        0        0 2023-04-18 08:36:39.000000 jaquar-0.5.1/jaquar/templates/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-04-18 08:39:58.000000 jaquar-0.5.1/jaquar/templates/static/js/
--rw-rw-rw-   0        0        0        0 2023-04-18 08:36:27.000000 jaquar-0.5.1/jaquar/templates/static/js/scripts.js
--rw-rw-rw-   0        0        0       43 2023-04-18 08:14:51.000000 jaquar-0.5.1/jaquar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:39:58.000000 jaquar-0.5.1/jaquar.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-18 08:39:57.000000 jaquar-0.5.1/jaquar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-18 08:39:57.000000 jaquar-0.5.1/jaquar.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      234 2023-04-18 08:39:57.000000 jaquar-0.5.1/jaquar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-04-18 08:39:57.000000 jaquar-0.5.1/jaquar.egg-info/requires.txt
--rw-rw-rw-   0        0        0      311 2023-04-18 08:39:57.000000 jaquar-0.5.1/jaquar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 08:39:57.000000 jaquar-0.5.1/jaquar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       99 2023-04-18 06:04:11.000000 jaquar-0.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0      234 2023-04-18 08:39:58.000000 jaquar-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-04-18 08:39:58.000000 jaquar-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      473 2023-04-18 08:39:56.000000 jaquar-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:46:27.000000 jaquar-0.5.2/
+drwxrwxrwx   0        0        0        0 2023-04-18 08:46:27.000000 jaquar-0.5.2/jaquar/
+-rw-rw-rw-   0        0        0     4280 2023-04-18 08:46:08.000000 jaquar-0.5.2/jaquar/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:46:27.000000 jaquar-0.5.2/jaquar/templates/
+drwxrwxrwx   0        0        0        0 2023-04-18 08:46:27.000000 jaquar-0.5.2/jaquar/templates/static/
+drwxrwxrwx   0        0        0        0 2023-04-18 08:46:27.000000 jaquar-0.5.2/jaquar/templates/static/css/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:36:39.000000 jaquar-0.5.2/jaquar/templates/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-04-18 08:46:27.000000 jaquar-0.5.2/jaquar/templates/static/js/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:36:27.000000 jaquar-0.5.2/jaquar/templates/static/js/scripts.js
+-rw-rw-rw-   0        0        0       43 2023-04-18 08:14:51.000000 jaquar-0.5.2/jaquar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:46:27.000000 jaquar-0.5.2/jaquar.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-18 08:46:26.000000 jaquar-0.5.2/jaquar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-18 08:46:26.000000 jaquar-0.5.2/jaquar.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      234 2023-04-18 08:46:26.000000 jaquar-0.5.2/jaquar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-04-18 08:46:26.000000 jaquar-0.5.2/jaquar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      311 2023-04-18 08:46:26.000000 jaquar-0.5.2/jaquar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 08:46:26.000000 jaquar-0.5.2/jaquar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       99 2023-04-18 06:04:11.000000 jaquar-0.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      234 2023-04-18 08:46:27.000000 jaquar-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-04-18 08:46:27.000000 jaquar-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      473 2023-04-18 08:46:23.000000 jaquar-0.5.2/setup.py
```

### Comparing `jaquar-0.5.1/jaquar/cli.py` & `jaquar-0.5.2/jaquar/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import shutil
+import jaquar
 import click
 from jinja2 import Environment, FileSystemLoader
 
 env = Environment(loader=FileSystemLoader('templates'), autoescape=True)
 
 # Define the available commands using the `click` library.
 @click.group()
@@ -32,34 +33,40 @@
     os.makedirs(os.path.join(project_name, 'static', 'img'))
     os.makedirs(os.path.join(project_name, 'templates'))
     os.makedirs(os.path.join(project_name, 'views'))
     os.makedirs(os.path.join(project_name, 'tests'))
 
     
     # Copy files from template directory to project directory
-    shutil.copy('templates/jq.py', os.path.join(project_name, 'jq.py'))
-    shutil.copy('templates/__init__.py', os.path.join(project_name, '__init__.py'))
-    shutil.copy('templates/config/__init__.py', os.path.join(project_name, 'config', '__init__.py'))
-    shutil.copy('templates/config/urls.py', os.path.join(project_name, 'config', 'urls.py'))
-    shutil.copy('templates/config/settings.py', os.path.join(project_name, 'config', 'settings.py'))
-    shutil.copy('templates/models/__init__.py', os.path.join(project_name, 'models', '__init__.py'))
-    shutil.copy('templates/models/model.py', os.path.join(project_name, 'models', 'model.py'))
-    shutil.copy('templates/db/__init__.py', os.path.join(project_name, 'db', '__init__.py'))
-    shutil.copy('templates/db/migrations/__init__.py', os.path.join(project_name, 'db', 'migrations', '__init__.py'))
-    shutil.copy('templates/db/migrations/alembic.ini', os.path.join(project_name, 'db', 'migrations', 'alembic.ini'))
-    shutil.copy('templates/views/__init__.py', os.path.join(project_name, 'views', '__init__.py'))
-    shutil.copy('templates/views/index.py', os.path.join(project_name, 'views', 'index.py'))
-    shutil.copy('templates/templates/index.html.jq', os.path.join(project_name, 'templates', 'index.html.jq'))
-    # shutil.copy('templates/tests/__init__.py', os.path.join(project_name, 'tests', '__init__.py'))
-    shutil.copy('templates/tests/test_index.py', os.path.join(project_name, 'tests', 'test_index.py'))
-    shutil.copy('templates/static/css/style.css', os.path.join(project_name, 'static', 'css', 'style.css'))
-    shutil.copy('templates/static/js/script.js', os.path.join(project_name, 'static', 'js', 'script.js'))
-    # shutil.copy('templates/static/img/logo.png', os.path.join(project_name, 'static', 'img', 'logo.png'))
+    # Get the path to the template directory inside the jaquar package
+    template_dir = os.path.join(os.path.dirname(jaquar.__file__), 'templates')
 
-    
+    # Get the name of the project from the user
+    project_name = input('Enter a name for your project: ')
+
+    # Create the project directory
+    os.makedirs(project_name)
+
+    # Copy files from template directory to project directory
+    shutil.copy(os.path.join(template_dir, 'jq.py'), os.path.join(project_name, 'jq.py'))
+    shutil.copy(os.path.join(template_dir, '__init__.py'), os.path.join(project_name, '__init__.py'))
+    shutil.copy(os.path.join(template_dir, 'config', '__init__.py'), os.path.join(project_name, 'config', '__init__.py'))
+    shutil.copy(os.path.join(template_dir, 'config', 'urls.py'), os.path.join(project_name, 'config', 'urls.py'))
+    shutil.copy(os.path.join(template_dir, 'config', 'settings.py'), os.path.join(project_name, 'config', 'settings.py'))
+    shutil.copy(os.path.join(template_dir, 'models', '__init__.py'), os.path.join(project_name, 'models', '__init__.py'))
+    shutil.copy(os.path.join(template_dir, 'models', 'model.py'), os.path.join(project_name, 'models', 'model.py'))
+    shutil.copy(os.path.join(template_dir, 'db', '__init__.py'), os.path.join(project_name, 'db', '__init__.py'))
+    shutil.copy(os.path.join(template_dir, 'db', 'migrations', '__init__.py'), os.path.join(project_name, 'db', 'migrations', '__init__.py'))
+    shutil.copy(os.path.join(template_dir, 'db', 'migrations', 'alembic.ini'), os.path.join(project_name, 'db', 'migrations', 'alembic.ini'))
+    shutil.copy(os.path.join(template_dir, 'views', '__init__.py'), os.path.join(project_name, 'views', '__init__.py'))
+    shutil.copy(os.path.join(template_dir, 'views', 'index.py'), os.path.join(project_name, 'views', 'index.py'))
+    shutil.copy(os.path.join(template_dir, 'templates', 'index.html.jq'), os.path.join(project_name, 'templates', 'index.html.jq'))
+    shutil.copy(os.path.join(template_dir, 'tests', 'test_index.py'), os.path.join(project_name, 'tests', 'test_index.py'))
+    shutil.copy(os.path.join(template_dir, 'static', 'css', 'style.css'), os.path.join(project_name, 'static', 'css', 'style.css'))
+    shutil.copy(os.path.join(template_dir, 'static', 'js', 'script.js'), os.path.join(project_name, 'static', 'js', 'script.js'))
 
     
     # Render README and manage.py templates and write to file
     template = env.get_template('README.md')
     with open(os.path.join(project_name, 'README.md'), 'w') as f:
         f.write(template.render(project_name=project_name))
```

