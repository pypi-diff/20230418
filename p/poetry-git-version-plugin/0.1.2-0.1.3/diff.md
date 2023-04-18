# Comparing `tmp/poetry_git_version_plugin-0.1.2.tar.gz` & `tmp/poetry_git_version_plugin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_git_version_plugin-0.1.2.tar", max compression
+gzip compressed data, was "poetry_git_version_plugin-0.1.3.tar", max compression
```

## Comparing `poetry_git_version_plugin-0.1.2.tar` & `poetry_git_version_plugin-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1055 2023-04-16 19:45:04.526406 poetry_git_version_plugin-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2023-04-16 19:48:08.369382 poetry_git_version_plugin-0.1.2/poetry_git_version_plugin/__init__.py
--rw-r--r--   0        0        0      310 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.2/poetry_git_version_plugin/commands.py
--rw-r--r--   0        0        0     1250 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.2/poetry_git_version_plugin/config.py
--rw-r--r--   0        0        0      758 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.2/poetry_git_version_plugin/exceptions.py
--rw-r--r--   0        0        0     1461 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.2/poetry_git_version_plugin/plugins.py
--rw-r--r--   0        0        0     4506 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.2/poetry_git_version_plugin/services.py
--rw-r--r--   0        0        0     2228 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1077 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.2/readme.md
--rw-r--r--   0        0        0     2723 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-04-16 19:45:04.526406 poetry_git_version_plugin-0.1.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-18 08:53:02.585461 poetry_git_version_plugin-0.1.3/poetry_git_version_plugin/__init__.py
+-rw-r--r--   0        0        0      310 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.3/poetry_git_version_plugin/commands.py
+-rw-r--r--   0        0        0     1250 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.3/poetry_git_version_plugin/config.py
+-rw-r--r--   0        0        0      758 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.3/poetry_git_version_plugin/exceptions.py
+-rw-r--r--   0        0        0     1461 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.3/poetry_git_version_plugin/plugins.py
+-rw-r--r--   0        0        0     4506 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.3/poetry_git_version_plugin/services.py
+-rw-r--r--   0        0        0     2509 2023-04-18 08:29:46.694155 poetry_git_version_plugin-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1248 2023-04-16 19:55:03.123301 poetry_git_version_plugin-0.1.3/readme.md
+-rw-r--r--   0        0        0     2844 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.3/PKG-INFO
```

### Comparing `poetry_git_version_plugin-0.1.2/LICENSE` & `poetry_git_version_plugin-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.2/poetry_git_version_plugin/config.py` & `poetry_git_version_plugin-0.1.3/poetry_git_version_plugin/config.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.2/poetry_git_version_plugin/exceptions.py` & `poetry_git_version_plugin-0.1.3/poetry_git_version_plugin/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.2/poetry_git_version_plugin/plugins.py` & `poetry_git_version_plugin-0.1.3/poetry_git_version_plugin/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.2/poetry_git_version_plugin/services.py` & `poetry_git_version_plugin-0.1.3/poetry_git_version_plugin/services.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.2/pyproject.toml` & `poetry_git_version_plugin-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -12,55 +12,64 @@
 readme = "readme.md"
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Intended Audience :: System Administrators",
-    # "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Version Control :: Git",
     "Topic :: Software Development",
     "Topic :: System :: Archiving :: Packaging",
     "Topic :: System :: Installation/Setup",
     "Topic :: System :: Software Distribution",
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3 :: Only",
 ]
 packages = [{include = "poetry_git_version_plugin"}]
 
 [tool.poetry.plugins."poetry.plugin"]
 poetry-git-version-plugin = "poetry_git_version_plugin.plugins:PoetryGitVersionPlugin"
 
 [tool.poetry.plugins."poetry.application.plugin"]
 poetry-git-version-plugin = "poetry_git_version_plugin.plugins:PoetryGitVersionApplicationPlugin"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 poetry = "^1.2.2"
 gitpython = "^3.1.29"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 ruff = "^0.0.260"
 black = "^23.3.0"
+isort = "^5.12.0"
 
 [tool.black]
 skip-string-normalization = true
 line-length = 120
 
 [tool.isort]
 profile = "black"
 line_length = 120
 
+[tool.ruff]
+# select = ["A", "B", "C", "D", "E", "F", "I", "UP"]
+select = ["A", "B", "C", "E", "F", "I", "UP"]
+# fixable = ["A", "B", "C", "D", "E", "F", "I", "UP"]
+fixable = ["A"]
+ignore = ["UP004", "D100", "D101", "D102", "D103", "D104", "D107", "D400", "D415"]
+line-length = 120
+target-version = "py38"
+
 [tool.coverage.run]
 omit = [
     "*/tests/*",
     "install-poetry.py"
 ]
 
 [tool.coverage.report]
```

### Comparing `poetry_git_version_plugin-0.1.2/PKG-INFO` & `poetry_git_version_plugin-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: poetry-git-version-plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: Poetry plugin to get package version from git
 Home-page: https://gitlab.com/rocshers/python/poetry-git-version-plugin
 License: MIT
 Author: irocshers
 Author-email: develop.iam@rocshers.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Software Distribution
@@ -36,17 +35,18 @@
 
 # Poetry Git Version Plugin
 
 Poetry plugin to get package version from git.
 
 ## Functionality
 
-- Project tag parsing
+- Git tag parsing
+- Make alpha version
 - Substitution of the project tag (if any) in the poetry.version value
-- ~~Maintenance of PEP 440~~
+- Maintenance of PEP 440
 - Command to output a new version
 
 ## Quick start
 
 ```bash
 poetry self add poetry-git-version-plugin
 poetry git-version # Write your git tag
@@ -61,22 +61,27 @@
 poetry = ">=1.2.0"
 ```
 
 ## Setup
 
 ```toml
 [tool.poetry-git-version-plugin]
-# Ignore "tag missing" errors
+# Ignore "tag missing" errors and other errors
+# Default = true
 ignore_errors = true
 
 # If the tag is missing.
 # Returns a version, computed from the latest version tag.
 # It takes the version tag, increases the version tag by the number of commits since, adds a local label specifying the git commit hash and the dirty status.
 # Example: 1.3.2+5-5babef6
 make_alpha_version = true
+
+# Format for alpha version
+# Default = '{version}.a{distance}+{commit_hash}'
+format_alpha_version = '{version}+{distance}'
 ```
 
 ## Contribute
 
 Issue Tracker: <https://gitlab.com/rocshers/python/poetry-git-version-plugin/-/issues>  
 Source Code: <https://gitlab.com/rocshers/python/poetry-git-version-plugin>
```

