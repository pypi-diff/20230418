# Comparing `tmp/repo_helper_sphinx_theme-0.0.2.tar.gz` & `tmp/repo_helper_sphinx_theme-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/repo_helper_sphinx_theme-0.0.2.tar", last modified: Thu Jul 30 08:06:11 2020, max compression
+gzip compressed data, was "repo_helper_sphinx_theme-0.0.3.tar", last modified: Tue Apr 18 18:13:44 2023, max compression
```

## Comparing `repo_helper_sphinx_theme-0.0.2.tar` & `repo_helper_sphinx_theme-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,12 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-30 08:06:11.000000 repo_helper_sphinx_theme-0.0.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)      287 2020-07-30 08:05:45.000000 repo_helper_sphinx_theme-0.0.2/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2020-07-30 08:05:45.000000 repo_helper_sphinx_theme-0.0.2/requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-30 08:06:11.000000 repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6612 2020-07-30 08:06:11.000000 repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-30 08:06:11.000000 repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       25 2020-07-30 08:06:11.000000 repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-30 08:06:11.000000 repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      718 2020-07-30 08:06:11.000000 repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       31 2020-07-30 08:06:11.000000 repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       74 2020-07-30 08:06:11.000000 repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     6612 2020-07-30 08:06:11.000000 repo_helper_sphinx_theme-0.0.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1752 2020-07-30 08:05:45.000000 repo_helper_sphinx_theme-0.0.2/__pkginfo__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1300 2020-07-30 08:06:11.000000 repo_helper_sphinx_theme-0.0.2/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-30 08:06:11.000000 repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-30 08:06:11.000000 repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme/static/
--rw-rw-r--   0 travis    (2000) travis    (2000)       42 2020-07-30 08:05:45.000000 repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme/static/custom.css
--rw-rw-r--   0 travis    (2000) travis    (2000)      846 2020-07-30 08:05:45.000000 repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme/static/header.js
--rw-rw-r--   0 travis    (2000) travis    (2000)    20176 2020-07-30 08:05:45.000000 repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme/static/repo_helper.css_t
--rw-rw-r--   0 travis    (2000) travis    (2000)     2407 2020-07-30 08:05:45.000000 repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme/theme.conf
--rw-rw-r--   0 travis    (2000) travis    (2000)      621 2020-07-30 08:05:45.000000 repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme/relations.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4213 2020-07-30 08:05:45.000000 repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme/layout.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     2644 2020-07-30 08:05:45.000000 repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1719 2020-07-30 08:05:45.000000 repo_helper_sphinx_theme-0.0.2/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     4369 2020-07-30 08:05:45.000000 repo_helper_sphinx_theme-0.0.2/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      123 2020-07-30 08:05:45.000000 repo_helper_sphinx_theme-0.0.2/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      516 2020-07-30 08:05:45.000000 repo_helper_sphinx_theme-0.0.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6390 2023-04-18 18:13:44.365505 repo_helper_sphinx_theme-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4715 2023-04-18 18:13:44.365505 repo_helper_sphinx_theme-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1719 2023-04-18 18:13:44.357505 repo_helper_sphinx_theme-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4857 2023-04-18 18:13:44.365505 repo_helper_sphinx_theme-0.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-18 18:13:44.365505 repo_helper_sphinx_theme-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2407 2023-04-18 18:13:12.793400 repo_helper_sphinx_theme-0.0.3/repo_helper_sphinx_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-04-18 18:13:12.789400 repo_helper_sphinx_theme-0.0.3/repo_helper_sphinx_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4213 2023-04-18 18:13:12.789400 repo_helper_sphinx_theme-0.0.3/repo_helper_sphinx_theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-04-18 18:13:12.793400 repo_helper_sphinx_theme-0.0.3/repo_helper_sphinx_theme/relations.html
+-rw-r--r--   0 runner    (1001) docker     (122)      846 2023-04-18 18:13:12.793400 repo_helper_sphinx_theme-0.0.3/repo_helper_sphinx_theme/static/header.js
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-18 18:13:12.793400 repo_helper_sphinx_theme-0.0.3/repo_helper_sphinx_theme/static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (122)    20176 2023-04-18 18:13:12.793400 repo_helper_sphinx_theme-0.0.3/repo_helper_sphinx_theme/static/repo_helper.css_t
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme/static/header.js` & `repo_helper_sphinx_theme-0.0.3/repo_helper_sphinx_theme/static/header.js`

 * *Files identical despite different names*

### Comparing `repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme/static/repo_helper.css_t` & `repo_helper_sphinx_theme-0.0.3/repo_helper_sphinx_theme/static/repo_helper.css_t`

 * *Files identical despite different names*

### Comparing `repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme/theme.conf` & `repo_helper_sphinx_theme-0.0.3/repo_helper_sphinx_theme/theme.conf`

 * *Files identical despite different names*

### Comparing `repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme/relations.html` & `repo_helper_sphinx_theme-0.0.3/repo_helper_sphinx_theme/relations.html`

 * *Files identical despite different names*

### Comparing `repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme/layout.html` & `repo_helper_sphinx_theme-0.0.3/repo_helper_sphinx_theme/layout.html`

 * *Files identical despite different names*

### Comparing `repo_helper_sphinx_theme-0.0.2/repo_helper_sphinx_theme/__init__.py` & `repo_helper_sphinx_theme-0.0.3/repo_helper_sphinx_theme/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,33 +38,40 @@
 #  LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 #  NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 #  SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
 # stdlib
 import os
+from typing import Any, Dict
 
 # 3rd party
 import alabaster  # type: ignore
-from alabaster import get_path, update_context  # type: ignore
+from alabaster import get_path, update_context
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
-
 __license__: str = "BSD"
-__version__: str = "0.0.2"
+__version__: str = "0.0.3"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["get_path", "update_context", "setup"]
 
 
-def setup(app):
-	# add_html_theme is new in Sphinx 1.6+
+def setup(app) -> Dict[str, Any]:
+	"""
+	Setup Sphinx app.
+
+	:param app:
+	"""
+
 	alabaster.setup(app)
-	if hasattr(app, "add_html_theme"):
-		theme_path = os.path.abspath(os.path.dirname(__file__))
-		app.add_html_theme("repo_helper_sphinx_theme", theme_path)
+
+	theme_path = os.path.abspath(os.path.dirname(__file__))
+	app.add_html_theme("repo_helper_sphinx_theme", theme_path)
+
 	app.connect("html-page-context", update_context)
+
 	return {
 			"version": __version__,
 			"parallel_read_safe": True,
 			}
```

### Comparing `repo_helper_sphinx_theme-0.0.2/LICENSE` & `repo_helper_sphinx_theme-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `repo_helper_sphinx_theme-0.0.2/README.rst` & `repo_helper_sphinx_theme-0.0.3/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -15,48 +15,58 @@
 .. list-table::
 	:stub-columns: 1
 	:widths: 10 90
 
 	* - Docs
 	  - |docs| |docs_check|
 	* - Tests
-	  - |travis| |actions_windows| |actions_macos| |codefactor|
+	  - |actions_linux| |actions_windows| |actions_macos|
 	* - PyPI
 	  - |pypi-version| |supported-versions| |supported-implementations| |wheel|
 	* - Activity
-	  - |commits-latest| |commits-since| |maintained|
+	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
+	* - QA
+	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
-	  - |license| |language| |requires| |pre_commit|
+	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/repo_helper_sphinx_theme/latest?logo=read-the-docs
-	:target: https://repo_helper_sphinx_theme.readthedocs.io/en/latest/?badge=latest
-	:alt: Documentation Status
+.. |docs| image:: https://img.shields.io/readthedocs/repo-helper-sphinx-theme/latest?logo=read-the-docs
+	:target: https://repo-helper-sphinx-theme.readthedocs.io/en/latest
+	:alt: Documentation Build Status
 
-.. |docs_check| image:: https://github.com/domdfcoding/repo_helper_sphinx_theme/workflows/Docs%20Check/badge.svg
-	:target: https://github.com/domdfcoding/repo_helper_sphinx_theme/actions?query=workflow%3A%22Docs+Check%22
+.. |docs_check| image:: https://github.com/repo-helper/repo_helper_sphinx_theme/workflows/Docs%20Check/badge.svg
+	:target: https://github.com/repo-helper/repo_helper_sphinx_theme/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
-.. |travis| image:: https://img.shields.io/travis/com/domdfcoding/repo_helper_sphinx_theme/master?logo=travis
-	:target: https://travis-ci.com/domdfcoding/repo_helper_sphinx_theme
-	:alt: Travis Build Status
-
-.. |actions_windows| image:: https://github.com/domdfcoding/repo_helper_sphinx_theme/workflows/Windows%20Tests/badge.svg
-	:target: https://github.com/domdfcoding/repo_helper_sphinx_theme/actions?query=workflow%3A%22Windows+Tests%22
-	:alt: Windows Tests Status
-
-.. |actions_macos| image:: https://github.com/domdfcoding/repo_helper_sphinx_theme/workflows/macOS%20Tests/badge.svg
-	:target: https://github.com/domdfcoding/repo_helper_sphinx_theme/actions?query=workflow%3A%22macOS+Tests%22
-	:alt: macOS Tests Status
+.. |actions_linux| image:: https://github.com/repo-helper/repo_helper_sphinx_theme/workflows/Linux/badge.svg
+	:target: https://github.com/repo-helper/repo_helper_sphinx_theme/actions?query=workflow%3A%22Linux%22
+	:alt: Linux Test Status
+
+.. |actions_windows| image:: https://github.com/repo-helper/repo_helper_sphinx_theme/workflows/Windows/badge.svg
+	:target: https://github.com/repo-helper/repo_helper_sphinx_theme/actions?query=workflow%3A%22Windows%22
+	:alt: Windows Test Status
+
+.. |actions_macos| image:: https://github.com/repo-helper/repo_helper_sphinx_theme/workflows/macOS/badge.svg
+	:target: https://github.com/repo-helper/repo_helper_sphinx_theme/actions?query=workflow%3A%22macOS%22
+	:alt: macOS Test Status
+
+.. |actions_flake8| image:: https://github.com/repo-helper/repo_helper_sphinx_theme/workflows/Flake8/badge.svg
+	:target: https://github.com/repo-helper/repo_helper_sphinx_theme/actions?query=workflow%3A%22Flake8%22
+	:alt: Flake8 Status
+
+.. |actions_mypy| image:: https://github.com/repo-helper/repo_helper_sphinx_theme/workflows/mypy/badge.svg
+	:target: https://github.com/repo-helper/repo_helper_sphinx_theme/actions?query=workflow%3A%22mypy%22
+	:alt: mypy status
 
-.. |requires| image:: https://requires.io/github/domdfcoding/repo_helper_sphinx_theme/requirements.svg?branch=master
-	:target: https://requires.io/github/domdfcoding/repo_helper_sphinx_theme/requirements/?branch=master
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/repo-helper/repo_helper_sphinx_theme/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/repo-helper/repo_helper_sphinx_theme/
 	:alt: Requirements Status
 
-.. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/repo_helper_sphinx_theme?logo=codefactor
-	:target: https://www.codefactor.io/repository/github/domdfcoding/repo_helper_sphinx_theme
+.. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/repo_helper_sphinx_theme?logo=codefactor
+	:target: https://www.codefactor.io/repository/github/repo-helper/repo_helper_sphinx_theme
 	:alt: CodeFactor Grade
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/repo_helper_sphinx_theme
 	:target: https://pypi.org/project/repo_helper_sphinx_theme/
 	:alt: PyPI - Package Version
 
 .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/repo_helper_sphinx_theme?logo=python&logoColor=white
@@ -67,35 +77,35 @@
 	:target: https://pypi.org/project/repo_helper_sphinx_theme/
 	:alt: PyPI - Supported Implementations
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/repo_helper_sphinx_theme
 	:target: https://pypi.org/project/repo_helper_sphinx_theme/
 	:alt: PyPI - Wheel
 
-.. |license| image:: https://img.shields.io/github/license/domdfcoding/repo_helper_sphinx_theme
-	:target: https://github.com/domdfcoding/repo_helper_sphinx_theme/blob/master/LICENSE
+.. |license| image:: https://img.shields.io/github/license/repo-helper/repo_helper_sphinx_theme
+	:target: https://github.com/repo-helper/repo_helper_sphinx_theme/blob/master/LICENSE
 	:alt: License
 
-.. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/repo_helper_sphinx_theme
+.. |language| image:: https://img.shields.io/github/languages/top/repo-helper/repo_helper_sphinx_theme
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/repo_helper_sphinx_theme/v0.0.2
-	:target: https://github.com/domdfcoding/repo_helper_sphinx_theme/pulse
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/repo_helper_sphinx_theme/v0.0.3
+	:target: https://github.com/repo-helper/repo_helper_sphinx_theme/pulse
 	:alt: GitHub commits since tagged version
 
-.. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/repo_helper_sphinx_theme
-	:target: https://github.com/domdfcoding/repo_helper_sphinx_theme/commit/master
+.. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/repo_helper_sphinx_theme
+	:target: https://github.com/repo-helper/repo_helper_sphinx_theme/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2020
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
-.. |pre_commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
-	:target: https://github.com/pre-commit/pre-commit
-	:alt: pre-commit
+.. |pypi-downloads| image:: https://img.shields.io/pypi/dm/repo_helper_sphinx_theme
+	:target: https://pypi.org/project/repo_helper_sphinx_theme/
+	:alt: PyPI - Downloads
 
 .. end shields
 
 |
 
 Installation
 --------------
```

