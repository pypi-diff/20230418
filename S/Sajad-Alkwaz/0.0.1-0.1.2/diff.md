# Comparing `tmp/Sajad-Alkwaz-0.0.1.tar.gz` & `tmp/Sajad-Alkwaz-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sajad-Alkwaz-0.0.1.tar", last modified: Tue Apr 18 03:12:18 2023, max compression
+gzip compressed data, was "Sajad-Alkwaz-0.1.2.tar", last modified: Tue Apr 18 03:50:57 2023, max compression
```

## Comparing `Sajad-Alkwaz-0.0.1.tar` & `Sajad-Alkwaz-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 03:12:18.601080 Sajad-Alkwaz-0.0.1/
--rw-rw-rw-   0        0        0     1108 2023-04-18 01:03:43.000000 Sajad-Alkwaz-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      402 2023-04-18 03:12:18.601080 Sajad-Alkwaz-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-04-18 02:21:19.000000 Sajad-Alkwaz-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 03:12:18.601080 Sajad-Alkwaz-0.0.1/Sajad_Alkwaz.egg-info/
--rw-rw-rw-   0        0        0      402 2023-04-18 03:12:18.000000 Sajad-Alkwaz-0.0.1/Sajad_Alkwaz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-04-18 03:12:18.000000 Sajad-Alkwaz-0.0.1/Sajad_Alkwaz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 03:12:18.000000 Sajad-Alkwaz-0.0.1/Sajad_Alkwaz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-18 03:12:18.000000 Sajad-Alkwaz-0.0.1/Sajad_Alkwaz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 03:12:18.000000 Sajad-Alkwaz-0.0.1/Sajad_Alkwaz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 03:12:18.601080 Sajad-Alkwaz-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      682 2023-04-18 03:11:52.000000 Sajad-Alkwaz-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 03:50:57.669445 Sajad-Alkwaz-0.1.2/
+-rw-rw-rw-   0        0        0     1108 2023-04-18 01:03:43.000000 Sajad-Alkwaz-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      402 2023-04-18 03:50:57.669445 Sajad-Alkwaz-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-04-18 02:21:19.000000 Sajad-Alkwaz-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 03:50:57.669445 Sajad-Alkwaz-0.1.2/Sajad_Alkwaz.egg-info/
+-rw-rw-rw-   0        0        0      402 2023-04-18 03:50:57.000000 Sajad-Alkwaz-0.1.2/Sajad_Alkwaz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-04-18 03:50:57.000000 Sajad-Alkwaz-0.1.2/Sajad_Alkwaz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 03:50:57.000000 Sajad-Alkwaz-0.1.2/Sajad_Alkwaz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 03:50:57.000000 Sajad-Alkwaz-0.1.2/Sajad_Alkwaz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 03:50:57.669445 Sajad-Alkwaz-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      629 2023-04-18 03:49:10.000000 Sajad-Alkwaz-0.1.2/setup.py
```

### Comparing `Sajad-Alkwaz-0.0.1/LICENSE` & `Sajad-Alkwaz-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Sajad-Alkwaz-0.0.1/setup.py` & `Sajad-Alkwaz-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Sajad-Alkwaz",
-    version="0.0.1",
+    version="0.1.2",
     description="Solve some data analysis problems",
     author="Sajad Beassm",
     author_email="sajad.beassm.bi.2020@uoitc.edu.iq",
     packages=find_packages(),
     readme="README.md",
     requires_python=">=3.7",
-    install_requires=["numpy", "pandas", "scikit-learn"],
+    
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     url="https://github.com/SajadAlkwaz/Sajad-Alkwaz",
     bugtrack_url="https://github.com/pypa/sampleproject/issues"
```

