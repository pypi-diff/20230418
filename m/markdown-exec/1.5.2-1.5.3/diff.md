# Comparing `tmp/markdown_exec-1.5.2.tar.gz` & `tmp/markdown_exec-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_exec-1.5.2.tar", last modified: Tue Apr 18 09:59:47 2023, max compression
+gzip compressed data, was "markdown_exec-1.5.3.tar", last modified: Tue Apr 18 12:58:19 2023, max compression
```

## Comparing `markdown_exec-1.5.2.tar` & `markdown_exec-1.5.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      754 2023-04-10 19:47:46.084183 markdown_exec-1.5.2/LICENSE
--rw-r--r--   0        0        0     3354 2023-04-16 18:40:30.714066 markdown_exec-1.5.2/README.md
--rw-r--r--   0        0        0     3595 2023-04-18 09:59:47.521432 markdown_exec-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     4162 2023-04-17 12:40:04.204193 markdown_exec-1.5.2/src/markdown_exec/__init__.py
--rw-r--r--   0        0        0     5657 2023-04-16 18:40:30.810731 markdown_exec-1.5.2/src/markdown_exec/ansi.css
--rw-r--r--   0        0        0       51 2022-11-24 19:29:10.145475 markdown_exec-1.5.2/src/markdown_exec/formatters/__init__.py
--rw-r--r--   0        0        0     4554 2023-04-17 12:40:04.204193 markdown_exec-1.5.2/src/markdown_exec/formatters/base.py
--rw-r--r--   0        0        0      846 2023-04-16 18:40:30.810731 markdown_exec-1.5.2/src/markdown_exec/formatters/bash.py
--rw-r--r--   0        0        0      815 2023-04-16 18:40:30.810731 markdown_exec-1.5.2/src/markdown_exec/formatters/console.py
--rw-r--r--   0        0        0      276 2023-04-16 18:40:30.810731 markdown_exec-1.5.2/src/markdown_exec/formatters/markdown.py
--rw-r--r--   0        0        0      854 2023-04-17 14:01:39.509387 markdown_exec-1.5.2/src/markdown_exec/formatters/pycon.py
--rw-r--r--   0        0        0     2406 2023-04-16 18:40:30.810731 markdown_exec-1.5.2/src/markdown_exec/formatters/python.py
--rw-r--r--   0        0        0      836 2023-04-16 18:40:30.810731 markdown_exec-1.5.2/src/markdown_exec/formatters/sh.py
--rw-r--r--   0        0        0     2046 2023-04-16 18:40:30.810731 markdown_exec-1.5.2/src/markdown_exec/formatters/tree.py
--rw-r--r--   0        0        0     2089 2023-04-16 18:40:30.834064 markdown_exec-1.5.2/src/markdown_exec/logger.py
--rw-r--r--   0        0        0     2620 2023-04-18 09:56:51.630595 markdown_exec-1.5.2/src/markdown_exec/mkdocs_plugin.py
--rw-r--r--   0        0        0     4261 2023-04-17 13:48:51.537991 markdown_exec-1.5.2/src/markdown_exec/processors.py
--rw-r--r--   0        0        0        0 2023-04-10 19:47:45.977517 markdown_exec-1.5.2/src/markdown_exec/py.typed
--rw-r--r--   0        0        0     6144 2023-04-18 09:45:50.883905 markdown_exec-1.5.2/src/markdown_exec/rendering.py
--rw-r--r--   0        0        0      166 2023-04-10 19:47:45.974184 markdown_exec-1.5.2/tests/__init__.py
--rw-r--r--   0        0        0      635 2023-04-16 18:40:30.837398 markdown_exec-1.5.2/tests/conftest.py
--rw-r--r--   0        0        0     1443 2023-04-16 18:40:30.854064 markdown_exec-1.5.2/tests/test_base_formatter.py
--rw-r--r--   0        0        0      630 2023-04-17 13:49:16.754400 markdown_exec-1.5.2/tests/test_converter.py
--rw-r--r--   0        0        0     4337 2023-04-17 14:00:35.590141 markdown_exec-1.5.2/tests/test_python.py
--rw-r--r--   0        0        0     2027 2023-04-16 18:40:30.854064 markdown_exec-1.5.2/tests/test_shell.py
--rw-r--r--   0        0        0     2335 2023-04-17 12:40:04.207527 markdown_exec-1.5.2/tests/test_toc.py
--rw-r--r--   0        0        0      488 2023-04-16 18:40:30.854064 markdown_exec-1.5.2/tests/test_tree.py
--rw-r--r--   0        0        0      995 2022-02-06 15:25:17.240565 markdown_exec-1.5.2/tests/test_validator.py
--rw-r--r--   0        0        0     4874 1970-01-01 00:00:00.000000 markdown_exec-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-04-10 19:47:46.084183 markdown_exec-1.5.3/LICENSE
+-rw-r--r--   0        0        0     3354 2023-04-16 18:40:30.714066 markdown_exec-1.5.3/README.md
+-rw-r--r--   0        0        0     3595 2023-04-18 12:58:19.114518 markdown_exec-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     4162 2023-04-17 12:40:04.204193 markdown_exec-1.5.3/src/markdown_exec/__init__.py
+-rw-r--r--   0        0        0     5657 2023-04-16 18:40:30.810731 markdown_exec-1.5.3/src/markdown_exec/ansi.css
+-rw-r--r--   0        0        0       51 2022-11-24 19:29:10.145475 markdown_exec-1.5.3/src/markdown_exec/formatters/__init__.py
+-rw-r--r--   0        0        0     4554 2023-04-17 12:40:04.204193 markdown_exec-1.5.3/src/markdown_exec/formatters/base.py
+-rw-r--r--   0        0        0      846 2023-04-16 18:40:30.810731 markdown_exec-1.5.3/src/markdown_exec/formatters/bash.py
+-rw-r--r--   0        0        0      815 2023-04-16 18:40:30.810731 markdown_exec-1.5.3/src/markdown_exec/formatters/console.py
+-rw-r--r--   0        0        0      276 2023-04-16 18:40:30.810731 markdown_exec-1.5.3/src/markdown_exec/formatters/markdown.py
+-rw-r--r--   0        0        0      854 2023-04-17 14:01:39.509387 markdown_exec-1.5.3/src/markdown_exec/formatters/pycon.py
+-rw-r--r--   0        0        0     2406 2023-04-16 18:40:30.810731 markdown_exec-1.5.3/src/markdown_exec/formatters/python.py
+-rw-r--r--   0        0        0      836 2023-04-16 18:40:30.810731 markdown_exec-1.5.3/src/markdown_exec/formatters/sh.py
+-rw-r--r--   0        0        0     2046 2023-04-16 18:40:30.810731 markdown_exec-1.5.3/src/markdown_exec/formatters/tree.py
+-rw-r--r--   0        0        0     2089 2023-04-16 18:40:30.834064 markdown_exec-1.5.3/src/markdown_exec/logger.py
+-rw-r--r--   0        0        0     3278 2023-04-18 12:38:06.420523 markdown_exec-1.5.3/src/markdown_exec/mkdocs_plugin.py
+-rw-r--r--   0        0        0     4261 2023-04-17 13:48:51.537991 markdown_exec-1.5.3/src/markdown_exec/processors.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:47:45.977517 markdown_exec-1.5.3/src/markdown_exec/py.typed
+-rw-r--r--   0        0        0     8519 2023-04-18 12:56:30.339394 markdown_exec-1.5.3/src/markdown_exec/rendering.py
+-rw-r--r--   0        0        0      166 2023-04-10 19:47:45.974184 markdown_exec-1.5.3/tests/__init__.py
+-rw-r--r--   0        0        0      635 2023-04-16 18:40:30.837398 markdown_exec-1.5.3/tests/conftest.py
+-rw-r--r--   0        0        0     1443 2023-04-16 18:40:30.854064 markdown_exec-1.5.3/tests/test_base_formatter.py
+-rw-r--r--   0        0        0      932 2023-04-18 12:39:58.642494 markdown_exec-1.5.3/tests/test_converter.py
+-rw-r--r--   0        0        0     4337 2023-04-17 14:00:35.590141 markdown_exec-1.5.3/tests/test_python.py
+-rw-r--r--   0        0        0     2027 2023-04-16 18:40:30.854064 markdown_exec-1.5.3/tests/test_shell.py
+-rw-r--r--   0        0        0     2335 2023-04-17 12:40:04.207527 markdown_exec-1.5.3/tests/test_toc.py
+-rw-r--r--   0        0        0      488 2023-04-16 18:40:30.854064 markdown_exec-1.5.3/tests/test_tree.py
+-rw-r--r--   0        0        0      995 2022-02-06 15:25:17.240565 markdown_exec-1.5.3/tests/test_validator.py
+-rw-r--r--   0        0        0     4874 1970-01-01 00:00:00.000000 markdown_exec-1.5.3/PKG-INFO
```

### Comparing `markdown_exec-1.5.2/LICENSE` & `markdown_exec-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.2/README.md` & `markdown_exec-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.2/pyproject.toml` & `markdown_exec-1.5.3/pyproject.toml`

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
-version = "1.5.2"
+version = "1.5.3"
 
 [project.license]
 text = "ISC"
 
 [project.optional-dependencies]
 ansi = [
     "pygments-ansi-color",
```

### Comparing `markdown_exec-1.5.2/src/markdown_exec/__init__.py` & `markdown_exec-1.5.3/src/markdown_exec/__init__.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.2/src/markdown_exec/ansi.css` & `markdown_exec-1.5.3/src/markdown_exec/ansi.css`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.2/src/markdown_exec/formatters/base.py` & `markdown_exec-1.5.3/src/markdown_exec/formatters/base.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.2/src/markdown_exec/formatters/bash.py` & `markdown_exec-1.5.3/src/markdown_exec/formatters/bash.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.2/src/markdown_exec/formatters/console.py` & `markdown_exec-1.5.3/src/markdown_exec/formatters/console.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.2/src/markdown_exec/formatters/pycon.py` & `markdown_exec-1.5.3/src/markdown_exec/formatters/pycon.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.2/src/markdown_exec/formatters/python.py` & `markdown_exec-1.5.3/src/markdown_exec/formatters/python.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.2/src/markdown_exec/formatters/sh.py` & `markdown_exec-1.5.3/src/markdown_exec/formatters/sh.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.2/src/markdown_exec/formatters/tree.py` & `markdown_exec-1.5.3/src/markdown_exec/formatters/tree.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.2/src/markdown_exec/logger.py` & `markdown_exec-1.5.3/src/markdown_exec/logger.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.2/src/markdown_exec/mkdocs_plugin.py` & `markdown_exec-1.5.3/src/markdown_exec/mkdocs_plugin.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from mkdocs.config import Config, config_options
 from mkdocs.plugins import BasePlugin
 from mkdocs.utils import write_file
 
 from markdown_exec import formatter, formatters, validator
 from markdown_exec.logger import patch_loggers
-from markdown_exec.rendering import MarkdownConverter
+from markdown_exec.rendering import MarkdownConverter, markdown_config
 
 if TYPE_CHECKING:
     from jinja2 import Environment
     from mkdocs.structure.files import Files
 
 try:
     __import__("pygments_ansi_color")
@@ -45,32 +45,49 @@
 
 
 class MarkdownExecPlugin(BasePlugin):
     """MkDocs plugin to easily enable custom fences for code blocks execution."""
 
     config_scheme = (("languages", config_options.Type(list, default=list(formatters.keys()))),)
 
-    def on_config(self, config: Config, **kwargs: Any) -> Config:  # noqa: ARG002,D102
+    def on_config(self, config: Config, **kwargs: Any) -> Config:  # noqa: ARG002
+        """Configure the plugin.
+
+        Hook for the [`on_config` event](https://www.mkdocs.org/user-guide/plugins/#on_config).
+        In this hook, we add custom fences for all the supported languages.
+
+        We also save the Markdown extensions configuration
+        into [`markdown_config`][markdown_exec.rendering.markdown_config].
+
+        Arguments:
+            config: The MkDocs config object.
+            **kwargs: Additional arguments passed by MkDocs.
+
+        Returns:
+            The modified config.
+        """
         self.languages = self.config["languages"]
         mdx_configs = config.setdefault("mdx_configs", {})
         superfences = mdx_configs.setdefault("pymdownx.superfences", {})
         custom_fences = superfences.setdefault("custom_fences", [])
         for language in self.languages:
             custom_fences.append(
                 {
                     "name": language,
                     "class": language,
                     "validator": validator,
                     "format": formatter,
                 },
             )
+        markdown_config.save(config["markdown_extensions"], config["mdx_configs"])
         return config
 
     def on_env(self, env: Environment, *, config: Config, files: Files) -> Environment | None:  # noqa: ARG002,D102
         css_filename = "assets/_markdown_exec_ansi.css"
         css_content = Path(__file__).parent.joinpath("ansi.css").read_text()
         write_file(css_content.encode("utf-8"), os.path.join(config["site_dir"], css_filename))
         config["extra_css"].insert(0, css_filename)
         return env
 
     def on_post_build(self, *, config: Config) -> None:  # noqa: ARG002,D102
         MarkdownConverter.counter = 0
+        markdown_config.reset()
```

### Comparing `markdown_exec-1.5.2/src/markdown_exec/processors.py` & `markdown_exec-1.5.3/src/markdown_exec/processors.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.2/src/markdown_exec/rendering.py` & `markdown_exec-1.5.3/src/markdown_exec/rendering.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Markdown extensions and helpers."""
 
 from __future__ import annotations
 
 from functools import lru_cache
-from itertools import chain
 from textwrap import indent
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 from markdown import Markdown
 from markupsafe import Markup
 
 from markdown_exec.processors import (
     HeadingReportingTreeprocessor,
     IdPrependingTreeprocessor,
@@ -104,14 +103,75 @@
         return tabbed((source_tab_title, source_block), (result_tab_title, output))
     if location == "tabbed-right":
         return tabbed((result_tab_title, output), (source_tab_title, source_block))
 
     raise ValueError(f"unsupported location for sources: {location}")
 
 
+class MarkdownConfig:
+    """This class returns a singleton used to store Markdown extensions configuration.
+
+    You don't have to instantiate the singleton yourself:
+    we provide it as [`markdown_config`][markdown_exec.rendering.markdown_config].
+    """
+
+    _singleton: MarkdownConfig | None = None
+
+    def __new__(cls) -> MarkdownConfig:  # noqa: D102
+        if cls._singleton is None:
+            cls._singleton = super().__new__(cls)
+        return cls._singleton
+
+    def __init__(self) -> None:  # noqa: D107
+        self.exts: list[str | Extension] | None = None
+        self.exts_config: dict[str, dict[str, Any]] | None = None
+
+    def save(self, exts: list[str | Extension], exts_config: dict[str, dict[str, Any]]) -> None:
+        """Save Markdown extensions and their configuration.
+
+        Parameters:
+            exts: The Markdown extensions.
+            exts_config: The extensions configuration.
+        """
+        self.exts = exts
+        self.exts_config = exts_config
+
+    def reset(self) -> None:
+        """Reset Markdown extensions and their configuration."""
+        self.exts = None
+        self.exts_config = None
+
+
+markdown_config = MarkdownConfig()
+"""This object can be used to save the configuration of your Markdown extensions.
+
+For example, since we provide a MkDocs plugin, we use it to store the configuration
+that was read from `mkdocs.yml`:
+
+```python
+from markdown_exec.rendering import markdown_config
+
+# ...in relevant events/hooks, access and modify extensions and their configs, then:
+markdown_config.save(extensions, extensions_config)
+```
+
+See the actual event hook: [`on_config`][markdown_exec.mkdocs_plugin.MarkdownExecPlugin.on_config].
+See the [`save`][markdown_exec.rendering.MarkdownConfig.save]
+and [`reset`][markdown_exec.rendering.MarkdownConfig.reset] methods.
+
+Without it, Markdown Exec will rely on the `registeredExtensions` attribute
+of the original Markdown instance, which does not forward everything
+that was configured, notably extensions like `tables`. Other extensions
+such as `attr_list` are visible, but fail to register properly when
+reusing their instances. It means that the rendered HTML might differ
+from what you expect (tables not rendered, attribute lists not injected,
+emojis not working, etc.).
+"""
+
+
 @lru_cache(maxsize=None)
 def _register_headings_processors(md: Markdown) -> None:
     md.treeprocessors.register(
         InsertHeadings(md),
         InsertHeadings.name,
         priority=75,  # right before markdown.blockprocessors.HashHeaderProcessor
     )
@@ -120,16 +180,17 @@
         RemoveHeadings.name,
         priority=4,  # right after toc
     )
 
 
 def _mimic(md: Markdown, headings: list[Element], *, update_toc: bool = True) -> Markdown:
     new_md = Markdown()
-    extensions: list[Extension | str] = list(chain(md.registeredExtensions, ["tables", "md_in_html"]))
-    new_md.registerExtensions(extensions, {})
+    extensions: list[Extension | str] = markdown_config.exts or md.registeredExtensions  # type: ignore[assignment]
+    extensions_config: dict[str, dict[str, Any]] = markdown_config.exts_config or {}
+    new_md.registerExtensions(extensions, extensions_config)
     new_md.treeprocessors.register(
         IdPrependingTreeprocessor(md, ""),
         IdPrependingTreeprocessor.name,
         priority=4,  # right after 'toc' (needed because that extension adds ids to headings)
     )
     new_md._original_md = md  # type: ignore[attr-defined]
```

### Comparing `markdown_exec-1.5.2/tests/conftest.py` & `markdown_exec-1.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.2/tests/test_base_formatter.py` & `markdown_exec-1.5.3/tests/test_base_formatter.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.2/tests/test_converter.py` & `markdown_exec-1.5.3/tests/test_converter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Tests for the Markdown converter."""
 
 from __future__ import annotations
 
 from textwrap import dedent
 from typing import TYPE_CHECKING
 
+from markdown_exec.rendering import MarkdownConfig, markdown_config
+
 if TYPE_CHECKING:
     from markdown import Markdown
 
 
 def test_rendering_nested_blocks(md: Markdown) -> None:
     """Assert nested blocks are properly handled.
 
@@ -23,7 +25,14 @@
             print("**Bold!**")
             ```
             ````
             """,
         ),
     )
     assert html == "<p><strong>Bold!</strong></p>"
+
+
+def test_instantiating_config_singleton() -> None:
+    """Assert that the Markdown config instances act as a singleton."""
+    assert MarkdownConfig() is markdown_config
+    markdown_config.save([], {})
+    markdown_config.reset()
```

### Comparing `markdown_exec-1.5.2/tests/test_python.py` & `markdown_exec-1.5.3/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.2/tests/test_shell.py` & `markdown_exec-1.5.3/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.2/tests/test_toc.py` & `markdown_exec-1.5.3/tests/test_toc.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.2/tests/test_validator.py` & `markdown_exec-1.5.3/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.5.2/PKG-INFO` & `markdown_exec-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-exec
-Version: 1.5.2
+Version: 1.5.3
 Summary: Utilities to execute code blocks in Markdown files.
 Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

