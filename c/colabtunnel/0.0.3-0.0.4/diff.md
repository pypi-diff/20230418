# Comparing `tmp/colabtunnel-0.0.3.tar.gz` & `tmp/colabtunnel-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colabtunnel-0.0.3.tar", last modified: Tue Apr 18 11:10:55 2023, max compression
+gzip compressed data, was "colabtunnel-0.0.4.tar", last modified: Tue Apr 18 11:18:32 2023, max compression
```

## Comparing `colabtunnel-0.0.3.tar` & `colabtunnel-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwx------   0 root         (0) root         (0)        0 2023-04-18 11:10:55.000000 colabtunnel-0.0.3/
--rw-------   0 root         (0) root         (0)     1071 2023-04-18 11:02:08.000000 colabtunnel-0.0.3/LICENSE
--rw-------   0 root         (0) root         (0)      612 2023-04-18 11:10:55.000000 colabtunnel-0.0.3/PKG-INFO
--rw-------   0 root         (0) root         (0)        0 2023-04-18 11:02:08.000000 colabtunnel-0.0.3/README.md
-drwx------   0 root         (0) root         (0)        0 2023-04-18 11:10:55.000000 colabtunnel-0.0.3/colabtunnel/
--rw-------   0 root         (0) root         (0)       59 2023-04-18 11:04:39.000000 colabtunnel-0.0.3/colabtunnel/__init__.py
--rw-------   0 root         (0) root         (0)     1653 2023-04-18 11:05:22.000000 colabtunnel-0.0.3/colabtunnel/colabtunnel.py
-drwx------   0 root         (0) root         (0)        0 2023-04-18 11:10:55.000000 colabtunnel-0.0.3/colabtunnel.egg-info/
--rw-------   0 root         (0) root         (0)      612 2023-04-18 11:10:55.000000 colabtunnel-0.0.3/colabtunnel.egg-info/PKG-INFO
--rw-------   0 root         (0) root         (0)      217 2023-04-18 11:10:55.000000 colabtunnel-0.0.3/colabtunnel.egg-info/SOURCES.txt
--rw-------   0 root         (0) root         (0)        1 2023-04-18 11:10:55.000000 colabtunnel-0.0.3/colabtunnel.egg-info/dependency_links.txt
--rw-------   0 root         (0) root         (0)       12 2023-04-18 11:10:55.000000 colabtunnel-0.0.3/colabtunnel.egg-info/top_level.txt
--rw-------   0 root         (0) root         (0)       38 2023-04-18 11:10:55.000000 colabtunnel-0.0.3/setup.cfg
--rw-------   0 root         (0) root         (0)      749 2023-04-18 11:04:41.000000 colabtunnel-0.0.3/setup.py
+drwx------   0 root         (0) root         (0)        0 2023-04-18 11:18:32.000000 colabtunnel-0.0.4/
+-rw-------   0 root         (0) root         (0)     1071 2023-04-18 11:02:08.000000 colabtunnel-0.0.4/LICENSE
+-rw-------   0 root         (0) root         (0)      612 2023-04-18 11:18:32.000000 colabtunnel-0.0.4/PKG-INFO
+-rw-------   0 root         (0) root         (0)        0 2023-04-18 11:02:08.000000 colabtunnel-0.0.4/README.md
+drwx------   0 root         (0) root         (0)        0 2023-04-18 11:18:32.000000 colabtunnel-0.0.4/colabtunnel/
+-rw-------   0 root         (0) root         (0)       59 2023-04-18 11:15:38.000000 colabtunnel-0.0.4/colabtunnel/__init__.py
+-rw-------   0 root         (0) root         (0)     1913 2023-04-18 11:14:48.000000 colabtunnel-0.0.4/colabtunnel/colabtunnel.py
+drwx------   0 root         (0) root         (0)        0 2023-04-18 11:18:32.000000 colabtunnel-0.0.4/colabtunnel.egg-info/
+-rw-------   0 root         (0) root         (0)      612 2023-04-18 11:18:31.000000 colabtunnel-0.0.4/colabtunnel.egg-info/PKG-INFO
+-rw-------   0 root         (0) root         (0)      217 2023-04-18 11:18:31.000000 colabtunnel-0.0.4/colabtunnel.egg-info/SOURCES.txt
+-rw-------   0 root         (0) root         (0)        1 2023-04-18 11:18:31.000000 colabtunnel-0.0.4/colabtunnel.egg-info/dependency_links.txt
+-rw-------   0 root         (0) root         (0)       12 2023-04-18 11:18:31.000000 colabtunnel-0.0.4/colabtunnel.egg-info/top_level.txt
+-rw-------   0 root         (0) root         (0)       38 2023-04-18 11:18:32.000000 colabtunnel-0.0.4/setup.cfg
+-rw-------   0 root         (0) root         (0)      749 2023-04-18 11:15:40.000000 colabtunnel-0.0.4/setup.py
```

### Comparing `colabtunnel-0.0.3/LICENSE` & `colabtunnel-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `colabtunnel-0.0.3/PKG-INFO` & `colabtunnel-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colabtunnel
-Version: 0.0.3
+Version: 0.0.4
 Summary: Run code-server on Google Colab with persistence of settings and code.
 Home-page: https://github.com/amitness/colab-tunnel
 Author: Amit Chaudhary
 Author-email: meamitkc@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `colabtunnel-0.0.3/colabtunnel/colabtunnel.py` & `colabtunnel-0.0.4/colabtunnel/colabtunnel.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
+from pathlib import Path
 import subprocess
 from importlib import import_module
-import uuid
-import subprocess
 
 message = """
 - Ready!
 - Open VSCode on your laptop and open the command prompt
 - Select: 'Remote-Tunnels: Connect to Tunnel' to connect to colab
 """.strip()
 
@@ -38,21 +37,28 @@
         print(f"Ran: {command}")
 
 
 def colabtunnel() -> None:
     print("Mounting Google Drive...")
     drive = import_module("google.colab.drive")
     drive.mount("/content/drive")
+    
+    # Create a folder on drive to store all the code files
+    drive_folder = '/content/drive/MyDrive/colab/'
+    Path(drive_folder).mkdir(parents=True, exist_ok=True)
+    
+    # Make a /colab path to easily access the folder
+    run(f'ln -s {drive_folder} /')
 
     print("Installing python libraries...")
     run("pip3 install --user flake8 black ipywidgets twine")
     run("pip3 install -U ipykernel")
     run("sudo apt install htop -y")
 
     print("Installing vscode-cli...")
     run(
         "curl -Lk https://code.visualstudio.com/sha/download?build=stable&os=cli-alpine-x64 --output vscode_cli.tar.gz"
     )
     run("tar -xf vscode_cli.tar.gz")
 
     print("Starting the tunnel")
-    start_tunnel()
+    start_tunnel()
```

### Comparing `colabtunnel-0.0.3/colabtunnel.egg-info/PKG-INFO` & `colabtunnel-0.0.4/colabtunnel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colabtunnel
-Version: 0.0.3
+Version: 0.0.4
 Summary: Run code-server on Google Colab with persistence of settings and code.
 Home-page: https://github.com/amitness/colab-tunnel
 Author: Amit Chaudhary
 Author-email: meamitkc@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `colabtunnel-0.0.3/setup.py` & `colabtunnel-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="colabtunnel",
-    version="0.0.3",
+    version="0.0.4",
     license="MIT",
     description="Run code-server on Google Colab with persistence of settings and code.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

