# Comparing `tmp/connpy-3.0.6.tar.gz` & `tmp/connpy-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connpy-3.0.6.tar", last modified: Sun Apr 16 01:41:45 2023, max compression
+gzip compressed data, was "connpy-3.0.7.tar", last modified: Tue Apr 18 21:02:41 2023, max compression
```

## Comparing `connpy-3.0.6.tar` & `connpy-3.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:41:45.301464 connpy-3.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-16 01:41:34.000000 connpy-3.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-16 01:41:45.301464 connpy-3.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-04-16 01:41:34.000000 connpy-3.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:41:45.301464 connpy-3.0.6/connpy/
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-04-16 01:41:34.000000 connpy-3.0.6/connpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-16 01:41:34.000000 connpy-3.0.6/connpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-16 01:41:34.000000 connpy-3.0.6/connpy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-16 01:41:34.000000 connpy-3.0.6/connpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-04-16 01:41:34.000000 connpy-3.0.6/connpy/completion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11869 2023-04-16 01:41:34.000000 connpy-3.0.6/connpy/configfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47695 2023-04-16 01:41:34.000000 connpy-3.0.6/connpy/connapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27894 2023-04-16 01:41:34.000000 connpy-3.0.6/connpy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:41:45.301464 connpy-3.0.6/connpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-16 01:41:45.000000 connpy-3.0.6/connpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-16 01:41:45.000000 connpy-3.0.6/connpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 01:41:45.000000 connpy-3.0.6/connpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-16 01:41:45.000000 connpy-3.0.6/connpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-16 01:41:45.000000 connpy-3.0.6/connpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 01:41:45.000000 connpy-3.0.6/connpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-16 01:41:45.301464 connpy-3.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-16 01:41:34.000000 connpy-3.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:41.223078 connpy-3.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-18 21:02:30.000000 connpy-3.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-18 21:02:41.223078 connpy-3.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-04-18 21:02:30.000000 connpy-3.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:41.223078 connpy-3.0.7/connpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-04-18 21:02:30.000000 connpy-3.0.7/connpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-18 21:02:30.000000 connpy-3.0.7/connpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 21:02:30.000000 connpy-3.0.7/connpy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-04-18 21:02:30.000000 connpy-3.0.7/connpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-04-18 21:02:30.000000 connpy-3.0.7/connpy/completion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11869 2023-04-18 21:02:30.000000 connpy-3.0.7/connpy/configfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47695 2023-04-18 21:02:30.000000 connpy-3.0.7/connpy/connapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27894 2023-04-18 21:02:30.000000 connpy-3.0.7/connpy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:41.223078 connpy-3.0.7/connpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-18 21:02:41.000000 connpy-3.0.7/connpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-18 21:02:41.000000 connpy-3.0.7/connpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:02:41.000000 connpy-3.0.7/connpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-18 21:02:41.000000 connpy-3.0.7/connpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-18 21:02:41.000000 connpy-3.0.7/connpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 21:02:41.000000 connpy-3.0.7/connpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-18 21:02:41.227078 connpy-3.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-18 21:02:30.000000 connpy-3.0.7/setup.py
```

### Comparing `connpy-3.0.6/LICENSE` & `connpy-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `connpy-3.0.6/PKG-INFO` & `connpy-3.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.0.6
+Version: 3.0.7
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.0.6/README.md` & `connpy-3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `connpy-3.0.6/connpy/__init__.py` & `connpy-3.0.7/connpy/__init__.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.6/connpy/api.py` & `connpy-3.0.7/connpy/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,18 @@
                 pid = int(f.readline().strip())
                 port = int(f.readline().strip())
             PID_FILE=PID_FILE2
         except:
             print("Connpy api server is not running.")
             return 
     # Send a SIGTERM signal to the process
-    os.kill(pid, signal.SIGTERM)
+    try:
+        os.kill(pid, signal.SIGTERM)
+    except:
+        pass
     # Delete the PID file
     os.remove(PID_FILE)
     print(f"Server with process ID {pid} stopped.")
     return port
 
 def debug_api(port=8048):
     app.custom_config = configfile()
```

### Comparing `connpy-3.0.6/connpy/completion.py` & `connpy-3.0.7/connpy/completion.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.6/connpy/configfile.py` & `connpy-3.0.7/connpy/configfile.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.6/connpy/connapp.py` & `connpy-3.0.7/connpy/connapp.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.6/connpy/core.py` & `connpy-3.0.7/connpy/core.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.6/connpy.egg-info/PKG-INFO` & `connpy-3.0.7/connpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.0.6
+Version: 3.0.7
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.0.6/setup.cfg` & `connpy-3.0.7/setup.cfg`

 * *Files identical despite different names*

