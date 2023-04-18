# Comparing `tmp/betp-libv-0.1.0.tar.gz` & `tmp/betp-libv-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betp-libv-0.1.0.tar", last modified: Tue Apr 18 19:13:58 2023, max compression
+gzip compressed data, was "dist/betp-libv-0.1.1.tar", last modified: Tue Apr 18 19:46:26 2023, max compression
```

## Comparing `betp-libv-0.1.0.tar` & `betp-libv-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 asvs       (501) staff       (20)        0 2023-04-18 19:13:58.072814 betp-libv-0.1.0/
--rw-r--r--   0 asvs       (501) staff       (20)      542 2023-04-18 19:13:58.072494 betp-libv-0.1.0/PKG-INFO
--rw-r--r--   0 asvs       (501) staff       (20)       74 2023-04-18 19:13:57.000000 betp-libv-0.1.0/README.md
-drwxr-xr-x   0 asvs       (501) staff       (20)        0 2023-04-18 19:13:58.071135 betp-libv-0.1.0/betp-libv/
--rw-r--r--   0 asvs       (501) staff       (20)        0 2023-04-18 19:13:57.000000 betp-libv-0.1.0/betp-libv/__init__.py
-drwxr-xr-x   0 asvs       (501) staff       (20)        0 2023-04-18 19:13:58.072017 betp-libv-0.1.0/betp_libv.egg-info/
--rw-r--r--   0 asvs       (501) staff       (20)      542 2023-04-18 19:13:58.000000 betp-libv-0.1.0/betp_libv.egg-info/PKG-INFO
--rw-r--r--   0 asvs       (501) staff       (20)      172 2023-04-18 19:13:58.000000 betp-libv-0.1.0/betp_libv.egg-info/SOURCES.txt
--rw-r--r--   0 asvs       (501) staff       (20)        1 2023-04-18 19:13:58.000000 betp-libv-0.1.0/betp_libv.egg-info/dependency_links.txt
--rw-r--r--   0 asvs       (501) staff       (20)       10 2023-04-18 19:13:58.000000 betp-libv-0.1.0/betp_libv.egg-info/top_level.txt
--rw-r--r--   0 asvs       (501) staff       (20)       38 2023-04-18 19:13:58.072890 betp-libv-0.1.0/setup.cfg
--rw-r--r--   0 asvs       (501) staff       (20)      662 2023-04-18 19:13:57.000000 betp-libv-0.1.0/setup.py
+drwxr-xr-x   0 naveen.bk   (503) staff       (20)        0 2023-04-18 19:46:26.000000 betp-libv-0.1.1/
+-rw-r--r--   0 naveen.bk   (503) staff       (20)      598 2023-04-18 19:46:26.000000 betp-libv-0.1.1/PKG-INFO
+drwxr-xr-x   0 naveen.bk   (503) staff       (20)        0 2023-04-18 19:46:26.000000 betp-libv-0.1.1/betp_libv.egg-info/
+-rw-r--r--   0 naveen.bk   (503) staff       (20)      598 2023-04-18 19:46:26.000000 betp-libv-0.1.1/betp_libv.egg-info/PKG-INFO
+-rw-r--r--   0 naveen.bk   (503) staff       (20)      193 2023-04-18 19:46:26.000000 betp-libv-0.1.1/betp_libv.egg-info/SOURCES.txt
+-rw-r--r--   0 naveen.bk   (503) staff       (20)       10 2023-04-18 19:46:26.000000 betp-libv-0.1.1/betp_libv.egg-info/top_level.txt
+-rw-r--r--   0 naveen.bk   (503) staff       (20)        1 2023-04-18 19:46:26.000000 betp-libv-0.1.1/betp_libv.egg-info/dependency_links.txt
+drwxr-xr-x   0 naveen.bk   (503) staff       (20)        0 2023-04-18 19:46:26.000000 betp-libv-0.1.1/betp-libv/
+-rw-r--r--   0 naveen.bk   (503) staff       (20)        0 2023-04-18 19:38:24.000000 betp-libv-0.1.1/betp-libv/__init__.py
+-rw-r--r--   0 naveen.bk   (503) staff       (20)       49 2023-04-18 19:42:14.000000 betp-libv-0.1.1/betp-libv/logback.py
+-rw-r--r--   0 naveen.bk   (503) staff       (20)       74 2023-04-18 19:38:24.000000 betp-libv-0.1.1/README.md
+-rw-r--r--   0 naveen.bk   (503) staff       (20)      662 2023-04-18 19:40:02.000000 betp-libv-0.1.1/setup.py
+-rw-r--r--   0 naveen.bk   (503) staff       (20)       38 2023-04-18 19:46:26.000000 betp-libv-0.1.1/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `betp-libv-0.1.0/setup.py` & `betp-libv-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='betp-libv',
-    version='0.1.0',
+    version='0.1.1',
     description='A sample Python package',
     author='Puddl',
     author_email='devppong@gmail.com',
     url='https://github.com/devppong/betp-libv',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

