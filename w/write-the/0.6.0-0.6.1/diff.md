# Comparing `tmp/write_the-0.6.0.tar.gz` & `tmp/write_the-0.6.1.tar.gz`

## Comparing `write_the-0.6.0.tar` & `write_the-0.6.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 write_the-0.6.0/mkdocs.yml
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 write_the-0.6.0/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 write_the-0.6.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.6.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 write_the-0.6.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 write_the-0.6.0/.pytest_cache/README.md
--rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 write_the-0.6.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0    10819 2020-02-02 00:00:00.000000 write_the-0.6.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 write_the-0.6.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.6.0/docs/CNAME
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 write_the-0.6.0/docs/index.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 write_the-0.6.0/docs/reference/cli.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 write_the-0.6.0/docs/reference/cst.md
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 write_the-0.6.0/docs/reference/docs.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 write_the-0.6.0/docs/reference/mkdocs.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 write_the-0.6.0/docs/reference/tests.md
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.6.0/docs/reference/utils.md
--rw-r--r--   0        0        0   123108 2020-02-02 00:00:00.000000 write_the-0.6.0/images/docs-help.png
--rw-r--r--   0        0        0    84667 2020-02-02 00:00:00.000000 write_the-0.6.0/images/mkdocs-help.png
--rw-r--r--   0        0        0   161159 2020-02-02 00:00:00.000000 write_the-0.6.0/images/multiply.png
--rw-r--r--   0        0        0   139626 2020-02-02 00:00:00.000000 write_the-0.6.0/images/tests-help.png
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 write_the-0.6.0/images/write-the-icon.svg
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 write_the-0.6.0/tests/test_cli_main.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 write_the-0.6.0/tests/test_cst_docstring_adder.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 write_the-0.6.0/tests/test_cst_docstring_remover.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 write_the-0.6.0/tests/test_cst_function_and_class_collector.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 write_the-0.6.0/tests/test_cst_node_extractor.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 write_the-0.6.0/tests/test_cst_node_remover.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 write_the-0.6.0/tests/test_cst_utils.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.6.0/tests/data/multiply.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 write_the-0.6.0/tests/data/multiply_docstring.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.6.0/write_the/__about__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.6.0/write_the/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.6.0/write_the/__main__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 write_the-0.6.0/write_the/utils.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.6.0/write_the/cli/__init__.py
--rw-r--r--   0        0        0     6764 2020-02-02 00:00:00.000000 write_the-0.6.0/write_the/cli/main.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.6.0/write_the/cst/__init__.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 write_the-0.6.0/write_the/cst/docstring_adder.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 write_the-0.6.0/write_the/cst/docstring_remover.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 write_the-0.6.0/write_the/cst/function_and_class_collector.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 write_the-0.6.0/write_the/cst/node_extractor.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 write_the-0.6.0/write_the/cst/node_remover.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 write_the-0.6.0/write_the/cst/utils.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.6.0/write_the/docs/__init__.py
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 write_the-0.6.0/write_the/docs/chain.py
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 write_the-0.6.0/write_the/docs/write.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.6.0/write_the/mkdocs/__init__.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 write_the-0.6.0/write_the/mkdocs/write.py
--rwxr-xr-x   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.6.0/write_the/tests/__init__.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 write_the-0.6.0/write_the/tests/chain.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 write_the-0.6.0/write_the/tests/write.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 write_the-0.6.0/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 write_the-0.6.0/README.md
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 write_the-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 write_the-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 write_the-0.6.1/mkdocs.yml
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 write_the-0.6.1/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 write_the-0.6.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.6.1/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 write_the-0.6.1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 write_the-0.6.1/.pytest_cache/README.md
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 write_the-0.6.1/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0    10819 2020-02-02 00:00:00.000000 write_the-0.6.1/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 write_the-0.6.1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.6.1/docs/CNAME
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 write_the-0.6.1/docs/index.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 write_the-0.6.1/docs/reference/cli.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 write_the-0.6.1/docs/reference/cst.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 write_the-0.6.1/docs/reference/docs.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 write_the-0.6.1/docs/reference/mkdocs.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 write_the-0.6.1/docs/reference/tests.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.6.1/docs/reference/utils.md
+-rw-r--r--   0        0        0   123108 2020-02-02 00:00:00.000000 write_the-0.6.1/images/docs-help.png
+-rw-r--r--   0        0        0    84667 2020-02-02 00:00:00.000000 write_the-0.6.1/images/mkdocs-help.png
+-rw-r--r--   0        0        0   161159 2020-02-02 00:00:00.000000 write_the-0.6.1/images/multiply.png
+-rw-r--r--   0        0        0   139626 2020-02-02 00:00:00.000000 write_the-0.6.1/images/tests-help.png
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 write_the-0.6.1/images/write-the-icon.svg
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 write_the-0.6.1/tests/test_cli_main.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 write_the-0.6.1/tests/test_cst_docstring_adder.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 write_the-0.6.1/tests/test_cst_docstring_remover.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 write_the-0.6.1/tests/test_cst_function_and_class_collector.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 write_the-0.6.1/tests/test_cst_node_extractor.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 write_the-0.6.1/tests/test_cst_node_remover.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 write_the-0.6.1/tests/test_cst_utils.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.6.1/tests/data/multiply.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 write_the-0.6.1/tests/data/multiply_docstring.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/__about__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/__main__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/utils.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/cli/__init__.py
+-rw-r--r--   0        0        0     6759 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/cli/main.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/cst/__init__.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/cst/docstring_adder.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/cst/docstring_remover.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/cst/function_and_class_collector.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/cst/node_extractor.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/cst/node_remover.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/cst/utils.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/docs/__init__.py
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/docs/chain.py
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/docs/write.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/mkdocs/__init__.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/mkdocs/write.py
+-rwxr-xr-x   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/tests/__init__.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/tests/chain.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/tests/write.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 write_the-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.6.1/LICENSE.txt
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 write_the-0.6.1/README.md
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 write_the-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 write_the-0.6.1/PKG-INFO
```

### Comparing `write_the-0.6.0/mkdocs.yml` & `write_the-0.6.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/.github/workflows/tests.yml` & `write_the-0.6.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/.pytest_cache/v/cache/lastfailed` & `write_the-0.6.1/.pytest_cache/v/cache/lastfailed`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/.pytest_cache/v/cache/nodeids` & `write_the-0.6.1/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/docs/index.md` & `write_the-0.6.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/images/docs-help.png` & `write_the-0.6.1/images/docs-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/images/mkdocs-help.png` & `write_the-0.6.1/images/mkdocs-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/images/multiply.png` & `write_the-0.6.1/images/multiply.png`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/images/tests-help.png` & `write_the-0.6.1/images/tests-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/images/write-the-icon.svg` & `write_the-0.6.1/images/write-the-icon.svg`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/tests/test_cli_main.py` & `write_the-0.6.1/tests/test_cli_main.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/tests/test_cst_docstring_adder.py` & `write_the-0.6.1/tests/test_cst_docstring_adder.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/tests/test_cst_docstring_remover.py` & `write_the-0.6.1/tests/test_cst_docstring_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/tests/test_cst_function_and_class_collector.py` & `write_the-0.6.1/tests/test_cst_function_and_class_collector.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/tests/test_cst_node_extractor.py` & `write_the-0.6.1/tests/test_cst_node_extractor.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/tests/test_cst_node_remover.py` & `write_the-0.6.1/tests/test_cst_node_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/tests/test_cst_utils.py` & `write_the-0.6.1/tests/test_cst_utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/write_the/utils.py` & `write_the-0.6.1/write_the/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/write_the/cli/main.py` & `write_the-0.6.1/write_the/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,16 @@
         ...,
         help="Path to the projects code. Uses docstings to build API reference.",
         file_okay=False,
     ),
     readme: Optional[Path] = typer.Option(
         None, help="Path to projects README (used to create index.md).", dir_okay=False
     ),
-    out_dir: Optional[Path] = typer.Option(
-        None, "--out", "-o", help="Path to save output (docs/ and yaml). Defaults to current directory."
+    out_dir: Path = typer.Option(
+        Path('.'), "--out", "-o", help="Path to save output (docs/ and yaml). Defaults to current directory."
     ),
 ):
     """
     Generate a mkdocs website for a project including the API reference.
     """
     write_the_mkdocs(code_dir=code_dir, readme=readme, out_dir=out_dir)
```

### Comparing `write_the-0.6.0/write_the/cst/docstring_adder.py` & `write_the-0.6.1/write_the/cst/docstring_adder.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/write_the/cst/docstring_remover.py` & `write_the-0.6.1/write_the/cst/docstring_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/write_the/cst/function_and_class_collector.py` & `write_the-0.6.1/write_the/cst/function_and_class_collector.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/write_the/cst/node_extractor.py` & `write_the-0.6.1/write_the/cst/node_extractor.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/write_the/cst/node_remover.py` & `write_the-0.6.1/write_the/cst/node_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/write_the/cst/utils.py` & `write_the-0.6.1/write_the/cst/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/write_the/docs/chain.py` & `write_the-0.6.1/write_the/docs/chain.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/write_the/docs/write.py` & `write_the-0.6.1/write_the/docs/write.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/write_the/mkdocs/write.py` & `write_the-0.6.1/write_the/mkdocs/write.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/write_the/tests/chain.py` & `write_the-0.6.1/write_the/tests/chain.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/write_the/tests/write.py` & `write_the-0.6.1/write_the/tests/write.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/LICENSE.txt` & `write_the-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/README.md` & `write_the-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/pyproject.toml` & `write_the-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `write_the-0.6.0/PKG-INFO` & `write_the-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: write-the
-Version: 0.6.0
+Version: 0.6.1
 Summary: AI-powered Code Generation and Refactoring Tool
 Project-URL: Documentation, https://github.com/wytamma/write-the#readme
 Project-URL: Issues, https://github.com/wytamma/write-the/issues
 Project-URL: Source, https://github.com/wytamma/write-the
 Author-email: wytamma <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

