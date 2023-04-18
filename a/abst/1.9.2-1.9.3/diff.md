# Comparing `tmp/abst-1.9.2.tar.gz` & `tmp/abst-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abst-1.9.2.tar", last modified: Thu Apr  6 09:14:12 2023, max compression
+gzip compressed data, was "abst-1.9.3.tar", last modified: Tue Apr 18 09:12:10 2023, max compression
```

## Comparing `abst-1.9.2.tar` & `abst-1.9.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:14:12.422695 abst-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-06 09:14:02.000000 abst-1.9.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-04-06 09:14:12.422695 abst-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-06 09:14:02.000000 abst-1.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:14:12.418695 abst-1.9.2/abst/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 09:14:02.000000 abst-1.9.2/abst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-06 09:14:02.000000 abst-1.9.2/abst/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:14:12.422695 abst-1.9.2/abst/bastion_support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 09:14:02.000000 abst-1.9.2/abst/bastion_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-06 09:14:02.000000 abst-1.9.2/abst/bastion_support/bastion_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    22731 2023-04-06 09:14:02.000000 abst-1.9.2/abst/bastion_support/oci_bastion.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-06 09:14:02.000000 abst-1.9.2/abst/cfg_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-06 09:14:02.000000 abst-1.9.2/abst/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-06 09:14:02.000000 abst-1.9.2/abst/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17258 2023-04-06 09:14:02.000000 abst-1.9.2/abst/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:14:12.422695 abst-1.9.2/abst/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 09:14:02.000000 abst-1.9.2/abst/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-06 09:14:02.000000 abst-1.9.2/abst/notifier/version_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-06 09:14:02.000000 abst-1.9.2/abst/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-06 09:14:02.000000 abst-1.9.2/abst/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:14:12.422695 abst-1.9.2/abst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-04-06 09:14:12.000000 abst-1.9.2/abst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-06 09:14:12.000000 abst-1.9.2/abst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 09:14:12.000000 abst-1.9.2/abst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-06 09:14:12.000000 abst-1.9.2/abst.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-06 09:14:12.000000 abst-1.9.2/abst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-06 09:14:12.000000 abst-1.9.2/abst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 09:14:12.000000 abst-1.9.2/abst.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 09:14:12.422695 abst-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-06 09:14:02.000000 abst-1.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:14:12.422695 abst-1.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-06 09:14:02.000000 abst-1.9.2/tests/test_sample_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:12:10.216003 abst-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-18 09:11:55.000000 abst-1.9.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-04-18 09:12:10.216003 abst-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-18 09:11:55.000000 abst-1.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:12:10.212002 abst-1.9.3/abst/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:11:55.000000 abst-1.9.3/abst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-18 09:11:55.000000 abst-1.9.3/abst/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:12:10.216003 abst-1.9.3/abst/bastion_support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:11:55.000000 abst-1.9.3/abst/bastion_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-18 09:11:55.000000 abst-1.9.3/abst/bastion_support/bastion_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22731 2023-04-18 09:11:55.000000 abst-1.9.3/abst/bastion_support/oci_bastion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-18 09:11:55.000000 abst-1.9.3/abst/cfg_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-18 09:11:55.000000 abst-1.9.3/abst/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-18 09:11:55.000000 abst-1.9.3/abst/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-04-18 09:11:55.000000 abst-1.9.3/abst/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:12:10.216003 abst-1.9.3/abst/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:11:55.000000 abst-1.9.3/abst/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-18 09:11:55.000000 abst-1.9.3/abst/notifier/version_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-18 09:11:55.000000 abst-1.9.3/abst/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-18 09:11:55.000000 abst-1.9.3/abst/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:12:10.216003 abst-1.9.3/abst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-04-18 09:12:10.000000 abst-1.9.3/abst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-18 09:12:10.000000 abst-1.9.3/abst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:12:10.000000 abst-1.9.3/abst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 09:12:10.000000 abst-1.9.3/abst.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-18 09:12:10.000000 abst-1.9.3/abst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 09:12:10.000000 abst-1.9.3/abst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:12:10.000000 abst-1.9.3/abst.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 09:12:10.216003 abst-1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-18 09:11:55.000000 abst-1.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:12:10.216003 abst-1.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-18 09:11:55.000000 abst-1.9.3/tests/test_sample_dict.py
```

### Comparing `abst-1.9.2/LICENSE.md` & `abst-1.9.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `abst-1.9.2/PKG-INFO` & `abst-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abst
-Version: 1.9.2
+Version: 1.9.3
 Summary: CLI Command making OCI Bastion and kubernetes usage simple and fast
 Home-page: https://github.com/jiri-otoupal/abst
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: MIT
 Keywords: Auto OCI Bastion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `abst-1.9.2/README.md` & `abst-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `abst-1.9.2/abst/bastion_support/bastion_scheduler.py` & `abst-1.9.3/abst/bastion_support/bastion_scheduler.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.2/abst/bastion_support/oci_bastion.py` & `abst-1.9.3/abst/bastion_support/oci_bastion.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.2/abst/cfg_func.py` & `abst-1.9.3/abst/cfg_func.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.2/abst/config.py` & `abst-1.9.3/abst/config.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.2/abst/dialogs.py` & `abst-1.9.3/abst/dialogs.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.2/abst/main.py` & `abst-1.9.3/abst/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import signal
 import subprocess
 from time import sleep
 
 import click
 import rich
 from InquirerPy import inquirer
+from requests import ConnectTimeout
 from rich.logging import RichHandler
 
 from abst.__version__ import __version_name__, __version__
 from abst.bastion_support.bastion_scheduler import BastionScheduler
 from abst.cfg_func import __upgrade
 from abst.config import default_creds_path, default_contexts_location, default_conf_path
 from abst.dialogs import helm_login_dialog
@@ -94,16 +95,16 @@
 
     display_scheduled()
 
 
 @cli.command(
     "use",
     help="Will Switch context to be used,"
-    " use default for default context specified"
-    " in creds.json",
+         " use default for default context specified"
+         " in creds.json",
 )
 @click.option("--debug", is_flag=True, default=False)
 @click.argument("context-name", default="")
 def use(debug, context_name):
     setup_calls(debug)
 
     used_context = context_name
@@ -249,15 +250,18 @@
 def create():
     signal.signal(signal.SIGINT, BastionScheduler.kill_all)
     signal.signal(signal.SIGTERM, BastionScheduler.kill_all)
 
 
 def setup_calls(debug):
     setup_debug(debug)
-    Notifier.notify()
+    try:
+        Notifier.notify()
+    except (ConnectionError, ConnectTimeout):
+        return False
 
 
 def setup_debug(debug):
     if not debug:
         logging.disable(logging.DEBUG)
         logging.disable(logging.INFO)
 
@@ -278,15 +282,15 @@
 def managed():
     pass
 
 
 @forward.command(
     "single",
     help="Creates only one bastion session and keeps reconnecting until"
-    " its deleted, does not create any more Bastion sessions",
+         " its deleted, does not create any more Bastion sessions",
 )
 @click.option("--shell", is_flag=True, default=False)
 @click.option("--debug", is_flag=True, default=False)
 @click.argument("context-name", default=None, required=False)
 def single_forward(shell, debug, context_name):
     """Creates only one bastion session
     ,connects and reconnects until its ttl runs out"""
@@ -300,15 +304,15 @@
 
     Bastion(used_name).create_forward_loop(shell=shell)
 
 
 @forward.command(
     "fullauto",
     help="Creates and connects to Bastion session indefinitely until "
-    "terminated by user",
+         "terminated by user",
 )
 @click.option("--shell", is_flag=True, default=False)
 @click.option("--debug", is_flag=True, default=False)
 @click.argument("context-name", default=None, required=False)
 def fullauto_forward(shell, debug, context_name):
     """Creates and connects to bastion sessions
     automatically until terminated"""
@@ -325,15 +329,15 @@
 
         sleep(1)
 
 
 @managed.command(
     "single",
     help="Creates only one bastion session and keeps reconnecting until"
-    " its deleted, does not create any more Bastion sessions",
+         " its deleted, does not create any more Bastion sessions",
 )
 @click.option("--shell", is_flag=True, default=False)
 @click.option("--debug", is_flag=True, default=False)
 @click.argument("context-name", default=None, required=False)
 def single_managed(shell, debug, context_name):
     """Creates only one bastion session
     ,connects and reconnects until its ttl runs out"""
@@ -346,15 +350,15 @@
 
     Bastion(used_name).create_managed_loop(shell=shell)
 
 
 @managed.command(
     "fullauto",
     help="Creates and connects to Bastion session indefinitely until "
-    "terminated by user",
+         "terminated by user",
 )
 @click.option("--shell", is_flag=True, default=False)
 @click.option("--debug", is_flag=True, default=False)
 @click.argument("context-name", default=None, required=False)
 def fullauto_managed(shell, debug, context_name):
     """Creates and connects to bastion sessions
     automatically until terminated"""
@@ -532,18 +536,18 @@
 
 @cp.command("login")
 @click.argument("secret_name")
 @click.argument("source_namespace")
 @click.argument("target_namespace")
 @click.option("--debug", is_flag=True, default=False)
 def cp_secret(
-    secret_name: str,
-    target_namespace: str,
-    source_namespace: str = "default",
-    debug=False,
+        secret_name: str,
+        target_namespace: str,
+        source_namespace: str = "default",
+        debug=False,
 ):
     """
     Copy Secret in current cluster from source namespace to target
     @param secret_name: Secret Name
     @param target_namespace: Target Namespace name
     @param source_namespace: Source Namespace name
     @return:
```

### Comparing `abst-1.9.2/abst/notifier/version_notifier.py` & `abst-1.9.3/abst/notifier/version_notifier.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.2/abst/tools.py` & `abst-1.9.3/abst/tools.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.2/abst/wrappers.py` & `abst-1.9.3/abst/wrappers.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.2/abst.egg-info/PKG-INFO` & `abst-1.9.3/abst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abst
-Version: 1.9.2
+Version: 1.9.3
 Summary: CLI Command making OCI Bastion and kubernetes usage simple and fast
 Home-page: https://github.com/jiri-otoupal/abst
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: MIT
 Keywords: Auto OCI Bastion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `abst-1.9.2/abst.egg-info/SOURCES.txt` & `abst-1.9.3/abst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abst-1.9.2/setup.py` & `abst-1.9.3/setup.py`

 * *Files identical despite different names*

