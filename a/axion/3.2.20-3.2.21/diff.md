# Comparing `tmp/axion-3.2.20-cp311-cp311-win_amd64.whl.zip` & `tmp/axion-3.2.21-cp311-cp311-macosx_10_9_universal2.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 620200 bytes, number of entries: 20
--rw-rw-rw-  2.0 fat     1080 b- defN 23-Apr-06 09:50 axion-3.2.20.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1289 b- defN 23-Apr-06 09:50 axion-3.2.20.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Apr-06 09:50 axion-3.2.20.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-06 09:50 axion-3.2.20.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      381 b- defN 23-Apr-06 09:50 axion-3.2.20.dist-info/RECORD
--rw-rw-rw-  2.0 fat    20992 b- defN 23-Apr-06 09:50 axion/__init__.pyd
--rw-rw-rw-  2.0 fat    80384 b- defN 23-Apr-06 09:49 axion/executor.pyd
--rw-rw-rw-  2.0 fat   283648 b- defN 23-Apr-06 09:49 axion/factory.pyd
--rw-rw-rw-  2.0 fat    79360 b- defN 23-Apr-06 09:49 axion/pipeline.pyd
--rw-rw-rw-  2.0 fat    53248 b- defN 23-Apr-06 09:49 axion/queues.pyd
--rw-rw-rw-  2.0 fat   194560 b- defN 23-Apr-06 09:49 axion/recorder.pyd
--rw-rw-rw-  2.0 fat    54784 b- defN 23-Apr-06 09:50 axion/scheduler.pyd
--rw-rw-rw-  2.0 fat    71680 b- defN 23-Apr-06 09:50 axion/service.pyd
--rw-rw-rw-  2.0 fat    54784 b- defN 23-Apr-06 09:50 axion/thread.pyd
--rw-rw-rw-  2.0 fat    22016 b- defN 23-Apr-06 09:50 axion/inst/__init__.pyd
--rw-rw-rw-  2.0 fat    52224 b- defN 23-Apr-06 09:50 axion/inst/ibase.pyd
--rw-rw-rw-  2.0 fat   221184 b- defN 23-Apr-06 09:50 axion/inst/nbase.pyd
--rw-rw-rw-  2.0 fat    80384 b- defN 23-Apr-06 09:50 axion/inst/sbase.pyd
--rw-rw-rw-  2.0 fat    61440 b- defN 23-Apr-06 09:50 axion/inst/tbase.pyd
--rw-rw-rw-  2.0 fat    61440 b- defN 23-Apr-06 09:50 axion/inst/utility.pyd
-20 files, 1394981 bytes uncompressed, 617786 bytes compressed:  55.7%
+Zip file size: 1468593 bytes, number of entries: 20
+-rw-r--r--  2.0 unx     1059 b- defN 23-Apr-18 13:17 axion-3.2.21.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1235 b- defN 23-Apr-18 13:17 axion-3.2.21.dist-info/METADATA
+-rw-r--r--  2.0 unx      115 b- defN 23-Apr-18 13:17 axion-3.2.21.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-18 13:17 axion-3.2.21.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      381 b- defN 23-Apr-18 13:17 axion-3.2.21.dist-info/RECORD
+-rwxr-xr-x  2.0 unx   122779 b- defN 23-Apr-18 13:16 axion/__init__.so
+-rwxr-xr-x  2.0 unx   308971 b- defN 23-Apr-18 13:17 axion/executor.so
+-rwxr-xr-x  2.0 unx   912794 b- defN 23-Apr-18 13:17 axion/factory.so
+-rwxr-xr-x  2.0 unx   308955 b- defN 23-Apr-18 13:17 axion/pipeline.so
+-rwxr-xr-x  2.0 unx   219465 b- defN 23-Apr-18 13:16 axion/queues.so
+-rwxr-xr-x  2.0 unx   680747 b- defN 23-Apr-18 13:16 axion/recorder.so
+-rwxr-xr-x  2.0 unx   220172 b- defN 23-Apr-18 13:17 axion/scheduler.so
+-rwxr-xr-x  2.0 unx   275546 b- defN 23-Apr-18 13:16 axion/service.so
+-rwxr-xr-x  2.0 unx   220233 b- defN 23-Apr-18 13:16 axion/thread.so
+-rwxr-xr-x  2.0 unx   122907 b- defN 23-Apr-18 13:17 axion/inst/__init__.so
+-rwxr-xr-x  2.0 unx   218168 b- defN 23-Apr-18 13:17 axion/inst/ibase.so
+-rwxr-xr-x  2.0 unx   732696 b- defN 23-Apr-18 13:17 axion/inst/nbase.so
+-rwxr-xr-x  2.0 unx   312232 b- defN 23-Apr-18 13:17 axion/inst/sbase.so
+-rwxr-xr-x  2.0 unx   271544 b- defN 23-Apr-18 13:17 axion/inst/tbase.so
+-rwxr-xr-x  2.0 unx   238826 b- defN 23-Apr-18 13:17 axion/inst/utility.so
+20 files, 5168826 bytes uncompressed, 1466209 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -1,61 +1,61 @@
-Filename: axion-3.2.20.dist-info/LICENSE
+Filename: axion-3.2.21.dist-info/LICENSE
 Comment: 
 
-Filename: axion-3.2.20.dist-info/METADATA
+Filename: axion-3.2.21.dist-info/METADATA
 Comment: 
 
-Filename: axion-3.2.20.dist-info/WHEEL
+Filename: axion-3.2.21.dist-info/WHEEL
 Comment: 
 
-Filename: axion-3.2.20.dist-info/top_level.txt
+Filename: axion-3.2.21.dist-info/top_level.txt
 Comment: 
 
-Filename: axion-3.2.20.dist-info/RECORD
+Filename: axion-3.2.21.dist-info/RECORD
 Comment: 
 
-Filename: axion/__init__.pyd
+Filename: axion/__init__.so
 Comment: 
 
-Filename: axion/executor.pyd
+Filename: axion/executor.so
 Comment: 
 
-Filename: axion/factory.pyd
+Filename: axion/factory.so
 Comment: 
 
-Filename: axion/pipeline.pyd
+Filename: axion/pipeline.so
 Comment: 
 
-Filename: axion/queues.pyd
+Filename: axion/queues.so
 Comment: 
 
-Filename: axion/recorder.pyd
+Filename: axion/recorder.so
 Comment: 
 
-Filename: axion/scheduler.pyd
+Filename: axion/scheduler.so
 Comment: 
 
-Filename: axion/service.pyd
+Filename: axion/service.so
 Comment: 
 
-Filename: axion/thread.pyd
+Filename: axion/thread.so
 Comment: 
 
-Filename: axion/inst/__init__.pyd
+Filename: axion/inst/__init__.so
 Comment: 
 
-Filename: axion/inst/ibase.pyd
+Filename: axion/inst/ibase.so
 Comment: 
 
-Filename: axion/inst/nbase.pyd
+Filename: axion/inst/nbase.so
 Comment: 
 
-Filename: axion/inst/sbase.pyd
+Filename: axion/inst/sbase.so
 Comment: 
 
-Filename: axion/inst/tbase.pyd
+Filename: axion/inst/tbase.so
 Comment: 
 
-Filename: axion/inst/utility.pyd
+Filename: axion/inst/utility.so
 Comment: 
 
 Zip file comment:
```

