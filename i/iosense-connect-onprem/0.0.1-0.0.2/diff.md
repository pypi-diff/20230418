# Comparing `tmp/iosense_connect_onprem-0.0.1.tar.gz` & `tmp/iosense_connect_onprem-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iosense_connect_onprem-0.0.1.tar", last modified: Tue Apr 18 04:10:41 2023, max compression
+gzip compressed data, was "dist\iosense_connect_onprem-0.0.2.tar", last modified: Tue Apr 18 05:58:17 2023, max compression
```

## Comparing `iosense_connect_onprem-0.0.1.tar` & `iosense_connect_onprem-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 04:10:41.048844 iosense_connect_onprem-0.0.1/
--rw-rw-rw-   0        0        0      158 2023-04-18 04:10:41.046189 iosense_connect_onprem-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      674 2023-04-15 12:45:17.000000 iosense_connect_onprem-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 04:10:40.961883 iosense_connect_onprem-0.0.1/iosense_connect_onprem/
--rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect_onprem-0.0.1/iosense_connect_onprem/__init__.py
--rw-rw-rw-   0        0        0    19726 2023-04-18 04:02:24.000000 iosense_connect_onprem-0.0.1/iosense_connect_onprem/data_access.py
-drwxrwxrwx   0        0        0        0 2023-04-18 04:10:41.044055 iosense_connect_onprem-0.0.1/iosense_connect_onprem.egg-info/
--rw-rw-rw-   0        0        0      158 2023-04-18 04:10:40.000000 iosense_connect_onprem-0.0.1/iosense_connect_onprem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-04-18 04:10:40.000000 iosense_connect_onprem-0.0.1/iosense_connect_onprem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 04:10:40.000000 iosense_connect_onprem-0.0.1/iosense_connect_onprem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-18 04:10:40.000000 iosense_connect_onprem-0.0.1/iosense_connect_onprem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 04:10:41.048844 iosense_connect_onprem-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      355 2023-04-18 04:10:37.000000 iosense_connect_onprem-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:58:17.606824 iosense_connect_onprem-0.0.2/
+-rw-rw-rw-   0        0        0     1087 2023-04-18 04:21:30.000000 iosense_connect_onprem-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1062 2023-04-18 05:58:17.604821 iosense_connect_onprem-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      683 2023-04-18 04:44:54.000000 iosense_connect_onprem-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 05:58:17.517831 iosense_connect_onprem-0.0.2/iosense_connect_onprem/
+-rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect_onprem-0.0.2/iosense_connect_onprem/__init__.py
+-rw-rw-rw-   0        0        0    19470 2023-04-18 05:58:11.000000 iosense_connect_onprem-0.0.2/iosense_connect_onprem/data_access.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:58:17.601824 iosense_connect_onprem-0.0.2/iosense_connect_onprem.egg-info/
+-rw-rw-rw-   0        0        0     1062 2023-04-18 05:58:17.000000 iosense_connect_onprem-0.0.2/iosense_connect_onprem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-04-18 05:58:17.000000 iosense_connect_onprem-0.0.2/iosense_connect_onprem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 05:58:17.000000 iosense_connect_onprem-0.0.2/iosense_connect_onprem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-04-18 05:58:17.000000 iosense_connect_onprem-0.0.2/iosense_connect_onprem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 05:58:17.606824 iosense_connect_onprem-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      626 2023-04-18 05:58:11.000000 iosense_connect_onprem-0.0.2/setup.py
```

### Comparing `iosense_connect_onprem-0.0.1/README.md` & `iosense_connect_onprem-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 #### Dependencies
 
 + pandas
 + requests
 + json 
 + time 
 + datetime 
++ numpy
 
 
 #### Documentation
 The official documentation is hosted on​ 
 
 #### Reach us
 For usage questions, please reach out to us at reachus@faclon.com
```

### Comparing `iosense_connect_onprem-0.0.1/iosense_connect_onprem/data_access.py` & `iosense_connect_onprem-0.0.2/iosense_connect_onprem/data_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,20 +222,14 @@
         :return: Dataframe with values
 
         Get Data Point fetches data containing values of last n data points of given sensor at given time.
 
         """
         try:
             metadata = {}
-            try:
-                end_time = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S')
-            except Exception:
-                if type(end_time) == str:
-                    end_time = str(end_time) + " 23:59:59"
-                pass
             end_time = pd.to_datetime(end_time)
             if IST:
                 end_time = end_time - timedelta(hours=5, minutes=30)
 
             end_time = int(round(end_time.timestamp()))
             if type(sensors) == list:
                 len_sensors = len(sensors)
```

