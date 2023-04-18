# Comparing `tmp/siggen-1.1.20221108.tar.gz` & `tmp/siggen-1.1.20230418.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siggen-1.1.20221108.tar", last modified: Tue Nov  8 17:28:18 2022, max compression
+gzip compressed data, was "siggen-1.1.20230418.tar", last modified: Tue Apr 18 16:11:09 2023, max compression
```

## Comparing `siggen-1.1.20221108.tar` & `siggen-1.1.20230418.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2022-11-08 17:28:18.519589 siggen-1.1.20221108/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      691 2019-04-02 20:07:00.000000 siggen-1.1.20221108/CODE_OF_CONDUCT.md
--rw-rw-r--   0 willkg    (1000) willkg    (1000)    15348 2022-11-08 17:27:22.000000 siggen-1.1.20221108/HISTORY.rst
--rw-rw-r--   0 willkg    (1000) willkg    (1000)    15977 2018-06-14 23:11:50.000000 siggen-1.1.20221108/LICENSE
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      236 2021-10-18 16:07:12.000000 siggen-1.1.20221108/MANIFEST.in
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      724 2022-11-07 18:57:11.000000 siggen-1.1.20221108/Makefile
--rw-rw-r--   0 willkg    (1000) willkg    (1000)    11890 2022-11-08 17:28:18.519589 siggen-1.1.20221108/PKG-INFO
--rw-rw-r--   0 willkg    (1000) willkg    (1000)    10927 2022-11-08 17:15:44.000000 siggen-1.1.20221108/README.rst
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2022-11-08 17:28:18.519589 siggen-1.1.20221108/bin/
--rwxrwxr-x   0 willkg    (1000) willkg    (1000)      516 2021-12-06 16:27:15.000000 siggen-1.1.20221108/bin/run_cmd_tests.sh
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      164 2022-11-08 17:28:18.519589 siggen-1.1.20221108/setup.cfg
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     2097 2022-11-07 19:49:47.000000 siggen-1.1.20221108/setup.py
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2022-11-08 17:28:18.519589 siggen-1.1.20221108/siggen/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      276 2022-11-08 17:27:22.000000 siggen-1.1.20221108/siggen/__init__.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     2909 2022-11-08 15:43:02.000000 siggen-1.1.20221108/siggen/cmd_doc.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     4452 2022-09-09 14:47:32.000000 siggen-1.1.20221108/siggen/cmd_fetch_data.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     8348 2022-11-08 15:48:03.000000 siggen-1.1.20221108/siggen/cmd_signature.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     1939 2022-11-08 15:48:03.000000 siggen-1.1.20221108/siggen/cmd_signify.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     4650 2022-11-08 15:48:03.000000 siggen-1.1.20221108/siggen/generator.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     2937 2022-11-08 15:43:02.000000 siggen-1.1.20221108/siggen/pipeline.rst
--rw-rw-r--   0 willkg    (1000) willkg    (1000)    35764 2022-11-08 15:48:03.000000 siggen-1.1.20221108/siggen/rules.py
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2022-11-08 17:28:18.519589 siggen-1.1.20221108/siggen/siglists/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     6836 2019-10-04 19:36:12.000000 siggen-1.1.20221108/siggen/siglists/README.rst
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     4326 2022-11-08 15:43:02.000000 siggen-1.1.20221108/siggen/siglists/irrelevant_signature_re.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     5381 2022-11-08 15:43:02.000000 siggen-1.1.20221108/siggen/siglists/prefix_signature_re.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     1095 2022-11-08 15:43:02.000000 siggen-1.1.20221108/siggen/siglists/signature_sentinels.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      241 2022-11-08 15:43:02.000000 siggen-1.1.20221108/siggen/siglists/signatures_with_line_numbers_re.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      702 2018-08-29 21:15:56.000000 siggen-1.1.20221108/siggen/siglists/trim_dll_signature_re.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     2947 2022-11-08 15:48:03.000000 siggen-1.1.20221108/siggen/siglists_utils.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)       40 2022-11-08 15:48:03.000000 siggen-1.1.20221108/siggen/socorro_sha.txt
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2022-11-08 17:28:18.519589 siggen-1.1.20221108/siggen/tests/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      200 2022-11-08 15:43:02.000000 siggen-1.1.20221108/siggen/tests/__init__.py
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2022-11-08 17:28:18.519589 siggen-1.1.20221108/siggen/tests/siglists/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)       77 2022-11-08 15:43:02.000000 siggen-1.1.20221108/siggen/tests/siglists/test-invalid-sig-list.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)       77 2022-11-08 15:43:02.000000 siggen-1.1.20221108/siggen/tests/siglists/test-sig-list.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      108 2022-11-08 15:43:02.000000 siggen-1.1.20221108/siggen/tests/siglists/test-valid-sig-list.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)    71053 2022-11-08 15:48:03.000000 siggen-1.1.20221108/siggen/tests/test_rules.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     2056 2022-11-08 15:48:03.000000 siggen-1.1.20221108/siggen/tests/test_siglists.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     2234 2022-11-08 15:48:03.000000 siggen-1.1.20221108/siggen/tests/test_signature_generator.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)    14493 2022-11-08 15:43:02.000000 siggen-1.1.20221108/siggen/tests/test_utils.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)    12586 2022-11-08 15:43:02.000000 siggen-1.1.20221108/siggen/utils.py
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2022-11-08 17:28:18.519589 siggen-1.1.20221108/siggen.egg-info/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)    11890 2022-11-08 17:28:18.000000 siggen-1.1.20221108/siggen.egg-info/PKG-INFO
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     1057 2022-11-08 17:28:18.000000 siggen-1.1.20221108/siggen.egg-info/SOURCES.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)        1 2022-11-08 17:28:18.000000 siggen-1.1.20221108/siggen.egg-info/dependency_links.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      130 2022-11-08 17:28:18.000000 siggen-1.1.20221108/siggen.egg-info/entry_points.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)       43 2022-11-08 17:28:18.000000 siggen-1.1.20221108/siggen.egg-info/requires.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)        7 2022-11-08 17:28:18.000000 siggen-1.1.20221108/siggen.egg-info/top_level.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      527 2022-11-07 18:57:11.000000 siggen-1.1.20221108/tox.ini
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2023-04-18 16:11:09.529395 siggen-1.1.20230418/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      691 2023-04-18 15:20:01.000000 siggen-1.1.20230418/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    18172 2023-04-18 16:10:15.000000 siggen-1.1.20230418/HISTORY.rst
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    15977 2023-04-18 15:20:01.000000 siggen-1.1.20230418/LICENSE
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      265 2023-04-18 16:10:15.000000 siggen-1.1.20230418/MANIFEST.in
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      722 2023-04-18 15:43:39.000000 siggen-1.1.20230418/Makefile
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    11890 2023-04-18 16:11:09.529395 siggen-1.1.20230418/PKG-INFO
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    10927 2023-04-18 15:20:01.000000 siggen-1.1.20230418/README.rst
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2023-04-18 16:11:09.525395 siggen-1.1.20230418/bin/
+-rwxrwxr-x   0 willkg    (1000) willkg    (1000)      516 2023-04-18 15:20:01.000000 siggen-1.1.20230418/bin/run_cmd_tests.sh
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     1023 2023-04-18 16:10:15.000000 siggen-1.1.20230418/pyproject.toml
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      166 2023-04-18 16:10:15.000000 siggen-1.1.20230418/requirements-dev.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)       38 2023-04-18 16:11:09.529395 siggen-1.1.20230418/setup.cfg
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     2097 2023-04-18 15:20:01.000000 siggen-1.1.20230418/setup.py
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2023-04-18 16:11:09.529395 siggen-1.1.20230418/siggen/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      276 2023-04-18 16:10:15.000000 siggen-1.1.20230418/siggen/__init__.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     2909 2023-04-18 15:20:06.000000 siggen-1.1.20230418/siggen/cmd_doc.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     4452 2023-04-18 15:20:01.000000 siggen-1.1.20230418/siggen/cmd_fetch_data.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     8348 2023-04-18 15:20:06.000000 siggen-1.1.20230418/siggen/cmd_signature.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     1939 2023-04-18 15:20:01.000000 siggen-1.1.20230418/siggen/cmd_signify.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     4650 2023-04-18 15:20:06.000000 siggen-1.1.20230418/siggen/generator.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     2937 2023-04-18 15:20:06.000000 siggen-1.1.20230418/siggen/pipeline.rst
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    36324 2023-04-18 15:24:55.000000 siggen-1.1.20230418/siggen/rules.py
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2023-04-18 16:11:09.529395 siggen-1.1.20230418/siggen/siglists/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     6836 2023-04-18 15:20:01.000000 siggen-1.1.20230418/siggen/siglists/README.rst
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     6269 2023-04-18 15:24:55.000000 siggen-1.1.20230418/siggen/siglists/irrelevant_signature_re.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     4901 2023-04-18 15:24:55.000000 siggen-1.1.20230418/siggen/siglists/prefix_signature_re.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     1095 2023-04-18 15:20:06.000000 siggen-1.1.20230418/siggen/siglists/signature_sentinels.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      241 2023-04-18 15:20:06.000000 siggen-1.1.20230418/siggen/siglists/signatures_with_line_numbers_re.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      702 2023-04-18 15:20:01.000000 siggen-1.1.20230418/siggen/siglists/trim_dll_signature_re.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     2941 2023-04-18 15:24:55.000000 siggen-1.1.20230418/siggen/siglists_utils.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)       40 2023-04-18 15:24:55.000000 siggen-1.1.20230418/siggen/socorro_sha.txt
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2023-04-18 16:11:09.529395 siggen-1.1.20230418/siggen/tests/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      200 2023-04-18 15:20:06.000000 siggen-1.1.20230418/siggen/tests/__init__.py
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2023-04-18 16:11:09.529395 siggen-1.1.20230418/siggen/tests/siglists/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)       77 2023-04-18 15:20:06.000000 siggen-1.1.20230418/siggen/tests/siglists/test-invalid-sig-list.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)       77 2023-04-18 15:20:06.000000 siggen-1.1.20230418/siggen/tests/siglists/test-sig-list.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      108 2023-04-18 15:20:06.000000 siggen-1.1.20230418/siggen/tests/siglists/test-valid-sig-list.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    72087 2023-04-18 15:24:55.000000 siggen-1.1.20230418/siggen/tests/test_rules.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     2056 2023-04-18 15:20:06.000000 siggen-1.1.20230418/siggen/tests/test_siglists.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     2234 2023-04-18 15:20:06.000000 siggen-1.1.20230418/siggen/tests/test_signature_generator.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    14493 2023-04-18 15:20:06.000000 siggen-1.1.20230418/siggen/tests/test_utils.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    12762 2023-04-18 15:24:55.000000 siggen-1.1.20230418/siggen/utils.py
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2023-04-18 16:11:09.529395 siggen-1.1.20230418/siggen.egg-info/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    11890 2023-04-18 16:11:09.000000 siggen-1.1.20230418/siggen.egg-info/PKG-INFO
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     1075 2023-04-18 16:11:09.000000 siggen-1.1.20230418/siggen.egg-info/SOURCES.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)        1 2023-04-18 16:11:09.000000 siggen-1.1.20230418/siggen.egg-info/dependency_links.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      130 2023-04-18 16:11:09.000000 siggen-1.1.20230418/siggen.egg-info/entry_points.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)       43 2023-04-18 16:11:09.000000 siggen-1.1.20230418/siggen.egg-info/requires.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)        7 2023-04-18 16:11:09.000000 siggen-1.1.20230418/siggen.egg-info/top_level.txt
```

### Comparing `siggen-1.1.20221108/CODE_OF_CONDUCT.md` & `siggen-1.1.20230418/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `siggen-1.1.20221108/LICENSE` & `siggen-1.1.20230418/LICENSE`

 * *Files identical despite different names*

### Comparing `siggen-1.1.20221108/Makefile` & `siggen-1.1.20230418/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 	rm -rf build dist ${PROJECT}.egg-info .tox .pytest-cache
 	rm -rf docs/_build/*
 	find ${PROJECT}/ tests/ -name __pycache__ | xargs rm -rf
 	find ${PROJECT}/ tests/ -name '*.pyc' | xargs rm -rf
 
 .PHONY: lint
 lint:  ## Lint files
-	tox -e py39-flake8
+	tox -e py39-lint
 
 .PHONY: test
 test:  ## Run tests
 	tox
 
 .PHONY: checkrot
 checkrot:  ## Check package rot for dev dependencies
```

### Comparing `siggen-1.1.20221108/PKG-INFO` & `siggen-1.1.20230418/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siggen
-Version: 1.1.20221108
+Version: 1.1.20230418
 Summary: Experimental extraction of Socorro signature generation
 Home-page: https://github.com/willkg/socorro-siggen
 Maintainer: Will Kahn-Greene
 Maintainer-email: willkg@mozilla.com
 License: Mozilla Public License v2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `siggen-1.1.20221108/README.rst` & `siggen-1.1.20230418/README.rst`

 * *Files identical despite different names*

### Comparing `siggen-1.1.20221108/bin/run_cmd_tests.sh` & `siggen-1.1.20230418/bin/run_cmd_tests.sh`

 * *Files identical despite different names*

### Comparing `siggen-1.1.20221108/setup.py` & `siggen-1.1.20230418/setup.py`

 * *Files identical despite different names*

### Comparing `siggen-1.1.20221108/siggen/cmd_doc.py` & `siggen-1.1.20230418/siggen/cmd_doc.py`

 * *Files identical despite different names*

### Comparing `siggen-1.1.20221108/siggen/cmd_fetch_data.py` & `siggen-1.1.20230418/siggen/cmd_fetch_data.py`

 * *Files identical despite different names*

### Comparing `siggen-1.1.20221108/siggen/cmd_signature.py` & `siggen-1.1.20230418/siggen/cmd_signature.py`

 * *Files identical despite different names*

### Comparing `siggen-1.1.20221108/siggen/cmd_signify.py` & `siggen-1.1.20230418/siggen/cmd_signify.py`

 * *Files identical despite different names*

### Comparing `siggen-1.1.20221108/siggen/generator.py` & `siggen-1.1.20230418/siggen/generator.py`

 * *Files identical despite different names*

### Comparing `siggen-1.1.20221108/siggen/pipeline.rst` & `siggen-1.1.20230418/siggen/pipeline.rst`

 * *Files identical despite different names*

### Comparing `siggen-1.1.20221108/siggen/rules.py` & `siggen-1.1.20230418/siggen/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
+from contextlib import suppress
 from functools import partial
 from itertools import islice
 import json
 import re
 
 from glom import glom
 
@@ -140,16 +141,17 @@
         # Remove rust-generated uniqueness hashes
         function = self.fixup_hash.sub("", function)
 
         return function
 
     def normalize_cpp_function(self, function, line):
         """Normalizes a single cpp frame with a function"""
-        # Drop member function cv/ref qualifiers like const, const&, &, and &&
-        for ref in ("const", "const&", "&&", "&"):
+        # Drop member function cv/ref qualifiers like const, const&, const &,
+        # &, and &&
+        for ref in ("const", "const&", "const &", "&&", "&"):
             if function.endswith(ref):
                 function = function[: -len(ref)].strip()
 
         # Convert `anonymous namespace' to (anonymous namespace)
 
         # Drop the prefix and return type if there is any if it's not operator
         # overloading--operator overloading syntax doesn't have the things
@@ -344,18 +346,16 @@
         # Shorten source_list to the first sentinel found
         sentinel_locations = []
         for a_sentinel in self.signature_sentinels:
             if type(a_sentinel) == tuple:
                 a_sentinel, condition_fn = a_sentinel
                 if not condition_fn(source_list):
                     continue
-            try:
+            with suppress(ValueError):
                 sentinel_locations.append(source_list.index(a_sentinel))
-            except ValueError:
-                pass
 
         if sentinel_locations:
             min_index = min(sentinel_locations)
             debug_notes.append(
                 'sentinel; starting at "{}" index {}'.format(
                     source_list[min_index], min_index
                 )
@@ -715,17 +715,28 @@
                 return True
 
         # Check the reason to see if it's one of a few values that indicate an OOM
         reason = crash_data.get("reason", None)
         if reason in self.oom_reason:
             return True
 
+        # Check js_large_allocation_failure to see if it's Reporting
+        js_large_allocation_failure = crash_data.get(
+            "js_large_allocation_failure", None
+        )
+        if js_large_allocation_failure == "Reporting":
+            return True
         return False
 
     def action(self, crash_data, result):
+        if crash_data.get("js_large_allocation_failure") == "Reporting":
+            # If a JSLargeAllocationFailure was Reporting, then it's an OOM | large
+            result.set_signature(self.name, f"OOM | large | {result.signature}")
+            return True
+
         try:
             size = int(crash_data.get("oom_allocation_size"))
         except (TypeError, AttributeError, KeyError):
             result.set_signature(self.name, f"OOM | unknown | {result.signature}")
             return True
 
         if size <= 262144:  # 256K
@@ -929,15 +940,15 @@
                 parts.append("(unknown)")
 
             conditions = [
                 # NOTE(willkg): The AsyncShutdownTimeout notation condition can either
                 # be a string that looks like a "name" or a dict with a "name" in it.
                 #
                 # This handles both variations.
-                c["name"] if isinstance(c, dict) else c
+                str(c["name"] if isinstance(c, dict) else c)
                 for c in shutdown_data.get("conditions") or []
             ]
             if conditions:
                 conditions.sort()
                 parts.append(",".join(conditions))
             else:
                 parts.append("(none)")
```

### Comparing `siggen-1.1.20221108/siggen/siglists/README.rst` & `siggen-1.1.20230418/siggen/siglists/README.rst`

 * *Files identical despite different names*

### Comparing `siggen-1.1.20221108/siggen/siglists/prefix_signature_re.txt` & `siggen-1.1.20230418/siggen/siglists/prefix_signature_re.txt`

 * *Files 20% similar despite different names*

```diff
@@ -29,17 +29,14 @@
 CleanupPerAppKey
 core::ops::function::Fn::call<T>
 core::option::expect_failed
 core::option::expect_none_failed
 core::ptr::drop_in_place
 core::ptr::real_drop_in_place
 core::result::unwrap_failed
-core::slice::index::slice_end_index_len_fail
-core::slice::index::slice_end_index_len_fail_rt
-core::slice::slice_index_order_fail
 core::str::slice_error_fail
 CreateFileMappingA
 __cxxabiv1::failed_throw
 CxxThrowException
 __delayLoadHelper2
 dlmalloc
 dvm
@@ -51,14 +48,15 @@
 fastzero_I
 FindElementCommon
 .*free
 ___forwarding___
 __forwarding_prep_0___
 __fsetlocking
 CCGraphBuilder::NoteXPCOMChild
+Gecko_AppendCString
 Gecko_FinalizeCString
 Gecko_SetLengthCString
 getanswer
 GetTickCount64
 gfxPlatform::Init
 gsignal
 handle_response
@@ -94,31 +92,26 @@
 memset
 MessageLoop::PostTask_Helper
 MessageLoop::PostTask
 mozalloc_abort
 mozalloc_handle_oom
 moz_malloc_size_of
 mozilla::CheckCheckedUnsafePtrs<T>::Check
-mozilla::detail::HashTable<.*>::
 mozilla::detail::InvalidArrayIndex_CRASH
 mozilla::detail::nsTStringRepr<T>::
 mozilla::dom::AutoJSAPI::Init
+mozilla::dom::Promise::
 mozilla::dom::ToJSValue
 mozilla::DOMEventTargetHelper::AddRef
 mozilla::Maybe<T>
-mozilla::MozPromise<T>::ThenCommand<T>::Track
-mozilla::MozPromise<T>::ThenInternal
 mozilla::net::ShutdownEvent::PostAndWait
-mozilla::OffTheBooksMutex::Lock
-SleepConditionVariable(CS|SRW)
 mozilla::TimeStamp::Now
 mozilla::TimeStamp::operator
 mozilla::TimeStampValue::operator-
 mozilla::TimeStampValue::operator!=
-mozilla::detail::MutexImpl::
 mozilla::detail::SupportCheckedUnsafePtrImpl<T>::~SupportCheckedUnsafePtrImpl
 mozilla::ipc::LogicError
 mozilla::ipc::MessageChannel::AssertWorkerThread
 mozilla::ipc::MessageChannel::Clear
 mozilla::ipc::MessageChannel::~MessageChannel
 mozilla::ipc::MessageChannel::Send
 mozilla::ipc::RPCChannel::Call
@@ -132,58 +125,53 @@
 mozilla::WrapNotNull<
 mozilla.*FatalError
 moz_xmalloc
 moz_xrealloc
 MOZ_CrashPrintf
 msvcr120\.dll@0x
 \<name omitted\>
+new\[\]
 NP_Shutdown
 (NS_)?(Lossy)?(Copy|Append|Convert).*UTF
 NS_CycleCollectorSuspect3
 -\[NSApplication _crashOnException:\]
 nsCRT::strcmp
 -\[NSObject doesNotRecognizeSelector:\]
 nsTArrayInfallibleAllocator
 NS_strcmp
 NS_strlen
-nsBaseHashtable<.*>::
-nsClassHashtable<.*>::
 nsCOMPtr
 NS_ABORT_OOM
-nsDataHashtable<.*>::
 NS_DebugBreak
 nsDebugImpl::Abort
 nsINode::GetParentNode
 nsThread::GetEvent
 [-+]\[NSException raise(:format:(arguments:)?)?\]
-nsInterfaceHashtable<.*>::
 nsINode::Slots
 nsObserverService
 nsTSubstring<.*>::
 NS_QuickSort
-nsRefPtr
 NSS
 nss
+nsStringBuffer::
 nsTArray<
 nsTArray_base<
 nsTArray_Impl<
-nsTHashtable<.*>::
 nsThread::Shutdown
 NtUser
 objc_exception_rethrow
 objc_exception_throw
 objc_addExceptionHandler
 objc_msgSend
 objc_release
 objc_retain
 operator new
 o_strcat_s
 <.*>::operator()
 pages_commit
-PLDHashTable::
 PL_
 port_
 PORT_
 _PR_
 PR_
 .*ProcessNextEvent
 pthread_cond_signal_thread_np
@@ -193,15 +181,14 @@
 _purecall
 raise
 RaiseFailFastException
 RpcpRaiseException
 RpcRaiseException
 realloc
 recv
-RefPtr
 ReleaseData
 _RTC_Terminate
 Rtl
 _Rtl
 __Rtl
 __rust_start_panic
 SEC_.*Item
@@ -218,19 +205,16 @@
 std::alloc::rust_oom
 std::_Allocate
 std::_Func_class<T>::
 std::_Func_impl_no_alloc<T>::
 std::_Func_impl<T>::
 std::_Function_base::_Base_manager<T>::
 std::_Function_handler<T>::
-std::_Hash<T>::
 std::list<.*>::
-std::collections::hash::map::
 std::vector<T>::_Emplace_reallocate<T>
-stdext::hash_map<T>::
 strcat
 strncmp
 ssl3_
 strchr
 strcmp
 strcpy
 .*strdup
```

### Comparing `siggen-1.1.20221108/siggen/siglists/signature_sentinels.txt` & `siggen-1.1.20230418/siggen/siglists/signature_sentinels.txt`

 * *Files identical despite different names*

### Comparing `siggen-1.1.20221108/siggen/siglists/trim_dll_signature_re.txt` & `siggen-1.1.20230418/siggen/siglists/trim_dll_signature_re.txt`

 * *Files identical despite different names*

### Comparing `siggen-1.1.20221108/siggen/siglists_utils.py` & `siggen-1.1.20230418/siggen/siglists_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,18 +78,18 @@
         for i, line in enumerate(fp):
             line = line.decode("utf-8", "strict").strip()
             if not line or line.startswith("#"):
                 continue
 
             try:
                 re.compile(line)
-            except Exception as ex:
+            except Exception as exc:
                 raise BadRegularExpressionLineError(
-                    "Regex error: {} in file {} at line {}".format(str(ex), filepath, i)
-                )
+                    f"Regex error: {exc} in file {filepath} at line {i}"
+                ) from exc
 
             lines.append(line)
 
     if source in _SPECIAL_EXTENDED_VALUES:
         lines = lines + _SPECIAL_EXTENDED_VALUES[source]
 
     return tuple(lines)
```

### Comparing `siggen-1.1.20221108/siggen/tests/test_rules.py` & `siggen-1.1.20230418/siggen/tests/test_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,18 +39,18 @@
     actual_function = rules.fix_missing_module(frame).get("function")
     assert actual_function == expected_function
 
 
 class TestCSignatureTool:
     @staticmethod
     def setup_config_c_sig_tool(
-        ig=["ignored1"],
-        pr=["pre1", "pre2"],
-        si=["fnNeedNumber"],
-        td=[r"foo32\.dll.*"],
+        ig=("ignored1",),
+        pr=("pre1", "pre2"),
+        si=("fnNeedNumber",),
+        td=(r"foo32\.dll.*",),
         ss=("sentinel", ("sentinel2", lambda x: "ff" in x)),
     ):
         tool = rules.CSignatureTool()
         tool.irrelevant_signature_re = tool.build_re(ig)
         tool.prefix_signature_re = tool.build_re(pr)
         tool.signatures_with_line_numbers_re = tool.build_re(si)
         tool.signature_sentinels = ss
@@ -361,14 +361,19 @@
                 "JSObject::allocKindForTenure",
             ),
             (
                 "mozilla::jni::GlobalRef<mozilla::jni::Object>::operator=(mozilla::jni::Ref<mozilla::jni::Object, _jobject*> const&)&",
                 "23",  # noqa
                 "mozilla::jni::GlobalRef<T>::operator=",
             ),
+            (
+                "mozilla::Maybe<unsigned long>::value() const &",
+                "23",  # noqa
+                "mozilla::Maybe<T>::value",
+            ),
             # Normalize anonymous namespace
             ("`anonymous namespace'::foo", "23", "(anonymous namespace)::foo"),
             ("(anonymous namespace)::foo", "23", "(anonymous namespace)::foo"),
             # Normalize lambda numbers
             (
                 "ShutdownWorkThreads::$_52::__invoke",
                 "23",
@@ -1372,14 +1377,29 @@
     def test_predicate_reason(self, reason, expected):
         crash_data = {"reason": reason}
         result = generator.Result()
         result.signature = "Text"
         rule = rules.OOMSignature()
         assert rule.predicate(crash_data, result) is expected
 
+    @pytest.mark.parametrize(
+        "value, expected",
+        [
+            (None, False),
+            ("Reporting", True),
+            ("Reported", False),
+        ],
+    )
+    def test_predicate_js_large_allocation_failure(self, value, expected):
+        crash_data = {"js_large_allocation_failure": value}
+        result = generator.Result()
+        result.signature = "Text"
+        rule = rules.OOMSignature()
+        assert rule.predicate(crash_data, result) is expected
+
     def test_action_success(self):
         crash_data = {}
         result = generator.Result()
         result.signature = "hello"
         rule = rules.OOMSignature()
         action_result = rule.action(crash_data, result)
 
@@ -1401,14 +1421,25 @@
         result = generator.Result()
         result.signature = "hello"
 
         rule = rules.OOMSignature()
         action_result = rule.action(crash_data, result)
 
         assert action_result is True
+        assert result.signature == "OOM | large | hello"
+
+    def test_action_js_large_allocation_failure(self):
+        crash_data = {"js_large_allocation_failure": "Reporting"}
+        result = generator.Result()
+        result.signature = "hello"
+
+        rule = rules.OOMSignature()
+        action_result = rule.action(crash_data, result)
+
+        assert action_result is True
         assert result.signature == "OOM | large | hello"
 
 
 class TestBadHardware:
     @pytest.mark.parametrize(
         "reason, expected",
         [
```

### Comparing `siggen-1.1.20221108/siggen/tests/test_siglists.py` & `siggen-1.1.20230418/siggen/tests/test_siglists.py`

 * *Files identical despite different names*

### Comparing `siggen-1.1.20221108/siggen/tests/test_signature_generator.py` & `siggen-1.1.20230418/siggen/tests/test_signature_generator.py`

 * *Files identical despite different names*

### Comparing `siggen-1.1.20221108/siggen/tests/test_utils.py` & `siggen-1.1.20230418/siggen/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `siggen-1.1.20221108/siggen/utils.py` & `siggen-1.1.20230418/siggen/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,20 @@
         "threads": glom(processed_crash, "json_dump.threads", default=None),
         # text or None
         "os": glom(processed_crash, "json_dump.system_info.os", default=None),
         # int or None
         "oom_allocation_size": int_or_none(
             glom(processed_crash, "oom_allocation_size", default=None)
         ),
+        # str or None
+        "js_large_allocation_failure": glom(
+            processed_crash,
+            "js_large_allocation_failure",
+            default=None,
+        ),
         # text or None
         "abort_message": glom(processed_crash, "abort_message", default=None),
         # text or None
         "mdsw_status_string": glom(processed_crash, "mdsw_status_string", default=None),
         # text json with "phase", "conditions" (complicated--see code) or None
         "async_shutdown_timeout": glom(
             processed_crash, "async_shutdown_timeout", default=None
@@ -296,15 +302,15 @@
 
     # Keeps track of open delimiters so we can match and close them
     levels = []
 
     # The current token we're building
     current = []
 
-    for i, char in enumerate(function):
+    for _, char in enumerate(function):
         if char in OPEN:
             levels.append(char)
             current.append(char)
         elif char in CLOSE:
             if levels and DELIMITERS[levels[-1]] == char:
                 levels.pop()
                 current.append(char)
```

### Comparing `siggen-1.1.20221108/siggen.egg-info/PKG-INFO` & `siggen-1.1.20230418/siggen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siggen
-Version: 1.1.20221108
+Version: 1.1.20230418
 Summary: Experimental extraction of Socorro signature generation
 Home-page: https://github.com/willkg/socorro-siggen
 Maintainer: Will Kahn-Greene
 Maintainer-email: willkg@mozilla.com
 License: Mozilla Public License v2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `siggen-1.1.20221108/siggen.egg-info/SOURCES.txt` & `siggen-1.1.20230418/siggen.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 CODE_OF_CONDUCT.md
 HISTORY.rst
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
-setup.cfg
+pyproject.toml
+requirements-dev.txt
 setup.py
-tox.ini
 bin/run_cmd_tests.sh
 siggen/__init__.py
 siggen/cmd_doc.py
 siggen/cmd_fetch_data.py
 siggen/cmd_signature.py
 siggen/cmd_signify.py
 siggen/generator.py
```

