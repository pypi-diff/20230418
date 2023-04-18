# Comparing `tmp/phope-0.0.4.tar.gz` & `tmp/phope-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phope-0.0.4.tar", last modified: Tue Feb 28 00:30:46 2023, max compression
+gzip compressed data, was "phope-0.0.5.tar", last modified: Tue Apr 18 03:08:24 2023, max compression
```

## Comparing `phope-0.0.4.tar` & `phope-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-02-28 00:30:46.965911 phope-0.0.4/
--rw-r--r--   0 yt        (1000) yt        (1000)     3147 2023-02-28 00:30:46.965911 phope-0.0.4/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)     2637 2023-02-28 00:29:29.000000 phope-0.0.4/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-02-28 00:30:46.965911 phope-0.0.4/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      921 2023-02-28 00:28:45.000000 phope-0.0.4/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-02-28 00:30:46.949265 phope-0.0.4/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-02-28 00:30:46.949265 phope-0.0.4/src/phope.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     3147 2023-02-28 00:30:46.000000 phope-0.0.4/src/phope.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      199 2023-02-28 00:30:46.000000 phope-0.0.4/src/phope.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-02-28 00:30:46.000000 phope-0.0.4/src/phope.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-02-28 00:30:46.000000 phope-0.0.4/src/phope.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        6 2023-02-28 00:30:46.000000 phope-0.0.4/src/phope.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     2381 2023-02-28 00:27:40.000000 phope-0.0.4/src/phope.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-04-18 03:08:24.441402 phope-0.0.5/
+-rw-r--r--   0 yt        (1000) yt        (1000)     3147 2023-04-18 03:08:24.438990 phope-0.0.5/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)     2637 2023-02-28 00:29:29.000000 phope-0.0.5/README.md
+-rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-04-18 03:08:24.441402 phope-0.0.5/setup.cfg
+-rw-r--r--   0 yt        (1000) yt        (1000)      921 2023-04-18 03:07:53.000000 phope-0.0.5/setup.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-04-18 03:08:24.431829 phope-0.0.5/src/
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-04-18 03:08:24.438990 phope-0.0.5/src/phope.egg-info/
+-rw-r--r--   0 yt        (1000) yt        (1000)     3147 2023-04-18 03:08:23.000000 phope-0.0.5/src/phope.egg-info/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)      199 2023-04-18 03:08:23.000000 phope-0.0.5/src/phope.egg-info/SOURCES.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-04-18 03:08:23.000000 phope-0.0.5/src/phope.egg-info/dependency_links.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-04-18 03:08:23.000000 phope-0.0.5/src/phope.egg-info/entry_points.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        6 2023-04-18 03:08:23.000000 phope-0.0.5/src/phope.egg-info/top_level.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)     2383 2023-04-18 03:04:36.000000 phope-0.0.5/src/phope.py
```

### Comparing `phope-0.0.4/PKG-INFO` & `phope-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phope
-Version: 0.0.4
+Version: 0.0.5
 Summary: universal biomarker prediction tool
 Home-page: https://github.com/ytakefuji/patient
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/patient
 Platform: UNKNOWN
```

### Comparing `phope-0.0.4/README.md` & `phope-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `phope-0.0.4/setup.py` & `phope-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="phope",
-    version="0.0.4",
+    version="0.0.5",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="universal biomarker prediction tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ytakefuji/patient",
     project_urls={
```

### Comparing `phope-0.0.4/src/phope.egg-info/PKG-INFO` & `phope-0.0.5/src/phope.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phope
-Version: 0.0.4
+Version: 0.0.5
 Summary: universal biomarker prediction tool
 Home-page: https://github.com/ytakefuji/patient
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/patient
 Platform: UNKNOWN
```

### Comparing `phope-0.0.4/src/phope.py` & `phope-0.0.5/src/phope.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,14 +56,14 @@
  print(model_m2.coefficients)
  print(m2+': ',round(y2,3))
  d[m2][days]=y2
  ax2.plot(X[0:days],d[m2][0:days],linestyle='None',marker='o')
  ax2.plot(X[days],d[m2][days],linestyle='None',color='r',marker='o')
  ax2.plot(X[0:days+1],model_m2(X[0:days+1]),linestyle='--',color='k')
  ax2.legend([m2],loc=3,bbox_to_anchor= (0.7, 0.6))
- plt.text(20,90,'r2_'+m1+': '+str(round(m1_error,3)))
- plt.text(70,90,'degree: '+str(degree1))
- plt.text(20,60,'r2_'+m2+': '+str(round(m2_error,3)))
- plt.text(70,60,'degree: '+str(degree2))
+ plt.text(20,50,'r2_'+m1+': '+str(round(m1_error,2)))
+ plt.text(100,50,'degree: '+str(degree1))
+ plt.text(20,70,'r2_'+m2+': '+str(round(m2_error,2)))
+ plt.text(100,70,'degree: '+str(degree2))
  plt.savefig(m1+'_'+m2+'.png',bbox_inches='tight')
  plt.show()
 main()
```

