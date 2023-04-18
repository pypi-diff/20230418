# Comparing `tmp/discuit-0.2.0.tar.gz` & `tmp/discuit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discuit-0.2.0.tar", last modified: Tue Apr 18 07:29:07 2023, max compression
+gzip compressed data, was "discuit-0.2.1.tar", last modified: Tue Apr 18 07:59:13 2023, max compression
```

## Comparing `discuit-0.2.0.tar` & `discuit-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-04-18 07:29:07.604421 discuit-0.2.0/
--rw-r--r--   0 doerte     (501) staff       (20)      454 2023-02-25 18:49:41.000000 discuit-0.2.0/CITATION.cff
--rw-r--r--   0 doerte     (501) staff       (20)    11359 2023-02-15 15:09:44.000000 discuit-0.2.0/LICENSE
--rw-r--r--   0 doerte     (501) staff       (20)       70 2023-02-15 15:09:44.000000 discuit-0.2.0/MANIFEST.in
--rw-r--r--   0 doerte     (501) staff       (20)       68 2023-02-25 18:49:41.000000 discuit-0.2.0/NOTICE
--rw-r--r--   0 doerte     (501) staff       (20)     7883 2023-04-18 07:29:07.604507 discuit-0.2.0/PKG-INFO
--rw-r--r--   0 doerte     (501) staff       (20)     6801 2023-04-18 07:21:17.000000 discuit-0.2.0/README.md
-drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-04-18 07:29:07.602930 discuit-0.2.0/discuit/
--rw-r--r--   0 doerte     (501) staff       (20)      192 2023-02-24 12:59:01.000000 discuit-0.2.0/discuit/__init__.py
--rw-r--r--   0 doerte     (501) staff       (20)    16746 2023-04-18 06:56:27.000000 discuit-0.2.0/discuit/run_discuit.py
-drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-04-18 07:29:07.604066 discuit-0.2.0/discuit.egg-info/
--rw-r--r--   0 doerte     (501) staff       (20)     7883 2023-04-18 07:29:07.000000 discuit-0.2.0/discuit.egg-info/PKG-INFO
--rw-r--r--   0 doerte     (501) staff       (20)      334 2023-04-18 07:29:07.000000 discuit-0.2.0/discuit.egg-info/SOURCES.txt
--rw-r--r--   0 doerte     (501) staff       (20)        1 2023-04-18 07:29:07.000000 discuit-0.2.0/discuit.egg-info/dependency_links.txt
--rw-r--r--   0 doerte     (501) staff       (20)        1 2023-02-25 18:42:43.000000 discuit-0.2.0/discuit.egg-info/not-zip-safe
--rw-r--r--   0 doerte     (501) staff       (20)      276 2023-04-18 07:29:07.000000 discuit-0.2.0/discuit.egg-info/requires.txt
--rw-r--r--   0 doerte     (501) staff       (20)        8 2023-04-18 07:29:07.000000 discuit-0.2.0/discuit.egg-info/top_level.txt
--rw-r--r--   0 doerte     (501) staff       (20)      376 2023-02-25 18:49:41.000000 discuit-0.2.0/pyproject.toml
--rw-r--r--   0 doerte     (501) staff       (20)     1897 2023-04-18 07:29:07.604899 discuit-0.2.0/setup.cfg
--rw-r--r--   0 doerte     (501) staff       (20)       87 2023-02-15 15:09:44.000000 discuit-0.2.0/setup.py
-drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-04-18 07:29:07.604190 discuit-0.2.0/tests/
--rw-r--r--   0 doerte     (501) staff       (20)      343 2023-02-24 12:59:25.000000 discuit-0.2.0/tests/test_my_module.py
+drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-04-18 07:59:13.367019 discuit-0.2.1/
+-rw-r--r--   0 doerte     (501) staff       (20)      454 2023-04-18 07:52:44.000000 discuit-0.2.1/CITATION.cff
+-rw-r--r--   0 doerte     (501) staff       (20)    11359 2023-02-15 15:09:44.000000 discuit-0.2.1/LICENSE
+-rw-r--r--   0 doerte     (501) staff       (20)       70 2023-02-15 15:09:44.000000 discuit-0.2.1/MANIFEST.in
+-rw-r--r--   0 doerte     (501) staff       (20)       68 2023-02-25 18:49:41.000000 discuit-0.2.1/NOTICE
+-rw-r--r--   0 doerte     (501) staff       (20)     7883 2023-04-18 07:59:13.367077 discuit-0.2.1/PKG-INFO
+-rw-r--r--   0 doerte     (501) staff       (20)     6801 2023-04-18 07:21:17.000000 discuit-0.2.1/README.md
+drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-04-18 07:59:13.365679 discuit-0.2.1/discuit/
+-rw-r--r--   0 doerte     (501) staff       (20)      192 2023-02-24 12:59:01.000000 discuit-0.2.1/discuit/__init__.py
+-rw-r--r--   0 doerte     (501) staff       (20)    16136 2023-04-18 07:50:10.000000 discuit-0.2.1/discuit/run_discuit.py
+drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-04-18 07:59:13.366666 discuit-0.2.1/discuit.egg-info/
+-rw-r--r--   0 doerte     (501) staff       (20)     7883 2023-04-18 07:59:13.000000 discuit-0.2.1/discuit.egg-info/PKG-INFO
+-rw-r--r--   0 doerte     (501) staff       (20)      334 2023-04-18 07:59:13.000000 discuit-0.2.1/discuit.egg-info/SOURCES.txt
+-rw-r--r--   0 doerte     (501) staff       (20)        1 2023-04-18 07:59:13.000000 discuit-0.2.1/discuit.egg-info/dependency_links.txt
+-rw-r--r--   0 doerte     (501) staff       (20)        1 2023-02-25 18:42:43.000000 discuit-0.2.1/discuit.egg-info/not-zip-safe
+-rw-r--r--   0 doerte     (501) staff       (20)      276 2023-04-18 07:59:13.000000 discuit-0.2.1/discuit.egg-info/requires.txt
+-rw-r--r--   0 doerte     (501) staff       (20)        8 2023-04-18 07:59:13.000000 discuit-0.2.1/discuit.egg-info/top_level.txt
+-rw-r--r--   0 doerte     (501) staff       (20)      376 2023-02-25 18:49:41.000000 discuit-0.2.1/pyproject.toml
+-rw-r--r--   0 doerte     (501) staff       (20)     1897 2023-04-18 07:59:13.367458 discuit-0.2.1/setup.cfg
+-rw-r--r--   0 doerte     (501) staff       (20)       87 2023-02-15 15:09:44.000000 discuit-0.2.1/setup.py
+drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-04-18 07:59:13.366782 discuit-0.2.1/tests/
+-rw-r--r--   0 doerte     (501) staff       (20)      343 2023-02-24 12:59:25.000000 discuit-0.2.1/tests/test_my_module.py
```

### Comparing `discuit-0.2.0/LICENSE` & `discuit-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discuit-0.2.0/PKG-INFO` & `discuit-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discuit
-Version: 0.2.0
+Version: 0.2.1
 Summary: Dynamic item set clustering UI tool: The goal of this package is to split datasets (e.g. words defined by several variables) into subsets that are as comparable as possible.
 Home-page: https://github.com/doerte/discuit-project
 Author: Dörte de Kok
 Author-email: me@doerte.eu
 Project-URL: Bug Tracker, https://github.com/doerte/discuit-project/issues
 Keywords: clustering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `discuit-0.2.0/README.md` & `discuit-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `discuit-0.2.0/discuit/run_discuit.py` & `discuit-0.2.1/discuit/run_discuit.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,37 +164,34 @@
     if (len(categorical_features) != 0) and (len(continuous_features) != 0):
         for k in cl_range:
             kproto = KPrototypes(n_clusters=k, max_iter=20)
             kproto.fit_predict(mark_array, categorical=categorical_features_idx)
             sil = metrics.silhouette_score(transformed_data, kproto.labels_, sample_size=1000)
             if sil > largest_sil[1]:
                 largest_sil = (k, sil)
-        check_sil(largest_sil[1])
         kproto_final = KPrototypes(n_clusters=largest_sil[0], max_iter=20)
 
         pred_cluster = kproto_final.fit_predict(mark_array, categorical=categorical_features_idx)
 
     elif (len(categorical_features) != 0) and (len(continuous_features) == 0):
         for k in cl_range:
             kmode = KModes(n_clusters=k, init="random", n_init=5)
             kmode.fit_predict(transformed_data)
             sil = metrics.silhouette_score(transformed_data, kmode.labels_, sample_size=1000)
             if sil > largest_sil[1]:
                 largest_sil = (k, sil)
-        check_sil(largest_sil)
         kmode_final = KModes(n_clusters=largest_sil[0], init="random", n_init=5)
         pred_cluster = kmode_final.fit_predict(transformed_data)
     else:
         for k in cl_range:
             km = KMeans(n_clusters=k, n_init=1, init='k-means++')
             km.fit_predict(transformed_data)
             sil = metrics.silhouette_score(transformed_data, km.labels_, sample_size=1000)
             if sil > largest_sil[1]:
                 largest_sil = (k, sil)
-        check_sil(largest_sil)
         km_final = KMeans(n_clusters=largest_sil[0], init='k-means++', n_init=1)
         pred_cluster = km_final.fit_predict(transformed_data)
 
     clusters: List[List[int]] = [[] for _ in range(largest_sil[0])]
 
     for i, cluster in enumerate(pred_cluster):
         clusters[cluster].append(i)
@@ -205,29 +202,14 @@
         cluster_new = []
         for item in cluster:
             cluster_new.append(transformed_data.iloc[item].name)
         final_clusters.append(cluster_new)
 
     return final_clusters
 
-def check_sil(sil):
-    while True:
-        if sil < 0.1:
-            txt = input("\nThe silhouette score is lower than 0.1. This indicates that your data might not be suitable "
-                "for clustering. Do you want to proceed (p) or abort (a)?")
-            if txt == "p":
-                print("yippieh, proceed")
-                break
-            if txt == "a":
-                print("oh no, abort")
-                break
-            print("nothing useful entered :( ")
-        else:
-            break
-
 def divide_in_sets(clusters, output_sets):
     # divide clusters evenly amongst desired sets
     for cluster in clusters:
         for item in cluster:
             output_sets[output_sets.index(min(output_sets, key=len))].append(item)
```

### Comparing `discuit-0.2.0/discuit.egg-info/PKG-INFO` & `discuit-0.2.1/discuit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discuit
-Version: 0.2.0
+Version: 0.2.1
 Summary: Dynamic item set clustering UI tool: The goal of this package is to split datasets (e.g. words defined by several variables) into subsets that are as comparable as possible.
 Home-page: https://github.com/doerte/discuit-project
 Author: Dörte de Kok
 Author-email: me@doerte.eu
 Project-URL: Bug Tracker, https://github.com/doerte/discuit-project/issues
 Keywords: clustering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `discuit-0.2.0/setup.cfg` & `discuit-0.2.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 keywords = clustering
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = discuit
 project_urls = 
 	Bug Tracker = https://github.com/doerte/discuit-project/issues
 url = https://github.com/doerte/discuit-project
-version = 0.2.0
+version = 0.2.1
 
 [options]
 zip_safe = False
 python_requires = >=3.7
 include_package_data = True
 packages = find:
 install_requires =
```

