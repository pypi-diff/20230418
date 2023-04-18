# Comparing `tmp/proteinTools-1.1.0.tar.gz` & `tmp/proteinTools-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-1.1.0.tar", last modified: Tue Apr 18 13:21:25 2023, max compression
+gzip compressed data, was "proteinTools-1.1.1.tar", last modified: Tue Apr 18 14:14:24 2023, max compression
```

## Comparing `proteinTools-1.1.0.tar` & `proteinTools-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 13:21:25.883401 proteinTools-1.1.0/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.1.0/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-18 13:21:25.879541 proteinTools-1.1.0/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.1.0/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 13:21:25.802013 proteinTools-1.1.0/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    47864 2023-04-18 13:21:17.000000 proteinTools-1.1.0/proteinTools/PT.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.1.0/proteinTools/__init__.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 13:21:25.860545 proteinTools-1.1.0/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-18 13:21:25.000000 proteinTools-1.1.0/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-18 13:21:25.000000 proteinTools-1.1.0/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-18 13:21:25.000000 proteinTools-1.1.0/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       48 2023-04-18 13:21:25.000000 proteinTools-1.1.0/proteinTools.egg-info/requires.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-18 13:21:25.000000 proteinTools-1.1.0/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-18 13:21:25.887610 proteinTools-1.1.0/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      512 2023-04-18 13:20:56.000000 proteinTools-1.1.0/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 14:14:24.934043 proteinTools-1.1.1/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.1.1/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-18 14:14:24.929192 proteinTools-1.1.1/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.1.1/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 14:14:24.860252 proteinTools-1.1.1/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    48681 2023-04-18 14:14:11.000000 proteinTools-1.1.1/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.1.1/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 14:14:24.914067 proteinTools-1.1.1/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-18 14:14:24.000000 proteinTools-1.1.1/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-18 14:14:24.000000 proteinTools-1.1.1/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-18 14:14:24.000000 proteinTools-1.1.1/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       68 2023-04-18 14:14:24.000000 proteinTools-1.1.1/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-18 14:14:24.000000 proteinTools-1.1.1/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-18 14:14:24.938602 proteinTools-1.1.1/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      538 2023-04-18 14:12:40.000000 proteinTools-1.1.1/setup.py
```

### Comparing `proteinTools-1.1.0/LICENSE` & `proteinTools-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-1.1.0/proteinTools/PT.py` & `proteinTools-1.1.1/proteinTools/PT.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import xml.etree.ElementTree as ET
 import sys
 import csv
 import mygene 
 import requests
 from functools import cached_property, lru_cache
 import urllib
+import openbabel
+import pubchempy as pcp
 import pandas as pd
 import numpy as np
 import traceback
 from io import StringIO
 from chembl_webresource_client.new_client import new_client
 import re
 mg = mygene.MyGeneInfo()
@@ -125,15 +127,15 @@
         self.atoms = []
         
    
     def download(self, directory = os.getcwd()):
         """
         Download Ligand
     
-        This method downloads the specific ligand structural file based on the ligand ID. 
+        This method downloads the specific ligand structural file based on the ligand ID. Scrapes atoms if file is downloaded outside of protein scope.
     
         Parameters
         ----------
         arg1 : str
             Directory structural file will be downloaded in. Defaults to current user directory.
         """
         try:
@@ -143,15 +145,26 @@
             try:
                 pcp.download('SDF', self.ID + '.sdf' , self.ID, 'smiles', overwrite = True) 
             except:
                 try:
                     pcp.download('SDF', self.ID + '.sdf' , self.ID, 'inchikey', overwrite = True) 
                 except:
                     print('Ligand identifier not found! File downloaded incorrectly')
-            
+        if len(self.atoms) == 0:
+            os.system('obabel -isdf "' + self.ID + '.sdf" -O "' + self.ID + '.pdb" --gen3d')
+            with open(self.ID + '.pdb', 'r') as f:
+                atoms = f.readlines()
+            os.remove(self.ID + '.pdb')
+            for line in atoms:
+                if line[0:4] == 'ATOM' or line[0:6] == 'HETATM':
+                    element = line[76:80].strip()
+                    if element not in atom_keys:
+                        element = element[:1]
+                    atm = atom(element, float(line[30:38].strip()), float(line[38:47].strip()), float(line[47:56].strip()), data = line)
+                    self.atoms.append(atm)
         
     @cached_property
     def center(self):
         """
         Ligand Center of Mass
     
         This property returns the center of mass of the ligand, which is generated from all atom components. 
@@ -1092,9 +1105,10 @@
     - Add more ID conversions
     '''
 
 '''
 #For unit testing    
 if __name__ == '__main__':
     p = Protein('1E66')
-    p.download()
-'''
+    lig = ligand('C1=CC=C(C=C1)C=O')
+    lig.download()
+'''
```

### Comparing `proteinTools-1.1.0/setup.py` & `proteinTools-1.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name = "proteinTools",
-    version = "1.1.0",
+    version = "1.1.1",
     author = "Christian de Frondeville",
     description = "Lightweight package which simplifies interacting with proteins.",
     long_description = long_description,
     packages = ["proteinTools"],
-    install_requires=['pandas','urllib3','chembl-webresource-client','mygene']
+    install_requires=['pandas','urllib3','chembl-webresource-client','mygene', 'openbabel', 'pubchempy']
 
 )
```

