# Comparing `tmp/tupa123-1.3.7.tar.gz` & `tmp/tupa123-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.3.7.tar", last modified: Tue Apr 18 11:51:49 2023, max compression
+gzip compressed data, was "tupa123-1.3.8.tar", last modified: Tue Apr 18 11:59:24 2023, max compression
```

## Comparing `tupa123-1.3.7.tar` & `tupa123-1.3.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 11:51:49.195545 tupa123-1.3.7/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.3.7/LICENSE.txt
--rw-rw-rw-   0        0        0     2345 2023-04-18 11:51:49.195545 tupa123-1.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     1869 2023-04-18 11:48:41.000000 tupa123-1.3.7/README.md
--rw-rw-rw-   0        0        0       42 2023-04-18 11:51:49.195545 tupa123-1.3.7/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-04-18 11:46:01.000000 tupa123-1.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:51:49.179924 tupa123-1.3.7/tupa123/
--rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.3.7/tupa123/__init__.py
--rw-rw-rw-   0        0        0    59976 2023-04-17 20:49:14.000000 tupa123-1.3.7/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:51:49.195545 tupa123-1.3.7/tupa123.egg-info/
--rw-rw-rw-   0        0        0     2345 2023-04-18 11:51:49.000000 tupa123-1.3.7/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-18 11:51:49.000000 tupa123-1.3.7/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 11:51:49.000000 tupa123-1.3.7/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-18 11:51:49.000000 tupa123-1.3.7/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-18 11:51:49.000000 tupa123-1.3.7/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 11:59:24.769330 tupa123-1.3.8/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.3.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     2094 2023-04-18 11:59:24.769330 tupa123-1.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1618 2023-04-18 11:58:24.000000 tupa123-1.3.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 11:59:24.784951 tupa123-1.3.8/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-04-18 11:54:21.000000 tupa123-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:59:24.769330 tupa123-1.3.8/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.3.8/tupa123/__init__.py
+-rw-rw-rw-   0        0        0    59976 2023-04-17 20:49:14.000000 tupa123-1.3.8/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:59:24.769330 tupa123-1.3.8/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     2094 2023-04-18 11:59:24.000000 tupa123-1.3.8/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-18 11:59:24.000000 tupa123-1.3.8/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 11:59:24.000000 tupa123-1.3.8/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-18 11:59:24.000000 tupa123-1.3.8/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-18 11:59:24.000000 tupa123-1.3.8/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.3.7/LICENSE.txt` & `tupa123-1.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.3.7/PKG-INFO` & `tupa123-1.3.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.3.7
+Version: 1.3.8
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 Fully connected four-layer neural network <br>
 Solves a huge number of cases, classification and regression <br>
-The following sequence explains how to use with the help of two example files. <br>
-The first file contains the learning process, where the neural network finds its weights <br>
-The second file demonstrates the network's ability to make predictions on new, unseen data that is not part of the training set <br>
+Fast, robust and very simple to use, <i> this is the way </i> <br>
 <br>
 <br>
 #Manual = https://www.mediafire.com/file/xygt3o9zf7iw3id/Manual_Tupa123.pdf <br>
 <br>
-#Quick Guide = https://www.mediafire.com/file/a0db7fb3lfsxvaj/Guia_Rapido.pdf/file <br>
+#Quick Guide = https://www.mediafire.com/file/a0db7fb3lfsxvaj/Guia_Rapido.pdf <br>
 <br>
 #Excel example data = https://www.mediafire.com/file/o2nzsmnvweh8w1a/ALETAS.xlsx<br>
 #Excel example (old version) = https://www.mediafire.com/file/0xmx5quakd21txu/ALETAS.xls <br>
 <br>
 <br>
 <br>
 #-----FILE TO MACHINE LEARNING <br>
```

### Comparing `tupa123-1.3.7/README.md` & `tupa123-1.3.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Fully connected four-layer neural network <br>
 Solves a huge number of cases, classification and regression <br>
-The following sequence explains how to use with the help of two example files. <br>
-The first file contains the learning process, where the neural network finds its weights <br>
-The second file demonstrates the network's ability to make predictions on new, unseen data that is not part of the training set <br>
+Fast, robust and very simple to use, <i> this is the way </i> <br>
 <br>
 <br>
 #Manual = https://www.mediafire.com/file/xygt3o9zf7iw3id/Manual_Tupa123.pdf <br>
 <br>
-#Quick Guide = https://www.mediafire.com/file/a0db7fb3lfsxvaj/Guia_Rapido.pdf/file <br>
+#Quick Guide = https://www.mediafire.com/file/a0db7fb3lfsxvaj/Guia_Rapido.pdf <br>
 <br>
 #Excel example data = https://www.mediafire.com/file/o2nzsmnvweh8w1a/ALETAS.xlsx<br>
 #Excel example (old version) = https://www.mediafire.com/file/0xmx5quakd21txu/ALETAS.xls <br>
 <br>
 <br>
 <br>
 #-----FILE TO MACHINE LEARNING <br>
```

### Comparing `tupa123-1.3.7/setup.py` & `tupa123-1.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.3.7',
+    version='1.3.8',
     license = 'MIT',
     license_files=('LICENSE.txt',),    
     packages=['tupa123'],
     install_requires=['numpy','matplotlib','pandas'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
     description= 'fully connected neural network with four layers',
```

### Comparing `tupa123-1.3.7/tupa123/tupa123.py` & `tupa123-1.3.8/tupa123/tupa123.py`

 * *Files identical despite different names*

### Comparing `tupa123-1.3.7/tupa123.egg-info/PKG-INFO` & `tupa123-1.3.8/tupa123.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.3.7
+Version: 1.3.8
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 Fully connected four-layer neural network <br>
 Solves a huge number of cases, classification and regression <br>
-The following sequence explains how to use with the help of two example files. <br>
-The first file contains the learning process, where the neural network finds its weights <br>
-The second file demonstrates the network's ability to make predictions on new, unseen data that is not part of the training set <br>
+Fast, robust and very simple to use, <i> this is the way </i> <br>
 <br>
 <br>
 #Manual = https://www.mediafire.com/file/xygt3o9zf7iw3id/Manual_Tupa123.pdf <br>
 <br>
-#Quick Guide = https://www.mediafire.com/file/a0db7fb3lfsxvaj/Guia_Rapido.pdf/file <br>
+#Quick Guide = https://www.mediafire.com/file/a0db7fb3lfsxvaj/Guia_Rapido.pdf <br>
 <br>
 #Excel example data = https://www.mediafire.com/file/o2nzsmnvweh8w1a/ALETAS.xlsx<br>
 #Excel example (old version) = https://www.mediafire.com/file/0xmx5quakd21txu/ALETAS.xls <br>
 <br>
 <br>
 <br>
 #-----FILE TO MACHINE LEARNING <br>
```

