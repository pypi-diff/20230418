# Comparing `tmp/Turing Pi BMC-0.1.0.tar.gz` & `tmp/Turing Pi BMC-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Turing Pi BMC-0.1.0.tar", last modified: Sat Mar  4 12:58:09 2023, max compression
+gzip compressed data, was "Turing Pi BMC-0.2.0.tar", last modified: Mon Apr 17 22:18:43 2023, max compression
```

## Comparing `Turing Pi BMC-0.1.0.tar` & `Turing Pi BMC-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-04 12:58:09.838699 Turing Pi BMC-0.1.0/
--rw-rw-rw-   0        0        0     1088 2023-03-04 12:28:43.000000 Turing Pi BMC-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1141 2023-03-04 12:58:09.839759 Turing Pi BMC-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-03-04 12:28:43.000000 Turing Pi BMC-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-04 12:58:09.781542 Turing Pi BMC-0.1.0/Turing_Pi_BMC.egg-info/
--rw-rw-rw-   0        0        0     1141 2023-03-04 12:58:09.000000 Turing Pi BMC-0.1.0/Turing_Pi_BMC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2023-03-04 12:58:09.000000 Turing Pi BMC-0.1.0/Turing_Pi_BMC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-04 12:58:09.000000 Turing Pi BMC-0.1.0/Turing_Pi_BMC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-03-04 12:58:09.000000 Turing Pi BMC-0.1.0/Turing_Pi_BMC.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-03-04 12:58:09.000000 Turing Pi BMC-0.1.0/Turing_Pi_BMC.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-04 12:58:09.836751 Turing Pi BMC-0.1.0/bmc/
--rw-rw-rw-   0        0        0       18 2023-03-04 12:28:43.000000 Turing Pi BMC-0.1.0/bmc/__init__.py
--rw-rw-rw-   0        0        0     5646 2023-03-04 12:28:43.000000 Turing Pi BMC-0.1.0/bmc/cluster.py
--rw-rw-rw-   0        0        0     1160 2023-03-04 12:28:43.000000 Turing Pi BMC-0.1.0/bmc/cluster_request.py
--rw-rw-rw-   0        0        0      104 2023-03-04 12:28:43.000000 Turing Pi BMC-0.1.0/bmc/exceptions.py
--rw-rw-rw-   0        0        0     2632 2023-03-04 12:28:43.000000 Turing Pi BMC-0.1.0/bmc/node.py
--rw-rw-rw-   0        0        0      171 2023-03-04 12:28:43.000000 Turing Pi BMC-0.1.0/bmc/sdcard.py
--rw-rw-rw-   0        0        0      247 2023-03-04 12:28:43.000000 Turing Pi BMC-0.1.0/bmc/turing_pi_types.py
--rw-rw-rw-   0        0        0      237 2023-03-04 12:28:43.000000 Turing Pi BMC-0.1.0/bmc/usb_mode.py
--rw-rw-rw-   0        0        0       90 2023-03-04 12:28:43.000000 Turing Pi BMC-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      911 2023-03-04 12:58:09.842746 Turing Pi BMC-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:18:43.740735 Turing Pi BMC-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-17 22:18:43.740735 Turing Pi BMC-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:18:43.740735 Turing Pi BMC-0.2.0/Turing_Pi_BMC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-17 22:18:43.000000 Turing Pi BMC-0.2.0/Turing_Pi_BMC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-17 22:18:43.000000 Turing Pi BMC-0.2.0/Turing_Pi_BMC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 22:18:43.000000 Turing Pi BMC-0.2.0/Turing_Pi_BMC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-17 22:18:43.000000 Turing Pi BMC-0.2.0/Turing_Pi_BMC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 22:18:43.000000 Turing Pi BMC-0.2.0/Turing_Pi_BMC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:18:43.740735 Turing Pi BMC-0.2.0/bmc/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/bmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/bmc/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/bmc/cluster_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/bmc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/bmc/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/bmc/sdcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/bmc/turing_pi_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/bmc/usb_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-17 22:18:43.740735 Turing Pi BMC-0.2.0/setup.cfg
```

### Comparing `Turing Pi BMC-0.1.0/LICENSE` & `Turing Pi BMC-0.2.0/LICENSE`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2017 AlexaBible.com (Peter McDonald)
+Copyright (c) 2023 Rock Profile (Peter McDonald)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `Turing Pi BMC-0.1.0/PKG-INFO` & `Turing Pi BMC-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-Metadata-Version: 2.1
-Name: Turing Pi BMC
-Version: 0.1.0
-Summary: Package to manage a Turing Pi 2 cluster using the BMC API
-Home-page: https://github.com/petermcd/bmc
-Author: Peter McDonald
-Author-email: git@petermcdonald.co.uk
-Project-URL: Bug Tracker, https://github.com/petermcd/turing-pi-bmc/issues
-Project-URL: Source, https://github.com/petermcd/turing-pi-bmc
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: build
-License-File: LICENSE
-
-# BMC
-
-BMC is a simple package to interact with the Turing Pi 2 BMC enabling features such as
-turning on power to nodes.
-
-## Usage
-
-```python
-from ipaddress import IPv4Address
-from bmc.cluster import Cluster
-
-cluster = Cluster(cluster_ip=IPv4Address('192.168.1.170'))
-sdcard = cluster.get_sdcard()
-print(sdcard)
-```
+Metadata-Version: 2.1
+Name: Turing Pi BMC
+Version: 0.2.0
+Summary: Package to manage a Turing Pi 2 cluster using the BMC API
+Home-page: https://github.com/petermcd/bmc
+Author: Peter McDonald
+Author-email: git@petermcdonald.co.uk
+Project-URL: Bug Tracker, https://github.com/petermcd/turing-pi-bmc/issues
+Project-URL: Source, https://github.com/petermcd/turing-pi-bmc
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: build
+License-File: LICENSE
+
+# BMC
+
+BMC is a simple package to interact with the Turing Pi 2 BMC enabling features such as
+turning on power to nodes.
+
+## Usage
+
+```python
+from ipaddress import IPv4Address
+from bmc.cluster import Cluster
+
+cluster = Cluster(cluster_ip=IPv4Address('192.168.1.170'))
+sdcard = cluster.get_sdcard()
+print(sdcard)
+```
```

### Comparing `Turing Pi BMC-0.1.0/Turing_Pi_BMC.egg-info/PKG-INFO` & `Turing Pi BMC-0.2.0/Turing_Pi_BMC.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-Metadata-Version: 2.1
-Name: Turing-Pi-BMC
-Version: 0.1.0
-Summary: Package to manage a Turing Pi 2 cluster using the BMC API
-Home-page: https://github.com/petermcd/bmc
-Author: Peter McDonald
-Author-email: git@petermcdonald.co.uk
-Project-URL: Bug Tracker, https://github.com/petermcd/turing-pi-bmc/issues
-Project-URL: Source, https://github.com/petermcd/turing-pi-bmc
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: build
-License-File: LICENSE
-
-# BMC
-
-BMC is a simple package to interact with the Turing Pi 2 BMC enabling features such as
-turning on power to nodes.
-
-## Usage
-
-```python
-from ipaddress import IPv4Address
-from bmc.cluster import Cluster
-
-cluster = Cluster(cluster_ip=IPv4Address('192.168.1.170'))
-sdcard = cluster.get_sdcard()
-print(sdcard)
-```
+Metadata-Version: 2.1
+Name: Turing-Pi-BMC
+Version: 0.2.0
+Summary: Package to manage a Turing Pi 2 cluster using the BMC API
+Home-page: https://github.com/petermcd/bmc
+Author: Peter McDonald
+Author-email: git@petermcdonald.co.uk
+Project-URL: Bug Tracker, https://github.com/petermcd/turing-pi-bmc/issues
+Project-URL: Source, https://github.com/petermcd/turing-pi-bmc
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: build
+License-File: LICENSE
+
+# BMC
+
+BMC is a simple package to interact with the Turing Pi 2 BMC enabling features such as
+turning on power to nodes.
+
+## Usage
+
+```python
+from ipaddress import IPv4Address
+from bmc.cluster import Cluster
+
+cluster = Cluster(cluster_ip=IPv4Address('192.168.1.170'))
+sdcard = cluster.get_sdcard()
+print(sdcard)
+```
```

### Comparing `Turing Pi BMC-0.1.0/bmc/cluster_request.py` & `Turing Pi BMC-0.2.0/bmc/cluster_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         Args:
             cluster_ip: IP for the cluster
         """
         self._cluster_ip = cluster_ip
 
     def make_request(self, url: str):
         """
-        Make a request to the cluster.
+        Make a request to the cluster using the API.
 
         Args:
             url: The url for the request
 
         Raises:
             RequestException: On incorrect response code or invalid response
```

### Comparing `Turing Pi BMC-0.1.0/bmc/node.py` & `Turing Pi BMC-0.2.0/bmc/node.py`

 * *Files identical despite different names*

