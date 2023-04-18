# Comparing `tmp/syncdsgen-0.0.5.tar.gz` & `tmp/syncdsgen-0.0.6.tar.gz`

## Comparing `syncdsgen-0.0.5.tar` & `syncdsgen-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0     2063 2020-02-02 00:00:00.000000 syncdsgen-0.0.5/requirements.txt
--rwxr-xr-x   0        0        0     9221 2020-02-02 00:00:00.000000 syncdsgen-0.0.5/syncdsgen_demo.ipynb
--rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 syncdsgen-0.0.5/.vscode/settings.json
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 syncdsgen-0.0.5/SynCDsGen/__init__.py
--rwxr-xr-x   0        0        0    13147 2020-02-02 00:00:00.000000 syncdsgen-0.0.5/SynCDsGen/syncdsgen.py
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 syncdsgen-0.0.5/.gitignore
--rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 syncdsgen-0.0.5/LICENCE
--rwxr-xr-x   0        0        0      479 2020-02-02 00:00:00.000000 syncdsgen-0.0.5/README.md
--rwxr-xr-x   0        0        0      601 2020-02-02 00:00:00.000000 syncdsgen-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 syncdsgen-0.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0     2063 2020-02-02 00:00:00.000000 syncdsgen-0.0.6/requirements.txt
+-rwxr-xr-x   0        0        0     9221 2020-02-02 00:00:00.000000 syncdsgen-0.0.6/syncdsgen_demo.ipynb
+-rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 syncdsgen-0.0.6/.vscode/settings.json
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 syncdsgen-0.0.6/SynCDsGen/__init__.py
+-rwxr-xr-x   0        0        0    13204 2020-02-02 00:00:00.000000 syncdsgen-0.0.6/SynCDsGen/syncdsgen.py
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 syncdsgen-0.0.6/.gitignore
+-rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 syncdsgen-0.0.6/LICENCE
+-rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 syncdsgen-0.0.6/README.md
+-rwxr-xr-x   0        0        0      601 2020-02-02 00:00:00.000000 syncdsgen-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 syncdsgen-0.0.6/PKG-INFO
```

### Comparing `syncdsgen-0.0.5/requirements.txt` & `syncdsgen-0.0.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `syncdsgen-0.0.5/syncdsgen_demo.ipynb` & `syncdsgen-0.0.6/syncdsgen_demo.ipynb`

 * *Files identical despite different names*

### Comparing `syncdsgen-0.0.5/SynCDsGen/syncdsgen.py` & `syncdsgen-0.0.6/SynCDsGen/syncdsgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,8 +284,8 @@
             CDs_samples.append(CDs_sample)
 
         self.AAs_indices_sequences = torch.vstack(AAs_samples).numpy().astype(int)
         self.CDs__indices_sequences = torch.vstack(CDs_samples).numpy().astype(int)
 
         self.build_dataframe()
 
-        return self.synthetic_data
+        return self.synthetic_data, self.AAs_indices_sequences, self.CDs__indices_sequences
```

### Comparing `syncdsgen-0.0.5/LICENCE` & `syncdsgen-0.0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `syncdsgen-0.0.5/pyproject.toml` & `syncdsgen-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "syncdsgen"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Ramses TANANKEM", email="tanankemr@gmail.com" },
 ]
 description = "A package to generate synthetic coding sequences data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `syncdsgen-0.0.5/PKG-INFO` & `syncdsgen-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncdsgen
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package to generate synthetic coding sequences data
 Project-URL: Homepage, https://github.com/wl-research/syncdsgen
 Author-email: Ramses TANANKEM <tanankemr@gmail.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 
 ## SynCDsGen(Synthetic Coding Sequences Generator) is a module to sample synthetic coding sequences data from a given generative model.
 
 ## Installation
 
 ### Installation by using the pip package:
 ```
-!pip install syncdsgen
+!pip install syncdsgen --upgrade
 ```
 ### Installation by cloning the repo:
 You can clone the repo: 
 ```
 git clone https://github.com/wl-research/syncdsgen
 ```
 And install requirements:
```

