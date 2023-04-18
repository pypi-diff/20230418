# Comparing `tmp/wwpdb.utils.config-0.6.tar.gz` & `tmp/wwpdb.utils.config-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wwpdb.utils.config-0.6.tar", last modified: Thu Feb 21 12:13:08 2019, max compression
+gzip compressed data, was "dist/wwpdb.utils.config-0.7.tar", last modified: Sat Apr 20 13:15:44 2019, max compression
```

## Comparing `wwpdb.utils.config-0.6.tar` & `wwpdb.utils.config-0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 peisach    (501) staff       (20)        0 2019-02-21 12:13:08.000000 wwpdb.utils.config-0.6/
--rw-r--r--   0 peisach    (501) staff       (20)      758 2019-02-21 12:13:08.000000 wwpdb.utils.config-0.6/PKG-INFO
--rw-r--r--   0 peisach    (501) staff       (20)      496 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.6/README.md
--rw-r--r--   0 peisach    (501) staff       (20)      108 2019-02-21 12:13:08.000000 wwpdb.utils.config-0.6/setup.cfg
--rwxr-xr-x   0 peisach    (501) staff       (20)     2350 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.6/setup.py
-drwxr-xr-x   0 peisach    (501) staff       (20)        0 2019-02-21 12:13:08.000000 wwpdb.utils.config-0.6/wwpdb/
--rw-r--r--   0 peisach    (501) staff       (20)       65 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.6/wwpdb/__init__.py
-drwxr-xr-x   0 peisach    (501) staff       (20)        0 2019-02-21 12:13:08.000000 wwpdb.utils.config-0.6/wwpdb/utils/
--rw-r--r--   0 peisach    (501) staff       (20)       65 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.6/wwpdb/utils/__init__.py
-drwxr-xr-x   0 peisach    (501) staff       (20)        0 2019-02-21 12:13:08.000000 wwpdb.utils.config-0.6/wwpdb/utils/config/
--rw-r--r--   0 peisach    (501) staff       (20)     2699 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.6/wwpdb/utils/config/ConfigInfo.py
--rw-r--r--   0 peisach    (501) staff       (20)    42263 2019-02-21 12:10:12.000000 wwpdb.utils.config-0.6/wwpdb/utils/config/ConfigInfoData.py
--rw-r--r--   0 peisach    (501) staff       (20)     9398 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.6/wwpdb/utils/config/ConfigInfoDataSet.py
--rw-r--r--   0 peisach    (501) staff       (20)     6059 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.6/wwpdb/utils/config/ConfigInfoDataSetExec.py
--rw-r--r--   0 peisach    (501) staff       (20)     7707 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.6/wwpdb/utils/config/ConfigInfoFallBack.py
--rw-r--r--   0 peisach    (501) staff       (20)    20525 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.6/wwpdb/utils/config/ConfigInfoFile.py
--rw-r--r--   0 peisach    (501) staff       (20)    27429 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.6/wwpdb/utils/config/ConfigInfoFileExec.py
--rw-r--r--   0 peisach    (501) staff       (20)     2855 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.6/wwpdb/utils/config/ConfigInfoGroupDataSet.py
--rw-r--r--   0 peisach    (501) staff       (20)    27780 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.6/wwpdb/utils/config/ConfigInfoShellExec.py
--rw-r--r--   0 peisach    (501) staff       (20)     6929 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.6/wwpdb/utils/config/ConfigInfoSiteAccess.py
--rw-r--r--   0 peisach    (501) staff       (20)      154 2019-02-21 12:06:42.000000 wwpdb.utils.config-0.6/wwpdb/utils/config/__init__.py
-drwxr-xr-x   0 peisach    (501) staff       (20)        0 2019-02-21 12:13:08.000000 wwpdb.utils.config-0.6/wwpdb.utils.config.egg-info/
--rw-r--r--   0 peisach    (501) staff       (20)      758 2019-02-21 12:13:08.000000 wwpdb.utils.config-0.6/wwpdb.utils.config.egg-info/PKG-INFO
--rw-r--r--   0 peisach    (501) staff       (20)      799 2019-02-21 12:13:08.000000 wwpdb.utils.config-0.6/wwpdb.utils.config.egg-info/SOURCES.txt
--rw-r--r--   0 peisach    (501) staff       (20)        1 2019-02-21 12:13:08.000000 wwpdb.utils.config-0.6/wwpdb.utils.config.egg-info/dependency_links.txt
--rw-r--r--   0 peisach    (501) staff       (20)      153 2019-02-21 12:13:08.000000 wwpdb.utils.config-0.6/wwpdb.utils.config.egg-info/entry_points.txt
--rw-r--r--   0 peisach    (501) staff       (20)        1 2019-02-05 03:16:38.000000 wwpdb.utils.config-0.6/wwpdb.utils.config.egg-info/not-zip-safe
--rw-r--r--   0 peisach    (501) staff       (20)       72 2019-02-21 12:13:08.000000 wwpdb.utils.config-0.6/wwpdb.utils.config.egg-info/requires.txt
--rw-r--r--   0 peisach    (501) staff       (20)        6 2019-02-21 12:13:08.000000 wwpdb.utils.config-0.6/wwpdb.utils.config.egg-info/top_level.txt
+drwxr-xr-x   0 peisach    (501) staff       (20)        0 2019-04-20 13:15:44.000000 wwpdb.utils.config-0.7/
+drwxr-xr-x   0 peisach    (501) staff       (20)        0 2019-04-20 13:15:44.000000 wwpdb.utils.config-0.7/wwpdb.utils.config.egg-info/
+-rw-r--r--   0 peisach    (501) staff       (20)      758 2019-04-20 13:15:44.000000 wwpdb.utils.config-0.7/wwpdb.utils.config.egg-info/PKG-INFO
+-rw-r--r--   0 peisach    (501) staff       (20)        1 2019-02-05 03:16:38.000000 wwpdb.utils.config-0.7/wwpdb.utils.config.egg-info/not-zip-safe
+-rw-r--r--   0 peisach    (501) staff       (20)      799 2019-04-20 13:15:44.000000 wwpdb.utils.config-0.7/wwpdb.utils.config.egg-info/SOURCES.txt
+-rw-r--r--   0 peisach    (501) staff       (20)      153 2019-04-20 13:15:44.000000 wwpdb.utils.config-0.7/wwpdb.utils.config.egg-info/entry_points.txt
+-rw-r--r--   0 peisach    (501) staff       (20)       72 2019-04-20 13:15:44.000000 wwpdb.utils.config-0.7/wwpdb.utils.config.egg-info/requires.txt
+-rw-r--r--   0 peisach    (501) staff       (20)        6 2019-04-20 13:15:44.000000 wwpdb.utils.config-0.7/wwpdb.utils.config.egg-info/top_level.txt
+-rw-r--r--   0 peisach    (501) staff       (20)        1 2019-04-20 13:15:44.000000 wwpdb.utils.config-0.7/wwpdb.utils.config.egg-info/dependency_links.txt
+-rw-r--r--   0 peisach    (501) staff       (20)      758 2019-04-20 13:15:44.000000 wwpdb.utils.config-0.7/PKG-INFO
+drwxr-xr-x   0 peisach    (501) staff       (20)        0 2019-04-20 13:15:44.000000 wwpdb.utils.config-0.7/wwpdb/
+-rw-r--r--   0 peisach    (501) staff       (20)       65 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.7/wwpdb/__init__.py
+drwxr-xr-x   0 peisach    (501) staff       (20)        0 2019-04-20 13:15:44.000000 wwpdb.utils.config-0.7/wwpdb/utils/
+drwxr-xr-x   0 peisach    (501) staff       (20)        0 2019-04-20 13:15:44.000000 wwpdb.utils.config-0.7/wwpdb/utils/config/
+-rw-r--r--   0 peisach    (501) staff       (20)    27429 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.7/wwpdb/utils/config/ConfigInfoFileExec.py
+-rw-r--r--   0 peisach    (501) staff       (20)     2699 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.7/wwpdb/utils/config/ConfigInfo.py
+-rw-r--r--   0 peisach    (501) staff       (20)    27780 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.7/wwpdb/utils/config/ConfigInfoShellExec.py
+-rw-r--r--   0 peisach    (501) staff       (20)     9398 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.7/wwpdb/utils/config/ConfigInfoDataSet.py
+-rw-r--r--   0 peisach    (501) staff       (20)      154 2019-04-20 13:12:31.000000 wwpdb.utils.config-0.7/wwpdb/utils/config/__init__.py
+-rw-r--r--   0 peisach    (501) staff       (20)    20525 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.7/wwpdb/utils/config/ConfigInfoFile.py
+-rw-r--r--   0 peisach    (501) staff       (20)     7707 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.7/wwpdb/utils/config/ConfigInfoFallBack.py
+-rw-r--r--   0 peisach    (501) staff       (20)     6059 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.7/wwpdb/utils/config/ConfigInfoDataSetExec.py
+-rw-r--r--   0 peisach    (501) staff       (20)     2855 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.7/wwpdb/utils/config/ConfigInfoGroupDataSet.py
+-rw-r--r--   0 peisach    (501) staff       (20)     6929 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.7/wwpdb/utils/config/ConfigInfoSiteAccess.py
+-rw-r--r--   0 peisach    (501) staff       (20)    42358 2019-04-20 13:01:13.000000 wwpdb.utils.config-0.7/wwpdb/utils/config/ConfigInfoData.py
+-rw-r--r--   0 peisach    (501) staff       (20)       65 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.7/wwpdb/utils/__init__.py
+-rw-r--r--   0 peisach    (501) staff       (20)      496 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.7/README.md
+-rwxr-xr-x   0 peisach    (501) staff       (20)     2350 2019-01-21 01:33:36.000000 wwpdb.utils.config-0.7/setup.py
+-rw-r--r--   0 peisach    (501) staff       (20)      108 2019-04-20 13:15:44.000000 wwpdb.utils.config-0.7/setup.cfg
```

### Comparing `wwpdb.utils.config-0.6/PKG-INFO` & `wwpdb.utils.config-0.7/wwpdb.utils.config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.config
-Version: 0.6
+Version: 0.7
 Summary: wwPDB Python Configuration Parsing
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Description: See:  README.md
 Platform: UNKNOWN
@@ -13,9 +13,9 @@
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: dev
```

### Comparing `wwpdb.utils.config-0.6/setup.py` & `wwpdb.utils.config-0.7/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.config-0.6/wwpdb/utils/config/ConfigInfo.py` & `wwpdb.utils.config-0.7/wwpdb/utils/config/ConfigInfo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.config-0.6/wwpdb/utils/config/ConfigInfoData.py` & `wwpdb.utils.config-0.7/wwpdb/utils/config/ConfigInfoData.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,14 +459,15 @@
                                    'WWPDB_DEPLOY_PRODUCTION_UCSD': 'https://deposit-rcsb-west.wwpdb.org/deposition',
                                    'WWPDB_DEPLOY_BETA_RU': 'https://onedep-beta-dep-1.rcsb.rutgers.edu',
                                    'WWPDB_DEPLOY_PRODUCTION_PDBJ': 'https://deposit-pdbj.wwpdb.org/deposition',
                                    'PDBE_PROD': 'https://deposit-pdbe.wwpdb.org/deposition',
                                    'PDBE_LEGACY': 'https://deposit-pdbe.wwpdb.org/deposition',
                                    'PDBE_STG': 'https://wwwdev.ebi.ac.uk/pdbe-da-staging/deposition',
                                    'PDBE_DEV': 'https://wwwdev.ebi.ac.uk/pdbe-da/deposition',
+                                   'PDBE_VAL': 'https://validate-pdbe.wwpdb.org/validservice',
                                    #'PDBE_DEV': 'https://dev.pdbe.org/deposition',
                                    'WWPDB_DEPLOY_ALPHA_RU': 'https://da-dep-alpha-0.rcsb.rutgers.edu/deposition',
                                    'WWPDB_DEPLOY_TEST_RU': 'https://wwpdb-deploy-test-1.wwpdb.org/deposition',
                                    'WWPDB_DEPLOY_VALSRV2_RU': 'https://validate-rcsb-1.wwpdb.org/validservice',
                                    'WWPDB_DEPLOY_VALSRV2_UCSD': 'https://validate-rcsb-3.wwpdb.org/validservice',
                                    }
     """Dictionary of well known project deposition service entry points"""
```

### Comparing `wwpdb.utils.config-0.6/wwpdb/utils/config/ConfigInfoDataSet.py` & `wwpdb.utils.config-0.7/wwpdb/utils/config/ConfigInfoDataSet.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.config-0.6/wwpdb/utils/config/ConfigInfoDataSetExec.py` & `wwpdb.utils.config-0.7/wwpdb/utils/config/ConfigInfoDataSetExec.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.config-0.6/wwpdb/utils/config/ConfigInfoFallBack.py` & `wwpdb.utils.config-0.7/wwpdb/utils/config/ConfigInfoFallBack.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.config-0.6/wwpdb/utils/config/ConfigInfoFile.py` & `wwpdb.utils.config-0.7/wwpdb/utils/config/ConfigInfoFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.config-0.6/wwpdb/utils/config/ConfigInfoFileExec.py` & `wwpdb.utils.config-0.7/wwpdb/utils/config/ConfigInfoFileExec.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.config-0.6/wwpdb/utils/config/ConfigInfoGroupDataSet.py` & `wwpdb.utils.config-0.7/wwpdb/utils/config/ConfigInfoGroupDataSet.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.config-0.6/wwpdb/utils/config/ConfigInfoShellExec.py` & `wwpdb.utils.config-0.7/wwpdb/utils/config/ConfigInfoShellExec.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.config-0.6/wwpdb/utils/config/ConfigInfoSiteAccess.py` & `wwpdb.utils.config-0.7/wwpdb/utils/config/ConfigInfoSiteAccess.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.config-0.6/wwpdb.utils.config.egg-info/PKG-INFO` & `wwpdb.utils.config-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.config
-Version: 0.6
+Version: 0.7
 Summary: wwPDB Python Configuration Parsing
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Description: See:  README.md
 Platform: UNKNOWN
@@ -13,9 +13,9 @@
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: dev
```

### Comparing `wwpdb.utils.config-0.6/wwpdb.utils.config.egg-info/SOURCES.txt` & `wwpdb.utils.config-0.7/wwpdb.utils.config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

