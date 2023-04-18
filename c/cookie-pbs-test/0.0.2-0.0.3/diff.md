# Comparing `tmp/cookie_pbs_test-0.0.2.tar.gz` & `tmp/cookie_pbs_test-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookie_pbs_test-0.0.2.tar", max compression
+gzip compressed data, was "cookie_pbs_test-0.0.3.tar", max compression
```

## Comparing `cookie_pbs_test-0.0.2.tar` & `cookie_pbs_test-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1073 2023-04-18 11:47:26.929900 cookie_pbs_test-0.0.2/LICENSE
--rw-r--r--   0        0        0     2067 2023-04-18 11:47:26.940324 cookie_pbs_test-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-04-18 11:47:26.944620 cookie_pbs_test-0.0.2/cookie_pbs_test/__init__.py
--rw-r--r--   0        0        0      313 2023-04-18 12:17:39.431710 cookie_pbs_test-0.0.2/cookie_pbs_test/main.py
--rw-r--r--   0        0        0     1680 2023-04-18 12:42:16.736549 cookie_pbs_test-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2587 1970-01-01 00:00:00.000000 cookie_pbs_test-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-18 11:47:26.929900 cookie_pbs_test-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2067 2023-04-18 11:47:26.940324 cookie_pbs_test-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 11:47:26.944620 cookie_pbs_test-0.0.3/cookie_pbs_test/__init__.py
+-rw-r--r--   0        0        0      313 2023-04-18 12:17:39.431710 cookie_pbs_test-0.0.3/cookie_pbs_test/main.py
+-rw-r--r--   0        0        0     1680 2023-04-18 12:44:55.469065 cookie_pbs_test-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2587 1970-01-01 00:00:00.000000 cookie_pbs_test-0.0.3/PKG-INFO
```

### Comparing `cookie_pbs_test-0.0.2/LICENSE` & `cookie_pbs_test-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cookie_pbs_test-0.0.2/README.md` & `cookie_pbs_test-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cookie_pbs_test-0.0.2/pyproject.toml` & `cookie_pbs_test-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cookie_pbs_test"
-version = "0.0.2"
+version = "0.0.3"
 description = "testing my cookiecutter "
 authors = ["Bernard Salanie <fbsalanie@columbia.edu>"]
 repository = "https://github.com/bsalanie/cookie-pbs-test"
 documentation = "https://bsalanie.github.io/cookie-pbs-test/"
 readme = "README.md"
 packages = [
   {include = "cookie_pbs_test"}
```

### Comparing `cookie_pbs_test-0.0.2/PKG-INFO` & `cookie_pbs_test-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookie-pbs-test
-Version: 0.0.2
+Version: 0.0.3
 Summary: testing my cookiecutter 
 Home-page: https://github.com/bsalanie/cookie-pbs-test
 Author: Bernard Salanie
 Author-email: fbsalanie@columbia.edu
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

