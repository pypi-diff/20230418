# Comparing `tmp/unigui-1.3.6.tar.gz` & `tmp/unigui-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unigui-1.3.6.tar", last modified: Fri Apr 14 15:04:56 2023, max compression
+gzip compressed data, was "unigui-1.3.7.tar", last modified: Mon Apr 17 22:01:53 2023, max compression
```

## Comparing `unigui-1.3.6.tar` & `unigui-1.3.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-14 15:04:56.218741 unigui-1.3.6/
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.3.6/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.3.6/MANIFEST.in
--rw-r--r--   0 george    (1000) george    (1000)    18851 2023-04-14 15:04:56.218741 unigui-1.3.6/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)    18581 2023-03-08 16:33:36.000000 unigui-1.3.6/README.md
--rw-r--r--   0 george    (1000) george    (1000)       38 2023-04-14 15:04:56.218741 unigui-1.3.6/setup.cfg
--rw-r--r--   0 george    (1000) george    (1000)      565 2023-04-14 15:04:24.000000 unigui-1.3.6/setup.py
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-14 15:04:56.212074 unigui-1.3.6/unigui/
--rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:50.000000 unigui-1.3.6/unigui/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     7493 2023-03-08 16:33:36.000000 unigui-1.3.6/unigui/guielements.py
--rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.3.6/unigui/manager.py
--rw-r--r--   0 george    (1000) george    (1000)     3654 2022-09-03 18:32:40.000000 unigui-1.3.6/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.3.6/unigui/userset.py
--rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:22.000000 unigui-1.3.6/unigui/utils.py
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-14 15:04:56.215407 unigui-1.3.6/unigui/web/
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-14 15:04:56.215407 unigui-1.3.6/unigui/web/css/
--rw-r--r--   0 george    (1000) george    (1000)     3267 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/css/993.ac2fa104.css
--rw-r--r--   0 george    (1000) george    (1000)        0 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/css/app.31d6cfe0.css
--rw-r--r--   0 george    (1000) george    (1000)   219590 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/css/vendor.49a52e8f.css
--rw-r--r--   0 george    (1000) george    (1000)    64483 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/favicon.ico
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-14 15:04:56.215407 unigui-1.3.6/unigui/web/fonts/
--rw-r--r--   0 george    (1000) george    (1000)    20436 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0 george    (1000) george    (1000)    20544 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0 george    (1000) george    (1000)    20416 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0 george    (1000) george    (1000)    20408 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0 george    (1000) george    (1000)    20424 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0 george    (1000) george    (1000)    20344 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0 george    (1000) george    (1000)   164912 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0 george    (1000) george    (1000)   128360 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-14 15:04:56.215407 unigui-1.3.6/unigui/web/icons/
--rw-r--r--   0 george    (1000) george    (1000)    12324 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/icons/favicon-128x128.png
--rw-r--r--   0 george    (1000) george    (1000)      859 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/icons/favicon-16x16.png
--rw-r--r--   0 george    (1000) george    (1000)     2039 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/icons/favicon-32x32.png
--rw-r--r--   0 george    (1000) george    (1000)     9643 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/icons/favicon-96x96.png
--rw-r--r--   0 george    (1000) george    (1000)      907 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/index.html
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-14 15:04:56.215407 unigui-1.3.6/unigui/web/js/
--rw-r--r--   0 george    (1000) george    (1000)      763 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/js/193.b4cc3ffe.js
--rw-r--r--   0 george    (1000) george    (1000)     6560 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/js/430.4be6e8a8.js
--rw-r--r--   0 george    (1000) george    (1000)    39467 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/js/993.814659bd.js
--rw-r--r--   0 george    (1000) george    (1000)     5868 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/js/app.f2f7d718.js
--rw-r--r--   0 george    (1000) george    (1000)   847622 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/js/vendor.c0de6c67.js
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-14 15:04:56.215407 unigui-1.3.6/unigui.egg-info/
--rw-r--r--   0 george    (1000) george    (1000)    18851 2023-04-14 15:04:56.000000 unigui-1.3.6/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)     1194 2023-04-14 15:04:56.000000 unigui-1.3.6/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-04-14 15:04:56.000000 unigui-1.3.6/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.3.6/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-04-14 15:04:56.000000 unigui-1.3.6/unigui.egg-info/top_level.txt
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-17 22:01:53.631464 unigui-1.3.7/
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.3.7/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.3.7/MANIFEST.in
+-rw-r--r--   0 george    (1000) george    (1000)    18851 2023-04-17 22:01:53.631464 unigui-1.3.7/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)    18581 2023-03-08 16:33:36.000000 unigui-1.3.7/README.md
+-rw-r--r--   0 george    (1000) george    (1000)       38 2023-04-17 22:01:53.631464 unigui-1.3.7/setup.cfg
+-rw-r--r--   0 george    (1000) george    (1000)      565 2023-04-17 22:01:38.000000 unigui-1.3.7/setup.py
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-17 22:01:53.628131 unigui-1.3.7/unigui/
+-rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:50.000000 unigui-1.3.7/unigui/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     7560 2023-04-17 20:46:05.000000 unigui-1.3.7/unigui/guielements.py
+-rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.3.7/unigui/manager.py
+-rw-r--r--   0 george    (1000) george    (1000)     3654 2022-09-03 18:32:40.000000 unigui-1.3.7/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.3.7/unigui/userset.py
+-rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:22.000000 unigui-1.3.7/unigui/utils.py
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-17 22:01:53.628131 unigui-1.3.7/unigui/web/
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-17 22:01:53.628131 unigui-1.3.7/unigui/web/css/
+-rw-r--r--   0 george    (1000) george    (1000)     3267 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/css/855.47c4761e.css
+-rw-r--r--   0 george    (1000) george    (1000)        0 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/css/app.31d6cfe0.css
+-rw-r--r--   0 george    (1000) george    (1000)   219590 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/css/vendor.49a52e8f.css
+-rw-r--r--   0 george    (1000) george    (1000)    64483 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/favicon.ico
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-17 22:01:53.631464 unigui-1.3.7/unigui/web/fonts/
+-rw-r--r--   0 george    (1000) george    (1000)    20436 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0 george    (1000) george    (1000)    20544 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0 george    (1000) george    (1000)    20416 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0 george    (1000) george    (1000)    20408 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0 george    (1000) george    (1000)    20424 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0 george    (1000) george    (1000)    20344 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0 george    (1000) george    (1000)   164912 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0 george    (1000) george    (1000)   128360 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-17 22:01:53.631464 unigui-1.3.7/unigui/web/icons/
+-rw-r--r--   0 george    (1000) george    (1000)    12324 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/icons/favicon-128x128.png
+-rw-r--r--   0 george    (1000) george    (1000)      859 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/icons/favicon-16x16.png
+-rw-r--r--   0 george    (1000) george    (1000)     2039 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/icons/favicon-32x32.png
+-rw-r--r--   0 george    (1000) george    (1000)     9643 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/icons/favicon-96x96.png
+-rw-r--r--   0 george    (1000) george    (1000)      907 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/index.html
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-17 22:01:53.631464 unigui-1.3.7/unigui/web/js/
+-rw-r--r--   0 george    (1000) george    (1000)      763 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/js/193.b4cc3ffe.js
+-rw-r--r--   0 george    (1000) george    (1000)     6560 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/js/430.4be6e8a8.js
+-rw-r--r--   0 george    (1000) george    (1000)    39631 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/js/855.e620c0f1.js
+-rw-r--r--   0 george    (1000) george    (1000)     5868 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/js/app.ed80a2d1.js
+-rw-r--r--   0 george    (1000) george    (1000)   847622 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/js/vendor.c0de6c67.js
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-17 22:01:53.628131 unigui-1.3.7/unigui.egg-info/
+-rw-r--r--   0 george    (1000) george    (1000)    18851 2023-04-17 22:01:53.000000 unigui-1.3.7/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)     1194 2023-04-17 22:01:53.000000 unigui-1.3.7/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-04-17 22:01:53.000000 unigui-1.3.7/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.3.7/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-04-17 22:01:53.000000 unigui-1.3.7/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.3.6/LICENSE` & `unigui-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/PKG-INFO` & `unigui-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.3.6
+Version: 1.3.7
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `unigui-1.3.6/README.md` & `unigui-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/setup.py` & `unigui-1.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.3.6',      
+      version='1.3.7',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal app browser',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.3.6/unigui/guielements.py` & `unigui-1.3.7/unigui/guielements.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,18 +91,18 @@
             self.ratio = "9/9"
 
 class Graph(Gui):
     '''has to contain nodes, edges, see Readme'''
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.type='graph'
-        if not hasattr(self,'width'):
-            self.width = 800.0              
-        if not hasattr(self,'height'):
-            self.height = 600.0              
+        if not hasattr(self,'minwidth'):
+            self.minwidth = 600.0              
+        if not hasattr(self,'minheight'):
+            self.minheight = 600.0              
         self.check('nodes', 'edges')
 
 class Switch(Gui):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.check('value')        
 
@@ -149,19 +149,21 @@
             del t.rows[value]  
         t.value = None    
 
 class Table(Gui):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)             
         self.check('rows', 'headers','value')
-        if not hasattr(self,'edit') or self.edit != False:
+        if not hasattr(self,'edit') or self.edit:
             if not hasattr(self,'modify'):
                 self.modify = accept_cell_value 
             if not hasattr(self,'delete'):
                 self.delete = standart_table_delete 
+        if not hasattr(self,'rows'):
+            self.rows = []
 
     def selected_list(self):                            
         return [self.value] if self.value != None else [] if type(self.value) == int else self.value   
 
     def clean(self):
         self.rows = []
         self.value = [] if isinstance(self.value,(tuple, list)) else None
```

### Comparing `unigui-1.3.6/unigui/manager.py` & `unigui-1.3.7/unigui/manager.py`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/unigui/server.py` & `unigui-1.3.7/unigui/server.py`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/unigui/utils.py` & `unigui-1.3.7/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/unigui/web/css/993.ac2fa104.css` & `unigui-1.3.7/unigui/web/css/855.47c4761e.css`

 * *Files 16% similar despite different names*

```diff
@@ -1 +1 @@
-thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-3bf1da74]{display:flex;justify-content:center}.custom-caption[data-v-3bf1da74]{padding:5px!important}.web-camera-container[data-v-3bf1da74]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-3bf1da74]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-3bf1da74]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-3bf1da74]{opacity:1}.web-camera-container .camera-shoot[data-v-3bf1da74]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-3bf1da74]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-3bf1da74]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-3bf1da74]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-3bf1da74]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-3bf1da74]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-3bf1da74]{animation:preload-3bf1da74 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-3bf1da74]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-3bf1da74]:nth-child(3){animation-delay:.4s}@keyframes preload-3bf1da74{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-3bf1da74]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
+thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-e163239e]{display:flex;justify-content:center}.custom-caption[data-v-e163239e]{padding:5px!important}.web-camera-container[data-v-e163239e]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-e163239e]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-e163239e]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-e163239e]{opacity:1}.web-camera-container .camera-shoot[data-v-e163239e]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-e163239e]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-e163239e]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-e163239e]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-e163239e]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-e163239e]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-e163239e]{animation:preload-e163239e 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-e163239e]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-e163239e]:nth-child(3){animation-delay:.4s}@keyframes preload-e163239e{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-e163239e]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
```

### Comparing `unigui-1.3.6/unigui/web/css/vendor.49a52e8f.css` & `unigui-1.3.7/unigui/web/css/vendor.49a52e8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/unigui/web/favicon.ico` & `unigui-1.3.7/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.3.7/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.3.7/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.3.7/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.3.7/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.3.7/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.3.7/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.3.7/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `unigui-1.3.7/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/unigui/web/icons/favicon-128x128.png` & `unigui-1.3.7/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/unigui/web/icons/favicon-16x16.png` & `unigui-1.3.7/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/unigui/web/icons/favicon-32x32.png` & `unigui-1.3.7/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/unigui/web/icons/favicon-96x96.png` & `unigui-1.3.7/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/unigui/web/index.html` & `unigui-1.3.7/unigui/web/index.html`

 * *Files 18% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.c0de6c67.js></script><script defer src=js/app.f2f7d718.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.c0de6c67.js></script><script defer src=js/app.ed80a2d1.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.3.6/unigui/web/js/193.b4cc3ffe.js` & `unigui-1.3.7/unigui/web/js/193.b4cc3ffe.js`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/unigui/web/js/430.4be6e8a8.js` & `unigui-1.3.7/unigui/web/js/430.4be6e8a8.js`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/unigui/web/js/993.814659bd.js` & `unigui-1.3.7/unigui/web/js/855.e620c0f1.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [993], {
-        4993: (e, t, a) => {
+    [855], {
+        9855: (e, t, a) => {
             a.r(t), a.d(t, {
-                default: () => Ot
+                default: () => Qt
             });
             var l = a(3673),
                 s = a(2323);
             const o = (0, l._)("div", {
                 class: "q-pa-lg"
             }, null, -1);
 
@@ -216,15 +216,15 @@
                     e.styleSize = `height: ${h+s}px; width: ${n.clientWidth+c+t}px;`
                 }
             }
 
             function V(e) {
                 const t = u.screen.blocks;
                 let a = window.innerHeight;
-                a -= 10;
+                a -= 2;
                 let l = {},
                     s = new Map,
                     o = {};
                 for (let [d, r] of Object.entries(y)) o[r.name] = r.$el.getBoundingClientRect().height;
                 let i = [];
                 for (let d of t) {
                     const e = [];
@@ -477,15 +477,15 @@
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"]))], 8, le)))), 256))])),
                     _: 1
                 })
             }
             var ie = a(8880);
-            const ne = e => ((0, l.dD)("data-v-3bf1da74"), e = e(), (0, l.Cn)(), e),
+            const ne = e => ((0, l.dD)("data-v-e163239e"), e = e(), (0, l.Cn)(), e),
                 de = ["width", "height"],
                 re = ["src"],
                 ce = {
                     key: 15,
                     class: "web-camera-container"
                 },
                 he = {
@@ -1420,22 +1420,28 @@
                 }),
                 Ye = (0, U.Z)(Be, [
                     ["render", Ke]
                 ]),
                 Fe = Ye;
 
             function Xe(e) {
+                let t = e.minheight ? e.minheight : m,
+                    a = e.minwidth ? e.minwidth : f;
+                return `height: ${t}px; width: ${a}px`
+            }
+
+            function Je(e) {
                 let t = new FormData;
                 t.append("image", e);
                 let a = new XMLHttpRequest;
                 a.open("POST", "http://localhost:8000", !0), a.onload = function() {
                     200 === this.status ? console.log(this.response) : console.error(a)
                 }, a.send(t)
             }
-            const Je = (0, l.aZ)({
+            const Ge = (0, l.aZ)({
                 name: "element",
                 components: {
                     utable: Ue,
                     cgraph: Fe
                 },
                 methods: {
                     log(e) {
@@ -1501,38 +1507,39 @@
                             }), e)
                         }
                         this.isPhotoTaken = !this.isPhotoTaken;
                         const e = this.$refs.canvas.getContext("2d");
                         e.drawImage(this.$refs.camera, 0, 0, 450, 337.5)
                     },
                     downloadImage() {
-                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(Xe, "image/jpeg")
+                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(Je, "image/jpeg")
                     },
                     geom() {
-                        const e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling,
-                            t = "docviewer" == this.type ? e : e.querySelector("table" == this.type ? ".scroll" : ".q-tree"),
-                            a = e.getBoundingClientRect();
+                        const e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
+                        let t = this.type;
+                        const a = "docviewer" == t || "graph" == t ? e : e.querySelector("table" == t ? ".scroll" : ".q-tree"),
+                            l = e.getBoundingClientRect();
                         return {
                             el: e,
-                            inner: t,
-                            left: a.left,
-                            right: a.right,
-                            top: a.top,
-                            scrollHeight: t.scrollHeight,
-                            scrollWidth: t.scrollWidth
+                            inner: a,
+                            left: l.left,
+                            right: l.right,
+                            top: l.top,
+                            scrollHeight: a.scrollHeight,
+                            scrollWidth: a.scrollWidth
                         }
                     }
                 },
                 mounted() {
                     b[this.fullname] = this, g && console.log("mounted", this.fullname)
                 },
                 data() {
                     return {
                         value: this.data.value,
-                        styleSize: w,
+                        styleSize: Xe(this.data),
                         options: [],
                         expandedKeys: [],
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
                             backgroundColor: "#027be3",
                             width: "4px",
@@ -1572,15 +1579,15 @@
                         return this.data.label ? this.data.label : "_" != this.data.name[0] ? this.data.name : ""
                     },
                     text() {
                         return this.data.text
                     },
                     expanding() {
                         let e = this.type;
-                        return "tree" == e || "table" == e || "list" == e || "docviewer" == e
+                        return "tree" == e || "table" == e || "list" == e || "docviewer" == e || "graph" == e
                     },
                     expanding_width() {
                         return !this.data.width && this.expanding
                     },
                     expanding_height() {
                         return !this.data.height && this.expanding
                     },
@@ -1638,50 +1645,50 @@
                         g && console.log("selection changed", e, this.$refs.inputRef), Array.isArray(e) || (e = [0, 0]);
                         let t = this.$refs.inputRef.$el;
                         t.focus();
                         let a = t.getElementsByTagName("textarea");
                         0 == a.length && (a = t.getElementsByTagName("input")), a[0].setSelectionRange(e[0], e[1])
                     },
                     data(e, t) {
-                        g && console.log("data update", this.fullname, t.name), this.expanding && (this.styleSize = w, console.log(`${this.name} size changed`)), this.value = this.data.value, this.updated = this.value, b[this.fullname] = this
+                        g && console.log("data update", this.fullname, t.name), this.expanding && (this.styleSize = Xe(this.data), console.log(`${this.name} size changed`)), this.value = this.data.value, this.updated = this.value, b[this.fullname] = this
                     }
                 }
             });
-            var Ge = a(4027),
-                et = a(9721),
-                tt = a(8886),
-                at = a(8761),
-                lt = a(1232),
-                st = a(5551),
-                ot = a(5869),
-                it = a(1745);
-            const nt = (0, U.Z)(Je, [
+            var et = a(4027),
+                tt = a(9721),
+                at = a(8886),
+                lt = a(8761),
+                st = a(1232),
+                ot = a(5551),
+                it = a(5869),
+                nt = a(1745);
+            const dt = (0, U.Z)(Ge, [
                     ["render", xe],
-                    ["__scopeId", "data-v-3bf1da74"]
+                    ["__scopeId", "data-v-e163239e"]
                 ]),
-                dt = nt;
-            R()(Je, "components", {
-                QImg: Ge.Z,
+                rt = dt;
+            R()(Ge, "components", {
+                QImg: et.Z,
                 QIcon: P.Z,
                 QSelect: He.Z,
-                QBadge: et.Z,
+                QBadge: tt.Z,
                 QCheckbox: Ve.Z,
-                QToggle: tt.Z,
-                QBtnToggle: at.Z,
+                QToggle: at.Z,
+                QBtnToggle: lt.Z,
                 QInput: $e.Z,
-                QScrollArea: lt.Z,
-                QTree: st.Z,
-                QSeparator: ot.Z,
-                QUploader: it.Z,
+                QScrollArea: st.Z,
+                QTree: ot.Z,
+                QSeparator: it.Z,
+                QUploader: nt.Z,
                 QBtn: ze.Z
             });
-            const rt = (0, l.aZ)({
+            const ct = (0, l.aZ)({
                 name: "block",
                 components: {
-                    element: dt
+                    element: rt
                 },
                 data() {
                     return {
                         styleSize: w,
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
@@ -1748,42 +1755,42 @@
                 },
                 watch: {
                     data(e) {
                         g && console.log("data update", this.name), this.styleSize = w, y[this.name] = this, this.expanding && (b[this.fullname] = this)
                     }
                 }
             });
-            var ct = a(151);
-            const ht = (0, U.Z)(rt, [
+            var ht = a(151);
+            const ut = (0, U.Z)(ct, [
                     ["render", oe]
                 ]),
-                ut = ht;
-            R()(rt, "components", {
-                QCard: ct.Z,
+                pt = ut;
+            R()(ct, "components", {
+                QCard: ht.Z,
                 QIcon: P.Z,
-                QScrollArea: lt.Z
+                QScrollArea: st.Z
             });
-            const pt = (0, l.aZ)({
+            const gt = (0, l.aZ)({
                     name: "zone",
                     components: {
-                        block: ut
+                        block: pt
                     },
                     props: {
                         data: Object
                     }
                 }),
-                gt = (0, U.Z)(pt, [
+                mt = (0, U.Z)(gt, [
                     ["render", J]
                 ]),
-                mt = gt,
-                ft = {
+                ft = mt,
+                wt = {
                     class: "row q-gutter-sm row-md"
                 };
 
-            function wt(e, t, a, o, i, n) {
+            function yt(e, t, a, o, i, n) {
                 const d = (0, l.up)("block"),
                     r = (0, l.up)("q-item-label"),
                     c = (0, l.up)("q-space"),
                     h = (0, l.up)("q-btn"),
                     u = (0, l.up)("q-card"),
                     p = (0, l.up)("q-dialog");
                 return (0, l.wg)(), (0, l.j4)(p, {
@@ -1799,32 +1806,32 @@
                             key: 0,
                             data: a.data
                         }, null, 8, ["data"])) : (0, l.kq)("", !0), (0, l.Wm)(r, {
                             class: "text-h6"
                         }, {
                             default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(a.data.text ? a.data.text : ""), 1)])),
                             _: 1
-                        }), (0, l._)("div", ft, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
+                        }), (0, l._)("div", wt, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
                             class: "col-md-3",
                             label: e,
                             color: a.buttons[0] == e ? "primary" : "secondary",
                             onClick: t => n.sendMessage(e)
                         }, null, 8, ["label", "color", "onClick"])))), 256))])])),
                         _: 1
                     }, 8, ["style"])])),
                     _: 1
                 }, 8, ["onHide"])
             }
-            const yt = {
+            const bt = {
                 props: {
                     data: Object,
                     buttons: Array
                 },
                 components: {
-                    block: ut
+                    block: pt
                 },
                 emits: ["ok", "hide"],
                 methods: {
                     show() {
                         this.$refs.dialog.show()
                     },
                     sendMessage(e) {
@@ -1840,30 +1847,30 @@
                         this.$emit("ok"), this.hide()
                     },
                     onCancelClick() {
                         this.hide()
                     }
                 }
             };
-            var bt = a(5926),
-                kt = a(2025);
-            const vt = (0, U.Z)(yt, [
-                    ["render", wt]
+            var kt = a(5926),
+                vt = a(2025);
+            const Ct = (0, U.Z)(bt, [
+                    ["render", yt]
                 ]),
-                Ct = vt;
-            R()(yt, "components", {
-                QDialog: bt.Z,
-                QCard: ct.Z,
+                xt = Ct;
+            R()(bt, "components", {
+                QDialog: kt.Z,
+                QCard: ht.Z,
                 QItemLabel: N.Z,
-                QSpace: kt.Z,
+                QSpace: vt.Z,
                 QBtn: ze.Z
             });
-            var xt = !0;
-            let qt = null;
-            const _t = (0, l.aZ)({
+            var qt = !0;
+            let _t = null;
+            const jt = (0, l.aZ)({
                 name: "MainLayout",
                 data() {
                     return {
                         leftDrawerOpen: !1,
                         menu: [],
                         tab: "",
                         localServer: !0,
@@ -1872,15 +1879,15 @@
                             blocks: []
                         },
                         prevHeight: 0
                     }
                 },
                 components: {
                     menubar: B,
-                    zone: mt
+                    zone: ft
                 },
                 created() {
                     v(this)
                 },
                 unmounted() {
                     window.removeEventListener("resize", this.onResize)
                 },
@@ -1897,15 +1904,15 @@
                     },
                     lens(e) {
                         let t = {
                                 title: "Photo lens",
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0,
-                                component: Ct
+                                component: xt
                             },
                             {
                                 height: a,
                                 ...l
                             } = e;
                         l.width = 750;
                         let s = {
@@ -1923,85 +1930,85 @@
                         let a = t,
                             l = {
                                 message: e,
                                 type: t,
                                 position: "top",
                                 icon: a
                             };
-                        "progress" == t ? null == qt ? (l = {
+                        "progress" == t ? null == _t ? (l = {
                             group: !1,
                             timeout: 0,
                             spinner: !0,
                             type: "info",
                             message: e || "Progress..",
                             position: "top",
                             color: "secondary"
-                        }, qt = this.$q.notify(l)) : null == e ? (qt(), qt = null) : (l = {
+                        }, _t = this.$q.notify(l)) : null == e ? (_t(), _t = null) : (l = {
                             caption: e
-                        }, qt(l)) : ("error" == t && l.type, this.$q.notify(l))
+                        }, _t(l)) : ("error" == t && l.type, this.$q.notify(l))
                     },
                     error(e) {
                         this.notify(e, "error")
                     },
                     info(e) {
                         this.notify(e, "info")
                     },
                     processMessage(e) {
-                        if (xt) xt = !1, this.menu = e[0].map((e => ({
+                        if (qt) qt = !1, this.menu = e[0].map((e => ({
                             name: e[0],
                             icon: e[1],
                             order: e[2]
                         }))), Q(), this.screen = e[1], this.tab = this.screen.name, g && console.log("init loading..");
                         else if ("screen" == e.type) A(), Q(), this.screen = e;
                         else if ("dialog" == e.type) {
                             let t = {
                                 title: e.name,
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0
                             };
-                            t.component = Ct, t.componentProps = {
+                            t.component = xt, t.componentProps = {
                                 data: e.content ? e.content : e,
                                 buttons: e.buttons
                             }, this.$q.dialog(t)
                         } else if (e.hasOwnProperty("answer")) $(e);
                         else {
                             e.update && M(e);
                             let t = !1;
                             for (let a of k) a in e && (this.notify(e[a], a), t = !0);
                             t || e.update || (this.error("Invalid data came from the server! Look the console."), console.log(`Invalid data came from the server! ${e}`))
                         }
-                        qt && !e.progress && this.notify(null, "progress")
+                        _t && !e.progress && this.notify(null, "progress")
                     }
                 },
                 mounted() {
                     Q(), window.addEventListener("resize", this.onResize)
                 },
                 updated() {
                     g && console.log("before updated")
                 }
             });
-            var jt = a(9214),
-                St = a(3812),
-                At = a(9570),
-                Zt = a(7547),
-                Mt = a(3269),
-                $t = a(2652),
-                zt = a(4379);
-            const Dt = (0, U.Z)(_t, [
+            var St = a(9214),
+                At = a(3812),
+                Zt = a(9570),
+                Mt = a(7547),
+                $t = a(3269),
+                zt = a(2652),
+                Dt = a(4379);
+            const Ot = (0, U.Z)(jt, [
                     ["render", i]
                 ]),
-                Ot = Dt;
-            R()(_t, "components", {
-                QLayout: jt.Z,
-                QHeader: St.Z,
-                QToolbar: At.Z,
+                Qt = Ot;
+            R()(jt, "components", {
+                QLayout: St.Z,
+                QHeader: At.Z,
+                QToolbar: Zt.Z,
                 QBtn: ze.Z,
                 QItemLabel: N.Z,
-                QTabs: Zt.Z,
-                QTab: Mt.Z,
-                QPageContainer: $t.Z,
-                QPage: zt.Z
+                QTabs: Mt.Z,
+                QTab: $t.Z,
+                QPageContainer: zt.Z,
+                QPage: Dt.Z
             })
         }
     }
 ]);
```

### Comparing `unigui-1.3.6/unigui/web/js/app.f2f7d718.js` & `unigui-1.3.7/unigui/web/js/app.ed80a2d1.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(993)]).then(r.bind(r, 4993)),
+                        component: () => Promise.all([r.e(736), r.e(855)]).then(r.bind(r, 9855)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -160,24 +160,24 @@
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, n) => (r.f[n](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             193: "b4cc3ffe",
             430: "4be6e8a8",
-            993: "814659bd"
+            855: "e620c0f1"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
             736: "49a52e8f",
-            993: "ac2fa104"
+            855: "47c4761e"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
             } catch (e) {
@@ -260,15 +260,15 @@
                 e(n, l, o, a)
             })),
             o = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                993: 1
+                855: 1
             };
             o[e] ? t.push(o[e]) : 0 !== o[e] && r[e] && t.push(o[e] = n(e).then((() => {
                 o[e] = 0
             }), (t => {
                 throw delete o[e], t
             })))
         }
```

### Comparing `unigui-1.3.6/unigui/web/js/vendor.c0de6c67.js` & `unigui-1.3.7/unigui/web/js/vendor.c0de6c67.js`

 * *Files identical despite different names*

### Comparing `unigui-1.3.6/unigui.egg-info/PKG-INFO` & `unigui-1.3.7/unigui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.3.6
+Version: 1.3.7
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `unigui-1.3.6/unigui.egg-info/SOURCES.txt` & `unigui-1.3.7/unigui.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 unigui.egg-info/PKG-INFO
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/993.ac2fa104.css
+unigui/web/css/855.47c4761e.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.49a52e8f.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
@@ -28,10 +28,10 @@
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
 unigui/web/js/193.b4cc3ffe.js
 unigui/web/js/430.4be6e8a8.js
-unigui/web/js/993.814659bd.js
-unigui/web/js/app.f2f7d718.js
+unigui/web/js/855.e620c0f1.js
+unigui/web/js/app.ed80a2d1.js
 unigui/web/js/vendor.c0de6c67.js
```

