# Comparing `tmp/pMTnet_Omni_Document-0.0.8.tar.gz` & `tmp/pMTnet_Omni_Document-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pMTnet_Omni_Document-0.0.8.tar", last modified: Mon Mar 13 23:47:32 2023, max compression
+gzip compressed data, was "pMTnet_Omni_Document-0.0.9.tar", last modified: Mon Mar 20 00:47:36 2023, max compression
```

## Comparing `pMTnet_Omni_Document-0.0.8.tar` & `pMTnet_Omni_Document-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 YuqiuYang   (504) staff       (20)        0 2023-03-13 23:47:32.691646 pMTnet_Omni_Document-0.0.8/
--rw-r--r--   0 YuqiuYang   (504) staff       (20)     1073 2023-02-09 23:42:34.000000 pMTnet_Omni_Document-0.0.8/LICENSE
--rw-r--r--   0 YuqiuYang   (504) staff       (20)     3903 2023-03-13 23:47:32.688583 pMTnet_Omni_Document-0.0.8/PKG-INFO
--rw-r--r--   0 YuqiuYang   (504) staff       (20)     3451 2023-02-13 22:31:44.000000 pMTnet_Omni_Document-0.0.8/README.md
-drwxr-xr-x   0 YuqiuYang   (504) staff       (20)        0 2023-03-13 23:47:32.633975 pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document/
--rw-r--r--   0 YuqiuYang   (504) staff       (20)      318 2023-03-13 23:45:11.000000 pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document/__init__.py
--rw-r--r--   0 YuqiuYang   (504) staff       (20)     2221 2023-03-13 23:21:25.000000 pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document/__main__.py
--rw-r--r--   0 YuqiuYang   (504) staff       (20)    27563 2023-03-13 23:46:28.000000 pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document/data_curation.py
-drwxr-xr-x   0 YuqiuYang   (504) staff       (20)        0 2023-03-13 23:47:32.652603 pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document/validation_data/
--rw-r--r--   0 YuqiuYang   (504) staff       (20)     5551 2023-03-03 23:50:40.000000 pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document/validation_data/human_alpha.txt
--rw-r--r--   0 YuqiuYang   (504) staff       (20)     7849 2023-03-03 23:50:40.000000 pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document/validation_data/human_beta.txt
--rw-r--r--   0 YuqiuYang   (504) staff       (20)    15374 2023-03-03 23:50:40.000000 pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document/validation_data/mouse_alpha.txt
--rw-r--r--   0 YuqiuYang   (504) staff       (20)     2568 2023-03-03 23:50:40.000000 pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document/validation_data/mouse_beta.txt
--rw-r--r--   0 YuqiuYang   (504) staff       (20)   189931 2023-03-03 23:40:11.000000 pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document/validation_data/valid_mhc.txt
-drwxr-xr-x   0 YuqiuYang   (504) staff       (20)        0 2023-03-13 23:47:32.641994 pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document.egg-info/
--rw-r--r--   0 YuqiuYang   (504) staff       (20)     3903 2023-03-13 23:47:32.000000 pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document.egg-info/PKG-INFO
--rw-r--r--   0 YuqiuYang   (504) staff       (20)      610 2023-03-13 23:47:32.000000 pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document.egg-info/SOURCES.txt
--rw-r--r--   0 YuqiuYang   (504) staff       (20)        1 2023-03-13 23:47:32.000000 pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document.egg-info/dependency_links.txt
--rw-r--r--   0 YuqiuYang   (504) staff       (20)       71 2023-03-13 23:47:32.000000 pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document.egg-info/requires.txt
--rw-r--r--   0 YuqiuYang   (504) staff       (20)       21 2023-03-13 23:47:32.000000 pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document.egg-info/top_level.txt
--rw-r--r--   0 YuqiuYang   (504) staff       (20)       38 2023-03-13 23:47:32.691871 pMTnet_Omni_Document-0.0.8/setup.cfg
--rw-r--r--   0 YuqiuYang   (504) staff       (20)     1765 2023-03-13 23:45:06.000000 pMTnet_Omni_Document-0.0.8/setup.py
+drwxr-xr-x   0 YuqiuYang   (504) staff       (20)        0 2023-03-20 00:47:36.473029 pMTnet_Omni_Document-0.0.9/
+-rw-r--r--   0 YuqiuYang   (504) staff       (20)     1073 2023-02-09 23:42:34.000000 pMTnet_Omni_Document-0.0.9/LICENSE
+-rw-r--r--   0 YuqiuYang   (504) staff       (20)     3903 2023-03-20 00:47:36.471538 pMTnet_Omni_Document-0.0.9/PKG-INFO
+-rw-r--r--   0 YuqiuYang   (504) staff       (20)     3451 2023-02-13 22:31:44.000000 pMTnet_Omni_Document-0.0.9/README.md
+drwxr-xr-x   0 YuqiuYang   (504) staff       (20)        0 2023-03-20 00:47:36.431491 pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document/
+-rw-r--r--   0 YuqiuYang   (504) staff       (20)      318 2023-03-20 00:47:20.000000 pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document/__init__.py
+-rw-r--r--   0 YuqiuYang   (504) staff       (20)     2221 2023-03-13 23:21:25.000000 pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document/__main__.py
+-rw-r--r--   0 YuqiuYang   (504) staff       (20)    27563 2023-03-19 23:48:48.000000 pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document/data_curation.py
+drwxr-xr-x   0 YuqiuYang   (504) staff       (20)        0 2023-03-20 00:47:36.467872 pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document/validation_data/
+-rw-r--r--   0 YuqiuYang   (504) staff       (20)     5551 2023-03-03 23:50:40.000000 pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document/validation_data/human_alpha.txt
+-rw-r--r--   0 YuqiuYang   (504) staff       (20)     7849 2023-03-03 23:50:40.000000 pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document/validation_data/human_beta.txt
+-rw-r--r--   0 YuqiuYang   (504) staff       (20)    15374 2023-03-03 23:50:40.000000 pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document/validation_data/mouse_alpha.txt
+-rw-r--r--   0 YuqiuYang   (504) staff       (20)     2568 2023-03-03 23:50:40.000000 pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document/validation_data/mouse_beta.txt
+-rw-r--r--   0 YuqiuYang   (504) staff       (20)   189931 2023-03-03 23:40:11.000000 pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document/validation_data/valid_mhc.txt
+drwxr-xr-x   0 YuqiuYang   (504) staff       (20)        0 2023-03-20 00:47:36.451375 pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document.egg-info/
+-rw-r--r--   0 YuqiuYang   (504) staff       (20)     3903 2023-03-20 00:47:36.000000 pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document.egg-info/PKG-INFO
+-rw-r--r--   0 YuqiuYang   (504) staff       (20)      610 2023-03-20 00:47:36.000000 pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document.egg-info/SOURCES.txt
+-rw-r--r--   0 YuqiuYang   (504) staff       (20)        1 2023-03-20 00:47:36.000000 pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document.egg-info/dependency_links.txt
+-rw-r--r--   0 YuqiuYang   (504) staff       (20)       71 2023-03-20 00:47:36.000000 pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document.egg-info/requires.txt
+-rw-r--r--   0 YuqiuYang   (504) staff       (20)       21 2023-03-20 00:47:36.000000 pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document.egg-info/top_level.txt
+-rw-r--r--   0 YuqiuYang   (504) staff       (20)       38 2023-03-20 00:47:36.473207 pMTnet_Omni_Document-0.0.9/setup.cfg
+-rw-r--r--   0 YuqiuYang   (504) staff       (20)     1765 2023-03-20 00:47:04.000000 pMTnet_Omni_Document-0.0.9/setup.py
```

### Comparing `pMTnet_Omni_Document-0.0.8/LICENSE` & `pMTnet_Omni_Document-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pMTnet_Omni_Document-0.0.8/PKG-INFO` & `pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pMTnet_Omni_Document
-Version: 0.0.8
+Name: pMTnet-Omni-Document
+Version: 0.0.9
 Summary: Document for pMTnet Omni
 Author: Yi Han, Yuqiu Yang, Tao Wang
 Author-email: yi.han@utsouthwestern.edu, yuqiuy@smu.edu, Tao.Wang@UTSouthwestern.edu
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.9
```

### Comparing `pMTnet_Omni_Document-0.0.8/README.md` & `pMTnet_Omni_Document-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document/__main__.py` & `pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document/__main__.py`

 * *Files identical despite different names*

### Comparing `pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document/data_curation.py` & `pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document/data_curation.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,33 +267,33 @@
         # the query result (which can be NaN). If not, we use the user seq.
         if va != '':
             human_df.at[i, 'vaseq'] = human_df.at[i, 'vaseq_ref']
         if vb != '':
             human_df.at[i, 'vbseq'] = human_df.at[i, 'vbseq_ref']
 
     human_df = human_df.drop(columns=['vaseq_ref', 'vbseq_ref']).fillna('')
-    invalid_human_df = human_df[(human_df['vaseq'] == '') |
+    invalid_human_df = human_df[(human_df['vaseq'] == '') &
                                 (human_df['vbseq'] == '')].reset_index(drop=True)
-    human_df = human_df[(human_df['vaseq'] != '') &
+    human_df = human_df[(human_df['vaseq'] != '') |
                         (human_df['vbseq'] != '')].reset_index(drop=True)
     print("\tQuerying mouse reference data\n")
     for i in tqdm(range(mouse_df.shape[0])):
         va = mouse_df.at[i, 'va']
         vb = mouse_df.at[i, 'vb']
         # If va/vb can be found we use the reference
         # Otherwise, we use the user input
         if va != '':
             mouse_df.at[i, 'vaseq'] = mouse_df.at[i, 'vaseq_ref']
         if vb != '':
             mouse_df.at[i, 'vbseq'] = mouse_df.at[i, 'vbseq_ref']
 
     mouse_df = mouse_df.drop(columns=['vaseq_ref', 'vbseq_ref']).fillna('')
-    invalid_mouse_df = mouse_df[(mouse_df['vaseq'] == '') |
+    invalid_mouse_df = mouse_df[(mouse_df['vaseq'] == '') &
                                 (mouse_df['vbseq'] == '')].reset_index(drop=True)
-    mouse_df = mouse_df[(mouse_df['vaseq'] != '') &
+    mouse_df = mouse_df[(mouse_df['vaseq'] != '') |
                         (mouse_df['vbseq'] != '')].reset_index(drop=True)
 
     df = pd.concat([human_df, mouse_df], axis=0,
                    ignore_index=True).reset_index(drop=True)
     invalid_df = pd.concat([invalid_human_df, invalid_mouse_df],
                            axis=0, ignore_index=True).reset_index(drop=True)
     return df, invalid_df
```

### Comparing `pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document/validation_data/human_alpha.txt` & `pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document/validation_data/human_alpha.txt`

 * *Files identical despite different names*

### Comparing `pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document/validation_data/human_beta.txt` & `pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document/validation_data/human_beta.txt`

 * *Files identical despite different names*

### Comparing `pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document/validation_data/mouse_alpha.txt` & `pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document/validation_data/mouse_alpha.txt`

 * *Files identical despite different names*

### Comparing `pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document/validation_data/mouse_beta.txt` & `pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document/validation_data/mouse_beta.txt`

 * *Files identical despite different names*

### Comparing `pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document/validation_data/valid_mhc.txt` & `pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document/validation_data/valid_mhc.txt`

 * *Files identical despite different names*

### Comparing `pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document.egg-info/PKG-INFO` & `pMTnet_Omni_Document-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pMTnet-Omni-Document
-Version: 0.0.8
+Name: pMTnet_Omni_Document
+Version: 0.0.9
 Summary: Document for pMTnet Omni
 Author: Yi Han, Yuqiu Yang, Tao Wang
 Author-email: yi.han@utsouthwestern.edu, yuqiuy@smu.edu, Tao.Wang@UTSouthwestern.edu
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.9
```

### Comparing `pMTnet_Omni_Document-0.0.8/pMTnet_Omni_Document.egg-info/SOURCES.txt` & `pMTnet_Omni_Document-0.0.9/pMTnet_Omni_Document.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pMTnet_Omni_Document-0.0.8/setup.py` & `pMTnet_Omni_Document-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup 
 import sys 
 import os 
 import shutil
 import distutils.cmd
 
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 
 class PypiCommand(distutils.cmd.Command):
     
     description = "Build and upload for PyPI."
     user_options = []
     
     def initialize_options(self):
```

