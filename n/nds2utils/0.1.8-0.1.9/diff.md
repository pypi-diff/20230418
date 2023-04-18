# Comparing `tmp/nds2utils-0.1.8-py3-none-any.whl.zip` & `tmp/nds2utils-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,12 @@
-Zip file size: 62690 bytes, number of entries: 12
--rw-r--r--  2.0 unx      156 b- defN 22-Mar-31 06:29 nds2utils/__init__.py
--rw-r--r--  2.0 unx    71228 b- defN 22-Mar-16 21:59 nds2utils/dataUtils.py
--rw-r--r--  2.0 unx   125334 b- defN 23-Jan-23 00:41 nds2utils/data_utils.py
--rw-r--r--  2.0 unx    10592 b- defN 22-Oct-26 19:19 nds2utils/make_interactive_svg.py
--rw-r--r--  2.0 unx    44568 b- defN 22-Mar-08 01:35 nds2utils/plotUtils.py
--rw-r--r--  2.0 unx    45201 b- defN 22-Oct-26 19:19 nds2utils/plot_utils.py
--rw-r--r--  2.0 unx       22 b- defN 23-Jan-23 00:41 nds2utils/version.py
--rw-r--r--  2.0 unx     1074 b- defN 23-Jan-23 00:41 nds2utils-0.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     9806 b- defN 23-Jan-23 00:41 nds2utils-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-23 00:41 nds2utils-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jan-23 00:41 nds2utils-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      962 b- defN 23-Jan-23 00:41 nds2utils-0.1.8.dist-info/RECORD
-12 files, 309045 bytes uncompressed, 61090 bytes compressed:  80.2%
+Zip file size: 40354 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      156 b- defN 23-Feb-12 04:34 nds2utils/__init__.py
+-rw-r--r--  2.0 unx   125566 b- defN 23-Apr-18 17:40 nds2utils/data_utils.py
+-rw-r--r--  2.0 unx    10592 b- defN 23-Feb-12 04:34 nds2utils/make_interactive_svg.py
+-rw-r--r--  2.0 unx    45201 b- defN 23-Feb-12 04:34 nds2utils/plot_utils.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-18 17:28 nds2utils/version.py
+-rw-r--r--  2.0 unx     1074 b- defN 23-Apr-18 17:43 nds2utils-0.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9806 b- defN 23-Apr-18 17:43 nds2utils-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 17:43 nds2utils-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-18 17:43 nds2utils-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      802 b- defN 23-Apr-18 17:43 nds2utils-0.1.9.dist-info/RECORD
+10 files, 193321 bytes uncompressed, 38994 bytes compressed:  79.8%
```

## zipnote {}

```diff
@@ -1,37 +1,31 @@
 Filename: nds2utils/__init__.py
 Comment: 
 
-Filename: nds2utils/dataUtils.py
-Comment: 
-
 Filename: nds2utils/data_utils.py
 Comment: 
 
 Filename: nds2utils/make_interactive_svg.py
 Comment: 
 
-Filename: nds2utils/plotUtils.py
-Comment: 
-
 Filename: nds2utils/plot_utils.py
 Comment: 
 
 Filename: nds2utils/version.py
 Comment: 
 
-Filename: nds2utils-0.1.8.dist-info/LICENSE
+Filename: nds2utils-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: nds2utils-0.1.8.dist-info/METADATA
+Filename: nds2utils-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: nds2utils-0.1.8.dist-info/WHEEL
+Filename: nds2utils-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: nds2utils-0.1.8.dist-info/top_level.txt
+Filename: nds2utils-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: nds2utils-0.1.8.dist-info/RECORD
+Filename: nds2utils-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nds2utils/data_utils.py

```diff
@@ -327,16 +327,19 @@
         on_cds_machine = False
 
     # choose our NDS host
     gps_now = int(gpstime.gpsnow())
 
     # if on CDS and data is less than 28 days old
     if on_cds_machine and gps_now - gps_start < 3600 * 24 * 28:
-        server = "h1daqnds0"
-        port = 8088
+        nds_string = os.environ["NDSSERVER"]
+        server_port = nds_string.split(",")[0]
+
+        server = server_port.split(":")[0]
+        port = int(server_port.split(":")[1])
         allow_data_on_tape = "False"
     else:
         all_chans_in_h1 = np.all(["H1:" in chan for chan in channels])
         if all_chans_in_h1:
             server = "nds.ligo-wa.caltech.edu"
             port = 31200
             allow_data_on_tape = "True"
@@ -344,23 +347,28 @@
             server = "nds.ligo-la.caltech.edu"
             port = 31200
             allow_data_on_tape = "True"
         else:
             server = "nds.ligo.caltech.edu"
             port = 31200
             allow_data_on_tape = "True"
+
     return server, port, allow_data_on_tape
 
 def select_port_given_server(server):
     """Returns the port associated with a server
     """
     if server == "h1daqnds0":
         port = 8088
     elif server == "h1daqnds1":
         port = 8088
+    elif server == "l1nds1":
+        port = 8088
+    elif server == "l1nds0":
+        port = 8088
     elif server == "nds.ligo-wa.caltech.edu":
         port = 31200
     elif server == "nds.ligo-la.caltech.edu":
         port = 31200
     elif server == "nds.ligo.caltech.edu":
         port = 31200
     return port
```

## nds2utils/version.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

## Comparing `nds2utils-0.1.8.dist-info/LICENSE` & `nds2utils-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nds2utils-0.1.8.dist-info/METADATA` & `nds2utils-0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nds2utils
-Version: 0.1.8
+Version: 0.1.9
 Summary: nds2 utilities for reading LIGO data quickly and easily
 Home-page: https://git.ligo.org/craig-cahillane/nds2utils
 Author: Craig Cahillane
 Author-email: ccahilla@caltech.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `nds2utils-0.1.8.dist-info/RECORD` & `nds2utils-0.1.9.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 nds2utils/__init__.py,sha256=-gGj73mA34dczVL_JlSqWJm71Y9krOes9-Fjuhp5ozo,156
-nds2utils/dataUtils.py,sha256=qUyIC4NZzdu5fnMO7iJ1Q2y2a2BET7dklV27H1Fqpgo,71228
-nds2utils/data_utils.py,sha256=hdvpT1nBM5I6UO3QGJFZef2dD19oiT3_NVzQucbNMj8,125334
+nds2utils/data_utils.py,sha256=1cHU21fqYemzWnHK6ninhKDfnk-TaaZuP-KtlY1Hm0A,125566
 nds2utils/make_interactive_svg.py,sha256=SFNYxb7pptYPsENr_RJZtyu3fugiRmvwr4LWkn_5yTw,10592
-nds2utils/plotUtils.py,sha256=bIG7Ya3drotD5xhHnuN7rSDKOopq6c5gnbD8_pOnZ9k,44568
 nds2utils/plot_utils.py,sha256=jti5VqKGdoX2BYXve9y7YxLYOymZJzdcvcpCQUs_124,45201
-nds2utils/version.py,sha256=C69ADlbQREQlR15trneyA2sk8x0-oH4rDAX5fsv19_U,22
-nds2utils-0.1.8.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
-nds2utils-0.1.8.dist-info/METADATA,sha256=PkNlb2o0cMSPwlRWXIFxrWuWDwHqSd9okS9ILAdaQDg,9806
-nds2utils-0.1.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-nds2utils-0.1.8.dist-info/top_level.txt,sha256=IbvRdyU4pFzD67v0zDNImWIpTAT6_8voTVEuwyW7Ax0,10
-nds2utils-0.1.8.dist-info/RECORD,,
+nds2utils/version.py,sha256=XIaxbMbyiP-L3kguR1GhxirFblTXiHR1lMfDVITvHUI,22
+nds2utils-0.1.9.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
+nds2utils-0.1.9.dist-info/METADATA,sha256=zuj3gfalV4-gM436kbEk_x_s9JFbpht06bPz5kobWhg,9806
+nds2utils-0.1.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+nds2utils-0.1.9.dist-info/top_level.txt,sha256=IbvRdyU4pFzD67v0zDNImWIpTAT6_8voTVEuwyW7Ax0,10
+nds2utils-0.1.9.dist-info/RECORD,,
```

