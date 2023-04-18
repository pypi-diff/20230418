# Comparing `tmp/spwn-1.2.3.tar.gz` & `tmp/spwn-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spwn-1.2.3.tar", last modified: Wed Mar 29 18:07:58 2023, max compression
+gzip compressed data, was "spwn-1.2.4.tar", last modified: Tue Apr 18 14:32:45 2023, max compression
```

## Comparing `spwn-1.2.3.tar` & `spwn-1.2.4.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-03-29 18:07:58.416674 spwn-1.2.3/
--rw-rw-r--   0 marco     (1000) marco     (1000)     1071 2022-11-23 16:39:40.000000 spwn-1.2.3/LICENSE
--rw-rw-r--   0 marco     (1000) marco     (1000)     6664 2023-03-29 18:07:58.416674 spwn-1.2.3/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)     6208 2023-02-22 19:16:58.000000 spwn-1.2.3/README.md
--rw-rw-r--   0 marco     (1000) marco     (1000)       38 2023-03-29 18:07:58.416674 spwn-1.2.3/setup.cfg
--rw-rw-r--   0 marco     (1000) marco     (1000)      691 2023-03-29 17:28:13.000000 spwn-1.2.3/setup.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-03-29 18:07:58.416674 spwn-1.2.3/spwn/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2022-11-23 16:39:40.000000 spwn-1.2.3/spwn/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     3824 2023-02-22 18:56:22.000000 spwn-1.2.3/spwn/analyzer.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     1381 2023-02-07 19:08:30.000000 spwn-1.2.3/spwn/angr-scan.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      296 2022-12-21 14:15:48.000000 spwn-1.2.3/spwn/binary.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2384 2023-02-22 18:43:05.000000 spwn-1.2.3/spwn/configgenerator.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      814 2022-12-21 14:15:58.000000 spwn-1.2.3/spwn/configmanager.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     1966 2022-12-21 14:29:09.000000 spwn-1.2.3/spwn/customanalyzer.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     4015 2023-03-29 15:55:49.000000 spwn-1.2.3/spwn/filemanager.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     1493 2023-01-15 13:28:29.000000 spwn-1.2.3/spwn/libc.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      112 2022-12-21 14:17:19.000000 spwn-1.2.3/spwn/loader.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     3747 2022-12-21 14:17:55.000000 spwn-1.2.3/spwn/scripter.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     6075 2023-02-28 22:18:25.000000 spwn-1.2.3/spwn/spwn.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2784 2022-12-21 14:18:42.000000 spwn-1.2.3/spwn/utils.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-03-29 18:07:58.416674 spwn-1.2.3/spwn.egg-info/
--rw-rw-r--   0 marco     (1000) marco     (1000)     6664 2023-03-29 18:07:58.000000 spwn-1.2.3/spwn.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)      424 2023-03-29 18:07:58.000000 spwn-1.2.3/spwn.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2023-03-29 18:07:58.000000 spwn-1.2.3/spwn.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       40 2023-03-29 18:07:58.000000 spwn-1.2.3/spwn.egg-info/entry_points.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       21 2023-03-29 18:07:58.000000 spwn-1.2.3/spwn.egg-info/requires.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        5 2023-03-29 18:07:58.000000 spwn-1.2.3/spwn.egg-info/top_level.txt
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 14:32:45.111154 spwn-1.2.4/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1071 2023-04-12 12:46:15.000000 spwn-1.2.4/LICENSE
+-rw-r--r--   0 marco     (1000) marco     (1000)     7372 2023-04-18 14:32:45.111154 spwn-1.2.4/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)     6916 2023-04-18 13:24:55.000000 spwn-1.2.4/README.md
+-rw-r--r--   0 marco     (1000) marco     (1000)       38 2023-04-18 14:32:45.111154 spwn-1.2.4/setup.cfg
+-rw-r--r--   0 marco     (1000) marco     (1000)      691 2023-04-18 13:43:37.000000 spwn-1.2.4/setup.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 14:32:45.111154 spwn-1.2.4/spwn/
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2023-04-12 12:46:15.000000 spwn-1.2.4/spwn/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     3952 2023-04-17 13:18:21.000000 spwn-1.2.4/spwn/analyzer.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      296 2023-04-12 12:46:15.000000 spwn-1.2.4/spwn/binary.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2459 2023-04-18 12:27:58.000000 spwn-1.2.4/spwn/configgenerator.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1189 2023-04-18 12:31:23.000000 spwn-1.2.4/spwn/configmanager.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1966 2023-04-12 12:46:15.000000 spwn-1.2.4/spwn/customanalyzer.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     4015 2023-04-12 12:46:15.000000 spwn-1.2.4/spwn/filemanager.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1493 2023-04-12 12:46:15.000000 spwn-1.2.4/spwn/libc.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      112 2023-04-12 12:46:15.000000 spwn-1.2.4/spwn/loader.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     4250 2023-04-18 13:12:59.000000 spwn-1.2.4/spwn/scripter.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     6275 2023-04-18 13:22:39.000000 spwn-1.2.4/spwn/spwn.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2784 2023-04-12 12:46:15.000000 spwn-1.2.4/spwn/utils.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 14:32:45.111154 spwn-1.2.4/spwn.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)     7372 2023-04-18 14:32:45.000000 spwn-1.2.4/spwn.egg-info/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)      406 2023-04-18 14:32:45.000000 spwn-1.2.4/spwn.egg-info/SOURCES.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)        1 2023-04-18 14:32:45.000000 spwn-1.2.4/spwn.egg-info/dependency_links.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       40 2023-04-18 14:32:45.000000 spwn-1.2.4/spwn.egg-info/entry_points.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       21 2023-04-18 14:32:45.000000 spwn-1.2.4/spwn.egg-info/requires.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)        5 2023-04-18 14:32:45.000000 spwn-1.2.4/spwn.egg-info/top_level.txt
```

### Comparing `spwn-1.2.3/LICENSE` & `spwn-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spwn-1.2.3/PKG-INFO` & `spwn-1.2.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spwn
-Version: 1.2.3
+Version: 1.2.4
 Summary: Automatic tool to quickly start a pwn CTF challenge
 Home-page: https://github.com/MarcoMeinardi/spwn
 Author: Chino
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
@@ -14,15 +14,15 @@
 
 # Spwn
 
 This repository started as a translation of
 [pwninit](https://github.com/io12/pwninit). It has been created because I
 love the utilities provided by pwninit, but I'm too lazy to learn Rust and
 I wanted to customize it, so I rewrote it in python (and added
-some more features).
+~~some~~ a lot more features).
 
 ## Features
  * Auto detect files (binary, libc, loader)
  * Get loader from libc version (if missing)
  * Unstrip the libc with `pwn.libcdb.unstrip_libc`
  * Set binary and loader executable
  * Set runpath and interpreter for the debug binary
@@ -38,22 +38,23 @@
  * Launch decompiler
  * Run [cwe_checker](https://github.com/fkie-cad/cwe_checker)
  * Launch custom user-provided commands
  * Launch custom user-provided python scripts
 
 ## Usage
 ```
-spwn [-h] [-i] [-io] [-nd] [--setup] [{inter,i,ionly,io,nd,nodecomp,setup,} ...]
+spwn [-h] [-i] [-io] [-nd] [--config] [{inter,i,ionly,io,nd,nodecomp,config} ...] [template]
 
 options:
   -h, --help            show this help message and exit
   -i, --inter           Interactively create interaction functions
   -io, --ionly          Create the interaction functions, without doing any analysis
   -nd, --nodecomp       Don't open the decompiler
-  --setup               Setup configs and quit
+  --config              Setup configs and quit
+  template              template to use
 ```
 
 If the files have weird names (such as the libc name not starting with
 "libc"), the autodetection will fail and fall in the manual selection,
 the best fix for this is to rename the files.
 
 To understand how the interactions creation works, I suggest to just try
@@ -103,14 +104,27 @@
 if you want to change the location of the config file, you will have to
 edit the source code. The variable is `CONFIG_PATH` in `spwn.py`.
 Its location should be
 `~/.local/lib/python3.{python-version}/site-packages/spwn/spwn.py`.
 Note that if you reinstall or update `spwn`, this variable will be
 overwritten.
 
+### Multiple templates
+You can have multiple templates and select which one to use from command
+line. You have to place your templates in the same directory of the base
+template (`template_file`), and name it
+`{custom_template_prefix}{name}.py`. To use it, you just have to specify
+`name` in the command line (`spwn {name}`).
+
+The whole file will be treated as a format string, so, be careful to put
+double curly brackets if they don't have to be treated as format
+specifiers (`my_set = {{1, 2, 3}}`). The actual format specifiers (which
+you have to place in single curly brackets) are: `{binary}`, `{libc}`,
+`{debug_dir}` and `{interactions}`.
+
 ### Suppress warnings
 Don't show warning messages for non installed non-vital dependencies.
 
 ### Custom commands
 The pre and post analysis commands, are in the form `[command, timeout]`.
 `command` is a list of strings and should contain the `"{binary}"` or
 `"{debug_binary}"` string in order to be formatted with the correct
```

### Comparing `spwn-1.2.3/README.md` & `spwn-1.2.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Spwn
 
 This repository started as a translation of
 [pwninit](https://github.com/io12/pwninit). It has been created because I
 love the utilities provided by pwninit, but I'm too lazy to learn Rust and
 I wanted to customize it, so I rewrote it in python (and added
-some more features).
+~~some~~ a lot more features).
 
 ## Features
  * Auto detect files (binary, libc, loader)
  * Get loader from libc version (if missing)
  * Unstrip the libc with `pwn.libcdb.unstrip_libc`
  * Set binary and loader executable
  * Set runpath and interpreter for the debug binary
@@ -24,22 +24,23 @@
  * Launch decompiler
  * Run [cwe_checker](https://github.com/fkie-cad/cwe_checker)
  * Launch custom user-provided commands
  * Launch custom user-provided python scripts
 
 ## Usage
 ```
-spwn [-h] [-i] [-io] [-nd] [--setup] [{inter,i,ionly,io,nd,nodecomp,setup,} ...]
+spwn [-h] [-i] [-io] [-nd] [--config] [{inter,i,ionly,io,nd,nodecomp,config} ...] [template]
 
 options:
   -h, --help            show this help message and exit
   -i, --inter           Interactively create interaction functions
   -io, --ionly          Create the interaction functions, without doing any analysis
   -nd, --nodecomp       Don't open the decompiler
-  --setup               Setup configs and quit
+  --config              Setup configs and quit
+  template              template to use
 ```
 
 If the files have weird names (such as the libc name not starting with
 "libc"), the autodetection will fail and fall in the manual selection,
 the best fix for this is to rename the files.
 
 To understand how the interactions creation works, I suggest to just try
@@ -89,14 +90,27 @@
 if you want to change the location of the config file, you will have to
 edit the source code. The variable is `CONFIG_PATH` in `spwn.py`.
 Its location should be
 `~/.local/lib/python3.{python-version}/site-packages/spwn/spwn.py`.
 Note that if you reinstall or update `spwn`, this variable will be
 overwritten.
 
+### Multiple templates
+You can have multiple templates and select which one to use from command
+line. You have to place your templates in the same directory of the base
+template (`template_file`), and name it
+`{custom_template_prefix}{name}.py`. To use it, you just have to specify
+`name` in the command line (`spwn {name}`).
+
+The whole file will be treated as a format string, so, be careful to put
+double curly brackets if they don't have to be treated as format
+specifiers (`my_set = {{1, 2, 3}}`). The actual format specifiers (which
+you have to place in single curly brackets) are: `{binary}`, `{libc}`,
+`{debug_dir}` and `{interactions}`.
+
 ### Suppress warnings
 Don't show warning messages for non installed non-vital dependencies.
 
 ### Custom commands
 The pre and post analysis commands, are in the form `[command, timeout]`.
 `command` is a list of strings and should contain the `"{binary}"` or
 `"{debug_binary}"` string in order to be formatted with the correct
```

### Comparing `spwn-1.2.3/setup.py` & `spwn-1.2.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md") as f:
 	long_description = f.read()
 
 setuptools.setup(
 	name="spwn",
-	version="1.2.3",
+	version="1.2.4",
 	author="Chino",
 	description="Automatic tool to quickly start a pwn CTF challenge",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	classifiers=[
 		"Environment :: Console",
 		"Operating System :: POSIX :: Linux",
```

### Comparing `spwn-1.2.3/spwn/analyzer.py` & `spwn-1.2.4/spwn/analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,21 +58,22 @@
 
 		if dangerous_functions:
 			print("[!] There are some dangerous functions:")
 			print(" ".join(dangerous_functions))
 
 	def run_yara(self) -> None:
 		rules = yara.compile(self.configs.yara_rules)
-		with open(self.files.binary.name, "rb") as f:
-			matches = rules.match(data=f.read())
+		matches = rules.match(self.files.binary.name)
 
 		if matches:
 			print("[!] yara found something")
 			for match in matches:
-				print(match)
+				addresses = [instance.offset for string_match in match.strings for instance in string_match.instances]
+				print(f'[*] {match.rule} at {", ".join(map(hex, addresses))}')
+			print()
 
 	def open_decompiler(self) -> None:
 		if self.configs.idafree_command and self.files.binary.pwnfile.arch == "amd64" and self.files.binary.pwnfile.bits == 64:
 			subprocess.Popen(self.configs.idafree_command.format(binary=self.files.binary.name), shell=True, start_new_session=True)
 		elif self.configs.decompiler_command:
 			subprocess.Popen(self.configs.decompiler_command.format(binary=self.files.binary.name), shell=True, start_new_session=True)
```

### Comparing `spwn-1.2.3/spwn/configgenerator.py` & `spwn-1.2.4/spwn/configgenerator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import os
 import requests
 import json
 
 
 default_configs = {
 	"debug_dir": "debug",
-	"suppress_warnings": False,
 	"script_file": "a.py",
+	"pwn_process": "r",
+	"tab": "\t",
 	"template_file": "~/.config/spwn/template.py",
+	"custom_template_prefix": "template_",
+	"suppress_warnings": False,
 	"yara_rules": "~/.config/spwn/findcrypt3.rules",
 	"preanalysis_commands": [],
 	"postanalysis_commands": [],
 	"preanalysis_scripts": [],
 	"postanalysis_scripts": [],
 	"idafree_command": "",
 	"decompiler_command": ""
```

### Comparing `spwn-1.2.3/spwn/customanalyzer.py` & `spwn-1.2.4/spwn/customanalyzer.py`

 * *Files identical despite different names*

### Comparing `spwn-1.2.3/spwn/filemanager.py` & `spwn-1.2.4/spwn/filemanager.py`

 * *Files identical despite different names*

### Comparing `spwn-1.2.3/spwn/libc.py` & `spwn-1.2.4/spwn/libc.py`

 * *Files identical despite different names*

### Comparing `spwn-1.2.3/spwn/spwn.py` & `spwn-1.2.4/spwn/spwn.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import argparse
 import os
 import shutil
 import sys
 
+sys.argv.append("NOTERM")  # HACK to prevent pwntools to messup the terminal, the added arg will be removed by pwnlib
+
 from spwn.filemanager import FileManager
 from spwn.analyzer import Analyzer
 from spwn.scripter import Scripter
 from spwn.configmanager import ConfigManager
 from spwn.customanalyzer import CustomAnalyzer
 from spwn.configgenerator import ConfigGenerator
 
@@ -166,39 +168,49 @@
 		"-nd", "--nodecomp",
 		action="store_true",
 		default=False,
 		help="Don't open the decompiler"
 	)
 
 	parser.add_argument(
-		"mode",
-		choices=["inter", "i", "ionly", "io", "nd", "nodecomp", "setup", []],
-		nargs="*",
-		help="Use these if you don't want to type '-'"
-	)
-
-	parser.add_argument(
-		"--setup",
+		"--config",
 		action="store_true",
 		default=False,
 		help="Setup configs and quit"
 	)
 
+	parser.add_argument(
+		"others",
+		nargs=argparse.REMAINDER,
+		help="You can avoid typing the hyphens and/or specify the template"
+	)
+
 	args = parser.parse_args(sys.argv[1:])
+	others = set(args.others)
 
-	args.ionly    |= any(arg in ["ionly", "io"] for arg in args.mode)
-	args.inter    |= any(arg in ["interactive", "inter", "i"] for arg in args.mode)
-	args.nodecomp |= any(arg in ["nodecomp", "nd"] for arg in args.mode)
+	possible_arguments = {
+		"ionly": "ionly",
+		"io": "ionly",
+		"interactive": "inter",
+		"inter": "inter",
+		"i": "inter",
+		"nodecomp": "nodecomp",
+		"nd": "nodecomp"
+	}
+
+	for arg in possible_arguments:
+		if arg in others:
+			setattr(args, possible_arguments[arg], True)
+			others.remove(arg)
 
-	if args.setup or "setup" in args.mode:
-		ConfigGenerator().maybe_create_config()
+	ConfigGenerator().maybe_create_config()
+	if args.config or "config" in others:
 		print("[*] Setup completed")
 	else:
-		ConfigGenerator().maybe_create_config()
-
 		global configs
-		configs = ConfigManager(CONFIG_PATH)
+		template = others.pop() if others else None
+		configs = ConfigManager(CONFIG_PATH, template)
 
 		if args.ionly:
 			Spwn(interactions_only=True)
 		else:
 			Spwn(create_interactions=args.inter, no_decompiler=args.nodecomp)
```

### Comparing `spwn-1.2.3/spwn/utils.py` & `spwn-1.2.4/spwn/utils.py`

 * *Files identical despite different names*

### Comparing `spwn-1.2.3/spwn.egg-info/PKG-INFO` & `spwn-1.2.4/spwn.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spwn
-Version: 1.2.3
+Version: 1.2.4
 Summary: Automatic tool to quickly start a pwn CTF challenge
 Home-page: https://github.com/MarcoMeinardi/spwn
 Author: Chino
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
@@ -14,15 +14,15 @@
 
 # Spwn
 
 This repository started as a translation of
 [pwninit](https://github.com/io12/pwninit). It has been created because I
 love the utilities provided by pwninit, but I'm too lazy to learn Rust and
 I wanted to customize it, so I rewrote it in python (and added
-some more features).
+~~some~~ a lot more features).
 
 ## Features
  * Auto detect files (binary, libc, loader)
  * Get loader from libc version (if missing)
  * Unstrip the libc with `pwn.libcdb.unstrip_libc`
  * Set binary and loader executable
  * Set runpath and interpreter for the debug binary
@@ -38,22 +38,23 @@
  * Launch decompiler
  * Run [cwe_checker](https://github.com/fkie-cad/cwe_checker)
  * Launch custom user-provided commands
  * Launch custom user-provided python scripts
 
 ## Usage
 ```
-spwn [-h] [-i] [-io] [-nd] [--setup] [{inter,i,ionly,io,nd,nodecomp,setup,} ...]
+spwn [-h] [-i] [-io] [-nd] [--config] [{inter,i,ionly,io,nd,nodecomp,config} ...] [template]
 
 options:
   -h, --help            show this help message and exit
   -i, --inter           Interactively create interaction functions
   -io, --ionly          Create the interaction functions, without doing any analysis
   -nd, --nodecomp       Don't open the decompiler
-  --setup               Setup configs and quit
+  --config              Setup configs and quit
+  template              template to use
 ```
 
 If the files have weird names (such as the libc name not starting with
 "libc"), the autodetection will fail and fall in the manual selection,
 the best fix for this is to rename the files.
 
 To understand how the interactions creation works, I suggest to just try
@@ -103,14 +104,27 @@
 if you want to change the location of the config file, you will have to
 edit the source code. The variable is `CONFIG_PATH` in `spwn.py`.
 Its location should be
 `~/.local/lib/python3.{python-version}/site-packages/spwn/spwn.py`.
 Note that if you reinstall or update `spwn`, this variable will be
 overwritten.
 
+### Multiple templates
+You can have multiple templates and select which one to use from command
+line. You have to place your templates in the same directory of the base
+template (`template_file`), and name it
+`{custom_template_prefix}{name}.py`. To use it, you just have to specify
+`name` in the command line (`spwn {name}`).
+
+The whole file will be treated as a format string, so, be careful to put
+double curly brackets if they don't have to be treated as format
+specifiers (`my_set = {{1, 2, 3}}`). The actual format specifiers (which
+you have to place in single curly brackets) are: `{binary}`, `{libc}`,
+`{debug_dir}` and `{interactions}`.
+
 ### Suppress warnings
 Don't show warning messages for non installed non-vital dependencies.
 
 ### Custom commands
 The pre and post analysis commands, are in the form `[command, timeout]`.
 `command` is a list of strings and should contain the `"{binary}"` or
 `"{debug_binary}"` string in order to be formatted with the correct
```

