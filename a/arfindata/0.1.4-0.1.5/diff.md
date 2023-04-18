# Comparing `tmp/arfindata-0.1.4.tar.gz` & `tmp/arfindata-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\arfindata-0.1.4.tar", last modified: Mon Apr 17 23:47:10 2023, max compression
+gzip compressed data, was "dist\arfindata-0.1.5.tar", last modified: Tue Apr 18 20:49:40 2023, max compression
```

## Comparing `arfindata-0.1.4.tar` & `arfindata-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 23:47:10.238335 arfindata-0.1.4/
--rw-rw-rw-   0        0        0     1088 2023-04-17 19:43:26.000000 arfindata-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0      332 2023-04-17 23:47:10.238335 arfindata-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3842 2023-04-17 22:09:45.000000 arfindata-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 23:47:10.225243 arfindata-0.1.4/arfindata/
--rw-rw-rw-   0        0        0     3241 2023-04-17 21:21:22.000000 arfindata-0.1.4/arfindata/ARdata.py
--rw-rw-rw-   0        0        0       98 2023-04-17 19:35:47.000000 arfindata-0.1.4/arfindata/__init__.py
--rw-rw-rw-   0        0        0     4200 2023-04-17 23:19:24.000000 arfindata-0.1.4/arfindata/sh.py
--rw-rw-rw-   0        0        0     5096 2023-04-17 23:19:25.000000 arfindata-0.1.4/arfindata/sz.py
-drwxrwxrwx   0        0        0        0 2023-04-17 23:47:10.236341 arfindata-0.1.4/arfindata.egg-info/
--rw-rw-rw-   0        0        0      332 2023-04-17 23:47:09.000000 arfindata-0.1.4/arfindata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-04-17 23:47:10.000000 arfindata-0.1.4/arfindata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 23:47:09.000000 arfindata-0.1.4/arfindata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-17 23:47:09.000000 arfindata-0.1.4/arfindata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-17 23:47:09.000000 arfindata-0.1.4/arfindata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 23:47:10.239333 arfindata-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      838 2023-04-17 23:35:48.000000 arfindata-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:49:40.528033 arfindata-0.1.5/
+-rw-rw-rw-   0        0        0     1088 2023-04-17 19:43:26.000000 arfindata-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      332 2023-04-18 20:49:40.527035 arfindata-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3842 2023-04-17 22:09:45.000000 arfindata-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 20:49:40.515066 arfindata-0.1.5/arfindata/
+-rw-rw-rw-   0        0        0     3855 2023-04-18 20:29:22.000000 arfindata-0.1.5/arfindata/ARdata.py
+-rw-rw-rw-   0        0        0       98 2023-04-17 19:35:47.000000 arfindata-0.1.5/arfindata/__init__.py
+-rw-rw-rw-   0        0        0     4200 2023-04-17 23:19:24.000000 arfindata-0.1.5/arfindata/sh.py
+-rw-rw-rw-   0        0        0     5096 2023-04-17 23:19:25.000000 arfindata-0.1.5/arfindata/sz.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:49:40.525040 arfindata-0.1.5/arfindata.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-04-18 20:49:39.000000 arfindata-0.1.5/arfindata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-04-18 20:49:40.000000 arfindata-0.1.5/arfindata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 20:49:39.000000 arfindata-0.1.5/arfindata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-18 20:49:40.000000 arfindata-0.1.5/arfindata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-18 20:49:40.000000 arfindata-0.1.5/arfindata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 20:49:40.528033 arfindata-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      838 2023-04-18 20:30:09.000000 arfindata-0.1.5/setup.py
```

### Comparing `arfindata-0.1.4/LICENSE.txt` & `arfindata-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arfindata-0.1.4/README.md` & `arfindata-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `arfindata-0.1.4/arfindata/ARdata.py` & `arfindata-0.1.5/arfindata/ARdata.py`

 * *Files 12% similar despite different names*

```diff
@@ -69,21 +69,43 @@
     def matches(self):
         txt = self.txt
         
         p_year= re.compile('.*?(\d{4}) .*?年度报告.*?')
         p_rev = re.compile('(?<=\n)营业总?收入（?(\w*?)?）?\s?\n?\s*([\d+,.]*)\s\n?')
         p_eps = re.compile('(?<=\n)基本每股收益（元/?／?\n?股）\s?\n?([-\d+,.]*)\s?\n?')
         
+        revenue=[]
+        eps=[]
+        
         year = [int(p_year.findall(text)[0]) for text in txt]
         dw = [p_rev.search(text).group(1) for text in txt ]
-        revenue=[float(p_rev.search(text).group(2).replace(',',''))*10000
-                 if w=="万元" or w=="万" 
-                 else float(p_rev.search(text).group(2).replace(',',''))
-                 for text,w in zip(txt,dw)]
-        eps=[p_eps.search(text).group(1) for text in txt]
+        for text,w in zip(txt,dw):
+            try:
+                if w=="万元" or w=="万":
+                    r=float(p_rev.search(text).group(2).replace(',',''))*10000
+                else:
+                    r=float(p_rev.search(text).group(2).replace(',',''))
+            except:
+                r='none'
+            revenue.append(r)
+                
+
+        for text in txt:
+            try:
+                e=p_eps.search(text).group(1)
+            except:
+                e='none'
+            eps.append(e)
+            
+        #revenue=[float(p_rev.search(text).group(2).replace(',',''))*10000
+        #         if w=="万元" or w=="万" 
+        #         else float(p_rev.search(text).group(2).replace(',',''))
+        #         for text,w in zip(txt,dw)]
+        #eps=[p_eps.search(text).group(1) for text in txt]
+        
         return [year,revenue,eps]
     
     def pdf_to_data(self):
         self.read_report()
         data = self.matches()
         df = pd.DataFrame({'Year':data[0],
                            'Revenue':data[1],
```

### Comparing `arfindata-0.1.4/arfindata/sh.py` & `arfindata-0.1.5/arfindata/sh.py`

 * *Files identical despite different names*

### Comparing `arfindata-0.1.4/arfindata/sz.py` & `arfindata-0.1.5/arfindata/sz.py`

 * *Files identical despite different names*

### Comparing `arfindata-0.1.4/setup.py` & `arfindata-0.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Package meta-data.
 NAME = 'arfindata'
 DESCRIPTION = "Python package for the aquisition and pre-treatment of China's listed companies' annual reports"
 URL = 'https://github.com/napstablook04/ARfindata'
 EMAIL = 'linkfr@163.com'    # 你的邮箱
 AUTHOR = 'linkfr'     # 你的名字
 REQUIRES_PYTHON = '>=3.6.0' # 项目支持的python版本
-VERSION = '0.1.4'           # 项目版本号
+VERSION = '0.1.5'           # 项目版本号
 REQUIRED = ['pandas','selenium','fitz','pdfplumber','requests']
 
 setup(
     name=NAME,
     version=VERSION,
     description=DESCRIPTION,
     author=AUTHOR,
```

