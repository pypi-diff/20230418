# Comparing `tmp/pystemd-0.7.0.tar.gz` & `tmp/pystemd-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pystemd-0.7.0.tar", last modified: Sun Dec  8 01:39:04 2019, max compression
+gzip compressed data, was "dist/pystemd-0.8.0.tar", last modified: Tue Sep 29 16:50:45 2020, max compression
```

## Comparing `pystemd-0.7.0.tar` & `pystemd-0.8.0.tar`

### file list

```diff
@@ -1,47 +1,53 @@
-drwxr-xr-x   0 aleivag   (1001) aleivag   (1001)        0 2019-12-08 01:39:04.000000 pystemd-0.7.0/
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)    26530 2019-12-08 01:38:54.000000 pystemd-0.7.0/LICENSE
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)       87 2019-12-08 01:38:54.000000 pystemd-0.7.0/MANIFEST.in
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)    10591 2019-12-08 01:39:04.000000 pystemd-0.7.0/PKG-INFO
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)     7805 2019-12-08 01:38:54.000000 pystemd-0.7.0/README.md
-drwxr-xr-x   0 aleivag   (1001) aleivag   (1001)        0 2019-12-08 01:39:04.000000 pystemd-0.7.0/pystemd/
-drwxr-xr-x   0 aleivag   (1001) aleivag   (1001)        0 2019-12-08 01:39:04.000000 pystemd-0.7.0/pystemd/DBus/
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)      525 2019-12-08 01:38:54.000000 pystemd-0.7.0/pystemd/DBus/__init__.py
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)       10 2019-12-08 01:39:04.000000 pystemd-0.7.0/pystemd/RELEASE
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)     3874 2019-12-08 01:38:54.000000 pystemd-0.7.0/pystemd/__init__.py
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)      551 2019-12-08 01:38:54.000000 pystemd-0.7.0/pystemd/__version__.py
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)     9119 2019-12-08 01:38:54.000000 pystemd-0.7.0/pystemd/base.py
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)   253696 2019-12-08 01:39:03.000000 pystemd-0.7.0/pystemd/daemon.c
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)     2480 2019-12-08 01:38:54.000000 pystemd-0.7.0/pystemd/daemon.pyx
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)   289540 2019-12-08 01:39:03.000000 pystemd-0.7.0/pystemd/dbusexc.c
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)     5585 2019-12-08 01:38:54.000000 pystemd-0.7.0/pystemd/dbusexc.pyx
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)   980132 2019-12-08 01:39:04.000000 pystemd-0.7.0/pystemd/dbuslib.c
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)    21726 2019-12-08 01:38:54.000000 pystemd-0.7.0/pystemd/dbuslib.pyx
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)      262 2019-12-08 01:38:54.000000 pystemd-0.7.0/pystemd/exceptions.py
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)   192015 2019-12-08 01:39:04.000000 pystemd-0.7.0/pystemd/journal.c
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)     1730 2019-12-08 01:38:54.000000 pystemd-0.7.0/pystemd/journal.pyx
-drwxr-xr-x   0 aleivag   (1001) aleivag   (1001)        0 2019-12-08 01:39:04.000000 pystemd-0.7.0/pystemd/machine1/
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)      311 2019-12-08 01:38:54.000000 pystemd-0.7.0/pystemd/machine1/__init__.py
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)      736 2019-12-08 01:38:54.000000 pystemd-0.7.0/pystemd/machine1/machine.py
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)      534 2019-12-08 01:38:54.000000 pystemd-0.7.0/pystemd/machine1/manager.py
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)    11841 2019-12-08 01:38:54.000000 pystemd-0.7.0/pystemd/run.py
-drwxr-xr-x   0 aleivag   (1001) aleivag   (1001)        0 2019-12-08 01:39:04.000000 pystemd-0.7.0/pystemd/systemd1/
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)      302 2019-12-08 01:38:54.000000 pystemd-0.7.0/pystemd/systemd1/__init__.py
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)     2037 2019-12-08 01:38:54.000000 pystemd-0.7.0/pystemd/systemd1/manager.py
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)      726 2019-12-08 01:38:54.000000 pystemd-0.7.0/pystemd/systemd1/unit.py
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)     9612 2019-12-08 01:38:54.000000 pystemd-0.7.0/pystemd/systemd1/unit_signatures.py
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)     1113 2019-12-08 01:38:54.000000 pystemd-0.7.0/pystemd/utils.py
-drwxr-xr-x   0 aleivag   (1001) aleivag   (1001)        0 2019-12-08 01:39:04.000000 pystemd-0.7.0/pystemd.egg-info/
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)    10591 2019-12-08 01:39:04.000000 pystemd-0.7.0/pystemd.egg-info/PKG-INFO
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)      844 2019-12-08 01:39:04.000000 pystemd-0.7.0/pystemd.egg-info/SOURCES.txt
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)        1 2019-12-08 01:39:04.000000 pystemd-0.7.0/pystemd.egg-info/dependency_links.txt
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)        8 2019-12-08 01:39:04.000000 pystemd-0.7.0/pystemd.egg-info/top_level.txt
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)       73 2019-12-08 01:39:04.000000 pystemd-0.7.0/setup.cfg
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)     2942 2019-12-08 01:38:54.000000 pystemd-0.7.0/setup.py
-drwxr-xr-x   0 aleivag   (1001) aleivag   (1001)        0 2019-12-08 01:39:04.000000 pystemd-0.7.0/tests/
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)     3190 2019-12-08 01:38:54.000000 pystemd-0.7.0/tests/test_base.py
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)      702 2019-12-08 01:38:54.000000 pystemd-0.7.0/tests/test_daemon.py
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)     4066 2019-12-08 01:38:54.000000 pystemd-0.7.0/tests/test_dbus_arg_parsing.py
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)     2468 2019-12-08 01:38:54.000000 pystemd-0.7.0/tests/test_dbuslib.py
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)     1054 2019-12-08 01:38:54.000000 pystemd-0.7.0/tests/test_journal.py
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)      775 2019-12-08 01:38:54.000000 pystemd-0.7.0/tests/test_unit_signatures.py
--rw-r--r--   0 aleivag   (1001) aleivag   (1001)     1108 2019-12-08 01:38:54.000000 pystemd-0.7.0/tests/test_utils.py
+drwxrwxr-x   0 aleivag   (1000) aleivag   (1000)        0 2020-09-29 16:50:45.000000 pystemd-0.8.0/
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)    26530 2020-09-29 16:49:19.000000 pystemd-0.8.0/LICENSE
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)       87 2020-09-29 16:49:19.000000 pystemd-0.8.0/MANIFEST.in
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)    10519 2020-09-29 16:50:45.000000 pystemd-0.8.0/PKG-INFO
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)     7683 2020-09-29 16:49:19.000000 pystemd-0.8.0/README.md
+drwxrwxr-x   0 aleivag   (1000) aleivag   (1000)        0 2020-09-29 16:50:45.000000 pystemd-0.8.0/pystemd/
+drwxrwxr-x   0 aleivag   (1000) aleivag   (1000)        0 2020-09-29 16:50:45.000000 pystemd-0.8.0/pystemd/DBus/
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)      525 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/DBus/__init__.py
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)       10 2020-09-29 16:50:45.000000 pystemd-0.8.0/pystemd/RELEASE
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)     3874 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/__init__.py
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)      551 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/__version__.py
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)     9119 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/base.py
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)     1122 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/base.pyi
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)   255416 2020-09-29 16:50:40.000000 pystemd-0.8.0/pystemd/daemon.c
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)      513 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/daemon.pyi
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)     2480 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/daemon.pyx
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)   291459 2020-09-29 16:50:40.000000 pystemd-0.8.0/pystemd/dbusexc.c
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)     5585 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/dbusexc.pyx
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)   992046 2020-09-29 16:50:40.000000 pystemd-0.8.0/pystemd/dbuslib.c
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)     1736 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/dbuslib.pyi
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)    21728 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/dbuslib.pyx
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)      262 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/exceptions.py
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)   193123 2020-09-29 16:50:40.000000 pystemd-0.8.0/pystemd/journal.c
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)     1730 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/journal.pyx
+drwxrwxr-x   0 aleivag   (1000) aleivag   (1000)        0 2020-09-29 16:50:45.000000 pystemd-0.8.0/pystemd/machine1/
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)      311 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/machine1/__init__.py
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)      736 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/machine1/machine.py
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)      534 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/machine1/manager.py
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)    11680 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/run.py
+drwxrwxr-x   0 aleivag   (1000) aleivag   (1000)        0 2020-09-29 16:50:45.000000 pystemd-0.8.0/pystemd/systemd1/
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)      302 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/systemd1/__init__.py
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)     2037 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/systemd1/manager.py
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)     7575 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/systemd1/manager.pyi
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)      726 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/systemd1/unit.py
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)    14330 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/systemd1/unit.pyi
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)     9791 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/systemd1/unit_signatures.py
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)     1113 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/utils.py
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)      321 2020-09-29 16:49:19.000000 pystemd-0.8.0/pystemd/utils.pyi
+drwxrwxr-x   0 aleivag   (1000) aleivag   (1000)        0 2020-09-29 16:50:45.000000 pystemd-0.8.0/pystemd.egg-info/
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)    10519 2020-09-29 16:50:45.000000 pystemd-0.8.0/pystemd.egg-info/PKG-INFO
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)      973 2020-09-29 16:50:45.000000 pystemd-0.8.0/pystemd.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)        1 2020-09-29 16:50:45.000000 pystemd-0.8.0/pystemd.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)        8 2020-09-29 16:50:45.000000 pystemd-0.8.0/pystemd.egg-info/top_level.txt
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)       73 2020-09-29 16:50:45.000000 pystemd-0.8.0/setup.cfg
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)     3186 2020-09-29 16:49:19.000000 pystemd-0.8.0/setup.py
+drwxrwxr-x   0 aleivag   (1000) aleivag   (1000)        0 2020-09-29 16:50:45.000000 pystemd-0.8.0/tests/
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)     3190 2020-09-29 16:49:19.000000 pystemd-0.8.0/tests/test_base.py
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)      702 2020-09-29 16:49:19.000000 pystemd-0.8.0/tests/test_daemon.py
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)     4066 2020-09-29 16:49:19.000000 pystemd-0.8.0/tests/test_dbus_arg_parsing.py
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)     2469 2020-09-29 16:49:19.000000 pystemd-0.8.0/tests/test_dbuslib.py
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)     1054 2020-09-29 16:49:19.000000 pystemd-0.8.0/tests/test_journal.py
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)      775 2020-09-29 16:49:19.000000 pystemd-0.8.0/tests/test_unit_signatures.py
+-rw-rw-r--   0 aleivag   (1000) aleivag   (1000)     1108 2020-09-29 16:49:19.000000 pystemd-0.8.0/tests/test_utils.py
```

### Comparing `pystemd-0.7.0/LICENSE` & `pystemd-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pystemd-0.7.0/PKG-INFO` & `pystemd-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pystemd
-Version: 0.7.0
+Version: 0.8.0
 Summary: A systemd binding for python
 Home-page: https://github.com/facebookincubator/pystemd
 Author: Alvaro Leiva
 Author-email: aleivag@fb.com
 License: LGPL-2.1+
 Description: pystemd
         =======
         
-        [![Build Status](https://travis-ci.org/facebookincubator/pystemd.svg)](http://travis-ci.org/facebookincubator/pystemd) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+        ![Continuous Integration](https://github.com/facebookincubator/pystemd/workflows/Continuous%20Integration/badge.svg?event=push)
         
         This library allows you to talk to systemd over dbus from python, without
         actually thinking that you are talking to systemd over dbus. This allows you to
         programmatically start/stop/restart/kill and verify services status from
         systemd point of view, avoiding executing `subprocess.Popen(['systemctl', ...`
         and then parsing the output to know the result.
         
@@ -219,15 +219,15 @@
         
         * Python headers: Just use your distro's package (e.g. python-dev).
         * systemd headers: Chances are you already have this. Normally, it is called
         `libsystemd-dev` or `systemd-devel`. You need to have at least v237.
         Please note that CentOS 7 ships with version 219. To work around this, please read
           [this](_docs/centos7.md).
         * systemd library: check if `pkg-config --cflags --libs libsystemd` returns
-        `-lsystemd` if not you can install normally install `systemd-libs` or
+        `-lsystemd` if not you can install `systemd-libs` or
         `libsystemd` depending on your distribution, version needs to be at least
         v237.
         * gcc: or any compiler that `setup.py` will accept.
         
         if you want to install from source then after you clone this repo you need to
         
         ```bash
@@ -263,11 +263,12 @@
 Platform: UNKNOWN
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Description-Content-Type: text/markdown
```

### Comparing `pystemd-0.7.0/README.md` & `pystemd-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 pystemd
 =======
 
-[![Build Status](https://travis-ci.org/facebookincubator/pystemd.svg)](http://travis-ci.org/facebookincubator/pystemd) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+![Continuous Integration](https://github.com/facebookincubator/pystemd/workflows/Continuous%20Integration/badge.svg?event=push)
 
 This library allows you to talk to systemd over dbus from python, without
 actually thinking that you are talking to systemd over dbus. This allows you to
 programmatically start/stop/restart/kill and verify services status from
 systemd point of view, avoiding executing `subprocess.Popen(['systemctl', ...`
 and then parsing the output to know the result.
 
@@ -211,15 +211,15 @@
 
 * Python headers: Just use your distro's package (e.g. python-dev).
 * systemd headers: Chances are you already have this. Normally, it is called
 `libsystemd-dev` or `systemd-devel`. You need to have at least v237.
 Please note that CentOS 7 ships with version 219. To work around this, please read
   [this](_docs/centos7.md).
 * systemd library: check if `pkg-config --cflags --libs libsystemd` returns
-`-lsystemd` if not you can install normally install `systemd-libs` or
+`-lsystemd` if not you can install `systemd-libs` or
 `libsystemd` depending on your distribution, version needs to be at least
 v237.
 * gcc: or any compiler that `setup.py` will accept.
 
 if you want to install from source then after you clone this repo you need to
 
 ```bash
```

### Comparing `pystemd-0.7.0/pystemd/DBus/__init__.py` & `pystemd-0.8.0/pystemd/DBus/__init__.py`

 * *Files identical despite different names*

### Comparing `pystemd-0.7.0/pystemd/__init__.py` & `pystemd-0.8.0/pystemd/__init__.py`

 * *Files identical despite different names*

### Comparing `pystemd-0.7.0/pystemd/__version__.py` & `pystemd-0.8.0/pystemd/__version__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # the root directory of this source tree.
 #
 
 import os
 import sys
 
 
-__version__ = "0.7"
+__version__ = "0.8"
 
 _endstr = ".dev"
 
 release_file = os.path.join(os.path.dirname(__file__), "RELEASE")
 if os.path.exists(release_file):
     with open(release_file) as release_fileobj:
         _endstr = ".{}".format(release_fileobj.read().strip())
```

### Comparing `pystemd-0.7.0/pystemd/base.py` & `pystemd-0.8.0/pystemd/base.py`

 * *Files identical despite different names*

### Comparing `pystemd-0.7.0/pystemd/daemon.c` & `pystemd-0.8.0/pystemd/daemon.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.14 */
+/* Generated by Cython 0.29.21 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "libraries": [
             "systemd"
@@ -19,16 +19,16 @@
 #define PY_SSIZE_T_CLEAN
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_14"
-#define CYTHON_HEX_VERSION 0x001D0EF0
+#define CYTHON_ABI "0_29_21"
+#define CYTHON_HEX_VERSION 0x001D15F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -447,15 +447,19 @@
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
+  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #else
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+  #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
@@ -496,26 +500,35 @@
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBaseString_Type            PyUnicode_Type
   #define PyStringObject               PyUnicodeObject
   #define PyString_Type                PyUnicode_Type
   #define PyString_Check               PyUnicode_Check
   #define PyString_CheckExact          PyUnicode_CheckExact
+#ifndef PyObject_Unicode
   #define PyObject_Unicode             PyObject_Str
 #endif
+#endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
 #ifndef PySet_CheckExact
   #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
 #endif
+#if PY_VERSION_HEX >= 0x030900A4
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
+#else
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
+#endif
 #if CYTHON_ASSUME_SAFE_MACROS
   #define __Pyx_PySequence_SIZE(seq)  Py_SIZE(seq)
 #else
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
@@ -547,15 +560,15 @@
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
   #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
   #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? PyMethod_New(func, self) : (Py_INCREF(func), func))
+  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
@@ -588,19 +601,18 @@
 #endif
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
-
+#define __PYX_MARK_ERR_POS(f_index, lineno) \
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
-{ \
-  __pyx_filename = __pyx_f[f_index]; __pyx_lineno = lineno; __pyx_clineno = __LINE__; goto Ln_error; \
-}
+    { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifndef __PYX_EXTERN_C
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
@@ -1139,15 +1151,15 @@
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len)) {
         Py_INCREF(x);
         PyList_SET_ITEM(list, len, x);
-        Py_SIZE(list) = len+1;
+        __Pyx_SET_SIZE(list, len + 1);
         return 0;
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
 #endif
@@ -1522,14 +1534,17 @@
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7pystemd_6daemon_1listen_fds(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_7pystemd_6daemon_1listen_fds = {"listen_fds", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pystemd_6daemon_1listen_fds, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_7pystemd_6daemon_1listen_fds(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   int __pyx_v_unset_environment;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("listen_fds (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_unset_environment,0};
     PyObject* values[1] = {0};
     if (unlikely(__pyx_kwds)) {
@@ -1581,14 +1596,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_6daemon_listen_fds(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_unset_environment) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("listen_fds", 0);
 
   /* "pystemd/daemon.pyx":24
  * 
  * def listen_fds(int unset_environment=0):
  *   return dbusc.sd_listen_fds(unset_environment)             # <<<<<<<<<<<<<<
  * 
@@ -1632,14 +1650,17 @@
 static PyObject *__pyx_pw_7pystemd_6daemon_3notify(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_7pystemd_6daemon_2notify[] = "\n  interface to systemd sd_notify,\n\n  params:\n    unset_environment[int] = 1 if we should remove the notify information,\n      otherwize 0.\n    states/kwstates = array with states statements that are 'IDENTIFIER=VALUE'.\n      e.g: 'READY=1' or keywords states like `ready=1`\n      (This will be clear in usage).\n\n  usage:\n    * `pystemd.daemon.notify(1, ready=1)`: this will signal `READY=1` to systemd\n      notify and will remove all information from the environment. You should not\n      try to talk to systemd notify socket again.\n    *  `pystemd.daemon.notify(True, \"READY=1\")`: same as above just passed as a\n      string.\n    *  `pystemd.daemon.notify(False, ready=1, status='gime gime gime')`: will\n      signal systemd that the app is ready and also set the status to\n      'gime gime gime'. This command does not clean the notify environment.\n\n    For info on sd_notify, check https://github.com/systemd/systemd/blob/master/src/systemd/sd-daemon.h#L173-L232\n\n  ";
 static PyMethodDef __pyx_mdef_7pystemd_6daemon_3notify = {"notify", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pystemd_6daemon_3notify, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pystemd_6daemon_2notify};
 static PyObject *__pyx_pw_7pystemd_6daemon_3notify(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   int __pyx_v_unset_environment;
   PyObject *__pyx_v_states = 0;
   PyObject *__pyx_v_kwstates = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("notify (wrapper)", 0);
   __pyx_v_kwstates = PyDict_New(); if (unlikely(!__pyx_v_kwstates)) return NULL;
   __Pyx_GOTREF(__pyx_v_kwstates);
   if (PyTuple_GET_SIZE(__pyx_args) > 1) {
     __pyx_v_states = PyTuple_GetSlice(__pyx_args, 1, PyTuple_GET_SIZE(__pyx_args));
@@ -1709,14 +1730,17 @@
  *   )
  */
 
 static PyObject *__pyx_pf_7pystemd_6daemon_6notify_genexpr(PyObject *__pyx_self) {
   struct __pyx_obj_7pystemd_6daemon___pyx_scope_struct_1_genexpr *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_7pystemd_6daemon___pyx_scope_struct_1_genexpr *)__pyx_tp_new_7pystemd_6daemon___pyx_scope_struct_1_genexpr(__pyx_ptype_7pystemd_6daemon___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_7pystemd_6daemon___pyx_scope_struct_1_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 54, __pyx_L1_error)
   } else {
@@ -1752,14 +1776,17 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("genexpr", 0);
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
@@ -1935,14 +1962,17 @@
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   char const *__pyx_t_8;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("notify", 0);
   __pyx_cur_scope = (struct __pyx_obj_7pystemd_6daemon___pyx_scope_struct__notify *)__pyx_tp_new_7pystemd_6daemon___pyx_scope_struct__notify(__pyx_ptype_7pystemd_6daemon___pyx_scope_struct__notify, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_7pystemd_6daemon___pyx_scope_struct__notify *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 27, __pyx_L1_error)
   } else {
@@ -2105,14 +2135,17 @@
   int __pyx_v_status;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("booted", 0);
 
   /* "pystemd/daemon.pyx":63
  * def booted():
  *   "Returns True if system was booted with systemd"
  *   cdef int status = dbusc.sd_booted()             # <<<<<<<<<<<<<<
  *   if status >=0:
@@ -2212,14 +2245,17 @@
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7pystemd_6daemon_7watchdog_enabled(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_7pystemd_6daemon_6watchdog_enabled[] = "\n  returns 0 if watchdog is not enabled, and returns the number of usec between\n  keep-alive notification messages that the service manager expects.\n  ";
 static PyMethodDef __pyx_mdef_7pystemd_6daemon_7watchdog_enabled = {"watchdog_enabled", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pystemd_6daemon_7watchdog_enabled, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pystemd_6daemon_6watchdog_enabled};
 static PyObject *__pyx_pw_7pystemd_6daemon_7watchdog_enabled(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   int __pyx_v_unset_environment;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("watchdog_enabled (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_unset_environment,0};
     PyObject* values[1] = {0};
     if (unlikely(__pyx_kwds)) {
@@ -2276,14 +2312,17 @@
   uint64_t __pyx_v_usec;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("watchdog_enabled", 0);
 
   /* "pystemd/daemon.pyx":80
  *     uint64_t usec
  * 
  *   result = dbusc.sd_watchdog_enabled(unset_environment, &usec)             # <<<<<<<<<<<<<<
  *   if result < 0:
@@ -2827,14 +2866,17 @@
   /*--- Function export code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   if (PyType_Ready(&__pyx_type_7pystemd_6daemon___pyx_scope_struct__notify) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_7pystemd_6daemon___pyx_scope_struct__notify.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7pystemd_6daemon___pyx_scope_struct__notify.tp_dictoffset && __pyx_type_7pystemd_6daemon___pyx_scope_struct__notify.tp_getattro == PyObject_GenericGetAttr)) {
@@ -2877,25 +2919,27 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
-#if PY_MAJOR_VERSION < 3
-#ifdef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC void
-#else
+#ifndef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
+#elif PY_MAJOR_VERSION < 3
+#ifdef __cplusplus
+#define __Pyx_PyMODINIT_FUNC extern "C" void
+#else
+#define __Pyx_PyMODINIT_FUNC void
 #endif
 #else
-#ifdef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC PyObject *
+#ifdef __cplusplus
+#define __Pyx_PyMODINIT_FUNC extern "C" PyObject *
 #else
-#define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
+#define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
 __Pyx_PyMODINIT_FUNC initdaemon(void) CYTHON_SMALL_CODE; /*proto*/
 __Pyx_PyMODINIT_FUNC initdaemon(void)
@@ -2972,14 +3016,17 @@
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module 'daemon' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
@@ -3060,22 +3107,22 @@
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "pystemd.daemon")) {
       if (unlikely(PyDict_SetItemString(modules, "pystemd.daemon", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
-  if (__Pyx_InitCachedBuiltins() < 0) goto __pyx_L1_error;
+  if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
-  if (__Pyx_InitCachedConstants() < 0) goto __pyx_L1_error;
+  if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
-  if (unlikely(__Pyx_modinit_type_init_code() != 0)) goto __pyx_L1_error;
+  if (unlikely(__Pyx_modinit_type_init_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
@@ -3272,15 +3319,15 @@
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
             continue;
         }
         name = first_kw_arg;
         #if PY_MAJOR_VERSION < 3
-        if (likely(PyString_CheckExact(key)) || likely(PyString_Check(key))) {
+        if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
                     break;
                 }
                 name++;
@@ -3299,15 +3346,15 @@
             }
         } else
         #endif
         if (likely(PyUnicode_Check(key))) {
             while (*name) {
                 int cmp = (**name == key) ? 0 :
                 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                    (PyUnicode_GET_SIZE(**name) != PyUnicode_GET_SIZE(key)) ? 1 :
+                    (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
                     PyUnicode_Compare(**name, key);
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
                     break;
                 }
@@ -3315,15 +3362,15 @@
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
                 while (argname != first_kw_arg) {
                     int cmp = (**argname == key) ? 0 :
                     #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                        (PyUnicode_GET_SIZE(**argname) != PyUnicode_GET_SIZE(key)) ? 1 :
+                        (__Pyx_PyUnicode_GET_LENGTH(**argname) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                     #endif
                         PyUnicode_Compare(**argname, key);
                     if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                     if (cmp == 0) goto arg_passed_twice;
                     argname++;
                 }
             }
@@ -4358,15 +4405,15 @@
         goto bad;
     empty_dict = PyDict_New();
     if (!empty_dict)
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
-            if (strchr(__Pyx_MODULE_NAME, '.')) {
+            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
                 module = PyImport_ImportModuleLevelObject(
                     name, global_dict, empty_dict, list, 1);
                 if (!module) {
                     if (!PyErr_ExceptionMatches(PyExc_ImportError))
                         goto bad;
                     PyErr_Clear();
                 }
@@ -4515,15 +4562,15 @@
     }
     Py_XDECREF(owned_metaclass);
     return result;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -4619,15 +4666,15 @@
         entries[pos].code_object = code_object;
         Py_DECREF(tmp);
         return;
     }
     if (__pyx_code_cache.count == __pyx_code_cache.max_count) {
         int new_max = __pyx_code_cache.max_count + 64;
         entries = (__Pyx_CodeObjectCacheEntry*)PyMem_Realloc(
-            __pyx_code_cache.entries, (size_t)new_max*sizeof(__Pyx_CodeObjectCacheEntry));
+            __pyx_code_cache.entries, ((size_t)new_max) * sizeof(__Pyx_CodeObjectCacheEntry));
         if (unlikely(!entries)) {
             return;
         }
         __pyx_code_cache.entries = entries;
         __pyx_code_cache.max_count = new_max;
     }
     for (i=__pyx_code_cache.count; i>pos; i--) {
```

### Comparing `pystemd-0.7.0/pystemd/daemon.pyx` & `pystemd-0.8.0/pystemd/daemon.pyx`

 * *Files identical despite different names*

### Comparing `pystemd-0.7.0/pystemd/dbusexc.c` & `pystemd-0.8.0/pystemd/dbusexc.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.14 */
+/* Generated by Cython 0.29.21 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "libraries": [
             "systemd"
         ],
@@ -18,16 +18,16 @@
 #define PY_SSIZE_T_CLEAN
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_14"
-#define CYTHON_HEX_VERSION 0x001D0EF0
+#define CYTHON_ABI "0_29_21"
+#define CYTHON_HEX_VERSION 0x001D15F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -446,15 +446,19 @@
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
+  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #else
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+  #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
@@ -495,26 +499,35 @@
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBaseString_Type            PyUnicode_Type
   #define PyStringObject               PyUnicodeObject
   #define PyString_Type                PyUnicode_Type
   #define PyString_Check               PyUnicode_Check
   #define PyString_CheckExact          PyUnicode_CheckExact
+#ifndef PyObject_Unicode
   #define PyObject_Unicode             PyObject_Str
 #endif
+#endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
 #ifndef PySet_CheckExact
   #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
 #endif
+#if PY_VERSION_HEX >= 0x030900A4
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
+#else
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
+#endif
 #if CYTHON_ASSUME_SAFE_MACROS
   #define __Pyx_PySequence_SIZE(seq)  Py_SIZE(seq)
 #else
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
@@ -546,15 +559,15 @@
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
   #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
   #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? PyMethod_New(func, self) : (Py_INCREF(func), func))
+  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
@@ -587,19 +600,18 @@
 #endif
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
-
+#define __PYX_MARK_ERR_POS(f_index, lineno) \
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
-{ \
-  __pyx_filename = __pyx_f[f_index]; __pyx_lineno = lineno; __pyx_clineno = __LINE__; goto Ln_error; \
-}
+    { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifndef __PYX_EXTERN_C
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
@@ -1058,15 +1070,15 @@
 
 /* CalculateMetaclass.proto */
 static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases);
 
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 
-/* CythonFunction.proto */
+/* CythonFunctionShared.proto */
 #define __Pyx_CyFunction_USED 1
 #define __Pyx_CYFUNCTION_STATICMETHOD  0x01
 #define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
 #define __Pyx_CYFUNCTION_CCLASS        0x04
 #define __Pyx_CyFunction_GetClosure(f)\
     (((__pyx_CyFunctionObject *) (f))->func_closure)
 #define __Pyx_CyFunction_GetClassObj(f)\
@@ -1086,25 +1098,24 @@
     PyObject *func_doc;
     PyObject *func_globals;
     PyObject *func_code;
     PyObject *func_closure;
     PyObject *func_classobj;
     void *defaults;
     int defaults_pyobjects;
+    size_t defaults_size;  // used by FusedFunction for copying defaults
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
 } __pyx_CyFunctionObject;
 static PyTypeObject *__pyx_CyFunctionType = 0;
 #define __Pyx_CyFunction_Check(obj)  (__Pyx_TypeCheck(obj, __pyx_CyFunctionType))
-#define __Pyx_CyFunction_NewEx(ml, flags, qualname, self, module, globals, code)\
-    __Pyx_CyFunction_New(__pyx_CyFunctionType, ml, flags, qualname, self, module, globals, code)
-static PyObject *__Pyx_CyFunction_New(PyTypeObject *, PyMethodDef *ml,
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *self,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
                                                          size_t size,
                                                          int pyobjects);
@@ -1112,14 +1123,21 @@
                                                             PyObject *tuple);
 static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *m,
                                                              PyObject *dict);
 static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *m,
                                                               PyObject *dict);
 static int __pyx_CyFunction_init(void);
 
+/* CythonFunction.proto */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+
 /* SetNameInClass.proto */
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
 #define __Pyx_SetNameInClass(ns, name, value)\
     (likely(PyDict_CheckExact(ns)) ? _PyDict_SetItem_KnownHash(ns, name, value, ((PyASCIIObject *) name)->hash) : PyObject_SetItem(ns, name, value))
 #elif CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_SetNameInClass(ns, name, value)\
     (likely(PyDict_CheckExact(ns)) ? PyDict_SetItem(ns, name, value) : PyObject_SetItem(ns, name, value))
@@ -1458,14 +1476,17 @@
 static PyObject *__pyx_pw_7pystemd_7dbusexc_13DBusBaseError_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_7pystemd_7dbusexc_13DBusBaseError_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pystemd_7dbusexc_13DBusBaseError_1__init__, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_7pystemd_7dbusexc_13DBusBaseError_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_errno = 0;
   PyObject *__pyx_v_err_name = 0;
   PyObject *__pyx_v_err_message = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_errno,&__pyx_n_s_err_name,&__pyx_n_s_err_message,0};
     PyObject* values[4] = {0,0,0,0};
     values[2] = ((PyObject *)((PyObject *)Py_None));
@@ -1554,14 +1575,17 @@
   int __pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   Py_ssize_t __pyx_t_6;
   Py_UCS4 __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
   /* "pystemd/dbusexc.pyx":16
  * class DBusBaseError(Exception):
  *     def __init__(self, errno, err_name=None, err_message=None):
  *       is_base_error = self.__class__.__name__ == 'DBusBaseError'             # <<<<<<<<<<<<<<
  *       custom_msg = (
@@ -1815,14 +1839,17 @@
 /* Python wrapper */
 static PyObject *__pyx_pw_7pystemd_7dbusexc_1DBusError(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_7pystemd_7dbusexc_1DBusError = {"DBusError", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pystemd_7dbusexc_1DBusError, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_7pystemd_7dbusexc_1DBusError(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_err_no = 0;
   PyObject *__pyx_v_err_name = 0;
   PyObject *__pyx_v_err_message = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("DBusError (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_err_no,&__pyx_n_s_err_name,&__pyx_n_s_err_message,0};
     PyObject* values[3] = {0,0,0};
     values[1] = ((PyObject *)Py_None);
@@ -1895,14 +1922,17 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("DBusError", 0);
 
   /* "pystemd/dbusexc.pyx":214
  * 
  * def DBusError(err_no, err_name=None, err_message=""):
  *     return DBUS_ERROR_MAP.get(             # <<<<<<<<<<<<<<
  *         err_name, OS_ERROR_MAP.get(err_no, DBusBaseError)
@@ -2291,25 +2321,27 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
-#if PY_MAJOR_VERSION < 3
-#ifdef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC void
-#else
+#ifndef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
+#elif PY_MAJOR_VERSION < 3
+#ifdef __cplusplus
+#define __Pyx_PyMODINIT_FUNC extern "C" void
+#else
+#define __Pyx_PyMODINIT_FUNC void
 #endif
 #else
-#ifdef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC PyObject *
+#ifdef __cplusplus
+#define __Pyx_PyMODINIT_FUNC extern "C" PyObject *
 #else
-#define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
+#define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
 __Pyx_PyMODINIT_FUNC initdbusexc(void) CYTHON_SMALL_CODE; /*proto*/
 __Pyx_PyMODINIT_FUNC initdbusexc(void)
@@ -2386,14 +2418,17 @@
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module 'dbusexc' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
@@ -2474,17 +2509,17 @@
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "pystemd.dbusexc")) {
       if (unlikely(PyDict_SetItemString(modules, "pystemd.dbusexc", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
-  if (__Pyx_InitCachedBuiltins() < 0) goto __pyx_L1_error;
+  if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
-  if (__Pyx_InitCachedConstants() < 0) goto __pyx_L1_error;
+  if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
   (void)__Pyx_modinit_type_init_code();
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
@@ -2526,15 +2561,15 @@
   /* "pystemd/dbusexc.pyx":15
  * 
  * class DBusBaseError(Exception):
  *     def __init__(self, errno, err_name=None, err_message=None):             # <<<<<<<<<<<<<<
  *       is_base_error = self.__class__.__name__ == 'DBusBaseError'
  *       custom_msg = (
  */
-  __pyx_t_4 = __Pyx_CyFunction_NewEx(&__pyx_mdef_7pystemd_7dbusexc_13DBusBaseError_1__init__, 0, __pyx_n_s_DBusBaseError___init, NULL, __pyx_n_s_pystemd_dbusexc, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pystemd_7dbusexc_13DBusBaseError_1__init__, 0, __pyx_n_s_DBusBaseError___init, NULL, __pyx_n_s_pystemd_dbusexc, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__5);
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "pystemd/dbusexc.pyx":14
  * 
@@ -4043,15 +4078,15 @@
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
             continue;
         }
         name = first_kw_arg;
         #if PY_MAJOR_VERSION < 3
-        if (likely(PyString_CheckExact(key)) || likely(PyString_Check(key))) {
+        if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
                     break;
                 }
                 name++;
@@ -4070,15 +4105,15 @@
             }
         } else
         #endif
         if (likely(PyUnicode_Check(key))) {
             while (*name) {
                 int cmp = (**name == key) ? 0 :
                 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                    (PyUnicode_GET_SIZE(**name) != PyUnicode_GET_SIZE(key)) ? 1 :
+                    (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
                     PyUnicode_Compare(**name, key);
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
                     break;
                 }
@@ -4086,15 +4121,15 @@
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
                 while (argname != first_kw_arg) {
                     int cmp = (**argname == key) ? 0 :
                     #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                        (PyUnicode_GET_SIZE(**argname) != PyUnicode_GET_SIZE(key)) ? 1 :
+                        (__Pyx_PyUnicode_GET_LENGTH(**argname) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                     #endif
                         PyUnicode_Compare(**argname, key);
                     if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                     if (cmp == 0) goto arg_passed_twice;
                     argname++;
                 }
             }
@@ -4725,15 +4760,15 @@
         goto bad;
     empty_dict = PyDict_New();
     if (!empty_dict)
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
-            if (strchr(__Pyx_MODULE_NAME, '.')) {
+            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
                 module = PyImport_ImportModuleLevelObject(
                     name, global_dict, empty_dict, list, 1);
                 if (!module) {
                     if (!PyErr_ExceptionMatches(PyExc_ImportError))
                         goto bad;
                     PyErr_Clear();
                 }
@@ -4838,15 +4873,15 @@
     return cached_type;
 bad:
     Py_XDECREF(cached_type);
     cached_type = NULL;
     goto done;
 }
 
-/* CythonFunction */
+/* CythonFunctionShared */
 #include <structmember.h>
 static PyObject *
 __Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, CYTHON_UNUSED void *closure)
 {
     if (unlikely(op->func_doc == NULL)) {
         if (op->func.m_ml->ml_doc) {
 #if PY_MAJOR_VERSION >= 3
@@ -5145,18 +5180,17 @@
     {0, 0, 0, 0}
 };
 #if PY_VERSION_HEX < 0x030500A0
 #define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func_weakreflist)
 #else
 #define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func.m_weakreflist)
 #endif
-static PyObject *__Pyx_CyFunction_New(PyTypeObject *type, PyMethodDef *ml, int flags, PyObject* qualname,
-                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
-    __pyx_CyFunctionObject *op = PyObject_GC_New(__pyx_CyFunctionObject, type);
-    if (op == NULL)
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject *op, PyMethodDef *ml, int flags, PyObject* qualname,
+                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    if (unlikely(op == NULL))
         return NULL;
     op->flags = flags;
     __Pyx_CyFunction_weakreflist(op) = NULL;
     op->func.m_ml = ml;
     op->func.m_self = (PyObject *) op;
     Py_XINCREF(closure);
     op->func_closure = closure;
@@ -5169,20 +5203,20 @@
     op->func_doc = NULL;
     op->func_classobj = NULL;
     op->func_globals = globals;
     Py_INCREF(op->func_globals);
     Py_XINCREF(code);
     op->func_code = code;
     op->defaults_pyobjects = 0;
+    op->defaults_size = 0;
     op->defaults = NULL;
     op->defaults_tuple = NULL;
     op->defaults_kwdict = NULL;
     op->defaults_getter = NULL;
     op->func_annotations = NULL;
-    PyObject_GC_Track(op);
     return (PyObject *) op;
 }
 static int
 __Pyx_CyFunction_clear(__pyx_CyFunctionObject *m)
 {
     Py_CLEAR(m->func_closure);
     Py_CLEAR(m->func.m_module);
@@ -5237,26 +5271,28 @@
         for (i = 0; i < m->defaults_pyobjects; i++)
             Py_VISIT(pydefaults[i]);
     }
     return 0;
 }
 static PyObject *__Pyx_CyFunction_descr_get(PyObject *func, PyObject *obj, PyObject *type)
 {
+#if PY_MAJOR_VERSION < 3
     __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
     if (m->flags & __Pyx_CYFUNCTION_STATICMETHOD) {
         Py_INCREF(func);
         return func;
     }
     if (m->flags & __Pyx_CYFUNCTION_CLASSMETHOD) {
         if (type == NULL)
             type = (PyObject *)(Py_TYPE(obj));
         return __Pyx_PyMethod_New(func, type, (PyObject *)(Py_TYPE(type)));
     }
     if (obj == Py_None)
         obj = NULL;
+#endif
     return __Pyx_PyMethod_New(func, obj, type);
 }
 static PyObject*
 __Pyx_CyFunction_repr(__pyx_CyFunctionObject *op)
 {
 #if PY_MAJOR_VERSION >= 3
     return PyUnicode_FromFormat("<cyfunction %U at %p>",
@@ -5422,14 +5458,15 @@
 static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *func, size_t size, int pyobjects) {
     __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
     m->defaults = PyObject_Malloc(size);
     if (unlikely(!m->defaults))
         return PyErr_NoMemory();
     memset(m->defaults, 0, size);
     m->defaults_pyobjects = pyobjects;
+    m->defaults_size = size;
     return m->defaults;
 }
 static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *func, PyObject *tuple) {
     __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
     m->defaults_tuple = tuple;
     Py_INCREF(tuple);
 }
@@ -5440,14 +5477,27 @@
 }
 static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
     __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
     m->func_annotations = dict;
     Py_INCREF(dict);
 }
 
+/* CythonFunction */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
+                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyObject *op = __Pyx_CyFunction_Init(
+        PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
+        ml, flags, qualname, closure, module, globals, code
+    );
+    if (likely(op)) {
+        PyObject_GC_Track(op);
+    }
+    return op;
+}
+
 /* Py3ClassCreate */
 static PyObject *__Pyx_Py3MetaclassPrepare(PyObject *metaclass, PyObject *bases, PyObject *name,
                                            PyObject *qualname, PyObject *mkw, PyObject *modname, PyObject *doc) {
     PyObject *ns;
     if (metaclass) {
         PyObject *prep = __Pyx_PyObject_GetAttrStr(metaclass, __pyx_n_s_prepare);
         if (prep) {
@@ -5533,15 +5583,15 @@
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
 }
 #endif
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -5637,15 +5687,15 @@
         entries[pos].code_object = code_object;
         Py_DECREF(tmp);
         return;
     }
     if (__pyx_code_cache.count == __pyx_code_cache.max_count) {
         int new_max = __pyx_code_cache.max_count + 64;
         entries = (__Pyx_CodeObjectCacheEntry*)PyMem_Realloc(
-            __pyx_code_cache.entries, (size_t)new_max*sizeof(__Pyx_CodeObjectCacheEntry));
+            __pyx_code_cache.entries, ((size_t)new_max) * sizeof(__Pyx_CodeObjectCacheEntry));
         if (unlikely(!entries)) {
             return;
         }
         __pyx_code_cache.entries = entries;
         __pyx_code_cache.max_count = new_max;
     }
     for (i=__pyx_code_cache.count; i>pos; i--) {
```

### Comparing `pystemd-0.7.0/pystemd/dbusexc.pyx` & `pystemd-0.8.0/pystemd/dbusexc.pyx`

 * *Files identical despite different names*

### Comparing `pystemd-0.7.0/pystemd/dbuslib.c` & `pystemd-0.8.0/pystemd/dbuslib.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.14 */
+/* Generated by Cython 0.29.21 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "libraries": [
             "systemd"
@@ -19,16 +19,16 @@
 #define PY_SSIZE_T_CLEAN
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_14"
-#define CYTHON_HEX_VERSION 0x001D0EF0
+#define CYTHON_ABI "0_29_21"
+#define CYTHON_HEX_VERSION 0x001D15F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -447,15 +447,19 @@
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
+  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #else
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+  #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
@@ -496,26 +500,35 @@
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBaseString_Type            PyUnicode_Type
   #define PyStringObject               PyUnicodeObject
   #define PyString_Type                PyUnicode_Type
   #define PyString_Check               PyUnicode_Check
   #define PyString_CheckExact          PyUnicode_CheckExact
+#ifndef PyObject_Unicode
   #define PyObject_Unicode             PyObject_Str
 #endif
+#endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
 #ifndef PySet_CheckExact
   #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
 #endif
+#if PY_VERSION_HEX >= 0x030900A4
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
+#else
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
+#endif
 #if CYTHON_ASSUME_SAFE_MACROS
   #define __Pyx_PySequence_SIZE(seq)  Py_SIZE(seq)
 #else
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
@@ -547,15 +560,15 @@
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
   #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
   #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? PyMethod_New(func, self) : (Py_INCREF(func), func))
+  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
@@ -588,19 +601,18 @@
 #endif
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
-
+#define __PYX_MARK_ERR_POS(f_index, lineno) \
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
-{ \
-  __pyx_filename = __pyx_f[f_index]; __pyx_lineno = lineno; __pyx_clineno = __LINE__; goto Ln_error; \
-}
+    { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifndef __PYX_EXTERN_C
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
@@ -1196,15 +1208,15 @@
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
         Py_INCREF(x);
         PyList_SET_ITEM(list, len, x);
-        Py_SIZE(list) = len+1;
+        __Pyx_SET_SIZE(list, len + 1);
         return 0;
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
@@ -1388,15 +1400,15 @@
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len)) {
         Py_INCREF(x);
         PyList_SET_ITEM(list, len, x);
-        Py_SIZE(list) = len+1;
+        __Pyx_SET_SIZE(list, len + 1);
         return 0;
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
 #endif
@@ -1519,15 +1531,15 @@
 #else
 static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 
-/* CythonFunction.proto */
+/* CythonFunctionShared.proto */
 #define __Pyx_CyFunction_USED 1
 #define __Pyx_CYFUNCTION_STATICMETHOD  0x01
 #define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
 #define __Pyx_CYFUNCTION_CCLASS        0x04
 #define __Pyx_CyFunction_GetClosure(f)\
     (((__pyx_CyFunctionObject *) (f))->func_closure)
 #define __Pyx_CyFunction_GetClassObj(f)\
@@ -1547,25 +1559,24 @@
     PyObject *func_doc;
     PyObject *func_globals;
     PyObject *func_code;
     PyObject *func_closure;
     PyObject *func_classobj;
     void *defaults;
     int defaults_pyobjects;
+    size_t defaults_size;  // used by FusedFunction for copying defaults
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
 } __pyx_CyFunctionObject;
 static PyTypeObject *__pyx_CyFunctionType = 0;
 #define __Pyx_CyFunction_Check(obj)  (__Pyx_TypeCheck(obj, __pyx_CyFunctionType))
-#define __Pyx_CyFunction_NewEx(ml, flags, qualname, self, module, globals, code)\
-    __Pyx_CyFunction_New(__pyx_CyFunctionType, ml, flags, qualname, self, module, globals, code)
-static PyObject *__Pyx_CyFunction_New(PyTypeObject *, PyMethodDef *ml,
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *self,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
                                                          size_t size,
                                                          int pyobjects);
@@ -1573,14 +1584,21 @@
                                                             PyObject *tuple);
 static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *m,
                                                              PyObject *dict);
 static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *m,
                                                               PyObject *dict);
 static int __pyx_CyFunction_init(void);
 
+/* CythonFunction.proto */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+
 /* SliceObject.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetSlice(
         PyObject* obj, Py_ssize_t cstart, Py_ssize_t cstop,
         PyObject** py_start, PyObject** py_stop, PyObject** py_slice,
         int has_cstart, int has_cstop, int wraparound);
 
 /* ListExtend.proto */
@@ -1654,14 +1672,17 @@
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
+/* PyObjectGetAttrStrNoError.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
+
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
@@ -2367,14 +2388,17 @@
 /* Python wrapper */
 static PyObject *__pyx_pw_7pystemd_7dbuslib_14VariableReturn_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_7pystemd_7dbuslib_14VariableReturn_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pystemd_7dbuslib_14VariableReturn_1__init__, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_7pystemd_7dbuslib_14VariableReturn_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_parent = 0;
   PyObject *__pyx_v_v_type = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_parent,&__pyx_n_s_v_type,0};
     PyObject* values[3] = {0,0,0};
     values[1] = ((PyObject *)((PyObject *)Py_None));
@@ -2443,14 +2467,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_14VariableReturn___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_parent, PyObject *__pyx_v_v_type) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
   /* "pystemd/dbuslib.pyx":40
  * class VariableReturn(object):
  *   def __init__(self, parent=None, v_type=None):
  *     self.data = []             # <<<<<<<<<<<<<<
  *     self.parent = parent
@@ -2510,14 +2537,17 @@
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7pystemd_7dbuslib_14VariableReturn_3create_child(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_7pystemd_7dbuslib_14VariableReturn_3create_child = {"create_child", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pystemd_7dbuslib_14VariableReturn_3create_child, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_7pystemd_7dbuslib_14VariableReturn_3create_child(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_v_type = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("create_child (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_v_type,0};
     PyObject* values[2] = {0,0};
     values[1] = ((PyObject *)((PyObject *)Py_None));
@@ -2578,14 +2608,17 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("create_child", 0);
 
   /* "pystemd/dbuslib.pyx":45
  * 
  *   def create_child(self, v_type=None):
  *     self.data.append(             # <<<<<<<<<<<<<<
  *       VariableReturn(
@@ -2696,14 +2729,17 @@
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7pystemd_7dbuslib_14VariableReturn_5append(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_7pystemd_7dbuslib_14VariableReturn_5append = {"append", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pystemd_7dbuslib_14VariableReturn_5append, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_7pystemd_7dbuslib_14VariableReturn_5append(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_dt = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("append (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_dt,0};
     PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
@@ -2757,14 +2793,17 @@
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_14VariableReturn_4append(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_dt) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("append", 0);
 
   /* "pystemd/dbuslib.pyx":53
  * 
  *   def append(self, dt):
  *     self.data.append(dt)             # <<<<<<<<<<<<<<
  * 
@@ -2827,14 +2866,17 @@
  * 
  */
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_14VariableReturn_4dump_genexpr(PyObject *__pyx_self) {
   struct __pyx_obj_7pystemd_7dbuslib___pyx_scope_struct_1_genexpr *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_7pystemd_7dbuslib___pyx_scope_struct_1_genexpr *)__pyx_tp_new_7pystemd_7dbuslib___pyx_scope_struct_1_genexpr(__pyx_ptype_7pystemd_7dbuslib___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_7pystemd_7dbuslib___pyx_scope_struct_1_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 67, __pyx_L1_error)
   } else {
@@ -2868,14 +2910,17 @@
   Py_ssize_t __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("genexpr", 0);
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L8_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
@@ -2993,14 +3038,17 @@
   PyObject *(*__pyx_t_5)(PyObject *);
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   int __pyx_t_11;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dump", 0);
   __pyx_cur_scope = (struct __pyx_obj_7pystemd_7dbuslib___pyx_scope_struct__dump *)__pyx_tp_new_7pystemd_7dbuslib___pyx_scope_struct__dump(__pyx_ptype_7pystemd_7dbuslib___pyx_scope_struct__dump, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_7pystemd_7dbuslib___pyx_scope_struct__dump *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 55, __pyx_L1_error)
   } else {
@@ -3483,14 +3531,17 @@
  *         assert self._msg == NULL
  *         self._msg = msg
  */
 
 static PyObject *__pyx_f_7pystemd_7dbuslib_11DbusMessage_set_bus_message(struct __pyx_obj_7pystemd_7dbuslib_DbusMessage *__pyx_v_self, sd_bus_message *__pyx_v_msg) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_bus_message", 0);
 
   /* "pystemd/dbuslib.pyx":87
  * 
  *     cdef set_bus_message(self, dbusc.sd_bus_message *msg):
  *         assert self._msg == NULL             # <<<<<<<<<<<<<<
  *         self._msg = msg
@@ -3568,14 +3619,17 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_t_7;
   int __pyx_t_8;
   int __pyx_t_9;
   Py_ssize_t __pyx_t_10;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("process_reply", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
@@ -4767,14 +4821,17 @@
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7pystemd_7dbuslib_11DbusMessage_3process_reply(PyObject *__pyx_v_self, PyObject *__pyx_arg_with_headers); /*proto*/
 static char __pyx_doc_7pystemd_7dbuslib_11DbusMessage_2process_reply[] = "\n          Read through a sd_bus_message reply object and return the answer to that call.\n          It's loosely based on bus_message_dump in           https://github.com/systemd/systemd/blob/master/src/libsystemd/sd-bus/bus-dump.c\n          except that will dump to stdout, this will give you a nice python array (you\n          are welcome!).\n\n          The nice thing about this method, is that it will enter complex types like\n          arrays or struc. so if the answer is in the form of \"a(sbi)\", it can return\n          as an answer [[b'a', True, 0], [b'b', False, 1], ...]\n        ";
 static PyObject *__pyx_pw_7pystemd_7dbuslib_11DbusMessage_3process_reply(PyObject *__pyx_v_self, PyObject *__pyx_arg_with_headers) {
   bool __pyx_v_with_headers;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("process_reply (wrapper)", 0);
   assert(__pyx_arg_with_headers); {
     __pyx_v_with_headers = __Pyx_PyObject_IsTrue(__pyx_arg_with_headers); if (unlikely((__pyx_v_with_headers == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 91, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
@@ -4790,14 +4847,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_11DbusMessage_2process_reply(struct __pyx_obj_7pystemd_7dbuslib_DbusMessage *__pyx_v_self, bool __pyx_v_with_headers) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("process_reply", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_f_7pystemd_7dbuslib_11DbusMessage_process_reply(__pyx_v_self, __pyx_v_with_headers, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -4826,14 +4886,17 @@
   bool __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   bool __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_empty", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
@@ -4922,14 +4985,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_11DbusMessage_4is_empty(struct __pyx_obj_7pystemd_7dbuslib_DbusMessage *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_empty", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_7pystemd_7dbuslib_11DbusMessage_is_empty(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -4962,14 +5028,17 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   bool __pyx_t_9;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_signal", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
@@ -5087,14 +5156,17 @@
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7pystemd_7dbuslib_11DbusMessage_7is_signal(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_7pystemd_7dbuslib_11DbusMessage_7is_signal(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   char const *__pyx_v_interface;
   char const *__pyx_v_member;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_signal (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_interface,&__pyx_n_s_member,0};
     PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
@@ -5147,14 +5219,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_11DbusMessage_6is_signal(struct __pyx_obj_7pystemd_7dbuslib_DbusMessage *__pyx_v_self, char const *__pyx_v_interface, char const *__pyx_v_member) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_signal", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_7pystemd_7dbuslib_11DbusMessage_is_signal(__pyx_v_self, __pyx_v_interface, __pyx_v_member, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -5184,14 +5259,17 @@
   uint8_t __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   uint8_t __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_type", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
@@ -5289,14 +5367,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_11DbusMessage_8get_type(struct __pyx_obj_7pystemd_7dbuslib_DbusMessage *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_type", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_uint8_t(__pyx_f_7pystemd_7dbuslib_11DbusMessage_get_type(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -5326,14 +5407,17 @@
   uint64_t __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   uint64_t __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_cookie", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
@@ -5431,14 +5515,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_11DbusMessage_10get_cookie(struct __pyx_obj_7pystemd_7dbuslib_DbusMessage *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_cookie", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_uint64_t(__pyx_f_7pystemd_7dbuslib_11DbusMessage_get_cookie(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -5468,14 +5555,17 @@
   uint64_t __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   uint64_t __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_reply_cookie", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
@@ -5573,14 +5663,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_11DbusMessage_12get_reply_cookie(struct __pyx_obj_7pystemd_7dbuslib_DbusMessage *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_reply_cookie", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_uint64_t(__pyx_f_7pystemd_7dbuslib_11DbusMessage_get_reply_cookie(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -5610,14 +5703,17 @@
   int64_t __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int64_t __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_priority", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
@@ -5715,14 +5811,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_11DbusMessage_14get_priority(struct __pyx_obj_7pystemd_7dbuslib_DbusMessage *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_priority", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_int64_t(__pyx_f_7pystemd_7dbuslib_11DbusMessage_get_priority(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -5751,14 +5850,17 @@
   char const *__pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   char const *__pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_path", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
@@ -5847,14 +5949,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_11DbusMessage_16get_path(struct __pyx_obj_7pystemd_7dbuslib_DbusMessage *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_path", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_f_7pystemd_7dbuslib_11DbusMessage_get_path(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 261, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -5883,14 +5988,17 @@
   char const *__pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   char const *__pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_interface", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
@@ -5979,14 +6087,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_11DbusMessage_18get_interface(struct __pyx_obj_7pystemd_7dbuslib_DbusMessage *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_interface", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_f_7pystemd_7dbuslib_11DbusMessage_get_interface(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 264, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -6015,14 +6126,17 @@
   char const *__pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   char const *__pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_member", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
@@ -6111,14 +6225,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_11DbusMessage_20get_member(struct __pyx_obj_7pystemd_7dbuslib_DbusMessage *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_member", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_f_7pystemd_7dbuslib_11DbusMessage_get_member(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -6147,14 +6264,17 @@
   char const *__pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   char const *__pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_destination", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
@@ -6243,14 +6363,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_11DbusMessage_22get_destination(struct __pyx_obj_7pystemd_7dbuslib_DbusMessage *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_destination", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_f_7pystemd_7dbuslib_11DbusMessage_get_destination(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -6279,14 +6402,17 @@
   char const *__pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   char const *__pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_sender", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
@@ -6375,14 +6501,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_11DbusMessage_24get_sender(struct __pyx_obj_7pystemd_7dbuslib_DbusMessage *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_sender", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_f_7pystemd_7dbuslib_11DbusMessage_get_sender(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -6543,14 +6672,17 @@
   return __pyx_r;
 }
 
 static int __pyx_pf_7pystemd_7dbuslib_11DbusMessage_7headers_2__set__(struct __pyx_obj_7pystemd_7dbuslib_DbusMessage *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
   if (!(likely(PyDict_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_v_value)->tp_name), 0))) __PYX_ERR(0, 75, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_value;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->headers);
   __Pyx_DECREF(__pyx_v_self->headers);
@@ -6617,14 +6749,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_11DbusMessage_26__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7pystemd_7dbuslib_DbusMessage *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self._msg cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._msg cannot be converted to a Python object for pickling")
@@ -6671,14 +6806,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_11DbusMessage_28__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7pystemd_7dbuslib_DbusMessage *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("self._msg cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._msg cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
@@ -6713,14 +6851,17 @@
  * 
  */
 
 /* Python wrapper */
 static int __pyx_pw_7pystemd_7dbuslib_4DBus_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_7pystemd_7dbuslib_4DBus_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_user_mode = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_user_mode,0};
     PyObject* values[1] = {0};
     values[0] = ((PyObject *)Py_False);
@@ -6769,14 +6910,17 @@
   return __pyx_r;
 }
 
 static int __pyx_pf_7pystemd_7dbuslib_4DBus___init__(struct __pyx_obj_7pystemd_7dbuslib_DBus *__pyx_v_self, PyObject *__pyx_v_user_mode) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   bool __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
   /* "pystemd/dbuslib.pyx":282
  * 
  *     def __init__(self, user_mode=False):
  *       self.user_mode = user_mode             # <<<<<<<<<<<<<<
  * 
@@ -6827,14 +6971,17 @@
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_4DBus_2__enter__(struct __pyx_obj_7pystemd_7dbuslib_DBus *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__enter__", 0);
 
   /* "pystemd/dbuslib.pyx":285
  * 
  *     def __enter__(self):
  *         self.open()             # <<<<<<<<<<<<<<
  *         return self
@@ -6920,14 +7067,17 @@
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_4DBus_4__exit__(struct __pyx_obj_7pystemd_7dbuslib_DBus *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_errs) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__exit__", 0);
 
   /* "pystemd/dbuslib.pyx":289
  * 
  *     def __exit__(self, *errs):
  *         self.close()             # <<<<<<<<<<<<<<
  * 
@@ -7072,14 +7222,17 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("open", 0);
 
   /* "pystemd/dbuslib.pyx":301
  *     def open(self):
  *         cdef int rets
  *         rets = self.open_dbus_bus()             # <<<<<<<<<<<<<<
  *         if (rets < 0):
@@ -7284,14 +7437,17 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("process", 0);
 
   /* "pystemd/dbuslib.pyx":312
  *         cdef:
  *             int r
  *             DbusMessage msg = DbusMessage()             # <<<<<<<<<<<<<<
  * 
@@ -7463,14 +7619,17 @@
   double __pyx_t_14;
   int __pyx_t_15;
   int __pyx_t_16;
   Py_ssize_t __pyx_t_17;
   Py_UCS4 __pyx_t_18;
   PyObject *__pyx_t_19 = NULL;
   PyObject *__pyx_t_20 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_msg_append", 0);
 
   /* "pystemd/dbuslib.pyx":324
  * 
  *       cdef char * arg_type_c
  *       cdef char arg_type = <char>arg_type_i             # <<<<<<<<<<<<<<
  * 
@@ -8028,15 +8187,15 @@
   __pyx_t_1 = (__pyx_t_15 != 0);
   if (__pyx_t_1) {
 
     /* "pystemd/dbuslib.pyx":392
  *           msg_call,
  *           arg_type,
  *           <char*>arg_value)             # <<<<<<<<<<<<<<
- *       elif arg_type == -1: # close container
+ *       elif arg_type_i == -1: # close container
  *         r = dbusc.sd_bus_message_close_container(msg_call)
  */
     __pyx_t_5 = __Pyx_PyObject_AsWritableString(__pyx_v_arg_value); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 392, __pyx_L1_error)
 
     /* "pystemd/dbuslib.pyx":389
  *           <int>arg_value)
  *       elif arg_type in CONTAINER_TYPES: # open container
@@ -8055,34 +8214,34 @@
  */
     goto __pyx_L4;
   }
 
   /* "pystemd/dbuslib.pyx":393
  *           arg_type,
  *           <char*>arg_value)
- *       elif arg_type == -1: # close container             # <<<<<<<<<<<<<<
+ *       elif arg_type_i == -1: # close container             # <<<<<<<<<<<<<<
  *         r = dbusc.sd_bus_message_close_container(msg_call)
  *       else:
  */
-  __pyx_t_1 = ((__pyx_v_arg_type == -1L) != 0);
+  __pyx_t_1 = ((__pyx_v_arg_type_i == -1L) != 0);
   if (likely(__pyx_t_1)) {
 
     /* "pystemd/dbuslib.pyx":394
  *           <char*>arg_value)
- *       elif arg_type == -1: # close container
+ *       elif arg_type_i == -1: # close container
  *         r = dbusc.sd_bus_message_close_container(msg_call)             # <<<<<<<<<<<<<<
  *       else:
  *         raise DBusError(
  */
     __pyx_v_r = sd_bus_message_close_container(__pyx_v_msg_call);
 
     /* "pystemd/dbuslib.pyx":393
  *           arg_type,
  *           <char*>arg_value)
- *       elif arg_type == -1: # close container             # <<<<<<<<<<<<<<
+ *       elif arg_type_i == -1: # close container             # <<<<<<<<<<<<<<
  *         r = dbusc.sd_bus_message_close_container(msg_call)
  *       else:
  */
     goto __pyx_L4;
   }
 
   /* "pystemd/dbuslib.pyx":396
@@ -8226,14 +8385,17 @@
 static PyObject *__pyx_pw_7pystemd_7dbuslib_4DBus_13call_method(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_7pystemd_7dbuslib_4DBus_13call_method(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   char const *__pyx_v_destination;
   char const *__pyx_v_path;
   char const *__pyx_v_interface;
   char const *__pyx_v_method;
   PyObject *__pyx_v_args = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("call_method (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_destination,&__pyx_n_s_path,&__pyx_n_s_interface,&__pyx_n_s_method,&__pyx_n_s_args,0};
     PyObject* values[5] = {0,0,0,0,0};
     if (unlikely(__pyx_kwds)) {
@@ -8352,14 +8514,17 @@
   char const *__pyx_t_22;
   PyObject *__pyx_t_23 = NULL;
   PyObject *__pyx_t_24 = NULL;
   PyObject *__pyx_t_25 = NULL;
   PyObject *__pyx_t_26 = NULL;
   PyObject *__pyx_t_27 = NULL;
   PyObject *__pyx_t_28 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("call_method", 0);
 
   /* "pystemd/dbuslib.pyx":411
  *             int arg_type
  * 
  *             dbusc.sd_bus_message *msg_call = NULL             # <<<<<<<<<<<<<<
  *             dbusc.sd_bus_message *msg_reply = NULL
@@ -9072,14 +9237,17 @@
 static PyObject *__pyx_pw_7pystemd_7dbuslib_4DBus_15get_property(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_7pystemd_7dbuslib_4DBus_15get_property(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   char const *__pyx_v_destination;
   char const *__pyx_v_path;
   char const *__pyx_v_interface;
   char const *__pyx_v_property;
   char const *__pyx_v_rtype;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_property (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_destination,&__pyx_n_s_path,&__pyx_n_s_interface,&__pyx_n_s_property,&__pyx_n_s_rtype,0};
     PyObject* values[5] = {0,0,0,0,0};
     if (unlikely(__pyx_kwds)) {
@@ -9174,14 +9342,17 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_property", 0);
 
   /* "pystemd/dbuslib.pyx":462
  *         cdef:
  *           int r
  *           dbusc.sd_bus_error error = dbusc.sd_bus_error(NULL, NULL, 0)             # <<<<<<<<<<<<<<
  * 
@@ -9368,14 +9539,17 @@
 static PyObject *__pyx_pw_7pystemd_7dbuslib_4DBus_17match_signal(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_sender = 0;
   PyObject *__pyx_v_path = 0;
   PyObject *__pyx_v_interface = 0;
   PyObject *__pyx_v_member = 0;
   PyObject *__pyx_v_callback = 0;
   PyObject *__pyx_v_userdata = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("match_signal (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_sender,&__pyx_n_s_path,&__pyx_n_s_interface,&__pyx_n_s_member,&__pyx_n_s_callback,&__pyx_n_s_userdata,0};
     PyObject* values[6] = {0,0,0,0,0,0};
 
@@ -9496,14 +9670,17 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_t_8;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("match_signal", 0);
 
   /* "pystemd/dbuslib.pyx":502
  * 
  *       callback.metadata = {
  *         'userdata': userdata,             # <<<<<<<<<<<<<<
  *       }
@@ -9763,14 +9940,17 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_t_7;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("wait", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
@@ -9933,14 +10113,17 @@
   return __pyx_r;
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7pystemd_7dbuslib_4DBus_19wait(PyObject *__pyx_v_self, PyObject *__pyx_arg_timeout); /*proto*/
 static PyObject *__pyx_pw_7pystemd_7dbuslib_4DBus_19wait(PyObject *__pyx_v_self, PyObject *__pyx_arg_timeout) {
   uint64_t __pyx_v_timeout;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("wait (wrapper)", 0);
   assert(__pyx_arg_timeout); {
     __pyx_v_timeout = __Pyx_PyInt_As_uint64_t(__pyx_arg_timeout); if (unlikely((__pyx_v_timeout == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 521, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
@@ -9956,14 +10139,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_4DBus_18wait(struct __pyx_obj_7pystemd_7dbuslib_DBus *__pyx_v_self, uint64_t __pyx_v_timeout) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("wait", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_f_7pystemd_7dbuslib_4DBus_wait(__pyx_v_self, __pyx_v_timeout, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 521, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -9997,14 +10183,17 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   char const *__pyx_t_5;
   int __pyx_t_6;
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_unique_name", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
@@ -10187,14 +10376,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_4DBus_20get_unique_name(struct __pyx_obj_7pystemd_7dbuslib_DBus *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_unique_name", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_f_7pystemd_7dbuslib_4DBus_get_unique_name(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 526, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -10223,14 +10415,17 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_fd", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
@@ -10319,14 +10514,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_4DBus_22get_fd(struct __pyx_obj_7pystemd_7dbuslib_DBus *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_fd", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_7pystemd_7dbuslib_4DBus_get_fd(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 538, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -10361,14 +10559,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_4DBus_24__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7pystemd_7dbuslib_DBus *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self.bus cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.bus cannot be converted to a Python object for pickling")
@@ -10415,14 +10616,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_4DBus_26__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7pystemd_7dbuslib_DBus *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("self.bus cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.bus cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
@@ -10457,14 +10661,17 @@
  * 
  */
 
 /* Python wrapper */
 static int __pyx_pw_7pystemd_7dbuslib_11DBusMachine_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_7pystemd_7dbuslib_11DBusMachine_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   char *__pyx_v_machine;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_machine,0};
     PyObject* values[1] = {0};
     if (unlikely(__pyx_kwds)) {
@@ -10591,14 +10798,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_11DBusMachine_2__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7pystemd_7dbuslib_DBusMachine *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self.bus cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.bus cannot be converted to a Python object for pickling")
@@ -10645,14 +10855,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_11DBusMachine_4__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7pystemd_7dbuslib_DBusMachine *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("self.bus cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.bus cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
@@ -10687,14 +10900,17 @@
  * 
  */
 
 /* Python wrapper */
 static int __pyx_pw_7pystemd_7dbuslib_10DBusRemote_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_7pystemd_7dbuslib_10DBusRemote_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   char *__pyx_v_host;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_host,0};
     PyObject* values[1] = {0};
     if (unlikely(__pyx_kwds)) {
@@ -10774,14 +10990,17 @@
  */
 
 static int __pyx_f_7pystemd_7dbuslib_10DBusRemote_open_dbus_bus(struct __pyx_obj_7pystemd_7dbuslib_DBusRemote *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   char const *__pyx_t_2;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("open_dbus_bus", 0);
 
   /* "pystemd/dbuslib.pyx":562
  * 
  *   cdef int open_dbus_bus(self):
  *     return dbusc.sd_bus_open_system_remote(&(self.bus), self.remote)             # <<<<<<<<<<<<<<
  * 
@@ -10831,14 +11050,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_10DBusRemote_2__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7pystemd_7dbuslib_DBusRemote *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self.bus cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.bus cannot be converted to a Python object for pickling")
@@ -10885,14 +11107,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_10DBusRemote_4__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7pystemd_7dbuslib_DBusRemote *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("self.bus cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.bus cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
@@ -10928,14 +11153,17 @@
  */
 
 /* Python wrapper */
 static int __pyx_pw_7pystemd_7dbuslib_11DBusAddress_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_7pystemd_7dbuslib_11DBusAddress_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_address = 0;
   PyObject *__pyx_v_peer_to_peer = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_address,&__pyx_n_s_peer_to_peer,0};
     PyObject* values[2] = {0,0};
     values[1] = ((PyObject *)Py_False);
@@ -10993,14 +11221,17 @@
 }
 
 static int __pyx_pf_7pystemd_7dbuslib_11DBusAddress___init__(struct __pyx_obj_7pystemd_7dbuslib_DBusAddress *__pyx_v_self, PyObject *__pyx_v_address, PyObject *__pyx_v_peer_to_peer) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
   /* "pystemd/dbuslib.pyx":570
  * 
  *   def __init__(self, address, peer_to_peer=False):
  *     self.address = bytes(address)             # <<<<<<<<<<<<<<
  *     self.peer_to_peer = int(peer_to_peer)
@@ -11057,14 +11288,17 @@
 
 static int __pyx_f_7pystemd_7dbuslib_11DBusAddress_open_dbus_bus(struct __pyx_obj_7pystemd_7dbuslib_DBusAddress *__pyx_v_self) {
   int __pyx_v_r;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   char const *__pyx_t_2;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("open_dbus_bus", 0);
 
   /* "pystemd/dbuslib.pyx":574
  * 
  *   cdef int open_dbus_bus(self):
  *     r = dbusc.sd_bus_new(&(self.bus))             # <<<<<<<<<<<<<<
  *     if r < 0:
@@ -11285,14 +11519,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_11DBusAddress_2__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7pystemd_7dbuslib_DBusAddress *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self.bus cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.bus cannot be converted to a Python object for pickling")
@@ -11339,14 +11576,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_11DBusAddress_4__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7pystemd_7dbuslib_DBusAddress *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("self.bus cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.bus cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
@@ -11383,14 +11623,17 @@
 
 static PyObject *__pyx_f_7pystemd_7dbuslib_cast_data_to(union __pyx_t_7pystemd_5dbusc_basic_data __pyx_v_basic, PyObject *__pyx_v_cast_type) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("cast_data_to", 0);
 
   /* "pystemd/dbuslib.pyx":601
  *   like the first one more than the second one)
  *   """
  *   if cast_type == dbusc.SD_BUS_TYPE_BYTE:             # <<<<<<<<<<<<<<
  *     return basic.u8
@@ -11923,14 +12166,17 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   char *__pyx_t_3;
   char *__pyx_t_4;
   char *__pyx_t_5;
   char *__pyx_t_6;
   int __pyx_t_7;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("find_closure", 0);
 
   /* "pystemd/dbuslib.pyx":631
  * 
  * cpdef int find_closure(char* args, char open, char close):
  *   cdef int counter = 0             # <<<<<<<<<<<<<<
  *   cdef int n
@@ -12091,14 +12337,17 @@
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7pystemd_7dbuslib_1find_closure(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_7pystemd_7dbuslib_1find_closure(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   char *__pyx_v_args;
   char __pyx_v_open;
   char __pyx_v_close;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("find_closure (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_args,&__pyx_n_s_open,&__pyx_n_s_close,0};
     PyObject* values[3] = {0,0,0};
     if (unlikely(__pyx_kwds)) {
@@ -12161,14 +12410,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_find_closure(CYTHON_UNUSED PyObject *__pyx_self, char *__pyx_v_args, char __pyx_v_open, char __pyx_v_close) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("find_closure", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_7pystemd_7dbuslib_find_closure(__pyx_v_args, __pyx_v_open, __pyx_v_close, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 630, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -12193,14 +12445,17 @@
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7pystemd_7dbuslib_3compile_simple(PyObject *__pyx_self, PyObject *__pyx_arg_arg); /*proto*/
 static PyMethodDef __pyx_mdef_7pystemd_7dbuslib_3compile_simple = {"compile_simple", (PyCFunction)__pyx_pw_7pystemd_7dbuslib_3compile_simple, METH_O, 0};
 static PyObject *__pyx_pw_7pystemd_7dbuslib_3compile_simple(PyObject *__pyx_self, PyObject *__pyx_arg_arg) {
   char *__pyx_v_arg;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("compile_simple (wrapper)", 0);
   assert(__pyx_arg_arg); {
     __pyx_v_arg = __Pyx_PyObject_AsWritableString(__pyx_arg_arg); if (unlikely((!__pyx_v_arg) && PyErr_Occurred())) __PYX_ERR(0, 648, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
@@ -12241,14 +12496,17 @@
 static PyObject *__pyx_pf_7pystemd_7dbuslib_14compile_simple_process_simple(PyObject *__pyx_self, PyObject *__pyx_v_v) {
   struct __pyx_obj_7pystemd_7dbuslib___pyx_scope_struct_2_compile_simple *__pyx_cur_scope;
   struct __pyx_obj_7pystemd_7dbuslib___pyx_scope_struct_2_compile_simple *__pyx_outer_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("process_simple", 0);
   __pyx_outer_scope = (struct __pyx_obj_7pystemd_7dbuslib___pyx_scope_struct_2_compile_simple *) __Pyx_CyFunction_GetClosure(__pyx_self);
   __pyx_cur_scope = __pyx_outer_scope;
 
   /* "pystemd/dbuslib.pyx":653
  * 
  *   def process_simple(v):
@@ -12308,14 +12566,17 @@
   struct __pyx_obj_7pystemd_7dbuslib___pyx_scope_struct_2_compile_simple *__pyx_cur_scope;
   char *__pyx_v_off;
   PyObject *__pyx_v_process_simple = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("compile_simple", 0);
   __pyx_cur_scope = (struct __pyx_obj_7pystemd_7dbuslib___pyx_scope_struct_2_compile_simple *)__pyx_tp_new_7pystemd_7dbuslib___pyx_scope_struct_2_compile_simple(__pyx_ptype_7pystemd_7dbuslib___pyx_scope_struct_2_compile_simple, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_7pystemd_7dbuslib___pyx_scope_struct_2_compile_simple *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 648, __pyx_L1_error)
   } else {
@@ -12343,15 +12604,15 @@
   /* "pystemd/dbuslib.pyx":652
  *   cdef char *off = &res
  * 
  *   def process_simple(v):             # <<<<<<<<<<<<<<
  *     return [(res, v)]
  * 
  */
-  __pyx_t_1 = __Pyx_CyFunction_NewEx(&__pyx_mdef_7pystemd_7dbuslib_14compile_simple_1process_simple, 0, __pyx_n_s_compile_simple_locals_process_si, ((PyObject*)__pyx_cur_scope), __pyx_n_s_pystemd_dbuslib, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 652, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_7pystemd_7dbuslib_14compile_simple_1process_simple, 0, __pyx_n_s_compile_simple_locals_process_si, ((PyObject*)__pyx_cur_scope), __pyx_n_s_pystemd_dbuslib, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 652, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_process_simple = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "pystemd/dbuslib.pyx":655
  *     return [(res, v)]
  * 
@@ -12405,14 +12666,17 @@
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7pystemd_7dbuslib_5compile_array(PyObject *__pyx_self, PyObject *__pyx_arg_args); /*proto*/
 static PyMethodDef __pyx_mdef_7pystemd_7dbuslib_5compile_array = {"compile_array", (PyCFunction)__pyx_pw_7pystemd_7dbuslib_5compile_array, METH_O, 0};
 static PyObject *__pyx_pw_7pystemd_7dbuslib_5compile_array(PyObject *__pyx_self, PyObject *__pyx_arg_args) {
   char *__pyx_v_args;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("compile_array (wrapper)", 0);
   assert(__pyx_arg_args); {
     __pyx_v_args = __Pyx_PyObject_AsWritableString(__pyx_arg_args); if (unlikely((!__pyx_v_args) && PyErr_Occurred())) __PYX_ERR(0, 657, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
@@ -12460,14 +12724,17 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t __pyx_t_4;
   PyObject *(*__pyx_t_5)(PyObject *);
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("process_array", 0);
   __pyx_outer_scope = (struct __pyx_obj_7pystemd_7dbuslib___pyx_scope_struct_3_compile_array *) __Pyx_CyFunction_GetClosure(__pyx_self);
   __pyx_cur_scope = __pyx_outer_scope;
 
   /* "pystemd/dbuslib.pyx":663
  * 
  *   def process_array(v):
@@ -12642,14 +12909,17 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *(*__pyx_t_5)(PyObject *);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("compile_array", 0);
   __pyx_cur_scope = (struct __pyx_obj_7pystemd_7dbuslib___pyx_scope_struct_3_compile_array *)__pyx_tp_new_7pystemd_7dbuslib___pyx_scope_struct_3_compile_array(__pyx_ptype_7pystemd_7dbuslib___pyx_scope_struct_3_compile_array, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_7pystemd_7dbuslib___pyx_scope_struct_3_compile_array *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 657, __pyx_L1_error)
   } else {
@@ -12758,15 +13028,15 @@
   /* "pystemd/dbuslib.pyx":662
  *   off, pr = COMPILE_METHODS.get(array_type, compile_simple)(args[1:])
  * 
  *   def process_array(v):             # <<<<<<<<<<<<<<
  *     cdef list ret = [(dbusc.SD_BUS_TYPE_ARRAY, off[1:])]
  *     for i in v:
  */
-  __pyx_t_1 = __Pyx_CyFunction_NewEx(&__pyx_mdef_7pystemd_7dbuslib_13compile_array_1process_array, 0, __pyx_n_s_compile_array_locals_process_arr, ((PyObject*)__pyx_cur_scope), __pyx_n_s_pystemd_dbuslib, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 662, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_7pystemd_7dbuslib_13compile_array_1process_array, 0, __pyx_n_s_compile_array_locals_process_arr, ((PyObject*)__pyx_cur_scope), __pyx_n_s_pystemd_dbuslib, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 662, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_process_array = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "pystemd/dbuslib.pyx":669
  *     return ret
  * 
@@ -12837,14 +13107,17 @@
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7pystemd_7dbuslib_7compile_struct(PyObject *__pyx_self, PyObject *__pyx_arg_args); /*proto*/
 static PyMethodDef __pyx_mdef_7pystemd_7dbuslib_7compile_struct = {"compile_struct", (PyCFunction)__pyx_pw_7pystemd_7dbuslib_7compile_struct, METH_O, 0};
 static PyObject *__pyx_pw_7pystemd_7dbuslib_7compile_struct(PyObject *__pyx_self, PyObject *__pyx_arg_args) {
   char *__pyx_v_args;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("compile_struct (wrapper)", 0);
   assert(__pyx_arg_args); {
     __pyx_v_args = __Pyx_PyObject_AsWritableString(__pyx_arg_args); if (unlikely((!__pyx_v_args) && PyErr_Occurred())) __PYX_ERR(0, 672, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
@@ -12887,14 +13160,17 @@
   struct __pyx_obj_7pystemd_7dbuslib___pyx_scope_struct_4_compile_struct *__pyx_outer_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("process_struct", 0);
   __pyx_outer_scope = (struct __pyx_obj_7pystemd_7dbuslib___pyx_scope_struct_4_compile_struct *) __Pyx_CyFunction_GetClosure(__pyx_self);
   __pyx_cur_scope = __pyx_outer_scope;
 
   /* "pystemd/dbuslib.pyx":683
  * 
  *   def process_struct(v):
@@ -13020,14 +13296,17 @@
   int __pyx_v_closing;
   PyObject *__pyx_v_process_struct = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   char *__pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("compile_struct", 0);
   __pyx_cur_scope = (struct __pyx_obj_7pystemd_7dbuslib___pyx_scope_struct_4_compile_struct *)__pyx_tp_new_7pystemd_7dbuslib___pyx_scope_struct_4_compile_struct(__pyx_ptype_7pystemd_7dbuslib___pyx_scope_struct_4_compile_struct, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_7pystemd_7dbuslib___pyx_scope_struct_4_compile_struct *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 672, __pyx_L1_error)
   } else {
@@ -13073,15 +13352,15 @@
   /* "pystemd/dbuslib.pyx":682
  *   cs = compile_args(struc_extend)
  * 
  *   def process_struct(v):             # <<<<<<<<<<<<<<
  *     return (
  *       [(dbusc.SD_BUS_TYPE_STRUCT, struc_extend)] +
  */
-  __pyx_t_1 = __Pyx_CyFunction_NewEx(&__pyx_mdef_7pystemd_7dbuslib_14compile_struct_1process_struct, 0, __pyx_n_s_compile_struct_locals_process_st, ((PyObject*)__pyx_cur_scope), __pyx_n_s_pystemd_dbuslib, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 682, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_7pystemd_7dbuslib_14compile_struct_1process_struct, 0, __pyx_n_s_compile_struct_locals_process_st, ((PyObject*)__pyx_cur_scope), __pyx_n_s_pystemd_dbuslib, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 682, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_process_struct = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "pystemd/dbuslib.pyx":688
  *       [(-1, None)]
  *     )
@@ -13152,14 +13431,17 @@
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *(*__pyx_t_7)(PyObject *);
   int __pyx_t_8;
   Py_ssize_t __pyx_t_9;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("compile_args", 0);
 
   /* "pystemd/dbuslib.pyx":699
  * cpdef list compile_args(char *args):
  *   cdef:
  *     int i = 0             # <<<<<<<<<<<<<<
  *     int size_of_args = len(args)
@@ -13354,14 +13636,17 @@
   return __pyx_r;
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7pystemd_7dbuslib_9compile_args(PyObject *__pyx_self, PyObject *__pyx_arg_args); /*proto*/
 static PyObject *__pyx_pw_7pystemd_7dbuslib_9compile_args(PyObject *__pyx_self, PyObject *__pyx_arg_args) {
   char *__pyx_v_args;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("compile_args (wrapper)", 0);
   assert(__pyx_arg_args); {
     __pyx_v_args = __Pyx_PyObject_AsWritableString(__pyx_arg_args); if (unlikely((!__pyx_v_args) && PyErr_Occurred())) __PYX_ERR(0, 697, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
@@ -13377,14 +13662,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_8compile_args(CYTHON_UNUSED PyObject *__pyx_self, char *__pyx_v_args) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("compile_args", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_f_7pystemd_7dbuslib_compile_args(__pyx_v_args, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 697, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -13420,14 +13708,17 @@
   Py_ssize_t __pyx_t_3;
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *(*__pyx_t_8)(PyObject *);
   int __pyx_t_9;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("apply_args", 0);
 
   /* "pystemd/dbuslib.pyx":714
  * 
  * cpdef list apply_args(list args, list values):
  *   cdef list ret = []             # <<<<<<<<<<<<<<
  *   for cfunc, value in zip(args, values):
@@ -13622,14 +13913,17 @@
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7pystemd_7dbuslib_11apply_args(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_7pystemd_7dbuslib_11apply_args(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_args = 0;
   PyObject *__pyx_v_values = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("apply_args (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_args,&__pyx_n_s_values,0};
     PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
@@ -13688,14 +13982,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_10apply_args(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_args, PyObject *__pyx_v_values) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("apply_args", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_f_7pystemd_7dbuslib_apply_args(__pyx_v_args, __pyx_v_values, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 713, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -13732,14 +14029,17 @@
   Py_ssize_t __pyx_t_3;
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *(*__pyx_t_8)(PyObject *);
   int __pyx_t_9;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("apply_signature", 0);
 
   /* "pystemd/dbuslib.pyx":720
  * 
  * cpdef list apply_signature(char *signature, list values):
  *   cdef list args = compile_args(signature)             # <<<<<<<<<<<<<<
  *   cdef list ret = []
@@ -13947,14 +14247,17 @@
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7pystemd_7dbuslib_13apply_signature(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_7pystemd_7dbuslib_13apply_signature(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   char *__pyx_v_signature;
   PyObject *__pyx_v_values = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("apply_signature (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_signature,&__pyx_n_s_values,0};
     PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
@@ -14012,14 +14315,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_12apply_signature(CYTHON_UNUSED PyObject *__pyx_self, char *__pyx_v_signature, PyObject *__pyx_v_values) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("apply_signature", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_f_7pystemd_7dbuslib_apply_signature(__pyx_v_signature, __pyx_v_values, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 719, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -14057,14 +14363,17 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("path_encode", 0);
 
   /* "pystemd/dbuslib.pyx":743
  *     int r
  * 
  *   try:             # <<<<<<<<<<<<<<
  *     r = dbusc.sd_bus_path_encode(prefix, external_id, &ret_path)
@@ -14198,14 +14507,17 @@
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7pystemd_7dbuslib_15path_encode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_7pystemd_7dbuslib_14path_encode[] = "Python wrapper for sd_bus_path_encode, it produce a encoded version of a\n  systemd path:\n\n  example:\n\n  In [1]: path_encode(b'/org/freedesktop/systemd1/unit', b'postfix.service')\n  Out[1]: b'/org/freedesktop/systemd1/unit/postfix_2eservice'\n\n  cdocs: https://www.freedesktop.org/software/systemd/man/sd_bus_path_encode.html\n  ";
 static PyObject *__pyx_pw_7pystemd_7dbuslib_15path_encode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   char *__pyx_v_prefix;
   char *__pyx_v_external_id;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("path_encode (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_prefix,&__pyx_n_s_external_id,0};
     PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
@@ -14258,14 +14570,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_14path_encode(CYTHON_UNUSED PyObject *__pyx_self, char *__pyx_v_prefix, char *__pyx_v_external_id) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("path_encode", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_f_7pystemd_7dbuslib_path_encode(__pyx_v_prefix, __pyx_v_external_id, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 727, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -14303,14 +14618,17 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("path_decode", 0);
 
   /* "pystemd/dbuslib.pyx":772
  *     int r
  * 
  *   try:             # <<<<<<<<<<<<<<
  *     r = dbusc.sd_bus_path_decode(path, prefix, &answer)
@@ -14444,14 +14762,17 @@
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7pystemd_7dbuslib_17path_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_7pystemd_7dbuslib_16path_decode[] = "Python wrapper for sd_bus_path_decode, it produce a decoded version of a\n  systemd path:\n\n  example:\n\n  In [1]: path_decode(\n  ...    b'/org/freedesktop/systemd1/unit/postfix_2eservice',\n  ...    b'/org/freedesktop/systemd1/unit')\n  Out[1]: b'postfix.service'\n\n  cdocs: https://www.freedesktop.org/software/systemd/man/sd_bus_path_encode.html\n  ";
 static PyObject *__pyx_pw_7pystemd_7dbuslib_17path_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   char *__pyx_v_path;
   char *__pyx_v_prefix;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("path_decode (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_path,&__pyx_n_s_prefix,0};
     PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
@@ -14504,14 +14825,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pystemd_7dbuslib_16path_decode(CYTHON_UNUSED PyObject *__pyx_self, char *__pyx_v_path, char *__pyx_v_prefix) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("path_decode", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_f_7pystemd_7dbuslib_path_decode(__pyx_v_path, __pyx_v_prefix, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 754, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -14540,14 +14864,17 @@
   PyObject *__pyx_v_mycallback = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("match_signal_callback_handler", 0);
 
   /* "pystemd/dbuslib.pyx":789
  * ) except -1:
  *   cdef:
  *     DbusMessage msg = DbusMessage()             # <<<<<<<<<<<<<<
  *     object mycallback = <object> userdata
@@ -14653,14 +14980,17 @@
 static char *__pyx_f_7pystemd_7dbuslib__b2c(PyObject *__pyx_v_py_value) {
   char *__pyx_v_output;
   char *__pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   char *__pyx_t_3;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_b2c", 0);
 
   /* "pystemd/dbuslib.pyx":805
  * cdef char* _b2c(bytes py_value):
  *   "Interface to convert byte (as return by x2char_star) to char* respecting Null"
  *   cdef char * output = NULL             # <<<<<<<<<<<<<<
  * 
@@ -14751,17 +15081,17 @@
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
-    ++Py_REFCNT(o);
+    __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
     __pyx_pw_7pystemd_7dbuslib_11DbusMessage_1__dealloc__(o);
-    --Py_REFCNT(o);
+    __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
     PyErr_Restore(etype, eval, etb);
   }
   Py_CLEAR(p->body);
   Py_CLEAR(p->headers);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
@@ -16381,14 +16711,17 @@
   /*--- Function export code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_vtabptr_7pystemd_7dbuslib_DbusMessage = &__pyx_vtable_7pystemd_7dbuslib_DbusMessage;
   __pyx_vtable_7pystemd_7dbuslib_DbusMessage.ref = (sd_bus_message **(*)(struct __pyx_obj_7pystemd_7dbuslib_DbusMessage *))__pyx_f_7pystemd_7dbuslib_11DbusMessage_ref;
   __pyx_vtable_7pystemd_7dbuslib_DbusMessage.msg = (sd_bus_message *(*)(struct __pyx_obj_7pystemd_7dbuslib_DbusMessage *))__pyx_f_7pystemd_7dbuslib_11DbusMessage_msg;
   __pyx_vtable_7pystemd_7dbuslib_DbusMessage.set_bus_message = (PyObject *(*)(struct __pyx_obj_7pystemd_7dbuslib_DbusMessage *, sd_bus_message *))__pyx_f_7pystemd_7dbuslib_11DbusMessage_set_bus_message;
   __pyx_vtable_7pystemd_7dbuslib_DbusMessage.process_reply = (PyObject *(*)(struct __pyx_obj_7pystemd_7dbuslib_DbusMessage *, bool, int __pyx_skip_dispatch))__pyx_f_7pystemd_7dbuslib_11DbusMessage_process_reply;
@@ -16544,25 +16877,27 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
-#if PY_MAJOR_VERSION < 3
-#ifdef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC void
-#else
+#ifndef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
+#elif PY_MAJOR_VERSION < 3
+#ifdef __cplusplus
+#define __Pyx_PyMODINIT_FUNC extern "C" void
+#else
+#define __Pyx_PyMODINIT_FUNC void
 #endif
 #else
-#ifdef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC PyObject *
+#ifdef __cplusplus
+#define __Pyx_PyMODINIT_FUNC extern "C" PyObject *
 #else
-#define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
+#define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
 __Pyx_PyMODINIT_FUNC initdbuslib(void) CYTHON_SMALL_CODE; /*proto*/
 __Pyx_PyMODINIT_FUNC initdbuslib(void)
@@ -16640,14 +16975,17 @@
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module 'dbuslib' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
@@ -16728,22 +17066,22 @@
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "pystemd.dbuslib")) {
       if (unlikely(PyDict_SetItemString(modules, "pystemd.dbuslib", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
-  if (__Pyx_InitCachedBuiltins() < 0) goto __pyx_L1_error;
+  if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
-  if (__Pyx_InitCachedConstants() < 0) goto __pyx_L1_error;
+  if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
-  if (unlikely(__Pyx_modinit_type_init_code() != 0)) goto __pyx_L1_error;
+  if (unlikely(__Pyx_modinit_type_init_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
@@ -16902,53 +17240,53 @@
   /* "pystemd/dbuslib.pyx":39
  * 
  * class VariableReturn(object):
  *   def __init__(self, parent=None, v_type=None):             # <<<<<<<<<<<<<<
  *     self.data = []
  *     self.parent = parent
  */
-  __pyx_t_3 = __Pyx_CyFunction_NewEx(&__pyx_mdef_7pystemd_7dbuslib_14VariableReturn_1__init__, 0, __pyx_n_s_VariableReturn___init, NULL, __pyx_n_s_pystemd_dbuslib, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7pystemd_7dbuslib_14VariableReturn_1__init__, 0, __pyx_n_s_VariableReturn___init, NULL, __pyx_n_s_pystemd_dbuslib, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__25);
   if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_init, __pyx_t_3) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pystemd/dbuslib.pyx":44
  *     self.v_type = v_type
  * 
  *   def create_child(self, v_type=None):             # <<<<<<<<<<<<<<
  *     self.data.append(
  *       VariableReturn(
  */
-  __pyx_t_3 = __Pyx_CyFunction_NewEx(&__pyx_mdef_7pystemd_7dbuslib_14VariableReturn_3create_child, 0, __pyx_n_s_VariableReturn_create_child, NULL, __pyx_n_s_pystemd_dbuslib, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7pystemd_7dbuslib_14VariableReturn_3create_child, 0, __pyx_n_s_VariableReturn_create_child, NULL, __pyx_n_s_pystemd_dbuslib, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__28);
   if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_create_child, __pyx_t_3) < 0) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pystemd/dbuslib.pyx":52
  *     return self.data[-1]
  * 
  *   def append(self, dt):             # <<<<<<<<<<<<<<
  *     self.data.append(dt)
  * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_NewEx(&__pyx_mdef_7pystemd_7dbuslib_14VariableReturn_5append, 0, __pyx_n_s_VariableReturn_append, NULL, __pyx_n_s_pystemd_dbuslib, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7pystemd_7dbuslib_14VariableReturn_5append, 0, __pyx_n_s_VariableReturn_append, NULL, __pyx_n_s_pystemd_dbuslib, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_append, __pyx_t_3) < 0) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pystemd/dbuslib.pyx":55
  *     self.data.append(dt)
  * 
  *   def dump(self):             # <<<<<<<<<<<<<<
  *     o = [
  *       e.dump() if isinstance(e, VariableReturn) else e
  */
-  __pyx_t_3 = __Pyx_CyFunction_NewEx(&__pyx_mdef_7pystemd_7dbuslib_14VariableReturn_7dump, 0, __pyx_n_s_VariableReturn_dump, NULL, __pyx_n_s_pystemd_dbuslib, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7pystemd_7dbuslib_14VariableReturn_7dump, 0, __pyx_n_s_VariableReturn_dump, NULL, __pyx_n_s_pystemd_dbuslib, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_dump, __pyx_t_3) < 0) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pystemd/dbuslib.pyx":38
  * )
  * 
@@ -17151,15 +17489,15 @@
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
             continue;
         }
         name = first_kw_arg;
         #if PY_MAJOR_VERSION < 3
-        if (likely(PyString_CheckExact(key)) || likely(PyString_Check(key))) {
+        if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
                     break;
                 }
                 name++;
@@ -17178,15 +17516,15 @@
             }
         } else
         #endif
         if (likely(PyUnicode_Check(key))) {
             while (*name) {
                 int cmp = (**name == key) ? 0 :
                 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                    (PyUnicode_GET_SIZE(**name) != PyUnicode_GET_SIZE(key)) ? 1 :
+                    (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
                     PyUnicode_Compare(**name, key);
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
                     break;
                 }
@@ -17194,15 +17532,15 @@
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
                 while (argname != first_kw_arg) {
                     int cmp = (**argname == key) ? 0 :
                     #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                        (PyUnicode_GET_SIZE(**argname) != PyUnicode_GET_SIZE(key)) ? 1 :
+                        (__Pyx_PyUnicode_GET_LENGTH(**argname) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                     #endif
                         PyUnicode_Compare(**argname, key);
                     if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                     if (cmp == 0) goto arg_passed_twice;
                     argname++;
                 }
             }
@@ -18971,15 +19309,15 @@
     return cached_type;
 bad:
     Py_XDECREF(cached_type);
     cached_type = NULL;
     goto done;
 }
 
-/* CythonFunction */
+/* CythonFunctionShared */
 #include <structmember.h>
 static PyObject *
 __Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, CYTHON_UNUSED void *closure)
 {
     if (unlikely(op->func_doc == NULL)) {
         if (op->func.m_ml->ml_doc) {
 #if PY_MAJOR_VERSION >= 3
@@ -19278,18 +19616,17 @@
     {0, 0, 0, 0}
 };
 #if PY_VERSION_HEX < 0x030500A0
 #define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func_weakreflist)
 #else
 #define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func.m_weakreflist)
 #endif
-static PyObject *__Pyx_CyFunction_New(PyTypeObject *type, PyMethodDef *ml, int flags, PyObject* qualname,
-                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
-    __pyx_CyFunctionObject *op = PyObject_GC_New(__pyx_CyFunctionObject, type);
-    if (op == NULL)
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject *op, PyMethodDef *ml, int flags, PyObject* qualname,
+                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    if (unlikely(op == NULL))
         return NULL;
     op->flags = flags;
     __Pyx_CyFunction_weakreflist(op) = NULL;
     op->func.m_ml = ml;
     op->func.m_self = (PyObject *) op;
     Py_XINCREF(closure);
     op->func_closure = closure;
@@ -19302,20 +19639,20 @@
     op->func_doc = NULL;
     op->func_classobj = NULL;
     op->func_globals = globals;
     Py_INCREF(op->func_globals);
     Py_XINCREF(code);
     op->func_code = code;
     op->defaults_pyobjects = 0;
+    op->defaults_size = 0;
     op->defaults = NULL;
     op->defaults_tuple = NULL;
     op->defaults_kwdict = NULL;
     op->defaults_getter = NULL;
     op->func_annotations = NULL;
-    PyObject_GC_Track(op);
     return (PyObject *) op;
 }
 static int
 __Pyx_CyFunction_clear(__pyx_CyFunctionObject *m)
 {
     Py_CLEAR(m->func_closure);
     Py_CLEAR(m->func.m_module);
@@ -19370,26 +19707,28 @@
         for (i = 0; i < m->defaults_pyobjects; i++)
             Py_VISIT(pydefaults[i]);
     }
     return 0;
 }
 static PyObject *__Pyx_CyFunction_descr_get(PyObject *func, PyObject *obj, PyObject *type)
 {
+#if PY_MAJOR_VERSION < 3
     __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
     if (m->flags & __Pyx_CYFUNCTION_STATICMETHOD) {
         Py_INCREF(func);
         return func;
     }
     if (m->flags & __Pyx_CYFUNCTION_CLASSMETHOD) {
         if (type == NULL)
             type = (PyObject *)(Py_TYPE(obj));
         return __Pyx_PyMethod_New(func, type, (PyObject *)(Py_TYPE(type)));
     }
     if (obj == Py_None)
         obj = NULL;
+#endif
     return __Pyx_PyMethod_New(func, obj, type);
 }
 static PyObject*
 __Pyx_CyFunction_repr(__pyx_CyFunctionObject *op)
 {
 #if PY_MAJOR_VERSION >= 3
     return PyUnicode_FromFormat("<cyfunction %U at %p>",
@@ -19555,14 +19894,15 @@
 static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *func, size_t size, int pyobjects) {
     __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
     m->defaults = PyObject_Malloc(size);
     if (unlikely(!m->defaults))
         return PyErr_NoMemory();
     memset(m->defaults, 0, size);
     m->defaults_pyobjects = pyobjects;
+    m->defaults_size = size;
     return m->defaults;
 }
 static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *func, PyObject *tuple) {
     __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
     m->defaults_tuple = tuple;
     Py_INCREF(tuple);
 }
@@ -19573,14 +19913,27 @@
 }
 static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
     __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
     m->func_annotations = dict;
     Py_INCREF(dict);
 }
 
+/* CythonFunction */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
+                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyObject *op = __Pyx_CyFunction_Init(
+        PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
+        ml, flags, qualname, closure, module, globals, code
+    );
+    if (likely(op)) {
+        PyObject_GC_Track(op);
+    }
+    return op;
+}
+
 /* SliceObject */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetSlice(PyObject* obj,
         Py_ssize_t cstart, Py_ssize_t cstop,
         PyObject** _py_start, PyObject** _py_stop, PyObject** _py_slice,
         int has_cstart, int has_cstop, CYTHON_UNUSED int wraparound) {
 #if CYTHON_USE_TYPE_SLOTS
     PyMappingMethods* mp;
@@ -19941,14 +20294,36 @@
     Py_DECREF(ob);
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
 }
 
+/* PyObjectGetAttrStrNoError */
+static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
+        __Pyx_PyErr_Clear();
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
+    PyObject *result;
+#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
+        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
+    }
+#endif
+    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
+    if (unlikely(!result)) {
+        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
+    }
+    return result;
+}
+
 /* SetupReduce */
 static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
   int ret;
   PyObject *name_attr;
   name_attr = __Pyx_PyObject_GetAttrStr(meth, __pyx_n_s_name_2);
   if (likely(name_attr)) {
       ret = PyObject_RichCompareBool(name_attr, name, Py_EQ);
@@ -19968,51 +20343,59 @@
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto GOOD;
+    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto GOOD;
+    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
 #endif
 #if CYTHON_USE_PYTYPE_LOOKUP
-    object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto BAD;
+    object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
-    object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto BAD;
+    object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
-    reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto BAD;
+    reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
 #if CYTHON_USE_PYTYPE_LOOKUP
-        object_reduce = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto BAD;
+        object_reduce = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto __PYX_BAD;
 #else
-        object_reduce = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto BAD;
+        object_reduce = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto __PYX_BAD;
 #endif
-        reduce = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce); if (unlikely(!reduce)) goto BAD;
+        reduce = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce); if (unlikely(!reduce)) goto __PYX_BAD;
         if (reduce == object_reduce || __Pyx_setup_reduce_is_named(reduce, __pyx_n_s_reduce_cython)) {
-            reduce_cython = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_cython); if (unlikely(!reduce_cython)) goto BAD;
-            ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce, reduce_cython); if (unlikely(ret < 0)) goto BAD;
-            ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce_cython); if (unlikely(ret < 0)) goto BAD;
+            reduce_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_reduce_cython);
+            if (likely(reduce_cython)) {
+                ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce, reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
+                ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
+            } else if (reduce == object_reduce || PyErr_Occurred()) {
+                goto __PYX_BAD;
+            }
             setstate = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_setstate);
             if (!setstate) PyErr_Clear();
             if (!setstate || __Pyx_setup_reduce_is_named(setstate, __pyx_n_s_setstate_cython)) {
-                setstate_cython = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_setstate_cython); if (unlikely(!setstate_cython)) goto BAD;
-                ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate, setstate_cython); if (unlikely(ret < 0)) goto BAD;
-                ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate_cython); if (unlikely(ret < 0)) goto BAD;
+                setstate_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_setstate_cython);
+                if (likely(setstate_cython)) {
+                    ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate, setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
+                    ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
+                } else if (!setstate || PyErr_Occurred()) {
+                    goto __PYX_BAD;
+                }
             }
             PyType_Modified((PyTypeObject*)type_obj);
         }
     }
-    goto GOOD;
-BAD:
+    goto __PYX_GOOD;
+__PYX_BAD:
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
-GOOD:
+__PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
@@ -20047,15 +20430,15 @@
         goto bad;
     empty_dict = PyDict_New();
     if (!empty_dict)
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
-            if (strchr(__Pyx_MODULE_NAME, '.')) {
+            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
                 module = PyImport_ImportModuleLevelObject(
                     name, global_dict, empty_dict, list, 1);
                 if (!module) {
                     if (!PyErr_ExceptionMatches(PyExc_ImportError))
                         goto bad;
                     PyErr_Clear();
                 }
@@ -20204,15 +20587,15 @@
     }
     Py_XDECREF(owned_metaclass);
     return result;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -20308,15 +20691,15 @@
         entries[pos].code_object = code_object;
         Py_DECREF(tmp);
         return;
     }
     if (__pyx_code_cache.count == __pyx_code_cache.max_count) {
         int new_max = __pyx_code_cache.max_count + 64;
         entries = (__Pyx_CodeObjectCacheEntry*)PyMem_Realloc(
-            __pyx_code_cache.entries, (size_t)new_max*sizeof(__Pyx_CodeObjectCacheEntry));
+            __pyx_code_cache.entries, ((size_t)new_max) * sizeof(__Pyx_CodeObjectCacheEntry));
         if (unlikely(!entries)) {
             return;
         }
         __pyx_code_cache.entries = entries;
         __pyx_code_cache.max_count = new_max;
     }
     for (i=__pyx_code_cache.count; i>pos; i--) {
```

### Comparing `pystemd-0.7.0/pystemd/dbuslib.pyx` & `pystemd-0.8.0/pystemd/dbuslib.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
           arg_type_c,
           <int>arg_value)
       elif arg_type in CONTAINER_TYPES: # open container
         r = dbusc.sd_bus_message_open_container(
           msg_call,
           arg_type,
           <char*>arg_value)
-      elif arg_type == -1: # close container
+      elif arg_type_i == -1: # close container
         r = dbusc.sd_bus_message_close_container(msg_call)
       else:
         raise DBusError(
           -42, None, "Unknown arg type %s for %s" % (arg_type, arg_value))
 
     def call_method(
             self,
```

### Comparing `pystemd-0.7.0/pystemd/journal.c` & `pystemd-0.8.0/pystemd/journal.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.14 */
+/* Generated by Cython 0.29.21 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "libraries": [
             "systemd"
@@ -19,16 +19,16 @@
 #define PY_SSIZE_T_CLEAN
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_14"
-#define CYTHON_HEX_VERSION 0x001D0EF0
+#define CYTHON_ABI "0_29_21"
+#define CYTHON_HEX_VERSION 0x001D15F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -447,15 +447,19 @@
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
+  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #else
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+  #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
@@ -496,26 +500,35 @@
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBaseString_Type            PyUnicode_Type
   #define PyStringObject               PyUnicodeObject
   #define PyString_Type                PyUnicode_Type
   #define PyString_Check               PyUnicode_Check
   #define PyString_CheckExact          PyUnicode_CheckExact
+#ifndef PyObject_Unicode
   #define PyObject_Unicode             PyObject_Str
 #endif
+#endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
 #ifndef PySet_CheckExact
   #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
 #endif
+#if PY_VERSION_HEX >= 0x030900A4
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
+#else
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
+#endif
 #if CYTHON_ASSUME_SAFE_MACROS
   #define __Pyx_PySequence_SIZE(seq)  Py_SIZE(seq)
 #else
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
@@ -547,15 +560,15 @@
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
   #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
   #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? PyMethod_New(func, self) : (Py_INCREF(func), func))
+  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
@@ -588,19 +601,18 @@
 #endif
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
-
+#define __PYX_MARK_ERR_POS(f_index, lineno) \
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
-{ \
-  __pyx_filename = __pyx_f[f_index]; __pyx_lineno = lineno; __pyx_clineno = __LINE__; goto Ln_error; \
-}
+    { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifndef __PYX_EXTERN_C
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
@@ -933,15 +945,15 @@
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len)) {
         Py_INCREF(x);
         PyList_SET_ITEM(list, len, x);
-        Py_SIZE(list) = len+1;
+        __Pyx_SET_SIZE(list, len + 1);
         return 0;
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
 #endif
@@ -1416,14 +1428,17 @@
   int __pyx_t_8;
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   char *__pyx_t_13;
   size_t __pyx_t_14;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("sendv", 0);
 
   /* "pystemd/journal.pyx":45
  *     x2char_star(i)
  *     for i in args
  *   ] + [             # <<<<<<<<<<<<<<
  *     b"=".join([x2char_star(key), x2char_star(val, convert_all=True)])
@@ -1789,14 +1804,17 @@
 static PyObject *__pyx_pw_7pystemd_7journal_3log(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_7pystemd_7journal_2log[] = "\n  Send a `message` to the journal with the `priority` specified\n  examples:\n\n  ```python\nimport logging\nimport pystemd.journal\n\npystemd.journal.log(\n  logging.INFO,\n  \"everything is awesome\",\n  SYSLOG_IDENTIFIER=\"tegan\"\n)\n  ```\n  ";
 static PyMethodDef __pyx_mdef_7pystemd_7journal_3log = {"log", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pystemd_7journal_3log, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pystemd_7journal_2log};
 static PyObject *__pyx_pw_7pystemd_7journal_3log(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   int __pyx_v_priority;
   PyObject *__pyx_v_message = 0;
   PyObject *__pyx_v_kwargs = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("log (wrapper)", 0);
   __pyx_v_kwargs = PyDict_New(); if (unlikely(!__pyx_v_kwargs)) return NULL;
   __Pyx_GOTREF(__pyx_v_kwargs);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_priority,&__pyx_n_s_message,0};
@@ -1863,14 +1881,17 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("log", 0);
 
   /* "pystemd/journal.pyx":81
  *   """
  * 
  *   stack = inspect.stack()[0]             # <<<<<<<<<<<<<<
  * 
@@ -2287,25 +2308,27 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
-#if PY_MAJOR_VERSION < 3
-#ifdef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC void
-#else
+#ifndef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
+#elif PY_MAJOR_VERSION < 3
+#ifdef __cplusplus
+#define __Pyx_PyMODINIT_FUNC extern "C" void
+#else
+#define __Pyx_PyMODINIT_FUNC void
 #endif
 #else
-#ifdef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC PyObject *
+#ifdef __cplusplus
+#define __Pyx_PyMODINIT_FUNC extern "C" PyObject *
 #else
-#define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
+#define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
 __Pyx_PyMODINIT_FUNC initjournal(void) CYTHON_SMALL_CODE; /*proto*/
 __Pyx_PyMODINIT_FUNC initjournal(void)
@@ -2380,14 +2403,17 @@
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec_journal(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module 'journal' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
@@ -2468,17 +2494,17 @@
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "pystemd.journal")) {
       if (unlikely(PyDict_SetItemString(modules, "pystemd.journal", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
-  if (__Pyx_InitCachedBuiltins() < 0) goto __pyx_L1_error;
+  if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
-  if (__Pyx_InitCachedConstants() < 0) goto __pyx_L1_error;
+  if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
   (void)__Pyx_modinit_type_init_code();
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
@@ -3542,15 +3568,15 @@
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
             continue;
         }
         name = first_kw_arg;
         #if PY_MAJOR_VERSION < 3
-        if (likely(PyString_CheckExact(key)) || likely(PyString_Check(key))) {
+        if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
                     break;
                 }
                 name++;
@@ -3569,15 +3595,15 @@
             }
         } else
         #endif
         if (likely(PyUnicode_Check(key))) {
             while (*name) {
                 int cmp = (**name == key) ? 0 :
                 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                    (PyUnicode_GET_SIZE(**name) != PyUnicode_GET_SIZE(key)) ? 1 :
+                    (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
                     PyUnicode_Compare(**name, key);
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
                     break;
                 }
@@ -3585,15 +3611,15 @@
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
                 while (argname != first_kw_arg) {
                     int cmp = (**argname == key) ? 0 :
                     #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                        (PyUnicode_GET_SIZE(**argname) != PyUnicode_GET_SIZE(key)) ? 1 :
+                        (__Pyx_PyUnicode_GET_LENGTH(**argname) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                     #endif
                         PyUnicode_Compare(**argname, key);
                     if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                     if (cmp == 0) goto arg_passed_twice;
                     argname++;
                 }
             }
@@ -3781,15 +3807,15 @@
         goto bad;
     empty_dict = PyDict_New();
     if (!empty_dict)
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
-            if (strchr(__Pyx_MODULE_NAME, '.')) {
+            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
                 module = PyImport_ImportModuleLevelObject(
                     name, global_dict, empty_dict, list, 1);
                 if (!module) {
                     if (!PyErr_ExceptionMatches(PyExc_ImportError))
                         goto bad;
                     PyErr_Clear();
                 }
@@ -3921,15 +3947,15 @@
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
 }
 #endif
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -4025,15 +4051,15 @@
         entries[pos].code_object = code_object;
         Py_DECREF(tmp);
         return;
     }
     if (__pyx_code_cache.count == __pyx_code_cache.max_count) {
         int new_max = __pyx_code_cache.max_count + 64;
         entries = (__Pyx_CodeObjectCacheEntry*)PyMem_Realloc(
-            __pyx_code_cache.entries, (size_t)new_max*sizeof(__Pyx_CodeObjectCacheEntry));
+            __pyx_code_cache.entries, ((size_t)new_max) * sizeof(__Pyx_CodeObjectCacheEntry));
         if (unlikely(!entries)) {
             return;
         }
         __pyx_code_cache.entries = entries;
         __pyx_code_cache.max_count = new_max;
     }
     for (i=__pyx_code_cache.count; i>pos; i--) {
```

### Comparing `pystemd-0.7.0/pystemd/journal.pyx` & `pystemd-0.8.0/pystemd/journal.pyx`

 * *Files identical despite different names*

### Comparing `pystemd-0.7.0/pystemd/machine1/machine.py` & `pystemd-0.8.0/pystemd/machine1/machine.py`

 * *Files identical despite different names*

### Comparing `pystemd-0.7.0/pystemd/machine1/manager.py` & `pystemd-0.8.0/pystemd/machine1/manager.py`

 * *Files identical despite different names*

### Comparing `pystemd-0.7.0/pystemd/run.py` & `pystemd-0.8.0/pystemd/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,73 +78,71 @@
     pty=None,
     pty_master=None,
     pty_path=None,
     stdin=None,
     stdout=None,
     stderr=None,
     _wait_polling=None,
+    slice_=None,
 ):
     """
     pystemd.run imitates systemd-run, but with a pythonic feel to it.
 
     Options:
 
         cmd: Array with the command to execute (absolute path only)
         address: A custom dbus socket address
-        service_type: Set the unit type, eg: notify, onshot. If you dont give a
+        service_type: Set the unit type, e.g. notify, oneshot. If you dont give a
             value, the unit type will be whatever systemd thinks is the default.
-        name: Name of the unit, if not provided autogenerated.
+        name: Name of the unit. If not provided, it will be autogenerated.
         user: Username to execute the command, defaults to current user.
         user_mode: Equivalent to running `systemd-run --user`. Defaults to True
             if current user id not root (uid = 0).
         nice: Nice level to run the command.
-        runtime_max_sec: set seconds before sending a sigterm to the process, if
+        runtime_max_sec: Set seconds before sending a sigterm to the process, if
            the service does not die nicely, it will send a sigkill.
-        env: A dict with environmental variables.
+        env: A dict with environment variables.
         extra: If you know what you are doing, you can pass extra configuration
             settings to the start_transient_unit method.
         machine: Machine name to execute the command, by default we connect to
             the host's dbus.
-        wait: wait for command completition before returning control, defaults
+        wait: Wait for command completition before returning control, defaults
             to False.
         remain_after_exit: If True, the transient unit will remain after cmd
-            has finish, also if true, this methods will return
+            has finished, also if true, this methods will return
             pystemd.systemd1.Unit object. defaults to False and this method
             returns None and the unit will be gone as soon as is done.
         collect: Unload unit after it ran, even when failed.
         raise_on_fail: Will raise a PystemdRunError is cmd exit with non 0
             status code, it wont take affect unless you set wait=True,
             defaults to False.
         pty: Set this variable to True if you want a pty to be created. if you
             pass a `machine`, the pty will be created in the machine. Setting
             this value will ignore whatever you set in pty_master and pty_path.
-        pty_master: it has only meaning if you pass a pty_path also, this file
-            descriptor will be used to foward redirection to `stdin` and `stdout`
+        pty_master: It has only meaning if you pass a pty_path also, this file
+            descriptor will be used to forward redirection to `stdin` and `stdout`
             if no `stdin` or `stdout` is present, then this value does nothing.
         pty_path: Setting this value will pass this pty_path to the created
             process and will connect the process stdin, stdout and stderr to this
             pty. by itself it only ensure that your process has a real pty that
             can have ioctl operation over it. if you also pass a `pty_master`,
             `stdin` and `stdout` the pty forwars is handle for you.
-        stdin: Specify a file descriptor for stdin, by default this is `None`
-            and your unit will not have a stdin, you can specify it as
-            `sys.stdin.fileno()`, or as a regular numer, e.g. `0`. If you set
-            pty = True, or pass `pty_master` then this file descriptor will be
-            read and forward to the pty.
-        stdout: Specify a file descriptor for stdout, by default this is `None`
-            and your unit will not have a stdout, you can specify it as
-            `sys.stdout.fileno()`, or `open('/tmp/out', 'w').fileno()`, or a
-            regular number, e.g. `1`. If you set pty = True, or pass `pty_master`
-            then that pty will be read and forward to this file descriptor.
-        stderr: Specify a file descriptor for stderr, by default this is `None`
-            and your unit will not have a stderr, you can specify it as
-            `sys.stderr.fileno()`, or `open('/tmp/err', 'w').fileno()`, or a
-            regular number, e.g. `2`.
+        stdin: Specify a file descriptor for stdin. By default this is `None`
+            and your unit will not have a stdin. If you set pty = True, or set a
+            `pty_master` then that pty will be read and forwarded to this file
+            descriptor.
+        stdout: Specify a file descriptor for stdout. By default this is `None`
+            and your unit will not have a stdout. If you set pty = True, or set a
+            `pty_master` then that pty will be read and forwarded to this file
+            descriptor.
+        stderr: Specify a file descriptor for stderr. By default this is `None`
+            and your unit will not have a stderr.
+        slice_: the slice under you want to run the unit.
 
-    More info in:
+    More info and examples in:
     https://github.com/facebookincubator/pystemd/blob/master/_docs/pystemd.run.md
 
     """
 
     def bus_factory():
         if address:
             return DBusAddress(x2char_star(address))
@@ -171,14 +169,17 @@
                 with pystemd.machine1.Machine(machine) as m:
                     pty_master, pty_path = m.Machine.OpenPTY()
             else:
                 pty_master, pty_follower = ptylib.openpty()
                 pty_path = os.ttyname(pty_follower).encode()
                 ctexit.register(os.close, pty_master)
 
+        if slice_:
+            unit_properties[b"Slice"] = x2char_star(slice_)
+
         if pty_path:
             unit_properties.update(
                 {
                     b"StandardInput": b"tty",
                     b"StandardOutput": b"tty",
                     b"StandardError": b"tty",
                     b"TTYPath": pty_path,
```

### Comparing `pystemd-0.7.0/pystemd/systemd1/manager.py` & `pystemd-0.8.0/pystemd/systemd1/manager.py`

 * *Files identical despite different names*

### Comparing `pystemd-0.7.0/pystemd/systemd1/unit.py` & `pystemd-0.8.0/pystemd/systemd1/unit.py`

 * *Files identical despite different names*

### Comparing `pystemd-0.7.0/pystemd/systemd1/unit_signatures.py` & `pystemd-0.8.0/pystemd/systemd1/unit_signatures.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,19 @@
     b"StandardError": b"s",
     b"TTYPath": b"s",
     b"TTYReset": b"b",
     b"TTYVHangup": b"b",
     b"TTYVTDisallocate": b"b",
     b"IgnoreSIGPIPE": b"b",
     b"StandardInputFileDescriptor": b"h",
+    b"StandardOutputFile": b"s",
+    b"StandardOutputFileToAppend": b"s",
     b"StandardOutputFileDescriptor": b"h",
+    b"StandardErrorFile": b"s",
+    b"StandardErrorFileToAppend": b"s",
     b"StandardErrorFileDescriptor": b"h",
     b"StandardInputData": b"ay",
     b"Environment": b"as",
     b"PassEnvironment": b"as",
     b"UnsetEnvironment": b"as",
     b"EnvironmentFiles": b"a(sb)",
     # timer signatures
@@ -224,14 +228,15 @@
     b"CPUQuota": lambda _, value: (b"CPUQuotaPerSecUSec", b"t", int(value * 10 ** 6)),
     b"CPUQuotaPerSecUSec": b"t",
     b"IPAccounting": b"b",
     b"IPAddressAllow": b"a(iayu)",
     b"IPAddressDeny": b"a(iayu)",
     # Timer properties
     b"TimersMonotonic": b"a(st)",
+    b"TimersCalendar": b"a(ss)",
     b"WakeSystem": b"b",
     b"Persistent": b"b",
     # Socket Signatures
     b"BindIPv6Only": b"s",
     b"Backlog": b"u",
     b"TimeoutUSec": b"t",
     b"BindToDevice": b"s",
```

### Comparing `pystemd-0.7.0/pystemd/utils.py` & `pystemd-0.8.0/pystemd/utils.py`

 * *Files identical despite different names*

### Comparing `pystemd-0.7.0/pystemd.egg-info/PKG-INFO` & `pystemd-0.8.0/pystemd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pystemd
-Version: 0.7.0
+Version: 0.8.0
 Summary: A systemd binding for python
 Home-page: https://github.com/facebookincubator/pystemd
 Author: Alvaro Leiva
 Author-email: aleivag@fb.com
 License: LGPL-2.1+
 Description: pystemd
         =======
         
-        [![Build Status](https://travis-ci.org/facebookincubator/pystemd.svg)](http://travis-ci.org/facebookincubator/pystemd) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+        ![Continuous Integration](https://github.com/facebookincubator/pystemd/workflows/Continuous%20Integration/badge.svg?event=push)
         
         This library allows you to talk to systemd over dbus from python, without
         actually thinking that you are talking to systemd over dbus. This allows you to
         programmatically start/stop/restart/kill and verify services status from
         systemd point of view, avoiding executing `subprocess.Popen(['systemctl', ...`
         and then parsing the output to know the result.
         
@@ -219,15 +219,15 @@
         
         * Python headers: Just use your distro's package (e.g. python-dev).
         * systemd headers: Chances are you already have this. Normally, it is called
         `libsystemd-dev` or `systemd-devel`. You need to have at least v237.
         Please note that CentOS 7 ships with version 219. To work around this, please read
           [this](_docs/centos7.md).
         * systemd library: check if `pkg-config --cflags --libs libsystemd` returns
-        `-lsystemd` if not you can install normally install `systemd-libs` or
+        `-lsystemd` if not you can install `systemd-libs` or
         `libsystemd` depending on your distribution, version needs to be at least
         v237.
         * gcc: or any compiler that `setup.py` will accept.
         
         if you want to install from source then after you clone this repo you need to
         
         ```bash
@@ -263,11 +263,12 @@
 Platform: UNKNOWN
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Description-Content-Type: text/markdown
```

### Comparing `pystemd-0.7.0/pystemd.egg-info/SOURCES.txt` & `pystemd-0.8.0/pystemd.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,36 +3,42 @@
 README.md
 setup.cfg
 setup.py
 pystemd/RELEASE
 pystemd/__init__.py
 pystemd/__version__.py
 pystemd/base.py
+pystemd/base.pyi
 pystemd/daemon.c
+pystemd/daemon.pyi
 pystemd/daemon.pyx
 pystemd/dbusexc.c
 pystemd/dbusexc.pyx
 pystemd/dbuslib.c
+pystemd/dbuslib.pyi
 pystemd/dbuslib.pyx
 pystemd/exceptions.py
 pystemd/journal.c
 pystemd/journal.pyx
 pystemd/run.py
 pystemd/utils.py
+pystemd/utils.pyi
 pystemd.egg-info/PKG-INFO
 pystemd.egg-info/SOURCES.txt
 pystemd.egg-info/dependency_links.txt
 pystemd.egg-info/top_level.txt
 pystemd/DBus/__init__.py
 pystemd/machine1/__init__.py
 pystemd/machine1/machine.py
 pystemd/machine1/manager.py
 pystemd/systemd1/__init__.py
 pystemd/systemd1/manager.py
+pystemd/systemd1/manager.pyi
 pystemd/systemd1/unit.py
+pystemd/systemd1/unit.pyi
 pystemd/systemd1/unit_signatures.py
 tests/test_base.py
 tests/test_daemon.py
 tests/test_dbus_arg_parsing.py
 tests/test_dbuslib.py
 tests/test_journal.py
 tests/test_unit_signatures.py
```

### Comparing `pystemd-0.7.0/setup.py` & `pystemd-0.8.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -70,14 +70,17 @@
 
         external_modules = cythonize(
             [Extension("*", ["pystemd/*.pyx"], libraries=["systemd"])]
         )
     except ImportError:
         raise RuntimeError("Cython not installed.")
 
+package_data = ["pystemd/RELEASE"]
+package_data.extend(glob.glob("pystemd/*.pyi"))
+package_data.extend(glob.glob("pystemd/*/*.pyi"))
 
 setup(
     name="pystemd",
     version=__version__,
     packages=["pystemd", "pystemd.systemd1", "pystemd.machine1", "pystemd.DBus"],
     author="Alvaro Leiva",
     author_email="aleivag@fb.com",
@@ -86,18 +89,21 @@
     classifiers=[
         "Operating System :: POSIX :: Linux",
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
         "Development Status :: 3 - Alpha",
         "Topic :: Utilities",
         "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
     ],
     keywords=["systemd"],
     description="A systemd binding for python",
-    package_data={"pystemd": ["RELEASE"]},
+    package_data={
+        "pystemd": [str(Path(p).relative_to("pystemd")) for p in package_data]
+    },
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="LGPL-2.1+",
 )
```

### Comparing `pystemd-0.7.0/tests/test_base.py` & `pystemd-0.8.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pystemd-0.7.0/tests/test_daemon.py` & `pystemd-0.8.0/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `pystemd-0.7.0/tests/test_dbus_arg_parsing.py` & `pystemd-0.8.0/tests/test_dbus_arg_parsing.py`

 * *Files identical despite different names*

### Comparing `pystemd-0.7.0/tests/test_dbuslib.py` & `pystemd-0.8.0/tests/test_dbuslib.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     def test_weird_decode(self):
         self.assertEqual(path_decode(b"/o/s1_2eservice", b"/o"), self.EXTERNAL_ID)
 
 
 class TestDBusError(TestCase):
     def test_connecting_to_serverless_socket_raises_connection_refused_error(
-        self
+        self,
     ) -> None:
         with tempfile.TemporaryDirectory() as temporary_directory:
             socket_path = pathlib.Path(temporary_directory) / "test_socket"
             with socket.socket(
                 family=socket.AF_UNIX, type=socket.SOCK_STREAM
             ) as server:
                 server.bind(bytes(socket_path))
```

### Comparing `pystemd-0.7.0/tests/test_journal.py` & `pystemd-0.8.0/tests/test_journal.py`

 * *Files identical despite different names*

### Comparing `pystemd-0.7.0/tests/test_unit_signatures.py` & `pystemd-0.8.0/tests/test_unit_signatures.py`

 * *Files identical despite different names*

### Comparing `pystemd-0.7.0/tests/test_utils.py` & `pystemd-0.8.0/tests/test_utils.py`

 * *Files identical despite different names*

