# Comparing `tmp/northgravity-0.1.4.tar.gz` & `tmp/northgravity-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/northgravity-0.1.4.tar", last modified: Wed Feb  8 14:30:53 2023, max compression
+gzip compressed data, was "northgravity-0.1.5.tar", last modified: Tue Apr 18 12:32:31 2023, max compression
```

## Comparing `northgravity-0.1.4.tar` & `northgravity-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 Izabella   (502) staff       (20)        0 2023-02-08 14:30:53.749232 northgravity-0.1.4/
--rw-r--r--   0 Izabella   (502) staff       (20)     1055 2022-12-19 09:31:57.000000 northgravity-0.1.4/LICENSE
--rw-r--r--   0 Izabella   (502) staff       (20)    27037 2023-02-08 14:30:53.749030 northgravity-0.1.4/PKG-INFO
--rw-r--r--   0 Izabella   (502) staff       (20)    26604 2023-02-08 14:30:53.000000 northgravity-0.1.4/README.md
-drwxr-xr-x   0 Izabella   (502) staff       (20)        0 2023-02-08 14:30:53.747939 northgravity-0.1.4/northgravity/
--rw-r--r--   0 Izabella   (502) staff       (20)     1112 2022-12-19 09:32:25.000000 northgravity-0.1.4/northgravity/Authenticator.py
--rw-r--r--   0 Izabella   (502) staff       (20)     9175 2022-12-19 09:32:25.000000 northgravity-0.1.4/northgravity/DatalakeHandler.py
--rw-r--r--   0 Izabella   (502) staff       (20)      309 2023-02-08 13:50:54.000000 northgravity-0.1.4/northgravity/ExceptionHandler.py
--rw-r--r--   0 Izabella   (502) staff       (20)     6567 2022-12-19 09:32:25.000000 northgravity-0.1.4/northgravity/HTTPCalller.py
--rw-r--r--   0 Izabella   (502) staff       (20)     1792 2023-02-08 10:48:38.000000 northgravity-0.1.4/northgravity/StatusHandler.py
--rw-r--r--   0 Izabella   (502) staff       (20)     8501 2022-12-19 09:32:25.000000 northgravity-0.1.4/northgravity/TaskHandler.py
--rw-r--r--   0 Izabella   (502) staff       (20)    13042 2023-02-07 13:45:08.000000 northgravity-0.1.4/northgravity/Timeseries.py
--rw-r--r--   0 Izabella   (502) staff       (20)      567 2023-02-07 14:34:06.000000 northgravity-0.1.4/northgravity/__init__.py
--rw-r--r--   0 Izabella   (502) staff       (20)      122 2023-02-08 14:30:53.000000 northgravity-0.1.4/northgravity/constants.py
-drwxr-xr-x   0 Izabella   (502) staff       (20)        0 2023-02-08 14:30:53.748744 northgravity-0.1.4/northgravity.egg-info/
--rw-r--r--   0 Izabella   (502) staff       (20)    27037 2023-02-08 14:30:53.000000 northgravity-0.1.4/northgravity.egg-info/PKG-INFO
--rw-r--r--   0 Izabella   (502) staff       (20)      464 2023-02-08 14:30:53.000000 northgravity-0.1.4/northgravity.egg-info/SOURCES.txt
--rw-r--r--   0 Izabella   (502) staff       (20)        1 2023-02-08 14:30:53.000000 northgravity-0.1.4/northgravity.egg-info/dependency_links.txt
--rw-r--r--   0 Izabella   (502) staff       (20)       33 2023-02-08 14:30:53.000000 northgravity-0.1.4/northgravity.egg-info/requires.txt
--rw-r--r--   0 Izabella   (502) staff       (20)       13 2023-02-08 14:30:53.000000 northgravity-0.1.4/northgravity.egg-info/top_level.txt
--rw-r--r--   0 Izabella   (502) staff       (20)       38 2023-02-08 14:30:53.749284 northgravity-0.1.4/setup.cfg
--rw-r--r--   0 Izabella   (502) staff       (20)      829 2022-12-19 09:31:57.000000 northgravity-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:32:31.781472 northgravity-0.1.5/
+-rw-rw-r--   0 root         (0) root         (0)     1055 2023-04-18 12:31:14.000000 northgravity-0.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    27037 2023-04-18 12:32:31.781472 northgravity-0.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    26604 2023-04-18 12:32:31.000000 northgravity-0.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:32:31.781472 northgravity-0.1.5/northgravity/
+-rw-rw-r--   0 root         (0) root         (0)     1112 2023-04-18 12:31:14.000000 northgravity-0.1.5/northgravity/Authenticator.py
+-rw-rw-r--   0 root         (0) root         (0)     9175 2023-04-18 12:31:14.000000 northgravity-0.1.5/northgravity/DatalakeHandler.py
+-rw-rw-r--   0 root         (0) root         (0)      309 2023-04-18 12:31:14.000000 northgravity-0.1.5/northgravity/ExceptionHandler.py
+-rw-rw-r--   0 root         (0) root         (0)     6567 2023-04-18 12:31:14.000000 northgravity-0.1.5/northgravity/HTTPCalller.py
+-rw-rw-r--   0 root         (0) root         (0)     1792 2023-04-18 12:31:14.000000 northgravity-0.1.5/northgravity/StatusHandler.py
+-rw-rw-r--   0 root         (0) root         (0)    10261 2023-04-18 12:31:14.000000 northgravity-0.1.5/northgravity/TaskHandler.py
+-rw-rw-r--   0 root         (0) root         (0)    13042 2023-04-18 12:31:14.000000 northgravity-0.1.5/northgravity/Timeseries.py
+-rw-rw-r--   0 root         (0) root         (0)      567 2023-04-18 12:31:14.000000 northgravity-0.1.5/northgravity/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      122 2023-04-18 12:32:31.000000 northgravity-0.1.5/northgravity/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:32:31.781472 northgravity-0.1.5/northgravity.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    27037 2023-04-18 12:32:31.000000 northgravity-0.1.5/northgravity.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2023-04-18 12:32:31.000000 northgravity-0.1.5/northgravity.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 12:32:31.000000 northgravity-0.1.5/northgravity.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-04-18 12:32:31.000000 northgravity-0.1.5/northgravity.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 12:32:31.000000 northgravity-0.1.5/northgravity.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 12:32:31.781472 northgravity-0.1.5/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      829 2023-04-18 12:31:14.000000 northgravity-0.1.5/setup.py
```

### Comparing `northgravity-0.1.4/LICENSE` & `northgravity-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.4/PKG-INFO` & `northgravity-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: northgravity
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python SDK for NorthGravity platform
 Home-page: https://www.northgravity.com/
 Author: NorthGravity
 Author-email: info@northgravity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,19 +39,19 @@
 - **Time Series Handler** - retrieves data directly from the time series database
 
 
 
 ## How to install and set the package: 
 ### Install
 ```text
-pip3 install northgravity==0.1.4
+pip3 install northgravity==0.1.5
 ```
 As the library is available from pip, it can be installed as a specific version within a Python Task from within requirements.txt just by adding:
 ```text
-northgravity==0.1.4
+northgravity==0.1.5
 ```
 The package relies on the requests library so, in the project, the user must install this library in the requirements.txt file.
 ```text
 pip3 install requests==2.25.1
 ```
```

### Comparing `northgravity-0.1.4/README.md` & `northgravity-0.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 - **Time Series Handler** - retrieves data directly from the time series database
 
 
 
 ## How to install and set the package: 
 ### Install
 ```text
-pip3 install northgravity==0.1.4
+pip3 install northgravity==0.1.5
 ```
 As the library is available from pip, it can be installed as a specific version within a Python Task from within requirements.txt just by adding:
 ```text
-northgravity==0.1.4
+northgravity==0.1.5
 ```
 The package relies on the requests library so, in the project, the user must install this library in the requirements.txt file.
 ```text
 pip3 install requests==2.25.1
 ```
```

### Comparing `northgravity-0.1.4/northgravity/Authenticator.py` & `northgravity-0.1.5/northgravity/Authenticator.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.4/northgravity/DatalakeHandler.py` & `northgravity-0.1.5/northgravity/DatalakeHandler.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.4/northgravity/HTTPCalller.py` & `northgravity-0.1.5/northgravity/HTTPCalller.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.4/northgravity/StatusHandler.py` & `northgravity-0.1.5/northgravity/StatusHandler.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.4/northgravity/TaskHandler.py` & `northgravity-0.1.5/northgravity/TaskHandler.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,47 @@
 
 
 class TaskHandler:
     def __init__(self):
         self.pipeline_id = os.environ.get('PIPELINE_ID')
         self.caller = HTTPCaller()
         self.main_path = os.getcwd()
+    
+    # ---------------
+    # GET TASKS
+    # ---------------
+    def get_all_tasks_definitions(self, group_name=None, readable_name=None, category=None, size='all', from_page=0):
+        '''Searching Method to find the task definitions and documentation from management component of the current stage.
+        By default all tasks that can be accessed. 
+        The search can be modified in the query to get tasks from a group, from a category, or a task with a name displayed in the UI.
+        :param: group_name: name of the group in datalake. Accepts '*' as a wild cart in search
+        :param: readableName: name of the task in the UI. Accepts '*' as a wild cart in search
+        :param: category: name of the category in the UI or the backend category from the task_params.json. If '*' is used, the search will be performed on the backend categories.
+        :return: list of json file type elements
+        '''
+        # Prepare query parameters
+        init_query = {"readableName": readable_name, "category": category, "groupName": group_name}
+        query = format_query(init_query)
+
+        task_list = []
+
+        next_from_page=from_page
+        while True:
+            if size == 'all' or size > 1_000:
+                path = f'/mgmt/task?query={query}&size=1000&from={next_from_page}' 
+            else:
+                path = f'/mgmt/task?query={query}&size={size}&from={next_from_page}'
+            response = self.caller.get(path)
+            reponse_json = response.json()
+            task_list.extend(reponse_json['items'])
+            next_from_page += 1_000
+            if (size == 'all' and reponse_json['totalSize'] < next_from_page) or (size != 'all' and size < next_from_page):
+                break
+
+        return task_list
 
     # ---------------
     # BASE METHODS
     # ---------------
     def get_storage_value(self, key):
         '''Read a value from the Storage with a key
         :param: key: the key to get the value from storage
```

### Comparing `northgravity-0.1.4/northgravity/Timeseries.py` & `northgravity-0.1.5/northgravity/Timeseries.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.4/northgravity/__init__.py` & `northgravity-0.1.5/northgravity/__init__.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.4/northgravity.egg-info/PKG-INFO` & `northgravity-0.1.5/northgravity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: northgravity
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python SDK for NorthGravity platform
 Home-page: https://www.northgravity.com/
 Author: NorthGravity
 Author-email: info@northgravity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,19 +39,19 @@
 - **Time Series Handler** - retrieves data directly from the time series database
 
 
 
 ## How to install and set the package: 
 ### Install
 ```text
-pip3 install northgravity==0.1.4
+pip3 install northgravity==0.1.5
 ```
 As the library is available from pip, it can be installed as a specific version within a Python Task from within requirements.txt just by adding:
 ```text
-northgravity==0.1.4
+northgravity==0.1.5
 ```
 The package relies on the requests library so, in the project, the user must install this library in the requirements.txt file.
 ```text
 pip3 install requests==2.25.1
 ```
```

### Comparing `northgravity-0.1.4/setup.py` & `northgravity-0.1.5/setup.py`

 * *Files identical despite different names*

