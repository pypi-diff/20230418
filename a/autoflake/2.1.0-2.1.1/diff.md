# Comparing `tmp/autoflake-2.1.0.tar.gz` & `tmp/autoflake-2.1.1.tar.gz`

## Comparing `autoflake-2.1.0.tar` & `autoflake-2.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0    47002 2020-02-02 00:00:00.000000 autoflake-2.1.0/autoflake.py
--rwxr-xr-x   0        0        0    91308 2020-02-02 00:00:00.000000 autoflake-2.1.0/test_autoflake.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 autoflake-2.1.0/.gitignore
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 autoflake-2.1.0/AUTHORS.rst
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 autoflake-2.1.0/LICENSE
--rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 autoflake-2.1.0/README.md
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 autoflake-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 autoflake-2.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0    46884 2020-02-02 00:00:00.000000 autoflake-2.1.1/autoflake.py
+-rwxr-xr-x   0        0        0    90488 2020-02-02 00:00:00.000000 autoflake-2.1.1/test_autoflake.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 autoflake-2.1.1/.gitignore
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 autoflake-2.1.1/AUTHORS.rst
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 autoflake-2.1.1/LICENSE
+-rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 autoflake-2.1.1/README.md
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 autoflake-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 autoflake-2.1.1/PKG-INFO
```

### Comparing `autoflake-2.1.0/autoflake.py` & `autoflake-2.1.1/autoflake.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 import tokenize
 
 import pyflakes.api
 import pyflakes.messages
 import pyflakes.reporter
 
 
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 
 
 _LOGGER = logging.getLogger("autoflake")
 _LOGGER.propagate = False
 
 ATOMS = frozenset([tokenize.NAME, tokenize.NUMBER, tokenize.STRING])
 
@@ -1190,19 +1190,15 @@
         "no": False,
         "false": False,
         "off": False,
     }
 
     if "config_file" in flag_args:
         config_file = pathlib.Path(flag_args["config_file"]).resolve()
-
-        if config_file.suffix == ".toml":
-            config = process_pyproject_toml(config_file)
-        else:
-            config = process_config_file(config_file)
+        config = process_config_file(config_file)
 
         if not config:
             _LOGGER.error(
                 "can't parse config file '%s'",
                 config_file,
             )
             return flag_args, False
```

### Comparing `autoflake-2.1.0/test_autoflake.py` & `autoflake-2.1.1/test_autoflake.py`

 * *Files 1% similar despite different names*

```diff
@@ -3381,40 +3381,14 @@
             assert success is True
             assert args == self.with_defaults(
                 files=files,
                 config_file=temp_config,
                 check=True,
             )
 
-    def test_config_option_toml(self):
-        with temporary_file(
-            suffix=".toml",
-            contents=(
-                "[tool.autoflake]\n"
-                "check = true\n"
-                'exclude = [\n  "build",\n  ".venv",\n]'
-            ),
-        ) as temp_config:
-            self.create_file("test_me.py")
-            files = [self.effective_path("test_me.py")]
-
-            args, success = autoflake.merge_configuration_file(
-                {
-                    "files": files,
-                    "config_file": temp_config,
-                },
-            )
-            assert success is True
-            assert args == self.with_defaults(
-                files=files,
-                config_file=temp_config,
-                check=True,
-                exclude="build,.venv",
-            )
-
     def test_load_false(self):
         self.create_file("test_me.py")
         self.create_file(
             "setup.cfg",
             "[autoflake]\nexpand-star-imports = no\n",
         )
         files = [self.effective_path("test_me.py")]
```

### Comparing `autoflake-2.1.0/AUTHORS.rst` & `autoflake-2.1.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `autoflake-2.1.0/LICENSE` & `autoflake-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autoflake-2.1.0/README.md` & `autoflake-2.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -197,11 +197,11 @@
 
 ## Using [pre-commit](https://pre-commit.com) hooks
 
 Add the following to your `.pre-commit-config.yaml`
 
 ```yaml
 -   repo: https://github.com/PyCQA/autoflake
-    rev: v2.1.0
+    rev: v2.1.1
     hooks:
     -   id: autoflake
 ```
```

### Comparing `autoflake-2.1.0/pyproject.toml` & `autoflake-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autoflake-2.1.0/PKG-INFO` & `autoflake-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoflake
-Version: 2.1.0
+Version: 2.1.1
 Summary: Removes unused imports and unused variables
 Project-URL: Homepage, https://www.github.com/PyCQA/autoflake
 License: MIT
 License-File: AUTHORS.rst
 License-File: LICENSE
 Keywords: automatic,clean,fix,import,unused
 Classifier: Environment :: Console
@@ -217,11 +217,11 @@
 
 ## Using [pre-commit](https://pre-commit.com) hooks
 
 Add the following to your `.pre-commit-config.yaml`
 
 ```yaml
 -   repo: https://github.com/PyCQA/autoflake
-    rev: v2.1.0
+    rev: v2.1.1
     hooks:
     -   id: autoflake
 ```
```

