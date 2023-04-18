# Comparing `tmp/xplt-0.4.0.tar.gz` & `tmp/xplt-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xplt-0.4.0.tar", last modified: Wed Feb 15 09:11:36 2023, max compression
+gzip compressed data, was "xplt-0.4.1.tar", last modified: Tue Apr 18 09:49:55 2023, max compression
```

## Comparing `xplt-0.4.0.tar` & `xplt-0.4.1.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:11:36.836083 xplt-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:11:36.824083 xplt-0.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)   306475 2023-02-15 09:11:27.000000 xplt-0.4.0/.github/sampleplot.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:11:36.824083 xplt-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-02-15 09:11:27.000000 xplt-0.4.0/.github/workflows/qa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-02-15 09:11:27.000000 xplt-0.4.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-02-15 09:11:27.000000 xplt-0.4.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-02-15 09:11:27.000000 xplt-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-02-15 09:11:27.000000 xplt-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-02-15 09:11:36.832083 xplt-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-02-15 09:11:27.000000 xplt-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:11:36.824083 xplt-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-15 09:11:27.000000 xplt-0.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-15 09:11:27.000000 xplt-0.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-02-15 09:11:27.000000 xplt-0.4.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:11:36.824083 xplt-0.4.0/docs/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)   198024 2023-02-15 09:11:27.000000 xplt-0.4.0/docs/gallery/bpm.png
--rw-r--r--   0 runner    (1001) docker     (123)   220074 2023-02-15 09:11:27.000000 xplt-0.4.0/docs/gallery/floorplot.png
--rw-r--r--   0 runner    (1001) docker     (123)   322259 2023-02-15 09:11:27.000000 xplt-0.4.0/docs/gallery/phasespaceplot.png
--rw-r--r--   0 runner    (1001) docker     (123)   106520 2023-02-15 09:11:27.000000 xplt-0.4.0/docs/gallery/spill.png
--rw-r--r--   0 runner    (1001) docker     (123)   206605 2023-02-15 09:11:27.000000 xplt-0.4.0/docs/gallery/spillquality.png
--rw-r--r--   0 runner    (1001) docker     (123)   186129 2023-02-15 09:11:27.000000 xplt-0.4.0/docs/gallery/twissplot.png
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-15 09:11:27.000000 xplt-0.4.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-02-15 09:11:27.000000 xplt-0.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-02-15 09:11:27.000000 xplt-0.4.0/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-02-15 09:11:27.000000 xplt-0.4.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-02-15 09:11:27.000000 xplt-0.4.0/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:11:36.832083 xplt-0.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)  2689969 2023-02-15 09:11:27.000000 xplt-0.4.0/examples/animations.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   142849 2023-02-15 09:11:27.000000 xplt-0.4.0/examples/colors.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   221195 2023-02-15 09:11:27.000000 xplt-0.4.0/examples/hamiltonians.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   235359 2023-02-15 09:11:27.000000 xplt-0.4.0/examples/line.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1819373 2023-02-15 09:11:27.000000 xplt-0.4.0/examples/phasespace.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-15 09:11:27.000000 xplt-0.4.0/examples/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)   478501 2023-02-15 09:11:27.000000 xplt-0.4.0/examples/timestructure.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   146369 2023-02-15 09:11:27.000000 xplt-0.4.0/examples/twiss.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    57663 2023-02-15 09:11:27.000000 xplt-0.4.0/examples/units.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-02-15 09:11:27.000000 xplt-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 09:11:36.836083 xplt-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:11:36.832083 xplt-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-15 09:11:27.000000 xplt-0.4.0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-02-15 09:11:27.000000 xplt-0.4.0/tests/test_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:11:36.832083 xplt-0.4.0/xplt/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-02-15 09:11:27.000000 xplt-0.4.0/xplt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24365 2023-02-15 09:11:27.000000 xplt-0.4.0/xplt/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-02-15 09:11:27.000000 xplt-0.4.0/xplt/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-02-15 09:11:27.000000 xplt-0.4.0/xplt/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-02-15 09:11:27.000000 xplt-0.4.0/xplt/line.py
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-02-15 09:11:27.000000 xplt-0.4.0/xplt/particles.py
--rw-r--r--   0 runner    (1001) docker     (123)    27417 2023-02-15 09:11:27.000000 xplt-0.4.0/xplt/phasespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    41556 2023-02-15 09:11:27.000000 xplt-0.4.0/xplt/timestructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-02-15 09:11:27.000000 xplt-0.4.0/xplt/twiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-02-15 09:11:27.000000 xplt-0.4.0/xplt/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-02-15 09:11:27.000000 xplt-0.4.0/xplt/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:11:36.832083 xplt-0.4.0/xplt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-02-15 09:11:36.000000 xplt-0.4.0/xplt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-02-15 09:11:36.000000 xplt-0.4.0/xplt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 09:11:36.000000 xplt-0.4.0/xplt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-15 09:11:36.000000 xplt-0.4.0/xplt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-15 09:11:36.000000 xplt-0.4.0/xplt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:49:55.398734 xplt-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:49:55.382734 xplt-0.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)   306475 2023-04-18 09:49:46.000000 xplt-0.4.1/.github/sampleplot.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:49:55.382734 xplt-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-18 09:49:46.000000 xplt-0.4.1/.github/workflows/qa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-18 09:49:46.000000 xplt-0.4.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-18 09:49:46.000000 xplt-0.4.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-18 09:49:46.000000 xplt-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-18 09:49:46.000000 xplt-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-18 09:49:46.000000 xplt-0.4.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-18 09:49:55.398734 xplt-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-18 09:49:46.000000 xplt-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:49:55.382734 xplt-0.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-18 09:49:46.000000 xplt-0.4.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-18 09:49:46.000000 xplt-0.4.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-18 09:49:46.000000 xplt-0.4.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:49:55.386734 xplt-0.4.1/docs/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)   198024 2023-04-18 09:49:46.000000 xplt-0.4.1/docs/gallery/bpm.png
+-rw-r--r--   0 runner    (1001) docker     (123)   220074 2023-04-18 09:49:46.000000 xplt-0.4.1/docs/gallery/floorplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)   322259 2023-04-18 09:49:46.000000 xplt-0.4.1/docs/gallery/phasespaceplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)   106520 2023-04-18 09:49:46.000000 xplt-0.4.1/docs/gallery/spill.png
+-rw-r--r--   0 runner    (1001) docker     (123)   206605 2023-04-18 09:49:46.000000 xplt-0.4.1/docs/gallery/spillquality.png
+-rw-r--r--   0 runner    (1001) docker     (123)   186129 2023-04-18 09:49:46.000000 xplt-0.4.1/docs/gallery/twissplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-18 09:49:46.000000 xplt-0.4.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-18 09:49:46.000000 xplt-0.4.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-18 09:49:46.000000 xplt-0.4.1/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-18 09:49:46.000000 xplt-0.4.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-18 09:49:46.000000 xplt-0.4.1/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:49:55.394734 xplt-0.4.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)  2689969 2023-04-18 09:49:46.000000 xplt-0.4.1/examples/animations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   142849 2023-04-18 09:49:46.000000 xplt-0.4.1/examples/colors.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   221195 2023-04-18 09:49:46.000000 xplt-0.4.1/examples/hamiltonians.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   235359 2023-04-18 09:49:46.000000 xplt-0.4.1/examples/line.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1819373 2023-04-18 09:49:46.000000 xplt-0.4.1/examples/phasespace.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-18 09:49:46.000000 xplt-0.4.1/examples/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   478503 2023-04-18 09:49:46.000000 xplt-0.4.1/examples/timestructure.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   146369 2023-04-18 09:49:46.000000 xplt-0.4.1/examples/twiss.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    57663 2023-04-18 09:49:46.000000 xplt-0.4.1/examples/units.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-18 09:49:46.000000 xplt-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 09:49:55.398734 xplt-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:49:55.394734 xplt-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-18 09:49:46.000000 xplt-0.4.1/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-18 09:49:46.000000 xplt-0.4.1/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:49:55.394734 xplt-0.4.1/xplt/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-18 09:49:46.000000 xplt-0.4.1/xplt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24365 2023-04-18 09:49:46.000000 xplt-0.4.1/xplt/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-18 09:49:46.000000 xplt-0.4.1/xplt/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-18 09:49:46.000000 xplt-0.4.1/xplt/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-04-18 09:49:46.000000 xplt-0.4.1/xplt/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-18 09:49:46.000000 xplt-0.4.1/xplt/particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27417 2023-04-18 09:49:46.000000 xplt-0.4.1/xplt/phasespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43203 2023-04-18 09:49:46.000000 xplt-0.4.1/xplt/timestructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-18 09:49:46.000000 xplt-0.4.1/xplt/twiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-04-18 09:49:46.000000 xplt-0.4.1/xplt/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-04-18 09:49:46.000000 xplt-0.4.1/xplt/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:49:55.394734 xplt-0.4.1/xplt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-18 09:49:55.000000 xplt-0.4.1/xplt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-18 09:49:55.000000 xplt-0.4.1/xplt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:49:55.000000 xplt-0.4.1/xplt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 09:49:55.000000 xplt-0.4.1/xplt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 09:49:55.000000 xplt-0.4.1/xplt.egg-info/top_level.txt
```

### Comparing `xplt-0.4.0/.github/sampleplot.png` & `xplt-0.4.1/.github/sampleplot.png`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/.github/workflows/qa.yaml` & `xplt-0.4.1/.github/workflows/qa.yaml`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/.github/workflows/test.yaml` & `xplt-0.4.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/.gitignore` & `xplt-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/PKG-INFO` & `xplt-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xplt
-Version: 0.4.0
+Version: 0.4.1
 Summary: Plotting for Xsuite
 Author-email: "Philipp Niedermayer (github.com/eltos)" <eltos@outlook.de>
 Project-URL: homepage, https://github.com/eltos/xplt
 Project-URL: documentation, https://eltos.github.io/xplt
 Project-URL: repository, https://github.com/eltos/xplt
 Keywords: python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `xplt-0.4.0/README.md` & `xplt-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/docs/Makefile` & `xplt-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/docs/conf.py` & `xplt-0.4.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         # build link
         root = "xplt" + os.path.sep
         if root not in sourcefile:
             return None  # external source
         else:
             path = (root + sourcefile.split(root)[-1]).replace(os.path.sep, "/")
             filename = f"{path}#L{line}-L{line + len(sourcecode) - 1}"
-            return f"https://github.com/eltos/xplt/blob/main/{filename}"
+            return f"https://github.com/eltos/xplt/blob/v{version}/{filename}"
     except:
         return None
 
 
 # Example notebooks
 def np_example_notebooks_init(app, *args):
     global np_example_notebooks
```

### Comparing `xplt-0.4.0/docs/gallery/bpm.png` & `xplt-0.4.1/docs/gallery/bpm.png`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/docs/gallery/floorplot.png` & `xplt-0.4.1/docs/gallery/floorplot.png`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/docs/gallery/phasespaceplot.png` & `xplt-0.4.1/docs/gallery/phasespaceplot.png`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/docs/gallery/spill.png` & `xplt-0.4.1/docs/gallery/spill.png`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/docs/gallery/spillquality.png` & `xplt-0.4.1/docs/gallery/spillquality.png`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/docs/gallery/twissplot.png` & `xplt-0.4.1/docs/gallery/twissplot.png`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/docs/make.bat` & `xplt-0.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/docs/quickstart.md` & `xplt-0.4.1/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/docs/usage.md` & `xplt-0.4.1/docs/usage.md`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/examples/animations.ipynb` & `xplt-0.4.1/examples/animations.ipynb`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/examples/colors.ipynb` & `xplt-0.4.1/examples/colors.ipynb`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/examples/hamiltonians.ipynb` & `xplt-0.4.1/examples/hamiltonians.ipynb`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/examples/line.ipynb` & `xplt-0.4.1/examples/line.ipynb`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/examples/phasespace.ipynb` & `xplt-0.4.1/examples/phasespace.ipynb`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/examples/timestructure.ipynb` & `xplt-0.4.1/examples/timestructure.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996744791666667%*

 * *Differences: {"'cells'": "{22: {'source': ['plot = xplt.TimeIntervalPlot(particles, dt_max=1e-9, log=True, "*

 * *            "twiss=tw)']}}"}*

```diff
@@ -397,15 +397,15 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "plot = xplt.TimeIntervalPlot(particles, tmax=1e-9, log=True, twiss=tw)"
+                "plot = xplt.TimeIntervalPlot(particles, dt_max=1e-9, log=True, twiss=tw)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8b3cf244-0b54-4e57-a1f8-57710aabe34f",
             "metadata": {},
             "source": [
```

### Comparing `xplt-0.4.0/examples/twiss.ipynb` & `xplt-0.4.1/examples/twiss.ipynb`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/examples/units.ipynb` & `xplt-0.4.1/examples/units.ipynb`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/pyproject.toml` & `xplt-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/tests/test_examples.py` & `xplt-0.4.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/xplt/__init__.py` & `xplt-0.4.1/xplt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 __author__ = "Philipp Niedermayer"
 __contact__ = "eltos@outlook.de"
 
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 # allow usage of xplt.mpl.* without importing matplotlib
 import matplotlib as mpl
 
 from .units import register_property
 from .colors import *
 from .line import KnlPlot, FloorPlot
```

### Comparing `xplt-0.4.0/xplt/base.py` & `xplt-0.4.1/xplt/base.py`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/xplt/colors.py` & `xplt-0.4.1/xplt/colors.py`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/xplt/hooks.py` & `xplt-0.4.1/xplt/hooks.py`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/xplt/line.py` & `xplt-0.4.1/xplt/line.py`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/xplt/particles.py` & `xplt-0.4.1/xplt/particles.py`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/xplt/phasespace.py` & `xplt-0.4.1/xplt/phasespace.py`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/xplt/timestructure.py` & `xplt-0.4.1/xplt/timestructure.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,64 +18,80 @@
 
 from .util import defaults
 from .base import XManifoldPlot
 from .particles import ParticlePlotMixin, ParticlesPlot
 from .units import Prop
 
 
-def binned_timeseries(times, n, what=None, range=None):
+def binned_timeseries(times, *, what=None, n=None, dt=None, t_range=None, moments=1):
     """Get binned timeseries with equally spaced time bins
 
     From the particle arrival times (non-equally distributed timestamps), a timeseries with equally
-    spaced time bins is derived. The time bin size is determined based on the number of bins.
-    The parameter ``what`` determines what is returned for the timeseries. By default (what=None), the
-    number of particles arriving within each time bin is returned. Alternatively, a particle property
-    can be passed as array, in which case that property is averaged over all particles arriving within
-    the respective bin (or 0 if no particles arrive within a time bin).
+    spaced time bins is derived. The parameter ``what`` determines what is returned for the timeseries.
+    By default (what=None), the number of particles arriving within each time bin is returned.
+    Alternatively, a particle property can be passed as array, in which case that property is averaged
+    over all particles arriving within the respective bin (or 0 if no particles arrive within a time bin).
+    It is also possible to specify the moments to return, i.e. the power to which the property is raised
+    before averaging. This allows to determine mean (1st moment, default) and variance (difference between
+    2nd and 1st moment) etc.
 
     Args:
         times (np.ndarray): Array of particle arrival times.
-        n (int): Number of bins.
+        n (int | None): Number of bins. Must not be used together with dt.
+        dt (float | None): Bin width in seconds. Must not be used together with n.
+        t_range (tuple[float] | None): Tuple of (min, max) time values to consider. If None, the range is determined from the data.
         what (np.ndarray | None): Array of associated data or None. Must have same shape as times. See above.
-        range (tuple[int] | None): Tuple of (min, max) time values to consider. If None, the range is determined from the data.
+        moments (int | list[int]): The moment(s) to return for associated data if what is not None. See above.
 
     Returns:
         The timeseries as tuple (t_min, dt, values) where
         t_min is the start time of the timeseries data,
         dt is the time bin width and
         values are the values of the timeseries as array of length n.
     """
 
+    t_min = np.min(times) if t_range is None or t_range[0] is None else t_range[0]
+    t_max = np.max(times) if t_range is None or t_range[1] is None else t_range[1]
+
+    if n is not None and dt is None:
+        # number of bins requested, adjust bin width accordingly
+        dt = (t_max - t_min) / n
+    elif n is None and dt is not None:
+        # bin width requested, adjust number of bins accordingly
+        n = int(np.ceil((t_max - t_min) / dt))
+    else:
+        raise ValueError(f"Exactly one of n or dt must be specified, but got n={n} and dt={dt}")
+
     # Note: The code below was optimized to run much faster than an ordinary
     # np.histogram, which quickly slows down for large datasets.
     # If you intend to change something here, make sure to benchmark it!
 
-    t_min = np.min(times) if range is None or range[0] is None else range[0]
-    t_max = np.max(times) if range is None or range[1] is None else range[1]
-    dt = (t_max - t_min) / n
     # count timestamps in bins
-    bins = ((times - t_min) / dt).astype(int)
+    bins = np.floor((times - t_min) / dt).astype(int)
     # bins are i*dt <= t < (i+1)*dt where i = 0 .. n-1
     mask = (bins >= 0) & (bins < n)  # igore times outside range
     bins = bins[mask]
     # count particles per time bin
     counts = np.bincount(bins, minlength=n)[:n]
 
     if what is None:
         # Return particle counts
         return t_min, dt, counts
 
     else:
         # Return 'what' averaged
-        v = np.zeros(n)
-        # sum up 'what' for all the particles in each bin
-        np.add.at(v, bins, what[mask])
-        # divide by particle count to get mean (default to 0)
-        v[counts > 0] /= counts[counts > 0]
-        return t_min, dt, v
+        result = [t_min, dt]
+        for m in [moments] if isinstance(moments, int) else moments:
+            v = np.zeros(n)
+            # sum up 'what' for all the particles in each bin
+            np.add.at(v, bins, what[mask] ** m)
+            # divide by particle count to get mean (default to 0)
+            v[counts > 0] /= counts[counts > 0]
+            result.append(v)
+        return result
 
 
 class TimePlot(ParticlesPlot):
     def __init__(self, particles=None, kind="x+y", **kwargs):
         """
         A thin wrapper around the ParticlesPlot plotting data as function of time.
         For more information refer to the documentation of the :class:`~xplt.particles.ParticlesPlot` class.
@@ -99,17 +115,17 @@
     def __init__(
         self,
         particles=None,
         kind="count",
         *,
         bin_time=None,
         bin_count=None,
-        exact_bin_time=True,
         relative=False,
         mask=None,
+        time_range=None,
         plot_kwargs=None,
         **kwargs,
     ):
         """
         A binned histogram plot of particles as function of times.
 
         The plot is based on the particle arrival time, which is:
@@ -122,22 +138,20 @@
         Useful to plot time structures of particles loss, such as spill structures.
 
         Args:
             particles (Any): Particles data to plot.
             kind (str | list): Defines the properties to plot, including 'count' (default), 'rate', 'cumulative', or a particle property to average.
                 This is a manifold subplot specification string like ``"count-cumulative"``, see :class:`~.base.XManifoldPlot` for details.
                 In addition, abbreviations for x-y-parameter pairs are supported (e.g. ``P`` for ``Px+Py``).
-            bin_time (float): Time bin width if bin_count is None.
+            bin_time (float): Time bin width (in s) if bin_count is None.
             bin_count (int): Number of bins if bin_time is None.
-            exact_bin_time (bool): What to do if bin_time is given but length of data is not an exact multiple of it.
-                If True, overhanging data is removed such that the data length is a multiple of bin_time.
-                If False, bin_time is adjusted instead.
             relative (bool): If True, plot relative numbers normalized to total count.
                 If what is a particle property, this has no effect.
             mask (Any): An index mask to select particles to plot. If None, all particles are plotted.
+            time_range (tuple): Time range of particles to consider. If None, all particles are considered.
             plot_kwargs (dict): Keyword arguments passed to the plot function.
             kwargs: See :class:`~.particles.ParticlePlotMixin` and :class:`~.base.XPlot` for additional arguments
 
         """
         kwargs = self._init_particle_mixin(**kwargs)
         kwargs["data_units"] = defaults(
             kwargs.get("data_units"),
@@ -149,18 +163,20 @@
             on_x="t",
             on_y=kind,
             **kwargs,
         )
 
         if bin_time is None and bin_count is None:
             bin_count = 100
+        if bin_time is not None and bin_count is not None:
+            raise ValueError("Only one of bin_time or bin_count may be specified.")
         self.bin_time = bin_time
         self.bin_count = bin_count
-        self.exact_bin_time = exact_bin_time
         self.relative = relative
+        self.time_range = time_range
 
         # Format plot axes
         self.axis(-1).set(xlabel=self.label_for("t"), ylim=(0, None))
         if self.relative:
             for a in self.axflat:
                 a.yaxis.set_major_formatter(mpl.ticker.PercentFormatter(1))
 
@@ -195,41 +211,36 @@
         Returns:
             list: Changed artists
         """
 
         # extract times
         times = self._get_masked(particles, "t", mask)
 
-        # re-sample times into equally binned time series
-        if self.bin_count:
-            n = self.bin_count
-            t_range = None
-        elif self.exact_bin_time:
-            n = int((np.max(times) - np.min(times)) / self.bin_time)
-            t_range = np.min(times) + np.array([0, n * self.bin_time])
-        else:
-            n = int(round((np.max(times) - np.min(times)) / self.bin_time))
-            t_range = None
-
         # update plots
         changed = []
         for i, ppp in enumerate(self.on_y):
             for j, pp in enumerate(ppp):
                 count_based = False
                 for k, p in enumerate(pp):
                     prop = self._get_property(p)
                     count_based = prop.key in ("count", "rate", "cumulative")
                     if count_based:
                         property = None
                     else:
                         property = self._get_masked(particles, prop.key, mask)
 
-                    t_min, dt, timeseries = binned_timeseries(times, n, property, t_range)
+                    t_min, dt, timeseries = binned_timeseries(
+                        times,
+                        what=property,
+                        n=self.bin_count,
+                        dt=self.bin_time,
+                        t_range=self.time_range,
+                    )
                     timeseries = timeseries.astype(np.float64)
-                    edges = np.linspace(t_min, t_min + dt * n, n + 1)
+                    edges = np.linspace(t_min, t_min + dt * timeseries.size, timeseries.size + 1)
 
                     self.annotate(
                         f'$\\Delta t_\\mathrm{{bin}} = {pint.Quantity(dt, "s").to_compact():~.4L}$'
                     )
 
                     if self.relative:
                         if not count_based:
@@ -275,14 +286,15 @@
         kind="count",
         *,
         fmax=None,
         relative=False,
         log=None,
         scaling=None,
         mask=None,
+        time_range=None,
         plot_kwargs=None,
         **kwargs,
     ):
         """
         A frequency plot based on particle arrival times.
 
         The particle arrival time is:
@@ -303,21 +315,23 @@
                 This is a manifold subplot specification string like ``"count-cumulative"``, see :class:`~.base.XManifoldPlot` for details.
                 In addition, abbreviations for x-y-parameter pairs are supported (e.g. ``P`` for ``Px+Py``).
             fmax (float): Maximum frequency (in Hz) to plot.
             relative (bool): If True, plot relative frequencies (f/frev) instead of absolute frequencies (f).
             log (bool): If True, plot on a log scale.
             scaling (str | dict): Scaling of the FFT. Can be 'amplitude' or 'pds' or a dict with a scaling per property.
             mask (Any): An index mask to select particles to plot. If None, all particles are plotted.
+            time_range (tuple): Time range of particles to consider. If None, all particles are considered.
             plot_kwargs (dict): Keyword arguments passed to the plot function.
             kwargs: See :class:`~.particles.ParticlePlotMixin` and :class:`~.base.XPlot` for additional arguments
 
         """
 
         self._fmax = fmax
         self.relative = relative
+        self.time_range = time_range
         self._scaling = scaling
         if log is None:
             log = not relative
 
         kwargs = self._init_particle_mixin(
             **kwargs,
         )
@@ -362,15 +376,15 @@
         return "pds" if key == "count" else "amplitude"
 
     def fmax(self, particles):
         if self._fmax is not None:
             return self._fmax
         if self.relative:
             return self.frev(particles)
-        raise ValueError("fmax must be specified.")
+        raise ValueError("fmax must be specified when plotting absolut frequencies.")
 
     def update(self, particles, mask=None, autoscale=False):
         """Update plot with new data
 
         Args:
             particles (Any): Particles data to plot.
             mask (Any): An index mask to select particles to plot. If None, all particles are plotted.
@@ -399,15 +413,17 @@
 
                     if count_based:
                         property = None
                     else:
                         property = self._get_masked(particles, prop.key, mask)
 
                     # compute binned timeseries
-                    t_min, dt, timeseries = binned_timeseries(times, n, property)
+                    t_min, dt, timeseries = binned_timeseries(
+                        times, what=property, n=n, t_range=self.time_range
+                    )
 
                     # calculate fft without DC component
                     freq = np.fft.rfftfreq(n, d=dt)[1:]
                     if self.relative:
                         freq /= self.frev(particles)
                     else:
                         freq *= self.factor_for("f")
@@ -415,14 +431,18 @@
                     if self._get_scaling(prop.key) == "amplitude":
                         # amplitude in units of p
                         mag *= 2 / len(timeseries) * self.factor_for(p)
                     elif self._get_scaling(prop.key) == "pds":
                         # power density spectrum in a.u.
                         mag = mag**2
 
+                    # cut data above fmax which was only added to increase FFT performance
+                    visible = np.argwhere(freq <= fmax)
+                    freq, mag = freq[visible], mag[visible]
+
                     # update plot
                     self.artists[i][j][k].set_data(freq, mag)
                     changed.append(self.artists[i][j][k])
 
                 if autoscale:
                     a = self.axis(i, j)
                     a.relim()
@@ -472,55 +492,55 @@
 
 
 class TimeIntervalPlot(XManifoldPlot, ParticlePlotMixin):
     def __init__(
         self,
         particles=None,
         *,
-        tmax=None,
+        dt_max,
         bin_time=None,
         bin_count=None,
         exact_bin_time=True,
         log=True,
         mask=None,
+        time_range=None,
         plot_kwargs=None,
         **kwargs,
     ):
         """
         A histogram plot of particle arrival intervals (i.e. delay between consecutive particles).
 
         The plot is based on the particle arrival time, which is:
             - For circular lines: at_turn / frev - zeta / beta / c0
             - For linear lines: zeta / beta / c0
 
         Useful to plot time structures of particles loss, such as spill structures.
 
         Args:
             particles (Any): Particles data to plot.
-            tmax (float): Maximum interval (in s) to plot.
-            bin_time (float): Time bin width if bin_count is None.
+            dt_max (float): Maximum interval (in s) to plot.
+            bin_time (float): Time bin width (in s) if bin_count is None.
             bin_count (int): Number of bins if bin_time is None.
-            exact_bin_time (bool): What to do if bin_time is given but tmax is not an exact multiple of it.
-                If True, tmax is adjusted to be a multiple of bin_time.
+            exact_bin_time (bool): What to do if bin_time is given but dt_max is not an exact multiple of it.
+                If True, dt_max is adjusted to be a multiple of bin_time.
                 If False, bin_time is adjusted instead.
             log (bool): If True, plot on a log scale.
             mask (Any): An index mask to select particles to plot. If None, all particles are plotted.
+            time_range (tuple): Time range of particles to consider. If None, all particles are considered.
             plot_kwargs (dict): Keyword arguments passed to the plot function.
             kwargs: See :class:`~.particles.ParticlePlotMixin` and :class:`~.base.XPlot` for additional arguments
 
 
         """
-        if tmax is None:
-            raise ValueError("tmax must be specified.")
 
         if bin_time is not None:
             if exact_bin_time:
-                tmax = bin_time * round(tmax / bin_time)
+                dt_max = bin_time * round(dt_max / bin_time)
             else:
-                bin_time = tmax / round(tmax / bin_time)
+                bin_time = dt_max / round(dt_max / bin_time)
 
         kwargs = self._init_particle_mixin(**kwargs)
         kwargs["data_units"] = defaults(
             kwargs.get("data_units"),
             dt=Prop("$\\Delta t$", unit="s", description="Delay between consecutive particles"),
             count=Prop("$N$", unit="1", description="Particles per bin"),
         )
@@ -530,53 +550,56 @@
             **kwargs,
         )
 
         if bin_time is None and bin_count is None:
             bin_count = 100
         self._bin_time = bin_time
         self._bin_count = bin_count
-        self.tmax = tmax
+        self.time_range = time_range
+        self.dt_max = dt_max
 
         # create plot elements
         def create_artists(i, j, k, ax, p):
             return ax.step([], [], **defaults(plot_kwargs, lw=1))[0]
 
         self._create_artists(create_artists)
 
         # Format plot axes
         ax = self.axis(-1)
-        ax.set(xlim=(self.bin_time if log else 0, self.tmax * self.factor_for("t")))
+        ax.set(xlim=(self.bin_time if log else 0, self.dt_max * self.factor_for("t")))
         if log:
             ax.set(xscale="log", yscale="log")
         else:
             ax.set(ylim=(0, None))
 
         # set data
         if particles is not None:
             self.update(particles, mask=mask, autoscale=True)
 
     @property
     def bin_time(self):
-        return self._bin_time or self.tmax / self._bin_count
+        return self._bin_time or self.dt_max / self._bin_count
 
     @property
     def bin_count(self):
-        return int(np.ceil(self.tmax / self.bin_time))
+        return int(np.ceil(self.dt_max / self.bin_time))
 
     def update(self, particles, mask=None, autoscale=False):
         """Update plot with new data
 
         Args:
             particles (Any): Particles data to plot.
             mask (Any): An index mask to select particles to plot. If None, all particles are plotted.
             autoscale (bool): Whether or not to perform autoscaling on all axes.
         """
 
         # extract times
         times = self._get_masked(particles, "t", mask)
+        if self.time_range:
+            times = times[(self.time_range[0] <= times) & (times < self.time_range[1])]
         delay = self.factor_for("t") * np.diff(sorted(times))
 
         # calculate and plot histogram
         counts, edges = np.histogram(
             delay, bins=self.bin_count, range=(0, self.bin_count * self.bin_time)
         )
         steps = (np.append(edges, edges[-1]), np.concatenate(([0], counts, [0])))
@@ -790,15 +813,15 @@
         )
         if self.evaluate_bins is not None:
             nebins = int(ncbins / self.evaluate_bins)
         else:
             nebins = int(ncbins * self.evaluate_dt / (np.max(times) - np.min(times)))
 
         # bin into counting bins
-        t_min, dt, counts = binned_timeseries(times, ncbins)
+        t_min, dt, counts = binned_timeseries(times, n=ncbins)
         edges = np.linspace(t_min, t_min + dt * ncbins, ncbins + 1)
 
         # make 2D array by subdividing into evaluation bins
         N = counts[: int(len(counts) / nebins) * nebins].reshape((-1, nebins))
         E = edges[: int(len(edges) / nebins + 1) * nebins : nebins]
 
         self.annotate(
@@ -835,20 +858,21 @@
 
 class TimeVariationScalePlot(XManifoldPlot, ParticlePlotMixin, MetricesMixin):
     def __init__(
         self,
         particles=None,
         kind="cv",
         *,
-        time_range=None,
         counting_dt_min=None,
         counting_dt_max=None,
         counting_bins_per_evaluation=50,
+        std=True,
         poisson=True,
         mask=None,
+        time_range=None,
         log=True,
         plot_kwargs=None,
         **kwargs,
     ):
         """Plot variability of particle time as function of timescale
 
         The particle arrival times are histogramed into counting bins, the width of which
@@ -861,24 +885,26 @@
         If the particle data corresponds to particles lost at the extraction septum,
         the plot yields the spill quality on different timescales.
 
 
         Args:
             particles (Any): Particles data to plot.
             kind (str | list): Metric to plot. See above for list of implemented metrics.
-            time_range (tuple): Time range of particles to consider. If None, all particles are considered.
             counting_dt_min (float): Minimum time bin width for counting.
             counting_dt_max (float): Maximum time bin width for counting.
             counting_bins_per_evaluation (int): Number of counting bins used to evaluate metric over.
                 Use None to evaluate metric once over all bins. Otherwise, the metric is evaluated
                 over each ``counting_bins_per_evaluation`` consecutive bins, and average and std of
-                all evaluations plotted. This suppresses fluctuations on timescales > 100*t_bin
-                to influence the metric.
+                all evaluations plotted. This suppresses fluctuations on larger timescales to affect
+                the metric of smaller timescales.
+            std (bool): Whether or not to plot standard deviation of variability.
+                Only relevant if counting_bins_per_evaluation is not None.
             poisson (bool): Whether or not to plot the Poisson limit.
             mask (Any): An index mask to select particles to plot. If None, all particles are plotted.
+            time_range (tuple): Time range of particles to consider. If None, all particles are considered.
             log (bool): Whether or not to plot the x-axis in log scale.
             plot_kwargs (dict): Keyword arguments passed to the plot function.
             kwargs: See :class:`~.particles.ParticlePlotMixin` and :class:`~.base.XPlot` for additional arguments
 
 
         """
         kwargs = self._init_particle_mixin(
@@ -896,26 +922,27 @@
         )
 
         self.time_range = time_range
         self.counting_dt_min = counting_dt_min
         self.counting_dt_max = counting_dt_max
         self.counting_bins_per_evaluation = counting_bins_per_evaluation
         self.log = log
+        std = std and self.counting_bins_per_evaluation
 
         # Format plot axes
         self._format_metric_axes(kwargs.get("ax") is None)
         for a in self.axflat:
             a.set(xscale="log" if self.log else "lin")
 
         # Create plot elements
         def create_artists(i, j, k, ax, p):
             kwargs = defaults(plot_kwargs, label=self._legend_label_for(p))
             plot = ax.plot([], [], **kwargs)[0]
             kwargs.update(color=plot.get_color())
-            if self.counting_bins_per_evaluation:
+            if std:
                 self._errkw = kwargs.copy()
                 self._errkw.update(zorder=1.8, alpha=0.3, ls="-", lw=0)
                 errorbar = ax.fill_between([], [], [], **self._errkw)
             else:
                 errorbar = None
             if poisson:
                 kwargs.update(zorder=1.9, ls=":", label="Poisson limit")
@@ -923,15 +950,15 @@
             else:
                 pstep = None
             return [plot, errorbar, pstep]
 
         self._create_artists(create_artists)
 
         # legend with combined patch
-        if self.counting_bins_per_evaluation:
+        if std:
             # merge plot and errorbar patches
             for i, h in enumerate(self._legend_entries):
                 labels = [h[0].get_label()] + [_.get_label() for _ in h[2:]]
                 self._legend_entries[i] = [tuple(h[0:2])] + h[2:]
                 self.legend(i, show="auto", labels=labels)
 
         # set data
@@ -949,15 +976,15 @@
         Returns:
             Changed artists
         """
 
         # extract times
         times = self._get_masked(particles, "t", mask)
         if self.time_range:
-            times = times[(self.time_range[0] < times) & (times < self.time_range[1])]
+            times = times[(self.time_range[0] <= times) & (times < self.time_range[1])]
         ntotal = times.size
         duration = np.max(times) - np.min(times)
 
         # annotate plot
         # f'$\\langle\\dot{{N}}\\rangle = {pint.Quantity(ntotal/duration, "1/s"):~.4L}$\n'
         self.annotate(
             "$\\Delta t_\\mathrm{evaluate} = "
@@ -998,15 +1025,15 @@
 
         # compute metrices
         DT = np.empty(ncbins_arr.size)
         F = {m: np.empty_like(DT) for m in self.on_y_unique}
         F_std = {m: np.empty_like(DT) for m in self.on_y_unique}
         F_poisson = {m: np.empty_like(DT) for m in self.on_y_unique}
         for i, nbin in enumerate(ncbins_arr):
-            _, DT[i], N = binned_timeseries(times, nbin)
+            _, DT[i], N = binned_timeseries(times, n=nbin)
 
             # calculate metric on sliding window
             stride = min(self.counting_bins_per_evaluation or N.size, N.size)
             N = np.lib.stride_tricks.sliding_window_view(N, stride)
 
             for metric in F.keys():
                 # calculate metrics
```

### Comparing `xplt-0.4.0/xplt/twiss.py` & `xplt-0.4.1/xplt/twiss.py`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/xplt/units.py` & `xplt-0.4.1/xplt/units.py`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/xplt/util.py` & `xplt-0.4.1/xplt/util.py`

 * *Files identical despite different names*

### Comparing `xplt-0.4.0/xplt.egg-info/PKG-INFO` & `xplt-0.4.1/xplt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xplt
-Version: 0.4.0
+Version: 0.4.1
 Summary: Plotting for Xsuite
 Author-email: "Philipp Niedermayer (github.com/eltos)" <eltos@outlook.de>
 Project-URL: homepage, https://github.com/eltos/xplt
 Project-URL: documentation, https://eltos.github.io/xplt
 Project-URL: repository, https://github.com/eltos/xplt
 Keywords: python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `xplt-0.4.0/xplt.egg-info/SOURCES.txt` & `xplt-0.4.1/xplt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .gitignore
 .pre-commit-config.yaml
+CITATION.cff
 README.md
 pyproject.toml
 .github/sampleplot.png
 .github/workflows/qa.yaml
 .github/workflows/release.yaml
 .github/workflows/test.yaml
 docs/Makefile
```

