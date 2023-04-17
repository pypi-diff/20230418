# Comparing `tmp/estimated-taxes-1.0.8.tar.gz` & `tmp/estimated-taxes-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estimated-taxes-1.0.8.tar", last modified: Fri Dec 25 10:49:20 2020, max compression
+gzip compressed data, was "estimated-taxes-1.0.9.tar", last modified: Fri Feb 19 21:38:57 2021, max compression
```

## Comparing `estimated-taxes-1.0.8.tar` & `estimated-taxes-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 nkouevda   (501) staff       (20)        0 2020-12-25 10:49:20.025738 estimated-taxes-1.0.8/
--rw-r--r--   0 nkouevda   (501) staff       (20)     2472 2020-12-25 10:49:20.025355 estimated-taxes-1.0.8/PKG-INFO
--rw-r--r--   0 nkouevda   (501) staff       (20)     1621 2020-12-25 02:24:06.000000 estimated-taxes-1.0.8/README.md
-drwxr-xr-x   0 nkouevda   (501) staff       (20)        0 2020-12-25 10:49:20.020044 estimated-taxes-1.0.8/estimated_taxes/
--rw-r--r--   0 nkouevda   (501) staff       (20)       37 2020-12-25 10:32:19.000000 estimated-taxes-1.0.8/estimated_taxes/__init__.py
--rw-r--r--   0 nkouevda   (501) staff       (20)       22 2020-12-25 10:47:19.000000 estimated-taxes-1.0.8/estimated_taxes/__version__.py
--rw-r--r--   0 nkouevda   (501) staff       (20)      456 2019-03-24 21:19:22.000000 estimated-taxes-1.0.8/estimated_taxes/argument_parser.py
--rw-r--r--   0 nkouevda   (501) staff       (20)     3551 2020-12-25 10:44:32.000000 estimated-taxes-1.0.8/estimated_taxes/calculator.py
-drwxr-xr-x   0 nkouevda   (501) staff       (20)        0 2020-12-25 10:49:20.024635 estimated-taxes-1.0.8/estimated_taxes/constants/
--rw-r--r--   0 nkouevda   (501) staff       (20)       35 2019-06-27 01:15:18.000000 estimated-taxes-1.0.8/estimated_taxes/constants/__init__.py
--rw-r--r--   0 nkouevda   (501) staff       (20)     9745 2020-12-25 10:44:32.000000 estimated-taxes-1.0.8/estimated_taxes/constants/ca.py
--rw-r--r--   0 nkouevda   (501) staff       (20)    10833 2020-12-25 10:44:32.000000 estimated-taxes-1.0.8/estimated_taxes/constants/fed.py
--rw-r--r--   0 nkouevda   (501) staff       (20)      625 2020-12-25 10:39:49.000000 estimated-taxes-1.0.8/estimated_taxes/estimated_taxes.py
--rw-r--r--   0 nkouevda   (501) staff       (20)      954 2020-12-25 10:48:28.000000 estimated-taxes-1.0.8/estimated_taxes/formatter.py
--rw-r--r--   0 nkouevda   (501) staff       (20)     1031 2019-03-25 00:20:28.000000 estimated-taxes-1.0.8/estimated_taxes/loader.py
--rw-r--r--   0 nkouevda   (501) staff       (20)     3750 2020-12-25 10:44:32.000000 estimated-taxes-1.0.8/estimated_taxes/model.py
-drwxr-xr-x   0 nkouevda   (501) staff       (20)        0 2020-12-25 10:49:20.022918 estimated-taxes-1.0.8/estimated_taxes.egg-info/
--rw-r--r--   0 nkouevda   (501) staff       (20)     2472 2020-12-25 10:49:19.000000 estimated-taxes-1.0.8/estimated_taxes.egg-info/PKG-INFO
--rw-r--r--   0 nkouevda   (501) staff       (20)      596 2020-12-25 10:49:19.000000 estimated-taxes-1.0.8/estimated_taxes.egg-info/SOURCES.txt
--rw-r--r--   0 nkouevda   (501) staff       (20)        1 2020-12-25 10:49:19.000000 estimated-taxes-1.0.8/estimated_taxes.egg-info/dependency_links.txt
--rw-r--r--   0 nkouevda   (501) staff       (20)       74 2020-12-25 10:49:19.000000 estimated-taxes-1.0.8/estimated_taxes.egg-info/entry_points.txt
--rw-r--r--   0 nkouevda   (501) staff       (20)        7 2020-12-25 10:49:19.000000 estimated-taxes-1.0.8/estimated_taxes.egg-info/requires.txt
--rw-r--r--   0 nkouevda   (501) staff       (20)       16 2020-12-25 10:49:19.000000 estimated-taxes-1.0.8/estimated_taxes.egg-info/top_level.txt
--rw-r--r--   0 nkouevda   (501) staff       (20)       38 2020-12-25 10:49:20.025885 estimated-taxes-1.0.8/setup.cfg
--rw-r--r--   0 nkouevda   (501) staff       (20)      745 2020-01-04 20:31:38.000000 estimated-taxes-1.0.8/setup.py
+drwxr-xr-x   0 nkouevda   (501) staff       (20)        0 2021-02-19 21:38:57.489900 estimated-taxes-1.0.9/
+-rw-r--r--   0 nkouevda   (501) staff       (20)     2472 2021-02-19 21:38:57.489595 estimated-taxes-1.0.9/PKG-INFO
+-rw-r--r--   0 nkouevda   (501) staff       (20)     1621 2020-12-25 02:24:06.000000 estimated-taxes-1.0.9/README.md
+drwxr-xr-x   0 nkouevda   (501) staff       (20)        0 2021-02-19 21:38:57.485344 estimated-taxes-1.0.9/estimated_taxes/
+-rw-r--r--   0 nkouevda   (501) staff       (20)       37 2020-12-25 10:32:19.000000 estimated-taxes-1.0.9/estimated_taxes/__init__.py
+-rw-r--r--   0 nkouevda   (501) staff       (20)      659 2021-01-02 00:47:49.000000 estimated-taxes-1.0.9/estimated_taxes/__main__.py
+-rw-r--r--   0 nkouevda   (501) staff       (20)       22 2021-02-19 21:38:15.000000 estimated-taxes-1.0.9/estimated_taxes/__version__.py
+-rw-r--r--   0 nkouevda   (501) staff       (20)      456 2019-03-24 21:19:22.000000 estimated-taxes-1.0.9/estimated_taxes/argument_parser.py
+-rw-r--r--   0 nkouevda   (501) staff       (20)     3551 2020-12-25 10:44:32.000000 estimated-taxes-1.0.9/estimated_taxes/calculator.py
+drwxr-xr-x   0 nkouevda   (501) staff       (20)        0 2021-02-19 21:38:57.489113 estimated-taxes-1.0.9/estimated_taxes/constants/
+-rw-r--r--   0 nkouevda   (501) staff       (20)       35 2019-06-27 01:15:18.000000 estimated-taxes-1.0.9/estimated_taxes/constants/__init__.py
+-rw-r--r--   0 nkouevda   (501) staff       (20)    10036 2021-02-19 21:38:15.000000 estimated-taxes-1.0.9/estimated_taxes/constants/ca.py
+-rw-r--r--   0 nkouevda   (501) staff       (20)    13844 2021-02-19 21:38:15.000000 estimated-taxes-1.0.9/estimated_taxes/constants/fed.py
+-rw-r--r--   0 nkouevda   (501) staff       (20)      663 2021-02-19 21:38:15.000000 estimated-taxes-1.0.9/estimated_taxes/constants/util.py
+-rw-r--r--   0 nkouevda   (501) staff       (20)      954 2021-02-19 21:38:25.000000 estimated-taxes-1.0.9/estimated_taxes/formatter.py
+-rw-r--r--   0 nkouevda   (501) staff       (20)     1031 2019-03-25 00:20:28.000000 estimated-taxes-1.0.9/estimated_taxes/loader.py
+-rw-r--r--   0 nkouevda   (501) staff       (20)     3783 2021-02-19 21:38:15.000000 estimated-taxes-1.0.9/estimated_taxes/model.py
+drwxr-xr-x   0 nkouevda   (501) staff       (20)        0 2021-02-19 21:38:57.487496 estimated-taxes-1.0.9/estimated_taxes.egg-info/
+-rw-r--r--   0 nkouevda   (501) staff       (20)     2472 2021-02-19 21:38:57.000000 estimated-taxes-1.0.9/estimated_taxes.egg-info/PKG-INFO
+-rw-r--r--   0 nkouevda   (501) staff       (20)      623 2021-02-19 21:38:57.000000 estimated-taxes-1.0.9/estimated_taxes.egg-info/SOURCES.txt
+-rw-r--r--   0 nkouevda   (501) staff       (20)        1 2021-02-19 21:38:57.000000 estimated-taxes-1.0.9/estimated_taxes.egg-info/dependency_links.txt
+-rw-r--r--   0 nkouevda   (501) staff       (20)       67 2021-02-19 21:38:57.000000 estimated-taxes-1.0.9/estimated_taxes.egg-info/entry_points.txt
+-rw-r--r--   0 nkouevda   (501) staff       (20)        7 2021-02-19 21:38:57.000000 estimated-taxes-1.0.9/estimated_taxes.egg-info/requires.txt
+-rw-r--r--   0 nkouevda   (501) staff       (20)       16 2021-02-19 21:38:57.000000 estimated-taxes-1.0.9/estimated_taxes.egg-info/top_level.txt
+-rw-r--r--   0 nkouevda   (501) staff       (20)       38 2021-02-19 21:38:57.490025 estimated-taxes-1.0.9/setup.cfg
+-rw-r--r--   0 nkouevda   (501) staff       (20)      738 2021-01-02 00:49:25.000000 estimated-taxes-1.0.9/setup.py
```

### Comparing `estimated-taxes-1.0.8/PKG-INFO` & `estimated-taxes-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estimated-taxes
-Version: 1.0.8
+Version: 1.0.9
 Summary: Estimated taxes calculator
 Home-page: https://github.com/nkouevda/estimated-taxes
 Author: Nikita Kouevda
 Author-email: nkouevda@gmail.com
 License: MIT
 Description: # estimated-taxes
```

### Comparing `estimated-taxes-1.0.8/README.md` & `estimated-taxes-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `estimated-taxes-1.0.8/estimated_taxes/calculator.py` & `estimated-taxes-1.0.9/estimated_taxes/calculator.py`

 * *Files identical despite different names*

### Comparing `estimated-taxes-1.0.8/estimated_taxes/constants/ca.py` & `estimated-taxes-1.0.9/estimated_taxes/constants/ca.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,40 +13,41 @@
 - Income tax
   - https://www.ftb.ca.gov/forms/2016/16_540bk.pdf
   - https://www.ftb.ca.gov/forms/2017/17-540-booklet.html
   - (2018 is only available by request)
   - https://www.ftb.ca.gov/forms/2019/2019-540-booklet.pdf
 """
 
+from . import util
 from .. import model
 
 WITHHOLDING_ALLOWANCE = {
     2016: 119.90,
     2017: 122.10,
     2018: 125.40,
     2019: 129.80,
     2020: 134.20,
     2021: 136.40,
 }
 
-INCOME_TAX_WITHHOLDING = {
+INCOME_TAX_WITHHOLDING = util.copy_single_to_married_separately({
     2016: {
         model.FilingStatus.SINGLE: model.BracketGroup.from_dict({
             0: 0.011,
             7850: 0.022,
             18610: 0.044,
             29372: 0.066,
             40773: 0.088,
             51530: 0.1023,
             263222: 0.1133,
             315866: 0.1243,
             526443: 0.1353,
             1000000: 0.1463,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.011,
             15700: 0.022,
             37220: 0.044,
             58744: 0.066,
             81546: 0.088,
             103060: 0.1023,
             526444: 0.1133,
@@ -64,15 +65,15 @@
             41629: 0.088,
             52612: 0.1023,
             268750: 0.1133,
             322499: 0.1243,
             537498: 0.1353,
             1000000: 0.1463,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.011,
             16030: 0.022,
             38002: 0.044,
             59978: 0.066,
             83258: 0.088,
             105224: 0.1023,
             537500: 0.1133,
@@ -90,15 +91,15 @@
             42711: 0.088,
             53980: 0.1023,
             275738: 0.1133,
             330884: 0.1243,
             551473: 0.1353,
             1000000: 0.1463,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.011,
             16446: 0.022,
             38990: 0.044,
             61538: 0.066,
             85422: 0.088,
             107960: 0.1023,
             551476: 0.1133,
@@ -116,15 +117,15 @@
             44377: 0.088,
             56085: 0.1023,
             286492: 0.1133,
             343788: 0.1243,
             572980: 0.1353,
             1000000: 0.1463,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.011,
             17088: 0.022,
             40510: 0.044,
             63938: 0.066,
             88754: 0.088,
             112170: 0.1023,
             572984: 0.1133,
@@ -142,15 +143,15 @@
             45753: 0.088,
             57824: 0.1023,
             295373: 0.1133,
             354445: 0.1243,
             590742: 0.1353,
             1000000: 0.1463,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.011,
             17618: 0.022,
             41766: 0.044,
             65920: 0.066,
             91506: 0.088,
             115648: 0.1023,
             590746: 0.1133,
@@ -168,75 +169,75 @@
             46394: 0.088,
             58634: 0.1023,
             299508: 0.1133,
             359407: 0.1243,
             599012: 0.1353,
             1000000: 0.1463,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.011,
             17864: 0.022,
             42350: 0.044,
             66842: 0.066,
             92788: 0.088,
             117268: 0.1023,
             599016: 0.1133,
             718814: 0.1243,
             1000000: 0.1353,
             1198024: 0.1463,
         }),
     },
-}
+})
 
-STANDARD_DEDUCTION = {
+STANDARD_DEDUCTION = util.copy_single_to_married_separately({
     2015: {
         model.FilingStatus.SINGLE: 4044,
-        model.FilingStatus.MARRIED: 8088,
+        model.FilingStatus.MARRIED_JOINTLY: 8088,
     },
     2016: {
         model.FilingStatus.SINGLE: 4129,
-        model.FilingStatus.MARRIED: 8258,
+        model.FilingStatus.MARRIED_JOINTLY: 8258,
     },
     2017: {
         model.FilingStatus.SINGLE: 4236,
-        model.FilingStatus.MARRIED: 8472,
+        model.FilingStatus.MARRIED_JOINTLY: 8472,
     },
     2018: {
         model.FilingStatus.SINGLE: 4401,
-        model.FilingStatus.MARRIED: 8802,
+        model.FilingStatus.MARRIED_JOINTLY: 8802,
     },
     2019: {
         model.FilingStatus.SINGLE: 4537,
-        model.FilingStatus.MARRIED: 9074,
+        model.FilingStatus.MARRIED_JOINTLY: 9074,
     },
     2020: {
         model.FilingStatus.SINGLE: 4601,
-        model.FilingStatus.MARRIED: 9202,
+        model.FilingStatus.MARRIED_JOINTLY: 9202,
     },
     # TODO(nkouevda): Update; copied from 2020 for now
     2021: {
         model.FilingStatus.SINGLE: 4601,
-        model.FilingStatus.MARRIED: 9202,
+        model.FilingStatus.MARRIED_JOINTLY: 9202,
     },
-}
+})
 
-INCOME_TAX = {
+INCOME_TAX = util.copy_single_to_married_separately({
     2016: {
         model.FilingStatus.SINGLE: model.BracketGroup.from_dict({
             0: 0.01,
             8015: 0.02,
             19001: 0.04,
             29989: 0.06,
             41629: 0.08,
             52612: 0.093,
             268750: 0.103,
             322499: 0.113,
             537498: 0.123,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.01,
             16030: 0.02,
             38002: 0.04,
             59978: 0.06,
             83258: 0.08,
             105224: 0.093,
             537500: 0.103,
@@ -252,15 +253,15 @@
             30769: 0.06,
             42711: 0.08,
             53980: 0.093,
             275738: 0.103,
             330884: 0.113,
             551473: 0.123,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.01,
             16446: 0.02,
             38990: 0.04,
             61538: 0.06,
             85422: 0.08,
             107960: 0.093,
             551476: 0.103,
@@ -276,15 +277,15 @@
             31969: 0.06,
             44377: 0.08,
             56085: 0.093,
             286492: 0.103,
             343788: 0.113,
             572980: 0.123,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.01,
             17088: 0.02,
             40510: 0.04,
             63938: 0.06,
             88754: 0.08,
             112170: 0.093,
             572984: 0.103,
@@ -300,15 +301,15 @@
             32960: 0.06,
             45753: 0.08,
             57824: 0.093,
             295373: 0.103,
             354445: 0.113,
             590742: 0.123,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.01,
             17618: 0.02,
             41766: 0.04,
             65920: 0.06,
             91506: 0.08,
             115648: 0.093,
             590746: 0.103,
@@ -324,15 +325,15 @@
             33421: 0.06,
             46394: 0.08,
             58634: 0.093,
             299508: 0.103,
             359407: 0.113,
             599012: 0.123,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.01,
             17864: 0.02,
             42350: 0.04,
             66842: 0.06,
             92788: 0.08,
             117268: 0.093,
             599016: 0.103,
@@ -349,20 +350,20 @@
             33421: 0.06,
             46394: 0.08,
             58634: 0.093,
             299508: 0.103,
             359407: 0.113,
             599012: 0.123,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.01,
             17864: 0.02,
             42350: 0.04,
             66842: 0.06,
             92788: 0.08,
             117268: 0.093,
             599016: 0.103,
             718814: 0.113,
             1198024: 0.123,
         }),
     },
-}
+})
```

### Comparing `estimated-taxes-1.0.8/estimated_taxes/constants/fed.py` & `estimated-taxes-1.0.9/estimated_taxes/constants/fed.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,38 +14,39 @@
   - https://www.irs.gov/pub/irs-prior/i1040gi--2016.pdf
   - https://www.irs.gov/pub/irs-prior/i1040gi--2017.pdf
   - https://www.irs.gov/pub/irs-prior/i1040gi--2018.pdf
   - https://www.irs.gov/pub/irs-prior/i1040gi--2019.pdf
   - https://www.irs.gov/pub/irs-pdf/i1040gi.pdf
 """
 
+from . import util
 from .. import model
 
 WITHHOLDING_ALLOWANCE = {
     2016: 4050,
     2017: 4050,
     2018: 4150,
     2019: 4200,
     2020: 4300,
     2021: 4300,
 }
 
-INCOME_TAX_WITHHOLDING = {
+INCOME_TAX_WITHHOLDING = util.copy_single_to_married_separately({
     2016: {
         model.FilingStatus.SINGLE: model.BracketGroup.from_dict({
             0: 0.00,
             2250: 0.10,
             11525: 0.15,
             39900: 0.25,
             93400: 0.28,
             192400: 0.33,
             415600: 0.35,
             417300: 0.396,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.00,
             8550: 0.10,
             27100: 0.15,
             83850: 0.25,
             160450: 0.28,
             240000: 0.33,
             421900: 0.35,
@@ -59,15 +60,15 @@
             11625: 0.15,
             40250: 0.25,
             94200: 0.28,
             193950: 0.33,
             419000: 0.35,
             420700: 0.396,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.00,
             8650: 0.10,
             27300: 0.15,
             84550: 0.25,
             161750: 0.28,
             242000: 0.33,
             425350: 0.35,
@@ -81,15 +82,15 @@
             13225: 0.12,
             42400: 0.22,
             86200: 0.24,
             161200: 0.32,
             203700: 0.35,
             503700: 0.37,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.00,
             11550: 0.10,
             30600: 0.12,
             88950: 0.22,
             176550: 0.24,
             326550: 0.32,
             411550: 0.35,
@@ -103,15 +104,15 @@
             13500: 0.12,
             43275: 0.22,
             88000: 0.24,
             164525: 0.32,
             207900: 0.35,
             514100: 0.37,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.00,
             11800: 0.10,
             31200: 0.12,
             90750: 0.22,
             180200: 0.24,
             333250: 0.32,
             420000: 0.35,
@@ -125,15 +126,15 @@
             13675: 0.12,
             43925: 0.22,
             89325: 0.24,
             167100: 0.32,
             211150: 0.35,
             522200: 0.37,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.00,
             11900: 0.10,
             31650: 0.12,
             92150: 0.22,
             182950: 0.24,
             338500: 0.32,
             426600: 0.35,
@@ -147,26 +148,26 @@
             13900: 0.12,
             44475: 0.22,
             90325: 0.24,
             168875: 0.32,
             213375: 0.35,
             527550: 0.37,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.00,
             12200: 0.10,
             32100: 0.12,
             93250: 0.22,
             184950: 0.24,
             342050: 0.32,
             431050: 0.35,
             640500: 0.37,
         }),
     },
-}
+})
 
 WITHHOLDING_SUPPLEMENTAL_RATE = {
     2016: 0.25,
     2017: 0.25,
     2018: 0.22,
     2019: 0.22,
     2020: 0.22,
@@ -178,40 +179,40 @@
     2017: float('inf'),
     2018: 10000,
     2019: 10000,
     2020: 10000,
     2021: 10000,
 }
 
-STANDARD_DEDUCTION = {
+STANDARD_DEDUCTION = util.copy_single_to_married_separately({
     2016: {
         model.FilingStatus.SINGLE: 6300,
-        model.FilingStatus.MARRIED: 12600,
+        model.FilingStatus.MARRIED_JOINTLY: 12600,
     },
     2017: {
         model.FilingStatus.SINGLE: 6350,
-        model.FilingStatus.MARRIED: 12700,
+        model.FilingStatus.MARRIED_JOINTLY: 12700,
     },
     2018: {
         model.FilingStatus.SINGLE: 12000,
-        model.FilingStatus.MARRIED: 24000,
+        model.FilingStatus.MARRIED_JOINTLY: 24000,
     },
     2019: {
         model.FilingStatus.SINGLE: 12200,
-        model.FilingStatus.MARRIED: 24400,
+        model.FilingStatus.MARRIED_JOINTLY: 24400,
     },
     2020: {
         model.FilingStatus.SINGLE: 12400,
-        model.FilingStatus.MARRIED: 24800,
+        model.FilingStatus.MARRIED_JOINTLY: 24800,
     },
     2021: {
         model.FilingStatus.SINGLE: 12550,
-        model.FilingStatus.MARRIED: 25100,
+        model.FilingStatus.MARRIED_JOINTLY: 25100,
     },
-}
+})
 
 PERSONAL_EXEMPTION = {
     2016: 4050,
     2017: 4050,
     2018: 0,
     2019: 0,
     2020: 0,
@@ -227,203 +228,289 @@
             9275: 0.15,
             37650: 0.25,
             91150: 0.28,
             190150: 0.33,
             413350: 0.35,
             415050: 0.396,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.10,
             18550: 0.15,
             75300: 0.25,
             151900: 0.28,
             231450: 0.33,
             413350: 0.35,
             466950: 0.396,
         }),
+        model.FilingStatus.MARRIED_SEPARATELY: model.BracketGroup.from_dict({
+            0: 0.10,
+            9275: 0.15,
+            37650: 0.25,
+            75950: 0.28,
+            115725: 0.33,
+            206675: 0.35,
+            233475: 0.396,
+        }),
     },
     2017: {
         model.FilingStatus.SINGLE: model.BracketGroup.from_dict({
             0: 0.10,
             9325: 0.15,
             37950: 0.25,
             91900: 0.28,
             191650: 0.33,
             416700: 0.35,
             418400: 0.396,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.10,
             18650: 0.15,
             75900: 0.25,
             153100: 0.28,
             233350: 0.33,
             416700: 0.35,
             470700: 0.396,
         }),
+        model.FilingStatus.MARRIED_SEPARATELY: model.BracketGroup.from_dict({
+            0: 0.10,
+            9325: 0.15,
+            37950: 0.25,
+            76550: 0.28,
+            116675: 0.33,
+            208350: 0.35,
+            235350: 0.396,
+        }),
     },
     2018: {
         model.FilingStatus.SINGLE: model.BracketGroup.from_dict({
             0: 0.10,
             9525: 0.12,
             38700: 0.22,
             82500: 0.24,
             157500: 0.32,
             200000: 0.35,
             500000: 0.37,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.10,
             19050: 0.12,
             77400: 0.22,
             165000: 0.24,
             315000: 0.32,
             400000: 0.35,
             600000: 0.37,
         }),
+        model.FilingStatus.MARRIED_SEPARATELY: model.BracketGroup.from_dict({
+            0: 0.10,
+            9525: 0.12,
+            38700: 0.22,
+            82500: 0.24,
+            157500: 0.32,
+            200000: 0.35,
+            300000: 0.37,
+        }),
     },
     2019: {
         model.FilingStatus.SINGLE: model.BracketGroup.from_dict({
             0: 0.10,
             9700: 0.12,
             39475: 0.22,
             84200: 0.24,
             160725: 0.32,
             204100: 0.35,
             510300: 0.37,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.10,
             19400: 0.12,
             78950: 0.22,
             168400: 0.24,
             321450: 0.32,
             408200: 0.35,
             612350: 0.37,
         }),
+        model.FilingStatus.MARRIED_SEPARATELY: model.BracketGroup.from_dict({
+            0: 0.10,
+            9700: 0.12,
+            39475: 0.22,
+            84200: 0.24,
+            160725: 0.32,
+            204100: 0.35,
+            306175: 0.37,
+        }),
     },
     2020: {
         model.FilingStatus.SINGLE: model.BracketGroup.from_dict({
             0: 0.10,
             9875: 0.12,
             40125: 0.22,
             85525: 0.24,
             163300: 0.32,
             207350: 0.35,
             518400: 0.37,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.10,
             19750: 0.12,
             80250: 0.22,
             171050: 0.24,
             326600: 0.32,
             414700: 0.35,
             622050: 0.37,
         }),
+        model.FilingStatus.MARRIED_SEPARATELY: model.BracketGroup.from_dict({
+            0: 0.10,
+            9875: 0.12,
+            40125: 0.22,
+            85525: 0.24,
+            163300: 0.32,
+            207350: 0.35,
+            311025: 0.37,
+        }),
     },
     2021: {
         model.FilingStatus.SINGLE: model.BracketGroup.from_dict({
             0: 0.10,
             9950: 0.12,
             40525: 0.22,
             86375: 0.24,
             164925: 0.32,
             209425: 0.35,
             523600: 0.37,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.10,
             19900: 0.12,
             81050: 0.22,
             172750: 0.24,
             329850: 0.32,
             418850: 0.35,
             628300: 0.37,
         }),
+        model.FilingStatus.MARRIED_SEPARATELY: model.BracketGroup.from_dict({
+            0: 0.10,
+            9950: 0.12,
+            40525: 0.22,
+            86375: 0.24,
+            164925: 0.32,
+            209425: 0.35,
+            314150: 0.37,
+        }),
     },
 }
 
 LONG_TERM_CAPITAL_GAINS_TAX = {
     2016: {
         model.FilingStatus.SINGLE: model.BracketGroup.from_dict({
             0: 0.0,
             37650: 0.15,
             415050: 0.20,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.0,
             75300: 0.15,
             466950: 0.20,
         }),
+        model.FilingStatus.MARRIED_SEPARATELY: model.BracketGroup.from_dict({
+            0: 0.0,
+            37650: 0.15,
+            233475: 0.20,
+        }),
     },
     2017: {
         model.FilingStatus.SINGLE: model.BracketGroup.from_dict({
             0: 0.0,
             37950: 0.15,
             418400: 0.20,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.0,
             75900: 0.15,
             470700: 0.20,
         }),
+        model.FilingStatus.MARRIED_SEPARATELY: model.BracketGroup.from_dict({
+            0: 0.0,
+            37950: 0.15,
+            235350: 0.20,
+        }),
     },
     2018: {
         model.FilingStatus.SINGLE: model.BracketGroup.from_dict({
             0: 0.0,
             38600: 0.15,
             425800: 0.20,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.0,
             77200: 0.15,
             479000: 0.20,
         }),
+        model.FilingStatus.MARRIED_SEPARATELY: model.BracketGroup.from_dict({
+            0: 0.0,
+            38600: 0.15,
+            239500: 0.20,
+        }),
     },
     2019: {
         model.FilingStatus.SINGLE: model.BracketGroup.from_dict({
             0: 0.0,
             39375: 0.15,
             434550: 0.20,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.0,
             78750: 0.15,
             488850: 0.20,
         }),
+        model.FilingStatus.MARRIED_SEPARATELY: model.BracketGroup.from_dict({
+            0: 0.0,
+            39375: 0.15,
+            244425: 0.20,
+        }),
     },
     2020: {
         model.FilingStatus.SINGLE: model.BracketGroup.from_dict({
             0: 0.0,
             40000: 0.15,
             441450: 0.20,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.0,
             80000: 0.15,
             496600: 0.20,
         }),
+        model.FilingStatus.MARRIED_SEPARATELY: model.BracketGroup.from_dict({
+            0: 0.0,
+            40000: 0.15,
+            248300: 0.20,
+        }),
     },
     2021: {
         model.FilingStatus.SINGLE: model.BracketGroup.from_dict({
             0: 0.0,
             40400: 0.15,
             445850: 0.20,
         }),
-        model.FilingStatus.MARRIED: model.BracketGroup.from_dict({
+        model.FilingStatus.MARRIED_JOINTLY: model.BracketGroup.from_dict({
             0: 0.0,
             80800: 0.15,
             501600: 0.20,
         }),
+        model.FilingStatus.MARRIED_SEPARATELY: model.BracketGroup.from_dict({
+            0: 0.0,
+            40400: 0.15,
+            250800: 0.20,
+        }),
     },
 }
 
 ADDITIONAL_MEDICARE_TAX = {
     model.FilingStatus.SINGLE: model.AdditionalTax(200000, 0.009),
-    model.FilingStatus.MARRIED: model.AdditionalTax(250000, 0.009),
+    model.FilingStatus.MARRIED_JOINTLY: model.AdditionalTax(250000, 0.009),
+    model.FilingStatus.MARRIED_SEPARATELY: model.AdditionalTax(125000, 0.009),
 }
 
 NET_INVESTMENT_INCOME_TAX = {
     model.FilingStatus.SINGLE: model.AdditionalTax(200000, 0.038),
-    model.FilingStatus.MARRIED: model.AdditionalTax(250000, 0.038),
+    model.FilingStatus.MARRIED_JOINTLY: model.AdditionalTax(250000, 0.038),
+    model.FilingStatus.MARRIED_SEPARATELY: model.AdditionalTax(125000, 0.038),
 }
```

### Comparing `estimated-taxes-1.0.8/estimated_taxes/estimated_taxes.py` & `estimated-taxes-1.0.9/estimated_taxes/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import sys
+
 from . import argument_parser
 from . import calculator
 from . import formatter
 from . import loader
 
 
 def main():
@@ -15,10 +17,12 @@
 
   fed_tax = calculator.get_fed_tax(data, fed_withholding.tax, ca_withholding.tax)
   ca_tax = calculator.get_ca_tax(data, ca_withholding.tax)
 
   output = formatter.format(data, fed_withholding, ca_withholding, fed_tax, ca_tax)
   print(output)
 
+  return 0
+
 
 if __name__ == '__main__':
-  main()
+  sys.exit(main())
```

### Comparing `estimated-taxes-1.0.8/estimated_taxes/formatter.py` & `estimated-taxes-1.0.9/estimated_taxes/formatter.py`

 * *Files identical despite different names*

### Comparing `estimated-taxes-1.0.8/estimated_taxes/loader.py` & `estimated-taxes-1.0.9/estimated_taxes/loader.py`

 * *Files identical despite different names*

### Comparing `estimated-taxes-1.0.8/estimated_taxes/model.py` & `estimated-taxes-1.0.9/estimated_taxes/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 # `constants.*` depends on `model`, so we can't import from `constants` here
 MIN_YEAR = 2016
 MAX_YEAR = 2021
 
 
 class FilingStatus(Enum):
   SINGLE = 1
-  MARRIED = 2
+  MARRIED_JOINTLY = 2
+  MARRIED_SEPARATELY = 3
 
 
 @dataclass(frozen=True)
 class Bracket(object):
   lower_bound: float
   upper_bound: float
   rate: float
```

### Comparing `estimated-taxes-1.0.8/estimated_taxes.egg-info/PKG-INFO` & `estimated-taxes-1.0.9/estimated_taxes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estimated-taxes
-Version: 1.0.8
+Version: 1.0.9
 Summary: Estimated taxes calculator
 Home-page: https://github.com/nkouevda/estimated-taxes
 Author: Nikita Kouevda
 Author-email: nkouevda@gmail.com
 License: MIT
 Description: # estimated-taxes
```

### Comparing `estimated-taxes-1.0.8/estimated_taxes.egg-info/SOURCES.txt` & `estimated-taxes-1.0.9/estimated_taxes.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 README.md
 setup.py
 estimated_taxes/__init__.py
+estimated_taxes/__main__.py
 estimated_taxes/__version__.py
 estimated_taxes/argument_parser.py
 estimated_taxes/calculator.py
-estimated_taxes/estimated_taxes.py
 estimated_taxes/formatter.py
 estimated_taxes/loader.py
 estimated_taxes/model.py
 estimated_taxes.egg-info/PKG-INFO
 estimated_taxes.egg-info/SOURCES.txt
 estimated_taxes.egg-info/dependency_links.txt
 estimated_taxes.egg-info/entry_points.txt
 estimated_taxes.egg-info/requires.txt
 estimated_taxes.egg-info/top_level.txt
 estimated_taxes/constants/__init__.py
 estimated_taxes/constants/ca.py
-estimated_taxes/constants/fed.py
+estimated_taxes/constants/fed.py
+estimated_taxes/constants/util.py
```

### Comparing `estimated-taxes-1.0.8/setup.py` & `estimated-taxes-1.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,11 +20,11 @@
     license='MIT',
     packages=setuptools.find_packages(),
     install_requires=[
         'pyyaml',
     ],
     entry_points={
         'console_scripts': [
-            'estimated-taxes=estimated_taxes.estimated_taxes:main',
+            'estimated-taxes=estimated_taxes.__main__:main',
         ],
     },
 )
```

