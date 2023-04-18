# Comparing `tmp/python-linstor-1.8.0.tar.gz` & `tmp/python-linstor-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-linstor-1.8.0.tar", last modified: Tue Jun 15 14:03:36 2021, max compression
+gzip compressed data, was "python-linstor-1.9.0.tar", last modified: Wed Jul 28 07:19:04 2021, max compression
```

## Comparing `python-linstor-1.8.0.tar` & `python-linstor-1.9.0.tar`

### file list

```diff
@@ -1,53 +1,41 @@
-drwxr-xr-x   0 rp        (1000) rp        (1000)        0 2021-06-15 14:03:36.000000 python-linstor-1.8.0/
-drwxr-xr-x   0 rp        (1000) rp        (1000)        0 2021-06-15 14:03:36.000000 python-linstor-1.8.0/python_linstor.egg-info/
--rw-r--r--   0 rp        (1000) rp        (1000)        1 2021-06-15 14:03:36.000000 python-linstor-1.8.0/python_linstor.egg-info/dependency_links.txt
--rw-r--r--   0 rp        (1000) rp        (1000)       30 2021-06-15 14:03:36.000000 python-linstor-1.8.0/python_linstor.egg-info/requires.txt
--rw-r--r--   0 rp        (1000) rp        (1000)        8 2021-06-15 14:03:36.000000 python-linstor-1.8.0/python_linstor.egg-info/top_level.txt
--rw-r--r--   0 rp        (1000) rp        (1000)      984 2021-06-15 14:03:36.000000 python-linstor-1.8.0/python_linstor.egg-info/SOURCES.txt
--rw-r--r--   0 rp        (1000) rp        (1000)     2514 2021-06-15 14:03:36.000000 python-linstor-1.8.0/python_linstor.egg-info/PKG-INFO
-drwxr-xr-x   0 rp        (1000) rp        (1000)        0 2021-06-15 14:03:36.000000 python-linstor-1.8.0/linstor-common/
--rw-r--r--   0 rp        (1000) rp        (1000)    92744 2021-06-10 11:18:48.000000 python-linstor-1.8.0/linstor-common/consts.json
--rwxr-xr-x   0 rp        (1000) rp        (1000)     5841 2020-12-18 07:30:56.000000 python-linstor-1.8.0/linstor-common/gendrbdoptions.py
--rw-r--r--   0 rp        (1000) rp        (1000)     1533 2020-02-14 07:40:54.000000 python-linstor-1.8.0/linstor-common/Makefile
--rw-r--r--   0 rp        (1000) rp        (1000)    25486 2021-06-15 14:03:36.000000 python-linstor-1.8.0/linstor-common/drbdoptions.json
--rw-r--r--   0 rp        (1000) rp        (1000)    49668 2021-06-07 12:06:32.000000 python-linstor-1.8.0/linstor-common/properties.json
--rwxr-xr-x   0 rp        (1000) rp        (1000)     8300 2020-12-18 07:30:56.000000 python-linstor-1.8.0/linstor-common/genproperties.py
--rwxr-xr-x   0 rp        (1000) rp        (1000)    12391 2020-08-03 09:36:02.000000 python-linstor-1.8.0/linstor-common/genconsts.py
--rw-r--r--   0 rp        (1000) rp        (1000)     9963 2021-04-28 06:48:24.000000 python-linstor-1.8.0/linstor-common/drbdsetup.xml
-drwxr-xr-x   0 rp        (1000) rp        (1000)        0 2021-06-15 14:03:36.000000 python-linstor-1.8.0/linstor_tests/
--rw-r--r--   0 rp        (1000) rp        (1000)     1312 2019-06-07 10:19:42.000000 python-linstor-1.8.0/linstor_tests/test_responses.py
--rw-r--r--   0 rp        (1000) rp        (1000)      495 2020-01-10 08:12:05.000000 python-linstor-1.8.0/linstor_tests/__init__.py
--rw-r--r--   0 rp        (1000) rp        (1000)     1087 2019-05-17 09:11:43.000000 python-linstor-1.8.0/linstor_tests/test_utils.py
--rw-r--r--   0 rp        (1000) rp        (1000)      239 2020-09-09 13:35:54.000000 python-linstor-1.8.0/MANIFEST.in
--rw-r--r--   0 rp        (1000) rp        (1000)     2514 2021-06-15 14:03:36.000000 python-linstor-1.8.0/PKG-INFO
-drwxr-xr-x   0 rp        (1000) rp        (1000)        0 2021-06-15 14:03:36.000000 python-linstor-1.8.0/linstor/
--rw-r--r--   0 rp        (1000) rp        (1000)     1839 2019-08-06 05:19:56.000000 python-linstor-1.8.0/linstor/errors.py
--rw-r--r--   0 rp        (1000) rp        (1000)     7878 2021-04-27 07:46:28.000000 python-linstor-1.8.0/linstor/kv.py
--rw-r--r--   0 rp        (1000) rp        (1000)       18 2021-06-15 07:33:27.000000 python-linstor-1.8.0/linstor/version.py
--rw-r--r--   0 rp        (1000) rp        (1000)   136716 2021-06-14 11:56:29.000000 python-linstor-1.8.0/linstor/linstorapi.py
--rw-r--r--   0 rp        (1000) rp        (1000)       63 2020-09-23 11:24:25.000000 python-linstor-1.8.0/linstor/consts_githash.py
--rw-r--r--   0 rp        (1000) rp        (1000)    59554 2021-06-10 13:08:51.000000 python-linstor-1.8.0/linstor/responses.py
--rw-r--r--   0 rp        (1000) rp        (1000)     6242 2021-04-27 07:46:28.000000 python-linstor-1.8.0/linstor/size_calc.py
--rw-r--r--   0 rp        (1000) rp        (1000)     2057 2020-09-09 13:29:17.000000 python-linstor-1.8.0/linstor/config.py
--rw-r--r--   0 rp        (1000) rp        (1000)    10996 2021-06-14 12:01:43.000000 python-linstor-1.8.0/linstor/resourcegroup.py
--rw-r--r--   0 rp        (1000) rp        (1000)   187308 2021-06-15 14:03:36.000000 python-linstor-1.8.0/linstor/properties.py
--rw-r--r--   0 rp        (1000) rp        (1000)    43270 2021-06-15 14:03:36.000000 python-linstor-1.8.0/linstor/sharedconsts.py
--rw-r--r--   0 rp        (1000) rp        (1000)      646 2020-09-09 13:29:17.000000 python-linstor-1.8.0/linstor/__init__.py
--rw-r--r--   0 rp        (1000) rp        (1000)    32642 2021-06-14 12:00:15.000000 python-linstor-1.8.0/linstor/resource.py
--rwxr-xr-x   0 rp        (1000) rp        (1000)     4319 2021-04-27 11:32:53.000000 python-linstor-1.8.0/setup.py
--rw-r--r--   0 rp        (1000) rp        (1000)      223 2021-06-15 14:03:36.000000 python-linstor-1.8.0/setup.cfg
-drwxr-xr-x   0 rp        (1000) rp        (1000)        0 2021-06-15 14:03:36.000000 python-linstor-1.8.0/debian/
-drwxr-xr-x   0 rp        (1000) rp        (1000)        0 2021-06-15 14:03:36.000000 python-linstor-1.8.0/debian/source/
--rw-r--r--   0 rp        (1000) rp        (1000)       12 2018-06-15 09:07:07.000000 python-linstor-1.8.0/debian/source/format
--rw-r--r--   0 rp        (1000) rp        (1000)     2817 2018-06-15 09:07:07.000000 python-linstor-1.8.0/debian/copyright
-drwxr-xr-x   0 rp        (1000) rp        (1000)        0 2021-06-15 14:03:36.000000 python-linstor-1.8.0/debian/patches/
--rw-r--r--   0 rp        (1000) rp        (1000)        0 2018-06-15 09:07:07.000000 python-linstor-1.8.0/debian/patches/series
--rw-r--r--   0 rp        (1000) rp        (1000)    28771 2021-06-15 07:33:27.000000 python-linstor-1.8.0/debian/changelog
--rwxr-xr-x   0 rp        (1000) rp        (1000)      225 2020-01-10 08:12:05.000000 python-linstor-1.8.0/debian/rules
--rw-r--r--   0 rp        (1000) rp        (1000)      703 2020-01-10 08:12:05.000000 python-linstor-1.8.0/debian/control
--rw-r--r--   0 rp        (1000) rp        (1000)        2 2018-06-15 09:07:07.000000 python-linstor-1.8.0/debian/compat
--rw-r--r--   0 rp        (1000) rp        (1000)       26 2018-07-13 05:22:13.000000 python-linstor-1.8.0/debian/clean
--rw-r--r--   0 rp        (1000) rp        (1000)     2387 2021-04-28 07:08:48.000000 python-linstor-1.8.0/Makefile
--rw-r--r--   0 rp        (1000) rp        (1000)     1186 2019-05-31 05:19:06.000000 python-linstor-1.8.0/README.md
--rw-r--r--   0 rp        (1000) rp        (1000)      227 2020-03-13 06:35:09.000000 python-linstor-1.8.0/setup.cfg.py2
--rw-r--r--   0 rp        (1000) rp        (1000)     7652 2021-04-27 07:46:28.000000 python-linstor-1.8.0/COPYING
+drwxr-xr-x   0 rp        (1000) rp        (1000)        0 2021-07-28 07:19:04.784028 python-linstor-1.9.0/
+-rw-r--r--   0 rp        (1000) rp        (1000)     7652 2021-07-28 07:18:52.000000 python-linstor-1.9.0/COPYING
+-rw-r--r--   0 rp        (1000) rp        (1000)      239 2021-07-28 07:18:52.000000 python-linstor-1.9.0/MANIFEST.in
+-rw-r--r--   0 rp        (1000) rp        (1000)     2387 2021-07-28 07:18:52.000000 python-linstor-1.9.0/Makefile
+-rw-r--r--   0 rp        (1000) rp        (1000)     2341 2021-07-28 07:19:04.784028 python-linstor-1.9.0/PKG-INFO
+-rw-r--r--   0 rp        (1000) rp        (1000)     1186 2021-07-28 07:18:52.000000 python-linstor-1.9.0/README.md
+drwxr-xr-x   0 rp        (1000) rp        (1000)        0 2021-07-28 07:19:04.780694 python-linstor-1.9.0/linstor/
+-rw-r--r--   0 rp        (1000) rp        (1000)      646 2021-07-28 07:18:52.000000 python-linstor-1.9.0/linstor/__init__.py
+-rw-r--r--   0 rp        (1000) rp        (1000)     2057 2021-07-28 07:18:52.000000 python-linstor-1.9.0/linstor/config.py
+-rw-r--r--   0 rp        (1000) rp        (1000)     1839 2021-07-28 07:18:52.000000 python-linstor-1.9.0/linstor/errors.py
+-rw-r--r--   0 rp        (1000) rp        (1000)     7878 2021-07-28 07:18:52.000000 python-linstor-1.9.0/linstor/kv.py
+-rw-r--r--   0 rp        (1000) rp        (1000)   136761 2021-07-28 07:18:52.000000 python-linstor-1.9.0/linstor/linstorapi.py
+-rw-r--r--   0 rp        (1000) rp        (1000)   192371 2021-07-28 07:19:04.000000 python-linstor-1.9.0/linstor/properties.py
+-rw-r--r--   0 rp        (1000) rp        (1000)    32642 2021-07-28 07:18:52.000000 python-linstor-1.9.0/linstor/resource.py
+-rw-r--r--   0 rp        (1000) rp        (1000)    10996 2021-07-28 07:18:52.000000 python-linstor-1.9.0/linstor/resourcegroup.py
+-rw-r--r--   0 rp        (1000) rp        (1000)    59629 2021-07-28 07:18:52.000000 python-linstor-1.9.0/linstor/responses.py
+-rw-r--r--   0 rp        (1000) rp        (1000)    43737 2021-07-28 07:19:04.000000 python-linstor-1.9.0/linstor/sharedconsts.py
+-rw-r--r--   0 rp        (1000) rp        (1000)     6242 2021-07-28 07:18:52.000000 python-linstor-1.9.0/linstor/size_calc.py
+-rw-r--r--   0 rp        (1000) rp        (1000)       18 2021-07-28 07:18:52.000000 python-linstor-1.9.0/linstor/version.py
+drwxr-xr-x   0 rp        (1000) rp        (1000)        0 2021-07-28 07:19:04.784028 python-linstor-1.9.0/linstor-common/
+-rw-r--r--   0 rp        (1000) rp        (1000)     1533 2021-07-28 07:18:54.000000 python-linstor-1.9.0/linstor-common/Makefile
+-rw-r--r--   0 rp        (1000) rp        (1000)    93911 2021-07-28 07:18:54.000000 python-linstor-1.9.0/linstor-common/consts.json
+-rw-r--r--   0 rp        (1000) rp        (1000)    25486 2021-07-28 07:19:04.000000 python-linstor-1.9.0/linstor-common/drbdoptions.json
+-rw-r--r--   0 rp        (1000) rp        (1000)     9963 2021-07-28 07:18:54.000000 python-linstor-1.9.0/linstor-common/drbdsetup.xml
+-rwxr-xr-x   0 rp        (1000) rp        (1000)    12391 2021-07-28 07:18:54.000000 python-linstor-1.9.0/linstor-common/genconsts.py
+-rwxr-xr-x   0 rp        (1000) rp        (1000)     5841 2021-07-28 07:18:54.000000 python-linstor-1.9.0/linstor-common/gendrbdoptions.py
+-rwxr-xr-x   0 rp        (1000) rp        (1000)     8300 2021-07-28 07:18:54.000000 python-linstor-1.9.0/linstor-common/genproperties.py
+-rw-r--r--   0 rp        (1000) rp        (1000)    52425 2021-07-28 07:18:54.000000 python-linstor-1.9.0/linstor-common/properties.json
+drwxr-xr-x   0 rp        (1000) rp        (1000)        0 2021-07-28 07:19:04.784028 python-linstor-1.9.0/linstor_tests/
+-rw-r--r--   0 rp        (1000) rp        (1000)      495 2021-07-28 07:18:52.000000 python-linstor-1.9.0/linstor_tests/__init__.py
+-rw-r--r--   0 rp        (1000) rp        (1000)     1312 2021-07-28 07:18:52.000000 python-linstor-1.9.0/linstor_tests/test_responses.py
+-rw-r--r--   0 rp        (1000) rp        (1000)     1087 2021-07-28 07:18:52.000000 python-linstor-1.9.0/linstor_tests/test_utils.py
+drwxr-xr-x   0 rp        (1000) rp        (1000)        0 2021-07-28 07:19:04.784028 python-linstor-1.9.0/python_linstor.egg-info/
+-rw-r--r--   0 rp        (1000) rp        (1000)     2341 2021-07-28 07:19:04.000000 python-linstor-1.9.0/python_linstor.egg-info/PKG-INFO
+-rw-r--r--   0 rp        (1000) rp        (1000)      826 2021-07-28 07:19:04.000000 python-linstor-1.9.0/python_linstor.egg-info/SOURCES.txt
+-rw-r--r--   0 rp        (1000) rp        (1000)        1 2021-07-28 07:19:04.000000 python-linstor-1.9.0/python_linstor.egg-info/dependency_links.txt
+-rw-r--r--   0 rp        (1000) rp        (1000)       30 2021-07-28 07:19:04.000000 python-linstor-1.9.0/python_linstor.egg-info/requires.txt
+-rw-r--r--   0 rp        (1000) rp        (1000)        8 2021-07-28 07:19:04.000000 python-linstor-1.9.0/python_linstor.egg-info/top_level.txt
+-rw-r--r--   0 rp        (1000) rp        (1000)      223 2021-07-28 07:19:04.784028 python-linstor-1.9.0/setup.cfg
+-rw-r--r--   0 rp        (1000) rp        (1000)      227 2021-07-28 07:18:52.000000 python-linstor-1.9.0/setup.cfg.py2
+-rwxr-xr-x   0 rp        (1000) rp        (1000)     4319 2021-07-28 07:18:52.000000 python-linstor-1.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python-linstor-1.8.0/python_linstor.egg-info/SOURCES.txt` & `python-linstor-1.9.0/python_linstor.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,16 @@
 COPYING
 MANIFEST.in
 Makefile
 README.md
 setup.cfg
 setup.cfg.py2
 setup.py
-debian/changelog
-debian/clean
-debian/compat
-debian/control
-debian/copyright
-debian/rules
-debian/patches/series
-debian/source/format
 linstor/__init__.py
 linstor/config.py
-linstor/consts_githash.py
 linstor/errors.py
 linstor/kv.py
 linstor/linstorapi.py
 linstor/properties.py
 linstor/resource.py
 linstor/resourcegroup.py
 linstor/responses.py
```

### Comparing `python-linstor-1.8.0/python_linstor.egg-info/PKG-INFO` & `python-linstor-1.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 Metadata-Version: 2.1
 Name: python-linstor
-Version: 1.8.0
+Version: 1.9.0
 Summary: Linstor python api
 Home-page: https://www.linbit.com
 Author: Robert Altnoeder <robert.altnoeder@linbit.com>, Roland Kammerer <roland.kammerer@linbit.com>, Rene Peinthor <rene.peinthor@linbit.com>, Moritz Wanzenboeck <moritz.wanzenboeck@linbit.com>
 Author-email: rene.peinthor@linbit.com
 Maintainer: LINBIT HA-Solutions GmbH
 Maintainer-email: drbd-user@lists.linbit.com
 License: LGPLv3
 Project-URL: Source Code, https://github.com/LINBIT/linstor-api-py
 Project-URL: Documentation, https://linbit.github.io/linstor-api-py
-Description: # LINSTOR Python API
-        
-        This repository contains a Python library to communicate with a linstor controller.
-        
-        LINSTOR, developed by [LINBIT](https://www.linbit.com), is a software that manages DRBD replicated
-        LVM/ZFS volumes across a group of machines. It maintains DRBD configuration on the participating machines.  It
-        creates/deletes the backing LVM/ZFS volumes. It automatically places the backing LVM/ZFS volumes among the
-        participating machines.
-        
-        # Online API documentation
-        A rendered html documentation for the LINSTOR Python API can be found [here](https://linbit.github.io/linstor-api-py/).
-        
-        # Using Linstor
-        Please read the user-guide provided at [docs.linbit.com](https://docs.linbit.com).
-        
-        # Support
-        For further products and professional support, please
-        [contact](http://links.linbit.com/support) us.
-        
-        # Releases
-        Releases generated by git tags on github are snapshots of the git repository at the given time. You most
-        likely do not want to use these. They might lack things such as generated man pages, the `configure` script,
-        and other generated files. If you want to build from a tarball, use the ones [provided by us](https://www.linbit.com/en/drbd-community/drbd-download/).
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: COPYING
+
+# LINSTOR Python API
+
+This repository contains a Python library to communicate with a linstor controller.
+
+LINSTOR, developed by [LINBIT](https://www.linbit.com), is a software that manages DRBD replicated
+LVM/ZFS volumes across a group of machines. It maintains DRBD configuration on the participating machines.  It
+creates/deletes the backing LVM/ZFS volumes. It automatically places the backing LVM/ZFS volumes among the
+participating machines.
+
+# Online API documentation
+A rendered html documentation for the LINSTOR Python API can be found [here](https://linbit.github.io/linstor-api-py/).
+
+# Using Linstor
+Please read the user-guide provided at [docs.linbit.com](https://docs.linbit.com).
+
+# Support
+For further products and professional support, please
+[contact](http://links.linbit.com/support) us.
+
+# Releases
+Releases generated by git tags on github are snapshots of the git repository at the given time. You most
+likely do not want to use these. They might lack things such as generated man pages, the `configure` script,
+and other generated files. If you want to build from a tarball, use the ones [provided by us](https://www.linbit.com/en/drbd-community/drbd-download/).
+
+
```

### Comparing `python-linstor-1.8.0/linstor-common/consts.json` & `python-linstor-1.9.0/linstor-common/consts.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9892802450229708%*

 * *Differences: {'insert': "[(543, OrderedDict([('name', 'KEY_STOR_POOL_REMOTE_SPDK_API_HOST'), ('value', "*

 * *           "'RemoteSpdk/ApiHost'), ('type', 'string')])), (544, OrderedDict([('name', "*

 * *           "'KEY_STOR_POOL_REMOTE_SPDK_API_PORT'), ('value', 'RemoteSpdk/ApiPort'), ('type', "*

 * *           "'string')])), (545, OrderedDict([('name', 'KEY_STOR_POOL_REMOTE_SPDK_API_USER_NAME'), "*

 * *           "('value', 'RemoteSpdk/UserName'), ('type', 'string')])), (546, OrderedDict([('name', "*

 * *           "'KEY_STOR_POOL_REMOTE_SPDK […]*

```diff
@@ -3207,14 +3207,44 @@
     },
     {
         "name": "KEY_STOR_POOL_EXOS_POOL_SN",
         "type": "string",
         "value": "PoolSN"
     },
     {
+        "name": "KEY_STOR_POOL_REMOTE_SPDK_API_HOST",
+        "type": "string",
+        "value": "RemoteSpdk/ApiHost"
+    },
+    {
+        "name": "KEY_STOR_POOL_REMOTE_SPDK_API_PORT",
+        "type": "string",
+        "value": "RemoteSpdk/ApiPort"
+    },
+    {
+        "name": "KEY_STOR_POOL_REMOTE_SPDK_API_USER_NAME",
+        "type": "string",
+        "value": "RemoteSpdk/UserName"
+    },
+    {
+        "name": "KEY_STOR_POOL_REMOTE_SPDK_API_USER_PW",
+        "type": "string",
+        "value": "RemoteSpdk/UserPassword"
+    },
+    {
+        "name": "KEY_STOR_POOL_REMOTE_SPDK_API_USER_NAME_ENV",
+        "type": "string",
+        "value": "RemoteSpdk/UserNameEnv"
+    },
+    {
+        "name": "KEY_STOR_POOL_REMOTE_SPDK_API_USER_PW_ENV",
+        "type": "string",
+        "value": "RemoteSpdk/UserPasswordEnv"
+    },
+    {
         "name": "KEY_PREF_NIC",
         "type": "string",
         "value": "PrefNic"
     },
     {
         "blockcomment": "Storage pool traits keys"
     },
@@ -3397,14 +3427,19 @@
     },
     {
         "name": "VAL_NODE_TYPE_OPENFLEX_TARGET",
         "type": "string",
         "value": "Openflex_Target"
     },
     {
+        "name": "VAL_NODE_TYPE_REMOTE_SPDK",
+        "type": "string",
+        "value": "Remote_Spdk"
+    },
+    {
         "name": "VAL_NODE_TYPE_EXOS_TARGET",
         "type": "string",
         "value": "Exos_Target"
     },
     {
         "blockcomment": "Writecache option values"
     },
```

### Comparing `python-linstor-1.8.0/linstor-common/gendrbdoptions.py` & `python-linstor-1.9.0/linstor-common/gendrbdoptions.py`

 * *Files identical despite different names*

### Comparing `python-linstor-1.8.0/linstor-common/Makefile` & `python-linstor-1.9.0/linstor-common/Makefile`

 * *Files identical despite different names*

### Comparing `python-linstor-1.8.0/linstor-common/drbdoptions.json` & `python-linstor-1.9.0/linstor-common/drbdoptions.json`

 * *Files identical despite different names*

### Comparing `python-linstor-1.8.0/linstor-common/properties.json` & `python-linstor-1.9.0/linstor-common/properties.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9842340049656226%*

 * *Differences: {"'objects'": "{'controller': {insert: [(58, 'storage_pool_remote_spdk_api_host'), (59, "*

 * *              "'storage_pool_remote_spdk_api_port'), (60, 'storage_pool_remote_spdk_user_name'), "*

 * *              "(61, 'storage_pool_remote_spdk_user_name_env'), (62, "*

 * *              "'storage_pool_remote_spdk_user_pw'), (63, "*

 * *              "'storage_pool_remote_spdk_user_pw_env')]}, 'node': {insert: [(44, "*

 * *              "'storage_pool_remote_spdk_api_host'), (45, 'storage_pool_remote_spdk_api_port'), "*

 * *              […]*

```diff
@@ -55,14 +55,20 @@
             "stordriver_zfs_create_options",
             "storage_pool_openflex_api_host",
             "storage_pool_openflex_api_port",
             "storage_pool_openflex_user_name",
             "storage_pool_openflex_user_pw",
             "storage_pool_openflex_job_wait_delay",
             "storage_pool_openflex_job_wait_max_count",
+            "storage_pool_remote_spdk_api_host",
+            "storage_pool_remote_spdk_api_port",
+            "storage_pool_remote_spdk_user_name",
+            "storage_pool_remote_spdk_user_name_env",
+            "storage_pool_remote_spdk_user_pw",
+            "storage_pool_remote_spdk_user_pw_env",
             "storage_pool_exos_vlm_type",
             "storage_pool_exos_create_vlm_options",
             "autoplacer_strat_weights_max_freespace",
             "autoplacer_strat_weights_min_reserved_space",
             "autoplacer_strat_weights_min_rsc_count",
             "autoplacer_strat_weights_max_throughput",
             "autoplacer_pre_select_script_filename",
@@ -141,14 +147,20 @@
             "storage_pool_openflex_api_port",
             "storage_pool_openflex_user_name",
             "storage_pool_openflex_user_pw",
             "storage_pool_openflex_stor_dev",
             "storage_pool_openflex_stor_dev_host",
             "storage_pool_openflex_job_wait_delay",
             "storage_pool_openflex_job_wait_max_count",
+            "storage_pool_remote_spdk_api_host",
+            "storage_pool_remote_spdk_api_port",
+            "storage_pool_remote_spdk_user_name",
+            "storage_pool_remote_spdk_user_name_env",
+            "storage_pool_remote_spdk_user_pw",
+            "storage_pool_remote_spdk_user_pw_env",
             "storage_pool_exos_vlm_type",
             "storage_pool_exos_create_vlm_options",
             "autoplacer_max_throughput",
             "proxy_auto_enable",
             "site",
             "drbd_auto_diskful_allow_cleanup"
         ],
@@ -245,14 +257,20 @@
             "storage_pool_openflex_api_host",
             "storage_pool_openflex_api_port",
             "storage_pool_openflex_user_name",
             "storage_pool_openflex_user_pw",
             "storage_pool_openflex_stor_dev",
             "storage_pool_openflex_stor_dev_host",
             "storage_pool_openflex_stor_pool",
+            "storage_pool_remote_spdk_api_host",
+            "storage_pool_remote_spdk_api_port",
+            "storage_pool_remote_spdk_user_name",
+            "storage_pool_remote_spdk_user_name_env",
+            "storage_pool_remote_spdk_user_pw",
+            "storage_pool_remote_spdk_user_pw_env",
             "storage_pool_exos_vlm_type",
             "storage_pool_exos_create_vlm_options",
             "storage_pool_exos_enclosure",
             "storage_pool_exos_pool_sn",
             "autoplacer_max_throughput"
         ],
         "storagepool-definition": [
@@ -1192,14 +1210,68 @@
             "key": [
                 "NAMESPC_STORAGE_DRIVER",
                 "KEY_STOR_POOL_OPENFLEX_USER_PW"
             ],
             "type": "regex",
             "value": ".+"
         },
+        "storage_pool_remote_spdk_api_host": {
+            "info": "Remote SPDK API host name",
+            "key": [
+                "NAMESPC_STORAGE_DRIVER",
+                "KEY_STOR_POOL_REMOTE_SPDK_API_HOST"
+            ],
+            "type": "regex",
+            "value": ".+"
+        },
+        "storage_pool_remote_spdk_api_port": {
+            "info": "Remote SPDK API port",
+            "key": [
+                "NAMESPC_STORAGE_DRIVER",
+                "KEY_STOR_POOL_REMOTE_SPDK_API_PORT"
+            ],
+            "type": "regex",
+            "value": "[0-9]+"
+        },
+        "storage_pool_remote_spdk_user_name": {
+            "info": "Remote SPDK API user name",
+            "key": [
+                "NAMESPC_STORAGE_DRIVER",
+                "KEY_STOR_POOL_REMOTE_SPDK_API_USER_NAME"
+            ],
+            "type": "regex",
+            "value": ".+"
+        },
+        "storage_pool_remote_spdk_user_name_env": {
+            "info": "Environment variable containing remote SPDK API user name",
+            "key": [
+                "NAMESPC_STORAGE_DRIVER",
+                "KEY_STOR_POOL_REMOTE_SPDK_API_USER_NAME_ENV"
+            ],
+            "type": "regex",
+            "value": ".+"
+        },
+        "storage_pool_remote_spdk_user_pw": {
+            "info": "Remote SPDK API password",
+            "key": [
+                "NAMESPC_STORAGE_DRIVER",
+                "KEY_STOR_POOL_REMOTE_SPDK_API_USER_PW"
+            ],
+            "type": "regex",
+            "value": ".+"
+        },
+        "storage_pool_remote_spdk_user_pw_env": {
+            "info": "Environment variable containing remote SPDK API password",
+            "key": [
+                "NAMESPC_STORAGE_DRIVER",
+                "KEY_STOR_POOL_REMOTE_SPDK_API_USER_PW_ENV"
+            ],
+            "type": "regex",
+            "value": ".+"
+        },
         "stordriver_file_dir": {
             "internal": true,
             "key": [
                 "NAMESPC_STORAGE_DRIVER",
                 "KEY_STOR_POOL_FILE_DIRECTORY"
             ],
             "type": "regex",
```

### Comparing `python-linstor-1.8.0/linstor-common/genproperties.py` & `python-linstor-1.9.0/linstor-common/genproperties.py`

 * *Files identical despite different names*

### Comparing `python-linstor-1.8.0/linstor-common/genconsts.py` & `python-linstor-1.9.0/linstor-common/genconsts.py`

 * *Files identical despite different names*

### Comparing `python-linstor-1.8.0/linstor-common/drbdsetup.xml` & `python-linstor-1.9.0/linstor-common/drbdsetup.xml`

 * *Files identical despite different names*

### Comparing `python-linstor-1.8.0/linstor_tests/test_responses.py` & `python-linstor-1.9.0/linstor_tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `python-linstor-1.8.0/linstor_tests/test_utils.py` & `python-linstor-1.9.0/linstor_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-linstor-1.8.0/PKG-INFO` & `python-linstor-1.9.0/python_linstor.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 Metadata-Version: 2.1
 Name: python-linstor
-Version: 1.8.0
+Version: 1.9.0
 Summary: Linstor python api
 Home-page: https://www.linbit.com
 Author: Robert Altnoeder <robert.altnoeder@linbit.com>, Roland Kammerer <roland.kammerer@linbit.com>, Rene Peinthor <rene.peinthor@linbit.com>, Moritz Wanzenboeck <moritz.wanzenboeck@linbit.com>
 Author-email: rene.peinthor@linbit.com
 Maintainer: LINBIT HA-Solutions GmbH
 Maintainer-email: drbd-user@lists.linbit.com
 License: LGPLv3
 Project-URL: Source Code, https://github.com/LINBIT/linstor-api-py
 Project-URL: Documentation, https://linbit.github.io/linstor-api-py
-Description: # LINSTOR Python API
-        
-        This repository contains a Python library to communicate with a linstor controller.
-        
-        LINSTOR, developed by [LINBIT](https://www.linbit.com), is a software that manages DRBD replicated
-        LVM/ZFS volumes across a group of machines. It maintains DRBD configuration on the participating machines.  It
-        creates/deletes the backing LVM/ZFS volumes. It automatically places the backing LVM/ZFS volumes among the
-        participating machines.
-        
-        # Online API documentation
-        A rendered html documentation for the LINSTOR Python API can be found [here](https://linbit.github.io/linstor-api-py/).
-        
-        # Using Linstor
-        Please read the user-guide provided at [docs.linbit.com](https://docs.linbit.com).
-        
-        # Support
-        For further products and professional support, please
-        [contact](http://links.linbit.com/support) us.
-        
-        # Releases
-        Releases generated by git tags on github are snapshots of the git repository at the given time. You most
-        likely do not want to use these. They might lack things such as generated man pages, the `configure` script,
-        and other generated files. If you want to build from a tarball, use the ones [provided by us](https://www.linbit.com/en/drbd-community/drbd-download/).
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: COPYING
+
+# LINSTOR Python API
+
+This repository contains a Python library to communicate with a linstor controller.
+
+LINSTOR, developed by [LINBIT](https://www.linbit.com), is a software that manages DRBD replicated
+LVM/ZFS volumes across a group of machines. It maintains DRBD configuration on the participating machines.  It
+creates/deletes the backing LVM/ZFS volumes. It automatically places the backing LVM/ZFS volumes among the
+participating machines.
+
+# Online API documentation
+A rendered html documentation for the LINSTOR Python API can be found [here](https://linbit.github.io/linstor-api-py/).
+
+# Using Linstor
+Please read the user-guide provided at [docs.linbit.com](https://docs.linbit.com).
+
+# Support
+For further products and professional support, please
+[contact](http://links.linbit.com/support) us.
+
+# Releases
+Releases generated by git tags on github are snapshots of the git repository at the given time. You most
+likely do not want to use these. They might lack things such as generated man pages, the `configure` script,
+and other generated files. If you want to build from a tarball, use the ones [provided by us](https://www.linbit.com/en/drbd-community/drbd-download/).
+
+
```

### Comparing `python-linstor-1.8.0/linstor/errors.py` & `python-linstor-1.9.0/linstor/errors.py`

 * *Files identical despite different names*

### Comparing `python-linstor-1.8.0/linstor/kv.py` & `python-linstor-1.9.0/linstor/kv.py`

 * *Files identical despite different names*

### Comparing `python-linstor-1.8.0/linstor/linstorapi.py` & `python-linstor-1.9.0/linstor/linstorapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,16 @@
     :param bool keep_alive: Tries to keep the connection alive
     """
     _node_types = [
         apiconsts.VAL_NODE_TYPE_CTRL,
         apiconsts.VAL_NODE_TYPE_AUX,
         apiconsts.VAL_NODE_TYPE_CMBD,
         apiconsts.VAL_NODE_TYPE_STLT,
-        apiconsts.VAL_NODE_TYPE_OPENFLEX_TARGET
+        apiconsts.VAL_NODE_TYPE_OPENFLEX_TARGET,
+        apiconsts.VAL_NODE_TYPE_REMOTE_SPDK
     ]
 
     API_SINGLE_NODE_REQ = "API_SINGLE_NODE_REQ"
 
     APICALL2RESPONSE = {
         apiconsts.API_LST_NODE: NodeListResponse,
         apiconsts.API_LST_STOR_POOL: StoragePoolListResponse,
```

### Comparing `python-linstor-1.8.0/linstor/responses.py` & `python-linstor-1.9.0/linstor/responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,28 +413,30 @@
     LVMThin = "LVM_THIN"
     ZFS = "ZFS"
     ZFSThin = "ZFS_THIN"
     Diskless = "DISKLESS"
     FILE = "FILE"
     FILEThin = "FILE_THIN"
     SPDK = "SPDK"
+    REMOTE_SPDK = "REMOTE_SPDK"
     OPENFLEX_TARGET = "OPENFLEX_TARGET"
     EXOS = "EXOS"
 
     @staticmethod
     def list():
         return [
             StoragePoolDriver.LVM,
             StoragePoolDriver.LVMThin,
             StoragePoolDriver.ZFS,
             StoragePoolDriver.ZFSThin,
             StoragePoolDriver.Diskless,
             StoragePoolDriver.FILE,
             StoragePoolDriver.FILEThin,
             StoragePoolDriver.SPDK,
+            StoragePoolDriver.REMOTE_SPDK,
             StoragePoolDriver.OPENFLEX_TARGET,
             StoragePoolDriver.EXOS
         ]
 
     @classmethod
     def diskless_driver(cls):
         return [
```

### Comparing `python-linstor-1.8.0/linstor/size_calc.py` & `python-linstor-1.9.0/linstor/size_calc.py`

 * *Files identical despite different names*

### Comparing `python-linstor-1.8.0/linstor/config.py` & `python-linstor-1.9.0/linstor/config.py`

 * *Files identical despite different names*

### Comparing `python-linstor-1.8.0/linstor/resourcegroup.py` & `python-linstor-1.9.0/linstor/resourcegroup.py`

 * *Files identical despite different names*

### Comparing `python-linstor-1.8.0/linstor/properties.py` & `python-linstor-1.9.0/linstor/properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -311,14 +311,40 @@
                           'type': 'regex',
                           'value': '[0-9]+'},
                       {   'info': 'Maximum retries with wait delay until '
                                   'openflex fails',
                           'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_OPENFLEX_JOB_WAIT_MAX_COUNT,
                           'type': 'regex',
                           'value': '[0-9]+'},
+                      {   'info': 'Remote SPDK API host name',
+                          'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_REMOTE_SPDK_API_HOST,
+                          'type': 'regex',
+                          'value': '.+'},
+                      {   'info': 'Remote SPDK API port',
+                          'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_REMOTE_SPDK_API_PORT,
+                          'type': 'regex',
+                          'value': '[0-9]+'},
+                      {   'info': 'Remote SPDK API user name',
+                          'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_REMOTE_SPDK_API_USER_NAME,
+                          'type': 'regex',
+                          'value': '.+'},
+                      {   'info': 'Environment variable containing remote SPDK '
+                                  'API user name',
+                          'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_REMOTE_SPDK_API_USER_NAME_ENV,
+                          'type': 'regex',
+                          'value': '.+'},
+                      {   'info': 'Remote SPDK API password',
+                          'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_REMOTE_SPDK_API_USER_PW,
+                          'type': 'regex',
+                          'value': '.+'},
+                      {   'info': 'Environment variable containing remote SPDK '
+                                  'API password',
+                          'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_REMOTE_SPDK_API_USER_PW_ENV,
+                          'type': 'regex',
+                          'value': '.+'},
                       {   'info': 'linear: Volumes are created from Disk '
                                   'Groups (vdisks), virtual: Volumes are '
                                   'created from Pools which is a set of Disk '
                                   'Groups (vdisks)',
                           'key': consts.NAMESPC_EXOS + '/' + consts.KEY_STOR_POOL_EXOS_VLM_TYPE,
                           'type': 'symbol',
                           'values': ['linear', 'virtual']},
@@ -1288,14 +1314,40 @@
                     'type': 'regex',
                     'value': '[0-9]+'},
                 {   'info': 'Maximum retries with wait delay until openflex '
                             'fails',
                     'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_OPENFLEX_JOB_WAIT_MAX_COUNT,
                     'type': 'regex',
                     'value': '[0-9]+'},
+                {   'info': 'Remote SPDK API host name',
+                    'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_REMOTE_SPDK_API_HOST,
+                    'type': 'regex',
+                    'value': '.+'},
+                {   'info': 'Remote SPDK API port',
+                    'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_REMOTE_SPDK_API_PORT,
+                    'type': 'regex',
+                    'value': '[0-9]+'},
+                {   'info': 'Remote SPDK API user name',
+                    'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_REMOTE_SPDK_API_USER_NAME,
+                    'type': 'regex',
+                    'value': '.+'},
+                {   'info': 'Environment variable containing remote SPDK API '
+                            'user name',
+                    'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_REMOTE_SPDK_API_USER_NAME_ENV,
+                    'type': 'regex',
+                    'value': '.+'},
+                {   'info': 'Remote SPDK API password',
+                    'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_REMOTE_SPDK_API_USER_PW,
+                    'type': 'regex',
+                    'value': '.+'},
+                {   'info': 'Environment variable containing remote SPDK API '
+                            'password',
+                    'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_REMOTE_SPDK_API_USER_PW_ENV,
+                    'type': 'regex',
+                    'value': '.+'},
                 {   'info': 'linear: Volumes are created from Disk Groups '
                             '(vdisks), virtual: Volumes are created from Pools '
                             'which is a set of Disk Groups (vdisks)',
                     'key': consts.NAMESPC_EXOS + '/' + consts.KEY_STOR_POOL_EXOS_VLM_TYPE,
                     'type': 'symbol',
                     'values': ['linear', 'virtual']},
                 {   'info': 'Any additional parameters appended to '
@@ -2680,14 +2732,40 @@
                            'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_OPENFLEX_STOR_DEV_HOST,
                            'type': 'regex',
                            'value': '.+'},
                        {   'info': 'Openflex storage pool name',
                            'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_OPENFLEX_STOR_POOL,
                            'type': 'regex',
                            'value': '[0-9]+'},
+                       {   'info': 'Remote SPDK API host name',
+                           'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_REMOTE_SPDK_API_HOST,
+                           'type': 'regex',
+                           'value': '.+'},
+                       {   'info': 'Remote SPDK API port',
+                           'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_REMOTE_SPDK_API_PORT,
+                           'type': 'regex',
+                           'value': '[0-9]+'},
+                       {   'info': 'Remote SPDK API user name',
+                           'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_REMOTE_SPDK_API_USER_NAME,
+                           'type': 'regex',
+                           'value': '.+'},
+                       {   'info': 'Environment variable containing remote '
+                                   'SPDK API user name',
+                           'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_REMOTE_SPDK_API_USER_NAME_ENV,
+                           'type': 'regex',
+                           'value': '.+'},
+                       {   'info': 'Remote SPDK API password',
+                           'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_REMOTE_SPDK_API_USER_PW,
+                           'type': 'regex',
+                           'value': '.+'},
+                       {   'info': 'Environment variable containing remote '
+                                   'SPDK API password',
+                           'key': consts.NAMESPC_STORAGE_DRIVER + '/' + consts.KEY_STOR_POOL_REMOTE_SPDK_API_USER_PW_ENV,
+                           'type': 'regex',
+                           'value': '.+'},
                        {   'info': 'linear: Volumes are created from Disk '
                                    'Groups (vdisks), virtual: Volumes are '
                                    'created from Pools which is a set of Disk '
                                    'Groups (vdisks)',
                            'key': consts.NAMESPC_EXOS + '/' + consts.KEY_STOR_POOL_EXOS_VLM_TYPE,
                            'type': 'symbol',
                            'values': ['linear', 'virtual']},
```

### Comparing `python-linstor-1.8.0/linstor/sharedconsts.py` & `python-linstor-1.9.0/linstor/sharedconsts.py`

 * *Files 2% similar despite different names*

```diff
@@ -660,14 +660,20 @@
 KEY_STOR_POOL_EXOS_API_USER_ENV = str('UsernameEnv')
 KEY_STOR_POOL_EXOS_API_PASSWORD = str('Password')
 KEY_STOR_POOL_EXOS_API_PASSWORD_ENV = str('PasswordEnv')
 KEY_STOR_POOL_EXOS_VLM_TYPE = str('VolumeType')
 KEY_STOR_POOL_EXOS_CREATE_VOLUME_OPTIONS = str('CreateVolumeOptions')
 KEY_STOR_POOL_EXOS_ENCLOSURE = str('Enclosure')
 KEY_STOR_POOL_EXOS_POOL_SN = str('PoolSN')
+KEY_STOR_POOL_REMOTE_SPDK_API_HOST = str('RemoteSpdk/ApiHost')
+KEY_STOR_POOL_REMOTE_SPDK_API_PORT = str('RemoteSpdk/ApiPort')
+KEY_STOR_POOL_REMOTE_SPDK_API_USER_NAME = str('RemoteSpdk/UserName')
+KEY_STOR_POOL_REMOTE_SPDK_API_USER_PW = str('RemoteSpdk/UserPassword')
+KEY_STOR_POOL_REMOTE_SPDK_API_USER_NAME_ENV = str('RemoteSpdk/UserNameEnv')
+KEY_STOR_POOL_REMOTE_SPDK_API_USER_PW_ENV = str('RemoteSpdk/UserPasswordEnv')
 KEY_PREF_NIC = str('PrefNic')
 
 
 # ## Storage pool traits keys ###
 KEY_STOR_POOL_SUPPORTS_SNAPSHOTS = str('SupportsSnapshots')
 KEY_STOR_POOL_PROVISIONING = str('Provisioning')
 # Unit of smallest allocation. The size in KiB as a decimal number.
@@ -718,14 +724,15 @@
 
 # ## Node Type values ###
 VAL_NODE_TYPE_CTRL = str('Controller')
 VAL_NODE_TYPE_STLT = str('Satellite')
 VAL_NODE_TYPE_CMBD = str('Combined')
 VAL_NODE_TYPE_AUX = str('Auxiliary')
 VAL_NODE_TYPE_OPENFLEX_TARGET = str('Openflex_Target')
+VAL_NODE_TYPE_REMOTE_SPDK = str('Remote_Spdk')
 VAL_NODE_TYPE_EXOS_TARGET = str('Exos_Target')
 
 
 # ## Writecache option values ###
 VAL_WRITECACHE_FUA_ON = str('On')
 VAL_WRITECACHE_FUA_OFF = str('Off')
```

### Comparing `python-linstor-1.8.0/linstor/__init__.py` & `python-linstor-1.9.0/linstor/__init__.py`

 * *Files identical despite different names*

### Comparing `python-linstor-1.8.0/linstor/resource.py` & `python-linstor-1.9.0/linstor/resource.py`

 * *Files identical despite different names*

### Comparing `python-linstor-1.8.0/setup.py` & `python-linstor-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-linstor-1.8.0/Makefile` & `python-linstor-1.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `python-linstor-1.8.0/README.md` & `python-linstor-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `python-linstor-1.8.0/COPYING` & `python-linstor-1.9.0/COPYING`

 * *Files identical despite different names*

