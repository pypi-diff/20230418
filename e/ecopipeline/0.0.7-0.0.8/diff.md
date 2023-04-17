# Comparing `tmp/ecopipeline-0.0.7.tar.gz` & `tmp/ecopipeline-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecopipeline-0.0.7.tar", last modified: Fri Apr 14 19:22:19 2023, max compression
+gzip compressed data, was "ecopipeline-0.0.8.tar", last modified: Mon Apr 17 22:11:58 2023, max compression
```

## Comparing `ecopipeline-0.0.7.tar` & `ecopipeline-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 19:22:16.602633 ecopipeline-0.0.7/
--rw-rw-rw-   0        0        0        0 2023-02-17 15:53:40.000000 ecopipeline-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1086 2023-04-14 19:22:19.640019 ecopipeline-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      641 2023-04-10 20:35:13.000000 ecopipeline-0.0.7/README.md
--rw-rw-rw-   0        0        0      108 2023-04-10 17:10:50.000000 ecopipeline-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      735 2023-04-14 19:22:19.747578 ecopipeline-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-04-10 17:18:28.000000 ecopipeline-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 19:22:16.718633 ecopipeline-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 19:22:16.706633 ecopipeline-0.0.7/src/ecopipeline/
--rw-rw-rw-   0        0        0     2060 2023-04-13 22:42:27.000000 ecopipeline-0.0.7/src/ecopipeline/__init__.py
--rw-rw-rw-   0        0        0     5746 2023-04-10 17:21:13.000000 ecopipeline-0.0.7/src/ecopipeline/bayview.py
--rw-rw-rw-   0        0        0      809 2023-03-31 18:26:04.000000 ecopipeline-0.0.7/src/ecopipeline/config.py
--rw-rw-rw-   0        0        0    13858 2023-04-10 20:26:32.000000 ecopipeline-0.0.7/src/ecopipeline/extract.py
--rw-rw-rw-   0        0        0    24099 2023-04-10 17:21:39.000000 ecopipeline-0.0.7/src/ecopipeline/lbnl.py
--rw-rw-rw-   0        0        0     9434 2023-04-10 18:47:39.000000 ecopipeline-0.0.7/src/ecopipeline/load.py
--rw-rw-rw-   0        0        0    30494 2023-04-14 19:16:37.000000 ecopipeline-0.0.7/src/ecopipeline/transform.py
--rw-rw-rw-   0        0        0     2780 2023-04-14 17:28:33.000000 ecopipeline-0.0.7/src/ecopipeline/unit_convert.py
-drwxrwxrwx   0        0        0        0 2023-04-14 19:22:16.762633 ecopipeline-0.0.7/src/ecopipeline.egg-info/
--rw-rw-rw-   0        0        0     1086 2023-04-14 19:22:16.000000 ecopipeline-0.0.7/src/ecopipeline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      462 2023-04-14 19:22:16.000000 ecopipeline-0.0.7/src/ecopipeline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 19:22:16.000000 ecopipeline-0.0.7/src/ecopipeline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-04-14 19:22:16.000000 ecopipeline-0.0.7/src/ecopipeline.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-14 19:22:16.000000 ecopipeline-0.0.7/src/ecopipeline.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 22:11:58.200955 ecopipeline-0.0.8/
+-rw-rw-rw-   0        0        0        0 2023-02-17 15:53:40.000000 ecopipeline-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1086 2023-04-17 22:11:58.222247 ecopipeline-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2023-04-10 20:35:13.000000 ecopipeline-0.0.8/README.md
+-rw-rw-rw-   0        0        0      108 2023-04-10 17:10:50.000000 ecopipeline-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      735 2023-04-17 22:11:58.261081 ecopipeline-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-04-10 17:18:28.000000 ecopipeline-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:11:56.592953 ecopipeline-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 22:11:57.604954 ecopipeline-0.0.8/src/ecopipeline/
+-rw-rw-rw-   0        0        0     2105 2023-04-17 22:11:31.000000 ecopipeline-0.0.8/src/ecopipeline/__init__.py
+-rw-rw-rw-   0        0        0     5746 2023-04-10 17:21:13.000000 ecopipeline-0.0.8/src/ecopipeline/bayview.py
+-rw-rw-rw-   0        0        0      809 2023-03-31 18:26:04.000000 ecopipeline-0.0.8/src/ecopipeline/config.py
+-rw-rw-rw-   0        0        0    14785 2023-04-17 21:25:54.000000 ecopipeline-0.0.8/src/ecopipeline/extract.py
+-rw-rw-rw-   0        0        0    24099 2023-04-10 17:21:39.000000 ecopipeline-0.0.8/src/ecopipeline/lbnl.py
+-rw-rw-rw-   0        0        0     9434 2023-04-10 18:47:39.000000 ecopipeline-0.0.8/src/ecopipeline/load.py
+-rw-rw-rw-   0        0        0    30761 2023-04-17 21:59:13.000000 ecopipeline-0.0.8/src/ecopipeline/transform.py
+-rw-rw-rw-   0        0        0     2780 2023-04-14 17:28:33.000000 ecopipeline-0.0.8/src/ecopipeline/unit_convert.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:11:58.116955 ecopipeline-0.0.8/src/ecopipeline.egg-info/
+-rw-rw-rw-   0        0        0     1086 2023-04-17 22:11:56.000000 ecopipeline-0.0.8/src/ecopipeline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2023-04-17 22:11:56.000000 ecopipeline-0.0.8/src/ecopipeline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 22:11:56.000000 ecopipeline-0.0.8/src/ecopipeline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-04-17 22:11:56.000000 ecopipeline-0.0.8/src/ecopipeline.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-17 22:11:56.000000 ecopipeline-0.0.8/src/ecopipeline.egg-info/top_level.txt
```

### Comparing `ecopipeline-0.0.7/PKG-INFO` & `ecopipeline-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.0.7
+Version: 0.0.8
 Summary: Contains functions for use in Ecotope Datapipelines
 Author: Nolan and SU Students
 Author-email: nolan@ecotope.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `ecopipeline-0.0.7/README.md` & `ecopipeline-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.7/setup.cfg` & `ecopipeline-0.0.8/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 636f 7069 7065 6c69 6e65 0d0a   = ecopipeline..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 370d  version = 0.0.7.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 380d  version = 0.0.8.
 00000030: 0a61 7574 686f 7220 3d20 4e6f 6c61 6e20  .author = Nolan 
 00000040: 616e 6420 5355 2053 7475 6465 6e74 730d  and SU Students.
 00000050: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000060: 6e6f 6c61 6e40 6563 6f74 6f70 652e 636f  nolan@ecotope.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2043 6f6e 7461 696e 7320 6675 6e63 7469   Contains functi
 00000090: 6f6e 7320 666f 7220 7573 6520 696e 2045  ons for use in E
```

### Comparing `ecopipeline-0.0.7/src/ecopipeline/__init__.py` & `ecopipeline-0.0.8/src/ecopipeline/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from .extract import get_noaa_data, json_to_df, extract_files, get_last_full_day_from_db, extract_new, csv_to_df, get_sub_dirs
+from .extract import get_noaa_data, json_to_df, extract_files, get_last_full_day_from_db, get_db_row_from_time, extract_new, csv_to_df, get_sub_dirs
 from .transform import rename_sensors, avg_duplicate_times, remove_outliers, ffill_missing, sensor_adjustment, get_energy_by_min, verify_power_energy, round_time, aggregate_df, join_to_hourly, concat_last_row, join_to_daily, get_temp_zones120, get_storage_gals120, cop_method_2
 from .load import get_login_info, connect_db, check_table_exists, create_new_table, load_database, load_overwrite_database
 from .lbnl import nclarity_filter_new, site_specific, condensate_calculations, gas_valve_diff, gather_outdoor_conditions, nclarity_csv_to_df, add_date, aqsuite_filter_new, get_refrig_charge, elev_correction, change_ID_to_HVAC, get_cop_values, get_cfm_values, replace_humidity, create_fan_curves, lbnl_temperature_conversions, lbnl_pressure_conversions, lbnl_sat_calculations
 from .bayview import calculate_cop_values, aggregate_values
-__all__ = ["get_last_full_day_from_db", "set_input", "set_output","get_noaa_data", "json_to_df", "extract_files", "avg_duplicate_times", "remove_outliers", "ffill_missing", "sensor_adjustment", "get_energy_by_min", "verify_power_energy",
+__all__ = ["get_last_full_day_from_db", "get_db_row_from_time" "set_input", "set_output","get_noaa_data", "json_to_df", "extract_files", "avg_duplicate_times", "remove_outliers", "ffill_missing", "sensor_adjustment", "get_energy_by_min", "verify_power_energy",
            "set_data", "aggregate_values", "calculate_cop_values", "get_login_info", "connect_db", "check_table_exists", "create_new_table", "createUnknownColumns", "load_database", "load_overwrite_database", "rename_sensors", "round_time", "aggregate_df", 
            "extract_new", "csv_to_df", "set_config", "get_sub_dirs", "join_to_hourly", "concat_last_row", "join_to_daily", "get_temp_zones120", "get_storage_gals120", "cop_method_2",  "site_specific", "condensate_calculations", "gas_valve_diff",
            "nclarity_filter_new", "gather_outdoor_conditions", "nclarity_csv_to_df", "add_date", "aqsuite_filter_new", "elev_correction", "get_refrig_charge", "change_ID_to_HVAC", "get_cop_values", "get_cfm_values", "replace_humidity", "create_fan_curves", 
            "lbnl_temperature_conversions", "lbnl_pressure_conversions", "lbnl_sat_calculations"]
```

### Comparing `ecopipeline-0.0.7/src/ecopipeline/bayview.py` & `ecopipeline-0.0.8/src/ecopipeline/bayview.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.7/src/ecopipeline/config.py` & `ecopipeline-0.0.8/src/ecopipeline/config.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.7/src/ecopipeline/extract.py` & `ecopipeline-0.0.8/src/ecopipeline/extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,42 @@
         print("Unable to find last timestamp in database. Using default time to extract data.")
 
     db_cursor.close()
     db_connection.close()
 
     return return_time
 
+def get_db_row_from_time(time: datetime) -> pd.DataFrame:
+    """
+    Extracts a row from the applicable minute table in the database for the given datetime or returns empty dataframe if none exists
+
+    Args:
+        time (datetime): The time index to get the row from
+    Returns: 
+        pd.DataFrame: Pandas Dataframe containing the row or empty if no row exists for the timestamp
+    """
+    config_dict = get_login_info(["minute"])
+    db_connection, db_cursor = connect_db(config_info=config_dict['database'])
+    row_data = pd.DataFrame()
+
+    try:
+        db_cursor.execute(
+            f"SELECT * FROM {config_dict['minute']['table_name']} WHERE time_pt = '{time}'")
+
+        row_data = pd.DataFrame(db_cursor.fetchall())
+    except mysqlerrors.Error as e:
+        print("Error executing sql query.")
+        print("MySQL error: {}".format(e))
+
+    db_cursor.close()
+    db_connection.close()
+
+    return row_data
+
+
 
 def extract_new(time: datetime, json_filenames: List[str]) -> List[str]:
     """
     Function filters the filenames to only those newer than the last date.
 
     Args: 
         time (datetime): The point in time for which we want to start the data extraction from
```

### Comparing `ecopipeline-0.0.7/src/ecopipeline/lbnl.py` & `ecopipeline-0.0.8/src/ecopipeline/lbnl.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.7/src/ecopipeline/load.py` & `ecopipeline-0.0.8/src/ecopipeline/load.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.7/src/ecopipeline/transform.py` & `ecopipeline-0.0.8/src/ecopipeline/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,39 +143,42 @@
     bounds_df.set_index(['variable_name'], inplace=True)
     bounds_df = bounds_df[bounds_df.index.notnull()]
 
     df.apply(_rm_cols, args=(bounds_df,))
     return df
 
 
-def _ffill(col, ffill_df):  # Helper function for ffill_missing
+def _ffill(col, ffill_df, previous_fill: pd.DataFrame = None):  # Helper function for ffill_missing
     """
     Function will take in a pandas series and ffill information from a pandas dataframe,
     then for each entry in the series, either forward fill unconditionally or up to the 
     provided limit based on the information in provided dataframe. 
 
     Args: 
         col (pd.Series): Pandas series
         ffill_df (pd.DataFrame): Pandas dataframe
     Returns: 
         None (df is modified, not returned)
     """
     if (col.name in ffill_df.index):
+        #set initial fill value where needed for first row
+        if previous_fill is not None and len(col) > 0 and col[0] == np.nan:
+            col[0] = previous_fill[col.name][0]
         cp = ffill_df.loc[col.name]["changepoint"]
         length = ffill_df.loc[col.name]["ffill_length"]
         if (length != length):  # check for nan, set to 0
             length = 0
         length = int(length)  # casting to int to avoid float errors
         if (cp == 1):  # ffill unconditionally
             col.fillna(method='ffill', inplace=True)
         elif (cp == 0):  # ffill only up to length
             col.fillna(method='ffill', inplace=True, limit=length)
 
 
-def ffill_missing(df: pd.DataFrame, vars_filename: str = f"{_input_directory}Variable_Names.csv") -> pd.DataFrame:
+def ffill_missing(df: pd.DataFrame, vars_filename: str = f"{_input_directory}Variable_Names.csv", previous_fill: pd.DataFrame = None) -> pd.DataFrame:
     """
     Function will take a pandas dataframe and forward fill select variables with no entry. 
     Args: 
         df (pd.DataFrame): Pandas dataframe
         variable_names_path (str): file location of file containing sensor aliases to their corresponding name (default value of Variable_Names.csv)
     Returns: 
         pd.DataFrame: Pandas dataframe
@@ -190,18 +193,17 @@
     ffill_df = ffill_df.loc[:, [
         "variable_name", "changepoint", "ffill_length"]]
     # drop data without changepoint AND ffill_length
     ffill_df.dropna(axis=0, thresh=2, inplace=True)
     ffill_df.set_index(['variable_name'], inplace=True)
     ffill_df = ffill_df[ffill_df.index.notnull()]  # drop data without names
 
-    df.apply(_ffill, args=(ffill_df,))
+    df.apply(_ffill, args=(ffill_df,previous_fill))
     return df
 
-
 def sensor_adjustment(df: pd.DataFrame) -> pd.DataFrame:
     """
     Reads in input/adjustments.csv and applies necessary adjustments to the dataframe
 
     Args: 
         df (pd.DataFrame): DataFrame to be adjusted
     Returns:
```

### Comparing `ecopipeline-0.0.7/src/ecopipeline/unit_convert.py` & `ecopipeline-0.0.8/src/ecopipeline/unit_convert.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.7/src/ecopipeline.egg-info/PKG-INFO` & `ecopipeline-0.0.8/src/ecopipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.0.7
+Version: 0.0.8
 Summary: Contains functions for use in Ecotope Datapipelines
 Author: Nolan and SU Students
 Author-email: nolan@ecotope.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

