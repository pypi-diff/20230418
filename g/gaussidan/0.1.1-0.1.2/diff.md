# Comparing `tmp/gaussidan-0.1.1.tar.gz` & `tmp/gaussidan-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaussidan-0.1.1.tar", max compression
+gzip compressed data, was "gaussidan-0.1.2.tar", max compression
```

## Comparing `gaussidan-0.1.1.tar` & `gaussidan-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      165 2022-11-01 19:26:52.461536 gaussidan-0.1.1/gaussidan/__init__.py
--rw-r--r--   0        0        0     1069 2022-11-01 19:23:14.934802 gaussidan-0.1.1/gaussidan/fit_gaussian.py
--rw-r--r--   0        0        0      659 2022-08-31 14:03:00.107879 gaussidan-0.1.1/gaussidan/plot_gaussian.py
--rw-r--r--   0        0        0      447 2022-11-01 19:30:05.570877 gaussidan-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      626 2022-11-01 19:30:12.646001 gaussidan-0.1.1/setup.py
--rw-r--r--   0        0        0      338 2022-11-01 19:30:12.646250 gaussidan-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      165 2022-11-01 19:26:52.461536 gaussidan-0.1.2/gaussidan/__init__.py
+-rw-r--r--   0        0        0     1069 2022-11-01 19:23:14.934802 gaussidan-0.1.2/gaussidan/fit_gaussian.py
+-rw-r--r--   0        0        0      659 2022-08-31 14:03:00.107879 gaussidan-0.1.2/gaussidan/plot_gaussian.py
+-rw-r--r--   0        0        0      444 2023-04-18 18:41:44.805669 gaussidan-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      625 2023-04-18 18:41:50.603930 gaussidan-0.1.2/setup.py
+-rw-r--r--   0        0        0      537 2023-04-18 18:41:50.604151 gaussidan-0.1.2/PKG-INFO
```

### Comparing `gaussidan-0.1.1/gaussidan/fit_gaussian.py` & `gaussidan-0.1.2/gaussidan/fit_gaussian.py`

 * *Files identical despite different names*

### Comparing `gaussidan-0.1.1/gaussidan/plot_gaussian.py` & `gaussidan-0.1.2/gaussidan/plot_gaussian.py`

 * *Files identical despite different names*

### Comparing `gaussidan-0.1.1/setup.py` & `gaussidan-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['lmfit>=1.0.3,<2.0.0', 'numpy>=1.23.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'gaussidan',
-    'version': '0.1.1',
+    'version': '0.1.2',
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
-    'python_requires': '>=3.10,<3.12',
+    'python_requires': '>=3.6,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

