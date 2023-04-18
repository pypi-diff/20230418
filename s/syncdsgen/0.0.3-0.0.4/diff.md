# Comparing `tmp/syncdsgen-0.0.3.tar.gz` & `tmp/syncdsgen-0.0.4.tar.gz`

## Comparing `syncdsgen-0.0.3.tar` & `syncdsgen-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0     2063 2020-02-02 00:00:00.000000 syncdsgen-0.0.3/requirements.txt
--rwxr-xr-x   0        0        0     9221 2020-02-02 00:00:00.000000 syncdsgen-0.0.3/syncdsgen_demo.ipynb
--rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 syncdsgen-0.0.3/.vscode/settings.json
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 syncdsgen-0.0.3/SynCDsGen/__init__.py
--rwxr-xr-x   0        0        0    13147 2020-02-02 00:00:00.000000 syncdsgen-0.0.3/SynCDsGen/syncdsgen.py
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 syncdsgen-0.0.3/.gitignore
--rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 syncdsgen-0.0.3/LICENCE
--rwxr-xr-x   0        0        0      479 2020-02-02 00:00:00.000000 syncdsgen-0.0.3/README.md
--rwxr-xr-x   0        0        0      615 2020-02-02 00:00:00.000000 syncdsgen-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 syncdsgen-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0     2063 2020-02-02 00:00:00.000000 syncdsgen-0.0.4/requirements.txt
+-rwxr-xr-x   0        0        0     9221 2020-02-02 00:00:00.000000 syncdsgen-0.0.4/syncdsgen_demo.ipynb
+-rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 syncdsgen-0.0.4/.vscode/settings.json
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 syncdsgen-0.0.4/SynCDsGen/__init__.py
+-rwxr-xr-x   0        0        0    13147 2020-02-02 00:00:00.000000 syncdsgen-0.0.4/SynCDsGen/syncdsgen.py
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 syncdsgen-0.0.4/.gitignore
+-rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 syncdsgen-0.0.4/LICENCE
+-rwxr-xr-x   0        0        0      479 2020-02-02 00:00:00.000000 syncdsgen-0.0.4/README.md
+-rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 syncdsgen-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 syncdsgen-0.0.4/PKG-INFO
```

### Comparing `syncdsgen-0.0.3/requirements.txt` & `syncdsgen-0.0.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `syncdsgen-0.0.3/syncdsgen_demo.ipynb` & `syncdsgen-0.0.4/syncdsgen_demo.ipynb`

 * *Files identical despite different names*

### Comparing `syncdsgen-0.0.3/SynCDsGen/syncdsgen.py` & `syncdsgen-0.0.4/SynCDsGen/syncdsgen.py`

 * *Files identical despite different names*

### Comparing `syncdsgen-0.0.3/LICENCE` & `syncdsgen-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `syncdsgen-0.0.3/pyproject.toml` & `syncdsgen-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [dependencies]
 torch = "*"
-pyro = "*"
+pyro-ppl = "*"
 pandas = "*"
 numpy = "*"
-re = "*"
-enum ="*"
 
 [project]
 name = "syncdsgen"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Ramses TANANKEM", email="tanankemr@gmail.com" },
 ]
 description = "A package to generate synthetic coding sequences data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `syncdsgen-0.0.3/PKG-INFO` & `syncdsgen-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncdsgen
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package to generate synthetic coding sequences data
 Project-URL: Homepage, https://github.com/wl-research/syncdsgen
 Author-email: Ramses TANANKEM <tanankemr@gmail.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

