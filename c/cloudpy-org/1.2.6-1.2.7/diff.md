# Comparing `tmp/cloudpy_org-1.2.6.tar.gz` & `tmp/cloudpy_org-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpy_org-1.2.6.tar", last modified: Fri Apr 14 19:14:04 2023, max compression
+gzip compressed data, was "dist\cloudpy_org-1.2.7.tar", last modified: Tue Apr 18 15:12:49 2023, max compression
```

## Comparing `cloudpy_org-1.2.6.tar` & `cloudpy_org-1.2.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 19:14:04.334997 cloudpy_org-1.2.6/
--rw-rw-rw-   0        0        0      899 2023-04-14 19:14:04.334496 cloudpy_org-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 19:14:04.183958 cloudpy_org-1.2.6/cloudpy_org/
--rw-rw-rw-   0        0        0       46 2023-01-27 10:30:03.000000 cloudpy_org-1.2.6/cloudpy_org/__init__.py
--rw-rw-rw-   0        0        0    46837 2023-04-14 19:05:11.000000 cloudpy_org-1.2.6/cloudpy_org/tools.py
-drwxrwxrwx   0        0        0        0 2023-04-14 19:14:04.304633 cloudpy_org-1.2.6/cloudpy_org.egg-info/
--rw-rw-rw-   0        0        0      899 2023-04-14 19:14:02.000000 cloudpy_org-1.2.6/cloudpy_org.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-04-14 19:14:03.000000 cloudpy_org-1.2.6/cloudpy_org.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 19:14:02.000000 cloudpy_org-1.2.6/cloudpy_org.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-04-14 19:14:02.000000 cloudpy_org-1.2.6/cloudpy_org.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-14 19:14:02.000000 cloudpy_org-1.2.6/cloudpy_org.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 19:14:04.334997 cloudpy_org-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1288 2023-04-14 17:41:26.000000 cloudpy_org-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:12:49.224343 cloudpy_org-1.2.7/
+-rw-rw-rw-   0        0        0      899 2023-04-18 15:12:49.223682 cloudpy_org-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 15:12:49.128670 cloudpy_org-1.2.7/cloudpy_org/
+-rw-rw-rw-   0        0        0       46 2023-01-27 10:30:03.000000 cloudpy_org-1.2.7/cloudpy_org/__init__.py
+-rw-rw-rw-   0        0        0    48754 2023-04-18 15:08:13.000000 cloudpy_org-1.2.7/cloudpy_org/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:12:49.203998 cloudpy_org-1.2.7/cloudpy_org.egg-info/
+-rw-rw-rw-   0        0        0      899 2023-04-18 15:12:47.000000 cloudpy_org-1.2.7/cloudpy_org.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-04-18 15:12:48.000000 cloudpy_org-1.2.7/cloudpy_org.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 15:12:47.000000 cloudpy_org-1.2.7/cloudpy_org.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-04-18 15:12:48.000000 cloudpy_org-1.2.7/cloudpy_org.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-18 15:12:48.000000 cloudpy_org-1.2.7/cloudpy_org.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 15:12:49.224343 cloudpy_org-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1288 2023-04-18 15:08:40.000000 cloudpy_org-1.2.7/setup.py
```

### Comparing `cloudpy_org-1.2.6/PKG-INFO` & `cloudpy_org-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy_org
-Version: 1.2.6
+Version: 1.2.7
 Summary: Cloud data pipeline organization and automation library.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.2.6/cloudpy_org/tools.py` & `cloudpy_org-1.2.7/cloudpy_org/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,15 +247,16 @@
         return self.this_source_code, self.theseparams, self.this_returns, self.this_description
     #██████████████████████████████████████████████████████████████████████████          
 class processing_tools:
     
     def __init__(self,encryptedSession:str='',bucket_name:str=''):
 
         self.sta_bucket,self.environment = '','local'
-        self.local_directory = os.getcwd() + '/'
+        self.__root_path = os.getcwd()
+        self.local_directory = self.__root_path + '/'
         self.s3_bucket = bucket_name.replace('/','') + '/'
         if bucket_name != '':
             self.sta_bucket =  's3://' + bucket_name + '/'
             self.environment = bucket_name
         self.documentation_path = self.local_directory + 'documentation/'
         self.documentation_JSON_path = self.documentation_path + "json/"  
         self.settings = self.sta_bucket + 'settings/'
@@ -988,9 +989,47 @@
                 yearmonths.append(max_yearmonth)
             yearmonths.sort()
             if max_yearmonth < min_yearmonth:
                 print('If max_yearmonth is not provided, it will be current yearmonth by default. Otherwise it must be greater or equal than min_yearmonth.')
         elif min_good == True:
             print('Invalid max_yearmonth input.')
         return yearmonths
-
-            
+    #__________________________________________________________________________
+    
+    def clean_file_name(self,file_name:str,date_id_label:bool=False,time_id_label:bool=False)->str:
+        '''
+        ***
+        Given a file name, returns a clean, lower case, trimmed version of it, with optional date_id and or time_id labels.
+        ***
+        '''
+        ext = file_name[::-1].split('.')[0][::-1].lower().replace(' ','')
+        file_name = file_name.lower().strip().replace(' ','_').replace('.' + ext,'')
+        if date_id_label or time_id_label:
+            date_id,time_id = self.date_time_id()
+            if date_id_label:
+                file_name += '_' + str(date_id)
+            if time_id_label:
+                file_name += '_' + self.fixed_size_int_to_str(time_id,5)
+        file_name += '.' + ext
+        return file_name
+    #__________________________________________________________________________
+    
+    def clean_filepath(self,file_name:str,folder_path:str=None,date_id_label:bool=False,time_id_label:bool=False)->str:
+        '''
+        ***
+        Given a file name, and folder location returns a clean, lower case, trimmed version of it, with optional date_id and or time_id labels.
+        If not folder path is specified, then the local path of the location where the cloudpy_org module is called will be displayed along with the clean file name.
+        ***
+        '''
+        if folder_path == None:
+            folder_path = self.__root_path
+        file_name = self.clean_file_name(
+            file_name=file_name
+            ,date_id_label=date_id_label
+            ,time_id_label=time_id_label)
+        x = ''
+        if len(folder_path) > 1 and folder_path[::-1][0] not in ['/','\\']:
+            x = '/'
+            if '\\' in folder_path:
+                x = '\\'
+        file_path = folder_path + x + file_name
+        return file_path
```

### Comparing `cloudpy_org-1.2.6/cloudpy_org.egg-info/PKG-INFO` & `cloudpy_org-1.2.7/cloudpy_org.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy-org
-Version: 1.2.6
+Version: 1.2.7
 Summary: Cloud data pipeline organization and automation library.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.2.6/setup.py` & `cloudpy_org-1.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from os import path
 
 
 long_description = 'A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.'
 
 setup(
     name="cloudpy_org",
-    version="1.2.6",
+    version="1.2.7",
     description="Cloud data pipeline organization and automation library.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://www.cloudpy.org/",
     author="cloudpy.org",
     author_email="admin@cloudpy.org",
     license="MIT",
```

