# Comparing `tmp/poimage-0.0.8.tar.gz` & `tmp/poimage-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poimage-0.0.8.tar", last modified: Sun Feb 12 10:01:32 2023, max compression
+gzip compressed data, was "poimage-0.0.9.tar", last modified: Sun Feb 12 10:34:25 2023, max compression
```

## Comparing `poimage-0.0.8.tar` & `poimage-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-02-12 10:01:32.926820 poimage-0.0.8/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poimage-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     5260 2023-02-12 10:01:32.926820 poimage-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4730 2022-10-28 04:35:32.000000 poimage-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-02-12 10:01:32.893555 poimage-0.0.8/poimage/
--rw-rw-rw-   0        0        0       33 2022-09-15 15:08:00.000000 poimage-0.0.8/poimage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-12 10:01:32.906815 poimage-0.0.8/poimage/api/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poimage-0.0.8/poimage/api/__init__.py
--rw-rw-rw-   0        0        0     3064 2023-02-12 10:00:10.000000 poimage-0.0.8/poimage/api/image.py
-drwxrwxrwx   0        0        0        0 2023-02-12 10:01:32.911811 poimage-0.0.8/poimage/core/
--rw-rw-rw-   0        0        0     7297 2023-02-11 06:42:33.000000 poimage-0.0.8/poimage/core/ImageType.py
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poimage-0.0.8/poimage/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-12 10:01:32.913811 poimage-0.0.8/poimage/lib/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poimage-0.0.8/poimage/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-12 10:01:32.918809 poimage-0.0.8/poimage/lib/image/
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 poimage-0.0.8/poimage/lib/image/__init__.py
--rw-rw-rw-   0        0        0     2790 2022-10-23 06:14:12.000000 poimage-0.0.8/poimage/lib/image/add_watermark_service.py
--rw-rw-rw-   0        0        0     2237 2022-09-01 13:34:44.000000 poimage-0.0.8/poimage/lib/image/eliminate_background.py
-drwxrwxrwx   0        0        0        0 2023-02-12 10:01:32.903786 poimage-0.0.8/poimage.egg-info/
--rw-rw-rw-   0        0        0     5260 2023-02-12 10:01:32.000000 poimage-0.0.8/poimage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      507 2023-02-12 10:01:32.000000 poimage-0.0.8/poimage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-12 10:01:32.000000 poimage-0.0.8/poimage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-11 06:42:51.000000 poimage-0.0.8/poimage.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       61 2023-02-12 10:01:32.000000 poimage-0.0.8/poimage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-02-12 10:01:32.000000 poimage-0.0.8/poimage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      766 2023-02-12 10:01:32.928818 poimage-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poimage-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-12 10:01:32.924814 poimage-0.0.8/tests/
--rw-rw-rw-   0        0        0      183 2022-09-15 15:01:36.000000 poimage-0.0.8/tests/__init__.py
--rw-rw-rw-   0        0        0      765 2023-02-11 06:42:33.000000 poimage-0.0.8/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-02-12 10:34:25.317326 poimage-0.0.9/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poimage-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5260 2023-02-12 10:34:25.317326 poimage-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4730 2022-10-28 04:35:32.000000 poimage-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-02-12 10:34:25.284501 poimage-0.0.9/poimage/
+-rw-rw-rw-   0        0        0       33 2022-09-15 15:08:00.000000 poimage-0.0.9/poimage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-12 10:34:25.298622 poimage-0.0.9/poimage/api/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poimage-0.0.9/poimage/api/__init__.py
+-rw-rw-rw-   0        0        0     3063 2023-02-12 10:34:01.000000 poimage-0.0.9/poimage/api/image.py
+drwxrwxrwx   0        0        0        0 2023-02-12 10:34:25.302621 poimage-0.0.9/poimage/core/
+-rw-rw-rw-   0        0        0     7297 2023-02-11 06:42:33.000000 poimage-0.0.9/poimage/core/ImageType.py
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poimage-0.0.9/poimage/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-12 10:34:25.304623 poimage-0.0.9/poimage/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poimage-0.0.9/poimage/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-12 10:34:25.311333 poimage-0.0.9/poimage/lib/image/
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 poimage-0.0.9/poimage/lib/image/__init__.py
+-rw-rw-rw-   0        0        0     2790 2022-10-23 06:14:12.000000 poimage-0.0.9/poimage/lib/image/add_watermark_service.py
+-rw-rw-rw-   0        0        0     2237 2022-09-01 13:34:44.000000 poimage-0.0.9/poimage/lib/image/eliminate_background.py
+drwxrwxrwx   0        0        0        0 2023-02-12 10:34:25.295623 poimage-0.0.9/poimage.egg-info/
+-rw-rw-rw-   0        0        0     5260 2023-02-12 10:34:25.000000 poimage-0.0.9/poimage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      507 2023-02-12 10:34:25.000000 poimage-0.0.9/poimage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-12 10:34:25.000000 poimage-0.0.9/poimage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-11 06:42:51.000000 poimage-0.0.9/poimage.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       61 2023-02-12 10:34:25.000000 poimage-0.0.9/poimage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-02-12 10:34:25.000000 poimage-0.0.9/poimage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      766 2023-02-12 10:34:25.319318 poimage-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poimage-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-12 10:34:25.316317 poimage-0.0.9/tests/
+-rw-rw-rw-   0        0        0      183 2022-09-15 15:01:36.000000 poimage-0.0.9/tests/__init__.py
+-rw-rw-rw-   0        0        0      765 2023-02-11 06:42:33.000000 poimage-0.0.9/tests/test.py
```

### Comparing `poimage-0.0.8/LICENSE` & `poimage-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `poimage-0.0.8/PKG-INFO` & `poimage-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poimage
-Version: 0.0.8
+Version: 0.0.9
 Summary: pip install poimage
 Home-page: http://python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poimage/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poimage/blob/master/README.md
```

### Comparing `poimage-0.0.8/README.md` & `poimage-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `poimage-0.0.8/poimage/api/image.py` & `poimage-0.0.9/poimage/api/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     #     解析二维码
     #     :param qrcode_path: 二维码图片的路径
     #     :return:
     #     """
     #     mainImage.decode_qrcode(qrcode_path)
 
 
-def del_water_mark(input_image, output_image=r'./del_water_mark.jpg'):
+def del_watermark(input_image, output_image=r'./del_water_mark.jpg'):
     """
     去除微信文章的水印
     :param input_image:
     :param output_image:
     :return:
     """
     dir = os.getcwd()
```

### Comparing `poimage-0.0.8/poimage/core/ImageType.py` & `poimage-0.0.9/poimage/core/ImageType.py`

 * *Files identical despite different names*

### Comparing `poimage-0.0.8/poimage/lib/image/add_watermark_service.py` & `poimage-0.0.9/poimage/lib/image/add_watermark_service.py`

 * *Files identical despite different names*

### Comparing `poimage-0.0.8/poimage/lib/image/eliminate_background.py` & `poimage-0.0.9/poimage/lib/image/eliminate_background.py`

 * *Files identical despite different names*

### Comparing `poimage-0.0.8/poimage.egg-info/PKG-INFO` & `poimage-0.0.9/poimage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poimage
-Version: 0.0.8
+Version: 0.0.9
 Summary: pip install poimage
 Home-page: http://python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poimage/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poimage/blob/master/README.md
```

### Comparing `poimage-0.0.8/setup.cfg` & `poimage-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f69 6d61 6765 0d0a 7665 7273   = poimage..vers
-00000020: 696f 6e20 3d20 302e 302e 380d 0a64 6573  ion = 0.0.8..des
+00000020: 696f 6e20 3d20 302e 302e 390d 0a64 6573  ion = 0.0.9..des
 00000030: 6372 6970 7469 6f6e 203d 2070 6970 2069  cription = pip i
 00000040: 6e73 7461 6c6c 2070 6f69 6d61 6765 0d0a  nstall poimage..
 00000050: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000060: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
 00000070: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
 00000080: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
 00000090: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
```

### Comparing `poimage-0.0.8/tests/test.py` & `poimage-0.0.9/tests/test.py`

 * *Files identical despite different names*

