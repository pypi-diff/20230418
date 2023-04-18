# Comparing `tmp/recfast4py-0.2.4.tar.gz` & `tmp/recfast4py-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recfast4py-0.2.4.tar", last modified: Mon Mar 28 14:54:53 2022, max compression
+gzip compressed data, was "recfast4py-0.2.5.tar", last modified: Tue Apr 18 13:42:35 2023, max compression
```

## Comparing `recfast4py-0.2.4.tar` & `recfast4py-0.2.5.tar`

### file list

```diff
@@ -1,54 +1,59 @@
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2022-03-28 14:54:53.253433 recfast4py-0.2.4/
--rw-r--r--   0 uweschmitt   (501) staff       (20)      164 2017-09-08 11:49:33.000000 recfast4py-0.2.4/AUTHORS.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1569 2017-03-14 15:09:27.000000 recfast4py-0.2.4/CONTRIBUTING.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      314 2017-09-08 11:49:02.000000 recfast4py-0.2.4/HISTORY.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      514 2017-03-14 14:20:31.000000 recfast4py-0.2.4/LICENSE
--rw-r--r--   0 uweschmitt   (501) staff       (20)      217 2018-10-10 12:37:16.000000 recfast4py-0.2.4/MANIFEST.in
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1478 2017-03-21 13:34:04.000000 recfast4py-0.2.4/Makefile
--rw-r--r--   0 uweschmitt   (501) staff       (20)      870 2022-03-28 14:54:53.253283 recfast4py-0.2.4/PKG-INFO
--rw-r--r--   0 uweschmitt   (501) staff       (20)      130 2017-03-14 14:17:40.000000 recfast4py-0.2.4/README.rst
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2022-03-28 14:54:53.247916 recfast4py-0.2.4/docs/
--rw-r--r--   0 uweschmitt   (501) staff       (20)        9 2017-03-14 15:09:54.000000 recfast4py-0.2.4/docs/.gitignore
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6777 2017-03-14 14:59:53.000000 recfast4py-0.2.4/docs/Makefile
--rw-r--r--   0 uweschmitt   (501) staff       (20)       27 2017-03-14 14:59:53.000000 recfast4py-0.2.4/docs/authors.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      515 2017-03-14 14:59:53.000000 recfast4py-0.2.4/docs/check_sphinx.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     8562 2019-05-09 14:45:36.000000 recfast4py-0.2.4/docs/conf.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)       32 2017-03-14 14:59:53.000000 recfast4py-0.2.4/docs/contributing.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)       27 2017-03-14 14:59:53.000000 recfast4py-0.2.4/docs/history.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      607 2017-03-14 14:59:53.000000 recfast4py-0.2.4/docs/index.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      230 2017-03-14 14:59:53.000000 recfast4py-0.2.4/docs/installation.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6466 2017-03-14 14:59:53.000000 recfast4py-0.2.4/docs/make.bat
--rw-r--r--   0 uweschmitt   (501) staff       (20)       67 2017-03-28 12:31:43.000000 recfast4py-0.2.4/docs/modules.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      481 2017-03-28 12:31:43.000000 recfast4py-0.2.4/docs/recfast4py.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      395 2017-03-14 14:59:53.000000 recfast4py-0.2.4/docs/usage.rst
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2022-03-28 14:54:53.252182 recfast4py-0.2.4/recfast4py/
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     3175 2017-03-14 14:18:01.000000 recfast4py-0.2.4/recfast4py/DM_annihilation.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1036 2017-03-14 14:18:01.000000 recfast4py-0.2.4/recfast4py/DM_annihilation.Recfast.h
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)    42560 2021-04-16 07:26:49.000000 recfast4py-0.2.4/recfast4py/ODE_solver.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2955 2020-02-13 17:11:51.000000 recfast4py-0.2.4/recfast4py/ODE_solver.Recfast.h
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     3902 2018-04-10 15:58:01.000000 recfast4py-0.2.4/recfast4py/Rec_corrs_CT.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1278 2017-03-14 14:18:01.000000 recfast4py-0.2.4/recfast4py/Rec_corrs_CT.Recfast.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)      191 2018-08-15 14:00:23.000000 recfast4py-0.2.4/recfast4py/__init__.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)   239221 2022-03-28 14:54:53.000000 recfast4py-0.2.4/recfast4py/_recfast.cpp
--rw-r--r--   0 uweschmitt   (501) staff       (20)      789 2022-03-28 14:54:53.000000 recfast4py-0.2.4/recfast4py/_recfast.h
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     6675 2017-03-14 14:18:01.000000 recfast4py-0.2.4/recfast4py/constants.Recfast.h
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2485 2017-03-14 14:18:01.000000 recfast4py-0.2.4/recfast4py/cosmology.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1974 2017-03-14 14:18:01.000000 recfast4py-0.2.4/recfast4py/cosmology.Recfast.h
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2022-03-28 14:54:53.253015 recfast4py-0.2.4/recfast4py/data/
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)    23196 2017-03-14 14:18:01.000000 recfast4py-0.2.4/recfast4py/data/DXe_Xe.CT2010.dat
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     8479 2021-04-16 07:26:49.000000 recfast4py-0.2.4/recfast4py/evalode.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1627 2017-03-14 14:18:01.000000 recfast4py-0.2.4/recfast4py/evalode.Recfast.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1022 2017-03-21 11:08:15.000000 recfast4py-0.2.4/recfast4py/recfast.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)      227 2017-03-14 14:17:40.000000 recfast4py-0.2.4/recfast4py/recfast4py.py
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)    15164 2020-02-13 17:11:51.000000 recfast4py-0.2.4/recfast4py/recombination.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2256 2019-05-09 11:00:46.000000 recfast4py-0.2.4/recfast4py/recombination.Recfast.h
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2022-03-28 14:54:53.252908 recfast4py-0.2.4/recfast4py.egg-info/
--rw-r--r--   0 uweschmitt   (501) staff       (20)      870 2022-03-28 14:54:53.000000 recfast4py-0.2.4/recfast4py.egg-info/PKG-INFO
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1120 2022-03-28 14:54:53.000000 recfast4py-0.2.4/recfast4py.egg-info/SOURCES.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2022-03-28 14:54:53.000000 recfast4py-0.2.4/recfast4py.egg-info/dependency_links.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2020-02-13 17:14:41.000000 recfast4py-0.2.4/recfast4py.egg-info/not-zip-safe
--rw-r--r--   0 uweschmitt   (501) staff       (20)        6 2022-03-28 14:54:53.000000 recfast4py-0.2.4/recfast4py.egg-info/requires.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)       11 2022-03-28 14:54:53.000000 recfast4py-0.2.4/recfast4py.egg-info/top_level.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)      170 2019-05-09 10:27:13.000000 recfast4py-0.2.4/requirements.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)       38 2022-03-28 14:54:53.253477 recfast4py-0.2.4/setup.cfg
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2449 2022-03-28 14:54:47.000000 recfast4py-0.2.4/setup.py
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 13:42:35.714640 recfast4py-0.2.5/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      164 2017-09-08 11:49:33.000000 recfast4py-0.2.5/AUTHORS.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1569 2017-03-14 15:09:27.000000 recfast4py-0.2.5/CONTRIBUTING.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      314 2017-09-08 11:49:02.000000 recfast4py-0.2.5/HISTORY.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      514 2017-03-14 14:20:31.000000 recfast4py-0.2.5/LICENSE
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      246 2023-04-18 13:41:29.000000 recfast4py-0.2.5/MANIFEST.in
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1673 2023-04-18 13:40:26.000000 recfast4py-0.2.5/Makefile
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1134 2023-04-18 13:42:35.714745 recfast4py-0.2.5/PKG-INFO
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      130 2017-03-14 14:17:40.000000 recfast4py-0.2.5/README.rst
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 13:42:35.710770 recfast4py-0.2.5/docs/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)        9 2017-03-14 15:09:54.000000 recfast4py-0.2.5/docs/.gitignore
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6777 2017-03-14 14:59:53.000000 recfast4py-0.2.5/docs/Makefile
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       27 2017-03-14 14:59:53.000000 recfast4py-0.2.5/docs/authors.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      515 2017-03-14 14:59:53.000000 recfast4py-0.2.5/docs/check_sphinx.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     8562 2019-05-09 14:45:36.000000 recfast4py-0.2.5/docs/conf.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       32 2017-03-14 14:59:53.000000 recfast4py-0.2.5/docs/contributing.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       27 2017-03-14 14:59:53.000000 recfast4py-0.2.5/docs/history.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      607 2017-03-14 14:59:53.000000 recfast4py-0.2.5/docs/index.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      230 2017-03-14 14:59:53.000000 recfast4py-0.2.5/docs/installation.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6466 2017-03-14 14:59:53.000000 recfast4py-0.2.5/docs/make.bat
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       67 2017-03-28 12:31:43.000000 recfast4py-0.2.5/docs/modules.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      481 2017-03-28 12:31:43.000000 recfast4py-0.2.5/docs/recfast4py.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      395 2017-03-14 14:59:53.000000 recfast4py-0.2.5/docs/usage.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      757 2023-04-18 13:07:47.000000 recfast4py-0.2.5/pyproject.toml
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      170 2019-05-09 10:27:13.000000 recfast4py-0.2.5/requirements.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1366 2023-04-18 13:42:35.715144 recfast4py-0.2.5/setup.cfg
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      657 2023-04-18 13:39:15.000000 recfast4py-0.2.5/setup.py
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 13:42:35.707509 recfast4py-0.2.5/src/
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 13:42:35.713473 recfast4py-0.2.5/src/recfast4py/
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     3175 2017-03-14 14:18:01.000000 recfast4py-0.2.5/src/recfast4py/DM_annihilation.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1036 2017-03-14 14:18:01.000000 recfast4py-0.2.5/src/recfast4py/DM_annihilation.Recfast.h
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)    42560 2021-04-16 07:26:49.000000 recfast4py-0.2.5/src/recfast4py/ODE_solver.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2955 2020-02-13 17:11:51.000000 recfast4py-0.2.5/src/recfast4py/ODE_solver.Recfast.h
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     3902 2018-04-10 15:58:01.000000 recfast4py-0.2.5/src/recfast4py/Rec_corrs_CT.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1278 2017-03-14 14:18:01.000000 recfast4py-0.2.5/src/recfast4py/Rec_corrs_CT.Recfast.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      191 2018-08-15 14:00:23.000000 recfast4py-0.2.5/src/recfast4py/__init__.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)   239221 2022-03-28 14:54:53.000000 recfast4py-0.2.5/src/recfast4py/_recfast.cpp
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      789 2022-03-28 14:54:53.000000 recfast4py-0.2.5/src/recfast4py/_recfast.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1737 2019-05-09 11:06:37.000000 recfast4py-0.2.5/src/recfast4py/_recfast.pyx
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     6675 2017-03-14 14:18:01.000000 recfast4py-0.2.5/src/recfast4py/constants.Recfast.h
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2485 2017-03-14 14:18:01.000000 recfast4py-0.2.5/src/recfast4py/cosmology.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1974 2017-03-14 14:18:01.000000 recfast4py-0.2.5/src/recfast4py/cosmology.Recfast.h
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 13:42:35.714334 recfast4py-0.2.5/src/recfast4py/data/
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)    23196 2017-03-14 14:18:01.000000 recfast4py-0.2.5/src/recfast4py/data/DXe_Xe.CT2010.dat
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     8479 2021-04-16 07:26:49.000000 recfast4py-0.2.5/src/recfast4py/evalode.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1627 2017-03-14 14:18:01.000000 recfast4py-0.2.5/src/recfast4py/evalode.Recfast.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1022 2017-03-21 11:08:15.000000 recfast4py-0.2.5/src/recfast4py/recfast.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      227 2017-03-14 14:17:40.000000 recfast4py-0.2.5/src/recfast4py/recfast4py.py
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)    15164 2020-02-13 17:11:51.000000 recfast4py-0.2.5/src/recfast4py/recombination.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2256 2019-05-09 11:00:46.000000 recfast4py-0.2.5/src/recfast4py/recombination.Recfast.h
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 13:42:35.714219 recfast4py-0.2.5/src/recfast4py.egg-info/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1134 2023-04-18 13:42:35.000000 recfast4py-0.2.5/src/recfast4py.egg-info/PKG-INFO
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1298 2023-04-18 13:42:35.000000 recfast4py-0.2.5/src/recfast4py.egg-info/SOURCES.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2023-04-18 13:42:35.000000 recfast4py-0.2.5/src/recfast4py.egg-info/dependency_links.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2023-04-18 13:37:09.000000 recfast4py-0.2.5/src/recfast4py.egg-info/not-zip-safe
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      212 2023-04-18 13:42:35.000000 recfast4py-0.2.5/src/recfast4py.egg-info/requires.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       11 2023-04-18 13:42:35.000000 recfast4py-0.2.5/src/recfast4py.egg-info/top_level.txt
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 13:42:35.714475 recfast4py-0.2.5/tests/
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1251 2019-05-09 14:45:55.000000 recfast4py-0.2.5/tests/test_recfast4py.py
```

### Comparing `recfast4py-0.2.4/CONTRIBUTING.rst` & `recfast4py-0.2.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/LICENSE` & `recfast4py-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/PKG-INFO` & `recfast4py-0.2.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 Metadata-Version: 2.1
 Name: recfast4py
-Version: 0.2.4
-Summary: A slightly modified version of Recfast++ to do the recombination computation
-Home-page: http://refreweb.phys.ethz.ch/software/recfast4py/0.1.3
-Author: Joel Akeret, Uwe Schmitt
-Author-email: jakeret@phys.ethz.ch
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Version: 0.2.5
+Author: Uwe Schmitt et al
+Author-email: uwe.schmitt@id.ethz.ch
+License: GPLv3
+Project-URL: Source, https://cosmo-docs.phys.ethz.ch/PyCosmo
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Scientific/Engineering :: Astronomy
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst; charset=UTF-8
+Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =============================
 recfast4py
 =============================
 
@@ -26,9 +33,7 @@
 
 
 Features
 --------
 
 * TODO
 
-
-
```

### Comparing `recfast4py-0.2.4/docs/Makefile` & `recfast4py-0.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/docs/check_sphinx.py` & `recfast4py-0.2.5/docs/check_sphinx.py`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/docs/conf.py` & `recfast4py-0.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/docs/index.rst` & `recfast4py-0.2.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/docs/make.bat` & `recfast4py-0.2.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/recfast4py/DM_annihilation.Recfast.cpp` & `recfast4py-0.2.5/src/recfast4py/DM_annihilation.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/recfast4py/DM_annihilation.Recfast.h` & `recfast4py-0.2.5/src/recfast4py/DM_annihilation.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/recfast4py/ODE_solver.Recfast.cpp` & `recfast4py-0.2.5/src/recfast4py/ODE_solver.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/recfast4py/ODE_solver.Recfast.h` & `recfast4py-0.2.5/src/recfast4py/ODE_solver.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/recfast4py/Rec_corrs_CT.Recfast.cpp` & `recfast4py-0.2.5/src/recfast4py/Rec_corrs_CT.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/recfast4py/Rec_corrs_CT.Recfast.h` & `recfast4py-0.2.5/src/recfast4py/Rec_corrs_CT.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/recfast4py/_recfast.cpp` & `recfast4py-0.2.5/src/recfast4py/_recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/recfast4py/_recfast.h` & `recfast4py-0.2.5/src/recfast4py/_recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/recfast4py/constants.Recfast.h` & `recfast4py-0.2.5/src/recfast4py/constants.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/recfast4py/cosmology.Recfast.cpp` & `recfast4py-0.2.5/src/recfast4py/cosmology.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/recfast4py/cosmology.Recfast.h` & `recfast4py-0.2.5/src/recfast4py/cosmology.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/recfast4py/data/DXe_Xe.CT2010.dat` & `recfast4py-0.2.5/src/recfast4py/data/DXe_Xe.CT2010.dat`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/recfast4py/evalode.Recfast.cpp` & `recfast4py-0.2.5/src/recfast4py/evalode.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/recfast4py/evalode.Recfast.h` & `recfast4py-0.2.5/src/recfast4py/evalode.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/recfast4py/recfast.py` & `recfast4py-0.2.5/src/recfast4py/recfast.py`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/recfast4py/recombination.Recfast.cpp` & `recfast4py-0.2.5/src/recfast4py/recombination.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/recfast4py/recombination.Recfast.h` & `recfast4py-0.2.5/src/recfast4py/recombination.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.4/recfast4py.egg-info/PKG-INFO` & `recfast4py-0.2.5/src/recfast4py.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 Metadata-Version: 2.1
 Name: recfast4py
-Version: 0.2.4
-Summary: A slightly modified version of Recfast++ to do the recombination computation
-Home-page: http://refreweb.phys.ethz.ch/software/recfast4py/0.1.3
-Author: Joel Akeret, Uwe Schmitt
-Author-email: jakeret@phys.ethz.ch
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Version: 0.2.5
+Author: Uwe Schmitt et al
+Author-email: uwe.schmitt@id.ethz.ch
+License: GPLv3
+Project-URL: Source, https://cosmo-docs.phys.ethz.ch/PyCosmo
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Scientific/Engineering :: Astronomy
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst; charset=UTF-8
+Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =============================
 recfast4py
 =============================
 
@@ -26,9 +33,7 @@
 
 
 Features
 --------
 
 * TODO
 
-
-
```

