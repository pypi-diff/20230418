# Comparing `tmp/gaussidan-0.1.2.tar.gz` & `tmp/gaussidan-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaussidan-0.1.2.tar", max compression
+gzip compressed data, was "gaussidan-0.1.3.tar", max compression
```

## Comparing `gaussidan-0.1.2.tar` & `gaussidan-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      165 2022-11-01 19:26:52.461536 gaussidan-0.1.2/gaussidan/__init__.py
--rw-r--r--   0        0        0     1069 2022-11-01 19:23:14.934802 gaussidan-0.1.2/gaussidan/fit_gaussian.py
--rw-r--r--   0        0        0      659 2022-08-31 14:03:00.107879 gaussidan-0.1.2/gaussidan/plot_gaussian.py
--rw-r--r--   0        0        0      444 2023-04-18 18:41:44.805669 gaussidan-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      625 2023-04-18 18:41:50.603930 gaussidan-0.1.2/setup.py
--rw-r--r--   0        0        0      537 2023-04-18 18:41:50.604151 gaussidan-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      165 2022-11-01 19:26:52.461536 gaussidan-0.1.3/gaussidan/__init__.py
+-rw-r--r--   0        0        0     1069 2022-11-01 19:23:14.934802 gaussidan-0.1.3/gaussidan/fit_gaussian.py
+-rw-r--r--   0        0        0      659 2022-08-31 14:03:00.107879 gaussidan-0.1.3/gaussidan/plot_gaussian.py
+-rw-r--r--   0        0        0      443 2023-04-18 19:21:57.635153 gaussidan-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      627 2023-04-18 19:22:02.812139 gaussidan-0.1.3/setup.py
+-rw-r--r--   0        0        0      489 2023-04-18 19:22:02.812480 gaussidan-0.1.3/PKG-INFO
```

### Comparing `gaussidan-0.1.2/gaussidan/fit_gaussian.py` & `gaussidan-0.1.3/gaussidan/fit_gaussian.py`

 * *Files identical despite different names*

### Comparing `gaussidan-0.1.2/gaussidan/plot_gaussian.py` & `gaussidan-0.1.3/gaussidan/plot_gaussian.py`

 * *Files identical despite different names*

### Comparing `gaussidan-0.1.2/setup.py` & `gaussidan-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 packages = \
 ['gaussidan']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['lmfit>=1.0.3,<2.0.0', 'numpy>=1.23.2,<2.0.0']
+['lmfit>=1.0.3,<2.0.0', 'numpy>=1.19.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'gaussidan',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': '',
     'long_description': None,
     'author': 'Daniel Williams',
     'author_email': 'daniel.mays.williams@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.6,<3.12',
+    'python_requires': '>=3.6.8,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

