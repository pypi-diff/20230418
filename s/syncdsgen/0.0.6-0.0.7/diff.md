# Comparing `tmp/syncdsgen-0.0.6.tar.gz` & `tmp/syncdsgen-0.0.7.tar.gz`

## Comparing `syncdsgen-0.0.6.tar` & `syncdsgen-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0     2063 2020-02-02 00:00:00.000000 syncdsgen-0.0.6/requirements.txt
--rwxr-xr-x   0        0        0     9221 2020-02-02 00:00:00.000000 syncdsgen-0.0.6/syncdsgen_demo.ipynb
--rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 syncdsgen-0.0.6/.vscode/settings.json
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 syncdsgen-0.0.6/SynCDsGen/__init__.py
--rwxr-xr-x   0        0        0    13204 2020-02-02 00:00:00.000000 syncdsgen-0.0.6/SynCDsGen/syncdsgen.py
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 syncdsgen-0.0.6/.gitignore
--rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 syncdsgen-0.0.6/LICENCE
--rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 syncdsgen-0.0.6/README.md
--rwxr-xr-x   0        0        0      601 2020-02-02 00:00:00.000000 syncdsgen-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 syncdsgen-0.0.6/PKG-INFO
+-rwxr-xr-x   0        0        0     2063 2020-02-02 00:00:00.000000 syncdsgen-0.0.7/requirements.txt
+-rwxr-xr-x   0        0        0     9221 2020-02-02 00:00:00.000000 syncdsgen-0.0.7/syncdsgen_demo.ipynb
+-rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 syncdsgen-0.0.7/.vscode/settings.json
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 syncdsgen-0.0.7/SynCDsGen/__init__.py
+-rwxr-xr-x   0        0        0    13261 2020-02-02 00:00:00.000000 syncdsgen-0.0.7/SynCDsGen/syncdsgen.py
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 syncdsgen-0.0.7/.gitignore
+-rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 syncdsgen-0.0.7/LICENCE
+-rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 syncdsgen-0.0.7/README.md
+-rwxr-xr-x   0        0        0      601 2020-02-02 00:00:00.000000 syncdsgen-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 syncdsgen-0.0.7/PKG-INFO
```

### Comparing `syncdsgen-0.0.6/requirements.txt` & `syncdsgen-0.0.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `syncdsgen-0.0.6/syncdsgen_demo.ipynb` & `syncdsgen-0.0.7/syncdsgen_demo.ipynb`

 * *Files identical despite different names*

### Comparing `syncdsgen-0.0.6/SynCDsGen/syncdsgen.py` & `syncdsgen-0.0.7/SynCDsGen/syncdsgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,15 +217,15 @@
             CDs_samples.append(CDs_sample)
 
         self.AAs_indices_sequences = torch.vstack(AAs_samples).numpy().astype(int)
         self.CDs__indices_sequences = torch.vstack(CDs_samples).numpy().astype(int)
 
         self.build_dataframe()
 
-        return self.synthetic_data
+        return self.synthetic_data, self.AAs_indices_sequences, self.CDs__indices_sequences
 
 
 class AutoregressiveSynCDsGenerator(SynCDsGenerator):
     def __init__(self, generatorConf:SyncCDsGeneratorConf):
         SynCDsGenerator.__init__(self, generatorConf)
 
         assert len(self.generatorConf.constraints_dict) > 0, "For a StochasticSynCDsGenerator, we should set the SyncCDsGeneratorConf's constraints_dict to a non empty dictionary"
```

### Comparing `syncdsgen-0.0.6/LICENCE` & `syncdsgen-0.0.7/LICENCE`

 * *Files identical despite different names*

### Comparing `syncdsgen-0.0.6/pyproject.toml` & `syncdsgen-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "syncdsgen"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Ramses TANANKEM", email="tanankemr@gmail.com" },
 ]
 description = "A package to generate synthetic coding sequences data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `syncdsgen-0.0.6/PKG-INFO` & `syncdsgen-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncdsgen
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package to generate synthetic coding sequences data
 Project-URL: Homepage, https://github.com/wl-research/syncdsgen
 Author-email: Ramses TANANKEM <tanankemr@gmail.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

