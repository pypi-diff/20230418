# Comparing `tmp/proteinTools-1.0.2.tar.gz` & `tmp/proteinTools-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-1.0.2.tar", last modified: Tue Apr 18 02:01:13 2023, max compression
+gzip compressed data, was "proteinTools-1.0.3.tar", last modified: Tue Apr 18 04:15:54 2023, max compression
```

## Comparing `proteinTools-1.0.2.tar` & `proteinTools-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 02:01:12.920702 proteinTools-1.0.2/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.0.2/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-18 02:01:12.915719 proteinTools-1.0.2/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.0.2/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 02:01:12.715826 proteinTools-1.0.2/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    47489 2023-04-18 01:59:27.000000 proteinTools-1.0.2/proteinTools/PT.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.0.2/proteinTools/__init__.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 02:01:12.882815 proteinTools-1.0.2/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-18 02:01:12.000000 proteinTools-1.0.2/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-18 02:01:12.000000 proteinTools-1.0.2/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-18 02:01:12.000000 proteinTools-1.0.2/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       48 2023-04-18 02:01:12.000000 proteinTools-1.0.2/proteinTools.egg-info/requires.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-18 02:01:12.000000 proteinTools-1.0.2/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-18 02:01:12.926850 proteinTools-1.0.2/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      512 2023-04-18 02:00:52.000000 proteinTools-1.0.2/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 04:15:54.578052 proteinTools-1.0.3/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.0.3/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-18 04:15:54.575267 proteinTools-1.0.3/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.0.3/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 04:15:54.492921 proteinTools-1.0.3/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    47548 2023-04-18 04:15:11.000000 proteinTools-1.0.3/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.0.3/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 04:15:54.556880 proteinTools-1.0.3/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-18 04:15:54.000000 proteinTools-1.0.3/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-18 04:15:54.000000 proteinTools-1.0.3/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-18 04:15:54.000000 proteinTools-1.0.3/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       48 2023-04-18 04:15:54.000000 proteinTools-1.0.3/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-18 04:15:54.000000 proteinTools-1.0.3/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-18 04:15:54.586537 proteinTools-1.0.3/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      512 2023-04-18 04:15:39.000000 proteinTools-1.0.3/setup.py
```

### Comparing `proteinTools-1.0.2/LICENSE` & `proteinTools-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-1.0.2/proteinTools/PT.py` & `proteinTools-1.0.3/proteinTools/PT.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from io import StringIO
 from chembl_webresource_client.new_client import new_client
 import re
 mg = mygene.MyGeneInfo()
 
 #Utility dictionaries containing element/mass mappings as well as FASTA mapping
 FASTAdict = {'ALA':'A', 'ALX':'B', 'CYS': 'C', 'ASP' : 'D', 'GLU': 'E', 'PHE': 'F', 'GLY': 'G', 'HIS': 'H', 'ILE': 'I', 'LYS':'K', 'LEU':'L', 'MET': 'M', 'ASN':'N', 'PRO':'P', 'GLN': 'Q', 'ARG':'R', 'SER': 'S', 'THR': 'T', 'VAL': 'V', 'TRP': 'W', 'UNK':'X', 'TYR':'Y', 'GLX':'Z'}
-atom_dict = {'H':1.01, 'C':12.01, 'O':16.00, 'N':14.01, 'P':30.97, 'F':18.998, 'S':32.06, 'B':10.81, 'K':39.1, 'I':126.904, 'BR':79.904, 'CL':35.453, 'CA':40.08, 'NA':22.99, 'MG':24.305, 'AL':26.98, 'CR':51.996, 'NE':20.179, 'BE':9.01, 'FE':55.847, 'CO':58.933,'AG':107.868, 'CD':112.41, 'NI':58.693, 'ZN':65.39, 'BE':9.0122, 'IN':114.818, 'SI':28.085, 'SC':44.956, 'TI':47.867, 'V':50.941, 'MN':54.938, 'CU':63.546, 'GA':59.723, 'GE':72.64, 'SE':78.96, 'KR':83.8, 'ZR':91.224, 'NB':92.906, 'PD':106.42, 'SN':118.71, 'SB':121.76, 'XE':131.293, 'BA':137.327, 'LA':138.91, 'LI':6.941, 'HG':200.59, 'PB':207.2, 'BI':208.98, 'PO':209, 'TI':204.3833, 'AU':196.9665, 'IR':192.217, 'PT':195.078, 'RE':186.207, 'W':183.84, 'TA':180.948, 'YB':173.04, 'EU':151.964, 'ND':144.25, 'CE':140.116, 'TH':232.04, 'U':238.029, 'PU':244, 'FR':223, 'PA':231.04, 'HO':164.93, 'SM':150.36, 'PR':140.908, 'TE':127.6, 'TC':98, 'Y':88.906}
+atom_dict = {'H':1.01, 'C':12.01, 'O':16.00, 'N':14.01, 'P':30.97, 'F':18.998, 'FE':55.845, 'S':32.06, 'B':10.81, 'K':39.1, 'I':126.904, 'BR':79.904, 'CL':35.453, 'CA':40.08, 'NA':22.99, 'MG':24.305, 'AL':26.98, 'CR':51.996, 'NE':20.179, 'BE':9.01, 'FE':55.847, 'CO':58.933,'AG':107.868, 'CD':112.41, 'NI':58.693, 'ZN':65.39, 'BE':9.0122, 'IN':114.818, 'SI':28.085, 'SC':44.956, 'TI':47.867, 'V':50.941, 'MN':54.938, 'CU':63.546, 'GA':59.723, 'GE':72.64, 'SE':78.96, 'KR':83.8, 'ZR':91.224, 'NB':92.906, 'PD':106.42, 'SN':118.71, 'SB':121.76, 'XE':131.293, 'BA':137.327, 'LA':138.91, 'LI':6.941, 'HG':200.59, 'PB':207.2, 'BI':208.98, 'PO':209, 'TI':204.3833, 'AU':196.9665, 'IR':192.217, 'PT':195.078, 'RE':186.207, 'W':183.84, 'TA':180.948, 'YB':173.04, 'EU':151.964, 'ND':144.25, 'CE':140.116, 'TH':232.04, 'U':238.029, 'PU':244, 'FR':223, 'PA':231.04, 'HO':164.93, 'SM':150.36, 'PR':140.908, 'TE':127.6, 'TC':98, 'Y':88.906}
 atom_keys = atom_dict.keys()
 
 class atom:
     """
     Atom class
 
     This class contains the essential parameters of an individual atom in a protein structural file, including the coordinates, element, atomic mass, parent residue, and line data.
@@ -419,14 +419,16 @@
                             lignum = int(line[22:27])
                             if lignum != currnum:
                                 currnum = lignum
                                 lig = ligand(ligands)
                                 self.ligand_list.append(lig)
                                 current_ligand_index += 1
                             element = line[77:79].strip()
+                        print(line)
+                        print(element)
                         if element not in atom_keys:
                             element = element[:1]
                         atm = atom(element, float(line[30:38].strip()), float(line[38:47].strip()), float(line[47:56].strip()), data = line)
                         self.ligand_list[current_ligand_index].atoms.append(atm)
                      
                     #Queries secondary structure  
                     elif line[0:5] == 'SHEET':
@@ -1076,18 +1078,17 @@
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
-    p = Protein('1HK4')
+    p = Protein('101m')
     p.download()
-    print(p[1].structure)
+
     #new = Protein(p.Uniprot)
     #new.download()
     #print(new.interactions)
     #print(protein.interactions)
-'''
```

### Comparing `proteinTools-1.0.2/setup.py` & `proteinTools-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name = "proteinTools",
-    version = "1.0.2",
+    version = "1.0.3",
     author = "Christian de Frondeville",
     description = "Lightweight package which simplifies interacting with proteins.",
     long_description = long_description,
     packages = ["proteinTools"],
     install_requires=['pandas','urllib3','chembl-webresource-client','mygene']
 
 )
```

