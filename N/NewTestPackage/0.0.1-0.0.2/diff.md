# Comparing `tmp/NewTestPackage-0.0.1.tar.gz` & `tmp/NewTestPackage-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NewTestPackage-0.0.1.tar", last modified: Mon Apr 17 13:16:05 2023, max compression
+gzip compressed data, was "NewTestPackage-0.0.2.tar", last modified: Tue Apr 18 15:55:08 2023, max compression
```

## Comparing `NewTestPackage-0.0.1.tar` & `NewTestPackage-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 13:16:05.823580 NewTestPackage-0.0.1/
--rw-rw-rw-   0        0        0     1086 2023-04-17 13:06:35.000000 NewTestPackage-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-17 13:06:35.000000 NewTestPackage-0.0.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-04-17 13:16:05.807957 NewTestPackage-0.0.1/NewTestPackage.egg-info/
--rw-rw-rw-   0        0        0     1399 2023-04-17 13:16:03.000000 NewTestPackage-0.0.1/NewTestPackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-04-17 13:16:03.000000 NewTestPackage-0.0.1/NewTestPackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 13:16:03.000000 NewTestPackage-0.0.1/NewTestPackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 13:16:03.000000 NewTestPackage-0.0.1/NewTestPackage.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-04-17 13:16:03.000000 NewTestPackage-0.0.1/NewTestPackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1399 2023-04-17 13:16:05.823580 NewTestPackage-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      608 2023-04-17 13:06:35.000000 NewTestPackage-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 13:16:05.823580 NewTestPackage-0.0.1/newtestpackage/
--rw-rw-rw-   0        0        0      143 2023-04-17 13:06:35.000000 NewTestPackage-0.0.1/newtestpackage/__init__.py
--rw-rw-rw-   0        0        0       20 2023-04-17 13:06:35.000000 NewTestPackage-0.0.1/newtestpackage/newtestpackage.py
--rw-rw-rw-   0        0        0        0 2023-04-17 13:06:35.000000 NewTestPackage-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0      422 2023-04-17 13:16:05.839206 NewTestPackage-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1819 2023-04-17 13:06:35.000000 NewTestPackage-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:55:08.595932 NewTestPackage-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-18 15:54:57.000000 NewTestPackage-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-18 15:54:57.000000 NewTestPackage-0.0.2/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:55:08.595932 NewTestPackage-0.0.2/NewTestPackage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-18 15:55:08.000000 NewTestPackage-0.0.2/NewTestPackage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-18 15:55:08.000000 NewTestPackage-0.0.2/NewTestPackage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:55:08.000000 NewTestPackage-0.0.2/NewTestPackage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:55:08.000000 NewTestPackage-0.0.2/NewTestPackage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 15:55:08.000000 NewTestPackage-0.0.2/NewTestPackage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-18 15:55:08.595932 NewTestPackage-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-18 15:54:57.000000 NewTestPackage-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:55:08.595932 NewTestPackage-0.0.2/newtestpackage/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-18 15:54:57.000000 NewTestPackage-0.0.2/newtestpackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 15:54:57.000000 NewTestPackage-0.0.2/newtestpackage/newtestpackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:54:57.000000 NewTestPackage-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-18 15:55:08.595932 NewTestPackage-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-18 15:54:57.000000 NewTestPackage-0.0.2/setup.py
```

### Comparing `NewTestPackage-0.0.1/NewTestPackage.egg-info/PKG-INFO` & `NewTestPackage-0.0.2/NewTestPackage.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 2.1
-Name: NewTestPackage
-Version: 0.0.1
-Summary: to just test geo 
-Home-page: https://github.com/Maherhassanali/NewTestPackage
-Author: maher
-Author-email: maherarmoongisanalyst@gmail.com
-License: MIT license
-Keywords: newtestpackage
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# NewTestPackage
-
-
-[![image](https://img.shields.io/pypi/v/NewTestPackage.svg)](https://pypi.python.org/pypi/NewTestPackage)
-[![image](https://img.shields.io/conda/vn/conda-forge/NewTestPackage.svg)](https://anaconda.org/conda-forge/NewTestPackage)
-
-
-**to just test geo **
-
-
--   Free software: MIT license
--   Documentation: https://Maherhassanali.github.io/NewTestPackage
-    
-
-## Features
-
--   TODO
-
-## Credits
-
-This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
+Metadata-Version: 2.1
+Name: NewTestPackage
+Version: 0.0.2
+Summary: to just test geo 
+Home-page: https://github.com/Maherhassanali/NewTestPackage
+Author: maher
+Author-email: maherarmoongisanalyst@gmail.com
+License: MIT license
+Keywords: newtestpackage
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# NewTestPackage
+
+
+[![image](https://img.shields.io/pypi/v/NewTestPackage.svg)](https://pypi.python.org/pypi/NewTestPackage)
+[![image](https://img.shields.io/conda/vn/conda-forge/NewTestPackage.svg)](https://anaconda.org/conda-forge/NewTestPackage)
+
+
+**to just test geo **
+
+
+-   Free software: MIT license
+-   Documentation: https://Maherhassanali.github.io/NewTestPackage
+    
+
+## Features
+
+-   TODO
+
+## Credits
+
+This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `NewTestPackage-0.0.1/PKG-INFO` & `NewTestPackage-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 2.1
-Name: NewTestPackage
-Version: 0.0.1
-Summary: to just test geo 
-Home-page: https://github.com/Maherhassanali/NewTestPackage
-Author: maher
-Author-email: maherarmoongisanalyst@gmail.com
-License: MIT license
-Keywords: newtestpackage
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# NewTestPackage
-
-
-[![image](https://img.shields.io/pypi/v/NewTestPackage.svg)](https://pypi.python.org/pypi/NewTestPackage)
-[![image](https://img.shields.io/conda/vn/conda-forge/NewTestPackage.svg)](https://anaconda.org/conda-forge/NewTestPackage)
-
-
-**to just test geo **
-
-
--   Free software: MIT license
--   Documentation: https://Maherhassanali.github.io/NewTestPackage
-    
-
-## Features
-
--   TODO
-
-## Credits
-
-This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
+Metadata-Version: 2.1
+Name: NewTestPackage
+Version: 0.0.2
+Summary: to just test geo 
+Home-page: https://github.com/Maherhassanali/NewTestPackage
+Author: maher
+Author-email: maherarmoongisanalyst@gmail.com
+License: MIT license
+Keywords: newtestpackage
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# NewTestPackage
+
+
+[![image](https://img.shields.io/pypi/v/NewTestPackage.svg)](https://pypi.python.org/pypi/NewTestPackage)
+[![image](https://img.shields.io/conda/vn/conda-forge/NewTestPackage.svg)](https://anaconda.org/conda-forge/NewTestPackage)
+
+
+**to just test geo **
+
+
+-   Free software: MIT license
+-   Documentation: https://Maherhassanali.github.io/NewTestPackage
+    
+
+## Features
+
+-   TODO
+
+## Credits
+
+This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `NewTestPackage-0.0.1/README.md` & `NewTestPackage-0.0.2/README.md`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# NewTestPackage
-
-
-[![image](https://img.shields.io/pypi/v/NewTestPackage.svg)](https://pypi.python.org/pypi/NewTestPackage)
-[![image](https://img.shields.io/conda/vn/conda-forge/NewTestPackage.svg)](https://anaconda.org/conda-forge/NewTestPackage)
-
-
-**to just test geo **
-
-
--   Free software: MIT license
--   Documentation: https://Maherhassanali.github.io/NewTestPackage
-    
-
-## Features
-
--   TODO
-
-## Credits
-
-This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
+# NewTestPackage
+
+
+[![image](https://img.shields.io/pypi/v/NewTestPackage.svg)](https://pypi.python.org/pypi/NewTestPackage)
+[![image](https://img.shields.io/conda/vn/conda-forge/NewTestPackage.svg)](https://anaconda.org/conda-forge/NewTestPackage)
+
+
+**to just test geo **
+
+
+-   Free software: MIT license
+-   Documentation: https://Maherhassanali.github.io/NewTestPackage
+    
+
+## Features
+
+-   TODO
+
+## Credits
+
+This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

