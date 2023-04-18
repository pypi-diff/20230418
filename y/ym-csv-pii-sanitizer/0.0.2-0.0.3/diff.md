# Comparing `tmp/ym_csv_pii_sanitizer-0.0.2.tar.gz` & `tmp/ym_csv_pii_sanitizer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ym_csv_pii_sanitizer-0.0.2.tar", last modified: Sun Apr 16 11:13:04 2023, max compression
+gzip compressed data, was "ym_csv_pii_sanitizer-0.0.3.tar", last modified: Tue Apr 18 13:24:08 2023, max compression
```

## Comparing `ym_csv_pii_sanitizer-0.0.2.tar` & `ym_csv_pii_sanitizer-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 11:13:04.856838 ym_csv_pii_sanitizer-0.0.2/
--rw-r--r--   0 alexilin   (501) staff       (20)      440 2023-04-16 11:13:04.856680 ym_csv_pii_sanitizer-0.0.2/PKG-INFO
--rw-r--r--   0 alexilin   (501) staff       (20)      835 2023-04-16 10:36:49.000000 ym_csv_pii_sanitizer-0.0.2/README.md
--rw-r--r--   0 alexilin   (501) staff       (20)       89 2023-04-16 10:26:20.000000 ym_csv_pii_sanitizer-0.0.2/pyproject.toml
--rw-r--r--   0 alexilin   (501) staff       (20)       38 2023-04-16 11:13:04.856873 ym_csv_pii_sanitizer-0.0.2/setup.cfg
--rw-r--r--   0 alexilin   (501) staff       (20)      885 2023-04-16 11:12:59.000000 ym_csv_pii_sanitizer-0.0.2/setup.py
-drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 11:13:04.855542 ym_csv_pii_sanitizer-0.0.2/ym_csv_pii_sanitizer/
--rw-r--r--   0 alexilin   (501) staff       (20)        0 2023-04-15 11:44:38.000000 ym_csv_pii_sanitizer-0.0.2/ym_csv_pii_sanitizer/__init__.py
--rw-r--r--   0 alexilin   (501) staff       (20)     3140 2023-04-15 11:28:31.000000 ym_csv_pii_sanitizer-0.0.2/ym_csv_pii_sanitizer/main.py
--rw-r--r--   0 alexilin   (501) staff       (20)     1078 2023-04-15 11:36:09.000000 ym_csv_pii_sanitizer-0.0.2/ym_csv_pii_sanitizer/test_main.py
-drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 11:13:04.856510 ym_csv_pii_sanitizer-0.0.2/ym_csv_pii_sanitizer.egg-info/
--rw-r--r--   0 alexilin   (501) staff       (20)      440 2023-04-16 11:13:04.000000 ym_csv_pii_sanitizer-0.0.2/ym_csv_pii_sanitizer.egg-info/PKG-INFO
--rw-r--r--   0 alexilin   (501) staff       (20)      395 2023-04-16 11:13:04.000000 ym_csv_pii_sanitizer-0.0.2/ym_csv_pii_sanitizer.egg-info/SOURCES.txt
--rw-r--r--   0 alexilin   (501) staff       (20)        1 2023-04-16 11:13:04.000000 ym_csv_pii_sanitizer-0.0.2/ym_csv_pii_sanitizer.egg-info/dependency_links.txt
--rw-r--r--   0 alexilin   (501) staff       (20)       71 2023-04-16 11:13:04.000000 ym_csv_pii_sanitizer-0.0.2/ym_csv_pii_sanitizer.egg-info/entry_points.txt
--rw-r--r--   0 alexilin   (501) staff       (20)       25 2023-04-16 11:13:04.000000 ym_csv_pii_sanitizer-0.0.2/ym_csv_pii_sanitizer.egg-info/requires.txt
--rw-r--r--   0 alexilin   (501) staff       (20)       21 2023-04-16 11:13:04.000000 ym_csv_pii_sanitizer-0.0.2/ym_csv_pii_sanitizer.egg-info/top_level.txt
+drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-18 13:24:08.665928 ym_csv_pii_sanitizer-0.0.3/
+-rw-r--r--   0 alexilin   (501) staff       (20)      408 2023-04-18 13:24:08.665769 ym_csv_pii_sanitizer-0.0.3/PKG-INFO
+-rw-r--r--   0 alexilin   (501) staff       (20)      923 2023-04-18 13:15:01.000000 ym_csv_pii_sanitizer-0.0.3/README.md
+-rw-r--r--   0 alexilin   (501) staff       (20)       90 2023-04-17 09:37:13.000000 ym_csv_pii_sanitizer-0.0.3/pyproject.toml
+-rw-r--r--   0 alexilin   (501) staff       (20)       38 2023-04-18 13:24:08.665967 ym_csv_pii_sanitizer-0.0.3/setup.cfg
+-rw-r--r--   0 alexilin   (501) staff       (20)      959 2023-04-18 13:22:49.000000 ym_csv_pii_sanitizer-0.0.3/setup.py
+drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-18 13:24:08.664639 ym_csv_pii_sanitizer-0.0.3/ym_csv_pii_sanitizer/
+-rw-r--r--   0 alexilin   (501) staff       (20)       34 2023-04-18 11:52:09.000000 ym_csv_pii_sanitizer-0.0.3/ym_csv_pii_sanitizer/__init__.py
+-rw-r--r--   0 alexilin   (501) staff       (20)     9550 2023-04-18 12:53:15.000000 ym_csv_pii_sanitizer-0.0.3/ym_csv_pii_sanitizer/main.py
+-rw-r--r--   0 alexilin   (501) staff       (20)      524 2023-04-18 13:03:25.000000 ym_csv_pii_sanitizer-0.0.3/ym_csv_pii_sanitizer/test_main.py
+drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-18 13:24:08.665567 ym_csv_pii_sanitizer-0.0.3/ym_csv_pii_sanitizer.egg-info/
+-rw-r--r--   0 alexilin   (501) staff       (20)      408 2023-04-18 13:24:08.000000 ym_csv_pii_sanitizer-0.0.3/ym_csv_pii_sanitizer.egg-info/PKG-INFO
+-rw-r--r--   0 alexilin   (501) staff       (20)      395 2023-04-18 13:24:08.000000 ym_csv_pii_sanitizer-0.0.3/ym_csv_pii_sanitizer.egg-info/SOURCES.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)        1 2023-04-18 13:24:08.000000 ym_csv_pii_sanitizer-0.0.3/ym_csv_pii_sanitizer.egg-info/dependency_links.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)       71 2023-04-18 13:24:08.000000 ym_csv_pii_sanitizer-0.0.3/ym_csv_pii_sanitizer.egg-info/entry_points.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)       63 2023-04-18 13:24:08.000000 ym_csv_pii_sanitizer-0.0.3/ym_csv_pii_sanitizer.egg-info/requires.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)       21 2023-04-18 13:24:08.000000 ym_csv_pii_sanitizer-0.0.3/ym_csv_pii_sanitizer.egg-info/top_level.txt
```

### Comparing `ym_csv_pii_sanitizer-0.0.2/README.md` & `ym_csv_pii_sanitizer-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -40,14 +40,19 @@
 INPUT - Path to csv file to sanitize.
 OUTPUT - Optional output path for result csv file.
 
 ## Publishing to pypi
 
 Run to build:
 ```
+pip install build
 python -m build
 ```
 
 Run to publish:
+
+TOKEN should be replaced with pypi.org API TOKEN
+
 ```
+pip install twine
 twine upload dist/* -u __token__ -p TOKEN
-```
+```
```

### Comparing `ym_csv_pii_sanitizer-0.0.2/setup.py` & `ym_csv_pii_sanitizer-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
-DESCRIPTION = 'Redact a PHI (personal health information) data from a CSV file.'
-LONG_DESCRIPTION = """## Installation\n\n```pip install ym_csv_pii_sanitizer```\n\n```python -m spacy download en_core_web_sm```\n\n## Usage\n\n```ym_csv_pii_sanitizer PATH_TO_CSV_FILE```"""
+VERSION = '0.0.3'
+DESCRIPTION = """Redact a PHI (personal health
+information) data from a CSV file."""
+LONG_DESCRIPTION = """## Installation\n\n
+```pip install ym_csv_pii_sanitizer```\n\n
+```python -m spacy download en_core_web_lg```\n\n
+## Usage\n\n```ym_csv_pii_sanitizer PATH_TO_CSV_FILE```"""
 
 setup(
     name="ym_csv_pii_sanitizer",
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     author="Alex Ilin",
     author_email="alex.ilin@ymeadows.com",
     packages=find_packages(),
     install_requires=[
         'typer',
-        'spacy',
-        'phonenumbers'
+        'presidio_analyzer',
+        'presidio_anonymizer',
+        'transformers',
+        'torch'
     ],
-    classifiers= [
+    classifiers=[
         "Programming Language :: Python :: 3"
     ],
     entry_points={
-        "console_scripts": ["ym_csv_pii_sanitizer = ym_csv_pii_sanitizer.main:run"],
+        "console_scripts":
+        ["ym_csv_pii_sanitizer = ym_csv_pii_sanitizer.main:run"],
     },
 )
```

