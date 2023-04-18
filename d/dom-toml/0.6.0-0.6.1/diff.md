# Comparing `tmp/dom_toml-0.6.0.tar.gz` & `tmp/dom_toml-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dom_toml-0.6.0.tar", last modified: Thu Apr 28 21:20:32 2022, max compression
+gzip compressed data, was "dom_toml-0.6.1.tar", last modified: Tue Apr 18 15:09:57 2023, max compression
```

## Comparing `dom_toml-0.6.0.tar` & `dom_toml-0.6.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2022-04-28 21:20:01.673102 dom_toml-0.6.0/LICENSE
--rw-r--r--   0        0        0     5069 2022-04-28 21:20:01.673102 dom_toml-0.6.0/README.rst
--rw-r--r--   0        0        0     6670 2022-04-28 21:20:01.673102 dom_toml-0.6.0/dom_toml/__init__.py
--rw-r--r--   0        0        0     1816 2022-04-28 21:20:01.673102 dom_toml-0.6.0/dom_toml/decoder.py
--rw-r--r--   0        0        0     5470 2022-04-28 21:20:01.673102 dom_toml-0.6.0/dom_toml/encoder.py
--rw-r--r--   0        0        0     7446 2022-04-28 21:20:01.673102 dom_toml-0.6.0/dom_toml/parser.py
--rw-r--r--   0        0        0        0 2022-04-28 21:20:01.673102 dom_toml-0.6.0/dom_toml/py.typed
--rw-r--r--   0        0        0     4480 2022-04-28 21:20:01.673102 dom_toml-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     6466 1970-01-01 00:00:00.000000 dom_toml-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-18 15:09:29.631723 dom_toml-0.6.1/LICENSE
+-rw-r--r--   0        0        0     5071 2023-04-18 15:09:29.631723 dom_toml-0.6.1/README.rst
+-rw-r--r--   0        0        0     6670 2023-04-18 15:09:29.631723 dom_toml-0.6.1/dom_toml/__init__.py
+-rw-r--r--   0        0        0     1816 2023-04-18 15:09:29.631723 dom_toml-0.6.1/dom_toml/decoder.py
+-rw-r--r--   0        0        0     5470 2023-04-18 15:09:29.631723 dom_toml-0.6.1/dom_toml/encoder.py
+-rw-r--r--   0        0        0     7446 2023-04-18 15:09:29.631723 dom_toml-0.6.1/dom_toml/parser.py
+-rw-r--r--   0        0        0        0 2023-04-18 15:09:29.631723 dom_toml-0.6.1/dom_toml/py.typed
+-rw-r--r--   0        0        0     4534 2023-04-18 15:09:29.631723 dom_toml-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6519 1970-01-01 00:00:00.000000 dom_toml-0.6.1/PKG-INFO
```

### Comparing `dom_toml-0.6.0/LICENSE` & `dom_toml-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dom_toml-0.6.0/README.rst` & `dom_toml-0.6.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/dom_toml/latest?logo=read-the-docs
-	:target: https://dom_toml.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/dom-toml/latest?logo=read-the-docs
+	:target: https://dom-toml.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/domdfcoding/dom_toml/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/domdfcoding/dom_toml/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/domdfcoding/dom_toml/workflows/Linux/badge.svg
@@ -54,16 +54,16 @@
 	:target: https://github.com/domdfcoding/dom_toml/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/dom_toml/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/dom_toml/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/dom_toml/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/dom_toml/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/dom_toml/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/dom_toml/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/dom_toml/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/dom_toml?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/dom_toml?logo=codefactor
@@ -97,23 +97,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/dom_toml
 	:target: https://github.com/domdfcoding/dom_toml/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/dom_toml
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/dom_toml/v0.6.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/dom_toml/v0.6.1
 	:target: https://github.com/domdfcoding/dom_toml/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/dom_toml
 	:target: https://github.com/domdfcoding/dom_toml/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/dom_toml
 	:target: https://pypi.org/project/dom_toml/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `dom_toml-0.6.0/dom_toml/__init__.py` & `dom_toml-0.6.1/dom_toml/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 # this package
 from dom_toml.encoder import TomlEncoder
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.6.0"
+__version__: str = "0.6.1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["TomlEncoder", "dumps", "loads", "dump", "load", "_M"]
 
 _M = TypeVar("_M", bound=MutableMapping[str, Any])
```

### Comparing `dom_toml-0.6.0/dom_toml/decoder.py` & `dom_toml-0.6.1/dom_toml/decoder.py`

 * *Files identical despite different names*

### Comparing `dom_toml-0.6.0/dom_toml/encoder.py` & `dom_toml-0.6.1/dom_toml/encoder.py`

 * *Files identical despite different names*

### Comparing `dom_toml-0.6.0/dom_toml/parser.py` & `dom_toml-0.6.1/dom_toml/parser.py`

 * *Files identical despite different names*

### Comparing `dom_toml-0.6.0/pyproject.toml` & `dom_toml-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "flit-core<4,>=3.2",]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "dom_toml"
-version = "0.6.0"
+version = "0.6.1"
 description = "Dom's tools for Tom's Obvious, Minimal Language."
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = [ "configuration", "serialize", "toml",]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -17,14 +17,15 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 dependencies = [ "domdf-python-tools>=2.8.0", "toml>=0.10.2",]
 dynamic = []
@@ -37,15 +38,15 @@
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/domdfcoding/dom_toml"
 "Issue Tracker" = "https://github.com/domdfcoding/dom_toml/issues"
 "Source Code" = "https://github.com/domdfcoding/dom_toml"
-Documentation = "https://dom_toml.readthedocs.io/en/latest"
+Documentation = "https://dom-toml.readthedocs.io/en/latest"
 
 [tool.mkrecipe]
 conda-channels = [ "conda-forge", "domdfcoding",]
 extras = "all"
 license-key = "MIT"
 
 [tool.sphinx-pyproject]
@@ -58,25 +59,25 @@
 package_root = "dom_toml"
 extensions = [
     "sphinx_toolbox",
     "sphinx_toolbox.more_autodoc",
     "sphinx_toolbox.more_autosummary",
     "sphinx_toolbox.documentation_summary",
     "sphinx_toolbox.tweaks.param_dash",
+    "sphinxcontrib.toctree_plus",
     "sphinx_toolbox.tweaks.latex_layout",
     "sphinx_toolbox.tweaks.latex_toc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinxcontrib.extras_require",
     "sphinx.ext.todo",
     "sphinxemoji.sphinxemoji",
     "notfound.extension",
     "sphinx_copybutton",
     "sphinxcontrib.default_values",
-    "sphinxcontrib.toctree_plus",
     "sphinx_debuginfo",
     "sphinx_licenseinfo",
     "seed_intersphinx_mapping",
     "html_section",
     "sphinx_toolbox.more_autosummary.column_widths",
 ]
 sphinxemoji_style = "twemoji"
@@ -131,21 +132,21 @@
 [tool.whey]
 base-classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 
 [tool.mypy]
-python_version = "3.6"
+python_version = "3.8"
 namespace_packages = true
 check_untyped_defs = true
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
 [tool.snippet-fmt]
```

### Comparing `dom_toml-0.6.0/PKG-INFO` & `dom_toml-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dom_toml
-Version: 0.6.0
+Version: 0.6.1
 Summary: Dom's tools for Tom's Obvious, Minimal Language.
 Keywords: configuration,serialize,toml
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,21 +13,22 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: domdf-python-tools>=2.8.0
 Requires-Dist: toml>=0.10.2
-Project-URL: Documentation, https://dom_toml.readthedocs.io/en/latest
+Project-URL: Documentation, https://dom-toml.readthedocs.io/en/latest
 Project-URL: Homepage, https://github.com/domdfcoding/dom_toml
 Project-URL: Issue Tracker, https://github.com/domdfcoding/dom_toml/issues
 Project-URL: Source Code, https://github.com/domdfcoding/dom_toml
 
 #########
 dom_toml
 #########
@@ -56,16 +57,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/dom_toml/latest?logo=read-the-docs
-	:target: https://dom_toml.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/dom-toml/latest?logo=read-the-docs
+	:target: https://dom-toml.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/domdfcoding/dom_toml/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/domdfcoding/dom_toml/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/domdfcoding/dom_toml/workflows/Linux/badge.svg
@@ -84,16 +85,16 @@
 	:target: https://github.com/domdfcoding/dom_toml/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/dom_toml/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/dom_toml/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/dom_toml/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/dom_toml/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/dom_toml/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/dom_toml/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/dom_toml/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/dom_toml?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/dom_toml?logo=codefactor
@@ -127,23 +128,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/dom_toml
 	:target: https://github.com/domdfcoding/dom_toml/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/dom_toml
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/dom_toml/v0.6.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/dom_toml/v0.6.1
 	:target: https://github.com/domdfcoding/dom_toml/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/dom_toml
 	:target: https://github.com/domdfcoding/dom_toml/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/dom_toml
 	:target: https://pypi.org/project/dom_toml/
 	:alt: PyPI - Downloads
 
 .. end shields
```

