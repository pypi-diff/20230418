# Comparing `tmp/neuro-analysis-py-0.0.1.tar.gz` & `tmp/neuro-analysis-py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro-analysis-py-0.0.1.tar", last modified: Tue Apr 18 20:25:04 2023, max compression
+gzip compressed data, was "neuro-analysis-py-0.0.2.tar", last modified: Tue Apr 18 21:28:57 2023, max compression
```

## Comparing `neuro-analysis-py-0.0.1.tar` & `neuro-analysis-py-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 20:25:04.456104 neuro-analysis-py-0.0.1/
--rw-rw-rw-   0        0        0      326 2023-04-18 20:25:04.456104 neuro-analysis-py-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      889 2023-04-18 20:17:19.000000 neuro-analysis-py-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:25:04.455106 neuro-analysis-py-0.0.1/neuro_analysis_py.egg-info/
--rw-rw-rw-   0        0        0      326 2023-04-18 20:25:04.000000 neuro-analysis-py-0.0.1/neuro_analysis_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-18 20:25:04.000000 neuro-analysis-py-0.0.1/neuro_analysis_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       37 2023-04-18 20:25:04.000000 neuro-analysis-py-0.0.1/neuro_analysis_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-04-18 20:25:04.000000 neuro-analysis-py-0.0.1/neuro_analysis_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-18 20:25:04.000000 neuro-analysis-py-0.0.1/neuro_analysis_py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-18 20:25:04.455106 neuro-analysis-py-0.0.1/neuro_py/
--rw-rw-rw-   0        0        0        0 2023-04-12 15:12:14.000000 neuro-analysis-py-0.0.1/neuro_py/__init__.py
--rw-rw-rw-   0        0        0      115 2023-04-18 20:25:04.457101 neuro-analysis-py-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1121 2023-04-18 20:24:47.000000 neuro-analysis-py-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 21:28:57.302003 neuro-analysis-py-0.0.2/
+-rw-rw-rw-   0        0        0      326 2023-04-18 21:28:57.303000 neuro-analysis-py-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1371 2023-04-18 20:59:09.000000 neuro-analysis-py-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 21:28:57.301005 neuro-analysis-py-0.0.2/neuro_analysis_py.egg-info/
+-rw-rw-rw-   0        0        0      326 2023-04-18 21:28:56.000000 neuro-analysis-py-0.0.2/neuro_analysis_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-18 21:28:57.000000 neuro-analysis-py-0.0.2/neuro_analysis_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       37 2023-04-18 21:28:56.000000 neuro-analysis-py-0.0.2/neuro_analysis_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      181 2023-04-18 21:28:56.000000 neuro-analysis-py-0.0.2/neuro_analysis_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-18 21:28:56.000000 neuro-analysis-py-0.0.2/neuro_analysis_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 21:28:57.302003 neuro-analysis-py-0.0.2/neuro_py/
+-rw-rw-rw-   0        0        0        0 2023-04-12 15:12:14.000000 neuro-analysis-py-0.0.2/neuro_py/__init__.py
+-rw-rw-rw-   0        0        0      115 2023-04-18 21:28:57.311980 neuro-analysis-py-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1090 2023-04-18 21:25:38.000000 neuro-analysis-py-0.0.2/setup.py
```

### Comparing `neuro-analysis-py-0.0.1/setup.py` & `neuro-analysis-py-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from setuptools import find_packages, setup
 
 setup(
     name="neuro-analysis-py",
-    version='0.0.1',
+    version='0.0.2',
     url='https://github.com/ryanharvey1/neuro_py/',
     license='MIT License',
     author='Ryan Harvey',
     author_email='ryanh412@gmail.com',
     description='Analysis of neuroelectrophysiology data in Python.',
     install_requires=['numpy>=1.23.0', 
                     'scipy>=1.9.0', 
                     'matplotlib>=1.5.0', 
                     'dill', 
                     'scikit-learn',
                     'pandas>=1.5.0',
                     'numba>=0.56.0',
                     'pillow>=9.3.0',
                     'track_linearization',
-                    'pickle',
                     'matplotlib',
                     'tqdm>=4.64.0',
                     'joblib>=1.2.0',
                     'pyfftw',
                     'pycircstat',
                     ],
     dependency_links=['https://github.com/ryanharvey1/nelpy'],
```

