# Comparing `tmp/mailchimp_auto-0.1.0.tar.gz` & `tmp/mailchimp_auto-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailchimp_auto-0.1.0.tar", max compression
+gzip compressed data, was "mailchimp_auto-0.1.1.tar", max compression
```

## Comparing `mailchimp_auto-0.1.0.tar` & `mailchimp_auto-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,28 @@
--rw-r--r--   0        0        0     1109 2022-07-29 09:27:53.535053 mailchimp_auto-0.1.0/LICENSE
--rw-r--r--   0        0        0       23 2022-07-25 16:25:25.410612 mailchimp_auto-0.1.0/mailchimp_auto/__init__.py
--rw-r--r--   0        0        0       30 2022-07-28 03:19:05.663432 mailchimp_auto-0.1.0/mailchimp_auto/__main__.py
--rw-r--r--   0        0        0     2626 2022-07-29 13:25:33.766807 mailchimp_auto-0.1.0/mailchimp_auto/main.py
--rw-r--r--   0        0        0      100 2022-07-24 07:44:45.649546 mailchimp_auto-0.1.0/mailchimp_auto/scripts/__init__.py
--rw-r--r--   0        0        0      304 2022-07-28 03:50:44.565144 mailchimp_auto-0.1.0/mailchimp_auto/scripts/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      302 2022-07-28 03:50:01.545198 mailchimp_auto-0.1.0/mailchimp_auto/scripts/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2119 2022-07-29 14:52:08.622928 mailchimp_auto-0.1.0/mailchimp_auto/scripts/__pycache__/campaign_detail.cpython-310.pyc
--rw-r--r--   0        0        0     2047 2022-07-28 09:31:03.311745 mailchimp_auto-0.1.0/mailchimp_auto/scripts/__pycache__/campaign_detail.cpython-39.pyc
--rw-r--r--   0        0        0     4824 2022-07-29 04:19:53.900195 mailchimp_auto-0.1.0/mailchimp_auto/scripts/__pycache__/Config.cpython-310.pyc
--rw-r--r--   0        0        0     1040 2022-07-28 18:19:18.988003 mailchimp_auto-0.1.0/mailchimp_auto/scripts/__pycache__/create_campaign.cpython-310.pyc
--rw-r--r--   0        0        0     1272 2022-07-29 13:59:03.645127 mailchimp_auto-0.1.0/mailchimp_auto/scripts/__pycache__/directory.cpython-310.pyc
--rw-r--r--   0        0        0     1255 2022-07-28 03:50:02.233963 mailchimp_auto-0.1.0/mailchimp_auto/scripts/__pycache__/directory.cpython-39.pyc
--rw-r--r--   0        0        0     2036 2022-07-29 11:28:38.063372 mailchimp_auto-0.1.0/mailchimp_auto/scripts/__pycache__/engine.cpython-310.pyc
--rw-r--r--   0        0        0     4242 2022-07-28 18:28:04.948045 mailchimp_auto-0.1.0/mailchimp_auto/scripts/__pycache__/gspread_data.cpython-310.pyc
--rw-r--r--   0        0        0     5145 2022-07-28 09:31:03.315482 mailchimp_auto-0.1.0/mailchimp_auto/scripts/__pycache__/gspread_data.cpython-39.pyc
--rw-r--r--   0        0        0      815 2022-07-28 18:27:10.768090 mailchimp_auto-0.1.0/mailchimp_auto/scripts/__pycache__/load_newsletter_template.cpython-310.pyc
--rw-r--r--   0        0        0     1715 2022-07-29 11:28:39.309434 mailchimp_auto-0.1.0/mailchimp_auto/scripts/__pycache__/template.cpython-310.pyc
--rw-r--r--   0        0        0     7630 2022-07-29 14:52:09.936194 mailchimp_auto-0.1.0/mailchimp_auto/scripts/__pycache__/template_Config.cpython-310.pyc
--rw-r--r--   0        0        0     6794 2022-07-28 03:50:03.606464 mailchimp_auto-0.1.0/mailchimp_auto/scripts/__pycache__/template_Config.cpython-39.pyc
--rw-r--r--   0        0        0     2227 2022-07-29 14:37:40.095405 mailchimp_auto-0.1.0/mailchimp_auto/scripts/campaign_detail.py
--rw-r--r--   0        0        0     6743 2022-07-29 04:19:46.696796 mailchimp_auto-0.1.0/mailchimp_auto/scripts/Config.py
--rw-r--r--   0        0        0     1179 2022-07-28 18:17:46.083655 mailchimp_auto-0.1.0/mailchimp_auto/scripts/create_campaign.py
--rw-r--r--   0        0        0     1185 2022-07-29 13:59:00.610017 mailchimp_auto-0.1.0/mailchimp_auto/scripts/directory.py
--rw-r--r--   0        0        0     2544 2022-07-29 09:55:00.547896 mailchimp_auto-0.1.0/mailchimp_auto/scripts/engine.py
--rw-r--r--   0        0        0     4990 2022-07-28 18:27:48.400688 mailchimp_auto-0.1.0/mailchimp_auto/scripts/gspread_data.py
--rw-r--r--   0        0        0      923 2022-07-28 18:22:08.573407 mailchimp_auto-0.1.0/mailchimp_auto/scripts/load_newsletter_template.py
--rw-r--r--   0        0        0     1722 2022-07-29 09:53:01.407045 mailchimp_auto-0.1.0/mailchimp_auto/scripts/template.py
--rw-r--r--   0        0        0    10833 2022-07-29 14:39:32.838012 mailchimp_auto-0.1.0/mailchimp_auto/scripts/template_Config.py
--rw-r--r--   0        0        0      553 2022-07-29 15:45:15.902869 mailchimp_auto-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8387 2022-07-29 15:44:10.674030 mailchimp_auto-0.1.0/README.md
--rw-r--r--   0        0        0     9280 2022-07-29 15:45:20.574600 mailchimp_auto-0.1.0/setup.py
--rw-r--r--   0        0        0     8735 2022-07-29 15:45:20.574600 mailchimp_auto-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1109 2023-04-07 14:08:44.827816 mailchimp_auto-0.1.1/LICENSE
+-rw-r--r--   0        0        0       23 2023-04-07 14:08:44.889239 mailchimp_auto-0.1.1/mailchimp_auto/__init__.py
+-rw-r--r--   0        0        0       30 2023-04-07 14:08:44.889239 mailchimp_auto-0.1.1/mailchimp_auto/__main__.py
+-rw-r--r--   0        0        0     2626 2023-04-07 15:01:46.394914 mailchimp_auto-0.1.1/mailchimp_auto/main.py
+-rw-r--r--   0        0        0      100 2023-04-07 14:08:44.892240 mailchimp_auto-0.1.1/mailchimp_auto/scripts/__init__.py
+-rw-r--r--   0        0        0      299 2023-04-07 14:53:24.951465 mailchimp_auto-0.1.1/mailchimp_auto/scripts/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2119 2023-04-07 15:01:51.078310 mailchimp_auto-0.1.1/mailchimp_auto/scripts/__pycache__/campaign_detail.cpython-39.pyc
+-rw-r--r--   0        0        0     4750 2023-04-07 15:01:51.901036 mailchimp_auto-0.1.1/mailchimp_auto/scripts/__pycache__/Config.cpython-39.pyc
+-rw-r--r--   0        0        0     1878 2023-04-18 14:37:52.351598 mailchimp_auto-0.1.1/mailchimp_auto/scripts/__pycache__/create_campaign.cpython-39.pyc
+-rw-r--r--   0        0        0     1255 2023-04-07 14:53:24.955461 mailchimp_auto-0.1.1/mailchimp_auto/scripts/__pycache__/directory.cpython-39.pyc
+-rw-r--r--   0        0        0     2084 2023-04-07 14:57:22.904640 mailchimp_auto-0.1.1/mailchimp_auto/scripts/__pycache__/engine.cpython-39.pyc
+-rw-r--r--   0        0        0     4342 2023-04-07 15:01:51.081991 mailchimp_auto-0.1.1/mailchimp_auto/scripts/__pycache__/gspread_data.cpython-39.pyc
+-rw-r--r--   0        0        0     1245 2023-04-07 14:53:27.478816 mailchimp_auto-0.1.1/mailchimp_auto/scripts/__pycache__/image_processor.cpython-39.pyc
+-rw-r--r--   0        0        0     2926 2023-04-18 14:36:55.144025 mailchimp_auto-0.1.1/mailchimp_auto/scripts/__pycache__/template_action.cpython-39.pyc
+-rw-r--r--   0        0        0     7566 2023-04-07 15:01:51.905538 mailchimp_auto-0.1.1/mailchimp_auto/scripts/__pycache__/template_Config.cpython-39.pyc
+-rw-r--r--   0        0        0     2227 2023-04-07 15:01:26.130444 mailchimp_auto-0.1.1/mailchimp_auto/scripts/campaign_detail.py
+-rw-r--r--   0        0        0     6743 2023-04-07 15:01:22.120425 mailchimp_auto-0.1.1/mailchimp_auto/scripts/Config.py
+-rw-r--r--   0        0        0     2384 2023-04-18 14:37:46.437017 mailchimp_auto-0.1.1/mailchimp_auto/scripts/create_campaign.py
+-rw-r--r--   0        0        0     1185 2023-04-07 14:08:44.902246 mailchimp_auto-0.1.1/mailchimp_auto/scripts/directory.py
+-rw-r--r--   0        0        0     2673 2023-04-07 14:57:20.562773 mailchimp_auto-0.1.1/mailchimp_auto/scripts/engine.py
+-rw-r--r--   0        0        0     4495 2023-04-07 15:01:32.574080 mailchimp_auto-0.1.1/mailchimp_auto/scripts/gspread_data.py
+-rw-r--r--   0        0        0     1509 2023-04-07 14:08:44.903247 mailchimp_auto-0.1.1/mailchimp_auto/scripts/image_processor.py
+-rw-r--r--   0        0        0      923 2023-04-18 14:36:27.516614 mailchimp_auto-0.1.1/mailchimp_auto/scripts/load_newsletter_template.py
+-rw-r--r--   0        0        0     3391 2023-04-18 14:36:23.426083 mailchimp_auto-0.1.1/mailchimp_auto/scripts/template_action.py
+-rw-r--r--   0        0        0    10833 2023-04-07 15:01:38.764330 mailchimp_auto-0.1.1/mailchimp_auto/scripts/template_Config.py
+-rw-r--r--   0        0        0      572 2023-04-18 14:59:02.109975 mailchimp_auto-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10648 2023-04-07 14:08:44.828815 mailchimp_auto-0.1.1/README.md
+-rw-r--r--   0        0        0    11063 1970-01-01 00:00:00.000000 mailchimp_auto-0.1.1/PKG-INFO
```

### Comparing `mailchimp_auto-0.1.0/LICENSE` & `mailchimp_auto-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mailchimp_auto-0.1.0/mailchimp_auto/main.py` & `mailchimp_auto-0.1.1/mailchimp_auto/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     
     try:    
         engine.connect(account_username = user)
         engine.create_new_campaign(account_username = user,template_name=template, preview=preview)
         print("The task has been completed!")
     except ApiClientError as error:
         typer.echo("Error: {}".format(error.text))
-        typer.echo("Please run `python -m auto_mailchimp config` to check your mailchimp API, server prefix!")        
+        typer.echo("Please run `python -m mailchimp_auto config` to check your mailchimp API, server prefix!")        
     
 @app.command(short_help="Setup Mailchimp API, Mailchimp server prefix, Google Service account's json file, MUST SETUP this first before running this program")
 def config():
     Config.config_page()
         
 @app.command(short_help="To check your account config file, either account config file or template config file.")
 def config_file(config_file_type:str=typer.Argument(..., help="Choose either `account` or `template` to see its config file location.")):
```

### Comparing `mailchimp_auto-0.1.0/mailchimp_auto/scripts/__pycache__/campaign_detail.cpython-310.pyc` & `mailchimp_auto-0.1.1/mailchimp_auto/scripts/__pycache__/campaign_detail.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 29 14:37:40 2022 UTC, .py size: 2227 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-00000000: 6f0d 0d0a 0000 0000 b4f0 e362 b308 0000  o..........b....
+00000000: 610d 0d0a 0000 0000 4630 3064 b308 0000  a.......F00d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 5400 6503  m.Z...d.d.l.T.e.
 00000050: 8300 5a05 6505 a006 6507 a101 0100 4700  ..Z.e...e.....G.
 00000060: 6404 6405 8400 6405 8302 5a08 6406 5300  d.d...d...Z.d.S.
 00000070: 2907 e900 0000 0029 01da 0e67 6574 4773  )......)...getGs
 00000080: 7072 6561 6444 6174 6129 01da 0f52 6177  preadData)...Raw
 00000090: 436f 6e66 6967 5061 7273 6572 2901 da01  ConfigParser)...
 000000a0: 2a63 0000 0000 0000 0000 0000 0000 0000  *c..............
-000000b0: 0000 0400 0000 4000 0000 732e 0000 0065  ......@...s....e
-000000c0: 005a 0164 005a 0264 0165 0364 0265 0366  .Z.d.Z.d.e.d.e.f
-000000d0: 0464 0364 0484 045a 0464 0564 0684 005a  .d.d...Z.d.d...Z
-000000e0: 0564 0764 0884 005a 0664 0953 0029 0ada  .d.d...Z.d.S.)..
-000000f0: 0449 6e66 6fda 0e61 6363 6f75 6e74 5f63  .Info..account_c
+000000b0: 0000 0300 0000 4000 0000 732c 0000 0065  ......@...s,...e
+000000c0: 005a 0164 005a 0265 0365 0364 019c 0264  .Z.d.Z.e.e.d...d
+000000d0: 0264 0384 045a 0464 0464 0584 005a 0564  .d...Z.d.d...Z.d
+000000e0: 0664 0784 005a 0664 0853 0029 09da 0449  .d...Z.d.S.)...I
+000000f0: 6e66 6fa9 02da 0e61 6363 6f75 6e74 5f63  nfo....account_c
 00000100: 686f 6963 65da 0f74 656d 706c 6174 655f  hoice..template_
 00000110: 6368 6f69 6365 6303 0000 0000 0000 0000  choicec.........
 00000120: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
 00000130: 2200 0000 7c02 7c00 5f00 7c01 7c00 5f01  "...|.|._.|.|._.
 00000140: 7402 7c00 6a01 7c00 6a00 6401 8d02 7c00  t.|.j.|.j.d...|.
-00000150: 5f03 6400 5300 2902 4e29 0272 0600 0000  _.d.S.).N).r....
-00000160: 7207 0000 0029 0472 0700 0000 7206 0000  r....).r....r...
-00000170: 0072 0200 0000 da02 6763 2903 da04 7365  .r......gc)...se
-00000180: 6c66 7206 0000 0072 0700 0000 a900 720a  lfr....r......r.
-00000190: 0000 00fa 7243 3a5c 5573 6572 735c 7479  ....rC:\Users\ty
-000001a0: 735c 446f 6375 6d65 6e74 735c 5072 6f6a  s\Documents\Proj
-000001b0: 6563 745c 6d61 696c 6368 696d 705f 6372  ect\mailchimp_cr
-000001c0: 6561 7469 6f6e 5f70 726f 6a65 6374 5c6d  eation_project\m
-000001d0: 6169 6c63 6869 6d70 2d61 7574 6f5c 6d61  ailchimp-auto\ma
-000001e0: 696c 6368 696d 705f 6175 746f 5c73 6372  ilchimp_auto\scr
-000001f0: 6970 7473 5c63 616d 7061 6967 6e5f 6465  ipts\campaign_de
-00000200: 7461 696c 2e70 79da 085f 5f69 6e69 745f  tail.py..__init_
-00000210: 5f09 0000 0073 0600 0000 0601 0601 1601  _....s..........
-00000220: 7a0d 496e 666f 2e5f 5f69 6e69 745f 5f63  z.Info.__init__c
-00000230: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00000240: 0600 0000 4300 0000 7390 0000 0074 006a  ....C...s....t.j
-00000250: 017c 006a 0264 0164 0264 038d 037c 005f  .|.j.d.d.d...|._
-00000260: 0374 006a 017c 006a 0264 0464 0064 038d  .t.j.|.j.d.d.d..
-00000270: 037c 005f 0474 057c 006a 0483 0164 056b  .|._.t.|.j...d.k
-00000280: 0472 3564 0664 0664 0664 0664 0664 079c  .r5d.d.d.d.d.d..
-00000290: 057d 0164 0864 0984 007c 006a 04a0 0674  .}.d.d...|.j...t
-000002a0: 07a0 087c 01a1 01a1 01a0 0964 0aa1 0144  ...|.......d...D
-000002b0: 0083 017c 005f 047c 006a 0aa0 0ba1 007d  ...|._.|.j.....}
-000002c0: 027c 006a 0a6a 0c7c 006a 037c 006a 0464  .|.j.j.|.j.|.j.d
-000002d0: 0b8d 027c 005f 0d7c 006a 0d53 0029 0c4e  ...|._.|.j.S.).N
-000002e0: da1d 776f 726b 7368 6565 745f 7469 746c  ..worksheet_titl
-000002f0: 655f 6361 6d70 6169 676e 5f69 6e66 6f7a  e_campaign_infoz
-00000300: 0d43 616d 7061 6967 6e20 496e 666f a901  .Campaign Info..
-00000310: da08 6661 6c6c 6261 636b da0d 6361 6d70  ..fallback..camp
-00000320: 6169 676e 5f69 6e66 6f72 0100 0000 da00  aign_infor......
-00000330: a905 fa01 22fa 0127 fa01 20fa 015b fa01  ...."..'.. ..[..
-00000340: 5d63 0100 0000 0000 0000 0000 0000 0200  ]c..............
-00000350: 0000 0300 0000 5300 0000 f310 0000 0067  ......S........g
-00000360: 007c 005d 047d 017c 0191 0271 0253 0072  .|.].}.|...q.S.r
-00000370: 0a00 0000 720a 0000 00a9 02da 022e 30da  ....r.........0.
-00000380: 0178 720a 0000 0072 0a00 0000 720b 0000  .xr....r....r...
-00000390: 00da 0a3c 6c69 7374 636f 6d70 3e14 0000  ...<listcomp>...
-000003a0: 00f3 0200 0000 1000 7a28 496e 666f 2e67  ........z(Info.g
-000003b0: 6574 4361 6d70 6169 676e 496e 666f 2e3c  etCampaignInfo.<
-000003c0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-000003d0: 703e fa01 2c29 025a 0f77 6f72 6b73 6865  p>..,).Z.workshe
-000003e0: 6574 5f74 6974 6c65 5a14 6d75 6c74 6970  et_titleZ.multip
-000003f0: 6c65 5f63 656c 6c5f 7261 6e67 6573 290e  le_cell_ranges).
-00000400: da06 636f 6e66 6967 da03 6765 7472 0700  ..config..getr..
-00000410: 0000 720d 0000 005a 1963 616d 7061 6967  ..r....Z.campaig
-00000420: 6e5f 696e 666f 5f63 656c 6c5f 7261 6e67  n_info_cell_rang
-00000430: 6573 da03 6c65 6eda 0974 7261 6e73 6c61  es..len..transla
-00000440: 7465 da03 7374 72da 096d 616b 6574 7261  te..str..maketra
-00000450: 6e73 da05 7370 6c69 7472 0800 0000 5a12  ns..splitr....Z.
-00000460: 6163 6365 7373 5f73 7072 6561 6473 6865  access_spreadshe
-00000470: 6574 5a11 6765 745f 6361 6d70 6169 676e  etZ.get_campaign
-00000480: 5f69 6e66 6f72 1000 0000 2903 7209 0000  _infor....).r...
-00000490: 00da 0f63 6861 725f 746f 5f72 6570 6c61  ...char_to_repla
-000004a0: 6365 5a12 576f 726b 7368 6565 745f 7365  ceZ.Worksheet_se
-000004b0: 6c65 6374 6564 720a 0000 0072 0a00 0000  lectedr....r....
-000004c0: 720b 0000 00da 0f67 6574 4361 6d70 6169  r......getCampai
-000004d0: 676e 496e 666f 0e00 0000 7310 0000 0014  gnInfo....s.....
-000004e0: 0114 010e 0210 0124 010a 0216 0106 017a  .......$.......z
-000004f0: 1449 6e66 6f2e 6765 7443 616d 7061 6967  .Info.getCampaig
-00000500: 6e49 6e66 6f63 0100 0000 0000 0000 0000  nInfoc..........
-00000510: 0000 0200 0000 0600 0000 4300 0000 737a  ..........C...sz
-00000520: 0000 0074 006a 017c 006a 0264 0164 0264  ...t.j.|.j.d.d.d
-00000530: 038d 037c 005f 0374 006a 017c 006a 0264  ...|._.t.j.|.j.d
-00000540: 0464 0064 038d 037c 005f 0464 0564 0564  .d.d...|._.d.d.d
-00000550: 0564 0564 0564 069c 057d 0164 0764 0884  .d.d.d...}.d.d..
-00000560: 0074 057c 006a 0483 01a0 0674 05a0 077c  .t.|.j.....t...|
-00000570: 01a1 01a1 01a0 0864 09a1 0144 0083 017c  .......d...D...|
-00000580: 005f 047c 006a 09a0 0a7c 006a 037c 006a  ._.|.j...|.j.|.j
-00000590: 04a1 027c 005f 0b7c 006a 0b53 0029 0a4e  ...|._.|.j.S.).N
-000005a0: da20 776f 726b 7368 6565 745f 7469 746c  . worksheet_titl
-000005b0: 655f 6361 6d70 6169 676e 5f63 6f6e 7465  e_campaign_conte
-000005c0: 6e74 7a10 4361 6d70 6169 676e 2043 6f6e  ntz.Campaign Con
-000005d0: 7465 6e74 720e 0000 005a 1063 616d 7061  tentr....Z.campa
-000005e0: 6967 6e5f 636f 6e74 656e 7472 1100 0000  ign_contentr....
-000005f0: 7212 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00000600: 0000 0200 0000 0300 0000 5300 0000 7218  ..........S...r.
-00000610: 0000 0072 0a00 0000 720a 0000 0072 1900  ...r....r....r..
-00000620: 0000 720a 0000 0072 0a00 0000 720b 0000  ..r....r....r...
-00000630: 0072 1c00 0000 2100 0000 721d 0000 007a  .r....!...r....z
-00000640: 2749 6e66 6f2e 6765 7468 746d 6c43 6f6e  'Info.gethtmlCon
-00000650: 7465 6e74 2e3c 6c6f 6361 6c73 3e2e 3c6c  tent.<locals>.<l
-00000660: 6973 7463 6f6d 703e 721e 0000 0029 0c72  istcomp>r....).r
-00000670: 1f00 0000 7220 0000 0072 0700 0000 7228  ....r ...r....r(
-00000680: 0000 005a 1c63 616d 7061 6967 6e5f 636f  ...Z.campaign_co
-00000690: 6e74 656e 745f 6365 6c6c 5f72 616e 6765  ntent_cell_range
-000006a0: 7372 2300 0000 7222 0000 0072 2400 0000  sr#...r"...r$...
-000006b0: 7225 0000 0072 0800 0000 5a10 6765 745f  r%...r....Z.get_
-000006c0: 636f 6e74 656e 745f 696e 666f da04 6461  content_info..da
-000006d0: 7461 2902 7209 0000 0072 2600 0000 720a  ta).r....r&...r.
-000006e0: 0000 0072 0a00 0000 720b 0000 00da 0e67  ...r....r......g
-000006f0: 6574 6874 6d6c 436f 6e74 656e 741a 0000  ethtmlContent...
-00000700: 0073 0c00 0000 1403 1401 1002 2801 1402  .s..........(...
-00000710: 0601 7a13 496e 666f 2e67 6574 6874 6d6c  ..z.Info.gethtml
-00000720: 436f 6e74 656e 744e 2907 da08 5f5f 6e61  ContentN)...__na
-00000730: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000740: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7223  ..__qualname__r#
-00000750: 0000 0072 0c00 0000 7227 0000 0072 2a00  ...r....r'...r*.
-00000760: 0000 720a 0000 0072 0a00 0000 720a 0000  ..r....r....r...
-00000770: 0072 0b00 0000 7205 0000 0008 0000 0073  .r....r........s
-00000780: 0800 0000 0800 1201 0805 0c0c 7205 0000  ............r...
-00000790: 004e 2909 5a23 6d61 696c 6368 696d 705f  .N).Z#mailchimp_
-000007a0: 6175 746f 2e73 6372 6970 7473 2e67 7370  auto.scripts.gsp
-000007b0: 7265 6164 5f64 6174 6172 0200 0000 da0c  read_datar......
-000007c0: 636f 6e66 6967 7061 7273 6572 7203 0000  configparserr...
-000007d0: 005a 206d 6169 6c63 6869 6d70 5f61 7574  .Z mailchimp_aut
-000007e0: 6f2e 7363 7269 7074 732e 6469 7265 6374  o.scripts.direct
-000007f0: 6f72 7972 1f00 0000 da04 7265 6164 da0f  oryr......read..
-00000800: 7465 6d70 6c61 7465 5f63 6f6e 6669 6772  template_configr
-00000810: 0500 0000 720a 0000 0072 0a00 0000 720a  ....r....r....r.
-00000820: 0000 0072 0b00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000830: 653e 0100 0000 730c 0000 000c 000c 0108  e>....s.........
-00000840: 0106 020a 0112 02                        .......
+00000150: 5f03 6400 5300 2902 4e72 0600 0000 2904  _.d.S.).Nr....).
+00000160: 7208 0000 0072 0700 0000 7202 0000 00da  r....r....r.....
+00000170: 0267 6329 03da 0473 656c 6672 0700 0000  .gc)...selfr....
+00000180: 7208 0000 00a9 0072 0b00 0000 fa6f 433a  r......r.....oC:
+00000190: 5c55 7365 7273 5c79 6f6e 6773 6865 6e67  \Users\yongsheng
+000001a0: 2e74 616e 5c44 6f63 756d 656e 7473 5c43  .tan\Documents\C
+000001b0: 6f64 696e 675c 6769 7468 7562 2d70 726f  oding\github-pro
+000001c0: 6a65 6374 5c6d 6169 6c63 6869 6d70 5f61  ject\mailchimp_a
+000001d0: 7574 6f5c 6d61 696c 6368 696d 705f 6175  uto\mailchimp_au
+000001e0: 746f 5c73 6372 6970 7473 5c63 616d 7061  to\scripts\campa
+000001f0: 6967 6e5f 6465 7461 696c 2e70 79da 085f  ign_detail.py.._
+00000200: 5f69 6e69 745f 5f09 0000 0073 0600 0000  _init__....s....
+00000210: 0001 0601 0601 7a0d 496e 666f 2e5f 5f69  ......z.Info.__i
+00000220: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
+00000230: 0000 0300 0000 0600 0000 4300 0000 7390  ..........C...s.
+00000240: 0000 0074 006a 017c 006a 0264 0164 0264  ...t.j.|.j.d.d.d
+00000250: 038d 037c 005f 0374 006a 017c 006a 0264  ...|._.t.j.|.j.d
+00000260: 0464 0064 038d 037c 005f 0474 057c 006a  .d.d...|._.t.|.j
+00000270: 0483 0164 056b 0472 6a64 0664 0664 0664  ...d.k.rjd.d.d.d
+00000280: 0664 0664 079c 057d 0164 0864 0984 007c  .d.d...}.d.d...|
+00000290: 006a 04a0 0674 07a0 087c 01a1 01a1 01a0  .j...t...|......
+000002a0: 0964 0aa1 0144 0083 017c 005f 047c 006a  .d...D...|._.|.j
+000002b0: 0aa0 0ba1 007d 027c 006a 0a6a 0c7c 006a  .....}.|.j.j.|.j
+000002c0: 037c 006a 0464 0b8d 027c 005f 0d7c 006a  .|.j.d...|._.|.j
+000002d0: 0d53 0029 0c4e da1d 776f 726b 7368 6565  .S.).N..workshee
+000002e0: 745f 7469 746c 655f 6361 6d70 6169 676e  t_title_campaign
+000002f0: 5f69 6e66 6f7a 0d43 616d 7061 6967 6e20  _infoz.Campaign 
+00000300: 496e 666f a901 da08 6661 6c6c 6261 636b  Info....fallback
+00000310: da0d 6361 6d70 6169 676e 5f69 6e66 6f72  ..campaign_infor
+00000320: 0100 0000 da00 a905 fa01 22fa 0127 fa01  .........."..'..
+00000330: 20fa 015b fa01 5d63 0100 0000 0000 0000   ..[..]c........
+00000340: 0000 0000 0200 0000 0300 0000 5300 0000  ............S...
+00000350: 7310 0000 0067 007c 005d 087d 017c 0191  s....g.|.].}.|..
+00000360: 0271 0453 0072 0b00 0000 720b 0000 00a9  .q.S.r....r.....
+00000370: 02da 022e 30da 0178 720b 0000 0072 0b00  ....0..xr....r..
+00000380: 0000 720c 0000 00da 0a3c 6c69 7374 636f  ..r......<listco
+00000390: 6d70 3e14 0000 00f3 0000 0000 7a28 496e  mp>.........z(In
+000003a0: 666f 2e67 6574 4361 6d70 6169 676e 496e  fo.getCampaignIn
+000003b0: 666f 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  fo.<locals>.<lis
+000003c0: 7463 6f6d 703e fa01 2c29 025a 0f77 6f72  tcomp>..,).Z.wor
+000003d0: 6b73 6865 6574 5f74 6974 6c65 5a14 6d75  ksheet_titleZ.mu
+000003e0: 6c74 6970 6c65 5f63 656c 6c5f 7261 6e67  ltiple_cell_rang
+000003f0: 6573 290e da06 636f 6e66 6967 da03 6765  es)...config..ge
+00000400: 7472 0800 0000 720e 0000 005a 1963 616d  tr....r....Z.cam
+00000410: 7061 6967 6e5f 696e 666f 5f63 656c 6c5f  paign_info_cell_
+00000420: 7261 6e67 6573 da03 6c65 6eda 0974 7261  ranges..len..tra
+00000430: 6e73 6c61 7465 da03 7374 72da 096d 616b  nslate..str..mak
+00000440: 6574 7261 6e73 da05 7370 6c69 7472 0900  etrans..splitr..
+00000450: 0000 5a12 6163 6365 7373 5f73 7072 6561  ..Z.access_sprea
+00000460: 6473 6865 6574 5a11 6765 745f 6361 6d70  dsheetZ.get_camp
+00000470: 6169 676e 5f69 6e66 6f72 1100 0000 2903  aign_infor....).
+00000480: 720a 0000 00da 0f63 6861 725f 746f 5f72  r......char_to_r
+00000490: 6570 6c61 6365 5a12 576f 726b 7368 6565  eplaceZ.Workshee
+000004a0: 745f 7365 6c65 6374 6564 720b 0000 0072  t_selectedr....r
+000004b0: 0b00 0000 720c 0000 00da 0f67 6574 4361  ....r......getCa
+000004c0: 6d70 6169 676e 496e 666f 0e00 0000 7310  mpaignInfo....s.
+000004d0: 0000 0000 0114 0114 020e 0110 0124 020a  .............$..
+000004e0: 0116 017a 1449 6e66 6f2e 6765 7443 616d  ...z.Info.getCam
+000004f0: 7061 6967 6e49 6e66 6f63 0100 0000 0000  paignInfoc......
+00000500: 0000 0000 0000 0200 0000 0600 0000 4300  ..............C.
+00000510: 0000 737a 0000 0074 006a 017c 006a 0264  ..sz...t.j.|.j.d
+00000520: 0164 0264 038d 037c 005f 0374 006a 017c  .d.d...|._.t.j.|
+00000530: 006a 0264 0464 0064 038d 037c 005f 0464  .j.d.d.d...|._.d
+00000540: 0564 0564 0564 0564 0564 069c 057d 0164  .d.d.d.d.d...}.d
+00000550: 0764 0884 0074 057c 006a 0483 01a0 0674  .d...t.|.j.....t
+00000560: 05a0 077c 01a1 01a1 01a0 0864 09a1 0144  ...|.......d...D
+00000570: 0083 017c 005f 047c 006a 09a0 0a7c 006a  ...|._.|.j...|.j
+00000580: 037c 006a 04a1 027c 005f 0b7c 006a 0b53  .|.j...|._.|.j.S
+00000590: 0029 0a4e da20 776f 726b 7368 6565 745f  .).N. worksheet_
+000005a0: 7469 746c 655f 6361 6d70 6169 676e 5f63  title_campaign_c
+000005b0: 6f6e 7465 6e74 7a10 4361 6d70 6169 676e  ontentz.Campaign
+000005c0: 2043 6f6e 7465 6e74 720f 0000 005a 1063   Contentr....Z.c
+000005d0: 616d 7061 6967 6e5f 636f 6e74 656e 7472  ampaign_contentr
+000005e0: 1200 0000 7213 0000 0063 0100 0000 0000  ....r....c......
+000005f0: 0000 0000 0000 0200 0000 0300 0000 5300  ..............S.
+00000600: 0000 7310 0000 0067 007c 005d 087d 017c  ..s....g.|.].}.|
+00000610: 0191 0271 0453 0072 0b00 0000 720b 0000  ...q.S.r....r...
+00000620: 0072 1900 0000 720b 0000 0072 0b00 0000  .r....r....r....
+00000630: 720c 0000 0072 1c00 0000 2100 0000 721d  r....r....!...r.
+00000640: 0000 007a 2749 6e66 6f2e 6765 7468 746d  ...z'Info.gethtm
+00000650: 6c43 6f6e 7465 6e74 2e3c 6c6f 6361 6c73  lContent.<locals
+00000660: 3e2e 3c6c 6973 7463 6f6d 703e 721e 0000  >.<listcomp>r...
+00000670: 0029 0c72 1f00 0000 7220 0000 0072 0800  .).r....r ...r..
+00000680: 0000 7228 0000 005a 1c63 616d 7061 6967  ..r(...Z.campaig
+00000690: 6e5f 636f 6e74 656e 745f 6365 6c6c 5f72  n_content_cell_r
+000006a0: 616e 6765 7372 2300 0000 7222 0000 0072  angesr#...r"...r
+000006b0: 2400 0000 7225 0000 0072 0900 0000 5a10  $...r%...r....Z.
+000006c0: 6765 745f 636f 6e74 656e 745f 696e 666f  get_content_info
+000006d0: da04 6461 7461 2902 720a 0000 0072 2600  ..data).r....r&.
+000006e0: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
+000006f0: 00da 0e67 6574 6874 6d6c 436f 6e74 656e  ...gethtmlConten
+00000700: 741a 0000 0073 0c00 0000 0003 1401 1402  t....s..........
+00000710: 1001 2802 1401 7a13 496e 666f 2e67 6574  ..(...z.Info.get
+00000720: 6874 6d6c 436f 6e74 656e 744e 2907 da08  htmlContentN)...
+00000730: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000740: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000750: 5f5f 7223 0000 0072 0d00 0000 7227 0000  __r#...r....r'..
+00000760: 0072 2a00 0000 720b 0000 0072 0b00 0000  .r*...r....r....
+00000770: 720b 0000 0072 0c00 0000 7205 0000 0008  r....r....r.....
+00000780: 0000 0073 0600 0000 0801 1005 080c 7205  ...s..........r.
+00000790: 0000 004e 2909 5a23 6d61 696c 6368 696d  ...N).Z#mailchim
+000007a0: 705f 6175 746f 2e73 6372 6970 7473 2e67  p_auto.scripts.g
+000007b0: 7370 7265 6164 5f64 6174 6172 0200 0000  spread_datar....
+000007c0: da0c 636f 6e66 6967 7061 7273 6572 7203  ..configparserr.
+000007d0: 0000 005a 206d 6169 6c63 6869 6d70 5f61  ...Z mailchimp_a
+000007e0: 7574 6f2e 7363 7269 7074 732e 6469 7265  uto.scripts.dire
+000007f0: 6374 6f72 7972 1f00 0000 da04 7265 6164  ctoryr......read
+00000800: da0f 7465 6d70 6c61 7465 5f63 6f6e 6669  ..template_confi
+00000810: 6772 0500 0000 720b 0000 0072 0b00 0000  gr....r....r....
+00000820: 720b 0000 0072 0c00 0000 da08 3c6d 6f64  r....r......<mod
+00000830: 756c 653e 0100 0000 730a 0000 000c 010c  ule>....s.......
+00000840: 0108 0206 010a 02                        .......
```

### Comparing `mailchimp_auto-0.1.0/mailchimp_auto/scripts/__pycache__/Config.cpython-310.pyc` & `mailchimp_auto-0.1.1/mailchimp_auto/scripts/__pycache__/Config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 29 04:19:46 2022 UTC, .py size: 6743 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,302 +1,297 @@
-00000000: 6f0d 0d0a 0000 0000 e25f e362 571a 0000  o........_.bW...
+00000000: 610d 0d0a 0000 0000 4230 3064 571a 0000  a.......B00dW...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 ac00 0000 6400  .....@...s....d.
+00000020: 0005 0000 0040 0000 0073 a200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5400 6400 6404 6c04 6d05 5a05 0100 6501  T.d.d.l.m.Z...e.
 00000060: 8300 5a06 6405 6406 8400 5a07 6407 6408  ..Z.d.d...Z.d.d.
-00000070: 8400 5a08 6409 6509 640a 6509 6604 640b  ..Z.d.e.d.e.f.d.
-00000080: 640c 8404 5a0a 641a 640f 6509 6410 6509  d...Z.d.d.e.d.e.
-00000090: 6411 6509 6606 6412 6413 8405 5a0b 641b  d.e.f.d.d...Z.d.
-000000a0: 640f 6509 640a 650c 6501 1900 6604 6414  d.e.d.e.e...f.d.
-000000b0: 6415 8405 5a0d 641b 640f 6509 640a 650c  d...Z.d.d.e.d.e.
-000000c0: 6501 1900 6604 6416 6417 8405 5a0e 6418  e...f.d.d...Z.d.
-000000d0: 6419 8400 5a0f 6402 5300 291c e900 0000  d...Z.d.S.).....
-000000e0: 0029 01da 0f52 6177 436f 6e66 6967 5061  .)...RawConfigPa
-000000f0: 7273 6572 4e29 01da 012a 2901 da0a 6372  rserN)...*)...cr
-00000100: 6561 7465 5f64 6972 6300 0000 0000 0000  eate_dirc.......
-00000110: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-00000120: 0073 2400 0000 7400 8300 0100 7401 8300  .s$...t.....t...
-00000130: 7d00 7402 7c00 8301 7d01 7403 7c00 7c01  }.t.|...}.t.|.|.
-00000140: 6401 8d02 0100 6400 5300 2902 4e29 02da  d.....d.S.).N)..
-00000150: 0d61 6374 696f 6e5f 6368 6f69 6365 da0e  .action_choice..
-00000160: 6163 636f 756e 745f 6368 6f69 6365 2904  account_choice).
-00000170: 7204 0000 00da 0d73 656c 6563 745f 6163  r......select_ac
-00000180: 7469 6f6e da0e 7365 6c65 6374 5f61 6363  tion..select_acc
-00000190: 6f75 6e74 da0c 7772 6974 655f 636f 6e66  ount..write_conf
-000001a0: 6967 2902 5a0f 6163 7469 6f6e 5f73 656c  ig).Z.action_sel
-000001b0: 6563 7465 645a 1061 6363 6f75 6e74 5f73  ectedZ.account_s
-000001c0: 656c 6563 7465 64a9 0072 0a00 0000 fa69  elected..r.....i
-000001d0: 433a 5c55 7365 7273 5c74 7973 5c44 6f63  C:\Users\tys\Doc
-000001e0: 756d 656e 7473 5c50 726f 6a65 6374 5c6d  uments\Project\m
-000001f0: 6169 6c63 6869 6d70 5f63 7265 6174 696f  ailchimp_creatio
-00000200: 6e5f 7072 6f6a 6563 745c 6d61 696c 6368  n_project\mailch
-00000210: 696d 702d 6175 746f 5c6d 6169 6c63 6869  imp-auto\mailchi
-00000220: 6d70 5f61 7574 6f5c 7363 7269 7074 735c  mp_auto\scripts\
-00000230: 436f 6e66 6967 2e70 79da 0b63 6f6e 6669  Config.py..confi
-00000240: 675f 7061 6765 0a00 0000 7308 0000 0006  g_page....s.....
-00000250: 0106 0108 0110 0172 0c00 0000 6300 0000  .......r....c...
-00000260: 0000 0000 0000 0000 0003 0000 000a 0000  ................
-00000270: 0043 0000 0073 be00 0000 7400 6401 8301  .C...s....t.d...
-00000280: 0100 7400 6402 8301 0100 7400 6403 8301  ..t.d.....t.d...
-00000290: 0100 7401 7402 6404 8301 a003 a100 8301  ..t.t.d.........
-000002a0: 6405 6b04 7231 7402 6404 8301 a003 a100  d.k.r1t.d.......
-000002b0: 4400 5d14 7d00 7400 7404 7c00 8301 6406  D.].}.t.t.|...d.
-000002c0: 7404 7402 6404 8301 6a05 7c00 6407 6400  t.t.d...j.|.d.d.
-000002d0: 6408 8d03 8301 8303 0100 711c 7400 6409  d.........q.t.d.
-000002e0: 8301 0100 7400 640a 8301 0100 7400 640b  ....t.d.....t.d.
-000002f0: 8301 0100 7400 640c 8301 0100 7400 640d  ....t.d.....t.d.
-00000300: 8301 0100 6700 640e a201 7d01 7406 640f  ....g.d...}.t.d.
-00000310: 8301 7d02 7c02 7c01 7601 725d 7400 6410  ..}.|.|.v.r]t.d.
-00000320: 8301 0100 7406 640f 8301 7d02 7c02 7c01  ....t.d...}.|.|.
-00000330: 7601 7351 7c02 5300 2911 4e7a 1a0a 4375  v.sQ|.S.).Nz..Cu
-00000340: 7272 656e 7420 4d61 696c 6368 696d 7020  rrent Mailchimp 
-00000350: 7265 6d6f 7465 3a7a 1e41 6363 6f75 6e74  remote:z.Account
-00000360: 2055 7365 726e 616d 6509 5365 7276 6572   Username.Server
-00000370: 2050 7265 6669 787a 1f3d 3d3d 3d3d 3d3d   Prefixz.=======
-00000380: 3d3d 3d3d 3d3d 3d3d 3d3d 093d 3d3d 3d3d  ==========.=====
-00000390: 3d3d 3d3d 3d3d 3d3d fa0c 6163 636f 756e  ========..accoun
-000003a0: 742e 636f 6e66 7201 0000 007a 0209 09da  t.confr....z....
-000003b0: 0d73 6572 7665 725f 7072 6566 6978 a901  .server_prefix..
-000003c0: da08 6661 6c6c 6261 636b da01 0a7a 1865  ..fallback...z.e
-000003d0: 2920 4564 6974 2065 7869 7374 696e 6720  ) Edit existing 
-000003e0: 6163 636f 756e 747a 0e6e 2920 4e65 7720  accountz.n) New 
-000003f0: 6163 636f 756e 747a 1164 2920 4465 6c65  accountz.d) Dele
-00000400: 7465 2061 6363 6f75 6e74 7a07 7129 2071  te accountz.q) q
-00000410: 7569 7429 04da 0165 da01 6eda 0164 da01  uit)...e..n..d..
-00000420: 717a 0a65 2f6e 2f64 2f71 203e 207a 4754  qz.e/n/d/q > zGT
-00000430: 6869 7320 7661 6c75 6520 6d75 7374 2062  his value must b
-00000440: 6520 6120 7369 6e67 6c65 2063 6861 7261  e a single chara
-00000450: 6374 6572 2c20 6f6e 6520 6f66 2074 6865  cter, one of the
-00000460: 2066 6f6c 6c6f 7769 6e67 3a20 652c 206e   following: e, n
-00000470: 2c20 642c 2071 2907 da05 7072 696e 74da  , d, q)...print.
-00000480: 036c 656e da0b 7265 6164 5f63 6f6e 6669  .len..read_confi
-00000490: 67da 0873 6563 7469 6f6e 73da 0373 7472  g..sections..str
-000004a0: da03 6765 74da 0569 6e70 7574 2903 da07  ..get..input)...
-000004b0: 6163 636f 756e 74da 1261 6363 6570 7461  account..accepta
-000004c0: 626c 655f 6368 6f69 6365 7372 0500 0000  ble_choicesr....
-000004d0: 720a 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
-000004e0: 0700 0000 1000 0000 7324 0000 0008 0208  ........s$......
-000004f0: 0108 0114 0310 0126 0108 0108 0108 0108  .......&........
-00000500: 0108 0108 0208 0108 0108 0108 0108 fe04  ................
-00000510: 0372 0700 0000 da0a 6163 745f 6368 6f69  .r......act_choi
-00000520: 6365 da06 7265 7475 726e 6301 0000 0000  ce..returnc.....
-00000530: 0000 0000 0000 0004 0000 0008 0000 0043  ...............C
-00000540: 0000 0073 0201 0000 7c00 6401 6b02 7207  ...s....|.d.k.r.
-00000550: 0900 7c00 5300 7c00 6402 6b03 727f 7400  ..|.S.|.d.k.r.t.
-00000560: 7401 6403 8301 a002 a100 8301 727f 7403  t.d.........r.t.
-00000570: 6404 8301 0100 7403 6405 8301 0100 7404  d.....t.d.....t.
-00000580: 7401 6403 8301 a002 a100 8301 4400 5d0c  t.d.........D.].
-00000590: 5c02 7d01 7d02 7403 7c01 6406 1700 6407  \.}.}.t.|.d...d.
-000005a0: 7c02 8303 0100 7123 6408 6409 8400 7401  |.....q#d.d...t.
-000005b0: 6403 8301 a002 a100 4400 8301 7d03 7c03  d.......D...}.|.
-000005c0: a005 640a 6409 8400 7406 6406 7400 7401  ..d.d...t.d.t.t.
-000005d0: 6403 8301 a002 a100 8301 6406 1700 6406  d.........d...d.
-000005e0: 8303 4400 8301 a101 0100 7407 640b 8301  ..D.......t.d...
-000005f0: 7d00 7c00 7c03 7601 7265 7403 640c 8301  }.|.|.v.ret.d...
-00000600: 0100 7407 640b 8301 7d00 7c00 7c03 7601  ..t.d...}.|.|.v.
-00000610: 7359 7a0f 7401 6403 8301 a002 a100 7408  sYz.t.d.......t.
-00000620: 7c00 8301 6406 1800 1900 7d00 5700 7c00  |...d.....}.W.|.
-00000630: 5300 0400 7409 797e 0100 0100 0100 5900  S...t.y~......Y.
-00000640: 7c00 5300 7700 7c00 5300 290d 4e72 1500  |.S.w.|.S.).Nr..
-00000650: 0000 7213 0000 0072 0d00 0000 7a10 0a53  ..r....r....z..S
-00000660: 656c 6563 7420 6163 636f 756e 742e 7a39  elect account.z9
-00000670: 4368 6f6f 7365 2061 206e 756d 6265 7220  Choose a number 
-00000680: 6672 6f6d 2062 656c 6f77 2c20 6f72 2074  from below, or t
-00000690: 7970 6520 696e 2061 6e20 6578 6973 7469  ype in an existi
-000006a0: 6e67 2076 616c 7565 2ee9 0100 0000 7a02  ng value......z.
-000006b0: 3e20 6301 0000 0000 0000 0000 0000 0002  > c.............
-000006c0: 0000 0003 0000 0053 0000 0073 1000 0000  .......S...s....
-000006d0: 6700 7c00 5d04 7d01 7c01 9102 7102 5300  g.|.].}.|...q.S.
-000006e0: 720a 0000 0072 0a00 0000 2902 da02 2e30  r....r....)....0
-000006f0: 721d 0000 0072 0a00 0000 720a 0000 0072  r....r....r....r
-00000700: 0b00 0000 da0a 3c6c 6973 7463 6f6d 703e  ......<listcomp>
-00000710: 3200 0000 7302 0000 0010 007a 2273 656c  2...s......z"sel
-00000720: 6563 745f 6163 636f 756e 742e 3c6c 6f63  ect_account.<loc
-00000730: 616c 733e 2e3c 6c69 7374 636f 6d70 3e63  als>.<listcomp>c
-00000740: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000750: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
-00000760: 005d 067d 0174 007c 0183 0191 0271 0253  .].}.t.|.....q.S
-00000770: 0072 0a00 0000 2901 721a 0000 0029 0272  .r....).r....).r
-00000780: 2200 0000 da05 696e 6465 7872 0a00 0000  ".....indexr....
-00000790: 720a 0000 0072 0b00 0000 7223 0000 0033  r....r....r#...3
-000007a0: 0000 0073 0200 0000 1400 7a0a 4163 636f  ...s......z.Acco
-000007b0: 756e 7420 3e20 7a1b 4e6f 2063 686f 6963  unt > z.No choic
-000007c0: 6573 2077 6974 6820 796f 7572 2069 6e70  es with your inp
-000007d0: 7574 2e29 0a72 1700 0000 7218 0000 0072  ut.).r....r....r
-000007e0: 1900 0000 7216 0000 00da 0965 6e75 6d65  ....r......enume
-000007f0: 7261 7465 da06 6578 7465 6e64 da05 7261  rate..extend..ra
-00000800: 6e67 6572 1c00 0000 da03 696e 74da 0a56  nger......int..V
-00000810: 616c 7565 4572 726f 7229 0472 1f00 0000  alueError).r....
-00000820: 7224 0000 0072 1d00 0000 721e 0000 0072  r$...r....r....r
-00000830: 0a00 0000 720a 0000 0072 0b00 0000 7208  ....r....r....r.
-00000840: 0000 0027 0000 0073 2e00 0000 0801 0201  ...'...s........
-00000850: 0414 18ee 0801 0801 1802 1201 1602 2c01  ..............,.
-00000860: 0801 0802 0801 0801 08fe 0203 1a01 0403  ................
-00000870: 0cfe 0201 0401 02fe 0402 7208 0000 0072  ..........r....r
-00000880: 0d00 0000 da00 da0b 636f 6e66 6967 5f66  ........config_f
-00000890: 696c 6572 0500 0000 7206 0000 0063 0300  iler....r....c..
-000008a0: 0000 0000 0000 0000 0000 0900 0000 0800  ................
-000008b0: 0000 4300 0000 7348 0100 0074 006a 01a0  ..C...sH...t.j..
-000008c0: 0274 037c 00a1 027d 0074 047c 0083 017d  .t.|...}.t.|...}
-000008d0: 0374 05a0 067c 03a1 0101 007c 0164 016b  .t...|.....|.d.k
-000008e0: 0272 5174 0774 0864 0283 01a0 09a1 0083  .rQt.t.d........
-000008f0: 0164 036b 0472 5174 05a0 0a7c 02a1 0101  .d.k.rQt...|....
-00000900: 0074 0b7c 0364 0483 028f 0d7d 0474 05a0  .t.|.d.....}.t..
-00000910: 0c7c 04a1 0101 0057 0064 0004 0004 0083  .|.....W.d......
-00000920: 0301 006e 0831 0073 3877 0101 0001 0001  ...n.1.s8w......
-00000930: 0059 0001 0074 0d7c 0283 0164 0517 007d  .Y...t.|...d...}
-00000940: 0574 006a 01a0 0274 0e7c 05a1 027d 0674  .t.j...t.|...}.t
-00000950: 00a0 0f7c 06a1 0101 0064 0053 007c 0164  ...|.....d.S.|.d
-00000960: 0676 0072 9874 056a 107c 0264 0764 0064  .v.r.t.j.|.d.d.d
-00000970: 088d 037d 0774 056a 107c 0264 0964 0064  ...}.t.j.|.d.d.d
-00000980: 088d 037d 087c 0164 0a6b 0272 7b74 1164  ...}.|.d.k.r{t.d
-00000990: 0b83 017d 0274 05a0 127c 02a1 0101 0074  ...}.t...|.....t
-000009a0: 137c 077c 087c 0264 0c8d 0301 0064 0053  .|.|.|.d.....d.S
-000009b0: 007c 0164 0d6b 0272 9274 0774 0864 0283  .|.d.k.r.t.t.d..
-000009c0: 01a0 09a1 0083 0164 036b 0472 9274 137c  .......d.k.r.t.|
-000009d0: 077c 087c 0264 0c8d 0301 0064 0053 0074  .|.|.d.....d.S.t
-000009e0: 1464 0e83 0101 0064 0053 007c 0164 0f6b  .d.....d.S.|.d.k
-000009f0: 0272 9e64 0053 0074 1464 1083 0101 0064  .r.d.S.t.d.....d
-00000a00: 0053 0029 114e 7214 0000 0072 0d00 0000  .S.).Nr....r....
-00000a10: 7201 0000 00da 0177 fa05 2e6a 736f 6e29  r......w...json)
-00000a20: 0272 1200 0000 7213 0000 00da 0761 7069  .r....r......api
-00000a30: 5f6b 6579 720f 0000 0072 0e00 0000 7213  _keyr....r....r.
-00000a40: 0000 007a 2c0a 456e 7465 7220 7573 6572  ...z,.Enter user
-00000a50: 6e61 6d65 206f 6620 4d61 696c 6368 696d  name of Mailchim
-00000a60: 7020 4163 636f 756e 742e 0a6e 616d 653a  p Account..name:
-00000a70: 2029 0372 2e00 0000 720e 0000 0072 0600   ).r....r....r..
-00000a80: 0000 7212 0000 007a 134e 6f20 6163 636f  ..r....z.No acco
-00000a90: 756e 7420 746f 2065 6469 7421 7215 0000  unt to edit!r...
-00000aa0: 007a 154e 6f20 6163 636f 756e 7420 746f  .z.No account to
-00000ab0: 2064 656c 6574 6521 2915 da02 6f73 da04   delete!)...os..
-00000ac0: 7061 7468 da04 6a6f 696e da0d 636f 6e66  path..join..conf
-00000ad0: 6967 5f66 6f6c 6465 72da 1063 6f6e 6669  ig_folder..confi
-00000ae0: 675f 6669 6c65 5f70 6174 68da 0463 6f6e  g_file_path..con
-00000af0: 66da 0472 6561 6472 1700 0000 7218 0000  f..readr....r...
-00000b00: 0072 1900 0000 da0e 7265 6d6f 7665 5f73  .r......remove_s
-00000b10: 6563 7469 6f6e da04 6f70 656e da05 7772  ection..open..wr
-00000b20: 6974 6572 1a00 0000 da16 7365 7276 6963  iter......servic
-00000b30: 655f 6163 636f 756e 745f 666f 6c64 6572  e_account_folder
-00000b40: da06 756e 6c69 6e6b 721b 0000 0072 1c00  ..unlinkr....r..
-00000b50: 0000 da0b 6164 645f 7365 6374 696f 6eda  ....add_section.
-00000b60: 0b6d 6169 6e5f 636f 6e66 6967 7216 0000  .main_configr...
-00000b70: 0029 0972 2b00 0000 7205 0000 0072 0600  .).r+...r....r..
-00000b80: 0000 7230 0000 00da 0a63 6f6e 6669 6766  ..r0.....configf
-00000b90: 696c 65da 0c73 615f 6669 6c65 5f6e 616d  ile..sa_file_nam
-00000ba0: 65da 1173 615f 6675 6c6c 5f66 696c 655f  e..sa_full_file_
-00000bb0: 6e61 6d65 722e 0000 0072 0e00 0000 720a  namer....r....r.
-00000bc0: 0000 0072 0a00 0000 720b 0000 0072 0900  ...r....r....r..
-00000bd0: 0000 3f00 0000 7330 0000 000e 0108 010a  ..?...s0........
-00000be0: 011c 020a 010c 010c 011c ff0c 030e 010e  ................
-00000bf0: 0108 0210 0110 0108 0408 010a 0112 021c  ................
-00000c00: 0112 010c 0208 0204 010c 0372 0900 0000  ...........r....
-00000c10: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000c20: 0004 0000 0043 0000 0073 2400 0000 7400  .....C...s$...t.
-00000c30: 6a01 a002 7403 7c00 a102 7d00 7404 7c00  j...t.|...}.t.|.
-00000c40: 8301 7d01 7405 a006 7c01 a101 0100 7405  ..}.t...|.....t.
-00000c50: 5300 a901 4e29 0772 2f00 0000 7230 0000  S...N).r/...r0..
-00000c60: 0072 3100 0000 7232 0000 0072 3300 0000  .r1...r2...r3...
-00000c70: 7234 0000 0072 3500 0000 2902 722b 0000  r4...r5...).r+..
-00000c80: 0072 3000 0000 720a 0000 0072 0a00 0000  .r0...r....r....
-00000c90: 720b 0000 0072 1800 0000 6300 0000 7308  r....r....c...s.
-00000ca0: 0000 000e 0108 010a 0104 0172 1800 0000  ...........r....
-00000cb0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000cc0: 0004 0000 0043 0000 0073 1200 0000 7400  .....C...s....t.
-00000cd0: 6a01 a002 7403 7c00 a102 7d00 7c00 5300  j...t.|...}.|.S.
-00000ce0: 7240 0000 0029 0472 2f00 0000 7230 0000  r@...).r/...r0..
-00000cf0: 0072 3100 0000 7232 0000 0029 0172 2b00  .r1...r2...).r+.
-00000d00: 0000 720a 0000 0072 0a00 0000 720b 0000  ..r....r....r...
-00000d10: 0072 3300 0000 6900 0000 7304 0000 000e  .r3...i...s.....
-00000d20: 0104 0172 3300 0000 6303 0000 0000 0000  ...r3...c.......
-00000d30: 0000 0000 000c 0000 0008 0000 0043 0000  .............C..
-00000d40: 0073 a401 0000 7400 7c02 8301 6401 1700  .s....t.|...d...
-00000d50: 7d03 7401 6a02 6a03 7d04 7401 6a02 a004  }.t.j.j.}.t.j...
-00000d60: 7405 7c03 a102 7d05 7406 8300 7d06 7407  t.|...}.t...}.t.
-00000d70: 6402 7c00 9b00 6403 9d03 8301 7d07 7408  d.|...d.....}.t.
-00000d80: 7c07 8301 6404 6b02 7224 7c00 6e01 7c07  |...d.k.r$|.n.|.
-00000d90: 7d07 7c07 a009 6405 a101 6406 1900 7d08  }.|...d...d...}.
-00000da0: 7408 7c08 8301 6404 6b02 7235 7c01 6e01  t.|...d.k.r5|.n.
-00000db0: 7c08 7d08 740a 6a0b 7c02 6407 6400 6408  |.}.t.j.|.d.d.d.
-00000dc0: 8d03 7d09 7407 6409 7c09 9b00 6403 9d03  ..}.t.d.|...d...
-00000dd0: 8301 7d0a 7408 7c0a 8301 6404 6b03 7277  ..}.t.|...d.k.rw
-00000de0: 7c0a a00c 640a 640b a102 a009 640c 6406  |...d.d.....d.d.
-00000df0: a102 6406 1900 640d 6b03 7277 740d 640e  ..d...d.k.rwt.d.
-00000e00: 8301 0100 7407 640f 8301 7d0a 7408 7c0a  ....t.d...}.t.|.
-00000e10: 8301 6404 6b03 7277 7c0a a00c 640a 640b  ..d.k.rw|...d.d.
-00000e20: a102 a009 640c 6406 a102 6406 1900 640d  ....d.d...d...d.
-00000e30: 6b03 735b 7408 7c0a 8301 6404 6b02 727f  k.s[t.|...d.k.r.
-00000e40: 7c09 6e01 7c0a 7d0a 7a14 740e a00f 7c0a  |.n.|.}.z.t...|.
-00000e50: a00c 640a 640b a102 7c05 a102 0100 740d  ..d.d...|.....t.
-00000e60: 6410 7c05 9b00 640c 9d03 8301 0100 5700  d.|...d.......W.
-00000e70: 6e0a 0400 740e 6a10 799f 0100 0100 0100  n...t.j.y.......
-00000e80: 5900 6e01 7700 740a a011 7c02 6411 7c07  Y.n.w.t...|.d.|.
-00000e90: a103 0100 740a a011 7c02 6412 7c08 a103  ....t...|.d.|...
-00000ea0: 0100 740a a011 7c02 6407 7c05 a103 0100  ..t...|.d.|.....
-00000eb0: 7412 7c06 6413 8302 8f0e 7d0b 740a a013  t.|.d.....}.t...
-00000ec0: 7c0b a101 0100 5700 6400 0400 0400 8303  |.....W.d.......
-00000ed0: 0100 6400 5300 3100 73cb 7701 0100 0100  ..d.S.1.s.w.....
-00000ee0: 0100 5900 0100 6400 5300 2914 4e72 2d00  ..Y...d.S.).Nr-.
-00000ef0: 0000 7a42 0a4d 6169 6c63 6869 6d70 2041  ..zB.Mailchimp A
-00000f00: 5049 0a45 6e74 6572 2061 2073 7472 696e  PI.Enter a strin
-00000f10: 6720 7661 6c75 652e 2050 7265 7373 2045  g value. Press E
-00000f20: 6e74 6572 2066 6f72 2074 6865 2064 6566  nter for the def
-00000f30: 6175 6c74 2028 7a03 293a 2072 0100 0000  ault (z.): r....
-00000f40: fa01 2d72 2100 0000 da19 7365 7276 6963  ..-r!.....servic
-00000f50: 655f 6163 636f 756e 745f 6669 6c65 5f70  e_account_file_p
-00000f60: 6174 6872 0f00 0000 7a7d 0a53 6572 7669  athr....z}.Servi
-00000f70: 6365 5f61 6363 6f75 6e74 5f66 696c 652e  ce_account_file.
-00000f80: 0a47 6f6f 676c 6520 5365 7276 6963 6520  .Google Service 
-00000f90: 4163 636f 756e 7420 4372 6564 656e 7469  Account Credenti
-00000fa0: 616c 7320 4a53 4f4e 2066 696c 6520 7061  als JSON file pa
-00000fb0: 7468 2e0a 456e 7465 7220 6120 7374 7269  th..Enter a stri
-00000fc0: 6e67 2076 616c 7565 2e20 5072 6573 7320  ng value. Press 
-00000fd0: 456e 7465 7220 666f 7220 7468 6520 6465  Enter for the de
-00000fe0: 6661 756c 7420 28fa 0122 722a 0000 00da  fault (.."r*....
-00000ff0: 012e da04 6a73 6f6e 7a2d 5468 6520 6669  ....jsonz-The fi
-00001000: 6c65 2066 6f72 6d61 7420 7368 6f75 6c64  le format should
-00001010: 2065 6e64 2077 6974 6820 2e6a 736f 6e20   end with .json 
-00001020: 666f 726d 6174 217a 4a50 6c65 6173 6520  format!zJPlease 
-00001030: 7265 2d69 6e73 6572 7420 6167 6169 6e20  re-insert again 
-00001040: 476f 6f67 6c65 2053 6572 7669 6365 2041  Google Service A
-00001050: 6363 6f75 6e74 2043 7265 6465 6e74 6961  ccount Credentia
-00001060: 6c73 204a 534f 4e20 6669 6c65 2070 6174  ls JSON file pat
-00001070: 683a 207a 3b0a 476f 6f67 6c65 2073 6572  h: z;.Google ser
-00001080: 7669 6365 2061 6363 6f75 6e74 2066 696c  vice account fil
-00001090: 6520 2869 6e20 6a73 6f6e 2066 6f72 6d61  e (in json forma
-000010a0: 7429 2069 7320 636f 7069 6564 2074 6f20  t) is copied to 
-000010b0: 722e 0000 0072 0e00 0000 722c 0000 0029  r....r....r,...)
-000010c0: 1472 1a00 0000 722f 0000 0072 3000 0000  .r....r/...r0...
-000010d0: da07 6469 726e 616d 6572 3100 0000 7239  ..dirnamer1...r9
-000010e0: 0000 0072 3300 0000 721c 0000 0072 1700  ...r3...r....r..
-000010f0: 0000 da06 7273 706c 6974 7234 0000 0072  ....rsplitr4...r
-00001100: 1b00 0000 da07 7265 706c 6163 6572 1600  ......replacer..
-00001110: 0000 da06 7368 7574 696c da04 636f 7079  ....shutil..copy
-00001120: da0d 5361 6d65 4669 6c65 4572 726f 72da  ..SameFileError.
-00001130: 0373 6574 7237 0000 0072 3800 0000 290c  .setr7...r8...).
-00001140: 722e 0000 0072 0e00 0000 7206 0000 0072  r....r....r....r
-00001150: 3e00 0000 7246 0000 0072 3f00 0000 7230  >...rF...r?...r0
-00001160: 0000 005a 0b6e 6577 5f61 7069 5f6b 6579  ...Z.new_api_key
-00001170: 5a11 6e65 775f 7365 7276 6572 5f70 7265  Z.new_server_pre
-00001180: 6669 785a 0f67 735f 6163 636f 756e 745f  fixZ.gs_account_
-00001190: 6a73 6f6e 5a13 6e65 775f 6773 5f61 6363  jsonZ.new_gs_acc
-000011a0: 6f75 6e74 5f6a 736f 6e72 3d00 0000 720a  ount_jsonr=...r.
-000011b0: 0000 0072 0a00 0000 720b 0000 0072 3c00  ...r....r....r<.
-000011c0: 0000 6d00 0000 7336 0000 000c 0108 010e  ..m...s6........
-000011d0: 0106 0310 0214 010e 0314 0210 0310 0128  ...............(
-000011e0: 0208 0108 0128 fe14 0402 0214 0114 010e  .....(..........
-000011f0: 0104 0102 ff0e 040e 010e 010c 020c 0122  ..............."
-00001200: ff72 3c00 0000 2903 720d 0000 0072 2a00  .r<...).r....r*.
-00001210: 0000 722a 0000 0029 0172 0d00 0000 2910  ..r*...).r....).
-00001220: da0c 636f 6e66 6967 7061 7273 6572 7202  ..configparserr.
-00001230: 0000 0072 2f00 0000 7249 0000 005a 206d  ...r/...rI...Z m
-00001240: 6169 6c63 6869 6d70 5f61 7574 6f2e 7363  ailchimp_auto.sc
-00001250: 7269 7074 732e 6469 7265 6374 6f72 7972  ripts.directoryr
-00001260: 0400 0000 7234 0000 0072 0c00 0000 7207  ....r4...r....r.
-00001270: 0000 0072 1a00 0000 7208 0000 0072 0900  ...r....r....r..
-00001280: 0000 da04 7479 7065 7218 0000 0072 3300  ....typer....r3.
-00001290: 0000 723c 0000 0072 0a00 0000 720a 0000  ..r<...r....r...
-000012a0: 0072 0a00 0000 720b 0000 00da 083c 6d6f  .r....r......<mo
-000012b0: 6475 6c65 3e01 0000 0073 1a00 0000 0c00  dule>....s......
-000012c0: 0801 0801 0801 0c01 0603 0802 0806 1217  ................
-000012d0: 1818 1824 1806 0c04                      ...$....
+00000070: 8400 5a08 6509 6509 6409 9c02 640a 640b  ..Z.e.e.d...d.d.
+00000080: 8404 5a0a 6418 6509 6509 6509 640e 9c03  ..Z.d.e.e.e.d...
+00000090: 640f 6410 8405 5a0b 6419 6509 650c 6501  d.d...Z.d.e.e.e.
+000000a0: 1900 6411 9c02 6412 6413 8405 5a0d 641a  ..d...d.d...Z.d.
+000000b0: 6509 650c 6501 1900 6411 9c02 6414 6415  e.e.e...d...d.d.
+000000c0: 8405 5a0e 6416 6417 8400 5a0f 6402 5300  ..Z.d.d...Z.d.S.
+000000d0: 291b e900 0000 0029 01da 0f52 6177 436f  )......)...RawCo
+000000e0: 6e66 6967 5061 7273 6572 4e29 01da 012a  nfigParserN)...*
+000000f0: 2901 da0a 6372 6561 7465 5f64 6972 6300  )...create_dirc.
+00000100: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00000110: 0000 0043 0000 0073 2400 0000 7400 8300  ...C...s$...t...
+00000120: 0100 7401 8300 7d00 7402 7c00 8301 7d01  ..t...}.t.|...}.
+00000130: 7403 7c00 7c01 6401 8d02 0100 6400 5300  t.|.|.d.....d.S.
+00000140: 2902 4e29 02da 0d61 6374 696f 6e5f 6368  ).N)...action_ch
+00000150: 6f69 6365 da0e 6163 636f 756e 745f 6368  oice..account_ch
+00000160: 6f69 6365 2904 7204 0000 00da 0d73 656c  oice).r......sel
+00000170: 6563 745f 6163 7469 6f6e da0e 7365 6c65  ect_action..sele
+00000180: 6374 5f61 6363 6f75 6e74 da0c 7772 6974  ct_account..writ
+00000190: 655f 636f 6e66 6967 2902 5a0f 6163 7469  e_config).Z.acti
+000001a0: 6f6e 5f73 656c 6563 7465 645a 1061 6363  on_selectedZ.acc
+000001b0: 6f75 6e74 5f73 656c 6563 7465 64a9 0072  ount_selected..r
+000001c0: 0a00 0000 fa66 433a 5c55 7365 7273 5c79  .....fC:\Users\y
+000001d0: 6f6e 6773 6865 6e67 2e74 616e 5c44 6f63  ongsheng.tan\Doc
+000001e0: 756d 656e 7473 5c43 6f64 696e 675c 6769  uments\Coding\gi
+000001f0: 7468 7562 2d70 726f 6a65 6374 5c6d 6169  thub-project\mai
+00000200: 6c63 6869 6d70 5f61 7574 6f5c 6d61 696c  lchimp_auto\mail
+00000210: 6368 696d 705f 6175 746f 5c73 6372 6970  chimp_auto\scrip
+00000220: 7473 5c43 6f6e 6669 672e 7079 da0b 636f  ts\Config.py..co
+00000230: 6e66 6967 5f70 6167 650a 0000 0073 0800  nfig_page....s..
+00000240: 0000 0001 0601 0601 0801 720c 0000 0063  ..........r....c
+00000250: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00000260: 0a00 0000 4300 0000 73b8 0000 0074 0064  ....C...s....t.d
+00000270: 0183 0101 0074 0064 0283 0101 0074 0064  .....t.d.....t.d
+00000280: 0383 0101 0074 0174 0264 0483 01a0 03a1  .....t.t.d......
+00000290: 0083 0164 056b 0472 6274 0264 0483 01a0  ...d.k.rbt.d....
+000002a0: 03a1 0044 005d 287d 0074 0074 047c 0083  ...D.](}.t.t.|..
+000002b0: 0164 0674 0474 0264 0483 016a 057c 0064  .d.t.t.d...j.|.d
+000002c0: 0764 0064 088d 0383 0183 0301 0071 3874  .d.d.........q8t
+000002d0: 0064 0983 0101 0074 0064 0a83 0101 0074  .d.....t.d.....t
+000002e0: 0064 0b83 0101 0074 0064 0c83 0101 0074  .d.....t.d.....t
+000002f0: 0064 0d83 0101 0067 0064 0ea2 017d 0174  .d.....g.d...}.t
+00000300: 0664 0f83 017d 027c 027c 0176 0172 b474  .d...}.|.|.v.r.t
+00000310: 0064 1083 0101 0074 0664 0f83 017d 0271  .d.....t.d...}.q
+00000320: 9a7c 0253 0029 114e 7a1a 0a43 7572 7265  .|.S.).Nz..Curre
+00000330: 6e74 204d 6169 6c63 6869 6d70 2072 656d  nt Mailchimp rem
+00000340: 6f74 653a 7a1e 4163 636f 756e 7420 5573  ote:z.Account Us
+00000350: 6572 6e61 6d65 0953 6572 7665 7220 5072  ername.Server Pr
+00000360: 6566 6978 7a1f 3d3d 3d3d 3d3d 3d3d 3d3d  efixz.==========
+00000370: 3d3d 3d3d 3d3d 3d09 3d3d 3d3d 3d3d 3d3d  =======.========
+00000380: 3d3d 3d3d 3dfa 0c61 6363 6f75 6e74 2e63  =====..account.c
+00000390: 6f6e 6672 0100 0000 7a02 0909 da0d 7365  onfr....z.....se
+000003a0: 7276 6572 5f70 7265 6669 78a9 01da 0866  rver_prefix....f
+000003b0: 616c 6c62 6163 6bda 010a 7a18 6529 2045  allback...z.e) E
+000003c0: 6469 7420 6578 6973 7469 6e67 2061 6363  dit existing acc
+000003d0: 6f75 6e74 7a0e 6e29 204e 6577 2061 6363  ountz.n) New acc
+000003e0: 6f75 6e74 7a11 6429 2044 656c 6574 6520  ountz.d) Delete 
+000003f0: 6163 636f 756e 747a 0771 2920 7175 6974  accountz.q) quit
+00000400: 2904 da01 65da 016e da01 64da 0171 7a0a  )...e..n..d..qz.
+00000410: 652f 6e2f 642f 7120 3e20 7a47 5468 6973  e/n/d/q > zGThis
+00000420: 2076 616c 7565 206d 7573 7420 6265 2061   value must be a
+00000430: 2073 696e 676c 6520 6368 6172 6163 7465   single characte
+00000440: 722c 206f 6e65 206f 6620 7468 6520 666f  r, one of the fo
+00000450: 6c6c 6f77 696e 673a 2065 2c20 6e2c 2064  llowing: e, n, d
+00000460: 2c20 7129 07da 0570 7269 6e74 da03 6c65  , q)...print..le
+00000470: 6eda 0b72 6561 645f 636f 6e66 6967 da08  n..read_config..
+00000480: 7365 6374 696f 6e73 da03 7374 72da 0367  sections..str..g
+00000490: 6574 da05 696e 7075 7429 03da 0761 6363  et..input)...acc
+000004a0: 6f75 6e74 da12 6163 6365 7074 6162 6c65  ount..acceptable
+000004b0: 5f63 686f 6963 6573 7205 0000 0072 0a00  _choicesr....r..
+000004c0: 0000 720a 0000 0072 0b00 0000 7207 0000  ..r....r....r...
+000004d0: 0010 0000 0073 2200 0000 0002 0801 0801  .....s".........
+000004e0: 0803 1401 1001 2601 0801 0801 0801 0801  ......&.........
+000004f0: 0802 0801 0801 0801 0801 0a01 7207 0000  ............r...
+00000500: 0029 02da 0a61 6374 5f63 686f 6963 65da  .)...act_choice.
+00000510: 0672 6574 7572 6e63 0100 0000 0000 0000  .returnc........
+00000520: 0000 0000 0400 0000 0800 0000 4300 0000  ............C...
+00000530: 73f4 0000 007c 0064 016b 0272 0a6e e67c  s....|.d.k.r.n.|
+00000540: 0064 026b 0372 f074 0074 0164 0383 01a0  .d.k.r.t.t.d....
+00000550: 02a1 0083 0172 f074 0364 0483 0101 0074  .....r.t.d.....t
+00000560: 0364 0583 0101 0074 0474 0164 0383 01a0  .d.....t.t.d....
+00000570: 02a1 0083 0144 005d 185c 027d 017d 0274  .....D.].\.}.}.t
+00000580: 037c 0164 0617 0064 077c 0283 0301 0071  .|.d...d.|.....q
+00000590: 4264 0864 0984 0074 0164 0383 01a0 02a1  Bd.d...t.d......
+000005a0: 0044 0083 017d 037c 03a0 0564 0a64 0984  .D...}.|...d.d..
+000005b0: 0074 0664 0674 0074 0164 0383 01a0 02a1  .t.d.t.t.d......
+000005c0: 0083 0164 0617 0064 0683 0344 0083 01a1  ...d...d...D....
+000005d0: 0101 0074 0764 0b83 017d 007c 007c 0376  ...t.d...}.|.|.v
+000005e0: 0172 c074 0364 0c83 0101 0074 0764 0b83  .r.t.d.....t.d..
+000005f0: 017d 0071 a67a 1c74 0164 0383 01a0 02a1  .}.q.z.t.d......
+00000600: 0074 087c 0083 0164 0618 0019 007d 0057  .t.|...d.....}.W
+00000610: 006e 1204 0074 0979 ee01 0001 0001 0059  .n...t.y.......Y
+00000620: 006e 0230 007c 0053 0029 0d4e 7215 0000  .n.0.|.S.).Nr...
+00000630: 0072 1300 0000 720d 0000 007a 100a 5365  .r....r....z..Se
+00000640: 6c65 6374 2061 6363 6f75 6e74 2e7a 3943  lect account.z9C
+00000650: 686f 6f73 6520 6120 6e75 6d62 6572 2066  hoose a number f
+00000660: 726f 6d20 6265 6c6f 772c 206f 7220 7479  rom below, or ty
+00000670: 7065 2069 6e20 616e 2065 7869 7374 696e  pe in an existin
+00000680: 6720 7661 6c75 652e e901 0000 007a 023e  g value......z.>
+00000690: 2063 0100 0000 0000 0000 0000 0000 0200   c..............
+000006a0: 0000 0300 0000 5300 0000 7310 0000 0067  ......S...s....g
+000006b0: 007c 005d 087d 017c 0191 0271 0453 0072  .|.].}.|...q.S.r
+000006c0: 0a00 0000 720a 0000 0029 02da 022e 3072  ....r....)....0r
+000006d0: 1d00 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
+000006e0: 0000 00da 0a3c 6c69 7374 636f 6d70 3e32  .....<listcomp>2
+000006f0: 0000 00f3 0000 0000 7a22 7365 6c65 6374  ........z"select
+00000700: 5f61 6363 6f75 6e74 2e3c 6c6f 6361 6c73  _account.<locals
+00000710: 3e2e 3c6c 6973 7463 6f6d 703e 6301 0000  >.<listcomp>c...
+00000720: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00000730: 0053 0000 0073 1400 0000 6700 7c00 5d0c  .S...s....g.|.].
+00000740: 7d01 7400 7c01 8301 9102 7104 5300 720a  }.t.|.....q.S.r.
+00000750: 0000 0029 0172 1a00 0000 2902 7222 0000  ...).r....).r"..
+00000760: 00da 0569 6e64 6578 720a 0000 0072 0a00  ...indexr....r..
+00000770: 0000 720b 0000 0072 2300 0000 3300 0000  ..r....r#...3...
+00000780: 7224 0000 007a 0a41 6363 6f75 6e74 203e  r$...z.Account >
+00000790: 207a 1b4e 6f20 6368 6f69 6365 7320 7769   z.No choices wi
+000007a0: 7468 2079 6f75 7220 696e 7075 742e 290a  th your input.).
+000007b0: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
+000007c0: 1600 0000 da09 656e 756d 6572 6174 65da  ......enumerate.
+000007d0: 0665 7874 656e 64da 0572 616e 6765 721c  .extend..ranger.
+000007e0: 0000 00da 0369 6e74 da0a 5661 6c75 6545  .....int..ValueE
+000007f0: 7272 6f72 2904 721f 0000 0072 2500 0000  rror).r....r%...
+00000800: 721d 0000 0072 1e00 0000 720a 0000 0072  r....r....r....r
+00000810: 0a00 0000 720b 0000 0072 0800 0000 2700  ....r....r....'.
+00000820: 0000 7324 0000 0000 0108 0102 0218 0108  ..s$............
+00000830: 0108 0218 0112 0216 012c 0108 0208 0108  .........,......
+00000840: 010a 0102 011c 010c 0106 0172 0800 0000  ...........r....
+00000850: 720d 0000 00da 0029 03da 0b63 6f6e 6669  r......)...confi
+00000860: 675f 6669 6c65 7205 0000 0072 0600 0000  g_filer....r....
+00000870: 6303 0000 0000 0000 0000 0000 0009 0000  c...............
+00000880: 0008 0000 0043 0000 0073 4601 0000 7400  .....C...sF...t.
+00000890: 6a01 a002 7403 7c00 a102 7d00 7404 7c00  j...t.|...}.t.|.
+000008a0: 8301 7d03 7405 a006 7c03 a101 0100 7c01  ..}.t...|.....|.
+000008b0: 6401 6b02 72a0 7407 7408 6402 8301 a009  d.k.r.t.t.d.....
+000008c0: a100 8301 6403 6b04 72a0 7405 a00a 7c02  ....d.k.r.t...|.
+000008d0: a101 0100 740b 7c03 6404 8302 8f1a 7d04  ....t.|.d.....}.
+000008e0: 7405 a00c 7c04 a101 0100 5700 6400 0400  t...|.....W.d...
+000008f0: 0400 8303 0100 6e10 3100 7370 3000 0100  ......n.1.sp0...
+00000900: 0100 0100 5900 0100 740d 7c02 8301 6405  ....Y...t.|...d.
+00000910: 1700 7d05 7400 6a01 a002 740e 7c05 a102  ..}.t.j...t.|...
+00000920: 7d06 7400 a00f 7c06 a101 0100 6ea2 7c01  }.t...|.....n.|.
+00000930: 6406 7600 9001 722e 7405 6a10 7c02 6407  d.v...r.t.j.|.d.
+00000940: 6400 6408 8d03 7d07 7405 6a10 7c02 6409  d.d...}.t.j.|.d.
+00000950: 6400 6408 8d03 7d08 7c01 640a 6b02 72f4  d.d...}.|.d.k.r.
+00000960: 7411 640b 8301 7d02 7405 a012 7c02 a101  t.d...}.t...|...
+00000970: 0100 7413 7c07 7c08 7c02 640c 8d03 0100  ..t.|.|.|.d.....
+00000980: 6e38 7c01 640d 6b02 9001 7224 7407 7408  n8|.d.k...r$t.t.
+00000990: 6402 8301 a009 a100 8301 6403 6b04 9001  d.........d.k...
+000009a0: 7224 7413 7c07 7c08 7c02 640c 8d03 0100  r$t.|.|.|.d.....
+000009b0: 6e08 7414 640e 8301 0100 6e14 7c01 640f  n.t.d.....n.|.d.
+000009c0: 6b02 9001 723a 6e08 7414 6410 8301 0100  k...r:n.t.d.....
+000009d0: 6400 5300 2911 4e72 1400 0000 720d 0000  d.S.).Nr....r...
+000009e0: 0072 0100 0000 da01 77fa 052e 6a73 6f6e  .r......w...json
+000009f0: 2902 7212 0000 0072 1300 0000 da07 6170  ).r....r......ap
+00000a00: 695f 6b65 7972 0f00 0000 720e 0000 0072  i_keyr....r....r
+00000a10: 1300 0000 7a2c 0a45 6e74 6572 2075 7365  ....z,.Enter use
+00000a20: 726e 616d 6520 6f66 204d 6169 6c63 6869  rname of Mailchi
+00000a30: 6d70 2041 6363 6f75 6e74 2e0a 6e61 6d65  mp Account..name
+00000a40: 3a20 2903 722f 0000 0072 0e00 0000 7206  : ).r/...r....r.
+00000a50: 0000 0072 1200 0000 7a13 4e6f 2061 6363  ...r....z.No acc
+00000a60: 6f75 6e74 2074 6f20 6564 6974 2172 1500  ount to edit!r..
+00000a70: 0000 7a15 4e6f 2061 6363 6f75 6e74 2074  ..z.No account t
+00000a80: 6f20 6465 6c65 7465 2129 15da 026f 73da  o delete!)...os.
+00000a90: 0470 6174 68da 046a 6f69 6eda 0d63 6f6e  .path..join..con
+00000aa0: 6669 675f 666f 6c64 6572 da10 636f 6e66  fig_folder..conf
+00000ab0: 6967 5f66 696c 655f 7061 7468 da04 636f  ig_file_path..co
+00000ac0: 6e66 da04 7265 6164 7217 0000 0072 1800  nf..readr....r..
+00000ad0: 0000 7219 0000 00da 0e72 656d 6f76 655f  ..r......remove_
+00000ae0: 7365 6374 696f 6eda 046f 7065 6eda 0577  section..open..w
+00000af0: 7269 7465 721a 0000 00da 1673 6572 7669  riter......servi
+00000b00: 6365 5f61 6363 6f75 6e74 5f66 6f6c 6465  ce_account_folde
+00000b10: 72da 0675 6e6c 696e 6b72 1b00 0000 721c  r..unlinkr....r.
+00000b20: 0000 00da 0b61 6464 5f73 6563 7469 6f6e  .....add_section
+00000b30: da0b 6d61 696e 5f63 6f6e 6669 6772 1600  ..main_configr..
+00000b40: 0000 2909 722c 0000 0072 0500 0000 7206  ..).r,...r....r.
+00000b50: 0000 0072 3100 0000 da0a 636f 6e66 6967  ...r1.....config
+00000b60: 6669 6c65 da0c 7361 5f66 696c 655f 6e61  file..sa_file_na
+00000b70: 6d65 da11 7361 5f66 756c 6c5f 6669 6c65  me..sa_full_file
+00000b80: 5f6e 616d 6572 2f00 0000 720e 0000 0072  _namer/...r....r
+00000b90: 0a00 0000 720a 0000 0072 0b00 0000 7209  ....r....r....r.
+00000ba0: 0000 003f 0000 0073 2e00 0000 0001 0e01  ...?...s........
+00000bb0: 0801 0a02 1c01 0a01 0c01 2802 0c01 0e01  ..........(.....
+00000bc0: 0c02 0a01 1001 1004 0801 0801 0a02 1001  ................
+00000bd0: 2001 1002 0a02 0a01 0203 7209 0000 0029   .........r....)
+00000be0: 0272 2c00 0000 7220 0000 0063 0100 0000  .r,...r ...c....
+00000bf0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00000c00: 4300 0000 7324 0000 0074 006a 01a0 0274  C...s$...t.j...t
+00000c10: 037c 00a1 027d 0074 047c 0083 017d 0174  .|...}.t.|...}.t
+00000c20: 05a0 067c 01a1 0101 0074 0553 00a9 014e  ...|.....t.S...N
+00000c30: 2907 7230 0000 0072 3100 0000 7232 0000  ).r0...r1...r2..
+00000c40: 0072 3300 0000 7234 0000 0072 3500 0000  .r3...r4...r5...
+00000c50: 7236 0000 0029 0272 2c00 0000 7231 0000  r6...).r,...r1..
+00000c60: 0072 0a00 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00000c70: 7218 0000 0063 0000 0073 0800 0000 0001  r....c...s......
+00000c80: 0e01 0801 0a01 7218 0000 0063 0100 0000  ......r....c....
+00000c90: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00000ca0: 4300 0000 7312 0000 0074 006a 01a0 0274  C...s....t.j...t
+00000cb0: 037c 00a1 027d 007c 0053 0072 4100 0000  .|...}.|.S.rA...
+00000cc0: 2904 7230 0000 0072 3100 0000 7232 0000  ).r0...r1...r2..
+00000cd0: 0072 3300 0000 2901 722c 0000 0072 0a00  .r3...).r,...r..
+00000ce0: 0000 720a 0000 0072 0b00 0000 7234 0000  ..r....r....r4..
+00000cf0: 0069 0000 0073 0400 0000 0001 0e01 7234  .i...s........r4
+00000d00: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
+00000d10: 0c00 0000 0800 0000 4300 0000 7380 0100  ........C...s...
+00000d20: 0074 007c 0283 0164 0117 007d 0374 016a  .t.|...d...}.t.j
+00000d30: 026a 037d 0474 016a 02a0 0474 057c 03a1  .j.}.t.j...t.|..
+00000d40: 027d 0574 0683 007d 0674 0764 027c 009b  .}.t...}.t.d.|..
+00000d50: 0064 039d 0383 017d 0774 087c 0783 0164  .d.....}.t.|...d
+00000d60: 046b 0272 487c 006e 027c 077d 077c 07a0  .k.rH|.n.|.}.|..
+00000d70: 0964 05a1 0164 0619 007d 0874 087c 0883  .d...d...}.t.|..
+00000d80: 0164 046b 0272 6a7c 016e 027c 087d 0874  .d.k.rj|.n.|.}.t
+00000d90: 0a6a 0b7c 0264 0764 0064 088d 037d 0974  .j.|.d.d.d...}.t
+00000da0: 0764 097c 099b 0064 039d 0383 017d 0a74  .d.|...d.....}.t
+00000db0: 087c 0a83 0164 046b 0372 c87c 0aa0 0c64  .|...d.k.r.|...d
+00000dc0: 0a64 0ba1 02a0 0964 0c64 06a1 0264 0619  .d.....d.d...d..
+00000dd0: 0064 0d6b 0372 c874 0d64 0e83 0101 0074  .d.k.r.t.d.....t
+00000de0: 0764 0f83 017d 0a71 8e74 087c 0a83 0164  .d...}.q.t.|...d
+00000df0: 046b 0272 d87c 096e 027c 0a7d 0a7a 2874  .k.r.|.n.|.}.z(t
+00000e00: 0ea0 0f7c 0aa0 0c64 0a64 0ba1 027c 05a1  ...|...d.d...|..
+00000e10: 0201 0074 0d64 107c 059b 0064 0c9d 0383  ...t.d.|...d....
+00000e20: 0101 0057 006e 1604 0074 0e6a 1090 0179  ...W.n...t.j...y
+00000e30: 1a01 0001 0001 0059 006e 0230 0074 0aa0  .......Y.n.0.t..
+00000e40: 117c 0264 117c 07a1 0301 0074 0aa0 117c  .|.d.|.....t...|
+00000e50: 0264 127c 08a1 0301 0074 0aa0 117c 0264  .d.|.....t...|.d
+00000e60: 077c 05a1 0301 0074 127c 0664 1383 028f  .|.....t.|.d....
+00000e70: 1a7d 0b74 0aa0 137c 0ba1 0101 0057 0064  .}.t...|.....W.d
+00000e80: 0004 0004 0083 0301 006e 1231 0090 0173  .........n.1...s
+00000e90: 7230 0001 0001 0001 0059 0001 0064 0053  r0.......Y...d.S
+00000ea0: 0029 144e 722e 0000 007a 420a 4d61 696c  .).Nr....zB.Mail
+00000eb0: 6368 696d 7020 4150 490a 456e 7465 7220  chimp API.Enter 
+00000ec0: 6120 7374 7269 6e67 2076 616c 7565 2e20  a string value. 
+00000ed0: 5072 6573 7320 456e 7465 7220 666f 7220  Press Enter for 
+00000ee0: 7468 6520 6465 6661 756c 7420 287a 0329  the default (z.)
+00000ef0: 3a20 7201 0000 00fa 012d 7221 0000 00da  : r......-r!....
+00000f00: 1973 6572 7669 6365 5f61 6363 6f75 6e74  .service_account
+00000f10: 5f66 696c 655f 7061 7468 720f 0000 007a  _file_pathr....z
+00000f20: 7d0a 5365 7276 6963 655f 6163 636f 756e  }.Service_accoun
+00000f30: 745f 6669 6c65 2e0a 476f 6f67 6c65 2053  t_file..Google S
+00000f40: 6572 7669 6365 2041 6363 6f75 6e74 2043  ervice Account C
+00000f50: 7265 6465 6e74 6961 6c73 204a 534f 4e20  redentials JSON 
+00000f60: 6669 6c65 2070 6174 682e 0a45 6e74 6572  file path..Enter
+00000f70: 2061 2073 7472 696e 6720 7661 6c75 652e   a string value.
+00000f80: 2050 7265 7373 2045 6e74 6572 2066 6f72   Press Enter for
+00000f90: 2074 6865 2064 6566 6175 6c74 2028 fa01   the default (..
+00000fa0: 2272 2b00 0000 da01 2eda 046a 736f 6e7a  "r+........jsonz
+00000fb0: 2d54 6865 2066 696c 6520 666f 726d 6174  -The file format
+00000fc0: 2073 686f 756c 6420 656e 6420 7769 7468   should end with
+00000fd0: 202e 6a73 6f6e 2066 6f72 6d61 7421 7a4a   .json format!zJ
+00000fe0: 506c 6561 7365 2072 652d 696e 7365 7274  Please re-insert
+00000ff0: 2061 6761 696e 2047 6f6f 676c 6520 5365   again Google Se
+00001000: 7276 6963 6520 4163 636f 756e 7420 4372  rvice Account Cr
+00001010: 6564 656e 7469 616c 7320 4a53 4f4e 2066  edentials JSON f
+00001020: 696c 6520 7061 7468 3a20 7a3b 0a47 6f6f  ile path: z;.Goo
+00001030: 676c 6520 7365 7276 6963 6520 6163 636f  gle service acco
+00001040: 756e 7420 6669 6c65 2028 696e 206a 736f  unt file (in jso
+00001050: 6e20 666f 726d 6174 2920 6973 2063 6f70  n format) is cop
+00001060: 6965 6420 746f 2072 2f00 0000 720e 0000  ied to r/...r...
+00001070: 0072 2d00 0000 2914 721a 0000 0072 3000  .r-...).r....r0.
+00001080: 0000 7231 0000 00da 0764 6972 6e61 6d65  ..r1.....dirname
+00001090: 7232 0000 0072 3a00 0000 7234 0000 0072  r2...r:...r4...r
+000010a0: 1c00 0000 7217 0000 00da 0672 7370 6c69  ....r......rspli
+000010b0: 7472 3500 0000 721b 0000 00da 0772 6570  tr5...r......rep
+000010c0: 6c61 6365 7216 0000 00da 0673 6875 7469  lacer......shuti
+000010d0: 6cda 0463 6f70 79da 0d53 616d 6546 696c  l..copy..SameFil
+000010e0: 6545 7272 6f72 da03 7365 7472 3800 0000  eError..setr8...
+000010f0: 7239 0000 0029 0c72 2f00 0000 720e 0000  r9...).r/...r...
+00001100: 0072 0600 0000 723f 0000 0072 4700 0000  .r....r?...rG...
+00001110: 7240 0000 0072 3100 0000 5a0b 6e65 775f  r@...r1...Z.new_
+00001120: 6170 695f 6b65 795a 116e 6577 5f73 6572  api_keyZ.new_ser
+00001130: 7665 725f 7072 6566 6978 5a0f 6773 5f61  ver_prefixZ.gs_a
+00001140: 6363 6f75 6e74 5f6a 736f 6e5a 136e 6577  ccount_jsonZ.new
+00001150: 5f67 735f 6163 636f 756e 745f 6a73 6f6e  _gs_account_json
+00001160: 723e 0000 0072 0a00 0000 720a 0000 0072  r>...r....r....r
+00001170: 0b00 0000 723d 0000 006d 0000 0073 3000  ....r=...m...s0.
+00001180: 0000 0001 0c01 0801 0e03 0602 1001 1403  ................
+00001190: 0e02 1403 1001 1002 2801 0801 0a02 1402  ........(.......
+000011a0: 0201 1401 1401 1001 0603 0e01 0e01 0e02  ................
+000011b0: 0c01 723d 0000 0029 0372 0d00 0000 722b  ..r=...).r....r+
+000011c0: 0000 0072 2b00 0000 2901 720d 0000 0029  ...r+...).r....)
+000011d0: 0172 0d00 0000 2910 da0c 636f 6e66 6967  .r....)...config
+000011e0: 7061 7273 6572 7202 0000 0072 3000 0000  parserr....r0...
+000011f0: 724a 0000 005a 206d 6169 6c63 6869 6d70  rJ...Z mailchimp
+00001200: 5f61 7574 6f2e 7363 7269 7074 732e 6469  _auto.scripts.di
+00001210: 7265 6374 6f72 7972 0400 0000 7235 0000  rectoryr....r5..
+00001220: 0072 0c00 0000 7207 0000 0072 1a00 0000  .r....r....r....
+00001230: 7208 0000 0072 0900 0000 da04 7479 7065  r....r......type
+00001240: 7218 0000 0072 3400 0000 723d 0000 0072  r....r4...r=...r
+00001250: 0a00 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
+00001260: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00001270: 0073 1800 0000 0c01 0801 0801 0801 0c03  .s..............
+00001280: 0602 0806 0817 1018 1424 1606 1604       .........$....
```

### Comparing `mailchimp_auto-0.1.0/mailchimp_auto/scripts/__pycache__/directory.cpython-310.pyc` & `mailchimp_auto-0.1.1/mailchimp_auto/scripts/__pycache__/directory.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 29 13:59:00 2022 UTC, .py size: 1185 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-00000000: 6f0d 0d0a 0000 0000 a4e7 e362 a104 0000  o..........b....
+00000000: 610d 0d0a 0000 0000 ec23 3064 a104 0000  a........#0d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 ae00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6501  d.l.Z.d.d.l.Z.e.
 00000040: 6a02 a003 a100 5a04 6500 6a05 a006 6504  j.....Z.e.j...e.
 00000050: 6402 6403 a103 5a07 6500 6a05 a006 6507  d.d...Z.e.j...e.
 00000060: 6404 a102 5a08 6500 6a05 a006 6507 6405  d...Z.e.j...e.d.
 00000070: a102 5a09 6500 6a05 a006 6509 6406 a102  ..Z.e.j...e.d...
 00000080: 5a0a 6500 6a05 a006 6507 6407 a102 5a0b  Z.e.j...e.d...Z.
 00000090: 6500 6a05 a006 6509 6408 a102 5a0c 6500  e.j...e.d...Z.e.
 000000a0: 6a05 a006 6509 6409 a102 5a0d 6500 6a05  j...e.d...Z.e.j.
 000000b0: a006 6509 640a a102 5a0e 640b 640c 8400  ..e.d...Z.d.d...
-000000c0: 5a0f 640d 6510 6602 640e 640f 8404 5a11  Z.d.e.f.d.d...Z.
+000000c0: 5a0f 6510 640d 9c01 640e 640f 8404 5a11  Z.e.d...d.d...Z.
 000000d0: 6410 6411 8400 5a12 6401 5300 2912 e900  d.d...Z.d.S.)...
 000000e0: 0000 004e 5a09 446f 6375 6d65 6e74 737a  ...NZ.Documentsz
 000000f0: 0e6d 6169 6c63 6869 6d70 2d61 7574 6fda  .mailchimp-auto.
 00000100: 0874 656d 706c 6174 657a 072e 636f 6e66  .templatez..conf
 00000110: 6967 5a14 7365 7276 6963 655f 6163 636f  igZ.service_acco
 00000120: 756e 745f 6669 6c65 da06 6f75 7470 7574  unt_file..output
 00000130: 7a14 6175 7468 6f72 697a 6564 5f75 7365  z.authorized_use
@@ -30,51 +30,50 @@
 000001d0: 01da 0865 7869 7374 5f6f 6b29 06da 026f  ...exist_ok)...o
 000001e0: 73da 086d 616b 6564 6972 73da 156d 6169  s..makedirs..mai
 000001f0: 6c63 6869 6d70 5f61 7574 6f5f 666f 6c64  lchimp_auto_fold
 00000200: 6572 da0f 7465 6d70 6c61 7465 5f66 6f6c  er..template_fol
 00000210: 6465 72da 1673 6572 7669 6365 5f61 6363  der..service_acc
 00000220: 6f75 6e74 5f66 6f6c 6465 72da 0d6f 7574  ount_folder..out
 00000230: 7075 745f 666f 6c64 6572 a900 720b 0000  put_folder..r...
-00000240: 0072 0b00 0000 fa6c 433a 5c55 7365 7273  .r.....lC:\Users
-00000250: 5c74 7973 5c44 6f63 756d 656e 7473 5c50  \tys\Documents\P
-00000260: 726f 6a65 6374 5c6d 6169 6c63 6869 6d70  roject\mailchimp
-00000270: 5f63 7265 6174 696f 6e5f 7072 6f6a 6563  _creation_projec
-00000280: 745c 6d61 696c 6368 696d 702d 6175 746f  t\mailchimp-auto
-00000290: 5c6d 6169 6c63 6869 6d70 5f61 7574 6f5c  \mailchimp_auto\
-000002a0: 7363 7269 7074 735c 6469 7265 6374 6f72  scripts\director
-000002b0: 792e 7079 da0a 6372 6561 7465 5f64 6972  y.py..create_dir
-000002c0: 1000 0000 730a 0000 000e 010e 010e 010e  ....s...........
-000002d0: 0112 0172 0d00 0000 da04 6669 6c65 6301  ...r......filec.
-000002e0: 0000 0000 0000 0000 0000 0001 0000 0008  ................
-000002f0: 0000 0043 0000 0073 4000 0000 7400 6a01  ...C...s@...t.j.
-00000300: a002 7c00 a101 731e 7403 7c00 6401 8302  ..|...s.t.|.d...
-00000310: 8f09 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
-00000320: 6400 5300 3100 7317 7701 0100 0100 0100  d.S.1.s.w.......
-00000330: 5900 0100 6400 5300 6400 5300 2902 4eda  Y...d.S.d.S.).N.
-00000340: 0177 2904 7205 0000 00da 0470 6174 68da  .w).r......path.
-00000350: 0669 7366 696c 65da 046f 7065 6e29 0172  .isfile..open).r
-00000360: 0e00 0000 720b 0000 0072 0b00 0000 720c  ....r....r....r.
-00000370: 0000 00da 0b63 7265 6174 655f 6669 6c65  .....create_file
-00000380: 1700 0000 730a 0000 000c 010c 0102 0122  ....s.........."
-00000390: ff04 ff72 1300 0000 6300 0000 0000 0000  ...r....c.......
-000003a0: 0000 0000 0002 0000 0003 0000 0047 0000  .............G..
-000003b0: 0073 1600 0000 7c00 4400 5d06 7d01 7400  .s....|.D.].}.t.
-000003c0: 7c01 8301 0100 7102 6400 5300 2901 4e29  |.....q.d.S.).N)
-000003d0: 0172 1300 0000 2902 da05 6669 6c65 7372  .r....)...filesr
-000003e0: 0e00 0000 720b 0000 0072 0b00 0000 720c  ....r....r....r.
-000003f0: 0000 00da 0c63 7265 6174 655f 6669 6c65  .....create_file
-00000400: 731c 0000 0073 0600 0000 0801 0a01 04ff  s....s..........
-00000410: 7215 0000 0029 1372 0500 0000 da07 7061  r....).r......pa
-00000420: 7468 6c69 62da 0450 6174 68da 0468 6f6d  thlib..Path..hom
-00000430: 655a 0968 6f6d 655f 7061 7468 7210 0000  eZ.home_pathr...
-00000440: 00da 046a 6f69 6e72 0700 0000 7208 0000  ...joinr....r...
-00000450: 005a 0d63 6f6e 6669 675f 666f 6c64 6572  .Z.config_folder
-00000460: 7209 0000 0072 0a00 0000 5a14 6175 7468  r....r....Z.auth
-00000470: 6f72 697a 6564 5f75 7365 725f 6669 6c65  orized_user_file
-00000480: da0f 7465 6d70 6c61 7465 5f63 6f6e 6669  ..template_confi
-00000490: 675a 0e61 6363 6f75 6e74 5f63 6f6e 6669  gZ.account_confi
-000004a0: 6772 0d00 0000 da03 7374 7272 1300 0000  gr......strr....
-000004b0: 7215 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
-000004c0: 0b00 0000 720c 0000 00da 083c 6d6f 6475  ....r......<modu
-000004d0: 6c65 3e01 0000 0073 1c00 0000 0800 0801  le>....s........
-000004e0: 0a02 1001 0e01 0e01 0e01 0e01 0e02 0e01  ................
-000004f0: 0e01 0803 0e07 0c05                      ........
+00000240: 0072 0b00 0000 fa69 433a 5c55 7365 7273  .r.....iC:\Users
+00000250: 5c79 6f6e 6773 6865 6e67 2e74 616e 5c44  \yongsheng.tan\D
+00000260: 6f63 756d 656e 7473 5c43 6f64 696e 675c  ocuments\Coding\
+00000270: 6769 7468 7562 2d70 726f 6a65 6374 5c6d  github-project\m
+00000280: 6169 6c63 6869 6d70 5f61 7574 6f5c 6d61  ailchimp_auto\ma
+00000290: 696c 6368 696d 705f 6175 746f 5c73 6372  ilchimp_auto\scr
+000002a0: 6970 7473 5c64 6972 6563 746f 7279 2e70  ipts\directory.p
+000002b0: 79da 0a63 7265 6174 655f 6469 7210 0000  y..create_dir...
+000002c0: 0073 0a00 0000 0001 0e01 0e01 0e01 0e01  .s..............
+000002d0: 720d 0000 00a9 01da 0466 696c 6563 0100  r........filec..
+000002e0: 0000 0000 0000 0000 0000 0100 0000 0800  ................
+000002f0: 0000 4300 0000 733a 0000 0074 006a 01a0  ..C...s:...t.j..
+00000300: 027c 00a1 0173 3674 037c 0064 0183 028f  .|...s6t.|.d....
+00000310: 1001 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
+00000320: 1031 0073 2c30 0001 0001 0001 0059 0001  .1.s,0.......Y..
+00000330: 0064 0053 0029 024e da01 7729 0472 0500  .d.S.).N..w).r..
+00000340: 0000 da04 7061 7468 da06 6973 6669 6c65  ....path..isfile
+00000350: da04 6f70 656e 720e 0000 0072 0b00 0000  ..openr....r....
+00000360: 720b 0000 0072 0c00 0000 da0b 6372 6561  r....r......crea
+00000370: 7465 5f66 696c 6517 0000 0073 0600 0000  te_file....s....
+00000380: 0001 0c01 0c01 7214 0000 0063 0000 0000  ......r....c....
+00000390: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+000003a0: 4700 0000 7316 0000 007c 0044 005d 0c7d  G...s....|.D.].}
+000003b0: 0174 007c 0183 0101 0071 0464 0053 0029  .t.|.....q.d.S.)
+000003c0: 014e 2901 7214 0000 0029 02da 0566 696c  .N).r....)...fil
+000003d0: 6573 720f 0000 0072 0b00 0000 720b 0000  esr....r....r...
+000003e0: 0072 0c00 0000 da0c 6372 6561 7465 5f66  .r......create_f
+000003f0: 696c 6573 1c00 0000 7304 0000 0000 0108  iles....s.......
+00000400: 0172 1600 0000 2913 7205 0000 00da 0770  .r....).r......p
+00000410: 6174 686c 6962 da04 5061 7468 da04 686f  athlib..Path..ho
+00000420: 6d65 5a09 686f 6d65 5f70 6174 6872 1100  meZ.home_pathr..
+00000430: 0000 da04 6a6f 696e 7207 0000 0072 0800  ....joinr....r..
+00000440: 0000 5a0d 636f 6e66 6967 5f66 6f6c 6465  ..Z.config_folde
+00000450: 7272 0900 0000 720a 0000 005a 1461 7574  rr....r....Z.aut
+00000460: 686f 7269 7a65 645f 7573 6572 5f66 696c  horized_user_fil
+00000470: 65da 0f74 656d 706c 6174 655f 636f 6e66  e..template_conf
+00000480: 6967 5a0e 6163 636f 756e 745f 636f 6e66  igZ.account_conf
+00000490: 6967 720d 0000 00da 0373 7472 7214 0000  igr......strr...
+000004a0: 0072 1600 0000 720b 0000 0072 0b00 0000  .r....r....r....
+000004b0: 720b 0000 0072 0c00 0000 da08 3c6d 6f64  r....r......<mod
+000004c0: 756c 653e 0100 0000 731a 0000 0008 0108  ule>....s.......
+000004d0: 020a 0110 010e 010e 010e 010e 020e 010e  ................
+000004e0: 010e 0308 070e 05                        .......
```

### Comparing `mailchimp_auto-0.1.0/mailchimp_auto/scripts/__pycache__/gspread_data.cpython-310.pyc` & `mailchimp_auto-0.1.1/mailchimp_auto/scripts/__pycache__/gspread_data.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 28 18:27:48 2022 UTC, .py size: 4990 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,266 +1,272 @@
-00000000: 6f0d 0d0a 0000 0000 24d5 e262 7e13 0000  o.......$..b~...
+00000000: 610d 0d0a 0000 0000 4c30 3064 8f11 0000  a.......L00d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
+00000020: 0003 0000 0040 0000 0073 8200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6401 6c04 5a05 6400  m.Z...d.d.l.Z.d.
 00000050: 6401 6c06 5a07 6400 6401 6c08 5a08 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c09 6d0a 5a0a 0100 6400 6404 6c0b  d.l.m.Z...d.d.l.
-00000070: 5400 6400 6401 6c0c 5a0c 650a 8300 5a0d  T.d.d.l.Z.e...Z.
-00000080: 650d a00e 650f a101 0100 4700 6405 6406  e...e.....G.d.d.
-00000090: 8400 6406 8302 5a10 6401 5300 2907 e900  ..d...Z.d.S.)...
-000000a0: 0000 004e 2902 da04 4469 6374 da05 556e  ...N)...Dict..Un
-000000b0: 696f 6e29 01da 0f52 6177 436f 6e66 6967  ion)...RawConfig
-000000c0: 5061 7273 6572 2901 da01 2a63 0000 0000  Parser)...*c....
-000000d0: 0000 0000 0000 0000 0000 0000 0800 0000  ................
-000000e0: 4000 0000 7368 0000 0065 005a 0164 005a  @...sh...e.Z.d.Z
-000000f0: 0264 1064 0265 0364 0365 0366 0464 0464  .d.d.e.d.e.f.d.d
-00000100: 0584 055a 0464 0664 0784 005a 0564 0865  ...Z.d.d...Z.d.e
-00000110: 0364 0965 0665 0365 0766 0219 0064 0a65  .d.e.e.e.f...d.e
-00000120: 0865 0365 0366 0219 0066 0664 0b64 0c84  .e.e.f...f.d.d..
-00000130: 045a 0964 0865 0364 0965 0665 0365 0766  .Z.d.e.d.e.e.e.f
-00000140: 0219 0066 0464 0d64 0e84 045a 0a64 0f53  ...f.d.d...Z.d.S
-00000150: 0029 11da 0e67 6574 4773 7072 6561 6444  .)...getGspreadD
-00000160: 6174 61da 00da 0e61 6363 6f75 6e74 5f63  ata....account_c
-00000170: 686f 6963 65da 0f74 656d 706c 6174 655f  hoice..template_
-00000180: 6368 6f69 6365 6303 0000 0000 0000 0000  choicec.........
-00000190: 0000 0003 0000 0005 0000 0043 0000 0073  ...........C...s
-000001a0: 2e00 0000 7c01 7c00 5f00 7c02 7c00 5f01  ....|.|._.|.|._.
-000001b0: 7402 6a03 7c00 6a01 6401 6402 6403 8d03  t.j.|.j.d.d.d...
-000001c0: 7c00 5f04 7c00 a005 a100 7c00 5f06 6402  |._.|.....|._.d.
-000001d0: 5300 2904 6147 0100 005f 7375 6d6d 6172  S.).aG..._summar
-000001e0: 795f 0a0a 2020 2020 2020 2020 4172 6773  y_..        Args
-000001f0: 3a0a 2020 2020 2020 2020 2020 2020 6372  :.            cr
-00000200: 6564 656e 7469 616c 7320 2864 6963 742c  edentials (dict,
-00000210: 206f 7074 696f 6e61 6c29 3a20 476f 6f67   optional): Goog
-00000220: 6c65 204f 6175 7468 322e 3020 4a53 4f4e  le Oauth2.0 JSON
-00000230: 2063 7265 6465 6e74 6961 6c73 2069 6e20   credentials in 
-00000240: 7079 7468 6f6e 2064 6963 7420 696e 7374  python dict inst
-00000250: 6561 6420 6f66 206f 7269 6769 6e61 6c20  ead of original 
-00000260: 6a73 6f6e 2066 6f72 6d61 742e 2044 6566  json format. Def
-00000270: 6175 6c74 7320 746f 2063 7265 6465 6e74  aults to credent
-00000280: 6961 6c73 2e0a 2020 2020 2020 2020 2020  ials..          
-00000290: 2020 7573 6572 5f61 7574 686f 7269 7a65    user_authorize
-000002a0: 6420 2864 6963 742c 206f 7074 696f 6e61  d (dict, optiona
-000002b0: 6c29 3a20 6175 7468 6f72 697a 6564 2075  l): authorized u
-000002c0: 7365 7227 7320 636c 6965 6e74 2069 642c  ser's client id,
-000002d0: 2063 6c69 656e 7420 7365 6372 6574 2c20   client secret, 
-000002e0: 6574 6320 696e 2070 7974 686f 6e20 6469  etc in python di
-000002f0: 6374 2066 6f72 6d61 742e 2044 6566 6175  ct format. Defau
-00000300: 6c74 7320 746f 2075 7365 725f 6175 7468  lts to user_auth
-00000310: 6f72 697a 6564 2e0a 2020 2020 2020 2020  orized..        
-00000320: da0f 7370 7265 6164 7368 6565 745f 7572  ..spreadsheet_ur
-00000330: 6c4e a901 da08 6661 6c6c 6261 636b 2907  lN....fallback).
-00000340: 7208 0000 0072 0900 0000 da06 636f 6e66  r....r......conf
-00000350: 6967 da03 6765 7472 0a00 0000 da12 6163  ig..getr......ac
-00000360: 6365 7373 5f73 7072 6561 6473 6865 6574  cess_spreadsheet
-00000370: da05 7368 6565 7429 03da 0473 656c 6672  ..sheet)...selfr
-00000380: 0800 0000 7209 0000 00a9 0072 1200 0000  ....r......r....
-00000390: fa6f 433a 5c55 7365 7273 5c74 7973 5c44  .oC:\Users\tys\D
-000003a0: 6f63 756d 656e 7473 5c50 726f 6a65 6374  ocuments\Project
-000003b0: 5c6d 6169 6c63 6869 6d70 5f63 7265 6174  \mailchimp_creat
-000003c0: 696f 6e5f 7072 6f6a 6563 745c 6d61 696c  ion_project\mail
-000003d0: 6368 696d 702d 6175 746f 5c6d 6169 6c63  chimp-auto\mailc
-000003e0: 6869 6d70 5f61 7574 6f5c 7363 7269 7074  himp_auto\script
-000003f0: 735c 6773 7072 6561 645f 6461 7461 2e70  s\gspread_data.p
-00000400: 79da 085f 5f69 6e69 745f 5f0e 0000 0073  y..__init__....s
-00000410: 0800 0000 0608 0601 1401 0e01 7a17 6765  ............z.ge
-00000420: 7447 7370 7265 6164 4461 7461 2e5f 5f69  tGspreadData.__i
-00000430: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
-00000440: 0000 0500 0000 0a00 0000 4300 0000 7396  ..........C...s.
-00000450: 0000 0074 0083 007d 017c 01a0 0174 02a1  ...t...}.|...t..
-00000460: 0101 007c 016a 037c 006a 0464 0164 0064  ...|.j.|.j.d.d.d
-00000470: 028d 037d 027a 1074 056a 067c 0264 038d  ...}.z.t.j.|.d..
-00000480: 017c 005f 077c 006a 07a0 087c 006a 09a1  .|._.|.j...|.j..
-00000490: 017d 0357 006e 1d04 0074 056a 0a6a 0b79  .}.W.n...t.j.j.y
-000004a0: 3e01 007d 0401 007a 0f74 0c7c 049b 0083  >..}...z.t.|....
-000004b0: 0101 0074 0c64 0483 0101 0057 0059 0064  ...t.d.....W.Y.d
-000004c0: 007d 047e 046e 0564 007d 047e 0477 0177  .}.~.n.d.}.~.w.w
-000004d0: 0074 0da0 0e64 0574 0f7c 0383 019b 009d  .t...d.t.|......
-000004e0: 02a1 0101 007c 0353 0029 064e da19 7365  .....|.S.).N..se
-000004f0: 7276 6963 655f 6163 636f 756e 745f 6669  rvice_account_fi
-00000500: 6c65 5f70 6174 6872 0b00 0000 2901 da08  le_pathr....)...
-00000510: 6669 6c65 6e61 6d65 7a4d 506c 6561 7365  filenamezMPlease
-00000520: 2063 686f 6f73 6520 7468 6520 476f 6f67   choose the Goog
-00000530: 6c65 2061 6363 6f75 6e74 2074 6861 7420  le account that 
-00000540: 6861 7320 7065 726d 6973 7369 6f6e 2074  has permission t
-00000550: 6f20 6f70 656e 2074 6865 2073 7072 6561  o open the sprea
-00000560: 6473 6865 6574 217a 1a54 6865 2074 7970  dsheet!z.The typ
-00000570: 6520 6f66 2073 6865 6574 206f 626a 6563  e of sheet objec
-00000580: 743a 2029 1072 0400 0000 da04 7265 6164  t: ).r......read
-00000590: 5a0e 6163 636f 756e 745f 636f 6e66 6967  Z.account_config
-000005a0: 720e 0000 0072 0800 0000 da07 6773 7072  r....r......gspr
-000005b0: 6561 645a 0f73 6572 7669 6365 5f61 6363  eadZ.service_acc
-000005c0: 6f75 6e74 da02 6763 5a0b 6f70 656e 5f62  ount..gcZ.open_b
-000005d0: 795f 7572 6c72 0a00 0000 da0a 6578 6365  y_urlr......exce
-000005e0: 7074 696f 6e73 5a08 4150 4945 7272 6f72  ptionsZ.APIError
-000005f0: da05 7072 696e 74da 076c 6f67 6769 6e67  ..print..logging
-00000600: da05 6465 6275 67da 0474 7970 6529 0572  ..debug..type).r
-00000610: 1100 0000 5a0a 7470 6c5f 636f 6e66 6967  ....Z.tpl_config
-00000620: 7215 0000 0072 1000 0000 da05 6572 726f  r....r......erro
-00000630: 7272 1200 0000 7212 0000 0072 1300 0000  rr....r....r....
-00000640: 720f 0000 0020 0000 0073 1a00 0000 0601  r.... ...s......
-00000650: 0a01 1201 0203 0e02 1203 1201 0a01 1401  ................
-00000660: 0880 02fe 1406 0401 7a21 6765 7447 7370  ........z!getGsp
-00000670: 7265 6164 4461 7461 2e61 6363 6573 735f  readData.access_
-00000680: 7370 7265 6164 7368 6565 74da 0f77 6f72  spreadsheet..wor
-00000690: 6b73 6865 6574 5f74 6974 6c65 da14 6d75  ksheet_title..mu
-000006a0: 6c74 6970 6c65 5f63 656c 6c5f 7261 6e67  ltiple_cell_rang
-000006b0: 6573 da06 7265 7475 726e 6303 0000 0000  es..returnc.....
-000006c0: 0000 0000 0000 0009 0000 0009 0000 0043  ...............C
-000006d0: 0000 0073 9c00 0000 6401 6401 6401 6401  ...s....d.d.d.d.
-000006e0: 6401 6402 9c05 7d03 6403 6404 8400 7400  d.d...}.d.d...t.
-000006f0: 7c02 8301 a001 7400 a002 7c03 a101 a101  |.....t...|.....
-00000700: a003 6405 a101 4400 8301 7d02 7c00 6a04  ..d...D...}.|.j.
-00000710: a005 7c01 a101 7d04 6700 7d05 6900 7d06  ..|...}.g.}.i.}.
-00000720: 7c02 4400 5d0a 7d07 7c05 a006 7c04 a007  |.D.].}.|...|...
-00000730: 7c07 a101 a101 0100 7126 7c05 4400 5d18  |.......q&|.D.].
-00000740: 7d08 7a0d 7c06 a008 7c08 6406 1900 7c08  }.z.|...|.d...|.
-00000750: 6407 1900 6901 a101 0100 5700 7133 0400  d...i.....W.q3..
-00000760: 7409 794b 0100 0100 0100 5900 7133 7700  t.yK......Y.q3w.
-00000770: 7c06 5300 2908 615a 0200 005f 7375 6d6d  |.S.).aZ..._summ
-00000780: 6172 795f 0a0a 2020 2020 2020 2020 4172  ary_..        Ar
-00000790: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-000007a0: 776f 726b 7368 6565 745f 7469 746c 6520  worksheet_title 
-000007b0: 2873 7472 293a 2047 6f6f 676c 6520 7370  (str): Google sp
-000007c0: 7265 6164 7368 6565 7420 776f 726b 7368  readsheet worksh
-000007d0: 6565 7420 7469 746c 650a 2020 2020 2020  eet title.      
-000007e0: 2020 2020 2020 6d75 6c74 6970 6c65 5f63        multiple_c
-000007f0: 656c 6c5f 7261 6e67 6573 2028 4c69 7374  ell_ranges (List
-00000800: 5b73 7472 5d29 3a20 496e 7075 7420 476f  [str]): Input Go
-00000810: 6f67 6c65 2073 7072 6561 6473 6865 6574  ogle spreadsheet
-00000820: 2773 206d 756c 7469 706c 6520 6365 6c6c  's multiple cell
-00000830: 2072 616e 6765 7320 6f66 2032 200a 2020   ranges of 2 .  
-00000840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000860: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
-00000870: 7320 2864 696d 656e 7369 6f6e 3a20 6920  s (dimension: i 
-00000880: 7820 3229 2069 6e20 6c69 7374 2c20 652e  x 2) in list, e.
-00000890: 672e 2c20 5b22 4131 3a42 3622 2c20 2241  g., ["A1:B6", "A
-000008a0: 383a 4239 222c 200a 2020 2020 2020 2020  8:B9", .        
-000008b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008d0: 2020 2020 2241 3131 3a42 3131 225d 0a20      "A11:B11"]. 
-000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000900: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-00000910: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00000920: 2020 2020 2020 2020 2044 6963 745b 7374           Dict[st
-00000930: 722c 2073 7472 5d3a 2072 6574 7572 6e73  r, str]: returns
-00000940: 2074 6865 2064 6963 7420 6b65 7920 7661   the dict key va
-00000950: 6c75 6520 7061 6972 2077 6865 7265 6279  lue pair whereby
-00000960: 2074 6865 206b 6579 2069 7320 7468 6520   the key is the 
-00000970: 6669 7273 7420 636f 6c75 6d6e 206f 6620  first column of 
-00000980: 0a20 2020 2020 2020 2020 2020 2061 7267  .            arg
-00000990: 733a 206d 756c 7469 706c 655f 6365 6c6c  s: multiple_cell
-000009a0: 5f72 616e 6765 7320 616e 6420 7468 6520  _ranges and the 
-000009b0: 7661 6c75 6520 6973 2069 7473 2073 6563  value is its sec
-000009c0: 6f6e 6420 636f 6c75 6d6e 2e20 0a20 2020  ond column. .   
-000009d0: 2020 2020 2072 0700 0000 a905 fa01 22fa       r........".
-000009e0: 0127 fa01 20fa 015b fa01 5d63 0100 0000  .'.. ..[..]c....
-000009f0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00000a00: 5300 0000 f310 0000 0067 007c 005d 047d  S........g.|.].}
-00000a10: 017c 0191 0271 0253 0072 1200 0000 7212  .|...q.S.r....r.
-00000a20: 0000 00a9 02da 022e 30da 0178 7212 0000  ........0..xr...
-00000a30: 0072 1200 0000 7213 0000 00da 0a3c 6c69  .r....r......<li
-00000a40: 7374 636f 6d70 3e44 0000 00f3 0200 0000  stcomp>D........
-00000a50: 1000 7a34 6765 7447 7370 7265 6164 4461  ..z4getGspreadDa
-00000a60: 7461 2e67 6574 5f63 616d 7061 6967 6e5f  ta.get_campaign_
-00000a70: 696e 666f 2e3c 6c6f 6361 6c73 3e2e 3c6c  info.<locals>.<l
-00000a80: 6973 7463 6f6d 703e fa01 2c72 0100 0000  istcomp>..,r....
-00000a90: e901 0000 0029 0ada 0373 7472 da09 7472  .....)...str..tr
-00000aa0: 616e 736c 6174 65da 096d 616b 6574 7261  anslate..maketra
-00000ab0: 6e73 da05 7370 6c69 7472 1000 0000 da09  ns..splitr......
-00000ac0: 776f 726b 7368 6565 74da 0665 7874 656e  worksheet..exten
-00000ad0: 6472 0e00 0000 da06 7570 6461 7465 da0a  dr......update..
-00000ae0: 496e 6465 7845 7272 6f72 2909 7211 0000  IndexError).r...
-00000af0: 0072 2000 0000 7221 0000 00da 0f63 6861  .r ...r!.....cha
-00000b00: 725f 746f 5f72 6570 6c61 6365 5a12 776f  r_to_replaceZ.wo
-00000b10: 726b 7368 6565 745f 6361 6d70 6169 676e  rksheet_campaign
-00000b20: 5a12 6361 6d70 6169 676e 5f69 6e66 6f5f  Z.campaign_info_
-00000b30: 6c69 7374 5a12 6361 6d70 6169 676e 5f69  listZ.campaign_i
-00000b40: 6e66 6f5f 6469 6374 5a0a 6365 6c6c 5f72  nfo_dictZ.cell_r
-00000b50: 616e 6765 da05 696e 6465 7872 1200 0000  ange..indexr....
-00000b60: 7212 0000 0072 1300 0000 da11 6765 745f  r....r......get_
-00000b70: 6361 6d70 6169 676e 5f69 6e66 6f35 0000  campaign_info5..
-00000b80: 0073 1c00 0000 100e 2401 0c02 0401 0401  .s......$.......
-00000b90: 0802 1201 0801 0201 1a01 0c01 0401 02ff  ................
-00000ba0: 0402 7a20 6765 7447 7370 7265 6164 4461  ..z getGspreadDa
-00000bb0: 7461 2e67 6574 5f63 616d 7061 6967 6e5f  ta.get_campaign_
-00000bc0: 696e 666f 6303 0000 0000 0000 0000 0000  infoc...........
-00000bd0: 000c 0000 0006 0000 0043 0000 0073 fc00  .........C...s..
-00000be0: 0000 7400 7c02 8301 6401 6b02 721e 6402  ..t.|...d.k.r.d.
-00000bf0: 6402 6402 6402 6402 6403 9c05 7d03 6404  d.d.d.d.d...}.d.
-00000c00: 6405 8400 7c02 a001 7402 a003 7c03 a101  d...|...t...|...
-00000c10: a101 a004 6406 a101 4400 8301 7d02 7c00  ....d...D...}.|.
-00000c20: 6a05 a006 7c01 a101 7d04 7407 8300 7d05  j...|...}.t...}.
-00000c30: 7c04 a008 7c02 a101 7d06 7409 6407 740a  |...|...}.t.d.t.
-00000c40: 7c06 8301 6408 8303 4400 5d47 7d07 7c06  |...d...D.]G}.|.
-00000c50: 7c07 1900 a00b 6407 a101 7d08 7c05 a00c  |.....d...}.|...
-00000c60: 7c08 6407 1900 6900 6901 a101 0100 740d  |.d...i.i.....t.
-00000c70: 6a0e a00f 7c06 7c07 1900 a101 7d09 7c09  j...|.|.....}.|.
-00000c80: 6a10 6407 1900 7d0a 740d 6a0e 7c09 6a11  j.d...}.t.j.|.j.
-00000c90: 6408 6400 8502 1900 7c0a 6409 8d02 7d0b  d.d.....|.d...}.
-00000ca0: 7c0b 6a12 6402 7413 6a14 640a 640b 8d03  |.j.d.t.j.d.d...
-00000cb0: 0100 7c0b 6a15 6407 640c 640a 640d 8d03  ..|.j.d.d.d.d...
-00000cc0: 0100 7c05 7c08 6407 1900 1900 a00c 7c0b  ..|.|.d.......|.
-00000cd0: a016 a100 a101 0100 7134 7c05 5300 290e  ........q4|.S.).
-00000ce0: 4e72 3100 0000 7207 0000 0072 2300 0000  Nr1...r....r#...
-00000cf0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000d00: 0003 0000 0053 0000 0072 2900 0000 7212  .....S...r)...r.
-00000d10: 0000 0072 1200 0000 722a 0000 0072 1200  ...r....r*...r..
-00000d20: 0000 7212 0000 0072 1300 0000 722d 0000  ..r....r....r-..
-00000d30: 0056 0000 0072 2e00 0000 7a33 6765 7447  .V...r....z3getG
-00000d40: 7370 7265 6164 4461 7461 2e67 6574 5f63  spreadData.get_c
-00000d50: 6f6e 7465 6e74 5f69 6e66 6f2e 3c6c 6f63  ontent_info.<loc
-00000d60: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
-00000d70: 2f00 0000 7201 0000 0072 3000 0000 2901  /...r....r0...).
-00000d80: da07 636f 6c75 6d6e 7354 2901 da07 696e  ..columnsT)...in
-00000d90: 706c 6163 65da 0361 6e79 2903 5a04 6178  place..any).Z.ax
-00000da0: 6973 da03 686f 7772 3d00 0000 2917 721e  is..howr=...).r.
-00000db0: 0000 0072 3200 0000 7231 0000 0072 3300  ...r2...r1...r3.
-00000dc0: 0000 7234 0000 0072 1000 0000 7235 0000  ..r4...r....r5..
-00000dd0: 00da 0464 6963 745a 0962 6174 6368 5f67  ...dictZ.batch_g
-00000de0: 6574 da05 7261 6e67 65da 036c 656e da03  et..range..len..
-00000df0: 706f 7072 3700 0000 da02 7064 5a09 4461  popr7.....pdZ.Da
-00000e00: 7461 4672 616d 655a 0c66 726f 6d5f 7265  taFrameZ.from_re
-00000e10: 636f 7264 735a 0469 6c6f 63da 0676 616c  cordsZ.iloc..val
-00000e20: 7565 73da 0772 6570 6c61 6365 da02 6e70  ues..replace..np
-00000e30: da03 6e61 6e5a 0664 726f 706e 615a 0774  ..nanZ.dropnaZ.t
-00000e40: 6f5f 6469 6374 290c 7211 0000 0072 2000  o_dict).r....r .
-00000e50: 0000 7221 0000 0072 3900 0000 5a16 776f  ..r!...r9...Z.wo
-00000e60: 726b 7368 6565 745f 636f 6e74 656e 745f  rksheet_content_
-00000e70: 696e 666f 5a11 636f 6e74 656e 745f 696e  infoZ.content_in
-00000e80: 666f 5f64 6963 745a 1163 6f6e 7465 6e74  fo_dictZ.content
-00000e90: 5f69 6e66 6f5f 6c69 7374 723a 0000 00da  _info_listr:....
-00000ea0: 0c73 6563 7469 6f6e 5f6e 616d 65da 0264  .section_name..d
-00000eb0: 66da 0a68 6561 6465 725f 726f 775a 0e64  f..header_rowZ.d
-00000ec0: 665f 7769 7468 5f68 6561 6465 7272 1200  f_with_headerr..
-00000ed0: 0000 7212 0000 0072 1300 0000 da10 6765  ..r....r......ge
-00000ee0: 745f 636f 6e74 656e 745f 696e 666f 5300  t_content_infoS.
-00000ef0: 0000 7320 0000 000c 0110 0120 010c 0206  ..s ....... ....
-00000f00: 010a 0114 020e 0112 0110 010a 0118 0112  ................
-00000f10: 0110 0118 0104 017a 1f67 6574 4773 7072  .......z.getGspr
-00000f20: 6561 6444 6174 612e 6765 745f 636f 6e74  eadData.get_cont
-00000f30: 656e 745f 696e 666f 4e29 0272 0700 0000  ent_infoN).r....
-00000f40: 7207 0000 0029 0bda 085f 5f6e 616d 655f  r....)...__name_
-00000f50: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000f60: 5f71 7561 6c6e 616d 655f 5f72 3100 0000  _qualname__r1...
-00000f70: 7214 0000 0072 0f00 0000 7203 0000 00da  r....r....r.....
-00000f80: 046c 6973 7472 0200 0000 723b 0000 0072  .listr....r;...r
-00000f90: 4c00 0000 7212 0000 0072 1200 0000 7212  L...r....r....r.
-00000fa0: 0000 0072 1300 0000 7206 0000 000d 0000  ...r....r.......
-00000fb0: 0073 0a00 0000 0800 1401 0812 2615 1e1e  .s..........&...
-00000fc0: 7206 0000 0029 1172 1800 0000 da06 7479  r....).r......ty
-00000fd0: 7069 6e67 7202 0000 0072 0300 0000 5a06  pingr....r....Z.
-00000fe0: 7061 6e64 6173 7244 0000 00da 056e 756d  pandasrD.....num
-00000ff0: 7079 7247 0000 00da 026f 73da 0c63 6f6e  pyrG.....os..con
-00001000: 6669 6770 6172 7365 7272 0400 0000 da20  figparserr..... 
-00001010: 6d61 696c 6368 696d 705f 6175 746f 2e73  mailchimp_auto.s
-00001020: 6372 6970 7473 2e64 6972 6563 746f 7279  cripts.directory
-00001030: 721c 0000 0072 0d00 0000 7217 0000 00da  r....r....r.....
-00001040: 0f74 656d 706c 6174 655f 636f 6e66 6967  .template_config
-00001050: 7206 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-00001060: 1200 0000 7213 0000 00da 083c 6d6f 6475  ....r......<modu
-00001070: 6c65 3e01 0000 0073 1600 0000 0800 1001  le>....s........
-00001080: 0801 0801 0801 0c01 0801 0801 0602 0a01  ................
-00001090: 1202                                     ..
+00000070: 5400 6400 6401 6c0c 5a0c 6400 6401 6c0d  T.d.d.l.Z.d.d.l.
+00000080: 5a0d 6400 6405 6c0e 6d0f 5a0f 0100 650a  Z.d.d.l.m.Z...e.
+00000090: 8300 5a10 6510 a011 6512 a101 0100 4700  ..Z.e...e.....G.
+000000a0: 6406 6407 8400 6407 8302 5a13 6401 5300  d.d...d...Z.d.S.
+000000b0: 2908 e900 0000 004e 2902 da04 4469 6374  )......N)...Dict
+000000c0: da05 556e 696f 6e29 01da 0f52 6177 436f  ..Union)...RawCo
+000000d0: 6e66 6967 5061 7273 6572 2901 da01 2a29  nfigParser)...*)
+000000e0: 01da 0c75 706c 6f61 645f 696d 6167 6563  ...upload_imagec
+000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000100: 0500 0000 4000 0000 7360 0000 0065 005a  ....@...s`...e.Z
+00000110: 0164 005a 0264 0e65 0365 0364 029c 0264  .d.Z.d.e.e.d...d
+00000120: 0364 0484 055a 0464 0564 0684 005a 0565  .d...Z.d.d...Z.e
+00000130: 0365 0665 0365 0766 0219 0065 0865 0365  .e.e.e.f...e.e.e
+00000140: 0366 0219 0064 079c 0364 0864 0984 045a  .f...d...d.d...Z
+00000150: 0965 0365 0665 0365 0766 0219 0064 0a9c  .e.e.e.e.f...d..
+00000160: 0264 0b64 0c84 045a 0a64 0d53 0029 0fda  .d.d...Z.d.S.)..
+00000170: 0e67 6574 4773 7072 6561 6444 6174 61da  .getGspreadData.
+00000180: 0029 02da 0e61 6363 6f75 6e74 5f63 686f  .)...account_cho
+00000190: 6963 65da 0f74 656d 706c 6174 655f 6368  ice..template_ch
+000001a0: 6f69 6365 6303 0000 0000 0000 0000 0000  oicec...........
+000001b0: 0003 0000 0005 0000 0043 0000 0073 2e00  .........C...s..
+000001c0: 0000 7c01 7c00 5f00 7c02 7c00 5f01 7402  ..|.|._.|.|._.t.
+000001d0: 6a03 7c00 6a01 6401 6402 6403 8d03 7c00  j.|.j.d.d.d...|.
+000001e0: 5f04 7c00 a005 a100 7c00 5f06 6402 5300  _.|.....|._.d.S.
+000001f0: 2904 6147 0100 005f 7375 6d6d 6172 795f  ).aG..._summary_
+00000200: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00000210: 2020 2020 2020 2020 2020 2020 6372 6564              cred
+00000220: 656e 7469 616c 7320 2864 6963 742c 206f  entials (dict, o
+00000230: 7074 696f 6e61 6c29 3a20 476f 6f67 6c65  ptional): Google
+00000240: 204f 6175 7468 322e 3020 4a53 4f4e 2063   Oauth2.0 JSON c
+00000250: 7265 6465 6e74 6961 6c73 2069 6e20 7079  redentials in py
+00000260: 7468 6f6e 2064 6963 7420 696e 7374 6561  thon dict instea
+00000270: 6420 6f66 206f 7269 6769 6e61 6c20 6a73  d of original js
+00000280: 6f6e 2066 6f72 6d61 742e 2044 6566 6175  on format. Defau
+00000290: 6c74 7320 746f 2063 7265 6465 6e74 6961  lts to credentia
+000002a0: 6c73 2e0a 2020 2020 2020 2020 2020 2020  ls..            
+000002b0: 7573 6572 5f61 7574 686f 7269 7a65 6420  user_authorized 
+000002c0: 2864 6963 742c 206f 7074 696f 6e61 6c29  (dict, optional)
+000002d0: 3a20 6175 7468 6f72 697a 6564 2075 7365  : authorized use
+000002e0: 7227 7320 636c 6965 6e74 2069 642c 2063  r's client id, c
+000002f0: 6c69 656e 7420 7365 6372 6574 2c20 6574  lient secret, et
+00000300: 6320 696e 2070 7974 686f 6e20 6469 6374  c in python dict
+00000310: 2066 6f72 6d61 742e 2044 6566 6175 6c74   format. Default
+00000320: 7320 746f 2075 7365 725f 6175 7468 6f72  s to user_author
+00000330: 697a 6564 2e0a 2020 2020 2020 2020 da0f  ized..        ..
+00000340: 7370 7265 6164 7368 6565 745f 7572 6c4e  spreadsheet_urlN
+00000350: a901 da08 6661 6c6c 6261 636b 2907 7209  ....fallback).r.
+00000360: 0000 0072 0a00 0000 da06 636f 6e66 6967  ...r......config
+00000370: da03 6765 7472 0b00 0000 da12 6163 6365  ..getr......acce
+00000380: 7373 5f73 7072 6561 6473 6865 6574 da05  ss_spreadsheet..
+00000390: 7368 6565 7429 03da 0473 656c 6672 0900  sheet)...selfr..
+000003a0: 0000 720a 0000 00a9 0072 1300 0000 fa6c  ..r......r.....l
+000003b0: 433a 5c55 7365 7273 5c79 6f6e 6773 6865  C:\Users\yongshe
+000003c0: 6e67 2e74 616e 5c44 6f63 756d 656e 7473  ng.tan\Documents
+000003d0: 5c43 6f64 696e 675c 6769 7468 7562 2d70  \Coding\github-p
+000003e0: 726f 6a65 6374 5c6d 6169 6c63 6869 6d70  roject\mailchimp
+000003f0: 5f61 7574 6f5c 6d61 696c 6368 696d 705f  _auto\mailchimp_
+00000400: 6175 746f 5c73 6372 6970 7473 5c67 7370  auto\scripts\gsp
+00000410: 7265 6164 5f64 6174 612e 7079 da08 5f5f  read_data.py..__
+00000420: 696e 6974 5f5f 1000 0000 7308 0000 0000  init__....s.....
+00000430: 0706 0106 0114 017a 1767 6574 4773 7072  .......z.getGspr
+00000440: 6561 6444 6174 612e 5f5f 696e 6974 5f5f  eadData.__init__
+00000450: 6301 0000 0000 0000 0000 0000 0005 0000  c...............
+00000460: 000a 0000 0043 0000 0073 9600 0000 7400  .....C...s....t.
+00000470: 8300 7d01 7c01 a001 7402 a101 0100 7c01  ..}.|...t.....|.
+00000480: 6a03 7c00 6a04 6401 6400 6402 8d03 7d02  j.|.j.d.d.d...}.
+00000490: 7a20 7405 6a06 7c02 6403 8d01 7c00 5f07  z t.j.|.d...|._.
+000004a0: 7c00 6a07 a008 7c00 6a09 a101 7d03 5700  |.j...|.j...}.W.
+000004b0: 6e3a 0400 7405 6a0a 6a0b 797c 0100 7d04  n:..t.j.j.y|..}.
+000004c0: 0100 7a1e 740c 7c04 9b00 8301 0100 740c  ..z.t.|.......t.
+000004d0: 6404 8301 0100 5700 5900 6400 7d04 7e04  d.....W.Y.d.}.~.
+000004e0: 6e0a 6400 7d04 7e04 3000 3000 740d a00e  n.d.}.~.0.0.t...
+000004f0: 6405 740f 7c03 8301 9b00 9d02 a101 0100  d.t.|...........
+00000500: 7c03 5300 2906 4eda 1973 6572 7669 6365  |.S.).N..service
+00000510: 5f61 6363 6f75 6e74 5f66 696c 655f 7061  _account_file_pa
+00000520: 7468 720c 0000 0029 01da 0866 696c 656e  thr....)...filen
+00000530: 616d 657a 4d50 6c65 6173 6520 6368 6f6f  amezMPlease choo
+00000540: 7365 2074 6865 2047 6f6f 676c 6520 6163  se the Google ac
+00000550: 636f 756e 7420 7468 6174 2068 6173 2070  count that has p
+00000560: 6572 6d69 7373 696f 6e20 746f 206f 7065  ermission to ope
+00000570: 6e20 7468 6520 7370 7265 6164 7368 6565  n the spreadshee
+00000580: 7421 7a1a 5468 6520 7479 7065 206f 6620  t!z.The type of 
+00000590: 7368 6565 7420 6f62 6a65 6374 3a20 2910  sheet object: ).
+000005a0: 7204 0000 00da 0472 6561 64da 0e61 6363  r......read..acc
+000005b0: 6f75 6e74 5f63 6f6e 6669 6772 0f00 0000  ount_configr....
+000005c0: 7209 0000 00da 0767 7370 7265 6164 5a0f  r......gspreadZ.
+000005d0: 7365 7276 6963 655f 6163 636f 756e 74da  service_account.
+000005e0: 0267 635a 0b6f 7065 6e5f 6279 5f75 726c  .gcZ.open_by_url
+000005f0: 720b 0000 00da 0a65 7863 6570 7469 6f6e  r......exception
+00000600: 735a 0841 5049 4572 726f 72da 0570 7269  sZ.APIError..pri
+00000610: 6e74 da07 6c6f 6767 696e 67da 0564 6562  nt..logging..deb
+00000620: 7567 da04 7479 7065 2905 7212 0000 005a  ug..type).r....Z
+00000630: 0a74 706c 5f63 6f6e 6669 6772 1600 0000  .tpl_configr....
+00000640: 7211 0000 00da 0565 7272 6f72 7213 0000  r......errorr...
+00000650: 0072 1300 0000 7214 0000 0072 1000 0000  .r....r....r....
+00000660: 1c00 0000 7316 0000 0000 0106 010a 0112  ....s...........
+00000670: 0202 010e 0112 0112 010a 011e 0114 017a  ...............z
+00000680: 2167 6574 4773 7072 6561 6444 6174 612e  !getGspreadData.
+00000690: 6163 6365 7373 5f73 7072 6561 6473 6865  access_spreadshe
+000006a0: 6574 2903 da0f 776f 726b 7368 6565 745f  et)...worksheet_
+000006b0: 7469 746c 65da 146d 756c 7469 706c 655f  title..multiple_
+000006c0: 6365 6c6c 5f72 616e 6765 73da 0672 6574  cell_ranges..ret
+000006d0: 7572 6e63 0300 0000 0000 0000 0000 0000  urnc............
+000006e0: 0900 0000 0900 0000 4300 0000 739e 0000  ........C...s...
+000006f0: 0064 0164 0164 0164 0164 0164 029c 057d  .d.d.d.d.d.d...}
+00000700: 0364 0364 0484 0074 007c 0283 01a0 0174  .d.d...t.|.....t
+00000710: 00a0 027c 03a1 01a1 01a0 0364 05a1 0144  ...|.......d...D
+00000720: 0083 017d 027c 006a 04a0 057c 01a1 017d  ...}.|.j...|...}
+00000730: 0467 007d 0569 007d 067c 0244 005d 147d  .g.}.i.}.|.D.].}
+00000740: 077c 05a0 067c 04a0 077c 07a1 01a1 0101  .|...|...|......
+00000750: 0071 4c7c 0544 005d 327d 087a 1a7c 06a0  .qL|.D.]2}.z.|..
+00000760: 087c 0864 0619 007c 0864 0719 0069 01a1  .|.d...|.d...i..
+00000770: 0101 0057 0071 6604 0074 0979 9601 0001  ...W.qf..t.y....
+00000780: 0001 0059 0071 6630 0071 667c 0653 0029  ...Y.qf0.qf|.S.)
+00000790: 0861 5a02 0000 5f73 756d 6d61 7279 5f0a  .aZ..._summary_.
+000007a0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+000007b0: 2020 2020 2020 2020 2020 2077 6f72 6b73             works
+000007c0: 6865 6574 5f74 6974 6c65 2028 7374 7229  heet_title (str)
+000007d0: 3a20 476f 6f67 6c65 2073 7072 6561 6473  : Google spreads
+000007e0: 6865 6574 2077 6f72 6b73 6865 6574 2074  heet worksheet t
+000007f0: 6974 6c65 0a20 2020 2020 2020 2020 2020  itle.           
+00000800: 206d 756c 7469 706c 655f 6365 6c6c 5f72   multiple_cell_r
+00000810: 616e 6765 7320 284c 6973 745b 7374 725d  anges (List[str]
+00000820: 293a 2049 6e70 7574 2047 6f6f 676c 6520  ): Input Google 
+00000830: 7370 7265 6164 7368 6565 7427 7320 6d75  spreadsheet's mu
+00000840: 6c74 6970 6c65 2063 656c 6c20 7261 6e67  ltiple cell rang
+00000850: 6573 206f 6620 3220 0a20 2020 2020 2020  es of 2 .       
+00000860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000880: 2020 2020 2063 6f6c 756d 6e73 2028 6469       columns (di
+00000890: 6d65 6e73 696f 6e3a 2069 2078 2032 2920  mension: i x 2) 
+000008a0: 696e 206c 6973 742c 2065 2e67 2e2c 205b  in list, e.g., [
+000008b0: 2241 313a 4236 222c 2022 4138 3a42 3922  "A1:B6", "A8:B9"
+000008c0: 2c20 0a20 2020 2020 2020 2020 2020 2020  , .             
+000008d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000008f0: 4131 313a 4231 3122 5d0a 2020 2020 2020  A11:B11"].      
+00000900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000920: 2020 2020 2020 0a20 2020 2020 2020 2052        .        R
+00000930: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00000940: 2020 2020 4469 6374 5b73 7472 2c20 7374      Dict[str, st
+00000950: 725d 3a20 7265 7475 726e 7320 7468 6520  r]: returns the 
+00000960: 6469 6374 206b 6579 2076 616c 7565 2070  dict key value p
+00000970: 6169 7220 7768 6572 6562 7920 7468 6520  air whereby the 
+00000980: 6b65 7920 6973 2074 6865 2066 6972 7374  key is the first
+00000990: 2063 6f6c 756d 6e20 6f66 200a 2020 2020   column of .    
+000009a0: 2020 2020 2020 2020 6172 6773 3a20 6d75          args: mu
+000009b0: 6c74 6970 6c65 5f63 656c 6c5f 7261 6e67  ltiple_cell_rang
+000009c0: 6573 2061 6e64 2074 6865 2076 616c 7565  es and the value
+000009d0: 2069 7320 6974 7320 7365 636f 6e64 2063   is its second c
+000009e0: 6f6c 756d 6e2e 200a 2020 2020 2020 2020  olumn. .        
+000009f0: 7208 0000 00a9 05fa 0122 fa01 27fa 0120  r........"..'.. 
+00000a00: fa01 5bfa 015d 6301 0000 0000 0000 0000  ..[..]c.........
+00000a10: 0000 0002 0000 0003 0000 0053 0000 0073  ...........S...s
+00000a20: 1000 0000 6700 7c00 5d08 7d01 7c01 9102  ....g.|.].}.|...
+00000a30: 7104 5300 7213 0000 0072 1300 0000 a902  q.S.r....r......
+00000a40: da02 2e30 da01 7872 1300 0000 7213 0000  ...0..xr....r...
+00000a50: 0072 1400 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
+00000a60: 703e 3900 0000 f300 0000 007a 3467 6574  p>9........z4get
+00000a70: 4773 7072 6561 6444 6174 612e 6765 745f  GspreadData.get_
+00000a80: 6361 6d70 6169 676e 5f69 6e66 6f2e 3c6c  campaign_info.<l
+00000a90: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00000aa0: 3efa 012c 7201 0000 00e9 0100 0000 290a  >..,r.........).
+00000ab0: da03 7374 72da 0974 7261 6e73 6c61 7465  ..str..translate
+00000ac0: da09 6d61 6b65 7472 616e 73da 0573 706c  ..maketrans..spl
+00000ad0: 6974 7211 0000 00da 0977 6f72 6b73 6865  itr......workshe
+00000ae0: 6574 da06 6578 7465 6e64 720f 0000 00da  et..extendr.....
+00000af0: 0675 7064 6174 65da 0a49 6e64 6578 4572  .update..IndexEr
+00000b00: 726f 7229 0972 1200 0000 7222 0000 0072  ror).r....r"...r
+00000b10: 2300 0000 da0f 6368 6172 5f74 6f5f 7265  #.....char_to_re
+00000b20: 706c 6163 655a 1277 6f72 6b73 6865 6574  placeZ.worksheet
+00000b30: 5f63 616d 7061 6967 6e5a 1263 616d 7061  _campaignZ.campa
+00000b40: 6967 6e5f 696e 666f 5f6c 6973 745a 1263  ign_info_listZ.c
+00000b50: 616d 7061 6967 6e5f 696e 666f 5f64 6963  ampaign_info_dic
+00000b60: 745a 0a63 656c 6c5f 7261 6e67 65da 0569  tZ.cell_range..i
+00000b70: 6e64 6578 7213 0000 0072 1300 0000 7214  ndexr....r....r.
+00000b80: 0000 00da 1167 6574 5f63 616d 7061 6967  .....get_campaig
+00000b90: 6e5f 696e 666f 2a00 0000 731a 0000 0000  n_info*...s.....
+00000ba0: 0e10 0124 020c 0104 0104 0208 0112 0108  ...$............
+00000bb0: 0102 011a 010c 0108 017a 2067 6574 4773  .........z getGs
+00000bc0: 7072 6561 6444 6174 612e 6765 745f 6361  preadData.get_ca
+00000bd0: 6d70 6169 676e 5f69 6e66 6f29 0272 2200  mpaign_info).r".
+00000be0: 0000 7223 0000 0063 0300 0000 0000 0000  ..r#...c........
+00000bf0: 0000 0000 0c00 0000 0600 0000 4300 0000  ............C...
+00000c00: 73fc 0000 0074 007c 0283 0164 016b 0272  s....t.|...d.k.r
+00000c10: 3c64 0264 0264 0264 0264 0264 039c 057d  <d.d.d.d.d.d...}
+00000c20: 0364 0464 0584 007c 02a0 0174 02a0 037c  .d.d...|...t...|
+00000c30: 03a1 01a1 01a0 0464 06a1 0144 0083 017d  .......d...D...}
+00000c40: 027c 006a 05a0 067c 01a1 017d 0474 0783  .|.j...|...}.t..
+00000c50: 007d 057c 04a0 087c 02a1 017d 0674 0964  .}.|...|...}.t.d
+00000c60: 0774 0a7c 0683 0164 0883 0344 005d 8e7d  .t.|...d...D.].}
+00000c70: 077c 067c 0719 00a0 0b64 07a1 017d 087c  .|.|.....d...}.|
+00000c80: 05a0 0c7c 0864 0719 0069 0069 01a1 0101  ...|.d...i.i....
+00000c90: 0074 0d6a 0ea0 0f7c 067c 0719 00a1 017d  .t.j...|.|.....}
+00000ca0: 097c 096a 1064 0719 007d 0a74 0d6a 0e7c  .|.j.d...}.t.j.|
+00000cb0: 096a 1164 0864 0085 0219 007c 0a64 098d  .j.d.d.....|.d..
+00000cc0: 027d 0b7c 0b6a 1264 0274 136a 1464 0a64  .}.|.j.d.t.j.d.d
+00000cd0: 0b8d 0301 007c 0b6a 1564 0764 0c64 0a64  .....|.j.d.d.d.d
+00000ce0: 0d8d 0301 007c 057c 0864 0719 0019 00a0  .....|.|.d......
+00000cf0: 0c7c 0ba0 16a1 00a1 0101 0071 687c 0553  .|.........qh|.S
+00000d00: 0029 0e4e 7232 0000 0072 0800 0000 7225  .).Nr2...r....r%
+00000d10: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00000d20: 0200 0000 0300 0000 5300 0000 7310 0000  ........S...s...
+00000d30: 0067 007c 005d 087d 017c 0191 0271 0453  .g.|.].}.|...q.S
+00000d40: 0072 1300 0000 7213 0000 0072 2b00 0000  .r....r....r+...
+00000d50: 7213 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+00000d60: 2e00 0000 4b00 0000 722f 0000 007a 3367  ....K...r/...z3g
+00000d70: 6574 4773 7072 6561 6444 6174 612e 6765  etGspreadData.ge
+00000d80: 745f 636f 6e74 656e 745f 696e 666f 2e3c  t_content_info.<
+00000d90: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00000da0: 703e 7230 0000 0072 0100 0000 7231 0000  p>r0...r....r1..
+00000db0: 0029 01da 0763 6f6c 756d 6e73 5429 01da  .)...columnsT)..
+00000dc0: 0769 6e70 6c61 6365 da03 616e 7929 035a  .inplace..any).Z
+00000dd0: 0461 7869 73da 0368 6f77 723e 0000 0029  .axis..howr>...)
+00000de0: 1772 2000 0000 7233 0000 0072 3200 0000  .r ...r3...r2...
+00000df0: 7234 0000 0072 3500 0000 7211 0000 0072  r4...r5...r....r
+00000e00: 3600 0000 da04 6469 6374 5a09 6261 7463  6.....dictZ.batc
+00000e10: 685f 6765 74da 0572 616e 6765 da03 6c65  h_get..range..le
+00000e20: 6eda 0370 6f70 7238 0000 00da 0270 645a  n..popr8.....pdZ
+00000e30: 0944 6174 6146 7261 6d65 5a0c 6672 6f6d  .DataFrameZ.from
+00000e40: 5f72 6563 6f72 6473 5a04 696c 6f63 da06  _recordsZ.iloc..
+00000e50: 7661 6c75 6573 da07 7265 706c 6163 65da  values..replace.
+00000e60: 026e 70da 036e 616e 5a06 6472 6f70 6e61  .np..nanZ.dropna
+00000e70: 5a07 746f 5f64 6963 7429 0c72 1200 0000  Z.to_dict).r....
+00000e80: 7222 0000 0072 2300 0000 723a 0000 005a  r"...r#...r:...Z
+00000e90: 1677 6f72 6b73 6865 6574 5f63 6f6e 7465  .worksheet_conte
+00000ea0: 6e74 5f69 6e66 6f5a 1163 6f6e 7465 6e74  nt_infoZ.content
+00000eb0: 5f69 6e66 6f5f 6469 6374 5a11 636f 6e74  _info_dictZ.cont
+00000ec0: 656e 745f 696e 666f 5f6c 6973 7472 3b00  ent_info_listr;.
+00000ed0: 0000 da0c 7365 6374 696f 6e5f 6e61 6d65  ....section_name
+00000ee0: da02 6466 da0a 6865 6164 6572 5f72 6f77  ..df..header_row
+00000ef0: 5a0e 6466 5f77 6974 685f 6865 6164 6572  Z.df_with_header
+00000f00: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
+00000f10: 1067 6574 5f63 6f6e 7465 6e74 5f69 6e66  .get_content_inf
+00000f20: 6f48 0000 0073 2000 0000 0001 0c01 1001  oH...s .........
+00000f30: 2002 0c01 0601 0a02 1401 0e01 1201 1001   ...............
+00000f40: 0a01 1801 1201 1001 1806 7a1f 6765 7447  ..........z.getG
+00000f50: 7370 7265 6164 4461 7461 2e67 6574 5f63  spreadData.get_c
+00000f60: 6f6e 7465 6e74 5f69 6e66 6f4e 2902 7208  ontent_infoN).r.
+00000f70: 0000 0072 0800 0000 290b da08 5f5f 6e61  ...r....)...__na
+00000f80: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000f90: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7232  ..__qualname__r2
+00000fa0: 0000 0072 1500 0000 7210 0000 0072 0300  ...r....r....r..
+00000fb0: 0000 da04 6c69 7374 7202 0000 0072 3c00  ....listr....r<.
+00000fc0: 0000 724d 0000 0072 1300 0000 7213 0000  ..rM...r....r...
+00000fd0: 0072 1300 0000 7214 0000 0072 0700 0000  .r....r....r....
+00000fe0: 0f00 0000 7308 0000 0008 0112 0c08 0e22  ....s.........."
+00000ff0: 1e72 0700 0000 2914 721a 0000 00da 0674  .r....).r......t
+00001000: 7970 696e 6772 0200 0000 7203 0000 005a  ypingr....r....Z
+00001010: 0670 616e 6461 7372 4500 0000 da05 6e75  .pandasrE.....nu
+00001020: 6d70 7972 4800 0000 da02 6f73 da0c 636f  mpyrH.....os..co
+00001030: 6e66 6967 7061 7273 6572 7204 0000 00da  nfigparserr.....
+00001040: 206d 6169 6c63 6869 6d70 5f61 7574 6f2e   mailchimp_auto.
+00001050: 7363 7269 7074 732e 6469 7265 6374 6f72  scripts.director
+00001060: 7972 1e00 0000 da02 7265 5a26 6d61 696c  yr......reZ&mail
+00001070: 6368 696d 705f 6175 746f 2e73 6372 6970  chimp_auto.scrip
+00001080: 7473 2e69 6d61 6765 5f70 726f 6365 7373  ts.image_process
+00001090: 6f72 7206 0000 0072 0e00 0000 7218 0000  orr....r....r...
+000010a0: 00da 0f74 656d 706c 6174 655f 636f 6e66  ...template_conf
+000010b0: 6967 7207 0000 0072 1300 0000 7213 0000  igr....r....r...
+000010c0: 0072 1300 0000 7214 0000 00da 083c 6d6f  .r....r......<mo
+000010d0: 6475 6c65 3e01 0000 0073 1800 0000 0801  dule>....s......
+000010e0: 1001 0801 0801 0801 0c01 0801 0801 0801  ................
+000010f0: 0c02 0601 0a02                           ......
```

### Comparing `mailchimp_auto-0.1.0/mailchimp_auto/scripts/__pycache__/template.cpython-310.pyc` & `mailchimp_auto-0.1.1/mailchimp_auto/scripts/__pycache__/engine.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 29 09:53:01 2022 UTC, .py size: 1722 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,108 +1,131 @@
-00000000: 6f0d 0d0a 0000 0000 fdad e362 ba06 0000  o..........b....
+00000000: 610d 0d0a 0000 0000 502f 3064 710a 0000  a.......P/0dq...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000b 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
-00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
-00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
-00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
-00000060: 0100 6400 6405 6c09 5a09 6400 6405 6c0a  ..d.d.l.Z.d.d.l.
-00000070: 5a0a 6508 8300 5a0b 650b a00c 6504 6a0d  Z.e...Z.e...e.j.
-00000080: a101 0100 0906 0907 640f 6408 650e 6409  ........d.d.e.d.
-00000090: 650e 640a 650e 640b 650f 640c 6405 660a  e.d.e.d.e.d.d.f.
-000000a0: 640d 640e 8405 5a10 6405 5300 2910 e900  d.d...Z.d.S.)...
-000000b0: 0000 0029 02da 0b45 6e76 6972 6f6e 6d65  ...)...Environme
-000000c0: 6e74 da10 4669 6c65 5379 7374 656d 4c6f  nt..FileSystemLo
-000000d0: 6164 6572 2901 da09 6469 7265 6374 6f72  ader)...director
-000000e0: 7929 01da 0449 6e66 6f29 01da 0f52 6177  y)...Info)...Raw
-000000f0: 436f 6e66 6967 5061 7273 6572 4efa 0a6d  ConfigParserN..m
-00000100: 6173 7465 722e 6874 6d46 da0e 6163 636f  aster.htmF..acco
-00000110: 756e 745f 6368 6f69 6365 da0d 7465 6d70  unt_choice..temp
-00000120: 6c61 7465 5f6e 616d 65da 0e69 6e70 7574  late_name..input
-00000130: 5f66 696c 654e 616d 65da 0770 7265 7669  _fileName..previ
-00000140: 6577 da06 7265 7475 726e 6304 0000 0000  ew..returnc.....
-00000150: 0000 0000 0000 000b 0000 0008 0000 0043  ...............C
-00000160: 0000 0073 a800 0000 7400 7401 6a02 6401  ...s....t.t.j.d.
-00000170: 8d01 7d04 7403 7c04 6402 8d01 7d05 7c01  ..}.t.|.d...}.|.
-00000180: 9b00 6403 7c02 9b00 9d03 7d06 7404 7c00  ..d.|.....}.t.|.
-00000190: 7c01 6404 8d02 a005 a100 7d07 7c05 a006  |.d.......}.|...
-000001a0: 7c06 a101 6a07 640b 6900 7c07 a401 8e01  |...j.d.i.|.....
-000001b0: 7d08 7c03 7252 7408 6a09 a00a 7401 6a0b  }.|.rRt.j...t.j.
-000001c0: 6405 a102 7d09 740c 7c09 6406 6407 6408  d...}.t.|.d.d.d.
-000001d0: 8d03 8f0d 7d0a 7c0a a00d 7c08 a101 0100  ....}.|...|.....
-000001e0: 5700 6409 0400 0400 8303 0100 6e08 3100  W.d.........n.1.
-000001f0: 7346 7701 0100 0100 0100 5900 0100 740e  sFw.......Y...t.
-00000200: 640a 7c09 9b00 9d02 8301 0100 7c08 5300  d.|.........|.S.
-00000210: 290c 618b 0100 005f 7375 6d6d 6172 795f  ).a...._summary_
-00000220: 0a0a 2020 2020 3a70 6172 616d 2061 6363  ..    :param acc
-00000230: 6f75 6e74 5f63 686f 6963 653a 205f 6465  ount_choice: _de
-00000240: 7363 7269 7074 696f 6e5f 0a20 2020 203a  scription_.    :
-00000250: 7479 7065 2061 6363 6f75 6e74 5f63 686f  type account_cho
-00000260: 6963 653a 2073 7472 0a20 2020 203a 7061  ice: str.    :pa
-00000270: 7261 6d20 7465 6d70 6c61 7465 5f6e 616d  ram template_nam
-00000280: 653a 205f 6465 7363 7269 7074 696f 6e5f  e: _description_
-00000290: 0a20 2020 203a 7479 7065 2074 656d 706c  .    :type templ
-000002a0: 6174 655f 6e61 6d65 3a20 7374 720a 2020  ate_name: str.  
-000002b0: 2020 3a70 6172 616d 2069 6e70 7574 5f66    :param input_f
-000002c0: 696c 654e 616d 653a 205f 6465 7363 7269  ileName: _descri
-000002d0: 7074 696f 6e5f 2c20 6465 6661 756c 7473  ption_, defaults
-000002e0: 2074 6f20 226d 6173 7465 722e 6874 6d22   to "master.htm"
-000002f0: 0a20 2020 203a 7479 7065 2069 6e70 7574  .    :type input
-00000300: 5f66 696c 654e 616d 653a 2073 7472 2c20  _fileName: str, 
-00000310: 6f70 7469 6f6e 616c 0a20 2020 203a 7061  optional.    :pa
-00000320: 7261 6d20 7072 6576 6965 773a 205f 6465  ram preview: _de
-00000330: 7363 7269 7074 696f 6e5f 2c20 6465 6661  scription_, defa
-00000340: 756c 7473 2074 6f20 4661 6c73 650a 2020  ults to False.  
-00000350: 2020 3a74 7970 6520 7072 6576 6965 773a    :type preview:
-00000360: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0a   bool, optional.
-00000370: 2020 2020 3a72 6574 7572 6e3a 205f 6465      :return: _de
-00000380: 7363 7269 7074 696f 6e5f 0a20 2020 203a  scription_.    :
-00000390: 7274 7970 653a 205f 7479 7065 5f0a 2020  rtype: _type_.  
-000003a0: 2020 2901 da0a 7365 6172 6368 7061 7468    )...searchpath
-000003b0: 2901 da06 6c6f 6164 6572 fa01 2f29 0272  )...loader../).r
-000003c0: 0800 0000 da0f 7465 6d70 6c61 7465 5f63  ......template_c
-000003d0: 686f 6963 657a 0969 6e64 6578 2e68 746d  hoicez.index.htm
-000003e0: da01 777a 0575 7466 2d38 2901 da08 656e  ..wz.utf-8)...en
-000003f0: 636f 6469 6e67 4e7a 2f50 6c65 6173 6520  codingNz/Please 
-00000400: 6368 6563 6b20 796f 7572 2067 656e 6572  check your gener
-00000410: 6174 6564 2074 656d 706c 6174 6520 6f75  ated template ou
-00000420: 7470 7574 2061 7420 a900 290f 7203 0000  tput at ..).r...
-00000430: 0072 0400 0000 da0f 7465 6d70 6c61 7465  .r......template
-00000440: 5f66 6f6c 6465 7272 0200 0000 7205 0000  _folderr....r...
-00000450: 00da 0e67 6574 6874 6d6c 436f 6e74 656e  ...gethtmlConten
-00000460: 74da 0c67 6574 5f74 656d 706c 6174 65da  t..get_template.
-00000470: 0672 656e 6465 72da 026f 73da 0470 6174  .render..os..pat
-00000480: 68da 046a 6f69 6eda 0d6f 7574 7075 745f  h..join..output_
-00000490: 666f 6c64 6572 da04 6f70 656e da05 7772  folder..open..wr
-000004a0: 6974 65da 0570 7269 6e74 290b 7208 0000  ite..print).r...
-000004b0: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
-000004c0: 5a0a 6669 6c65 4c6f 6164 6572 da03 656e  Z.fileLoader..en
-000004d0: 765a 0c74 656d 706c 6174 655f 6c6f 63da  vZ.template_loc.
-000004e0: 0464 6174 61da 0872 656e 6465 7265 64da  .data..rendered.
-000004f0: 0b6f 7574 7075 745f 6669 6c65 da01 6672  .output_file..fr
-00000500: 1300 0000 7213 0000 00fa 6b43 3a5c 5573  ....r.....kC:\Us
-00000510: 6572 735c 7479 735c 446f 6375 6d65 6e74  ers\tys\Document
-00000520: 735c 5072 6f6a 6563 745c 6d61 696c 6368  s\Project\mailch
-00000530: 696d 705f 6372 6561 7469 6f6e 5f70 726f  imp_creation_pro
-00000540: 6a65 6374 5c6d 6169 6c63 6869 6d70 2d61  ject\mailchimp-a
-00000550: 7574 6f5c 6d61 696c 6368 696d 705f 6175  uto\mailchimp_au
-00000560: 746f 5c73 6372 6970 7473 5c74 656d 706c  to\scripts\templ
-00000570: 6174 652e 7079 da16 6765 6e65 7261 7465  ate.py..generate
-00000580: 5f68 746d 6c5f 7465 6d70 6c61 7465 0c00  _html_template..
-00000590: 0000 7318 0000 000c 120a 010e 0310 0116  ..s.............
-000005a0: 0304 0210 0110 010c 011c ff0e 0204 0172  ...............r
-000005b0: 2500 0000 2902 7207 0000 0046 2911 da06  %...).r....F)...
-000005c0: 6a69 6e6a 6132 7202 0000 0072 0300 0000  jinja2r....r....
-000005d0: da16 6d61 696c 6368 696d 705f 6175 746f  ..mailchimp_auto
-000005e0: 2e73 6372 6970 7473 7204 0000 00da 266d  .scriptsr.....&m
-000005f0: 6169 6c63 6869 6d70 5f61 7574 6f2e 7363  ailchimp_auto.sc
-00000600: 7269 7074 732e 6361 6d70 6169 676e 5f64  ripts.campaign_d
-00000610: 6574 6169 6c72 0500 0000 da0c 636f 6e66  etailr......conf
-00000620: 6967 7061 7273 6572 7206 0000 0072 1800  igparserr....r..
-00000630: 0000 da07 6c6f 6767 696e 67da 0663 6f6e  ....logging..con
-00000640: 6669 67da 0472 6561 64da 0f74 656d 706c  fig..read..templ
-00000650: 6174 655f 636f 6e66 6967 da03 7374 72da  ate_config..str.
-00000660: 0462 6f6f 6c72 2500 0000 7213 0000 0072  .boolr%...r....r
-00000670: 1300 0000 7213 0000 0072 2400 0000 da08  ....r....r$.....
-00000680: 3c6d 6f64 756c 653e 0100 0000 7322 0000  <module>....s"..
-00000690: 0010 000c 010c 010c 0108 0108 0106 020c  ................
-000006a0: 0102 0402 010c fe02 0102 ff02 0202 fe02  ................
-000006b0: 020e fe                                  ...
+00000020: 0004 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
+00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
+00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
+00000050: 6d06 5a06 0100 6400 6404 6c07 5400 6400  m.Z...d.d.l.T.d.
+00000060: 6405 6c08 6d09 5a09 0100 6400 6404 6c0a  d.l.m.Z...d.d.l.
+00000070: 5400 6400 6401 6c0b 5a0b 650c 6509 650c  T.d.d.l.Z.e.e.e.
+00000080: 650c 6602 1900 6406 9c02 6407 6408 8404  e.f...d...d.d...
+00000090: 5a0d 650c 650c 650e 6409 9c03 640a 640b  Z.e.e.e.d...d.d.
+000000a0: 8404 5a0f 6401 5300 290c e900 0000 004e  ..Z.d.S.)......N
+000000b0: 2901 da1a 6361 6d70 6169 676e 5f63 7265  )...campaign_cre
+000000c0: 6174 696f 6e5f 6675 6e63 7469 6f6e 2903  ation_function).
+000000d0: da16 6765 6e65 7261 7465 5f68 746d 6c5f  ..generate_html_
+000000e0: 7465 6d70 6c61 7465 da0f 7570 6c6f 6164  template..upload
+000000f0: 5f74 656d 706c 6174 65da 1467 6574 5f65  _template..get_e
+00000100: 6469 7461 626c 655f 636f 6e74 656e 7429  ditable_content)
+00000110: 01da 012a 2901 da05 5475 706c 6529 02da  ...*)...Tuple)..
+00000120: 1061 6363 6f75 6e74 5f75 7365 726e 616d  .account_usernam
+00000130: 65da 0672 6574 7572 6e63 0100 0000 0000  e..returnc......
+00000140: 0000 0000 0000 0400 0000 0400 0000 4300  ..............C.
+00000150: 0000 7328 0000 0074 0064 0183 017d 017c  ..s(...t.d...}.|
+00000160: 01a0 017c 0064 02a1 027d 027c 01a0 017c  ...|.d...}.|...|
+00000170: 0064 03a1 027d 037c 027c 0366 0253 0029  .d...}.|.|.f.S.)
+00000180: 044e 7a0c 6163 636f 756e 742e 636f 6e66  .Nz.account.conf
+00000190: da07 6170 695f 6b65 79da 0d73 6572 7665  ..api_key..serve
+000001a0: 725f 7072 6566 6978 2902 5a0b 7265 6164  r_prefix).Z.read
+000001b0: 5f63 6f6e 6669 67da 0367 6574 2904 7208  _config..get).r.
+000001c0: 0000 00da 0663 6f6e 6669 6772 0a00 0000  .....configr....
+000001d0: 720b 0000 00a9 0072 0e00 0000 fa66 433a  r......r.....fC:
+000001e0: 5c55 7365 7273 5c79 6f6e 6773 6865 6e67  \Users\yongsheng
+000001f0: 2e74 616e 5c44 6f63 756d 656e 7473 5c43  .tan\Documents\C
+00000200: 6f64 696e 675c 6769 7468 7562 2d70 726f  oding\github-pro
+00000210: 6a65 6374 5c6d 6169 6c63 6869 6d70 5f61  ject\mailchimp_a
+00000220: 7574 6f5c 6d61 696c 6368 696d 705f 6175  uto\mailchimp_au
+00000230: 746f 5c73 6372 6970 7473 5c65 6e67 696e  to\scripts\engin
+00000240: 652e 7079 da07 636f 6e6e 6563 740b 0000  e.py..connect...
+00000250: 0073 0800 0000 0001 0801 0c01 0c01 7210  .s............r.
+00000260: 0000 0029 0372 0800 0000 da0d 7465 6d70  ...).r......temp
+00000270: 6c61 7465 5f6e 616d 65da 0770 7265 7669  late_name..previ
+00000280: 6577 6303 0000 0000 0000 0000 0000 0009  ewc.............
+00000290: 0000 0006 0000 0043 0000 0073 8400 0000  .......C...s....
+000002a0: 7c02 736e 7400 7c00 8301 5c02 7d03 7d04  |.snt.|...\.}.}.
+000002b0: 7401 a002 a100 7d05 7c05 a003 7c03 7c04  t.....}.|...|.|.
+000002c0: 6401 9c02 a101 0100 7404 7c00 7c01 6402  d.......t.|.|.d.
+000002d0: 8d02 7d06 7405 7c01 7c06 7c05 6403 8d03  ..}.t.|.|.|.d...
+000002e0: 7d07 7406 7c00 7c01 7c05 7c07 6404 8d04  }.t.|.|.|.|.d...
+000002f0: 7d08 7407 a008 7c08 6405 1900 a101 0100  }.t...|.d.......
+00000300: 7409 7c07 7c05 6406 8d02 0100 6e12 7c02  t.|.|.d.....n.|.
+00000310: 7280 7404 7c00 7c01 7c02 6407 8d03 7d06  r.t.|.|.|.d...}.
+00000320: 6408 5300 2909 6178 0200 005f 7375 6d6d  d.S.).ax..._summ
+00000330: 6172 795f 0a0a 2020 2020 3a70 6172 616d  ary_..    :param
+00000340: 2061 6363 6f75 6e74 5f75 7365 726e 616d   account_usernam
+00000350: 653a 205f 6465 7363 7269 7074 696f 6e5f  e: _description_
+00000360: 0a20 2020 203a 7479 7065 2061 6363 6f75  .    :type accou
+00000370: 6e74 5f75 7365 726e 616d 653a 2073 7472  nt_username: str
+00000380: 0a20 2020 203a 7061 7261 6d20 7465 6d70  .    :param temp
+00000390: 6c61 7465 5f6e 616d 653a 205f 6465 7363  late_name: _desc
+000003a0: 7269 7074 696f 6e5f 0a20 2020 203a 7479  ription_.    :ty
+000003b0: 7065 2074 656d 706c 6174 655f 6e61 6d65  pe template_name
+000003c0: 3a20 7374 720a 2020 2020 3a70 6172 616d  : str.    :param
+000003d0: 2070 7265 7669 6577 3a20 5f64 6573 6372   preview: _descr
+000003e0: 6970 7469 6f6e 5f0a 2020 2020 3a74 7970  iption_.    :typ
+000003f0: 6520 7072 6576 6965 773a 2062 6f6f 6c0a  e preview: bool.
+00000400: 0a20 2020 2045 7870 6c61 6e61 7469 6f6e  .    Explanation
+00000410: 3a20 0a20 2020 2023 2048 6f77 2074 6f20  : .    # How to 
+00000420: 7374 6172 7420 7468 6973 2070 726f 6772  start this progr
+00000430: 616d 0a20 2020 2060 7079 7468 6f6e 206d  am.    `python m
+00000440: 6169 6c63 6869 6d70 6361 6d70 2e70 7960  ailchimpcamp.py`
+00000450: 206f 7220 6070 7974 686f 6e20 6d61 696c   or `python mail
+00000460: 6368 696d 7063 616d 702e 7079 2072 756e  chimpcamp.py run
+00000470: 600a 2020 2020 0a20 2020 2023 2050 726f  `.    .    # Pro
+00000480: 6365 7373 6573 2062 6569 6e67 2072 756e  cesses being run
+00000490: 3a0a 2020 2020 312e 2063 6f6e 6e65 6374  :.    1. connect
+000004a0: 2074 6f20 796f 7572 206d 6169 6c63 6869   to your mailchi
+000004b0: 6d70 2061 6363 6f75 6e74 2075 7369 6e67  mp account using
+000004c0: 2041 5049 206b 6579 2e0a 2020 2020 322e   API key..    2.
+000004d0: 2063 7265 6174 6520 6120 6361 6d70 6169   create a campai
+000004e0: 676e 2075 6e64 6572 2079 6f75 7220 6365  gn under your ce
+000004f0: 7274 6169 6e20 6175 6469 656e 6365 206c  rtain audience l
+00000500: 6973 742e 0a20 2020 2033 2e20 6765 6e65  ist..    3. gene
+00000510: 7261 7465 2061 2068 746d 6c20 7465 6d70  rate a html temp
+00000520: 6c61 7465 2062 6173 6564 206f 6e20 796f  late based on yo
+00000530: 7572 2067 6f6f 676c 6520 7370 7265 6164  ur google spread
+00000540: 7368 6565 7420 696e 7075 742e 0a20 2020  sheet input..   
+00000550: 2034 2e20 7570 6c6f 6164 2074 6861 7420   4. upload that 
+00000560: 6874 6d6c 2074 656d 706c 6174 6520 746f  html template to
+00000570: 2074 6865 206d 6169 6c63 6869 6d70 2073   the mailchimp s
+00000580: 6572 7665 7220 6173 2074 6865 2063 616d  erver as the cam
+00000590: 7061 6967 6e20 636f 6e74 656e 742e 0a20  paign content.. 
+000005a0: 2020 2029 0272 0a00 0000 5a06 7365 7276     ).r....Z.serv
+000005b0: 6572 2902 da0e 6163 636f 756e 745f 6368  er)...account_ch
+000005c0: 6f69 6365 7211 0000 0029 0372 1100 0000  oicer....).r....
+000005d0: 5a09 6874 6d6c 5f63 6f64 65da 0663 6c69  Z.html_code..cli
+000005e0: 656e 7429 0472 1300 0000 5a0f 7465 6d70  ent).r....Z.temp
+000005f0: 6c61 7465 5f63 686f 6963 6572 1400 0000  late_choicer....
+00000600: da0b 7465 6d70 6c61 7465 5f69 64da 0269  ..template_id..i
+00000610: 6429 0272 1500 0000 7214 0000 0029 0372  d).r....r....).r
+00000620: 1300 0000 7211 0000 0072 1200 0000 4e29  ....r....r....N)
+00000630: 0a72 1000 0000 da13 6d61 696c 6368 696d  .r......mailchim
+00000640: 705f 6d61 726b 6574 696e 675a 0643 6c69  p_marketingZ.Cli
+00000650: 656e 745a 0a73 6574 5f63 6f6e 6669 6772  entZ.set_configr
+00000660: 0300 0000 7204 0000 0072 0200 0000 da07  ....r....r......
+00000670: 6c6f 6767 696e 67da 0469 6e66 6f72 0500  logging..infor..
+00000680: 0000 2909 7208 0000 0072 1100 0000 7212  ..).r....r....r.
+00000690: 0000 0072 0a00 0000 720b 0000 0072 1400  ...r....r....r..
+000006a0: 0000 5a0d 7265 6e64 6572 6564 5f68 746d  ..Z.rendered_htm
+000006b0: 6c72 1500 0000 5a08 6361 6d70 6169 676e  lr....Z.campaign
+000006c0: 720e 0000 0072 0e00 0000 720f 0000 00da  r....r....r.....
+000006d0: 1363 7265 6174 655f 6e65 775f 6361 6d70  .create_new_camp
+000006e0: 6169 676e 1200 0000 7322 0000 0000 1504  aign....s"......
+000006f0: 010c 0208 0104 0102 0102 fe08 060c 040e  ................
+00000700: 0304 0102 0104 fe06 040e 020e 0204 0172  ...............r
+00000710: 1a00 0000 2910 7217 0000 005a 266d 6169  ....).r....Z&mai
+00000720: 6c63 6869 6d70 5f61 7574 6f2e 7363 7269  lchimp_auto.scri
+00000730: 7074 732e 6372 6561 7465 5f63 616d 7061  pts.create_campa
+00000740: 6967 6e72 0200 0000 5a26 6d61 696c 6368  ignr....Z&mailch
+00000750: 696d 705f 6175 746f 2e73 6372 6970 7473  imp_auto.scripts
+00000760: 2e74 656d 706c 6174 655f 6163 7469 6f6e  .template_action
+00000770: 7203 0000 0072 0400 0000 7205 0000 005a  r....r....r....Z
+00000780: 1d6d 6169 6c63 6869 6d70 5f61 7574 6f2e  .mailchimp_auto.
+00000790: 7363 7269 7074 732e 436f 6e66 6967 da06  scripts.Config..
+000007a0: 7479 7069 6e67 7207 0000 005a 266d 6169  typingr....Z&mai
+000007b0: 6c63 6869 6d70 5f61 7574 6f2e 7363 7269  lchimp_auto.scri
+000007c0: 7074 732e 6361 6d70 6169 676e 5f64 6574  pts.campaign_det
+000007d0: 6169 6c72 1800 0000 da03 7374 7272 1000  ailr......strr..
+000007e0: 0000 da04 626f 6f6c 721a 0000 0072 0e00  ....boolr....r..
+000007f0: 0000 720e 0000 0072 0e00 0000 720f 0000  ..r....r....r...
+00000800: 00da 083c 6d6f 6475 6c65 3e02 0000 0073  ...<module>....s
+00000810: 1000 0000 0801 0c01 1401 0801 0c01 0801  ................
+00000820: 0803 1807                                ....
```

### Comparing `mailchimp_auto-0.1.0/mailchimp_auto/scripts/__pycache__/template_Config.cpython-310.pyc` & `mailchimp_auto-0.1.1/mailchimp_auto/scripts/__pycache__/template_Config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 29 14:39:32 2022 UTC, .py size: 10833 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,477 +1,473 @@
-00000000: 6f0d 0d0a 0000 0000 24f1 e362 512a 0000  o.......$..bQ*..
+00000000: 610d 0d0a 0000 0000 5230 3064 512a 0000  a.......R00dQ*..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 5a04 6400  m.Z...d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6400 6404 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6403 6c0a 5a0a 6501 8300 5a0b 4700 6406  d.l.Z.e...Z.G.d.
 00000080: 6407 8400 6407 8302 5a0c 6403 5300 2908  d...d...Z.d.S.).
 00000090: e900 0000 0029 01da 0f52 6177 436f 6e66  .....)...RawConf
 000000a0: 6967 5061 7273 6572 2901 da06 6578 6973  igParser)...exis
 000000b0: 7473 4e29 01da 0964 6972 6563 746f 7279  tsN)...directory
 000000c0: 2901 da13 6578 7472 6163 745f 6964 5f66  )...extract_id_f
 000000d0: 726f 6d5f 7572 6c63 0000 0000 0000 0000  rom_urlc........
-000000e0: 0000 0000 0000 0000 0700 0000 4000 0000  ............@...
-000000f0: 73c4 0000 0065 005a 0164 005a 0264 0165  s....e.Z.d.Z.d.e
-00000100: 0366 0264 0264 0384 045a 0464 0464 0584  .f.d.d...Z.d.d..
-00000110: 005a 0564 0665 0364 0765 0366 0464 0864  .Z.d.e.d.e.f.d.d
-00000120: 0984 045a 0664 2264 0b65 0364 0765 0765  ...Z.d"d.e.d.e.e
-00000130: 0819 0066 0464 0c64 0d84 055a 0964 2364  ...f.d.d...Z.d#d
-00000140: 0b65 0364 0f65 0364 1065 0366 0664 1164  .e.d.e.d.e.f.d.d
-00000150: 1284 055a 0a64 2264 0b65 0364 0765 0765  ...Z.d"d.e.d.e.e
-00000160: 0819 0066 0464 1364 1484 055a 0b64 0f65  ...f.d.d...Z.d.e
-00000170: 0364 1565 0366 0464 1664 1784 045a 0c64  .d.e.f.d.d...Z.d
-00000180: 1865 0366 0264 1964 1a84 045a 0d64 1865  .e.f.d.d...Z.d.e
-00000190: 0366 0264 1b64 1c84 045a 0e64 1d64 1e84  .f.d.d...Z.d.d..
-000001a0: 005a 0f64 1065 0364 0f65 0366 0464 1f64  .Z.d.e.d.e.f.d.d
-000001b0: 2084 045a 1064 2153 0029 24da 0d43 6f6e   ..Z.d!S.)$..Con
-000001c0: 6669 6775 7261 7469 6f6e da07 7375 626a  figuration..subj
-000001d0: 6563 7463 0200 0000 0000 0000 0000 0000  ectc............
-000001e0: 0200 0000 0200 0000 4300 0000 730a 0000  ........C...s...
-000001f0: 007c 017c 005f 0064 0053 00a9 014e 2901  .|.|._.d.S...N).
-00000200: 7207 0000 0029 02da 0473 656c 6672 0700  r....)...selfr..
-00000210: 0000 a900 720a 0000 00fa 7243 3a5c 5573  ....r.....rC:\Us
-00000220: 6572 735c 7479 735c 446f 6375 6d65 6e74  ers\tys\Document
-00000230: 735c 5072 6f6a 6563 745c 6d61 696c 6368  s\Project\mailch
-00000240: 696d 705f 6372 6561 7469 6f6e 5f70 726f  imp_creation_pro
-00000250: 6a65 6374 5c6d 6169 6c63 6869 6d70 2d61  ject\mailchimp-a
-00000260: 7574 6f5c 6d61 696c 6368 696d 705f 6175  uto\mailchimp_au
-00000270: 746f 5c73 6372 6970 7473 5c74 656d 706c  to\scripts\templ
-00000280: 6174 655f 436f 6e66 6967 2e70 79da 085f  ate_Config.py.._
-00000290: 5f69 6e69 745f 5f0c 0000 0073 0200 0000  _init__....s....
-000002a0: 0a01 7a16 436f 6e66 6967 7572 6174 696f  ..z.Configuratio
-000002b0: 6e2e 5f5f 696e 6974 5f5f 6301 0000 0000  n.__init__c.....
-000002c0: 0000 0000 0000 0004 0000 000b 0000 0043  ...............C
-000002d0: 0000 0073 da00 0000 7400 6401 8301 0100  ...s....t.d.....
-000002e0: 7400 6402 8301 0100 7400 6403 8301 0100  t.d.....t.d.....
-000002f0: 7401 7c00 a002 a100 a003 a100 8301 6404  t.|...........d.
-00000300: 6b04 7233 7c00 a002 a100 a003 a100 4400  k.r3|.........D.
-00000310: 5d16 7d01 7400 7404 7c01 8301 6405 7405  ].}.t.t.|...d.t.
-00000320: 7404 7c00 a002 a100 6a06 7c01 6406 6400  t.|.....j.|.d.d.
-00000330: 6407 8d03 8301 8301 8303 0100 711c 7400  d...........q.t.
-00000340: 6408 8301 0100 7400 6409 7c00 6a07 9b00  d.....t.d.|.j...
-00000350: 9d02 8301 0100 7400 640a 7c00 6a07 9b00  ......t.d.|.j...
-00000360: 9d02 8301 0100 7400 640b 7c00 6a07 9b00  ......t.d.|.j...
-00000370: 9d02 8301 0100 7400 640c 8301 0100 6700  ......t.d.....g.
-00000380: 640d a201 7d02 7408 640e 8301 7d03 7c03  d...}.t.d...}.|.
-00000390: 7c02 7601 726b 7400 640f 8301 0100 7408  |.v.rkt.d.....t.
-000003a0: 640e 8301 7d03 7c03 7c02 7601 735f 7c03  d...}.|.|.v.s_|.
-000003b0: 5300 2910 4e7a 1443 7572 7265 6e74 2074  S.).Nz.Current t
-000003c0: 656d 706c 6174 6528 7329 3a7a 1954 656d  emplate(s):z.Tem
-000003d0: 706c 6174 6509 0909 5370 7265 6164 7368  plate...Spreadsh
-000003e0: 6565 7420 4964 7a1a 3d3d 3d3d 3d3d 3d3d  eet Idz.========
-000003f0: 0909 093d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ...=============
-00000400: 3d3d 7201 0000 007a 0209 09da 0f73 7072  ==r....z.....spr
-00000410: 6561 6473 6865 6574 5f75 726c a901 da08  eadsheet_url....
-00000420: 6661 6c6c 6261 636b da01 0a7a 1165 2920  fallback...z.e) 
-00000430: 4564 6974 2065 7869 7374 696e 6720 7a07  Edit existing z.
-00000440: 6e29 204e 6577 207a 0a64 2920 4465 6c65  n) New z.d) Dele
-00000450: 7465 207a 0771 2920 7175 6974 2904 da01  te z.q) quit)...
-00000460: 65da 016e da01 64da 0171 7a0a 652f 6e2f  e..n..d..qz.e/n/
-00000470: 642f 7120 3e20 7a47 5468 6973 2076 616c  d/q > zGThis val
-00000480: 7565 206d 7573 7420 6265 2061 2073 696e  ue must be a sin
-00000490: 676c 6520 6368 6172 6163 7465 722c 206f  gle character, o
-000004a0: 6e65 206f 6620 7468 6520 666f 6c6c 6f77  ne of the follow
-000004b0: 696e 673a 2065 2c20 6e2c 2064 2c20 7129  ing: e, n, d, q)
-000004c0: 09da 0570 7269 6e74 da03 6c65 6eda 0b72  ...print..len..r
-000004d0: 6561 645f 636f 6e66 6967 da08 7365 6374  ead_config..sect
-000004e0: 696f 6e73 da03 7374 7272 0500 0000 da03  ions..strr......
-000004f0: 6765 7472 0700 0000 da05 696e 7075 7429  getr......input)
-00000500: 0472 0900 0000 da14 7465 6d70 6c61 7465  .r......template
-00000510: 5f66 6f6c 6465 725f 6e61 6d65 da12 6163  _folder_name..ac
-00000520: 6365 7074 6162 6c65 5f63 686f 6963 6573  ceptable_choices
-00000530: da0d 6163 7469 6f6e 5f63 686f 6963 6572  ..action_choicer
-00000540: 0a00 0000 720a 0000 0072 0b00 0000 da0d  ....r....r......
-00000550: 7365 6c65 6374 5f61 6374 696f 6e0f 0000  select_action...
-00000560: 0073 2400 0000 0802 0801 0801 1402 1001  .s$.............
-00000570: 2a01 0802 1001 1001 1001 0801 0802 0801  *...............
-00000580: 0801 0801 0801 08fe 0403 7a1b 436f 6e66  ..........z.Conf
-00000590: 6967 7572 6174 696f 6e2e 7365 6c65 6374  iguration.select
-000005a0: 5f61 6374 696f 6eda 0a61 6374 5f63 686f  _action..act_cho
-000005b0: 6963 65da 0672 6574 7572 6e63 0200 0000  ice..returnc....
-000005c0: 0000 0000 0000 0000 0600 0000 0800 0000  ................
-000005d0: 4300 0000 7346 0100 0064 007d 027c 0164  C...sF...d.}.|.d
-000005e0: 016b 0272 0909 007c 0253 007c 0164 0276  .k.r...|.S.|.d.v
-000005f0: 0072 9474 007c 00a0 01a1 00a0 02a1 0083  .r.t.|..........
-00000600: 0164 036b 0472 9474 0364 047c 006a 049b  .d.k.r.t.d.|.j..
-00000610: 0064 059d 0383 0101 0074 0364 0683 0101  .d.......t.d....
-00000620: 0074 057c 00a0 01a1 00a0 02a1 0083 0144  .t.|...........D
-00000630: 005d 0c5c 027d 037d 0474 037c 0364 0717  .].\.}.}.t.|.d..
-00000640: 0064 087c 0483 0301 0071 2c64 0964 0a84  .d.|.....q,d.d..
-00000650: 007c 00a0 01a1 00a0 02a1 0044 0083 017d  .|.........D...}
-00000660: 057c 05a0 0664 0b64 0a84 0074 0764 0774  .|...d.d...t.d.t
-00000670: 007c 00a0 01a1 00a0 02a1 0083 0164 0717  .|...........d..
-00000680: 0064 0783 0344 0083 01a1 0101 0074 087c  .d...D.......t.|
-00000690: 006a 04a0 09a1 009b 0064 0c9d 0283 017d  .j.......d.....}
-000006a0: 027c 027c 0576 0172 7a74 0364 0d83 0101  .|.|.v.rzt.d....
-000006b0: 0074 087c 006a 04a0 09a1 009b 0064 0c9d  .t.|.j.......d..
-000006c0: 0283 017d 027c 027c 0576 0173 687a 0f7c  ...}.|.|.v.shz.|
-000006d0: 00a0 01a1 00a0 02a1 0074 0a7c 0283 0164  .........t.|...d
-000006e0: 0718 0019 007d 0257 007c 0253 0004 0074  .....}.W.|.S...t
-000006f0: 0b79 9301 0001 0001 0059 007c 0253 0077  .y.......Y.|.S.w
-00000700: 007c 0164 0e6b 0272 a174 0864 0f7c 006a  .|.d.k.r.t.d.|.j
-00000710: 049b 0064 109d 0383 017d 027c 0253 0029  ...d.....}.|.S.)
-00000720: 114e 7214 0000 0029 0272 1100 0000 7213  .Nr....).r....r.
-00000730: 0000 0072 0100 0000 7a08 0a53 656c 6563  ...r....z..Selec
-00000740: 7420 da01 2e7a 3943 686f 6f73 6520 6120  t ...z9Choose a 
-00000750: 6e75 6d62 6572 2066 726f 6d20 6265 6c6f  number from belo
-00000760: 772c 206f 7220 7479 7065 2069 6e20 616e  w, or type in an
-00000770: 2065 7869 7374 696e 6720 7661 6c75 652e   existing value.
-00000780: e901 0000 007a 023e 2063 0100 0000 0000  .....z.> c......
-00000790: 0000 0000 0000 0200 0000 0300 0000 5300  ..............S.
-000007a0: 0000 7310 0000 0067 007c 005d 047d 017c  ..s....g.|.].}.|
-000007b0: 0191 0271 0253 0072 0a00 0000 720a 0000  ...q.S.r....r...
-000007c0: 0029 02da 022e 30da 0d63 6f6e 665f 7661  .)....0..conf_va
-000007d0: 7269 6162 6c65 720a 0000 0072 0a00 0000  riabler....r....
-000007e0: 720b 0000 00da 0a3c 6c69 7374 636f 6d70  r......<listcomp
-000007f0: 3e33 0000 0073 0200 0000 1000 7a31 436f  >3...s......z1Co
-00000800: 6e66 6967 7572 6174 696f 6e2e 7365 6c65  nfiguration.sele
-00000810: 6374 5f74 656d 706c 6174 652e 3c6c 6f63  ct_template.<loc
-00000820: 616c 733e 2e3c 6c69 7374 636f 6d70 3e63  als>.<listcomp>c
-00000830: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000840: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
-00000850: 005d 067d 0174 007c 0183 0191 0271 0253  .].}.t.|.....q.S
-00000860: 0072 0a00 0000 2901 7219 0000 0029 0272  .r....).r....).r
-00000870: 2400 0000 da05 696e 6465 7872 0a00 0000  $.....indexr....
-00000880: 720a 0000 0072 0b00 0000 7226 0000 0034  r....r....r&...4
-00000890: 0000 0073 0200 0000 1400 7a03 203e 207a  ...s......z. > z
-000008a0: 1b4e 6f20 6368 6f69 6365 7320 7769 7468  .No choices with
-000008b0: 2079 6f75 7220 696e 7075 742e 7212 0000   your input.r...
-000008c0: 007a 130a 456e 7465 7220 6e61 6d65 206f  .z..Enter name o
-000008d0: 6620 6e65 7720 7a08 2e0a 6e61 6d65 3a20  f new z...name: 
-000008e0: 290c 7216 0000 0072 1700 0000 7218 0000  ).r....r....r...
-000008f0: 0072 1500 0000 7207 0000 00da 0965 6e75  .r....r......enu
-00000900: 6d65 7261 7465 da06 6578 7465 6e64 da05  merate..extend..
-00000910: 7261 6e67 6572 1b00 0000 da05 7469 746c  ranger......titl
-00000920: 65da 0369 6e74 da0a 5661 6c75 6545 7272  e..int..ValueErr
-00000930: 6f72 2906 7209 0000 0072 2000 0000 5a0a  or).r....r ...Z.
-00000940: 7470 6c5f 6368 6f69 6365 7227 0000 0072  tpl_choicer'...r
-00000950: 2500 0000 721d 0000 0072 0a00 0000 720a  %...r....r....r.
-00000960: 0000 0072 0b00 0000 da0f 7365 6c65 6374  ...r......select
-00000970: 5f74 656d 706c 6174 6526 0000 0073 3400  _template&...s4.
-00000980: 0000 0401 0802 0201 0418 1cea 1201 0801  ................
-00000990: 1802 1201 1602 2c01 1401 0802 0801 1401  ......,.........
-000009a0: 08fe 0203 1a01 0407 0cfa 0201 0405 02fa  ................
-000009b0: 0803 1201 0402 7a1d 436f 6e66 6967 7572  ......z.Configur
-000009c0: 6174 696f 6e2e 7365 6c65 6374 5f74 656d  ation.select_tem
-000009d0: 706c 6174 65fa 0d74 656d 706c 6174 652e  plate..template.
-000009e0: 636f 6e66 da0b 636f 6e66 6967 5f66 696c  conf..config_fil
-000009f0: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
-00000a00: 0000 0400 0000 4300 0000 732c 0000 0074  ......C...s,...t
-00000a10: 006a 01a0 0274 036a 047c 01a1 027d 017c  .j...t.j.|...}.|
-00000a20: 00a0 057c 01a1 017c 005f 0174 06a0 077c  ...|...|._.t...|
-00000a30: 006a 01a1 0101 0074 0653 0072 0800 0000  .j.....t.S.r....
-00000a40: 2908 da02 6f73 da04 7061 7468 da04 6a6f  )...os..path..jo
-00000a50: 696e 7204 0000 00da 0d63 6f6e 6669 675f  inr......config_
-00000a60: 666f 6c64 6572 da10 636f 6e66 6967 5f66  folder..config_f
-00000a70: 696c 655f 7061 7468 da04 636f 6e66 da04  ile_path..conf..
-00000a80: 7265 6164 a902 7209 0000 0072 3000 0000  read..r....r0...
-00000a90: 720a 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
-00000aa0: 1700 0000 4400 0000 7308 0000 0010 010c  ....D...s.......
-00000ab0: 010c 0104 017a 1943 6f6e 6669 6775 7261  .....z.Configura
-00000ac0: 7469 6f6e 2e72 6561 645f 636f 6e66 6967  tion.read_config
-00000ad0: da00 721e 0000 00da 0f74 656d 706c 6174  ..r......templat
-00000ae0: 655f 6368 6f69 6365 6304 0000 0000 0000  e_choicec.......
-00000af0: 0000 0000 0006 0000 0008 0000 0043 0000  .............C..
-00000b00: 0073 2a01 0000 7400 6a01 a002 7403 6a04  .s*...t.j...t.j.
-00000b10: 7c01 a102 7d01 7c00 a005 7c01 a101 7d04  |...}.|...|...}.
-00000b20: 7406 a007 7c04 a101 0100 7c02 6401 6b02  t...|.....|.d.k.
-00000b30: 724c 7408 7c00 a009 a100 a00a a100 8301  rLt.|...........
-00000b40: 6402 6b04 724c 7406 a00b 7c03 a101 0100  d.k.rLt...|.....
-00000b50: 740c 7c04 6403 8302 8f0d 7d05 7406 a00d  t.|.d.....}.t...
-00000b60: 7c05 a101 0100 5700 6400 0400 0400 8303  |.....W.d.......
-00000b70: 0100 6e08 3100 733a 7701 0100 0100 0100  ..n.1.s:w.......
-00000b80: 5900 0100 740e a00f 7400 6a01 a002 7403  Y...t...t.j...t.
-00000b90: 6a10 7c03 a102 a101 0100 6400 5300 7c02  j.|.......d.S.|.
-00000ba0: 6404 7600 7284 7c02 6405 6b02 7262 7406  d.v.r.|.d.k.rbt.
-00000bb0: a011 7c03 a101 0100 7c00 6a12 7c03 7c02  ..|.....|.j.|.|.
-00000bc0: 6406 8d02 0100 6400 5300 7c02 6407 6b02  d.....d.S.|.d.k.
-00000bd0: 7279 7408 7c00 a009 a100 a00a a100 8301  ryt.|...........
-00000be0: 6402 6b04 7279 7c00 6a12 7c03 7c02 6406  d.k.ry|.j.|.|.d.
-00000bf0: 8d02 0100 6400 5300 7413 6408 7c00 6a14  ....d.S.t.d.|.j.
-00000c00: 9b00 6409 9d03 8301 0100 6400 5300 7c02  ..d.......d.S.|.
-00000c10: 640a 6b02 728a 6400 5300 7413 6408 7c00  d.k.r.d.S.t.d.|.
-00000c20: 6a14 9b00 640b 9d03 8301 0100 6400 5300  j...d.......d.S.
-00000c30: 290c 4e72 1300 0000 7201 0000 00da 0177  ).Nr....r......w
-00000c40: 2902 7211 0000 0072 1200 0000 7212 0000  ).r....r....r...
-00000c50: 0029 0272 3a00 0000 721e 0000 0072 1100  .).r:...r....r..
-00000c60: 0000 7a03 4e6f 207a 0920 746f 2065 6469  ..z.No z. to edi
-00000c70: 7421 7214 0000 007a 0b20 746f 2064 656c  t!r....z. to del
-00000c80: 6574 6521 2915 7231 0000 0072 3200 0000  ete!).r1...r2...
-00000c90: 7233 0000 0072 0400 0000 7234 0000 0072  r3...r....r4...r
-00000ca0: 3500 0000 7236 0000 0072 3700 0000 7216  5...r6...r7...r.
-00000cb0: 0000 0072 1700 0000 7218 0000 00da 0e72  ...r....r......r
-00000cc0: 656d 6f76 655f 7365 6374 696f 6eda 046f  emove_section..o
-00000cd0: 7065 6eda 0577 7269 7465 da06 7368 7574  pen..write..shut
-00000ce0: 696c da06 726d 7472 6565 da0f 7465 6d70  il..rmtree..temp
-00000cf0: 6c61 7465 5f66 6f6c 6465 72da 0b61 6464  late_folder..add
-00000d00: 5f73 6563 7469 6f6e da0b 6d61 696e 5f63  _section..main_c
-00000d10: 6f6e 6669 6772 1500 0000 7207 0000 0029  onfigr....r....)
-00000d20: 0672 0900 0000 7230 0000 0072 1e00 0000  .r....r0...r....
-00000d30: 723a 0000 0072 3200 0000 da0a 636f 6e66  r:...r2.....conf
-00000d40: 6967 6669 6c65 720a 0000 0072 0a00 0000  igfiler....r....
-00000d50: 720b 0000 00da 0c77 7269 7465 5f63 6f6e  r......write_con
-00000d60: 6669 674a 0000 0073 2600 0000 1001 0a01  figJ...s&.......
-00000d70: 0a01 1c02 0a01 0c01 0c01 1cff 1a04 0802  ................
-00000d80: 0801 0a01 1201 1c01 1201 1602 0802 0401  ................
-00000d90: 1603 7a1a 436f 6e66 6967 7572 6174 696f  ..z.Configuratio
-00000da0: 6e2e 7772 6974 655f 636f 6e66 6967 6302  n.write_configc.
-00000db0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000dc0: 0000 0043 0000 0073 1400 0000 7400 6a01  ...C...s....t.j.
-00000dd0: a002 7403 6a04 7c01 a102 7d01 7c01 5300  ..t.j.|...}.|.S.
-00000de0: 7208 0000 0029 0572 3100 0000 7232 0000  r....).r1...r2..
-00000df0: 0072 3300 0000 7204 0000 0072 3400 0000  .r3...r....r4...
-00000e00: 7238 0000 0072 0a00 0000 720a 0000 0072  r8...r....r....r
-00000e10: 0b00 0000 7235 0000 0067 0000 0073 0400  ....r5...g...s..
-00000e20: 0000 1001 0401 7a1e 436f 6e66 6967 7572  ......z.Configur
-00000e30: 6174 696f 6e2e 636f 6e66 6967 5f66 696c  ation.config_fil
-00000e40: 655f 7061 7468 721c 0000 0063 0300 0000  e_pathr....c....
-00000e50: 0000 0000 0000 0000 0700 0000 0800 0000  ................
-00000e60: 4300 0000 7370 0100 007c 0164 016b 0273  C...sp...|.d.k.s
-00000e70: 087c 0164 026b 0272 b674 006a 017c 0264  .|.d.k.r.t.j.|.d
-00000e80: 0364 0064 048d 037d 0374 0264 057c 039b  .d.d...}.t.d.|..
-00000e90: 0064 069d 0383 017d 0474 0374 046a 05a0  .d.....}.t.t.j..
-00000ea0: 067c 04a0 0764 0764 08a1 02a1 0183 0101  .|...d.d........
-00000eb0: 0074 046a 05a0 067c 04a0 0764 0764 08a1  .t.j...|...d.d..
-00000ec0: 02a1 0173 5074 087c 0483 0164 096b 0472  ...sPt.|...d.k.r
-00000ed0: 5074 0364 0a83 0101 0074 0264 0b7c 039b  Pt.d.....t.d.|..
-00000ee0: 0064 069d 0383 017d 0474 046a 05a0 067c  .d.....}.t.j...|
-00000ef0: 04a0 0764 0764 08a1 02a1 0173 5074 087c  ...d.d.....sPt.|
-00000f00: 0483 0164 096b 0473 347c 04a0 0764 0764  ...d.k.s4|...d.d
-00000f10: 08a1 027d 0474 087c 0483 0164 096b 0272  ...}.t.|...d.k.r
-00000f20: 5e7c 036e 017c 047d 0474 046a 05a0 0974  ^|.n.|.}.t.j...t
-00000f30: 0a6a 0b7c 02a1 027d 057a 1074 0ca0 0d7c  .j.|...}.z.t...|
-00000f40: 047c 05a1 0201 0074 0364 0c7c 059b 0064  .|.....t.d.|...d
-00000f50: 0d9d 0383 0101 0057 006e 1204 0074 0c6a  .......W.n...t.j
-00000f60: 0e79 8201 0001 0001 0059 006e 0904 0074  .y.......Y.n...t
-00000f70: 0f79 8a01 0001 0001 0059 006e 0177 0074  .y.......Y.n.w.t
-00000f80: 00a0 107c 0264 037c 05a1 0301 007c 00a0  ...|.d.|.....|..
-00000f90: 1164 0ea1 017c 005f 0574 127c 006a 0564  .d...|._.t.|.j.d
-00000fa0: 0f83 028f 0e7d 0674 00a0 137c 06a1 0101  .....}.t...|....
-00000fb0: 0057 0064 0004 0004 0083 0301 0064 0053  .W.d.........d.S
-00000fc0: 0031 0073 af77 0101 0001 0001 0059 0001  .1.s.w.......Y..
-00000fd0: 0064 0053 0064 0053 0029 104e 7212 0000  .d.S.d.S.).Nr...
-00000fe0: 0072 1100 0000 da13 7465 6d70 6c61 7465  .r......template
-00000ff0: 5f66 6f6c 6465 725f 6469 7272 0e00 0000  _folder_dirr....
-00001000: 7a76 0a54 656d 706c 6174 6520 666f 6c64  zv.Template fold
-00001010: 6572 2e0a 5468 6520 6669 6c65 2070 6174  er..The file pat
-00001020: 6820 6f66 2074 6865 2048 544d 4c20 656d  h of the HTML em
-00001030: 6169 6c20 7465 6d70 6c61 7465 2066 6f6c  ail template fol
-00001040: 6465 722e 0a45 6e74 6572 2061 2073 7472  der..Enter a str
-00001050: 696e 6720 7661 6c75 652e 2050 7265 7373  ing value. Press
-00001060: 2045 6e74 6572 2066 6f72 2074 6865 2064   Enter for the d
-00001070: 6566 6175 6c74 2028 fa03 293a 20fa 0122  efault (..): .."
-00001080: 7239 0000 0072 0100 0000 7a2b 506c 6561  r9...r....z+Plea
-00001090: 7365 2065 6e74 6572 2061 2076 616c 6964  se enter a valid
-000010a0: 2074 656d 706c 6174 6520 666f 6c64 6572   template folder
-000010b0: 2070 6174 683a 207a 6f0a 5465 6d70 6c61   path: zo.Templa
-000010c0: 7465 2066 6f6c 6465 722e 0a54 6865 2066  te folder..The f
-000010d0: 696c 6520 7061 7468 206f 6620 7468 6520  ile path of the 
-000010e0: 4854 4d4c 2065 6d61 696c 2074 656d 706c  HTML email templ
-000010f0: 6174 652e 0a45 6e74 6572 2061 2073 7472  ate..Enter a str
-00001100: 696e 6720 7661 6c75 652e 2050 7265 7373  ing value. Press
-00001110: 2045 6e74 6572 2066 6f72 2074 6865 2064   Enter for the d
-00001120: 6566 6175 6c74 2028 7a25 0a59 6f75 7220  efault (z%.Your 
-00001130: 6669 6c65 2069 7320 636f 7069 6564 2061  file is copied a
-00001140: 6e64 2075 706c 6f61 6465 6420 746f 2072  nd uploaded to r
-00001150: 2200 0000 722f 0000 0072 3b00 0000 2914  "...r/...r;...).
-00001160: 7236 0000 0072 1a00 0000 721b 0000 0072  r6...r....r....r
-00001170: 1500 0000 7231 0000 0072 3200 0000 da05  ....r1...r2.....
-00001180: 6973 6469 72da 0772 6570 6c61 6365 7216  isdir..replacer.
-00001190: 0000 0072 3300 0000 7204 0000 0072 4100  ...r3...r....rA.
-000011a0: 0000 723f 0000 00da 0863 6f70 7974 7265  ..r?.....copytre
-000011b0: 65da 0d53 616d 6546 696c 6545 7272 6f72  e..SameFileError
-000011c0: da0f 4669 6c65 4578 6973 7473 4572 726f  ..FileExistsErro
-000011d0: 72da 0373 6574 7235 0000 0072 3d00 0000  r..setr5...r=...
-000011e0: 723e 0000 0029 0772 0900 0000 721e 0000  r>...).r....r...
-000011f0: 0072 1c00 0000 7246 0000 005a 176e 6577  .r....rF...Z.new
-00001200: 5f74 656d 706c 6174 655f 666f 6c64 6572  _template_folder
-00001210: 5f64 6972 da0c 7465 6d70 6c61 7465 5f6c  _dir..template_l
-00001220: 6f63 7244 0000 0072 0a00 0000 720a 0000  ocrD...r....r...
-00001230: 0072 0b00 0000 da14 636f 7079 5f74 656d  .r......copy_tem
-00001240: 706c 6174 655f 666f 6c64 6572 6b00 0000  plate_folderk...
-00001250: 7332 0000 0010 0110 0110 0118 0120 0208  s2........... ..
-00001260: 0110 0120 fe0c 0314 0110 0402 030c 0114  ... ............
-00001270: 010e 0104 010c 0104 0102 ff0e 040c 010e  ................
-00001280: 010c 0122 ff04 e57a 2243 6f6e 6669 6775  ..."...z"Configu
-00001290: 7261 7469 6f6e 2e63 6f70 795f 7465 6d70  ration.copy_temp
-000012a0: 6c61 7465 5f66 6f6c 6465 72da 1174 656d  late_folder..tem
-000012b0: 706c 6174 655f 7365 6c65 6374 6564 6302  plate_selectedc.
-000012c0: 0000 0000 0000 0000 0000 0004 0000 0008  ................
-000012d0: 0000 0043 0000 0073 8400 0000 7400 6a01  ...C...s....t.j.
-000012e0: 7c01 6401 6400 6402 8d03 7c00 5f02 7403  |.d.d.d...|._.t.
-000012f0: 6403 7c00 6a02 9b00 6404 9d03 8301 7d02  d.|.j...d.....}.
-00001300: 7404 7c02 8301 6405 6b02 721b 7c00 6a02  t.|...d.k.r.|.j.
-00001310: 6e01 7c02 7d02 7400 a005 7c01 6401 7c02  n.|.}.t...|.d.|.
-00001320: a103 0100 7406 7c00 6a07 6406 8302 8f0e  ....t.|.j.d.....
-00001330: 7d03 7400 a008 7c03 a101 0100 5700 6400  }.t...|.....W.d.
-00001340: 0400 0400 8303 0100 6400 5300 3100 733b  ........d.S.1.s;
-00001350: 7701 0100 0100 0100 5900 0100 6400 5300  w.......Y...d.S.
-00001360: 2907 4e72 0d00 0000 720e 0000 007a 9f0a  ).Nr....r....z..
-00001370: 5370 7265 6164 7368 6565 7420 7572 6c2e  Spreadsheet url.
-00001380: 0a54 6865 2047 6f6f 676c 6520 7370 7265  .The Google spre
-00001390: 6164 7368 6565 7420 7572 6c20 7468 6174  adsheet url that
-000013a0: 2079 6f75 2077 616e 7420 746f 2070 6172   you want to par
-000013b0: 7365 2069 7420 746f 2074 6865 204a 696e  se it to the Jin
-000013c0: 6a61 3220 4854 4d4c 2065 6d61 696c 2074  ja2 HTML email t
-000013d0: 656d 706c 6174 653a 202e 0a45 6e74 6572  emplate: ..Enter
-000013e0: 2061 2073 7472 696e 6720 7661 6c75 652e   a string value.
-000013f0: 2050 7265 7373 2045 6e74 6572 2066 6f72   Press Enter for
-00001400: 2074 6865 2064 6566 6175 6c74 2028 7247   the default (rG
-00001410: 0000 0072 0100 0000 723b 0000 0029 0972  ...r....r;...).r
-00001420: 3600 0000 721a 0000 0072 0d00 0000 721b  6...r....r....r.
-00001430: 0000 0072 1600 0000 724e 0000 0072 3d00  ...r....rN...r=.
-00001440: 0000 7232 0000 0072 3e00 0000 2904 7209  ..r2...r>...).r.
-00001450: 0000 0072 5100 0000 5a13 6e65 775f 7370  ...rQ...Z.new_sp
-00001460: 7265 6164 7368 6565 745f 7572 6c72 4400  readsheet_urlrD.
-00001470: 0000 720a 0000 0072 0a00 0000 720b 0000  ..r....r....r...
-00001480: 00da 1173 6574 7570 5f53 7072 6561 6473  ...setup_Spreads
-00001490: 6865 6574 8a00 0000 730e 0000 0012 0112  heet....s.......
-000014a0: 0116 010e 010e 010c 0122 ff7a 1f43 6f6e  .........".z.Con
-000014b0: 6669 6775 7261 7469 6f6e 2e73 6574 7570  figuration.setup
-000014c0: 5f53 7072 6561 6473 6865 6574 6302 0000  _Spreadsheetc...
-000014d0: 0000 0000 0000 0000 000b 0000 0008 0000  ................
-000014e0: 0043 0000 0073 4401 0000 7400 6a01 7c01  .C...sD...t.j.|.
-000014f0: 6401 6402 6403 8d03 7d02 7402 6404 7c02  d.d.d...}.t.d.|.
-00001500: 9b00 6405 9d03 8301 7d03 7403 7c03 8301  ..d.....}.t.|...
-00001510: 6406 6b02 7218 7c02 6e01 7c03 7d03 7400  d.k.r.|.n.|.}.t.
-00001520: 6a01 7c01 6407 6400 6403 8d03 7d04 7402  j.|.d.d.d...}.t.
-00001530: 6408 7c04 9b00 6405 9d03 8301 7d05 7403  d.|...d.....}.t.
-00001540: 7c05 8301 6406 6b02 7232 7c04 6e01 7c05  |...d.k.r2|.n.|.
-00001550: 7d05 7400 6a01 7c01 6409 640a 6403 8d03  }.t.j.|.d.d.d...
-00001560: 7d06 7402 640b 7c06 9b00 6405 9d03 8301  }.t.d.|...d.....
-00001570: 7d07 7403 7c07 8301 6406 6b02 724c 7c06  }.t.|...d.k.rL|.
-00001580: 6e01 7c07 7d07 7400 6a01 7c01 640c 6400  n.|.}.t.j.|.d.d.
-00001590: 6403 8d03 7d08 7402 640d 7c08 9b00 6405  d...}.t.d.|...d.
-000015a0: 9d03 8301 7d09 7403 7c09 8301 6406 6b02  ....}.t.|...d.k.
-000015b0: 7266 7c08 6e01 7c09 7d09 7400 a004 7c01  rf|.n.|.}.t...|.
-000015c0: 6401 7c03 a103 0100 7400 a004 7c01 6409  d.|.....t...|.d.
-000015d0: 7c07 a103 0100 7400 a004 7c01 6407 7c05  |.....t...|.d.|.
-000015e0: a103 0100 7400 a004 7c01 640c 7c09 a103  ....t...|.d.|...
-000015f0: 0100 7405 7c00 6a06 640e 8302 8f0e 7d0a  ..t.|.j.d.....}.
-00001600: 7400 a007 7c0a a101 0100 5700 6400 0400  t...|.....W.d...
-00001610: 0400 8303 0100 6400 5300 3100 739b 7701  ......d.S.1.s.w.
-00001620: 0100 0100 0100 5900 0100 6400 5300 290f  ......Y...d.S.).
-00001630: 4eda 1d77 6f72 6b73 6865 6574 5f74 6974  N..worksheet_tit
-00001640: 6c65 5f63 616d 7061 6967 6e5f 696e 666f  le_campaign_info
-00001650: 7a0d 4361 6d70 6169 676e 2049 6e66 6f72  z.Campaign Infor
-00001660: 0e00 0000 7aa0 0a57 6f72 6b73 6865 6574  ....z..Worksheet
-00001670: 2054 6974 6c65 206f 6620 4361 6d70 6169   Title of Campai
-00001680: 676e 2049 6e66 6f2e 0a54 6865 2077 6f72  gn Info..The wor
-00001690: 6b73 6865 6574 2074 6974 6c65 206f 6620  ksheet title of 
-000016a0: 6361 6d70 6169 676e 2069 6e66 6f3a 202e  campaign info: .
-000016b0: 0a45 6e74 6572 2061 2073 6572 6965 7320  .Enter a series 
-000016c0: 6f66 2063 656c 6c20 7261 6e67 6573 2c20  of cell ranges, 
-000016d0: 7365 7061 7261 7465 6420 6279 2073 796d  separated by sym
-000016e0: 626f 6c20 282c 292e 2050 7265 7373 2045  bol (,). Press E
-000016f0: 6e74 6572 2066 6f72 2074 6865 2064 6566  nter for the def
-00001700: 6175 6c74 2028 7247 0000 0072 0100 0000  ault (rG...r....
-00001710: da0d 6361 6d70 6169 676e 5f69 6e66 6f7a  ..campaign_infoz
-00001720: b60a 4361 6d70 6169 676e 2049 6e66 6f2e  ..Campaign Info.
-00001730: 0a54 6865 2043 616d 7061 6967 6e20 696e  .The Campaign in
-00001740: 666f 2074 6861 7420 796f 7520 7761 6e74  fo that you want
-00001750: 2074 6f20 7061 7273 6520 6974 2074 6f20   to parse it to 
-00001760: 7468 6520 4a69 6e6a 6132 2048 544d 4c20  the Jinja2 HTML 
-00001770: 656d 6169 6c20 7465 6d70 6c61 7465 3a20  email template: 
-00001780: 2e0a 456e 7465 7220 6120 7365 7269 6573  ..Enter a series
-00001790: 206f 6620 6365 6c6c 2072 616e 6765 732c   of cell ranges,
-000017a0: 2073 6570 6172 6174 6564 2062 7920 7379   separated by sy
-000017b0: 6d62 6f6c 2028 2c29 2e20 5072 6573 7320  mbol (,). Press 
-000017c0: 456e 7465 7220 666f 7220 7468 6520 6465  Enter for the de
-000017d0: 6661 756c 7420 28da 2077 6f72 6b73 6865  fault (. workshe
-000017e0: 6574 5f74 6974 6c65 5f63 616d 7061 6967  et_title_campaig
-000017f0: 6e5f 636f 6e74 656e 747a 1043 616d 7061  n_contentz.Campa
-00001800: 6967 6e20 436f 6e74 656e 747a a60a 576f  ign Contentz..Wo
-00001810: 726b 7368 6565 7420 5469 746c 6520 6f66  rksheet Title of
-00001820: 2043 616d 7061 6967 6e20 436f 6e74 656e   Campaign Conten
-00001830: 742e 0a54 6865 2077 6f72 6b73 6865 6574  t..The worksheet
-00001840: 2074 6974 6c65 206f 6620 6361 6d70 6169   title of campai
-00001850: 676e 2063 6f6e 7465 6e74 3a20 2e0a 456e  gn content: ..En
-00001860: 7465 7220 6120 7365 7269 6573 206f 6620  ter a series of 
-00001870: 6365 6c6c 2072 616e 6765 732c 2073 6570  cell ranges, sep
-00001880: 6172 6174 6564 2062 7920 7379 6d62 6f6c  arated by symbol
-00001890: 2028 2c29 2e20 5072 6573 7320 456e 7465   (,). Press Ente
-000018a0: 7220 666f 7220 7468 6520 6465 6661 756c  r for the defaul
-000018b0: 7420 28da 1063 616d 7061 6967 6e5f 636f  t (..campaign_co
-000018c0: 6e74 656e 747a bb0a 4361 6d70 6169 676e  ntentz..Campaign
-000018d0: 2043 6f6e 7465 6e74 2e0a 5468 6520 4361   Content..The Ca
-000018e0: 6d70 6169 676e 2043 6f6e 7465 6e74 2074  mpaign Content t
-000018f0: 6861 7420 796f 7520 7761 6e74 2074 6f20  hat you want to 
-00001900: 7061 7373 2069 7420 746f 2074 6865 204a  pass it to the J
-00001910: 696e 6a61 3220 4854 4d4c 2065 6d61 696c  inja2 HTML email
-00001920: 2074 656d 706c 6174 653a 202e 0a45 6e74   template: ..Ent
-00001930: 6572 2061 2073 6572 6965 7320 6f66 2063  er a series of c
-00001940: 656c 6c20 7261 6e67 6573 2c20 7365 7061  ell ranges, sepa
-00001950: 7261 7465 6420 6279 2073 796d 626f 6c20  rated by symbol 
-00001960: 282c 292e 2050 7265 7373 2045 6e74 6572  (,). Press Enter
-00001970: 2066 6f72 2074 6865 2064 6566 6175 6c74   for the default
-00001980: 2028 723b 0000 0029 0872 3600 0000 721a   (r;...).r6...r.
-00001990: 0000 0072 1b00 0000 7216 0000 0072 4e00  ...r....r....rN.
-000019a0: 0000 723d 0000 0072 3200 0000 723e 0000  ..r=...r2...r>..
-000019b0: 0029 0b72 0900 0000 7251 0000 0072 5300  .).r....rQ...rS.
-000019c0: 0000 5a21 6e65 775f 776f 726b 7368 6565  ..Z!new_workshee
-000019d0: 745f 7469 746c 655f 6361 6d70 6169 676e  t_title_campaign
-000019e0: 5f69 6e66 6f72 5400 0000 5a11 6e65 775f  _inforT...Z.new_
-000019f0: 6361 6d70 6169 676e 5f69 6e66 6f72 5500  campaign_inforU.
-00001a00: 0000 5a24 6e65 775f 776f 726b 7368 6565  ..Z$new_workshee
-00001a10: 745f 7469 746c 655f 6361 6d70 6169 676e  t_title_campaign
-00001a20: 5f63 6f6e 7465 6e74 7256 0000 005a 146e  _contentrV...Z.n
-00001a30: 6577 5f63 616d 7061 6967 6e5f 636f 6e74  ew_campaign_cont
-00001a40: 656e 7472 4400 0000 720a 0000 0072 0a00  entrD...r....r..
-00001a50: 0000 720b 0000 00da 0e73 6574 7570 5f63  ..r......setup_c
-00001a60: 616d 7061 6967 6e92 0000 0073 2600 0000  ampaign....s&...
-00001a70: 1001 1001 1401 1002 1001 1401 1002 1001  ................
-00001a80: 1401 1002 1001 1401 0e02 0e01 0e01 0e01  ................
-00001a90: 0e01 0c01 22ff 7a1c 436f 6e66 6967 7572  ....".z.Configur
-00001aa0: 6174 696f 6e2e 7365 7475 705f 6361 6d70  ation.setup_camp
-00001ab0: 6169 676e 6301 0000 0000 0000 0000 0000  aignc...........
-00001ac0: 0003 0000 0004 0000 0043 0000 0073 2e00  .........C...s..
-00001ad0: 0000 7400 a001 a100 0100 7c00 a002 a100  ..t.......|.....
-00001ae0: 7d01 7c00 6a03 7c01 6401 8d01 7d02 7c00  }.|.j.|.d...}.|.
-00001af0: 6a04 7c01 7c02 6402 8d02 0100 6400 5300  j.|.|.d.....d.S.
-00001b00: 2903 4e29 0172 2000 0000 2902 721e 0000  ).N).r ...).r...
-00001b10: 0072 3a00 0000 2905 7204 0000 00da 0a63  .r:...).r......c
-00001b20: 7265 6174 655f 6469 7272 1f00 0000 722e  reate_dirr....r.
-00001b30: 0000 0072 4500 0000 2903 7209 0000 00da  ...rE...).r.....
-00001b40: 0f61 6374 696f 6e5f 7365 6c65 6374 6564  .action_selected
-00001b50: 7251 0000 0072 0a00 0000 720a 0000 0072  rQ...r....r....r
-00001b60: 0b00 0000 da0b 636f 6e66 6967 5f70 6167  ......config_pag
-00001b70: 65aa 0000 0073 0800 0000 0801 0801 0c02  e....s..........
-00001b80: 1202 7a19 436f 6e66 6967 7572 6174 696f  ..z.Configuratio
-00001b90: 6e2e 636f 6e66 6967 5f70 6167 6563 0300  n.config_pagec..
-00001ba0: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00001bb0: 0000 4300 0000 732a 0000 007c 006a 007c  ..C...s*...|.j.|
-00001bc0: 017c 0264 018d 0201 007c 006a 017c 0164  .|.d.....|.j.|.d
-00001bd0: 028d 0101 007c 006a 027c 0164 028d 0101  .....|.j.|.d....
-00001be0: 0064 0053 0029 034e 2902 721c 0000 0072  .d.S.).N).r....r
-00001bf0: 1e00 0000 2901 7251 0000 0029 0372 5000  ....).rQ...).rP.
-00001c00: 0000 7252 0000 0072 5700 0000 2903 7209  ..rR...rW...).r.
-00001c10: 0000 0072 3a00 0000 721e 0000 0072 0a00  ...r:...r....r..
-00001c20: 0000 720a 0000 0072 0b00 0000 7243 0000  ..r....r....rC..
-00001c30: 00b2 0000 0073 0600 0000 0e02 0c03 1003  .....s..........
-00001c40: 7a19 436f 6e66 6967 7572 6174 696f 6e2e  z.Configuration.
-00001c50: 6d61 696e 5f63 6f6e 6669 674e 2901 722f  main_configN).r/
-00001c60: 0000 0029 0372 2f00 0000 7239 0000 0072  ...).r/...r9...r
-00001c70: 3900 0000 2911 da08 5f5f 6e61 6d65 5f5f  9...)...__name__
-00001c80: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00001c90: 7175 616c 6e61 6d65 5f5f 7219 0000 0072  qualname__r....r
-00001ca0: 0c00 0000 721f 0000 0072 2e00 0000 da04  ....r....r......
-00001cb0: 7479 7065 7202 0000 0072 1700 0000 7245  typer....r....rE
-00001cc0: 0000 0072 3500 0000 7250 0000 0072 5200  ...r5...rP...rR.
-00001cd0: 0000 7257 0000 0072 5a00 0000 7243 0000  ..rW...rZ...rC..
-00001ce0: 0072 0a00 0000 720a 0000 0072 0a00 0000  .r....r....r....
-00001cf0: 720b 0000 0072 0600 0000 0b00 0000 7318  r....r........s.
-00001d00: 0000 0008 000e 0108 0312 1718 1e18 0618  ................
-00001d10: 1d12 040e 1f0e 0808 1816 0872 0600 0000  ...........r....
-00001d20: 290d da0c 636f 6e66 6967 7061 7273 6572  )...configparser
-00001d30: 7202 0000 00da 0b67 656e 6572 6963 7061  r......genericpa
-00001d40: 7468 7203 0000 0072 3100 0000 723f 0000  thr....r1...r?..
-00001d50: 00da 166d 6169 6c63 6869 6d70 5f61 7574  ...mailchimp_aut
-00001d60: 6f2e 7363 7269 7074 7372 0400 0000 5a0d  o.scriptsr....Z.
-00001d70: 6773 7072 6561 642e 7574 696c 7372 0500  gspread.utilsr..
-00001d80: 0000 da07 6c6f 6767 696e 6772 3600 0000  ....loggingr6...
-00001d90: 7206 0000 0072 0a00 0000 720a 0000 0072  r....r....r....r
-00001da0: 0a00 0000 720b 0000 00da 083c 6d6f 6475  ....r......<modu
-00001db0: 6c65 3e01 0000 0073 1200 0000 0c00 0c01  le>....s........
-00001dc0: 0801 0801 0c01 0c01 0801 0602 1202       ..............
+000000e0: 0000 0000 0000 0000 0500 0000 4000 0000  ............@...
+000000f0: 73b6 0000 0065 005a 0164 005a 0265 0364  s....e.Z.d.Z.e.d
+00000100: 019c 0164 0264 0384 045a 0464 0464 0584  ...d.d...Z.d.d..
+00000110: 005a 0565 0365 0364 069c 0264 0764 0884  .Z.e.e.d...d.d..
+00000120: 045a 0664 2165 0365 0765 0819 0064 0a9c  .Z.d!e.e.e...d..
+00000130: 0264 0b64 0c84 055a 0964 2265 0365 0365  .d.d...Z.d"e.e.e
+00000140: 0364 0e9c 0364 0f64 1084 055a 0a64 2365  .d...d.d...Z.d#e
+00000150: 0365 0765 0819 0064 0a9c 0264 1164 1284  .e.e...d...d.d..
+00000160: 055a 0b65 0365 0364 139c 0264 1464 1584  .Z.e.e.d...d.d..
+00000170: 045a 0c65 0364 169c 0164 1764 1884 045a  .Z.e.d...d.d...Z
+00000180: 0d65 0364 169c 0164 1964 1a84 045a 0e64  .e.d...d.d...Z.d
+00000190: 1b64 1c84 005a 0f65 0365 0364 1d9c 0264  .d...Z.e.e.d...d
+000001a0: 1e64 1f84 045a 1064 2053 0029 24da 0d43  .d...Z.d S.)$..C
+000001b0: 6f6e 6669 6775 7261 7469 6f6e a901 da07  onfiguration....
+000001c0: 7375 626a 6563 7463 0200 0000 0000 0000  subjectc........
+000001d0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+000001e0: 730a 0000 007c 017c 005f 0064 0053 00a9  s....|.|._.d.S..
+000001f0: 014e 7207 0000 0029 02da 0473 656c 6672  .Nr....)...selfr
+00000200: 0800 0000 a900 720b 0000 00fa 6f43 3a5c  ......r.....oC:\
+00000210: 5573 6572 735c 796f 6e67 7368 656e 672e  Users\yongsheng.
+00000220: 7461 6e5c 446f 6375 6d65 6e74 735c 436f  tan\Documents\Co
+00000230: 6469 6e67 5c67 6974 6875 622d 7072 6f6a  ding\github-proj
+00000240: 6563 745c 6d61 696c 6368 696d 705f 6175  ect\mailchimp_au
+00000250: 746f 5c6d 6169 6c63 6869 6d70 5f61 7574  to\mailchimp_aut
+00000260: 6f5c 7363 7269 7074 735c 7465 6d70 6c61  o\scripts\templa
+00000270: 7465 5f43 6f6e 6669 672e 7079 da08 5f5f  te_Config.py..__
+00000280: 696e 6974 5f5f 0c00 0000 7302 0000 0000  init__....s.....
+00000290: 017a 1643 6f6e 6669 6775 7261 7469 6f6e  .z.Configuration
+000002a0: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
+000002b0: 0000 0000 0000 0400 0000 0b00 0000 4300  ..............C.
+000002c0: 0000 73d4 0000 0074 0064 0183 0101 0074  ..s....t.d.....t
+000002d0: 0064 0283 0101 0074 0064 0383 0101 0074  .d.....t.d.....t
+000002e0: 017c 00a0 02a1 00a0 03a1 0083 0164 046b  .|...........d.k
+000002f0: 0472 667c 00a0 02a1 00a0 03a1 0044 005d  .rf|.........D.]
+00000300: 2c7d 0174 0074 047c 0183 0164 0574 0574  ,}.t.t.|...d.t.t
+00000310: 047c 00a0 02a1 006a 067c 0164 0664 0064  .|.....j.|.d.d.d
+00000320: 078d 0383 0183 0183 0301 0071 3874 0064  ...........q8t.d
+00000330: 0883 0101 0074 0064 097c 006a 079b 009d  .....t.d.|.j....
+00000340: 0283 0101 0074 0064 0a7c 006a 079b 009d  .....t.d.|.j....
+00000350: 0283 0101 0074 0064 0b7c 006a 079b 009d  .....t.d.|.j....
+00000360: 0283 0101 0074 0064 0c83 0101 0067 0064  .....t.d.....g.d
+00000370: 0da2 017d 0274 0864 0e83 017d 037c 037c  ...}.t.d...}.|.|
+00000380: 0276 0172 d074 0064 0f83 0101 0074 0864  .v.r.t.d.....t.d
+00000390: 0e83 017d 0371 b67c 0353 0029 104e 7a14  ...}.q.|.S.).Nz.
+000003a0: 4375 7272 656e 7420 7465 6d70 6c61 7465  Current template
+000003b0: 2873 293a 7a19 5465 6d70 6c61 7465 0909  (s):z.Template..
+000003c0: 0953 7072 6561 6473 6865 6574 2049 647a  .Spreadsheet Idz
+000003d0: 1a3d 3d3d 3d3d 3d3d 3d09 0909 3d3d 3d3d  .========...====
+000003e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d72 0100 0000  ===========r....
+000003f0: 7a02 0909 da0f 7370 7265 6164 7368 6565  z.....spreadshee
+00000400: 745f 7572 6ca9 01da 0866 616c 6c62 6163  t_url....fallbac
+00000410: 6bda 010a 7a11 6529 2045 6469 7420 6578  k...z.e) Edit ex
+00000420: 6973 7469 6e67 207a 076e 2920 4e65 7720  isting z.n) New 
+00000430: 7a0a 6429 2044 656c 6574 6520 7a07 7129  z.d) Delete z.q)
+00000440: 2071 7569 7429 04da 0165 da01 6eda 0164   quit)...e..n..d
+00000450: da01 717a 0a65 2f6e 2f64 2f71 203e 207a  ..qz.e/n/d/q > z
+00000460: 4754 6869 7320 7661 6c75 6520 6d75 7374  GThis value must
+00000470: 2062 6520 6120 7369 6e67 6c65 2063 6861   be a single cha
+00000480: 7261 6374 6572 2c20 6f6e 6520 6f66 2074  racter, one of t
+00000490: 6865 2066 6f6c 6c6f 7769 6e67 3a20 652c  he following: e,
+000004a0: 206e 2c20 642c 2071 2909 da05 7072 696e   n, d, q)...prin
+000004b0: 74da 036c 656e da0b 7265 6164 5f63 6f6e  t..len..read_con
+000004c0: 6669 67da 0873 6563 7469 6f6e 73da 0373  fig..sections..s
+000004d0: 7472 7205 0000 00da 0367 6574 7208 0000  trr......getr...
+000004e0: 00da 0569 6e70 7574 2904 720a 0000 00da  ...input).r.....
+000004f0: 1474 656d 706c 6174 655f 666f 6c64 6572  .template_folder
+00000500: 5f6e 616d 65da 1261 6363 6570 7461 626c  _name..acceptabl
+00000510: 655f 6368 6f69 6365 73da 0d61 6374 696f  e_choices..actio
+00000520: 6e5f 6368 6f69 6365 720b 0000 0072 0b00  n_choicer....r..
+00000530: 0000 720c 0000 00da 0d73 656c 6563 745f  ..r......select_
+00000540: 6163 7469 6f6e 0f00 0000 7322 0000 0000  action....s"....
+00000550: 0208 0108 0108 0214 0110 012a 0208 0110  ...........*....
+00000560: 0110 0110 0108 0208 0108 0108 0108 010a  ................
+00000570: 017a 1b43 6f6e 6669 6775 7261 7469 6f6e  .z.Configuration
+00000580: 2e73 656c 6563 745f 6163 7469 6f6e 2902  .select_action).
+00000590: da0a 6163 745f 6368 6f69 6365 da06 7265  ..act_choice..re
+000005a0: 7475 726e 6302 0000 0000 0000 0000 0000  turnc...........
+000005b0: 0006 0000 0008 0000 0043 0000 0073 4401  .........C...sD.
+000005c0: 0000 6400 7d02 7c01 6401 6b02 7210 9001  ..d.}.|.d.k.r...
+000005d0: 6e30 7c01 6402 7600 9001 7224 7400 7c00  n0|.d.v...r$t.|.
+000005e0: a001 a100 a002 a100 8301 6403 6b04 9001  ..........d.k...
+000005f0: 7224 7403 6404 7c00 6a04 9b00 6405 9d03  r$t.d.|.j...d...
+00000600: 8301 0100 7403 6406 8301 0100 7405 7c00  ....t.d.....t.|.
+00000610: a001 a100 a002 a100 8301 4400 5d18 5c02  ..........D.].\.
+00000620: 7d03 7d04 7403 7c03 6407 1700 6408 7c04  }.}.t.|.d...d.|.
+00000630: 8303 0100 715a 6409 640a 8400 7c00 a001  ....qZd.d...|...
+00000640: a100 a002 a100 4400 8301 7d05 7c05 a006  ......D...}.|...
+00000650: 640b 640a 8400 7407 6407 7400 7c00 a001  d.d...t.d.t.|...
+00000660: a100 a002 a100 8301 6407 1700 6407 8303  ........d...d...
+00000670: 4400 8301 a101 0100 7408 7c00 6a04 a009  D.......t.|.j...
+00000680: a100 9b00 640c 9d02 8301 7d02 7c02 7c05  ....d.....}.|.|.
+00000690: 7601 72f0 7403 640d 8301 0100 7408 7c00  v.r.t.d.....t.|.
+000006a0: 6a04 a009 a100 9b00 640c 9d02 8301 7d02  j.......d.....}.
+000006b0: 71ca 7a1c 7c00 a001 a100 a002 a100 740a  q.z.|.........t.
+000006c0: 7c02 8301 6407 1800 1900 7d02 5700 6e14  |...d.....}.W.n.
+000006d0: 0400 740b 9001 7920 0100 0100 0100 5900  ..t...y ......Y.
+000006e0: 6e02 3000 6e1c 7c01 640e 6b02 9001 7240  n.0.n.|.d.k...r@
+000006f0: 7408 640f 7c00 6a04 9b00 6410 9d03 8301  t.d.|.j...d.....
+00000700: 7d02 7c02 5300 2911 4e72 1500 0000 2902  }.|.S.).Nr....).
+00000710: 7212 0000 0072 1400 0000 7201 0000 007a  r....r....r....z
+00000720: 080a 5365 6c65 6374 20da 012e 7a39 4368  ..Select ...z9Ch
+00000730: 6f6f 7365 2061 206e 756d 6265 7220 6672  oose a number fr
+00000740: 6f6d 2062 656c 6f77 2c20 6f72 2074 7970  om below, or typ
+00000750: 6520 696e 2061 6e20 6578 6973 7469 6e67  e in an existing
+00000760: 2076 616c 7565 2ee9 0100 0000 7a02 3e20   value......z.> 
+00000770: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000780: 0003 0000 0053 0000 0073 1000 0000 6700  .....S...s....g.
+00000790: 7c00 5d08 7d01 7c01 9102 7104 5300 720b  |.].}.|...q.S.r.
+000007a0: 0000 0072 0b00 0000 2902 da02 2e30 da0d  ...r....)....0..
+000007b0: 636f 6e66 5f76 6172 6961 626c 6572 0b00  conf_variabler..
+000007c0: 0000 720b 0000 0072 0c00 0000 da0a 3c6c  ..r....r......<l
+000007d0: 6973 7463 6f6d 703e 3300 0000 f300 0000  istcomp>3.......
+000007e0: 007a 3143 6f6e 6669 6775 7261 7469 6f6e  .z1Configuration
+000007f0: 2e73 656c 6563 745f 7465 6d70 6c61 7465  .select_template
+00000800: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00000810: 6f6d 703e 6301 0000 0000 0000 0000 0000  omp>c...........
+00000820: 0002 0000 0004 0000 0053 0000 0073 1400  .........S...s..
+00000830: 0000 6700 7c00 5d0c 7d01 7400 7c01 8301  ..g.|.].}.t.|...
+00000840: 9102 7104 5300 720b 0000 0029 0172 1a00  ..q.S.r....).r..
+00000850: 0000 2902 7225 0000 00da 0569 6e64 6578  ..).r%.....index
+00000860: 720b 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+00000870: 2700 0000 3400 0000 7228 0000 007a 0320  '...4...r(...z. 
+00000880: 3e20 7a1b 4e6f 2063 686f 6963 6573 2077  > z.No choices w
+00000890: 6974 6820 796f 7572 2069 6e70 7574 2e72  ith your input.r
+000008a0: 1300 0000 7a13 0a45 6e74 6572 206e 616d  ....z..Enter nam
+000008b0: 6520 6f66 206e 6577 207a 082e 0a6e 616d  e of new z...nam
+000008c0: 653a 2029 0c72 1700 0000 7218 0000 0072  e: ).r....r....r
+000008d0: 1900 0000 7216 0000 0072 0800 0000 da09  ....r....r......
+000008e0: 656e 756d 6572 6174 65da 0665 7874 656e  enumerate..exten
+000008f0: 64da 0572 616e 6765 721c 0000 00da 0574  d..ranger......t
+00000900: 6974 6c65 da03 696e 74da 0a56 616c 7565  itle..int..Value
+00000910: 4572 726f 7229 0672 0a00 0000 7221 0000  Error).r....r!..
+00000920: 005a 0a74 706c 5f63 686f 6963 6572 2900  .Z.tpl_choicer).
+00000930: 0000 7226 0000 0072 1e00 0000 720b 0000  ..r&...r....r...
+00000940: 0072 0b00 0000 720c 0000 00da 0f73 656c  .r....r......sel
+00000950: 6563 745f 7465 6d70 6c61 7465 2600 0000  ect_template&...
+00000960: 732a 0000 0000 0104 0208 0104 0220 0112  s*........... ..
+00000970: 0108 0218 0112 0216 012c 0114 0208 0108  .........,......
+00000980: 0116 0102 011c 010e 0108 020a 0112 027a  ...............z
+00000990: 1d43 6f6e 6669 6775 7261 7469 6f6e 2e73  .Configuration.s
+000009a0: 656c 6563 745f 7465 6d70 6c61 7465 fa0d  elect_template..
+000009b0: 7465 6d70 6c61 7465 2e63 6f6e 6629 02da  template.conf)..
+000009c0: 0b63 6f6e 6669 675f 6669 6c65 7222 0000  .config_filer"..
+000009d0: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
+000009e0: 0000 0400 0000 4300 0000 732c 0000 0074  ......C...s,...t
+000009f0: 006a 01a0 0274 036a 047c 01a1 027d 017c  .j...t.j.|...}.|
+00000a00: 00a0 057c 01a1 017c 005f 0174 06a0 077c  ...|...|._.t...|
+00000a10: 006a 01a1 0101 0074 0653 0072 0900 0000  .j.....t.S.r....
+00000a20: 2908 da02 6f73 da04 7061 7468 da04 6a6f  )...os..path..jo
+00000a30: 696e 7204 0000 00da 0d63 6f6e 6669 675f  inr......config_
+00000a40: 666f 6c64 6572 da10 636f 6e66 6967 5f66  folder..config_f
+00000a50: 696c 655f 7061 7468 da04 636f 6e66 da04  ile_path..conf..
+00000a60: 7265 6164 a902 720a 0000 0072 3200 0000  read..r....r2...
+00000a70: 720b 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+00000a80: 1800 0000 4400 0000 7308 0000 0000 0110  ....D...s.......
+00000a90: 010c 010c 017a 1943 6f6e 6669 6775 7261  .....z.Configura
+00000aa0: 7469 6f6e 2e72 6561 645f 636f 6e66 6967  tion.read_config
+00000ab0: da00 2903 7232 0000 0072 1f00 0000 da0f  ..).r2...r......
+00000ac0: 7465 6d70 6c61 7465 5f63 686f 6963 6563  template_choicec
+00000ad0: 0400 0000 0000 0000 0000 0000 0600 0000  ................
+00000ae0: 0800 0000 4300 0000 7324 0100 0074 006a  ....C...s$...t.j
+00000af0: 01a0 0274 036a 047c 01a1 027d 017c 00a0  ...t.j.|...}.|..
+00000b00: 057c 01a1 017d 0474 06a0 077c 04a1 0101  .|...}.t...|....
+00000b10: 007c 0264 016b 0272 9674 087c 00a0 09a1  .|.d.k.r.t.|....
+00000b20: 00a0 0aa1 0083 0164 026b 0472 9674 06a0  .......d.k.r.t..
+00000b30: 0b7c 03a1 0101 0074 0c7c 0464 0383 028f  .|.....t.|.d....
+00000b40: 1a7d 0574 06a0 0d7c 05a1 0101 0057 0064  .}.t...|.....W.d
+00000b50: 0004 0004 0083 0301 006e 1031 0073 7430  .........n.1.st0
+00000b60: 0001 0001 0001 0059 0001 0074 0ea0 0f74  .......Y...t...t
+00000b70: 006a 01a0 0274 036a 107c 03a1 02a1 0101  .j...t.j.|......
+00000b80: 006e 8a7c 0264 0476 0090 0172 027c 0264  .n.|.d.v...r.|.d
+00000b90: 056b 0272 c274 06a0 117c 03a1 0101 007c  .k.r.t...|.....|
+00000ba0: 006a 127c 037c 0264 068d 0201 006e 3e7c  .j.|.|.d.....n>|
+00000bb0: 0264 076b 0272 ee74 087c 00a0 09a1 00a0  .d.k.r.t.|......
+00000bc0: 0aa1 0083 0164 026b 0472 ee7c 006a 127c  .....d.k.r.|.j.|
+00000bd0: 037c 0264 068d 0201 006e 1274 1364 087c  .|.d.....n.t.d.|
+00000be0: 006a 149b 0064 099d 0383 0101 006e 1e7c  .j...d.......n.|
+00000bf0: 0264 0a6b 0290 0172 0e6e 1274 1364 087c  .d.k...r.n.t.d.|
+00000c00: 006a 149b 0064 0b9d 0383 0101 0064 0053  .j...d.......d.S
+00000c10: 0029 0c4e 7214 0000 0072 0100 0000 da01  .).Nr....r......
+00000c20: 7729 0272 1200 0000 7213 0000 0072 1300  w).r....r....r..
+00000c30: 0000 a902 723c 0000 0072 1f00 0000 7212  ....r<...r....r.
+00000c40: 0000 007a 034e 6f20 7a09 2074 6f20 6564  ...z.No z. to ed
+00000c50: 6974 2172 1500 0000 7a0b 2074 6f20 6465  it!r....z. to de
+00000c60: 6c65 7465 2129 1572 3300 0000 7234 0000  lete!).r3...r4..
+00000c70: 0072 3500 0000 7204 0000 0072 3600 0000  .r5...r....r6...
+00000c80: 7237 0000 0072 3800 0000 7239 0000 0072  r7...r8...r9...r
+00000c90: 1700 0000 7218 0000 0072 1900 0000 da0e  ....r....r......
+00000ca0: 7265 6d6f 7665 5f73 6563 7469 6f6e da04  remove_section..
+00000cb0: 6f70 656e da05 7772 6974 65da 0673 6875  open..write..shu
+00000cc0: 7469 6cda 0672 6d74 7265 65da 0f74 656d  til..rmtree..tem
+00000cd0: 706c 6174 655f 666f 6c64 6572 da0b 6164  plate_folder..ad
+00000ce0: 645f 7365 6374 696f 6eda 0b6d 6169 6e5f  d_section..main_
+00000cf0: 636f 6e66 6967 7216 0000 0072 0800 0000  configr....r....
+00000d00: 2906 720a 0000 0072 3200 0000 721f 0000  ).r....r2...r...
+00000d10: 0072 3c00 0000 7234 0000 00da 0a63 6f6e  .r<...r4.....con
+00000d20: 6669 6766 696c 6572 0b00 0000 720b 0000  figfiler....r...
+00000d30: 0072 0c00 0000 da0c 7772 6974 655f 636f  .r......write_co
+00000d40: 6e66 6967 4a00 0000 7324 0000 0000 0110  nfigJ...s$......
+00000d50: 010a 010a 021c 010a 010c 0128 0318 020a  ...........(....
+00000d60: 0108 010a 0110 011c 0110 0214 020a 0102  ................
+00000d70: 037a 1a43 6f6e 6669 6775 7261 7469 6f6e  .z.Configuration
+00000d80: 2e77 7269 7465 5f63 6f6e 6669 6763 0200  .write_configc..
+00000d90: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00000da0: 0000 4300 0000 7314 0000 0074 006a 01a0  ..C...s....t.j..
+00000db0: 0274 036a 047c 01a1 027d 017c 0153 0072  .t.j.|...}.|.S.r
+00000dc0: 0900 0000 2905 7233 0000 0072 3400 0000  ....).r3...r4...
+00000dd0: 7235 0000 0072 0400 0000 7236 0000 0072  r5...r....r6...r
+00000de0: 3a00 0000 720b 0000 0072 0b00 0000 720c  :...r....r....r.
+00000df0: 0000 0072 3700 0000 6700 0000 7304 0000  ...r7...g...s...
+00000e00: 0000 0110 017a 1e43 6f6e 6669 6775 7261  .....z.Configura
+00000e10: 7469 6f6e 2e63 6f6e 6669 675f 6669 6c65  tion.config_file
+00000e20: 5f70 6174 6829 0272 1f00 0000 721d 0000  _path).r....r...
+00000e30: 0063 0300 0000 0000 0000 0000 0000 0700  .c..............
+00000e40: 0000 0800 0000 4300 0000 7350 0100 007c  ......C...sP...|
+00000e50: 0164 016b 0273 127c 0164 026b 0290 0172  .d.k.s.|.d.k...r
+00000e60: 4c74 006a 017c 0264 0364 0064 048d 037d  Lt.j.|.d.d.d...}
+00000e70: 0374 0264 057c 039b 0064 069d 0383 017d  .t.d.|...d.....}
+00000e80: 0474 0374 046a 05a0 067c 04a0 0764 0764  .t.t.j...|...d.d
+00000e90: 08a1 02a1 0183 0101 0074 046a 05a0 067c  .........t.j...|
+00000ea0: 04a0 0764 0764 08a1 02a1 0173 8474 087c  ...d.d.....s.t.|
+00000eb0: 0483 0164 096b 0472 8474 0364 0a83 0101  ...d.k.r.t.d....
+00000ec0: 0074 0264 0b7c 039b 0064 069d 0383 017d  .t.d.|...d.....}
+00000ed0: 0471 4a7c 04a0 0764 0764 08a1 027d 0474  .qJ|...d.d...}.t
+00000ee0: 087c 0483 0164 096b 0272 a07c 036e 027c  .|...d.k.r.|.n.|
+00000ef0: 047d 0474 046a 05a0 0974 0a6a 0b7c 02a1  .}.t.j...t.j.|..
+00000f00: 027d 057a 2074 0ca0 0d7c 047c 05a1 0201  .}.z t...|.|....
+00000f10: 0074 0364 0c7c 059b 0064 0d9d 0383 0101  .t.d.|...d......
+00000f20: 0057 006e 2404 0074 0c6a 0e79 e801 0001  .W.n$..t.j.y....
+00000f30: 0001 0059 006e 1204 0074 0f79 f801 0001  ...Y.n...t.y....
+00000f40: 0001 0059 006e 0230 0074 00a0 107c 0264  ...Y.n.0.t...|.d
+00000f50: 037c 05a1 0301 007c 00a0 1164 0ea1 017c  .|.....|...d...|
+00000f60: 005f 0574 127c 006a 0564 0f83 028f 1a7d  ._.t.|.j.d.....}
+00000f70: 0674 00a0 137c 06a1 0101 0057 0064 0004  .t...|.....W.d..
+00000f80: 0004 0083 0301 006e 1231 0090 0173 4230  .......n.1...sB0
+00000f90: 0001 0001 0001 0059 0001 0064 0053 0029  .......Y...d.S.)
+00000fa0: 104e 7213 0000 0072 1200 0000 da13 7465  .Nr....r......te
+00000fb0: 6d70 6c61 7465 5f66 6f6c 6465 725f 6469  mplate_folder_di
+00000fc0: 7272 0f00 0000 7a76 0a54 656d 706c 6174  rr....zv.Templat
+00000fd0: 6520 666f 6c64 6572 2e0a 5468 6520 6669  e folder..The fi
+00000fe0: 6c65 2070 6174 6820 6f66 2074 6865 2048  le path of the H
+00000ff0: 544d 4c20 656d 6169 6c20 7465 6d70 6c61  TML email templa
+00001000: 7465 2066 6f6c 6465 722e 0a45 6e74 6572  te folder..Enter
+00001010: 2061 2073 7472 696e 6720 7661 6c75 652e   a string value.
+00001020: 2050 7265 7373 2045 6e74 6572 2066 6f72   Press Enter for
+00001030: 2074 6865 2064 6566 6175 6c74 2028 fa03   the default (..
+00001040: 293a 20fa 0122 723b 0000 0072 0100 0000  ): .."r;...r....
+00001050: 7a2b 506c 6561 7365 2065 6e74 6572 2061  z+Please enter a
+00001060: 2076 616c 6964 2074 656d 706c 6174 6520   valid template 
+00001070: 666f 6c64 6572 2070 6174 683a 207a 6f0a  folder path: zo.
+00001080: 5465 6d70 6c61 7465 2066 6f6c 6465 722e  Template folder.
+00001090: 0a54 6865 2066 696c 6520 7061 7468 206f  .The file path o
+000010a0: 6620 7468 6520 4854 4d4c 2065 6d61 696c  f the HTML email
+000010b0: 2074 656d 706c 6174 652e 0a45 6e74 6572   template..Enter
+000010c0: 2061 2073 7472 696e 6720 7661 6c75 652e   a string value.
+000010d0: 2050 7265 7373 2045 6e74 6572 2066 6f72   Press Enter for
+000010e0: 2074 6865 2064 6566 6175 6c74 2028 7a25   the default (z%
+000010f0: 0a59 6f75 7220 6669 6c65 2069 7320 636f  .Your file is co
+00001100: 7069 6564 2061 6e64 2075 706c 6f61 6465  pied and uploade
+00001110: 6420 746f 2072 2300 0000 7231 0000 0072  d to r#...r1...r
+00001120: 3d00 0000 2914 7238 0000 0072 1b00 0000  =...).r8...r....
+00001130: 721c 0000 0072 1600 0000 7233 0000 0072  r....r....r3...r
+00001140: 3400 0000 da05 6973 6469 72da 0772 6570  4.....isdir..rep
+00001150: 6c61 6365 7217 0000 0072 3500 0000 7204  lacer....r5...r.
+00001160: 0000 0072 4400 0000 7242 0000 00da 0863  ...rD...rB.....c
+00001170: 6f70 7974 7265 65da 0d53 616d 6546 696c  opytree..SameFil
+00001180: 6545 7272 6f72 da0f 4669 6c65 4578 6973  eError..FileExis
+00001190: 7473 4572 726f 72da 0373 6574 7237 0000  tsError..setr7..
+000011a0: 0072 4000 0000 7241 0000 0029 0772 0a00  .r@...rA...).r..
+000011b0: 0000 721f 0000 0072 1d00 0000 7249 0000  ..r....r....rI..
+000011c0: 005a 176e 6577 5f74 656d 706c 6174 655f  .Z.new_template_
+000011d0: 666f 6c64 6572 5f64 6972 da0c 7465 6d70  folder_dir..temp
+000011e0: 6c61 7465 5f6c 6f63 7247 0000 0072 0b00  late_locrG...r..
+000011f0: 0000 720b 0000 0072 0c00 0000 da14 636f  ..r....r......co
+00001200: 7079 5f74 656d 706c 6174 655f 666f 6c64  py_template_fold
+00001210: 6572 6b00 0000 732a 0000 0000 0112 0110  erk...s*........
+00001220: 0110 0118 0220 0108 0112 010c 0114 0410  ..... ..........
+00001230: 0302 010c 0114 010e 0104 010c 0106 030e  ................
+00001240: 010c 010e 017a 2243 6f6e 6669 6775 7261  .....z"Configura
+00001250: 7469 6f6e 2e63 6f70 795f 7465 6d70 6c61  tion.copy_templa
+00001260: 7465 5f66 6f6c 6465 72a9 01da 1174 656d  te_folder....tem
+00001270: 706c 6174 655f 7365 6c65 6374 6564 6302  plate_selectedc.
+00001280: 0000 0000 0000 0000 0000 0004 0000 0008  ................
+00001290: 0000 0043 0000 0073 8200 0000 7400 6a01  ...C...s....t.j.
+000012a0: 7c01 6401 6400 6402 8d03 7c00 5f02 7403  |.d.d.d...|._.t.
+000012b0: 6403 7c00 6a02 9b00 6404 9d03 8301 7d02  d.|.j...d.....}.
+000012c0: 7404 7c02 8301 6405 6b02 7236 7c00 6a02  t.|...d.k.r6|.j.
+000012d0: 6e02 7c02 7d02 7400 a005 7c01 6401 7c02  n.|.}.t...|.d.|.
+000012e0: a103 0100 7406 7c00 6a07 6406 8302 8f1a  ....t.|.j.d.....
+000012f0: 7d03 7400 a008 7c03 a101 0100 5700 6400  }.t...|.....W.d.
+00001300: 0400 0400 8303 0100 6e10 3100 7374 3000  ........n.1.st0.
+00001310: 0100 0100 0100 5900 0100 6400 5300 2907  ......Y...d.S.).
+00001320: 4e72 0e00 0000 720f 0000 007a 9f0a 5370  Nr....r....z..Sp
+00001330: 7265 6164 7368 6565 7420 7572 6c2e 0a54  readsheet url..T
+00001340: 6865 2047 6f6f 676c 6520 7370 7265 6164  he Google spread
+00001350: 7368 6565 7420 7572 6c20 7468 6174 2079  sheet url that y
+00001360: 6f75 2077 616e 7420 746f 2070 6172 7365  ou want to parse
+00001370: 2069 7420 746f 2074 6865 204a 696e 6a61   it to the Jinja
+00001380: 3220 4854 4d4c 2065 6d61 696c 2074 656d  2 HTML email tem
+00001390: 706c 6174 653a 202e 0a45 6e74 6572 2061  plate: ..Enter a
+000013a0: 2073 7472 696e 6720 7661 6c75 652e 2050   string value. P
+000013b0: 7265 7373 2045 6e74 6572 2066 6f72 2074  ress Enter for t
+000013c0: 6865 2064 6566 6175 6c74 2028 724a 0000  he default (rJ..
+000013d0: 0072 0100 0000 723d 0000 0029 0972 3800  .r....r=...).r8.
+000013e0: 0000 721b 0000 0072 0e00 0000 721c 0000  ..r....r....r...
+000013f0: 0072 1700 0000 7251 0000 0072 4000 0000  .r....rQ...r@...
+00001400: 7234 0000 0072 4100 0000 2904 720a 0000  r4...rA...).r...
+00001410: 0072 5500 0000 5a13 6e65 775f 7370 7265  .rU...Z.new_spre
+00001420: 6164 7368 6565 745f 7572 6c72 4700 0000  adsheet_urlrG...
+00001430: 720b 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
+00001440: 1173 6574 7570 5f53 7072 6561 6473 6865  .setup_Spreadshe
+00001450: 6574 8a00 0000 730c 0000 0000 0112 0112  et....s.........
+00001460: 0116 010e 010e 017a 1f43 6f6e 6669 6775  .......z.Configu
+00001470: 7261 7469 6f6e 2e73 6574 7570 5f53 7072  ration.setup_Spr
+00001480: 6561 6473 6865 6574 6302 0000 0000 0000  eadsheetc.......
+00001490: 0000 0000 000b 0000 0008 0000 0043 0000  .............C..
+000014a0: 0073 4401 0000 7400 6a01 7c01 6401 6402  .sD...t.j.|.d.d.
+000014b0: 6403 8d03 7d02 7402 6404 7c02 9b00 6405  d...}.t.d.|...d.
+000014c0: 9d03 8301 7d03 7403 7c03 8301 6406 6b02  ....}.t.|...d.k.
+000014d0: 7230 7c02 6e02 7c03 7d03 7400 6a01 7c01  r0|.n.|.}.t.j.|.
+000014e0: 6407 6400 6403 8d03 7d04 7402 6408 7c04  d.d.d...}.t.d.|.
+000014f0: 9b00 6405 9d03 8301 7d05 7403 7c05 8301  ..d.....}.t.|...
+00001500: 6406 6b02 7264 7c04 6e02 7c05 7d05 7400  d.k.rd|.n.|.}.t.
+00001510: 6a01 7c01 6409 640a 6403 8d03 7d06 7402  j.|.d.d.d...}.t.
+00001520: 640b 7c06 9b00 6405 9d03 8301 7d07 7403  d.|...d.....}.t.
+00001530: 7c07 8301 6406 6b02 7298 7c06 6e02 7c07  |...d.k.r.|.n.|.
+00001540: 7d07 7400 6a01 7c01 640c 6400 6403 8d03  }.t.j.|.d.d.d...
+00001550: 7d08 7402 640d 7c08 9b00 6405 9d03 8301  }.t.d.|...d.....
+00001560: 7d09 7403 7c09 8301 6406 6b02 72cc 7c08  }.t.|...d.k.r.|.
+00001570: 6e02 7c09 7d09 7400 a004 7c01 6401 7c03  n.|.}.t...|.d.|.
+00001580: a103 0100 7400 a004 7c01 6409 7c07 a103  ....t...|.d.|...
+00001590: 0100 7400 a004 7c01 6407 7c05 a103 0100  ..t...|.d.|.....
+000015a0: 7400 a004 7c01 640c 7c09 a103 0100 7405  t...|.d.|.....t.
+000015b0: 7c00 6a06 640e 8302 8f1a 7d0a 7400 a007  |.j.d.....}.t...
+000015c0: 7c0a a101 0100 5700 6400 0400 0400 8303  |.....W.d.......
+000015d0: 0100 6e12 3100 9001 7336 3000 0100 0100  ..n.1...s60.....
+000015e0: 0100 5900 0100 6400 5300 290f 4eda 1d77  ..Y...d.S.).N..w
+000015f0: 6f72 6b73 6865 6574 5f74 6974 6c65 5f63  orksheet_title_c
+00001600: 616d 7061 6967 6e5f 696e 666f 7a0d 4361  ampaign_infoz.Ca
+00001610: 6d70 6169 676e 2049 6e66 6f72 0f00 0000  mpaign Infor....
+00001620: 7aa0 0a57 6f72 6b73 6865 6574 2054 6974  z..Worksheet Tit
+00001630: 6c65 206f 6620 4361 6d70 6169 676e 2049  le of Campaign I
+00001640: 6e66 6f2e 0a54 6865 2077 6f72 6b73 6865  nfo..The workshe
+00001650: 6574 2074 6974 6c65 206f 6620 6361 6d70  et title of camp
+00001660: 6169 676e 2069 6e66 6f3a 202e 0a45 6e74  aign info: ..Ent
+00001670: 6572 2061 2073 6572 6965 7320 6f66 2063  er a series of c
+00001680: 656c 6c20 7261 6e67 6573 2c20 7365 7061  ell ranges, sepa
+00001690: 7261 7465 6420 6279 2073 796d 626f 6c20  rated by symbol 
+000016a0: 282c 292e 2050 7265 7373 2045 6e74 6572  (,). Press Enter
+000016b0: 2066 6f72 2074 6865 2064 6566 6175 6c74   for the default
+000016c0: 2028 724a 0000 0072 0100 0000 da0d 6361   (rJ...r......ca
+000016d0: 6d70 6169 676e 5f69 6e66 6f7a b60a 4361  mpaign_infoz..Ca
+000016e0: 6d70 6169 676e 2049 6e66 6f2e 0a54 6865  mpaign Info..The
+000016f0: 2043 616d 7061 6967 6e20 696e 666f 2074   Campaign info t
+00001700: 6861 7420 796f 7520 7761 6e74 2074 6f20  hat you want to 
+00001710: 7061 7273 6520 6974 2074 6f20 7468 6520  parse it to the 
+00001720: 4a69 6e6a 6132 2048 544d 4c20 656d 6169  Jinja2 HTML emai
+00001730: 6c20 7465 6d70 6c61 7465 3a20 2e0a 456e  l template: ..En
+00001740: 7465 7220 6120 7365 7269 6573 206f 6620  ter a series of 
+00001750: 6365 6c6c 2072 616e 6765 732c 2073 6570  cell ranges, sep
+00001760: 6172 6174 6564 2062 7920 7379 6d62 6f6c  arated by symbol
+00001770: 2028 2c29 2e20 5072 6573 7320 456e 7465   (,). Press Ente
+00001780: 7220 666f 7220 7468 6520 6465 6661 756c  r for the defaul
+00001790: 7420 28da 2077 6f72 6b73 6865 6574 5f74  t (. worksheet_t
+000017a0: 6974 6c65 5f63 616d 7061 6967 6e5f 636f  itle_campaign_co
+000017b0: 6e74 656e 747a 1043 616d 7061 6967 6e20  ntentz.Campaign 
+000017c0: 436f 6e74 656e 747a a60a 576f 726b 7368  Contentz..Worksh
+000017d0: 6565 7420 5469 746c 6520 6f66 2043 616d  eet Title of Cam
+000017e0: 7061 6967 6e20 436f 6e74 656e 742e 0a54  paign Content..T
+000017f0: 6865 2077 6f72 6b73 6865 6574 2074 6974  he worksheet tit
+00001800: 6c65 206f 6620 6361 6d70 6169 676e 2063  le of campaign c
+00001810: 6f6e 7465 6e74 3a20 2e0a 456e 7465 7220  ontent: ..Enter 
+00001820: 6120 7365 7269 6573 206f 6620 6365 6c6c  a series of cell
+00001830: 2072 616e 6765 732c 2073 6570 6172 6174   ranges, separat
+00001840: 6564 2062 7920 7379 6d62 6f6c 2028 2c29  ed by symbol (,)
+00001850: 2e20 5072 6573 7320 456e 7465 7220 666f  . Press Enter fo
+00001860: 7220 7468 6520 6465 6661 756c 7420 28da  r the default (.
+00001870: 1063 616d 7061 6967 6e5f 636f 6e74 656e  .campaign_conten
+00001880: 747a bb0a 4361 6d70 6169 676e 2043 6f6e  tz..Campaign Con
+00001890: 7465 6e74 2e0a 5468 6520 4361 6d70 6169  tent..The Campai
+000018a0: 676e 2043 6f6e 7465 6e74 2074 6861 7420  gn Content that 
+000018b0: 796f 7520 7761 6e74 2074 6f20 7061 7373  you want to pass
+000018c0: 2069 7420 746f 2074 6865 204a 696e 6a61   it to the Jinja
+000018d0: 3220 4854 4d4c 2065 6d61 696c 2074 656d  2 HTML email tem
+000018e0: 706c 6174 653a 202e 0a45 6e74 6572 2061  plate: ..Enter a
+000018f0: 2073 6572 6965 7320 6f66 2063 656c 6c20   series of cell 
+00001900: 7261 6e67 6573 2c20 7365 7061 7261 7465  ranges, separate
+00001910: 6420 6279 2073 796d 626f 6c20 282c 292e  d by symbol (,).
+00001920: 2050 7265 7373 2045 6e74 6572 2066 6f72   Press Enter for
+00001930: 2074 6865 2064 6566 6175 6c74 2028 723d   the default (r=
+00001940: 0000 0029 0872 3800 0000 721b 0000 0072  ...).r8...r....r
+00001950: 1c00 0000 7217 0000 0072 5100 0000 7240  ....r....rQ...r@
+00001960: 0000 0072 3400 0000 7241 0000 0029 0b72  ...r4...rA...).r
+00001970: 0a00 0000 7255 0000 0072 5700 0000 5a21  ....rU...rW...Z!
+00001980: 6e65 775f 776f 726b 7368 6565 745f 7469  new_worksheet_ti
+00001990: 746c 655f 6361 6d70 6169 676e 5f69 6e66  tle_campaign_inf
+000019a0: 6f72 5800 0000 5a11 6e65 775f 6361 6d70  orX...Z.new_camp
+000019b0: 6169 676e 5f69 6e66 6f72 5900 0000 5a24  aign_inforY...Z$
+000019c0: 6e65 775f 776f 726b 7368 6565 745f 7469  new_worksheet_ti
+000019d0: 746c 655f 6361 6d70 6169 676e 5f63 6f6e  tle_campaign_con
+000019e0: 7465 6e74 725a 0000 005a 146e 6577 5f63  tentrZ...Z.new_c
+000019f0: 616d 7061 6967 6e5f 636f 6e74 656e 7472  ampaign_contentr
+00001a00: 4700 0000 720b 0000 0072 0b00 0000 720c  G...r....r....r.
+00001a10: 0000 00da 0e73 6574 7570 5f63 616d 7061  .....setup_campa
+00001a20: 6967 6e92 0000 0073 2400 0000 0001 1001  ign....s$.......
+00001a30: 1001 1402 1001 1001 1402 1001 1001 1402  ................
+00001a40: 1001 1001 1402 0e01 0e01 0e01 0e01 0e01  ................
+00001a50: 7a1c 436f 6e66 6967 7572 6174 696f 6e2e  z.Configuration.
+00001a60: 7365 7475 705f 6361 6d70 6169 676e 6301  setup_campaignc.
+00001a70: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+00001a80: 0000 0043 0000 0073 2e00 0000 7400 a001  ...C...s....t...
+00001a90: a100 0100 7c00 a002 a100 7d01 7c00 6a03  ....|.....}.|.j.
+00001aa0: 7c01 6401 8d01 7d02 7c00 6a04 7c01 7c02  |.d...}.|.j.|.|.
+00001ab0: 6402 8d02 0100 6400 5300 2903 4e29 0172  d.....d.S.).N).r
+00001ac0: 2100 0000 2902 721f 0000 0072 3c00 0000  !...).r....r<...
+00001ad0: 2905 7204 0000 00da 0a63 7265 6174 655f  ).r......create_
+00001ae0: 6469 7272 2000 0000 7230 0000 0072 4800  dirr ...r0...rH.
+00001af0: 0000 2903 720a 0000 00da 0f61 6374 696f  ..).r......actio
+00001b00: 6e5f 7365 6c65 6374 6564 7255 0000 0072  n_selectedrU...r
+00001b10: 0b00 0000 720b 0000 0072 0c00 0000 da0b  ....r....r......
+00001b20: 636f 6e66 6967 5f70 6167 65aa 0000 0073  config_page....s
+00001b30: 0800 0000 0001 0801 0802 0c02 7a19 436f  ............z.Co
+00001b40: 6e66 6967 7572 6174 696f 6e2e 636f 6e66  nfiguration.conf
+00001b50: 6967 5f70 6167 6572 3e00 0000 6303 0000  ig_pager>...c...
+00001b60: 0000 0000 0000 0000 0003 0000 0004 0000  ................
+00001b70: 0043 0000 0073 2a00 0000 7c00 6a00 7c01  .C...s*...|.j.|.
+00001b80: 7c02 6401 8d02 0100 7c00 6a01 7c01 6402  |.d.....|.j.|.d.
+00001b90: 8d01 0100 7c00 6a02 7c01 6402 8d01 0100  ....|.j.|.d.....
+00001ba0: 6400 5300 2903 4e29 0272 1d00 0000 721f  d.S.).N).r....r.
+00001bb0: 0000 0072 5400 0000 2903 7253 0000 0072  ...rT...).rS...r
+00001bc0: 5600 0000 725b 0000 0029 0372 0a00 0000  V...r[...).r....
+00001bd0: 723c 0000 0072 1f00 0000 720b 0000 0072  r<...r....r....r
+00001be0: 0b00 0000 720c 0000 0072 4600 0000 b200  ....r....rF.....
+00001bf0: 0000 7306 0000 0000 020e 030c 037a 1943  ..s..........z.C
+00001c00: 6f6e 6669 6775 7261 7469 6f6e 2e6d 6169  onfiguration.mai
+00001c10: 6e5f 636f 6e66 6967 4e29 0172 3100 0000  n_configN).r1...
+00001c20: 2903 7231 0000 0072 3b00 0000 723b 0000  ).r1...r;...r;..
+00001c30: 0029 0172 3100 0000 2911 da08 5f5f 6e61  .).r1...)...__na
+00001c40: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00001c50: da0c 5f5f 7175 616c 6e61 6d65 5f5f 721a  ..__qualname__r.
+00001c60: 0000 0072 0d00 0000 7220 0000 0072 3000  ...r....r ...r0.
+00001c70: 0000 da04 7479 7065 7202 0000 0072 1800  ....typer....r..
+00001c80: 0000 7248 0000 0072 3700 0000 7253 0000  ..rH...r7...rS..
+00001c90: 0072 5600 0000 725b 0000 0072 5e00 0000  .rV...r[...r^...
+00001ca0: 7246 0000 0072 0b00 0000 720b 0000 0072  rF...r....r....r
+00001cb0: 0b00 0000 720c 0000 0072 0600 0000 0b00  ....r....r......
+00001cc0: 0000 7316 0000 0008 010e 0308 1710 1e16  ..s.............
+00001cd0: 0614 1d16 0410 1f0e 080e 1808 0872 0600  .............r..
+00001ce0: 0000 290d da0c 636f 6e66 6967 7061 7273  ..)...configpars
+00001cf0: 6572 7202 0000 00da 0b67 656e 6572 6963  err......generic
+00001d00: 7061 7468 7203 0000 0072 3300 0000 7242  pathr....r3...rB
+00001d10: 0000 00da 166d 6169 6c63 6869 6d70 5f61  .....mailchimp_a
+00001d20: 7574 6f2e 7363 7269 7074 7372 0400 0000  uto.scriptsr....
+00001d30: 5a0d 6773 7072 6561 642e 7574 696c 7372  Z.gspread.utilsr
+00001d40: 0500 0000 da07 6c6f 6767 696e 6772 3800  ......loggingr8.
+00001d50: 0000 7206 0000 0072 0b00 0000 720b 0000  ..r....r....r...
+00001d60: 0072 0b00 0000 720c 0000 00da 083c 6d6f  .r....r......<mo
+00001d70: 6475 6c65 3e01 0000 0073 1000 0000 0c01  dule>....s......
+00001d80: 0c01 0801 0801 0c01 0c01 0802 0602       ..............
```

### Comparing `mailchimp_auto-0.1.0/mailchimp_auto/scripts/campaign_detail.py` & `mailchimp_auto-0.1.1/mailchimp_auto/scripts/campaign_detail.py`

 * *Files identical despite different names*

### Comparing `mailchimp_auto-0.1.0/mailchimp_auto/scripts/Config.py` & `mailchimp_auto-0.1.1/mailchimp_auto/scripts/Config.py`

 * *Files identical despite different names*

### Comparing `mailchimp_auto-0.1.0/mailchimp_auto/scripts/directory.py` & `mailchimp_auto-0.1.1/mailchimp_auto/scripts/directory.py`

 * *Files identical despite different names*

### Comparing `mailchimp_auto-0.1.0/mailchimp_auto/scripts/engine.py` & `mailchimp_auto-0.1.1/mailchimp_auto/scripts/create_campaign.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-# from mailchimp3 import MailChimp
 import mailchimp_marketing
-from mailchimp_auto.scripts.create_campaign import campaign_creation_function
-from mailchimp_auto.scripts.load_newsletter_template import customized_template # html_code is a variable
-from mailchimp_auto.scripts.template import generate_html_template
-from mailchimp_auto.scripts.Config import *
-from typing import Tuple
-from mailchimp_auto.scripts.campaign_detail import *
-
-# setup mailchimp account
-def connect(account_username: str) -> Tuple[str, str]:
-    config = read_config("account.conf")
-    api_key = config.get(account_username, "api_key")
-    server_prefix = config.get(account_username, "server_prefix")
-    return api_key, server_prefix
-    
-# create new campaign
-def create_new_campaign(account_username:str, template_name:str, preview:bool):
+import logging
+from typing import Dict
+from mailchimp_auto.scripts.campaign_detail import Info
+from typing import Union, Optional
+
+def campaign_creation_function(account_choice:str, template_choice: str,                              
+                               client: type[mailchimp_marketing.Client], recipients_segment: Optional[Union[str,int]]=None, template_id: int=0
+                               ) -> Dict:
     """_summary_
 
-    :param account_username: _description_
-    :type account_username: str
-    :param template_name: _description_
-    :type template_name: str
-    :param preview: _description_
-    :type preview: bool
-
-    Explanation: 
-    # How to start this program
-    `python mailchimpcamp.py` or `python mailchimpcamp.py run`
-    
-    # Processes being run:
-    1. connect to your mailchimp account using API key.
-    2. create a campaign under your certain audience list.
-    3. generate a html template based on your google spreadsheet input.
-    4. upload that html template to the mailchimp server as the campaign content.
+    :param account_choice: _description_
+    :type account_choice: str
+    :param template_choice: _description_
+    :type template_choice: str
+    :param recipients_segment: _description_
+    :type recipients_segment: Union[str,int]
+    :param client: _description_
+    :type client: type[mailchimp_marketing.Client]
+    :param template_id: _description_, defaults to 0
+    :type template_id: int, optional
+    :return: _description_
+    :rtype: Dict
     """
+    tpl = Info(account_choice = account_choice, template_choice=template_choice)
     
-    if not preview:
-        api_key, server_prefix = connect(account_username)
-        # authenticate using mailchimp api and username
-        client = mailchimp_marketing.Client()
-        client.set_config({
-            "api_key": api_key,
-            "server": server_prefix,
-            })
-
-        # create campaign
-        campaign = campaign_creation_function(account_choice=account_username, 
-                                            template_choice=template_name,
-                                            client=client)
-
-        # generate html template
-        rendered_html = generate_html_template(account_choice=account_username, template_name = template_name)  # need to input template path
-
-        # upload the html template to the campaign
-        customized_template(html_code=rendered_html, campaign_id=campaign["id"], client=client)
+    data = {
+        "type": "regular",
+        "recipients" :
+        {
+            "list_id": tpl.getCampaignInfo()["list_id"],
+        },
+        "settings":
+        {
+            "subject_line": tpl.getCampaignInfo()["subject_line"],
+            "preview_text": tpl.getCampaignInfo()["preview_text"],
+            "title":tpl.getCampaignInfo()["campaign_title"],
+            "from_name": tpl.getCampaignInfo()["from_name"],
+            "to_name": tpl.getCampaignInfo()["to_name"], 
+            "reply_to": tpl.getCampaignInfo()["reply_to"],           
+        },
+        "tracking":
+            {"opens": True,
+             "html_clicks":True,
+             "text_clicks":True,
+             }
+    }
+    
+    if recipients_segment:
+        if isinstance(recipients_segment, str):
+            data["settings"].update({"recipients":{"segment_opts": {"match": recipients_segment}}})
+        if isinstance(recipients_segment, int):
+            data["settings"].update({"recipients":{"segment_opts": {"saved_segment_id": recipients_segment}}})    
+    if template_id:
+        data["settings"].update({"template_id": template_id})
     
-    elif preview:
-        rendered_html = generate_html_template(account_choice=account_username, template_name = template_name, preview=preview)
-        
+    new_campaign = client.campaigns.create(data)
+    logging.debug("type of New campaign: " + str(type(new_campaign)))
+    logging.debug(new_campaign)
+        
+    return new_campaign
```

### Comparing `mailchimp_auto-0.1.0/mailchimp_auto/scripts/gspread_data.py` & `mailchimp_auto-0.1.1/mailchimp_auto/scripts/gspread_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,55 +2,44 @@
 from typing import Dict, Union
 import pandas as pd
 import numpy as np
 import os
 from configparser import RawConfigParser
 from mailchimp_auto.scripts.directory import *
 import logging
+import re
+from mailchimp_auto.scripts.image_processor import upload_image
 
 config = RawConfigParser()
 config.read(template_config)
 
 class getGspreadData: 
     def __init__(self, account_choice:str="", template_choice:str =""):
         """_summary_
 
         Args:
             credentials (dict, optional): Google Oauth2.0 JSON credentials in python dict instead of original json format. Defaults to credentials.
             user_authorized (dict, optional): authorized user's client id, client secret, etc in python dict format. Defaults to user_authorized.
         """
-        # self.user_authorized = db.all()[0]
         self.account_choice = account_choice
         self.template_choice = template_choice
         self.spreadsheet_url = config.get(self.template_choice, "spreadsheet_url", fallback=None)
         self.sheet = self.access_spreadsheet()
-
-    #def start_new_connection(self) -> None: # used when config
-    #    self.gc, user_authorized = gspread.oauth_from_dict(self.credentials)
-    #   db.truncate()
-    #    db.insert(json.loads(user_authorized))
     
     def access_spreadsheet(self):
         tpl_config = RawConfigParser()
         tpl_config.read(account_config)
         service_account_file_path = tpl_config.get(self.account_choice, "service_account_file_path", fallback=None)
-        #print(f"spreadsheet url 1: {self.spreadsheet_url}")
-        #print(f"template_choice1: {self.template_choice}")
+
         try:
-            #print(service_account_file_path)
             self.gc = gspread.service_account(filename=service_account_file_path) #oauth_from_dict(self.credentials, self.user_authorized)
-            #print(f"spreadsheet url 1: {self.spreadsheet_url}")
-            #logging.debug(str(self.spreadsheet_url))
             sheet = self.gc.open_by_url(self.spreadsheet_url)
         except gspread.exceptions.APIError as error:
             print(f"{error}")
             print("Please choose the Google account that has permission to open the spreadsheet!")
-            # self.start_new_connection()
-            # print(self.spreadsheet_url)
-            #sheet = self.gc.open_by_url(self.spreadsheet_url)
         logging.debug(f"The type of sheet object: {type(sheet)}")
         return sheet
 
     def get_campaign_info(self, worksheet_title:str, multiple_cell_ranges: Union[str, list]) -> Dict[str, str]: 
         """_summary_
 
         Args:
@@ -94,8 +83,13 @@
             content_info_dict.update({section_name[0]: {}})  
             df = pd.DataFrame.from_records(content_info_list[index])
             header_row = df.iloc[0]
             df_with_header = pd.DataFrame(df.values[1:], columns=header_row)
             df_with_header.replace("", np.nan, inplace=True)
             df_with_header.dropna(axis=0, how="any", inplace=True)
             content_info_dict[section_name[0]].update(df_with_header.to_dict())
+        
+    
+        #print(content_info_dict)
+        #print("--------content info dict above------------")
+                
         return content_info_dict
```

### Comparing `mailchimp_auto-0.1.0/mailchimp_auto/scripts/load_newsletter_template.py` & `mailchimp_auto-0.1.1/mailchimp_auto/scripts/load_newsletter_template.py`

 * *Files identical despite different names*

### Comparing `mailchimp_auto-0.1.0/mailchimp_auto/scripts/template_Config.py` & `mailchimp_auto-0.1.1/mailchimp_auto/scripts/template_Config.py`

 * *Files identical despite different names*

### Comparing `mailchimp_auto-0.1.0/pyproject.toml` & `mailchimp_auto-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "mailchimp_auto"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["tys203831 <tys203831@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 mailchimp_auto = "mailchimp_auto.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.9.12"
 typer = {extras = ["all"], version = "^0.6.1"}
 mailchimp-marketing = "^3.0.75"
 Jinja2 = "^3.1.2"
 pandas = "^1.4.3"
 gspread = "^5.4.0"
+Pillow = "^9.4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mailchimp_auto-0.1.0/README.md` & `mailchimp_auto-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,160 +1,203 @@
-# mailchimp_auto
-
-## Welcome to chronos’s documentation!
-`mailchimp_auto` is a command line application to automate the email creation process on MailChimp based on the google spreadsheet input. What it does is using Jinja2 template engine to loop over dummy values (e.g., website url, image url, string) on html template in order to create the html template to be uploaded to MailChimp server.
-
-(Note: This project is highly customized for personal use, but it's okay for reference.)
-
-## Introduction
-This package uses 2 major packages:
-* mailchimp-marketing to automate creating campaign on Mailchimp
-* jinja2 for managing tags inserted into the HTML email template to loop over and replace the data elements
-
-----
-## Motivation
-As a newbie hobbyist in Python, I found it very troublesome to drag and drop the editor in MailChimp in a weekly basis just to change some certain contents in the template that wastes me 30 minutes per change, thus I need a way to automate that campaign creation.
-
-----
-## Getting Started
-
-* `pip install mailchimp_auto`
-
----
-## Configuration
-### Account Configuration
-Before you start using this cli tool, you should setup Mailchimp API, Mailchimp server prefix, Google Service account's json file through the command line `mailchimp_auto config` or `python -m mailchimp_auto config`.
-
-And after the command has been run, the interface below will appear:
-
-```
-Current Mailchimp remote:
-Account Username        Server Prefix
-=================       =============
-TYONGSHENG               us1
-
-e) Edit existing account
-n) New account
-d) Delete account
-q) quit
-e/n/d/q > e
-```
-
-You are required to create (n), edit(e) the config variables such as mailchimp username, mailchimp API, and fill in the Google Service Account Credentials JSON path that you have downloaded. 
-
-```
-Select account.
-Choose a number from below, or type in an existing value.
-1 >  TYONGSHENG
-Account > 1
-
-Mailchimp API
-Enter a string value. Press Enter for the default (2exxxxxxxxxxxxxxxxxxxxxxxx-us1): 2exxxxxxxxxxxxxxxxxxxxxxxx-us1
-
-Service_account_file.
-Google Service Account Credentials JSON file path.
-Enter a string value. Press Enter for the default (C:\Users\tys\Documents\mailchimp-auto\.config\service_account_file\TYONGSHENG.json): C:\Users\tys\Documents\mailchimp-auto\.config\service_account_file\TYONGSHENG.json
-```
-
-For how to open a Google service account and download its JSON key, follow Step 1 to Step 5 [here](https://owaisqureshi.medium.com/access-google-sheets-api-in-python-using-service-account-3a0c6d89d5fc). 
-
-
-Feel free to delete (d) any entry you don't need anymore!
-
-### Template Configuration
-Type the command line `mailchimp_auto config-template` or `python -m mailchimp_auto config-template` to upload and save the HTML email template (in form of Jinja tags) to this program and also setup spreadsheet (using spreadsheet url) to get the data you want to parse or loop into the HTML email template. 
-
-```
-Current template(s):
-Template                        Spreadsheet Id
-========                        ===============
-my_weekly_newsletter             1h31GQRfBqUpMmPCXI013J1-Y-kinfgifN6Pa3dx3hB0
-
-
-e) Edit existing template
-n) New template
-d) Delete template
-q) quit
-e/n/d/q > e
-```
-
-But, before continue to enter any input into it, please prepare the few things below:
-
-(i) Create an google spreadsheet with two pages, "Campaign Info" and "Campaign Content". You can refer to the sample spreadsheet [here](https://docs.google.com/spreadsheets/d/1h31GQRfBqUpMmPCXI013J1-Y-kinfgifN6Pa3dx3hB0/edit?usp=sharing), whereby the data there are to be scraped through this program to be processed into the HTML email template to replace the dummy variables I have placed using Jinja2 library module. 
-
-(ii) Then, create an Jinja2 email template (`master.htm`) inside a folder. 
-
-Here are some simple Jinja template tags in order to create the Jinja2 email template (can skip this if you already know) or see [here](https://jinja.palletsprojects.com/en/3.1.x/templates/) if you want to know more: 
-* {{ ... }} for Expressions to print to the template output
-* {% ... %} for Statements
-
-So, for example, referring to the [spreadsheet](https://docs.google.com/spreadsheets/d/1h31GQRfBqUpMmPCXI013J1-Y-kinfgifN6Pa3dx3hB0/edit?usp=sharing), if you want to parse the `community_insights` table variable int, below is the sample Jinja2 template tags:
-
-```html
-{% for key in community_insights.heading %}
-    <p>Any html content you want to loop can put it here</p>
-    <p>And here is the dynamic variable here: {{ community_insights.heading[key] }}</p>
-{% endfor %}
-```
-![Gspread Data](images/spreadsheet_sample.png)
-
-For the template folder structure, you can refer here, whereby `master.htm` is the COMPULSORY file to have when generating html email output (refer to [sample template folder](sample_template) ): 
-```
-template
-\---<your template name>
-    |   master.htm
-```
-Tips: For me, I export the HTML email template from the MailChimp and then edit the HTML file through replacing the Jinja2 template tags onto some variables which I wish to loop the data into them.
-
-(iii) Continue back to the command line `mailchimp_auto config-template` and then do follow the following series of instructions: 
-
-Below are the commands when I want to edit (e) some config of my template. It does the same when you want to create (n) a new template source. 
-```
-Current template(s):
-Template                        Spreadsheet Id
-========                        ===============
-my_weekly_newsletter             1h31GQRfBqUpMmPCXI013J1-Y-kinfgifN6Pa3dx3hB0
-
-e) Edit existing template
-n) New template
-d) Delete template
-q) quit
-e/n/d/q > e
-
-Select template.
-Choose a number from below, or type in an existing value.
-1 >  my_weekly_newsletter
-Template > 1
-
-Template folder.
-The file path of the HTML email template folder.
-Enter a string value. Press Enter for the default (C:\Users\tys\Documents\mailchimp-auto\template\my_weekly_newsletter): C:\Users\tys\Documents\Project\mailchimp_creation_project\mailchimp-auto\sample_template
-
-Spreadsheet url.
-The Google spreadsheet url that you want to parse it to the Jinja2 HTML email template: .
-Enter a string value. Press Enter for the default (https://docs.google.com/spreadsheets/d/1h31GQRfBqUpMmPCXI013J1-Y-kinfgifN6Pa3dx3hB0/edit#gid=1758545491): https://docs.google.com/spreadsheets/d/1h31GQRfBqUpMmPCXI013J1-Y-kinfgifN6Pa3dx3hB0/edit#gid=1758545491
-
-Worksheet Title of Campaign Info.
-The worksheet title of campaign info: .
-Enter a series of cell ranges, separated by symbol (,). Press Enter for the default (Campaign Info): *Campaign Info*
-
-Campaign Info.
-The Campaign info that you want to parse it to the Jinja2 HTML email template: .
-Enter a series of cell ranges, separated by symbol (,). Press Enter for the default (A1:B8): *A1:B8*
-
-Worksheet Title of Campaign Content.
-The worksheet title of campaign content: .
-Enter a series of cell ranges, separated by symbol (,). Press Enter for the default (Campaign Content): Campaign Content
-
-Campaign Content.
-The Campaign Content that you want to pass it to the Jinja2 HTML email template: .
-Enter a series of cell ranges, separated by symbol (,). Press Enter for the default (A3:B5,A7:G20,A22:C31,A33:D41,A43:G48): A3:B5,A7:G20,A22:C31,A33:D41,A43:G48
-```
-
-
-## Running the program to automate the campaign creation
-Enter the command line `mailchimp_auto create --user <mailchimp_account_username> --template <your_template>` and then it will scrape data from Google Spreadsheet you assigned to and inserted them into the HTML email template to loop over and replace the data elements. 
-
-If you don't want to upload your processed HTML email template to mailchimp server first, add the command `--preview` behind the previous command line, e.g.,   `mailchimp_auto create --user <mailchimp_account_username> --template <your_template> --preview`.
-
-It's all done. Hope you are successful with that. If got any problem, kindly contact me. By the way, this is my first time creating a python library (or cli tool) to automate my task. I know some python syntax works not the best for the program (e.g., too much repetitive code, etc). But, I hope I could learn more through creating and maintaining this program.
-
+Metadata-Version: 2.1
+Name: mailchimp-auto
+Version: 0.1.1
+Summary: 
+Author: tys203831
+Author-email: tys203831@gmail.com
+Requires-Python: >=3.9.12,<4.0.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: Pillow (>=9.4.0,<10.0.0)
+Requires-Dist: gspread (>=5.4.0,<6.0.0)
+Requires-Dist: mailchimp-marketing (>=3.0.75,<4.0.0)
+Requires-Dist: pandas (>=1.4.3,<2.0.0)
+Requires-Dist: typer[all] (>=0.6.1,<0.7.0)
+Description-Content-Type: text/markdown
+
+# mailchimp_auto
+
+## Welcome to mailchimp_auto’s documentation!
+`mailchimp_auto` is a command line application to automate the email creation process on MailChimp based on the google spreadsheet input. What it does is using Jinja2 template engine to loop over dummy values (e.g., website url, image url, string) on html template in order to create the html template to be uploaded to MailChimp server.
+
+(Note: This project is highly customized for personal use, but it's okay for reference.)
+
+## Introduction
+This package uses 2 major packages:
+* `mailchimp-marketing` to automate creating campaign on Mailchimp
+* `jinja2` for managing tags inserted into the HTML email template to loop over and replace the data elements
+
+----
+## Motivation
+As a newbie hobbyist in Python, I found it very troublesome to drag and drop the editor in MailChimp in a weekly basis just to change some certain contents in the template that wastes me 30 minutes per change, thus I need a way to automate that campaign creation.
+
+----
+## Getting Started
+
+* `pip install mailchimp_auto` 
+* To get the latest release, `pip install git+https://github.com/tys203831/mailchimp_auto.git@main`
+
+---
+## Configuration
+### Account Configuration
+Before you start using this cli tool, you should setup Mailchimp API, Mailchimp server prefix, Google Service account's json file through the command line `mailchimp_auto config` or `python -m mailchimp_auto config`.
+
+And after the command has been run, the interface below will appear:
+
+```
+Current Mailchimp remote:
+Account Username        Server Prefix
+=================       =============
+TYONGSHENG               us1
+
+e) Edit existing account
+n) New account
+d) Delete account
+q) quit
+e/n/d/q > e
+```
+
+You are required to create (n), edit(e) the config variables such as mailchimp username, mailchimp API, and fill in the Google Service Account Credentials JSON path that you have downloaded. 
+
+```
+Select account.
+Choose a number from below, or type in an existing value.
+1 >  TYONGSHENG
+Account > 1
+
+Mailchimp API
+Enter a string value. Press Enter for the default (2exxxxxxxxxxxxxxxxxxxxxxxx-us1): 2exxxxxxxxxxxxxxxxxxxxxxxx-us1
+
+Service_account_file.
+Google Service Account Credentials JSON file path.
+Enter a string value. Press Enter for the default (C:\Users\tys\Documents\mailchimp-auto\.config\service_account_file\TYONGSHENG.json): C:\Users\tys\Documents\mailchimp-auto\.config\service_account_file\TYONGSHENG.json
+```
+
+For how to open a Google service account and download its JSON key, follow Step 1 to Step 5 [here](https://owaisqureshi.medium.com/access-google-sheets-api-in-python-using-service-account-3a0c6d89d5fc). 
+
+
+Feel free to delete (d) any entry you don't need anymore!
+
+### Template Configuration
+Type the command line `mailchimp_auto config-template` or `python -m mailchimp_auto config-template` to upload and save the HTML email template (in form of Jinja tags) to this program and also setup spreadsheet (using spreadsheet url) to get the data you want to parse or loop into the HTML email template. 
+
+```
+Current template(s):
+Template                        Spreadsheet Id
+========                        ===============
+my_weekly_newsletter             1h31GQRfBqUpMmPCXI013J1-Y-kinfgifN6Pa3dx3hB0
+
+
+e) Edit existing template
+n) New template
+d) Delete template
+q) quit
+e/n/d/q > e
+```
+
+But, before continue to enter any input into it, please prepare the few things below:
+
+(i) Create an google spreadsheet with two pages, "Campaign Info" and "Campaign Content". You can refer to the sample spreadsheet [here](https://docs.google.com/spreadsheets/d/1h31GQRfBqUpMmPCXI013J1-Y-kinfgifN6Pa3dx3hB0/edit?usp=sharing), whereby the data there are to be scraped through this program to be processed into the HTML email template to replace the dummy variables I have placed using Jinja2 library module. 
+
+(ii) Then, create an Jinja2 email template (`master.htm`) inside a folder. 
+
+Here are some simple Jinja template tags in order to create the Jinja2 email template (can skip this if you already know) or see [here](https://jinja.palletsprojects.com/en/3.1.x/templates/) if you want to know more: 
+* {{ ... }} for Expressions to print to the template output
+* {% ... %} for Statements
+
+So, for example, referring to the [spreadsheet](https://docs.google.com/spreadsheets/d/1h31GQRfBqUpMmPCXI013J1-Y-kinfgifN6Pa3dx3hB0/edit?usp=sharing), if you want to parse the `community_insights` table variable int, below is the sample Jinja2 template tags:
+
+```html
+{% for key in community_insights.heading %}
+    <p>Any html content you want to loop can put it here</p>
+    <p>And here is the dynamic variable here: {{ community_insights.heading[key] }}</p>
+{% endfor %}
+```
+![Gspread Data](images/spreadsheet_sample.png)
+
+For the template folder structure, you can refer here, whereby `master.htm` is the COMPULSORY file to have when generating html email output (refer to [sample template folder](sample_template) ): 
+```
+template
+\---<your template name>
+    |   master.htm
+```
+Tips: For me, I export the HTML email template from the MailChimp and then edit the HTML file through replacing the Jinja2 template tags onto some variables which I wish to loop the data into them.
+
+(iii) Continue back to the command line `mailchimp_auto config-template` and then do follow the following series of instructions: 
+
+Below are the commands when I want to edit (e) some config of my template. It does the same when you want to create (n) a new template source. 
+```
+Current template(s):
+Template                        Spreadsheet Id
+========                        ===============
+my_weekly_newsletter             1h31GQRfBqUpMmPCXI013J1-Y-kinfgifN6Pa3dx3hB0
+
+e) Edit existing template
+n) New template
+d) Delete template
+q) quit
+e/n/d/q > e
+
+Select template.
+Choose a number from below, or type in an existing value.
+1 >  my_weekly_newsletter
+Template > 1
+
+Template folder.
+The file path of the HTML email template folder.
+Enter a string value. Press Enter for the default (C:\Users\tys\Documents\mailchimp-auto\template\my_weekly_newsletter): C:\Users\tys\Documents\Project\mailchimp_creation_project\mailchimp-auto\sample_template
+
+Spreadsheet url.
+The Google spreadsheet url that you want to parse it to the Jinja2 HTML email template: .
+Enter a string value. Press Enter for the default (https://docs.google.com/spreadsheets/d/1h31GQRfBqUpMmPCXI013J1-Y-kinfgifN6Pa3dx3hB0/edit#gid=1758545491): https://docs.google.com/spreadsheets/d/1h31GQRfBqUpMmPCXI013J1-Y-kinfgifN6Pa3dx3hB0/edit#gid=1758545491
+
+Worksheet Title of Campaign Info.
+The worksheet title of campaign info: .
+Enter a series of cell ranges, separated by symbol (,). Press Enter for the default (Campaign Info): *Campaign Info*
+
+Campaign Info.
+The Campaign info that you want to parse it to the Jinja2 HTML email template: .
+Enter a series of cell ranges, separated by symbol (,). Press Enter for the default (A1:B8): *A1:B8*
+
+Worksheet Title of Campaign Content.
+The worksheet title of campaign content: .
+Enter a series of cell ranges, separated by symbol (,). Press Enter for the default (Campaign Content): Campaign Content
+
+Campaign Content.
+The Campaign Content that you want to pass it to the Jinja2 HTML email template: .
+Enter a series of cell ranges, separated by symbol (,). Press Enter for the default (A3:B5,A7:G20,A22:C31,A33:D41,A43:G48): A3:B5,A7:G20,A22:C31,A33:D41,A43:G48
+```
+
+
+## Running the program to automate the campaign creation
+Enter the command line `mailchimp_auto create --user <mailchimp_account_username> --template <your_template>` and then it will scrape data from Google Spreadsheet you assigned to and inserted them into the HTML email template to loop over and replace the data elements. 
+
+If you don't want to upload your processed HTML email template to mailchimp server first, add the command `--preview` behind the previous command line, e.g.,   `mailchimp_auto create --user <mailchimp_account_username> --template <your_template> --preview`.
+
+It's all done. Hope you are successful with that. If got any problem, kindly contact me. By the way, this is my first time creating a python library (or cli tool) to automate my task. I know some python syntax works not the best for the program (e.g., too much repetitive code, etc). But, I hope I could learn more through creating and maintaining this program.
+
+## Other information
+```
+
+ Usage: mailchimp_auto [OPTIONS] COMMAND [ARGS]...
+
+╭─ Options ────────────────────────────────────────────────────────────────────────╮
+│ --install-completion          Install completion for the current shell.          │
+│ --show-completion             Show completion for the current shell, to copy it  │
+│                               or customize the installation.                     │
+│ --help                        Show this message and exit.                        │
+╰──────────────────────────────────────────────────────────────────────────────────╯
+╭─ Commands ───────────────────────────────────────────────────────────────────────╮
+│ config           Setup Mailchimp API, Mailchimp server prefix, Google Service    │
+│                  account's json file, MUST SETUP this first before running this  │
+│                  program                                                         │
+│ config-file      To check your account config file, either account config file   │
+│                  or template config file.                                        │
+│ config-template  Setup Google spreadsheet, campaign info and its email content.  │
+│ create           Upload html email template to mailchimp server and create a     │
+│                  campaign.                                                       │
+╰──────────────────────────────────────────────────────────────────────────────────╯
+
+```
+
```

