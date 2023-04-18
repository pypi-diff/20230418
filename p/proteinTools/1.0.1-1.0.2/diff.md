# Comparing `tmp/proteinTools-1.0.1.tar.gz` & `tmp/proteinTools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-1.0.1.tar", last modified: Mon Apr 17 19:48:06 2023, max compression
+gzip compressed data, was "proteinTools-1.0.2.tar", last modified: Tue Apr 18 02:01:13 2023, max compression
```

## Comparing `proteinTools-1.0.1.tar` & `proteinTools-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-17 19:48:06.768603 proteinTools-1.0.1/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.0.1/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-17 19:48:06.761246 proteinTools-1.0.1/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.0.1/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-17 19:48:06.595533 proteinTools-1.0.1/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    47068 2023-04-17 19:45:09.000000 proteinTools-1.0.1/proteinTools/PT.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.0.1/proteinTools/__init__.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-17 19:48:06.733715 proteinTools-1.0.1/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-17 19:48:06.000000 proteinTools-1.0.1/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-17 19:48:06.000000 proteinTools-1.0.1/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-17 19:48:06.000000 proteinTools-1.0.1/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       48 2023-04-17 19:48:06.000000 proteinTools-1.0.1/proteinTools.egg-info/requires.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-17 19:48:06.000000 proteinTools-1.0.1/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-17 19:48:06.775256 proteinTools-1.0.1/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      512 2023-04-17 19:47:05.000000 proteinTools-1.0.1/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 02:01:12.920702 proteinTools-1.0.2/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.0.2/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-18 02:01:12.915719 proteinTools-1.0.2/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.0.2/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 02:01:12.715826 proteinTools-1.0.2/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    47489 2023-04-18 01:59:27.000000 proteinTools-1.0.2/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.0.2/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 02:01:12.882815 proteinTools-1.0.2/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-18 02:01:12.000000 proteinTools-1.0.2/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-18 02:01:12.000000 proteinTools-1.0.2/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-18 02:01:12.000000 proteinTools-1.0.2/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       48 2023-04-18 02:01:12.000000 proteinTools-1.0.2/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-18 02:01:12.000000 proteinTools-1.0.2/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-18 02:01:12.926850 proteinTools-1.0.2/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      512 2023-04-18 02:00:52.000000 proteinTools-1.0.2/setup.py
```

### Comparing `proteinTools-1.0.1/LICENSE` & `proteinTools-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-1.0.1/proteinTools/PT.py` & `proteinTools-1.0.2/proteinTools/PT.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,16 +132,26 @@
         This method downloads the specific ligand structural file based on the ligand ID. 
     
         Parameters
         ----------
         arg1 : str
             Directory structural file will be downloaded in. Defaults to current user directory.
         """
-        url = 'https://files.rcsb.org/ligands/download/' + self.ID + '_ideal.sdf'
-        urllib.request.urlretrieve(url, directory + '/' + self.ID + '.sdf')
+        try:
+            url = 'https://files.rcsb.org/ligands/download/' + self.ID + '_ideal.sdf'
+            urllib.request.urlretrieve(url, directory + '/' + self.ID + '.sdf')
+        except: 
+            try:
+                pcp.download('SDF', self.ID + '.sdf' , self.ID, 'smiles', overwrite = True) 
+            except:
+                try:
+                    pcp.download('SDF', self.ID + '.sdf' , self.ID, 'inchikey', overwrite = True) 
+                except:
+                    print('Ligand identifier not found! File downloaded incorrectly')
+            
         
     @cached_property
     def center(self):
         """
         Ligand Center of Mass
     
         This property returns the center of mass of the ligand, which is generated from all atom components.
```

### Comparing `proteinTools-1.0.1/setup.py` & `proteinTools-1.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name = "proteinTools",
-    version = "1.0.1",
+    version = "1.0.2",
     author = "Christian de Frondeville",
     description = "Lightweight package which simplifies interacting with proteins.",
     long_description = long_description,
     packages = ["proteinTools"],
     install_requires=['pandas','urllib3','chembl-webresource-client','mygene']
 
 )
```

