# Comparing `tmp/mesures-2.5.3.tar.gz` & `tmp/mesures-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mesures-2.5.3.tar", last modified: Wed Mar 29 16:51:04 2023, max compression
+gzip compressed data, was "dist/mesures-2.6.0.tar", last modified: Tue Apr 18 13:47:52 2023, max compression
```

## Comparing `mesures-2.5.3.tar` & `mesures-2.6.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-29 16:51:04.000000 mesures-2.5.3/
--rw-rw-r--   0 david     (1000) david     (1000)     2041 2022-11-15 17:47:41.000000 mesures-2.5.3/README.md
--rw-rw-r--   0 david     (1000) david     (1000)       25 2022-11-15 17:47:41.000000 mesures-2.5.3/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)      290 2023-03-29 16:51:04.000000 mesures-2.5.3/PKG-INFO
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-29 16:51:04.000000 mesures-2.5.3/mesures.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)      290 2023-03-29 16:51:04.000000 mesures-2.5.3/mesures.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-03-29 16:51:04.000000 mesures-2.5.3/mesures.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       33 2023-03-29 16:51:04.000000 mesures-2.5.3/mesures.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        8 2023-03-29 16:51:04.000000 mesures-2.5.3/mesures.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)      819 2023-03-29 16:51:04.000000 mesures-2.5.3/mesures.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)      560 2022-11-15 17:47:41.000000 mesures-2.5.3/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-29 16:51:04.000000 mesures-2.5.3/mesures/
--rw-rw-r--   0 david     (1000) david     (1000)     3075 2023-01-02 12:32:22.000000 mesures-2.5.3/mesures/almacenacau.py
--rw-rw-r--   0 david     (1000) david     (1000)     5138 2023-03-29 13:46:27.000000 mesures-2.5.3/mesures/f1.py
--rw-rw-r--   0 david     (1000) david     (1000)     3458 2023-02-15 12:32:06.000000 mesures-2.5.3/mesures/f5d.py
--rw-rw-r--   0 david     (1000) david     (1000)     3416 2023-01-02 12:32:22.000000 mesures-2.5.3/mesures/p5d.py
--rw-rw-r--   0 david     (1000) david     (1000)     1539 2023-01-02 12:32:22.000000 mesures-2.5.3/mesures/p2.py
--rw-rw-r--   0 david     (1000) david     (1000)     2049 2023-01-02 12:32:22.000000 mesures-2.5.3/mesures/cilcau.py
--rw-rw-r--   0 david     (1000) david     (1000)     2248 2023-03-29 16:50:14.000000 mesures-2.5.3/mesures/p1d.py
--rw-rw-r--   0 david     (1000) david     (1000)       75 2023-03-29 16:50:33.000000 mesures-2.5.3/mesures/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     5567 2023-03-29 16:50:14.000000 mesures-2.5.3/mesures/p1.py
--rw-rw-r--   0 david     (1000) david     (1000)     3636 2023-01-02 12:32:22.000000 mesures-2.5.3/mesures/a5d.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-29 16:51:04.000000 mesures-2.5.3/mesures/dates/
--rw-rw-r--   0 david     (1000) david     (1000)      256 2022-11-15 17:47:41.000000 mesures-2.5.3/mesures/dates/date.py
--rw-rw-r--   0 david     (1000) david     (1000)       96 2022-11-15 17:47:41.000000 mesures-2.5.3/mesures/dates/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     5801 2023-02-15 12:32:06.000000 mesures-2.5.3/mesures/f5.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-29 16:51:04.000000 mesures-2.5.3/mesures/parsers/
--rw-rw-r--   0 david     (1000) david     (1000)       24 2022-11-15 17:47:41.000000 mesures-2.5.3/mesures/parsers/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     4185 2022-11-29 14:12:56.000000 mesures-2.5.3/mesures/parsers/dummy_data.py
--rw-rw-r--   0 david     (1000) david     (1000)     3301 2023-01-02 12:32:22.000000 mesures-2.5.3/mesures/cupscau.py
--rw-rw-r--   0 david     (1000) david     (1000)     5896 2023-02-17 09:29:05.000000 mesures-2.5.3/mesures/mcil345.py
--rw-rw-r--   0 david     (1000) david     (1000)     4673 2023-01-02 12:32:22.000000 mesures-2.5.3/mesures/f3.py
--rw-rw-r--   0 david     (1000) david     (1000)     3017 2023-01-02 12:32:22.000000 mesures-2.5.3/mesures/cildat.py
--rw-rw-r--   0 david     (1000) david     (1000)     1995 2023-01-02 12:32:22.000000 mesures-2.5.3/mesures/p2d.py
--rw-rw-r--   0 david     (1000) david     (1000)     3009 2023-01-02 12:32:22.000000 mesures-2.5.3/mesures/agrecl.py
--rw-rw-r--   0 david     (1000) david     (1000)    19081 2022-11-15 17:47:41.000000 mesures-2.5.3/mesures/headers.py
--rw-rw-r--   0 david     (1000) david     (1000)     3649 2023-01-02 12:32:22.000000 mesures-2.5.3/mesures/b5d.py
--rw-rw-r--   0 david     (1000) david     (1000)     3263 2023-01-02 12:32:22.000000 mesures-2.5.3/mesures/enelectroaut.py
--rw-rw-r--   0 david     (1000) david     (1000)     3307 2023-01-02 12:32:22.000000 mesures-2.5.3/mesures/potelectro.py
--rw-rw-r--   0 david     (1000) david     (1000)     3185 2023-01-02 12:32:22.000000 mesures-2.5.3/mesures/cumpelectro.py
--rw-rw-r--   0 david     (1000) david     (1000)      624 2023-01-02 12:32:22.000000 mesures-2.5.3/mesures/cups45.py
--rw-rw-r--   0 david     (1000) david     (1000)     3259 2023-01-02 16:17:00.000000 mesures-2.5.3/mesures/cupsdat.py
--rw-rw-r--   0 david     (1000) david     (1000)     5899 2023-03-13 15:52:05.000000 mesures-2.5.3/mesures/medidas.py
--rw-rw-r--   0 david     (1000) david     (1000)     3405 2023-02-17 09:29:05.000000 mesures-2.5.3/mesures/autoconsumo.py
--rw-rw-r--   0 david     (1000) david     (1000)     3291 2023-01-02 12:32:22.000000 mesures-2.5.3/mesures/cupselectro.py
--rw-rw-r--   0 david     (1000) david     (1000)     5037 2023-01-02 12:32:22.000000 mesures-2.5.3/mesures/pmest.py
--rw-rw-r--   0 david     (1000) david     (1000)       32 2022-11-15 17:47:41.000000 mesures-2.5.3/requirements.txt
--rw-rw-r--   0 david     (1000) david     (1000)       79 2023-03-29 16:51:04.000000 mesures-2.5.3/setup.cfg
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-18 13:47:52.000000 mesures-2.6.0/
+-rw-rw-r--   0 david     (1000) david     (1000)     2041 2022-11-15 17:47:41.000000 mesures-2.6.0/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)       25 2022-11-15 17:47:41.000000 mesures-2.6.0/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)      290 2023-04-18 13:47:52.000000 mesures-2.6.0/PKG-INFO
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-18 13:47:52.000000 mesures-2.6.0/mesures.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)      290 2023-04-18 13:47:52.000000 mesures-2.6.0/mesures.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-04-18 13:47:52.000000 mesures-2.6.0/mesures.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       33 2023-04-18 13:47:52.000000 mesures-2.6.0/mesures.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        8 2023-04-18 13:47:52.000000 mesures-2.6.0/mesures.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      836 2023-04-18 13:47:52.000000 mesures-2.6.0/mesures.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      560 2022-11-15 17:47:41.000000 mesures-2.6.0/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-18 13:47:52.000000 mesures-2.6.0/mesures/
+-rw-rw-r--   0 david     (1000) david     (1000)     3141 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/almacenacau.py
+-rw-rw-r--   0 david     (1000) david     (1000)      434 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/utils.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5204 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/f1.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3524 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/f5d.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3482 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/p5d.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1539 2023-04-18 11:11:41.000000 mesures-2.6.0/mesures/p2.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2115 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/cilcau.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2314 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/p1d.py
+-rw-rw-r--   0 david     (1000) david     (1000)       75 2023-04-18 13:47:02.000000 mesures-2.6.0/mesures/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5633 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/p1.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3702 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/a5d.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-18 13:47:52.000000 mesures-2.6.0/mesures/dates/
+-rw-rw-r--   0 david     (1000) david     (1000)      256 2022-11-15 17:47:41.000000 mesures-2.6.0/mesures/dates/date.py
+-rw-rw-r--   0 david     (1000) david     (1000)       96 2022-11-15 17:47:41.000000 mesures-2.6.0/mesures/dates/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5867 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/f5.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-18 13:47:52.000000 mesures-2.6.0/mesures/parsers/
+-rw-rw-r--   0 david     (1000) david     (1000)       24 2022-11-15 17:47:41.000000 mesures-2.6.0/mesures/parsers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4185 2022-11-29 14:12:56.000000 mesures-2.6.0/mesures/parsers/dummy_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3367 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/cupscau.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5962 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/mcil345.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4739 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/f3.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3083 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/cildat.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2061 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/p2d.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3075 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/agrecl.py
+-rw-rw-r--   0 david     (1000) david     (1000)    19081 2022-11-15 17:47:41.000000 mesures-2.6.0/mesures/headers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3715 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/b5d.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3329 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/enelectroaut.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3373 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/potelectro.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3251 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/cumpelectro.py
+-rw-rw-r--   0 david     (1000) david     (1000)      624 2023-04-18 11:08:18.000000 mesures-2.6.0/mesures/cups45.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3325 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/cupsdat.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8317 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/medidas.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3471 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/autoconsumo.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3357 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/cupselectro.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5103 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/pmest.py
+-rw-rw-r--   0 david     (1000) david     (1000)       32 2022-11-15 17:47:41.000000 mesures-2.6.0/requirements.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       79 2023-04-18 13:47:52.000000 mesures-2.6.0/setup.cfg
```

### Comparing `mesures-2.5.3/README.md` & `mesures-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `mesures-2.5.3/mesures.egg-info/SOURCES.txt` & `mesures-2.6.0/mesures.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 mesures/p1.py
 mesures/p1d.py
 mesures/p2.py
 mesures/p2d.py
 mesures/p5d.py
 mesures/pmest.py
 mesures/potelectro.py
+mesures/utils.py
 mesures.egg-info/PKG-INFO
 mesures.egg-info/SOURCES.txt
 mesures.egg-info/dependency_links.txt
 mesures.egg-info/requires.txt
 mesures.egg-info/top_level.txt
 mesures/dates/__init__.py
 mesures/dates/date.py
```

### Comparing `mesures-2.5.3/setup.py` & `mesures-2.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `mesures-2.5.3/mesures/almacenacau.py` & `mesures-2.6.0/mesures/almacenacau.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
 from mesures.headers import ALMACENACAU_HEADER as columns
 from mesures.parsers.dummy_data import DummyKeys
+from mesures.utils import check_line_terminator_param
 import os
 import numpy as np
 import pandas as pd
 
 
 class ALMACENACAU(object):
     def __init__(self, data, distributor=None, compression='bz2', version=0):
@@ -73,14 +74,14 @@
         :return: file path of generated ALMACENACAU File
         """
         file_path = os.path.join('/tmp', self.filename)
         kwargs = {'sep': ';',
                   'header': False,
                   'columns': columns,
                   'index': False,
-                  'line_terminator': ';\n'
+                  check_line_terminator_param(): ';\n'
                   }
         if self.default_compression:
             kwargs.update({'compression': self.default_compression})
 
         self.file.to_csv(file_path, **kwargs)
         return file_path
```

### Comparing `mesures-2.5.3/mesures/f1.py` & `mesures-2.6.0/mesures/f1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
 from mesures.headers import F1_HEADER as COLUMNS
 from mesures.parsers.dummy_data import DummyCurve
+from mesures.utils import check_line_terminator_param
 from zipfile import ZipFile
 import os
 import pandas as pd
 
 
 class F1(object):
     def __init__(self, data, distributor=None, compression='bz2', version=0):
@@ -147,15 +148,15 @@
             dataf = self.file[(self.file['timestamp'] >= di) & (self.file['timestamp'] < df)]
             # dataf['timestamp'] = dataf['timestamp'].apply(lambda x: x.strftime('%Y/%m/%d %H:%M'))
             file_path = os.path.join('/tmp', self.filename)
             kwargs = {'sep': ';',
                       'header': False,
                       'columns': self.columns,
                       'index': False,
-                      'line_terminator': ';\n'
+                      check_line_terminator_param(): ';\n'
                       }
             if self.default_compression:
                 kwargs.update({'compression': self.default_compression})
 
             dataf.to_csv(file_path, **kwargs)
             daymin = df
             zipped_file.write(file_path, arcname=os.path.basename(file_path))
```

### Comparing `mesures-2.5.3/mesures/f5d.py` & `mesures-2.6.0/mesures/f5d.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
 from mesures.headers import F5D_HEADER as COLUMNS
 from mesures.f5 import F5, DTYPES
+from mesures.utils import check_line_terminator_param
 import os
 import pandas as pd
 
 TYPES = DTYPES.copy()
 TYPES.update({'factura': 'category'})
 
 
@@ -79,14 +80,14 @@
         :return: file path of generated F5D File
         """
         file_path = os.path.join('/tmp', self.filename)
         kwargs = {'sep': ';',
                   'header': False,
                   'columns': self.columns,
                   'index': False,
-                  'line_terminator': ';\n'
+                  check_line_terminator_param(): ';\n'
                   }
         if self.default_compression:
             kwargs.update({'compression': self.default_compression})
 
         self.file.to_csv(file_path, **kwargs)
         return file_path
```

### Comparing `mesures-2.5.3/mesures/p5d.py` & `mesures-2.6.0/mesures/p5d.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
 from mesures.headers import P5D_HEADER as COLUMNS
 from mesures.parsers.dummy_data import DummyCurve
+from mesures.utils import check_line_terminator_param
 import os
 import pandas as pd
 
 
 class P5D(object):
     def __init__(self, data, distributor=None, comer=None, compression='bz2', version=0):
         """
@@ -96,14 +97,14 @@
         :return: file path
         """
         file_path = os.path.join('/tmp', self.filename)
         kwargs = {'sep': ';',
                   'header': False,
                   'columns': self.columns,
                   'index': False,
-                  'line_terminator': ';\n'
+                  check_line_terminator_param(): ';\n'
                   }
         if self.default_compression:
             kwargs.update({'compression': self.default_compression})
 
         self.file.to_csv(file_path, **kwargs)
         return file_path
```

### Comparing `mesures-2.5.3/mesures/p2.py` & `mesures-2.6.0/mesures/p2.py`

 * *Files identical despite different names*

### Comparing `mesures-2.5.3/mesures/cilcau.py` & `mesures-2.6.0/mesures/cilcau.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
 from mesures.cupscau import CUPSCAU
 from mesures.headers import CILCAU_HEADER as columns
+from mesures.utils import check_line_terminator_param
 import os
 import numpy as np
 import pandas as pd
 
 
 class CILCAU(CUPSCAU):
     def __init__(self, data, distributor=None, compression='bz2', version=0):
@@ -49,14 +50,14 @@
         :return: file path of generated CUPSCAU File
         """
         file_path = os.path.join('/tmp', self.filename)
         kwargs = {'sep': ';',
                   'header': False,
                   'columns': columns,
                   'index': False,
-                  'line_terminator': ';\n'
+                  check_line_terminator_param(): ';\n'
                   }
         if self.default_compression:
             kwargs.update({'compression': self.default_compression})
 
         self.file.to_csv(file_path, **kwargs)
         return file_path
```

### Comparing `mesures-2.5.3/mesures/p1d.py` & `mesures-2.6.0/mesures/p1d.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
 from mesures.headers import P1_HEADER as COLUMNS
 from mesures.p1 import P1
+from mesures.utils import check_line_terminator_param
 import os
 
 
 class P1D(P1):
     def __init__(self, data, distributor=None, comer=None, compression='bz2', columns=COLUMNS, version=0):
         """
         :param data: list of dicts or absolute file_path
@@ -48,14 +49,14 @@
                 self.version = max(versions) + 1
 
         file_path = os.path.join('/tmp', self.filename)
         kwargs = {'sep': ';',
                   'header': False,
                   'columns': self.columns,
                   'index': False,
-                  'line_terminator': ';\n'
+                  check_line_terminator_param(): ';\n'
                   }
         if self.default_compression:
             kwargs.update({'compression': self.default_compression})
 
         self.file.to_csv(file_path, **kwargs)
         return file_path
```

### Comparing `mesures-2.5.3/mesures/p1.py` & `mesures-2.6.0/mesures/p1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
 from mesures.headers import P1_HEADER as COLUMNS
 from mesures.parsers.dummy_data import DummyCurve
+from mesures.utils import check_line_terminator_param
 from zipfile import ZipFile
 import os
 import pandas as pd
 
 
 class P1(object):
     def __init__(self, data, distributor=None, compression='bz2', columns=COLUMNS, version=0):
@@ -145,15 +146,15 @@
                         self.version = max(versions) + 1
                 # dataf['timestamp'] = dataf['timestamp'].apply(lambda x: x.strftime(DATETIME_HOUR_MASK))
                 file_path = os.path.join('/tmp', self.filename)
                 kwargs = {'sep': ';',
                           'header': False,
                           'columns': self.columns,
                           'index': False,
-                          'line_terminator': ';\n'
+                          check_line_terminator_param(): ';\n'
                           }
                 if self.default_compression:
                     kwargs.update({'compression': self.default_compression})
 
                 dataf.to_csv(file_path, **kwargs)
                 zipped_file.write(file_path, arcname=os.path.basename(file_path))
```

### Comparing `mesures-2.5.3/mesures/a5d.py` & `mesures-2.6.0/mesures/b5d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
-from mesures.headers import A5D_HEADER as columns
+from mesures.headers import B5D_HEADER as columns
 from mesures.parsers.dummy_data import DummyCurve
+from mesures.utils import check_line_terminator_param
 import os
 import pandas as pd
 
 
-class A5D():
+class B5D():
     def __init__(self, data, distributor=None, comer=None, compression='bz2', version=0):
         """
         :param data: list of dicts or absolute file_path
         :param distributor: str distributor REE code
         :param comer: str comer REE code
         :param compression: 'bz2', 'gz'... OR False otherwise
         """
         if isinstance(data, list):
             data = DummyCurve(data).curve_data
         self.file = self.reader(data)
         self.generation_date = datetime.now()
-        self.prefix = 'A5D'
+        self.prefix = 'B5D'
         self.default_compression = compression
         self.version = version
         self.distributor = distributor
         self.comer = comer
 
     def __repr__(self):
         return "{}: {} Wh".format(self.filename, self.total)
@@ -54,15 +55,15 @@
             return "{prefix}_{distributor}_{comer}_{timestamp}.{version}".format(
                 prefix=self.prefix, distributor=self.distributor, comer=self.comer,
                 timestamp=self.generation_date.strftime('%Y%m%d'), version=self.version
             )
 
     @property
     def total(self):
-        return int(self.file['ai'].sum())
+        return int(self.file['ae'].sum())
 
     @property
     def ai(self):
         return int(self.file['ai'].sum())
 
     @property
     def ae(self):
@@ -86,31 +87,30 @@
         else:
             raise Exception("Filepath must be an str or a list")
 
         df = df.groupby(['cups', 'timestamp', 'season', 'factura']).aggregate(
             {'ai': 'sum', 'ae': 'sum'}
         ).reset_index()
         df['timestamp'] = df['timestamp'].apply(lambda x: x.strftime('%Y/%m/%d %H:%M'))
-        for key in ['r1', 'r2', 'r3', 'r4', 'ae', 'method', 'firmeza']:
+        for key in ['r1', 'r2', 'r3', 'r4', 'method', 'firmeza']:
             df[key] = ''
+        df['ai'] = 0
         df = df[columns]
         return df
 
     def writer(self):
         """
-        A5D contains a hourly raw curve
+        B5D contains a hourly raw curve
         :return: file path
         """
         file_path = os.path.join('/tmp', self.filename)
-
         kwargs = {'sep': ';',
                   'header': False,
                   'columns': columns,
                   'index': False,
-                  'line_terminator': ';\n'
+                  check_line_terminator_param(): ';\n'
                   }
         if self.default_compression:
             kwargs.update({'compression': self.default_compression})
 
         self.file.to_csv(file_path, **kwargs)
-
         return file_path
```

### Comparing `mesures-2.5.3/mesures/f5.py` & `mesures-2.6.0/mesures/f5.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
 from mesures.headers import F5_HEADER as COLUMNS
 from mesures.parsers.dummy_data import DummyCurve
+from mesures.utils import check_line_terminator_param
 from zipfile import ZipFile
 import os
 import pandas as pd
 
 
 DTYPES = {'cups': 'category',
           'season': 'category',
@@ -158,15 +159,15 @@
             dataf = self.file[(self.file['timestamp'] >= di) & (self.file['timestamp'] < df)]
             # dataf['timestamp'] = dataf['timestamp'].apply(lambda x: x.strftime(DATETIME_HOUR_MASK))
             file_path = os.path.join('/tmp', self.filename)
             kwargs = {'sep': ';',
                       'header': False,
                       'columns': self.columns,
                       'index': False,
-                      'line_terminator': ';\n'
+                      check_line_terminator_param(): ';\n'
                       }
             if self.default_compression:
                 kwargs.update({'compression': self.default_compression})
 
             dataf.to_csv(file_path, **kwargs)
             daymin = df
             zipped_file.write(file_path, arcname=os.path.basename(file_path))
```

### Comparing `mesures-2.5.3/mesures/parsers/dummy_data.py` & `mesures-2.6.0/mesures/parsers/dummy_data.py`

 * *Files identical despite different names*

### Comparing `mesures-2.5.3/mesures/cupscau.py` & `mesures-2.6.0/mesures/cupscau.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
 from mesures.headers import CUPSCAU_HEADER as columns
 from mesures.parsers.dummy_data import DummyKeys
+from mesures.utils import check_line_terminator_param
 import os
 import numpy as np
 import pandas as pd
 
 
 class CUPSCAU(object):
     def __init__(self, data, distributor=None, compression='bz2', version=0):
@@ -87,14 +88,14 @@
         :return: file path of generated CUPSCAU File
         """
         file_path = os.path.join('/tmp', self.filename)
         kwargs = {'sep': ';',
                   'header': False,
                   'columns': columns,
                   'index': False,
-                  'line_terminator': ';\n'
+                  check_line_terminator_param(): ';\n'
                   }
         if self.default_compression:
             kwargs.update({'compression': self.default_compression})
 
         self.file.to_csv(file_path, **kwargs)
         return file_path
```

### Comparing `mesures-2.5.3/mesures/mcil345.py` & `mesures-2.6.0/mesures/mcil345.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
 from mesures.headers import MCIL345_HEADER as COLUMNS
 from mesures.parsers.dummy_data import DummyCurve
+from mesures.utils import check_line_terminator_param
 from zipfile import ZipFile
 import os
 import pandas as pd
 
 
 class MCIL345(object):
     def __init__(self, data, distributor=None, compression='bz2', version=0):
@@ -165,15 +166,15 @@
                         self.version = max(versions) + 1
 
                 file_path = os.path.join('/tmp', self.filename)
                 kwargs = {'sep': ';',
                           'header': False,
                           'columns': self.columns,
                           'index': False,
-                          'line_terminator': ';\n'
+                          check_line_terminator_param(): ';\n'
                           }
                 if self.default_compression:
                     kwargs.update({'compression': self.default_compression})
                 dataf.to_csv(file_path, **kwargs)
                 zipped_file.write(file_path, arcname=os.path.basename(file_path))
 
             daymin = df
```

### Comparing `mesures-2.5.3/mesures/f3.py` & `mesures-2.6.0/mesures/f3.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
 from mesures.headers import F3_HEADER as columns
 from mesures.parsers.dummy_data import DummyCurve
+from mesures.utils import check_line_terminator_param
 from zipfile import ZipFile
 import os
 import pandas as pd
 
 
 class F3(object):
     def __init__(self, data, distributor=None, compression='bz2', version=0):
@@ -121,15 +122,15 @@
             dataf['timestamp'] = dataf.apply(lambda row: row['timestamp'].strftime(DATETIME_HOUR_MASK),
                                              axis=1)
             file_path = os.path.join('/tmp', self.filename)
             kwargs = {'sep': ';',
                       'header': False,
                       'columns': columns,
                       'index': False,
-                      'line_terminator': ';\n'
+                      check_line_terminator_param(): ';\n'
                       }
             if self.default_compression:
                 kwargs.update({'compression': self.default_compression})
 
             dataf.to_csv(file_path, **kwargs)
             daymin = df
             zipped_file.write(file_path, arcname=os.path.basename(file_path))
```

### Comparing `mesures-2.5.3/mesures/cildat.py` & `mesures-2.6.0/mesures/cildat.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
 from mesures.headers import CILDAT_HEADER as COLUMNS
 from mesures.parsers.dummy_data import DummyKeys
+from mesures.utils import check_line_terminator_param
 import os
 import pandas as pd
 
 
 class CILDAT(object):
     def __init__(self, data, distributor=None, compression='bz2', version=0):
         """
@@ -77,15 +78,15 @@
         """
         file_path = os.path.join('/tmp', self.filename)
 
         kwargs = {'sep': ';',
                   'header': False,
                   'columns': COLUMNS,
                   'index': False,
-                  'line_terminator': ';\n'
+                  check_line_terminator_param(): ';\n'
                   }
 
         if self.default_compression:
             kwargs.update({'compression': self.default_compression})
 
         self.file.to_csv(file_path, **kwargs)
```

### Comparing `mesures-2.5.3/mesures/p2d.py` & `mesures-2.6.0/mesures/p2d.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 from mesures.headers import P2_HEADER as columns
 from mesures.p2 import P2
+from mesures.utils import check_line_terminator_param
 import os
 
 
 class P2D(P2):
     def __init__(self, data, distributor=None, comer=None, compression='bz2', version=0):
         """
         :param data: list of dicts or absolute file_path
@@ -38,14 +39,14 @@
         """
         file_path = os.path.join('/tmp', self.filename)
         self.file['timestamp'] = self.file.apply(lambda row: row['timestamp'].strftime('%Y/%m/%d %H:%M:%S'), axis=1)
         kwargs = {'sep': ';',
                   'header': False,
                   'columns': columns,
                   'index': False,
-                  'line_terminator': ';\n'
+                  check_line_terminator_param(): ';\n'
                   }
         if self.default_compression:
             kwargs.update({'compression': self.default_compression})
 
         self.file.to_csv(file_path, **kwargs)
         return file_path
```

### Comparing `mesures-2.5.3/mesures/agrecl.py` & `mesures-2.6.0/mesures/agrecl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
 from mesures.headers import AGRECL_HEADER as columns
 from mesures.parsers.dummy_data import DummyKeys
+from mesures.utils import check_line_terminator_param
 import os
 import pandas as pd
 
 
 class AGRECL(object):
     def __init__(self, data, distributor=None, compression='bz2', version=0):
         """
@@ -76,14 +77,14 @@
         :return: file path of generated AGRECL File
         """
         file_path = os.path.join('/tmp', self.filename)
         kwargs = {'sep': ';',
                   'header': False,
                   'columns': columns,
                   'index': False,
-                  'line_terminator': ';\n'
+                  check_line_terminator_param(): ';\n'
                   }
         if self.default_compression:
             kwargs.update({'compression': self.default_compression})
 
         self.file.to_csv(file_path, **kwargs)
         return file_path
```

### Comparing `mesures-2.5.3/mesures/headers.py` & `mesures-2.6.0/mesures/headers.py`

 * *Files identical despite different names*

### Comparing `mesures-2.5.3/mesures/b5d.py` & `mesures-2.6.0/mesures/a5d.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
-from mesures.headers import B5D_HEADER as columns
+from mesures.headers import A5D_HEADER as columns
 from mesures.parsers.dummy_data import DummyCurve
+from mesures.utils import check_line_terminator_param
 import os
 import pandas as pd
 
 
-class B5D():
+class A5D():
     def __init__(self, data, distributor=None, comer=None, compression='bz2', version=0):
         """
         :param data: list of dicts or absolute file_path
         :param distributor: str distributor REE code
         :param comer: str comer REE code
         :param compression: 'bz2', 'gz'... OR False otherwise
         """
         if isinstance(data, list):
             data = DummyCurve(data).curve_data
         self.file = self.reader(data)
         self.generation_date = datetime.now()
-        self.prefix = 'B5D'
+        self.prefix = 'A5D'
         self.default_compression = compression
         self.version = version
         self.distributor = distributor
         self.comer = comer
 
     def __repr__(self):
         return "{}: {} Wh".format(self.filename, self.total)
@@ -54,15 +55,15 @@
             return "{prefix}_{distributor}_{comer}_{timestamp}.{version}".format(
                 prefix=self.prefix, distributor=self.distributor, comer=self.comer,
                 timestamp=self.generation_date.strftime('%Y%m%d'), version=self.version
             )
 
     @property
     def total(self):
-        return int(self.file['ae'].sum())
+        return int(self.file['ai'].sum())
 
     @property
     def ai(self):
         return int(self.file['ai'].sum())
 
     @property
     def ae(self):
@@ -86,30 +87,31 @@
         else:
             raise Exception("Filepath must be an str or a list")
 
         df = df.groupby(['cups', 'timestamp', 'season', 'factura']).aggregate(
             {'ai': 'sum', 'ae': 'sum'}
         ).reset_index()
         df['timestamp'] = df['timestamp'].apply(lambda x: x.strftime('%Y/%m/%d %H:%M'))
-        for key in ['r1', 'r2', 'r3', 'r4', 'method', 'firmeza']:
+        for key in ['r1', 'r2', 'r3', 'r4', 'ae', 'method', 'firmeza']:
             df[key] = ''
-        df['ai'] = 0
         df = df[columns]
         return df
 
     def writer(self):
         """
-        B5D contains a hourly raw curve
+        A5D contains a hourly raw curve
         :return: file path
         """
         file_path = os.path.join('/tmp', self.filename)
+
         kwargs = {'sep': ';',
                   'header': False,
                   'columns': columns,
                   'index': False,
-                  'line_terminator': ';\n'
+                  check_line_terminator_param(): ';\n'
                   }
         if self.default_compression:
             kwargs.update({'compression': self.default_compression})
 
         self.file.to_csv(file_path, **kwargs)
+
         return file_path
```

### Comparing `mesures-2.5.3/mesures/enelectroaut.py` & `mesures-2.6.0/mesures/enelectroaut.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
 from mesures.headers import ENELECTROAUT_HEADER as columns
 from mesures.parsers.dummy_data import DummyCurve
+from mesures.utils import check_line_terminator_param
 from zipfile import ZipFile
 import os
 import pandas as pd
 
 
 class ENELECTROAUT(object):
     def __init__(self, data, distributor=None, compression='bz2', version=0):
@@ -77,15 +78,15 @@
         """
         zipped_file = ZipFile(os.path.join('/tmp', self.zip_filename), 'w')
         file_path = os.path.join('/tmp', self.filename)
         kwargs = {'sep': ';',
                   'header': False,
                   'columns': columns,
                   'index': False,
-                  'line_terminator': ';\n'
+                  check_line_terminator_param(): ';\n'
                   }
         if self.default_compression:
             kwargs.update({'compression': self.default_compression})
 
         self.file.to_csv(file_path, **kwargs)
         zipped_file.write(file_path, arcname=os.path.basename(file_path))
         zipped_file.close()
```

### Comparing `mesures-2.5.3/mesures/potelectro.py` & `mesures-2.6.0/mesures/potelectro.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
 from mesures.headers import POTELECTRO_HEADER as columns
 from mesures.parsers.dummy_data import DummyCurve
+from mesures.utils import check_line_terminator_param
 from zipfile import ZipFile
 import os
 import pandas as pd
 
 
 class POTELECTRO(object):
     def __init__(self, data, distributor=None, compression='bz2', version=0):
@@ -78,15 +79,15 @@
         """
         zipped_file = ZipFile(os.path.join('/tmp', self.zip_filename), 'w')
         file_path = os.path.join('/tmp', self.filename)
         kwargs = {'sep': ';',
                   'header': False,
                   'columns': columns,
                   'index': False,
-                  'line_terminator': ';\n'
+                  check_line_terminator_param(): ';\n'
                   }
         if self.default_compression:
             kwargs.update({'compression': self.default_compression})
 
         self.file.to_csv(file_path, **kwargs)
         zipped_file.write(file_path, arcname=os.path.basename(file_path))
         zipped_file.close()
```

### Comparing `mesures-2.5.3/mesures/cumpelectro.py` & `mesures-2.6.0/mesures/cumpelectro.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
 from mesures.headers import CUMPELECTRO_HEADER as columns
 from mesures.parsers.dummy_data import DummyCurve
+from mesures.utils import check_line_terminator_param
 from zipfile import ZipFile
 import os
 import pandas as pd
 
 
 class CUMPELECTRO(object):
     def __init__(self, data, distributor=None, compression='bz2', version=0):
@@ -76,15 +77,15 @@
         """
         zipped_file = ZipFile(os.path.join('/tmp', self.zip_filename), 'w')
         file_path = os.path.join('/tmp', self.filename)
         kwargs = {'sep': ';',
                   'header': False,
                   'columns': columns,
                   'index': False,
-                  'line_terminator': ';\n'
+                  check_line_terminator_param(): ';\n'
                   }
         if self.default_compression:
             kwargs.update({'compression': self.default_compression})
 
         self.file.to_csv(file_path, **kwargs)
         zipped_file.write(file_path, arcname=os.path.basename(file_path))
         zipped_file.close()
```

### Comparing `mesures-2.5.3/mesures/cups45.py` & `mesures-2.6.0/mesures/cups45.py`

 * *Files identical despite different names*

### Comparing `mesures-2.5.3/mesures/cupsdat.py` & `mesures-2.6.0/mesures/cupsdat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
 from mesures.headers import CUPSDAT_HEADER as COLUMNS
 from mesures.parsers.dummy_data import DummyKeys
+from mesures.utils import check_line_terminator_param
 import os
 import pandas as pd
 
 
 class CUPSDAT(object):
     def __init__(self, data, distributor=None, compression='bz2', columns=COLUMNS, version=0):
         """
@@ -83,15 +84,15 @@
 
         file_path = os.path.join('/tmp', self.filename)
 
         kwargs = {'sep': ';',
                   'header': False,
                   'columns': self.columns,
                   'index': False,
-                  'line_terminator': ';\n'
+                  check_line_terminator_param(): ';\n'
                   }
 
         if self.default_compression:
             kwargs.update({'compression': self.default_compression})
 
         self.file.to_csv(file_path, **kwargs)
```

### Comparing `mesures-2.5.3/mesures/medidas.py` & `mesures-2.6.0/mesures/pmest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
-from mesures.headers import MEDIDAS_HEADER as columns
+from mesures.headers import PMEST_HEADER as columns
 from mesures.parsers.dummy_data import DummyCurve
+from mesures.utils import check_line_terminator_param
 from zipfile import ZipFile
 import os
 import pandas as pd
 
 
-class MEDIDAS(object):
-    def __init__(self, data, period=2, distributor=None, file_type='medidas_cnmc', compression='bz2', version=0):
+class PMEST(object):
+    def __init__(self, data, distributor=None, compression='bz2', version=0):
         """
         :param data: list of dicts or absolute file_path
         :param distributor: str distributor REE code
-        :param file_type: str in ('medidas_cnmc', 'medidas_ree')
         :param compression: 'bz2', 'gz'... OR False otherwise
         """
         if isinstance(data, list):
             data = DummyCurve(data).curve_data
-        self.file_type = file_type
         self.file = self.reader(data)
         self.generation_date = datetime.now()
-        self.prefix = 'medidas'
+        self.prefix = 'PMEST'
         self.version = version
-        self.period = period
         self.distributor = distributor
         self.default_compression = compression
-        self.columns = columns
 
     def __repr__(self):
         return "{}: {} kWh".format(self.filename, self.total)
 
     def __gt__(self, other):
         return self.total > other.total
 
@@ -43,141 +40,116 @@
         return self.file.append(other.file)
 
     def __len__(self):
         return len(self.file)
 
     @property
     def filename(self):
-        filename = "{prefix}_{distributor}_{measures_date}_{period}_{timestamp}.{version}".format(
-            prefix=self.prefix,
-            distributor=self.distributor,
-            measures_date=self.measures_date,
-            period=self.period,
-            timestamp=self.generation_date.strftime('%Y%m%d'),
-            version=self.version
-        )
         if self.default_compression:
-            filename += '.{compression}'.format(compression=self.default_compression)
-
-        return filename
+            return "{prefix}_{distributor}_{measures_date}_{timestamp}.{version}.{compression}".format(
+                prefix=self.prefix, distributor=self.distributor, measures_date=self.measures_date.strftime('%Y%m%d'),
+                timestamp=self.generation_date.strftime('%Y%m%d'), version=self.version,
+                compression=self.default_compression
+            )
+        else:
+            return "{prefix}_{distributor}_{measures_date}_{timestamp}.{version}".format(
+                prefix=self.prefix, distributor=self.distributor, measures_date=self.measures_date.strftime('%Y%m%d'),
+                timestamp=self.generation_date.strftime('%Y%m%d'), version=self.version
+            )
 
     @property
-    def cnmc_filename(self):
-        filename = "{prefix}_{distributor}_{cil}_{measures_date}_{period}_{timestamp}.txt".format(
-            prefix=self.prefix,
-            distributor=self.distributor,
-            cil=self.cil,
-            measures_date=self.measures_date,
-            period=self.period,
+    def zip_filename(self):
+        return "{prefix}_{distributor}_{measures_date}_{timestamp}.zip".format(
+            prefix=self.prefix, distributor=self.distributor, measures_date=self.measures_date.strftime('%Y%m%d'),
             timestamp=self.generation_date.strftime('%Y%m%d')
         )
-
-        return filename
+    @property
+    def total(self):
+        return self.file['ai'].sum()
 
     @property
-    def zip_filename(self):
-        return "{prefix}_{distributor}_{measures_date}_{period}_{timestamp}.zip".format(
-            prefix=self.prefix, distributor=self.distributor, measures_date=self.measures_date,
-            period=self.period, timestamp=self.generation_date.strftime('%Y%m%d')
-        )
+    def ai(self):
+        return self.file['ai'].sum()
 
     @property
     def ae(self):
-        return int(self.file['ae'].sum())
+        return self.file['ae'].sum()
 
     @property
-    def r2(self):
-        return int(self.file['r2'].sum())
+    def r1(self):
+        return self.file['r1'].sum()
 
     @property
-    def r3(self):
-        return int(self.file['r3'].sum())
-
-    @property
-    def cils(self):
-        return list(set(self.file['cil']))
+    def r2(self):
+        return self.file['r2'].sum()
 
     @property
-    def hours_per_cil(self):
-        return self.file['cil'].value_counts().reset_index().to_dict('records')
+    def r3(self):
+        return self.file['r3'].sum()
 
     @property
-    def number_of_cils(self):
-        return len(list(set(self.file['cil'])))
+    def r4(self):
+        return self.file['r4'].sum()
 
     def reader(self, filepath):
         if isinstance(filepath, str):
-            df = pd.read_csv(filepath, sep=';', names=self.columns)
+            df = pd.read_csv(
+                filepath, sep=';', names=columns
+            )
         elif isinstance(filepath, list):
             df = pd.DataFrame(data=filepath)
         else:
             raise Exception("Filepath must be an str or a list")
-        try:
-            df['timestamp'] = df.apply(lambda row: row['timestamp'].strftime(DATETIME_MASK), axis=1)
-        except Exception as err:
-            # Timestamp is already well parsed
-            pass
 
-        # Group by CIL and balance energies
+        if 'tipo_medida' not in df:
+            # 8 absoluta
+            # 11 incremental
+            df['tipo_medida'] = 11
+        if 'method' not in df:
+            df['method'] = 7
         df = df.groupby(
-            ['cil',
-             'timestamp',
-             'season']
-        ).agg(
-            {'ai': 'sum',
-             'ae': 'sum',
-             'r1': 'sum',
-             'r2': 'sum',
-             'r3': 'sum',
-             'r4': 'sum',
-             'read_type': 'min'}
+            [
+                'pm', 'tipo_medida', 'timestamp', 'season', 'method'
+            ]
+        ).aggregate(
+            {
+                'ai': 'sum',
+                'ae': 'sum',
+                'r1': 'sum',
+                'r2': 'sum',
+                'r3': 'sum',
+                'r4': 'sum',
+            }
         ).reset_index()
-
-        df = df.sort_values(['cil', 'timestamp', 'season'])
-
-        for idx, row in df.iterrows():
-            ai_m = row.get('ai', 0.0)
-            ae_m = row.get('ae', 0.0)
-            balance = ae_m - ai_m
-            df.at[idx, 'ae'] = balance
-            # REE file does not admit negative balance
-            if self.file_type == 'medidas_ree':
-                df.at[idx, 'ae'] = max(0, balance)
-
-        for key in ['power_factor', 'power_factor_type']:
-            if key not in df:
-                df[key] = ''
-            df[key] = df[key].astype('str')
-
+        df = df[columns]
         return df
 
     def writer(self):
         """
-        MEDIDAS contains hourly generation curves
+        PMEST contains a curve files diary on zip
         :return: file path
         """
         daymin = self.file['timestamp'].min()
-        measures_date = datetime.strptime(daymin, DATETIME_MASK)
-        self.measures_date = measures_date.strftime('%Y%m')
-
-        cil = self.file['cil'].min()
-        self.cil = cil
+        daymax = self.file['timestamp'].max()
+        self.measures_date = daymin
+        zipped_file = ZipFile(os.path.join('/tmp', self.zip_filename), 'w')
+        while daymin <= daymax:
+            di = daymin
+            df = daymin + timedelta(days=1)
+            self.measures_date = di
+            dataf = self.file[(self.file['timestamp'] >= di) & (self.file['timestamp'] < df)]
+            dataf['timestamp'] = dataf.apply(lambda row: row['timestamp'].strftime('%Y/%m/%d %H'), axis=1)
+            file_path = os.path.join('/tmp', self.filename)
+            kwargs = {'sep': ';',
+                      'header': False,
+                      'columns': columns,
+                      'index': False,
+                      check_line_terminator_param(): ';\n'
+                      }
+            if self.default_compression:
+                kwargs.update({'compression': self.default_compression})
 
-        kwargs = {'sep': ';',
-                  'header': False,
-                  'columns': self.columns,
-                  'index': False,
-                  'line_terminator': ';\n'
-                  }
-
-        if self.file_type == 'medidas_cnmc':
-            file_path = os.path.join('/tmp', self.cnmc_filename)
-            self.file.to_csv(file_path, **kwargs)
-            zipped_file = ZipFile(os.path.join('/tmp', self.zip_filename), 'w')
+            dataf.to_csv(file_path, **kwargs)
+            daymin = df
             zipped_file.write(file_path, arcname=os.path.basename(file_path))
-            zipped_file.close()
-            file_path = zipped_file.filename
-        else:
-            file_path = os.path.join('/tmp', self.filename)
-            kwargs.update({'compression': self.default_compression})
-            self.file.to_csv(file_path, **kwargs)
-        return file_path
+        zipped_file.close()
+        return zipped_file.filename
```

### Comparing `mesures-2.5.3/mesures/autoconsumo.py` & `mesures-2.6.0/mesures/autoconsumo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
 from mesures.headers import AUTOCONSUMO_HEADER as columns
 from mesures.parsers.dummy_data import DummyKeys
+from mesures.utils import check_line_terminator_param
 import os
 import numpy as np
 import pandas as pd
 
 
 class AUTOCONSUMO(object):
     def __init__(self, data, distributor=None, compression='bz2', version=0):
@@ -82,14 +83,14 @@
         :return: file path of generated AUTOCONSUMO File
         """
         file_path = os.path.join('/tmp', self.filename)
         kwargs = {'sep': ';',
                   'header': False,
                   'columns': columns,
                   'index': False,
-                  'line_terminator': ';\n'
+                  check_line_terminator_param(): ';\n'
                   }
         if self.default_compression:
             kwargs.update({'compression': self.default_compression})
 
         self.file.to_csv(file_path, **kwargs)
         return file_path
```

### Comparing `mesures-2.5.3/mesures/cupselectro.py` & `mesures-2.6.0/mesures/cupselectro.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from mesures.dates import *
 from mesures.headers import CUPSELECTRO_HEADER as columns
 from mesures.parsers.dummy_data import DummyCurve
+from mesures.utils import check_line_terminator_param
 from zipfile import ZipFile
 import os
 import pandas as pd
 
 
 class CUPSELECTRO(object):
     def __init__(self, data, distributor=None, compression='bz2', version=0):
@@ -80,15 +81,15 @@
         """
         zipped_file = ZipFile(os.path.join('/tmp', self.zip_filename), 'w')
         file_path = os.path.join('/tmp', self.filename)
         kwargs = {'sep': ';',
                   'header': False,
                   'columns': columns,
                   'index': False,
-                  'line_terminator': ';\n'
+                  check_line_terminator_param(): ';\n'
                   }
         if self.default_compression:
             kwargs.update({'compression': self.default_compression})
 
         self.file.to_csv(file_path, **kwargs)
         zipped_file.write(file_path, arcname=os.path.basename(file_path))
         zipped_file.close()
```

