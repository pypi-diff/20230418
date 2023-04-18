# Comparing `tmp/cameralyze-1.4.4.tar.gz` & `tmp/cameralyze-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cameralyze-1.4.4.tar", last modified: Tue Apr 18 06:47:44 2023, max compression
+gzip compressed data, was "cameralyze-1.4.5.tar", last modified: Tue Apr 18 06:53:15 2023, max compression
```

## Comparing `cameralyze-1.4.4.tar` & `cameralyze-1.4.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-04-18 06:47:44.030881 cameralyze-1.4.4/
--rw-r--r--   0 ufukdag    (501) staff       (20)      279 2023-04-18 06:47:44.030705 cameralyze-1.4.4/PKG-INFO
--rw-r--r--   0 ufukdag    (501) staff       (20)      243 2023-03-22 09:58:11.000000 cameralyze-1.4.4/README.md
-drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-04-18 06:47:44.029187 cameralyze-1.4.4/cameralyze/
--rw-r--r--   0 ufukdag    (501) staff       (20)       26 2023-03-22 09:58:11.000000 cameralyze-1.4.4/cameralyze/__init__.py
--rw-r--r--   0 ufukdag    (501) staff       (20)     4548 2023-04-18 06:45:06.000000 cameralyze-1.4.4/cameralyze/model.py
-drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-04-18 06:47:44.030498 cameralyze-1.4.4/cameralyze.egg-info/
--rw-r--r--   0 ufukdag    (501) staff       (20)      279 2023-04-18 06:47:43.000000 cameralyze-1.4.4/cameralyze.egg-info/PKG-INFO
--rw-r--r--   0 ufukdag    (501) staff       (20)      230 2023-04-18 06:47:44.000000 cameralyze-1.4.4/cameralyze.egg-info/SOURCES.txt
--rw-r--r--   0 ufukdag    (501) staff       (20)        1 2023-04-18 06:47:43.000000 cameralyze-1.4.4/cameralyze.egg-info/dependency_links.txt
--rw-r--r--   0 ufukdag    (501) staff       (20)       33 2023-04-18 06:47:43.000000 cameralyze-1.4.4/cameralyze.egg-info/requires.txt
--rw-r--r--   0 ufukdag    (501) staff       (20)       11 2023-04-18 06:47:43.000000 cameralyze-1.4.4/cameralyze.egg-info/top_level.txt
--rw-r--r--   0 ufukdag    (501) staff       (20)       38 2023-04-18 06:47:44.030940 cameralyze-1.4.4/setup.cfg
--rw-r--r--   0 ufukdag    (501) staff       (20)      558 2023-04-18 06:47:23.000000 cameralyze-1.4.4/setup.py
+drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-04-18 06:53:15.178745 cameralyze-1.4.5/
+-rw-r--r--   0 ufukdag    (501) staff       (20)      279 2023-04-18 06:53:15.178562 cameralyze-1.4.5/PKG-INFO
+-rw-r--r--   0 ufukdag    (501) staff       (20)      243 2023-03-22 09:58:11.000000 cameralyze-1.4.5/README.md
+drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-04-18 06:53:15.177493 cameralyze-1.4.5/cameralyze/
+-rw-r--r--   0 ufukdag    (501) staff       (20)       26 2023-03-22 09:58:11.000000 cameralyze-1.4.5/cameralyze/__init__.py
+-rw-r--r--   0 ufukdag    (501) staff       (20)     4484 2023-04-18 06:52:44.000000 cameralyze-1.4.5/cameralyze/model.py
+drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-04-18 06:53:15.178345 cameralyze-1.4.5/cameralyze.egg-info/
+-rw-r--r--   0 ufukdag    (501) staff       (20)      279 2023-04-18 06:53:14.000000 cameralyze-1.4.5/cameralyze.egg-info/PKG-INFO
+-rw-r--r--   0 ufukdag    (501) staff       (20)      230 2023-04-18 06:53:15.000000 cameralyze-1.4.5/cameralyze.egg-info/SOURCES.txt
+-rw-r--r--   0 ufukdag    (501) staff       (20)        1 2023-04-18 06:53:14.000000 cameralyze-1.4.5/cameralyze.egg-info/dependency_links.txt
+-rw-r--r--   0 ufukdag    (501) staff       (20)       33 2023-04-18 06:53:15.000000 cameralyze-1.4.5/cameralyze.egg-info/requires.txt
+-rw-r--r--   0 ufukdag    (501) staff       (20)       11 2023-04-18 06:53:15.000000 cameralyze-1.4.5/cameralyze.egg-info/top_level.txt
+-rw-r--r--   0 ufukdag    (501) staff       (20)       38 2023-04-18 06:53:15.178802 cameralyze-1.4.5/setup.cfg
+-rw-r--r--   0 ufukdag    (501) staff       (20)      558 2023-04-18 06:52:40.000000 cameralyze-1.4.5/setup.py
```

### Comparing `cameralyze-1.4.4/cameralyze/model.py` & `cameralyze-1.4.5/cameralyze/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         return self.model
 
     def predict(self, image: Union[str, tuple] = None, text: str = None, **kwargs: Any) -> dict:
         api_call = requests.post(
             "{base_domain}/{path}/{unique_id}".format(base_domain=self.base_domain, path=self.__get_path(), unique_id=self.__get_unique_id()),
             json=self.__get_json(image=image, text=text, **kwargs)
         )
-        print(self.__get_json(image=image, text=text, **kwargs))
+
         return api_call.json() 
 
     def show_configuration(self):
         print(
             "You can see configuration in here:\n{platform_url}/model-detail/{model}".format(
                 platform_url=self.platform_url,
                 model=self.model
```

### Comparing `cameralyze-1.4.4/setup.py` & `cameralyze-1.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.4.4' 
+VERSION = '1.4.5' 
 DESCRIPTION = 'Cameralyze No-Code AI Platform'
 LONG_DESCRIPTION = 'Offical Cameralyze No-Code AI Platform package'
 
 setup(
         name="cameralyze", 
         version=VERSION,
         author="Cameralyze Inc",
```

