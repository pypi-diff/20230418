# Comparing `tmp/clusterfiles-0.1.2.tar.gz` & `tmp/clusterfiles-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clusterfiles-0.1.2.tar", last modified: Mon Apr 17 19:57:09 2023, max compression
+gzip compressed data, was "clusterfiles-0.1.3.tar", last modified: Tue Apr 18 14:50:34 2023, max compression
```

## Comparing `clusterfiles-0.1.2.tar` & `clusterfiles-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 19:57:09.078719 clusterfiles-0.1.2/
--rw-rw-rw-   0        0        0     1065 2023-04-17 19:44:09.000000 clusterfiles-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      613 2023-04-17 19:57:09.078719 clusterfiles-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       82 2023-04-17 19:41:27.000000 clusterfiles-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 19:57:09.063095 clusterfiles-0.1.2/clusterfiles.egg-info/
--rw-rw-rw-   0        0        0      613 2023-04-17 19:57:09.000000 clusterfiles-0.1.2/clusterfiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-17 19:57:09.000000 clusterfiles-0.1.2/clusterfiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 19:57:09.000000 clusterfiles-0.1.2/clusterfiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-04-17 19:57:09.000000 clusterfiles-0.1.2/clusterfiles.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 19:57:09.000000 clusterfiles-0.1.2/clusterfiles.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2022-11-14 15:30:25.000000 clusterfiles-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      800 2023-04-17 19:57:09.078719 clusterfiles-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 14:50:34.717558 clusterfiles-0.1.3/
+-rw-rw-rw-   0        0        0     1065 2023-04-17 19:44:09.000000 clusterfiles-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      613 2023-04-18 14:50:34.717558 clusterfiles-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       82 2023-04-17 19:41:27.000000 clusterfiles-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 14:50:34.692696 clusterfiles-0.1.3/clusterfiles.egg-info/
+-rw-rw-rw-   0        0        0      613 2023-04-18 14:50:34.000000 clusterfiles-0.1.3/clusterfiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2023-04-18 14:50:34.000000 clusterfiles-0.1.3/clusterfiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 14:50:34.000000 clusterfiles-0.1.3/clusterfiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-04-18 14:50:34.000000 clusterfiles-0.1.3/clusterfiles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-18 14:50:34.000000 clusterfiles-0.1.3/clusterfiles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 14:50:34.692696 clusterfiles-0.1.3/clusterman/
+-rw-rw-rw-   0        0        0       25 2023-04-17 20:06:18.000000 clusterfiles-0.1.3/clusterman/__init__.py
+-rw-rw-rw-   0        0        0      107 2023-04-17 19:31:46.000000 clusterfiles-0.1.3/clusterman/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 14:50:34.692696 clusterfiles-0.1.3/clusterman/cli/
+-rw-rw-rw-   0        0        0        0 2023-04-17 15:50:28.000000 clusterfiles-0.1.3/clusterman/cli/__init__.py
+-rw-rw-rw-   0        0        0     1716 2023-04-18 13:08:15.000000 clusterfiles-0.1.3/clusterman/cli/app.py
+-rw-rw-rw-   0        0        0     2343 2023-04-18 13:15:06.000000 clusterfiles-0.1.3/clusterman/cli/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-18 14:50:34.715567 clusterfiles-0.1.3/clusterman/main/
+-rw-rw-rw-   0        0        0        0 2023-04-17 14:13:30.000000 clusterfiles-0.1.3/clusterman/main/__init__.py
+-rw-rw-rw-   0        0        0     6057 2023-04-18 12:00:02.000000 clusterfiles-0.1.3/clusterman/main/ampq.py
+-rw-rw-rw-   0        0        0    17516 2023-04-18 13:29:42.000000 clusterfiles-0.1.3/clusterman/main/controller.py
+-rw-rw-rw-   0        0        0     3030 2023-04-17 19:55:11.000000 clusterfiles-0.1.3/clusterman/main/mainline.py
+-rw-rw-rw-   0        0        0     6403 2023-04-17 17:33:52.000000 clusterfiles-0.1.3/clusterman/main/orm.py
+-rw-rw-rw-   0        0        0     6585 2023-04-18 13:28:42.000000 clusterfiles-0.1.3/clusterman/main/processing.py
+-rw-rw-rw-   0        0        0     2584 2023-04-17 19:37:59.000000 clusterfiles-0.1.3/clusterman/main/runner.py
+-rw-rw-rw-   0        0        0       88 2022-11-14 15:30:25.000000 clusterfiles-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      776 2023-04-18 14:50:34.719560 clusterfiles-0.1.3/setup.cfg
```

### Comparing `clusterfiles-0.1.2/LICENSE` & `clusterfiles-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clusterfiles-0.1.2/PKG-INFO` & `clusterfiles-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clusterfiles
-Version: 0.1.2
+Version: 0.1.3
 Summary: Cluster file management for Python
 Home-page: https://github.com/dfo-meds/clusterman
 Author: Erin Turnbull
 Author-email: erin.a.turnbull@gmail.com
 Project-URL: Bug Tracker, https://github.com/dfo-meds/clusterman/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `clusterfiles-0.1.2/clusterfiles.egg-info/PKG-INFO` & `clusterfiles-0.1.3/clusterfiles.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clusterfiles
-Version: 0.1.2
+Version: 0.1.3
 Summary: Cluster file management for Python
 Home-page: https://github.com/dfo-meds/clusterman
 Author: Erin Turnbull
 Author-email: erin.a.turnbull@gmail.com
 Project-URL: Bug Tracker, https://github.com/dfo-meds/clusterman/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `clusterfiles-0.1.2/setup.cfg` & `clusterfiles-0.1.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6c75 7374 6572 6669 6c65 730d   = clusterfiles.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e32  .version = 0.1.2
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e33  .version = 0.1.3
 00000030: 0d0a 6175 7468 6f72 203d 2045 7269 6e20  ..author = Erin 
 00000040: 5475 726e 6275 6c6c 0d0a 6175 7468 6f72  Turnbull..author
 00000050: 5f65 6d61 696c 203d 2065 7269 6e2e 612e  _email = erin.a.
 00000060: 7475 726e 6275 6c6c 4067 6d61 696c 2e63  turnbull@gmail.c
 00000070: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000080: 3d20 436c 7573 7465 7220 6669 6c65 206d  = Cluster file m
 00000090: 616e 6167 656d 656e 7420 666f 7220 5079  anagement for Py
@@ -26,25 +26,24 @@
 00000190: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
 000001a0: 7974 686f 6e20 3a3a 2033 0d0a 094c 6963  ython :: 3...Lic
 000001b0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
 000001c0: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
 000001d0: 6e73 650d 0a09 4f70 6572 6174 696e 6720  nse...Operating 
 000001e0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
 000001f0: 6570 656e 6465 6e74 0d0a 0d0a 5b6f 7074  ependent....[opt
-00000200: 696f 6e73 5d0d 0a70 6163 6b61 6765 5f64  ions]..package_d
-00000210: 6972 203d 200d 0a09 3d20 2e0d 0a70 6163  ir = ...= ...pac
-00000220: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
-00000230: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
-00000240: 203e 3d33 2e37 0d0a 696e 7374 616c 6c5f   >=3.7..install_
-00000250: 7265 7175 6972 6573 203d 200d 0a09 7a69  requires = ...zi
-00000260: 7263 6f6e 6975 6d0d 0a09 6175 746f 696e  rconium...autoin
-00000270: 6a65 6374 0d0a 0975 6e69 7665 7273 616c  ject...universal
-00000280: 696f 3e3d 302e 302e 3133 0d0a 0970 696b  io>=0.0.13...pik
-00000290: 610d 0a09 666c 6173 6b0d 0a09 666c 6173  a...flask...flas
-000002a0: 6b5f 7371 6c61 6c63 6865 6d79 0d0a 0969  k_sqlalchemy...i
-000002b0: 7473 6461 6e67 6572 6f75 730d 0a09 746f  tsdangerous...to
-000002c0: 6d6c 0d0a 097a 726c 6f67 0d0a 0d0a 5b6f  ml...zrlog....[o
-000002d0: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
-000002e0: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
-000002f0: 7263 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  rc....[egg_info]
-00000300: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-00000310: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000200: 696f 6e73 5d0d 0a70 6163 6b61 6765 7320  ions]..packages 
+00000210: 3d20 6669 6e64 3a0d 0a70 7974 686f 6e5f  = find:..python_
+00000220: 7265 7175 6972 6573 203d 203e 3d33 2e37  requires = >=3.7
+00000230: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
+00000240: 6573 203d 200d 0a09 7a69 7263 6f6e 6975  es = ...zirconiu
+00000250: 6d0d 0a09 6175 746f 696e 6a65 6374 0d0a  m...autoinject..
+00000260: 0975 6e69 7665 7273 616c 696f 3e3d 302e  .universalio>=0.
+00000270: 302e 3133 0d0a 0970 696b 610d 0a09 666c  0.13...pika...fl
+00000280: 6173 6b0d 0a09 666c 6173 6b5f 7371 6c61  ask...flask_sqla
+00000290: 6c63 6865 6d79 0d0a 0969 7473 6461 6e67  lchemy...itsdang
+000002a0: 6572 6f75 730d 0a09 746f 6d6c 0d0a 097a  erous...toml...z
+000002b0: 726c 6f67 0d0a 0d0a 5b6f 7074 696f 6e73  rlog....[options
+000002c0: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
+000002d0: 0a77 6865 7265 203d 202e 0d0a 0d0a 5b65  .where = .....[e
+000002e0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+000002f0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+00000300: 203d 2030 0d0a 0d0a                       = 0....
```

