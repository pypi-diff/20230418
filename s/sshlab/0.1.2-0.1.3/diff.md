# Comparing `tmp/sshlab-0.1.2.tar.gz` & `tmp/sshlab-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sshlab-0.1.2.tar", last modified: Sat Apr  1 10:36:50 2023, max compression
+gzip compressed data, was "sshlab-0.1.3.tar", last modified: Tue Apr 18 19:14:50 2023, max compression
```

## Comparing `sshlab-0.1.2.tar` & `sshlab-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:36:50.720016 sshlab-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-01 10:36:39.000000 sshlab-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-01 10:36:50.720016 sshlab-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-01 10:36:39.000000 sshlab-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 10:36:50.720016 sshlab-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-01 10:36:39.000000 sshlab-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:36:50.716016 sshlab-0.1.2/sshlab/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-01 10:36:39.000000 sshlab-0.1.2/sshlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-01 10:36:39.000000 sshlab-0.1.2/sshlab/sshlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-01 10:36:39.000000 sshlab-0.1.2/sshlab/sshlab_kill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-01 10:36:39.000000 sshlab-0.1.2/sshlab/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-01 10:36:39.000000 sshlab-0.1.2/sshlab/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:36:50.720016 sshlab-0.1.2/sshlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-01 10:36:50.000000 sshlab-0.1.2/sshlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-01 10:36:50.000000 sshlab-0.1.2/sshlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 10:36:50.000000 sshlab-0.1.2/sshlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-01 10:36:50.000000 sshlab-0.1.2/sshlab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-01 10:36:50.000000 sshlab-0.1.2/sshlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-01 10:36:50.000000 sshlab-0.1.2/sshlab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:14:50.736395 sshlab-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-18 19:14:39.000000 sshlab-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-18 19:14:50.732396 sshlab-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-18 19:14:39.000000 sshlab-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 19:14:50.736395 sshlab-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-18 19:14:39.000000 sshlab-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:14:50.732396 sshlab-0.1.3/sshlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-18 19:14:39.000000 sshlab-0.1.3/sshlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-18 19:14:39.000000 sshlab-0.1.3/sshlab/sshlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-18 19:14:39.000000 sshlab-0.1.3/sshlab/sshlab_kill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-18 19:14:39.000000 sshlab-0.1.3/sshlab/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 19:14:39.000000 sshlab-0.1.3/sshlab/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:14:50.732396 sshlab-0.1.3/sshlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-18 19:14:50.000000 sshlab-0.1.3/sshlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-18 19:14:50.000000 sshlab-0.1.3/sshlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:14:50.000000 sshlab-0.1.3/sshlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-18 19:14:50.000000 sshlab-0.1.3/sshlab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 19:14:50.000000 sshlab-0.1.3/sshlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 19:14:50.000000 sshlab-0.1.3/sshlab.egg-info/top_level.txt
```

### Comparing `sshlab-0.1.2/LICENSE` & `sshlab-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sshlab-0.1.2/PKG-INFO` & `sshlab-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sshlab
-Version: 0.1.2
+Version: 0.1.3
 Summary: A tool for launching Jupyter Notebooks on remote servers using SSH
 Home-page: https://github.com/vuillaut/sshlab
 Author: Thomas Vuillaume
 Author-email: thomas.vuillaume@lapp.in2p3.fr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sshlab-0.1.2/setup.py` & `sshlab-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `sshlab-0.1.2/sshlab/sshlab.py` & `sshlab-0.1.3/sshlab/sshlab.py`

 * *Files identical despite different names*

### Comparing `sshlab-0.1.2/sshlab/sshlab_kill.py` & `sshlab-0.1.3/sshlab/sshlab_kill.py`

 * *Files identical despite different names*

### Comparing `sshlab-0.1.2/sshlab/utils.py` & `sshlab-0.1.3/sshlab/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     while not is_port_available(port):
         port += 1
     return port
 
 
 # Function to get the PID of the remote Jupyter process
 def get_remote_jupyter_pid(user, server):
-    jupyter_pid_cmd = f"ssh {user}@{server} 'pgrep -f jupyter'"
+    jupyter_pid_cmd = f"ssh {user}@{server} 'pgrep -f jupyter -u {user}'"
     try:
         output = subprocess.check_output(jupyter_pid_cmd, shell=True).decode().strip().split('\n')[0].strip()
         pid = int(output)
     except (subprocess.CalledProcessError, ValueError):
         pid = None
 
     return pid
```

### Comparing `sshlab-0.1.2/sshlab.egg-info/PKG-INFO` & `sshlab-0.1.3/sshlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sshlab
-Version: 0.1.2
+Version: 0.1.3
 Summary: A tool for launching Jupyter Notebooks on remote servers using SSH
 Home-page: https://github.com/vuillaut/sshlab
 Author: Thomas Vuillaume
 Author-email: thomas.vuillaume@lapp.in2p3.fr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

