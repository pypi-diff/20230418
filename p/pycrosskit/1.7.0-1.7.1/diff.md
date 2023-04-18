# Comparing `tmp/pycrosskit-1.7.0.tar.gz` & `tmp/pycrosskit-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrosskit-1.7.0.tar", last modified: Mon Apr 17 23:12:45 2023, max compression
+gzip compressed data, was "pycrosskit-1.7.1.tar", last modified: Tue Apr 18 15:43:39 2023, max compression
```

## Comparing `pycrosskit-1.7.0.tar` & `pycrosskit-1.7.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:12:45.397373 pycrosskit-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-04-17 23:12:45.397373 pycrosskit-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:12:45.389373 pycrosskit-1.7.0/pycrosskit/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:12:45.393373 pycrosskit-1.7.0/pycrosskit/env_platforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/env_platforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/env_platforms/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/env_platforms/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/env_platforms/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/envariables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:12:45.393373 pycrosskit-1.7.0/pycrosskit/shortcut_platforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/shortcut_platforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/shortcut_platforms/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/shortcut_platforms/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:12:45.393373 pycrosskit-1.7.0/pycrosskit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-04-17 23:12:45.000000 pycrosskit-1.7.0/pycrosskit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-17 23:12:45.000000 pycrosskit-1.7.0/pycrosskit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:12:45.000000 pycrosskit-1.7.0/pycrosskit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 23:12:45.000000 pycrosskit-1.7.0/pycrosskit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-17 23:12:45.000000 pycrosskit-1.7.0/pycrosskit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-17 23:12:45.000000 pycrosskit-1.7.0/pycrosskit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:12:45.000000 pycrosskit-1.7.0/pycrosskit.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 23:12:45.397373 pycrosskit-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:12:45.397373 pycrosskit-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/tests/test_env_vars_linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/tests/test_env_vars_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/tests/test_shortcut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.778058 pycrosskit-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-18 15:43:28.000000 pycrosskit-1.7.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-04-18 15:43:39.778058 pycrosskit-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-18 15:43:28.000000 pycrosskit-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.778058 pycrosskit-1.7.1/pycrosskit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-18 15:43:28.000000 pycrosskit-1.7.1/pycrosskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-18 15:43:28.000000 pycrosskit-1.7.1/pycrosskit/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-18 15:43:28.000000 pycrosskit-1.7.1/pycrosskit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.778058 pycrosskit-1.7.1/pycrosskit/env_platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:28.000000 pycrosskit-1.7.1/pycrosskit/env_platforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-18 15:43:28.000000 pycrosskit-1.7.1/pycrosskit/env_platforms/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-18 15:43:28.000000 pycrosskit-1.7.1/pycrosskit/env_platforms/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-04-18 15:43:28.000000 pycrosskit-1.7.1/pycrosskit/env_platforms/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-18 15:43:28.000000 pycrosskit-1.7.1/pycrosskit/envariables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.778058 pycrosskit-1.7.1/pycrosskit/shortcut_platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:28.000000 pycrosskit-1.7.1/pycrosskit/shortcut_platforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-18 15:43:28.000000 pycrosskit-1.7.1/pycrosskit/shortcut_platforms/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-18 15:43:28.000000 pycrosskit-1.7.1/pycrosskit/shortcut_platforms/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-18 15:43:28.000000 pycrosskit-1.7.1/pycrosskit/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.778058 pycrosskit-1.7.1/pycrosskit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-04-18 15:43:39.000000 pycrosskit-1.7.1/pycrosskit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-18 15:43:39.000000 pycrosskit-1.7.1/pycrosskit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:43:39.000000 pycrosskit-1.7.1/pycrosskit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-18 15:43:39.000000 pycrosskit-1.7.1/pycrosskit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 15:43:39.000000 pycrosskit-1.7.1/pycrosskit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 15:43:39.000000 pycrosskit-1.7.1/pycrosskit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:43:39.000000 pycrosskit-1.7.1/pycrosskit.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:43:39.778058 pycrosskit-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-18 15:43:28.000000 pycrosskit-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.778058 pycrosskit-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-18 15:43:28.000000 pycrosskit-1.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-18 15:43:28.000000 pycrosskit-1.7.1/tests/test_env_vars_linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-18 15:43:28.000000 pycrosskit-1.7.1/tests/test_env_vars_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-18 15:43:28.000000 pycrosskit-1.7.1/tests/test_shortcut.py
```

### Comparing `pycrosskit-1.7.0/LICENSE.md` & `pycrosskit-1.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.0/PKG-INFO` & `pycrosskit-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrosskit
-Version: 1.7.0
+Version: 1.7.1
 Summary: Cross Platform Toolkit for Windows and Linux in order to make variables and shortcuts easy 
 Home-page: https://github.com/jiri-otoupal/py-cross-kit
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: Apache 2.0
 Keywords: Python Cross Platform Toolkit
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pycrosskit-1.7.0/README.md` & `pycrosskit-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.0/pycrosskit/__init__.py` & `pycrosskit-1.7.1/pycrosskit/__init__.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.0/pycrosskit/env_platforms/linux.py` & `pycrosskit-1.7.1/pycrosskit/env_platforms/linux.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import os
 import subprocess
-from typing import Union, Any, Tuple
+from typing import Union, Any
 
 from pycrosskit.env_platforms.exceptions import VarNotFound
 
 
 class LinVar:
     shell = "bash"
     shell_file = "~/.bashrc"
@@ -18,52 +18,30 @@
         return cls
 
     @classmethod
     def __fetch_bashrc_line(cls, shell_file="~/.bashrc") -> str:
         """
         Generator that fetches bashrc lines one by one
         """
-        _, shell_file = cls.get_shell(shell_file)
-
         with open(os.path.expanduser(shell_file), "r") as f:
             line = True
             while line:
                 line = f.readline()
                 yield line
 
     @classmethod
-    def get_shell(
-            cls, shell: str = "bash", shell_file: str = "~/.bashrc"
-    ) -> Tuple[str, str]:
-        """
-        Get Shell that is used for every access
-        :param shell: Shell binary name
-        :param shell_file: Shell file path
-        :return: shell binary name, shell file path
-        """
-        if cls.shell_file != "~/.bashrc":
-            shell_file = cls.shell_file
-
-        if cls.shell != "bash":
-            shell = cls.shell
-
-        return shell, shell_file
-
-    @classmethod
     def unset(cls, key: str, shell_file="~/.bashrc"):
         """
         Unsets variable from environment
         :param shell_file: Custom Shell file path
         :param key: Key of variable
 
         Can throw PermissionError if bashrc is not accessible
         """
-        shell, shell_file = cls.get_shell(shell_file)
-
-        cls.logger.debug(f"Unsetting system variable {key} {shell} {shell_file}")
+        cls.logger.debug(f"Unsetting system variable {key} {shell_file}")
 
         replacement_lines = []
 
         for line in cls.__fetch_bashrc_line(shell_file):
 
             # Way faster than regex
             # Do search without quotes
@@ -90,16 +68,14 @@
         Get Environment Variable
         :param shell: Custom Shell
         :param shell_file: Custom shell file path
         :param key: Key of variable
         :param default: Returned if variable empty or undefined
         :return:
         """
-        shell, shell_file = cls.get_shell(shell, shell_file)
-
         cls.logger.debug(f"Getting variable {key} {shell} {shell_file}")
         value: str = subprocess.check_output(
             ["/usr/bin/env", shell, "-ic", f". {shell_file} && echo -n ${key}"],
             stderr=subprocess.DEVNULL,
         ).decode("utf-8")
 
         # Check for empty or unset variable
@@ -119,11 +95,9 @@
     def set(cls, key: str, value: str, shell_file="~/.bashrc"):
         """
         Set Environment Variable
         :param shell_file: Custom Shell File Path
         :param key: Key of variable
         :param value: Value to be set
         """
-        shell, shell_file = cls.get_shell(shell_file)
-
         os.system(f"echo '{cls.EXPORT_STRING(key, value)}' >> {shell_file}")
-        cls.logger.debug(f"Set variable {key} {value} {shell} {shell_file}")
+        cls.logger.debug(f"Set variable {key} {value} {shell_file}")
```

### Comparing `pycrosskit-1.7.0/pycrosskit/env_platforms/windows.py` & `pycrosskit-1.7.1/pycrosskit/env_platforms/windows.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                 .replace("%", "")
             )
 
         return value
 
     @classmethod
     def __get_policy_key_readonly(
-        cls, reg_path: str, reg_key: winreg.HKEY_CURRENT_USER
+            cls, reg_path: str, reg_key=winreg.HKEY_CURRENT_USER
     ):
         root = winreg.ConnectRegistry(None, reg_key)
         policy_key = winreg.OpenKeyEx(root, reg_path)
         return policy_key, root
 
     @classmethod
     def __unset(cls, key: str, policy_key: winreg.HKEYType, registry: bool):
@@ -53,46 +53,46 @@
             if err != 0:
                 raise VarNotFound("Environment Variable not found")
         else:
             winreg.DeleteKey(policy_key, str(key))
 
     @classmethod
     def unset(
-        cls,
-        key,
-        reg_path=r"SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall",
-        registry=True,
-        silent=False,
+            cls,
+            key,
+            reg_path=r"SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall",
+            registry=True,
+            silent=False,
     ):
         """
         Unsets variable from environment or registry
         :param key: Variable name
         :param reg_path: Register path for windows
         :param registry: Only for windows, if true variable is obtained from registry path
                         if false variable is obtained to environment variables
         :param silent: If unset should fail silently in case that variable does not exist
         """
         try:
             cls.logger.debug(f"Unsetting system variable {key}")
-            policy_key, root = cls.__get_policy_key_readonly(reg_path)
+            policy_key, _ = cls.__get_policy_key_readonly(reg_path)
             cls.__unset(key, policy_key, registry)
             cls.logger.debug(f"Finished Unsetting system variable {key}")
         except FileNotFoundError as ex:
             if not silent:
                 cls.logger.debug(f"Unset of variable {key} failed")
                 raise VarNotFound(str(ex))
             cls.logger.debug(f"Unset of variable {key} failed silently")
 
     @classmethod
     def get(
-        cls,
-        key: str,
-        default: Union[Any, VarNotFound] = VarNotFound,
-        reg_path: str = r"SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall",
-        registry: bool = True,
+            cls,
+            key: str,
+            default: Union[Any, VarNotFound] = VarNotFound,
+            reg_path: str = r"SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall",
+            registry: bool = True,
     ) -> str:
         """
         Get Environment Variable
         :param default: Value returned if not found
         ( raises VarNotFound exception if not set)
         :param key: Variable Name
         :param reg_path: Register path for windows
@@ -111,22 +111,22 @@
                 return default
             cls.logger.debug(f"Variable {key} not found")
             raise ex
         return value
 
     @classmethod
     def set(
-        cls,
-        key,
-        value,
-        subkey="",
-        reg_path=r"SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall",
-        reg_key=winreg.HKEY_CURRENT_USER,
-        registry=True,
-        silent=False,
+            cls,
+            key,
+            value,
+            subkey="",
+            reg_path=r"SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall",
+            reg_key=winreg.HKEY_CURRENT_USER,
+            registry=True,
+            silent=False,
     ):
         """
         Set Environment Variable
         :param silent: If permission error should fail silently
         :param key: Variable Name
         :param value: Variable Value
         :param subkey: Sub-Key under key ( like file in folder )
```

### Comparing `pycrosskit-1.7.0/pycrosskit/envariables.py` & `pycrosskit-1.7.1/pycrosskit/envariables.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.0/pycrosskit/shortcut_platforms/linux.py` & `pycrosskit-1.7.1/pycrosskit/shortcut_platforms/linux.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     if os.path.exists(ud_file):
         val = desktop
         with open(ud_file, "r") as fh:
             text = fh.readlines()
         for line in text:
             if "DESKTOP" in line:
                 line = line.replace("$HOME", homedir)[:-1]
-                key, val = line.split("=")
+                _, val = line.split("=")
                 val = val.replace('"', "").replace("'", "")
         desktop = val
     return desktop
 
 
 def get_startmenu() -> str:
     """Get user start menu location.
@@ -153,15 +153,15 @@
         desktop_path = user_folders.desktop + "/" + shortcut_name + scut_ext
         if os.path.exists(desktop_path):
             os.chmod(desktop_path, stat.S_IWRITE)
             os.remove(desktop_path)
     return desktop_path, startmenu_path
 
 
-def __write_shortcut(dest_path: Path, shortcut_instance: str, file_content: str):
+def __write_shortcut(dest_path: Path, shortcut_instance: Shortcut, file_content: str):
     """Writes shortcut content to destination.
 
     :param Path dest_path: Path where write file
     :param str shortcut_instance: Instance of shortcut that will be used
     :param str file_content: Content of future icon from DESKTOP_FORM.format(...)
     """
     if not dest_path.parent.exists():
```

### Comparing `pycrosskit-1.7.0/pycrosskit/shortcut_platforms/windows.py` & `pycrosskit-1.7.1/pycrosskit/shortcut_platforms/windows.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.0/pycrosskit/shortcuts.py` & `pycrosskit-1.7.1/pycrosskit/shortcuts.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.0/pycrosskit.egg-info/PKG-INFO` & `pycrosskit-1.7.1/pycrosskit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrosskit
-Version: 1.7.0
+Version: 1.7.1
 Summary: Cross Platform Toolkit for Windows and Linux in order to make variables and shortcuts easy 
 Home-page: https://github.com/jiri-otoupal/py-cross-kit
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: Apache 2.0
 Keywords: Python Cross Platform Toolkit
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pycrosskit-1.7.0/pycrosskit.egg-info/SOURCES.txt` & `pycrosskit-1.7.1/pycrosskit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.0/setup.py` & `pycrosskit-1.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.0/tests/test_env_vars_linux.py` & `pycrosskit-1.7.1/tests/test_env_vars_linux.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.0/tests/test_env_vars_windows.py` & `pycrosskit-1.7.1/tests/test_env_vars_windows.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.0/tests/test_shortcut.py` & `pycrosskit-1.7.1/tests/test_shortcut.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 class Test_Shortcuts(unittest.TestCase):
     def test_create_desktop(self):
         sh = Shortcut("Test", "__init__.py", desktop=True)
         self.assertEqual(True, os.path.exists(sh.desktop_path))
 
     def test_delete_desktop(self):
-        desktop, startmenu = Shortcut.delete("Test", desktop=True)
+        desktop, _ = Shortcut.delete("Test", desktop=True)
         self.assertEqual(True, not os.path.exists(desktop))
 
     def test_create_startmenu(self):
         sh = Shortcut("Test", "__init__.py", start_menu=True)
         self.assertEqual(True, os.path.exists(sh.startmenu_path))
 
     def test_delete_startmenu(self):
-        desktop, startmenu = Shortcut.delete("Test", start_menu=True)
+        _, startmenu = Shortcut.delete("Test", start_menu=True)
         self.assertEqual(True, not os.path.exists(startmenu))
 
     def test_create_both(self):
         sh = Shortcut("Test", "__init__.py", desktop=True, start_menu=True)
         self.assertEqual(True, os.path.exists(sh.desktop_path))
         self.assertEqual(True, os.path.exists(sh.startmenu_path))
```

