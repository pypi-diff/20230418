# Comparing `tmp/apkutils-1.3.0.tar.gz` & `tmp/apkutils-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkutils-1.3.0.tar", max compression
+gzip compressed data, was "apkutils-1.4.0.tar", max compression
```

## Comparing `apkutils-1.3.0.tar` & `apkutils-1.4.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
--rw-r--r--   0        0        0     1065 2022-05-31 07:54:58.000000 apkutils-1.3.0/LICENSE
--rw-r--r--   0        0        0       50 2023-04-11 08:51:48.957974 apkutils-1.3.0/apkutils/__init__.py
--rw-r--r--   0        0        0    21364 2023-04-11 08:42:08.633938 apkutils-1.3.0/apkutils/apk.py
--rw-r--r--   0        0        0    74509 2023-04-11 07:35:49.515179 apkutils-1.3.0/apkutils/apkfile.py
--rw-r--r--   0        0        0   109909 2023-04-11 08:50:18.990039 apkutils-1.3.0/apkutils/axml/__init__.py
--rw-r--r--   0        0        0     7039 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/axml/bytecode.py
--rw-r--r--   0        0        0     2115 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/axml/public.py
--rw-r--r--   0        0        0   191132 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/axml/public.xml
--rw-r--r--   0        0        0     2083 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/axml/types.py
--rw-r--r--   0        0        0      807 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/cert.py
--rw-r--r--   0        0        0     4209 2023-04-11 07:59:16.076423 apkutils-1.3.0/apkutils/cli.py
--rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/__init__.py
--rw-r--r--   0        0        0     2787 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/byteio.py
--rw-r--r--   0        0        0     7947 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/dalvik.py
--rw-r--r--   0        0        0     4237 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/dalvikformats.py
--rw-r--r--   0        0        0    12065 2022-07-13 08:37:53.000000 apkutils-1.3.0/apkutils/dex/dexparser.py
--rw-r--r--   0        0        0     1541 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/flags.py
--rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/__init__.py
--rw-r--r--   0        0        0     1703 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/arraytypes.py
--rw-r--r--   0        0        0     6678 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/constantpool.py
--rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/constants/__init__.py
--rw-r--r--   0        0        0     6062 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/constants/calc.py
--rw-r--r--   0        0        0     5657 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/constants/genlookup.py
--rw-r--r--   0        0        0  1800593 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/constants/lookup.py
--rw-r--r--   0        0        0      728 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/error.py
--rw-r--r--   0        0        0     2867 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/genmathops.py
--rw-r--r--   0        0        0     7859 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/ir.py
--rw-r--r--   0        0        0     3479 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/jvmops.py
--rw-r--r--   0        0        0     5689 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/mathops.py
--rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/optimization/__init__.py
--rw-r--r--   0        0        0     3059 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/optimization/consts.py
--rw-r--r--   0        0        0     3199 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/optimization/jumps.py
--rw-r--r--   0        0        0     1550 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/optimization/options.py
--rw-r--r--   0        0        0     8878 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/optimization/registers.py
--rw-r--r--   0        0        0     8891 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/optimization/stack.py
--rw-r--r--   0        0        0     1310 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/scalartypes.py
--rw-r--r--   0        0        0     4130 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/writebytecode.py
--rw-r--r--   0        0        0     4080 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/writeclass.py
--rw-r--r--   0        0        0    24612 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/jvm/writeir.py
--rw-r--r--   0        0        0     1767 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/mutf8.py
--rw-r--r--   0        0        0     4029 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/treelist.py
--rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/typeinference/__init__.py
--rw-r--r--   0        0        0    11171 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/typeinference/typeinference.py
--rw-r--r--   0        0        0     1158 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/dex/util.py
--rw-r--r--   0        0        0        0 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/elf/__init__.py
--rw-r--r--   0        0        0     6655 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/elf/elfparser.py
--rwxr-xr-x   0        0        0    69313 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/gdiff.py
--rw-r--r--   0        0        0    16570 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/intersection.py
--rw-r--r--   0        0        0     6155 2022-05-31 07:54:58.000000 apkutils-1.3.0/apkutils/wildcard.py
--rw-r--r--   0        0        0     1006 2023-04-11 07:57:06.813221 apkutils-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1191 1970-01-01 00:00:00.000000 apkutils-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-05-31 07:54:58.000000 apkutils-1.4.0/LICENSE
+-rw-r--r--   0        0        0       97 2023-04-18 08:30:43.959470 apkutils-1.4.0/apkutils/__init__.py
+-rw-r--r--   0        0        0       90 2023-04-18 08:30:40.360003 apkutils-1.4.0/apkutils/__main__.py
+-rw-r--r--   0        0        0    21370 2023-04-18 03:31:17.215836 apkutils-1.4.0/apkutils/apk.py
+-rw-r--r--   0        0        0    74581 2023-04-17 03:31:03.047483 apkutils-1.4.0/apkutils/apkfile.py
+-rw-r--r--   0        0        0   111058 2023-04-18 08:21:26.441141 apkutils-1.4.0/apkutils/axml/__init__.py
+-rw-r--r--   0        0        0     7039 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/axml/bytecode.py
+-rw-r--r--   0        0        0     2115 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/axml/public.py
+-rw-r--r--   0        0        0   191132 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/axml/public.xml
+-rw-r--r--   0        0        0        0 2023-04-17 04:21:15.167233 apkutils-1.4.0/apkutils/axml/types.py
+-rw-r--r--   0        0        0      807 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/cert.py
+-rw-r--r--   0        0        0     4209 2023-04-11 07:59:16.076423 apkutils-1.4.0/apkutils/cli.py
+-rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/__init__.py
+-rw-r--r--   0        0        0     2787 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/byteio.py
+-rw-r--r--   0        0        0     7947 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/dalvik.py
+-rw-r--r--   0        0        0     4237 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/dalvikformats.py
+-rw-r--r--   0        0        0    12065 2022-07-13 08:37:53.000000 apkutils-1.4.0/apkutils/dex/dexparser.py
+-rw-r--r--   0        0        0     1541 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/flags.py
+-rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/__init__.py
+-rw-r--r--   0        0        0     1703 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/arraytypes.py
+-rw-r--r--   0        0        0     6678 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/constantpool.py
+-rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/constants/__init__.py
+-rw-r--r--   0        0        0     6062 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/constants/calc.py
+-rw-r--r--   0        0        0     5657 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/constants/genlookup.py
+-rw-r--r--   0        0        0  1800593 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/constants/lookup.py
+-rw-r--r--   0        0        0      728 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/error.py
+-rw-r--r--   0        0        0     2867 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/genmathops.py
+-rw-r--r--   0        0        0     7859 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/ir.py
+-rw-r--r--   0        0        0     3479 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/jvmops.py
+-rw-r--r--   0        0        0     5689 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/mathops.py
+-rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/optimization/__init__.py
+-rw-r--r--   0        0        0     3059 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/optimization/consts.py
+-rw-r--r--   0        0        0     3199 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/optimization/jumps.py
+-rw-r--r--   0        0        0     1550 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/optimization/options.py
+-rw-r--r--   0        0        0     8878 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/optimization/registers.py
+-rw-r--r--   0        0        0     8891 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/optimization/stack.py
+-rw-r--r--   0        0        0     1310 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/scalartypes.py
+-rw-r--r--   0        0        0     4130 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/writebytecode.py
+-rw-r--r--   0        0        0     4080 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/writeclass.py
+-rw-r--r--   0        0        0    24612 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/jvm/writeir.py
+-rw-r--r--   0        0        0     1767 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/mutf8.py
+-rw-r--r--   0        0        0     4029 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/treelist.py
+-rw-r--r--   0        0        0      596 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/typeinference/__init__.py
+-rw-r--r--   0        0        0    11171 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/typeinference/typeinference.py
+-rw-r--r--   0        0        0     1158 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/dex/util.py
+-rw-r--r--   0        0        0        0 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/elf/__init__.py
+-rw-r--r--   0        0        0     6655 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/elf/elfparser.py
+-rwxr-xr-x   0        0        0    69313 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/gdiff.py
+-rw-r--r--   0        0        0    16570 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/intersection.py
+-rw-r--r--   0        0        0     6155 2022-05-31 07:54:58.000000 apkutils-1.4.0/apkutils/wildcard.py
+-rw-r--r--   0        0        0     1006 2023-04-18 08:28:56.450458 apkutils-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1191 1970-01-01 00:00:00.000000 apkutils-1.4.0/PKG-INFO
```

### Comparing `apkutils-1.3.0/LICENSE` & `apkutils-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/apk.py` & `apkutils-1.4.0/apkutils/apk.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,20 +78,18 @@
     
     def parse_dex(self):
         self._init_dex_strings()
         return self
     
     def parse_arsc(self):
         self._init_arsc()
-        return self
-    
-    def parse_app_icons(self):
         self._init_app_icons()
+        self._init_app_name()
         return self
-
+    
     def __enter__(self):
         return self
 
     def __exit__(self, *args, **kwargs):
         self.close()
 
     def close(self):
@@ -113,28 +111,28 @@
                         return
                     buff = etree.tostring(
                         self.axml, pretty_print=True, encoding="utf-8"
                     )
                     if buff is None:
                         return
                     self.manifest = buff.decode("UTF-8")
-                except:
+                except Exception:
                     traceback.print_exc()
                     return
-        except:
+        except Exception:
             traceback.print_exc()
             return
 
         # fix manifest
         self.manifest = re.sub(
             r'\s:(="[\w]*?\.[\.\w]*")', r" android:name\1", self.manifest
         )
 
         soup = BeautifulSoup(self.manifest, "lxml-xml")
-        self._package_name = soup.manifest["package"]
+        self._package_name = soup.manifest.get("package", "")
         self._version_code = soup.manifest.get("android:versionCode")
         self._version_name = soup.manifest.get("android:versionName")
 
         uses_sdk = soup.select_one("uses-sdk")
         if uses_sdk is None:
             uses_sdk = {}
         self._min_sdk_version = uses_sdk.get("android:minSdkVersion", 1)
```

### Comparing `apkutils-1.3.0/apkutils/apkfile.py` & `apkutils-1.4.0/apkutils/apkfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1441,26 +1441,28 @@
         arcname = os.path.sep.join(
             x for x in arcname.split(os.path.sep) if x not in invalid_path_parts
         )
         if os.path.sep == "\\":
             # filter illegal characters on Windows
             arcname = self._sanitize_windows_name(arcname, os.path.sep)
 
-        # NOTE 文件名超过255无法写入
+        # NOTE 文件名和目录名超过255无法写入
         arr = arcname.split(os.path.sep)
-        name = arr[-1]
-        if len(name) > 255:
-            extension = os.path.splitext(name)[1]
-            name = "too_long_" + str(crc32(name.encode("utf-8"))) + extension
-            arr = arr[:-1]
-            print("{} 存在超过255个字符的文件名，跳过解压。".format(os.path.sep.join(arr)))
+        # name = arr[-1]
+        for item in arr:
+            # FIXME 对于文件名过长的文件，无法解压，暂时跳过
+            if len(item) > 255:
+                print("{} 文件名太长，跳过解压。".format(os.path.sep.join(arr)))
+                return
+        # if len(name) > 255:
+            # extension = os.path.splitext(name)[1]
+            # name = "too_long_" + str(crc32(name.encode("utf-8"))) + extension
+            # arr = arr[:-1]
             # arr.append(name)
             # arcname = os.path.sep.join(arr)
-            # FIXME 对于该类文件名暂时无法解压，暂时跳过
-            return
 
         targetpath = os.path.join(targetpath, arcname)
         targetpath = os.path.normpath(targetpath)
         
         # Create all upper directories if necessary.
         upperdirs = os.path.dirname(targetpath)
         if upperdirs and not os.path.exists(upperdirs):
```

### Comparing `apkutils-1.3.0/apkutils/axml/__init__.py` & `apkutils-1.4.0/apkutils/axml/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,143 @@
-# Copy from https://github.com/kin9-0rz/androguard/blob/master/androguard/core/bytecodes/axml/__init__.py
-
 import binascii
 import collections
 import logging
 import re
-import sys
 from collections import defaultdict
 from struct import pack, unpack
 from xml.sax.saxutils import escape
 
 from lxml import etree
 
 from apkutils.axml import bytecode, public
-from apkutils.axml.types import *
 
 log = logging.getLogger("axml")
 
 
-# Constants for ARSC Files
-# see http://androidxref.com/9.0.0_r3/xref/frameworks/base/libs/androidfw/include/androidfw/ResourceTypes.h#215
+# --------------------------------- AXML格式说明 --------------------------------- #
+
+# 看看这个图 https://cloud.tencent.com/developer/article/1870329
+# 整体分为4大部分
+# magic 4bytes 0x03
+    # chunk type 0x03
+    # header size 0x8=0x4*2
+# 文件大小 4bytes
+
+# String Chunk
+# ResourceID Chunk
+# XmlConContent Chunk
+
+#!SECTION String Chunk
+# magic 4bytes 0x001C0001，
+    # chunk type 0x1
+    # header size 0x1C=4*7
+# chunk size 4bytes
+# StringCount 字符串数量 4bytes，这个值未必是对的。
+# Style数量 4bytes
+# flag 4bytes
+# string pool offset 4bytes，这个值？
+# style pool offset 4bytes - header end
+
+# StringOffsets StringCount * 4bytes
+# StypeOffsets  StyleCount * 4bytes
+# String Pool
+# Style Pool
+
+#!SECTION ResourceID Chunk
+# magic 4bytes 0x00080180
+    # chunk type 0x180
+    # header size 0x8
+# chunk size 4bytes
+# NOTE 这个计算不好说
+# resourceIDs (chunk_size/4-2)*4
+
+#!SECTION Xml Content Chunk
+# magic 4bytes 0x0010 0104
+    # chunk type 0x104
+    # header size 0x10
+# chunk size 4bytes
+# line number 4bytes
+# 未知flag 4bytes
+
+# name 4bytes
+# 未知 4bytes
+# 未知 4bytes
+
+#!SECTION Start Tag Chunk
+# magic 4bytes 0x0010 0102
+    # chunk type 0x102
+    # header size 0x10
+# chunk size 4bytes
+# line number 4bytes
+# 未知flag 4bytes
+
+# namespace uri 4bytes
+# name 4bytes
+# flags 4bytes 0x0014 0014 
+# attribute count 4bytes
+# class count 4bytes
+# TODO 这个计算方式是？
+# attributes  attribute_count * 5 * 4bytes
+
+# ---------------------------------------------------------------------------- #
+
+# ------------------------------- ResourceTypes ------------------------------ #
+# See http://androidxref.com/9.0.0_r3/xref/frameworks/base/libs/androidfw/include/androidfw/ResourceTypes.h#258
+# 资源块中值的类型
+TYPE_NULL = 0x00 # 数据只有0或1
+# The 'data' holds a ResTable_ref, a reference to another resource table entry.
+TYPE_REFERENCE = 0x01
+# The 'data' holds an attribute resource identifier.
+TYPE_ATTRIBUTE = 0x02
+# “data”保存了包含资源表的全局值字符串池的索引。
+TYPE_STRING = 0x03
+# The 'data' holds a single-precision floating point number.
+TYPE_FLOAT = 0x04
+# The 'data' holds a complex number encoding a dimension value
+# such as "100in".
+TYPE_DIMENSION = 0x05
+# The 'data' holds a complex number encoding a fraction of a
+# container.
+TYPE_FRACTION = 0x06
+# The 'data' holds a dynamic ResTable_ref, which needs to be
+# resolved before it can be used like a TYPE_REFERENCE.
+TYPE_DYNAMIC_REFERENCE = 0x07
+# The 'data' holds an attribute resource identifier, which needs to be resolved
+# before it can be used like a TYPE_ATTRIBUTE.
+TYPE_DYNAMIC_ATTRIBUTE = 0x08
+# Beginning of integer flavors...
+TYPE_FIRST_INT = 0x10
+# The 'data' is a raw integer value of the form n..n.
+TYPE_INT_DEC = 0x10
+# The 'data' is a raw integer value of the form 0xn..n.
+TYPE_INT_HEX = 0x11
+# The 'data' is either 0 or 1, for input "false" or "true" respectively.
+TYPE_INT_BOOLEAN = 0x12
+# Beginning of color integer flavors...
+TYPE_FIRST_COLOR_INT = 0x1c
+# The 'data' is a raw integer value of the form #aarrggbb.
+TYPE_INT_COLOR_ARGB8 = 0x1c
+# The 'data' is a raw integer value of the form #rrggbb.
+TYPE_INT_COLOR_RGB8 = 0x1d
+# The 'data' is a raw integer value of the form #argb.
+TYPE_INT_COLOR_ARGB4 = 0x1e
+# The 'data' is a raw integer value of the form #rgb.
+TYPE_INT_COLOR_RGB4 = 0x1f
+# ...end of integer flavors.
+TYPE_LAST_COLOR_INT = 0x1f
+# ...end of integer flavors.
+TYPE_LAST_INT = 0x1f
+
+# ------------------------- 头部格式定义 ------------------------- #
+# http://androidxref.com/9.0.0_r3/xref/frameworks/base/libs/androidfw/include/androidfw/ResourceTypes.h#193
+# ---------------------------------------------------------------------------- #
 RES_NULL_TYPE = 0x0000
 RES_STRING_POOL_TYPE = 0x0001
 RES_TABLE_TYPE = 0x0002
+
 RES_XML_TYPE = 0x0003
 
 RES_XML_FIRST_CHUNK_TYPE = 0x0100
 RES_XML_START_NAMESPACE_TYPE = 0x0100
 RES_XML_END_NAMESPACE_TYPE = 0x0101
 RES_XML_START_ELEMENT_TYPE = 0x0102
 RES_XML_END_ELEMENT_TYPE = 0x0103
@@ -45,22 +157,15 @@
 
 # Position of the fields inside an attribute
 ATTRIBUTE_IX_NAMESPACE_URI = 0
 ATTRIBUTE_IX_NAME = 1
 ATTRIBUTE_IX_VALUE_STRING = 2
 ATTRIBUTE_IX_VALUE_TYPE = 3
 ATTRIBUTE_IX_VALUE_DATA = 4
-ATTRIBUTE_LENGHT = 5
-
-# Internally used state variables for AXMLParser
-START_DOCUMENT = 0
-END_DOCUMENT = 1
-START_TAG = 2
-END_TAG = 3
-TEXT = 4
+ATTRIBUTE_LENGHT = 5 # 5个字节
 
 # Table used to lookup functions to determine the value representation in ARSCParser
 TYPE_TABLE = {
     TYPE_ATTRIBUTE: "attribute",
     TYPE_DIMENSION: "dimension",
     TYPE_FLOAT: "float",
     TYPE_FRACTION: "fraction",
@@ -91,14 +196,18 @@
 
 def complexToFloat(xcomplex):
     """
     Convert a complex unit into float
     """
     return float(xcomplex & 0xFFFFFF00) * RADIX_MULTS[(xcomplex >> 4) & 3]
 
+def print_nrange(alist:list, n: int):
+    for b in [alist[i:i + n] for i in range(0, len(alist), n)]:
+        print(b)
+
 
 class StringBlock:
     """
     StringBlock is a CHUNK inside an AXML File: `ResStringPool_header`
     It contains all strings, which are used by referecing to ID's
 
     See http://androidxref.com/9.0.0_r3/xref/frameworks/base/libs/androidfw/include/androidfw/ResourceTypes.h#436
@@ -155,22 +264,23 @@
             
             # NOTE stringCount 有可能是伪造的
             # 正常情况下，stringCount + 8，就是buff当前的位置
             if self.stringsOffset + 8 == buff.get_idx():
                 self.stringCount = i
                 buff.set_idx(buff.get_idx())
                 break
-
+        
         # And a list of styles
         # again, a list of offsets
         for i in range(self.styleCount):
             self.m_styleOffsets.append(unpack("<I", buff.read(4))[0])
 
         size = self.header.size - self.stringsOffset
 
+
         # if there are styles as well, we do not want to read them too.
         # Only read them, if no
         if self.stylesOffset != 0 and self.styleCount != 0:
             size = self.stylesOffset - self.stringsOffset
 
         if (size % 4) != 0:
             log.warning("Size of strings is not aligned by four bytes.")
@@ -182,16 +292,14 @@
 
             if (size % 4) != 0:
                 log.warning("Size of styles is not aligned by four bytes.")
 
             for i in range(0, size // 4):
                 self.m_styles.append(unpack("<I", buff.read(4))[0])
         
-        # self.show()
-        
     def __repr__(self):
         return "<StringPool #strings={}, #styles={}, UTF8={}>".format(
             self.stringCount, self.styleCount, self.m_isUTF8
         )
 
     def __getitem__(self, idx):
         """
@@ -388,14 +496,21 @@
         if self.styleCount > 0:
             print()
             print("Styles Table: ")
             for i in range(self.styleCount):
                 print("{:08d} {}".format(i, repr(self.getStyle(i))))
 
 
+# AXMLParser 专用事件
+START_DOCUMENT = 0
+END_DOCUMENT = 1
+START_TAG = 2
+END_TAG = 3
+TEXT = 4
+
 class AXMLParser:
     """
     AXMLParser reads through all chunks in the AXML file
     and implements a state machine to return information about
     the current chunk, which can then be read by :class:`~AXMLPrinter`.
 
     An AXML file is a file which contains multiple chunks of data, defined
@@ -419,108 +534,68 @@
     def __init__(self, raw_buff, is_android_manifest=False):
         self._reset()
 
         self._valid = True
         self.axml_tampered = False
         self.buff = bytecode.BuffHandle(raw_buff)
         
-        # Minimum is a single ARSCHeader, which would be a strange edge case...
         if self.buff.size() < 8:
-            log.error(
-                "Filesize is too small to be a valid AXML file! Filesize: {}".format(
-                    self.buff.size()
-                )
-            )
             self._valid = False
             return
 
-        # This would be even stranger, if an AXML file is larger than 4GB...
-        # But this is not possible as the maximum chunk size is a unsigned 4 byte int.
         if self.buff.size() > 0xFFFFFFFF:
-            log.error(
-                "Filesize is too large to be a valid AXML file! Filesize: {}".format(
-                    self.buff.size()
-                )
-            )
             self._valid = False
             return
 
+        # 解析AXML头，4个字节是类型，4个字节是文件大小
         try:
             axml_header = ARSCHeader(self.buff)
         except ResParserError as e:
             log.error("Error parsing first resource header: %s", e)
             self._valid = False
             return
 
         self.filesize = axml_header.size
 
-        if axml_header.header_size == 28024:
-            # Can be a common error: the file is not an AXML but a plain XML
-            # The file will then usually start with '<?xm' / '3C 3F 78 6D'
-            log.warning(
-                "Header size is 28024! Are you trying to parse a plain XML file?"
-            )
-
         if axml_header.header_size != 8:
-            log.error(
-                "This does not look like an AXML file. header size does not equal 8! header size = {}".format(
-                    axml_header.header_size
-                )
-            )
             self._valid = False
             return
 
         if self.filesize > self.buff.size():
-            log.error(
-                "This does not look like an AXML file. Declared filesize does not match real size: {} vs {}".format(
-                    self.filesize, self.buff.size()
-                )
-            )
             self._valid = False
             return
 
         if self.filesize < self.buff.size():
-            # The file can still be parsed up to the point where the chunk should end.
             self.axml_tampered = True
-            log.warning(
-                "Declared filesize ({}) is smaller than total file size ({}). "
-                "Was something appended to the file? Trying to parse it anyways.".format(
-                    self.filesize, self.buff.size()
-                )
-            )
 
         # NOTE 判断是否是AXML文件，没啥用
         if axml_header.type != RES_XML_TYPE:
             self.axml_tampered = True
 
-        # Now we parse the STRING POOL
+        # 解析下一个头 - String Pool Chunk
         try:
             header = ARSCHeader(self.buff, expected_type=RES_STRING_POOL_TYPE)
         except ResParserError as e:
             log.error("Error parsing resource header of string pool: %s", e)
             self._valid = False
             return
 
         if header.header_size != 0x1C:
-            log.error(
-                "This does not look like an AXML file. String chunk header size does not equal 28! header size = {}".format(
-                    header.header_size
-                )
-            )
             self._valid = False
             return
 
         self.sb = StringBlock(self.buff, header, is_android_manifest)
         
         # Stores resource ID mappings, if any
         self.m_resourceIDs = []
 
         # Store a list of prefix/uri mappings encountered
         self.namespaces = []
 
+
     def is_valid(self):
         """
         Get the state of the AXMLPrinter.
         if an error happend somewhere in the process of parsing the file,
         this flag is set to False.
         """
         return self._valid
@@ -554,18 +629,16 @@
             try:
                 h = ARSCHeader(self.buff)
             except ResParserError as e:
                 log.error("Error parsing resource header: %s", e)
                 self._valid = False
                 return
 
-            # Special chunk: Resource Map. This chunk might be contained inside
-            # the file, after the string pool.
+            # Special chunk: Resource Map. 
             if h.type == RES_XML_RESOURCE_MAP_TYPE:
-                log.debug("AXML contains a RESOURCE MAP")
                 # Check size: < 8 bytes mean that the chunk is not complete
                 # Should be aligned to 4 bytes.
                 if h.size < 8 or (h.size % 4) != 0:
                     log.error("Invalid chunk size in chunk XML_RESOURCE_MAP")
                     self._valid = False
                     return
 
@@ -642,15 +715,14 @@
                 self.namespaces.append((prefix, uri))
 
                 # We can continue with the next chunk, as we store the namespace
                 # mappings for each tag
                 continue
 
             if h.type == RES_XML_END_NAMESPACE_TYPE:
-                # END_PREFIX contains again prefix and uri field
                 (prefix,) = unpack("<L", self.buff.read(4))
                 (uri,) = unpack("<L", self.buff.read(4))
 
                 # We remove the last namespace mapping matching
                 if (prefix, uri) in self.namespaces:
                     self.namespaces.remove((prefix, uri))
                 else:
@@ -661,45 +733,61 @@
 
                 # We can continue with the next chunk, as we store the namespace
                 # mappings for each tag
                 continue
 
             # START_TAG is the start of a new tag.
             if h.type == RES_XML_START_ELEMENT_TYPE:
-                # The TAG consists of some fields:
                 # * (chunk_size, line_number, comment_index - we read before)
                 # * namespace_uri
                 # * name
                 # * flags
                 # * attribute_count
                 # * class_attribute
-                # After that, there are two lists of attributes, 20 bytes each
-
                 # Namespace URI (String ID)
                 (self.m_namespaceUri,) = unpack("<L", self.buff.read(4))
                 # Name of the Tag (String ID)
                 (self.m_name,) = unpack("<L", self.buff.read(4))
+
+                # 属性结构体的开始偏移量
+                (attributeStart,) = unpack("<H", self.buff.read(2))
+                # 属性结构体的大小
+                (attributeSize,) = unpack("<H", self.buff.read(2))
+
+                (attributeCount,) = unpack("<H", self.buff.read(2))
+                (idIndex,) = unpack("<H", self.buff.read(2))
+                (classIndex,) = unpack("<H", self.buff.read(2))
+                (styleIndex,) = unpack("<H", self.buff.read(2))
                 
-                # NOTE : Flags skip
-                _ = self.buff.read(4)
-                # Attribute Count
-                (attributeCount,) = unpack("<L", self.buff.read(4))
-                # Class Attribute
-                (self.m_classAttribute,) = unpack("<L", self.buff.read(4))
-
-                self.m_idAttribute = (attributeCount >> 16) - 1
-                self.m_attribute_count = attributeCount & 0xFFFF
-                self.m_styleAttribute = (self.m_classAttribute >> 16) - 1
-                self.m_classAttribute = (self.m_classAttribute & 0xFFFF) - 1
-
-                # Now, we parse the attributes.
-                # Each attribute has 5 fields of 4 byte
-                for i in range(0, self.m_attribute_count * ATTRIBUTE_LENGHT):
-                    # Each field is linearly parsed into the array
-                    # Each Attribute contains:
+                self.m_attribute_count = attributeCount
+                self.m_idAttribute = idIndex
+                self.m_classAttribute = classIndex
+                self.m_styleAttribute = styleIndex
+
+                # 结构体的字节数
+                nbytes = int(attributeSize/4) # 一次读4个字节
+                # 一次nop的数量，至少要4个字节，一次可以nop 4*n个字节。
+                nop_num = attributeSize - 20
+                skip_n = int(nop_num/4)
+                max_n = 5+skip_n
+
+                counter = 0
+                for i in range(0, (self.m_attribute_count * nbytes)):  # noqa: E501
+                    counter += 1
+                    # ! nop_num > 0 是必须的，针对没有nop的情况。
+                    if nop_num>0 and counter == max_n:
+                        self.buff.read(nop_num)
+                        counter = 0
+                        continue
+
+                    if nop_num > 0 and counter >= 6:
+                        self.buff.read(nop_num)
+                        continue
+
+                    # 属性结构默认是20，但是，可以根据 attributeSize 填充其他数据。
                     # * Namespace URI (String ID)
                     # * Name (String ID)
                     # * Value
                     # * Type
                     # * Data
                     self.m_attributes.append(unpack("<L", self.buff.read(4))[0])
 
@@ -711,46 +799,35 @@
 
                 self.m_event = START_TAG
                 break
 
             if h.type == RES_XML_END_ELEMENT_TYPE:
                 (self.m_namespaceUri,) = unpack("<L", self.buff.read(4))
                 (self.m_name,) = unpack("<L", self.buff.read(4))
-
                 self.m_event = END_TAG
                 break
 
             if h.type == RES_XML_CDATA_TYPE:
                 # The CDATA field is like an attribute.
                 # It contains an index into the String pool
                 # as well as a typed value.
                 # usually, this typed value is set to UNDEFINED
 
                 # ResStringPool_ref data --> uint32_t index
                 (self.m_name,) = unpack("<L", self.buff.read(4))
-
                 # Res_value typedData:
                 # uint16_t size
                 # uint8_t res0 -> always zero
                 # uint8_t dataType
                 # uint32_t data
                 # For now, we ingore these values
                 size, res0, dataType, data = unpack("<HBBL", self.buff.read(8))
-
-                log.debug(
-                    "found a CDATA Chunk: "
-                    "index={: 6d}, size={: 4d}, res0={: 4d}, dataType={: 4d}, data={: 4d}".format(
-                        self.m_name, size, res0, dataType, data
-                    )
-                )
-
                 self.m_event = TEXT
                 break
 
-            # Still here? Looks like we read an unknown XML header, try to skip it...
             log.warning(
                 "Unknown XML Chunk: 0x{:04x}, skipping {} bytes.".format(h.type, h.size)
             )
             self.buff.set_idx(h.end)
 
     @property
     def name(self):
@@ -888,21 +965,21 @@
         if uri == 0xFFFFFFFF:
             return ""
 
         return self.sb[uri]
 
     def getAttributeName(self, index):
         """
-        Returns the String which represents the attribute name
+        获取属性名
         """
         offset = self._get_attribute_offset(index)
         name = self.m_attributes[offset + ATTRIBUTE_IX_NAME]
-
         res = self.sb[name]
-        # If the result is a (null) string, we need to look it up.
+        # 如果能够从字符串池中获取到属性名，那么直接返回。
+
         if not res or res == ":":
             attr = self.m_resourceIDs[name]
             if attr in public.SYSTEM_RESOURCES["attributes"]["inverse"]:
                 res = (
                     "android:" + public.SYSTEM_RESOURCES["attributes"]["inverse"][attr]
                 )
             else:
@@ -957,18 +1034,20 @@
     :param _type: The numeric type of the value
     :param _data: The numeric data of the value
     :param lookup_string: A function how to resolve strings from integer IDs
     """
 
     # Function to prepend android prefix for attributes/references from the
     # android library
-    fmt_package = lambda x: "android:" if x >> 24 == 1 else ""
+    def fmt_package(x):
+        return "android:" if x >> 24 == 1 else ""
 
     # Function to represent integers
-    fmt_int = lambda x: (0x7FFFFFFF & x) - 0x80000000 if x > 0x7FFFFFFF else x
+    def fmt_int(x):
+        return (2147483647 & x) - 2147483648 if x > 2147483647 else x
 
     if _type == TYPE_STRING:
         return lookup_string(_data)
 
     elif _type == TYPE_ATTRIBUTE:
         return "?{}{:08X}".format(fmt_package(_data), _data)
 
@@ -1021,44 +1100,37 @@
 
         self.root = None
         self.packerwarning = False
         cur = []
 
         while self.axml.is_valid():
             _type = next(self.axml)
-
             if _type == START_TAG:
                 uri = self._print_namespace(self.axml.namespace)
                 uri, name = self._fix_name(uri, self.axml.name)
                 tag = "{}{}".format(uri, name)
 
                 comment = self.axml.comment
                 if comment:
                     if self.root is None:
                         log.warning(
-                            "Can not attach comment with content '{}' without root!".format(
+                            "Can not attach comment with content '{}' without root!".format(  # noqa: E501
                                 comment
                             )
                         )
                     else:
                         cur[-1].append(etree.Comment(comment))
 
-                log.debug("START_TAG: {} (line={})".format(tag, self.axml.m_lineNumber))
                 elem = etree.Element(tag, nsmap=self.axml.nsmap)
-
                 for i in range(self.axml.getAttributeCount()):
                     uri = self._print_namespace(self.axml.getAttributeNamespace(i))
-                    uri, name = self._fix_name(uri, self.axml.getAttributeName(i))
+                    attribute_name = self.axml.getAttributeName(i)
+                    uri, name = self._fix_name(uri, attribute_name)
                     value = self._fix_value(self._get_attribute_value(i))
 
-                    log.debug(
-                        "found an attribute: {}{}='{}'".format(
-                            uri, name, value.encode("utf-8")
-                        )
-                    )
                     if "{}{}".format(uri, name) in elem.attrib:
                         log.warning(
                             "Duplicate attribute '{}{}'! Will overwrite!".format(
                                 uri, name
                             )
                         )
                     elem.set("{}{}".format(uri, name), value)
@@ -1212,15 +1284,15 @@
                 )
                 prefix = self._print_namespace(self.axml.nsmap[embedded_prefix])
                 name = new_name
             else:
                 # Print out an extra warning
                 log.warning(
                     "Confused: name contains a unknown namespace prefix: '{}'. "
-                    "This is either a broken AXML file or some attempt to break stuff.".format(
+                    "This is either a broken AXML file or some attempt to break stuff.".format(  # noqa: E501
                         name
                     )
                 )
         if not re.match(r"^[a-zA-Z0-9._-]*$", name):
             log.warning("Name '{}' contains invalid characters!".format(name))
             self.packerwarning = True
             name = re.sub(r"[^a-zA-Z0-9._-]", "_", name)
@@ -1416,15 +1488,15 @@
         )
 
         # skip to the start of the first chunk's data, skipping trailing header bytes (there should be none)
         self.buff.set_idx(self.header.start + self.header.header_size)
 
         # Now parse the data:
         # We should find one ResStringPool_header and one or more ResTable_package chunks inside
-        while self.buff.get_idx() <= self.header.end - ARSCHeader.SIZE:
+        while self.buff.get_idx() <= self.header.end - ARSCHeader.HEADER_SIZE:
             res_header = ARSCHeader(self.buff)
 
             if res_header.end > self.header.end:
                 # this inner chunk crosses the boundary of the table chunk
                 log.warning(
                     "Invalid chunk found! It is larger than the outer chunk: %s",
                     res_header,
@@ -1480,16 +1552,16 @@
                 )
                 log.debug("Constructed a PackageContext: %s", pc)
 
                 # skip to the first header in this table package chunk
                 # FIXME is this correct? We have already read the first two sections!
                 # self.buff.set_idx(res_header.start + res_header.header_size)
                 # this looks more like we want: (???)
-                # FIXME it looks like that the two string pools we have read might not be concatenated to each other,
-                # thus jumping to the sum of the sizes might not be correct...
+                # FIXME 
+                # 看起来我们读到的两个字符串池可能不会相互连接，因此跳转到大小的和可能是不正确的…
                 next_idx = (
                     res_header.start
                     + res_header.header_size
                     + type_sp_header.size
                     + key_sp_header.size
                 )
 
@@ -1508,15 +1580,15 @@
                         "Please open a issue at https://github.com/androguard/androguard/issues"
                     )
                     log.error("Thank you!")
 
                 self.buff.set_idx(next_idx)
 
                 # Read all other headers
-                while self.buff.get_idx() <= res_header.end - ARSCHeader.SIZE:
+                while self.buff.get_idx() <= res_header.end - ARSCHeader.HEADER_SIZE:
                     pkg_chunk_header = ARSCHeader(self.buff)
                     log.debug("Found a header: {}".format(pkg_chunk_header))
                     if pkg_chunk_header.start + pkg_chunk_header.size > res_header.end:
                         # we are way off the package chunk; bail out
                         break
 
                     self.packages[package_name].append(pkg_chunk_header)
@@ -2312,65 +2384,60 @@
             self.mTableStrings,
             self.mKeyStrings,
         )
 
 
 class ARSCHeader:
     """
-    Object which contains a Resource Chunk.
-    This is an implementation of the `ResChunk_header`.
+    通常是 
+    magic   03 00 08 00
+    文件大小 FF FF FF FF 
 
-    It will throw an :class:`ResParserError` if the header could not be read successfully.
+    这个头结构是通用的，适合里面所有的结构。
 
-    It is not checked if the data is outside the buffer size nor if the current
-    chunk fits into the parent chunk (if any)!
-
-    The parameter `expected_type` can be used to immediately check the header for the type or raise a :class:`ResParserError`.
-    This is useful if you know what type of chunk must follow.
 
     See http://androidxref.com/9.0.0_r3/xref/frameworks/base/libs/androidfw/include/androidfw/ResourceTypes.h#196
     :raises: ResParserError
     """
-
-    # This is the minimal size such a header must have. There might be other header data too!
-    SIZE = 2 + 2 + 4
+    HEADER_SIZE = 2 + 2 + 4
 
     def __init__(self, buff, expected_type=None):
         """
         :param androguard.core.bytecode.BuffHandle buff: the buffer set to the position where the header starts.
         :param int expected_type: the type of the header which is expected.
         """
         self.start = buff.get_idx()
         # Make sure we do not read over the buffer:
-        if buff.size() < self.start + self.SIZE:
+        if buff.size() < self.start + self.HEADER_SIZE:
             raise ResParserError(
                 "Can not read over the buffer size! Offset={}".format(self.start)
             )
 
-        self._type, self._header_size, self._size = unpack("<HHL", buff.read(self.SIZE))
+        self._type, self._header_size, self._size = unpack("<HHL", buff.read(self.HEADER_SIZE))
 
         if expected_type and self._type != expected_type:
             raise ResParserError(
                 "Header type is not equal the expected type: Got 0x{:04x}, wanted 0x{:04x}".format(
                     self._type, expected_type
                 )
             )
 
         # Assert that the read data will fit into the chunk.
         # The total size must be equal or larger than the header size
-        if self._header_size < self.SIZE:
+        if self._header_size < self.HEADER_SIZE:
             raise ResParserError(
                 "declared header size is smaller than required size of {}! Offset={}".format(
-                    self.SIZE, self.start
+                    self.HEADER_SIZE, self.start
                 )
             )
-        if self._size < self.SIZE:
+        
+        if self._size < self.HEADER_SIZE:
             raise ResParserError(
                 "declared chunk size is smaller than required size of {}! Offset={}".format(
-                    self.SIZE, self.start
+                    self.HEADER_SIZE, self.start
                 )
             )
         if self._size < self._header_size:
             raise ResParserError(
                 "declared chunk size ({}) is smaller than header size ({})! Offset={}".format(
                     self._size, self._header_size, self.start
                 )
@@ -2427,15 +2494,16 @@
     """
 
     def __init__(self, buff, header):
         self.header = header
         self.start = buff.get_idx()
         self.id = unpack("<I", buff.read(4))[0]
         # 128 times 16bit -> read 256 bytes
-        # TODO why not read a null terminated string in buffer (like the meth name suggests) instead of parsing it later in get_name()?
+        # TODO why not read a null terminated string in buffer 
+        # (like the meth name suggests) instead of parsing it later in get_name()?
         self.name = buff.readNullString(256)
         self.typeStrings = unpack("<I", buff.read(4))[0]
         self.lastPublicType = unpack("<I", buff.read(4))[0]
         self.keyStrings = unpack("<I", buff.read(4))[0]
         self.lastPublicKey = unpack("<I", buff.read(4))[0]
         self.mResId = self.id << 24
 
@@ -2498,15 +2566,16 @@
     def get_type(self):
         return self.parent.mTableStrings.getString(self.id - 1)
 
     def get_package_name(self):
         return self.parent.get_package_name()
 
     def __repr__(self):
-        return "<ARSCResType(start=0x%x, id=0x%x, flags=0x%x, entryCount=%d, entriesStart=0x%x, mResId=0x%x, %s)>" % (
+        return ("<ARSCResType(start=0x%x, id=0x%x, flags=0x%x, ",
+                "entryCount=%d, entriesStart=0x%x, mResId=0x%x, %s)>") % (
             self.start,
             self.id,
             self.flags,
             self.entryCount,
             self.entriesStart,
             self.mResId,
             "table:" + self.parent.mTableStrings.getString(self.id - 1),
@@ -2561,15 +2630,15 @@
             # struct of
             # uint16_t screenWidth
             # uint16_t screenHeight
             self.screenSize = unpack("<I", buff.read(4))[0]
 
             # struct of
             # uint16_t sdkVersion
-            # uint16_t minorVersion  which should be always 0, as the meaning is not defined
+            # uint16_t minorVersion，它应该总是0，因为含义没有定义
             self.version = unpack("<I", buff.read(4))[0]
 
             # The next three fields seems to be optional
             if self.size >= 32:
                 # struct of
                 # uint8_t screenLayout
                 # uint8_t uiMode
@@ -3016,15 +3085,15 @@
             TYPE_TABLE.get(self.data_type, "0x%x" % self.data_type),
             self.data,
         )
 
 
 def get_arsc_info(arscobj):
     """
-    Return a string containing all resources packages ordered by packagename, locale and type.
+    返回一个字符串，包含按包名、地区和类型排序的所有资源包。
 
     :param arscobj: :class:`~ARSCParser`
     :return: a string
     """
     buff = ""
     for package in arscobj.get_packages_names():
         buff += package + ":\n"
```

### Comparing `apkutils-1.3.0/apkutils/axml/bytecode.py` & `apkutils-1.4.0/apkutils/axml/bytecode.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/axml/public.py` & `apkutils-1.4.0/apkutils/axml/public.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/axml/public.xml` & `apkutils-1.4.0/apkutils/axml/public.xml`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/cert.py` & `apkutils-1.4.0/apkutils/cert.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/cli.py` & `apkutils-1.4.0/apkutils/cli.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/__init__.py` & `apkutils-1.4.0/apkutils/dex/__init__.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/byteio.py` & `apkutils-1.4.0/apkutils/dex/byteio.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/dalvik.py` & `apkutils-1.4.0/apkutils/dex/dalvik.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/dalvikformats.py` & `apkutils-1.4.0/apkutils/dex/dalvikformats.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/dexparser.py` & `apkutils-1.4.0/apkutils/dex/dexparser.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/flags.py` & `apkutils-1.4.0/apkutils/dex/flags.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/__init__.py` & `apkutils-1.4.0/apkutils/dex/jvm/__init__.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/arraytypes.py` & `apkutils-1.4.0/apkutils/dex/jvm/arraytypes.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/constantpool.py` & `apkutils-1.4.0/apkutils/dex/jvm/constantpool.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/constants/__init__.py` & `apkutils-1.4.0/apkutils/dex/jvm/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/constants/calc.py` & `apkutils-1.4.0/apkutils/dex/jvm/constants/calc.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/constants/genlookup.py` & `apkutils-1.4.0/apkutils/dex/jvm/constants/genlookup.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/constants/lookup.py` & `apkutils-1.4.0/apkutils/dex/jvm/constants/lookup.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/error.py` & `apkutils-1.4.0/apkutils/dex/jvm/error.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/genmathops.py` & `apkutils-1.4.0/apkutils/dex/jvm/genmathops.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/ir.py` & `apkutils-1.4.0/apkutils/dex/jvm/ir.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/jvmops.py` & `apkutils-1.4.0/apkutils/dex/jvm/jvmops.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/mathops.py` & `apkutils-1.4.0/apkutils/dex/jvm/mathops.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/optimization/__init__.py` & `apkutils-1.4.0/apkutils/dex/jvm/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/optimization/consts.py` & `apkutils-1.4.0/apkutils/dex/jvm/optimization/consts.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/optimization/jumps.py` & `apkutils-1.4.0/apkutils/dex/jvm/optimization/jumps.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/optimization/options.py` & `apkutils-1.4.0/apkutils/dex/jvm/optimization/options.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/optimization/registers.py` & `apkutils-1.4.0/apkutils/dex/jvm/optimization/registers.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/optimization/stack.py` & `apkutils-1.4.0/apkutils/dex/jvm/optimization/stack.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/scalartypes.py` & `apkutils-1.4.0/apkutils/dex/jvm/scalartypes.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/writebytecode.py` & `apkutils-1.4.0/apkutils/dex/jvm/writebytecode.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/writeclass.py` & `apkutils-1.4.0/apkutils/dex/jvm/writeclass.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/jvm/writeir.py` & `apkutils-1.4.0/apkutils/dex/jvm/writeir.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/mutf8.py` & `apkutils-1.4.0/apkutils/dex/mutf8.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/treelist.py` & `apkutils-1.4.0/apkutils/dex/treelist.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/typeinference/__init__.py` & `apkutils-1.4.0/apkutils/dex/typeinference/__init__.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/typeinference/typeinference.py` & `apkutils-1.4.0/apkutils/dex/typeinference/typeinference.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/dex/util.py` & `apkutils-1.4.0/apkutils/dex/util.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/elf/elfparser.py` & `apkutils-1.4.0/apkutils/elf/elfparser.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/gdiff.py` & `apkutils-1.4.0/apkutils/gdiff.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/intersection.py` & `apkutils-1.4.0/apkutils/intersection.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/apkutils/wildcard.py` & `apkutils-1.4.0/apkutils/wildcard.py`

 * *Files identical despite different names*

### Comparing `apkutils-1.3.0/pyproject.toml` & `apkutils-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   "Natural Language :: Chinese (Simplified)",
   "Development Status :: 3 - Alpha",
 ]
 description = "一个APK解析库"
 license = "MIT"
 name = "apkutils"
 repository = "https://gitee.com/kin9-0rz/apkutils"
-version = "1.3.0"
+version = "1.4.0"
 
 [tool.poetry.dependencies]
 Pygments = "^2.12.0"
 beautifulsoup4 = "^4.10.0"
 click = "^8.0.3"
 cryptography = "^35.0.0"
 lxml = "^4.6.4"
```

### Comparing `apkutils-1.3.0/PKG-INFO` & `apkutils-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkutils
-Version: 1.3.0
+Version: 1.4.0
 Summary: 一个APK解析库
 Home-page: https://gitee.com/kin9-0rz/apkutils
 License: MIT
 Author: kin9-0rz
 Author-email: kin9-0rz@outlook.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 3 - Alpha
```

