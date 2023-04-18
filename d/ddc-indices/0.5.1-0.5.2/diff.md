# Comparing `tmp/ddc-indices-0.5.1.tar.gz` & `tmp/ddc-indices-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddc-indices-0.5.1.tar", last modified: Mon Apr  3 13:39:03 2023, max compression
+gzip compressed data, was "ddc-indices-0.5.2.tar", last modified: Tue Apr 18 18:55:28 2023, max compression
```

## Comparing `ddc-indices-0.5.1.tar` & `ddc-indices-0.5.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:39:03.823534 ddc-indices-0.5.1/
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-04-03 11:17:54.000000 ddc-indices-0.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1421 2023-04-03 13:39:03.823534 ddc-indices-0.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1014 2023-04-03 13:20:02.000000 ddc-indices-0.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:39:03.823534 ddc-indices-0.5.1/ddc_indices/
--rw-rw-rw-   0 root         (0) root         (0)      122 2023-04-03 11:17:54.000000 ddc-indices-0.5.1/ddc_indices/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-03 13:20:02.000000 ddc-indices-0.5.1/ddc_indices/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    11160 2023-04-03 11:17:54.000000 ddc-indices-0.5.1/ddc_indices/compute.py
--rw-rw-rw-   0 root         (0) root         (0)    26052 2023-04-03 11:17:54.000000 ddc-indices-0.5.1/ddc_indices/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3749 2023-04-03 11:17:54.000000 ddc-indices-0.5.1/ddc_indices/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2023-04-03 11:17:54.000000 ddc-indices-0.5.1/ddc_indices/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     8419 2023-04-03 11:17:54.000000 ddc-indices-0.5.1/ddc_indices/eto.py
--rw-rw-rw-   0 root         (0) root         (0)    30095 2023-04-03 11:17:54.000000 ddc-indices-0.5.1/ddc_indices/indices.py
--rw-rw-rw-   0 root         (0) root         (0)     3002 2023-04-03 11:17:54.000000 ddc-indices-0.5.1/ddc_indices/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     6952 2023-04-03 11:17:54.000000 ddc-indices-0.5.1/ddc_indices/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:39:03.823534 ddc-indices-0.5.1/ddc_indices.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1421 2023-04-03 13:39:03.000000 ddc-indices-0.5.1/ddc_indices.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      436 2023-04-03 13:39:03.000000 ddc-indices-0.5.1/ddc_indices.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-03 13:39:03.000000 ddc-indices-0.5.1/ddc_indices.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2023-04-03 13:39:03.000000 ddc-indices-0.5.1/ddc_indices.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-03 13:39:03.000000 ddc-indices-0.5.1/ddc_indices.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      737 2023-04-03 13:20:02.000000 ddc-indices-0.5.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-03 13:39:03.823534 ddc-indices-0.5.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 18:55:28.709706 ddc-indices-0.5.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-04-03 11:17:54.000000 ddc-indices-0.5.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-04-18 18:55:28.699706 ddc-indices-0.5.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1014 2023-04-03 13:20:02.000000 ddc-indices-0.5.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 18:55:28.699706 ddc-indices-0.5.2/ddc_indices/
+-rw-rw-rw-   0 root         (0) root         (0)      122 2023-04-03 11:17:54.000000 ddc-indices-0.5.2/ddc_indices/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-18 18:34:49.000000 ddc-indices-0.5.2/ddc_indices/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11160 2023-04-03 11:17:54.000000 ddc-indices-0.5.2/ddc_indices/compute.py
+-rw-rw-rw-   0 root         (0) root         (0)    26052 2023-04-03 11:17:54.000000 ddc-indices-0.5.2/ddc_indices/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3749 2023-04-03 11:17:54.000000 ddc-indices-0.5.2/ddc_indices/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2023-04-03 11:17:54.000000 ddc-indices-0.5.2/ddc_indices/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     8419 2023-04-03 11:17:54.000000 ddc-indices-0.5.2/ddc_indices/eto.py
+-rw-rw-rw-   0 root         (0) root         (0)    29996 2023-04-18 18:34:49.000000 ddc-indices-0.5.2/ddc_indices/indices.py
+-rw-rw-rw-   0 root         (0) root         (0)     3002 2023-04-03 11:17:54.000000 ddc-indices-0.5.2/ddc_indices/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     6952 2023-04-03 11:17:54.000000 ddc-indices-0.5.2/ddc_indices/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 18:55:28.699706 ddc-indices-0.5.2/ddc_indices.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-04-18 18:55:28.000000 ddc-indices-0.5.2/ddc_indices.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      436 2023-04-18 18:55:28.000000 ddc-indices-0.5.2/ddc_indices.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 18:55:28.000000 ddc-indices-0.5.2/ddc_indices.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2023-04-18 18:55:28.000000 ddc-indices-0.5.2/ddc_indices.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-18 18:55:28.000000 ddc-indices-0.5.2/ddc_indices.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      737 2023-04-18 18:34:49.000000 ddc-indices-0.5.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 18:55:28.709706 ddc-indices-0.5.2/setup.cfg
```

### Comparing `ddc-indices-0.5.1/LICENSE` & `ddc-indices-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ddc-indices-0.5.1/PKG-INFO` & `ddc-indices-0.5.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddc-indices
-Version: 0.5.1
+Version: 0.5.2
 Summary: Package for calculating meteorological indices
 Author-email: Balint Alfoldy <balint.alfoldy@lechnerkozpont.hu>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ddc-indices-0.5.1/README.md` & `ddc-indices-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `ddc-indices-0.5.1/ddc_indices/compute.py` & `ddc-indices-0.5.2/ddc_indices/compute.py`

 * *Files identical despite different names*

### Comparing `ddc-indices-0.5.1/ddc_indices/config.py` & `ddc-indices-0.5.2/ddc_indices/config.py`

 * *Files identical despite different names*

### Comparing `ddc-indices-0.5.1/ddc_indices/constants.py` & `ddc-indices-0.5.2/ddc_indices/constants.py`

 * *Files identical despite different names*

### Comparing `ddc-indices-0.5.1/ddc_indices/errors.py` & `ddc-indices-0.5.2/ddc_indices/errors.py`

 * *Files identical despite different names*

### Comparing `ddc-indices-0.5.1/ddc_indices/eto.py` & `ddc-indices-0.5.2/ddc_indices/eto.py`

 * *Files identical despite different names*

### Comparing `ddc-indices-0.5.1/ddc_indices/indices.py` & `ddc-indices-0.5.2/ddc_indices/indices.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,21 +316,20 @@
                 dataset.y <= config.bbox.maxy)
             x_idx = np.where(x_mask)
             y_idx = np.where(y_mask)
             # have to select based of index/position because of upper-left, lower-left indexing
             dataset = dataset.isel(x=x_idx[0], y=y_idx[0])
 
         # Resample if needed
-        if config.periodicity.name == (Periodicity.daily.name and
-                                       config.periods[0].value['unit'] == "month"):
+        if (config.periodicity.name == Periodicity.daily.name) and (config.periods[0].value['unit'] == "month"):
             dataset = dataset.resample(time='1MS').sum(
                 dim='time', skipna=False).chunk(chunks='auto')
             warnings.warn(
                 "periodicity is daily -- resampling data to monthly")
-        elif config.periodicity == Periodicity.monthly and config.periods[0].value['unit'] == "day":
+        elif (config.periodicity == Periodicity.monthly) and (config.periods[0].value['unit'] == "day"):
             raise IndexCalculationError(
                 "Invalid combination of data periodicity and period "
                 "-- Can't resample monthly periodicity to daily periods")
 
         return dataset
 
     @staticmethod
@@ -552,21 +551,20 @@
                 dataset.y <= config.bbox.maxy)
             x_idx = np.where(x_mask)
             y_idx = np.where(y_mask)
             # have to select based of index/position because of upper-left, lower-left indexing
             dataset = dataset.isel(x=x_idx[0], y=y_idx[0])
 
         # Resample if needed
-        if config.periodicity.name == (Periodicity.daily.name and
-                                       config.periods[0].value['unit'] == "month"):
+        if (config.periodicity.name == Periodicity.daily.name) and (config.periods[0].value['unit'] == "month"):
             dataset = dataset.resample(time='1MS').sum(
                 dim='time', skipna=False).chunk(chunks='auto')
             warnings.warn(
                 "periodicity is daily -- resampling data to monthly")
-        elif config.periodicity == Periodicity.monthly and config.periods[0].value['unit'] == "day":
+        elif (config.periodicity == Periodicity.monthly) and (config.periods[0].value['unit'] == "day"):
             raise IndexCalculationError(
                 "Invalid combination of data periodicity and period "
                 "-- Can't resample monthly periodicity to daily periods")
 
         return dataset
 
     @staticmethod
@@ -732,21 +730,20 @@
                 dataset.y <= config.bbox.maxy)
             x_idx = np.where(x_mask)
             y_idx = np.where(y_mask)
             # have to select based of index/position because of upper-left, lower-left indexing
             dataset = dataset.isel(x=x_idx[0], y=y_idx[0])
 
         # Resample if needed
-        if config.periodicity.name == (Periodicity.daily.name and
-                                       config.periods[0].value['unit'] == "month"):
+        if (config.periodicity.name == Periodicity.daily.name) and (config.periods[0].value['unit'] == "month"):
             dataset = dataset.resample(time='1MS').sum(
                 dim='time', skipna=False).chunk(chunks='auto')
             warnings.warn(
                 "periodicity is daily -- resampling data to monthly")
-        elif config.periodicity == Periodicity.monthly and config.periods[0].value['unit'] == "day":
+        elif (config.periodicity == Periodicity.monthly) and (config.periods[0].value['unit'] == "day"):
             raise IndexCalculationError(
                 "Invalid combination of data periodicity and period "
                 "-- Can't resample monthly periodicity to daily periods")
 
         return dataset
 
     @staticmethod
```

### Comparing `ddc-indices-0.5.1/ddc_indices/metadata.py` & `ddc-indices-0.5.2/ddc_indices/metadata.py`

 * *Files identical despite different names*

### Comparing `ddc-indices-0.5.1/ddc_indices/utils.py` & `ddc-indices-0.5.2/ddc_indices/utils.py`

 * *Files identical despite different names*

### Comparing `ddc-indices-0.5.1/ddc_indices.egg-info/PKG-INFO` & `ddc-indices-0.5.2/ddc_indices.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddc-indices
-Version: 0.5.1
+Version: 0.5.2
 Summary: Package for calculating meteorological indices
 Author-email: Balint Alfoldy <balint.alfoldy@lechnerkozpont.hu>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ddc-indices-0.5.1/pyproject.toml` & `ddc-indices-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ddc-indices"
-version = "0.5.1"
+version = "0.5.2"
 description = "Package for calculating meteorological indices"
 authors = [{ name="Balint Alfoldy", email="balint.alfoldy@lechnerkozpont.hu" }]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

