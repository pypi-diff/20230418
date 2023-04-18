# Comparing `tmp/bmgen-2023.4.0b2.tar.gz` & `tmp/bmgen-2023.4.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmgen-2023.4.0b2.tar", last modified: Tue Apr 18 05:23:05 2023, max compression
+gzip compressed data, was "bmgen-2023.4.0b3.tar", last modified: Tue Apr 18 17:39:56 2023, max compression
```

## Comparing `bmgen-2023.4.0b2.tar` & `bmgen-2023.4.0b3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ever      (1000) ever      (1000)        0 2023-04-18 05:23:05.716219 bmgen-2023.4.0b2/
--rw-rw-r--   0 ever      (1000) ever      (1000)    15830 2023-04-17 17:28:00.000000 bmgen-2023.4.0b2/LICENSE
--rw-rw-r--   0 ever      (1000) ever      (1000)     2013 2023-04-18 05:23:05.716219 bmgen-2023.4.0b2/PKG-INFO
--rw-r--r--   0 ever      (1000) ever      (1000)     1675 2023-04-17 17:30:23.000000 bmgen-2023.4.0b2/README.md
-drwxrwxr-x   0 ever      (1000) ever      (1000)        0 2023-04-18 05:23:05.716219 bmgen-2023.4.0b2/bmgen/
--rw-r--r--   0 ever      (1000) ever      (1000)     4965 2023-04-17 17:23:15.000000 bmgen-2023.4.0b2/bmgen/__main__.py
--rw-rw-r--   0 ever      (1000) ever      (1000)       28 2023-04-18 05:19:41.000000 bmgen-2023.4.0b2/bmgen/info.py
-drwxrwxr-x   0 ever      (1000) ever      (1000)        0 2023-04-18 05:23:05.716219 bmgen-2023.4.0b2/bmgen.egg-info/
--rw-r--r--   0 ever      (1000) ever      (1000)     2013 2023-04-18 05:23:05.000000 bmgen-2023.4.0b2/bmgen.egg-info/PKG-INFO
--rw-r--r--   0 ever      (1000) ever      (1000)      234 2023-04-18 05:23:05.000000 bmgen-2023.4.0b2/bmgen.egg-info/SOURCES.txt
--rw-r--r--   0 ever      (1000) ever      (1000)        1 2023-04-18 05:23:05.000000 bmgen-2023.4.0b2/bmgen.egg-info/dependency_links.txt
--rw-r--r--   0 ever      (1000) ever      (1000)       46 2023-04-18 05:23:05.000000 bmgen-2023.4.0b2/bmgen.egg-info/entry_points.txt
--rw-r--r--   0 ever      (1000) ever      (1000)        9 2023-04-18 05:23:05.000000 bmgen-2023.4.0b2/bmgen.egg-info/requires.txt
--rw-r--r--   0 ever      (1000) ever      (1000)        1 2023-04-18 05:23:05.000000 bmgen-2023.4.0b2/bmgen.egg-info/top_level.txt
--rw-rw-r--   0 ever      (1000) ever      (1000)       38 2023-04-18 05:23:05.716219 bmgen-2023.4.0b2/setup.cfg
--rw-r--r--   0 ever      (1000) ever      (1000)      748 2023-04-17 17:23:18.000000 bmgen-2023.4.0b2/setup.py
+drwxrwxr-x   0 ever      (1000) ever      (1000)        0 2023-04-18 17:39:56.830132 bmgen-2023.4.0b3/
+-rw-rw-r--   0 ever      (1000) ever      (1000)    15830 2023-04-17 17:28:00.000000 bmgen-2023.4.0b3/LICENSE
+-rw-rw-r--   0 ever      (1000) ever      (1000)     2427 2023-04-18 17:39:56.830132 bmgen-2023.4.0b3/PKG-INFO
+-rw-r--r--   0 ever      (1000) ever      (1000)     2089 2023-04-18 17:26:41.000000 bmgen-2023.4.0b3/README.md
+drwxrwxr-x   0 ever      (1000) ever      (1000)        0 2023-04-18 17:39:56.826132 bmgen-2023.4.0b3/bmgen/
+-rw-rw-r--   0 ever      (1000) ever      (1000)     5387 2023-04-18 17:32:45.000000 bmgen-2023.4.0b3/bmgen/__main__.py
+-rw-rw-r--   0 ever      (1000) ever      (1000)       28 2023-04-18 17:38:08.000000 bmgen-2023.4.0b3/bmgen/info.py
+drwxrwxr-x   0 ever      (1000) ever      (1000)        0 2023-04-18 17:39:56.830132 bmgen-2023.4.0b3/bmgen.egg-info/
+-rw-r--r--   0 ever      (1000) ever      (1000)     2427 2023-04-18 17:39:56.000000 bmgen-2023.4.0b3/bmgen.egg-info/PKG-INFO
+-rw-r--r--   0 ever      (1000) ever      (1000)      234 2023-04-18 17:39:56.000000 bmgen-2023.4.0b3/bmgen.egg-info/SOURCES.txt
+-rw-r--r--   0 ever      (1000) ever      (1000)        1 2023-04-18 17:39:56.000000 bmgen-2023.4.0b3/bmgen.egg-info/dependency_links.txt
+-rw-r--r--   0 ever      (1000) ever      (1000)       46 2023-04-18 17:39:56.000000 bmgen-2023.4.0b3/bmgen.egg-info/entry_points.txt
+-rw-r--r--   0 ever      (1000) ever      (1000)        9 2023-04-18 17:39:56.000000 bmgen-2023.4.0b3/bmgen.egg-info/requires.txt
+-rw-r--r--   0 ever      (1000) ever      (1000)        1 2023-04-18 17:39:56.000000 bmgen-2023.4.0b3/bmgen.egg-info/top_level.txt
+-rw-rw-r--   0 ever      (1000) ever      (1000)       38 2023-04-18 17:39:56.830132 bmgen-2023.4.0b3/setup.cfg
+-rw-r--r--   0 ever      (1000) ever      (1000)      748 2023-04-17 17:23:18.000000 bmgen-2023.4.0b3/setup.py
```

### Comparing `bmgen-2023.4.0b2/LICENSE` & `bmgen-2023.4.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `bmgen-2023.4.0b2/PKG-INFO` & `bmgen-2023.4.0b3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmgen
-Version: 2023.4.0b2
+Version: 2023.4.0b3
 Summary: Broken Mouse Studios' build solution
 Home-page: https://git.brokenmouse.studio/bms/bmgen
 Author: bms
 Author-email: bmgen@brokenmouse.studio
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -28,39 +28,56 @@
 
 ## Installation
 - Install bmgen via `pip install bmgen` or `python3 -m pip install bmgen`
 
 ## Building a simple C project
 This example shows a script which builds two files named `main.c` and `game.c` into a binary named `mygame` with `SDL2`.
 
+The directory structure created by bmgen will look like this:
+```
+- bin/
+  - dbg/
+    - obj/
+      - main.o
+      - game.o
+    - mygame
+```
+
 The following is a breakdown of the script.
 
 1. First import the `clang` command:
 ```python
 from bmgen.commands.clang import clang
 ```
-2. Then set the output directory -- which will also instantly get created -- and tell the `clang` command to create it's object directory inside the output directory:
+2. Then set the base output directory and tell bmgen to create the base, variant and the `clang` command's object directory:
 ```python
-inst.set_output_dir('bin')
+inst.base_output_dir = 'bin'
+inst.update_output_dir()
 clang.update_object_dir()
 ```
 3. Build the program via `clang`:
 ```python
 clang('mygame', ['main.c', 'game.c'], ['sdl2'])
 ```
 
 The final `bmgen.py` looks like this:
 ```python
 from bmgen.commands.clang import clang
 
-inst.set_output_dir('bin')
+inst.base_output_dir = 'bin'
+inst.update_output_dir()
 clang.update_object_dir()
 
 clang('mygame', ['main.c', 'game.c'], ['sdl2'])
 ```
 
 Building the program is now as easy as running `bmgen` in your terminal!
 
 ## License
+© Broken Mouse Studios 2023<br>
+https://brokenmouse.studio
+
 This software and it's accompanying files are licensed under the *Mozilla Public License Version 2.0*.
 
 For the license's contents, see [LICENSE](LICENSE) or go to https://mozilla.org/MPL/2.0/.
+
+By submitting patches or merge/pull requests, you grant Broken Mouse Studios the permission to use, copy, modify, distribute, publish and/or relicense the contributions you have made to the project.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bmgen-2023.4.0b2/README.md` & `bmgen-2023.4.0b3/bmgen.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: bmgen
+Version: 2023.4.0b3
+Summary: Broken Mouse Studios' build solution
+Home-page: https://git.brokenmouse.studio/bms/bmgen
+Author: bms
+Author-email: bmgen@brokenmouse.studio
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # bmgen - Broken Mouse Studios' build solution
 
 ## DISCLAIMER
 This project is currently in it's beta phase!
 
 It needs to be cleaned up and does not yet have it's full set of features. You may quickly hit it's limits.
 
@@ -16,39 +28,56 @@
 
 ## Installation
 - Install bmgen via `pip install bmgen` or `python3 -m pip install bmgen`
 
 ## Building a simple C project
 This example shows a script which builds two files named `main.c` and `game.c` into a binary named `mygame` with `SDL2`.
 
+The directory structure created by bmgen will look like this:
+```
+- bin/
+  - dbg/
+    - obj/
+      - main.o
+      - game.o
+    - mygame
+```
+
 The following is a breakdown of the script.
 
 1. First import the `clang` command:
 ```python
 from bmgen.commands.clang import clang
 ```
-2. Then set the output directory -- which will also instantly get created -- and tell the `clang` command to create it's object directory inside the output directory:
+2. Then set the base output directory and tell bmgen to create the base, variant and the `clang` command's object directory:
 ```python
-inst.set_output_dir('bin')
+inst.base_output_dir = 'bin'
+inst.update_output_dir()
 clang.update_object_dir()
 ```
 3. Build the program via `clang`:
 ```python
 clang('mygame', ['main.c', 'game.c'], ['sdl2'])
 ```
 
 The final `bmgen.py` looks like this:
 ```python
 from bmgen.commands.clang import clang
 
-inst.set_output_dir('bin')
+inst.base_output_dir = 'bin'
+inst.update_output_dir()
 clang.update_object_dir()
 
 clang('mygame', ['main.c', 'game.c'], ['sdl2'])
 ```
 
 Building the program is now as easy as running `bmgen` in your terminal!
 
 ## License
+© Broken Mouse Studios 2023<br>
+https://brokenmouse.studio
+
 This software and it's accompanying files are licensed under the *Mozilla Public License Version 2.0*.
 
 For the license's contents, see [LICENSE](LICENSE) or go to https://mozilla.org/MPL/2.0/.
+
+By submitting patches or merge/pull requests, you grant Broken Mouse Studios the permission to use, copy, modify, distribute, publish and/or relicense the contributions you have made to the project.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bmgen-2023.4.0b2/bmgen/__main__.py` & `bmgen-2023.4.0b3/bmgen/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,39 +29,46 @@
     def get_printable_command(args: List[str], prefix: str | None=None) -> str:
         printable_args = []
         for arg in args:
             quote = '\'' if ' ' in arg else ''
             printable_args.append(quote + arg.translate(bmgen.ESCAPE_MAP) + quote)
         return (f'{colorama.Fore.YELLOW}{colorama.Style.BRIGHT}[{prefix}]{colorama.Style.NORMAL} ' if prefix else '') + colorama.Fore.BLUE + ' '.join(printable_args) + colorama.Fore.RESET
     
-    def __init__(self, rebuild: bool):
+    def __init__(self, args: any):
+        self.base_output_dir = '.'
         self.command_id = 0
         self.failed_command_num = 0
         self.output_dir = ''
-        self.rebuild = rebuild
+        self.rebuild = args.rebuild
+        self.release_mode = args.release
+        self.variant_dir = None
     
     def print_error(self, msg: str, prefix: str='ERROR') -> None:
         print(f'{colorama.Fore.RED}{colorama.Style.BRIGHT}[{prefix}]{colorama.Style.NORMAL} {msg}{colorama.Fore.RESET}', file=sys.stderr)
     
     def abort(self, msg: str) -> None:
         self.print_error(msg, prefix='BUILD FAILED')
         self.print_error(f'{self.failed_command_num} command{"" if self.failed_command_num == 1 else "s"} failed')
         sys.exit(1)
     
-    def set_output_dir(self, new: str) -> None:
+    def skip_file(self, source_path: str, output_path: str) -> bool:
+        return os.path.exists(output_path) and os.path.getmtime(source_path) < os.path.getmtime(output_path)
+    
+    def update_output_dir(self) -> None:
+        base = self.base_output_dir
+        variant_dir = self.variant_dir if self.variant_dir else 'release' if self.release_mode else 'dbg'
+        new = os.path.join(base, variant_dir)
         self.output_dir = new
         
-        if os.path.islink(new):
-            if not os.path.exists(new):
-                os.makedirs(Path(new).resolve())
+        if os.path.islink(base):
+            if not os.path.exists(base):
+                os.makedirs(os.path.join(Path(base).resolve(), variant_dir), exist_ok=True)
         else:
-            os.symlink(tempfile.mkdtemp(prefix='bmgen-'), new)
-    
-    def skip_file(self, source_path: str, output_path: str) -> bool:
-        return os.path.exists(output_path) and os.path.getmtime(source_path) < os.path.getmtime(output_path)
+            os.symlink(tempfile.mkdtemp(prefix='bmgen-'), base)
+        os.makedirs(new, exist_ok=True)
     
     def start_command(self, title: str) -> None:
         print(f'{colorama.Fore.MAGENTA}{colorama.Style.BRIGHT}[{self.command_id}]{colorama.Style.NORMAL} {title}{colorama.Fore.RESET}')
     
     def command_error(self, msg: str, mandatory: bool) -> None:
         self.failed_command_num += 1
         self.print_error(msg)
@@ -91,14 +98,15 @@
 
 def main() -> None:
     ap = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     ap.add_argument('--version', action='store_true', help='print version and exit')
     ap.add_argument('-d', '--directory', default='.', help='specify the working directory')
     ap.add_argument('-s', '--script', default='bmgen.py', help="path of the build script to execute")
     ap.add_argument('-r', '--rebuild', action='store_true', help="force the execution of all commands")
+    ap.add_argument('-R', '--release', action='store_true', help='build in release-mode')
     args = ap.parse_args()
     
     if args.version:
         print('bmgen v' + VERSION)
         return
     
     os.chdir(args.directory)
@@ -106,18 +114,17 @@
     if not os.path.exists(args.script):
         print(f'Script "{args.script}" does not exist!', file=sys.stderr)
         sys.exit(1)
     
     with open(args.script, 'r') as f:
         script_code = f.read()
     
-    # TODO debug and release builds
     # TODO separate the code for modifying builtins
     start_time = time.time()
-    inst = bmgen(args.rebuild)
+    inst = bmgen(args)
     exec('import builtins\nbuiltins.bmgen = _bmgen\nbuiltins.inst = _inst\ndel _bmgen\ndel _inst\n' + script_code, {}, {'_bmgen': bmgen, '_inst': inst})
     
     if inst.command_id > 0:
         print()
     
     print(f'{colorama.Fore.GREEN}{colorama.Style.BRIGHT}Build finished after {"%.3f"%(time.time() - start_time)} seconds')
     if inst.failed_command_num > 0:
```

### Comparing `bmgen-2023.4.0b2/bmgen.egg-info/PKG-INFO` & `bmgen-2023.4.0b3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: bmgen
-Version: 2023.4.0b2
-Summary: Broken Mouse Studios' build solution
-Home-page: https://git.brokenmouse.studio/bms/bmgen
-Author: bms
-Author-email: bmgen@brokenmouse.studio
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # bmgen - Broken Mouse Studios' build solution
 
 ## DISCLAIMER
 This project is currently in it's beta phase!
 
 It needs to be cleaned up and does not yet have it's full set of features. You may quickly hit it's limits.
 
@@ -28,39 +16,56 @@
 
 ## Installation
 - Install bmgen via `pip install bmgen` or `python3 -m pip install bmgen`
 
 ## Building a simple C project
 This example shows a script which builds two files named `main.c` and `game.c` into a binary named `mygame` with `SDL2`.
 
+The directory structure created by bmgen will look like this:
+```
+- bin/
+  - dbg/
+    - obj/
+      - main.o
+      - game.o
+    - mygame
+```
+
 The following is a breakdown of the script.
 
 1. First import the `clang` command:
 ```python
 from bmgen.commands.clang import clang
 ```
-2. Then set the output directory -- which will also instantly get created -- and tell the `clang` command to create it's object directory inside the output directory:
+2. Then set the base output directory and tell bmgen to create the base, variant and the `clang` command's object directory:
 ```python
-inst.set_output_dir('bin')
+inst.base_output_dir = 'bin'
+inst.update_output_dir()
 clang.update_object_dir()
 ```
 3. Build the program via `clang`:
 ```python
 clang('mygame', ['main.c', 'game.c'], ['sdl2'])
 ```
 
 The final `bmgen.py` looks like this:
 ```python
 from bmgen.commands.clang import clang
 
-inst.set_output_dir('bin')
+inst.base_output_dir = 'bin'
+inst.update_output_dir()
 clang.update_object_dir()
 
 clang('mygame', ['main.c', 'game.c'], ['sdl2'])
 ```
 
 Building the program is now as easy as running `bmgen` in your terminal!
 
 ## License
+© Broken Mouse Studios 2023<br>
+https://brokenmouse.studio
+
 This software and it's accompanying files are licensed under the *Mozilla Public License Version 2.0*.
 
 For the license's contents, see [LICENSE](LICENSE) or go to https://mozilla.org/MPL/2.0/.
+
+By submitting patches or merge/pull requests, you grant Broken Mouse Studios the permission to use, copy, modify, distribute, publish and/or relicense the contributions you have made to the project.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bmgen-2023.4.0b2/setup.py` & `bmgen-2023.4.0b3/setup.py`

 * *Files identical despite different names*

