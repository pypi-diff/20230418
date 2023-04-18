# Comparing `tmp/colabtunnel-0.0.6.tar.gz` & `tmp/colabtunnel-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colabtunnel-0.0.6.tar", last modified: Tue Apr 18 13:31:03 2023, max compression
+gzip compressed data, was "colabtunnel-0.0.7.tar", last modified: Tue Apr 18 14:14:19 2023, max compression
```

## Comparing `colabtunnel-0.0.6.tar` & `colabtunnel-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 amitness   (501) staff       (20)        0 2023-04-18 13:31:03.656842 colabtunnel-0.0.6/
--rw-r--r--   0 amitness   (501) staff       (20)     1071 2023-04-18 12:12:51.000000 colabtunnel-0.0.6/LICENSE
--rw-r--r--   0 amitness   (501) staff       (20)     2799 2023-04-18 13:31:03.656723 colabtunnel-0.0.6/PKG-INFO
--rw-r--r--   0 amitness   (501) staff       (20)     2263 2023-04-18 13:29:26.000000 colabtunnel-0.0.6/README.md
-drwxr-xr-x   0 amitness   (501) staff       (20)        0 2023-04-18 13:31:03.656066 colabtunnel-0.0.6/colabtunnel/
--rw-r--r--   0 amitness   (501) staff       (20)       59 2023-04-18 13:30:47.000000 colabtunnel-0.0.6/colabtunnel/__init__.py
--rw-r--r--   0 amitness   (501) staff       (20)     1993 2023-04-18 12:12:51.000000 colabtunnel-0.0.6/colabtunnel/colabtunnel.py
-drwxr-xr-x   0 amitness   (501) staff       (20)        0 2023-04-18 13:31:03.656550 colabtunnel-0.0.6/colabtunnel.egg-info/
--rw-r--r--   0 amitness   (501) staff       (20)     2799 2023-04-18 13:31:03.000000 colabtunnel-0.0.6/colabtunnel.egg-info/PKG-INFO
--rw-r--r--   0 amitness   (501) staff       (20)      217 2023-04-18 13:31:03.000000 colabtunnel-0.0.6/colabtunnel.egg-info/SOURCES.txt
--rw-r--r--   0 amitness   (501) staff       (20)        1 2023-04-18 13:31:03.000000 colabtunnel-0.0.6/colabtunnel.egg-info/dependency_links.txt
--rw-r--r--   0 amitness   (501) staff       (20)       12 2023-04-18 13:31:03.000000 colabtunnel-0.0.6/colabtunnel.egg-info/top_level.txt
--rw-r--r--   0 amitness   (501) staff       (20)       38 2023-04-18 13:31:03.656887 colabtunnel-0.0.6/setup.cfg
--rw-r--r--   0 amitness   (501) staff       (20)      725 2023-04-18 13:30:43.000000 colabtunnel-0.0.6/setup.py
+drwxr-xr-x   0 amitness   (501) staff       (20)        0 2023-04-18 14:14:19.929221 colabtunnel-0.0.7/
+-rw-r--r--   0 amitness   (501) staff       (20)     1799 2023-04-18 12:12:51.000000 colabtunnel-0.0.7/.gitignore
+-rw-r--r--   0 amitness   (501) staff       (20)     1071 2023-04-18 12:12:51.000000 colabtunnel-0.0.7/LICENSE
+-rw-r--r--   0 amitness   (501) staff       (20)      107 2023-04-18 12:12:51.000000 colabtunnel-0.0.7/Makefile
+-rw-r--r--   0 amitness   (501) staff       (20)     2779 2023-04-18 14:14:19.929109 colabtunnel-0.0.7/PKG-INFO
+-rw-r--r--   0 amitness   (501) staff       (20)     2263 2023-04-18 13:29:26.000000 colabtunnel-0.0.7/README.md
+drwxr-xr-x   0 amitness   (501) staff       (20)        0 2023-04-18 14:14:19.928487 colabtunnel-0.0.7/colabtunnel/
+-rw-r--r--   0 amitness   (501) staff       (20)       59 2023-04-18 14:13:24.000000 colabtunnel-0.0.7/colabtunnel/__init__.py
+-rw-r--r--   0 amitness   (501) staff       (20)     2113 2023-04-18 14:13:08.000000 colabtunnel-0.0.7/colabtunnel/colabtunnel.py
+drwxr-xr-x   0 amitness   (501) staff       (20)        0 2023-04-18 14:14:19.928928 colabtunnel-0.0.7/colabtunnel.egg-info/
+-rw-r--r--   0 amitness   (501) staff       (20)     2779 2023-04-18 14:14:19.000000 colabtunnel-0.0.7/colabtunnel.egg-info/PKG-INFO
+-rw-r--r--   0 amitness   (501) staff       (20)      237 2023-04-18 14:14:19.000000 colabtunnel-0.0.7/colabtunnel.egg-info/SOURCES.txt
+-rw-r--r--   0 amitness   (501) staff       (20)        1 2023-04-18 14:14:19.000000 colabtunnel-0.0.7/colabtunnel.egg-info/dependency_links.txt
+-rw-r--r--   0 amitness   (501) staff       (20)       12 2023-04-18 14:14:19.000000 colabtunnel-0.0.7/colabtunnel.egg-info/top_level.txt
+-rw-r--r--   0 amitness   (501) staff       (20)       38 2023-04-18 14:14:19.929262 colabtunnel-0.0.7/setup.cfg
+-rw-r--r--   0 amitness   (501) staff       (20)      725 2023-04-18 14:13:20.000000 colabtunnel-0.0.7/setup.py
```

### Comparing `colabtunnel-0.0.6/LICENSE` & `colabtunnel-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `colabtunnel-0.0.6/PKG-INFO` & `colabtunnel-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: colabtunnel
-Version: 0.0.6
+Version: 0.0.7
 Summary: Connect to Google Colab VM locally from VSCode
 Home-page: https://github.com/amitness/colab-tunnel
 Author: Amit Chaudhary
 Author-email: meamitkc@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -58,9 +57,7 @@
 <img width="676" alt="image" src="https://user-images.githubusercontent.com/8587189/232767113-b7acac1c-c236-4dcb-852c-fbe179e3e6ab.png">
 </p>
 
 5. You will be connected to the virtual machine and can access the folders. Open the `/colab` folder and store your code there for persistence on Google Drive. The workflow is similar to the Remote SSH plugin
 
 ![image](https://user-images.githubusercontent.com/8587189/232769273-52d3e26a-3aec-436d-9b60-97e1d190ddf7.png)
 
-
-
```

### Comparing `colabtunnel-0.0.6/README.md` & `colabtunnel-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `colabtunnel-0.0.6/colabtunnel/colabtunnel.py` & `colabtunnel-0.0.7/colabtunnel/colabtunnel.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from pathlib import Path
 import subprocess
 from importlib import import_module
 import time
+import sys
+
 
 message = """
 - Ready!
 - Open VSCode on your laptop and open the command prompt
 - Select: 'Remote-Tunnels: Connect to Tunnel' to connect to colab
 """.strip()
 
@@ -35,26 +37,29 @@
 
 
 def run(command: str) -> None:
     process = subprocess.run(command.split())
     if process.returncode == 0:
         print(f"Ran: {command}")
 
+def is_colab():
+    return 'google.colab' in sys.modules
 
 def colabtunnel() -> None:
-    print("Mounting Google Drive...")
-    drive = import_module("google.colab.drive")
-    drive.mount("/content/drive")
+    if is_colab():
+        print("Mounting Google Drive...")
+        drive = import_module("google.colab.drive")
+        drive.mount("/content/drive")
     
-    # Create a folder on drive to store all the code files
-    drive_folder = '/content/drive/MyDrive/colab/'
-    Path(drive_folder).mkdir(parents=True, exist_ok=True)
+        # Create a folder on drive to store all the code files
+        drive_folder = '/content/drive/MyDrive/colab/'
+        Path(drive_folder).mkdir(parents=True, exist_ok=True)
     
-    # Make a /colab path to easily access the folder
-    run(f'ln -s {drive_folder} /')
+        # Make a /colab path to easily access the folder
+        run(f'ln -s {drive_folder} /')
 
     print("Installing python libraries...")
     run("pip3 install --user flake8 black ipywidgets twine")
     run("pip3 install -U ipykernel")
     run("sudo apt install htop -y")
 
     print("Installing vscode-cli...")
```

### Comparing `colabtunnel-0.0.6/colabtunnel.egg-info/PKG-INFO` & `colabtunnel-0.0.7/colabtunnel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: colabtunnel
-Version: 0.0.6
+Version: 0.0.7
 Summary: Connect to Google Colab VM locally from VSCode
 Home-page: https://github.com/amitness/colab-tunnel
 Author: Amit Chaudhary
 Author-email: meamitkc@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -58,9 +57,7 @@
 <img width="676" alt="image" src="https://user-images.githubusercontent.com/8587189/232767113-b7acac1c-c236-4dcb-852c-fbe179e3e6ab.png">
 </p>
 
 5. You will be connected to the virtual machine and can access the folders. Open the `/colab` folder and store your code there for persistence on Google Drive. The workflow is similar to the Remote SSH plugin
 
 ![image](https://user-images.githubusercontent.com/8587189/232769273-52d3e26a-3aec-436d-9b60-97e1d190ddf7.png)
 
-
-
```

### Comparing `colabtunnel-0.0.6/setup.py` & `colabtunnel-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="colabtunnel",
-    version="0.0.6",
+    version="0.0.7",
     license="MIT",
     description="Connect to Google Colab VM locally from VSCode",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

