# Comparing `tmp/cleez-0.1.1.tar.gz` & `tmp/cleez-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleez-0.1.1.tar", max compression
+gzip compressed data, was "cleez-0.1.2.tar", max compression
```

## Comparing `cleez-0.1.1.tar` & `cleez-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      583 2023-04-17 08:35:32.159563 cleez-0.1.1/LICENSE
--rw-r--r--   0        0        0      896 2023-04-17 09:52:54.513608 cleez-0.1.1/README.rst
--rw-r--r--   0        0        0     3065 2023-04-17 19:10:48.351415 cleez-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      340 2023-04-17 16:19:10.886202 cleez-0.1.1/src/cleez/__init__.py
--rw-r--r--   0        0        0     4598 2023-04-17 18:29:05.545545 cleez-0.1.1/src/cleez/cleez.py
--rw-r--r--   0        0        0      371 2023-04-16 21:08:33.001276 cleez-0.1.1/src/cleez/colors.py
--rw-r--r--   0        0        0     1200 2023-04-17 17:46:43.468653 cleez-0.1.1/src/cleez/command.py
--rw-r--r--   0        0        0      268 2023-04-17 18:11:58.414950 cleez-0.1.1/src/cleez/exceptions.py
--rw-r--r--   0        0        0     2213 2023-04-17 19:10:01.539479 cleez-0.1.1/src/cleez/help.py
--rw-r--r--   0        0        0     1758 1970-01-01 00:00:00.000000 cleez-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-04-17 08:35:32.159563 cleez-0.1.2/LICENSE
+-rw-r--r--   0        0        0      896 2023-04-17 09:52:54.513608 cleez-0.1.2/README.rst
+-rw-r--r--   0        0        0     3102 2023-04-18 16:41:05.082118 cleez-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      340 2023-04-17 16:19:10.886202 cleez-0.1.2/src/cleez/__init__.py
+-rw-r--r--   0        0        0     4598 2023-04-17 18:29:05.545545 cleez-0.1.2/src/cleez/cleez.py
+-rw-r--r--   0        0        0      371 2023-04-16 21:08:33.001276 cleez-0.1.2/src/cleez/colors.py
+-rw-r--r--   0        0        0     1237 2023-04-18 13:52:32.245318 cleez-0.1.2/src/cleez/command.py
+-rw-r--r--   0        0        0      268 2023-04-17 18:11:58.414950 cleez-0.1.2/src/cleez/exceptions.py
+-rw-r--r--   0        0        0     2692 2023-04-17 19:57:10.619068 cleez-0.1.2/src/cleez/help.py
+-rw-r--r--   0        0        0     1758 1970-01-01 00:00:00.000000 cleez-0.1.2/PKG-INFO
```

### Comparing `cleez-0.1.1/LICENSE` & `cleez-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cleez-0.1.1/README.rst` & `cleez-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `cleez-0.1.1/pyproject.toml` & `cleez-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "cleez"
-version = "0.1.1"
+version = "0.1.2"
 homepage = "https://github.com/abilian/cleez"
 description = "Simple class-based CLI framework."
 authors = ["Abilian SAS <sf@abilian.com>"]
 readme = "README.rst"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
@@ -86,14 +86,15 @@
     "PLC", "PLE", "PLR", "PLW",
 ]
 # Add later: "ANN", "ERA"...
 
 ignore = [
     "S101",  # Use of `assert` detected
     "SIM108", # Use ternary operator
+    "A001",  # Shadowing of built-in
 ]
 
 # ---
 
 [tool.bandit]
 skips = [
   "B404", # blacklist
```

### Comparing `cleez-0.1.1/src/cleez/cleez.py` & `cleez-0.1.2/src/cleez/cleez.py`

 * *Files identical despite different names*

### Comparing `cleez-0.1.1/src/cleez/command.py` & `cleez-0.1.2/src/cleez/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 
         for argument in self.arguments:
             subparser.add_argument(*argument.args, **argument.kwargs)
 
         for option in self.options:
             subparser.add_argument(*option.args, **option.kwargs)
 
-        self.subparsers = subparser.add_subparsers()
+        if " " not in self.name:
+            self.subparsers = subparser.add_subparsers()
 
 
 class Argument:
     def __init__(self, *args, **kwargs):
         self.args = args
         self.kwargs = kwargs
```

### Comparing `cleez-0.1.1/src/cleez/help.py` & `cleez-0.1.2/src/cleez/help.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,34 +32,44 @@
             print(f"  {blue(option.args[0])}  {option.kwargs['help']}")
         print()
 
     def print_commands(self, commands: list[Command]):
         print(bold("Available commands:"))
 
         commands = self.get_commands(commands)
-
         simple_commands = [command for command in commands if " " not in command.name]
         complex_commands = [command for command in commands if " " in command.name]
+
+        self.print_simple_commands_help(simple_commands)
+        self.print_complex_commands_help(complex_commands)
+
+    def print_simple_commands_help(self, commands: list[Command]):
+        if not commands:
+            return
         max_command_length = max(len(command.name) for command in commands)
         w = max_command_length
-
-        for command in simple_commands:
+        for command in commands:
             cmd_name = f"{command.name:<{w}}"
-            print(f"  {blue(cmd_name)}  {command.__doc__}")
+            help = (command.__doc__ or "").split("\n")[0].strip()
+            print(f"  {blue(cmd_name)}  {help}")
 
-        groups = groupby(complex_commands, lambda command: command.name.split(" ")[0])
+    def print_complex_commands_help(self, commands: list[Command]):
+        if not commands:
+            return
+        max_command_length = max(len(command.name) for command in commands)
+        w = max_command_length
+        groups = groupby(commands, lambda command: command.name.split(" ")[0])
         for group_name, group in groups:
             print()
             print(f" {green(group_name)}")
 
             for command in group:
-                if not command.name:
-                    continue
                 cmd_name = f"{command.name:<{w}}"
-                print(f"  {blue(cmd_name)}  {command.__doc__}")
+                help = (command.__doc__ or "").split("\n")[0].strip()
+                print(f"  {blue(cmd_name)}  {help}")
 
     def get_commands(self, commands: list[Command]):
         def sorter(command):
             return len(command.name.split(" ")), command.name
 
         commands = [command for command in commands if command.name]
         commands = [command for command in commands if not command.hide_from_help]
```

### Comparing `cleez-0.1.1/PKG-INFO` & `cleez-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleez
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple class-based CLI framework.
 Home-page: https://github.com/abilian/cleez
 Author: Abilian SAS
 Author-email: sf@abilian.com
 Requires-Python: >=3.9,<4
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

