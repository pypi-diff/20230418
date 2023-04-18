# Comparing `tmp/recfast4py-0.2.6.tar.gz` & `tmp/recfast4py-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recfast4py-0.2.6.tar", last modified: Tue Apr 18 14:58:21 2023, max compression
+gzip compressed data, was "recfast4py-0.2.7.tar", last modified: Tue Apr 18 15:53:42 2023, max compression
```

## Comparing `recfast4py-0.2.6.tar` & `recfast4py-0.2.7.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 14:58:21.365550 recfast4py-0.2.6/
--rw-r--r--   0 uweschmitt   (501) staff       (20)      164 2017-09-08 11:49:33.000000 recfast4py-0.2.6/AUTHORS.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1569 2017-03-14 15:09:27.000000 recfast4py-0.2.6/CONTRIBUTING.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      314 2017-09-08 11:49:02.000000 recfast4py-0.2.6/HISTORY.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      514 2017-03-14 14:20:31.000000 recfast4py-0.2.6/LICENSE
--rw-r--r--   0 uweschmitt   (501) staff       (20)      246 2023-04-18 14:09:48.000000 recfast4py-0.2.6/MANIFEST.in
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1683 2023-04-18 14:57:39.000000 recfast4py-0.2.6/Makefile
--rw-r--r--   0 uweschmitt   (501) staff       (20)      893 2023-04-18 14:58:21.365418 recfast4py-0.2.6/PKG-INFO
--rw-r--r--   0 uweschmitt   (501) staff       (20)      101 2023-04-18 14:56:34.000000 recfast4py-0.2.6/README.rst
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 14:58:21.361758 recfast4py-0.2.6/docs/
--rw-r--r--   0 uweschmitt   (501) staff       (20)        9 2017-03-14 15:09:54.000000 recfast4py-0.2.6/docs/.gitignore
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6777 2017-03-14 14:59:53.000000 recfast4py-0.2.6/docs/Makefile
--rw-r--r--   0 uweschmitt   (501) staff       (20)       27 2017-03-14 14:59:53.000000 recfast4py-0.2.6/docs/authors.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      515 2017-03-14 14:59:53.000000 recfast4py-0.2.6/docs/check_sphinx.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     8562 2019-05-09 14:45:36.000000 recfast4py-0.2.6/docs/conf.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)       32 2017-03-14 14:59:53.000000 recfast4py-0.2.6/docs/contributing.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)       27 2017-03-14 14:59:53.000000 recfast4py-0.2.6/docs/history.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      607 2017-03-14 14:59:53.000000 recfast4py-0.2.6/docs/index.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      230 2017-03-14 14:59:53.000000 recfast4py-0.2.6/docs/installation.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6466 2017-03-14 14:59:53.000000 recfast4py-0.2.6/docs/make.bat
--rw-r--r--   0 uweschmitt   (501) staff       (20)       67 2017-03-28 12:31:43.000000 recfast4py-0.2.6/docs/modules.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      481 2017-03-28 12:31:43.000000 recfast4py-0.2.6/docs/recfast4py.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      395 2017-03-14 14:59:53.000000 recfast4py-0.2.6/docs/usage.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2013 2023-04-18 14:58:14.000000 recfast4py-0.2.6/pyproject.toml
--rw-r--r--   0 uweschmitt   (501) staff       (20)       38 2023-04-18 14:58:21.365585 recfast4py-0.2.6/setup.cfg
--rw-r--r--   0 uweschmitt   (501) staff       (20)      668 2023-04-18 14:57:27.000000 recfast4py-0.2.6/setup.py
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 14:58:21.358648 recfast4py-0.2.6/src/
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 14:58:21.364391 recfast4py-0.2.6/src/recfast4py/
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     3175 2017-03-14 14:18:01.000000 recfast4py-0.2.6/src/recfast4py/DM_annihilation.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1036 2017-03-14 14:18:01.000000 recfast4py-0.2.6/src/recfast4py/DM_annihilation.Recfast.h
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)    42560 2021-04-16 07:26:49.000000 recfast4py-0.2.6/src/recfast4py/ODE_solver.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2955 2020-02-13 17:11:51.000000 recfast4py-0.2.6/src/recfast4py/ODE_solver.Recfast.h
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     3902 2018-04-10 15:58:01.000000 recfast4py-0.2.6/src/recfast4py/Rec_corrs_CT.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1278 2017-03-14 14:18:01.000000 recfast4py-0.2.6/src/recfast4py/Rec_corrs_CT.Recfast.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)      181 2023-04-18 14:51:17.000000 recfast4py-0.2.6/src/recfast4py/__init__.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)   239221 2022-03-28 14:54:53.000000 recfast4py-0.2.6/src/recfast4py/_recfast.cpp
--rw-r--r--   0 uweschmitt   (501) staff       (20)      789 2022-03-28 14:54:53.000000 recfast4py-0.2.6/src/recfast4py/_recfast.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1738 2023-04-18 14:44:23.000000 recfast4py-0.2.6/src/recfast4py/_recfast.pyx
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     6675 2017-03-14 14:18:01.000000 recfast4py-0.2.6/src/recfast4py/constants.Recfast.h
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2485 2017-03-14 14:18:01.000000 recfast4py-0.2.6/src/recfast4py/cosmology.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1974 2017-03-14 14:18:01.000000 recfast4py-0.2.6/src/recfast4py/cosmology.Recfast.h
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 14:58:21.365106 recfast4py-0.2.6/src/recfast4py/data/
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)    23196 2017-03-14 14:18:01.000000 recfast4py-0.2.6/src/recfast4py/data/DXe_Xe.CT2010.dat
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     8479 2021-04-16 07:26:49.000000 recfast4py-0.2.6/src/recfast4py/evalode.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1627 2017-03-14 14:18:01.000000 recfast4py-0.2.6/src/recfast4py/evalode.Recfast.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1056 2023-04-18 14:44:01.000000 recfast4py-0.2.6/src/recfast4py/recfast.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)      200 2023-04-18 14:51:44.000000 recfast4py-0.2.6/src/recfast4py/recfast4py.py
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)    15164 2020-02-13 17:11:51.000000 recfast4py-0.2.6/src/recfast4py/recombination.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2256 2019-05-09 11:00:46.000000 recfast4py-0.2.6/src/recfast4py/recombination.Recfast.h
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 14:58:21.364980 recfast4py-0.2.6/src/recfast4py.egg-info/
--rw-r--r--   0 uweschmitt   (501) staff       (20)      893 2023-04-18 14:58:21.000000 recfast4py-0.2.6/src/recfast4py.egg-info/PKG-INFO
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1234 2023-04-18 14:58:21.000000 recfast4py-0.2.6/src/recfast4py.egg-info/SOURCES.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2023-04-18 14:58:21.000000 recfast4py-0.2.6/src/recfast4py.egg-info/dependency_links.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)      184 2023-04-18 14:58:21.000000 recfast4py-0.2.6/src/recfast4py.egg-info/requires.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)       11 2023-04-18 14:58:21.000000 recfast4py-0.2.6/src/recfast4py.egg-info/top_level.txt
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 14:58:21.365244 recfast4py-0.2.6/tests/
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1114 2023-04-18 14:51:35.000000 recfast4py-0.2.6/tests/test_recfast4py.py
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 15:53:42.849764 recfast4py-0.2.7/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      164 2017-09-08 11:49:33.000000 recfast4py-0.2.7/AUTHORS.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1569 2017-03-14 15:09:27.000000 recfast4py-0.2.7/CONTRIBUTING.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      314 2017-09-08 11:49:02.000000 recfast4py-0.2.7/HISTORY.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      514 2017-03-14 14:20:31.000000 recfast4py-0.2.7/LICENSE
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      246 2023-04-18 14:09:48.000000 recfast4py-0.2.7/MANIFEST.in
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1683 2023-04-18 14:57:39.000000 recfast4py-0.2.7/Makefile
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      893 2023-04-18 15:53:42.849594 recfast4py-0.2.7/PKG-INFO
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      101 2023-04-18 14:56:34.000000 recfast4py-0.2.7/README.rst
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 15:53:42.842499 recfast4py-0.2.7/docs/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)        9 2017-03-14 15:09:54.000000 recfast4py-0.2.7/docs/.gitignore
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6777 2017-03-14 14:59:53.000000 recfast4py-0.2.7/docs/Makefile
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       27 2017-03-14 14:59:53.000000 recfast4py-0.2.7/docs/authors.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      515 2017-03-14 14:59:53.000000 recfast4py-0.2.7/docs/check_sphinx.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     8562 2019-05-09 14:45:36.000000 recfast4py-0.2.7/docs/conf.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       32 2017-03-14 14:59:53.000000 recfast4py-0.2.7/docs/contributing.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       27 2017-03-14 14:59:53.000000 recfast4py-0.2.7/docs/history.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      607 2017-03-14 14:59:53.000000 recfast4py-0.2.7/docs/index.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      230 2017-03-14 14:59:53.000000 recfast4py-0.2.7/docs/installation.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6466 2017-03-14 14:59:53.000000 recfast4py-0.2.7/docs/make.bat
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       67 2017-03-28 12:31:43.000000 recfast4py-0.2.7/docs/modules.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      481 2017-03-28 12:31:43.000000 recfast4py-0.2.7/docs/recfast4py.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      395 2017-03-14 14:59:53.000000 recfast4py-0.2.7/docs/usage.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2013 2023-04-18 15:53:35.000000 recfast4py-0.2.7/pyproject.toml
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       38 2023-04-18 15:53:42.849803 recfast4py-0.2.7/setup.cfg
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      734 2023-04-18 15:46:42.000000 recfast4py-0.2.7/setup.py
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 15:53:42.838029 recfast4py-0.2.7/src/
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 15:53:42.848060 recfast4py-0.2.7/src/recfast4py/
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     3175 2017-03-14 14:18:01.000000 recfast4py-0.2.7/src/recfast4py/DM_annihilation.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1036 2017-03-14 14:18:01.000000 recfast4py-0.2.7/src/recfast4py/DM_annihilation.Recfast.h
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)    42560 2021-04-16 07:26:49.000000 recfast4py-0.2.7/src/recfast4py/ODE_solver.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2955 2020-02-13 17:11:51.000000 recfast4py-0.2.7/src/recfast4py/ODE_solver.Recfast.h
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     3902 2018-04-10 15:58:01.000000 recfast4py-0.2.7/src/recfast4py/Rec_corrs_CT.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1278 2017-03-14 14:18:01.000000 recfast4py-0.2.7/src/recfast4py/Rec_corrs_CT.Recfast.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      181 2023-04-18 14:51:17.000000 recfast4py-0.2.7/src/recfast4py/__init__.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)   242951 2023-04-18 15:43:50.000000 recfast4py-0.2.7/src/recfast4py/_recfast.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)   243408 2023-04-18 15:53:42.000000 recfast4py-0.2.7/src/recfast4py/_recfast.cpp
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      789 2023-04-18 15:53:42.000000 recfast4py-0.2.7/src/recfast4py/_recfast.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1738 2023-04-18 14:44:23.000000 recfast4py-0.2.7/src/recfast4py/_recfast.pyx
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     6675 2017-03-14 14:18:01.000000 recfast4py-0.2.7/src/recfast4py/constants.Recfast.h
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2485 2017-03-14 14:18:01.000000 recfast4py-0.2.7/src/recfast4py/cosmology.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1974 2017-03-14 14:18:01.000000 recfast4py-0.2.7/src/recfast4py/cosmology.Recfast.h
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 15:53:42.848970 recfast4py-0.2.7/src/recfast4py/data/
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)    23196 2017-03-14 14:18:01.000000 recfast4py-0.2.7/src/recfast4py/data/DXe_Xe.CT2010.dat
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     8479 2021-04-16 07:26:49.000000 recfast4py-0.2.7/src/recfast4py/evalode.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1627 2017-03-14 14:18:01.000000 recfast4py-0.2.7/src/recfast4py/evalode.Recfast.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1056 2023-04-18 14:44:01.000000 recfast4py-0.2.7/src/recfast4py/recfast.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      200 2023-04-18 14:51:44.000000 recfast4py-0.2.7/src/recfast4py/recfast4py.py
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)    15164 2020-02-13 17:11:51.000000 recfast4py-0.2.7/src/recfast4py/recombination.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2256 2019-05-09 11:00:46.000000 recfast4py-0.2.7/src/recfast4py/recombination.Recfast.h
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 15:53:42.848830 recfast4py-0.2.7/src/recfast4py.egg-info/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      893 2023-04-18 15:53:42.000000 recfast4py-0.2.7/src/recfast4py.egg-info/PKG-INFO
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1260 2023-04-18 15:53:42.000000 recfast4py-0.2.7/src/recfast4py.egg-info/SOURCES.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2023-04-18 15:53:42.000000 recfast4py-0.2.7/src/recfast4py.egg-info/dependency_links.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      184 2023-04-18 15:53:42.000000 recfast4py-0.2.7/src/recfast4py.egg-info/requires.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       11 2023-04-18 15:53:42.000000 recfast4py-0.2.7/src/recfast4py.egg-info/top_level.txt
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 15:53:42.849274 recfast4py-0.2.7/tests/
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1114 2023-04-18 14:51:35.000000 recfast4py-0.2.7/tests/test_recfast4py.py
```

### Comparing `recfast4py-0.2.6/CONTRIBUTING.rst` & `recfast4py-0.2.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/LICENSE` & `recfast4py-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/Makefile` & `recfast4py-0.2.7/Makefile`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/PKG-INFO` & `recfast4py-0.2.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recfast4py
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python wrapper for recfast++
 Author-email: Uwe Schmitt <uwe.schmitt@id.ethz.ch>
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `recfast4py-0.2.6/docs/Makefile` & `recfast4py-0.2.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/docs/check_sphinx.py` & `recfast4py-0.2.7/docs/check_sphinx.py`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/docs/conf.py` & `recfast4py-0.2.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/docs/index.rst` & `recfast4py-0.2.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/docs/make.bat` & `recfast4py-0.2.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/pyproject.toml` & `recfast4py-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 40.6.0", "wheel", "numpy", "Cython"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "recfast4py"
-version = "0.2.6"
+version = "0.2.7"
 license = {text = "GPLv3"}
 description = "Python wrapper for recfast++"
 authors = [
     {name = "Uwe Schmitt", email = "uwe.schmitt@id.ethz.ch"},
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `recfast4py-0.2.6/src/recfast4py/DM_annihilation.Recfast.cpp` & `recfast4py-0.2.7/src/recfast4py/DM_annihilation.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/src/recfast4py/DM_annihilation.Recfast.h` & `recfast4py-0.2.7/src/recfast4py/DM_annihilation.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/src/recfast4py/ODE_solver.Recfast.cpp` & `recfast4py-0.2.7/src/recfast4py/ODE_solver.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/src/recfast4py/ODE_solver.Recfast.h` & `recfast4py-0.2.7/src/recfast4py/ODE_solver.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/src/recfast4py/Rec_corrs_CT.Recfast.cpp` & `recfast4py-0.2.7/src/recfast4py/Rec_corrs_CT.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/src/recfast4py/Rec_corrs_CT.Recfast.h` & `recfast4py-0.2.7/src/recfast4py/Rec_corrs_CT.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/src/recfast4py/_recfast.cpp` & `recfast4py-0.2.7/src/recfast4py/_recfast.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,47 @@
-/* Generated by Cython 0.29.28 */
+/* Generated by Cython 0.29.34 */
+
+/* BEGIN: Cython Metadata
+{
+    "distutils": {
+        "depends": [
+            "src/recfast4py/recombination.Recfast.h"
+        ],
+        "extra_compile_args": [
+            "-stdlib=libc++"
+        ],
+        "include_dirs": [
+            "src/recfast4py"
+        ],
+        "name": "recfast4py._recfast",
+        "sources": [
+            "src/recfast4py/_recfast.pyx",
+            "src/recfast4py/cosmology.Recfast.cpp",
+            "src/recfast4py/evalode.Recfast.cpp",
+            "src/recfast4py/recombination.Recfast.cpp",
+            "src/recfast4py/ODE_solver.Recfast.cpp",
+            "src/recfast4py/DM_annihilation.Recfast.cpp",
+            "src/recfast4py/Rec_corrs_CT.Recfast.cpp"
+        ]
+    },
+    "module_name": "recfast4py._recfast"
+}
+END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_28"
-#define CYTHON_HEX_VERSION 0x001D1CF0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -45,14 +72,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -81,18 +109,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -122,18 +154,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -145,15 +226,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -175,31 +256,34 @@
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 0
   #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
@@ -290,41 +374,27 @@
     #if __apple_build_version__ < 7000000
       #undef  CYTHON_FALLTHROUGH
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
 #endif
 
-#ifndef __cplusplus
-  #error "Cython files generated with the C++ option must be compiled with a C++ compiler."
-#endif
 #ifndef CYTHON_INLINE
   #if defined(__clang__)
     #define CYTHON_INLINE __inline__ __attribute__ ((__unused__))
-  #else
+  #elif defined(__GNUC__)
+    #define CYTHON_INLINE __inline__
+  #elif defined(_MSC_VER)
+    #define CYTHON_INLINE __inline
+  #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
+  #else
+    #define CYTHON_INLINE
   #endif
 #endif
-template<typename T>
-void __Pyx_call_destructor(T& x) {
-    x.~T();
-}
-template<typename T>
-class __Pyx_FakeReference {
-  public:
-    __Pyx_FakeReference() : ptr(NULL) { }
-    __Pyx_FakeReference(const T& ref) : ptr(const_cast<T*>(&ref)) { }
-    T *operator->() { return ptr; }
-    T *operator&() { return ptr; }
-    operator T&() { return *ptr; }
-    template<typename U> bool operator ==(U other) { return *ptr == other; }
-    template<typename U> bool operator !=(U other) { return *ptr != other; }
-  private:
-    T *ptr;
-};
 
 #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
   #define Py_OptimizeFlag 0
 #endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
@@ -505,35 +575,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -657,16 +727,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -693,20 +765,20 @@
   #endif
 #endif
 
 #define __PYX_HAVE__recfast4py___recfast
 #define __PYX_HAVE_API__recfast4py___recfast
 /* Early includes */
 #include <string.h>
+#include <stdlib.h>
 #include <string>
 #include "ios"
 #include "new"
 #include "stdexcept"
 #include "typeinfo"
-#include <stdlib.h>
 #include "recombination.Recfast.h"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
@@ -909,37 +981,37 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "recfast4py/_recfast.pyx",
+  "src/recfast4py/_recfast.pyx",
   "stringsource",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_10recfast4py_8_recfast___pyx_scope_struct__recombination;
 struct __pyx_obj_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr;
 
-/* "recfast4py/_recfast.pyx":28
+/* "recfast4py/_recfast.pyx":29
  * 
  * 
  * def recombination(double Yp, double T0, double Om, double Ob, double OL, double Ok, double h100,             # <<<<<<<<<<<<<<
  *                   double Nnu, double F, double fDM, int flag, int npz, double zstart, double zend):
  * 
  */
 struct __pyx_obj_10recfast4py_8_recfast___pyx_scope_struct__recombination {
   PyObject_HEAD
   int __pyx_v_npz;
   double *__pyx_v_results[5];
 };
 
 
-/* "recfast4py/_recfast.pyx":65
+/* "recfast4py/_recfast.pyx":66
  * 
  *     # arrays to lists
  *     result = tuple([results[i][j] for j in range(npz)] for i in range(5))             # <<<<<<<<<<<<<<
  * 
  *     free(results_array)
  */
 struct __pyx_obj_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr {
@@ -1074,14 +1146,20 @@
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
 #if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif // CYTHON_FAST_PYCALL
 #endif
@@ -1180,26 +1258,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1376,22 +1454,22 @@
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
 /* Module declarations from 'libc.string' */
 
-/* Module declarations from 'libcpp.string' */
-
 /* Module declarations from 'libc.stdlib' */
 
+/* Module declarations from 'libcpp.string' */
+
 /* Module declarations from 'recfast4py._recfast' */
 static PyTypeObject *__pyx_ptype_10recfast4py_8_recfast___pyx_scope_struct__recombination = 0;
 static PyTypeObject *__pyx_ptype_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr = 0;
-extern DL_EXPORT(std::string) installPath;
+__PYX_EXTERN_C DL_EXPORT(std::string) installPath;
 static int __pyx_v_10recfast4py_8_recfast_DEBUG;
 static std::string __pyx_convert_string_from_py_std__in_string(PyObject *); /*proto*/
 #define __Pyx_MODULE_NAME "recfast4py._recfast"
 extern int __pyx_module_is_main_recfast4py___recfast;
 int __pyx_module_is_main_recfast4py___recfast = 0;
 
 /* Implementation of 'recfast4py._recfast' */
@@ -1443,15 +1521,15 @@
 static const char __pyx_k_RuntimeError[] = "RuntimeError";
 static const char __pyx_k_DEBUG_RECFAST[] = "DEBUG_RECFAST";
 static const char __pyx_k_recombination[] = "recombination";
 static const char __pyx_k_results_array[] = "results_array";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_recfast4py__recfast[] = "recfast4py._recfast";
 static const char __pyx_k_Xe_frac_returned_code_s[] = "Xe_frac returned code %s";
-static const char __pyx_k_recfast4py__recfast_pyx[] = "recfast4py/_recfast.pyx";
+static const char __pyx_k_src_recfast4py__recfast_pyx[] = "src/recfast4py/_recfast.pyx";
 static const char __pyx_k_recombination_locals_genexpr[] = "recombination.<locals>.genexpr";
 static const char __pyx_k_A_module_to_compute_the_recombin[] = "A module to compute the recombination.\n";
 static PyObject *__pyx_n_s_;
 static PyObject *__pyx_kp_s_A_module_to_compute_the_recombin;
 static PyObject *__pyx_n_s_DEBUG_RECFAST;
 static PyObject *__pyx_n_s_F;
 static PyObject *__pyx_n_s_MemoryError;
@@ -1486,21 +1564,21 @@
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_npz;
 static PyObject *__pyx_n_s_os;
 static PyObject *__pyx_n_s_params;
 static PyObject *__pyx_n_s_path;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_recfast4py__recfast;
-static PyObject *__pyx_kp_s_recfast4py__recfast_pyx;
 static PyObject *__pyx_n_s_recombination;
 static PyObject *__pyx_n_s_recombination_locals_genexpr;
 static PyObject *__pyx_n_s_result;
 static PyObject *__pyx_n_s_results;
 static PyObject *__pyx_n_s_results_array;
 static PyObject *__pyx_n_s_send;
+static PyObject *__pyx_kp_s_src_recfast4py__recfast_pyx;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_throw;
 static PyObject *__pyx_kp_s_utf_8;
 static PyObject *__pyx_n_s_zend;
 static PyObject *__pyx_n_s_zstart;
 static PyObject *__pyx_pf_10recfast4py_8_recfast_13recombination_genexpr(PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_10recfast4py_8_recfast_recombination(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_Yp, double __pyx_v_T0, double __pyx_v_Om, double __pyx_v_Ob, double __pyx_v_OL, double __pyx_v_Ok, double __pyx_v_h100, double __pyx_v_Nnu, double __pyx_v_F, double __pyx_v_fDM, int __pyx_v_flag, int __pyx_v_npz, double __pyx_v_zstart, double __pyx_v_zend); /* proto */
@@ -1508,15 +1586,15 @@
 static PyObject *__pyx_tp_new_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_codeobj__4;
 /* Late includes */
 std::string installPath;
 
-/* "recfast4py/_recfast.pyx":28
+/* "recfast4py/_recfast.pyx":29
  * 
  * 
  * def recombination(double Yp, double T0, double Om, double Ob, double OL, double Ok, double h100,             # <<<<<<<<<<<<<<
  *                   double Nnu, double F, double fDM, int flag, int npz, double zstart, double zend):
  * 
  */
 
@@ -1587,91 +1665,91 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_Yp)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_T0)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 1); __PYX_ERR(0, 28, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 1); __PYX_ERR(0, 29, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_Om)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 2); __PYX_ERR(0, 28, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 2); __PYX_ERR(0, 29, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_Ob)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 3); __PYX_ERR(0, 28, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 3); __PYX_ERR(0, 29, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_OL)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 4); __PYX_ERR(0, 28, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 4); __PYX_ERR(0, 29, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_Ok)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 5); __PYX_ERR(0, 28, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 5); __PYX_ERR(0, 29, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_h100)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 6); __PYX_ERR(0, 28, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 6); __PYX_ERR(0, 29, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_Nnu)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 7); __PYX_ERR(0, 28, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 7); __PYX_ERR(0, 29, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (likely((values[8] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_F)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 8); __PYX_ERR(0, 28, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 8); __PYX_ERR(0, 29, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  9:
         if (likely((values[9] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fDM)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 9); __PYX_ERR(0, 28, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 9); __PYX_ERR(0, 29, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 10:
         if (likely((values[10] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_flag)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 10); __PYX_ERR(0, 28, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 10); __PYX_ERR(0, 29, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 11:
         if (likely((values[11] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_npz)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 11); __PYX_ERR(0, 28, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 11); __PYX_ERR(0, 29, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 12:
         if (likely((values[12] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_zstart)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 12); __PYX_ERR(0, 28, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 12); __PYX_ERR(0, 29, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 13:
         if (likely((values[13] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_zend)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 13); __PYX_ERR(0, 28, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 13); __PYX_ERR(0, 29, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "recombination") < 0)) __PYX_ERR(0, 28, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "recombination") < 0)) __PYX_ERR(0, 29, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 14) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -1683,46 +1761,46 @@
       values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
       values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
       values[10] = PyTuple_GET_ITEM(__pyx_args, 10);
       values[11] = PyTuple_GET_ITEM(__pyx_args, 11);
       values[12] = PyTuple_GET_ITEM(__pyx_args, 12);
       values[13] = PyTuple_GET_ITEM(__pyx_args, 13);
     }
-    __pyx_v_Yp = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_Yp == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 28, __pyx_L3_error)
-    __pyx_v_T0 = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_T0 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 28, __pyx_L3_error)
-    __pyx_v_Om = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_Om == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 28, __pyx_L3_error)
-    __pyx_v_Ob = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_Ob == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 28, __pyx_L3_error)
-    __pyx_v_OL = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_OL == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 28, __pyx_L3_error)
-    __pyx_v_Ok = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_Ok == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 28, __pyx_L3_error)
-    __pyx_v_h100 = __pyx_PyFloat_AsDouble(values[6]); if (unlikely((__pyx_v_h100 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 28, __pyx_L3_error)
-    __pyx_v_Nnu = __pyx_PyFloat_AsDouble(values[7]); if (unlikely((__pyx_v_Nnu == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
-    __pyx_v_F = __pyx_PyFloat_AsDouble(values[8]); if (unlikely((__pyx_v_F == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
-    __pyx_v_fDM = __pyx_PyFloat_AsDouble(values[9]); if (unlikely((__pyx_v_fDM == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
-    __pyx_v_flag = __Pyx_PyInt_As_int(values[10]); if (unlikely((__pyx_v_flag == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
-    __pyx_v_npz = __Pyx_PyInt_As_int(values[11]); if (unlikely((__pyx_v_npz == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
-    __pyx_v_zstart = __pyx_PyFloat_AsDouble(values[12]); if (unlikely((__pyx_v_zstart == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
-    __pyx_v_zend = __pyx_PyFloat_AsDouble(values[13]); if (unlikely((__pyx_v_zend == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
+    __pyx_v_Yp = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_Yp == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
+    __pyx_v_T0 = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_T0 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
+    __pyx_v_Om = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_Om == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
+    __pyx_v_Ob = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_Ob == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
+    __pyx_v_OL = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_OL == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
+    __pyx_v_Ok = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_Ok == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
+    __pyx_v_h100 = __pyx_PyFloat_AsDouble(values[6]); if (unlikely((__pyx_v_h100 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
+    __pyx_v_Nnu = __pyx_PyFloat_AsDouble(values[7]); if (unlikely((__pyx_v_Nnu == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
+    __pyx_v_F = __pyx_PyFloat_AsDouble(values[8]); if (unlikely((__pyx_v_F == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
+    __pyx_v_fDM = __pyx_PyFloat_AsDouble(values[9]); if (unlikely((__pyx_v_fDM == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
+    __pyx_v_flag = __Pyx_PyInt_As_int(values[10]); if (unlikely((__pyx_v_flag == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
+    __pyx_v_npz = __Pyx_PyInt_As_int(values[11]); if (unlikely((__pyx_v_npz == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
+    __pyx_v_zstart = __pyx_PyFloat_AsDouble(values[12]); if (unlikely((__pyx_v_zstart == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
+    __pyx_v_zend = __pyx_PyFloat_AsDouble(values[13]); if (unlikely((__pyx_v_zend == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 28, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 29, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("recfast4py._recfast.recombination", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_10recfast4py_8_recfast_recombination(__pyx_self, __pyx_v_Yp, __pyx_v_T0, __pyx_v_Om, __pyx_v_Ob, __pyx_v_OL, __pyx_v_Ok, __pyx_v_h100, __pyx_v_Nnu, __pyx_v_F, __pyx_v_fDM, __pyx_v_flag, __pyx_v_npz, __pyx_v_zstart, __pyx_v_zend);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_10recfast4py_8_recfast_13recombination_2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "recfast4py/_recfast.pyx":65
+/* "recfast4py/_recfast.pyx":66
  * 
  *     # arrays to lists
  *     result = tuple([results[i][j] for j in range(npz)] for i in range(5))             # <<<<<<<<<<<<<<
  * 
  *     free(results_array)
  */
 
@@ -1734,23 +1812,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr *)__pyx_tp_new_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr(__pyx_ptype_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 65, __pyx_L1_error)
+    __PYX_ERR(0, 66, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_10recfast4py_8_recfast___pyx_scope_struct__recombination *) __pyx_self;
   __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10recfast4py_8_recfast_13recombination_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_recombination_locals_genexpr, __pyx_n_s_recfast4py__recfast); if (unlikely(!gen)) __PYX_ERR(0, 65, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10recfast4py_8_recfast_13recombination_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_recombination_locals_genexpr, __pyx_n_s_recfast4py__recfast); if (unlikely(!gen)) __PYX_ERR(0, 66, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -1781,40 +1859,40 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L8_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 65, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 66, __pyx_L1_error)
   for (__pyx_t_1 = 0; __pyx_t_1 < 5; __pyx_t_1+=1) {
     __pyx_cur_scope->__pyx_v_i = __pyx_t_1;
-    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = __pyx_cur_scope->__pyx_outer_scope->__pyx_v_npz;
     __pyx_t_4 = __pyx_t_3;
     for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
       __pyx_cur_scope->__pyx_v_j = __pyx_t_5;
-      __pyx_t_6 = PyFloat_FromDouble(((__pyx_cur_scope->__pyx_outer_scope->__pyx_v_results[__pyx_cur_scope->__pyx_v_i])[__pyx_cur_scope->__pyx_v_j])); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 65, __pyx_L1_error)
+      __pyx_t_6 = PyFloat_FromDouble(((__pyx_cur_scope->__pyx_outer_scope->__pyx_v_results[__pyx_cur_scope->__pyx_v_i])[__pyx_cur_scope->__pyx_v_j])); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 66, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 65, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 66, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
     __Pyx_XGIVEREF(__pyx_r);
     __Pyx_RefNannyFinishContext();
     __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
     /* return from generator, yielding value */
     __pyx_generator->resume_label = 1;
     return __pyx_r;
     __pyx_L8_resume_from_yield:;
     __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 65, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 66, __pyx_L1_error)
   }
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
   __pyx_L1_error:;
@@ -1828,15 +1906,15 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recfast4py/_recfast.pyx":28
+/* "recfast4py/_recfast.pyx":29
  * 
  * 
  * def recombination(double Yp, double T0, double Om, double Ob, double OL, double Ok, double h100,             # <<<<<<<<<<<<<<
  *                   double Nnu, double F, double fDM, int flag, int npz, double zstart, double zend):
  * 
  */
 
@@ -1858,285 +1936,285 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("recombination", 0);
   __pyx_cur_scope = (struct __pyx_obj_10recfast4py_8_recfast___pyx_scope_struct__recombination *)__pyx_tp_new_10recfast4py_8_recfast___pyx_scope_struct__recombination(__pyx_ptype_10recfast4py_8_recfast___pyx_scope_struct__recombination, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_10recfast4py_8_recfast___pyx_scope_struct__recombination *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 28, __pyx_L1_error)
+    __PYX_ERR(0, 29, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_npz = __pyx_v_npz;
 
-  /* "recfast4py/_recfast.pyx":33
+  /* "recfast4py/_recfast.pyx":34
  *     cdef double[14] params
  * 
  *     params[0] = npz             # <<<<<<<<<<<<<<
  *     params[1] = zstart
  *     params[2] = zend
  */
   (__pyx_v_params[0]) = __pyx_cur_scope->__pyx_v_npz;
 
-  /* "recfast4py/_recfast.pyx":34
+  /* "recfast4py/_recfast.pyx":35
  * 
  *     params[0] = npz
  *     params[1] = zstart             # <<<<<<<<<<<<<<
  *     params[2] = zend
  *     params[3] = Yp
  */
   (__pyx_v_params[1]) = __pyx_v_zstart;
 
-  /* "recfast4py/_recfast.pyx":35
+  /* "recfast4py/_recfast.pyx":36
  *     params[0] = npz
  *     params[1] = zstart
  *     params[2] = zend             # <<<<<<<<<<<<<<
  *     params[3] = Yp
  *     params[4] = T0
  */
   (__pyx_v_params[2]) = __pyx_v_zend;
 
-  /* "recfast4py/_recfast.pyx":36
+  /* "recfast4py/_recfast.pyx":37
  *     params[1] = zstart
  *     params[2] = zend
  *     params[3] = Yp             # <<<<<<<<<<<<<<
  *     params[4] = T0
  *     params[5] = Om
  */
   (__pyx_v_params[3]) = __pyx_v_Yp;
 
-  /* "recfast4py/_recfast.pyx":37
+  /* "recfast4py/_recfast.pyx":38
  *     params[2] = zend
  *     params[3] = Yp
  *     params[4] = T0             # <<<<<<<<<<<<<<
  *     params[5] = Om
  *     params[6] = Ob
  */
   (__pyx_v_params[4]) = __pyx_v_T0;
 
-  /* "recfast4py/_recfast.pyx":38
+  /* "recfast4py/_recfast.pyx":39
  *     params[3] = Yp
  *     params[4] = T0
  *     params[5] = Om             # <<<<<<<<<<<<<<
  *     params[6] = Ob
  *     params[7] = OL
  */
   (__pyx_v_params[5]) = __pyx_v_Om;
 
-  /* "recfast4py/_recfast.pyx":39
+  /* "recfast4py/_recfast.pyx":40
  *     params[4] = T0
  *     params[5] = Om
  *     params[6] = Ob             # <<<<<<<<<<<<<<
  *     params[7] = OL
  *     params[8] = Ok
  */
   (__pyx_v_params[6]) = __pyx_v_Ob;
 
-  /* "recfast4py/_recfast.pyx":40
+  /* "recfast4py/_recfast.pyx":41
  *     params[5] = Om
  *     params[6] = Ob
  *     params[7] = OL             # <<<<<<<<<<<<<<
  *     params[8] = Ok
  *     params[9] = h100
  */
   (__pyx_v_params[7]) = __pyx_v_OL;
 
-  /* "recfast4py/_recfast.pyx":41
+  /* "recfast4py/_recfast.pyx":42
  *     params[6] = Ob
  *     params[7] = OL
  *     params[8] = Ok             # <<<<<<<<<<<<<<
  *     params[9] = h100
  *     params[10] = Nnu
  */
   (__pyx_v_params[8]) = __pyx_v_Ok;
 
-  /* "recfast4py/_recfast.pyx":42
+  /* "recfast4py/_recfast.pyx":43
  *     params[7] = OL
  *     params[8] = Ok
  *     params[9] = h100             # <<<<<<<<<<<<<<
  *     params[10] = Nnu
  *     params[11] = F
  */
   (__pyx_v_params[9]) = __pyx_v_h100;
 
-  /* "recfast4py/_recfast.pyx":43
+  /* "recfast4py/_recfast.pyx":44
  *     params[8] = Ok
  *     params[9] = h100
  *     params[10] = Nnu             # <<<<<<<<<<<<<<
  *     params[11] = F
  *     params[12] = fDM
  */
   (__pyx_v_params[10]) = __pyx_v_Nnu;
 
-  /* "recfast4py/_recfast.pyx":44
+  /* "recfast4py/_recfast.pyx":45
  *     params[9] = h100
  *     params[10] = Nnu
  *     params[11] = F             # <<<<<<<<<<<<<<
  *     params[12] = fDM
  *     params[13] = flag
  */
   (__pyx_v_params[11]) = __pyx_v_F;
 
-  /* "recfast4py/_recfast.pyx":45
+  /* "recfast4py/_recfast.pyx":46
  *     params[10] = Nnu
  *     params[11] = F
  *     params[12] = fDM             # <<<<<<<<<<<<<<
  *     params[13] = flag
  * 
  */
   (__pyx_v_params[12]) = __pyx_v_fDM;
 
-  /* "recfast4py/_recfast.pyx":46
+  /* "recfast4py/_recfast.pyx":47
  *     params[11] = F
  *     params[12] = fDM
  *     params[13] = flag             # <<<<<<<<<<<<<<
  * 
  *     cdef double * results[5]
  */
   (__pyx_v_params[13]) = __pyx_v_flag;
 
-  /* "recfast4py/_recfast.pyx":52
+  /* "recfast4py/_recfast.pyx":53
  *     cdef int i
  * 
  *     results_array = <double *>malloc(npz * 5 * sizeof(double))             # <<<<<<<<<<<<<<
  *     if results_array == NULL:
  *         raise MemoryError()
  */
   __pyx_v_results_array = ((double *)malloc(((__pyx_cur_scope->__pyx_v_npz * 5) * (sizeof(double)))));
 
-  /* "recfast4py/_recfast.pyx":53
+  /* "recfast4py/_recfast.pyx":54
  * 
  *     results_array = <double *>malloc(npz * 5 * sizeof(double))
  *     if results_array == NULL:             # <<<<<<<<<<<<<<
  *         raise MemoryError()
  * 
  */
   __pyx_t_1 = ((__pyx_v_results_array == NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "recfast4py/_recfast.pyx":54
+    /* "recfast4py/_recfast.pyx":55
  *     results_array = <double *>malloc(npz * 5 * sizeof(double))
  *     if results_array == NULL:
  *         raise MemoryError()             # <<<<<<<<<<<<<<
  * 
  *     for i in range(5):
  */
-    PyErr_NoMemory(); __PYX_ERR(0, 54, __pyx_L1_error)
+    PyErr_NoMemory(); __PYX_ERR(0, 55, __pyx_L1_error)
 
-    /* "recfast4py/_recfast.pyx":53
+    /* "recfast4py/_recfast.pyx":54
  * 
  *     results_array = <double *>malloc(npz * 5 * sizeof(double))
  *     if results_array == NULL:             # <<<<<<<<<<<<<<
  *         raise MemoryError()
  * 
  */
   }
 
-  /* "recfast4py/_recfast.pyx":56
+  /* "recfast4py/_recfast.pyx":57
  *         raise MemoryError()
  * 
  *     for i in range(5):             # <<<<<<<<<<<<<<
  *         results[i] = results_array + i * npz
  * 
  */
   for (__pyx_t_2 = 0; __pyx_t_2 < 5; __pyx_t_2+=1) {
     __pyx_v_i = __pyx_t_2;
 
-    /* "recfast4py/_recfast.pyx":57
+    /* "recfast4py/_recfast.pyx":58
  * 
  *     for i in range(5):
  *         results[i] = results_array + i * npz             # <<<<<<<<<<<<<<
  * 
  *     cdef err_code = Xe_frac(params, results[0], results[1], results[2], results[3], results[4], 1, DEBUG)
  */
     (__pyx_cur_scope->__pyx_v_results[__pyx_v_i]) = (__pyx_v_results_array + (__pyx_v_i * __pyx_cur_scope->__pyx_v_npz));
   }
 
-  /* "recfast4py/_recfast.pyx":59
+  /* "recfast4py/_recfast.pyx":60
  *         results[i] = results_array + i * npz
  * 
  *     cdef err_code = Xe_frac(params, results[0], results[1], results[2], results[3], results[4], 1, DEBUG)             # <<<<<<<<<<<<<<
  * 
  *     if err_code:
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(Xe_frac(__pyx_v_params, (__pyx_cur_scope->__pyx_v_results[0]), (__pyx_cur_scope->__pyx_v_results[1]), (__pyx_cur_scope->__pyx_v_results[2]), (__pyx_cur_scope->__pyx_v_results[3]), (__pyx_cur_scope->__pyx_v_results[4]), 1, __pyx_v_10recfast4py_8_recfast_DEBUG)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(Xe_frac(__pyx_v_params, (__pyx_cur_scope->__pyx_v_results[0]), (__pyx_cur_scope->__pyx_v_results[1]), (__pyx_cur_scope->__pyx_v_results[2]), (__pyx_cur_scope->__pyx_v_results[3]), (__pyx_cur_scope->__pyx_v_results[4]), 1, __pyx_v_10recfast4py_8_recfast_DEBUG)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_err_code = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "recfast4py/_recfast.pyx":61
+  /* "recfast4py/_recfast.pyx":62
  *     cdef err_code = Xe_frac(params, results[0], results[1], results[2], results[3], results[4], 1, DEBUG)
  * 
  *     if err_code:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("Xe_frac returned code %s" % err_code)
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_err_code); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 61, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_err_code); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 62, __pyx_L1_error)
   if (unlikely(__pyx_t_1)) {
 
-    /* "recfast4py/_recfast.pyx":62
+    /* "recfast4py/_recfast.pyx":63
  * 
  *     if err_code:
  *         raise RuntimeError("Xe_frac returned code %s" % err_code)             # <<<<<<<<<<<<<<
  * 
  *     # arrays to lists
  */
-    __pyx_t_3 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Xe_frac_returned_code_s, __pyx_v_err_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Xe_frac_returned_code_s, __pyx_v_err_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 63, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 63, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 62, __pyx_L1_error)
+    __PYX_ERR(0, 63, __pyx_L1_error)
 
-    /* "recfast4py/_recfast.pyx":61
+    /* "recfast4py/_recfast.pyx":62
  *     cdef err_code = Xe_frac(params, results[0], results[1], results[2], results[3], results[4], 1, DEBUG)
  * 
  *     if err_code:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("Xe_frac returned code %s" % err_code)
  * 
  */
   }
 
-  /* "recfast4py/_recfast.pyx":65
+  /* "recfast4py/_recfast.pyx":66
  * 
  *     # arrays to lists
  *     result = tuple([results[i][j] for j in range(npz)] for i in range(5))             # <<<<<<<<<<<<<<
  * 
  *     free(results_array)
  */
-  __pyx_t_4 = __pyx_pf_10recfast4py_8_recfast_13recombination_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_4 = __pyx_pf_10recfast4py_8_recfast_13recombination_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PySequence_Tuple(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PySequence_Tuple(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_result = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "recfast4py/_recfast.pyx":67
+  /* "recfast4py/_recfast.pyx":68
  *     result = tuple([results[i][j] for j in range(npz)] for i in range(5))
  * 
  *     free(results_array)             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   free(__pyx_v_results_array);
 
-  /* "recfast4py/_recfast.pyx":69
+  /* "recfast4py/_recfast.pyx":70
  *     free(results_array)
  * 
  *     return result             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "recfast4py/_recfast.pyx":28
+  /* "recfast4py/_recfast.pyx":29
  * 
  * 
  * def recombination(double Yp, double T0, double Om, double Ob, double OL, double Ok, double h100,             # <<<<<<<<<<<<<<
  *                   double Nnu, double F, double fDM, int flag, int npz, double zstart, double zend):
  * 
  */
 
@@ -2508,72 +2586,72 @@
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_npz, __pyx_k_npz, sizeof(__pyx_k_npz), 0, 0, 1, 1},
   {&__pyx_n_s_os, __pyx_k_os, sizeof(__pyx_k_os), 0, 0, 1, 1},
   {&__pyx_n_s_params, __pyx_k_params, sizeof(__pyx_k_params), 0, 0, 1, 1},
   {&__pyx_n_s_path, __pyx_k_path, sizeof(__pyx_k_path), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_recfast4py__recfast, __pyx_k_recfast4py__recfast, sizeof(__pyx_k_recfast4py__recfast), 0, 0, 1, 1},
-  {&__pyx_kp_s_recfast4py__recfast_pyx, __pyx_k_recfast4py__recfast_pyx, sizeof(__pyx_k_recfast4py__recfast_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_recombination, __pyx_k_recombination, sizeof(__pyx_k_recombination), 0, 0, 1, 1},
   {&__pyx_n_s_recombination_locals_genexpr, __pyx_k_recombination_locals_genexpr, sizeof(__pyx_k_recombination_locals_genexpr), 0, 0, 1, 1},
   {&__pyx_n_s_result, __pyx_k_result, sizeof(__pyx_k_result), 0, 0, 1, 1},
   {&__pyx_n_s_results, __pyx_k_results, sizeof(__pyx_k_results), 0, 0, 1, 1},
   {&__pyx_n_s_results_array, __pyx_k_results_array, sizeof(__pyx_k_results_array), 0, 0, 1, 1},
   {&__pyx_n_s_send, __pyx_k_send, sizeof(__pyx_k_send), 0, 0, 1, 1},
+  {&__pyx_kp_s_src_recfast4py__recfast_pyx, __pyx_k_src_recfast4py__recfast_pyx, sizeof(__pyx_k_src_recfast4py__recfast_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_throw, __pyx_k_throw, sizeof(__pyx_k_throw), 0, 0, 1, 1},
   {&__pyx_kp_s_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 0, 1, 0},
   {&__pyx_n_s_zend, __pyx_k_zend, sizeof(__pyx_k_zend), 0, 0, 1, 1},
   {&__pyx_n_s_zstart, __pyx_k_zstart, sizeof(__pyx_k_zstart), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 54, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 56, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 63, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "recfast4py/_recfast.pyx":25
+  /* "recfast4py/_recfast.pyx":26
  * cdef public string installPath = here
  * 
  * cdef int DEBUG = (os.environ.get("DEBUG_RECFAST", "") != "")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_n_s_DEBUG_RECFAST, __pyx_n_s_); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_n_s_DEBUG_RECFAST, __pyx_n_s_); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "recfast4py/_recfast.pyx":28
+  /* "recfast4py/_recfast.pyx":29
  * 
  * 
  * def recombination(double Yp, double T0, double Om, double Ob, double OL, double Ok, double h100,             # <<<<<<<<<<<<<<
  *                   double Nnu, double F, double fDM, int flag, int npz, double zstart, double zend):
  * 
  */
-  __pyx_tuple__3 = PyTuple_Pack(22, __pyx_n_s_Yp, __pyx_n_s_T0, __pyx_n_s_Om, __pyx_n_s_Ob, __pyx_n_s_OL, __pyx_n_s_Ok, __pyx_n_s_h100, __pyx_n_s_Nnu, __pyx_n_s_F, __pyx_n_s_fDM, __pyx_n_s_flag, __pyx_n_s_npz, __pyx_n_s_zstart, __pyx_n_s_zend, __pyx_n_s_params, __pyx_n_s_results, __pyx_n_s_results_array, __pyx_n_s_i, __pyx_n_s_err_code, __pyx_n_s_result, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(22, __pyx_n_s_Yp, __pyx_n_s_T0, __pyx_n_s_Om, __pyx_n_s_Ob, __pyx_n_s_OL, __pyx_n_s_Ok, __pyx_n_s_h100, __pyx_n_s_Nnu, __pyx_n_s_F, __pyx_n_s_fDM, __pyx_n_s_flag, __pyx_n_s_npz, __pyx_n_s_zstart, __pyx_n_s_zend, __pyx_n_s_params, __pyx_n_s_results, __pyx_n_s_results_array, __pyx_n_s_i, __pyx_n_s_err_code, __pyx_n_s_result, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(14, 0, 22, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_recfast4py__recfast_pyx, __pyx_n_s_recombination, 28, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(14, 0, 22, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_recfast4py__recfast_pyx, __pyx_n_s_recombination, 29, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -2610,23 +2688,23 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_10recfast4py_8_recfast___pyx_scope_struct__recombination) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10recfast4py_8_recfast___pyx_scope_struct__recombination) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10recfast4py_8_recfast___pyx_scope_struct__recombination.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10recfast4py_8_recfast___pyx_scope_struct__recombination.tp_dictoffset && __pyx_type_10recfast4py_8_recfast___pyx_scope_struct__recombination.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10recfast4py_8_recfast___pyx_scope_struct__recombination.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_10recfast4py_8_recfast___pyx_scope_struct__recombination = &__pyx_type_10recfast4py_8_recfast___pyx_scope_struct__recombination;
-  if (PyType_Ready(&__pyx_type_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr.tp_dictoffset && __pyx_type_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr = &__pyx_type_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr;
@@ -2830,15 +2908,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_recfast4py___recfast) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -2865,186 +2943,186 @@
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
   /* "recfast4py/_recfast.pyx":4
- * from libc.stdlib cimport malloc, free
+ * from libcpp.string cimport string
  * 
  * import os             # <<<<<<<<<<<<<<
  * 
- * cdef extern from "recombination.Recfast.h":
+ * 
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_os, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_os, __pyx_t_1) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "recfast4py/_recfast.pyx":11
+  /* "recfast4py/_recfast.pyx":12
  * 
  * 
  * __doc__ = "A module to compute the recombination.\n"             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_doc, __pyx_kp_s_A_module_to_compute_the_recombin) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_doc, __pyx_kp_s_A_module_to_compute_the_recombin) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
 
-  /* "recfast4py/_recfast.pyx":15
+  /* "recfast4py/_recfast.pyx":16
  * 
  * # see https://stackoverflow.com/questions/19225188/what-method-can-i-use-instead-of-file-in-python
  * from . import __file__ as __file             # <<<<<<<<<<<<<<
  * 
  * here = os.path.dirname(os.path.abspath(__file))
  */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_file);
   __Pyx_GIVEREF(__pyx_n_s_file);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_file);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_, __pyx_t_1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_, __pyx_t_1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_file); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_file); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_2, __pyx_t_1) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_2, __pyx_t_1) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "recfast4py/_recfast.pyx":17
+  /* "recfast4py/_recfast.pyx":18
  * from . import __file__ as __file
  * 
  * here = os.path.dirname(os.path.abspath(__file))             # <<<<<<<<<<<<<<
  * 
  * if bytes is not str:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_path); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_path); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_dirname); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_dirname); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_os); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_os); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_abspath); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_abspath); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_file_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_file_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_here, __pyx_t_3) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_here, __pyx_t_3) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "recfast4py/_recfast.pyx":19
+  /* "recfast4py/_recfast.pyx":20
  * here = os.path.dirname(os.path.abspath(__file))
  * 
  * if bytes is not str:             # <<<<<<<<<<<<<<
  *     # for python 3
  *     here = bytes(here, "utf-8")
  */
   __pyx_t_5 = ((&PyBytes_Type) != (&PyString_Type));
   __pyx_t_6 = (__pyx_t_5 != 0);
   if (__pyx_t_6) {
 
-    /* "recfast4py/_recfast.pyx":21
+    /* "recfast4py/_recfast.pyx":22
  * if bytes is not str:
  *     # for python 3
  *     here = bytes(here, "utf-8")             # <<<<<<<<<<<<<<
  * 
  * cdef public string installPath = here
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_here); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 21, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_here); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 21, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 22, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
     __Pyx_INCREF(__pyx_kp_s_utf_8);
     __Pyx_GIVEREF(__pyx_kp_s_utf_8);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_kp_s_utf_8);
     __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 21, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_d, __pyx_n_s_here, __pyx_t_3) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_d, __pyx_n_s_here, __pyx_t_3) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "recfast4py/_recfast.pyx":19
+    /* "recfast4py/_recfast.pyx":20
  * here = os.path.dirname(os.path.abspath(__file))
  * 
  * if bytes is not str:             # <<<<<<<<<<<<<<
  *     # for python 3
  *     here = bytes(here, "utf-8")
  */
   }
 
-  /* "recfast4py/_recfast.pyx":23
+  /* "recfast4py/_recfast.pyx":24
  *     here = bytes(here, "utf-8")
  * 
  * cdef public string installPath = here             # <<<<<<<<<<<<<<
  * 
  * cdef int DEBUG = (os.environ.get("DEBUG_RECFAST", "") != "")
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_here); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_here); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __pyx_convert_string_from_py_std__in_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_7 = __pyx_convert_string_from_py_std__in_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   installPath = __pyx_t_7;
 
-  /* "recfast4py/_recfast.pyx":25
+  /* "recfast4py/_recfast.pyx":26
  * cdef public string installPath = here
  * 
  * cdef int DEBUG = (os.environ.get("DEBUG_RECFAST", "") != "")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_environ); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_environ); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_4, __pyx_n_s_, Py_NE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_4, __pyx_n_s_, Py_NE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_10recfast4py_8_recfast_DEBUG = __pyx_t_8;
 
-  /* "recfast4py/_recfast.pyx":28
+  /* "recfast4py/_recfast.pyx":29
  * 
  * 
  * def recombination(double Yp, double T0, double Om, double Ob, double OL, double Ok, double h100,             # <<<<<<<<<<<<<<
  *                   double Nnu, double F, double fDM, int flag, int npz, double zstart, double zend):
  * 
  */
-  __pyx_t_3 = PyCFunction_NewEx(&__pyx_mdef_10recfast4py_8_recfast_1recombination, NULL, __pyx_n_s_recfast4py__recfast); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_3 = PyCFunction_NewEx(&__pyx_mdef_10recfast4py_8_recfast_1recombination, NULL, __pyx_n_s_recfast4py__recfast); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_recombination, __pyx_t_3) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_recombination, __pyx_t_3) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "recfast4py/_recfast.pyx":1
- * from libcpp.string cimport string             # <<<<<<<<<<<<<<
- * from libc.stdlib cimport malloc, free
+ * from libc.stdlib cimport free, malloc             # <<<<<<<<<<<<<<
+ * from libcpp.string cimport string
  * 
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
@@ -3650,28 +3728,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -3854,15 +3932,15 @@
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -3978,14 +4056,20 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -4041,22 +4125,32 @@
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -4931,14 +5025,20 @@
     if (unlikely(!method)) return NULL;
     return __Pyx__PyObject_CallMethod1(method, arg);
 }
 
 /* CoroutineBase */
 #include <structmember.h>
 #include <frameobject.h>
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 #define __Pyx_Coroutine_Undelegate(gen) Py_CLEAR((gen)->yieldfrom)
 static int __Pyx_PyGen__FetchStopIterationValue(CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject **pvalue) {
     PyObject *et, *ev, *tb;
     PyObject *value = NULL;
     __Pyx_ErrFetch(&et, &ev, &tb);
     if (!et) {
         Py_XDECREF(tb);
@@ -5918,19 +6018,41 @@
         return -1;
     }
     return 0;
 }
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
```

### Comparing `recfast4py-0.2.6/src/recfast4py/_recfast.h` & `recfast4py-0.2.7/src/recfast4py/_recfast.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.28 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef __PYX_HAVE__recfast4py___recfast
 #define __PYX_HAVE__recfast4py___recfast
 
 #include "Python.h"
 
 #ifndef __PYX_HAVE_API__recfast4py___recfast
```

### Comparing `recfast4py-0.2.6/src/recfast4py/_recfast.pyx` & `recfast4py-0.2.7/src/recfast4py/_recfast.pyx`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/src/recfast4py/constants.Recfast.h` & `recfast4py-0.2.7/src/recfast4py/constants.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/src/recfast4py/cosmology.Recfast.cpp` & `recfast4py-0.2.7/src/recfast4py/cosmology.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/src/recfast4py/cosmology.Recfast.h` & `recfast4py-0.2.7/src/recfast4py/cosmology.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/src/recfast4py/data/DXe_Xe.CT2010.dat` & `recfast4py-0.2.7/src/recfast4py/data/DXe_Xe.CT2010.dat`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/src/recfast4py/evalode.Recfast.cpp` & `recfast4py-0.2.7/src/recfast4py/evalode.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/src/recfast4py/evalode.Recfast.h` & `recfast4py-0.2.7/src/recfast4py/evalode.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/src/recfast4py/recfast.py` & `recfast4py-0.2.7/src/recfast4py/recfast.py`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/src/recfast4py/recombination.Recfast.cpp` & `recfast4py-0.2.7/src/recfast4py/recombination.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/src/recfast4py/recombination.Recfast.h` & `recfast4py-0.2.7/src/recfast4py/recombination.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.6/src/recfast4py.egg-info/PKG-INFO` & `recfast4py-0.2.7/src/recfast4py.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recfast4py
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python wrapper for recfast++
 Author-email: Uwe Schmitt <uwe.schmitt@id.ethz.ch>
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `recfast4py-0.2.6/src/recfast4py.egg-info/SOURCES.txt` & `recfast4py-0.2.7/src/recfast4py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 src/recfast4py/DM_annihilation.Recfast.cpp
 src/recfast4py/DM_annihilation.Recfast.h
 src/recfast4py/ODE_solver.Recfast.cpp
 src/recfast4py/ODE_solver.Recfast.h
 src/recfast4py/Rec_corrs_CT.Recfast.cpp
 src/recfast4py/Rec_corrs_CT.Recfast.h
 src/recfast4py/__init__.py
+src/recfast4py/_recfast.c
 src/recfast4py/_recfast.cpp
 src/recfast4py/_recfast.h
 src/recfast4py/_recfast.pyx
 src/recfast4py/constants.Recfast.h
 src/recfast4py/cosmology.Recfast.cpp
 src/recfast4py/cosmology.Recfast.h
 src/recfast4py/evalode.Recfast.cpp
```

### Comparing `recfast4py-0.2.6/tests/test_recfast4py.py` & `recfast4py-0.2.7/tests/test_recfast4py.py`

 * *Files identical despite different names*

