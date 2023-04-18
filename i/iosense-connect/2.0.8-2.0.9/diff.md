# Comparing `tmp/iosense_connect-2.0.8.tar.gz` & `tmp/iosense_connect-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iosense_connect-2.0.8.tar", last modified: Sat Apr 15 12:10:58 2023, max compression
+gzip compressed data, was "dist\iosense_connect-2.0.9.tar", last modified: Tue Apr 18 06:13:30 2023, max compression
```

## Comparing `iosense_connect-2.0.8.tar` & `iosense_connect-2.0.9.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 12:10:58.175881 iosense_connect-2.0.8/
--rw-rw-rw-   0        0        0      117 2023-04-15 12:10:58.173475 iosense_connect-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-04-06 06:23:07.000000 iosense_connect-2.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 12:10:58.113609 iosense_connect-2.0.8/iosense_connect/
--rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.0.8/iosense_connect/__init__.py
--rw-rw-rw-   0        0        0    19421 2023-04-15 12:10:25.000000 iosense_connect-2.0.8/iosense_connect/data_access.py
-drwxrwxrwx   0        0        0        0 2023-04-15 12:10:58.169022 iosense_connect-2.0.8/iosense_connect.egg-info/
--rw-rw-rw-   0        0        0      117 2023-04-15 12:10:57.000000 iosense_connect-2.0.8/iosense_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-04-15 12:10:57.000000 iosense_connect-2.0.8/iosense_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 12:10:57.000000 iosense_connect-2.0.8/iosense_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-15 12:10:57.000000 iosense_connect-2.0.8/iosense_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 12:10:58.175881 iosense_connect-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0      207 2023-04-15 12:10:44.000000 iosense_connect-2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:13:30.822833 iosense_connect-2.0.9/
+-rw-rw-rw-   0        0        0     1087 2023-04-18 04:21:30.000000 iosense_connect-2.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     1046 2023-04-18 06:13:30.822833 iosense_connect-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      674 2023-04-15 12:45:17.000000 iosense_connect-2.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 06:13:30.775959 iosense_connect-2.0.9/iosense_connect/
+-rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.0.9/iosense_connect/__init__.py
+-rw-rw-rw-   0        0        0    19328 2023-04-18 06:12:50.000000 iosense_connect-2.0.9/iosense_connect/data_access.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:13:30.807213 iosense_connect-2.0.9/iosense_connect.egg-info/
+-rw-rw-rw-   0        0        0     1046 2023-04-18 06:13:30.000000 iosense_connect-2.0.9/iosense_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-04-18 06:13:30.000000 iosense_connect-2.0.9/iosense_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 06:13:30.000000 iosense_connect-2.0.9/iosense_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-18 06:13:30.000000 iosense_connect-2.0.9/iosense_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 06:13:30.822833 iosense_connect-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      612 2023-04-18 06:13:28.000000 iosense_connect-2.0.9/setup.py
```

### Comparing `iosense_connect-2.0.8/README.md` & `iosense_connect-2.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 ### Project description
 Faclon I/O Sense Data Access Library
 ​
 #### Where to get it
 https://pypi.org/project/iosense/
 
 #### Installation
-pip install iosense-connect
+pip install iosense
 
-pip3 install iosense-connect
+pip3 install iosense
 
 #### Features
 Retrives following details:
 
 - User information.
 - Device Details.
 - Device metaData.
```

### Comparing `iosense_connect-2.0.8/iosense_connect/data_access.py` & `iosense_connect-2.0.9/iosense_connect/data_access.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # import libraries
 import json
 import sys
 import time
-from datetime import datetime,timedelta
-
+from datetime import datetime, timedelta
 import numpy as np
 import pandas as pd
 import requests
 import urllib3
 
 pd.options.mode.chained_assignment = None
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
@@ -29,15 +28,14 @@
 
         """
         try:
             url = "https://" + self.url + "/api/metaData/device/" + device_id
             header = {'userID': self.userID}
             payload = {}
             response = requests.request('GET', url, headers=header, data=payload, verify=False)
-            # print(response.text)
             if response.status_code != 200:
                 raw = json.loads(response.text)
                 raise ValueError(raw['error'])
             else:
                 raw_data = json.loads(response.text)['data']
                 return raw_data
 
@@ -55,16 +53,18 @@
 
         Maps sensor_alias/ sensor name with corresponding sensor ID
         replaces column names with sensor_alias_sensor_id
 
         """
 
         list1 = list(df['sensor'].unique())
+
         if len(raw_metadata) == 0:
             raw_metadata = DataAccess.get_device_metadata(self, device_id)
+            print(raw_metadata)
         sensor_spec = 'sensors'
         sensor_param_df = pd.DataFrame(raw_metadata[sensor_spec])
 
         for i in list1:
             sensor_param_df1 = sensor_param_df[sensor_param_df['sensorId'] == i]
             if len(sensor_param_df1) != 0:
                 # print('sensor_param_df',sensor_param_df1)
@@ -96,16 +96,19 @@
 
         for (value1, value2) in zip(sensor_id_list, sensor_name_list):
             # print(value1, value2)
             # print(data[str(value1)])
             df_meta = pd.DataFrame(data[str(value1)])
             # print(df_meta)
             df_meta = df_meta.set_index('paramName').transpose()
+            # print(df_meta)
             if 'm' in df_meta.columns and 'c' in df_meta.columns:
+                # print(df_meta.iloc[0]['m'],type(df_meta.iloc[0]['m']))
                 m = float(df_meta.iloc[0]['m'])
+                # print('M value',m)
                 c = int(df_meta.iloc[0]['c'])
                 # print(m, type(c))
                 # print(df[str(value2)])
                 df[str(value2)] =  df[str(value2)].replace('BAD 255', '-99999').replace('-','99999').replace('BAD undefined', '-99999').replace('BAD 0', '-99999')
                 df[str(value2)] = df[str(value2)].astype('float')
                 # print('==',df[str(value2)])
                 df[str(value2)] = (df[str(value2)] * m) + c
@@ -201,37 +204,30 @@
                 raw_data = json.loads(response.text)['data']
                 return raw_data
 
         except Exception as e:
             print('Failed to fetch user Information')
             print(e)
 
-    def get_dp(self, device_id, sensors=['D29'], n=1, cal=True, end_time=datetime.now(),IST=True):
+    def get_dp(self, device_id, sensors, n=1, cal=True, end_time=datetime.now(), IST=True):
         """
 
         :param device_id: string
-        :param sensors: list of sensors. Sensors is not None
-        :param n: number of data points
-        :param cal: True/False
-        :param end_time: 'year-month-day hours:minutes:seconds'
+        :param sensors: list of sensors
+        :param n: number of data points (default: 1)
+        :param cal: bool (default: True)
+        :param end_time: 'YYYY:MM:DD HH:MM:SS'
+        :param IST: bool (default: True)
         :return: Dataframe with values
 
         Get Data Point fetches data containing values of last n data points of given sensor at given time.
 
         """
         try:
             metadata = {}
-
-            try:
-                end_time = datetime.strptime(end_time, '%Y-%m-%d %H:%M:%S')
-                print(end_time)
-            except Exception as e:
-                end_time = end_time + " 23:59:59"
-                pass
-
             end_time = pd.to_datetime(end_time)
             if IST:
                 end_time = end_time - timedelta(hours=5, minutes=30)
             end_time = int(round(end_time.timestamp()))
             if type(sensors) == list:
                 len_sensors = len(sensors)
                 if len_sensors == 0:
@@ -254,34 +250,34 @@
                     sys.stdout.write("Approx Records Fetched %d" % (10000 * record))
                     sys.stdout.flush()
                 url = "https://" + self.url + "/api/apiLayer/getLimitedDataMultipleSensors/?device=" + device_id + "&sensor=" + sensor_values + "&eTime=" + str(
                     cursor['end']) + "&lim=" + str(cursor['limit']) + "&cursor=true"
                 response = requests.request("GET", url, headers=header, data=payload)
                 raw = json.loads(response.text)
                 if response.status_code != 200:
-                    raise ValueError(raw)
+                    raise ValueError(response.status_code)
                 if 'success' in raw:
                     raise ValueError(raw)
                 else:
                     raw_data = json.loads(response.text)['data']
                     cursor = json.loads(response.text)['cursor']
                     if len(raw_data) != 0:
                         df = pd.concat([df, pd.DataFrame(raw_data)])
                     counter = counter + 1
                 if cursor['end'] == None:
                     break
-            if len(df) != 0:
-                if IST:
-                    df['time'] = pd.to_datetime(df['time'], utc=False)
-                    df['time'] = df['time'].dt.tz_convert('Asia/Kolkata').dt.tz_localize(None)
-                df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata)
-                df = DataAccess.get_cleaned_table(self, df)
-
-                if str(cal).lower() == 'true':
-                    df = DataAccess.get_caliberation(self, device_id, metadata, df)
+            if len(df) == 0:
+                raise ValueError('No Data')
+            if IST:
+                df['time'] = pd.to_datetime(df['time'], utc=False)
+                df['time'] = df['time'].dt.tz_convert('Asia/Kolkata').dt.tz_localize(None)
+            df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata)
+            df = DataAccess.get_cleaned_table(self, df)
+            if str(cal).lower() == 'true':
+                df = DataAccess.get_caliberation(self, device_id, metadata, df)
             return df
         except Exception as e:
             print(e)
 
     def data_query(self, device_id, start_time, end_time=datetime.now(), sensors=None, cal=True, bands=None, IST=True ,echo=True):
         # df = pd.DataFrame()
         metadata = {}
@@ -290,19 +286,19 @@
             data_sensor = metadata['sensors']
             df_sensor = pd.DataFrame(data_sensor)
             sensor_id_list = list(df_sensor['sensorId'])
             sensors = sensor_id_list
         rawdata_res = []
         temp = ''
         try:
-            end_time = datetime.strptime(end_time, '%Y-%m-%d %H:%M:%S')
-        except Exception as e:
-            end_time = end_time + " 23:59:59"
+            end_time = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S')
+        except Exception:
+            if type(end_time) == str:
+                end_time = str(end_time) + " 23:59:59"
             pass
-
         s_time = pd.to_datetime(start_time)
         e_time = pd.to_datetime(end_time)
         if IST:
             s_time = s_time - timedelta(hours=5, minutes=30)
             e_time = e_time - timedelta(hours=5, minutes=30)
         st_time = int(round(s_time.timestamp())) * 10000
         en_time = int(round(e_time.timestamp())) * 10000
@@ -336,17 +332,17 @@
                     temp = url_api + device_id + "&sensor=" + sensor_values + "&sTime=" + str(
                         cursor['start']) + "&eTime=" + str(cursor['end']) + "&cursor=true&limit=50000"
 
             response = requests.request("GET", temp, headers=header, data=payload)
             raw = json.loads(response.text)
             # print(raw)
             if response.status_code != 200:
-                raise ValueError(raw)
+                raise ValueError(raw['error'])
             if 'success' in raw:
-                raise ValueError(raw)
+                raise ValueError(raw['error'])
 
             else:
                 raw_data = json.loads(response.text)['data']
                 # print('====================',raw_data)
                 cursor = json.loads(response.text)['cursor']
                 if len(raw_data) !=0:
                     rawdata_res = rawdata_res + raw_data
@@ -356,25 +352,20 @@
         # print(rawdata_res)
         df_raw = pd.DataFrame(rawdata_res)
 
         if len(df_raw) != 0 :
             if IST:
                 df_raw['time'] = pd.to_datetime(df_raw['time'], utc=False)
                 df_raw['time'] = df_raw['time'].dt.tz_convert('Asia/Kolkata').dt.tz_localize(None)
-
             if len(df_raw.columns) == 2:
                 df_raw['sensor'] = sensors[0]
-
             df, metadata = DataAccess.get_sensor_alias(self, device_id, df_raw, metadata)
             df = DataAccess.get_cleaned_table(self, df)
-
-            if cal or cal == 'true' or cal == "TRUE":
-                # #qq=qq[~qq['value'].isin(['','BAD 255','BAD 0','BAD undefined','-'])]
+            if str(cal).lower() == 'true':
                 df = DataAccess.get_caliberation(self, device_id, metadata, df)
-
             if bands is not None:
                 df = DataAccess.time_grouping(self, df, bands)
         else:
             df = df_raw
         return df
 
     def publish_event(self, title, message, meta_data, hover_data, event_tags, created_on):
```

