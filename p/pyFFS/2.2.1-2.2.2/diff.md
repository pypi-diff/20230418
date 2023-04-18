# Comparing `tmp/pyFFS-2.2.1.tar.gz` & `tmp/pyFFS-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyFFS-2.2.1.tar", last modified: Wed Sep 29 10:02:24 2021, max compression
+gzip compressed data, was "pyFFS-2.2.2.tar", last modified: Tue Apr 18 11:52:22 2023, max compression
```

## Comparing `pyFFS-2.2.1.tar` & `pyFFS-2.2.2.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2021-09-29 10:02:24.856482 pyFFS-2.2.1/
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      510 2021-06-30 14:27:48.000000 pyFFS-2.2.1/.readthedocs.yaml
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      145 2021-09-29 10:02:24.000000 pyFFS-2.2.1/AUTHORS
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     4056 2021-09-29 10:02:24.000000 pyFFS-2.2.1/ChangeLog
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1523 2021-06-30 14:27:48.000000 pyFFS-2.2.1/LICENSE.txt
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     3213 2021-09-29 10:02:24.856482 pyFFS-2.2.1/PKG-INFO
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1842 2021-09-29 10:00:08.000000 pyFFS-2.2.1/README.rst
-drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2021-09-29 10:02:24.848482 pyFFS-2.2.1/doc/
-drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2021-09-29 10:02:24.848482 pyFFS-2.2.1/doc/api/
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      796 2021-06-30 14:27:48.000000 pyFFS-2.2.1/doc/api/index.rst
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      104 2021-06-30 14:27:48.000000 pyFFS-2.2.1/doc/api/pyffs.czt.rst
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      104 2021-06-30 14:27:48.000000 pyFFS-2.2.1/doc/api/pyffs.ffs.rst
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      107 2021-06-30 14:27:48.000000 pyFFS-2.2.1/doc/api/pyffs.func.rst
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      113 2021-06-30 14:27:48.000000 pyFFS-2.2.1/doc/api/pyffs.interp.rst
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      107 2021-06-30 14:27:48.000000 pyFFS-2.2.1/doc/api/pyffs.util.rst
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     2745 2021-09-27 13:49:43.000000 pyFFS-2.2.1/doc/conf.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1072 2021-06-30 14:27:48.000000 pyFFS-2.2.1/doc/index.rst
-drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2021-09-29 10:02:24.848482 pyFFS-2.2.1/doc/theory/
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1597 2021-06-30 14:27:48.000000 pyFFS-2.2.1/doc/theory/CZT.rst
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1208 2021-06-30 14:27:48.000000 pyFFS-2.2.1/doc/theory/DFT.rst
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     5564 2021-06-30 14:27:48.000000 pyFFS-2.2.1/doc/theory/FS_eval_for_BL_signals.rst
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     4712 2021-06-30 14:27:48.000000 pyFFS-2.2.1/doc/theory/func_interpolation_BL_signals.rst
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      360 2021-06-30 14:27:48.000000 pyFFS-2.2.1/doc/theory/index.rst
-drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2021-09-29 10:02:24.852482 pyFFS-2.2.1/examples/
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     2191 2021-09-27 13:49:43.000000 pyFFS-2.2.1/examples/convolve_1d.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     4371 2021-09-29 09:54:45.000000 pyFFS-2.2.1/examples/convolve_2d.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      916 2021-09-27 13:49:43.000000 pyFFS-2.2.1/examples/ffs_1d.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1435 2021-09-27 13:49:43.000000 pyFFS-2.2.1/examples/ffs_2d.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     2891 2021-09-27 13:49:43.000000 pyFFS-2.2.1/examples/interp_1d.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     4620 2021-09-27 13:49:43.000000 pyFFS-2.2.1/examples/interp_2d.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1668 2021-09-27 13:49:43.000000 pyFFS-2.2.1/examples/util.py
--rwxrwxr-x   0 bezzam    (1001) bezzam    (1001)      132 2021-09-27 13:49:43.000000 pyFFS-2.2.1/format_code.sh
-drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2021-09-29 10:02:24.852482 pyFFS-2.2.1/profile/
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     4835 2021-09-27 13:49:43.000000 pyFFS-2.2.1/profile/bandlimited_interp1d_vary_M.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     2944 2021-09-27 13:49:43.000000 pyFFS-2.2.1/profile/bandlimited_interp1d_vary_width.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     4749 2021-09-27 13:49:43.000000 pyFFS-2.2.1/profile/bandlimited_interp2d_vary_M.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     3688 2021-09-27 13:49:43.000000 pyFFS-2.2.1/profile/bandlimited_interp2d_vary_width.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     2438 2021-09-29 09:54:45.000000 pyFFS-2.2.1/profile/convolve2d.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     2383 2021-09-27 13:49:43.000000 pyFFS-2.2.1/profile/ffs.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     2848 2021-09-27 13:49:43.000000 pyFFS-2.2.1/profile/ffsn.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     3141 2021-09-27 13:49:43.000000 pyFFS-2.2.1/profile/fs_interp1d_vary_M.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     3213 2021-09-27 13:49:43.000000 pyFFS-2.2.1/profile/fs_interp1d_vary_NFS.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     2842 2021-09-27 13:49:43.000000 pyFFS-2.2.1/profile/fs_interp2d_vary_M.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     3461 2021-09-27 13:49:43.000000 pyFFS-2.2.1/profile/fs_interp2d_vary_NFS.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     3883 2021-09-27 13:49:43.000000 pyFFS-2.2.1/profile/util.py
-drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2021-09-29 10:02:24.852482 pyFFS-2.2.1/pyFFS.egg-info/
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     3213 2021-09-29 10:02:24.000000 pyFFS-2.2.1/pyFFS.egg-info/PKG-INFO
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1305 2021-09-29 10:02:24.000000 pyFFS-2.2.1/pyFFS.egg-info/SOURCES.txt
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)        1 2021-09-29 10:02:24.000000 pyFFS-2.2.1/pyFFS.egg-info/dependency_links.txt
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)       46 2021-09-29 10:02:24.000000 pyFFS-2.2.1/pyFFS.egg-info/pbr.json
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      221 2021-09-29 10:02:24.000000 pyFFS-2.2.1/pyFFS.egg-info/requires.txt
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)        6 2021-09-29 10:02:24.000000 pyFFS-2.2.1/pyFFS.egg-info/top_level.txt
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)        1 2021-06-30 14:29:52.000000 pyFFS-2.2.1/pyFFS.egg-info/zip-safe
-drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2021-09-29 10:02:24.856482 pyFFS-2.2.1/pyffs/
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      623 2021-09-27 13:49:43.000000 pyFFS-2.2.1/pyffs/__init__.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     4389 2021-06-30 14:27:48.000000 pyFFS-2.2.1/pyffs/backend.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     3334 2021-09-29 09:54:45.000000 pyFFS-2.2.1/pyffs/conv.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     5667 2021-06-30 14:27:48.000000 pyFFS-2.2.1/pyffs/czt.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)    11063 2021-09-27 13:49:43.000000 pyFFS-2.2.1/pyffs/ffs.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     3866 2021-09-27 13:49:43.000000 pyFFS-2.2.1/pyffs/func.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     7553 2021-09-27 13:49:43.000000 pyFFS-2.2.1/pyffs/interp.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)    13966 2021-09-29 09:54:45.000000 pyFFS-2.2.1/pyffs/util.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      121 2021-09-27 13:49:43.000000 pyFFS-2.2.1/requirements.txt
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1079 2021-09-29 10:02:24.856482 pyFFS-2.2.1/setup.cfg
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      353 2021-06-30 14:27:48.000000 pyFFS-2.2.1/setup.py
-drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2021-09-29 10:02:24.856482 pyFFS-2.2.1/test/
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1799 2021-06-30 14:27:48.000000 pyFFS-2.2.1/test/test_czt.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     4688 2021-06-30 14:27:48.000000 pyFFS-2.2.1/test/test_ffs.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     2757 2021-06-30 14:27:48.000000 pyFFS-2.2.1/test/test_interp.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     3141 2021-09-27 13:49:43.000000 pyFFS-2.2.1/test/test_util.py
--rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1846 2021-09-27 13:49:43.000000 pyFFS-2.2.1/test.py
+drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2023-04-18 11:52:22.217771 pyFFS-2.2.2/
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      510 2021-06-30 14:27:48.000000 pyFFS-2.2.2/.readthedocs.yaml
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      145 2023-04-18 11:52:21.000000 pyFFS-2.2.2/AUTHORS
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     4259 2023-04-18 11:52:21.000000 pyFFS-2.2.2/ChangeLog
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1523 2021-06-30 14:27:48.000000 pyFFS-2.2.2/LICENSE.txt
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     3666 2023-04-18 11:52:22.217771 pyFFS-2.2.2/PKG-INFO
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     2878 2023-04-18 11:45:13.000000 pyFFS-2.2.2/README.rst
+drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2023-04-18 11:52:22.209771 pyFFS-2.2.2/doc/
+drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2023-04-18 11:52:22.209771 pyFFS-2.2.2/doc/api/
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      905 2023-04-18 11:45:13.000000 pyFFS-2.2.2/doc/api/index.rst
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      107 2023-04-18 11:45:13.000000 pyFFS-2.2.2/doc/api/pyffs.conv.rst
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      104 2021-06-30 14:27:48.000000 pyFFS-2.2.2/doc/api/pyffs.czt.rst
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      104 2021-06-30 14:27:48.000000 pyFFS-2.2.2/doc/api/pyffs.ffs.rst
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      107 2021-06-30 14:27:48.000000 pyFFS-2.2.2/doc/api/pyffs.func.rst
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      113 2021-06-30 14:27:48.000000 pyFFS-2.2.2/doc/api/pyffs.interp.rst
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      107 2021-06-30 14:27:48.000000 pyFFS-2.2.2/doc/api/pyffs.util.rst
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     2745 2022-12-23 11:12:06.000000 pyFFS-2.2.2/doc/conf.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1072 2021-06-30 14:27:48.000000 pyFFS-2.2.2/doc/index.rst
+drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2023-04-18 11:52:22.209771 pyFFS-2.2.2/doc/theory/
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1597 2021-06-30 14:27:48.000000 pyFFS-2.2.2/doc/theory/CZT.rst
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1208 2021-06-30 14:27:48.000000 pyFFS-2.2.2/doc/theory/DFT.rst
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     5564 2021-06-30 14:27:48.000000 pyFFS-2.2.2/doc/theory/FS_eval_for_BL_signals.rst
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     4712 2021-06-30 14:27:48.000000 pyFFS-2.2.2/doc/theory/func_interpolation_BL_signals.rst
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      360 2021-06-30 14:27:48.000000 pyFFS-2.2.2/doc/theory/index.rst
+drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2023-04-18 11:52:22.213771 pyFFS-2.2.2/examples/
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     2173 2022-04-17 09:13:58.000000 pyFFS-2.2.2/examples/convolve_1d.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     4371 2021-09-29 09:54:45.000000 pyFFS-2.2.2/examples/convolve_2d.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      916 2021-09-27 13:49:43.000000 pyFFS-2.2.2/examples/ffs_1d.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1435 2021-09-27 13:49:43.000000 pyFFS-2.2.2/examples/ffs_2d.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     2891 2022-04-14 14:28:01.000000 pyFFS-2.2.2/examples/interp_1d.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     4690 2022-04-17 12:55:51.000000 pyFFS-2.2.2/examples/interp_2d.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1753 2022-04-17 09:28:24.000000 pyFFS-2.2.2/examples/util.py
+-rwxrwxr-x   0 bezzam    (1001) bezzam    (1001)      132 2021-09-27 13:49:43.000000 pyFFS-2.2.2/format_code.sh
+drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2023-04-18 11:52:22.213771 pyFFS-2.2.2/profile/
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     4835 2022-04-14 14:27:09.000000 pyFFS-2.2.2/profile/bandlimited_interp1d_vary_M.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     2944 2021-09-27 13:49:43.000000 pyFFS-2.2.2/profile/bandlimited_interp1d_vary_width.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     4749 2022-04-14 14:28:01.000000 pyFFS-2.2.2/profile/bandlimited_interp2d_vary_M.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     3688 2022-04-14 14:28:01.000000 pyFFS-2.2.2/profile/bandlimited_interp2d_vary_width.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     2413 2022-04-17 09:26:02.000000 pyFFS-2.2.2/profile/convolve2d.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     2383 2021-09-27 13:49:43.000000 pyFFS-2.2.2/profile/ffs.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     2848 2022-04-14 14:28:01.000000 pyFFS-2.2.2/profile/ffsn.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     3141 2022-04-14 14:28:01.000000 pyFFS-2.2.2/profile/fs_interp1d_vary_M.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     3213 2022-04-14 14:28:01.000000 pyFFS-2.2.2/profile/fs_interp1d_vary_NFS.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     2842 2021-09-27 13:49:43.000000 pyFFS-2.2.2/profile/fs_interp2d_vary_M.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     3461 2021-09-27 13:49:43.000000 pyFFS-2.2.2/profile/fs_interp2d_vary_NFS.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     3934 2022-04-17 09:20:24.000000 pyFFS-2.2.2/profile/util.py
+drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2023-04-18 11:52:22.213771 pyFFS-2.2.2/pyFFS.egg-info/
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     3666 2023-04-18 11:52:21.000000 pyFFS-2.2.2/pyFFS.egg-info/PKG-INFO
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1328 2023-04-18 11:52:22.000000 pyFFS-2.2.2/pyFFS.egg-info/SOURCES.txt
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)        1 2023-04-18 11:52:21.000000 pyFFS-2.2.2/pyFFS.egg-info/dependency_links.txt
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)       46 2023-04-18 11:52:21.000000 pyFFS-2.2.2/pyFFS.egg-info/pbr.json
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      221 2023-04-18 11:52:21.000000 pyFFS-2.2.2/pyFFS.egg-info/requires.txt
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)        6 2023-04-18 11:52:21.000000 pyFFS-2.2.2/pyFFS.egg-info/top_level.txt
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)        1 2021-06-30 14:29:52.000000 pyFFS-2.2.2/pyFFS.egg-info/zip-safe
+drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2023-04-18 11:52:22.217771 pyFFS-2.2.2/pyffs/
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      623 2021-09-27 13:49:43.000000 pyFFS-2.2.2/pyffs/__init__.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     4529 2023-04-18 11:45:13.000000 pyFFS-2.2.2/pyffs/backend.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     3334 2021-09-29 09:54:45.000000 pyFFS-2.2.2/pyffs/conv.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     5667 2021-06-30 14:27:48.000000 pyFFS-2.2.2/pyffs/czt.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)    11063 2021-09-27 13:49:43.000000 pyFFS-2.2.2/pyffs/ffs.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     3866 2021-09-27 13:49:43.000000 pyFFS-2.2.2/pyffs/func.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     7553 2021-09-27 13:49:43.000000 pyFFS-2.2.2/pyffs/interp.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)    13966 2021-09-29 09:54:45.000000 pyFFS-2.2.2/pyffs/util.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      121 2023-04-18 11:51:03.000000 pyFFS-2.2.2/requirements.txt
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1079 2023-04-18 11:52:22.217771 pyFFS-2.2.2/setup.cfg
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      353 2021-06-30 14:27:48.000000 pyFFS-2.2.2/setup.py
+drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2023-04-18 11:52:22.217771 pyFFS-2.2.2/test/
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1799 2021-06-30 14:27:48.000000 pyFFS-2.2.2/test/test_czt.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     4688 2021-06-30 14:27:48.000000 pyFFS-2.2.2/test/test_ffs.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     2757 2021-06-30 14:27:48.000000 pyFFS-2.2.2/test/test_interp.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     3141 2022-04-14 14:28:01.000000 pyFFS-2.2.2/test/test_util.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1846 2022-04-14 14:28:01.000000 pyFFS-2.2.2/test.py
```

### Comparing `pyFFS-2.2.1/ChangeLog` & `pyFFS-2.2.2/ChangeLog`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 CHANGES
 =======
 
+v2.2.2
+------
+
+* Fix requirements. (#29)
+* [backend][BugFix] Testing for a CuPy install insufficient
+* Change to arxiv link
+* Add citation
+* Add convolution documentation. (#27)
+* Edit publishing steps
+
 v2.2.1
 ------
 
 * Refactor ffs\_shift operations
 * Fix link in README
 * Update README with publishing info
```

### Comparing `pyFFS-2.2.1/LICENSE.txt` & `pyFFS-2.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/PKG-INFO` & `pyFFS-2.2.2/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,96 +1,101 @@
-Metadata-Version: 2.1
-Name: pyFFS
-Version: 2.2.1
-Summary: Fast Fourier Series library
-Home-page: https://github.com/imagingofthings/pyFFS
-Author: Sepand KASHANI, Eric BEZZAM, Matthieu SIMEONI
-Author-email: kashani.sepand@gmail.com
-License: BSD
-Download-URL: https://github.com/imagingofthings/pyFFS
-Description: .. #############################################################################
-        .. README.rst
-        .. ==========
-        .. Author : Sepand KASHANI [kashani.sepand@gmail.com]
-        .. #############################################################################
-        
-        #####
-        pyFFS
-        #####
-        
-        *pyFFS* is a collection of efficient algorithms to compute Fourier Series and
-        related transforms.
-        
-        
-        Installation
-        ------------
-        
-        ::
-        
-            $ pip install pyFFS
-        
-        
-        Developer Install
-        -----------------
-        
-        Recommended setup using Anaconda, for optimized numerical libraries:
-        
-        ::
-        
-            # Create Anaconda environment
-            $ conda create --name pyffs python=3
-            $ conda activate pyffs
-        
-            # Clone repository
-            $ git clone https://github.com/imagingofthings/pyFFS.git
-            $ cd pyFFS
-            $ # git checkout <commit>
-        
-            # Install requirements with conda
-            $ conda install --file requirements.txt
-        
-            # Optionally install CuPy for GPU support
-            $ conda install -c conda-forge cupy
-        
-            # Install pyFFS
-            $ pip install -e .[dev]
-            $ pytest                        # Run test suite
-            $ python setup.py build_sphinx  # Generate documentation
-        
-        More information about CuPy setup can be found `here <https://docs.cupy.dev/en/stable/install.html#installation)>`_.
-        
-        New release
-        -----------
-        From master branch of original repo:
-        
-        ::
-        
-            # Create tag and upload
-            $ git tag -a vX.X.X -m "Description."
-            $ git push origin vX.X.X
-        
-            # Create package and upload to Pypi
-            $ python setup.py sdist
-            $ python -m twine upload  dist/pyFFS-X.X.X.tar.gz
-        
-        You will need a username and password for uploading to PyPi.
-        
-        Finally, `on GitHub <https://github.com/imagingofthings/pyFFS/releases>`_ set the new tag as the latest release by
-        pressing on it and at the bottom pressing "Create release".
-        
-        Remarks
-        -------
-        
-        pyFFS is developed and tested on x86_64 systems running Linux and macOS
-        Catalina.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst; charset=UTF-8
-Provides-Extra: dev
-Provides-Extra: cuda110
+.. #############################################################################
+.. README.rst
+.. ==========
+.. Author : Sepand KASHANI [kashani.sepand@gmail.com]
+.. #############################################################################
+
+#####
+pyFFS
+#####
+
+*pyFFS* is a collection of efficient algorithms to compute Fourier Series and
+related transforms.
+
+
+Installation
+------------
+
+::
+
+    $ pip install pyFFS
+
+
+Developer Install
+-----------------
+
+Recommended setup using Anaconda, for optimized numerical libraries:
+
+::
+
+    # Create Anaconda environment
+    $ conda create --name pyffs python=3
+    $ conda activate pyffs
+
+    # Clone repository
+    $ git clone https://github.com/imagingofthings/pyFFS.git
+    $ cd pyFFS
+    $ # git checkout <commit>
+
+    # Install requirements with conda
+    $ conda install --file requirements.txt
+
+    # Optionally install CuPy for GPU support
+    $ conda install -c conda-forge cupy
+
+    # Install pyFFS
+    $ pip install -e .[dev]
+    $ pytest                        # Run test suite
+    $ python setup.py build_sphinx  # Generate documentation
+
+More information about CuPy setup can be found `here <https://docs.cupy.dev/en/stable/install.html#installation)>`_.
+
+New release
+-----------
+From master branch of original repo:
+
+::
+
+    # Create tag and upload
+    $ git tag -a vX.X.X -m "Description."
+    $ git push origin vX.X.X
+
+    # Create package and upload to Pypi
+    $ python setup.py sdist
+    $ python -m twine upload  dist/pyFFS-X.X.X.tar.gz
+
+You will need a username and password for uploading to PyPi.
+
+Finally, `on GitHub <https://github.com/imagingofthings/pyFFS/releases>`_ set the new tag as the latest release by
+pressing on it, at top right selecting "Edit tag", and at the bottom pressing "Publish release".
+
+Remarks
+-------
+
+pyFFS is developed and tested on x86_64 systems running Linux and macOS
+Catalina.
+
+Citing this work
+----------------
+
+If you use this package in your own research, please cite `our paper <https://arxiv.org/abs/2110.00262>`_.
+
+::
+
+    @article{10.1137/21M1448641,
+        author = {Bezzam, Eric and Kashani, Sepand and Hurley, Paul and Vetterli, Martin and Simeoni, Matthieu},
+        title = {PyFFS: A Python Library for Fast Fourier Series Computation and Interpolation with GPU Acceleration},
+        year = {2022},
+        issue_date = {Aug 2022},
+        publisher = {Society for Industrial and Applied Mathematics},
+        address = {USA},
+        volume = {44},
+        number = {4},
+        issn = {1064-8275},
+        url = {https://doi.org/10.1137/21M1448641},
+        doi = {10.1137/21M1448641},
+        journal = {SIAM J. Sci. Comput.},
+        month = {jan},
+        pages = {C346–C366},
+        numpages = {21},
+        keywords = {GPU, chirp Z-transform, numerical library, 97N80, fast Fourier series, bandlimited interpolation, 65T40, 42B05, 97N50, Python}
+    }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyFFS-2.2.1/doc/api/index.rst` & `pyFFS-2.2.2/doc/api/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -37,18 +37,26 @@
     -----------------------
 
     .. autosummary::
 
       ~interp.fs_interp
       ~interp.fs_interpn
 
+    Circular Convolution
+    --------------------
+
+    .. autosummary::
+
+      ~conv.convolve
+
 
 Submodules
 ----------
 
 .. toctree::
 
    pyffs.czt
    pyffs.ffs
    pyffs.func
    pyffs.interp
+   pyffs.conv
    pyffs.util
```

### Comparing `pyFFS-2.2.1/doc/conf.py` & `pyFFS-2.2.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/doc/index.rst` & `pyFFS-2.2.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/doc/theory/CZT.rst` & `pyFFS-2.2.2/doc/theory/CZT.rst`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/doc/theory/DFT.rst` & `pyFFS-2.2.2/doc/theory/DFT.rst`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/doc/theory/FS_eval_for_BL_signals.rst` & `pyFFS-2.2.2/doc/theory/FS_eval_for_BL_signals.rst`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/doc/theory/func_interpolation_BL_signals.rst` & `pyFFS-2.2.2/doc/theory/func_interpolation_BL_signals.rst`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/examples/convolve_1d.py` & `pyFFS-2.2.2/examples/convolve_1d.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     convolve_scipy(diric_samples[idx], diric_samples[idx], mode="full", method="fft") / N_samples
 )
 output_fftconvolve = fftconvolve(diric_samples[idx], diric_samples[idx], mode="full") / N_samples
 t_vals_full = np.linspace(2 * np.min(sample_points), 2 * np.max(sample_points), num=len(output_fft))
 
 # plot
 fig, ax = plt.subplots(
-    nrows=2, ncols=1, num="Convolve bandlimited, periodic signals", figsize=(10, 10)
+    nrows=2, ncols=1, num="Convolve bandlimited, periodic signals"
 )
 ax[0].plot(sample_points[idx], diric_samples[idx])
 ax[0].set_xlim([np.min(sample_points), np.max(sample_points)])
 ax[0].set_ylabel("$f$")
 
 diric_samples_true = dirichlet(sample_points, T, 2 * T_c_diric, N_FS)
 ax[1].plot(
```

### Comparing `pyFFS-2.2.1/examples/convolve_2d.py` & `pyFFS-2.2.2/examples/convolve_2d.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/examples/ffs_1d.py` & `pyFFS-2.2.2/examples/ffs_1d.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/examples/ffs_2d.py` & `pyFFS-2.2.2/examples/ffs_2d.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/examples/interp_1d.py` & `pyFFS-2.2.2/examples/interp_1d.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/examples/interp_2d.py` & `pyFFS-2.2.2/examples/interp_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from scipy.interpolate import interp2d
 from scipy.signal import resample
 import matplotlib.pyplot as plt
 import pathlib as plib
 from util import plotting_setup, plot2d
 
 
-fig_path = plotting_setup()
+fig_path = plotting_setup(font_size=47  , figsize=(12, 10), linewidth=5)
 ALPHA = 0.8
 
 # signal parameters
 T = 2 * [1]
 T_c = 2 * [0]
 T_c_diric = 2 * [0.3]
 N_FS = 2 * [31]
@@ -62,15 +62,15 @@
 
 
 # -- plot cross section
 idx_yc = np.argmin(np.abs(points_y - y_val))
 idx_og = np.argmin(np.abs(np.squeeze(sample_points[1]) - y_val))
 idx_resample = np.argmin(np.abs(resampled_y - y_val))
 
-fig = plt.figure(figsize=(12, 10))
+fig = plt.figure()
 ax = fig.add_subplot(1, 1, 1)
 ax.plot(points_x, np.real(vals_true[:, idx_yc]), label="ground truth", alpha=ALPHA, linestyle="-")
 ax.plot(
     points_x, np.real(vals_ffs[:, idx_yc]), label="pyffs.fs_interpn", alpha=ALPHA, linestyle="--"
 )
 ax.plot(
     resampled_x,
@@ -78,14 +78,15 @@
     label="scipy.signal.resample",
     alpha=ALPHA,
     linestyle="-.",
 )
 ax.scatter(sample_points[0], diric_samples[:, idx_og], label="available samples")
 ax.set_xlabel("x [m]")
 ax.set_xlim([start[0], stop[0]])
+plt.xticks([0.25, 0.3, 0.35, 0.4, 0.45])
 plt.legend()
 plt.tight_layout()
 fig.savefig(plib.Path(fig_path) / "interp_2d_output_slice.png")
 
 # --- 2D plots
 pcolormesh = True
 x_shift = (sample_points[0][1, 0] - sample_points[0][0, 0]) / 2
```

### Comparing `pyFFS-2.2.1/examples/util.py` & `pyFFS-2.2.2/examples/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib
 import pathlib as plib
 
 
-def plotting_setup(font_size=30, linewidth=4, markersize=10, fig_folder="figs"):
+def plotting_setup(font_size=30, linewidth=4, markersize=10, fig_folder="figs", figsize=(10, 10)):
     font = {"family": "Times New Roman", "weight": "normal", "size": font_size}
     matplotlib.rc("font", **font)
+    matplotlib.rcParams["figure.figsize"] = figsize[0], figsize[1]
     matplotlib.rcParams["lines.linewidth"] = linewidth
     matplotlib.rcParams["lines.markersize"] = markersize
 
     fig_path = plib.Path(__file__).parent / fig_folder
     fig_path.mkdir(exist_ok=True)
     return fig_path
```

### Comparing `pyFFS-2.2.1/profile/bandlimited_interp1d_vary_M.py` & `pyFFS-2.2.2/profile/bandlimited_interp1d_vary_M.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/profile/bandlimited_interp1d_vary_width.py` & `pyFFS-2.2.2/profile/bandlimited_interp1d_vary_width.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/profile/bandlimited_interp2d_vary_M.py` & `pyFFS-2.2.2/profile/bandlimited_interp2d_vary_M.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/profile/bandlimited_interp2d_vary_width.py` & `pyFFS-2.2.2/profile/bandlimited_interp2d_vary_width.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/profile/convolve2d.py` & `pyFFS-2.2.2/profile/convolve2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pyffs.func import dirichlet_2D
 from scipy.signal import convolve2d as convolve_scipy
 
 
 @click.command()
 @click.option("--n_trials", type=int, default=1)
 def profile_ffsn(n_trials):
-    fig_path = plotting_setup(linewidth=3, font_size=20)
+    fig_path = plotting_setup()
 
     T = [1, 1]
     T_c = [0, 0]
     N_S_vals = np.logspace(np.log10(10), np.log10(300), num=10)
 
     n_std = 0.5
```

### Comparing `pyFFS-2.2.1/profile/ffs.py` & `pyFFS-2.2.2/profile/ffs.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/profile/ffsn.py` & `pyFFS-2.2.2/profile/ffsn.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/profile/fs_interp1d_vary_M.py` & `pyFFS-2.2.2/profile/fs_interp1d_vary_M.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/profile/fs_interp1d_vary_NFS.py` & `pyFFS-2.2.2/profile/fs_interp1d_vary_NFS.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/profile/fs_interp2d_vary_M.py` & `pyFFS-2.2.2/profile/fs_interp2d_vary_M.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/profile/fs_interp2d_vary_NFS.py` & `pyFFS-2.2.2/profile/fs_interp2d_vary_NFS.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/profile/util.py` & `pyFFS-2.2.2/profile/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 backend_to_label = {"numpy": "CPU", "cupy": "GPU"}
 
 
 def plotting_setup(font_size=30, linewidth=4, markersize=10, fig_folder="figs"):
     font = {"family": "Times New Roman", "weight": "normal", "size": font_size}
     matplotlib.rc("font", **font)
+    matplotlib.rcParams["figure.figsize"] = 10, 10
     matplotlib.rcParams["lines.linewidth"] = linewidth
     matplotlib.rcParams["lines.markersize"] = markersize
 
     fig_path = plib.Path(__file__).parent / fig_folder
     fig_path.mkdir(exist_ok=True)
     return fig_path
```

### Comparing `pyFFS-2.2.1/pyFFS.egg-info/SOURCES.txt` & `pyFFS-2.2.2/pyFFS.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 requirements.txt
 setup.cfg
 setup.py
 test.py
 doc/conf.py
 doc/index.rst
 doc/api/index.rst
+doc/api/pyffs.conv.rst
 doc/api/pyffs.czt.rst
 doc/api/pyffs.ffs.rst
 doc/api/pyffs.func.rst
 doc/api/pyffs.interp.rst
 doc/api/pyffs.util.rst
 doc/theory/CZT.rst
 doc/theory/DFT.rst
```

### Comparing `pyFFS-2.2.1/pyffs/__init__.py` & `pyFFS-2.2.2/pyffs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/pyffs/backend.py` & `pyFFS-2.2.2/pyffs/backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,21 +15,24 @@
 
 import os
 
 import numpy as np
 import scipy.fft
 
 
-CUPY_ENABLED = util.find_spec("cupy") is not None and int(os.getenv("CUPY_PYFFS", 1)) == 1
+CUPY_ENABLED = (util.find_spec("cupy") is not None) and (int(os.getenv("CUPY_PYFFS", 1)) == 1)
 AVAILABLE_MOD = [np]
 if CUPY_ENABLED:
-    import cupy as cp
-    import cupyx
-
-    AVAILABLE_MOD.append(cp)
+    try:
+        import cupy as cp
+        import cupyx
+        AVAILABLE_MOD.append(cp)
+    except ImportError:
+        # CuPy is installed, but GPU drivers probably missing.
+        CUPY_ENABLED = False
 
 
 def get_module(backend="numpy"):
     """
     Returns correct numerical module based on backend string.
 
     Parameters
```

### Comparing `pyFFS-2.2.1/pyffs/conv.py` & `pyFFS-2.2.2/pyffs/conv.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/pyffs/czt.py` & `pyFFS-2.2.2/pyffs/czt.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/pyffs/ffs.py` & `pyFFS-2.2.2/pyffs/ffs.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/pyffs/func.py` & `pyFFS-2.2.2/pyffs/func.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/pyffs/interp.py` & `pyFFS-2.2.2/pyffs/interp.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/pyffs/util.py` & `pyFFS-2.2.2/pyffs/util.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/setup.cfg` & `pyFFS-2.2.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 	numpy >= 1.10
 	scipy >= 1.5.0
 
 [options.extras_require]
 dev = 
 	sphinx == 2.1.*
 	sphinx_rtd_theme == 0.4.*
-	pytest >= 6.*
-	click >= 7.*
-	matplotlib >= 3.*
+	pytest >= 6.0
+	click >= 7.0
+	matplotlib >= 3.0
 cuda110 = cupy-cuda110 >= 8.6
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pyFFS-2.2.1/test/test_czt.py` & `pyFFS-2.2.2/test/test_czt.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/test/test_ffs.py` & `pyFFS-2.2.2/test/test_ffs.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/test/test_interp.py` & `pyFFS-2.2.2/test/test_interp.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/test/test_util.py` & `pyFFS-2.2.2/test/test_util.py`

 * *Files identical despite different names*

### Comparing `pyFFS-2.2.1/test.py` & `pyFFS-2.2.2/test.py`

 * *Files identical despite different names*

