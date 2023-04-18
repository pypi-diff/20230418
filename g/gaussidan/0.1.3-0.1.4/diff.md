# Comparing `tmp/gaussidan-0.1.3.tar.gz` & `tmp/gaussidan-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaussidan-0.1.3.tar", max compression
+gzip compressed data, was "gaussidan-0.1.4.tar", max compression
```

## Comparing `gaussidan-0.1.3.tar` & `gaussidan-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      165 2022-11-01 19:26:52.461536 gaussidan-0.1.3/gaussidan/__init__.py
--rw-r--r--   0        0        0     1069 2022-11-01 19:23:14.934802 gaussidan-0.1.3/gaussidan/fit_gaussian.py
--rw-r--r--   0        0        0      659 2022-08-31 14:03:00.107879 gaussidan-0.1.3/gaussidan/plot_gaussian.py
--rw-r--r--   0        0        0      443 2023-04-18 19:21:57.635153 gaussidan-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      627 2023-04-18 19:22:02.812139 gaussidan-0.1.3/setup.py
--rw-r--r--   0        0        0      489 2023-04-18 19:22:02.812480 gaussidan-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      165 2022-11-01 19:26:52.461536 gaussidan-0.1.4/gaussidan/__init__.py
+-rw-r--r--   0        0        0     1069 2022-11-01 19:23:14.934802 gaussidan-0.1.4/gaussidan/fit_gaussian.py
+-rw-r--r--   0        0        0      659 2022-08-31 14:03:00.107879 gaussidan-0.1.4/gaussidan/plot_gaussian.py
+-rw-r--r--   0        0        0      442 2023-04-18 19:33:34.454022 gaussidan-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      620 2023-04-18 19:33:40.741807 gaussidan-0.1.4/setup.py
+-rw-r--r--   0        0        0      482 2023-04-18 19:33:40.742055 gaussidan-0.1.4/PKG-INFO
```

### Comparing `gaussidan-0.1.3/gaussidan/fit_gaussian.py` & `gaussidan-0.1.4/gaussidan/fit_gaussian.py`

 * *Files identical despite different names*

### Comparing `gaussidan-0.1.3/gaussidan/plot_gaussian.py` & `gaussidan-0.1.4/gaussidan/plot_gaussian.py`

 * *Files identical despite different names*

### Comparing `gaussidan-0.1.3/setup.py` & `gaussidan-0.1.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['gaussidan']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['lmfit>=1.0.3,<2.0.0', 'numpy>=1.19.0,<2.0.0']
+['lmfit==1.0.2', 'numpy>=1.19.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'gaussidan',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': '',
     'long_description': None,
     'author': 'Daniel Williams',
     'author_email': 'daniel.mays.williams@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

