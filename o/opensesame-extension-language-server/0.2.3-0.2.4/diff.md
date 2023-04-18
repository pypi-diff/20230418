# Comparing `tmp/opensesame_extension_language_server-0.2.3.tar.gz` & `tmp/opensesame_extension_language_server-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensesame_extension_language_server-0.2.3.tar", max compression
+gzip compressed data, was "opensesame_extension_language_server-0.2.4.tar", max compression
```

## Comparing `opensesame_extension_language_server-0.2.3.tar` & `opensesame_extension_language_server-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      283 2023-03-20 08:56:18.047829 opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/__init__.py
--rw-r--r--   0        0        0      534 2023-03-20 08:56:18.047829 opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/__init__.py
--rw-r--r--   0        0        0     4555 2023-03-20 08:56:18.047829 opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/language_server.py
--rw-r--r--   0        0        0      932 2023-03-20 08:56:18.047829 opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/__init__.py
--rw-r--r--   0        0        0     1150 2023-03-20 08:56:18.047829 opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_css_code_edit.py
--rw-r--r--   0        0        0     1111 2023-03-20 08:56:18.047829 opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_json_code_edit.py
--rw-r--r--   0        0        0     7338 2023-03-20 08:56:18.047829 opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_language_server_code_edit.py
--rw-r--r--   0        0        0     1961 2023-03-20 08:56:18.047829 opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_python_code_edit.py
--rw-r--r--   0        0        0     1149 2023-03-20 08:56:18.047829 opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_r_code_edit.py
--rw-r--r--   0        0        0     1271 2023-03-20 08:56:18.047829 opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_typescript_code_edit.py
--rw-r--r--   0        0        0     1245 2023-03-20 08:56:18.051829 opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_yaml_code_edit.py
--rw-r--r--   0        0        0     5634 2023-03-20 08:56:18.051829 opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/preferences.ui
--rw-r--r--   0        0        0      762 2023-03-20 08:56:18.051829 opensesame_extension_language_server-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1040 2023-03-20 08:56:18.051829 opensesame_extension_language_server-0.2.3/readme.md
--rw-r--r--   0        0        0     1923 1970-01-01 00:00:00.000000 opensesame_extension_language_server-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      283 2023-04-18 14:50:59.884858 opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/__init__.py
+-rw-r--r--   0        0        0      534 2023-04-18 14:50:59.884858 opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/__init__.py
+-rw-r--r--   0        0        0     4555 2023-04-18 14:50:59.884858 opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/language_server.py
+-rw-r--r--   0        0        0      932 2023-04-18 14:50:59.884858 opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/__init__.py
+-rw-r--r--   0        0        0     1150 2023-04-18 14:50:59.884858 opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_css_code_edit.py
+-rw-r--r--   0        0        0     1111 2023-04-18 14:50:59.884858 opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_json_code_edit.py
+-rw-r--r--   0        0        0     7338 2023-04-18 14:50:59.884858 opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_language_server_code_edit.py
+-rw-r--r--   0        0        0     1961 2023-04-18 14:50:59.884858 opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_python_code_edit.py
+-rw-r--r--   0        0        0     1149 2023-04-18 14:50:59.884858 opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_r_code_edit.py
+-rw-r--r--   0        0        0     1271 2023-04-18 14:50:59.884858 opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_typescript_code_edit.py
+-rw-r--r--   0        0        0     1245 2023-04-18 14:50:59.884858 opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_yaml_code_edit.py
+-rw-r--r--   0        0        0     5634 2023-04-18 14:50:59.884858 opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/preferences.ui
+-rw-r--r--   0        0        0      761 2023-04-18 14:50:59.884858 opensesame_extension_language_server-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1040 2023-04-18 14:50:59.884858 opensesame_extension_language_server-0.2.4/readme.md
+-rw-r--r--   0        0        0     1922 1970-01-01 00:00:00.000000 opensesame_extension_language_server-0.2.4/PKG-INFO
```

### Comparing `opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/__init__.py` & `opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/__init__.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/language_server.py` & `opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/language_server.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/__init__.py` & `opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_css_code_edit.py` & `opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_css_code_edit.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_json_code_edit.py` & `opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_json_code_edit.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_language_server_code_edit.py` & `opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_language_server_code_edit.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_python_code_edit.py` & `opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_python_code_edit.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_r_code_edit.py` & `opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_r_code_edit.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_typescript_code_edit.py` & `opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_typescript_code_edit.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_yaml_code_edit.py` & `opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/lsp_code_edit_widgets/_yaml_code_edit.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_language_server-0.2.3/opensesame_extensions/language_server/language_server/preferences.ui` & `opensesame_extension_language_server-0.2.4/opensesame_extensions/language_server/language_server/preferences.ui`

 * *Files identical despite different names*

### Comparing `opensesame_extension_language_server-0.2.3/pyproject.toml` & `opensesame_extension_language_server-0.2.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "opensesame-extension-language_server"
-version = "0.2.3"
+version = "0.2.4"
 description = "Adds language-server support to OpenSesame and Rapunzel"
 authors = ["Sebastiaan Mathôt <s.mathot@cogsci.nl>"]
 readme = "readme.md"
 packages = [
     {include = "opensesame_extensions"},
 ]
 license = "COPYING"
 homepage = "https://rapunzel.cogsci.nl/manual/language-server/"
 repository = "https://github.com/open-cogsci/opensesame-extension-language_server"
 
 [tool.poetry.dependencies]
 python = ">= 3.7"
 opensesame-core = ">= 4.0.0a0"
-"pyqode3-language-server" = ">= 0.2.1"
+"pyqode.language-server" = ">= 0.2.3"
 
 [tool.wheel2deb.dependencies]
 python = ">= 3.7"
 opensesame = ">= 3.99.99"
-"pyqode-language-server" = ">= 0.2.1"
+"pyqode-language-server" = ">= 0.2.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `opensesame_extension_language_server-0.2.3/readme.md` & `opensesame_extension_language_server-0.2.4/readme.md`

 * *Files identical despite different names*

### Comparing `opensesame_extension_language_server-0.2.3/PKG-INFO` & `opensesame_extension_language_server-0.2.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: opensesame-extension-language-server
-Version: 0.2.3
+Version: 0.2.4
 Summary: Adds language-server support to OpenSesame and Rapunzel
 Home-page: https://rapunzel.cogsci.nl/manual/language-server/
 License: COPYING
 Author: Sebastiaan Mathôt
 Author-email: s.mathot@cogsci.nl
 Requires-Python: >=3.7
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: opensesame-core (>=4.0.0a0)
-Requires-Dist: pyqode3-language-server (>=0.2.1)
+Requires-Dist: pyqode.language-server (>=0.2.3)
 Project-URL: Repository, https://github.com/open-cogsci/opensesame-extension-language_server
 Description-Content-Type: text/markdown
 
 # Language-server extension for OpenSesame and Rapunzel
 
 Copyright 2020-2023 Sebastiaan Mathôt (@smathot)
```

