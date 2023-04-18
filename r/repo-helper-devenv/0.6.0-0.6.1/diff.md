# Comparing `tmp/repo_helper_devenv-0.6.0.tar.gz` & `tmp/repo_helper_devenv-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo_helper_devenv-0.6.0.tar", last modified: Mon Apr  4 19:00:33 2022, max compression
+gzip compressed data, was "repo_helper_devenv-0.6.1.tar", last modified: Tue Apr 18 18:31:59 2023, max compression
```

## Comparing `repo_helper_devenv-0.6.0.tar` & `repo_helper_devenv-0.6.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-04-04 19:00:33.624721 repo_helper_devenv-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6245 2022-04-04 19:00:33.664721 repo_helper_devenv-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-04-04 19:00:33.628721 repo_helper_devenv-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4416 2022-04-04 19:00:33.628721 repo_helper_devenv-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     4766 2022-04-04 19:00:33.632721 repo_helper_devenv-0.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3015 2022-04-04 18:59:58.836941 repo_helper_devenv-0.6.0/repo_helper_devenv/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     5649 2022-04-04 18:59:58.836941 repo_helper_devenv-0.6.0/repo_helper_devenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-04 18:59:58.836941 repo_helper_devenv-0.6.0/repo_helper_devenv/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-04-18 18:31:59.456460 repo_helper_devenv-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4425 2023-04-18 18:31:59.452460 repo_helper_devenv-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-04-18 18:31:59.444460 repo_helper_devenv-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4768 2023-04-18 18:31:59.456460 repo_helper_devenv-0.6.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-04-18 18:31:59.452460 repo_helper_devenv-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5700 2023-04-18 18:31:14.011763 repo_helper_devenv-0.6.1/repo_helper_devenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 18:31:14.011763 repo_helper_devenv-0.6.1/repo_helper_devenv/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     3039 2023-04-18 18:31:14.011763 repo_helper_devenv-0.6.1/repo_helper_devenv/cli.py
```

### Comparing `repo_helper_devenv-0.6.0/LICENSE` & `repo_helper_devenv-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `repo_helper_devenv-0.6.0/PKG-INFO` & `repo_helper_devenv-0.6.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: repo-helper-devenv
-Version: 0.6.0
+Version: 0.6.1
 Summary: Create virtual environments with repo-helper.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: repo-helper,virtualenv
 Home-page: https://github.com/repo-helper/repo_helper_devenv
 Project-URL: Issue Tracker, https://github.com/repo-helper/repo_helper_devenv/issues
 Project-URL: Source Code, https://github.com/repo-helper/repo_helper_devenv
-Project-URL: Documentation, https://repo_helper_devenv.readthedocs.io/en/latest
+Project-URL: Documentation, https://repo-helper-devenv.readthedocs.io/en/latest
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Requires-Dist: click>=7.1.2
 Requires-Dist: consolekit>=1.0.0
 Requires-Dist: deprecation-alias>=0.1.1
 Requires-Dist: domdf-python-tools>=1.5.0
@@ -61,16 +62,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/repo_helper_devenv/latest?logo=read-the-docs
-	:target: https://repo_helper_devenv.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/repo-helper-devenv/latest?logo=read-the-docs
+	:target: https://repo-helper-devenv.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/repo-helper/repo_helper_devenv/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/repo-helper/repo_helper_devenv/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/repo-helper/repo_helper_devenv/workflows/Linux/badge.svg
@@ -89,16 +90,16 @@
 	:target: https://github.com/repo-helper/repo_helper_devenv/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/repo-helper/repo_helper_devenv/workflows/mypy/badge.svg
 	:target: https://github.com/repo-helper/repo_helper_devenv/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/repo-helper/repo_helper_devenv/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/repo-helper/repo_helper_devenv/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/repo-helper/repo_helper_devenv/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/repo-helper/repo_helper_devenv/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/repo-helper/repo_helper_devenv/master?logo=coveralls
 	:target: https://coveralls.io/github/repo-helper/repo_helper_devenv?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/repo_helper_devenv?logo=codefactor
@@ -124,23 +125,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/repo_helper_devenv
 	:target: https://github.com/repo-helper/repo_helper_devenv/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/repo_helper_devenv
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/repo_helper_devenv/v0.6.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/repo_helper_devenv/v0.6.1
 	:target: https://github.com/repo-helper/repo_helper_devenv/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/repo_helper_devenv
 	:target: https://github.com/repo-helper/repo_helper_devenv/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/repo_helper_devenv
 	:target: https://pypi.org/project/repo_helper_devenv/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `repo_helper_devenv-0.6.0/pyproject.toml` & `repo_helper_devenv-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "repo_helper_devenv"
-version = "0.6.0"
+version = "0.6.1"
 description = "Create virtual environments with repo-helper."
 readme = "README.rst"
 keywords = [ "repo-helper", "virtualenv",]
 dynamic = []
 dependencies = [
     "click>=7.1.2",
     "consolekit>=1.0.0",
@@ -21,14 +21,15 @@
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Typing :: Typed",
 ]
@@ -42,15 +43,15 @@
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/repo-helper/repo_helper_devenv"
 "Issue Tracker" = "https://github.com/repo-helper/repo_helper_devenv/issues"
 "Source Code" = "https://github.com/repo-helper/repo_helper_devenv"
-Documentation = "https://repo_helper_devenv.readthedocs.io/en/latest"
+Documentation = "https://repo-helper-devenv.readthedocs.io/en/latest"
 
 [tool.sphinx-pyproject]
 github_username = "repo-helper"
 github_repository = "repo_helper_devenv"
 author = "Dominic Davis-Foster"
 project = "repo-helper-devenv"
 copyright = "2020-2021 Dominic Davis-Foster"
@@ -58,31 +59,30 @@
 package_root = "repo_helper_devenv"
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
     "sphinx_click",
-    "sphinx_toolbox_experimental.needspace",
     "sphinx_toolbox_experimental.missing_xref",
 ]
 sphinxemoji_style = "twemoji"
 gitstamp_fmt = "%d %b %Y"
 templates_path = [ "_templates",]
 html_static_path = [ "_static",]
 source_suffix = ".rst"
@@ -128,21 +128,21 @@
     "__getnewargs__",
     "__abstractmethods__",
     "__hash__",
 ]
 
 [tool.whey]
 base-classifiers = [ "Typing :: Typed",]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
 python-implementations = [ "CPython",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 
 [tool.mypy]
-python_version = "3.6"
+python_version = "3.8"
 namespace_packages = true
 check_untyped_defs = true
 warn_unused_ignores = true
 no_implicit_optional = true
 incremental = false
 show_error_codes = true
```

### Comparing `repo_helper_devenv-0.6.0/README.rst` & `repo_helper_devenv-0.6.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/repo_helper_devenv/latest?logo=read-the-docs
-	:target: https://repo_helper_devenv.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/repo-helper-devenv/latest?logo=read-the-docs
+	:target: https://repo-helper-devenv.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/repo-helper/repo_helper_devenv/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/repo-helper/repo_helper_devenv/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/repo-helper/repo_helper_devenv/workflows/Linux/badge.svg
@@ -52,16 +52,16 @@
 	:target: https://github.com/repo-helper/repo_helper_devenv/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/repo-helper/repo_helper_devenv/workflows/mypy/badge.svg
 	:target: https://github.com/repo-helper/repo_helper_devenv/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/repo-helper/repo_helper_devenv/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/repo-helper/repo_helper_devenv/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/repo-helper/repo_helper_devenv/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/repo-helper/repo_helper_devenv/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/repo-helper/repo_helper_devenv/master?logo=coveralls
 	:target: https://coveralls.io/github/repo-helper/repo_helper_devenv?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/repo_helper_devenv?logo=codefactor
@@ -87,23 +87,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/repo_helper_devenv
 	:target: https://github.com/repo-helper/repo_helper_devenv/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/repo_helper_devenv
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/repo_helper_devenv/v0.6.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/repo_helper_devenv/v0.6.1
 	:target: https://github.com/repo-helper/repo_helper_devenv/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/repo_helper_devenv
 	:target: https://github.com/repo-helper/repo_helper_devenv/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/repo_helper_devenv
 	:target: https://pypi.org/project/repo_helper_devenv/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `repo_helper_devenv-0.6.0/repo_helper_devenv/cli.py` & `repo_helper_devenv-0.6.1/repo_helper_devenv/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,21 +35,21 @@
 from consolekit.terminal_colours import ColourTrilean
 from domdf_python_tools.typing import PathLike
 from repo_helper.cli import cli_command
 
 __all__ = ["devenv", "version_callback"]
 
 
-def version_callback(ctx: click.Context, param: click.Option, value: int):  # noqa: D103
+def version_callback(ctx: click.Context, param: click.Option, value: int) -> None:  # noqa: D103
 	if not value or ctx.resilient_parsing:
 		return
 
 	# 3rd party
 	import repo_helper
-	import virtualenv  # type: ignore
+	import virtualenv  # type: ignore[import]
 	from domdf_python_tools.stringlist import DelimitedList
 
 	# this package
 	import repo_helper_devenv
 
 	parts = DelimitedList([f"repo_helper_devenv version {repo_helper_devenv.__version__}"])
 
@@ -78,15 +78,15 @@
 		)
 @cli_command()
 def devenv(
 		dest: PathLike = "venv",
 		verbose: int = 0,
 		colour: ColourTrilean = None,
 		upgrade: bool = False,
-		):
+		) -> None:
 	"""
 	Create a virtualenv.
 	"""
 
 	# 3rd party
 	from consolekit.terminal_colours import Fore, resolve_color_default
 	from domdf_python_tools.paths import PathPlus
```

### Comparing `repo_helper_devenv-0.6.0/repo_helper_devenv/__init__.py` & `repo_helper_devenv-0.6.1/repo_helper_devenv/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,26 +36,26 @@
 # stdlib
 import types
 from typing import Dict
 
 # 3rd party
 import pyproject_devenv
 import shippinglabel
-import virtualenv  # type: ignore
+import virtualenv  # type: ignore[import]
 from deprecation_alias import deprecated
 from domdf_python_tools.paths import PathPlus
 from domdf_python_tools.typing import PathLike
 from pyproject_devenv.config import ConfigDict
 from repo_helper.core import RepoHelper
-from virtualenv.run.session import Session  # type: ignore
+from virtualenv.run.session import Session  # type: ignore[import]
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020-2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.6.0"
+__version__: str = "0.6.1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["mkdevenv", "read_pyvenv", "install_requirements"]
 
 virtualenv_version = tuple(map(int, virtualenv.__version__.split('.')[:3]))
 
 
@@ -85,15 +85,15 @@
 		self.venv_dir = self.project_dir / venv_dir
 		self.verbosity: int = int(verbosity)
 		self.upgrade: bool = upgrade
 
 		# TODO: config option
 		self.extras_to_install = sorted(self.config["optional_dependencies"])
 
-	def install_project_requirements(self, of_session):
+	def install_project_requirements(self, of_session: Session) -> None:
 		"""
 		Install the project's requirements/dependencies.
 
 		:param of_session:
 		"""
 
 		self.report_installing("project requirements")
@@ -143,15 +143,15 @@
 		)
 def install_requirements(
 		session: Session,
 		requirements_file: PathLike,
 		verbosity: int = 1,
 		*,
 		upgrade: bool = False,
-		):
+		) -> None:
 	"""
 	Install requirements into a virtualenv.
 
 	:param session:
 	:param requirements_file:
 	:param verbosity: The verbosity of the function. ``0`` = quiet, ``2`` = very verbose.
 	:param upgrade: Whether to upgrade all specified packages to the newest available version.
@@ -160,15 +160,15 @@
 	"""
 
 	namespace = types.SimpleNamespace()
 	namespace.verbosity = int(verbosity)
 	namespace.upgrade = upgrade
 
 	_RepoHelperDevenv.install_requirements(
-			namespace,  # type: ignore
+			namespace,  # type: ignore[arg-type]
 			session,
 			requirements_file=requirements_file,
 			)
 
 
 def update_pyvenv(venv_dir: PathLike) -> None:
 	venv_dir = PathPlus(venv_dir)
```

