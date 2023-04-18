# Comparing `tmp/pulumi_twingate-0.0.5.tar.gz` & `tmp/pulumi_twingate-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_twingate-0.0.5.tar", last modified: Fri Apr 29 17:57:53 2022, max compression
+gzip compressed data, was "pulumi_twingate-0.0.9.tar", last modified: Wed May  4 00:04:24 2022, max compression
```

## Comparing `pulumi_twingate-0.0.5.tar` & `pulumi_twingate-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 17:57:53.318642 pulumi_twingate-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-04-29 17:57:53.318642 pulumi_twingate-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1018 2022-04-29 17:57:53.000000 pulumi_twingate-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 17:57:53.318642 pulumi_twingate-0.0.5/pulumi_twingate/
--rw-r--r--   0 runner    (1001) docker     (121)     1672 2022-04-29 17:57:53.000000 pulumi_twingate-0.0.5/pulumi_twingate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3514 2022-04-29 17:57:53.000000 pulumi_twingate-0.0.5/pulumi_twingate/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7788 2022-04-29 17:57:53.000000 pulumi_twingate-0.0.5/pulumi_twingate/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 17:57:53.318642 pulumi_twingate-0.0.5/pulumi_twingate/config/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-04-29 17:57:53.000000 pulumi_twingate-0.0.5/pulumi_twingate/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-04-29 17:57:53.000000 pulumi_twingate-0.0.5/pulumi_twingate/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (121)     2991 2022-04-29 17:57:53.000000 pulumi_twingate-0.0.5/pulumi_twingate/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    11870 2022-04-29 17:57:53.000000 pulumi_twingate-0.0.5/pulumi_twingate/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-04-29 17:57:53.000000 pulumi_twingate-0.0.5/pulumi_twingate/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-29 17:57:53.000000 pulumi_twingate-0.0.5/pulumi_twingate/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     9624 2022-04-29 17:57:53.000000 pulumi_twingate-0.0.5/pulumi_twingate/twingate_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)    12268 2022-04-29 17:57:53.000000 pulumi_twingate-0.0.5/pulumi_twingate/twingate_connector_tokens.py
--rw-r--r--   0 runner    (1001) docker     (121)     6963 2022-04-29 17:57:53.000000 pulumi_twingate-0.0.5/pulumi_twingate/twingate_remote_network.py
--rw-r--r--   0 runner    (1001) docker     (121)    18039 2022-04-29 17:57:53.000000 pulumi_twingate-0.0.5/pulumi_twingate/twingate_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 17:57:53.318642 pulumi_twingate-0.0.5/pulumi_twingate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-04-29 17:57:53.000000 pulumi_twingate-0.0.5/pulumi_twingate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      679 2022-04-29 17:57:53.000000 pulumi_twingate-0.0.5/pulumi_twingate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-29 17:57:53.000000 pulumi_twingate-0.0.5/pulumi_twingate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-29 17:57:53.000000 pulumi_twingate-0.0.5/pulumi_twingate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-04-29 17:57:53.000000 pulumi_twingate-0.0.5/pulumi_twingate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-04-29 17:57:53.000000 pulumi_twingate-0.0.5/pulumi_twingate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-29 17:57:53.318642 pulumi_twingate-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2235 2022-04-29 17:57:53.000000 pulumi_twingate-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 00:04:24.635563 pulumi_twingate-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-05-04 00:04:24.635563 pulumi_twingate-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1018 2022-05-04 00:04:24.000000 pulumi_twingate-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 00:04:24.631563 pulumi_twingate-0.0.9/pulumi_twingate/
+-rw-r--r--   0 runner    (1001) docker     (121)     1672 2022-05-04 00:04:24.000000 pulumi_twingate-0.0.9/pulumi_twingate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3514 2022-05-04 00:04:24.000000 pulumi_twingate-0.0.9/pulumi_twingate/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7788 2022-05-04 00:04:24.000000 pulumi_twingate-0.0.9/pulumi_twingate/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 00:04:24.635563 pulumi_twingate-0.0.9/pulumi_twingate/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-05-04 00:04:24.000000 pulumi_twingate-0.0.9/pulumi_twingate/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-05-04 00:04:24.000000 pulumi_twingate-0.0.9/pulumi_twingate/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2991 2022-05-04 00:04:24.000000 pulumi_twingate-0.0.9/pulumi_twingate/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11870 2022-05-04 00:04:24.000000 pulumi_twingate-0.0.9/pulumi_twingate/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-05-04 00:04:24.000000 pulumi_twingate-0.0.9/pulumi_twingate/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-04 00:04:24.000000 pulumi_twingate-0.0.9/pulumi_twingate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     9624 2022-05-04 00:04:24.000000 pulumi_twingate-0.0.9/pulumi_twingate/twingate_connector.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12268 2022-05-04 00:04:24.000000 pulumi_twingate-0.0.9/pulumi_twingate/twingate_connector_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6963 2022-05-04 00:04:24.000000 pulumi_twingate-0.0.9/pulumi_twingate/twingate_remote_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18039 2022-05-04 00:04:24.000000 pulumi_twingate-0.0.9/pulumi_twingate/twingate_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 00:04:24.635563 pulumi_twingate-0.0.9/pulumi_twingate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-05-04 00:04:24.000000 pulumi_twingate-0.0.9/pulumi_twingate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      679 2022-05-04 00:04:24.000000 pulumi_twingate-0.0.9/pulumi_twingate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-04 00:04:24.000000 pulumi_twingate-0.0.9/pulumi_twingate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-04 00:04:24.000000 pulumi_twingate-0.0.9/pulumi_twingate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-05-04 00:04:24.000000 pulumi_twingate-0.0.9/pulumi_twingate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-05-04 00:04:24.000000 pulumi_twingate-0.0.9/pulumi_twingate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-04 00:04:24.635563 pulumi_twingate-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2235 2022-05-04 00:04:24.000000 pulumi_twingate-0.0.9/setup.py
```

### Comparing `pulumi_twingate-0.0.5/PKG-INFO` & `pulumi_twingate-0.0.9/pulumi_twingate.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_twingate
-Version: 0.0.5
+Name: pulumi-twingate
+Version: 0.0.9
 Summary: A Pulumi package for creating and managing Twingate cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Twingate-Labs/pulumi-twingate
 Keywords: pulumi twingate category/Infrastructure
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_twingate-0.0.5/README.md` & `pulumi_twingate-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-0.0.5/pulumi_twingate/__init__.py` & `pulumi_twingate-0.0.9/pulumi_twingate/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-0.0.5/pulumi_twingate/_inputs.py` & `pulumi_twingate-0.0.9/pulumi_twingate/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-0.0.5/pulumi_twingate/_utilities.py` & `pulumi_twingate-0.0.9/pulumi_twingate/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-0.0.5/pulumi_twingate/config/vars.py` & `pulumi_twingate-0.0.9/pulumi_twingate/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-0.0.5/pulumi_twingate/outputs.py` & `pulumi_twingate-0.0.9/pulumi_twingate/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-0.0.5/pulumi_twingate/provider.py` & `pulumi_twingate-0.0.9/pulumi_twingate/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-0.0.5/pulumi_twingate/twingate_connector.py` & `pulumi_twingate-0.0.9/pulumi_twingate/twingate_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-0.0.5/pulumi_twingate/twingate_connector_tokens.py` & `pulumi_twingate-0.0.9/pulumi_twingate/twingate_connector_tokens.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-0.0.5/pulumi_twingate/twingate_remote_network.py` & `pulumi_twingate-0.0.9/pulumi_twingate/twingate_remote_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-0.0.5/pulumi_twingate/twingate_resource.py` & `pulumi_twingate-0.0.9/pulumi_twingate/twingate_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-0.0.5/pulumi_twingate.egg-info/PKG-INFO` & `pulumi_twingate-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-twingate
-Version: 0.0.5
+Name: pulumi_twingate
+Version: 0.0.9
 Summary: A Pulumi package for creating and managing Twingate cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Twingate-Labs/pulumi-twingate
 Keywords: pulumi twingate category/Infrastructure
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_twingate-0.0.5/pulumi_twingate.egg-info/SOURCES.txt` & `pulumi_twingate-0.0.9/pulumi_twingate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-0.0.5/setup.py` & `pulumi_twingate-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.5"
-PLUGIN_VERSION = "0.0.5"
+VERSION = "0.0.9"
+PLUGIN_VERSION = "0.0.9"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'twingate', PLUGIN_VERSION, '--server', 'https://github.com/Twingate-Labs/pulumi-twingate/releases/download/v${VERSION}'])
         except OSError as error:
```

