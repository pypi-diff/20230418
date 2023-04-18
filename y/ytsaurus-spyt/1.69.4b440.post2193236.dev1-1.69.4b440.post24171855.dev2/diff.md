# Comparing `tmp/ytsaurus-spyt-1.69.4b440.post2193236.dev1.tar.gz` & `tmp/ytsaurus-spyt-1.69.4b440.post24171855.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ytsaurus-spyt-1.69.4b440.post2193236.dev1.tar", last modified: Tue Apr 18 09:38:32 2023, max compression
+gzip compressed data, was "dist/ytsaurus-spyt-1.69.4b440.post24171855.dev2.tar", last modified: Tue Apr 18 10:21:21 2023, max compression
```

## Comparing `ytsaurus-spyt-1.69.4b440.post2193236.dev1.tar` & `ytsaurus-spyt-1.69.4b440.post24171855.dev2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-18 09:38:32.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-18 09:38:32.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/deps/
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-18 09:38:32.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/deps/bin/
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1192 2023-04-18 09:38:32.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/deps/bin/spark-discovery-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    11036 2023-04-18 09:38:32.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/deps/bin/spark-launch-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     2299 2023-04-18 09:38:32.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/deps/bin/spark-manage-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      760 2023-04-18 09:38:32.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/deps/bin/spark-shell-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1277 2023-04-18 09:38:32.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/deps/bin/spark-submit-yt
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-18 09:38:32.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/deps/jars/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)  1798367 2023-04-18 09:38:32.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/deps/jars/spark-yt-submit.jar
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-18 09:38:32.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/spyt/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       95 2023-02-22 20:15:30.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/spyt/__init__.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    16500 2023-04-10 10:41:56.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/spyt/client.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1106 2023-03-14 10:41:35.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/spyt/common.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     7434 2023-04-10 15:29:49.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/spyt/conf.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      326 2023-04-10 10:41:56.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/spyt/dependency_utils.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     3493 2023-03-18 23:30:06.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/spyt/enabler.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    35602 2023-04-18 09:31:33.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/spyt/standalone.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     9779 2023-03-14 10:41:35.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/spyt/submit.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     4003 2023-03-14 10:41:35.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/spyt/types.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    10300 2023-04-10 10:41:56.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/spyt/utils.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      179 2023-04-18 09:38:11.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/spyt/version.py
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-18 09:38:32.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/ytsaurus_spyt.egg-info/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      332 2023-04-18 09:38:32.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/ytsaurus_spyt.egg-info/PKG-INFO
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      540 2023-04-18 09:38:32.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/ytsaurus_spyt.egg-info/SOURCES.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        1 2023-04-18 09:38:32.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/ytsaurus_spyt.egg-info/dependency_links.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       40 2023-04-18 09:38:32.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/ytsaurus_spyt.egg-info/requires.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        5 2023-04-18 09:38:32.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/ytsaurus_spyt.egg-info/top_level.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      110 2023-02-22 20:15:30.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/MANIFEST.in
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1011 2023-04-10 10:41:56.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/setup.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      332 2023-04-18 09:38:32.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/PKG-INFO
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       38 2023-04-18 09:38:32.000000 ytsaurus-spyt-1.69.4b440.post2193236.dev1/setup.cfg
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1192 2023-04-18 10:21:20.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/spark-discovery-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    11036 2023-04-18 10:21:20.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/spark-launch-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     2299 2023-04-18 10:21:20.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/spark-manage-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      760 2023-04-18 10:21:20.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/spark-shell-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1277 2023-04-18 10:21:20.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/spark-submit-yt
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/jars/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)  1798367 2023-04-18 10:21:20.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/jars/spark-yt-submit.jar
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       95 2023-02-22 20:15:30.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/__init__.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    16500 2023-04-10 10:41:56.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/client.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1106 2023-03-14 10:41:35.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/common.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     7434 2023-04-10 15:29:49.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/conf.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      326 2023-04-10 10:41:56.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/dependency_utils.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     3493 2023-03-18 23:30:06.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/enabler.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    35663 2023-04-18 10:20:39.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/standalone.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     9779 2023-03-14 10:41:35.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/submit.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     4003 2023-03-14 10:41:35.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/types.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    10300 2023-04-10 10:41:56.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/utils.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      181 2023-04-18 10:20:58.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/version.py
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/ytsaurus_spyt.egg-info/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      333 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/ytsaurus_spyt.egg-info/PKG-INFO
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      540 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/ytsaurus_spyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        1 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/ytsaurus_spyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       40 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/ytsaurus_spyt.egg-info/requires.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        5 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/ytsaurus_spyt.egg-info/top_level.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      110 2023-02-22 20:15:30.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/MANIFEST.in
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1011 2023-04-10 10:41:56.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/setup.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      333 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/PKG-INFO
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       38 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/setup.cfg
```

### Comparing `ytsaurus-spyt-1.69.4b440.post2193236.dev1/deps/bin/spark-discovery-yt` & `ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/spark-discovery-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post2193236.dev1/deps/bin/spark-launch-yt` & `ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/spark-launch-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post2193236.dev1/deps/bin/spark-manage-yt` & `ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/spark-manage-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post2193236.dev1/deps/bin/spark-shell-yt` & `ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/spark-shell-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post2193236.dev1/deps/bin/spark-submit-yt` & `ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/spark-submit-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post2193236.dev1/deps/jars/spark-yt-submit.jar` & `ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/jars/spark-yt-submit.jar`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post2193236.dev1/spyt/client.py` & `ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/client.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post2193236.dev1/spyt/common.py` & `ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/common.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post2193236.dev1/spyt/conf.py` & `ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/conf.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post2193236.dev1/spyt/enabler.py` & `ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/enabler.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post2193236.dev1/spyt/standalone.py` & `ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/standalone.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,16 +213,17 @@
     _add_python_version(python_version, spark_base_args, client)
     _add_dedicated_driver_op_conf(spark_base_args, dedicated_driver_op)
     spark_env = _create_spark_env(client, spark_home)
 
     if local_files:
         remote_paths = {}
         new_spark_args = []
+        local_files_pattern = "[A-Za-z0-9]+:\/[^,]+(,[A-Za-z0-9]+:\/[^,]+)*" # Matches "FS:/..." path sequence
         for spark_arg in spark_args:
-            is_file_list = re.fullmatch("[A-Za-z0-9]+:\/[^,]+(,[A-Za-z0-9]+:\/[^,]+)*") # Matches "FS:/..." path sequence
+            is_file_list = re.fullmatch(local_files_pattern, spark_arg)
             if not is_file_list:
                 continue
             file_list = spark_arg.split(",")
             new_file_list = []
             for single_file in file_list:
                 if single_file.startswith('local:/'):
                     local_file_path = single_file[7:] # Drops prefix
```

### Comparing `ytsaurus-spyt-1.69.4b440.post2193236.dev1/spyt/submit.py` & `ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/submit.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post2193236.dev1/spyt/types.py` & `ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/types.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post2193236.dev1/spyt/utils.py` & `ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/utils.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post2193236.dev1/ytsaurus_spyt.egg-info/SOURCES.txt` & `ytsaurus-spyt-1.69.4b440.post24171855.dev2/ytsaurus_spyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post2193236.dev1/setup.py` & `ytsaurus-spyt-1.69.4b440.post24171855.dev2/setup.py`

 * *Files identical despite different names*

