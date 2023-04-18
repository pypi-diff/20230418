# Comparing `tmp/rolv-0.0.3.tar.gz` & `tmp/rolv-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rolv-0.0.3.tar", last modified: Sun Apr 16 21:04:34 2023, max compression
+gzip compressed data, was "rolv-0.0.4.tar", last modified: Tue Apr 18 21:04:12 2023, max compression
```

## Comparing `rolv-0.0.3.tar` & `rolv-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,46 @@
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-16 21:04:34.663756 rolv-0.0.3/
--rw-r--r--   0 dorus     (1000) dorus     (1000)      312 2023-04-16 21:04:34.663756 rolv-0.0.3/PKG-INFO
--rw-r--r--   0 dorus     (1000) dorus     (1000)      533 2023-04-16 17:44:08.000000 rolv-0.0.3/README.md
--rw-r--r--   0 dorus     (1000) dorus     (1000)      438 2023-04-16 13:26:21.000000 rolv-0.0.3/pyproject.toml
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-16 21:04:34.660423 rolv-0.0.3/rolv/
--rw-r--r--   0 dorus     (1000) dorus     (1000)     2153 2023-04-16 21:04:02.000000 rolv-0.0.3/rolv/__init__.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)      831 2023-04-16 20:17:20.000000 rolv-0.0.3/rolv/config.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1837 2023-04-16 20:16:15.000000 rolv-0.0.3/rolv/executables.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1511 2023-04-16 20:13:52.000000 rolv-0.0.3/rolv/lib.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)      840 2023-04-16 20:40:22.000000 rolv-0.0.3/rolv/package.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     3950 2023-04-16 20:13:52.000000 rolv-0.0.3/rolv/rc.py
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-16 21:04:34.660423 rolv-0.0.3/rolv/src/
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-16 21:04:34.660423 rolv-0.0.3/rolv/src/config/
--rw-r--r--   0 dorus     (1000) dorus     (1000)      371 2023-04-16 20:10:37.000000 rolv-0.0.3/rolv/src/config/default_aliases_and_functions
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-16 21:04:34.663756 rolv-0.0.3/rolv/src/executables/
--rwxr-xr-x   0 dorus     (1000) dorus     (1000)       93 2023-04-16 15:53:31.000000 rolv-0.0.3/rolv/src/executables/gitc
--rw-r--r--   0 dorus     (1000) dorus     (1000)      633 2023-04-16 20:13:04.000000 rolv-0.0.3/rolv/src/executables/readme.md
--rw-r--r--   0 dorus     (1000) dorus     (1000)        6 2023-04-16 20:19:07.000000 rolv-0.0.3/rolv/src/version
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-16 21:04:34.660423 rolv-0.0.3/rolv.egg-info/
--rw-r--r--   0 dorus     (1000) dorus     (1000)      312 2023-04-16 21:04:34.000000 rolv-0.0.3/rolv.egg-info/PKG-INFO
--rw-r--r--   0 dorus     (1000) dorus     (1000)      388 2023-04-16 21:04:34.000000 rolv-0.0.3/rolv.egg-info/SOURCES.txt
--rw-r--r--   0 dorus     (1000) dorus     (1000)        1 2023-04-16 21:04:34.000000 rolv-0.0.3/rolv.egg-info/dependency_links.txt
--rw-r--r--   0 dorus     (1000) dorus     (1000)      130 2023-04-16 21:04:34.000000 rolv-0.0.3/rolv.egg-info/entry_points.txt
--rw-r--r--   0 dorus     (1000) dorus     (1000)        5 2023-04-16 21:04:34.000000 rolv-0.0.3/rolv.egg-info/top_level.txt
--rw-r--r--   0 dorus     (1000) dorus     (1000)      613 2023-04-16 21:04:34.663756 rolv-0.0.3/setup.cfg
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.545524 rolv-0.0.4/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      312 2023-04-18 21:04:12.545524 rolv-0.0.4/PKG-INFO
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      533 2023-04-16 17:44:08.000000 rolv-0.0.4/README.md
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      438 2023-04-16 13:26:21.000000 rolv-0.0.4/pyproject.toml
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.528858 rolv-0.0.4/rolv/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     2197 2023-04-17 19:05:10.000000 rolv-0.0.4/rolv/__init__.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1245 2023-04-17 19:05:10.000000 rolv-0.0.4/rolv/apps.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      835 2023-04-17 19:05:10.000000 rolv-0.0.4/rolv/config.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      514 2023-04-17 19:05:10.000000 rolv-0.0.4/rolv/disk.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1841 2023-04-17 18:49:09.000000 rolv-0.0.4/rolv/executables.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1523 2023-04-17 19:05:28.000000 rolv-0.0.4/rolv/lib.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      842 2023-04-17 19:05:10.000000 rolv-0.0.4/rolv/package.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     4034 2023-04-17 19:02:32.000000 rolv-0.0.4/rolv/rc.py
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.528858 rolv-0.0.4/rolv/src/
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.522191 rolv-0.0.4/rolv/src/apps/
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.522191 rolv-0.0.4/rolv/src/apps/fzf/
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.538858 rolv-0.0.4/rolv/src/apps/fzf/bin/
+-rwxr-xr-x   0 dorus     (1000) dorus     (1000)  3252224 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/bin/fzf
+-rwxr-xr-x   0 dorus     (1000) dorus     (1000)     6274 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/bin/fzf-tmux
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.538858 rolv-0.0.4/rolv/src/apps/fzf/doc/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    21990 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/doc/fzf.txt
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.522191 rolv-0.0.4/rolv/src/apps/fzf/man/
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.538858 rolv-0.0.4/rolv/src/apps/fzf/man/man1/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1992 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/man/man1/fzf-tmux.1
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    40623 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/man/man1/fzf.1
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.542191 rolv-0.0.4/rolv/src/apps/fzf/plugin/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    31836 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/plugin/fzf.vim
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.542191 rolv-0.0.4/rolv/src/apps/fzf/shell/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    10214 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/shell/completion.bash
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    10650 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/shell/completion.zsh
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     3936 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/shell/key-bindings.bash
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     5727 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/shell/key-bindings.fish
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     3934 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/shell/key-bindings.zsh
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.545524 rolv-0.0.4/rolv/src/config/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     2292 2023-04-18 08:36:32.000000 rolv-0.0.4/rolv/src/config/default_aliases_and_functions
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.545524 rolv-0.0.4/rolv/src/executables/
+-rwxr-xr-x   0 dorus     (1000) dorus     (1000)       93 2023-04-16 15:53:31.000000 rolv-0.0.4/rolv/src/executables/gitc
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      633 2023-04-16 20:13:04.000000 rolv-0.0.4/rolv/src/executables/readme.md
+-rw-r--r--   0 dorus     (1000) dorus     (1000)       38 2023-04-18 21:04:06.000000 rolv-0.0.4/rolv/src/version
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.528858 rolv-0.0.4/rolv.egg-info/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      312 2023-04-18 21:04:12.000000 rolv-0.0.4/rolv.egg-info/PKG-INFO
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      809 2023-04-18 21:04:12.000000 rolv-0.0.4/rolv.egg-info/SOURCES.txt
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        1 2023-04-18 21:04:12.000000 rolv-0.0.4/rolv.egg-info/dependency_links.txt
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      130 2023-04-18 21:04:12.000000 rolv-0.0.4/rolv.egg-info/entry_points.txt
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        5 2023-04-18 21:04:12.000000 rolv-0.0.4/rolv.egg-info/top_level.txt
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      613 2023-04-18 21:04:12.545524 rolv-0.0.4/setup.cfg
```

### Comparing `rolv-0.0.3/README.md` & `rolv-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rolv-0.0.3/rolv/__init__.py` & `rolv-0.0.4/rolv/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from . import rc, executables, package
 
 
 def help_text():
-
-    print(f"""
+    print(
+        f"""
                   dP          
                   88          
 88d888b. .d8888b. 88 dP   .dP 
 88'  `88 88'  `88 88 88   d8' 
 88       88.  .88 88 88 .88'  
 dP       `88888P' dP 8888P'   v{package.get_version()}            
-""")
-    print("\"\"\"A simple tool to synchronize all my \nquality of life scripts between servers.\"\"\"\n")
+"""
+    )
+    print('"""A simple tool to synchronize all my \nquality of life scripts between servers."""\n')
     print("rolv.install    - install/update executables, aliases, etc")
     print("rolv.version    - get version of package")
     print("rolv.disclaimer - get a short list of things you need to know before using this package")
     print("\n")
 
+
 def disclaimer():
-    print("""
+    print(
+        """
 8888888b.  d8b                   888          d8b                                         
 888  "Y88b Y8P                   888          Y8P                                         
 888    888                       888                                                      
 888    888 888 .d8888b   .d8888b 888  8888b.  888 88888b.d88b.   .d88b.  888d888 .d8888b  
 888    888 888 88K      d88P"    888     "88b 888 888 "888 "88b d8P  Y8b 888P"   88K      
 888    888 888 "Y8888b. 888      888 .d888888 888 888  888  888 88888888 888     "Y8888b. 
 888  .d88P 888      X88 Y88b.    888 888  888 888 888  888  888 Y8b.     888          X88 
@@ -30,23 +33,26 @@
 
 This package is written by me, for me. Best not to use this package at all if you are not me.
 
 Will add/update the  ` # <rolv config> ... # </rolv config> `  block in any rc it can find.
   * Unless the ROLV_RC_FILE_PATH environment variable is set.
   
 Will delete any file under  ` $HOME/.local/bin `  that starts with  ` __rolv_ `  .   
-    """)
+    """
+    )
+
 
 def version():
     print(package.get_version())
 
 
 def install():
     print("\n")
     rc.set_rc_files()
     executables.sync_executables()
+    apps.sync_apps()
 
     print("\nTo make sure the ENV is up to date, be sure to open a new terminal window, or run (one of) the following command(s):")
     for path in rc.get_rc_file_paths():
         print(f"  source {path.as_posix()}")
     print("\nDone.")
     print("\n")
```

### Comparing `rolv-0.0.3/rolv/config.py` & `rolv-0.0.4/rolv/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .lib import insert, trim_newlines
 
 
 # Module methods
 # ====================================================================
 
 
-def get_rc_config():
+def get_rc_config(path):
     """provide config to be put in the rc files. Called by rc.compile_config_block()"""
     src_dir = Path(package.get_src_path())
 
     block = ""
 
     for path in ["config/default_aliases_and_functions"]:
         abs_path = src_dir.joinpath(path)
```

### Comparing `rolv-0.0.3/rolv/executables.py` & `rolv-0.0.4/rolv/executables.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from . import package
 
 
 # Module methods
 # ====================================================================
 
 
-def get_rc_config():
+def get_rc_config(path):
     """provide config to be put in the rc files. Called by rc.compile_config_block()"""
     lines = ["# -- Executables"]
     for executable in get_executable_paths():
         name = executable.stem
         lines.append(f'alias {name}="__rolv_{name}"')
 
     return "\n".join(lines)
```

### Comparing `rolv-0.0.3/rolv/lib.py` & `rolv-0.0.4/rolv/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
     General helper functions
 """
 
+import os
+
 
 def insert(text, space=1):
     """Tests if last char is newline, and if not, will add the newline"""
     # make sure that the text at least ends on a new line
     if len(text) == 0 or text[-1] != "\n":
         text = text + "\n"
 
@@ -53,7 +55,8 @@
     return "\n".join(lines)
 
 
 def trim_newlines(text_or_lines):
     text_or_lines = trim_preceeding_newlines(text_or_lines)
     text_or_lines = trim_trailing_newlines(text_or_lines)
     return text_or_lines
+
```

### Comparing `rolv-0.0.3/rolv/package.py` & `rolv-0.0.4/rolv/package.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 """
 
 import os
 from pathlib import Path
 from functools import cache
 import importlib.util
 
+
 def get_version():
-    with open(get_path("version"), 'r') as f:
+    with open(get_path("version"), "r") as f:
         return f.read()
 
+
 def get_src_path():
     path = importlib.util.find_spec("rolv.src").submodule_search_locations[0]
     return Path(path).resolve().as_posix()
 
 
 @cache
 def get_path(resource):
```

### Comparing `rolv-0.0.3/rolv/rc.py` & `rolv-0.0.4/rolv/rc.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,18 @@
     It does not determine the config to be added itself, for that it calls get_rc_config() methods of other modules.
 """
 
 import os
 import re
 from pathlib import Path
 
-from . import executables, config
+from . import executables, config, apps
 from .lib import insert, trim_trailing_newlines
 
 
-def compose_config():
-    """Called to compose new config to be put in the bashrc. Lacks the fencing, just the config.
-    If you want to read the current config block, see get_config_block()"""
-
-    block = ""
-    block += config.get_rc_config()
-    block += executables.get_rc_config()
-
-    return block
-
-
 def get_rc_file_paths():
     """Finds rc file paths if they exist in the default location, unless ROLV_RC_FILE_PATH is set, then it will only return that value."""
     # use single, configured path
     explicit_path = os.getenv("ROLV_RC_FILE_PATH")
     if explicit_path is not None:
         explicit_path = Path(explicit_path).resolve()
         if explicit_path.exists() == False:
@@ -44,14 +33,26 @@
 
 def set_rc_files():
     """Adds/updates the config block to rc file paths."""
     for abs_path in get_rc_file_paths():
         set_rc_file(abs_path)
 
 
+def compose_config(path):
+    """Called to compose new config to be put in the bashrc. Lacks the fencing, just the config.
+    If you want to read the current config block, see get_config_block()"""
+
+    block = ""
+    block += insert(config.get_rc_config(path))
+    block += insert(executables.get_rc_config(path))
+    block += insert(apps.get_rc_config(path))
+
+    return block
+
+
 def set_rc_file(path):
     """Updates/Places the rolv config block in the given rc file"""
     if path.exists() is False:
         print(f"File {path.as_posix()} not found. Aborting.")
         exit(0)
 
     rolv_block, other = get_config_block(path)
@@ -64,15 +65,15 @@
 
     # do nice spacing
     lines = [x.strip() for x in contents.split("\n")]
     if contents[-1] != "":
         contents += "\n"
 
     contents += "\n# <rolv config>\n# =======================================================\n"
-    contents += insert(compose_config(), space=0)
+    contents += insert(compose_config(path), space=0)
     contents += "# =======================================================\n# </rolv config>\n"
 
     with open(path, "w") as f:
         f.write(contents)
 
 
 def remove_bashrc_block(path):
```

### Comparing `rolv-0.0.3/rolv/src/executables/readme.md` & `rolv-0.0.4/rolv/src/executables/readme.md`

 * *Files identical despite different names*

### Comparing `rolv-0.0.3/setup.cfg` & `rolv-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rolv
-version = 0.0.3
+version = 0.0.4
 summary = Package to quickly set up linux terminal environment.
 home_page = https://github.com/dwrolvink/rolv
 author = https://github.com/dwrolvink
 author_email = dwrolvink@protonmail.com
 license = GNU General Public License v3 or later (GPLv3+)
 
 [options]
```

