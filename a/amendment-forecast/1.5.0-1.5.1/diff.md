# Comparing `tmp/amendment_forecast-1.5.0.tar.gz` & `tmp/amendment_forecast-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amendment_forecast-1.5.0.tar", last modified: Mon Feb 27 17:08:30 2023, max compression
+gzip compressed data, was "amendment_forecast-1.5.1.tar", last modified: Tue Apr 18 14:20:03 2023, max compression
```

## Comparing `amendment_forecast-1.5.0.tar` & `amendment_forecast-1.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 makanicartwright   (501) staff       (20)        0 2023-02-27 17:08:30.875832 amendment_forecast-1.5.0/
--rw-r--r--   0 makanicartwright   (501) staff       (20)     1009 2023-02-27 17:08:30.875887 amendment_forecast-1.5.0/PKG-INFO
--rw-r--r--   0 makanicartwright   (501) staff       (20)      630 2023-01-19 15:29:09.000000 amendment_forecast-1.5.0/README.md
--rw-r--r--   0 makanicartwright   (501) staff       (20)      104 2023-01-19 15:29:09.000000 amendment_forecast-1.5.0/pyproject.toml
--rw-r--r--   0 makanicartwright   (501) staff       (20)      548 2023-02-27 17:08:30.876136 amendment_forecast-1.5.0/setup.cfg
-drwxr-xr-x   0 makanicartwright   (501) staff       (20)        0 2023-02-27 17:08:30.874086 amendment_forecast-1.5.0/src/
-drwxr-xr-x   0 makanicartwright   (501) staff       (20)        0 2023-02-27 17:08:30.875207 amendment_forecast-1.5.0/src/amendment_forecast/
--rw-r--r--   0 makanicartwright   (501) staff       (20)        0 2023-01-19 15:29:09.000000 amendment_forecast-1.5.0/src/amendment_forecast/__init__.py
--rw-r--r--   0 makanicartwright   (501) staff       (20)    10621 2023-01-25 15:07:50.000000 amendment_forecast-1.5.0/src/amendment_forecast/main.py
--rw-r--r--   0 makanicartwright   (501) staff       (20)    33505 2023-02-27 17:07:32.000000 amendment_forecast-1.5.0/src/amendment_forecast/models.py
--rw-r--r--   0 makanicartwright   (501) staff       (20)     6261 2023-01-19 15:29:09.000000 amendment_forecast-1.5.0/src/amendment_forecast/utils.py
-drwxr-xr-x   0 makanicartwright   (501) staff       (20)        0 2023-02-27 17:08:30.875735 amendment_forecast-1.5.0/src/amendment_forecast.egg-info/
--rw-r--r--   0 makanicartwright   (501) staff       (20)     1009 2023-02-27 17:08:30.000000 amendment_forecast-1.5.0/src/amendment_forecast.egg-info/PKG-INFO
--rw-r--r--   0 makanicartwright   (501) staff       (20)      349 2023-02-27 17:08:30.000000 amendment_forecast-1.5.0/src/amendment_forecast.egg-info/SOURCES.txt
--rw-r--r--   0 makanicartwright   (501) staff       (20)        1 2023-02-27 17:08:30.000000 amendment_forecast-1.5.0/src/amendment_forecast.egg-info/dependency_links.txt
--rw-r--r--   0 makanicartwright   (501) staff       (20)       19 2023-02-27 17:08:30.000000 amendment_forecast-1.5.0/src/amendment_forecast.egg-info/top_level.txt
+drwxr-xr-x   0 makanicartwright   (501) staff       (20)        0 2023-04-18 14:20:03.990201 amendment_forecast-1.5.1/
+-rw-r--r--   0 makanicartwright   (501) staff       (20)     1009 2023-04-18 14:20:03.990252 amendment_forecast-1.5.1/PKG-INFO
+-rw-r--r--   0 makanicartwright   (501) staff       (20)      630 2023-01-19 15:29:09.000000 amendment_forecast-1.5.1/README.md
+-rw-r--r--   0 makanicartwright   (501) staff       (20)      104 2023-01-19 15:29:09.000000 amendment_forecast-1.5.1/pyproject.toml
+-rw-r--r--   0 makanicartwright   (501) staff       (20)      548 2023-04-18 14:20:03.990517 amendment_forecast-1.5.1/setup.cfg
+drwxr-xr-x   0 makanicartwright   (501) staff       (20)        0 2023-04-18 14:20:03.988501 amendment_forecast-1.5.1/src/
+drwxr-xr-x   0 makanicartwright   (501) staff       (20)        0 2023-04-18 14:20:03.989290 amendment_forecast-1.5.1/src/amendment_forecast/
+-rw-r--r--   0 makanicartwright   (501) staff       (20)        0 2023-01-19 15:29:09.000000 amendment_forecast-1.5.1/src/amendment_forecast/__init__.py
+-rw-r--r--   0 makanicartwright   (501) staff       (20)    10613 2023-04-18 14:18:35.000000 amendment_forecast-1.5.1/src/amendment_forecast/main.py
+-rw-r--r--   0 makanicartwright   (501) staff       (20)    33505 2023-02-27 17:07:32.000000 amendment_forecast-1.5.1/src/amendment_forecast/models.py
+-rw-r--r--   0 makanicartwright   (501) staff       (20)     6261 2023-01-19 15:29:09.000000 amendment_forecast-1.5.1/src/amendment_forecast/utils.py
+drwxr-xr-x   0 makanicartwright   (501) staff       (20)        0 2023-04-18 14:20:03.990113 amendment_forecast-1.5.1/src/amendment_forecast.egg-info/
+-rw-r--r--   0 makanicartwright   (501) staff       (20)     1009 2023-04-18 14:20:03.000000 amendment_forecast-1.5.1/src/amendment_forecast.egg-info/PKG-INFO
+-rw-r--r--   0 makanicartwright   (501) staff       (20)      349 2023-04-18 14:20:03.000000 amendment_forecast-1.5.1/src/amendment_forecast.egg-info/SOURCES.txt
+-rw-r--r--   0 makanicartwright   (501) staff       (20)        1 2023-04-18 14:20:03.000000 amendment_forecast-1.5.1/src/amendment_forecast.egg-info/dependency_links.txt
+-rw-r--r--   0 makanicartwright   (501) staff       (20)       19 2023-04-18 14:20:03.000000 amendment_forecast-1.5.1/src/amendment_forecast.egg-info/top_level.txt
```

### Comparing `amendment_forecast-1.5.0/PKG-INFO` & `amendment_forecast-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amendment_forecast
-Version: 1.5.0
+Version: 1.5.1
 Summary: A forecaster for sales data
 Home-page: https://github.com/amendmentai/forecast_models
 Author: Makani Cartwright
 Author-email: makani@amendmentai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `amendment_forecast-1.5.0/README.md` & `amendment_forecast-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `amendment_forecast-1.5.0/setup.cfg` & `amendment_forecast-1.5.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = amendment_forecast
-version = 1.5.0
+version = 1.5.1
 author = Makani Cartwright
 author_email = makani@amendmentai.com
 description = A forecaster for sales data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/amendmentai/forecast_models
 classifiers =
```

### Comparing `amendment_forecast-1.5.0/src/amendment_forecast/main.py` & `amendment_forecast-1.5.1/src/amendment_forecast/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 
 def get_forecast_periods(last_day, horizon_years, frequency) -> list:
     # Get start and end dates
     max_week = last_day.strftime("%Y %W")
     last_week_start = datetime.strptime(f"{max_week} w1", "%Y %W w%w")
     start_date = last_week_start + relativedelta(days=7)
     end_date = start_date + relativedelta(years=horizon_years)
+    # Truncate if the last week is the same as the first
+    period_list = pd.date_range(start=start_date, end=end_date, freq=frequency)
     if frequency == "W-MON":
-        # Truncate if the last week is the same as the first
-        period_list = pd.date_range(start=start_date, end=end_date, freq=frequency)
         first_week_number = pd.Timestamp(period_list[0]).isocalendar()[1]
         final_week_number = pd.Timestamp(period_list[-1]).isocalendar()[1]
         drop_final_week = False
         if first_week_number not in [52, 53]:
             if final_week_number == first_week_number:
                 drop_final_week = True
         else:
```

### Comparing `amendment_forecast-1.5.0/src/amendment_forecast/models.py` & `amendment_forecast-1.5.1/src/amendment_forecast/models.py`

 * *Files identical despite different names*

### Comparing `amendment_forecast-1.5.0/src/amendment_forecast/utils.py` & `amendment_forecast-1.5.1/src/amendment_forecast/utils.py`

 * *Files identical despite different names*

### Comparing `amendment_forecast-1.5.0/src/amendment_forecast.egg-info/PKG-INFO` & `amendment_forecast-1.5.1/src/amendment_forecast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amendment-forecast
-Version: 1.5.0
+Version: 1.5.1
 Summary: A forecaster for sales data
 Home-page: https://github.com/amendmentai/forecast_models
 Author: Makani Cartwright
 Author-email: makani@amendmentai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

