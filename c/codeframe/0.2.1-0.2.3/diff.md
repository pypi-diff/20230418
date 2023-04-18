# Comparing `tmp/codeframe-0.2.1.tar.gz` & `tmp/codeframe-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeframe-0.2.1.tar", last modified: Tue Apr 18 14:28:37 2023, max compression
+gzip compressed data, was "codeframe-0.2.3.tar", last modified: Tue Apr 18 14:42:20 2023, max compression
```

## Comparing `codeframe-0.2.1.tar` & `codeframe-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-18 14:28:37.959415 codeframe-0.2.1/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2219 2023-04-18 14:28:37.959415 codeframe-0.2.1/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1916 2023-04-14 15:32:36.000000 codeframe-0.2.1/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-18 14:28:37.959415 codeframe-0.2.1/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    37245 2023-04-18 14:28:21.000000 codeframe-0.2.1/bin/codeframe
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-18 14:28:37.959415 codeframe-0.2.1/codeframe/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2023-04-14 15:32:36.000000 codeframe-0.2.1/codeframe/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6511 2023-04-14 15:32:36.000000 codeframe-0.2.1/codeframe/config.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2299 2023-04-14 15:32:36.000000 codeframe-0.2.1/codeframe/prj_utils.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-04-18 14:28:37.000000 codeframe-0.2.1/codeframe/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-18 14:28:37.959415 codeframe-0.2.1/codeframe.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2219 2023-04-18 14:28:37.000000 codeframe-0.2.1/codeframe.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      282 2023-04-18 14:28:37.000000 codeframe-0.2.1/codeframe.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-04-18 14:28:37.000000 codeframe-0.2.1/codeframe.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        5 2023-04-18 14:28:37.000000 codeframe-0.2.1/codeframe.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2023-04-18 14:28:37.000000 codeframe-0.2.1/codeframe.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-04-18 14:28:37.959415 codeframe-0.2.1/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1198 2023-04-14 15:32:36.000000 codeframe-0.2.1/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-18 14:42:20.187620 codeframe-0.2.3/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     2219 2023-04-18 14:42:20.183620 codeframe-0.2.3/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1916 2023-04-14 15:32:36.000000 codeframe-0.2.3/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-18 14:42:20.183620 codeframe-0.2.3/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    37453 2023-04-18 14:41:28.000000 codeframe-0.2.3/bin/codeframe
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-18 14:42:20.183620 codeframe-0.2.3/codeframe/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2023-04-14 15:32:36.000000 codeframe-0.2.3/codeframe/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6511 2023-04-14 15:32:36.000000 codeframe-0.2.3/codeframe/config.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2299 2023-04-14 15:32:36.000000 codeframe-0.2.3/codeframe/prj_utils.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-04-18 14:42:19.000000 codeframe-0.2.3/codeframe/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-18 14:42:20.183620 codeframe-0.2.3/codeframe.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     2219 2023-04-18 14:42:20.000000 codeframe-0.2.3/codeframe.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      282 2023-04-18 14:42:20.000000 codeframe-0.2.3/codeframe.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-04-18 14:42:20.000000 codeframe-0.2.3/codeframe.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        5 2023-04-18 14:42:20.000000 codeframe-0.2.3/codeframe.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2023-04-18 14:42:20.000000 codeframe-0.2.3/codeframe.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-04-18 14:42:20.187620 codeframe-0.2.3/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1198 2023-04-14 15:32:36.000000 codeframe-0.2.3/setup.py
```

### Comparing `codeframe-0.2.1/PKG-INFO` & `codeframe-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeframe
-Version: 0.2.1
+Version: 0.2.3
 Summary: Creates a simple package structure, git, PyPI, bumpversion, pytest and configfile ready
 Home-page: http://gitlab.com/jaromrax/codeframe
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
```

### Comparing `codeframe-0.2.1/README.md` & `codeframe-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `codeframe-0.2.1/bin/codeframe` & `codeframe-0.2.3/bin/codeframe`

 * *Files 1% similar despite different names*

```diff
@@ -416,14 +416,18 @@
         this is a mandatory for Thread child
         '''
         global global_key
         self.t = threading.current_thread()
         while True:
             #print("!...  ........................keyboard listen START")
             listen_keyboard(on_press=self.press,
+                             # debug = True,
+                            delay_second_char=0.1,
+                            delay_other_chars=0.05,
+                            lower = False, # IT WAS DEFAULT
                             sequential=True) # syncio
             #print("!...  ........................keyboard listen STOP")
             #print("D...",f"/{global_key}/")
             if global_key.strip() == self.ending:
                 #print("!...  ........................keyboard listen BREAK")
                 break
         print("!...  ........................keyboard THREAD  ENDED")
```

### Comparing `codeframe-0.2.1/codeframe/config.py` & `codeframe-0.2.3/codeframe/config.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.2.1/codeframe/prj_utils.py` & `codeframe-0.2.3/codeframe/prj_utils.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.2.1/codeframe.egg-info/PKG-INFO` & `codeframe-0.2.3/codeframe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeframe
-Version: 0.2.1
+Version: 0.2.3
 Summary: Creates a simple package structure, git, PyPI, bumpversion, pytest and configfile ready
 Home-page: http://gitlab.com/jaromrax/codeframe
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
```

### Comparing `codeframe-0.2.1/setup.py` & `codeframe-0.2.3/setup.py`

 * *Files identical despite different names*

