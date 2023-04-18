# Comparing `tmp/colabtunnel-0.0.5.tar.gz` & `tmp/colabtunnel-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colabtunnel-0.0.5.tar", last modified: Tue Apr 18 12:13:30 2023, max compression
+gzip compressed data, was "colabtunnel-0.0.6.tar", last modified: Tue Apr 18 13:31:03 2023, max compression
```

## Comparing `colabtunnel-0.0.5.tar` & `colabtunnel-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxr-xr-x   0 amitness   (501) staff       (20)        0 2023-04-18 12:13:30.424833 colabtunnel-0.0.5/
--rw-r--r--   0 amitness   (501) staff       (20)     1799 2023-04-18 12:12:51.000000 colabtunnel-0.0.5/.gitignore
--rw-r--r--   0 amitness   (501) staff       (20)     1071 2023-04-18 12:12:51.000000 colabtunnel-0.0.5/LICENSE
--rw-r--r--   0 amitness   (501) staff       (20)      107 2023-04-18 12:12:51.000000 colabtunnel-0.0.5/Makefile
--rw-r--r--   0 amitness   (501) staff       (20)     2701 2023-04-18 12:13:30.424711 colabtunnel-0.0.5/PKG-INFO
--rw-r--r--   0 amitness   (501) staff       (20)     2159 2023-04-18 12:12:51.000000 colabtunnel-0.0.5/README.md
-drwxr-xr-x   0 amitness   (501) staff       (20)        0 2023-04-18 12:13:30.424065 colabtunnel-0.0.5/colabtunnel/
--rw-r--r--   0 amitness   (501) staff       (20)       59 2023-04-18 12:13:20.000000 colabtunnel-0.0.5/colabtunnel/__init__.py
--rw-r--r--   0 amitness   (501) staff       (20)     1993 2023-04-18 12:12:51.000000 colabtunnel-0.0.5/colabtunnel/colabtunnel.py
-drwxr-xr-x   0 amitness   (501) staff       (20)        0 2023-04-18 12:13:30.424528 colabtunnel-0.0.5/colabtunnel.egg-info/
--rw-r--r--   0 amitness   (501) staff       (20)     2701 2023-04-18 12:13:30.000000 colabtunnel-0.0.5/colabtunnel.egg-info/PKG-INFO
--rw-r--r--   0 amitness   (501) staff       (20)      237 2023-04-18 12:13:30.000000 colabtunnel-0.0.5/colabtunnel.egg-info/SOURCES.txt
--rw-r--r--   0 amitness   (501) staff       (20)        1 2023-04-18 12:13:30.000000 colabtunnel-0.0.5/colabtunnel.egg-info/dependency_links.txt
--rw-r--r--   0 amitness   (501) staff       (20)       12 2023-04-18 12:13:30.000000 colabtunnel-0.0.5/colabtunnel.egg-info/top_level.txt
--rw-r--r--   0 amitness   (501) staff       (20)       38 2023-04-18 12:13:30.424876 colabtunnel-0.0.5/setup.cfg
--rw-r--r--   0 amitness   (501) staff       (20)      749 2023-04-18 12:13:15.000000 colabtunnel-0.0.5/setup.py
+drwxr-xr-x   0 amitness   (501) staff       (20)        0 2023-04-18 13:31:03.656842 colabtunnel-0.0.6/
+-rw-r--r--   0 amitness   (501) staff       (20)     1071 2023-04-18 12:12:51.000000 colabtunnel-0.0.6/LICENSE
+-rw-r--r--   0 amitness   (501) staff       (20)     2799 2023-04-18 13:31:03.656723 colabtunnel-0.0.6/PKG-INFO
+-rw-r--r--   0 amitness   (501) staff       (20)     2263 2023-04-18 13:29:26.000000 colabtunnel-0.0.6/README.md
+drwxr-xr-x   0 amitness   (501) staff       (20)        0 2023-04-18 13:31:03.656066 colabtunnel-0.0.6/colabtunnel/
+-rw-r--r--   0 amitness   (501) staff       (20)       59 2023-04-18 13:30:47.000000 colabtunnel-0.0.6/colabtunnel/__init__.py
+-rw-r--r--   0 amitness   (501) staff       (20)     1993 2023-04-18 12:12:51.000000 colabtunnel-0.0.6/colabtunnel/colabtunnel.py
+drwxr-xr-x   0 amitness   (501) staff       (20)        0 2023-04-18 13:31:03.656550 colabtunnel-0.0.6/colabtunnel.egg-info/
+-rw-r--r--   0 amitness   (501) staff       (20)     2799 2023-04-18 13:31:03.000000 colabtunnel-0.0.6/colabtunnel.egg-info/PKG-INFO
+-rw-r--r--   0 amitness   (501) staff       (20)      217 2023-04-18 13:31:03.000000 colabtunnel-0.0.6/colabtunnel.egg-info/SOURCES.txt
+-rw-r--r--   0 amitness   (501) staff       (20)        1 2023-04-18 13:31:03.000000 colabtunnel-0.0.6/colabtunnel.egg-info/dependency_links.txt
+-rw-r--r--   0 amitness   (501) staff       (20)       12 2023-04-18 13:31:03.000000 colabtunnel-0.0.6/colabtunnel.egg-info/top_level.txt
+-rw-r--r--   0 amitness   (501) staff       (20)       38 2023-04-18 13:31:03.656887 colabtunnel-0.0.6/setup.cfg
+-rw-r--r--   0 amitness   (501) staff       (20)      725 2023-04-18 13:30:43.000000 colabtunnel-0.0.6/setup.py
```

### Comparing `colabtunnel-0.0.5/LICENSE` & `colabtunnel-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `colabtunnel-0.0.5/PKG-INFO` & `colabtunnel-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: colabtunnel
-Version: 0.0.5
-Summary: Run code-server on Google Colab with persistence of settings and code.
+Version: 0.0.6
+Summary: Connect to Google Colab VM locally from VSCode
 Home-page: https://github.com/amitness/colab-tunnel
 Author: Amit Chaudhary
 Author-email: meamitkc@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -17,14 +18,16 @@
 
 <img src="https://user-images.githubusercontent.com/8587189/232764837-40865915-1cef-40da-989b-f19773b15de1.png" align="right" width="75" height="75">
 
 # colab-tunnel
 
 Access Google Colab directly from your local VS Code editor using [remote tunnels](https://code.visualstudio.com/docs/remote/tunnels).
 
+https://user-images.githubusercontent.com/8587189/232783372-8f2a5f83-1e57-42f0-8740-4b7e5901b561.mp4
+
 ## Usage
 You can make a copy of this [notebook](https://colab.research.google.com/drive/1VAlrgB4IpBazkQRrZtSPjeTNR3P27FwQ?usp=sharing) to get started.
 
 On Google Colab, first install the library and the run the code.
 ```shell
 !pip install colabtunnel
 ```
@@ -55,7 +58,9 @@
 <img width="676" alt="image" src="https://user-images.githubusercontent.com/8587189/232767113-b7acac1c-c236-4dcb-852c-fbe179e3e6ab.png">
 </p>
 
 5. You will be connected to the virtual machine and can access the folders. Open the `/colab` folder and store your code there for persistence on Google Drive. The workflow is similar to the Remote SSH plugin
 
 ![image](https://user-images.githubusercontent.com/8587189/232769273-52d3e26a-3aec-436d-9b60-97e1d190ddf7.png)
 
+
+
```

### Comparing `colabtunnel-0.0.5/README.md` & `colabtunnel-0.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 <img src="https://user-images.githubusercontent.com/8587189/232764837-40865915-1cef-40da-989b-f19773b15de1.png" align="right" width="75" height="75">
 
 # colab-tunnel
 
 Access Google Colab directly from your local VS Code editor using [remote tunnels](https://code.visualstudio.com/docs/remote/tunnels).
 
+https://user-images.githubusercontent.com/8587189/232783372-8f2a5f83-1e57-42f0-8740-4b7e5901b561.mp4
+
 ## Usage
 You can make a copy of this [notebook](https://colab.research.google.com/drive/1VAlrgB4IpBazkQRrZtSPjeTNR3P27FwQ?usp=sharing) to get started.
 
 On Google Colab, first install the library and the run the code.
 ```shell
 !pip install colabtunnel
 ```
```

### Comparing `colabtunnel-0.0.5/colabtunnel/colabtunnel.py` & `colabtunnel-0.0.6/colabtunnel/colabtunnel.py`

 * *Files identical despite different names*

### Comparing `colabtunnel-0.0.5/colabtunnel.egg-info/PKG-INFO` & `colabtunnel-0.0.6/colabtunnel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: colabtunnel
-Version: 0.0.5
-Summary: Run code-server on Google Colab with persistence of settings and code.
+Version: 0.0.6
+Summary: Connect to Google Colab VM locally from VSCode
 Home-page: https://github.com/amitness/colab-tunnel
 Author: Amit Chaudhary
 Author-email: meamitkc@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -17,14 +18,16 @@
 
 <img src="https://user-images.githubusercontent.com/8587189/232764837-40865915-1cef-40da-989b-f19773b15de1.png" align="right" width="75" height="75">
 
 # colab-tunnel
 
 Access Google Colab directly from your local VS Code editor using [remote tunnels](https://code.visualstudio.com/docs/remote/tunnels).
 
+https://user-images.githubusercontent.com/8587189/232783372-8f2a5f83-1e57-42f0-8740-4b7e5901b561.mp4
+
 ## Usage
 You can make a copy of this [notebook](https://colab.research.google.com/drive/1VAlrgB4IpBazkQRrZtSPjeTNR3P27FwQ?usp=sharing) to get started.
 
 On Google Colab, first install the library and the run the code.
 ```shell
 !pip install colabtunnel
 ```
@@ -55,7 +58,9 @@
 <img width="676" alt="image" src="https://user-images.githubusercontent.com/8587189/232767113-b7acac1c-c236-4dcb-852c-fbe179e3e6ab.png">
 </p>
 
 5. You will be connected to the virtual machine and can access the folders. Open the `/colab` folder and store your code there for persistence on Google Drive. The workflow is similar to the Remote SSH plugin
 
 ![image](https://user-images.githubusercontent.com/8587189/232769273-52d3e26a-3aec-436d-9b60-97e1d190ddf7.png)
 
+
+
```

### Comparing `colabtunnel-0.0.5/setup.py` & `colabtunnel-0.0.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="colabtunnel",
-    version="0.0.5",
+    version="0.0.6",
     license="MIT",
-    description="Run code-server on Google Colab with persistence of settings and code.",
+    description="Connect to Google Colab VM locally from VSCode",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
```

