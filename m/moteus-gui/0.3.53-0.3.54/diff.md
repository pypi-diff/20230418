# Comparing `tmp/moteus_gui-0.3.53-py3-none-any.whl.zip` & `tmp/moteus_gui-0.3.54-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 13974 bytes, number of entries: 9
+Zip file size: 13973 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 21-Dec-22 22:21 moteus_gui/__init__.py
--rw-r--r--  2.0 unx    40041 b- defN 23-Feb-03 03:00 moteus_gui/tview.py
+-rw-r--r--  2.0 unx    40041 b- defN 23-Mar-21 01:34 moteus_gui/tview.py
 -rw-rw-r--  2.0 unx     5556 b- defN 22-Aug-08 01:13 moteus_gui/tview_main_window.ui
--rw-r--r--  2.0 unx      609 b- defN 23-Feb-09 02:25 moteus_gui/version.py
--rw-r--r--  2.0 unx     1093 b- defN 23-Feb-09 02:25 moteus_gui-0.3.53.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-09 02:25 moteus_gui-0.3.53.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 23-Feb-09 02:25 moteus_gui-0.3.53.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Feb-09 02:25 moteus_gui-0.3.53.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      731 b- defN 23-Feb-09 02:25 moteus_gui-0.3.53.dist-info/RECORD
-9 files, 48182 bytes uncompressed, 12706 bytes compressed:  73.6%
+-rw-r--r--  2.0 unx      609 b- defN 23-Apr-18 14:33 moteus_gui/version.py
+-rw-r--r--  2.0 unx     1093 b- defN 23-Apr-18 14:33 moteus_gui-0.3.54.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 14:33 moteus_gui-0.3.54.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 23-Apr-18 14:33 moteus_gui-0.3.54.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-18 14:33 moteus_gui-0.3.54.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      731 b- defN 23-Apr-18 14:33 moteus_gui-0.3.54.dist-info/RECORD
+9 files, 48182 bytes uncompressed, 12705 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: moteus_gui/tview_main_window.ui
 Comment: 
 
 Filename: moteus_gui/version.py
 Comment: 
 
-Filename: moteus_gui-0.3.53.dist-info/METADATA
+Filename: moteus_gui-0.3.54.dist-info/METADATA
 Comment: 
 
-Filename: moteus_gui-0.3.53.dist-info/WHEEL
+Filename: moteus_gui-0.3.54.dist-info/WHEEL
 Comment: 
 
-Filename: moteus_gui-0.3.53.dist-info/entry_points.txt
+Filename: moteus_gui-0.3.54.dist-info/entry_points.txt
 Comment: 
 
-Filename: moteus_gui-0.3.53.dist-info/top_level.txt
+Filename: moteus_gui-0.3.54.dist-info/top_level.txt
 Comment: 
 
-Filename: moteus_gui-0.3.53.dist-info/RECORD
+Filename: moteus_gui-0.3.54.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## moteus_gui/version.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-VERSION="0.3.53"
+VERSION="0.3.54"
```

## Comparing `moteus_gui-0.3.53.dist-info/METADATA` & `moteus_gui-0.3.54.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moteus-gui
-Version: 0.3.53
+Version: 0.3.54
 Summary: moteus brushless controller graphical user interfaces
 Home-page: https://github.com/mjbots/moteus
 Author: mjbots Robotic Systems
 Author-email: info@mjbots.com
 License: UNKNOWN
 Keywords: moteus
 Platform: UNKNOWN
```

## Comparing `moteus_gui-0.3.53.dist-info/RECORD` & `moteus_gui-0.3.54.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 moteus_gui/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 moteus_gui/tview.py,sha256=fAbWAw2LdNW9p1DxpDsTCzu0cjjpZUrzfIKyp8bOnSI,40041
 moteus_gui/tview_main_window.ui,sha256=q_qA1sooIWzprVT8eYAe0EH9lfu7zg-QP1diETCNFh8,5556
-moteus_gui/version.py,sha256=VDpiAI-Zx1KOAlKr1Ct6EA7oQsYRfG0Uk22SOSkKZkc,609
-moteus_gui-0.3.53.dist-info/METADATA,sha256=aH8T5F9SYkIyeZMu-ycm_9wf9ABuLaNy9xRuwZQgcIE,1093
-moteus_gui-0.3.53.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-moteus_gui-0.3.53.dist-info/entry_points.txt,sha256=67EsNPaSGC4ni3r4yIV-qEq8VYuJaDmQWTwGtB9Dedo,49
-moteus_gui-0.3.53.dist-info/top_level.txt,sha256=oPOkXR-zpPFhGiDcbnDY6scvNqQQAXWzV7oPD_GHMns,11
-moteus_gui-0.3.53.dist-info/RECORD,,
+moteus_gui/version.py,sha256=jmm_-XvCr1X4UYMgpel9H6m6QGgp-Q9okhEFMeGSxRs,609
+moteus_gui-0.3.54.dist-info/METADATA,sha256=H8sTjSvGx06B2bC8F68qBaqr3_NzWRUQlx-C90JUNkg,1093
+moteus_gui-0.3.54.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+moteus_gui-0.3.54.dist-info/entry_points.txt,sha256=67EsNPaSGC4ni3r4yIV-qEq8VYuJaDmQWTwGtB9Dedo,49
+moteus_gui-0.3.54.dist-info/top_level.txt,sha256=oPOkXR-zpPFhGiDcbnDY6scvNqQQAXWzV7oPD_GHMns,11
+moteus_gui-0.3.54.dist-info/RECORD,,
```

