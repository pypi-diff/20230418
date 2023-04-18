# Comparing `tmp/colabtunnel-0.0.4.tar.gz` & `tmp/colabtunnel-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colabtunnel-0.0.4.tar", last modified: Tue Apr 18 11:18:32 2023, max compression
+gzip compressed data, was "colabtunnel-0.0.5.tar", last modified: Tue Apr 18 12:13:30 2023, max compression
```

## Comparing `colabtunnel-0.0.4.tar` & `colabtunnel-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwx------   0 root         (0) root         (0)        0 2023-04-18 11:18:32.000000 colabtunnel-0.0.4/
--rw-------   0 root         (0) root         (0)     1071 2023-04-18 11:02:08.000000 colabtunnel-0.0.4/LICENSE
--rw-------   0 root         (0) root         (0)      612 2023-04-18 11:18:32.000000 colabtunnel-0.0.4/PKG-INFO
--rw-------   0 root         (0) root         (0)        0 2023-04-18 11:02:08.000000 colabtunnel-0.0.4/README.md
-drwx------   0 root         (0) root         (0)        0 2023-04-18 11:18:32.000000 colabtunnel-0.0.4/colabtunnel/
--rw-------   0 root         (0) root         (0)       59 2023-04-18 11:15:38.000000 colabtunnel-0.0.4/colabtunnel/__init__.py
--rw-------   0 root         (0) root         (0)     1913 2023-04-18 11:14:48.000000 colabtunnel-0.0.4/colabtunnel/colabtunnel.py
-drwx------   0 root         (0) root         (0)        0 2023-04-18 11:18:32.000000 colabtunnel-0.0.4/colabtunnel.egg-info/
--rw-------   0 root         (0) root         (0)      612 2023-04-18 11:18:31.000000 colabtunnel-0.0.4/colabtunnel.egg-info/PKG-INFO
--rw-------   0 root         (0) root         (0)      217 2023-04-18 11:18:31.000000 colabtunnel-0.0.4/colabtunnel.egg-info/SOURCES.txt
--rw-------   0 root         (0) root         (0)        1 2023-04-18 11:18:31.000000 colabtunnel-0.0.4/colabtunnel.egg-info/dependency_links.txt
--rw-------   0 root         (0) root         (0)       12 2023-04-18 11:18:31.000000 colabtunnel-0.0.4/colabtunnel.egg-info/top_level.txt
--rw-------   0 root         (0) root         (0)       38 2023-04-18 11:18:32.000000 colabtunnel-0.0.4/setup.cfg
--rw-------   0 root         (0) root         (0)      749 2023-04-18 11:15:40.000000 colabtunnel-0.0.4/setup.py
+drwxr-xr-x   0 amitness   (501) staff       (20)        0 2023-04-18 12:13:30.424833 colabtunnel-0.0.5/
+-rw-r--r--   0 amitness   (501) staff       (20)     1799 2023-04-18 12:12:51.000000 colabtunnel-0.0.5/.gitignore
+-rw-r--r--   0 amitness   (501) staff       (20)     1071 2023-04-18 12:12:51.000000 colabtunnel-0.0.5/LICENSE
+-rw-r--r--   0 amitness   (501) staff       (20)      107 2023-04-18 12:12:51.000000 colabtunnel-0.0.5/Makefile
+-rw-r--r--   0 amitness   (501) staff       (20)     2701 2023-04-18 12:13:30.424711 colabtunnel-0.0.5/PKG-INFO
+-rw-r--r--   0 amitness   (501) staff       (20)     2159 2023-04-18 12:12:51.000000 colabtunnel-0.0.5/README.md
+drwxr-xr-x   0 amitness   (501) staff       (20)        0 2023-04-18 12:13:30.424065 colabtunnel-0.0.5/colabtunnel/
+-rw-r--r--   0 amitness   (501) staff       (20)       59 2023-04-18 12:13:20.000000 colabtunnel-0.0.5/colabtunnel/__init__.py
+-rw-r--r--   0 amitness   (501) staff       (20)     1993 2023-04-18 12:12:51.000000 colabtunnel-0.0.5/colabtunnel/colabtunnel.py
+drwxr-xr-x   0 amitness   (501) staff       (20)        0 2023-04-18 12:13:30.424528 colabtunnel-0.0.5/colabtunnel.egg-info/
+-rw-r--r--   0 amitness   (501) staff       (20)     2701 2023-04-18 12:13:30.000000 colabtunnel-0.0.5/colabtunnel.egg-info/PKG-INFO
+-rw-r--r--   0 amitness   (501) staff       (20)      237 2023-04-18 12:13:30.000000 colabtunnel-0.0.5/colabtunnel.egg-info/SOURCES.txt
+-rw-r--r--   0 amitness   (501) staff       (20)        1 2023-04-18 12:13:30.000000 colabtunnel-0.0.5/colabtunnel.egg-info/dependency_links.txt
+-rw-r--r--   0 amitness   (501) staff       (20)       12 2023-04-18 12:13:30.000000 colabtunnel-0.0.5/colabtunnel.egg-info/top_level.txt
+-rw-r--r--   0 amitness   (501) staff       (20)       38 2023-04-18 12:13:30.424876 colabtunnel-0.0.5/setup.cfg
+-rw-r--r--   0 amitness   (501) staff       (20)      749 2023-04-18 12:13:15.000000 colabtunnel-0.0.5/setup.py
```

### Comparing `colabtunnel-0.0.4/LICENSE` & `colabtunnel-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `colabtunnel-0.0.4/colabtunnel/colabtunnel.py` & `colabtunnel-0.0.5/colabtunnel/colabtunnel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pathlib import Path
 import subprocess
 from importlib import import_module
+import time
 
 message = """
 - Ready!
 - Open VSCode on your laptop and open the command prompt
 - Select: 'Remote-Tunnels: Connect to Tunnel' to connect to colab
 """.strip()
 
@@ -18,14 +19,16 @@
     while True:
         line = p.stdout.readline().decode("utf-8")
         if show_outputs:
             print(line.strip())
         if "To grant access to the server" in line:
             print(line.strip())
         if "Open this link" in line:
+            print("Starting the tunnel")
+            time.sleep(5)
             print(message)
             print("Logs:")
             show_outputs = True
             line = ""
         if line == "" and p.poll() is not None:
             break
     return None
@@ -57,8 +60,8 @@
     print("Installing vscode-cli...")
     run(
         "curl -Lk https://code.visualstudio.com/sha/download?build=stable&os=cli-alpine-x64 --output vscode_cli.tar.gz"
     )
     run("tar -xf vscode_cli.tar.gz")
 
     print("Starting the tunnel")
-    start_tunnel()
+    start_tunnel()
```

### Comparing `colabtunnel-0.0.4/setup.py` & `colabtunnel-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="colabtunnel",
-    version="0.0.4",
+    version="0.0.5",
     license="MIT",
     description="Run code-server on Google Colab with persistence of settings and code.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

