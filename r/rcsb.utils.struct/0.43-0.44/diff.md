# Comparing `tmp/rcsb.utils.struct-0.43.tar.gz` & `tmp/rcsb.utils.struct-0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.struct-0.43.tar", last modified: Mon Jan  9 17:39:49 2023, max compression
+gzip compressed data, was "rcsb.utils.struct-0.44.tar", last modified: Tue Apr 18 21:10:14 2023, max compression
```

## Comparing `rcsb.utils.struct-0.43.tar` & `rcsb.utils.struct-0.44.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-09 17:39:48.998690 rcsb.utils.struct-0.43/
--rw-r--r--   0 vsts      (1001) docker     (122)     2424 2023-01-09 17:37:56.000000 rcsb.utils.struct-0.43/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-01-09 17:37:56.000000 rcsb.utils.struct-0.43/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-01-09 17:37:56.000000 rcsb.utils.struct-0.43/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1804 2023-01-09 17:39:48.998690 rcsb.utils.struct-0.43/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1006 2023-01-09 17:37:56.000000 rcsb.utils.struct-0.43/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-09 17:39:48.998690 rcsb.utils.struct-0.43/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-01-09 17:37:56.000000 rcsb.utils.struct-0.43/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-09 17:39:48.998690 rcsb.utils.struct-0.43/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-01-09 17:37:56.000000 rcsb.utils.struct-0.43/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-09 17:39:48.998690 rcsb.utils.struct-0.43/rcsb/utils/struct/
--rw-r--r--   0 vsts      (1001) docker     (122)    12976 2023-01-09 17:37:56.000000 rcsb.utils.struct-0.43/rcsb/utils/struct/CathClassificationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15599 2023-01-09 17:37:56.000000 rcsb.utils.struct-0.43/rcsb/utils/struct/EcodClassificationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3191 2023-01-09 17:37:56.000000 rcsb.utils.struct-0.43/rcsb/utils/struct/EntryInfoProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    20499 2023-01-09 17:37:56.000000 rcsb.utils.struct-0.43/rcsb/utils/struct/Scop2ClassificationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16717 2023-01-09 17:37:56.000000 rcsb.utils.struct-0.43/rcsb/utils/struct/ScopClassificationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)      154 2023-01-09 17:37:56.000000 rcsb.utils.struct-0.43/rcsb/utils/struct/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-09 17:39:48.998690 rcsb.utils.struct-0.43/rcsb.utils.struct.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1804 2023-01-09 17:39:48.000000 rcsb.utils.struct-0.43/rcsb.utils.struct.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      623 2023-01-09 17:39:48.000000 rcsb.utils.struct-0.43/rcsb.utils.struct.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-01-09 17:39:48.000000 rcsb.utils.struct-0.43/rcsb.utils.struct.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-01-09 17:38:32.000000 rcsb.utils.struct-0.43/rcsb.utils.struct.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-01-09 17:39:48.000000 rcsb.utils.struct-0.43/rcsb.utils.struct.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-01-09 17:39:48.000000 rcsb.utils.struct-0.43/rcsb.utils.struct.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-01-09 17:37:56.000000 rcsb.utils.struct-0.43/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-01-09 17:39:48.998690 rcsb.utils.struct-0.43/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2325 2023-01-09 17:37:56.000000 rcsb.utils.struct-0.43/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 21:10:14.009454 rcsb.utils.struct-0.44/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2496 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1804 2023-04-18 21:10:14.009454 rcsb.utils.struct-0.44/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1006 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 21:10:14.005454 rcsb.utils.struct-0.44/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 21:10:14.005454 rcsb.utils.struct-0.44/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 21:10:14.009454 rcsb.utils.struct-0.44/rcsb/utils/struct/
+-rw-r--r--   0 vsts      (1001) docker     (122)    12976 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/rcsb/utils/struct/CathClassificationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15694 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/rcsb/utils/struct/EcodClassificationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3191 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/rcsb/utils/struct/EntryInfoProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    20575 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/rcsb/utils/struct/Scop2ClassificationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16717 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/rcsb/utils/struct/ScopClassificationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      154 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/rcsb/utils/struct/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 21:10:14.005454 rcsb.utils.struct-0.44/rcsb.utils.struct.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1804 2023-04-18 21:10:13.000000 rcsb.utils.struct-0.44/rcsb.utils.struct.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      623 2023-04-18 21:10:13.000000 rcsb.utils.struct-0.44/rcsb.utils.struct.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-18 21:10:13.000000 rcsb.utils.struct-0.44/rcsb.utils.struct.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-18 21:09:04.000000 rcsb.utils.struct-0.44/rcsb.utils.struct.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-04-18 21:10:13.000000 rcsb.utils.struct-0.44/rcsb.utils.struct.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-04-18 21:10:13.000000 rcsb.utils.struct-0.44/rcsb.utils.struct.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-04-18 21:10:14.009454 rcsb.utils.struct-0.44/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2325 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/setup.py
```

### Comparing `rcsb.utils.struct-0.43/HISTORY.txt` & `rcsb.utils.struct-0.44/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,8 +29,9 @@
  23-Aug-2021    V0.36 Adjustments to ECOD lineage construction for unnamed nodes
  10-Sep-2021    V0.37 Separate protein type and structural class in tree representation.
  22-Sep-2021    V0.38 Add module EntryInfoProvider and associated tests (accessor methods only)
  23-Sep-2021    V0.39 Update SCOP version and path details
  16-Nov-2021    V0.40 Append additional ECOD annotations for given entryId and chainId instead of overwriting
  24-Feb-2022    V0.41 Resolve duplication issues with Scop2 tree node list, and fix parent ID lists for nodes with multiple parents
   9-Mar-2022    V0.42 Fix issue related to V0.41 update to Scop2 provider
-  6-Jan-2023    V0.43 Configuration changes to support tox 4
+  6-Jan-2023    V0.43 Configuration changes to support tox 4
+ 18-Apr-2023    V0.44 Fix Ecod and Scop2 provider fall-back file import
```

### Comparing `rcsb.utils.struct-0.43/LICENSE` & `rcsb.utils.struct-0.44/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.struct-0.43/PKG-INFO` & `rcsb.utils.struct-0.44/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.struct
-Version: 0.43
+Version: 0.44
 Summary: RCSB Python utility classes for accessing PDB primary structure data and features associated with these data
 Home-page: https://github.com/rcsb/py-rcsb_utils_seq
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.struct-0.43/README.md` & `rcsb.utils.struct-0.44/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.struct-0.43/rcsb/utils/struct/CathClassificationProvider.py` & `rcsb.utils.struct-0.44/rcsb/utils/struct/CathClassificationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.struct-0.43/rcsb/utils/struct/EcodClassificationProvider.py` & `rcsb.utils.struct-0.44/rcsb/utils/struct/EcodClassificationProvider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ##
 #  File:  EcodClassificationProvider.py
 #  Date:  3-Apr-2019 jdw
 #
 #  Updates:
 #  16-Nov-2021 dwp Append additional ecod annotations for given entryId and chainId instead of overwriting
+#  18-Apr-2023 aae Get version from data list directly rather than opening file twice
 #
 ##
 """
   Extract ECOD domain assignments, term descriptions and ECOD classification hierarchy
   from ECOD flat files.
 
 """
@@ -182,26 +183,26 @@
 
     def __fetchFromSource(self, urlTarget):
         """Fetch the classification names and domain assignments from the ECOD repo."""
         fU = FileUtil()
         fn = fU.getFileName(urlTarget)
         fp = os.path.join(self.__dirPath, fn)
         if not fU.exists(fp):
-            fU.get(urlTarget, fp)
+            ok = fU.get(urlTarget, fp)
+            if not ok:
+                return None
         #
-        with open(fp, "r", encoding="utf-8") as ifh:
-            line = ifh.readline()
-            line = ifh.readline()
-            line = ifh.readline()
-            ff = line[:-1].split()
-            self.__version = ff[-1]
-        #
-        nmL = self.__mU.doImport(fp, fmt="list", uncomment=True)
+        nmL = self.__mU.doImport(fp, fmt="list", uncomment=False)
         fU.remove(fp)
         #
+        # Get the version and remove commented lines
+        ff = nmL[2].split()
+        self.__version = ff[-1]
+        nmL = [line for line in nmL if not line.startswith("#")]
+        #
         return nmL
 
     def __extractDomainHierarchy(self, nmL):
         """
         #/data/ecod/database_versions/v280/ecod.develop280.domains.txt
         #ECOD version develop280
         #Domain list version 1.6
```

### Comparing `rcsb.utils.struct-0.43/rcsb/utils/struct/EntryInfoProvider.py` & `rcsb.utils.struct-0.44/rcsb/utils/struct/EntryInfoProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.struct-0.43/rcsb/utils/struct/Scop2ClassificationProvider.py` & `rcsb.utils.struct-0.44/rcsb/utils/struct/Scop2ClassificationProvider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ##
 #  File:  Scop2ClassificationProvider.py
 #  Date:  29-Jun-2021 jdw
 #
 #  Updates:
 #   10-Sep-2021 jdw split tree with type and class roots
 #   24-Feb-2022 dwp Resolve duplication issues with Scop2 tree node list, and fix parent ID lists for nodes with multiple parents
+#   18-Apr-2023 aae Use "pickle" as default file format
 ##
 """
   Extract SCOP2 domain assignments, term descriptions and SCOP2 classification hierarchy
   from SCOP2 and SCOP2B flat files.
 
 """
 
@@ -41,15 +42,15 @@
         #
         self.__version = "latest"
         self.__fmt = "pickle"
         self.__mU = MarshalUtil(workPath=self.__dirPath)
         self.__nD, self.__ntD, self.__pAD, self.__pBD, self.__pBRootD, self.__fD, self.__sfD, self.__sf2bD = self.__reload(useCache=self.__useCache, fmt=self.__fmt)
         #
         if not useCache and not self.testCache():
-            ok = self.__fetchFromBackup()
+            ok = self.__fetchFromBackup(fmt=self.__fmt)
             if ok:
                 self.__nD, self.__ntD, self.__pAD, self.__pBD, self.__pBRootD, self.__fD, self.__sfD, self.__sf2bD = self.__reload(useCache=True, fmt=self.__fmt)
         #
 
     def testCache(self):
         logger.info(
             "SCOP2 lengths nD %d pAD %d pBD %d pBRootD %d fD %d sfD %d sf2bD %d",
@@ -172,20 +173,20 @@
             logger.debug("Failing for %r with %s", domId, str(e))
         return None
 
     def getTreeNodeList(self):
         tnL = self.__exportTreeNodeList(self.__nD, self.__pAD, self.__pBRootD)
         return tnL
 
-    def __getAssignmentFileName(self, fmt="json"):
+    def __getAssignmentFileName(self, fmt="pickle"):
         ext = "json" if fmt == "json" else "pic"
         fn = "scop2_domain_assignments.%s" % ext
         return fn
 
-    def __reload(self, useCache=True, fmt="json"):
+    def __reload(self, useCache=True, fmt="pickle"):
         nD = ntD = pAD = pBD = pBRootD = fD = sfD = sf2bD = {}
         fn = self.__getAssignmentFileName(fmt=fmt)
         assignmentPath = os.path.join(self.__dirPath, fn)
         self.__mU.mkdir(self.__dirPath)
         #
         if useCache and self.__mU.exists(assignmentPath):
             sD = self.__mU.doImport(assignmentPath, fmt=fmt)
@@ -232,15 +233,15 @@
                 "superfamilies2b": sf2bD
             }
             ok = self.__mU.doExport(assignmentPath, sD, fmt=fmt, indent=3)
             logger.info("Cache save status %r", ok)
             #
         return nD, ntD, pAD, pBD, pBRootD, fD, sfD, sf2bD
 
-    def __fetchFromBackup(self, fmt="json"):
+    def __fetchFromBackup(self, fmt="pickle"):
         urlTarget = "https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/fall_back/SCOP2"
         #
         fn = self.__getAssignmentFileName(fmt=fmt)
         assignmentPath = os.path.join(self.__dirPath, fn)
         urlPath = os.path.join(urlTarget, fn)
         self.__mU.mkdir(assignmentPath)
         #
```

### Comparing `rcsb.utils.struct-0.43/rcsb/utils/struct/ScopClassificationProvider.py` & `rcsb.utils.struct-0.44/rcsb/utils/struct/ScopClassificationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.struct-0.43/rcsb.utils.struct.egg-info/PKG-INFO` & `rcsb.utils.struct-0.44/rcsb.utils.struct.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.struct
-Version: 0.43
+Version: 0.44
 Summary: RCSB Python utility classes for accessing PDB primary structure data and features associated with these data
 Home-page: https://github.com/rcsb/py-rcsb_utils_seq
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.struct-0.43/rcsb.utils.struct.egg-info/SOURCES.txt` & `rcsb.utils.struct-0.44/rcsb.utils.struct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.struct-0.43/setup.py` & `rcsb.utils.struct-0.44/setup.py`

 * *Files identical despite different names*

