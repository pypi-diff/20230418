# Comparing `tmp/PRauto-0.111.tar.gz` & `tmp/PRauto-0.112.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PRauto-0.111.tar", last modified: Tue Apr 18 11:28:02 2023, max compression
+gzip compressed data, was "PRauto-0.112.tar", last modified: Tue Apr 18 12:06:16 2023, max compression
```

## Comparing `PRauto-0.111.tar` & `PRauto-0.112.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 11:28:02.881348 PRauto-0.111/
--rw-rw-rw-   0        0        0     1098 2023-04-18 06:21:00.000000 PRauto-0.111/LICENSE
--rw-rw-rw-   0        0        0      365 2023-04-18 11:28:02.881348 PRauto-0.111/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-18 11:28:02.869869 PRauto-0.111/PRauto.egg-info/
--rw-rw-rw-   0        0        0      365 2023-04-18 11:28:02.000000 PRauto-0.111/PRauto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-04-18 11:28:02.000000 PRauto-0.111/PRauto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 11:28:02.000000 PRauto-0.111/PRauto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-04-18 11:28:02.000000 PRauto-0.111/PRauto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 11:28:02.000000 PRauto-0.111/PRauto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       12 2023-04-18 06:21:00.000000 PRauto-0.111/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 11:28:02.873869 PRauto-0.111/prauto/
--rw-rw-rw-   0        0        0        0 2023-04-17 00:34:40.000000 PRauto-0.111/prauto/__init__.py
--rw-rw-rw-   0        0        0     1787 2023-04-18 07:56:33.000000 PRauto-0.111/prauto/__main__.py
--rw-rw-rw-   0        0        0    12324 2023-04-18 10:56:42.000000 PRauto-0.111/prauto/get_preprocess.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:28:02.879379 PRauto-0.111/prauto/retriever/
--rw-rw-rw-   0        0        0        0 2023-04-17 00:31:39.000000 PRauto-0.111/prauto/retriever/__init__.py
--rw-rw-rw-   0        0        0     4848 2023-04-18 07:55:44.000000 PRauto-0.111/prauto/retriever/get_fasta.py
--rw-rw-rw-   0        0        0     2749 2023-04-18 10:56:42.000000 PRauto-0.111/prauto/retriever/get_ligand.py
--rw-rw-rw-   0        0        0     4274 2023-04-18 10:56:42.000000 PRauto-0.111/prauto/retriever/get_pdb.py
--rw-rw-rw-   0        0        0       42 2023-04-18 11:28:02.882352 PRauto-0.111/setup.cfg
--rw-rw-rw-   0        0        0     1293 2023-04-18 11:27:21.000000 PRauto-0.111/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:06:16.576630 PRauto-0.112/
+-rw-rw-rw-   0        0        0     1098 2023-04-18 06:21:00.000000 PRauto-0.112/LICENSE
+-rw-rw-rw-   0        0        0      365 2023-04-18 12:06:16.575629 PRauto-0.112/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-18 12:06:16.564630 PRauto-0.112/PRauto.egg-info/
+-rw-rw-rw-   0        0        0      365 2023-04-18 12:06:16.000000 PRauto-0.112/PRauto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-04-18 12:06:16.000000 PRauto-0.112/PRauto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 12:06:16.000000 PRauto-0.112/PRauto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-04-18 12:06:16.000000 PRauto-0.112/PRauto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 12:06:16.000000 PRauto-0.112/PRauto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       12 2023-04-18 06:21:00.000000 PRauto-0.112/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 12:06:16.568630 PRauto-0.112/prauto/
+-rw-rw-rw-   0        0        0        0 2023-04-17 00:34:40.000000 PRauto-0.112/prauto/__init__.py
+-rw-rw-rw-   0        0        0     1790 2023-04-18 12:03:28.000000 PRauto-0.112/prauto/__main__.py
+-rw-rw-rw-   0        0        0    12324 2023-04-18 10:56:42.000000 PRauto-0.112/prauto/get_preprocess.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:06:16.573629 PRauto-0.112/prauto/retriever/
+-rw-rw-rw-   0        0        0        0 2023-04-17 00:31:39.000000 PRauto-0.112/prauto/retriever/__init__.py
+-rw-rw-rw-   0        0        0     4848 2023-04-18 07:55:44.000000 PRauto-0.112/prauto/retriever/get_fasta.py
+-rw-rw-rw-   0        0        0     2749 2023-04-18 10:56:42.000000 PRauto-0.112/prauto/retriever/get_ligand.py
+-rw-rw-rw-   0        0        0     4274 2023-04-18 10:56:42.000000 PRauto-0.112/prauto/retriever/get_pdb.py
+-rw-rw-rw-   0        0        0       42 2023-04-18 12:06:16.576630 PRauto-0.112/setup.cfg
+-rw-rw-rw-   0        0        0     1293 2023-04-18 12:04:08.000000 PRauto-0.112/setup.py
```

### Comparing `PRauto-0.111/LICENSE` & `PRauto-0.112/LICENSE`

 * *Files identical despite different names*

### Comparing `PRauto-0.111/prauto/__main__.py` & `PRauto-0.112/prauto/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
-from retriever.get_fasta import *
-from retriever.get_pdb import *
-from retriever.get_ligand import *
+from .retriever.get_fasta import *
+from .retriever.get_pdb import *
+from .retriever.get_ligand import *
 from tqdm.auto import tqdm
 from tkinter import Tk
 from tkinter import filedialog
 
 root = Tk()
 root.withdraw()
```

### Comparing `PRauto-0.111/prauto/get_preprocess.py` & `PRauto-0.112/prauto/get_preprocess.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.111/prauto/retriever/get_fasta.py` & `PRauto-0.112/prauto/retriever/get_fasta.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.111/prauto/retriever/get_ligand.py` & `PRauto-0.112/prauto/retriever/get_ligand.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.111/prauto/retriever/get_pdb.py` & `PRauto-0.112/prauto/retriever/get_pdb.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.111/setup.py` & `PRauto-0.112/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import setup, find_packages
 import setuptools
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setuptools.setup(name='PRauto',
-        version = '0.111',
+        version = '0.112',
         packages = find_packages(include=['prauto','prauto.*']),
         url = 'https://github.com/KimJisanER/PRauto',
         license = 'MIT license',
         author = 'Ji San Kim',
         author_email = 'jisan1233@gmail.com',
         keywords = 'PDB, FASTA, sdf, Automation',
         description = """
```

