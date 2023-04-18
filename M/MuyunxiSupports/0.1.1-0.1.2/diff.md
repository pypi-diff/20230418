# Comparing `tmp/MuyunxiSupports-0.1.1.tar.gz` & `tmp/MuyunxiSupports-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MuyunxiSupports-0.1.1.tar", last modified: Mon Dec  5 03:01:29 2022, max compression
+gzip compressed data, was "MuyunxiSupports-0.1.2.tar", last modified: Tue Apr 18 12:01:06 2023, max compression
```

## Comparing `MuyunxiSupports-0.1.1.tar` & `MuyunxiSupports-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 muyunxi    (501) staff       (20)        0 2022-12-05 03:01:29.147187 MuyunxiSupports-0.1.1/
-drwxr-xr-x   0 muyunxi    (501) staff       (20)        0 2022-12-05 03:01:29.145944 MuyunxiSupports-0.1.1/MuyunxiSupports/
--rw-r--r--   0 muyunxi    (501) staff       (20)       49 2022-12-05 00:38:25.000000 MuyunxiSupports-0.1.1/MuyunxiSupports/__init__.py
--rw-r--r--   0 muyunxi    (501) staff       (20)     2878 2022-12-04 06:55:38.000000 MuyunxiSupports-0.1.1/MuyunxiSupports/log.py
--rw-r--r--   0 muyunxi    (501) staff       (20)      135 2022-12-05 00:38:19.000000 MuyunxiSupports-0.1.1/MuyunxiSupports/more_sys.py
-drwxr-xr-x   0 muyunxi    (501) staff       (20)        0 2022-12-05 03:01:29.146511 MuyunxiSupports-0.1.1/MuyunxiSupports.egg-info/
--rw-r--r--   0 muyunxi    (501) staff       (20)      250 2022-12-05 03:01:29.000000 MuyunxiSupports-0.1.1/MuyunxiSupports.egg-info/PKG-INFO
--rw-r--r--   0 muyunxi    (501) staff       (20)      253 2022-12-05 03:01:29.000000 MuyunxiSupports-0.1.1/MuyunxiSupports.egg-info/SOURCES.txt
--rw-r--r--   0 muyunxi    (501) staff       (20)        1 2022-12-05 03:01:29.000000 MuyunxiSupports-0.1.1/MuyunxiSupports.egg-info/dependency_links.txt
--rw-r--r--   0 muyunxi    (501) staff       (20)       16 2022-12-05 03:01:29.000000 MuyunxiSupports-0.1.1/MuyunxiSupports.egg-info/top_level.txt
--rw-r--r--   0 muyunxi    (501) staff       (20)      250 2022-12-05 03:01:29.147029 MuyunxiSupports-0.1.1/PKG-INFO
--rw-r--r--   0 muyunxi    (501) staff       (20)        0 2022-12-05 00:40:45.000000 MuyunxiSupports-0.1.1/README.md
--rw-r--r--   0 muyunxi    (501) staff       (20)       38 2022-12-05 03:01:29.147227 MuyunxiSupports-0.1.1/setup.cfg
--rw-r--r--   0 muyunxi    (501) staff       (20)      546 2022-12-05 02:56:30.000000 MuyunxiSupports-0.1.1/setup.py
+drwxr-xr-x   0 muyunxi    (501) staff       (20)        0 2023-04-18 12:01:06.225129 MuyunxiSupports-0.1.2/
+drwxr-xr-x   0 muyunxi    (501) staff       (20)        0 2023-04-18 12:01:06.224198 MuyunxiSupports-0.1.2/MuyunxiSupports.egg-info/
+-rw-r--r--   0 muyunxi    (501) staff       (20)      250 2023-04-18 12:01:06.000000 MuyunxiSupports-0.1.2/MuyunxiSupports.egg-info/PKG-INFO
+-rw-r--r--   0 muyunxi    (501) staff       (20)      227 2023-04-18 12:01:06.000000 MuyunxiSupports-0.1.2/MuyunxiSupports.egg-info/SOURCES.txt
+-rw-r--r--   0 muyunxi    (501) staff       (20)        1 2023-04-18 12:01:06.000000 MuyunxiSupports-0.1.2/MuyunxiSupports.egg-info/dependency_links.txt
+-rw-r--r--   0 muyunxi    (501) staff       (20)        4 2023-04-18 12:01:06.000000 MuyunxiSupports-0.1.2/MuyunxiSupports.egg-info/top_level.txt
+-rw-r--r--   0 muyunxi    (501) staff       (20)      250 2023-04-18 12:01:06.225199 MuyunxiSupports-0.1.2/PKG-INFO
+-rw-r--r--   0 muyunxi    (501) staff       (20)        0 2022-12-05 00:40:45.000000 MuyunxiSupports-0.1.2/README.md
+-rw-r--r--   0 muyunxi    (501) staff       (20)       38 2023-04-18 12:01:06.225440 MuyunxiSupports-0.1.2/setup.cfg
+-rw-r--r--   0 muyunxi    (501) staff       (20)      557 2023-04-18 12:00:34.000000 MuyunxiSupports-0.1.2/setup.py
+drwxr-xr-x   0 muyunxi    (501) staff       (20)        0 2023-04-18 12:01:06.224909 MuyunxiSupports-0.1.2/src/
+-rw-r--r--   0 muyunxi    (501) staff       (20)       49 2022-12-05 00:38:25.000000 MuyunxiSupports-0.1.2/src/__init__.py
+-rw-r--r--   0 muyunxi    (501) staff       (20)     2823 2023-04-18 11:57:26.000000 MuyunxiSupports-0.1.2/src/log.py
+-rw-r--r--   0 muyunxi    (501) staff       (20)      135 2022-12-05 00:38:19.000000 MuyunxiSupports-0.1.2/src/more_sys.py
```

### Comparing `MuyunxiSupports-0.1.1/MuyunxiSupports/log.py` & `MuyunxiSupports-0.1.2/src/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
         self.max_type_length = 16
 
         if os.path.exists(self.log_path):
             pass
         else:
             with open(self.log_path, 'w') as f:
                 pass
-        self.add_log(f'Start to Log "{log_name}" !!!')
 
     def get_time(self, _format='%Y-%m-%d %H:%M:%S'):
         return time.strftime(_format, time.localtime())
 
     def add_log(self, info:str, level:int = 0): # level: 0 普通；1 警告；2 错误；3 致命错误
         if level in self.type.keys():
             current_time = self.get_time()
```

### Comparing `MuyunxiSupports-0.1.1/setup.py` & `MuyunxiSupports-0.1.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 setup (
     name = 'MuyunxiSupports',
-    version = '0.1.1',
+    version = '0.1.2',
     description = '''Muyunxi's some Supports''',
     long_description = open('README.md', 'r').read(),
     include_package_data=True,
     author='Iewnfod',
     author_email='227919512@qq.com',
     maintainer='Iewnfod',
     maintainer_email='227919512@qq.com',
     license='MIT License',
-    packages=['MuyunxiSupports'],
+    packages=find_packages(),
     package_dir={
         'os': 'os',
         'sys': 'sys',
         'time': 'time'
     },
     python_requires = '>=3.7',
     url=''
```

