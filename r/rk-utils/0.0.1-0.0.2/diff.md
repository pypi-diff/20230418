# Comparing `tmp/rk_utils-0.0.1.tar.gz` & `tmp/rk_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rk_utils-0.0.1.tar", last modified: Fri Apr 14 17:38:11 2023, max compression
+gzip compressed data, was "rk_utils-0.0.2.tar", last modified: Tue Apr 18 18:16:54 2023, max compression
```

## Comparing `rk_utils-0.0.1.tar` & `rk_utils-0.0.2.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:38:11.191089 rk_utils-0.0.1/
--rw-r--r--   0 root         (0) root         (0)      619 2023-04-14 16:00:06.000000 rk_utils-0.0.1/.coveragerc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:38:11.183089 rk_utils-0.0.1/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:38:11.187089 rk_utils-0.0.1/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 16:00:06.000000 rk_utils-0.0.1/.github/workflows/ci.yml
--rw-r--r--   0 root         (0) root         (0)      620 2023-04-14 16:00:06.000000 rk_utils-0.0.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)       59 2023-04-14 16:00:06.000000 rk_utils-0.0.1/.isort.cfg
--rw-r--r--   0 root         (0) root         (0)     1737 2023-04-14 16:19:52.000000 rk_utils-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      557 2023-04-14 16:00:06.000000 rk_utils-0.0.1/.readthedocs.yml
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-14 16:00:06.000000 rk_utils-0.0.1/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)      138 2023-04-14 16:00:06.000000 rk_utils-0.0.1/CHANGELOG.rst
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 16:00:06.000000 rk_utils-0.0.1/CONTRIBUTING.rst
--rw-r--r--   0 root         (0) root         (0)     1094 2023-04-14 16:00:07.000000 rk_utils-0.0.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     2547 2023-04-14 17:38:11.191089 rk_utils-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2147 2023-04-14 16:00:06.000000 rk_utils-0.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:38:11.187089 rk_utils-0.0.1/docs/
--rw-r--r--   0 root         (0) root         (0)     1183 2023-04-14 16:00:06.000000 rk_utils-0.0.1/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:38:11.187089 rk_utils-0.0.1/docs/_static/
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-14 16:00:06.000000 rk_utils-0.0.1/docs/_static/.gitignore
--rw-r--r--   0 root         (0) root         (0)       43 2023-04-14 16:00:06.000000 rk_utils-0.0.1/docs/authors.rst
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-14 16:00:06.000000 rk_utils-0.0.1/docs/changelog.rst
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 16:00:06.000000 rk_utils-0.0.1/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-14 16:00:06.000000 rk_utils-0.0.1/docs/contributing.rst
--rw-r--r--   0 root         (0) root         (0)     2378 2023-04-14 16:00:06.000000 rk_utils-0.0.1/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 16:00:06.000000 rk_utils-0.0.1/docs/license.rst
--rw-r--r--   0 root         (0) root         (0)       41 2023-04-14 16:00:06.000000 rk_utils-0.0.1/docs/readme.rst
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 16:00:06.000000 rk_utils-0.0.1/docs/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      355 2023-04-14 17:34:19.000000 rk_utils-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1197 2023-04-14 17:38:11.191089 rk_utils-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      724 2023-04-14 16:00:07.000000 rk_utils-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:38:11.183089 rk_utils-0.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:38:11.187089 rk_utils-0.0.1/src/rk_utils/
--rw-r--r--   0 root         (0) root         (0)      593 2023-04-14 16:00:07.000000 rk_utils-0.0.1/src/rk_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4247 2023-04-14 16:00:07.000000 rk_utils-0.0.1/src/rk_utils/skeleton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:38:11.191089 rk_utils-0.0.1/src/rk_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2547 2023-04-14 17:38:11.000000 rk_utils-0.0.1/src/rk_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      691 2023-04-14 17:38:11.000000 rk_utils-0.0.1/src/rk_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 17:38:11.000000 rk_utils-0.0.1/src/rk_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 17:38:10.000000 rk_utils-0.0.1/src/rk_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       86 2023-04-14 17:38:11.000000 rk_utils-0.0.1/src/rk_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-14 17:38:11.000000 rk_utils-0.0.1/src/rk_utils.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:38:11.191089 rk_utils-0.0.1/tests/
--rw-r--r--   0 root         (0) root         (0)      286 2023-04-14 16:00:07.000000 rk_utils-0.0.1/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)      598 2023-04-14 16:00:07.000000 rk_utils-0.0.1/tests/test_skeleton.py
--rw-r--r--   0 root         (0) root         (0)     2944 2023-04-14 16:00:07.000000 rk_utils-0.0.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 18:16:54.019843 rk_utils-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)      619 2023-04-18 17:07:48.000000 rk_utils-0.0.2/.coveragerc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 18:16:54.003843 rk_utils-0.0.2/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 18:16:54.015843 rk_utils-0.0.2/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 17:07:48.000000 rk_utils-0.0.2/.github/workflows/ci.yml
+-rw-r--r--   0 root         (0) root         (0)      620 2023-04-18 17:07:48.000000 rk_utils-0.0.2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)       59 2023-04-18 17:07:48.000000 rk_utils-0.0.2/.isort.cfg
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-04-18 17:07:48.000000 rk_utils-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      557 2023-04-18 17:07:48.000000 rk_utils-0.0.2/.readthedocs.yml
+-rw-r--r--   0 root         (0) root         (0)       76 2023-04-18 17:07:48.000000 rk_utils-0.0.2/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)      138 2023-04-18 17:07:48.000000 rk_utils-0.0.2/CHANGELOG.rst
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 17:07:48.000000 rk_utils-0.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-04-18 17:07:48.000000 rk_utils-0.0.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     3000 2023-04-18 18:16:54.027843 rk_utils-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2611 2023-04-18 18:07:12.000000 rk_utils-0.0.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 18:16:54.019843 rk_utils-0.0.2/docs/
+-rw-r--r--   0 root         (0) root         (0)     1183 2023-04-18 17:07:48.000000 rk_utils-0.0.2/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 18:16:54.019843 rk_utils-0.0.2/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-18 17:07:48.000000 rk_utils-0.0.2/docs/_static/.gitignore
+-rw-r--r--   0 root         (0) root         (0)       43 2023-04-18 17:07:48.000000 rk_utils-0.0.2/docs/authors.rst
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-18 17:07:48.000000 rk_utils-0.0.2/docs/changelog.rst
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 17:07:48.000000 rk_utils-0.0.2/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-18 17:07:48.000000 rk_utils-0.0.2/docs/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-04-18 17:07:48.000000 rk_utils-0.0.2/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 17:07:48.000000 rk_utils-0.0.2/docs/license.rst
+-rw-r--r--   0 root         (0) root         (0)       41 2023-04-18 17:07:48.000000 rk_utils-0.0.2/docs/readme.rst
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 17:07:48.000000 rk_utils-0.0.2/docs/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      355 2023-04-18 17:07:48.000000 rk_utils-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-18 17:30:48.000000 rk_utils-0.0.2/requirements_dev.txt
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-04-18 18:16:54.027843 rk_utils-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      724 2023-04-18 17:07:48.000000 rk_utils-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 18:16:54.007843 rk_utils-0.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 18:16:54.019843 rk_utils-0.0.2/src/rk_utils/
+-rw-r--r--   0 root         (0) root         (0)      593 2023-04-18 17:07:48.000000 rk_utils-0.0.2/src/rk_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4247 2023-04-18 17:07:48.000000 rk_utils-0.0.2/src/rk_utils/skeleton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 18:16:54.019843 rk_utils-0.0.2/src/rk_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3000 2023-04-18 18:16:53.000000 rk_utils-0.0.2/src/rk_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      712 2023-04-18 18:16:53.000000 rk_utils-0.0.2/src/rk_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 18:16:53.000000 rk_utils-0.0.2/src/rk_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 18:16:53.000000 rk_utils-0.0.2/src/rk_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       86 2023-04-18 18:16:53.000000 rk_utils-0.0.2/src/rk_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-18 18:16:53.000000 rk_utils-0.0.2/src/rk_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 18:16:54.019843 rk_utils-0.0.2/tests/
+-rw-r--r--   0 root         (0) root         (0)      286 2023-04-18 17:07:48.000000 rk_utils-0.0.2/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)      598 2023-04-18 17:07:48.000000 rk_utils-0.0.2/tests/test_skeleton.py
+-rw-r--r--   0 root         (0) root         (0)     2985 2023-04-18 18:00:45.000000 rk_utils-0.0.2/tox.ini
```

### Comparing `rk_utils-0.0.1/.coveragerc` & `rk_utils-0.0.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `rk_utils-0.0.1/.gitignore` & `rk_utils-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rk_utils-0.0.1/.pre-commit-config.yaml` & `rk_utils-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rk_utils-0.0.1/.readthedocs.yml` & `rk_utils-0.0.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `rk_utils-0.0.1/LICENSE.txt` & `rk_utils-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rk_utils-0.0.1/PKG-INFO` & `rk_utils-0.0.2/src/rk_utils.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rk_utils
-Version: 0.0.1
+Name: rk-utils
+Version: 0.0.2
 Summary: Some useful Python utilities made by RKWS.
 Home-page: https://github.com/opposj/Rk-Utils
 Author: opposj
 Author-email: 18965385801@163.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -57,27 +57,38 @@
 
 
 .. _pyscaffold-notes:
 
 Making Changes & Contributing
 =============================
 
-This project uses `pre-commit`_, please make sure to install it before making any
-changes::
+For developers, extra requirements are in `requirements_dev.txt`::
 
-    pip install pre-commit
     cd rk_utils
-    pre-commit install
+    pip install -r requirements_dev.txt
 
-It is a good idea to update the hooks to the latest version::
+This project uses `pre-commit`_, and it is a good idea to update the hooks to
+the latest version before installing::
 
+    cd rk_utils
     pre-commit autoupdate
-
-Don't forget to tell your contributors to also install and use pre-commit.
+    pre-commit install
 
 .. _pre-commit: https://pre-commit.com/
 
+There are some useful `tox`_ commands that can be used to simplify developing::
+
+    cd rk_utils
+    tox  # to run all the tests
+    tox -e docs  # to build your documentation
+    tox -e build  # to build your package distribution
+    tox -e publish  # to test your project uploads correctly in test.pypi.org
+    tox -e publish -- --repository pypi  # to release your package to PyPI
+    tox -av  # to list all the tasks available
+
+.. _tox: https://tox.readthedocs.io/
+
 Note
 ====
 
 This project has been set up using PyScaffold 4.4. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `rk_utils-0.0.1/README.rst` & `rk_utils-0.0.2/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -41,27 +41,38 @@
 
 
 .. _pyscaffold-notes:
 
 Making Changes & Contributing
 =============================
 
-This project uses `pre-commit`_, please make sure to install it before making any
-changes::
+For developers, extra requirements are in `requirements_dev.txt`::
 
-    pip install pre-commit
     cd rk_utils
-    pre-commit install
+    pip install -r requirements_dev.txt
 
-It is a good idea to update the hooks to the latest version::
+This project uses `pre-commit`_, and it is a good idea to update the hooks to
+the latest version before installing::
 
+    cd rk_utils
     pre-commit autoupdate
-
-Don't forget to tell your contributors to also install and use pre-commit.
+    pre-commit install
 
 .. _pre-commit: https://pre-commit.com/
 
+There are some useful `tox`_ commands that can be used to simplify developing::
+
+    cd rk_utils
+    tox  # to run all the tests
+    tox -e docs  # to build your documentation
+    tox -e build  # to build your package distribution
+    tox -e publish  # to test your project uploads correctly in test.pypi.org
+    tox -e publish -- --repository pypi  # to release your package to PyPI
+    tox -av  # to list all the tasks available
+
+.. _tox: https://tox.readthedocs.io/
+
 Note
 ====
 
 This project has been set up using PyScaffold 4.4. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `rk_utils-0.0.1/docs/Makefile` & `rk_utils-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rk_utils-0.0.1/docs/index.rst` & `rk_utils-0.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rk_utils-0.0.1/setup.cfg` & `rk_utils-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `rk_utils-0.0.1/setup.py` & `rk_utils-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `rk_utils-0.0.1/src/rk_utils/__init__.py` & `rk_utils-0.0.2/src/rk_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rk_utils-0.0.1/src/rk_utils/skeleton.py` & `rk_utils-0.0.2/src/rk_utils/skeleton.py`

 * *Files identical despite different names*

### Comparing `rk_utils-0.0.1/src/rk_utils.egg-info/PKG-INFO` & `rk_utils-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rk-utils
-Version: 0.0.1
+Name: rk_utils
+Version: 0.0.2
 Summary: Some useful Python utilities made by RKWS.
 Home-page: https://github.com/opposj/Rk-Utils
 Author: opposj
 Author-email: 18965385801@163.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -57,27 +57,38 @@
 
 
 .. _pyscaffold-notes:
 
 Making Changes & Contributing
 =============================
 
-This project uses `pre-commit`_, please make sure to install it before making any
-changes::
+For developers, extra requirements are in `requirements_dev.txt`::
 
-    pip install pre-commit
     cd rk_utils
-    pre-commit install
+    pip install -r requirements_dev.txt
 
-It is a good idea to update the hooks to the latest version::
+This project uses `pre-commit`_, and it is a good idea to update the hooks to
+the latest version before installing::
 
+    cd rk_utils
     pre-commit autoupdate
-
-Don't forget to tell your contributors to also install and use pre-commit.
+    pre-commit install
 
 .. _pre-commit: https://pre-commit.com/
 
+There are some useful `tox`_ commands that can be used to simplify developing::
+
+    cd rk_utils
+    tox  # to run all the tests
+    tox -e docs  # to build your documentation
+    tox -e build  # to build your package distribution
+    tox -e publish  # to test your project uploads correctly in test.pypi.org
+    tox -e publish -- --repository pypi  # to release your package to PyPI
+    tox -av  # to list all the tasks available
+
+.. _tox: https://tox.readthedocs.io/
+
 Note
 ====
 
 This project has been set up using PyScaffold 4.4. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `rk_utils-0.0.1/src/rk_utils.egg-info/SOURCES.txt` & `rk_utils-0.0.2/src/rk_utils.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 .readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE.txt
 README.rst
 pyproject.toml
+requirements_dev.txt
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/ci.yml
 docs/Makefile
 docs/authors.rst
 docs/changelog.rst
```

### Comparing `rk_utils-0.0.1/tests/test_skeleton.py` & `rk_utils-0.0.2/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `rk_utils-0.0.1/tox.ini` & `rk_utils-0.0.2/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,16 @@
     BUILDDIR = {toxinidir}/docs/_build
     docs: BUILD = html
     doctests: BUILD = doctest
     linkcheck: BUILD = linkcheck
 deps =
     -r {toxinidir}/docs/requirements.txt
     # ^  requirements.txt shared with Read The Docs
+allowlist_externals =
+    sphinx-build
 commands =
     sphinx-build --color -b {env:BUILD} -d "{env:BUILDDIR}/doctrees" "{env:DOCSDIR}" "{env:BUILDDIR}/{env:BUILD}" {posargs}
 
 
 [testenv:publish]
 description =
     Publish the package you have been developing to a package index server.
```

