# Comparing `tmp/globalsearch-0.2.2.tar.gz` & `tmp/globalsearch-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globalsearch-0.2.2.tar", last modified: Thu Apr 13 18:09:31 2023, max compression
+gzip compressed data, was "globalsearch-0.2.3.tar", last modified: Tue Apr 18 20:16:38 2023, max compression
```

## Comparing `globalsearch-0.2.2.tar` & `globalsearch-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-13 18:09:31.706205 globalsearch-0.2.2/
--rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-13 18:09:31.706271 globalsearch-0.2.2/PKG-INFO
--rw-r--r--   0 weiju      (501) staff       (20)      252 2022-12-13 19:27:00.000000 globalsearch-0.2.2/README.md
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-13 18:09:31.701862 globalsearch-0.2.2/bin/
--rwxr--r--   0 weiju      (501) staff       (20)      533 2023-01-09 18:49:49.000000 globalsearch-0.2.2/bin/gs_prepare
--rwxr-xr-x   0 weiju      (501) staff       (20)     1268 2023-02-09 22:31:19.000000 globalsearch-0.2.2/bin/gs_submit
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-13 18:09:31.701044 globalsearch-0.2.2/globalsearch/
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-13 18:09:31.703296 globalsearch-0.2.2/globalsearch/control/
--rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-10 16:54:29.000000 globalsearch-0.2.2/globalsearch/control/__init__.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     6635 2023-02-24 18:56:53.000000 globalsearch-0.2.2/globalsearch/control/gs_prepare.py
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-13 18:09:31.705989 globalsearch-0.2.2/globalsearch/rnaseq/
--rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-09 00:21:15.000000 globalsearch-0.2.2/globalsearch/rnaseq/__init__.py
--rw-r--r--   0 weiju      (501) staff       (20)     7034 2023-03-21 18:06:55.000000 globalsearch-0.2.2/globalsearch/rnaseq/find_files.py
--rw-r--r--   0 weiju      (501) staff       (20)     2978 2023-04-07 20:18:38.000000 globalsearch-0.2.2/globalsearch/rnaseq/index_star.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     2130 2023-02-09 22:31:19.000000 globalsearch-0.2.2/globalsearch/rnaseq/make_kallisto_job.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     3120 2023-04-07 20:18:38.000000 globalsearch-0.2.2/globalsearch/rnaseq/make_star_idx_job.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     6330 2023-04-11 22:07:15.000000 globalsearch-0.2.2/globalsearch/rnaseq/make_star_salmon_job.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     1725 2023-04-13 18:08:53.000000 globalsearch-0.2.2/globalsearch/rnaseq/post_star_salmon.py
--rwxr--r--   0 weiju      (501) staff       (20)     5497 2023-01-06 20:10:59.000000 globalsearch-0.2.2/globalsearch/rnaseq/run_kallisto.py
--rw-r--r--   0 weiju      (501) staff       (20)    14661 2023-03-10 21:10:17.000000 globalsearch-0.2.2/globalsearch/rnaseq/run_spladder.py
--rwxr-xr-x   0 weiju      (501) staff       (20)    13278 2023-04-11 22:07:15.000000 globalsearch-0.2.2/globalsearch/rnaseq/run_star_salmon.py
--rw-r--r--   0 weiju      (501) staff       (20)     3664 2023-03-21 18:06:55.000000 globalsearch-0.2.2/globalsearch/rnaseq/trim_galore.py
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-13 18:09:31.703026 globalsearch-0.2.2/globalsearch.egg-info/
--rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-13 18:09:31.000000 globalsearch-0.2.2/globalsearch.egg-info/PKG-INFO
--rw-r--r--   0 weiju      (501) staff       (20)      751 2023-04-13 18:09:31.000000 globalsearch-0.2.2/globalsearch.egg-info/SOURCES.txt
--rw-r--r--   0 weiju      (501) staff       (20)        1 2023-04-13 18:09:31.000000 globalsearch-0.2.2/globalsearch.egg-info/dependency_links.txt
--rw-r--r--   0 weiju      (501) staff       (20)        1 2022-12-15 20:31:36.000000 globalsearch-0.2.2/globalsearch.egg-info/not-zip-safe
--rw-r--r--   0 weiju      (501) staff       (20)       25 2023-04-13 18:09:31.000000 globalsearch-0.2.2/globalsearch.egg-info/requires.txt
--rw-r--r--   0 weiju      (501) staff       (20)       13 2023-04-13 18:09:31.000000 globalsearch-0.2.2/globalsearch.egg-info/top_level.txt
--rw-r--r--   0 weiju      (501) staff       (20)       67 2023-04-13 18:09:31.706565 globalsearch-0.2.2/setup.cfg
--rw-r--r--   0 weiju      (501) staff       (20)     1611 2023-04-13 18:09:29.000000 globalsearch-0.2.2/setup.py
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-18 20:16:38.823653 globalsearch-0.2.3/
+-rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-18 20:16:38.823737 globalsearch-0.2.3/PKG-INFO
+-rw-r--r--   0 weiju      (501) staff       (20)      252 2022-12-13 19:27:00.000000 globalsearch-0.2.3/README.md
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-18 20:16:38.818825 globalsearch-0.2.3/bin/
+-rwxr--r--   0 weiju      (501) staff       (20)      533 2023-01-09 18:49:49.000000 globalsearch-0.2.3/bin/gs_prepare
+-rwxr-xr-x   0 weiju      (501) staff       (20)     1268 2023-02-09 22:31:19.000000 globalsearch-0.2.3/bin/gs_submit
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-18 20:16:38.817853 globalsearch-0.2.3/globalsearch/
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-18 20:16:38.820182 globalsearch-0.2.3/globalsearch/control/
+-rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-10 16:54:29.000000 globalsearch-0.2.3/globalsearch/control/__init__.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     6635 2023-02-24 18:56:53.000000 globalsearch-0.2.3/globalsearch/control/gs_prepare.py
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-18 20:16:38.823393 globalsearch-0.2.3/globalsearch/rnaseq/
+-rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-09 00:21:15.000000 globalsearch-0.2.3/globalsearch/rnaseq/__init__.py
+-rw-r--r--   0 weiju      (501) staff       (20)     7239 2023-04-18 20:14:08.000000 globalsearch-0.2.3/globalsearch/rnaseq/find_files.py
+-rw-r--r--   0 weiju      (501) staff       (20)     2978 2023-04-07 20:18:38.000000 globalsearch-0.2.3/globalsearch/rnaseq/index_star.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     2130 2023-02-09 22:31:19.000000 globalsearch-0.2.3/globalsearch/rnaseq/make_kallisto_job.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     3120 2023-04-07 20:18:38.000000 globalsearch-0.2.3/globalsearch/rnaseq/make_star_idx_job.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     6330 2023-04-11 22:07:15.000000 globalsearch-0.2.3/globalsearch/rnaseq/make_star_salmon_job.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     1725 2023-04-13 18:08:53.000000 globalsearch-0.2.3/globalsearch/rnaseq/post_star_salmon.py
+-rwxr--r--   0 weiju      (501) staff       (20)     5497 2023-01-06 20:10:59.000000 globalsearch-0.2.3/globalsearch/rnaseq/run_kallisto.py
+-rw-r--r--   0 weiju      (501) staff       (20)    14661 2023-03-10 21:10:17.000000 globalsearch-0.2.3/globalsearch/rnaseq/run_spladder.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)    13278 2023-04-11 22:07:15.000000 globalsearch-0.2.3/globalsearch/rnaseq/run_star_salmon.py
+-rw-r--r--   0 weiju      (501) staff       (20)     3664 2023-03-21 18:06:55.000000 globalsearch-0.2.3/globalsearch/rnaseq/trim_galore.py
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-18 20:16:38.819908 globalsearch-0.2.3/globalsearch.egg-info/
+-rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-18 20:16:38.000000 globalsearch-0.2.3/globalsearch.egg-info/PKG-INFO
+-rw-r--r--   0 weiju      (501) staff       (20)      751 2023-04-18 20:16:38.000000 globalsearch-0.2.3/globalsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 weiju      (501) staff       (20)        1 2023-04-18 20:16:38.000000 globalsearch-0.2.3/globalsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 weiju      (501) staff       (20)        1 2022-12-15 20:31:36.000000 globalsearch-0.2.3/globalsearch.egg-info/not-zip-safe
+-rw-r--r--   0 weiju      (501) staff       (20)       25 2023-04-18 20:16:38.000000 globalsearch-0.2.3/globalsearch.egg-info/requires.txt
+-rw-r--r--   0 weiju      (501) staff       (20)       13 2023-04-18 20:16:38.000000 globalsearch-0.2.3/globalsearch.egg-info/top_level.txt
+-rw-r--r--   0 weiju      (501) staff       (20)       67 2023-04-18 20:16:38.824036 globalsearch-0.2.3/setup.cfg
+-rw-r--r--   0 weiju      (501) staff       (20)     1611 2023-04-18 20:15:22.000000 globalsearch-0.2.3/setup.py
```

### Comparing `globalsearch-0.2.2/PKG-INFO` & `globalsearch-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globalsearch
-Version: 0.2.2
+Version: 0.2.3
 Summary: globalsearch is a collection of Python modules and command tools for the Global Search pipeline.
 Home-page: https://github.com/baliga-lab/Global_Search
 Author: Wei-ju Wu
 Author-email: weiju.wu@gmail.com
 Maintainer: Wei-ju Wu
 Maintainer-email: weiju.wu@gmail.com
 License: LGPL V3
```

### Comparing `globalsearch-0.2.2/bin/gs_prepare` & `globalsearch-0.2.3/bin/gs_prepare`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.2/bin/gs_submit` & `globalsearch-0.2.3/bin/gs_submit`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.2/globalsearch/control/gs_prepare.py` & `globalsearch-0.2.3/globalsearch/control/gs_prepare.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.2/globalsearch/rnaseq/find_files.py` & `globalsearch-0.2.3/globalsearch/rnaseq/find_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,19 +51,22 @@
     result = []
     filesys = rootfs.opendir(data_folder)
     for pat in patterns:
         templ = jinja2.Template(pat)
         patmatch = defaultdict(list)
         for read_num in [1, 2]:
             # keep "pairnum" for legacy reasons
-            pattern = templ.render({'pairnum': read_num, 'readnum': read_num})
-            pattern = fs.path.combine('/**', pattern)
+            pattern_replace_readnum = templ.render({'pairnum': read_num, 'readnum': read_num})
+            pattern = fs.path.combine('/**', pattern_replace_readnum)
             #print("SEARCHING PATTERN: '%s'" % pattern, flush=True)
-            for match in filesys.glob(pattern):
-                patmatch[read_num].append(fs.path.combine(data_folder, match.path))
+            if pattern_replace_readnum == pat and read_num == 2:  # no readnum provided in pattern
+                patmatch[read_num].append(None)
+            else:
+                for match in filesys.glob(pattern):
+                    patmatch[read_num].append(fs.path.combine(data_folder, match.path))
         #print("PATMATCH: ", patmatch)
         try:
             first = patmatch[1][0]
         except:
             # no match -> skip this pattern
             continue
         try:
```

### Comparing `globalsearch-0.2.2/globalsearch/rnaseq/index_star.py` & `globalsearch-0.2.3/globalsearch/rnaseq/index_star.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.2/globalsearch/rnaseq/make_kallisto_job.py` & `globalsearch-0.2.3/globalsearch/rnaseq/make_kallisto_job.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.2/globalsearch/rnaseq/make_star_idx_job.py` & `globalsearch-0.2.3/globalsearch/rnaseq/make_star_idx_job.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.2/globalsearch/rnaseq/make_star_salmon_job.py` & `globalsearch-0.2.3/globalsearch/rnaseq/make_star_salmon_job.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.2/globalsearch/rnaseq/post_star_salmon.py` & `globalsearch-0.2.3/globalsearch/rnaseq/post_star_salmon.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.2/globalsearch/rnaseq/run_kallisto.py` & `globalsearch-0.2.3/globalsearch/rnaseq/run_kallisto.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.2/globalsearch/rnaseq/run_spladder.py` & `globalsearch-0.2.3/globalsearch/rnaseq/run_spladder.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.2/globalsearch/rnaseq/run_star_salmon.py` & `globalsearch-0.2.3/globalsearch/rnaseq/run_star_salmon.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.2/globalsearch/rnaseq/trim_galore.py` & `globalsearch-0.2.3/globalsearch/rnaseq/trim_galore.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.2/globalsearch.egg-info/PKG-INFO` & `globalsearch-0.2.3/globalsearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globalsearch
-Version: 0.2.2
+Version: 0.2.3
 Summary: globalsearch is a collection of Python modules and command tools for the Global Search pipeline.
 Home-page: https://github.com/baliga-lab/Global_Search
 Author: Wei-ju Wu
 Author-email: weiju.wu@gmail.com
 Maintainer: Wei-ju Wu
 Maintainer-email: weiju.wu@gmail.com
 License: LGPL V3
```

### Comparing `globalsearch-0.2.2/globalsearch.egg-info/SOURCES.txt` & `globalsearch-0.2.3/globalsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.2/setup.py` & `globalsearch-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 NAME = 'globalsearch'
 PACKAGES = ['globalsearch.rnaseq', 'globalsearch.control']
 DESCRIPTION = 'globalsearch is a collection of Python modules and command tools for the Global Search pipeline.'
 LICENSE = 'LGPL V3'
 URI = 'https://github.com/baliga-lab/Global_Search'
 AUTHOR = 'Wei-ju Wu'
-VERSION = '0.2.2'
+VERSION = '0.2.3'
 
 KEYWORDS = ['global search', 'coral reef']
 
 # See trove classifiers
 # https://testpypi.python.org/pypi?%3Aaction=list_classifiers
 
 CLASSIFIERS = [
```

