# Comparing `tmp/jaquar-0.6.0.tar.gz` & `tmp/jaquar-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jaquar-0.6.0.tar", last modified: Tue Apr 18 09:27:46 2023, max compression
+gzip compressed data, was "dist\jaquar-0.6.1.tar", last modified: Tue Apr 18 09:30:05 2023, max compression
```

## Comparing `jaquar-0.6.0.tar` & `jaquar-0.6.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 09:27:46.000000 jaquar-0.6.0/
-drwxrwxrwx   0        0        0        0 2023-04-18 09:27:46.000000 jaquar-0.6.0/jaquar/
--rw-rw-rw-   0        0        0     3749 2023-04-18 09:27:23.000000 jaquar-0.6.0/jaquar/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:27:46.000000 jaquar-0.6.0/jaquar/templates/
-drwxrwxrwx   0        0        0        0 2023-04-18 09:27:46.000000 jaquar-0.6.0/jaquar/templates/static/
-drwxrwxrwx   0        0        0        0 2023-04-18 09:27:46.000000 jaquar-0.6.0/jaquar/templates/static/css/
--rw-rw-rw-   0        0        0        0 2023-04-18 08:36:39.000000 jaquar-0.6.0/jaquar/templates/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-04-18 09:27:46.000000 jaquar-0.6.0/jaquar/templates/static/js/
--rw-rw-rw-   0        0        0        0 2023-04-18 08:36:27.000000 jaquar-0.6.0/jaquar/templates/static/js/scripts.js
--rw-rw-rw-   0        0        0       43 2023-04-18 08:14:51.000000 jaquar-0.6.0/jaquar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:27:46.000000 jaquar-0.6.0/jaquar.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-18 09:27:45.000000 jaquar-0.6.0/jaquar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-18 09:27:45.000000 jaquar-0.6.0/jaquar.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      234 2023-04-18 09:27:45.000000 jaquar-0.6.0/jaquar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-04-18 09:27:45.000000 jaquar-0.6.0/jaquar.egg-info/requires.txt
--rw-rw-rw-   0        0        0      311 2023-04-18 09:27:45.000000 jaquar-0.6.0/jaquar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 09:27:45.000000 jaquar-0.6.0/jaquar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       99 2023-04-18 06:04:11.000000 jaquar-0.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0      234 2023-04-18 09:27:46.000000 jaquar-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-04-18 09:27:46.000000 jaquar-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0      505 2023-04-18 09:27:43.000000 jaquar-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:30:05.000000 jaquar-0.6.1/
+drwxrwxrwx   0        0        0        0 2023-04-18 09:30:05.000000 jaquar-0.6.1/jaquar/
+-rw-rw-rw-   0        0        0     3680 2023-04-18 09:29:34.000000 jaquar-0.6.1/jaquar/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:30:05.000000 jaquar-0.6.1/jaquar/templates/
+drwxrwxrwx   0        0        0        0 2023-04-18 09:30:05.000000 jaquar-0.6.1/jaquar/templates/static/
+drwxrwxrwx   0        0        0        0 2023-04-18 09:30:05.000000 jaquar-0.6.1/jaquar/templates/static/css/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:36:39.000000 jaquar-0.6.1/jaquar/templates/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-04-18 09:30:05.000000 jaquar-0.6.1/jaquar/templates/static/js/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:36:27.000000 jaquar-0.6.1/jaquar/templates/static/js/scripts.js
+-rw-rw-rw-   0        0        0       43 2023-04-18 08:14:51.000000 jaquar-0.6.1/jaquar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:30:05.000000 jaquar-0.6.1/jaquar.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-18 09:30:04.000000 jaquar-0.6.1/jaquar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-18 09:30:04.000000 jaquar-0.6.1/jaquar.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      234 2023-04-18 09:30:04.000000 jaquar-0.6.1/jaquar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-04-18 09:30:04.000000 jaquar-0.6.1/jaquar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      311 2023-04-18 09:30:04.000000 jaquar-0.6.1/jaquar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 09:30:04.000000 jaquar-0.6.1/jaquar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       99 2023-04-18 06:04:11.000000 jaquar-0.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      234 2023-04-18 09:30:05.000000 jaquar-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-04-18 09:30:05.000000 jaquar-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      505 2023-04-18 09:29:53.000000 jaquar-0.6.1/setup.py
```

### Comparing `jaquar-0.6.0/jaquar/cli.py` & `jaquar-0.6.1/jaquar/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,17 +35,14 @@
     os.makedirs(os.path.join(project_name, 'views'))
     os.makedirs(os.path.join(project_name, 'tests'))
 
     # Copy files from template directory to project directory
     # Get the path to the template directory inside the jaquar package
     template_dir = os.path.join(os.path.dirname(jaquar.__file__), 'templates')
 
-    # Create the project directory
-    os.makedirs(project_name)
-
     # Copy files from template directory to project directory
     shutil.copy(os.path.join(template_dir, 'jq.py'), os.path.join(project_name, 'jq.py'))
     shutil.copy(os.path.join(template_dir, 'config', '__init__.py'), os.path.join(project_name, 'config', '__init__.py'))
     shutil.copy(os.path.join(template_dir, 'config', 'urls.py'), os.path.join(project_name, 'config', 'urls.py'))
     shutil.copy(os.path.join(template_dir, 'config', 'settings.py'), os.path.join(project_name, 'config', 'settings.py'))
     shutil.copy(os.path.join(template_dir, 'models', '__init__.py'), os.path.join(project_name, 'models', '__init__.py'))
     shutil.copy(os.path.join(template_dir, 'models', 'model.py'), os.path.join(project_name, 'models', 'model.py'))
```

