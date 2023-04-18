# Comparing `tmp/atmoswing-vigicrues-1.0.0.tar.gz` & `tmp/atmoswing-vigicrues-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atmoswing-vigicrues-1.0.0.tar", last modified: Mon Apr 17 10:05:39 2023, max compression
+gzip compressed data, was "atmoswing-vigicrues-1.0.1.tar", last modified: Tue Apr 18 16:26:33 2023, max compression
```

## Comparing `atmoswing-vigicrues-1.0.0.tar` & `atmoswing-vigicrues-1.0.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:39.686263 atmoswing-vigicrues-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-17 10:05:39.686263 atmoswing-vigicrues-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-17 10:05:39.686263 atmoswing-vigicrues-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:39.674262 atmoswing-vigicrues-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:39.674262 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:39.682263 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/disseminations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/disseminations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/disseminations/dissemination.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:39.682263 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/postactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/postactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/postactions/export_bdapbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/postactions/export_prv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/postactions/postaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:39.682263 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/preactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/preactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/preactions/download_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/preactions/preaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/preactions/transform_ecmwf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/preactions/transform_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:39.678263 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-17 10:05:39.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-17 10:05:39.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 10:05:39.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-17 10:05:39.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-17 10:05:39.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:39.686263 atmoswing-vigicrues-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/tests/test_download_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/tests/test_export_bdapbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/tests/test_export_prv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:33.590480 atmoswing-vigicrues-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-18 16:26:33.590480 atmoswing-vigicrues-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-18 16:26:33.590480 atmoswing-vigicrues-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:33.586480 atmoswing-vigicrues-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:33.586480 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:33.586480 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/disseminations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/disseminations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/disseminations/dissemination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:33.586480 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/postactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/postactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/postactions/export_bdapbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/postactions/export_prv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/postactions/postaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:33.590480 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/download_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/preaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/transform_ecmwf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/transform_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:33.586480 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-18 16:26:33.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-18 16:26:33.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:26:33.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-18 16:26:33.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 16:26:33.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:33.590480 atmoswing-vigicrues-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/tests/test_download_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/tests/test_export_bdapbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/tests/test_export_prv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/tests/test_utils.py
```

### Comparing `atmoswing-vigicrues-1.0.0/LICENSE` & `atmoswing-vigicrues-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.0/pyproject.toml` & `atmoswing-vigicrues-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atmoswing-vigicrues"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Pascal Horton", email="pascal.horton@terranum.ch" },
 ]
 description = "Package to integrate AtmoSwing in the Vigicrues network."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/__init__.py` & `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/__init__.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/__main__.py` & `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/__main__.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/controller.py` & `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,14 @@
             else:
                 print("AtmoSwing Forecaster a été exécuté avec succès.")
         except Exception as e:
             print(f"Exception lors de l'exécution d'AtmoSwing Forecaster: {e}")
 
     def _build_atmoswing_cmd(self, options):
         now_str = self.date.strftime("%Y%m%d%H")
-        proxy = ''
         cmd = []
 
         if 'atmoswing_path' not in options or not options['atmoswing_path']:
             cmd.append("atmoswing-forecaster")
         else:
             cmd.append(options['atmoswing_path'])
```

### Comparing `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/disseminations/dissemination.py` & `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/disseminations/dissemination.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py` & `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/exceptions.py` & `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/exceptions.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/options.py` & `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/options.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/postactions/export_bdapbp.py` & `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/postactions/export_bdapbp.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/postactions/export_prv.py` & `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/postactions/export_prv.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/postactions/postaction.py` & `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/postactions/postaction.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/preactions/download_gfs.py` & `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/download_gfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
                     url = f"https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_{resol}." \
                           f"pl?file=gfs.t{forecast_hour}z.{sub_product}.{resol}." \
                           f"f{lead_time_str}&{levels}var_{variable.upper()}=on&" \
                           f"{subregion}&dir=%2Fgfs.{forecast_date}%2F" \
                           f"{forecast_hour}%2Fatmos"
 
-                    file_name = f'{forecast_date}{forecast_hour}.NWS_GFS_Forecast.' \
+                    file_name = f'{forecast_date}{forecast_hour}.NWS_GFS.' \
                                 f'{variable.lower()}.{lead_time_str}.grib2'
 
                     local_path = self._get_local_path(date_ref)
                     file_path = local_path / file_name
 
                     if file_path.exists():
                         continue
```

### Comparing `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py` & `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py`

 * *Files 15% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             else:
                 self.proxy_port = 1080
         else:
             self.proxy_host = None
 
         super().__init__()
 
-    def run(self, date):
+    def run(self, date) -> bool:
         """
         Exécution de la récupération par SFTP.
 
         Parameters
         ----------
         date : datetime
             Date de la prévision.
@@ -103,28 +103,38 @@
             if sftp:
                 sftp.close()
             if transport:
                 transport.close()
 
         except paramiko.ssh_exception.PasswordRequiredException as e:
             print(f"SFTP PasswordRequiredException {e}")
+            return False
         except paramiko.ssh_exception.BadAuthenticationType as e:
             print(f"SFTP BadAuthenticationType {e}")
+            return False
         except paramiko.ssh_exception.AuthenticationException as e:
             print(f"SFTP AuthenticationException {e}")
+            return False
         except paramiko.ssh_exception.ChannelException as e:
             print(f"SFTP ChannelException {e}")
+            return False
         except paramiko.ssh_exception.ProxyCommandFailure as e:
             print(f"SFTP ProxyCommandFailure {e}")
+            return False
         except paramiko.ssh_exception.SSHException as e:
             print(f"SFTP SSHException {e}")
+            return False
         except FileNotFoundError as e:
             print(f"SFTP FileNotFoundError {e}")
+            return False
         except Exception as e:
-            print(f"La diffusion SFTP a échoué ({e}).")
+            print(f"Le rapatriement des données par SFTP a échoué ({e}).")
+            return False
+
+        return True
 
     @staticmethod
     def _chdir_or_mkdir(dir_path, sftp):
         try:
             sftp.chdir(dir_path)
         except IOError:
             sftp.mkdir(dir_path)
```

### Comparing `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/preactions/transform_ecmwf.py` & `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/transform_ecmwf.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         Vrai (True) en cas de succès, faux (False) autrement.
         """
 
         input_dir = self._get_input_dir(date)
         forecast_date, forecast_hour = self._format_forecast_date(date)
 
         for variable in self.variables:
-            file_name_pattern = f'{forecast_date}{forecast_hour}.ECMWF_IFS_Forecast.' \
+            file_name_pattern = f'{forecast_date}{forecast_hour}.ECMWF_IFS.' \
                                 f'{variable.lower()}.*.grib2'
 
             input_files = sorted(input_dir.glob(file_name_pattern))
 
             if len(input_files) == 0:
                 return False
```

### Comparing `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/preactions/transform_gfs.py` & `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/transform_gfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         Vrai (True) en cas de succès, faux (False) autrement.
         """
 
         input_dir = self._get_input_dir(date)
         forecast_date, forecast_hour = self._format_forecast_date(date)
 
         for variable in self.variables:
-            file_name_pattern = f'{forecast_date}{forecast_hour}.NWS_GFS_Forecast.' \
+            file_name_pattern = f'{forecast_date}{forecast_hour}.NWS_GFS.' \
                                 f'{variable.lower()}.*.grib2'
 
             input_files = sorted(input_dir.glob(file_name_pattern))
 
             if len(input_files) == 0:
                 return False
```

### Comparing `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/utils.py` & `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/utils.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues.egg-info/SOURCES.txt` & `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.0/tests/test_controller.py` & `atmoswing-vigicrues-1.0.1/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.0/tests/test_download_gfs.py` & `atmoswing-vigicrues-1.0.1/tests/test_download_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.0/tests/test_exceptions.py` & `atmoswing-vigicrues-1.0.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.0/tests/test_export_bdapbp.py` & `atmoswing-vigicrues-1.0.1/tests/test_export_bdapbp.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.0/tests/test_export_prv.py` & `atmoswing-vigicrues-1.0.1/tests/test_export_prv.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.0/tests/test_options.py` & `atmoswing-vigicrues-1.0.1/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.0/tests/test_utils.py` & `atmoswing-vigicrues-1.0.1/tests/test_utils.py`

 * *Files identical despite different names*

