# Comparing `tmp/proteinTools-1.0.4.tar.gz` & `tmp/proteinTools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-1.0.4.tar", last modified: Tue Apr 18 04:26:51 2023, max compression
+gzip compressed data, was "proteinTools-1.1.0.tar", last modified: Tue Apr 18 13:21:25 2023, max compression
```

## Comparing `proteinTools-1.0.4.tar` & `proteinTools-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 04:26:51.731310 proteinTools-1.0.4/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.0.4/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-18 04:26:51.727697 proteinTools-1.0.4/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.0.4/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 04:26:51.653099 proteinTools-1.0.4/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    47501 2023-04-18 04:26:43.000000 proteinTools-1.0.4/proteinTools/PT.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.0.4/proteinTools/__init__.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 04:26:51.712586 proteinTools-1.0.4/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-18 04:26:51.000000 proteinTools-1.0.4/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-18 04:26:51.000000 proteinTools-1.0.4/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-18 04:26:51.000000 proteinTools-1.0.4/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       48 2023-04-18 04:26:51.000000 proteinTools-1.0.4/proteinTools.egg-info/requires.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-18 04:26:51.000000 proteinTools-1.0.4/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-18 04:26:51.735853 proteinTools-1.0.4/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      512 2023-04-18 04:21:01.000000 proteinTools-1.0.4/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 13:21:25.883401 proteinTools-1.1.0/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.1.0/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-18 13:21:25.879541 proteinTools-1.1.0/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.1.0/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 13:21:25.802013 proteinTools-1.1.0/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    47864 2023-04-18 13:21:17.000000 proteinTools-1.1.0/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.1.0/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 13:21:25.860545 proteinTools-1.1.0/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-18 13:21:25.000000 proteinTools-1.1.0/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-18 13:21:25.000000 proteinTools-1.1.0/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-18 13:21:25.000000 proteinTools-1.1.0/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       48 2023-04-18 13:21:25.000000 proteinTools-1.1.0/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-18 13:21:25.000000 proteinTools-1.1.0/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-18 13:21:25.887610 proteinTools-1.1.0/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      512 2023-04-18 13:20:56.000000 proteinTools-1.1.0/setup.py
```

### Comparing `proteinTools-1.0.4/LICENSE` & `proteinTools-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-1.0.4/proteinTools/PT.py` & `proteinTools-1.1.0/proteinTools/PT.py`

 * *Files 1% similar despite different names*

```diff
@@ -427,29 +427,41 @@
                             element = element[:1]
                         atm = atom(element, float(line[30:38].strip()), float(line[38:47].strip()), float(line[47:56].strip()), data = line)
                         self.ligand_list[current_ligand_index].atoms.append(atm)
                      
                     #Queries secondary structure  
                     elif line[0:5] == 'SHEET':
                         line = [i for i in line.split(' ') if i != '']
-                        start = int(line[5])
-                        end = int(line[8])
-                        chain = int(line[4])
+                        try:
+                            start = int(line[5])
+                            end = int(line[8])
+                            chain = line[4]
+                        except:
+                            start = int(line[6])
+                            end = int(line[9])
+                            chain = line[5]
+                        
                         chainindex = chainkeys.index(chain)
                         for i in range(0, chainindex):
                             start += self.chains[chainkeys[i]]
                             end += self.chains[chainkeys[i]]
 
                         for i in range(start, end + 1):
                             sheet.append(i)
                     elif line[0:5] == 'HELIX':
                         line = [i for i in line.split(' ') if i != '']
-                        start = int(line[5])
-                        end = int(line[8])
-                        chain = line[4]
+                        try:
+                            start = int(line[5])
+                            end = int(line[8])
+                            chain = line[4]
+                        except:
+                            start = int(line[6])
+                            end = int(line[9])
+                            chain = line[5] 
+                     
                         chainindex = chainkeys.index(chain)
                         for i in range(0, chainindex):
                             start += self.chains[chainkeys[i]]
                             end += self.chains[chainkeys[i]]
                         for i in range(start, end + 1):
                             helix.append(i)
                             
@@ -1079,15 +1091,10 @@
     - Add secondary structure prediction to residues (use s4pred?)
     - Add more ID conversions
     '''
 
 '''
 #For unit testing    
 if __name__ == '__main__':
-    p = Protein('101m')
+    p = Protein('1E66')
     p.download()
-
-    #new = Protein(p.Uniprot)
-    #new.download()
-    #print(new.interactions)
-    #print(protein.interactions)
 '''
```

### Comparing `proteinTools-1.0.4/setup.py` & `proteinTools-1.1.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name = "proteinTools",
-    version = "1.0.4",
+    version = "1.1.0",
     author = "Christian de Frondeville",
     description = "Lightweight package which simplifies interacting with proteins.",
     long_description = long_description,
     packages = ["proteinTools"],
     install_requires=['pandas','urllib3','chembl-webresource-client','mygene']
 
 )
```

