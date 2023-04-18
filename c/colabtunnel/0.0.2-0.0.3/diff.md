# Comparing `tmp/colabtunnel-0.0.2.tar.gz` & `tmp/colabtunnel-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colabtunnel-0.0.2.tar", last modified: Mon Apr 17 20:31:50 2023, max compression
+gzip compressed data, was "colabtunnel-0.0.3.tar", last modified: Tue Apr 18 11:10:55 2023, max compression
```

## Comparing `colabtunnel-0.0.2.tar` & `colabtunnel-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwx------   0 root         (0) root         (0)        0 2023-04-17 20:31:50.000000 colabtunnel-0.0.2/
--rw-------   0 root         (0) root         (0)     1071 2023-04-17 19:55:48.000000 colabtunnel-0.0.2/LICENSE
--rw-------   0 root         (0) root         (0)      598 2023-04-17 20:31:50.000000 colabtunnel-0.0.2/PKG-INFO
--rw-------   0 root         (0) root         (0)        0 2023-04-17 20:06:07.000000 colabtunnel-0.0.2/README.md
-drwx------   0 root         (0) root         (0)        0 2023-04-17 20:31:50.000000 colabtunnel-0.0.2/colabtunnel/
--rw-------   0 root         (0) root         (0)       59 2023-04-17 20:31:31.000000 colabtunnel-0.0.2/colabtunnel/__init__.py
--rw-------   0 root         (0) root         (0)     1647 2023-04-17 20:06:00.000000 colabtunnel-0.0.2/colabtunnel/colabtunnel.py
-drwx------   0 root         (0) root         (0)        0 2023-04-17 20:31:50.000000 colabtunnel-0.0.2/colabtunnel.egg-info/
--rw-------   0 root         (0) root         (0)      598 2023-04-17 20:31:50.000000 colabtunnel-0.0.2/colabtunnel.egg-info/PKG-INFO
--rw-------   0 root         (0) root         (0)      217 2023-04-17 20:31:50.000000 colabtunnel-0.0.2/colabtunnel.egg-info/SOURCES.txt
--rw-------   0 root         (0) root         (0)        1 2023-04-17 20:31:50.000000 colabtunnel-0.0.2/colabtunnel.egg-info/dependency_links.txt
--rw-------   0 root         (0) root         (0)       12 2023-04-17 20:31:50.000000 colabtunnel-0.0.2/colabtunnel.egg-info/top_level.txt
--rw-------   0 root         (0) root         (0)       38 2023-04-17 20:31:50.000000 colabtunnel-0.0.2/setup.cfg
--rw-------   0 root         (0) root         (0)      735 2023-04-17 20:31:26.000000 colabtunnel-0.0.2/setup.py
+drwx------   0 root         (0) root         (0)        0 2023-04-18 11:10:55.000000 colabtunnel-0.0.3/
+-rw-------   0 root         (0) root         (0)     1071 2023-04-18 11:02:08.000000 colabtunnel-0.0.3/LICENSE
+-rw-------   0 root         (0) root         (0)      612 2023-04-18 11:10:55.000000 colabtunnel-0.0.3/PKG-INFO
+-rw-------   0 root         (0) root         (0)        0 2023-04-18 11:02:08.000000 colabtunnel-0.0.3/README.md
+drwx------   0 root         (0) root         (0)        0 2023-04-18 11:10:55.000000 colabtunnel-0.0.3/colabtunnel/
+-rw-------   0 root         (0) root         (0)       59 2023-04-18 11:04:39.000000 colabtunnel-0.0.3/colabtunnel/__init__.py
+-rw-------   0 root         (0) root         (0)     1653 2023-04-18 11:05:22.000000 colabtunnel-0.0.3/colabtunnel/colabtunnel.py
+drwx------   0 root         (0) root         (0)        0 2023-04-18 11:10:55.000000 colabtunnel-0.0.3/colabtunnel.egg-info/
+-rw-------   0 root         (0) root         (0)      612 2023-04-18 11:10:55.000000 colabtunnel-0.0.3/colabtunnel.egg-info/PKG-INFO
+-rw-------   0 root         (0) root         (0)      217 2023-04-18 11:10:55.000000 colabtunnel-0.0.3/colabtunnel.egg-info/SOURCES.txt
+-rw-------   0 root         (0) root         (0)        1 2023-04-18 11:10:55.000000 colabtunnel-0.0.3/colabtunnel.egg-info/dependency_links.txt
+-rw-------   0 root         (0) root         (0)       12 2023-04-18 11:10:55.000000 colabtunnel-0.0.3/colabtunnel.egg-info/top_level.txt
+-rw-------   0 root         (0) root         (0)       38 2023-04-18 11:10:55.000000 colabtunnel-0.0.3/setup.cfg
+-rw-------   0 root         (0) root         (0)      749 2023-04-18 11:04:41.000000 colabtunnel-0.0.3/setup.py
```

### Comparing `colabtunnel-0.0.2/LICENSE` & `colabtunnel-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `colabtunnel-0.0.2/colabtunnel/colabtunnel.py` & `colabtunnel-0.0.3/colabtunnel/colabtunnel.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 def colabtunnel() -> None:
     print("Mounting Google Drive...")
     drive = import_module("google.colab.drive")
     drive.mount("/content/drive")
 
     print("Installing python libraries...")
-    run("pip3 install --user flake8 black ipywidgets")
+    run("pip3 install --user flake8 black ipywidgets twine")
     run("pip3 install -U ipykernel")
     run("sudo apt install htop -y")
 
     print("Installing vscode-cli...")
     run(
         "curl -Lk https://code.visualstudio.com/sha/download?build=stable&os=cli-alpine-x64 --output vscode_cli.tar.gz"
     )
```

### Comparing `colabtunnel-0.0.2/setup.py` & `colabtunnel-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="colabtunnel",
-    version="0.0.2",
+    version="0.0.3",
     license="MIT",
-    description="Connect to Google Colab VM from your local VSCode Editor",
+    description="Run code-server on Google Colab with persistence of settings and code.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
```

