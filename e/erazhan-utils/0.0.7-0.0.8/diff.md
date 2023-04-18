# Comparing `tmp/erazhan_utils-0.0.7.tar.gz` & `tmp/erazhan_utils-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/erazhan_utils-0.0.7.tar", last modified: Wed Jul 20 09:49:16 2022, max compression
+gzip compressed data, was "dist/erazhan_utils-0.0.8.tar", last modified: Tue Apr 18 08:03:25 2023, max compression
```

## Comparing `erazhan_utils-0.0.7.tar` & `erazhan_utils-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 zjy        (502) staff       (20)        0 2022-07-20 09:49:16.169741 erazhan_utils-0.0.7/
--rw-r--r--   0 zjy        (502) staff       (20)      312 2022-07-20 09:49:16.169368 erazhan_utils-0.0.7/PKG-INFO
--rw-r--r--   0 zjy        (502) staff       (20)     2796 2022-07-20 09:45:13.000000 erazhan_utils-0.0.7/README.md
-drwxr-xr-x   0 zjy        (502) staff       (20)        0 2022-07-20 09:49:16.166366 erazhan_utils-0.0.7/erazhan_utils/
--rw-r--r--   0 zjy        (502) staff       (20)      659 2022-07-20 09:45:13.000000 erazhan_utils-0.0.7/erazhan_utils/__init__.py
--rw-r--r--   0 zjy        (502) staff       (20)     2369 2022-07-20 09:45:13.000000 erazhan_utils-0.0.7/erazhan_utils/conn_pg.py
--rw-r--r--   0 zjy        (502) staff       (20)     1717 2022-06-07 05:26:20.000000 erazhan_utils-0.0.7/erazhan_utils/json_utils.py
--rw-r--r--   0 zjy        (502) staff       (20)     5065 2022-04-26 06:04:30.000000 erazhan_utils-0.0.7/erazhan_utils/logging_utils.py
--rw-r--r--   0 zjy        (502) staff       (20)     1189 2022-02-21 02:54:13.000000 erazhan_utils-0.0.7/erazhan_utils/os_utils.py
--rw-r--r--   0 zjy        (502) staff       (20)     1852 2022-02-23 07:19:52.000000 erazhan_utils-0.0.7/erazhan_utils/sklearn_utils.py
--rw-r--r--   0 zjy        (502) staff       (20)     2799 2022-06-28 03:23:08.000000 erazhan_utils-0.0.7/erazhan_utils/special_utils.py
--rw-r--r--   0 zjy        (502) staff       (20)     1586 2022-06-08 06:47:39.000000 erazhan_utils-0.0.7/erazhan_utils/test.py
--rw-r--r--   0 zjy        (502) staff       (20)     2362 2022-06-08 06:47:39.000000 erazhan_utils-0.0.7/erazhan_utils/time_utils.py
--rw-r--r--   0 zjy        (502) staff       (20)     3440 2022-02-23 09:44:49.000000 erazhan_utils-0.0.7/erazhan_utils/trie_tree.py
-drwxr-xr-x   0 zjy        (502) staff       (20)        0 2022-07-20 09:49:16.168848 erazhan_utils-0.0.7/erazhan_utils.egg-info/
--rw-r--r--   0 zjy        (502) staff       (20)      312 2022-07-20 09:49:15.000000 erazhan_utils-0.0.7/erazhan_utils.egg-info/PKG-INFO
--rw-r--r--   0 zjy        (502) staff       (20)      441 2022-07-20 09:49:15.000000 erazhan_utils-0.0.7/erazhan_utils.egg-info/SOURCES.txt
--rw-r--r--   0 zjy        (502) staff       (20)        1 2022-07-20 09:49:15.000000 erazhan_utils-0.0.7/erazhan_utils.egg-info/dependency_links.txt
--rw-r--r--   0 zjy        (502) staff       (20)       14 2022-07-20 09:49:15.000000 erazhan_utils-0.0.7/erazhan_utils.egg-info/top_level.txt
--rw-r--r--   0 zjy        (502) staff       (20)       38 2022-07-20 09:49:16.169869 erazhan_utils-0.0.7/setup.cfg
--rw-r--r--   0 zjy        (502) staff       (20)      874 2022-07-20 09:48:11.000000 erazhan_utils-0.0.7/setup.py
+drwxr-xr-x   0 zjy        (502) staff       (20)        0 2023-04-18 08:03:25.000000 erazhan_utils-0.0.8/
+-rw-r--r--   0 zjy        (502) staff       (20)      301 2023-04-18 08:03:25.000000 erazhan_utils-0.0.8/PKG-INFO
+drwxr-xr-x   0 zjy        (502) staff       (20)        0 2023-04-18 08:03:25.000000 erazhan_utils-0.0.8/erazhan_utils/
+-rw-r--r--   0 zjy        (502) staff       (20)     1102 2022-08-04 05:12:54.000000 erazhan_utils-0.0.8/erazhan_utils/os_utils.py
+-rw-r--r--   0 zjy        (502) staff       (20)      662 2023-04-18 07:56:27.000000 erazhan_utils-0.0.8/erazhan_utils/__init__.py
+-rw-r--r--   0 zjy        (502) staff       (20)     2362 2022-06-08 06:47:39.000000 erazhan_utils-0.0.8/erazhan_utils/time_utils.py
+-rw-r--r--   0 zjy        (502) staff       (20)     1586 2022-06-08 06:47:39.000000 erazhan_utils-0.0.8/erazhan_utils/test.py
+-rw-r--r--   0 zjy        (502) staff       (20)     2369 2022-07-20 09:45:13.000000 erazhan_utils-0.0.8/erazhan_utils/conn_pg.py
+-rw-r--r--   0 zjy        (502) staff       (20)     3440 2022-02-23 09:44:49.000000 erazhan_utils-0.0.8/erazhan_utils/trie_tree.py
+-rw-r--r--   0 zjy        (502) staff       (20)     2799 2022-09-07 02:28:34.000000 erazhan_utils-0.0.8/erazhan_utils/special_utils.py
+-rw-r--r--   0 zjy        (502) staff       (20)     1717 2022-06-07 05:26:20.000000 erazhan_utils-0.0.8/erazhan_utils/json_utils.py
+-rw-r--r--   0 zjy        (502) staff       (20)     1852 2022-02-23 07:19:52.000000 erazhan_utils-0.0.8/erazhan_utils/sklearn_utils.py
+-rw-r--r--   0 zjy        (502) staff       (20)     5153 2023-04-18 07:58:09.000000 erazhan_utils-0.0.8/erazhan_utils/logging_utils.py
+drwxr-xr-x   0 zjy        (502) staff       (20)        0 2023-04-18 08:03:25.000000 erazhan_utils-0.0.8/erazhan_utils.egg-info/
+-rw-r--r--   0 zjy        (502) staff       (20)      301 2023-04-18 08:03:25.000000 erazhan_utils-0.0.8/erazhan_utils.egg-info/PKG-INFO
+-rw-r--r--   0 zjy        (502) staff       (20)      441 2023-04-18 08:03:25.000000 erazhan_utils-0.0.8/erazhan_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 zjy        (502) staff       (20)       14 2023-04-18 08:03:25.000000 erazhan_utils-0.0.8/erazhan_utils.egg-info/top_level.txt
+-rw-r--r--   0 zjy        (502) staff       (20)        1 2023-04-18 08:03:25.000000 erazhan_utils-0.0.8/erazhan_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 zjy        (502) staff       (20)     3056 2023-04-18 08:02:25.000000 erazhan_utils-0.0.8/README.md
+-rw-r--r--   0 zjy        (502) staff       (20)      874 2023-04-18 07:55:56.000000 erazhan_utils-0.0.8/setup.py
+-rw-r--r--   0 zjy        (502) staff       (20)       38 2023-04-18 08:03:25.000000 erazhan_utils-0.0.8/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `erazhan_utils-0.0.7/README.md` & `erazhan_utils-0.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,175 +1,191 @@
 00000000: 6060 6061 6e67 756c 6172 3268 746d 6c0a  ```angular2html.
 00000010: 0a31 e380 81e5 9ca8 5079 5069 e5ae 98e7  .1......PyPi....
 00000020: bd91 e6b3 a8e5 868c e8b4 a6e5 8fb7 0a32  ...............2
 00000030: e380 81e5 889b e5bb ba70 7970 69e6 9687  .........pypi...
 00000040: e4bb b6e5 a4b9 e4bd 9ce4 b8ba e6a0 b9e7  ................
-00000050: 9bae e5bd 952c e588 9be5 bbba 746f 6f6c  .....,......tool
-00000060: 7362 7965 7261 7a68 616e e696 87e4 bbb6  sbyerazhan......
-00000070: e5a4 b9e4 bd9c e4b8 bae5 889b e5bb bae9  ................
-00000080: a1b9 e79b aee7 9a84 e590 8de7 a7b0 28e6  ..............(.
-00000090: 9c80 e590 8ee5 b0b1 e698 af70 6970 2069  ...........pip i
-000000a0: 6e73 7461 6c6c 2074 6f6f 6c73 6279 6572  nstall toolsbyer
-000000b0: 617a 6861 6e29 0a33 e380 81e5 9ca8 746f  azhan).3......to
-000000c0: 6f6c 7362 7965 7261 7a68 616e e696 87e4  olsbyerazhan....
-000000d0: bbb6 e5a4 b9e4 b8ad e588 9be5 bbba 5f5f  ..............__
-000000e0: 696e 6974 5f5f 2e70 7928 e58f afe4 bba5  init__.py(......
-000000f0: e4b8 bae7 a9ba 29e8 a1a8 e7a4 bae8 bf99  ......).........
-00000100: e698 afe4 b880 e4b8 aa70 6163 6b61 6765  .........package
-00000110: 2ce5 b9b6 e588 9be5 bbba e585 b6e5 ae83  ,...............
-00000120: e887 aae5 ae9a e4b9 89e6 9687 e4bb b62c  ...............,
-00000130: e4be 8be5 a682 7469 6d65 746f 6f6c 732e  ......timetools.
-00000140: 7079 0a34 e380 81e5 9ca8 e6a0 b9e7 9bae  py.4............
-00000150: e5bd 95e4 b88b e7bc 96e5 8699 7365 7475  ............setu
-00000160: 702e 7079 e696 87e4 bbb6 28e5 8f82 e880  p.py......(.....
-00000170: 83e7 bd91 e59d 80e6 8896 e880 85e8 87aa  ................
-00000180: e5b7 b1e4 b98b e589 8de5 819a e79a 8429  ...............)
-00000190: 0a35 e380 81e7 84b6 e590 8ee6 89a7 e8a1  .5..............
-000001a0: 8c70 7974 686f 6e20 7365 7475 702e 7079  .python setup.py
-000001b0: 2073 6469 7374 0a36 e380 81e9 878d e696   sdist.6........
-000001c0: b0e6 898b e58a a828 e4b8 8de8 a681 e5a4  .......(........
-000001d0: 8de5 88b6 2ce5 a682 e69e 9ce6 97b6 e69b  ....,...........
-000001e0: b4e6 96b0 e9a1 b9e7 9bae e588 99e4 b88d  ................
-000001f0: e794 a8e5 868d e880 83e8 9991 29e5 889b  ............)...
-00000200: e5bb ba2e 7079 7069 7263 e696 87e4 bbb6  ....pypirc......
-00000210: 28e6 9fa5 e79c 8be5 8faf e794 a87e 2f2e  (............~/.
-00000220: 7079 7069 7263 2ce5 8f82 e880 83e7 bd91  pypirc,.........
-00000230: e59d 80e6 8896 e880 85e8 87aa e5b7 b1e4  ................
-00000240: b98b e589 8de5 819a e79a 8429 0a37 e380  ...........).7..
-00000250: 81e6 9c80 e590 8ee6 89a7 e8a1 8c70 7974  .............pyt
-00000260: 686f 6e20 7365 7475 702e 7079 2073 6469  hon setup.py sdi
-00000270: 7374 2075 706c 6f61 6420 e69b b4e6 96b0  st upload ......
-00000280: e4b8 ba20 7477 696e 6520 7570 6c6f 6164  ... twine upload
-00000290: 2064 6973 742f 6572 617a 6861 6e5f 7574   dist/erazhan_ut
-000002a0: 696c 732d 302e 302e 312e 7461 722e 677a  ils-0.0.1.tar.gz
-000002b0: 28e9 809a e8bf 8770 6970 2069 6e73 7461  (......pip insta
-000002c0: 6c6c 2074 7769 6e65 e5ae 89e8 a385 7477  ll twine......tw
-000002d0: 696e 6529 0a0a e6b3 a8e6 848f 3ae5 9ca8  ine)........:...
-000002e0: 7769 6e31 30e4 b88a e693 8de4 bd9c e697  win10...........
-000002f0: b62c e8a6 81e7 94a8 e7ae a1e7 9086 e591  .,..............
-00000300: 98e5 90af e58a a863 6d64 2ce7 84b6 e590  .......cmd,.....
-00000310: 8ee8 bf9b e585 a5e5 88b0 e6a0 b9e7 9bae  ................
-00000320: e5bd 95e6 9687 e4bb b6e5 a4b9 e4b8 8b0a  ................
-00000330: 0ae5 ae98 e7bd 91e9 a1b9 e79b aee5 9cb0  ................
-00000340: e59d 800a 6874 7470 733a 2f2f 7079 7069  ....https://pypi
-00000350: 2e70 7974 686f 6e2e 6f72 672f 7369 6d70  .python.org/simp
-00000360: 6c65 2f65 7261 7a68 616e 2d75 7469 6c73  le/erazhan-utils
-00000370: 0ae9 98bf e987 8ce4 ba91 e9a1 b9e7 9bae  ................
-00000380: e59c b0e5 9d80 28e9 98bf e987 8ce4 ba91  ......(.........
-00000390: e995 9ce5 838f e4b8 80e8 88ac e8a6 81e9  ................
-000003a0: 9a94 e4b8 80e5 a4a9 e689 8de4 bc9a e69b  ................
-000003b0: b4e6 96b0 290a 6874 7470 3a2f 2f6d 6972  ....).http://mir
-000003c0: 726f 7273 2e61 6c69 7975 6e2e 636f 6d2f  rors.aliyun.com/
-000003d0: 7079 7069 2f73 696d 706c 652f 6572 617a  pypi/simple/eraz
-000003e0: 6861 6e2d 7574 696c 732f 0a0a e4bd bfe7  han-utils/......
-000003f0: 94a8 e592 8ce6 9bb4 e696 b00a 7069 7020  ............pip 
-00000400: 696e 7374 616c 6c20 6572 617a 6861 6e5f  install erazhan_
-00000410: 7574 696c 730a 7069 7020 696e 7374 616c  utils.pip instal
-00000420: 6c20 2d2d 7570 6772 6164 6520 6572 617a  l --upgrade eraz
-00000430: 6861 6e5f 7574 696c 730a 7069 7020 696e  han_utils.pip in
-00000440: 7374 616c 6c20 2d2d 5520 6572 617a 6861  stall --U erazha
-00000450: 6e5f 7574 696c 730a 0ae7 94a8 e5ae 98e7  n_utils.........
-00000460: bd91 e995 9ce5 838f 2868 7474 7020 2d3e  ........(http ->
-00000470: 2068 7474 7073 290a 7069 7020 696e 7374   https).pip inst
-00000480: 616c 6c20 2d2d 5520 6572 617a 6861 6e5f  all --U erazhan_
-00000490: 7574 696c 7320 2d69 2068 7474 7073 3a2f  utils -i https:/
-000004a0: 2f70 7970 692e 7079 7468 6f6e 2e6f 7267  /pypi.python.org
-000004b0: 2f73 696d 706c 650a 0ae5 8faa e58a a0e4  /simple.........
-000004c0: b88a 202d 6920 6874 7470 733a 2f2f 7079  .. -i https://py
-000004d0: 7069 2e70 7974 686f 6e2e 6f72 672f 7369  pi.python.org/si
-000004e0: 6d70 6c65 2023 2320 e4b8 8de9 9c80 e8a6  mple ## ........
-000004f0: 81e5 908e e99d a2e7 9a84 202d 2d74 7275  .......... --tru
-00000500: 7374 6564 2d68 6f73 7420 7079 7069 2e70  sted-host pypi.p
-00000510: 7974 686f 6e2e 6f72 670a 6874 7470 3a2f  ython.org.http:/
-00000520: 2f65 2e70 7970 692e 7079 7468 6f6e 2e6f  /e.pypi.python.o
-00000530: 7267 2f73 696d 706c 653f 0a0a e794 a8e5  rg/simple?......
-00000540: 9bbd e586 85e9 959c e583 8f0a 2d69 2068  ............-i h
-00000550: 7474 703a 2f2f 7079 7069 2e64 6f75 6261  ttp://pypi.douba
-00000560: 6e2e 636f 6d2f 7369 6d70 6c65 202d 2d74  n.com/simple --t
-00000570: 7275 7374 6564 2d68 6f73 7420 7079 7069  rusted-host pypi
-00000580: 2e64 6f75 6261 6e2e 636f 6d0a 0ae9 98bf  .douban.com.....
-00000590: e987 8ce4 ba91 e995 9ce5 838f efbc 9f0a  ................
-000005a0: 6874 7470 3a2f 2f6d 6972 726f 7273 2e61  http://mirrors.a
-000005b0: 6c69 7975 6e2e 636f 6d2f 7079 7069 2f73  liyun.com/pypi/s
-000005c0: 696d 706c 652f 0a0a e5ae 98e7 bd91 3a0a  imple/........:.
-000005d0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-000005e0: 2f0a e58f 82e8 8083 e7bd 91e5 9d80 3a0a  /.............:.
-000005f0: 6874 7470 733a 2f2f 626c 6f67 2e63 7364  https://blog.csd
-00000600: 6e2e 6e65 742f 6665 6e67 6d6d 3532 312f  n.net/fengmm521/
-00000610: 6172 7469 636c 652f 6465 7461 696c 732f  article/details/
-00000620: 3739 3134 3434 3037 0a68 7474 7073 3a2f  79144407.https:/
-00000630: 2f77 7777 2e63 6e62 6c6f 6773 2e63 6f6d  /www.cnblogs.com
-00000640: 2f42 6172 7279 626c 2f70 2f31 3230 3930  /Barrybl/p/12090
-00000650: 3533 342e 6874 6d6c 0a68 7474 7073 3a2f  534.html.https:/
-00000660: 2f77 7777 2e63 6e62 6c6f 6773 2e63 6f6d  /www.cnblogs.com
-00000670: 2f73 6d69 6c65 7965 732f 702f 3736 3537  /smileyes/p/7657
-00000680: 3539 312e 6874 6d6c 0a60 6060 0a0a 2323  591.html.```..##
-00000690: 2320 5f5f 7665 7273 696f 6e5f 5f20 3d20  # __version__ = 
-000006a0: 302e 302e 36e6 94b9 e58a a828 3230 3232  0.0.6......(2022
-000006b0: 2d30 362d 3038 290a 0a23 2323 2320 7469  -06-08)..#### ti
-000006c0: 6d65 5f75 7469 6c73 2e70 790a 0a31 2e20  me_utils.py..1. 
-000006d0: e69b b4e6 94b9 6261 636b 746f 5f4e 6461  ......backto_Nda
-000006e0: 7973 2c20 e5a2 9ee5 8aa0 e58f 82e6 95b0  ys, ............
-000006f0: 6461 7461 5f66 6f72 6d61 7428 e9bb 98e8  data_format(....
-00000700: aea4 3d27 2559 2d25 6d2d 2564 2729 0a32  ..='%Y-%m-%d').2
-00000710: 2e20 e5a2 9ee5 8aa0 6261 636b 746f 5f4e  . ......backto_N
-00000720: 746f 6461 792c 20e5 8faf e887 aae5 ae9a  today, .........
-00000730: e4b9 8964 6174 615f 666f 726d 6174 28e9  ...data_format(.
-00000740: bb98 e8ae a43d 2725 5925 6d25 6427 290a  .....='%Y%m%d').
-00000750: 332e 20e5 a29e e58a a074 7261 6e73 5f74  3. ......trans_t
-00000760: 696d 6573 7461 6d70 3273 7472 2c20 e697  imestamp2str, ..
-00000770: b6e9 97b4 e688 b3e8 bdac e5ad 97e7 aca6  ................
-00000780: e4b8 b20a 0a23 2323 2320 206a 736f 6e5f  .....####  json_
-00000790: 7574 696c 732e 7079 0a20 2020 0a31 2e20  utils.py.   .1. 
-000007a0: e69b b4e6 94b9 7361 7665 5f6a 736f 6e5f  ......save_json_
-000007b0: 6669 6c65 2c20 e5a2 9ee5 8aa0 e58f 82e6  file, ..........
-000007c0: 95b0 6d6f 6465 28e9 bb98 e8ae a43d 2769  ..mode(......='i
-000007d0: 6e64 656e 7427 292c 20e4 bf9d e5ad 98e6  ndent'), .......
-000007e0: 97b6 e698 afe5 90a6 e5b1 95e5 bc80 0a20  ............... 
-000007f0: 2020 0a23 2323 2320 6c6f 6767 696e 675f    .#### logging_
-00000800: 7574 696c 732e 7079 0a31 2e20 e69b b4e6  utils.py.1. ....
-00000810: 94b9 7570 6461 7465 5f6c 6f67 6765 722c  ..update_logger,
-00000820: 20e5 b086 e58f 82e6 95b0 e590 8d22 6170   ............"ap
-00000830: 705f 7665 7273 696f 6e22 e694 b9e4 b8ba  p_version"......
-00000840: 2261 7070 5f76 6572 7369 6f6e 5f6e 616d  "app_version_nam
-00000850: 6522 2c20 e5a2 9ee5 8aa0 e58f 82e6 95b0  e", ............
-00000860: 2275 7064 6174 655f 7479 7065 2228 e9bb  "update_type"(..
-00000870: 98e8 aea4 3d27 6461 7927 290a 0a23 2323  ....='day')..###
-00000880: 205f 5f76 6572 7369 6f6e 5f5f 203d 2030   __version__ = 0
-00000890: 2e30 2e37 e694 b9e5 8aa8 2832 3032 322d  .0.7......(2022-
-000008a0: 3037 2d32 3029 0a0a 2323 2320 5f5f 696e  07-20)..### __in
-000008b0: 6974 5f5f 2e70 790a 2d20 e5a2 9ee5 8aa0  it__.py.- ......
-000008c0: 6261 636b 746f 5f4e 746f 6461 79e5 8faf  backto_Ntoday...
-000008d0: e79b b4e6 8ea5 e5af bce5 85a5 2c20 6672  ............, fr
-000008e0: 6f6d 2065 7261 7a68 616e 5f75 7469 6c73  om erazhan_utils
-000008f0: 2069 6d70 6f72 7420 6261 636b 746f 5f4e   import backto_N
-00000900: 746f 6461 790a 2d20 7370 6563 6961 6c5f  today.- special_
-00000910: 7574 696c 732e 7079 e4b8 ade6 9687 e4bb  utils.py........
-00000920: b6e5 9d87 e79b b4e6 8ea5 e5af bce5 85a5  ................
-00000930: 0a2d 2063 6f6e 6e5f 7067 2e70 79e4 b8ad  .- conn_pg.py...
-00000940: e79b b4e6 8ea5 e5af bce5 85a5 0a0a 2323  ..............##
-00000950: 2323 2063 6f6e 6e5f 7067 2e70 790a 2d20  ## conn_pg.py.- 
-00000960: e5a2 9ee5 8aa0 e695 b0e6 8dae e5ba 93e8  ................
-00000970: afbb e58f 96ef bc8c e999 a4e5 8ebb e4ba  ................
-00000980: 86e6 9687 e4bb b6e4 b8ad e79a 84e8 b4a6  ................
-00000990: e58f b7e5 af86 e7a0 81ef bc8c e58c 85e5  ................
-000009a0: 90ab e588 9de5 a78b e58c 96e5 8f98 e987  ................
-000009b0: 8f63 6861 7273 6574 3d27 7574 6638 270a  .charset='utf8'.
-000009c0: 0a23 2323 2320 7370 6563 6961 6c5f 7574  .#### special_ut
-000009d0: 696c 732e 7079 0a0a 2d20 e5a2 9ee5 8aa0  ils.py..- ......
-000009e0: 7472 616e 735f 7369 6e67 6c65 514d 3264  trans_singleQM2d
-000009f0: 6f75 626c 6551 4d2c 20e5 b086 e696 87e6  oubleQM, .......
-00000a00: 9cac e4b8 ade7 9a84 e58d 95e5 bc95 e58f  ................
-00000a10: b7e6 9bbf e68d a2e6 8890 e58f 8ce5 bc95  ................
-00000a20: e58f b70a 2d20 e5a2 9ee5 8aa0 736f 7274  ....- ......sort
-00000a30: 5f64 6963 742c 20e5 afb9 e5ad 97e5 85b8  _dict, .........
-00000a40: e695 b0e6 8dae e8bf 9be8 a18c e68e 92e5  ................
-00000a50: ba8f 2c20 736f 7274 5f69 6e64 6578 3d30  .., sort_index=0
-00000a60: 2c31 e588 86e5 88ab e68c 896b 6579 2c76  ,1.........key,v
-00000a70: 616c 7565 e8bf 9be8 a18c e68e 92e5 ba8f  alue............
-00000a80: 0a2d 20e5 a29e e58a a06a 7564 6765 5f6e  .- ......judge_n
-00000a90: 6f74 2c20 e588 a4e6 96ad e590 a6e5 ae9a  ot, ............
-00000aa0: e79a 84e7 96be e797 852f e797 87e7 8ab6  ........./......
-00000ab0: efbc 8ce4 be8b e5a6 8222 e6b2 a1e6 9c89  ........."......
-00000ac0: e4be bfe7 a798 22e8 af86 e588 abe5 88b0  ......".........
-00000ad0: 22e4 bebf e7a7 9822 2c20 e4bd 86e5 b9b6  "......", ......
-00000ae0: e6b2 a1e6 9c89 e58f 91e7 949f            ............
+00000050: 9bae e5bd 952c e588 9be5 bbba 6572 617a  .....,......eraz
+00000060: 6861 6e5f 7574 696c 73e6 9687 e4bb b6e5  han_utils.......
+00000070: a4b9 e4bd 9ce4 b8ba e588 9be5 bbba e9a1  ................
+00000080: b9e7 9bae e79a 84e5 908d e7a7 b028 e69c  .............(..
+00000090: 80e5 908e e5b0 b1e6 98af 7069 7020 696e  ..........pip in
+000000a0: 7374 616c 6c20 6572 617a 6861 6e5f 7574  stall erazhan_ut
+000000b0: 696c 7329 0a33 e380 81e5 9ca8 6572 617a  ils).3......eraz
+000000c0: 6861 6e5f 7574 696c 73e6 9687 e4bb b6e5  han_utils.......
+000000d0: a4b9 e4b8 ade5 889b e5bb ba5f 5f69 6e69  ...........__ini
+000000e0: 745f 5f2e 7079 28e5 8faf e4bb a5e4 b8ba  t__.py(.........
+000000f0: e7a9 ba29 e8a1 a8e7 a4ba e8bf 99e6 98af  ...)............
+00000100: e4b8 80e4 b8aa 7061 636b 6167 652c e5b9  ......package,..
+00000110: b6e5 889b e5bb bae5 85b6 e5ae 83e8 87aa  ................
+00000120: e5ae 9ae4 b989 e696 87e4 bbb6 2ce4 be8b  ............,...
+00000130: e5a6 8274 696d 6574 6f6f 6c73 2e70 790a  ...timetools.py.
+00000140: 34e3 8081 e59c a8e6 a0b9 e79b aee5 bd95  4...............
+00000150: e4b8 8be7 bc96 e586 9973 6574 7570 2e70  .........setup.p
+00000160: 79e6 9687 e4bb b628 e58f 82e8 8083 e7bd  y......(........
+00000170: 91e5 9d80 e688 96e8 8085 e887 aae5 b7b1  ................
+00000180: e4b9 8be5 898d e581 9ae7 9a84 290a 35e3  ............).5.
+00000190: 8081 e784 b6e5 908e e689 a7e8 a18c 7079  ..............py
+000001a0: 7468 6f6e 2073 6574 7570 2e70 7920 7364  thon setup.py sd
+000001b0: 6973 740a 36e3 8081 e987 8de6 96b0 e689  ist.6...........
+000001c0: 8be5 8aa8 28e4 b88d e8a6 81e5 a48d e588  ....(...........
+000001d0: b62c e5a6 82e6 9e9c e697 b6e6 9bb4 e696  .,..............
+000001e0: b0e9 a1b9 e79b aee5 8899 e4b8 8de7 94a8  ................
+000001f0: e586 8de8 8083 e899 9129 e588 9be5 bbba  .........)......
+00000200: 2e70 7970 6972 63e6 9687 e4bb b628 e69f  .pypirc......(..
+00000210: a5e7 9c8b e58f afe7 94a8 7e2f 2e70 7970  ..........~/.pyp
+00000220: 6972 632c e58f 82e8 8083 e7bd 91e5 9d80  irc,............
+00000230: e688 96e8 8085 e887 aae5 b7b1 e4b9 8be5  ................
+00000240: 898d e581 9ae7 9a84 290a 37e3 8081 e69c  ........).7.....
+00000250: 80e5 908e e689 a7e8 a18c 7079 7468 6f6e  ..........python
+00000260: 2073 6574 7570 2e70 7920 7364 6973 7420   setup.py sdist 
+00000270: 7570 6c6f 6164 20e6 9bb4 e696 b0e4 b8ba  upload .........
+00000280: 2074 7769 6e65 2075 706c 6f61 6420 6469   twine upload di
+00000290: 7374 2f65 7261 7a68 616e 5f75 7469 6c73  st/erazhan_utils
+000002a0: 2d30 2e30 2e31 2e74 6172 2e67 7a28 e980  -0.0.1.tar.gz(..
+000002b0: 9ae8 bf87 7069 7020 696e 7374 616c 6c20  ....pip install 
+000002c0: 7477 696e 65e5 ae89 e8a3 8574 7769 6e65  twine......twine
+000002d0: 290a 0ae6 b3a8 e684 8f3a e59c a877 696e  )........:...win
+000002e0: 3130 e4b8 8ae6 938d e4bd 9ce6 97b6 2ce8  10............,.
+000002f0: a681 e794 a8e7 aea1 e790 86e5 9198 e590  ................
+00000300: afe5 8aa8 636d 642c e784 b6e5 908e e8bf  ....cmd,........
+00000310: 9be5 85a5 e588 b0e6 a0b9 e79b aee5 bd95  ................
+00000320: e696 87e4 bbb6 e5a4 b9e4 b88b 0a0a e5ae  ................
+00000330: 98e7 bd91 e9a1 b9e7 9bae e59c b0e5 9d80  ................
+00000340: 0a68 7474 7073 3a2f 2f70 7970 692e 7079  .https://pypi.py
+00000350: 7468 6f6e 2e6f 7267 2f73 696d 706c 652f  thon.org/simple/
+00000360: 6572 617a 6861 6e2d 7574 696c 730a e998  erazhan-utils...
+00000370: bfe9 878c e4ba 91e9 a1b9 e79b aee5 9cb0  ................
+00000380: e59d 8028 e998 bfe9 878c e4ba 91e9 959c  ...(............
+00000390: e583 8fe4 b880 e888 ace8 a681 e99a 94e4  ................
+000003a0: b880 e5a4 a9e6 898d e4bc 9ae6 9bb4 e696  ................
+000003b0: b029 0a68 7474 703a 2f2f 6d69 7272 6f72  .).http://mirror
+000003c0: 732e 616c 6979 756e 2e63 6f6d 2f70 7970  s.aliyun.com/pyp
+000003d0: 692f 7369 6d70 6c65 2f65 7261 7a68 616e  i/simple/erazhan
+000003e0: 2d75 7469 6c73 2f0a 0ae4 bdbf e794 a8e5  -utils/.........
+000003f0: 928c e69b b4e6 96b0 0a70 6970 2069 6e73  .........pip ins
+00000400: 7461 6c6c 2065 7261 7a68 616e 5f75 7469  tall erazhan_uti
+00000410: 6c73 0a70 6970 2069 6e73 7461 6c6c 202d  ls.pip install -
+00000420: 2d75 7067 7261 6465 2065 7261 7a68 616e  -upgrade erazhan
+00000430: 5f75 7469 6c73 0a70 6970 2069 6e73 7461  _utils.pip insta
+00000440: 6c6c 202d 2d55 2065 7261 7a68 616e 5f75  ll --U erazhan_u
+00000450: 7469 6c73 0a0a e794 a8e5 ae98 e7bd 91e9  tils............
+00000460: 959c e583 8f28 6874 7470 202d 3e20 6874  .....(http -> ht
+00000470: 7470 7329 0a70 6970 2069 6e73 7461 6c6c  tps).pip install
+00000480: 202d 2d55 2065 7261 7a68 616e 5f75 7469   --U erazhan_uti
+00000490: 6c73 202d 6920 6874 7470 733a 2f2f 7079  ls -i https://py
+000004a0: 7069 2e70 7974 686f 6e2e 6f72 672f 7369  pi.python.org/si
+000004b0: 6d70 6c65 0a0a e58f aae5 8aa0 e4b8 8a20  mple........... 
+000004c0: 2d69 2068 7474 7073 3a2f 2f70 7970 692e  -i https://pypi.
+000004d0: 7079 7468 6f6e 2e6f 7267 2f73 696d 706c  python.org/simpl
+000004e0: 6520 2323 20e4 b88d e99c 80e8 a681 e590  e ## ...........
+000004f0: 8ee9 9da2 e79a 8420 2d2d 7472 7573 7465  ....... --truste
+00000500: 642d 686f 7374 2070 7970 692e 7079 7468  d-host pypi.pyth
+00000510: 6f6e 2e6f 7267 0a68 7474 703a 2f2f 652e  on.org.http://e.
+00000520: 7079 7069 2e70 7974 686f 6e2e 6f72 672f  pypi.python.org/
+00000530: 7369 6d70 6c65 3f0a 0ae7 94a8 e59b bde5  simple?.........
+00000540: 8685 e995 9ce5 838f 0a2d 6920 6874 7470  .........-i http
+00000550: 3a2f 2f70 7970 692e 646f 7562 616e 2e63  ://pypi.douban.c
+00000560: 6f6d 2f73 696d 706c 6520 2d2d 7472 7573  om/simple --trus
+00000570: 7465 642d 686f 7374 2070 7970 692e 646f  ted-host pypi.do
+00000580: 7562 616e 2e63 6f6d 0a0a e998 bfe9 878c  uban.com........
+00000590: e4ba 91e9 959c e583 8fef bc9f 0a68 7474  .............htt
+000005a0: 703a 2f2f 6d69 7272 6f72 732e 616c 6979  p://mirrors.aliy
+000005b0: 756e 2e63 6f6d 2f70 7970 692f 7369 6d70  un.com/pypi/simp
+000005c0: 6c65 2f0a 0ae5 ae98 e7bd 913a 0a68 7474  le/........:.htt
+000005d0: 7073 3a2f 2f70 7970 692e 6f72 672f 0ae5  ps://pypi.org/..
+000005e0: 8f82 e880 83e7 bd91 e59d 803a 0a68 7474  ...........:.htt
+000005f0: 7073 3a2f 2f62 6c6f 672e 6373 646e 2e6e  ps://blog.csdn.n
+00000600: 6574 2f66 656e 676d 6d35 3231 2f61 7274  et/fengmm521/art
+00000610: 6963 6c65 2f64 6574 6169 6c73 2f37 3931  icle/details/791
+00000620: 3434 3430 370a 6874 7470 733a 2f2f 7777  44407.https://ww
+00000630: 772e 636e 626c 6f67 732e 636f 6d2f 4261  w.cnblogs.com/Ba
+00000640: 7272 7962 6c2f 702f 3132 3039 3035 3334  rrybl/p/12090534
+00000650: 2e68 746d 6c0a 6874 7470 733a 2f2f 7777  .html.https://ww
+00000660: 772e 636e 626c 6f67 732e 636f 6d2f 736d  w.cnblogs.com/sm
+00000670: 696c 6579 6573 2f70 2f37 3635 3735 3931  ileyes/p/7657591
+00000680: 2e68 746d 6c0a 6060 600a 0a23 2323 205f  .html.```..### _
+00000690: 5f76 6572 7369 6f6e 5f5f 203d 2030 2e30  _version__ = 0.0
+000006a0: 2e36 e694 b9e5 8aa8 2832 3032 322d 3036  .6......(2022-06
+000006b0: 2d30 3829 0a0a 2323 2323 2074 696d 655f  -08)..#### time_
+000006c0: 7574 696c 732e 7079 0a0a 312e 20e6 9bb4  utils.py..1. ...
+000006d0: e694 b962 6163 6b74 6f5f 4e64 6179 732c  ...backto_Ndays,
+000006e0: 20e5 a29e e58a a0e5 8f82 e695 b064 6174   ............dat
+000006f0: 615f 666f 726d 6174 28e9 bb98 e8ae a43d  a_format(......=
+00000700: 2725 592d 256d 2d25 6427 290a 322e 20e5  '%Y-%m-%d').2. .
+00000710: a29e e58a a062 6163 6b74 6f5f 4e74 6f64  .....backto_Ntod
+00000720: 6179 2c20 e58f afe8 87aa e5ae 9ae4 b989  ay, ............
+00000730: 6461 7461 5f66 6f72 6d61 7428 e9bb 98e8  data_format(....
+00000740: aea4 3d27 2559 256d 2564 2729 0a33 2e20  ..='%Y%m%d').3. 
+00000750: e5a2 9ee5 8aa0 7472 616e 735f 7469 6d65  ......trans_time
+00000760: 7374 616d 7032 7374 722c 20e6 97b6 e997  stamp2str, .....
+00000770: b4e6 88b3 e8bd ace5 ad97 e7ac a6e4 b8b2  ................
+00000780: 0a0a 2323 2323 2020 6a73 6f6e 5f75 7469  ..####  json_uti
+00000790: 6c73 2e70 790a 2020 200a 312e 20e6 9bb4  ls.py.   .1. ...
+000007a0: e694 b973 6176 655f 6a73 6f6e 5f66 696c  ...save_json_fil
+000007b0: 652c 20e5 a29e e58a a0e5 8f82 e695 b06d  e, ............m
+000007c0: 6f64 6528 e9bb 98e8 aea4 3d27 696e 6465  ode(......='inde
+000007d0: 6e74 2729 2c20 e4bf 9de5 ad98 e697 b6e6  nt'), ..........
+000007e0: 98af e590 a6e5 b195 e5bc 800a 2020 200a  ............   .
+000007f0: 2323 2323 206c 6f67 6769 6e67 5f75 7469  #### logging_uti
+00000800: 6c73 2e70 790a 312e 20e6 9bb4 e694 b975  ls.py.1. ......u
+00000810: 7064 6174 655f 6c6f 6767 6572 2c20 e5b0  pdate_logger, ..
+00000820: 86e5 8f82 e695 b0e5 908d 2261 7070 5f76  .........."app_v
+00000830: 6572 7369 6f6e 22e6 94b9 e4b8 ba22 6170  ersion"......"ap
+00000840: 705f 7665 7273 696f 6e5f 6e61 6d65 222c  p_version_name",
+00000850: 20e5 a29e e58a a0e5 8f82 e695 b022 7570   ............"up
+00000860: 6461 7465 5f74 7970 6522 28e9 bb98 e8ae  date_type"(.....
+00000870: a43d 2764 6179 2729 0a0a 2323 2320 5f5f  .='day')..### __
+00000880: 7665 7273 696f 6e5f 5f20 3d20 302e 302e  version__ = 0.0.
+00000890: 37e6 94b9 e58a a828 3230 3232 2d30 372d  7......(2022-07-
+000008a0: 3230 290a 0a23 2323 205f 5f69 6e69 745f  20)..### __init_
+000008b0: 5f2e 7079 0a2d 20e5 a29e e58a a062 6163  _.py.- ......bac
+000008c0: 6b74 6f5f 4e74 6f64 6179 e58f afe7 9bb4  kto_Ntoday......
+000008d0: e68e a5e5 afbc e585 a52c 2066 726f 6d20  ........., from 
+000008e0: 6572 617a 6861 6e5f 7574 696c 7320 696d  erazhan_utils im
+000008f0: 706f 7274 2062 6163 6b74 6f5f 4e74 6f64  port backto_Ntod
+00000900: 6179 0a2d 2073 7065 6369 616c 5f75 7469  ay.- special_uti
+00000910: 6c73 2e70 79e4 b8ad e696 87e4 bbb6 e59d  ls.py...........
+00000920: 87e7 9bb4 e68e a5e5 afbc e585 a50a 2d20  ..............- 
+00000930: 636f 6e6e 5f70 672e 7079 e4b8 ade7 9bb4  conn_pg.py......
+00000940: e68e a5e5 afbc e585 a50a 0a23 2323 2320  ...........#### 
+00000950: 636f 6e6e 5f70 672e 7079 0a2d 20e5 a29e  conn_pg.py.- ...
+00000960: e58a a0e6 95b0 e68d aee5 ba93 e8af bbe5  ................
+00000970: 8f96 efbc 8ce9 99a4 e58e bbe4 ba86 e696  ................
+00000980: 87e4 bbb6 e4b8 ade7 9a84 e8b4 a6e5 8fb7  ................
+00000990: e5af 86e7 a081 efbc 8ce5 8c85 e590 abe5  ................
+000009a0: 889d e5a7 8be5 8c96 e58f 98e9 878f 6368  ..............ch
+000009b0: 6172 7365 743d 2775 7466 3827 0a0a 2323  arset='utf8'..##
+000009c0: 2323 2073 7065 6369 616c 5f75 7469 6c73  ## special_utils
+000009d0: 2e70 790a 0a2d 20e5 a29e e58a a074 7261  .py..- ......tra
+000009e0: 6e73 5f73 696e 676c 6551 4d32 646f 7562  ns_singleQM2doub
+000009f0: 6c65 514d 2c20 e5b0 86e6 9687 e69c ace4  leQM, ..........
+00000a00: b8ad e79a 84e5 8d95 e5bc 95e5 8fb7 e69b  ................
+00000a10: bfe6 8da2 e688 90e5 8f8c e5bc 95e5 8fb7  ................
+00000a20: 0a2d 20e5 a29e e58a a073 6f72 745f 6469  .- ......sort_di
+00000a30: 6374 2c20 e5af b9e5 ad97 e585 b8e6 95b0  ct, ............
+00000a40: e68d aee8 bf9b e8a1 8ce6 8e92 e5ba 8f2c  ...............,
+00000a50: 2073 6f72 745f 696e 6465 783d 302c 31e5   sort_index=0,1.
+00000a60: 8886 e588 abe6 8c89 6b65 792c 7661 6c75  ........key,valu
+00000a70: 65e8 bf9b e8a1 8ce6 8e92 e5ba 8f0a 2d20  e.............- 
+00000a80: e5a2 9ee5 8aa0 6a75 6467 655f 6e6f 742c  ......judge_not,
+00000a90: 20e5 88a4 e696 ade5 90a6 e5ae 9ae7 9a84   ...............
+00000aa0: e796 bee7 9785 2fe7 9787 e78a b6ef bc8c  ....../.........
+00000ab0: e4be 8be5 a682 22e6 b2a1 e69c 89e4 bebf  ......".........
+00000ac0: e7a7 9822 e8af 86e5 88ab e588 b022 e4be  ..."........."..
+00000ad0: bfe7 a798 222c 20e4 bd86 e5b9 b6e6 b2a1  ....", .........
+00000ae0: e69c 89e5 8f91 e794 9f0a 0a23 2323 205f  ...........### _
+00000af0: 5f76 6572 7369 6f6e 5f5f 203d 2030 2e30  _version__ = 0.0
+00000b00: 2e38 e694 b9e5 8aa8 28e6 9caa e58f 91e5  .8......(.......
+00000b10: b883 290a 2d20 636f 6e6e 5f70 672e 7079  ..).- conn_pg.py
+00000b20: e4b8 ade4 b88d e694 bee5 88b0 5f5f 696e  ............__in
+00000b30: 6974 5f5f e4b8 adef bc8c e58d b3e5 afbc  it__............
+00000b40: e585 a5e6 94b9 e4b8 ba66 726f 6d20 6572  .........from er
+00000b50: 617a 6861 6e5f 7574 696c 732e 636f 6e6e  azhan_utils.conn
+00000b60: 5f70 6720 696d 706f 7274 204d 7973 716c  _pg import Mysql
+00000b70: 436f 6e6e 6563 7469 6f6e 0a2d 206c 6f67  Connection.- log
+00000b80: 6769 6e67 5f75 7469 6c73 2e70 79e4 b8ad  ging_utils.py...
+00000b90: e9a6 96e8 a18c e5a2 9ee5 8aa0 2320 636f  ............# co
+00000ba0: 6469 6e67 3a75 7466 2d38 2c20 4669 6c65  ding:utf-8, File
+00000bb0: 4c6f 6767 6572 e7b1 bbe4 b8ad 7570 6461  Logger......upda
+00000bc0: 7465 5f68 616e 646c 6572 efbc 8c63 7265  te_handler...cre
+00000bd0: 6174 655f 6c6f 6767 6572 e5a2 9ee5 8aa0  ate_logger......
+00000be0: 656e 636f 6469 6e67 3d27 7574 662d 3827  encoding='utf-8'
```

### Comparing `erazhan_utils-0.0.7/erazhan_utils/__init__.py` & `erazhan_utils-0.0.8/erazhan_utils/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # 版本更新需要保证代码兼容(原使用代码不出问题)
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 
 from . import time_utils,json_utils,logging_utils
 from . import os_utils,special_utils,sklearn_utils
 from . import trie_tree
 
 # 常用的一些函数，尽量保持不轻易变化
 from .time_utils import get_time, get_today, backto_Ndays, backto_Ntoday
 from .json_utils import read_json_file, save_json_file, read_txt_file, save_txt_file, trans2json
 from .logging_utils import create_log_file, FileLogger, write_logger, update_logger
 from .special_utils import remove_emoji,remove_quote,trans_singleQM2doubleQM,sort_dict, judge_not
-from .conn_pg import MysqlConnection
+#  from .conn_pg import MysqlConnection
```

### Comparing `erazhan_utils-0.0.7/erazhan_utils/conn_pg.py` & `erazhan_utils-0.0.8/erazhan_utils/conn_pg.py`

 * *Files identical despite different names*

### Comparing `erazhan_utils-0.0.7/erazhan_utils/json_utils.py` & `erazhan_utils-0.0.8/erazhan_utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `erazhan_utils-0.0.7/erazhan_utils/logging_utils.py` & `erazhan_utils-0.0.8/erazhan_utils/logging_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# coding:utf-8
 # -*- coding = utf-8 -*-
 # @time: 2022/2/21 11:22 上午
 # @Author: erazhan
 # @File: logging_utils.py
 
 # ----------------------------------------------------------------------------------------------------------------------
 import os
@@ -43,15 +44,15 @@
         self.update_type = update_type
 
         self.last_mday = time.localtime().tm_mday
         self.last_min = time.localtime().tm_min
         self.last_sec = time.localtime().tm_sec
 
     # 创建logger
-    def create_logger(self, log_file, logger_name = "disease", update_type = "day"):
+    def create_logger(self, log_file, logger_name = "disease", update_type = "day",encoding='utf-8'):
 
         assert update_type == self.update_type, "update_type 不一致"
         TN = time.localtime()
 
         # 后续更新时间
         if update_type == "day":
             if TN.tm_mday != self.last_mday:
@@ -85,20 +86,20 @@
 
         self.formatter.append(logging.Formatter("%(message)s"))
         self.formatter.append(logging.Formatter("[line:%(lineno)d] - %(levelname)s:\n %(message)s"))
         self.formatter.append(logging.Formatter("[line:%(lineno)d] %(asctime)s - %(levelname)s : %(message)s"))
         self.formatter.append(logging.Formatter("%(asctime)s - %(levelname)s : %(message)s"))
         self.formatter.append(logging.Formatter('%(asctime)s - %(filename)s[line:%(lineno)d] - %(levelname)s: %(message)s'))
 
-        self.fh = self.update_handler(self.formatter[4],log_file = log_file)
+        self.fh = self.update_handler(self.formatter[4],log_file = log_file,encoding=encoding)
 
     # 每天凌晨更新日志文件
-    def update_handler(self, formatter, log_file):
+    def update_handler(self, formatter, log_file, encoding='utf-8'):
 
-        new_fh = logging.FileHandler(log_file, mode='a')
+        new_fh = logging.FileHandler(log_file, mode='a',encoding = encoding)
         new_fh.setLevel(logging.INFO)
         new_fh.setFormatter(formatter)
         self.logger.addHandler(new_fh)
 
         return new_fh
 
 def write_logger(text, the_FH, info_type = "info"):
```

### Comparing `erazhan_utils-0.0.7/erazhan_utils/os_utils.py` & `erazhan_utils-0.0.8/erazhan_utils/os_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 # @Author: erazhan
 # @File: os_utils.py
 
 # ----------------------------------------------------------------------------------------------------------------------
 
 import os
 
-# 后续将本地笔记中的os.py总结完成
-# 以及调整顺序，按照名称吧
-
 def test_os__path__dirname():
     # 得到当前文件的绝对路径
     print(os.path.dirname(os.path.abspath(__file__)))
 
 
 def test_os__listdir(dir_path):
     # 得到指定文件夹下所有的文件和文件夹
```

### Comparing `erazhan_utils-0.0.7/erazhan_utils/sklearn_utils.py` & `erazhan_utils-0.0.8/erazhan_utils/sklearn_utils.py`

 * *Files identical despite different names*

### Comparing `erazhan_utils-0.0.7/erazhan_utils/special_utils.py` & `erazhan_utils-0.0.8/erazhan_utils/special_utils.py`

 * *Files identical despite different names*

### Comparing `erazhan_utils-0.0.7/erazhan_utils/test.py` & `erazhan_utils-0.0.8/erazhan_utils/test.py`

 * *Files identical despite different names*

### Comparing `erazhan_utils-0.0.7/erazhan_utils/time_utils.py` & `erazhan_utils-0.0.8/erazhan_utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `erazhan_utils-0.0.7/erazhan_utils/trie_tree.py` & `erazhan_utils-0.0.8/erazhan_utils/trie_tree.py`

 * *Files identical despite different names*

### Comparing `erazhan_utils-0.0.7/setup.py` & `erazhan_utils-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # @File: setup.py
 
 # ----------------------------------------------------------------------------------------------------------------------
 from setuptools import setup, find_packages
 
 setup(
     name = "erazhan_utils",
-    version = "0.0.7",  # 暂时在__init__.py文件中自定义__version__
+    version = "0.0.8",  # 暂时在__init__.py文件中自定义__version__
 
     keywords = ("erazhan_utils"),
     description = "some common tools in work",
     long_description = "some useful common tools",
     license = "MIT Licence",
 
     url = "https://github.com/erazhan/erazhan_utils",
```

