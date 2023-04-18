# Comparing `tmp/pysetns-0.2.2.tar.gz` & `tmp/pysetns-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pysetns/pysetns/dist/tmptvtq5yt4/pysetns-0.2.2.tar", last modified: Fri Feb  4 06:42:22 2022, max compression
+gzip compressed data, was "pysetns-0.2.3.tar", last modified: Tue Apr 18 15:52:26 2023, max compression
```

## Comparing `pysetns-0.2.2.tar` & `pysetns-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 06:42:22.000000 pysetns-0.2.2/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1073 2022-02-04 06:42:02.000000 pysetns-0.2.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 06:42:22.000000 pysetns-0.2.2/src/
--rw-r--r--   0 runner    (1001) docker     (121)     4071 2022-02-04 06:42:02.000000 pysetns-0.2.2/src/ext.c
--rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-02-04 06:42:02.000000 pysetns-0.2.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 06:42:22.000000 pysetns-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2214 2022-02-04 06:42:22.000000 pysetns-0.2.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 06:42:22.000000 pysetns-0.2.2/pysetns/
--rw-r--r--   0 runner    (1001) docker     (121)    10807 2022-02-04 06:42:02.000000 pysetns-0.2.2/pysetns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 06:42:22.000000 pysetns-0.2.2/pysetns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-02-04 06:42:22.000000 pysetns-0.2.2/pysetns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2214 2022-02-04 06:42:22.000000 pysetns-0.2.2/pysetns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-02-04 06:42:22.000000 pysetns-0.2.2/pysetns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 06:42:22.000000 pysetns-0.2.2/pysetns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-02-04 06:42:02.000000 pysetns-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:52:26.440292 pysetns-0.2.3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1073 2023-04-18 15:52:15.000000 pysetns-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-18 15:52:26.440292 pysetns-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-18 15:52:15.000000 pysetns-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:52:26.440292 pysetns-0.2.3/pysetns/
+-rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-04-18 15:52:15.000000 pysetns-0.2.3/pysetns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:52:26.440292 pysetns-0.2.3/pysetns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-18 15:52:26.000000 pysetns-0.2.3/pysetns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-18 15:52:26.000000 pysetns-0.2.3/pysetns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:52:26.000000 pysetns-0.2.3/pysetns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 15:52:26.000000 pysetns-0.2.3/pysetns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:52:26.440292 pysetns-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-18 15:52:15.000000 pysetns-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:52:26.440292 pysetns-0.2.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-18 15:52:15.000000 pysetns-0.2.3/src/ext.c
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pysetns-0.2.2/LICENSE` & `pysetns-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pysetns-0.2.2/src/ext.c` & `pysetns-0.2.3/src/ext.c`

 * *Files identical despite different names*

### Comparing `pysetns-0.2.2/setup.py` & `pysetns-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `pysetns-0.2.2/PKG-INFO` & `pysetns-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: pysetns
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python wrapper for setns Linux syscall.
 Home-page: https://github.com/baskiton/pysetns
 Author: Alexander Baskikh
 Author-email: baskiton@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/baskiton/pysetns
 Project-URL: Bug Tracker, https://github.com/baskiton/pysetns/issues
 Keywords: linux kernel namespace setns
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: System :: Operating System Kernels :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pysetns
 [![pypi](https://img.shields.io/pypi/v/pysetns?logo=python&logoColor=white)](https://pypi.org/project/pysetns/)
 [![downloads](https://img.shields.io/pypi/dm/pysetns?logo=python&logoColor=white)](https://pypi.org/project/pysetns/)
 [![license](https://img.shields.io/pypi/l/pysetns?logo=open-source-initiative&logoColor=white)](https://github.com/baskiton/pysetns/blob/main/LICENSE)
 
-[![build](https://img.shields.io/github/workflow/status/baskiton/pysetns/build?logo=github)](https://github.com/baskiton/pysetns/actions/workflows/build.yml)
-[![upload](https://img.shields.io/github/workflow/status/baskiton/pysetns/upload?label=upload&logo=github)](https://github.com/baskiton/pysetns/actions/workflows/pypi-upload.yml)
+[![build](https://img.shields.io/github/actions/workflow/status/baskiton/pysetns/build.yml?logo=github)](https://github.com/baskiton/pysetns/actions/workflows/build.yml)
+[![upload](https://img.shields.io/github/actions/workflow/status/baskiton/pysetns/pypi-upload.yml?label=upload&logo=github)](https://github.com/baskiton/pysetns/actions/workflows/pypi-upload.yml)
 [![docs](https://img.shields.io/readthedocs/pysetns?logo=readthedocs&logoColor=white)][documentation]
 
 `pysetns` - is a Python wrapper for the Linux `setns` system call. \
 See the [manpage][man_setns] for an introduction to `setns` and namespaces.
 
 To detail see the [documentation][documentation]
 
@@ -54,9 +53,7 @@
 ## Usage
 See [examples][examples]
 
 
 [man_setns]: https://man7.org/linux/man-pages/man2/setns.2.html
 [examples]: https://github.com/baskiton/pysetns/blob/main/examples
 [documentation]: https://pysetns.readthedocs.io
-
-
```

### Comparing `pysetns-0.2.2/pysetns/__init__.py` & `pysetns-0.2.3/pysetns/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import errno
 import os
 
 from typing import Callable, Union, Iterable
 
 from . import ext
 
-__version__ = '0.2.2'
+__version__ = '0.2.3'
 
 NS_TIME = ext.CLONE_NEWTIME     # time namespace (since Linux 5.8)
 NS_MNT = ext.CLONE_NEWNS        # mount namespace group (since Linux 3.8)
 NS_CGROUP = ext.CLONE_NEWCGROUP # cgroup namespace (since Linux 4.6)
 NS_UTS = ext.CLONE_NEWUTS       # utsname namespace (since Linux 3.0)
 NS_IPC = ext.CLONE_NEWIPC       # ipc namespace (since Linux 3.0)
 NS_USER = ext.CLONE_NEWUSER     # user namespace (since Linux 3.8)
@@ -230,19 +230,25 @@
             return os.open(f'/proc/{pid}/ns/{ns_str}', _OFLAGS)
         except OSError:
             return -1
 
     @staticmethod
     def _disallow_user_ns(target_pid) -> bool:
         # It is not permitted to use setns(2) to reenter the caller's current user namespace
-        try:
-            parent_ino = os.stat(f'/proc/{os.getpid()}/ns/user').st_ino
-            target_ino = os.stat(f'/proc/{target_pid}/ns/user').st_ino
-            return parent_ino == target_ino
-        except:
+        pp = f'/proc/{os.getpid()}'
+        tp = f'/proc/{target_pid}'
+        if os.path.isdir(pp) and os.path.isdir(tp):
+            try:
+                parent_ino = os.stat(os.path.join(pp, 'ns/user')).st_ino
+                target_ino = os.stat(os.path.join(tp, 'ns/user')).st_ino
+                return parent_ino == target_ino
+            except OSError:
+                # user namespace is not exist. disallow
+                return True
+        else:
             raise OSError(errno.ESRCH, os.strerror(errno.ESRCH))
 
     @staticmethod
     def _close_fds(fds: Union[int, Iterable]) -> None:
         if isinstance(fds, Iterable):
             for fd in fds:
                 Namespace._close_fds(fd)
```

### Comparing `pysetns-0.2.2/pysetns.egg-info/PKG-INFO` & `pysetns-0.2.3/pysetns.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: pysetns
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python wrapper for setns Linux syscall.
 Home-page: https://github.com/baskiton/pysetns
 Author: Alexander Baskikh
 Author-email: baskiton@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/baskiton/pysetns
 Project-URL: Bug Tracker, https://github.com/baskiton/pysetns/issues
 Keywords: linux kernel namespace setns
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: System :: Operating System Kernels :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pysetns
 [![pypi](https://img.shields.io/pypi/v/pysetns?logo=python&logoColor=white)](https://pypi.org/project/pysetns/)
 [![downloads](https://img.shields.io/pypi/dm/pysetns?logo=python&logoColor=white)](https://pypi.org/project/pysetns/)
 [![license](https://img.shields.io/pypi/l/pysetns?logo=open-source-initiative&logoColor=white)](https://github.com/baskiton/pysetns/blob/main/LICENSE)
 
-[![build](https://img.shields.io/github/workflow/status/baskiton/pysetns/build?logo=github)](https://github.com/baskiton/pysetns/actions/workflows/build.yml)
-[![upload](https://img.shields.io/github/workflow/status/baskiton/pysetns/upload?label=upload&logo=github)](https://github.com/baskiton/pysetns/actions/workflows/pypi-upload.yml)
+[![build](https://img.shields.io/github/actions/workflow/status/baskiton/pysetns/build.yml?logo=github)](https://github.com/baskiton/pysetns/actions/workflows/build.yml)
+[![upload](https://img.shields.io/github/actions/workflow/status/baskiton/pysetns/pypi-upload.yml?label=upload&logo=github)](https://github.com/baskiton/pysetns/actions/workflows/pypi-upload.yml)
 [![docs](https://img.shields.io/readthedocs/pysetns?logo=readthedocs&logoColor=white)][documentation]
 
 `pysetns` - is a Python wrapper for the Linux `setns` system call. \
 See the [manpage][man_setns] for an introduction to `setns` and namespaces.
 
 To detail see the [documentation][documentation]
 
@@ -54,9 +53,7 @@
 ## Usage
 See [examples][examples]
 
 
 [man_setns]: https://man7.org/linux/man-pages/man2/setns.2.html
 [examples]: https://github.com/baskiton/pysetns/blob/main/examples
 [documentation]: https://pysetns.readthedocs.io
-
-
```

### Comparing `pysetns-0.2.2/README.md` & `pysetns-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pysetns
 [![pypi](https://img.shields.io/pypi/v/pysetns?logo=python&logoColor=white)](https://pypi.org/project/pysetns/)
 [![downloads](https://img.shields.io/pypi/dm/pysetns?logo=python&logoColor=white)](https://pypi.org/project/pysetns/)
 [![license](https://img.shields.io/pypi/l/pysetns?logo=open-source-initiative&logoColor=white)](https://github.com/baskiton/pysetns/blob/main/LICENSE)
 
-[![build](https://img.shields.io/github/workflow/status/baskiton/pysetns/build?logo=github)](https://github.com/baskiton/pysetns/actions/workflows/build.yml)
-[![upload](https://img.shields.io/github/workflow/status/baskiton/pysetns/upload?label=upload&logo=github)](https://github.com/baskiton/pysetns/actions/workflows/pypi-upload.yml)
+[![build](https://img.shields.io/github/actions/workflow/status/baskiton/pysetns/build.yml?logo=github)](https://github.com/baskiton/pysetns/actions/workflows/build.yml)
+[![upload](https://img.shields.io/github/actions/workflow/status/baskiton/pysetns/pypi-upload.yml?label=upload&logo=github)](https://github.com/baskiton/pysetns/actions/workflows/pypi-upload.yml)
 [![docs](https://img.shields.io/readthedocs/pysetns?logo=readthedocs&logoColor=white)][documentation]
 
 `pysetns` - is a Python wrapper for the Linux `setns` system call. \
 See the [manpage][man_setns] for an introduction to `setns` and namespaces.
 
 To detail see the [documentation][documentation]
```

