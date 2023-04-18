# Comparing `tmp/aipha_geo_solutions-0.1.5.tar.gz` & `tmp/aipha_geo_solutions-0.1.6.tar.gz`

## Comparing `aipha_geo_solutions-0.1.5.tar` & `aipha_geo_solutions-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.5/example.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.5/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.5/src/aipha_geo_solutions/__init__.py
--rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.5/src/aipha_geo_solutions/operators.py
--rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.5/src/aipha_geo_solutions/webservice_api.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.5/LICENSE
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.5/README.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.6/example.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.6/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.6/src/aipha_geo_solutions/__init__.py
+-rw-r--r--   0        0        0     9593 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.6/src/aipha_geo_solutions/operators.py
+-rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.6/src/aipha_geo_solutions/webservice_api.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.6/LICENSE
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.6/README.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.6/PKG-INFO
```

### Comparing `aipha_geo_solutions-0.1.5/example.py` & `aipha_geo_solutions-0.1.6/example.py`

 * *Files identical despite different names*

### Comparing `aipha_geo_solutions-0.1.5/src/aipha_geo_solutions/operators.py` & `aipha_geo_solutions-0.1.6/src/aipha_geo_solutions/operators.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,31 +5,178 @@
 import time
 
 def list_running_services(client):
 
   return running_services_request(
         client.get_username(),
         client.get_token(),
-        client.get_server_address(),
-        client.get_verify_ssl())
+        client.get_server_address())
 
 
 def wait_for_completion(client,
   services):
   
   completed = False
   while not completed:
     time.sleep(10)
     completed =  check_services_completed(
         client.get_username(),
         client.get_token(),
         client.get_server_address(),
-        services,
-        client.get_verify_ssl()
-        )
+        services)
+
+
+def point_cloud_classification_inference(client,
+   file_in='file.laz',
+   file_out='classified_file.laz',
+   model_path='model_path',
+   cols_data='x,y,z,intensity',
+   cols_labels='classification'):
+
+  all_parameters = locals().copy()
+  del all_parameters['client']
+  return command_request(
+    client.get_username(),
+    client.get_token(),
+    "point cloud classification inference",
+    all_parameters,
+    client.get_server_address())
+
+
+def convert_laz_point_formats(client,
+   file_in='file.laz',
+   file_out='converted_file.laz',
+   format=7):
+
+  all_parameters = locals().copy()
+  del all_parameters['client']
+  return command_request(
+    client.get_username(),
+    client.get_token(),
+    "convert laz point formats",
+    all_parameters,
+    client.get_server_address())
+
+
+def point_cloud_crop_circle(client,
+   file_in='file.laz',
+   file_out='classified_file.laz',
+   latitude=0,
+   longitude=0,
+   radius=1):
+
+  all_parameters = locals().copy()
+  del all_parameters['client']
+  return command_request(
+    client.get_username(),
+    client.get_token(),
+    "point cloud crop circle",
+    all_parameters,
+    client.get_server_address())
+
+
+def union_point_clouds(client,
+   files_in='file.laz',
+   file_out='converted_file.laz'):
+
+  all_parameters = locals().copy()
+  del all_parameters['client']
+  return command_request(
+    client.get_username(),
+    client.get_token(),
+    "union point clouds",
+    all_parameters,
+    client.get_server_address())
+
+
+def point_cloud_filter_label_noise(client,
+   file_in_data='file.laz',
+   file_in_labels='converted_file.laz',
+   file_out='converted_file.laz',
+   k_nearest_neighbours=5,
+   sigma=10,
+   dim=3,
+   invalid_label=0):
+
+  all_parameters = locals().copy()
+  del all_parameters['client']
+  return command_request(
+    client.get_username(),
+    client.get_token(),
+    "point cloud filter label noise",
+    all_parameters,
+    client.get_server_address())
+
+
+def segment_objects(client,
+   in_points_file='file.laz',
+   in_labels_file='file.laz',
+   out_directory='objects',
+   out_prefix='object',
+   label_col='classification',
+   object_class=6,
+   max_distance=1,
+   min_points=1):
+
+  all_parameters = locals().copy()
+  del all_parameters['client']
+  return command_request(
+    client.get_username(),
+    client.get_token(),
+    "segment objects",
+    all_parameters,
+    client.get_server_address())
+
+
+def select_center_object(client,
+   in_directory='objects',
+   out_file='selected.laz',
+   latitude=1,
+   longitude=1):
+
+  all_parameters = locals().copy()
+  del all_parameters['client']
+  return command_request(
+    client.get_username(),
+    client.get_token(),
+    "select center object",
+    all_parameters,
+    client.get_server_address())
+
+
+def assign_point_labels(client,
+   file_source_in='file.laz',
+   file_labels_in='file.laz',
+   file_source_out='converted_file.laz'):
+
+  all_parameters = locals().copy()
+  del all_parameters['client']
+  return command_request(
+    client.get_username(),
+    client.get_token(),
+    "assign point labels",
+    all_parameters,
+    client.get_server_address())
+
+
+def select_points_by_value(client,
+   file_source_in='file.laz',
+   min_value=1,
+   max_value=1,
+   attribute='classification',
+   file_source_out='selected.laz'):
+
+  all_parameters = locals().copy()
+  del all_parameters['client']
+  return command_request(
+    client.get_username(),
+    client.get_token(),
+    "select points by value",
+    all_parameters,
+    client.get_server_address())
 
 
 def download_data_to_cloud(client,
    url='',
    protocol='',
    username='',
    password='',
@@ -41,17 +188,15 @@
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "download data to cloud",
     all_parameters,
-    client.get_server_address(),
-    client.get_verify_ssl()
-    )
+    client.get_server_address())
 
 
 def upload_data_from_cloud(client,
    url='',
    protocol='',
    username='',
    password='',
@@ -62,71 +207,43 @@
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "upload data from cloud",
     all_parameters,
-    client.get_server_address(),
-    client.get_verify_ssl()
-    )
+    client.get_server_address())
 
 
 def remove_files_from_cloud(client,
    target='/files',
    instance_type='nano'):
 
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "remove files from cloud",
     all_parameters,
-    client.get_server_address(),
-    client.get_verify_ssl()
-    )
+    client.get_server_address())
 
 
 def create_directory_in_cloud(client,
    destination='/files',
    instance_type='nano'):
 
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "create directory in cloud",
     all_parameters,
-    client.get_server_address(),
-    client.get_verify_ssl()
-    )
-
-
-def classify_each_file_in_folder(client,
-   command='classify 3D',
-   command_instance_type='nano',
-   adjustable_in_parameter_name='input_data_path',
-   adjustable_out_parameter_name='output_data_path',
-   input_data_path='/3D_data',
-   in_model_path='/3D_classification_model',
-   output_path='/3D_classification',
-   instance_type='nano'):
-
-  all_parameters = locals().copy()
-  del all_parameters['client']
-  return command_request(
-    client.get_username(),
-    client.get_token(),
-    "classify each file in folder",
-    all_parameters,
-    client.get_server_address(),
-    client.get_verify_ssl()
-    )
+    client.get_server_address())
 
 
 def qc_classification(client,
    project_id='',
    year='2022',
    lidar_new_data_folder='in/',
    out_folder='out/',
@@ -135,17 +252,15 @@
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "qc classification",
     all_parameters,
-    client.get_server_address(),
-    client.get_verify_ssl()
-    )
+    client.get_server_address())
 
 
 def lidar_completeness(client,
    project_id='',
    year='2022',
    lidar_new_data_folder='in/',
    out_folder='out/',
@@ -155,17 +270,15 @@
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "lidar completeness",
     all_parameters,
-    client.get_server_address(),
-    client.get_verify_ssl()
-    )
+    client.get_server_address())
 
 
 def ortho_completeness(client,
    project_id='',
    year='2022',
    orthophoto_folder='in/',
    out_folder='out/',
@@ -175,17 +288,15 @@
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "ortho completeness",
     all_parameters,
-    client.get_server_address(),
-    client.get_verify_ssl()
-    )
+    client.get_server_address())
 
 
 def vegetation_consistency(client,
    project_id='',
    year='2022',
    lidar_old_data_reduced_folder='in/',
    lidar_new_data_reduced_folder='in/',
@@ -195,17 +306,15 @@
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "vegetation consistency",
     all_parameters,
-    client.get_server_address(),
-    client.get_verify_ssl()
-    )
+    client.get_server_address())
 
 
 def generate_orthophoto_subset(client,
    trasse_id='',
    mapping_file='in/',
    orthophoto_path='in/',
    subset_path='out/',
@@ -214,17 +323,15 @@
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "generate orthophoto subset",
     all_parameters,
-    client.get_server_address(),
-    client.get_verify_ssl()
-    )
+    client.get_server_address())
 
 
 def sg_qc_data_processing_init(client,
    ftp_server='',
    ftp_user='',
    ftp_password='',
    ftp_port=21,
@@ -235,17 +342,15 @@
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "sg qc data processing init",
     all_parameters,
-    client.get_server_address(),
-    client.get_verify_ssl()
-    )
+    client.get_server_address())
 
 
 def sg_qc_data_processing(client,
    ftp_server='',
    ftp_user='',
    ftp_password='',
    ftp_port=21,
@@ -257,17 +362,15 @@
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "sg qc data processing",
     all_parameters,
-    client.get_server_address(),
-    client.get_verify_ssl()
-    )
+    client.get_server_address())
 
 
 def tower_displacement(client,
    spatial_reference=2056,
    laz_in_folder_new='laz_folder_new',
    laz_in_folder_old='laz_folder_old',
    laz_in_folder_ref='laz_folder_ref',
@@ -280,42 +383,36 @@
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "tower displacement",
     all_parameters,
-    client.get_server_address(),
-    client.get_verify_ssl()
-    )
+    client.get_server_address())
 
 
 def las2las(client,
    i='file.las',
    o='file.las',
    instance_type='nano'):
 
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "las2las",
     all_parameters,
-    client.get_server_address(),
-    client.get_verify_ssl()
-    )
+    client.get_server_address())
 
 
 def sleep_infinity(client,
    instance_type='nano'):
 
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "sleep infinity",
     all_parameters,
-    client.get_server_address(),
-    client.get_verify_ssl()
-    )
+    client.get_server_address())
```

### Comparing `aipha_geo_solutions-0.1.5/src/aipha_geo_solutions/webservice_api.py` & `aipha_geo_solutions-0.1.6/src/aipha_geo_solutions/webservice_api.py`

 * *Files identical despite different names*

### Comparing `aipha_geo_solutions-0.1.5/LICENSE` & `aipha_geo_solutions-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aipha_geo_solutions-0.1.5/pyproject.toml` & `aipha_geo_solutions-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aipha_geo_solutions"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Timo Hackel", email="timo.hackel@aipha.ch" },
 ]
 description = "A python API to the AIPHA webservices"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
```

### Comparing `aipha_geo_solutions-0.1.5/PKG-INFO` & `aipha_geo_solutions-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aipha_geo_solutions
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python API to the AIPHA webservices
 Project-URL: Homepage, https://github.com/AIPHA-Geo-Solutions/
 Project-URL: Bug Tracker, https://github.com/AIPHA-Geo-Solutions/AIPHAPythonAPI/issues
 Author-email: Timo Hackel <timo.hackel@aipha.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

