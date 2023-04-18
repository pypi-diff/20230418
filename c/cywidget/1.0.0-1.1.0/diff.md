# Comparing `tmp/cywidget-1.0.0.tar.gz` & `tmp/cywidget-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cywidget-1.0.0.tar", last modified: Tue Dec 13 16:41:35 2022, max compression
+gzip compressed data, was "cywidget-1.1.0.tar", last modified: Tue Apr 18 15:54:49 2023, max compression
```

## Comparing `cywidget-1.0.0.tar` & `cywidget-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2022-12-13 16:41:35.008764 cywidget-1.0.0/
--rw-r--r--   0 tmtabor    (501) staff       (20)     1574 2022-11-14 22:12:35.000000 cywidget-1.0.0/LICENSE.md
--rw-r--r--   0 tmtabor    (501) staff       (20)     1666 2022-12-13 16:41:35.008924 cywidget-1.0.0/PKG-INFO
--rw-r--r--   0 tmtabor    (501) staff       (20)      739 2022-11-14 22:28:44.000000 cywidget-1.0.0/README.md
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2022-12-13 16:41:35.006618 cywidget-1.0.0/cywidget/
--rw-r--r--   0 tmtabor    (501) staff       (20)      756 2022-12-07 18:42:38.000000 cywidget-1.0.0/cywidget/__init__.py
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2022-12-13 16:41:35.008242 cywidget-1.0.0/cywidget.egg-info/
--rw-r--r--   0 tmtabor    (501) staff       (20)     1666 2022-12-13 16:41:34.000000 cywidget-1.0.0/cywidget.egg-info/PKG-INFO
--rw-r--r--   0 tmtabor    (501) staff       (20)      272 2022-12-13 16:41:34.000000 cywidget-1.0.0/cywidget.egg-info/SOURCES.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)        1 2022-12-13 16:41:34.000000 cywidget-1.0.0/cywidget.egg-info/dependency_links.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)        1 2022-12-13 16:40:44.000000 cywidget-1.0.0/cywidget.egg-info/not-zip-safe
--rw-r--r--   0 tmtabor    (501) staff       (20)       34 2022-12-13 16:41:34.000000 cywidget-1.0.0/cywidget.egg-info/requires.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)        9 2022-12-13 16:41:34.000000 cywidget-1.0.0/cywidget.egg-info/top_level.txt
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2022-12-13 16:41:35.008517 cywidget-1.0.0/nbtools/
--rw-r--r--   0 tmtabor    (501) staff       (20)       26 2022-11-14 22:11:12.000000 cywidget-1.0.0/nbtools/cywidget.json
--rw-r--r--   0 tmtabor    (501) staff       (20)      105 2022-12-13 16:41:35.009463 cywidget-1.0.0/setup.cfg
--rw-r--r--   0 tmtabor    (501) staff       (20)     1413 2022-11-14 22:28:15.000000 cywidget-1.0.0/setup.py
+drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-04-18 15:54:49.174599 cywidget-1.1.0/
+-rw-r--r--   0 tmtabor    (501) staff       (20)     1574 2022-11-14 22:12:35.000000 cywidget-1.1.0/LICENSE.md
+-rw-r--r--   0 tmtabor    (501) staff       (20)     1307 2023-04-18 15:54:49.174707 cywidget-1.1.0/PKG-INFO
+-rw-r--r--   0 tmtabor    (501) staff       (20)      382 2023-04-04 16:11:59.000000 cywidget-1.1.0/README.md
+drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-04-18 15:54:49.171327 cywidget-1.1.0/cywidget/
+-rw-r--r--   0 tmtabor    (501) staff       (20)     1434 2023-04-04 16:12:18.000000 cywidget-1.1.0/cywidget/__init__.py
+drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-04-18 15:54:49.173743 cywidget-1.1.0/cywidget.egg-info/
+-rw-r--r--   0 tmtabor    (501) staff       (20)     1307 2023-04-18 15:54:49.000000 cywidget-1.1.0/cywidget.egg-info/PKG-INFO
+-rw-r--r--   0 tmtabor    (501) staff       (20)      272 2023-04-18 15:54:49.000000 cywidget-1.1.0/cywidget.egg-info/SOURCES.txt
+-rw-r--r--   0 tmtabor    (501) staff       (20)        1 2023-04-18 15:54:49.000000 cywidget-1.1.0/cywidget.egg-info/dependency_links.txt
+-rw-r--r--   0 tmtabor    (501) staff       (20)        1 2022-12-13 16:40:44.000000 cywidget-1.1.0/cywidget.egg-info/not-zip-safe
+-rw-r--r--   0 tmtabor    (501) staff       (20)       34 2023-04-18 15:54:49.000000 cywidget-1.1.0/cywidget.egg-info/requires.txt
+-rw-r--r--   0 tmtabor    (501) staff       (20)        9 2023-04-18 15:54:49.000000 cywidget-1.1.0/cywidget.egg-info/top_level.txt
+drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-04-18 15:54:49.174010 cywidget-1.1.0/nbtools/
+-rw-r--r--   0 tmtabor    (501) staff       (20)       26 2022-11-14 22:11:12.000000 cywidget-1.1.0/nbtools/cywidget.json
+-rw-r--r--   0 tmtabor    (501) staff       (20)      105 2023-04-18 15:54:49.175141 cywidget-1.1.0/setup.cfg
+-rw-r--r--   0 tmtabor    (501) staff       (20)     1413 2023-04-04 16:12:11.000000 cywidget-1.1.0/setup.py
```

### Comparing `cywidget-1.0.0/LICENSE.md` & `cywidget-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cywidget-1.0.0/setup.py` & `cywidget-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup_args = dict(
     name='cywidget',
-    version='1.0.0',
+    version='1.1.0',
     packages=['cywidget'],
     url="https://github.com/g2nb/cywidget",
     author="Thorin Tabor",
     author_email="tmtabor@cloud.ucsd.edu",
     description="A user-friend widget for Jupyter that accepts a Cytoscape file and visualizes the network",
     license="BSD-3-Clause",
     long_description=long_description,
@@ -24,15 +24,15 @@
     include_package_data=True,
     python_requires=">=3.7",
     platforms="Linux, Mac OS X, Windows",
     keywords=['cytoscape', 'bioinformatics', 'genomics', 'visualization', 'Jupyter', 'JupyterLab', 'JupyterLab3'],
     classifiers=[
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: MIT License',
+        'License :: OSI Approved :: BSD License',
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Framework :: Jupyter",
     ],
```

