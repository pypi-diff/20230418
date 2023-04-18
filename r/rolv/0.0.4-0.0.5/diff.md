# Comparing `tmp/rolv-0.0.4.tar.gz` & `tmp/rolv-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rolv-0.0.4.tar", last modified: Tue Apr 18 21:04:12 2023, max compression
+gzip compressed data, was "rolv-0.0.5.tar", last modified: Tue Apr 18 21:16:35 2023, max compression
```

## Comparing `rolv-0.0.4.tar` & `rolv-0.0.5.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.545524 rolv-0.0.4/
--rw-r--r--   0 dorus     (1000) dorus     (1000)      312 2023-04-18 21:04:12.545524 rolv-0.0.4/PKG-INFO
--rw-r--r--   0 dorus     (1000) dorus     (1000)      533 2023-04-16 17:44:08.000000 rolv-0.0.4/README.md
--rw-r--r--   0 dorus     (1000) dorus     (1000)      438 2023-04-16 13:26:21.000000 rolv-0.0.4/pyproject.toml
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.528858 rolv-0.0.4/rolv/
--rw-r--r--   0 dorus     (1000) dorus     (1000)     2197 2023-04-17 19:05:10.000000 rolv-0.0.4/rolv/__init__.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1245 2023-04-17 19:05:10.000000 rolv-0.0.4/rolv/apps.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)      835 2023-04-17 19:05:10.000000 rolv-0.0.4/rolv/config.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)      514 2023-04-17 19:05:10.000000 rolv-0.0.4/rolv/disk.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1841 2023-04-17 18:49:09.000000 rolv-0.0.4/rolv/executables.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1523 2023-04-17 19:05:28.000000 rolv-0.0.4/rolv/lib.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)      842 2023-04-17 19:05:10.000000 rolv-0.0.4/rolv/package.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     4034 2023-04-17 19:02:32.000000 rolv-0.0.4/rolv/rc.py
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.528858 rolv-0.0.4/rolv/src/
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.522191 rolv-0.0.4/rolv/src/apps/
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.522191 rolv-0.0.4/rolv/src/apps/fzf/
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.538858 rolv-0.0.4/rolv/src/apps/fzf/bin/
--rwxr-xr-x   0 dorus     (1000) dorus     (1000)  3252224 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/bin/fzf
--rwxr-xr-x   0 dorus     (1000) dorus     (1000)     6274 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/bin/fzf-tmux
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.538858 rolv-0.0.4/rolv/src/apps/fzf/doc/
--rw-r--r--   0 dorus     (1000) dorus     (1000)    21990 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/doc/fzf.txt
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.522191 rolv-0.0.4/rolv/src/apps/fzf/man/
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.538858 rolv-0.0.4/rolv/src/apps/fzf/man/man1/
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1992 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/man/man1/fzf-tmux.1
--rw-r--r--   0 dorus     (1000) dorus     (1000)    40623 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/man/man1/fzf.1
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.542191 rolv-0.0.4/rolv/src/apps/fzf/plugin/
--rw-r--r--   0 dorus     (1000) dorus     (1000)    31836 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/plugin/fzf.vim
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.542191 rolv-0.0.4/rolv/src/apps/fzf/shell/
--rw-r--r--   0 dorus     (1000) dorus     (1000)    10214 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/shell/completion.bash
--rw-r--r--   0 dorus     (1000) dorus     (1000)    10650 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/shell/completion.zsh
--rw-r--r--   0 dorus     (1000) dorus     (1000)     3936 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/shell/key-bindings.bash
--rw-r--r--   0 dorus     (1000) dorus     (1000)     5727 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/shell/key-bindings.fish
--rw-r--r--   0 dorus     (1000) dorus     (1000)     3934 2023-04-17 18:37:11.000000 rolv-0.0.4/rolv/src/apps/fzf/shell/key-bindings.zsh
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.545524 rolv-0.0.4/rolv/src/config/
--rw-r--r--   0 dorus     (1000) dorus     (1000)     2292 2023-04-18 08:36:32.000000 rolv-0.0.4/rolv/src/config/default_aliases_and_functions
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.545524 rolv-0.0.4/rolv/src/executables/
--rwxr-xr-x   0 dorus     (1000) dorus     (1000)       93 2023-04-16 15:53:31.000000 rolv-0.0.4/rolv/src/executables/gitc
--rw-r--r--   0 dorus     (1000) dorus     (1000)      633 2023-04-16 20:13:04.000000 rolv-0.0.4/rolv/src/executables/readme.md
--rw-r--r--   0 dorus     (1000) dorus     (1000)       38 2023-04-18 21:04:06.000000 rolv-0.0.4/rolv/src/version
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:04:12.528858 rolv-0.0.4/rolv.egg-info/
--rw-r--r--   0 dorus     (1000) dorus     (1000)      312 2023-04-18 21:04:12.000000 rolv-0.0.4/rolv.egg-info/PKG-INFO
--rw-r--r--   0 dorus     (1000) dorus     (1000)      809 2023-04-18 21:04:12.000000 rolv-0.0.4/rolv.egg-info/SOURCES.txt
--rw-r--r--   0 dorus     (1000) dorus     (1000)        1 2023-04-18 21:04:12.000000 rolv-0.0.4/rolv.egg-info/dependency_links.txt
--rw-r--r--   0 dorus     (1000) dorus     (1000)      130 2023-04-18 21:04:12.000000 rolv-0.0.4/rolv.egg-info/entry_points.txt
--rw-r--r--   0 dorus     (1000) dorus     (1000)        5 2023-04-18 21:04:12.000000 rolv-0.0.4/rolv.egg-info/top_level.txt
--rw-r--r--   0 dorus     (1000) dorus     (1000)      613 2023-04-18 21:04:12.545524 rolv-0.0.4/setup.cfg
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:16:35.885530 rolv-0.0.5/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      312 2023-04-18 21:16:35.885530 rolv-0.0.5/PKG-INFO
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      533 2023-04-16 17:44:08.000000 rolv-0.0.5/README.md
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      438 2023-04-16 13:26:21.000000 rolv-0.0.5/pyproject.toml
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:16:35.875530 rolv-0.0.5/rolv/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     2197 2023-04-17 19:05:10.000000 rolv-0.0.5/rolv/__init__.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1245 2023-04-17 19:05:10.000000 rolv-0.0.5/rolv/apps.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      835 2023-04-17 19:05:10.000000 rolv-0.0.5/rolv/config.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      514 2023-04-17 19:05:10.000000 rolv-0.0.5/rolv/disk.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1841 2023-04-17 18:49:09.000000 rolv-0.0.5/rolv/executables.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1523 2023-04-17 19:05:28.000000 rolv-0.0.5/rolv/lib.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      842 2023-04-17 19:05:10.000000 rolv-0.0.5/rolv/package.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     4034 2023-04-17 19:02:32.000000 rolv-0.0.5/rolv/rc.py
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:16:35.875530 rolv-0.0.5/rolv/src/
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:16:35.872197 rolv-0.0.5/rolv/src/apps/
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:16:35.878864 rolv-0.0.5/rolv/src/apps/fzf/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      374 2023-04-17 18:55:44.000000 rolv-0.0.5/rolv/src/apps/fzf/.fzf.bash
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      317 2023-04-17 18:55:40.000000 rolv-0.0.5/rolv/src/apps/fzf/.fzf.zsh
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:16:35.882197 rolv-0.0.5/rolv/src/apps/fzf/bin/
+-rwxr-xr-x   0 dorus     (1000) dorus     (1000)  3252224 2023-04-17 18:37:11.000000 rolv-0.0.5/rolv/src/apps/fzf/bin/fzf
+-rwxr-xr-x   0 dorus     (1000) dorus     (1000)     6274 2023-04-17 18:37:11.000000 rolv-0.0.5/rolv/src/apps/fzf/bin/fzf-tmux
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:16:35.882197 rolv-0.0.5/rolv/src/apps/fzf/doc/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    21990 2023-04-17 18:37:11.000000 rolv-0.0.5/rolv/src/apps/fzf/doc/fzf.txt
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:16:35.872197 rolv-0.0.5/rolv/src/apps/fzf/man/
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:16:35.882197 rolv-0.0.5/rolv/src/apps/fzf/man/man1/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1992 2023-04-17 18:37:11.000000 rolv-0.0.5/rolv/src/apps/fzf/man/man1/fzf-tmux.1
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    40623 2023-04-17 18:37:11.000000 rolv-0.0.5/rolv/src/apps/fzf/man/man1/fzf.1
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:16:35.885530 rolv-0.0.5/rolv/src/apps/fzf/plugin/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    31836 2023-04-17 18:37:11.000000 rolv-0.0.5/rolv/src/apps/fzf/plugin/fzf.vim
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:16:35.885530 rolv-0.0.5/rolv/src/apps/fzf/shell/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    10214 2023-04-17 18:37:11.000000 rolv-0.0.5/rolv/src/apps/fzf/shell/completion.bash
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    10650 2023-04-17 18:37:11.000000 rolv-0.0.5/rolv/src/apps/fzf/shell/completion.zsh
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     3936 2023-04-17 18:37:11.000000 rolv-0.0.5/rolv/src/apps/fzf/shell/key-bindings.bash
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     5727 2023-04-17 18:37:11.000000 rolv-0.0.5/rolv/src/apps/fzf/shell/key-bindings.fish
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     3934 2023-04-17 18:37:11.000000 rolv-0.0.5/rolv/src/apps/fzf/shell/key-bindings.zsh
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:16:35.885530 rolv-0.0.5/rolv/src/config/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     2292 2023-04-18 08:36:32.000000 rolv-0.0.5/rolv/src/config/default_aliases_and_functions
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:16:35.885530 rolv-0.0.5/rolv/src/executables/
+-rwxr-xr-x   0 dorus     (1000) dorus     (1000)       93 2023-04-16 15:53:31.000000 rolv-0.0.5/rolv/src/executables/gitc
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      633 2023-04-16 20:13:04.000000 rolv-0.0.5/rolv/src/executables/readme.md
+-rw-r--r--   0 dorus     (1000) dorus     (1000)       38 2023-04-18 21:16:29.000000 rolv-0.0.5/rolv/src/version
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-18 21:16:35.875530 rolv-0.0.5/rolv.egg-info/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      312 2023-04-18 21:16:35.000000 rolv-0.0.5/rolv.egg-info/PKG-INFO
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      864 2023-04-18 21:16:35.000000 rolv-0.0.5/rolv.egg-info/SOURCES.txt
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        1 2023-04-18 21:16:35.000000 rolv-0.0.5/rolv.egg-info/dependency_links.txt
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      130 2023-04-18 21:16:35.000000 rolv-0.0.5/rolv.egg-info/entry_points.txt
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        5 2023-04-18 21:16:35.000000 rolv-0.0.5/rolv.egg-info/top_level.txt
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      624 2023-04-18 21:16:35.888864 rolv-0.0.5/setup.cfg
```

### Comparing `rolv-0.0.4/README.md` & `rolv-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv/__init__.py` & `rolv-0.0.5/rolv/__init__.py`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv/apps.py` & `rolv-0.0.5/rolv/apps.py`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv/config.py` & `rolv-0.0.5/rolv/config.py`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv/disk.py` & `rolv-0.0.5/rolv/disk.py`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv/executables.py` & `rolv-0.0.5/rolv/executables.py`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv/lib.py` & `rolv-0.0.5/rolv/lib.py`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv/package.py` & `rolv-0.0.5/rolv/package.py`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv/rc.py` & `rolv-0.0.5/rolv/rc.py`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv/src/apps/fzf/bin/fzf` & `rolv-0.0.5/rolv/src/apps/fzf/bin/fzf`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv/src/apps/fzf/bin/fzf-tmux` & `rolv-0.0.5/rolv/src/apps/fzf/bin/fzf-tmux`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv/src/apps/fzf/doc/fzf.txt` & `rolv-0.0.5/rolv/src/apps/fzf/doc/fzf.txt`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv/src/apps/fzf/man/man1/fzf-tmux.1` & `rolv-0.0.5/rolv/src/apps/fzf/man/man1/fzf-tmux.1`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv/src/apps/fzf/man/man1/fzf.1` & `rolv-0.0.5/rolv/src/apps/fzf/man/man1/fzf.1`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv/src/apps/fzf/plugin/fzf.vim` & `rolv-0.0.5/rolv/src/apps/fzf/plugin/fzf.vim`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv/src/apps/fzf/shell/completion.bash` & `rolv-0.0.5/rolv/src/apps/fzf/shell/completion.bash`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv/src/apps/fzf/shell/completion.zsh` & `rolv-0.0.5/rolv/src/apps/fzf/shell/completion.zsh`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv/src/apps/fzf/shell/key-bindings.bash` & `rolv-0.0.5/rolv/src/apps/fzf/shell/key-bindings.bash`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv/src/apps/fzf/shell/key-bindings.fish` & `rolv-0.0.5/rolv/src/apps/fzf/shell/key-bindings.fish`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv/src/apps/fzf/shell/key-bindings.zsh` & `rolv-0.0.5/rolv/src/apps/fzf/shell/key-bindings.zsh`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv/src/config/default_aliases_and_functions` & `rolv-0.0.5/rolv/src/config/default_aliases_and_functions`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv/src/executables/readme.md` & `rolv-0.0.5/rolv/src/executables/readme.md`

 * *Files identical despite different names*

### Comparing `rolv-0.0.4/rolv.egg-info/SOURCES.txt` & `rolv-0.0.5/rolv.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 rolv/rc.py
 rolv.egg-info/PKG-INFO
 rolv.egg-info/SOURCES.txt
 rolv.egg-info/dependency_links.txt
 rolv.egg-info/entry_points.txt
 rolv.egg-info/top_level.txt
 rolv/src/version
+rolv/src/apps/fzf/.fzf.bash
+rolv/src/apps/fzf/.fzf.zsh
 rolv/src/apps/fzf/bin/fzf
 rolv/src/apps/fzf/bin/fzf-tmux
 rolv/src/apps/fzf/doc/fzf.txt
 rolv/src/apps/fzf/man/man1/fzf-tmux.1
 rolv/src/apps/fzf/man/man1/fzf.1
 rolv/src/apps/fzf/plugin/fzf.vim
 rolv/src/apps/fzf/shell/completion.bash
```

### Comparing `rolv-0.0.4/setup.cfg` & `rolv-0.0.5/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [metadata]
 name = rolv
-version = 0.0.4
+version = 0.0.5
 summary = Package to quickly set up linux terminal environment.
 home_page = https://github.com/dwrolvink/rolv
 author = https://github.com/dwrolvink
 author_email = dwrolvink@protonmail.com
 license = GNU General Public License v3 or later (GPLv3+)
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.9
 
 [options.package_data]
-* = *.md, LICENSE, src/**
+* = *.md, LICENSE, src/**, src/**/.*
 
 [options.entry_points]
 console_scripts = 
 	rolv = rolv:help_text
 	rolv.version = rolv:version
 	rolv.install = rolv:install
 	rolv.disclaimer = rolv:disclaimer
```

