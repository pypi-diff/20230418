# Comparing `tmp/write_the-0.6.1.tar.gz` & `tmp/write_the-0.6.2.tar.gz`

## Comparing `write_the-0.6.1.tar` & `write_the-0.6.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 write_the-0.6.1/mkdocs.yml
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 write_the-0.6.1/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 write_the-0.6.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.6.1/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 write_the-0.6.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 write_the-0.6.1/.pytest_cache/README.md
--rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 write_the-0.6.1/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0    10819 2020-02-02 00:00:00.000000 write_the-0.6.1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 write_the-0.6.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.6.1/docs/CNAME
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 write_the-0.6.1/docs/index.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 write_the-0.6.1/docs/reference/cli.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 write_the-0.6.1/docs/reference/cst.md
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 write_the-0.6.1/docs/reference/docs.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 write_the-0.6.1/docs/reference/mkdocs.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 write_the-0.6.1/docs/reference/tests.md
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.6.1/docs/reference/utils.md
--rw-r--r--   0        0        0   123108 2020-02-02 00:00:00.000000 write_the-0.6.1/images/docs-help.png
--rw-r--r--   0        0        0    84667 2020-02-02 00:00:00.000000 write_the-0.6.1/images/mkdocs-help.png
--rw-r--r--   0        0        0   161159 2020-02-02 00:00:00.000000 write_the-0.6.1/images/multiply.png
--rw-r--r--   0        0        0   139626 2020-02-02 00:00:00.000000 write_the-0.6.1/images/tests-help.png
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 write_the-0.6.1/images/write-the-icon.svg
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 write_the-0.6.1/tests/test_cli_main.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 write_the-0.6.1/tests/test_cst_docstring_adder.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 write_the-0.6.1/tests/test_cst_docstring_remover.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 write_the-0.6.1/tests/test_cst_function_and_class_collector.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 write_the-0.6.1/tests/test_cst_node_extractor.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 write_the-0.6.1/tests/test_cst_node_remover.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 write_the-0.6.1/tests/test_cst_utils.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.6.1/tests/data/multiply.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 write_the-0.6.1/tests/data/multiply_docstring.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/__about__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/__main__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/utils.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/cli/__init__.py
--rw-r--r--   0        0        0     6759 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/cli/main.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/cst/__init__.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/cst/docstring_adder.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/cst/docstring_remover.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/cst/function_and_class_collector.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/cst/node_extractor.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/cst/node_remover.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/cst/utils.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/docs/__init__.py
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/docs/chain.py
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/docs/write.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/mkdocs/__init__.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/mkdocs/write.py
--rwxr-xr-x   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/tests/__init__.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/tests/chain.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 write_the-0.6.1/write_the/tests/write.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 write_the-0.6.1/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.6.1/LICENSE.txt
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 write_the-0.6.1/README.md
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 write_the-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 write_the-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 write_the-0.6.2/mkdocs.yml
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 write_the-0.6.2/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 write_the-0.6.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.6.2/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 write_the-0.6.2/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 write_the-0.6.2/.pytest_cache/README.md
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 write_the-0.6.2/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0    10819 2020-02-02 00:00:00.000000 write_the-0.6.2/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 write_the-0.6.2/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.6.2/docs/CNAME
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 write_the-0.6.2/docs/index.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 write_the-0.6.2/docs/reference/cli.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 write_the-0.6.2/docs/reference/cst.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 write_the-0.6.2/docs/reference/docs.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 write_the-0.6.2/docs/reference/mkdocs.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 write_the-0.6.2/docs/reference/tests.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.6.2/docs/reference/utils.md
+-rw-r--r--   0        0        0   123108 2020-02-02 00:00:00.000000 write_the-0.6.2/images/docs-help.png
+-rw-r--r--   0        0        0    84667 2020-02-02 00:00:00.000000 write_the-0.6.2/images/mkdocs-help.png
+-rw-r--r--   0        0        0   161159 2020-02-02 00:00:00.000000 write_the-0.6.2/images/multiply.png
+-rw-r--r--   0        0        0   139626 2020-02-02 00:00:00.000000 write_the-0.6.2/images/tests-help.png
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 write_the-0.6.2/images/write-the-icon.svg
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 write_the-0.6.2/tests/test_cli_main.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 write_the-0.6.2/tests/test_cst_docstring_adder.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 write_the-0.6.2/tests/test_cst_docstring_remover.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 write_the-0.6.2/tests/test_cst_function_and_class_collector.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 write_the-0.6.2/tests/test_cst_node_extractor.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 write_the-0.6.2/tests/test_cst_node_remover.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 write_the-0.6.2/tests/test_cst_utils.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.6.2/tests/data/multiply.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 write_the-0.6.2/tests/data/multiply_docstring.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/__about__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/__main__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/utils.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/cli/__init__.py
+-rw-r--r--   0        0        0     6759 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/cli/main.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/cst/__init__.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/cst/docstring_adder.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/cst/docstring_remover.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/cst/function_and_class_collector.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/cst/node_extractor.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/cst/node_remover.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/cst/utils.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/docs/__init__.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/docs/chain.py
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/docs/write.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/mkdocs/__init__.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/mkdocs/write.py
+-rwxr-xr-x   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/tests/__init__.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/tests/chain.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/tests/write.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 write_the-0.6.2/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.6.2/LICENSE.txt
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 write_the-0.6.2/README.md
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 write_the-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 write_the-0.6.2/PKG-INFO
```

### Comparing `write_the-0.6.1/mkdocs.yml` & `write_the-0.6.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/.github/workflows/tests.yml` & `write_the-0.6.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/.pytest_cache/v/cache/lastfailed` & `write_the-0.6.2/.pytest_cache/v/cache/lastfailed`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/.pytest_cache/v/cache/nodeids` & `write_the-0.6.2/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/docs/index.md` & `write_the-0.6.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/images/docs-help.png` & `write_the-0.6.2/images/docs-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/images/mkdocs-help.png` & `write_the-0.6.2/images/mkdocs-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/images/multiply.png` & `write_the-0.6.2/images/multiply.png`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/images/tests-help.png` & `write_the-0.6.2/images/tests-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/images/write-the-icon.svg` & `write_the-0.6.2/images/write-the-icon.svg`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/tests/test_cli_main.py` & `write_the-0.6.2/tests/test_cli_main.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/tests/test_cst_docstring_adder.py` & `write_the-0.6.2/tests/test_cst_docstring_adder.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/tests/test_cst_docstring_remover.py` & `write_the-0.6.2/tests/test_cst_docstring_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/tests/test_cst_function_and_class_collector.py` & `write_the-0.6.2/tests/test_cst_function_and_class_collector.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/tests/test_cst_node_extractor.py` & `write_the-0.6.2/tests/test_cst_node_extractor.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/tests/test_cst_node_remover.py` & `write_the-0.6.2/tests/test_cst_node_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/tests/test_cst_utils.py` & `write_the-0.6.2/tests/test_cst_utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/write_the/utils.py` & `write_the-0.6.2/write_the/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/write_the/cli/main.py` & `write_the-0.6.2/write_the/cli/main.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/write_the/cst/docstring_adder.py` & `write_the-0.6.2/write_the/cst/docstring_adder.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/write_the/cst/docstring_remover.py` & `write_the-0.6.2/write_the/cst/docstring_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/write_the/cst/function_and_class_collector.py` & `write_the-0.6.2/write_the/cst/function_and_class_collector.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/write_the/cst/node_extractor.py` & `write_the-0.6.2/write_the/cst/node_extractor.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/write_the/cst/node_remover.py` & `write_the-0.6.2/write_the/cst/node_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/write_the/cst/utils.py` & `write_the-0.6.2/write_the/cst/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/write_the/docs/chain.py` & `write_the-0.6.2/write_the/docs/chain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from langchain.prompts import PromptTemplate
 from langchain.chains import LLMChain
 from langchain.llms import OpenAI
 import unittest.mock as mock
 
-llm = OpenAI(temperature=0, max_tokens=2000)
+
 docs_template = """
 Write Google style docstrings for the following code, using the multi-line format with a description and examples. 
 The first lines describe the code. Include parameter type definitions where possible, and specify any exceptions raised and side effects of the function. 
 For functions with multiple return values or ambiguous behaviour, provide clear guidelines for documenting the behaviour. 
 Please refer to the Google style guide for more information. Any notes should be include in the `Notes:` section of the docstring. Only return the docstring its self. 
 Return each docstring on a single line with the name of the function/class as the key and the docstring as the value. Separate each result by a newline. 
 If the function is a method return the name in the format Class.method. The Class docstrings should contain Description and Attributes. 
 Each result should be separated by multiple newlines. \n---\nEXAMPLE\n---\n\ndef add(a, b): \n    return a + b \nHere are formatted docstrings for only add:\n\nadd:\n  Sums 2 numbers.\n  Args:\n    a (int): The first number to add.\n    b (int): The second number to add.\n  Returns:\n    int: The sum of `a` and `b`.\n  Examples:\n    >>> add(1, 2)\n    3\n\n\n\n---\nCODE\n---\n{code}\nHere are formatted docstrings for only {nodes}:\n"""
-docs_prompt = PromptTemplate(input_variables=["code", "nodes"], template=docs_template)
-docs_chain = LLMChain(llm=llm, prompt=docs_prompt)
-
 
 def run(code, nodes: list) -> str:
     """
     Generates docstrings for a given code and list of nodes.
     Args:
       code (str): The code to generate docstrings for.
       nodes (list): A list of nodes to generate docstrings for.
@@ -28,9 +25,12 @@
       >>> run('from langchain.prompts import PromptTemplate', ['PromptTemplate'])
       'PromptTemplate:
         A class for generating prompts.
         Attributes:
           input_variables (list): A list of input variables for the prompt.
           template (str): The template for the prompt.'
     """
+    llm = OpenAI(temperature=0, max_tokens=2000)
+    docs_prompt = PromptTemplate(input_variables=["code", "nodes"], template=docs_template)
+    docs_chain = LLMChain(llm=llm, prompt=docs_prompt)
     nodes = ",".join(nodes)
     return docs_chain.predict(code=code, nodes=nodes)
```

### Comparing `write_the-0.6.1/write_the/docs/write.py` & `write_the-0.6.2/write_the/docs/write.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/write_the/mkdocs/write.py` & `write_the-0.6.2/write_the/mkdocs/write.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/write_the/tests/chain.py` & `write_the-0.6.2/write_the/tests/chain.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/write_the/tests/write.py` & `write_the-0.6.2/write_the/tests/write.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/LICENSE.txt` & `write_the-0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/README.md` & `write_the-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/pyproject.toml` & `write_the-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `write_the-0.6.1/PKG-INFO` & `write_the-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: write-the
-Version: 0.6.1
+Version: 0.6.2
 Summary: AI-powered Code Generation and Refactoring Tool
 Project-URL: Documentation, https://github.com/wytamma/write-the#readme
 Project-URL: Issues, https://github.com/wytamma/write-the/issues
 Project-URL: Source, https://github.com/wytamma/write-the
 Author-email: wytamma <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

