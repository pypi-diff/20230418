# Comparing `tmp/proteinTools-1.1.2.tar.gz` & `tmp/proteinTools-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-1.1.2.tar", last modified: Tue Apr 18 14:33:54 2023, max compression
+gzip compressed data, was "proteinTools-1.1.3.tar", last modified: Tue Apr 18 17:50:58 2023, max compression
```

## Comparing `proteinTools-1.1.2.tar` & `proteinTools-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 14:33:54.383721 proteinTools-1.1.2/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.1.2/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-18 14:33:54.380275 proteinTools-1.1.2/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.1.2/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 14:33:54.312622 proteinTools-1.1.2/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    48978 2023-04-18 14:33:39.000000 proteinTools-1.1.2/proteinTools/PT.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.1.2/proteinTools/__init__.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 14:33:54.368038 proteinTools-1.1.2/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-18 14:33:54.000000 proteinTools-1.1.2/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-18 14:33:54.000000 proteinTools-1.1.2/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-18 14:33:54.000000 proteinTools-1.1.2/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-18 14:33:54.000000 proteinTools-1.1.2/proteinTools.egg-info/requires.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-18 14:33:54.000000 proteinTools-1.1.2/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-18 14:33:54.388338 proteinTools-1.1.2/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      525 2023-04-18 14:32:27.000000 proteinTools-1.1.2/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 17:50:58.445222 proteinTools-1.1.3/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.1.3/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-18 17:50:58.437785 proteinTools-1.1.3/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.1.3/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 17:50:58.353604 proteinTools-1.1.3/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    49003 2023-04-18 17:50:02.000000 proteinTools-1.1.3/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.1.3/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 17:50:58.421396 proteinTools-1.1.3/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-18 17:50:58.000000 proteinTools-1.1.3/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-18 17:50:58.000000 proteinTools-1.1.3/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-18 17:50:58.000000 proteinTools-1.1.3/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-18 17:50:58.000000 proteinTools-1.1.3/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-18 17:50:58.000000 proteinTools-1.1.3/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-18 17:50:58.457193 proteinTools-1.1.3/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      523 2023-04-18 17:50:11.000000 proteinTools-1.1.3/setup.py
```

### Comparing `proteinTools-1.1.2/LICENSE` & `proteinTools-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-1.1.2/proteinTools/PT.py` & `proteinTools-1.1.3/proteinTools/PT.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,14 +395,15 @@
                             continue
                     os.rename(alphaname, protname)
                     self.cif = True
                 except:
                     print(self.protein + ' not found in any libraries!')
         
         #Atomizes protein file
+        os.chdir(destination)
         if self.cif == False:
             with open(self.protein + '.pdb', 'r') as f:
                 data = f.readlines()
             self.residue_list, curr_residue, curr_lig, currnum, curr_chain = [], -1, '', 0, ''
             if self.ID_type == 'PDB':
                 current_ligand_index, self.ligand_list = -1, []
             for count, line in enumerate(data):
@@ -1107,14 +1108,14 @@
             return 'N/A'
     '''
     TODO
     - Add secondary structure prediction to residues (use s4pred?)
     - Add more ID conversions
     '''
 
-'''
+
 #For unit testing    
 if __name__ == '__main__':
     p = Protein('1E66')
     lig = ligand('C1=CC=C(C=C1)C=O')
     lig.download()
-''' 
+
```

### Comparing `proteinTools-1.1.2/setup.py` & `proteinTools-1.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name = "proteinTools",
-    version = "1.1.2",
+    version = "1.1.3",
     author = "Christian de Frondeville",
     description = "Lightweight package which simplifies interacting with proteins.",
     long_description = long_description,
     packages = ["proteinTools"],
     install_requires=['pandas','urllib3','chembl-webresource-client','mygene', 'pubchempy']
-
 )
```

