# Comparing `tmp/rapidocr_web-0.1.2-py3-none-any.whl.zip` & `tmp/rapidocr_web-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 42650 bytes, number of entries: 13
--rw-r--r--  2.0 unx       74 b- defN 23-Apr-16 05:25 rapidocr_web/__init__.py
--rw-r--r--  2.0 unx     1505 b- defN 23-Apr-16 05:25 rapidocr_web/api.py
--rw-r--r--  2.0 unx     1128 b- defN 23-Apr-16 05:25 rapidocr_web/ocrweb.py
--rw-r--r--  2.0 unx     2954 b- defN 23-Apr-16 05:25 rapidocr_web/task.py
--rw-r--r--  2.0 unx    16958 b- defN 23-Apr-16 05:25 rapidocr_web/static/css/favicon.ico
--rw-r--r--  2.0 unx     2065 b- defN 23-Apr-16 05:25 rapidocr_web/static/css/main.css
--rw-r--r--  2.0 unx    86341 b- defN 23-Apr-16 05:25 rapidocr_web/static/js/jquery-3.0.0.min.js
--rw-r--r--  2.0 unx     8202 b- defN 23-Apr-16 05:25 rapidocr_web/templates/index.html
--rw-r--r--  2.0 unx     4576 b- defN 23-Apr-16 05:25 rapidocr_web-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-16 05:25 rapidocr_web-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       96 b- defN 23-Apr-16 05:25 rapidocr_web-0.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Apr-16 05:25 rapidocr_web-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1101 b- defN 23-Apr-16 05:25 rapidocr_web-0.1.2.dist-info/RECORD
-13 files, 125105 bytes uncompressed, 40800 bytes compressed:  67.4%
+Zip file size: 42678 bytes, number of entries: 13
+-rw-r--r--  2.0 unx       74 b- defN 23-Apr-18 01:13 rapidocr_web/__init__.py
+-rw-r--r--  2.0 unx     1571 b- defN 23-Apr-18 01:13 rapidocr_web/api.py
+-rw-r--r--  2.0 unx     1128 b- defN 23-Apr-18 01:13 rapidocr_web/ocrweb.py
+-rw-r--r--  2.0 unx     2954 b- defN 23-Apr-18 01:13 rapidocr_web/task.py
+-rw-r--r--  2.0 unx    16958 b- defN 23-Apr-18 01:13 rapidocr_web/static/css/favicon.ico
+-rw-r--r--  2.0 unx     2065 b- defN 23-Apr-18 01:13 rapidocr_web/static/css/main.css
+-rw-r--r--  2.0 unx    86341 b- defN 23-Apr-18 01:13 rapidocr_web/static/js/jquery-3.0.0.min.js
+-rw-r--r--  2.0 unx     8202 b- defN 23-Apr-18 01:13 rapidocr_web/templates/index.html
+-rw-r--r--  2.0 unx     4576 b- defN 23-Apr-18 01:13 rapidocr_web-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 01:13 rapidocr_web-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       96 b- defN 23-Apr-18 01:13 rapidocr_web-0.1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Apr-18 01:13 rapidocr_web-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1101 b- defN 23-Apr-18 01:13 rapidocr_web-0.1.3.dist-info/RECORD
+13 files, 125171 bytes uncompressed, 40828 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: rapidocr_web/static/js/jquery-3.0.0.min.js
 Comment: 
 
 Filename: rapidocr_web/templates/index.html
 Comment: 
 
-Filename: rapidocr_web-0.1.2.dist-info/METADATA
+Filename: rapidocr_web-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: rapidocr_web-0.1.2.dist-info/WHEEL
+Filename: rapidocr_web-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: rapidocr_web-0.1.2.dist-info/entry_points.txt
+Filename: rapidocr_web-0.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapidocr_web-0.1.2.dist-info/top_level.txt
+Filename: rapidocr_web-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: rapidocr_web-0.1.2.dist-info/RECORD
+Filename: rapidocr_web-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapidocr_web/api.py

```diff
@@ -1,12 +1,13 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
 import argparse
 import json
+from pathlib import Path
 
 import cv2
 import numpy as np
 import uvicorn
 from fastapi import FastAPI, UploadFile
 from PIL import Image
 from rapidocr_onnxruntime import RapidOCR
@@ -50,12 +51,13 @@
 def main():
     parser = argparse.ArgumentParser('rapidocr_api')
     parser.add_argument('-ip', '--ip', type=str, default='0.0.0.0',
                         help='IP Address')
     parser.add_argument('-p', '--port', type=int, default=9003,
                         help='IP port')
     args = parser.parse_args()
-    uvicorn.run(app, host=args.ip, port=args.port, reload=True)
+    uvicorn.run(f"{Path(__file__).stem}:app",
+                host=args.ip, port=args.port, reload=True)
 
 
 if __name__ == '__main__':
     main()
```

## Comparing `rapidocr_web-0.1.2.dist-info/METADATA` & `rapidocr_web-0.1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidocr-web
-Version: 0.1.2
+Version: 0.1.3
 Summary: A cross platform OCR Library based on OnnxRuntime.
 Home-page: https://github.com/RapidAI/RapidOCR
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Download-URL: https://github.com/RapidAI/RapidOCR.git
 Keywords: ocr,text_detection,text_recognition,db,onnxruntime,paddleocr,openvino,rapidocr
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rapidocr-web Version: 0.1.2 Summary: A cross
+Metadata-Version: 2.1 Name: rapidocr-web Version: 0.1.3 Summary: A cross
 platform OCR Library based on OnnxRuntime. Home-page: https://github.com/
 RapidAI/RapidOCR Author: SWHL Author-email: liekkaskono@163.com License:
 Apache-2.0 Download-URL: https://github.com/RapidAI/RapidOCR.git Keywords:
 ocr,text_detection,text_recognition,db,onnxruntime,paddleocr,openvino,rapidocr
 Platform: Any Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

## Comparing `rapidocr_web-0.1.2.dist-info/RECORD` & `rapidocr_web-0.1.3.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 rapidocr_web/__init__.py,sha256=m-UGKHJ-31qL7pBis4nfoFz5fzb-dXsiTLNqY-xpSoA,74
-rapidocr_web/api.py,sha256=MZISs0knHPIbo6nRrc11epJ8cZ8n7p5DgINPUvt8fXE,1505
+rapidocr_web/api.py,sha256=b8Pv_r_CBKh-_nmceyaF_wY36GZXB_nIzmq31HF4n20,1571
 rapidocr_web/ocrweb.py,sha256=fw9XEBoJZqUjbH19izaHJvXfQ-prwO_LoPjQuE3g8QY,1128
 rapidocr_web/task.py,sha256=l6PrccgTQDcvS8ZppZMfYuIPCYK-6ym_-02NWRm4Uak,2954
 rapidocr_web/static/css/favicon.ico,sha256=CBE1NF6iiIax8WqZVR-vPRaPTcmWjlTWsk1fzEbSd8c,16958
 rapidocr_web/static/css/main.css,sha256=2HcVvoa5oSQONnuC6IjjmBd127Jv9Y5EFJGy32nTEZk,2065
 rapidocr_web/static/js/jquery-3.0.0.min.js,sha256=JmvOoLtYsmqlsWxa7mDSLMwa6dZ9rrIdtrrVYRnDRH0,86341
 rapidocr_web/templates/index.html,sha256=xUe3Xce289Of4XTfeafPTX5JMRsOTdgv2Md5EQwxm48,8202
-rapidocr_web-0.1.2.dist-info/METADATA,sha256=jMN_zBBW35i3NI1OiTZ9HHv8gazdsFDrKmOLn1vrHQo,4576
-rapidocr_web-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rapidocr_web-0.1.2.dist-info/entry_points.txt,sha256=gKWhYdRif2OyYYQBX6An49Q7XaLO-nuCR2AoIp6LrS8,96
-rapidocr_web-0.1.2.dist-info/top_level.txt,sha256=dArjxF38AFvTF1Ae-mGaxBhwnETUJ4sLF_nQ93HC5A4,13
-rapidocr_web-0.1.2.dist-info/RECORD,,
+rapidocr_web-0.1.3.dist-info/METADATA,sha256=OLFKAL8F8H_Eoq_kRhU-Hdmf-i8B16h4He44WZokS44,4576
+rapidocr_web-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rapidocr_web-0.1.3.dist-info/entry_points.txt,sha256=gKWhYdRif2OyYYQBX6An49Q7XaLO-nuCR2AoIp6LrS8,96
+rapidocr_web-0.1.3.dist-info/top_level.txt,sha256=dArjxF38AFvTF1Ae-mGaxBhwnETUJ4sLF_nQ93HC5A4,13
+rapidocr_web-0.1.3.dist-info/RECORD,,
```

