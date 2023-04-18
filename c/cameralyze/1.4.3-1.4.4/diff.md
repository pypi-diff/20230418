# Comparing `tmp/cameralyze-1.4.3.tar.gz` & `tmp/cameralyze-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cameralyze-1.4.3.tar", last modified: Fri Mar 24 10:45:24 2023, max compression
+gzip compressed data, was "cameralyze-1.4.4.tar", last modified: Tue Apr 18 06:47:44 2023, max compression
```

## Comparing `cameralyze-1.4.3.tar` & `cameralyze-1.4.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-03-24 10:45:24.471152 cameralyze-1.4.3/
--rw-r--r--   0 ufukdag    (501) staff       (20)      279 2023-03-24 10:45:24.470942 cameralyze-1.4.3/PKG-INFO
--rw-r--r--   0 ufukdag    (501) staff       (20)      243 2023-03-22 09:58:11.000000 cameralyze-1.4.3/README.md
-drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-03-24 10:45:24.467884 cameralyze-1.4.3/cameralyze/
--rw-r--r--   0 ufukdag    (501) staff       (20)       26 2023-03-22 09:58:11.000000 cameralyze-1.4.3/cameralyze/__init__.py
--rw-r--r--   0 ufukdag    (501) staff       (20)     3791 2023-03-24 10:45:00.000000 cameralyze-1.4.3/cameralyze/model.py
-drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-03-24 10:45:24.470641 cameralyze-1.4.3/cameralyze.egg-info/
--rw-r--r--   0 ufukdag    (501) staff       (20)      279 2023-03-24 10:45:24.000000 cameralyze-1.4.3/cameralyze.egg-info/PKG-INFO
--rw-r--r--   0 ufukdag    (501) staff       (20)      230 2023-03-24 10:45:24.000000 cameralyze-1.4.3/cameralyze.egg-info/SOURCES.txt
--rw-r--r--   0 ufukdag    (501) staff       (20)        1 2023-03-24 10:45:24.000000 cameralyze-1.4.3/cameralyze.egg-info/dependency_links.txt
--rw-r--r--   0 ufukdag    (501) staff       (20)       33 2023-03-24 10:45:24.000000 cameralyze-1.4.3/cameralyze.egg-info/requires.txt
--rw-r--r--   0 ufukdag    (501) staff       (20)       11 2023-03-24 10:45:24.000000 cameralyze-1.4.3/cameralyze.egg-info/top_level.txt
--rw-r--r--   0 ufukdag    (501) staff       (20)       38 2023-03-24 10:45:24.471226 cameralyze-1.4.3/setup.cfg
--rw-r--r--   0 ufukdag    (501) staff       (20)      558 2023-03-24 10:45:22.000000 cameralyze-1.4.3/setup.py
+drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-04-18 06:47:44.030881 cameralyze-1.4.4/
+-rw-r--r--   0 ufukdag    (501) staff       (20)      279 2023-04-18 06:47:44.030705 cameralyze-1.4.4/PKG-INFO
+-rw-r--r--   0 ufukdag    (501) staff       (20)      243 2023-03-22 09:58:11.000000 cameralyze-1.4.4/README.md
+drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-04-18 06:47:44.029187 cameralyze-1.4.4/cameralyze/
+-rw-r--r--   0 ufukdag    (501) staff       (20)       26 2023-03-22 09:58:11.000000 cameralyze-1.4.4/cameralyze/__init__.py
+-rw-r--r--   0 ufukdag    (501) staff       (20)     4548 2023-04-18 06:45:06.000000 cameralyze-1.4.4/cameralyze/model.py
+drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-04-18 06:47:44.030498 cameralyze-1.4.4/cameralyze.egg-info/
+-rw-r--r--   0 ufukdag    (501) staff       (20)      279 2023-04-18 06:47:43.000000 cameralyze-1.4.4/cameralyze.egg-info/PKG-INFO
+-rw-r--r--   0 ufukdag    (501) staff       (20)      230 2023-04-18 06:47:44.000000 cameralyze-1.4.4/cameralyze.egg-info/SOURCES.txt
+-rw-r--r--   0 ufukdag    (501) staff       (20)        1 2023-04-18 06:47:43.000000 cameralyze-1.4.4/cameralyze.egg-info/dependency_links.txt
+-rw-r--r--   0 ufukdag    (501) staff       (20)       33 2023-04-18 06:47:43.000000 cameralyze-1.4.4/cameralyze.egg-info/requires.txt
+-rw-r--r--   0 ufukdag    (501) staff       (20)       11 2023-04-18 06:47:43.000000 cameralyze-1.4.4/cameralyze.egg-info/top_level.txt
+-rw-r--r--   0 ufukdag    (501) staff       (20)       38 2023-04-18 06:47:44.030940 cameralyze-1.4.4/setup.cfg
+-rw-r--r--   0 ufukdag    (501) staff       (20)      558 2023-04-18 06:47:23.000000 cameralyze-1.4.4/setup.py
```

### Comparing `cameralyze-1.4.3/cameralyze/model.py` & `cameralyze-1.4.4/cameralyze/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import requests
 import filetype
 
-from typing import Union
+from typing import Union, Any
 from uuid import uuid4
 
 
 class Connect:
     def __init__(self, api_key: str = None):
         self.model = None
         self.endpoint = None
         self.background_job = None
         self.flow = None
         self.beautify = False
         self.get_response = True
         self.base_domain = "https://api.server.cameralyze.co"
         self.test_temporary_image_domain = "https://tmp.cameralyze.co"
         self.upload_url = "https://platform.api.cameralyze.com/temporary-file/generate"
+        self.platform_url = "https://platform.cameralyze.co"
         self.api_key = api_key
+        self.configuration = None
         
     def beautify_response(self):
         self.beautify = True
         
         return self
         
     def open_response(self):
@@ -77,48 +79,66 @@
 
         requests.put(
             self.__get_presigned_upload_url(file_type=file_type, file_name=file_name), 
             data=local_file_body, 
             headers={'Content-Type': file_type, 'x-amz-acl': 'public-read'}
         )
 
-    def __get_json(self, image: Union[str, tuple] = None, text:str = None) -> dict:
+    def __get_json(self, image: Union[str, tuple] = None, text:str = None, **kwargs: Any) -> dict:
         json={"apiKey": self.api_key, "rawResponse": not self.beautify, "getResponse": self.get_response}
+        json.update(kwargs)
 
-        if isinstance(image, tuple):
-            json["fileId"] = image[0]
-            json["fileType"] = image[1]
-        elif image.startswith("http"):
-            json["url"] = image
-        elif image != None:
-            json["image"] = image
-        
+        if image != None:
+            if isinstance(image, tuple):
+                json["fileId"] = image[0]
+                json["fileType"] = image[1]
+            elif image.startswith("http"):
+                json["url"] = image
+            elif image != None:
+                json["image"] = image
+            
         if text != None:
             json["text"] = text
             
         if self.endpoint:
             json["applicationUuid"] = self.endpoint
         
         if self.background_job:
             json["applicationUuid"] = self.background_job
         
+        if self.configuration != None:
+            json["configuration"] = self.configuration
+
         return json
     
     def __get_path(self) -> str:
         if self.flow:
             return "flow"
         
         return "model"
     
     def __get_unique_id(self) -> str:
         if self.flow:
             return self.flow
         
         return self.model
 
-    def predict(self, image: Union[str, tuple] = None, text: str = None) -> dict:
+    def predict(self, image: Union[str, tuple] = None, text: str = None, **kwargs: Any) -> dict:
         api_call = requests.post(
             "{base_domain}/{path}/{unique_id}".format(base_domain=self.base_domain, path=self.__get_path(), unique_id=self.__get_unique_id()),
-            json=self.__get_json(image=image, text=text)
+            json=self.__get_json(image=image, text=text, **kwargs)
         )
-
+        print(self.__get_json(image=image, text=text, **kwargs))
         return api_call.json() 
+
+    def show_configuration(self):
+        print(
+            "You can see configuration in here:\n{platform_url}/model-detail/{model}".format(
+                platform_url=self.platform_url,
+                model=self.model
+            )
+        )
+    
+    def set_configuration(self, configuration: dict):
+        self.configuration = configuration
+
+        return self
```

### Comparing `cameralyze-1.4.3/setup.py` & `cameralyze-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.4.3' 
+VERSION = '1.4.4' 
 DESCRIPTION = 'Cameralyze No-Code AI Platform'
 LONG_DESCRIPTION = 'Offical Cameralyze No-Code AI Platform package'
 
 setup(
         name="cameralyze", 
         version=VERSION,
         author="Cameralyze Inc",
```

