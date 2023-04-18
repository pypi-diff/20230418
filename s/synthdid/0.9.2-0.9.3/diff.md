# Comparing `tmp/synthdid-0.9.2.tar.gz` & `tmp/synthdid-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\synthdid-0.9.2.tar", last modified: Tue Apr 18 02:20:34 2023, max compression
+gzip compressed data, was "dist\synthdid-0.9.3.tar", last modified: Tue Apr 18 03:40:11 2023, max compression
```

## Comparing `synthdid-0.9.2.tar` & `synthdid-0.9.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 02:20:34.979720 synthdid-0.9.2/
--rw-rw-rw-   0        0        0      432 2023-04-18 02:20:34.979720 synthdid-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-18 02:20:34.979720 synthdid-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0     1606 2023-04-18 02:20:24.000000 synthdid-0.9.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:20:34.969722 synthdid-0.9.2/synthdid/
--rw-rw-rw-   0        0        0        0 2023-04-17 22:50:30.000000 synthdid-0.9.2/synthdid/__init__.py
--rw-rw-rw-   0        0        0     1701 2023-04-17 22:50:30.000000 synthdid-0.9.2/synthdid/get_data.py
--rw-rw-rw-   0        0        0     3520 2023-04-17 22:50:30.000000 synthdid-0.9.2/synthdid/placebo_simulations.py
--rw-rw-rw-   0        0        0     6127 2023-04-18 02:08:10.000000 synthdid-0.9.2/synthdid/plots.py
--rw-rw-rw-   0        0        0     9303 2023-04-17 22:50:30.000000 synthdid-0.9.2/synthdid/sdid.py
--rw-rw-rw-   0        0        0     5439 2023-04-17 22:50:30.000000 synthdid-0.9.2/synthdid/solver.py
--rw-rw-rw-   0        0        0      410 2023-04-18 01:36:21.000000 synthdid-0.9.2/synthdid/summary.py
--rw-rw-rw-   0        0        0      792 2023-04-18 01:32:26.000000 synthdid-0.9.2/synthdid/synthdid.py
--rw-rw-rw-   0        0        0     3610 2023-04-17 22:50:30.000000 synthdid-0.9.2/synthdid/utils.py
--rw-rw-rw-   0        0        0     5043 2023-04-17 22:50:30.000000 synthdid-0.9.2/synthdid/vcov.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:20:34.978721 synthdid-0.9.2/synthdid.egg-info/
--rw-rw-rw-   0        0        0      432 2023-04-18 02:20:34.000000 synthdid-0.9.2/synthdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-04-18 02:20:34.000000 synthdid-0.9.2/synthdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 02:20:34.000000 synthdid-0.9.2/synthdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      623 2023-04-18 02:20:34.000000 synthdid-0.9.2/synthdid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-18 02:20:34.000000 synthdid-0.9.2/synthdid.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 03:40:11.840140 synthdid-0.9.3/
+-rw-rw-rw-   0        0        0     9195 2023-04-18 03:40:11.839137 synthdid-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-18 03:40:11.840140 synthdid-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     1855 2023-04-18 03:39:49.000000 synthdid-0.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 03:40:11.821134 synthdid-0.9.3/synthdid/
+-rw-rw-rw-   0        0        0        0 2023-04-17 22:50:30.000000 synthdid-0.9.3/synthdid/__init__.py
+-rw-rw-rw-   0        0        0     1701 2023-04-17 22:50:30.000000 synthdid-0.9.3/synthdid/get_data.py
+-rw-rw-rw-   0        0        0     3520 2023-04-17 22:50:30.000000 synthdid-0.9.3/synthdid/placebo_simulations.py
+-rw-rw-rw-   0        0        0     6127 2023-04-18 02:08:10.000000 synthdid-0.9.3/synthdid/plots.py
+-rw-rw-rw-   0        0        0     9303 2023-04-17 22:50:30.000000 synthdid-0.9.3/synthdid/sdid.py
+-rw-rw-rw-   0        0        0     5439 2023-04-17 22:50:30.000000 synthdid-0.9.3/synthdid/solver.py
+-rw-rw-rw-   0        0        0      410 2023-04-18 01:36:21.000000 synthdid-0.9.3/synthdid/summary.py
+-rw-rw-rw-   0        0        0      792 2023-04-18 01:32:26.000000 synthdid-0.9.3/synthdid/synthdid.py
+-rw-rw-rw-   0        0        0     3610 2023-04-17 22:50:30.000000 synthdid-0.9.3/synthdid/utils.py
+-rw-rw-rw-   0        0        0     5043 2023-04-17 22:50:30.000000 synthdid-0.9.3/synthdid/vcov.py
+drwxrwxrwx   0        0        0        0 2023-04-18 03:40:11.838135 synthdid-0.9.3/synthdid.egg-info/
+-rw-rw-rw-   0        0        0     9195 2023-04-18 03:40:11.000000 synthdid-0.9.3/synthdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-04-18 03:40:11.000000 synthdid-0.9.3/synthdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 03:40:11.000000 synthdid-0.9.3/synthdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      623 2023-04-18 03:40:11.000000 synthdid-0.9.3/synthdid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-18 03:40:11.000000 synthdid-0.9.3/synthdid.egg-info/top_level.txt
```

### Comparing `synthdid-0.9.2/setup.py` & `synthdid-0.9.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from setuptools import setup, find_packages
 
+with open("Readme.md", "r", encoding="utf-8") as f:
+    long_description = f.read()
 
 setup(
     dependency_links=[],
     install_requires=[
         "appdirs==1.4.3",
         "attrs==19.1.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
         "black==19.3b0; python_version >= '3.6'",
@@ -27,17 +29,19 @@
         "scipy==1.10.1; python_version >= '3.10' and python_version < '3.12' and platform_system != 'Windows' or platform_machine != 'x86'",
         "six==1.16.0",
         "statsmodels==0.13.5",
         "toml==0.10.0",
         "zipp==3.15.0",
     ],
     name="synthdid",
-    author="D2CML",
-    version="0.9.2",
+    author="D2CML Team, Alexander Quispe, Rodrigo  Grijalba, Jhon Flores, Franco Caceres",
+    version="0.9.3",
     packages=find_packages(),
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     keywords="causal-inference",
     url="https://github.com/d2cml-ai/synthdid.py",
     license="MIT",
     description="Synthdid",
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
```

### Comparing `synthdid-0.9.2/synthdid/get_data.py` & `synthdid-0.9.3/synthdid/get_data.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.2/synthdid/placebo_simulations.py` & `synthdid-0.9.3/synthdid/placebo_simulations.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.2/synthdid/plots.py` & `synthdid-0.9.3/synthdid/plots.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.2/synthdid/sdid.py` & `synthdid-0.9.3/synthdid/sdid.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.2/synthdid/solver.py` & `synthdid-0.9.3/synthdid/solver.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.2/synthdid/synthdid.py` & `synthdid-0.9.3/synthdid/synthdid.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.2/synthdid/utils.py` & `synthdid-0.9.3/synthdid/utils.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.2/synthdid/vcov.py` & `synthdid-0.9.3/synthdid/vcov.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.2/synthdid.egg-info/requires.txt` & `synthdid-0.9.3/synthdid.egg-info/requires.txt`

 * *Files identical despite different names*

