# Comparing `tmp/kft-0.1-py3.10.egg` & `tmp/kft-0.1.1-py3.10.egg`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 17519 bytes, number of entries: 15
--rw-rw-r--  2.0 unx     4686 b- defN 23-Apr-18 19:55 EGG-INFO/PKG-INFO
--rw-rw-r--  2.0 unx      267 b- defN 23-Apr-18 19:55 EGG-INFO/SOURCES.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Apr-18 19:55 EGG-INFO/dependency_links.txt
--rw-rw-r--  2.0 unx       55 b- defN 23-Apr-18 19:55 EGG-INFO/entry_points.txt
--rw-rw-r--  2.0 unx      119 b- defN 23-Apr-18 19:55 EGG-INFO/requires.txt
--rw-rw-r--  2.0 unx        4 b- defN 23-Apr-18 19:55 EGG-INFO/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Apr-18 19:55 EGG-INFO/zip-safe
--rw-rw-r--  2.0 unx        0 b- defN 23-Apr-18 19:54 kft/__init__.py
--rw-rw-r--  2.0 unx     5323 b- defN 23-Apr-18 19:54 kft/cli.py
--rw-rw-r--  2.0 unx     2907 b- defN 23-Apr-18 19:54 kft/kf_image_scanner.py
--rw-rw-r--  2.0 unx     9412 b- defN 23-Apr-18 19:54 kft/kf_upgrade_planner.py
--rw-rw-r--  2.0 unx      137 b- defN 23-Apr-18 19:55 kft/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--  2.0 unx     4283 b- defN 23-Apr-18 19:55 kft/__pycache__/cli.cpython-310.pyc
--rw-rw-r--  2.0 unx     2891 b- defN 23-Apr-18 19:55 kft/__pycache__/kf_image_scanner.cpython-310.pyc
--rw-rw-r--  2.0 unx     6443 b- defN 23-Apr-18 19:55 kft/__pycache__/kf_upgrade_planner.cpython-310.pyc
-15 files, 36529 bytes uncompressed, 15563 bytes compressed:  57.4%
+Zip file size: 17489 bytes, number of entries: 15
+-rw-rw-r--  2.0 unx     4638 b- defN 23-Apr-18 20:25 EGG-INFO/PKG-INFO
+-rw-rw-r--  2.0 unx      267 b- defN 23-Apr-18 20:25 EGG-INFO/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Apr-18 20:25 EGG-INFO/dependency_links.txt
+-rw-rw-r--  2.0 unx       55 b- defN 23-Apr-18 20:25 EGG-INFO/entry_points.txt
+-rw-rw-r--  2.0 unx      119 b- defN 23-Apr-18 20:25 EGG-INFO/requires.txt
+-rw-rw-r--  2.0 unx        4 b- defN 23-Apr-18 20:25 EGG-INFO/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Apr-18 20:25 EGG-INFO/zip-safe
+-rw-rw-r--  2.0 unx        0 b- defN 23-Apr-18 20:23 kft/__init__.py
+-rw-rw-r--  2.0 unx     5323 b- defN 23-Apr-18 20:23 kft/cli.py
+-rw-rw-r--  2.0 unx     2907 b- defN 23-Apr-18 20:23 kft/kf_image_scanner.py
+-rw-rw-r--  2.0 unx     9412 b- defN 23-Apr-18 20:23 kft/kf_upgrade_planner.py
+-rw-rw-r--  2.0 unx      137 b- defN 23-Apr-18 20:25 kft/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--  2.0 unx     4283 b- defN 23-Apr-18 20:25 kft/__pycache__/cli.cpython-310.pyc
+-rw-rw-r--  2.0 unx     2891 b- defN 23-Apr-18 20:25 kft/__pycache__/kf_image_scanner.cpython-310.pyc
+-rw-rw-r--  2.0 unx     6443 b- defN 23-Apr-18 20:25 kft/__pycache__/kf_upgrade_planner.cpython-310.pyc
+15 files, 36481 bytes uncompressed, 15533 bytes compressed:  57.4%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kft
-Version: 0.1
+Version: 0.1.1
 Summary: A collection of handy wrapper tools for operators of kubeflow environments
 Home-page: https://github.com/nishant-dash/kf-tools
 Author: Nishant Dash
 Author-email: nishant.dash@canonical.com
 License: MIT License
         
         Copyright (c) 2023 Nishant Dash
@@ -24,15 +24,14 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # kf-tools
 ### A collection of handy wrapper tools for operators of kubeflow environments
```

## kft/__pycache__/__init__.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 15:54:50 2023 UTC, .py size: 0 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4abd 3e64 0000 0000  o.......J.>d....
+00000000: 6f0d 0d0a 0000 0000 ecc3 3e64 0000 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0400 0000 6400  .....@...s....d.
 00000030: 5300 2901 4ea9 0072 0100 0000 7201 0000  S.).N..r....r...
 00000040: 0072 0100 0000 fa2c 6275 696c 642f 6264  .r.....,build/bd
 00000050: 6973 742e 6c69 6e75 782d 7838 365f 3634  ist.linux-x86_64
 00000060: 2f65 6767 2f6b 6674 2f5f 5f69 6e69 745f  /egg/kft/__init_
 00000070: 5f2e 7079 da08 3c6d 6f64 756c 653e 0100  _.py..<module>..
```

## kft/__pycache__/cli.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 15:54:50 2023 UTC, .py size: 5323 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4abd 3e64 cb14 0000  o.......J.>d....
+00000000: 6f0d 0d0a 0000 0000 ecc3 3e64 cb14 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 7201 0000 6400  .....@...sr...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6401 6c05 5a06 6400 6401 6c07 5a07 6500  d.l.Z.d.d.l.Z.e.
 00000060: a008 a100 6500 a009 a100 6404 6405 8400  ....e.....d.d...
 00000070: 8301 8301 5a0a 650a 6a0b 6406 6407 6408  ....Z.e.j.d.d.d.
```

## kft/__pycache__/kf_image_scanner.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 15:54:50 2023 UTC, .py size: 2907 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4abd 3e64 5b0b 0000  o.......J.>d[...
+00000000: 6f0d 0d0a 0000 0000 ecc3 3e64 5b0b 0000  o.........>d[...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 5a03 6401 6403 6c04 6d05 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6402 6c07 5a07 6401 6402 6c08 5a08 6401  d.l.Z.d.d.l.Z.d.
 00000060: 6404 6c09 6d0a 5a0a 0100 6401 6402 6c0b  d.l.m.Z...d.d.l.
 00000070: 5a0b 4700 6405 6406 8400 6406 8302 5a0c  Z.G.d.d...d...Z.
```

## kft/__pycache__/kf_upgrade_planner.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 15:54:50 2023 UTC, .py size: 9412 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4abd 3e64 c424 0000  o.......J.>d.$..
+00000000: 6f0d 0d0a 0000 0000 ecc3 3e64 c424 0000  o.........>d.$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d02 5a03 0100 6401 6402 6c04 5a04 6401  m.Z...d.d.l.Z.d.
 00000050: 6402 6c05 5a06 6401 6402 6c07 5a07 6401  d.l.Z.d.d.l.Z.d.
 00000060: 6404 6c08 6d09 5a0a 0100 6401 6405 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6406 6c0d 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

