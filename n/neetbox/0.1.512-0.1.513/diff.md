# Comparing `tmp/neetbox-0.1.512.tar.gz` & `tmp/neetbox-0.1.513.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neetbox-0.1.512.tar", max compression
+gzip compressed data, was "neetbox-0.1.513.tar", max compression
```

## Comparing `neetbox-0.1.512.tar` & `neetbox-0.1.513.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0     1067 2023-04-17 14:43:20.117488 neetbox-0.1.512/LICENSE
--rw-r--r--   0        0        0      397 2023-04-17 14:43:20.117488 neetbox-0.1.512/README.md
--rw-r--r--   0        0        0     2827 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/cli/__init__.py
--rw-r--r--   0        0        0     2910 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/cli/parse.py
--rw-r--r--   0        0        0     1154 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/config/__init__.py
--rw-r--r--   0        0        0     1383 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/config/_config.py
--rw-r--r--   0        0        0       66 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/core/__init__.py
--rw-r--r--   0        0        0     5874 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/core/registry.py
--rw-r--r--   0        0        0     2999 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/daemon/__init__.py
--rw-r--r--   0        0        0      872 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/daemon/_apis.py
--rw-r--r--   0        0        0     2161 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/daemon/_daemon.py
--rw-r--r--   0        0        0     7770 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/daemon/_daemon_client.py
--rw-r--r--   0        0        0     3226 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/daemon/_win_service.py
--rw-r--r--   0        0        0      337 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/integrations/__init__.py
--rw-r--r--   0        0        0     1182 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/integrations/engine.py
--rw-r--r--   0        0        0     3960 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/integrations/environment/hardware.py
--rw-r--r--   0        0        0     1746 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/integrations/environment/platform.py
--rw-r--r--   0        0        0     8536 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/integrations/resource.py
--rw-r--r--   0        0        0      313 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/logging/__init__.py
--rw-r--r--   0        0        0     2106 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/logging/_colorama.py
--rw-r--r--   0        0        0    12181 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/logging/flfs/ansiregular.flf
--rw-r--r--   0        0        0    12181 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/logging/flfs/ansishadow.flf
--rw-r--r--   0        0        0    11585 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/logging/flfs/isometrixc2.flf
--rw-r--r--   0        0        0    23112 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/logging/flfs/nscripts.flf
--rw-r--r--   0        0        0    21669 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/logging/flfs/nvscript.flf
--rw-r--r--   0        0        0     3921 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/logging/formatting.py
--rw-r--r--   0        0        0    18762 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/logging/logger.py
--rw-r--r--   0        0        0        0 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/pipeline/__init__.py
--rw-r--r--   0        0        0      275 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/pipeline/pipe.py
--rw-r--r--   0        0        0        0 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/plotting/__init__.py
--rw-r--r--   0        0        0     4922 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/plotting/plot.py
--rw-r--r--   0        0        0      108 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/torch/__init__.py
--rw-r--r--   0        0        0     5636 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/torch/arch/canny.py
--rw-r--r--   0        0        0     6703 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/torch/arch/cnn.py
--rw-r--r--   0        0        0     2400 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/torch/arch/kernels.py
--rw-r--r--   0        0        0     2699 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/torch/arch/mask_boundary_finder.py
--rw-r--r--   0        0        0     3678 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/torch/nlp.py
--rw-r--r--   0        0        0     4702 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/torch/profile.py
--rw-r--r--   0        0        0       78 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/utils/__init__.py
--rw-r--r--   0        0        0     2669 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/utils/_package.py
--rw-r--r--   0        0        0     1019 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/utils/format.py
--rw-r--r--   0        0        0     2303 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/utils/framing.py
--rw-r--r--   0        0        0     1238 2023-04-17 14:43:20.121488 neetbox-0.1.512/neetbox/utils/mvc.py
--rw-r--r--   0        0        0     1271 2023-04-17 14:43:20.121488 neetbox-0.1.512/pyproject.toml
--rw-r--r--   0        0        0     1678 1970-01-01 00:00:00.000000 neetbox-0.1.512/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-18 02:55:46.703036 neetbox-0.1.513/LICENSE
+-rw-r--r--   0        0        0      397 2023-04-18 02:55:46.703036 neetbox-0.1.513/README.md
+-rw-r--r--   0        0        0     2827 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/cli/__init__.py
+-rw-r--r--   0        0        0     2910 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/cli/parse.py
+-rw-r--r--   0        0        0     1154 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/config/__init__.py
+-rw-r--r--   0        0        0     1390 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/config/_config.py
+-rw-r--r--   0        0        0       66 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/core/__init__.py
+-rw-r--r--   0        0        0     5874 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/core/registry.py
+-rw-r--r--   0        0        0     2984 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/daemon/__init__.py
+-rw-r--r--   0        0        0      872 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/daemon/_apis.py
+-rw-r--r--   0        0        0     2161 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/daemon/_daemon.py
+-rw-r--r--   0        0        0     3086 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/daemon/_daemon_client.py
+-rw-r--r--   0        0        0     3226 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/daemon/_win_service.py
+-rw-r--r--   0        0        0      337 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/integrations/__init__.py
+-rw-r--r--   0        0        0     1182 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/integrations/engine.py
+-rw-r--r--   0        0        0     3962 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/integrations/environment/hardware.py
+-rw-r--r--   0        0        0     1748 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/integrations/environment/platform.py
+-rw-r--r--   0        0        0     8536 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/integrations/resource.py
+-rw-r--r--   0        0        0      313 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/logging/__init__.py
+-rw-r--r--   0        0        0     2106 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/logging/_colorama.py
+-rw-r--r--   0        0        0    12181 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/logging/flfs/ansiregular.flf
+-rw-r--r--   0        0        0    12181 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/logging/flfs/ansishadow.flf
+-rw-r--r--   0        0        0    11585 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/logging/flfs/isometrixc2.flf
+-rw-r--r--   0        0        0    23112 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/logging/flfs/nscripts.flf
+-rw-r--r--   0        0        0    21669 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/logging/flfs/nvscript.flf
+-rw-r--r--   0        0        0     3921 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/logging/formatting.py
+-rw-r--r--   0        0        0    18762 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/logging/logger.py
+-rw-r--r--   0        0        0      241 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/pipeline/__init__.py
+-rw-r--r--   0        0        0      299 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/pipeline/_pipe.py
+-rw-r--r--   0        0        0     5167 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/pipeline/_signal_and_slot.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/plotting/__init__.py
+-rw-r--r--   0        0        0     4922 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/plotting/plot.py
+-rw-r--r--   0        0        0      108 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/torch/__init__.py
+-rw-r--r--   0        0        0     5636 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/torch/arch/canny.py
+-rw-r--r--   0        0        0     6703 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/torch/arch/cnn.py
+-rw-r--r--   0        0        0     2400 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/torch/arch/kernels.py
+-rw-r--r--   0        0        0     2699 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/torch/arch/mask_boundary_finder.py
+-rw-r--r--   0        0        0     3678 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/torch/nlp.py
+-rw-r--r--   0        0        0     4702 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/torch/profile.py
+-rw-r--r--   0        0        0       78 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/utils/__init__.py
+-rw-r--r--   0        0        0     2705 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/utils/_package.py
+-rw-r--r--   0        0        0     1019 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/utils/format.py
+-rw-r--r--   0        0        0     2303 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/utils/framing.py
+-rw-r--r--   0        0        0     1238 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/utils/mvc.py
+-rw-r--r--   0        0        0     1271 2023-04-18 02:55:46.707036 neetbox-0.1.513/pyproject.toml
+-rw-r--r--   0        0        0     1678 1970-01-01 00:00:00.000000 neetbox-0.1.513/PKG-INFO
```

### Comparing `neetbox-0.1.512/LICENSE` & `neetbox-0.1.513/LICENSE`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/__init__.py` & `neetbox-0.1.513/neetbox/__init__.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/cli/parse.py` & `neetbox-0.1.513/neetbox/cli/parse.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/config/__init__.py` & `neetbox-0.1.513/neetbox/config/__init__.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/config/_config.py` & `neetbox-0.1.513/neetbox/config/_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,30 +8,31 @@
 from neetbox.utils.mvc import patch
 from multiprocessing import current_process
 
 DEFAULT_CONFIG = {
     "name": None,
     "version": None,
     "logging": {"logdir": None},
-    "pipeline": {},
+    "pipeline": {
+        "updateInterval": 10,
+    },
     "integrations": {
         "environment": {
             "gpus": "auto",
         },
         "datasets": [],
     },
     "daemon": {
         "enable": True,
         "displayName": None,
         "server": "localhost",
         "port": 20202,
-        "updateInterval": 10,
         "uploadInterval": 10,
         "info": ["log", "status"],
-        "allowIpython":False
+        "allowIpython": False,
     },
 }
 WORKSPACE_CONFIG: dict = DEFAULT_CONFIG.copy()
 
 
 def update_with(cfg: dict):
     def _update_dict_recursively(self: dict, the_other: dict):
```

### Comparing `neetbox-0.1.512/neetbox/core/registry.py` & `neetbox-0.1.513/neetbox/core/registry.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/daemon/__init__.py` & `neetbox-0.1.513/neetbox/daemon/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 #
 # Author: GavinGong aka VisualDust
 # URL:    https://gong.host
 # Date:   20230414
 
-from neetbox.daemon._daemon_client import connect_daemon, watch, listen
+from neetbox.daemon._daemon_client import connect_daemon
 from neetbox.logging import logger
 from neetbox.utils import pkg
 import platform
 import time
 import os
```

### Comparing `neetbox-0.1.512/neetbox/daemon/_apis.py` & `neetbox-0.1.513/neetbox/daemon/_apis.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/daemon/_daemon.py` & `neetbox-0.1.513/neetbox/daemon/_daemon.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/daemon/_win_service.py` & `neetbox-0.1.513/neetbox/daemon/_win_service.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/integrations/engine.py` & `neetbox-0.1.513/neetbox/integrations/engine.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/integrations/environment/hardware.py` & `neetbox-0.1.513/neetbox/integrations/environment/hardware.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import GPUtil
 import psutil
 from GPUtil import GPU
 
 import time
 from threading import Thread
 from neetbox.utils.mvc import Singleton
-from neetbox.daemon import watch
+from neetbox.pipeline import watch
 
 
 class _CPU_STAT(dict):
     def __init__(self, id=-1, percent=0.0, freq=0.0) -> None:
         self["id"] = id
         self["percent"] = percent
         self["freq"] = freq
```

### Comparing `neetbox-0.1.512/neetbox/integrations/environment/platform.py` & `neetbox-0.1.513/neetbox/integrations/environment/platform.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # URL:    https://gong.host
 # Date:   20230417
 
 import getpass
 import platform
 import locale
 import subprocess
-from neetbox.daemon import watch
+from neetbox.pipeline import watch
 from neetbox.utils.mvc import Singleton
 
 
 class __Platform(dict, metaclass=Singleton):
     def __init__(self):
         # system
         self["username"] = getpass.getuser()
```

### Comparing `neetbox-0.1.512/neetbox/integrations/resource.py` & `neetbox-0.1.513/neetbox/integrations/resource.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/logging/_colorama.py` & `neetbox-0.1.513/neetbox/logging/_colorama.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/logging/flfs/ansiregular.flf` & `neetbox-0.1.513/neetbox/logging/flfs/ansiregular.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/logging/flfs/ansishadow.flf` & `neetbox-0.1.513/neetbox/logging/flfs/ansishadow.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/logging/flfs/isometrixc2.flf` & `neetbox-0.1.513/neetbox/logging/flfs/isometrixc2.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/logging/flfs/nscripts.flf` & `neetbox-0.1.513/neetbox/logging/flfs/nscripts.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/logging/flfs/nvscript.flf` & `neetbox-0.1.513/neetbox/logging/flfs/nvscript.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/logging/formatting.py` & `neetbox-0.1.513/neetbox/logging/formatting.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/logging/logger.py` & `neetbox-0.1.513/neetbox/logging/logger.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/plotting/plot.py` & `neetbox-0.1.513/neetbox/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/torch/arch/canny.py` & `neetbox-0.1.513/neetbox/torch/arch/canny.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/torch/arch/cnn.py` & `neetbox-0.1.513/neetbox/torch/arch/cnn.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/torch/arch/kernels.py` & `neetbox-0.1.513/neetbox/torch/arch/kernels.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/torch/arch/mask_boundary_finder.py` & `neetbox-0.1.513/neetbox/torch/arch/mask_boundary_finder.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/torch/nlp.py` & `neetbox-0.1.513/neetbox/torch/nlp.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/torch/profile.py` & `neetbox-0.1.513/neetbox/torch/profile.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/utils/_package.py` & `neetbox-0.1.513/neetbox/utils/_package.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,17 @@
         caller_name = caller.module_name if caller.module else caller.filename
         retry = 4
         _installed = False
         while retry:
             if not retry:
                 error_str = f"Bad Input"
                 raise ValueError(error_str)
-            choice = input(
-                f"{caller_name} want to install {package} via pip. Allow? y/[n]:"
-            )
+            print(f"{caller_name} want to install {package} via pip.")
+            choice = input("Make your choice: [y]/n")
+            choice = choice or 'y'
             if choice in ["y", "yes"]:  # user choose to install
                 print(f"installing {package} via pip...")
                 pip.main(["install", package])
                 _installed = True
                 break
             if choice in ["n", "no"]:  # user choose not to install
                 if terminate:  # the package must be installed
```

### Comparing `neetbox-0.1.512/neetbox/utils/format.py` & `neetbox-0.1.513/neetbox/utils/format.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/utils/framing.py` & `neetbox-0.1.513/neetbox/utils/framing.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/neetbox/utils/mvc.py` & `neetbox-0.1.513/neetbox/utils/mvc.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.512/pyproject.toml` & `neetbox-0.1.513/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neetbox"
-version = "0.1.512"
+version = "0.1.513"
 description = "NEETBox contains useless CV code snippets."
 license = "MIT"
 authors = ["VisualDust <gavin@gong.host>"]
 maintainers = [
     "VisualDust <gavin@gong.host>",
     "PommesPeter <me@pommespeter.space>",
     "PaperCube <imzhy@hotmail.com>"
```

### Comparing `neetbox-0.1.512/PKG-INFO` & `neetbox-0.1.513/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neetbox
-Version: 0.1.512
+Version: 0.1.513
 Summary: NEETBox contains useless CV code snippets.
 Home-page: https://neetbox.550w.host
 License: MIT
 Keywords: computer vision,tools,logging
 Author: VisualDust
 Author-email: gavin@gong.host
 Maintainer: VisualDust
```

