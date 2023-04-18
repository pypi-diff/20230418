# Comparing `tmp/repo_helper_github-0.7.0.tar.gz` & `tmp/repo_helper_github-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo_helper_github-0.7.0.tar", last modified: Wed Apr  7 17:11:49 2021, max compression
+gzip compressed data, was "repo_helper_github-0.8.1.tar", last modified: Tue Apr 18 18:59:02 2023, max compression
```

## Comparing `repo_helper_github-0.7.0.tar` & `repo_helper_github-0.8.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0 runner    (1001) docker     (121)     6649 2021-04-07 17:11:49.358699 PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4777 2021-04-07 17:11:49.314699 README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      300 2021-04-07 17:11:49.314699 requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-04-07 17:11:49.310699 LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2486 2021-04-07 17:11:49.314699 pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2518 2021-04-07 17:11:49.302699 repo_helper_github/secret_validation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2021-04-07 17:11:49.302699 repo_helper_github/_github.py
--rw-r--r--   0 runner    (1001) docker     (121)     5046 2021-04-07 17:11:49.306699 repo_helper_github/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2278 2021-04-07 17:11:49.306699 repo_helper_github/options.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-07 17:11:49.302699 repo_helper_github/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     5804 2021-04-07 17:11:49.306699 repo_helper_github/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1539 2021-04-07 17:11:49.306699 repo_helper_github/_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    17680 2021-04-07 17:11:49.310699 repo_helper_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6703 2023-04-18 18:59:02.066599 repo_helper_github-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5086 2023-04-18 18:59:02.062599 repo_helper_github-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-04-18 18:59:02.058599 repo_helper_github-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4767 2023-04-18 18:59:02.066599 repo_helper_github-0.8.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-18 18:59:02.066599 repo_helper_github-0.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    17864 2023-04-18 18:58:31.722104 repo_helper_github-0.8.1/repo_helper_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2292 2023-04-18 18:58:31.722104 repo_helper_github-0.8.1/repo_helper_github/options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-04-18 18:58:31.722104 repo_helper_github-0.8.1/repo_helper_github/_github.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-04-18 18:58:31.722104 repo_helper_github-0.8.1/repo_helper_github/_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 18:58:31.722104 repo_helper_github-0.8.1/repo_helper_github/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     5046 2023-04-18 18:58:31.722104 repo_helper_github-0.8.1/repo_helper_github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2526 2023-04-18 18:58:31.722104 repo_helper_github-0.8.1/repo_helper_github/secret_validation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5827 2023-04-18 18:58:31.722104 repo_helper_github-0.8.1/repo_helper_github/exceptions.py
```

### Comparing `PKG-INFO` & `repo_helper_github-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 Metadata-Version: 2.1
 Name: repo-helper-github
-Version: 0.7.0
+Version: 0.8.1
 Summary: Manage GitHub repositories with repo-helper.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: github,repo-helper
 Home-page: https://github.com/repo-helper/repo_helper_github
 Project-URL: Issue Tracker, https://github.com/repo-helper/repo_helper_github/issues
 Project-URL: Source Code, https://github.com/repo-helper/repo_helper_github
-Project-URL: Documentation, https://repo_helper_github.readthedocs.io/en/latest
+Project-URL: Documentation, https://repo-helper-github.readthedocs.io/en/latest
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Requires-Dist: click>=7.1.2
 Requires-Dist: consolekit>=1.1.2
 Requires-Dist: cryptography==3.3.2; platform_system != "Linux"
-Requires-Dist: deprecation-alias>=0.1.1
+Requires-Dist: deprecation-alias>=0.2.0
 Requires-Dist: domdf-python-tools>=2.0.0
 Requires-Dist: dulwich!=0.20.7,!=0.20.8,!=0.20.9,>=0.20.5
 Requires-Dist: github3-py>=1.3.0
 Requires-Dist: github3-utils>=0.5.0
+Requires-Dist: packaging>=21.0
 Requires-Dist: pymacaroons>=0.13.0
 Requires-Dist: repo-helper>=2020.12.18
 Requires-Dist: southwark>=0.4.0
 Requires-Dist: typing-extensions>=3.7.4.3
 Description-Content-Type: text/x-rst
 
 
@@ -69,16 +71,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/repo_helper_github/latest?logo=read-the-docs
-	:target: https://repo_helper_github.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/repo-helper-github/latest?logo=read-the-docs
+	:target: https://repo-helper-github.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/repo-helper/repo_helper_github/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/repo-helper/repo_helper_github/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/repo-helper/repo_helper_github/workflows/Linux/badge.svg
@@ -97,16 +99,16 @@
 	:target: https://github.com/repo-helper/repo_helper_github/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/repo-helper/repo_helper_github/workflows/mypy/badge.svg
 	:target: https://github.com/repo-helper/repo_helper_github/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://requires.io/github/repo-helper/repo_helper_github/requirements.svg?branch=master
-	:target: https://requires.io/github/repo-helper/repo_helper_github/requirements/?branch=master
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/repo-helper/repo_helper_github/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/repo-helper/repo_helper_github/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/repo-helper/repo_helper_github/master?logo=coveralls
 	:target: https://coveralls.io/github/repo-helper/repo_helper_github?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/repo_helper_github?logo=codefactor
@@ -132,23 +134,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/repo_helper_github
 	:target: https://github.com/repo-helper/repo_helper_github/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/repo_helper_github
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/repo_helper_github/v0.7.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/repo_helper_github/v0.8.1
 	:target: https://github.com/repo-helper/repo_helper_github/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/repo_helper_github
 	:target: https://github.com/repo-helper/repo_helper_github/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2021
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/repo_helper_github
 	:target: https://pypi.org/project/repo_helper_github/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `README.rst` & `repo_helper_github-0.8.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/repo_helper_github/latest?logo=read-the-docs
-	:target: https://repo_helper_github.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/repo-helper-github/latest?logo=read-the-docs
+	:target: https://repo-helper-github.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/repo-helper/repo_helper_github/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/repo-helper/repo_helper_github/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/repo-helper/repo_helper_github/workflows/Linux/badge.svg
@@ -52,16 +52,16 @@
 	:target: https://github.com/repo-helper/repo_helper_github/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/repo-helper/repo_helper_github/workflows/mypy/badge.svg
 	:target: https://github.com/repo-helper/repo_helper_github/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://requires.io/github/repo-helper/repo_helper_github/requirements.svg?branch=master
-	:target: https://requires.io/github/repo-helper/repo_helper_github/requirements/?branch=master
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/repo-helper/repo_helper_github/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/repo-helper/repo_helper_github/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/repo-helper/repo_helper_github/master?logo=coveralls
 	:target: https://coveralls.io/github/repo-helper/repo_helper_github?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/repo_helper_github?logo=codefactor
@@ -87,23 +87,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/repo_helper_github
 	:target: https://github.com/repo-helper/repo_helper_github/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/repo_helper_github
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/repo_helper_github/v0.7.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/repo_helper_github/v0.8.1
 	:target: https://github.com/repo-helper/repo_helper_github/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/repo_helper_github
 	:target: https://github.com/repo-helper/repo_helper_github/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2021
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/repo_helper_github
 	:target: https://pypi.org/project/repo_helper_github/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `LICENSE` & `repo_helper_github-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `repo_helper_github/secret_validation.py` & `repo_helper_github-0.8.1/repo_helper_github/secret_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 #
 
 # stdlib
 import json
 from typing import List, Tuple
 
 # 3rd party
-from pymacaroons import Caveat, Macaroon  # type: ignore
+from pymacaroons import Caveat, Macaroon  # type: ignore[import]
 
 __all__ = ["no_op_validator", "validate_pypi_token"]
 
 
 def validate_pypi_token(token: str) -> Tuple[bool, str]:
 	"""
 	Returns whether the PyPI token *appears* to be valid.
```

### Comparing `repo_helper_github/_github.py` & `repo_helper_github-0.8.1/repo_helper_github/_github.py`

 * *Files identical despite different names*

### Comparing `repo_helper_github/cli.py` & `repo_helper_github-0.8.1/repo_helper_github/cli.py`

 * *Files identical despite different names*

### Comparing `repo_helper_github/options.py` & `repo_helper_github-0.8.1/repo_helper_github/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # stdlib
 from typing import Callable, TypeVar
 
 # 3rd party
 import click
 from domdf_python_tools.stringlist import DelimitedList
 
-__all__ = ["version_callback", "org_option"]
+__all__ = ["version_callback", "org_option", "_C"]
 
 _C = TypeVar("_C", bound=click.Command)
 
 
 def org_option() -> Callable[[_C], _C]:
 	"""
 	Creates a ``--org`` option to specify that the repository belongs to an organisation.
@@ -52,15 +52,15 @@
 			type=click.STRING,
 			help=desc,
 			is_flag=True,
 			default=False,
 			)
 
 
-def version_callback(ctx: click.Context, param: click.Option, value: int):  # noqa: D103
+def version_callback(ctx: click.Context, param: click.Option, value: int) -> None:  # noqa: D103
 	# 3rd party
 	import repo_helper
 
 	# this package
 	from repo_helper_github import __version__
 
 	if not value or ctx.resilient_parsing:  # pragma: no cover
```

### Comparing `repo_helper_github/exceptions.py` & `repo_helper_github-0.8.1/repo_helper_github/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,16 @@
 class NoSuchBranch(GitHubException):
 	"""
 	Exception raised when a branch does not exist.
 
 	:param username: The username of the account the repository belongs to.
 	:param repository: The name of the repository.
 	:param branch: The name of the branch.
+
+	.. latex:clearpage::
 	"""
 
 	#: The username of the account the repository belongs to.
 	username: str
 
 	#: The name of the repository.
 	repository: str
```

### Comparing `repo_helper_github/_types.py` & `repo_helper_github-0.8.1/repo_helper_github/_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,17 +19,14 @@
 #  MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 #  IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 #  DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
-# stdlib
-from typing import Dict, List
-
 # 3rd party
 from typing_extensions import TypedDict
 
 
 class _EditKwargs(TypedDict, total=False):
 	description: str
 	homepage: str
```

### Comparing `repo_helper_github/__init__.py` & `repo_helper_github-0.8.1/repo_helper_github/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 #  DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
 import tempfile
+from contextlib import suppress
 from getpass import getpass
 from typing import Callable, Dict, Iterator, Optional, Tuple, Union
 
 # 3rd party
 import click
 from consolekit.input import confirm
 from consolekit.terminal_colours import ColourTrilean, Fore, resolve_color_default
@@ -44,14 +45,15 @@
 from github3.exceptions import NotFoundError
 from github3.repos import contents
 from github3.repos.branch import Branch
 from github3_utils import echo_rate_limit as _utils_echo_rate_limit
 from github3_utils import get_user as _utils_get_user
 from github3_utils import protect_branch, secrets
 from github3_utils.check_labels import check_status_labels
+from packaging.version import InvalidVersion, Version
 from repo_helper.core import RepoHelper
 from repo_helper.files.ci_cd import ActionsManager, platform_ci_names
 from repo_helper.utils import set_gh_actions_versions
 from southwark.repo import Repo
 
 # this package
 from repo_helper_github._github import Github
@@ -65,15 +67,15 @@
 		OrganizationError
 		)
 from repo_helper_github.secret_validation import no_op_validator, validate_pypi_token
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020-2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.7.0"
+__version__: str = "0.8.1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = [
 		"github_command",
 		"echo_rate_limit",
 		"GitHubManager",
 		"IsolatedGitHubManager",
@@ -81,27 +83,25 @@
 		"compile_required_checks",
 		]
 
 echo_rate_limit = deprecated(
 		deprecated_in="0.5.0",
 		removed_in="1.0.0",
 		current_version=__version__,
-		details="Use the new 'github3-utils' package instead."
-		)(
-				_utils_echo_rate_limit
-				)
+		details="Use the new 'github3-utils' package instead.",
+		func=_utils_echo_rate_limit,
+		)
 
 get_user = deprecated(
 		deprecated_in="0.6.0",
 		removed_in="1.0.0",
 		current_version=__version__,
-		details="Use the new 'github3-utils' package instead."
-		)(
-				_utils_get_user
-				)
+		details="Use the new 'github3-utils' package instead.",
+		func=_utils_get_user,
+		)
 
 
 def _lower(string: str) -> str:
 	return string.lower().replace('_', '-')
 
 
 class GitHubManager(RepoHelper):
@@ -112,14 +112,17 @@
 	:param token: The token to authenticate with the GitHub API.
 	:param target_repo: The path to the root of the repository to manage files for.
 	:param managed_message: Message placed at the top of files to indicate that they are managed by ``repo_helper``.
 	:param verbose: Whether to show information on the GitHub API rate limit.
 	:param colour: Whether to use coloured output.
 
 	.. versionchanged:: 0.3.0  Added the ``verbose`` and ``colour`` options.
+
+	.. latex:clearpage::
+	.. autosummary-widths:: 47/100
 	"""  # noqa: D400
 
 	#:
 	github: GitHub
 
 	verbose: bool
 	"""
@@ -135,15 +138,15 @@
 	.. versionadded: 0.3.0
 	"""
 
 	def __init__(
 			self,
 			token: str,
 			target_repo: PathLike,
-			managed_message="This file is managed by 'repo_helper'. Don't edit it directly.",
+			managed_message: str = "This file is managed by 'repo_helper'. Don't edit it directly.",
 			*,
 			verbose: bool = False,
 			colour: ColourTrilean = True,
 			):
 		super().__init__(target_repo, managed_message)
 
 		self.github = Github(token=token)
@@ -165,17 +168,16 @@
 		:param org: Whether the repository should be created for the organization set as ``username``,
 			or for the authenticated user (default).
 
 		:rtype:
 
 		.. versionchanged:: 0.3.0
 
-			Removed the ``verbose`` option. Provide it to the class constructor instead.
-
-		.. versionchanged:: 0.3.0  Added the ``org`` argument.
+			* Removed the ``verbose`` option. Provide it to the class constructor instead.
+			* Added the ``org`` argument.
 		"""
 
 		with self.echo_rate_limit():
 			user = self.get_org_or_user(org)
 			repo_name = self.templates.globals["repo_name"]
 
 			repo: Optional[repos.Repository]
@@ -212,17 +214,16 @@
 		:param org: Whether the repository should be created for the organization set as ``username``,
 			or for the authenticated user (default).
 
 		:rtype:
 
 		.. versionchanged:: 0.3.0
 
-			Removed the ``verbose`` option. Provide it to the class constructor instead.
-
-		.. versionchanged:: 0.3.0  Added the ``org`` argument.
+			* Removed the ``verbose`` option. Provide it to the class constructor instead.
+			* Added the ``org`` argument.
 		"""
 
 		with self.echo_rate_limit():
 			user = self.get_org_or_user(org)
 			repo_name = self.templates.globals["repo_name"]
 			repo: repos.Repository = self._get_repository(user, repo_name, org)
 
@@ -290,19 +291,20 @@
 		.. versionadded:: 0.3.0
 
 		:param org: Whether the repository should be created for the organization set as ``username``,
 			or for the authenticated user (default).
 		:param overwrite: Overwrite existing values.
 		:default overwrite: ask first.
 
-		``PYPI_TOKEN`` and ``ANACONDA_TOKEN`` can either be passed as keyword arguments to this function or provided at the interactive prompt.
+		``PYPI_TOKEN`` and ``ANACONDA_TOKEN`` can either be passed as keyword arguments to this function
+		or provided at the interactive prompt.
 
 		:rtype:
 
-		.. versionchanged:: 0.4.0  Add ``overwrite``, ``PYPI_TOKEN``, ``ANACONDA_TOKEN`` options.
+		.. versionchanged:: 0.4.0  Added ``overwrite``, ``PYPI_TOKEN``, ``ANACONDA_TOKEN`` options.
 		"""
 
 		with self.echo_rate_limit():
 			user = self.get_org_or_user(org)
 			repo_name = self.templates.globals["repo_name"]
 			repo: repos.Repository = self._get_repository(user, repo_name, org)
 
@@ -363,18 +365,22 @@
 
 		.. versionadded:: 0.4.0
 
 		:param branch: The branch to update protection for.
 		:param org: Whether the repository should be created for the organization set as ``username``,
 			or for the authenticated user (default).
 
+		:rtype:
+
 		:raises:
 
 			* :exc:`~.NoSuchBranch` if the branch is not found.
 			* :exc:`~.NoSuchRepository` if the repository is not found.
+
+		.. latex:clearpage::
 		"""
 
 		with self.echo_rate_limit():
 			user = self.get_org_or_user(org)
 			repo_name = self.templates.globals["repo_name"]
 			repo: repos.Repository = self._get_repository(user, repo_name, org)
 
@@ -494,18 +500,17 @@
 		return 0
 
 
 encrypt_secret = deprecated(
 		deprecated_in="0.5.0",
 		removed_in="1.0.0",
 		current_version=__version__,
-		details="Use the new 'github3-utils' package instead."
-		)(
-				secrets.encrypt_secret
-				)
+		details="Use the new 'github3-utils' package instead.",
+		func=secrets.encrypt_secret,
+		)
 
 encrypt_secret.__doc__ = (encrypt_secret.__doc__ or '').replace(
 		":func:`~.get_secrets`",
 		":func:`~github3_utils.secrets.get_secrets`",
 		)
 
 
@@ -533,17 +538,21 @@
 		# elif platform == "macOS":
 		# 	ci_platform = platform_ci_names[platform]
 		# 	py_versions = actions_manager.get_macos_ci_versions()
 		else:
 			continue
 
 		for version in set_gh_actions_versions(py_versions):
-			if "alpha" in version or "beta" in version or "-dev" in version:
+			if version == "pypy-3.7":
 				continue
 
+			with suppress(InvalidVersion):
+				if Version(version).is_prerelease:
+					continue
+
 			yield f"{ci_platform} / Python {version}"
 
 	yield from [f"mypy / {platform_ci_names['Linux']}", "Flake8"]
 
 	if repo.templates.globals["enable_docs"]:
 		yield "docs"
```

