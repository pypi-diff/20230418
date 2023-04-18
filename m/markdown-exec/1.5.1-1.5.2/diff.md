# Comparing `tmp/markdown_exec-1.5.1.tar.gz` & `tmp/markdown_exec-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_exec-1.5.1.tar", last modified: Mon Apr 17 14:03:25 2023, max compression
+gzip compressed data, was "markdown_exec-1.5.2.tar", last modified: Tue Apr 18 09:59:47 2023, max compression
```

## Comparing `markdown_exec-1.5.1.tar` & `markdown_exec-1.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      754 2023-04-10 19:47:46.084183 markdown_exec-1.5.1/LICENSE
--rw-r--r--   0        0        0     3354 2023-04-16 18:40:30.714066 markdown_exec-1.5.1/README.md
--rw-r--r--   0        0        0     3595 2023-04-17 14:03:25.271466 markdown_exec-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     4162 2023-04-17 12:40:04.204193 markdown_exec-1.5.1/src/markdown_exec/__init__.py
--rw-r--r--   0        0        0     5657 2023-04-16 18:40:30.810731 markdown_exec-1.5.1/src/markdown_exec/ansi.css
--rw-r--r--   0        0        0       51 2022-11-24 19:29:10.145475 markdown_exec-1.5.1/src/markdown_exec/formatters/__init__.py
--rw-r--r--   0        0        0     4554 2023-04-17 12:40:04.204193 markdown_exec-1.5.1/src/markdown_exec/formatters/base.py
--rw-r--r--   0        0        0      846 2023-04-16 18:40:30.810731 markdown_exec-1.5.1/src/markdown_exec/formatters/bash.py
--rw-r--r--   0        0        0      815 2023-04-16 18:40:30.810731 markdown_exec-1.5.1/src/markdown_exec/formatters/console.py
--rw-r--r--   0        0        0      276 2023-04-16 18:40:30.810731 markdown_exec-1.5.1/src/markdown_exec/formatters/markdown.py
--rw-r--r--   0        0        0      854 2023-04-17 14:01:39.509387 markdown_exec-1.5.1/src/markdown_exec/formatters/pycon.py
--rw-r--r--   0        0        0     2406 2023-04-16 18:40:30.810731 markdown_exec-1.5.1/src/markdown_exec/formatters/python.py
--rw-r--r--   0        0        0      836 2023-04-16 18:40:30.810731 markdown_exec-1.5.1/src/markdown_exec/formatters/sh.py
--rw-r--r--   0        0        0     2046 2023-04-16 18:40:30.810731 markdown_exec-1.5.1/src/markdown_exec/formatters/tree.py
--rw-r--r--   0        0        0     2089 2023-04-16 18:40:30.834064 markdown_exec-1.5.1/src/markdown_exec/logger.py
--rw-r--r--   0        0        0     2450 2023-04-17 11:02:02.812131 markdown_exec-1.5.1/src/markdown_exec/mkdocs_plugin.py
--rw-r--r--   0        0        0     4261 2023-04-17 13:48:51.537991 markdown_exec-1.5.1/src/markdown_exec/processors.py
--rw-r--r--   0        0        0        0 2023-04-10 19:47:45.977517 markdown_exec-1.5.1/src/markdown_exec/py.typed
--rw-r--r--   0        0        0     6144 2023-04-17 13:49:52.704027 markdown_exec-1.5.1/src/markdown_exec/rendering.py
--rw-r--r--   0        0        0      166 2023-04-10 19:47:45.974184 markdown_exec-1.5.1/tests/__init__.py
--rw-r--r--   0        0        0      635 2023-04-16 18:40:30.837398 markdown_exec-1.5.1/tests/conftest.py
--rw-r--r--   0        0        0     1443 2023-04-16 18:40:30.854064 markdown_exec-1.5.1/tests/test_base_formatter.py
--rw-r--r--   0        0        0      630 2023-04-17 13:49:16.754400 markdown_exec-1.5.1/tests/test_converter.py
--rw-r--r--   0        0        0     4337 2023-04-17 14:00:35.590141 markdown_exec-1.5.1/tests/test_python.py
--rw-r--r--   0        0        0     2027 2023-04-16 18:40:30.854064 markdown_exec-1.5.1/tests/test_shell.py
--rw-r--r--   0        0        0     2335 2023-04-17 12:40:04.207527 markdown_exec-1.5.1/tests/test_toc.py
--rw-r--r--   0        0        0      488 2023-04-16 18:40:30.854064 markdown_exec-1.5.1/tests/test_tree.py
--rw-r--r--   0        0        0      995 2022-02-06 15:25:17.240565 markdown_exec-1.5.1/tests/test_validator.py
--rw-r--r--   0        0        0     4874 1970-01-01 00:00:00.000000 markdown_exec-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-04-10 19:47:46.084183 markdown_exec-1.5.2/LICENSE
+-rw-r--r--   0        0        0     3354 2023-04-16 18:40:30.714066 markdown_exec-1.5.2/README.md
+-rw-r--r--   0        0        0     3595 2023-04-18 09:59:47.521432 markdown_exec-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4162 2023-04-17 12:40:04.204193 markdown_exec-1.5.2/src/markdown_exec/__init__.py
+-rw-r--r--   0        0        0     5657 2023-04-16 18:40:30.810731 markdown_exec-1.5.2/src/markdown_exec/ansi.css
+-rw-r--r--   0        0        0       51 2022-11-24 19:29:10.145475 markdown_exec-1.5.2/src/markdown_exec/formatters/__init__.py
+-rw-r--r--   0        0        0     4554 2023-04-17 12:40:04.204193 markdown_exec-1.5.2/src/markdown_exec/formatters/base.py
+-rw-r--r--   0        0        0      846 2023-04-16 18:40:30.810731 markdown_exec-1.5.2/src/markdown_exec/formatters/bash.py
+-rw-r--r--   0        0        0      815 2023-04-16 18:40:30.810731 markdown_exec-1.5.2/src/markdown_exec/formatters/console.py
+-rw-r--r--   0        0        0      276 2023-04-16 18:40:30.810731 markdown_exec-1.5.2/src/markdown_exec/formatters/markdown.py
+-rw-r--r--   0        0        0      854 2023-04-17 14:01:39.509387 markdown_exec-1.5.2/src/markdown_exec/formatters/pycon.py
+-rw-r--r--   0        0        0     2406 2023-04-16 18:40:30.810731 markdown_exec-1.5.2/src/markdown_exec/formatters/python.py
+-rw-r--r--   0        0        0      836 2023-04-16 18:40:30.810731 markdown_exec-1.5.2/src/markdown_exec/formatters/sh.py
+-rw-r--r--   0        0        0     2046 2023-04-16 18:40:30.810731 markdown_exec-1.5.2/src/markdown_exec/formatters/tree.py
+-rw-r--r--   0        0        0     2089 2023-04-16 18:40:30.834064 markdown_exec-1.5.2/src/markdown_exec/logger.py
+-rw-r--r--   0        0        0     2620 2023-04-18 09:56:51.630595 markdown_exec-1.5.2/src/markdown_exec/mkdocs_plugin.py
+-rw-r--r--   0        0        0     4261 2023-04-17 13:48:51.537991 markdown_exec-1.5.2/src/markdown_exec/processors.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:47:45.977517 markdown_exec-1.5.2/src/markdown_exec/py.typed
+-rw-r--r--   0        0        0     6144 2023-04-18 09:45:50.883905 markdown_exec-1.5.2/src/markdown_exec/rendering.py
+-rw-r--r--   0        0        0      166 2023-04-10 19:47:45.974184 markdown_exec-1.5.2/tests/__init__.py
+-rw-r--r--   0        0        0      635 2023-04-16 18:40:30.837398 markdown_exec-1.5.2/tests/conftest.py
+-rw-r--r--   0        0        0     1443 2023-04-16 18:40:30.854064 markdown_exec-1.5.2/tests/test_base_formatter.py
+-rw-r--r--   0        0        0      630 2023-04-17 13:49:16.754400 markdown_exec-1.5.2/tests/test_converter.py
+-rw-r--r--   0        0        0     4337 2023-04-17 14:00:35.590141 markdown_exec-1.5.2/tests/test_python.py
+-rw-r--r--   0        0        0     2027 2023-04-16 18:40:30.854064 markdown_exec-1.5.2/tests/test_shell.py
+-rw-r--r--   0        0        0     2335 2023-04-17 12:40:04.207527 markdown_exec-1.5.2/tests/test_toc.py
+-rw-r--r--   0        0        0      488 2023-04-16 18:40:30.854064 markdown_exec-1.5.2/tests/test_tree.py
+-rw-r--r--   0        0        0      995 2022-02-06 15:25:17.240565 markdown_exec-1.5.2/tests/test_validator.py
+-rw-r--r--   0        0        0     4874 1970-01-01 00:00:00.000000 markdown_exec-1.5.2/PKG-INFO
```

### Comparing `markdown_exec-1.5.1/LICENSE` & `markdown_exec-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.1/README.md` & `markdown_exec-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.1/pyproject.toml` & `markdown_exec-1.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "Topic :: Software Development",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
     "pymdown-extensions>=9",
 ]
-version = "1.5.1"
+version = "1.5.2"
 
 [project.license]
 text = "ISC"
 
 [project.optional-dependencies]
 ansi = [
     "pygments-ansi-color",
```

### Comparing `markdown_exec-1.5.1/src/markdown_exec/__init__.py` & `markdown_exec-1.5.2/src/markdown_exec/__init__.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.1/src/markdown_exec/ansi.css` & `markdown_exec-1.5.2/src/markdown_exec/ansi.css`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.1/src/markdown_exec/formatters/base.py` & `markdown_exec-1.5.2/src/markdown_exec/formatters/base.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.1/src/markdown_exec/formatters/bash.py` & `markdown_exec-1.5.2/src/markdown_exec/formatters/bash.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.1/src/markdown_exec/formatters/console.py` & `markdown_exec-1.5.2/src/markdown_exec/formatters/console.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.1/src/markdown_exec/formatters/pycon.py` & `markdown_exec-1.5.2/src/markdown_exec/formatters/pycon.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.1/src/markdown_exec/formatters/python.py` & `markdown_exec-1.5.2/src/markdown_exec/formatters/python.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.1/src/markdown_exec/formatters/sh.py` & `markdown_exec-1.5.2/src/markdown_exec/formatters/sh.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.1/src/markdown_exec/formatters/tree.py` & `markdown_exec-1.5.2/src/markdown_exec/formatters/tree.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.1/src/markdown_exec/logger.py` & `markdown_exec-1.5.2/src/markdown_exec/logger.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.1/src/markdown_exec/mkdocs_plugin.py` & `markdown_exec-1.5.2/src/markdown_exec/mkdocs_plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from mkdocs.config import Config, config_options
 from mkdocs.plugins import BasePlugin
 from mkdocs.utils import write_file
 
 from markdown_exec import formatter, formatters, validator
 from markdown_exec.logger import patch_loggers
+from markdown_exec.rendering import MarkdownConverter
 
 if TYPE_CHECKING:
     from jinja2 import Environment
     from mkdocs.structure.files import Files
 
 try:
     __import__("pygments_ansi_color")
@@ -66,7 +67,10 @@
 
     def on_env(self, env: Environment, *, config: Config, files: Files) -> Environment | None:  # noqa: ARG002,D102
         css_filename = "assets/_markdown_exec_ansi.css"
         css_content = Path(__file__).parent.joinpath("ansi.css").read_text()
         write_file(css_content.encode("utf-8"), os.path.join(config["site_dir"], css_filename))
         config["extra_css"].insert(0, css_filename)
         return env
+
+    def on_post_build(self, *, config: Config) -> None:  # noqa: ARG002,D102
+        MarkdownConverter.counter = 0
```

### Comparing `markdown_exec-1.5.1/src/markdown_exec/processors.py` & `markdown_exec-1.5.2/src/markdown_exec/processors.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.1/src/markdown_exec/rendering.py` & `markdown_exec-1.5.2/src/markdown_exec/rendering.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.1/tests/conftest.py` & `markdown_exec-1.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.1/tests/test_base_formatter.py` & `markdown_exec-1.5.2/tests/test_base_formatter.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.1/tests/test_converter.py` & `markdown_exec-1.5.2/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.1/tests/test_python.py` & `markdown_exec-1.5.2/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.1/tests/test_shell.py` & `markdown_exec-1.5.2/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.1/tests/test_toc.py` & `markdown_exec-1.5.2/tests/test_toc.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.1/tests/test_validator.py` & `markdown_exec-1.5.2/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.1/PKG-INFO` & `markdown_exec-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-exec
-Version: 1.5.1
+Version: 1.5.2
 Summary: Utilities to execute code blocks in Markdown files.
 Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

