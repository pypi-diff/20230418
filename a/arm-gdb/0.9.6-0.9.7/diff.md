# Comparing `tmp/arm-gdb-0.9.6.tar.gz` & `tmp/arm-gdb-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arm-gdb-0.9.6.tar", last modified: Tue Apr  4 19:43:28 2023, max compression
+gzip compressed data, was "arm-gdb-0.9.7.tar", last modified: Tue Apr 18 06:58:09 2023, max compression
```

## Comparing `arm-gdb-0.9.6.tar` & `arm-gdb-0.9.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 pengi     (1000) pengi     (1000)        0 2023-04-04 19:43:28.527968 arm-gdb-0.9.6/
--rw-r--r--   0 pengi     (1000) pengi     (1000)     1058 2023-04-02 13:47:51.000000 arm-gdb-0.9.6/LICENSE
--rw-r--r--   0 pengi     (1000) pengi     (1000)    17667 2023-04-04 19:43:28.527968 arm-gdb-0.9.6/PKG-INFO
--rw-r--r--   0 pengi     (1000) pengi     (1000)    15872 2023-04-02 20:46:36.000000 arm-gdb-0.9.6/README.md
-drwxr-xr-x   0 pengi     (1000) pengi     (1000)        0 2023-04-04 19:43:28.527968 arm-gdb-0.9.6/arm_gdb/
--rw-r--r--   0 pengi     (1000) pengi     (1000)     1738 2023-04-04 17:47:23.000000 arm-gdb-0.9.6/arm_gdb/__init__.py
--rw-r--r--   0 pengi     (1000) pengi     (1000)     7899 2023-04-02 20:46:36.000000 arm-gdb-0.9.6/arm_gdb/common.py
--rw-r--r--   0 pengi     (1000) pengi     (1000)     8636 2023-04-04 16:39:02.000000 arm-gdb-0.9.6/arm_gdb/fpu.py
--rw-r--r--   0 pengi     (1000) pengi     (1000)     3645 2023-04-04 18:03:54.000000 arm-gdb-0.9.6/arm_gdb/lib.py
--rw-r--r--   0 pengi     (1000) pengi     (1000)     7017 2023-04-04 16:39:02.000000 arm-gdb-0.9.6/arm_gdb/nvic.py
--rw-r--r--   0 pengi     (1000) pengi     (1000)    33393 2023-04-04 19:39:03.000000 arm-gdb-0.9.6/arm_gdb/scb.py
--rw-r--r--   0 pengi     (1000) pengi     (1000)     8577 2023-04-04 16:39:02.000000 arm-gdb-0.9.6/arm_gdb/svd.py
--rw-r--r--   0 pengi     (1000) pengi     (1000)     2924 2023-04-04 19:39:03.000000 arm-gdb-0.9.6/arm_gdb/systick.py
-drwxr-xr-x   0 pengi     (1000) pengi     (1000)        0 2023-04-04 19:43:28.527968 arm-gdb-0.9.6/arm_gdb.egg-info/
--rw-r--r--   0 pengi     (1000) pengi     (1000)    17667 2023-04-04 19:43:28.000000 arm-gdb-0.9.6/arm_gdb.egg-info/PKG-INFO
--rw-r--r--   0 pengi     (1000) pengi     (1000)      319 2023-04-04 19:43:28.000000 arm-gdb-0.9.6/arm_gdb.egg-info/SOURCES.txt
--rw-r--r--   0 pengi     (1000) pengi     (1000)        1 2023-04-04 19:43:28.000000 arm-gdb-0.9.6/arm_gdb.egg-info/dependency_links.txt
--rw-r--r--   0 pengi     (1000) pengi     (1000)       15 2023-04-04 19:43:28.000000 arm-gdb-0.9.6/arm_gdb.egg-info/requires.txt
--rw-r--r--   0 pengi     (1000) pengi     (1000)        8 2023-04-04 19:43:28.000000 arm-gdb-0.9.6/arm_gdb.egg-info/top_level.txt
--rw-r--r--   0 pengi     (1000) pengi     (1000)      789 2023-04-04 17:47:23.000000 arm-gdb-0.9.6/pyproject.toml
--rw-r--r--   0 pengi     (1000) pengi     (1000)       38 2023-04-04 19:43:28.527968 arm-gdb-0.9.6/setup.cfg
+drwxr-xr-x   0 pengi     (1000) pengi     (1000)        0 2023-04-18 06:58:09.485230 arm-gdb-0.9.7/
+-rw-r--r--   0 pengi     (1000) pengi     (1000)     1058 2023-04-02 13:47:51.000000 arm-gdb-0.9.7/LICENSE
+-rw-r--r--   0 pengi     (1000) pengi     (1000)    17667 2023-04-18 06:58:09.485230 arm-gdb-0.9.7/PKG-INFO
+-rw-r--r--   0 pengi     (1000) pengi     (1000)    15872 2023-04-02 20:46:36.000000 arm-gdb-0.9.7/README.md
+drwxr-xr-x   0 pengi     (1000) pengi     (1000)        0 2023-04-18 06:58:09.485230 arm-gdb-0.9.7/arm_gdb/
+-rw-r--r--   0 pengi     (1000) pengi     (1000)     1738 2023-04-04 17:47:23.000000 arm-gdb-0.9.7/arm_gdb/__init__.py
+-rw-r--r--   0 pengi     (1000) pengi     (1000)     7899 2023-04-02 20:46:36.000000 arm-gdb-0.9.7/arm_gdb/common.py
+-rw-r--r--   0 pengi     (1000) pengi     (1000)     8636 2023-04-04 16:39:02.000000 arm-gdb-0.9.7/arm_gdb/fpu.py
+-rw-r--r--   0 pengi     (1000) pengi     (1000)     3645 2023-04-04 18:03:54.000000 arm-gdb-0.9.7/arm_gdb/lib.py
+-rw-r--r--   0 pengi     (1000) pengi     (1000)     7017 2023-04-04 16:39:02.000000 arm-gdb-0.9.7/arm_gdb/nvic.py
+-rw-r--r--   0 pengi     (1000) pengi     (1000)    33393 2023-04-04 19:56:32.000000 arm-gdb-0.9.7/arm_gdb/scb.py
+-rw-r--r--   0 pengi     (1000) pengi     (1000)     8577 2023-04-04 16:39:02.000000 arm-gdb-0.9.7/arm_gdb/svd.py
+-rw-r--r--   0 pengi     (1000) pengi     (1000)     2924 2023-04-04 19:39:03.000000 arm-gdb-0.9.7/arm_gdb/systick.py
+drwxr-xr-x   0 pengi     (1000) pengi     (1000)        0 2023-04-18 06:58:09.485230 arm-gdb-0.9.7/arm_gdb.egg-info/
+-rw-r--r--   0 pengi     (1000) pengi     (1000)    17667 2023-04-18 06:58:09.000000 arm-gdb-0.9.7/arm_gdb.egg-info/PKG-INFO
+-rw-r--r--   0 pengi     (1000) pengi     (1000)      319 2023-04-18 06:58:09.000000 arm-gdb-0.9.7/arm_gdb.egg-info/SOURCES.txt
+-rw-r--r--   0 pengi     (1000) pengi     (1000)        1 2023-04-18 06:58:09.000000 arm-gdb-0.9.7/arm_gdb.egg-info/dependency_links.txt
+-rw-r--r--   0 pengi     (1000) pengi     (1000)       15 2023-04-18 06:58:09.000000 arm-gdb-0.9.7/arm_gdb.egg-info/requires.txt
+-rw-r--r--   0 pengi     (1000) pengi     (1000)        8 2023-04-18 06:58:09.000000 arm-gdb-0.9.7/arm_gdb.egg-info/top_level.txt
+-rw-r--r--   0 pengi     (1000) pengi     (1000)      789 2023-04-04 17:47:23.000000 arm-gdb-0.9.7/pyproject.toml
+-rw-r--r--   0 pengi     (1000) pengi     (1000)       38 2023-04-18 06:58:09.485230 arm-gdb-0.9.7/setup.cfg
```

### Comparing `arm-gdb-0.9.6/LICENSE` & `arm-gdb-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `arm-gdb-0.9.6/PKG-INFO` & `arm-gdb-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arm-gdb
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python module for GDB to analyze ARM core registers
 Author-email: Max Sikström <max@pengi.se>
 License: Copyright (c) 2023 Max Sikström
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `arm-gdb-0.9.6/README.md` & `arm-gdb-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `arm-gdb-0.9.6/arm_gdb/__init__.py` & `arm-gdb-0.9.7/arm_gdb/__init__.py`

 * *Files identical despite different names*

### Comparing `arm-gdb-0.9.6/arm_gdb/common.py` & `arm-gdb-0.9.7/arm_gdb/common.py`

 * *Files identical despite different names*

### Comparing `arm-gdb-0.9.6/arm_gdb/fpu.py` & `arm-gdb-0.9.7/arm_gdb/fpu.py`

 * *Files identical despite different names*

### Comparing `arm-gdb-0.9.6/arm_gdb/lib.py` & `arm-gdb-0.9.7/arm_gdb/lib.py`

 * *Files identical despite different names*

### Comparing `arm-gdb-0.9.6/arm_gdb/nvic.py` & `arm-gdb-0.9.7/arm_gdb/nvic.py`

 * *Files identical despite different names*

### Comparing `arm-gdb-0.9.6/arm_gdb/scb.py` & `arm-gdb-0.9.7/arm_gdb/scb.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
                 ], "System reset request Secure only.")),
                 (None, FieldBitfield("SYSRESETREQ", 2, 1, "System Reset Request")),
             ]))),
             (None, RegisterDef("SCR", "System Control Register", 0xE000ED10, 4, filt(model, [
                 (None, FieldBitfield(
                     "SEVONPEND", 4, 1, "Determines whether an interrupt transition from inactive state to pending state is a wakeup event")),
                 ('v8', FieldBitfield(
-                    "SLEEPDEEPS", 2, 1, "Sleep deep secure. This field controls whether the SLEEPDEEP bit is only accessible from the Secure state.")),
+                    "SLEEPDEEPS", 3, 1, "Sleep deep secure. This field controls whether the SLEEPDEEP bit is only accessible from the Secure state.")),
                 (None, FieldBitfield(
                     "SLEEPDEEP", 2, 1, "Provides a qualifying hint indicating that waking from sleep might take longer")),
                 (None, FieldBitfield(
                     "SLEEPONEXIT", 1, 1, "Determines whether, on an exit from an ISR that returns to the base level of execution priority, the processor enters a sleep state")),
             ]))),
             (None, RegisterDef("CCR", "Configuration and Control Register", 0xE000ED14, 4, filt(model, [
                 ('v8', FieldBitfield("TRD", 20, 1, "Thread reentrancy disabled.")),
@@ -318,15 +318,15 @@
                               "Indicates when a Debug event has occurred."),
                 FieldBitfield("FORCED", 30, 1,
                               "Indicates that a fault with configurable priority has been escalated to a HardFault exception."),
                 FieldBitfield("VECTTBL", 1, 1,
                               "Indicates when a fault has occurred because of a vector table read error on exception processing."),
             ])),
             (None, RegisterDef("DFSR", "Debug Fault Status Register", 0xE000ED30, 4, filt(model, [
-                ('v8', FieldBitfieldEnum("PMU", 4, 1, [
+                ('v8', FieldBitfieldEnum("PMU", 5, 1, [
                     (0, True, "PMU event has not occurred.", None),
                     (1, False, "PMU event has occurred.", None),
                 ], "PMU event. Sticky flag indicating whether a PMU counter overflow event has occurred.")),
                 (None, FieldBitfieldEnum("EXTERNAL", 4, 1, [
                     (0, True, "No external debug request debug event", None),
                     (1, False, "External debug request debug event", None),
                 ], "Indicates a debug event generated because of the assertion of an external debug request")),
```

### Comparing `arm-gdb-0.9.6/arm_gdb/svd.py` & `arm-gdb-0.9.7/arm_gdb/svd.py`

 * *Files identical despite different names*

### Comparing `arm-gdb-0.9.6/arm_gdb/systick.py` & `arm-gdb-0.9.7/arm_gdb/systick.py`

 * *Files identical despite different names*

### Comparing `arm-gdb-0.9.6/arm_gdb.egg-info/PKG-INFO` & `arm-gdb-0.9.7/arm_gdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arm-gdb
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python module for GDB to analyze ARM core registers
 Author-email: Max Sikström <max@pengi.se>
 License: Copyright (c) 2023 Max Sikström
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `arm-gdb-0.9.6/pyproject.toml` & `arm-gdb-0.9.7/pyproject.toml`

 * *Files identical despite different names*

