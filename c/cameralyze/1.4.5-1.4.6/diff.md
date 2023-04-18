# Comparing `tmp/cameralyze-1.4.5.tar.gz` & `tmp/cameralyze-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cameralyze-1.4.5.tar", last modified: Tue Apr 18 06:53:15 2023, max compression
+gzip compressed data, was "cameralyze-1.4.6.tar", last modified: Tue Apr 18 07:23:58 2023, max compression
```

## Comparing `cameralyze-1.4.5.tar` & `cameralyze-1.4.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-04-18 06:53:15.178745 cameralyze-1.4.5/
--rw-r--r--   0 ufukdag    (501) staff       (20)      279 2023-04-18 06:53:15.178562 cameralyze-1.4.5/PKG-INFO
--rw-r--r--   0 ufukdag    (501) staff       (20)      243 2023-03-22 09:58:11.000000 cameralyze-1.4.5/README.md
-drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-04-18 06:53:15.177493 cameralyze-1.4.5/cameralyze/
--rw-r--r--   0 ufukdag    (501) staff       (20)       26 2023-03-22 09:58:11.000000 cameralyze-1.4.5/cameralyze/__init__.py
--rw-r--r--   0 ufukdag    (501) staff       (20)     4484 2023-04-18 06:52:44.000000 cameralyze-1.4.5/cameralyze/model.py
-drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-04-18 06:53:15.178345 cameralyze-1.4.5/cameralyze.egg-info/
--rw-r--r--   0 ufukdag    (501) staff       (20)      279 2023-04-18 06:53:14.000000 cameralyze-1.4.5/cameralyze.egg-info/PKG-INFO
--rw-r--r--   0 ufukdag    (501) staff       (20)      230 2023-04-18 06:53:15.000000 cameralyze-1.4.5/cameralyze.egg-info/SOURCES.txt
--rw-r--r--   0 ufukdag    (501) staff       (20)        1 2023-04-18 06:53:14.000000 cameralyze-1.4.5/cameralyze.egg-info/dependency_links.txt
--rw-r--r--   0 ufukdag    (501) staff       (20)       33 2023-04-18 06:53:15.000000 cameralyze-1.4.5/cameralyze.egg-info/requires.txt
--rw-r--r--   0 ufukdag    (501) staff       (20)       11 2023-04-18 06:53:15.000000 cameralyze-1.4.5/cameralyze.egg-info/top_level.txt
--rw-r--r--   0 ufukdag    (501) staff       (20)       38 2023-04-18 06:53:15.178802 cameralyze-1.4.5/setup.cfg
--rw-r--r--   0 ufukdag    (501) staff       (20)      558 2023-04-18 06:52:40.000000 cameralyze-1.4.5/setup.py
+drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-04-18 07:23:58.587673 cameralyze-1.4.6/
+-rw-r--r--   0 ufukdag    (501) staff       (20)      279 2023-04-18 07:23:58.587498 cameralyze-1.4.6/PKG-INFO
+-rw-r--r--   0 ufukdag    (501) staff       (20)      243 2023-03-22 09:58:11.000000 cameralyze-1.4.6/README.md
+drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-04-18 07:23:58.586483 cameralyze-1.4.6/cameralyze/
+-rw-r--r--   0 ufukdag    (501) staff       (20)       26 2023-03-22 09:58:11.000000 cameralyze-1.4.6/cameralyze/__init__.py
+-rw-r--r--   0 ufukdag    (501) staff       (20)     4473 2023-04-18 07:23:36.000000 cameralyze-1.4.6/cameralyze/model.py
+drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-04-18 07:23:58.587225 cameralyze-1.4.6/cameralyze.egg-info/
+-rw-r--r--   0 ufukdag    (501) staff       (20)      279 2023-04-18 07:23:58.000000 cameralyze-1.4.6/cameralyze.egg-info/PKG-INFO
+-rw-r--r--   0 ufukdag    (501) staff       (20)      230 2023-04-18 07:23:58.000000 cameralyze-1.4.6/cameralyze.egg-info/SOURCES.txt
+-rw-r--r--   0 ufukdag    (501) staff       (20)        1 2023-04-18 07:23:58.000000 cameralyze-1.4.6/cameralyze.egg-info/dependency_links.txt
+-rw-r--r--   0 ufukdag    (501) staff       (20)       33 2023-04-18 07:23:58.000000 cameralyze-1.4.6/cameralyze.egg-info/requires.txt
+-rw-r--r--   0 ufukdag    (501) staff       (20)       11 2023-04-18 07:23:58.000000 cameralyze-1.4.6/cameralyze.egg-info/top_level.txt
+-rw-r--r--   0 ufukdag    (501) staff       (20)       38 2023-04-18 07:23:58.587728 cameralyze-1.4.6/setup.cfg
+-rw-r--r--   0 ufukdag    (501) staff       (20)      558 2023-04-18 07:23:46.000000 cameralyze-1.4.6/setup.py
```

### Comparing `cameralyze-1.4.5/cameralyze/model.py` & `cameralyze-1.4.6/cameralyze/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,16 +80,15 @@
         requests.put(
             self.__get_presigned_upload_url(file_type=file_type, file_name=file_name), 
             data=local_file_body, 
             headers={'Content-Type': file_type, 'x-amz-acl': 'public-read'}
         )
 
     def __get_json(self, image: Union[str, tuple] = None, text:str = None, **kwargs: Any) -> dict:
-        json={"apiKey": self.api_key, "rawResponse": not self.beautify, "getResponse": self.get_response}
-        json.update(kwargs)
+        json={"apiKey": self.api_key, "rawResponse": not self.beautify, "getResponse": self.get_response, "input": kwargs}
 
         if image != None:
             if isinstance(image, tuple):
                 json["fileId"] = image[0]
                 json["fileType"] = image[1]
             elif image.startswith("http"):
                 json["url"] = image
```

### Comparing `cameralyze-1.4.5/setup.py` & `cameralyze-1.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.4.5' 
+VERSION = '1.4.6' 
 DESCRIPTION = 'Cameralyze No-Code AI Platform'
 LONG_DESCRIPTION = 'Offical Cameralyze No-Code AI Platform package'
 
 setup(
         name="cameralyze", 
         version=VERSION,
         author="Cameralyze Inc",
```

