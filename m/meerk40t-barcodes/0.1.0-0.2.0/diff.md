# Comparing `tmp/meerk40t-barcodes-0.1.0.tar.gz` & `tmp/meerk40t-barcodes-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meerk40t-barcodes-0.1.0.tar", last modified: Wed Oct  5 19:58:04 2022, max compression
+gzip compressed data, was "meerk40t-barcodes-0.2.0.tar", last modified: Tue Apr 18 20:34:29 2023, max compression
```

## Comparing `meerk40t-barcodes-0.1.0.tar` & `meerk40t-barcodes-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-10-05 19:58:04.797558 meerk40t-barcodes-0.1.0/
--rw-rw-rw-   0        0        0     1086 2022-10-05 19:57:23.000000 meerk40t-barcodes-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3169 2022-10-05 19:58:04.797558 meerk40t-barcodes-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1842 2022-10-05 19:57:23.000000 meerk40t-barcodes-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2022-10-05 19:58:04.784557 meerk40t-barcodes-0.1.0/barcodes/
--rw-rw-rw-   0        0        0       19 2022-10-05 19:57:23.000000 meerk40t-barcodes-0.1.0/barcodes/__init__.py
--rw-rw-rw-   0        0        0    51479 2022-10-05 19:57:23.000000 meerk40t-barcodes-0.1.0/barcodes/main.py
-drwxrwxrwx   0        0        0        0 2022-10-05 19:58:04.787558 meerk40t-barcodes-0.1.0/barcodes/tools/
--rw-rw-rw-   0        0        0        0 2022-10-05 19:57:23.000000 meerk40t-barcodes-0.1.0/barcodes/tools/__init__.py
--rw-rw-rw-   0        0        0    11818 2022-10-05 19:57:23.000000 meerk40t-barcodes-0.1.0/barcodes/tools/icons.py
-drwxrwxrwx   0        0        0        0 2022-10-05 19:58:04.796558 meerk40t-barcodes-0.1.0/meerk40t_barcodes.egg-info/
--rw-rw-rw-   0        0        0     3169 2022-10-05 19:58:04.000000 meerk40t-barcodes-0.1.0/meerk40t_barcodes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2022-10-05 19:58:04.000000 meerk40t-barcodes-0.1.0/meerk40t_barcodes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-05 19:58:04.000000 meerk40t-barcodes-0.1.0/meerk40t_barcodes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2022-10-05 19:58:04.000000 meerk40t-barcodes-0.1.0/meerk40t_barcodes.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       52 2022-10-05 19:58:04.000000 meerk40t-barcodes-0.1.0/meerk40t_barcodes.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-10-05 19:58:04.000000 meerk40t-barcodes-0.1.0/meerk40t_barcodes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-10-05 19:58:04.000000 meerk40t-barcodes-0.1.0/meerk40t_barcodes.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1094 2022-10-05 19:58:04.799558 meerk40t-barcodes-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      159 2022-10-05 19:57:23.000000 meerk40t-barcodes-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:34:29.951460 meerk40t-barcodes-0.2.0/
+-rw-rw-rw-   0        0        0     1086 2022-10-05 19:57:23.000000 meerk40t-barcodes-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4038 2023-04-18 20:34:29.952460 meerk40t-barcodes-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2614 2023-04-18 20:27:08.000000 meerk40t-barcodes-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 20:34:29.931459 meerk40t-barcodes-0.2.0/barcodes/
+-rw-rw-rw-   0        0        0       28 2023-04-18 20:27:08.000000 meerk40t-barcodes-0.2.0/barcodes/__init__.py
+-rw-rw-rw-   0        0        0    24622 2023-04-18 20:27:08.000000 meerk40t-barcodes-0.2.0/barcodes/bcode_logic.py
+-rw-rw-rw-   0        0        0    27455 2023-04-18 20:27:08.000000 meerk40t-barcodes-0.2.0/barcodes/gui.py
+-rw-rw-rw-   0        0        0    16153 2023-04-18 20:27:08.000000 meerk40t-barcodes-0.2.0/barcodes/main.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:34:29.936459 meerk40t-barcodes-0.2.0/barcodes/tools/
+-rw-rw-rw-   0        0        0        0 2022-10-05 19:57:23.000000 meerk40t-barcodes-0.2.0/barcodes/tools/__init__.py
+-rw-rw-rw-   0        0        0    11818 2022-10-05 19:57:23.000000 meerk40t-barcodes-0.2.0/barcodes/tools/icons.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:34:29.951460 meerk40t-barcodes-0.2.0/meerk40t_barcodes.egg-info/
+-rw-rw-rw-   0        0        0     4038 2023-04-18 20:34:29.000000 meerk40t-barcodes-0.2.0/meerk40t_barcodes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-04-18 20:34:29.000000 meerk40t-barcodes-0.2.0/meerk40t_barcodes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 20:34:29.000000 meerk40t-barcodes-0.2.0/meerk40t_barcodes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-04-18 20:34:29.000000 meerk40t-barcodes-0.2.0/meerk40t_barcodes.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       52 2023-04-18 20:34:29.000000 meerk40t-barcodes-0.2.0/meerk40t_barcodes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-18 20:34:29.000000 meerk40t-barcodes-0.2.0/meerk40t_barcodes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-10-05 19:58:04.000000 meerk40t-barcodes-0.2.0/meerk40t_barcodes.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1103 2023-04-18 20:34:29.954460 meerk40t-barcodes-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      159 2022-10-05 19:57:23.000000 meerk40t-barcodes-0.2.0/setup.py
```

### Comparing `meerk40t-barcodes-0.1.0/LICENSE` & `meerk40t-barcodes-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meerk40t-barcodes-0.1.0/barcodes/tools/icons.py` & `meerk40t-barcodes-0.2.0/barcodes/tools/icons.py`

 * *Files identical despite different names*

### Comparing `meerk40t-barcodes-0.1.0/setup.cfg` & `meerk40t-barcodes-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6565 726b 3430 742d 6261 7263   = meerk40t-barc
 00000020: 6f64 6573 0d0a 7665 7273 696f 6e20 3d20  odes..version = 
-00000030: 302e 312e 300d 0a64 6573 6372 6970 7469  0.1.0..descripti
+00000030: 302e 322e 300d 0a64 6573 6372 6970 7469  0.2.0..descripti
 00000040: 6f6e 203d 204d 6565 724b 3430 7420 4261  on = MeerK40t Ba
 00000050: 7263 6f64 6520 4578 7465 6e73 696f 6e0d  rcode Extension.
 00000060: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
 00000070: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
 00000080: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000a0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
@@ -42,28 +42,28 @@
 00000290: 6572 2c20 7665 6374 6f72 2c20 7061 7273  er, vector, pars
 000002a0: 6572 0d0a 6175 7468 6f72 203d 206a 7069  er..author = jpi
 000002b0: 726e 6179 0d0a 6175 7468 6f72 5f65 6d61  rnay..author_ema
 000002c0: 696c 203d 2074 6174 6172 697a 6540 676d  il = tatarize@gm
 000002d0: 6169 6c2e 636f 6d0d 0a75 726c 203d 2068  ail.com..url = h
 000002e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 000002f0: 6d2f 6d65 6572 6b34 3074 2f6d 6565 726b  m/meerk40t/meerk
-00000300: 3430 740d 0a6c 6963 656e 7365 203d 204d  40t..license = M
-00000310: 4954 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  IT....[options].
-00000320: 0a7a 6970 5f73 6166 6520 3d20 5472 7565  .zip_safe = True
-00000330: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
-00000340: 655f 6461 7461 203d 2054 7275 650d 0a70  e_data = True..p
-00000350: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
-00000360: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
-00000370: 0a09 3d20 2e0d 0a74 6573 745f 7375 6974  ..= ...test_suit
-00000380: 6520 3d20 7465 7374 0d0a 0d0a 5b70 6570  e = test....[pep
-00000390: 385d 0d0a 6d61 782d 6c69 6e65 2d6c 656e  8]..max-line-len
-000003a0: 6774 6820 3d20 3130 300d 0a0d 0a5b 6264  gth = 100....[bd
-000003b0: 6973 745f 7768 6565 6c5d 0d0a 756e 6976  ist_wheel]..univ
-000003c0: 6572 7361 6c20 3d20 310d 0a0d 0a5b 6f70  ersal = 1....[op
-000003d0: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
-000003e0: 7473 5d0d 0a6d 6565 726b 3430 742e 6578  ts]..meerk40t.ex
-000003f0: 7465 6e73 696f 6e20 3d20 4578 616d 706c  tension = Exampl
-00000400: 6520 3d20 6261 7263 6f64 6573 2e6d 6169  e = barcodes.mai
-00000410: 6e3a 706c 7567 696e 0d0a 0d0a 5b65 6767  n:plugin....[egg
-00000420: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000430: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000440: 2030 0d0a 0d0a                            0....
+00000300: 3430 742d 6261 7263 6f64 6573 0d0a 6c69  40t-barcodes..li
+00000310: 6365 6e73 6520 3d20 4d49 540d 0a0d 0a5b  cense = MIT....[
+00000320: 6f70 7469 6f6e 735d 0d0a 7a69 705f 7361  options]..zip_sa
+00000330: 6665 203d 2054 7275 650d 0a69 6e63 6c75  fe = True..inclu
+00000340: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
+00000350: 3d20 5472 7565 0d0a 7061 636b 6167 6573  = True..packages
+00000360: 203d 2066 696e 643a 0d0a 7061 636b 6167   = find:..packag
+00000370: 655f 6469 7220 3d20 0d0a 093d 202e 0d0a  e_dir = ...= ...
+00000380: 7465 7374 5f73 7569 7465 203d 2074 6573  test_suite = tes
+00000390: 740d 0a0d 0a5b 7065 7038 5d0d 0a6d 6178  t....[pep8]..max
+000003a0: 2d6c 696e 652d 6c65 6e67 7468 203d 2031  -line-length = 1
+000003b0: 3030 0d0a 0d0a 5b62 6469 7374 5f77 6865  00....[bdist_whe
+000003c0: 656c 5d0d 0a75 6e69 7665 7273 616c 203d  el]..universal =
+000003d0: 2031 0d0a 0d0a 5b6f 7074 696f 6e73 2e65   1....[options.e
+000003e0: 6e74 7279 5f70 6f69 6e74 735d 0d0a 6d65  ntry_points]..me
+000003f0: 6572 6b34 3074 2e65 7874 656e 7369 6f6e  erk40t.extension
+00000400: 203d 2045 7861 6d70 6c65 203d 2062 6172   = Example = bar
+00000410: 636f 6465 732e 6d61 696e 3a70 6c75 6769  codes.main:plugi
+00000420: 6e0d 0a0d 0a5b 6567 675f 696e 666f 5d0d  n....[egg_info].
+00000430: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+00000440: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

