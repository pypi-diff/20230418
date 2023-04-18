# Comparing `tmp/vaxa_plotly_branding-0.1.0.tar.gz` & `tmp/vaxa_plotly_branding-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vaxa_plotly_branding-0.1.0.tar", max compression
+gzip compressed data, was "vaxa_plotly_branding-0.1.1.tar", max compression
```

## Comparing `vaxa_plotly_branding-0.1.0.tar` & `vaxa_plotly_branding-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       64 2023-03-13 00:33:59.652967 vaxa_plotly_branding-0.1.0/README.md
--rw-r--r--   0        0        0      348 2023-03-13 00:33:15.702355 vaxa_plotly_branding-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      119 2023-03-12 12:15:57.665843 vaxa_plotly_branding-0.1.0/vaxa_plotly_branding/__init__.py
--rw-r--r--   0        0        0   117092 2023-03-12 12:15:57.667012 vaxa_plotly_branding-0.1.0/vaxa_plotly_branding/vaxa_analytics_plot_logo.png
--rw-r--r--   0        0        0     1172 2023-03-12 12:15:57.667164 vaxa_plotly_branding-0.1.0/vaxa_plotly_branding/vaxa_plotly_template.py
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 vaxa_plotly_branding-0.1.0/setup.py
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 vaxa_plotly_branding-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       64 2023-03-13 00:33:59.652967 vaxa_plotly_branding-0.1.1/README.md
+-rw-r--r--   0        0        0      366 2023-04-18 01:23:00.043373 vaxa_plotly_branding-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-03-12 12:15:57.665843 vaxa_plotly_branding-0.1.1/vaxa_plotly_branding/__init__.py
+-rw-r--r--   0        0        0   117092 2023-03-12 12:15:57.667012 vaxa_plotly_branding-0.1.1/vaxa_plotly_branding/vaxa_analytics_plot_logo.png
+-rw-r--r--   0        0        0     1172 2023-03-12 12:15:57.667164 vaxa_plotly_branding-0.1.1/vaxa_plotly_branding/vaxa_plotly_template.py
+-rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 vaxa_plotly_branding-0.1.1/setup.py
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 vaxa_plotly_branding-0.1.1/PKG-INFO
```

### Comparing `vaxa_plotly_branding-0.1.0/vaxa_plotly_branding/vaxa_analytics_plot_logo.png` & `vaxa_plotly_branding-0.1.1/vaxa_plotly_branding/vaxa_analytics_plot_logo.png`

 * *Files identical despite different names*

### Comparing `vaxa_plotly_branding-0.1.0/vaxa_plotly_branding/vaxa_plotly_template.py` & `vaxa_plotly_branding-0.1.1/vaxa_plotly_branding/vaxa_plotly_template.py`

 * *Files identical despite different names*

### Comparing `vaxa_plotly_branding-0.1.0/setup.py` & `vaxa_plotly_branding-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['vaxa_plotly_branding']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['plotly>=5.13.1,<6.0.0']
+['pillow>=9.5.0,<10.0.0', 'plotly>=5.13.1,<6.0.0']
 
 setup_kwargs = {
     'name': 'vaxa-plotly-branding',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': 'Automatically brands Plotly charts with Vaxa Analytics branding.',
     'author': 'Curtis West',
     'author_email': 'curtis@curtiswest.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `vaxa_plotly_branding-0.1.0/PKG-INFO` & `vaxa_plotly_branding-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: vaxa-plotly-branding
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Curtis West
 Author-email: curtis@curtiswest.net
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: plotly (>=5.13.1,<6.0.0)
 Description-Content-Type: text/markdown
 
 Automatically brands Plotly charts with Vaxa Analytics branding.
```

