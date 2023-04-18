# Comparing `tmp/csle_ryu-0.1.8.tar.gz` & `tmp/csle_ryu-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_ryu-0.1.8.tar", last modified: Mon Mar 20 15:26:19 2023, max compression
+gzip compressed data, was "csle_ryu-0.1.9.tar", last modified: Tue Mar 21 08:08:59 2023, max compression
```

## Comparing `csle_ryu-0.1.8.tar` & `csle_ryu-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:19.619567 csle_ryu-0.1.8/
--rw-r--r--   0 kimham     (501) staff       (20)      639 2023-03-20 15:26:19.619681 csle_ryu-0.1.8/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     3913 2023-01-11 18:45:47.000000 csle_ryu-0.1.8/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      669 2023-02-12 08:59:32.000000 csle_ryu-0.1.8/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1244 2023-03-20 15:26:19.620315 csle_ryu-0.1.8/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_ryu-0.1.8/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:19.608417 csle_ryu-0.1.8/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:19.611049 csle_ryu-0.1.8/src/csle_ryu/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_ryu-0.1.8/src/csle_ryu/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-03-20 15:26:11.000000 csle_ryu-0.1.8/src/csle_ryu/__version__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:19.613372 csle_ryu-0.1.8/src/csle_ryu/constants/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_ryu-0.1.8/src/csle_ryu/constants/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     2396 2022-12-07 13:41:42.000000 csle_ryu-0.1.8/src/csle_ryu/constants/constants.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:19.614858 csle_ryu-0.1.8/src/csle_ryu/controllers/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_ryu-0.1.8/src/csle_ryu/controllers/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     8323 2022-11-28 13:00:49.000000 csle_ryu-0.1.8/src/csle_ryu/controllers/learning_switch_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)    11773 2022-12-07 10:40:04.000000 csle_ryu-0.1.8/src/csle_ryu/controllers/learning_switch_stp_controller.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:19.618239 csle_ryu-0.1.8/src/csle_ryu/dao/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_ryu-0.1.8/src/csle_ryu/dao/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     4608 2023-03-01 07:00:43.000000 csle_ryu-0.1.8/src/csle_ryu/dao/agg_flow_statistic.py
--rw-r--r--   0 kimham     (501) staff       (20)     8639 2023-03-01 07:00:43.000000 csle_ryu-0.1.8/src/csle_ryu/dao/avg_flow_statistic.py
--rw-r--r--   0 kimham     (501) staff       (20)    15112 2023-03-01 07:00:43.000000 csle_ryu-0.1.8/src/csle_ryu/dao/avg_port_statistic.py
--rw-r--r--   0 kimham     (501) staff       (20)     7034 2023-03-01 07:00:43.000000 csle_ryu-0.1.8/src/csle_ryu/dao/flow_statistic.py
--rw-r--r--   0 kimham     (501) staff       (20)    10610 2023-03-15 10:22:13.000000 csle_ryu-0.1.8/src/csle_ryu/dao/port_statistic.py
--rw-r--r--   0 kimham     (501) staff       (20)      253 2022-11-28 13:00:49.000000 csle_ryu-0.1.8/src/csle_ryu/dao/ryu_controller_type.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:19.619022 csle_ryu-0.1.8/src/csle_ryu/monitor/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_ryu-0.1.8/src/csle_ryu/monitor/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    14351 2022-12-07 10:44:59.000000 csle_ryu-0.1.8/src/csle_ryu/monitor/flow_and_port_stats_monitor.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:19.612926 csle_ryu-0.1.8/src/csle_ryu.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      639 2023-03-20 15:26:19.000000 csle_ryu-0.1.8/src/csle_ryu.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)      873 2023-03-20 15:26:19.000000 csle_ryu-0.1.8/src/csle_ryu.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-03-20 15:26:19.000000 csle_ryu-0.1.8/src/csle_ryu.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:03:06.000000 csle_ryu-0.1.8/src/csle_ryu.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      230 2023-03-20 15:26:19.000000 csle_ryu-0.1.8/src/csle_ryu.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)        9 2023-03-20 15:26:19.000000 csle_ryu-0.1.8/src/csle_ryu.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:08:59.841196 csle_ryu-0.1.9/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      639 2023-03-21 08:08:59.841196 csle_ryu-0.1.9/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3913 2023-01-03 16:53:35.000000 csle_ryu-0.1.9/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      669 2023-02-11 20:28:41.000000 csle_ryu-0.1.9/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1244 2023-03-21 08:08:59.841196 csle_ryu-0.1.9/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2022-11-28 13:03:16.000000 csle_ryu-0.1.9/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:08:59.837195 csle_ryu-0.1.9/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:08:59.841196 csle_ryu-0.1.9/src/csle_ryu/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2022-11-28 13:03:16.000000 csle_ryu-0.1.9/src/csle_ryu/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-03-21 08:08:55.000000 csle_ryu-0.1.9/src/csle_ryu/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:08:59.841196 csle_ryu-0.1.9/src/csle_ryu/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_ryu-0.1.9/src/csle_ryu/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2466 2023-03-21 07:10:46.000000 csle_ryu-0.1.9/src/csle_ryu/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:08:59.841196 csle_ryu-0.1.9/src/csle_ryu/controllers/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_ryu-0.1.9/src/csle_ryu/controllers/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8323 2022-11-28 13:03:16.000000 csle_ryu-0.1.9/src/csle_ryu/controllers/learning_switch_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11773 2022-12-11 08:32:31.000000 csle_ryu-0.1.9/src/csle_ryu/controllers/learning_switch_stp_controller.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:08:59.841196 csle_ryu-0.1.9/src/csle_ryu/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_ryu-0.1.9/src/csle_ryu/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4608 2023-02-28 07:39:18.000000 csle_ryu-0.1.9/src/csle_ryu/dao/agg_flow_statistic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8639 2023-02-28 07:39:45.000000 csle_ryu-0.1.9/src/csle_ryu/dao/avg_flow_statistic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    15112 2023-02-28 07:39:59.000000 csle_ryu-0.1.9/src/csle_ryu/dao/avg_port_statistic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7034 2023-02-28 07:40:12.000000 csle_ryu-0.1.9/src/csle_ryu/dao/flow_statistic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10610 2023-03-17 07:49:22.000000 csle_ryu-0.1.9/src/csle_ryu/dao/port_statistic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      253 2022-11-28 13:03:16.000000 csle_ryu-0.1.9/src/csle_ryu/dao/ryu_controller_type.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:08:59.841196 csle_ryu-0.1.9/src/csle_ryu/monitor/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_ryu-0.1.9/src/csle_ryu/monitor/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14351 2022-12-11 08:32:31.000000 csle_ryu-0.1.9/src/csle_ryu/monitor/flow_and_port_stats_monitor.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:08:59.841196 csle_ryu-0.1.9/src/csle_ryu.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      639 2023-03-21 08:08:59.000000 csle_ryu-0.1.9/src/csle_ryu.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      873 2023-03-21 08:08:59.000000 csle_ryu-0.1.9/src/csle_ryu.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 08:08:59.000000 csle_ryu-0.1.9/src/csle_ryu.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:35:28.000000 csle_ryu-0.1.9/src/csle_ryu.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      230 2023-03-21 08:08:59.000000 csle_ryu-0.1.9/src/csle_ryu.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        9 2023-03-21 08:08:59.000000 csle_ryu-0.1.9/src/csle_ryu.egg-info/top_level.txt
```

### Comparing `csle_ryu-0.1.8/PKG-INFO` & `csle_ryu-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_ryu
-Version: 0.1.8
+Version: 0.1.9
 Summary: RYU SDN Controllers in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_ryu-0.1.8/README.md` & `csle_ryu-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.1.8/pyproject.toml` & `csle_ryu-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.1.8/setup.cfg` & `csle_ryu-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-collector>=0.1.8
+	csle-collector>=0.1.9
 	ryu>=4.34
 	eventlet>=0.30.2
 	confluent-kafka>=1.9.2
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
```

### Comparing `csle_ryu-0.1.8/src/csle_ryu/constants/constants.py` & `csle_ryu-0.1.9/src/csle_ryu/constants/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,15 +43,17 @@
     CONTROLLER_APP = "controller_app"
     NETWORK_ID_THIRD_OCTET = 252
     NETWORK_ID_FOURTH_OCTET = 251
     SUFFIX = "_1"
     DEFAULT_PORT = 6633
     DEFAULT_TRANSPORT_PROTOCOL = "tcp"
     SUBNETMASK_SUFFIX = "/29"
+    FULL_SUBNETMASK_SUFFIX = "/24"
     BITMASK = "255.255.255.248"
+    FULL_BITMASK = "255.255.255.0"
     STPLIB = "stplib"
     BYTE_COUNT = "byte_count"
     PACKET_COUNT = "packet_count"
     FLOW_COUNT = "flow_count"
     IN_PORT = "in_port"
     ETH_DST = "eth_dst"
     PRODUCER_RUNNING = "producer_running"
```

### Comparing `csle_ryu-0.1.8/src/csle_ryu/controllers/learning_switch_controller.py` & `csle_ryu-0.1.9/src/csle_ryu/controllers/learning_switch_controller.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.1.8/src/csle_ryu/controllers/learning_switch_stp_controller.py` & `csle_ryu-0.1.9/src/csle_ryu/controllers/learning_switch_stp_controller.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.1.8/src/csle_ryu/dao/agg_flow_statistic.py` & `csle_ryu-0.1.9/src/csle_ryu/dao/agg_flow_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.1.8/src/csle_ryu/dao/avg_flow_statistic.py` & `csle_ryu-0.1.9/src/csle_ryu/dao/avg_flow_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.1.8/src/csle_ryu/dao/avg_port_statistic.py` & `csle_ryu-0.1.9/src/csle_ryu/dao/avg_port_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.1.8/src/csle_ryu/dao/flow_statistic.py` & `csle_ryu-0.1.9/src/csle_ryu/dao/flow_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.1.8/src/csle_ryu/dao/port_statistic.py` & `csle_ryu-0.1.9/src/csle_ryu/dao/port_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.1.8/src/csle_ryu/monitor/flow_and_port_stats_monitor.py` & `csle_ryu-0.1.9/src/csle_ryu/monitor/flow_and_port_stats_monitor.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.1.8/src/csle_ryu.egg-info/PKG-INFO` & `csle_ryu-0.1.9/src/csle_ryu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-ryu
-Version: 0.1.8
+Version: 0.1.9
 Summary: RYU SDN Controllers in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_ryu-0.1.8/src/csle_ryu.egg-info/SOURCES.txt` & `csle_ryu-0.1.9/src/csle_ryu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

