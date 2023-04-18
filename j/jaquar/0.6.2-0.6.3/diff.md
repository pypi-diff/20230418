# Comparing `tmp/jaquar-0.6.2.tar.gz` & `tmp/jaquar-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jaquar-0.6.2.tar", last modified: Tue Apr 18 09:36:33 2023, max compression
+gzip compressed data, was "dist\jaquar-0.6.3.tar", last modified: Tue Apr 18 09:40:56 2023, max compression
```

## Comparing `jaquar-0.6.2.tar` & `jaquar-0.6.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 09:36:33.000000 jaquar-0.6.2/
-drwxrwxrwx   0        0        0        0 2023-04-18 09:36:33.000000 jaquar-0.6.2/jaquar/
--rw-rw-rw-   0        0        0     3680 2023-04-18 09:29:34.000000 jaquar-0.6.2/jaquar/cli.py
--rw-rw-rw-   0        0        0       43 2023-04-18 08:14:51.000000 jaquar-0.6.2/jaquar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:36:33.000000 jaquar-0.6.2/jaquar.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-18 09:36:32.000000 jaquar-0.6.2/jaquar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-18 09:36:32.000000 jaquar-0.6.2/jaquar.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      234 2023-04-18 09:36:32.000000 jaquar-0.6.2/jaquar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-04-18 09:36:32.000000 jaquar-0.6.2/jaquar.egg-info/requires.txt
--rw-rw-rw-   0        0        0      235 2023-04-18 09:36:32.000000 jaquar-0.6.2/jaquar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 09:36:32.000000 jaquar-0.6.2/jaquar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      138 2023-04-18 09:34:44.000000 jaquar-0.6.2/MANIFEST.in
--rw-rw-rw-   0        0        0      234 2023-04-18 09:36:33.000000 jaquar-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-04-18 09:36:33.000000 jaquar-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0      505 2023-04-18 09:36:30.000000 jaquar-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:40:56.000000 jaquar-0.6.3/
+drwxrwxrwx   0        0        0        0 2023-04-18 09:40:56.000000 jaquar-0.6.3/jaquar/
+-rw-rw-rw-   0        0        0     3688 2023-04-18 09:39:38.000000 jaquar-0.6.3/jaquar/cli.py
+-rw-rw-rw-   0        0        0       43 2023-04-18 08:14:51.000000 jaquar-0.6.3/jaquar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:40:56.000000 jaquar-0.6.3/jaquar.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-18 09:40:55.000000 jaquar-0.6.3/jaquar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-18 09:40:55.000000 jaquar-0.6.3/jaquar.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      234 2023-04-18 09:40:55.000000 jaquar-0.6.3/jaquar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-04-18 09:40:55.000000 jaquar-0.6.3/jaquar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      235 2023-04-18 09:40:55.000000 jaquar-0.6.3/jaquar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 09:40:55.000000 jaquar-0.6.3/jaquar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      138 2023-04-18 09:34:44.000000 jaquar-0.6.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      234 2023-04-18 09:40:56.000000 jaquar-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-04-18 09:40:56.000000 jaquar-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      616 2023-04-18 09:40:34.000000 jaquar-0.6.3/setup.py
```

### Comparing `jaquar-0.6.2/jaquar/cli.py` & `jaquar-0.6.3/jaquar/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,18 +48,18 @@
     shutil.copy(os.path.join(template_dir, 'models', 'model.py'), os.path.join(project_name, 'models', 'model.py'))
     shutil.copy(os.path.join(template_dir, 'db', '__init__.py'), os.path.join(project_name, 'db', '__init__.py'))
     shutil.copy(os.path.join(template_dir, 'db', 'migrations', '__init__.py'), os.path.join(project_name, 'db', 'migrations', '__init__.py'))
     shutil.copy(os.path.join(template_dir, 'db', 'migrations', 'alembic.ini'), os.path.join(project_name, 'db', 'migrations', 'alembic.ini'))
     shutil.copy(os.path.join(template_dir, 'views', '__init__.py'), os.path.join(project_name, 'views', '__init__.py'))
     shutil.copy(os.path.join(template_dir, 'views', 'index.py'), os.path.join(project_name, 'views', 'index.py'))
     shutil.copy(os.path.join(template_dir, 'templates', 'index.html.jq'), os.path.join(project_name, 'templates', 'index.html.jq'))
-    shutil.copy(os.path.join(template_dir, 'tests', 'test_index.py'), os.path.join(project_name, 'tests', 'test_index.py'))
-    shutil.copy(os.path.join(template_dir, 'tests', 'test_model.py'), os.path.join(project_name, 'tests', 'test_model.py'))
-    shutil.copy(os.path.join(template_dir, 'tests', 'test_urls.py'), os.path.join(project_name, 'tests', 'test_urls.py'))
-    shutil.copy(os.path.join(template_dir, 'tests', 'test_views.py'), os.path.join(project_name, 'tests', 'test_views.py'))
+    # shutil.copy(os.path.join(template_dir, 'tests', 'test_index.py'), os.path.join(project_name, 'tests', 'test_index.py'))
+    # shutil.copy(os.path.join(template_dir, 'tests', 'test_model.py'), os.path.join(project_name, 'tests', 'test_model.py'))
+    # shutil.copy(os.path.join(template_dir, 'tests', 'test_urls.py'), os.path.join(project_name, 'tests', 'test_urls.py'))
+    # shutil.copy(os.path.join(template_dir, 'tests', 'test_views.py'), os.path.join(project_name, 'tests', 'test_views.py'))
 
     click.echo(f"New Jaquar project '{project_name}' created successfully.")
 
 # Define the CLI entry point.
 if __name__ == '__main__':
     cli()
```

