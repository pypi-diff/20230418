# Comparing `tmp/divio_docs_gen-0.0.3.tar.gz` & `tmp/divio_docs_gen-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "divio_docs_gen-0.0.3.tar", last modified: Mon Apr 17 11:19:25 2023, max compression
+gzip compressed data, was "divio_docs_gen-0.0.4.tar", last modified: Tue Apr 18 11:34:43 2023, max compression
```

## Comparing `divio_docs_gen-0.0.3.tar` & `divio_docs_gen-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:19:25.563815 divio_docs_gen-0.0.3/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-04-17 11:19:15.000000 divio_docs_gen-0.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5597 2023-04-17 11:19:25.563815 divio_docs_gen-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4803 2023-04-17 11:19:15.000000 divio_docs_gen-0.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)      916 2023-04-17 11:19:15.000000 divio_docs_gen-0.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 11:19:25.563815 divio_docs_gen-0.0.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:19:25.559816 divio_docs_gen-0.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:19:25.563815 divio_docs_gen-0.0.3/src/divio_docs_gen/
--rw-r--r--   0 root         (0) root         (0)      135 2023-04-17 11:19:15.000000 divio_docs_gen-0.0.3/src/divio_docs_gen/__init__.py
--rw-r--r--   0 root         (0) root         (0)      131 2023-04-17 11:19:15.000000 divio_docs_gen-0.0.3/src/divio_docs_gen/__main__.py
--rw-r--r--   0 root         (0) root         (0)     4004 2023-04-17 11:19:15.000000 divio_docs_gen-0.0.3/src/divio_docs_gen/args.py
--rw-r--r--   0 root         (0) root         (0)      548 2023-04-17 11:19:15.000000 divio_docs_gen-0.0.3/src/divio_docs_gen/colourstring.py
--rw-r--r--   0 root         (0) root         (0)     4929 2023-04-17 11:19:15.000000 divio_docs_gen-0.0.3/src/divio_docs_gen/docsgen.py
--rw-r--r--   0 root         (0) root         (0)     7258 2023-04-17 11:19:15.000000 divio_docs_gen-0.0.3/src/divio_docs_gen/index.py
--rw-r--r--   0 root         (0) root         (0)     5531 2023-04-17 11:19:15.000000 divio_docs_gen-0.0.3/src/divio_docs_gen/repo.py
--rw-r--r--   0 root         (0) root         (0)     5411 2023-04-17 11:19:15.000000 divio_docs_gen-0.0.3/src/divio_docs_gen/sections.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-04-17 11:19:15.000000 divio_docs_gen-0.0.3/src/divio_docs_gen/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:19:25.563815 divio_docs_gen-0.0.3/src/divio_docs_gen.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5597 2023-04-17 11:19:25.000000 divio_docs_gen-0.0.3/src/divio_docs_gen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      513 2023-04-17 11:19:25.000000 divio_docs_gen-0.0.3/src/divio_docs_gen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 11:19:25.000000 divio_docs_gen-0.0.3/src/divio_docs_gen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-04-17 11:19:25.000000 divio_docs_gen-0.0.3/src/divio_docs_gen.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-17 11:19:25.000000 divio_docs_gen-0.0.3/src/divio_docs_gen.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 11:34:43.593698 divio_docs_gen-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5748 2023-04-18 11:34:43.593698 divio_docs_gen-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4954 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/README.md
+-rw-r--r--   0 root         (0) root         (0)      916 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 11:34:43.593698 divio_docs_gen-0.0.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 11:34:43.593698 divio_docs_gen-0.0.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 11:34:43.593698 divio_docs_gen-0.0.4/src/divio_docs_gen/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/src/divio_docs_gen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      131 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/src/divio_docs_gen/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     6275 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/src/divio_docs_gen/args.py
+-rw-r--r--   0 root         (0) root         (0)      548 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/src/divio_docs_gen/colourstring.py
+-rw-r--r--   0 root         (0) root         (0)     5316 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/src/divio_docs_gen/docsgen.py
+-rw-r--r--   0 root         (0) root         (0)     7748 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/src/divio_docs_gen/index.py
+-rw-r--r--   0 root         (0) root         (0)     5531 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/src/divio_docs_gen/repo.py
+-rw-r--r--   0 root         (0) root         (0)     5411 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/src/divio_docs_gen/sections.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/src/divio_docs_gen/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 11:34:43.593698 divio_docs_gen-0.0.4/src/divio_docs_gen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5748 2023-04-18 11:34:43.000000 divio_docs_gen-0.0.4/src/divio_docs_gen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      513 2023-04-18 11:34:43.000000 divio_docs_gen-0.0.4/src/divio_docs_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 11:34:43.000000 divio_docs_gen-0.0.4/src/divio_docs_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-04-18 11:34:43.000000 divio_docs_gen-0.0.4/src/divio_docs_gen.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-18 11:34:43.000000 divio_docs_gen-0.0.4/src/divio_docs_gen.egg-info/top_level.txt
```

### Comparing `divio_docs_gen-0.0.3/LICENSE` & `divio_docs_gen-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.0.3/PKG-INFO` & `divio_docs_gen-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: divio_docs_gen
-Version: 0.0.3
-Summary: Turn all the markdown files in your repos into one big, divio structrured documentation
-Author-email: Denperidge <denperidge@gmail.com>
-Project-URL: Homepage, https://github.com/Denperidge-Redpencil/divio-docs-gen
-Project-URL: Bug Tracker, https://github.com/Denperidge-Redpencil/divio-docs-gen/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Documentation
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Divio Docs Generator
 
 Automatically collect, aggregate and structure all your [divio-style documentation](https://documentation.divio.com/) into a tree of .md files.
 ```
 /{reponame}
     /tutorials
     /how-tos
@@ -31,30 +13,43 @@
     - If you have a how-to section in your README, that'll get extracted and put in the right spot
     - Or, if you have an how-to.md file, it'll get added in its entirety!
 - Any output structure: this script generates a simple markdown tree. Nothing proprietary, no vendor-lockin. It can be generated from GitHub Actions and put into a Jekyll pages site just as easily as it is run from a Raspberry Pi and used to render the contents of an Ember application.
 
 All you have to do is simply name your headers and/or files after the divio sections (`tutorial`, `how-to`, `explanation`, `reference`). (Oh, don't worry, the search is done through a case insensitive regex. Add more words as you please) 
 
 ## Getting-Started / tutorial
-*(You can also use the [repository template](https://github.com/Denperidge-Redpencil/Divio-Docs-Repo/)!)*
-
-- Clone the repository using `git clone https://github.com/Denperidge-Redpencil/divio-docs-gen.git && cd divio-docs-gen`
-- Install the pre-requirements using `python3 -m pip install -r requirements.txt`
-- Setup the docs.conf file (See the [reference below](#docsconf) and/or the [docs.conf.example](docs.conf.example) file)
-- And finally, run using `python3 app/index.py`!
+- Install the package (`python3 -m pip install divio_docs_gen`)
+- And then either...
+    - Setup the docs.conf file (See the [reference below](#docsconf) and/or the [docs.conf.example](docs.conf.example) file)
+    - Use throught the cli (`python3 -m divio_docs_gen --help`)
 
 ## How-To
+### Install from pip
+```bash
+python3 -m pip install divio_docs_gen
+```
+
+### Clone & run scripts locally
+```bash
+git clone https://github.com/Denperidge-Redpencil/divio-docs-gen.git
+cd divio-docs-gen
+python3 -m pip install -r requirements.txt
+python3 src.divio_docs_gen
+```
+
 ### Build & install package locally
 ```bash
-python3.10 -m pip install --upgrade build setuptools
-python3.10 -m build
-python3.10 -m pip install --force-reinstall ./dist/*.whl
+git clone https://github.com/Denperidge-Redpencil/divio-docs-gen.git
+cd divio-docs-gen/
+python3 -m pip install --upgrade build setuptools
+python3 -m build && python3 -m pip install --force-reinstall ./dist/*.whl
 ```
 *Note: other Python versions can be used!*
 
+
 ## Discussions
 The Divio structure is built upon splitting your documentation into 4 types of documentations. ![The overview of the divio documentation on their website](https://documentation.divio.com/_images/overview.png). In this repository they're referred to as sections.
 
 
 If you want to know more about the design principles of this project, feel free to check out my writeup [here](https://github.com/Denperidge-Redpencil/Learning.md/blob/main/Notes/docs.md#design-principles)!
```

### Comparing `divio_docs_gen-0.0.3/README.md` & `divio_docs_gen-0.0.4/src/divio_docs_gen.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: divio-docs-gen
+Version: 0.0.4
+Summary: Turn all the markdown files in your repos into one big, divio structrured documentation
+Author-email: Denperidge <denperidge@gmail.com>
+Project-URL: Homepage, https://github.com/Denperidge-Redpencil/divio-docs-gen
+Project-URL: Bug Tracker, https://github.com/Denperidge-Redpencil/divio-docs-gen/issues
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Documentation
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Divio Docs Generator
 
 Automatically collect, aggregate and structure all your [divio-style documentation](https://documentation.divio.com/) into a tree of .md files.
 ```
 /{reponame}
     /tutorials
     /how-tos
@@ -13,30 +31,43 @@
     - If you have a how-to section in your README, that'll get extracted and put in the right spot
     - Or, if you have an how-to.md file, it'll get added in its entirety!
 - Any output structure: this script generates a simple markdown tree. Nothing proprietary, no vendor-lockin. It can be generated from GitHub Actions and put into a Jekyll pages site just as easily as it is run from a Raspberry Pi and used to render the contents of an Ember application.
 
 All you have to do is simply name your headers and/or files after the divio sections (`tutorial`, `how-to`, `explanation`, `reference`). (Oh, don't worry, the search is done through a case insensitive regex. Add more words as you please) 
 
 ## Getting-Started / tutorial
-*(You can also use the [repository template](https://github.com/Denperidge-Redpencil/Divio-Docs-Repo/)!)*
-
-- Clone the repository using `git clone https://github.com/Denperidge-Redpencil/divio-docs-gen.git && cd divio-docs-gen`
-- Install the pre-requirements using `python3 -m pip install -r requirements.txt`
-- Setup the docs.conf file (See the [reference below](#docsconf) and/or the [docs.conf.example](docs.conf.example) file)
-- And finally, run using `python3 app/index.py`!
+- Install the package (`python3 -m pip install divio_docs_gen`)
+- And then either...
+    - Setup the docs.conf file (See the [reference below](#docsconf) and/or the [docs.conf.example](docs.conf.example) file)
+    - Use throught the cli (`python3 -m divio_docs_gen --help`)
 
 ## How-To
+### Install from pip
+```bash
+python3 -m pip install divio_docs_gen
+```
+
+### Clone & run scripts locally
+```bash
+git clone https://github.com/Denperidge-Redpencil/divio-docs-gen.git
+cd divio-docs-gen
+python3 -m pip install -r requirements.txt
+python3 src.divio_docs_gen
+```
+
 ### Build & install package locally
 ```bash
-python3.10 -m pip install --upgrade build setuptools
-python3.10 -m build
-python3.10 -m pip install --force-reinstall ./dist/*.whl
+git clone https://github.com/Denperidge-Redpencil/divio-docs-gen.git
+cd divio-docs-gen/
+python3 -m pip install --upgrade build setuptools
+python3 -m build && python3 -m pip install --force-reinstall ./dist/*.whl
 ```
 *Note: other Python versions can be used!*
 
+
 ## Discussions
 The Divio structure is built upon splitting your documentation into 4 types of documentations. ![The overview of the divio documentation on their website](https://documentation.divio.com/_images/overview.png). In this repository they're referred to as sections.
 
 
 If you want to know more about the design principles of this project, feel free to check out my writeup [here](https://github.com/Denperidge-Redpencil/Learning.md/blob/main/Notes/docs.md#design-principles)!
```

### Comparing `divio_docs_gen-0.0.3/pyproject.toml` & `divio_docs_gen-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "divio_docs_gen"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="Denperidge", email="denperidge@gmail.com" },
 ]
 description = "Turn all the markdown files in your repos into one big, divio structrured documentation"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `divio_docs_gen-0.0.3/src/divio_docs_gen/args.py` & `divio_docs_gen-0.0.4/src/divio_docs_gen/args.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,34 +4,60 @@
 from argparse import ArgumentParser
 
 """Code to handle configuration, through docs.conf or args"""
 
 """ Command-line args """
 parser = ArgumentParser()
 
-ouptut_config = parser.add_argument_group("Output configuration")
-ouptut_config.add_argument("--save-conf", 
+conf_sections = {
+    "output": "Output Configuration", 
+    "naming": "Naming Scheme", 
+    "repos": "Repository Selection"
+    }
+ouptut_config = parser.add_argument_group(conf_sections["output"])
+ouptut_config.add_argument("--save-conf",
+                    dest="SaveConf",
                     help="When used, save the current command line options into ./docs.conf", 
-                    action="store_true")
-ouptut_config.add_argument("--generate-nav", "--nav", 
+                    action="store_true",
+                    default=None,  # store_true default is False
+                    )
+ouptut_config.add_argument("--generate-nav", "--nav",
+                    dest="GenerateNav",
                     help="When used, add internal navigation to the top of each generated file", 
-                    action="store_true")
-ouptut_config.add_argument("--docs-base-dir", "--docs-dir", "--dir", "-d", 
+                    action="store_true",
+                    default=None,
+                    )
+ouptut_config.add_argument("--docs-base-dir", "--docs-dir", "--dir", "-d",
+                    dest="DocsBasedir",
                     help="What folder to output the docs in. Defaults to `docs/", 
-                    default="docs/")
+                    )
+ouptut_config.add_argument("--write-to-disk", "--write",
+                           dest="WriteToDisk",
+                           help="Whether to write the markdown to disk",
+                           action="store_true",
+                           default=None,
+                           )
+ouptut_config.add_argument("--dont-remove-tmp", "--tmp",
+                           dest="DontRemoveTmp",
+                           help="When used, the tmp/ folder does not get deleted",
+                           action="store_true",
+                           default=None,
+                           )
+
+naming_scheme = parser.add_argument_group(conf_sections["naming"])
+for section_key in ["tutorials", "how-tos", "explanations", "references"]:
+    short_hand = section_key[0] if section_key[0] != "h" else "ht"
+    naming_scheme.add_argument(f"--{section_key}", f"-{short_hand}", 
+                        dest=section_key,
+                        help=f"Sets the output folder name for {section_key}. Defaults to `{section_key}`"
+                        )
 
-naming_scheme = parser.add_argument_group("Naming scheme")
-for section in ["tutorials", "how-tos", "explanations", "references"]:
-    short_hand = section[0] if section[0] != "h" else "ht"
-    naming_scheme.add_argument(f"--{section}", f"-{short_hand}", 
-                        help=f"Sets the output folder name for {section}. Defaults to `{section}`", 
-                        default=section)
-
-repo_selection = parser.add_argument_group("Repository selection")
+repo_selection = parser.add_argument_group(conf_sections["repos"])
 repo_selection.add_argument("--defaultowner", "--owner", "-do", "-o", 
+                    dest="DefaultOwner",
                     help="Defines which user or org has to be checked for the repository in case its Path does not explicitly define an owner")
 
 repo_selection.add_argument("--repo",
                             help="""
                             Configures if/how a repo should be parsed
 
                             Syntax: OWNER/REPO_NAME [options]
@@ -44,49 +70,85 @@
                             """,
                             action="append",
                             dest="repos",
                             nargs="*")
 
 args = parser.parse_args()
 
+
+args_save_conf = bool(getattr(args, "SaveConf")) if hasattr(args, "SaveConf") else False
+
 """ Conf file """
 conf_file = path.join(getcwd(), "docs.conf")
 use_conf = path.exists(conf_file)
-if use_conf:
+if use_conf or args_save_conf:
     conf = ConfigParser()
-    conf.read("docs.conf")
+    if use_conf:
+        conf.read("docs.conf")
+    
+    for section_key in conf_sections:
+        section = conf_sections[section_key]
+        if section not in conf:
+            conf.add_section(section)
+
 
+""" Apply & save """
 def get_conf_value(section_id, value_id):
     return conf[section_id][value_id] if value_id in conf[section_id] else ""
 
 def get_arg_value(value_id):
-    return getattr(args, value_id) if hasattr(args, value_id) else ""
+    print(args)
+    return getattr(args, value_id) if hasattr(args, value_id) else None
 
 def get_value(section_id, value_id, default):
     """Gets the arg, whether it be from the config file or CLI"""
-    value = get_conf_value(section_id, value_id) if use_conf else get_arg_value(value_id.lower())
-    return value if value != "" else default
-
-args_default_owner = get_value("DEFAULT", "DefaultOwner", None)  # Used as default repo owner
-args_generate_nav = bool(get_value("DEFAULT", "GenerateNav", False))
-args_docs_basedir = get_value("DEFAULT", "DocsBasedir", "docs/")
+    # Get the value from cli if defined. Cli > conf
+    value = get_arg_value(value_id)
+    # If it's undefined in the CLI, check if conf can be used
+    if value is None and use_conf:
+        value = get_conf_value(section_id, value_id)
+    elif value is None:
+        value = default
+
+    if args_save_conf:
+        # If it should be saved, do that
+        conf[section_id][value_id] = str(value)
+        
+    return value
+
+args_default_owner = get_value(conf_sections["repos"], "DefaultOwner", None)  # Used as default repo owner
+args_write_to_disk = bool(get_value(conf_sections["output"], "WriteToDisk", False))
+args_generate_nav = bool(get_value(conf_sections["output"], "GenerateNav", False))
+args_docs_basedir = get_value(conf_sections["output"], "DocsBasedir", "docs/")
+args_dont_remove_tmp = bool(get_value(conf_sections["output"], "DontRemoveTmp", False))
 
 args_section_names = dict()
 for section_name in ["tutorials", "how-tos", "explanations", "references"]:
-    args_section_names[section_name] = get_value("DEFAULT", value_id=section_name, default=section_name).lower()
-
+    args_section_names[section_name] = get_value(conf_sections["naming"], value_id=section_name, default=section_name).lower()
+print(args_section_names)
 
 args_repoconfigs = []
-if use_conf:
-    conf_sections = conf.sections()
-    for conf_section_id in conf_sections:
-        conf_section = conf[conf_section_id]
-        args_repoconfigs.append(dict(conf_section))
-else:
+if get_arg_value("repos"):
     for repo_arg in get_arg_value("repos"):
         repo = dict()
         repo["path"] = repo_arg[0]
         for arg in repo_arg[1:]:
             key, value = arg.split("=", 1)
             repo[key] = value
         args_repoconfigs.append(repo)
+        conf[repo["path"]] = repo
+    
+if use_conf:
+    all_conf_sections = conf.sections()
+    for conf_section_id in all_conf_sections:
+        if conf_section_id in conf_sections.values(): continue
+        
 
+        conf_section = conf[conf_section_id]
+        repo = dict(conf_section)
+        if repo not in args_repoconfigs:
+            args_repoconfigs.append(repo)
+        
+
+if args_save_conf:
+    with open("docs.conf", mode="w", encoding="UTF-8") as configfile:
+        conf.write(configfile)
```

### Comparing `divio_docs_gen-0.0.3/src/divio_docs_gen/colourstring.py` & `divio_docs_gen-0.0.4/src/divio_docs_gen/colourstring.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.0.3/src/divio_docs_gen/docsgen.py` & `divio_docs_gen-0.0.4/src/divio_docs_gen/docsgen.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,15 +63,26 @@
 def make_and_get_sectiondir(reponame, section: Union[str,Section]):
     """Create a directory for the section in the repository's folder"""
     if isinstance(section, Section):
         section = section.name
     
     return join_and_make(make_and_get_repodir(reponame), section)
 
-def add_to_docs(reponame: str, section: Union[str,Section], content: str, filename="README.md", replaceContent=False, prepend=False) -> str:
+def add_to_data_output(data_output: dict, reponame: str, section_name: str, content: str):
+    if reponame not in data_output:
+        data_output[reponame] = dict()
+
+    if section_name not in data_output[reponame]:
+        data_output[reponame][section_name] = content
+    else:
+        data_output[reponame][section_name] += content
+    
+    return data_output
+
+def write_to_docs(reponame: str, section: Union[str,Section], content: str, filename="README.md", replaceContent=False, prepend=False) -> str:
     """Add CONTENT to the generated documentation. Optionally creates the needed directories, replaces contents..."""
     dir = make_and_get_sectiondir(reponame, section)
     full_filename = join(dir, filename)
     mode = "a+" if (not replaceContent) and (not prepend) else "w"
 
     if prepend:
         with open(full_filename, "r", encoding="UTF-8") as file:
@@ -93,14 +104,15 @@
     """Iterative version of add_repo_nav_to_file"""
     for filename in filenames:
         add_sibling_nav_to_file(filename, include_parent_nav)
 
 def add_sibling_nav_to_file(filename: str, include_parent_nav = True):
     """Add global navigation to the specified file"""
     # Save previous content
+    print(filename)
     with open(filename, "r", encoding="UTF-8") as file:
         prev_content = file.read()
     # Replace content
     with open(filename, "w", encoding="UTF-8") as file:
         # Whether to add ../
         if include_parent_nav:
             file.write(markdown_parent_nav())
```

### Comparing `divio_docs_gen-0.0.3/src/divio_docs_gen/index.py` & `divio_docs_gen-0.0.4/src/divio_docs_gen/index.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Native imports
 from pathlib import Path
 
 # Local imports
-from .repo import get_repos, Repo
+from .repo import get_repos, Repo, tmp_dir
 from .colourstring import ok, nok
 from .sections import sections, RepoSection
 from .table import setup_table, add_and_print, log_and_print, change_log_index
-from .docsgen import filepath_in_exceptions, add_to_docs, add_sibling_nav_to_files, generate_docs_nav_file, clear_docs
-from .args import args_repoconfigs, args_default_owner, args_generate_nav
+from .docsgen import filepath_in_exceptions, write_to_docs, add_sibling_nav_to_files, generate_docs_nav_file, clear_docs, add_to_data_output
+from .args import args_repoconfigs, args_default_owner, args_generate_nav, args_write_to_disk, args_dont_remove_tmp
 
 """Entrypoint for the application"""
 
 
-def generate_docs():    
+def generate_docs() -> dict:
+    data_output = dict()
+    
     # Get headers for CLI table
     headers = [
         "     repository     ", 
         sections['tutorials'].headertext, sections['howtos'].headertext,
         sections['explanations'].headertext, sections['references'].headertext]
 
     setup_table(headers)
@@ -105,16 +107,17 @@
                 if ignore:
                     log_and_print(f"Ignoring {ignore}")
                     continue
                 if copy:
                     copy_filename, copy_dest = copy.rsplit("/", 1)
                     copy_filename = Path(copy_filename).name # The selector can be a path, but only the filename should be kept for handling
                     log_and_print(f"Copying {copy_filename} to {copy_dest}")
-                    
-                    add_to_docs(repo.name, copy_dest, file_content, filename)
+                    # TODO copy in data_output?
+                    if args_write_to_disk:
+                        write_to_docs(repo.name, copy_dest, file_content, filename)
                     repo.files_to_copy.remove(copy)
                     repo.files_to_ignore.append(copy_filename)
                     
                     log_and_print(f"{copy_filename}'s content has been copied!")
                     continue
                     
 
@@ -135,15 +138,17 @@
                         ("filename", file_content) if section_in_filename \
                         else ("filecontent", repoSection.output)
 
                     print_msg = f"Adding {repo.name} - {repoSection.section.name} section from {location}"
 
                     log_and_print(print_msg)
 
-                    created_files.append(add_to_docs(repo.name, repoSection.section, content_to_add, filename=filename))
+                    data_output = add_to_data_output(data_output, repo.name, repoSection.section.name, content_to_add)
+                    if args_write_to_disk:
+                        created_files.append(write_to_docs(repo.name, repoSection.section, content_to_add, filename=filename))
                     log_and_print(print_msg.replace("Adding", "Added"))
 
                     change_log_index(-1)
                     log_and_print(f"...finished handling {filepath}")
                     log_and_print("")
                 else:
                     log_and_print(f"Section {repoSection.section.name} not found in {filepath}")
@@ -154,25 +159,31 @@
             padding = len(repoSection.section.headertext)
             output = ok(padding=padding) if found else nok(padding=padding)
 
             add_and_print(f" {output} |", f"Finished handling {repoSection.section.name}")
         
         
         # If a nav has to be created, do that
-        if args_generate_nav and len(created_files) > 0:
+        if args_write_to_disk and args_generate_nav and len(created_files) > 0:
             add_sibling_nav_to_files(created_files)
             generate_docs_nav_file(repo.name, 1)
 
         print()
         change_log_index(-1)
         log_and_print(f"... parsed {repo.name}\n")
 
 
     change_log_index(-1)
     log_and_print("... finished parsing repos")
 
     # Create a top level nav file
     generate_docs_nav_file("", 1, include_parent_nav=False)
 
+    if not args_dont_remove_tmp:
+        from shutil import rmtree
+        rmtree(tmp_dir)
+
+    return data_output
+
 
 if __name__ == "__main__":
     generate_docs()
```

### Comparing `divio_docs_gen-0.0.3/src/divio_docs_gen/repo.py` & `divio_docs_gen-0.0.4/src/divio_docs_gen/repo.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.0.3/src/divio_docs_gen/sections.py` & `divio_docs_gen-0.0.4/src/divio_docs_gen/sections.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.0.3/src/divio_docs_gen/table.py` & `divio_docs_gen-0.0.4/src/divio_docs_gen/table.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.0.3/src/divio_docs_gen.egg-info/PKG-INFO` & `divio_docs_gen-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: divio-docs-gen
-Version: 0.0.3
+Name: divio_docs_gen
+Version: 0.0.4
 Summary: Turn all the markdown files in your repos into one big, divio structrured documentation
 Author-email: Denperidge <denperidge@gmail.com>
 Project-URL: Homepage, https://github.com/Denperidge-Redpencil/divio-docs-gen
 Project-URL: Bug Tracker, https://github.com/Denperidge-Redpencil/divio-docs-gen/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
@@ -31,30 +31,43 @@
     - If you have a how-to section in your README, that'll get extracted and put in the right spot
     - Or, if you have an how-to.md file, it'll get added in its entirety!
 - Any output structure: this script generates a simple markdown tree. Nothing proprietary, no vendor-lockin. It can be generated from GitHub Actions and put into a Jekyll pages site just as easily as it is run from a Raspberry Pi and used to render the contents of an Ember application.
 
 All you have to do is simply name your headers and/or files after the divio sections (`tutorial`, `how-to`, `explanation`, `reference`). (Oh, don't worry, the search is done through a case insensitive regex. Add more words as you please) 
 
 ## Getting-Started / tutorial
-*(You can also use the [repository template](https://github.com/Denperidge-Redpencil/Divio-Docs-Repo/)!)*
-
-- Clone the repository using `git clone https://github.com/Denperidge-Redpencil/divio-docs-gen.git && cd divio-docs-gen`
-- Install the pre-requirements using `python3 -m pip install -r requirements.txt`
-- Setup the docs.conf file (See the [reference below](#docsconf) and/or the [docs.conf.example](docs.conf.example) file)
-- And finally, run using `python3 app/index.py`!
+- Install the package (`python3 -m pip install divio_docs_gen`)
+- And then either...
+    - Setup the docs.conf file (See the [reference below](#docsconf) and/or the [docs.conf.example](docs.conf.example) file)
+    - Use throught the cli (`python3 -m divio_docs_gen --help`)
 
 ## How-To
+### Install from pip
+```bash
+python3 -m pip install divio_docs_gen
+```
+
+### Clone & run scripts locally
+```bash
+git clone https://github.com/Denperidge-Redpencil/divio-docs-gen.git
+cd divio-docs-gen
+python3 -m pip install -r requirements.txt
+python3 src.divio_docs_gen
+```
+
 ### Build & install package locally
 ```bash
-python3.10 -m pip install --upgrade build setuptools
-python3.10 -m build
-python3.10 -m pip install --force-reinstall ./dist/*.whl
+git clone https://github.com/Denperidge-Redpencil/divio-docs-gen.git
+cd divio-docs-gen/
+python3 -m pip install --upgrade build setuptools
+python3 -m build && python3 -m pip install --force-reinstall ./dist/*.whl
 ```
 *Note: other Python versions can be used!*
 
+
 ## Discussions
 The Divio structure is built upon splitting your documentation into 4 types of documentations. ![The overview of the divio documentation on their website](https://documentation.divio.com/_images/overview.png). In this repository they're referred to as sections.
 
 
 If you want to know more about the design principles of this project, feel free to check out my writeup [here](https://github.com/Denperidge-Redpencil/Learning.md/blob/main/Notes/docs.md#design-principles)!
```

### Comparing `divio_docs_gen-0.0.3/src/divio_docs_gen.egg-info/SOURCES.txt` & `divio_docs_gen-0.0.4/src/divio_docs_gen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

