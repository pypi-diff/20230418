# Comparing `tmp/mkdocs-alias-plugin-0.5.0.tar.gz` & `tmp/mkdocs-alias-plugin-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-alias-plugin-0.5.0.tar", last modified: Wed Feb  8 16:59:43 2023, max compression
+gzip compressed data, was "mkdocs-alias-plugin-0.6.0.tar", last modified: Mon Apr 17 22:37:11 2023, max compression
```

## Comparing `mkdocs-alias-plugin-0.5.0.tar` & `mkdocs-alias-plugin-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 16:59:43.460425 mkdocs-alias-plugin-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-02-08 16:59:30.000000 mkdocs-alias-plugin-0.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-02-08 16:59:43.460425 mkdocs-alias-plugin-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-02-08 16:59:30.000000 mkdocs-alias-plugin-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 16:59:43.460425 mkdocs-alias-plugin-0.5.0/alias/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 16:59:30.000000 mkdocs-alias-plugin-0.5.0/alias/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-02-08 16:59:30.000000 mkdocs-alias-plugin-0.5.0/alias/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 16:59:43.460425 mkdocs-alias-plugin-0.5.0/mkdocs_alias_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-02-08 16:59:43.000000 mkdocs-alias-plugin-0.5.0/mkdocs_alias_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-02-08 16:59:43.000000 mkdocs-alias-plugin-0.5.0/mkdocs_alias_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 16:59:43.000000 mkdocs-alias-plugin-0.5.0/mkdocs_alias_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-08 16:59:43.000000 mkdocs-alias-plugin-0.5.0/mkdocs_alias_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-08 16:59:43.000000 mkdocs-alias-plugin-0.5.0/mkdocs_alias_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-08 16:59:43.000000 mkdocs-alias-plugin-0.5.0/mkdocs_alias_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 16:59:43.460425 mkdocs-alias-plugin-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-02-08 16:59:30.000000 mkdocs-alias-plugin-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:37:11.715792 mkdocs-alias-plugin-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-17 22:36:56.000000 mkdocs-alias-plugin-0.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-17 22:37:11.715792 mkdocs-alias-plugin-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-04-17 22:36:56.000000 mkdocs-alias-plugin-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:37:11.715792 mkdocs-alias-plugin-0.6.0/alias/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:36:56.000000 mkdocs-alias-plugin-0.6.0/alias/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-17 22:36:56.000000 mkdocs-alias-plugin-0.6.0/alias/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:37:11.715792 mkdocs-alias-plugin-0.6.0/mkdocs_alias_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-17 22:37:11.000000 mkdocs-alias-plugin-0.6.0/mkdocs_alias_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-17 22:37:11.000000 mkdocs-alias-plugin-0.6.0/mkdocs_alias_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 22:37:11.000000 mkdocs-alias-plugin-0.6.0/mkdocs_alias_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-17 22:37:11.000000 mkdocs-alias-plugin-0.6.0/mkdocs_alias_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 22:37:11.000000 mkdocs-alias-plugin-0.6.0/mkdocs_alias_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 22:37:11.000000 mkdocs-alias-plugin-0.6.0/mkdocs_alias_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 22:37:11.715792 mkdocs-alias-plugin-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-17 22:36:56.000000 mkdocs-alias-plugin-0.6.0/setup.py
```

### Comparing `mkdocs-alias-plugin-0.5.0/LICENSE.md` & `mkdocs-alias-plugin-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-alias-plugin-0.5.0/PKG-INFO` & `mkdocs-alias-plugin-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-alias-plugin
-Version: 0.5.0
+Version: 0.6.0
 Summary: An MkDocs plugin allowing links to your pages using a custom alias
 Home-page: https://github.com/eddyluten/mkdocs-alias-plugin
 Author: Eddy Luten
 Author-email: eddyluten@gmail.com
 License: MIT
 Keywords: mkdocs python markdown alias link wiki
 Classifier: License :: OSI Approved :: MIT License
@@ -76,14 +76,26 @@
 
 If you'd like to supply your own link text instead on a link-by-link basis, you can do so using a pipe to separate the title from the alias:
 
 ```md
 The song references [[wuthering-heights|Wuthering Heights]].
 ```
 
+As of version 0.6.0, you can also use link anchors in your aliases:
+
+```md
+The song references [[wuthering-heights#references]].
+```
+
+Or, also using a title:
+
+```md
+The song references [[wuthering-heights#references|Wuthering Heights]].
+```
+
 Please refer to the [MkDocs documentation](https://www.mkdocs.org/user-guide/writing-your-docs/#yaml-style-meta-data) for more information on how the meta-data block is used.
 
 ### Multiple Aliases
 
 As of version 0.3.0, it is possible to assign multiple aliases to a single page. This does come with the limitation that these aliases cannot define a per-alias title. The syntax for this is:
 
 ```yaml
@@ -163,14 +175,22 @@
 
 ```zsh
 pylint $(git ls-files '*.py') && pytest -vv
 ```
 
 ## Changelog
 
+### 0.6.0
+
+Adds support for page anchor links from within an alias. E.g.:
+
+```md
+[[my alias#my anchor]]
+````
+
 ### 0.5.0
 
 2023-02-08
 
 Adds the ability to use the `use_relative_link` config flag, which causes the plugin to generate relative links to the aliased document rather than absolute ones. This flag is useful for those who host their wikis in subdirectories.
 
 @SimonDelmas contributed this feature in PR #3. Thanks!
```

### Comparing `mkdocs-alias-plugin-0.5.0/README.md` & `mkdocs-alias-plugin-0.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -59,14 +59,26 @@
 
 If you'd like to supply your own link text instead on a link-by-link basis, you can do so using a pipe to separate the title from the alias:
 
 ```md
 The song references [[wuthering-heights|Wuthering Heights]].
 ```
 
+As of version 0.6.0, you can also use link anchors in your aliases:
+
+```md
+The song references [[wuthering-heights#references]].
+```
+
+Or, also using a title:
+
+```md
+The song references [[wuthering-heights#references|Wuthering Heights]].
+```
+
 Please refer to the [MkDocs documentation](https://www.mkdocs.org/user-guide/writing-your-docs/#yaml-style-meta-data) for more information on how the meta-data block is used.
 
 ### Multiple Aliases
 
 As of version 0.3.0, it is possible to assign multiple aliases to a single page. This does come with the limitation that these aliases cannot define a per-alias title. The syntax for this is:
 
 ```yaml
@@ -146,14 +158,22 @@
 
 ```zsh
 pylint $(git ls-files '*.py') && pytest -vv
 ```
 
 ## Changelog
 
+### 0.6.0
+
+Adds support for page anchor links from within an alias. E.g.:
+
+```md
+[[my alias#my anchor]]
+````
+
 ### 0.5.0
 
 2023-02-08
 
 Adds the ability to use the `use_relative_link` config flag, which causes the plugin to generate relative links to the aliased document rather than absolute ones. This flag is useful for those who host their wikis in subdirectories.
 
 @SimonDelmas contributed this feature in PR #3. Thanks!
```

### Comparing `mkdocs-alias-plugin-0.5.0/alias/plugin.py` & `mkdocs-alias-plugin-0.6.0/alias/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,19 @@
     page_file: File,
     use_relative: bool,
 ):
     """Callback used in the sub function within on_page_markdown."""
     if match.group(1) is not None:
         # if the alias match was escaped, return the unescaped version
         return match.group(0)[1:]
-    alias = aliases.get(match.group(2))
+    # split the tag up in case there's an anchor in the link
+    tag_bits = ['']
+    if match.group(2) is not None:
+        tag_bits = str(match.group(2)).split('#')
+    alias = aliases.get(tag_bits[0])
     if alias is None:
         log.warning(
             "Alias '%s' not found in '%s'",
             match.group(2),
             page_file.src_path
         )
         return match.group(0) # return the input string
@@ -60,14 +64,16 @@
     text = alias['text'] if match.group(3) is None else match.group(3)
     if text is None:
         text = alias['url']
 
     url = alias['url']
     if use_relative:
         url = get_relative_url(url, page_file.url)
+    if len(tag_bits) > 1:
+        url = f"{url}#{tag_bits[1]}"
 
     log.info(
         "replaced alias '%s' with '%s' to '%s'",
         alias['alias'],
         text,
         url
     )
```

### Comparing `mkdocs-alias-plugin-0.5.0/mkdocs_alias_plugin.egg-info/PKG-INFO` & `mkdocs-alias-plugin-0.6.0/mkdocs_alias_plugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-alias-plugin
-Version: 0.5.0
+Version: 0.6.0
 Summary: An MkDocs plugin allowing links to your pages using a custom alias
 Home-page: https://github.com/eddyluten/mkdocs-alias-plugin
 Author: Eddy Luten
 Author-email: eddyluten@gmail.com
 License: MIT
 Keywords: mkdocs python markdown alias link wiki
 Classifier: License :: OSI Approved :: MIT License
@@ -76,14 +76,26 @@
 
 If you'd like to supply your own link text instead on a link-by-link basis, you can do so using a pipe to separate the title from the alias:
 
 ```md
 The song references [[wuthering-heights|Wuthering Heights]].
 ```
 
+As of version 0.6.0, you can also use link anchors in your aliases:
+
+```md
+The song references [[wuthering-heights#references]].
+```
+
+Or, also using a title:
+
+```md
+The song references [[wuthering-heights#references|Wuthering Heights]].
+```
+
 Please refer to the [MkDocs documentation](https://www.mkdocs.org/user-guide/writing-your-docs/#yaml-style-meta-data) for more information on how the meta-data block is used.
 
 ### Multiple Aliases
 
 As of version 0.3.0, it is possible to assign multiple aliases to a single page. This does come with the limitation that these aliases cannot define a per-alias title. The syntax for this is:
 
 ```yaml
@@ -163,14 +175,22 @@
 
 ```zsh
 pylint $(git ls-files '*.py') && pytest -vv
 ```
 
 ## Changelog
 
+### 0.6.0
+
+Adds support for page anchor links from within an alias. E.g.:
+
+```md
+[[my alias#my anchor]]
+````
+
 ### 0.5.0
 
 2023-02-08
 
 Adds the ability to use the `use_relative_link` config flag, which causes the plugin to generate relative links to the aliased document rather than absolute ones. This flag is useful for those who host their wikis in subdirectories.
 
 @SimonDelmas contributed this feature in PR #3. Thanks!
```

### Comparing `mkdocs-alias-plugin-0.5.0/setup.py` & `mkdocs-alias-plugin-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='mkdocs-alias-plugin',
-    version='0.5.0',
+    version='0.6.0',
     description=
     'An MkDocs plugin allowing links to your pages using a custom alias',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='mkdocs python markdown alias link wiki',
     url='https://github.com/eddyluten/mkdocs-alias-plugin',
     author='Eddy Luten',
```

