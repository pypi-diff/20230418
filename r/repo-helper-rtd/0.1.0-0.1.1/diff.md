# Comparing `tmp/repo_helper_rtd-0.1.0.tar.gz` & `tmp/repo_helper_rtd-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpox8_rwp9/tmpcpdn4ebi/repo_helper_rtd-0.1.0.tar", last modified: Fri Dec 11 09:23:30 2020, max compression
+gzip compressed data, was "repo_helper_rtd-0.1.1.tar", last modified: Tue Apr 18 18:29:40 2023, max compression
```

## Comparing `repo_helper_rtd-0.1.0.tar` & `repo_helper_rtd-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-11 09:23:30.347713 repo_helper_rtd-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (116)     1064 2020-12-11 09:23:06.000000 repo_helper_rtd-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      158 2020-12-11 09:23:06.000000 repo_helper_rtd-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     6378 2020-12-11 09:23:30.347713 repo_helper_rtd-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4262 2020-12-11 09:23:06.000000 repo_helper_rtd-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1016 2020-12-11 09:23:06.000000 repo_helper_rtd-0.1.0/__pkginfo__.py
--rw-r--r--   0 runner    (1001) docker     (116)      106 2020-12-11 09:23:06.000000 repo_helper_rtd-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-11 09:23:30.343713 repo_helper_rtd-0.1.0/repo_helper_rtd/
--rw-r--r--   0 runner    (1001) docker     (116)     4226 2020-12-11 09:23:06.000000 repo_helper_rtd-0.1.0/repo_helper_rtd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2935 2020-12-11 09:23:06.000000 repo_helper_rtd-0.1.0/repo_helper_rtd/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     2222 2020-12-11 09:23:06.000000 repo_helper_rtd-0.1.0/repo_helper_rtd/options.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-11 09:23:30.347713 repo_helper_rtd-0.1.0/repo_helper_rtd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     6378 2020-12-11 09:23:30.000000 repo_helper_rtd-0.1.0/repo_helper_rtd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      448 2020-12-11 09:23:30.000000 repo_helper_rtd-0.1.0/repo_helper_rtd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-11 09:23:30.000000 repo_helper_rtd-0.1.0/repo_helper_rtd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       65 2020-12-11 09:23:30.000000 repo_helper_rtd-0.1.0/repo_helper_rtd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-11 09:23:29.000000 repo_helper_rtd-0.1.0/repo_helper_rtd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      117 2020-12-11 09:23:30.000000 repo_helper_rtd-0.1.0/repo_helper_rtd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2020-12-11 09:23:30.000000 repo_helper_rtd-0.1.0/repo_helper_rtd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      110 2020-12-11 09:23:06.000000 repo_helper_rtd-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1391 2020-12-11 09:23:30.347713 repo_helper_rtd-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      439 2020-12-11 09:23:06.000000 repo_helper_rtd-0.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5832 2023-04-18 18:29:40.462445 repo_helper_rtd-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4322 2023-04-18 18:29:40.458445 repo_helper_rtd-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-04-18 18:29:40.454445 repo_helper_rtd-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4425 2023-04-18 18:29:40.462445 repo_helper_rtd-0.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-04-18 18:29:40.458445 repo_helper_rtd-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3937 2023-04-18 18:29:09.802640 repo_helper_rtd-0.1.1/repo_helper_rtd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-04-18 18:29:09.802640 repo_helper_rtd-0.1.1/repo_helper_rtd/options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3020 2023-04-18 18:29:09.802640 repo_helper_rtd-0.1.1/repo_helper_rtd/cli.py
```

### Comparing `repo_helper_rtd-0.1.0/LICENSE` & `repo_helper_rtd-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `repo_helper_rtd-0.1.0/README.rst` & `repo_helper_rtd-0.1.1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -14,44 +14,54 @@
 .. list-table::
 	:stub-columns: 1
 	:widths: 10 90
 
 	* - Docs
 	  - |docs| |docs_check|
 	* - Tests
-	  - |travis| |actions_windows| |actions_macos| |codefactor| |pre_commit_ci|
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
 
-.. |docs| image:: https://img.shields.io/readthedocs/repo_helper_rtd/latest?logo=read-the-docs
-	:target: https://repo_helper_rtd.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/repo-helper-rtd/latest?logo=read-the-docs
+	:target: https://repo-helper-rtd.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/repo-helper/repo_helper_rtd/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/repo-helper/repo_helper_rtd/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
-.. |travis| image:: https://github.com/repo-helper/repo_helper_rtd/workflows/Linux%20Tests/badge.svg
-	:target: https://github.com/repo-helper/repo_helper_rtd/actions?query=workflow%3A%22Linux+Tests%22
+.. |actions_linux| image:: https://github.com/repo-helper/repo_helper_rtd/workflows/Linux/badge.svg
+	:target: https://github.com/repo-helper/repo_helper_rtd/actions?query=workflow%3A%22Linux%22
 	:alt: Linux Test Status
 
-.. |actions_windows| image:: https://github.com/repo-helper/repo_helper_rtd/workflows/Windows%20Tests/badge.svg
-	:target: https://github.com/repo-helper/repo_helper_rtd/actions?query=workflow%3A%22Windows+Tests%22
+.. |actions_windows| image:: https://github.com/repo-helper/repo_helper_rtd/workflows/Windows/badge.svg
+	:target: https://github.com/repo-helper/repo_helper_rtd/actions?query=workflow%3A%22Windows%22
 	:alt: Windows Test Status
 
-.. |actions_macos| image:: https://github.com/repo-helper/repo_helper_rtd/workflows/macOS%20Tests/badge.svg
-	:target: https://github.com/repo-helper/repo_helper_rtd/actions?query=workflow%3A%22macOS+Tests%22
+.. |actions_macos| image:: https://github.com/repo-helper/repo_helper_rtd/workflows/macOS/badge.svg
+	:target: https://github.com/repo-helper/repo_helper_rtd/actions?query=workflow%3A%22macOS%22
 	:alt: macOS Test Status
 
-.. |requires| image:: https://requires.io/github/repo-helper/repo_helper_rtd/requirements.svg?branch=master
-	:target: https://requires.io/github/repo-helper/repo_helper_rtd/requirements/?branch=master
+.. |actions_flake8| image:: https://github.com/repo-helper/repo_helper_rtd/workflows/Flake8/badge.svg
+	:target: https://github.com/repo-helper/repo_helper_rtd/actions?query=workflow%3A%22Flake8%22
+	:alt: Flake8 Status
+
+.. |actions_mypy| image:: https://github.com/repo-helper/repo_helper_rtd/workflows/mypy/badge.svg
+	:target: https://github.com/repo-helper/repo_helper_rtd/actions?query=workflow%3A%22mypy%22
+	:alt: mypy status
+
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/repo-helper/repo_helper_rtd/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/repo-helper/repo_helper_rtd/
 	:alt: Requirements Status
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/repo_helper_rtd?logo=codefactor
 	:target: https://www.codefactor.io/repository/github/repo-helper/repo_helper_rtd
 	:alt: CodeFactor Grade
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/repo_helper_rtd
@@ -73,32 +83,28 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/repo_helper_rtd
 	:target: https://github.com/repo-helper/repo_helper_rtd/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/repo_helper_rtd
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/repo_helper_rtd/v0.1.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/repo_helper_rtd/v0.1.1
 	:target: https://github.com/repo-helper/repo_helper_rtd/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/repo_helper_rtd
 	:target: https://github.com/repo-helper/repo_helper_rtd/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2020
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
-.. |pre_commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
-	:target: https://github.com/pre-commit/pre-commit
-	:alt: pre-commit
-
-.. |pre_commit_ci| image:: https://results.pre-commit.ci/badge/github/repo-helper/repo_helper_rtd/master.svg
-	:target: https://results.pre-commit.ci/latest/github/repo-helper/repo_helper_rtd/master
-	:alt: pre-commit.ci status
+.. |pypi-downloads| image:: https://img.shields.io/pypi/dm/repo_helper_rtd
+	:target: https://pypi.org/project/repo_helper_rtd/
+	:alt: PyPI - Downloads
 
 .. end shields
 
 Installation
 --------------
 
 .. start installation
```

### Comparing `repo_helper_rtd-0.1.0/repo_helper_rtd/__init__.py` & `repo_helper_rtd-0.1.1/repo_helper_rtd/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,49 +26,33 @@
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
 from typing import Dict, Optional, Union
 
 # 3rd party
-from apeye import RequestsURL
-from click.globals import resolve_color_default
+from apeye.requests_url import TrailingRequestsURL
+from click.globals import resolve_color_default  # type: ignore
 from domdf_python_tools.secrets import Secret
 from domdf_python_tools.typing import PathLike
 from repo_helper.core import RepoHelper
 from requests import Response
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.1.0"
+__version__: str = "0.1.1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["ReadTheDocsManager"]
 
 # Makes the docs link correctly
 Response.__module__ = "requests"
 
-
-class RequestsURLTS(RequestsURL):
-	"""
-	Extension of :class:`~apeye.requests_url.RequestsURL` which adds a trailing slash to the end of the URL.
-
-	:param url: The url to construct the :class:`~apeye.url.URL` object from.
-	"""
-
-	def __str__(self) -> str:
-		"""
-		Returns the :class:`~.RequestsURLTS` as a string.
-		"""
-
-		return super().__str__() + '/'
-
-
-RTD_API = RequestsURLTS("https://readthedocs.org/api/v3")
+RTD_API = TrailingRequestsURL("https://readthedocs.org/api/v3")
 
 
 class ReadTheDocsManager(RepoHelper):
 	"""
 	Subclass of :class:`repo_helper.core.RepoHelper`
 	with additional functions to update ReadTheDocs projects.
 
@@ -97,14 +81,15 @@
 			*,
 			colour: Optional[bool] = True,
 			):
 		super().__init__(target_repo, managed_message)
 
 		self.token = Secret(token)
 		self.colour = resolve_color_default(colour)
+		self.load_settings()
 
 	def get_update_json(self) -> Dict[str, Union[Dict[str, str], str]]:
 		"""
 		Returns the body JSON used to update the project.
 		"""
 
 		repo_url = "https://github.com/{username}/{repo_name}".format_map(self.templates.globals)
```

### Comparing `repo_helper_rtd-0.1.0/repo_helper_rtd/cli.py` & `repo_helper_rtd-0.1.1/repo_helper_rtd/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 # stdlib
 import sys
 from functools import partial
 from typing import Optional
 
 # 3rd party
-import click
+import click  # type: ignore
 from consolekit import CONTEXT_SETTINGS
 from consolekit.options import colour_option, version_option
 from repo_helper.cli import cli_group
 
 # this package
 from repo_helper_rtd.options import token_option, version_callback
 
@@ -70,22 +70,23 @@
 	# 3rd party
 	from domdf_python_tools.paths import PathPlus
 
 	# this package
 	from repo_helper_rtd import ReadTheDocsManager
 
 	manager = ReadTheDocsManager(token, PathPlus.cwd(), colour=colour)
+	manager.load_settings()
 	response = manager.new()
 
-	print(response)
 	if response.status_code // 100 == 2:
 		project_name = manager.templates.globals["repo_name"].lower().replace('_', '-')
 		click.echo(f"Success! View the project page at https://readthedocs.org/projects/{project_name}")
 		sys.exit(0)
 
+	print(response)
 	sys.exit(1)
 
 
 @colour_option()
 @token_option()
 @rtd_command()
 def update(token: str, colour: Optional[bool] = None):
@@ -95,15 +96,17 @@
 
 	# 3rd party
 	from domdf_python_tools.paths import PathPlus
 
 	# this package
 	from repo_helper_rtd import ReadTheDocsManager
 
-	response = ReadTheDocsManager(token, PathPlus.cwd(), colour=colour).update()
+	manager = ReadTheDocsManager(token, PathPlus.cwd(), colour=colour)
+	manager.load_settings()
+	response = manager.update()
 
-	print(response)
 	if response.status_code // 100 == 2:
 		click.echo("Up to date!")
 		sys.exit(0)
 
+	print(response)
 	sys.exit(1)
```

### Comparing `repo_helper_rtd-0.1.0/repo_helper_rtd/options.py` & `repo_helper_rtd-0.1.1/repo_helper_rtd/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
 from typing import Callable
 
 # 3rd party
-import click
+import click  # type: ignore
 from domdf_python_tools.stringlist import DelimitedList
 
 __all__ = ["token_option", "version_callback"]
 
 
 def token_option(token_var: str = "RTD_TOKEN") -> Callable:  # nosec: B107
 	"""
```

