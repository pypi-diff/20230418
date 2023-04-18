# Comparing `tmp/check_sdist-0.1.1.tar.gz` & `tmp/check_sdist-0.1.2.tar.gz`

## Comparing `check_sdist-0.1.1.tar` & `check_sdist-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 check_sdist-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 check_sdist-0.1.1/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 check_sdist-0.1.1/noxfile.py
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 check_sdist-0.1.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 check_sdist-0.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 check_sdist-0.1.1/.github/matchers/pylint.json
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 check_sdist-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 check_sdist-0.1.1/docs/conf.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 check_sdist-0.1.1/docs/index.rst
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/__init__.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/__main__.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/git.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/inject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/py.typed
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/sdist.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/_compat/__init__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/_compat/importlib.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/_compat/tomllib.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/resources/__init__.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/resources/default-ignore.txt
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/resources/junk-paths.txt
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 check_sdist-0.1.1/tests/downstream.toml
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 check_sdist-0.1.1/tests/test_downstream.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 check_sdist-0.1.1/tests/test_inject.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 check_sdist-0.1.1/tests/test_package.py
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 check_sdist-0.1.1/.gitignore
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 check_sdist-0.1.1/LICENSE
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 check_sdist-0.1.1/README.md
--rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 check_sdist-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 check_sdist-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 check_sdist-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 check_sdist-0.1.2/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 check_sdist-0.1.2/noxfile.py
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 check_sdist-0.1.2/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 check_sdist-0.1.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 check_sdist-0.1.2/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 check_sdist-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 check_sdist-0.1.2/docs/conf.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 check_sdist-0.1.2/docs/index.rst
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 check_sdist-0.1.2/src/check_sdist/__init__.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 check_sdist-0.1.2/src/check_sdist/__main__.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 check_sdist-0.1.2/src/check_sdist/git.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 check_sdist-0.1.2/src/check_sdist/inject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 check_sdist-0.1.2/src/check_sdist/py.typed
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 check_sdist-0.1.2/src/check_sdist/sdist.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 check_sdist-0.1.2/src/check_sdist/_compat/__init__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 check_sdist-0.1.2/src/check_sdist/_compat/importlib.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 check_sdist-0.1.2/src/check_sdist/_compat/tomllib.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 check_sdist-0.1.2/src/check_sdist/resources/__init__.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 check_sdist-0.1.2/src/check_sdist/resources/default-ignore.txt
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 check_sdist-0.1.2/src/check_sdist/resources/junk-paths.txt
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 check_sdist-0.1.2/tests/downstream.toml
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 check_sdist-0.1.2/tests/test_cli.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 check_sdist-0.1.2/tests/test_downstream.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 check_sdist-0.1.2/tests/test_inject.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 check_sdist-0.1.2/tests/test_package.py
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 check_sdist-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 check_sdist-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 check_sdist-0.1.2/README.md
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 check_sdist-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 check_sdist-0.1.2/PKG-INFO
```

### Comparing `check_sdist-0.1.1/.pre-commit-config.yaml` & `check_sdist-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.1/noxfile.py` & `check_sdist-0.1.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.1/.github/CONTRIBUTING.md` & `check_sdist-0.1.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.1/.github/matchers/pylint.json` & `check_sdist-0.1.2/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.1/.github/workflows/ci.yml` & `check_sdist-0.1.2/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
       - name: Install package
         run: python -m pip install .[test]
 
       - name: Test package
         run: python -m pytest -ra --cov=check-sdist
 
       - name: Upload coverage report
-        uses: codecov/codecov-action@v3.1.1
+        uses: codecov/codecov-action@v3.1.2
 
   dist:
     name: Distribution build
     runs-on: ubuntu-latest
     needs: [pre-commit]
 
     steps:
```

### Comparing `check_sdist-0.1.1/docs/conf.py` & `check_sdist-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.1/src/check_sdist/__main__.py` & `check_sdist-0.1.2/src/check_sdist/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
 import argparse
 import contextlib
+from collections.abc import Sequence
 from pathlib import Path
 
 import pathspec
 
+from . import __version__
 from ._compat import tomllib
 from .git import git_files
 from .inject import inject_junk_files
 from .resources import resources
 from .sdist import sdist_files
 
 
@@ -65,17 +67,20 @@
         print()
         return bool(sdist_only) + 2 * bool(git_only)
 
     print("SDist matches git")
     return 0
 
 
-def main() -> None:
+def main(sys_args: Sequence[str] | None = None, /) -> None:
     """Parse the command line arguments and call compare()."""
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(prog=None if sys_args is None else "check-sdist")
+    parser.add_argument(
+        "--version", action="version", version=f"%(prog)s {__version__}"
+    )
     parser.add_argument(
         "--source-dir",
         type=Path,
         default=Path.cwd(),
         help="The source directory to check (default: current directory)",
     )
     parser.add_argument(
@@ -90,15 +95,15 @@
     )
     parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         help="Print out SDist contents too",
     )
-    args = parser.parse_args()
+    args = parser.parse_args(sys_args)
 
     with contextlib.ExitStack() as stack:
         if args.inject_junk:
             stack.enter_context(inject_junk_files(args.source_dir))
 
     raise SystemExit(
         compare(args.source_dir, isolated=not args.no_isolation, verbose=args.verbose)
```

### Comparing `check_sdist-0.1.1/src/check_sdist/git.py` & `check_sdist-0.1.2/src/check_sdist/git.py`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.1/src/check_sdist/inject.py` & `check_sdist-0.1.2/src/check_sdist/inject.py`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.1/src/check_sdist/sdist.py` & `check_sdist-0.1.2/src/check_sdist/sdist.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,13 +20,15 @@
 
         with tarfile.open(outpath) as tar:
             prefixes = {n.split("/", maxsplit=1)[0] for n in tar.getnames()}
             if len(prefixes) != 1:
                 msg = f"malformted SDist, contains multiple packages {prefixes}"
                 raise AssertionError(msg)
             return frozenset(
-                t.name.split("/", maxsplit=1)[1] for t in tar.getmembers() if t.isfile()
+                t.name.split("/", maxsplit=1)[1]
+                for t in tar.getmembers()
+                if t.isfile() or t.issym()
             )
 
 
 if __name__ == "__main__":
     print(*sorted(sdist_files(Path.cwd(), True)), sep="\n")
```

### Comparing `check_sdist-0.1.1/tests/test_downstream.py` & `check_sdist-0.1.2/tests/test_downstream.py`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.1/tests/test_inject.py` & `check_sdist-0.1.2/tests/test_inject.py`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.1/tests/test_package.py` & `check_sdist-0.1.2/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.1/.gitignore` & `check_sdist-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.1/LICENSE` & `check_sdist-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.1/README.md` & `check_sdist-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.1/pyproject.toml` & `check_sdist-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.1/PKG-INFO` & `check_sdist-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: check-sdist
-Version: 0.1.1
+Version: 0.1.2
 Summary: Check the contents of an SDist vs. git
 Project-URL: Homepage, https://github.com/henryiii/check-sdist
 Project-URL: Bug Tracker, https://github.com/henryiii/check-sdist/issues
 Project-URL: Changelog, https://github.com/henryiii/check-sdist/releases
 Author-email: Henry Schreiner <henryschreineriii@gmail.com>
 License-File: LICENSE
 Keywords: lint,packaging,sdist
```

