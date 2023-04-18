# Comparing `tmp/ChromaticColorBurst-1.0.2.tar.gz` & `tmp/ChromaticColorBurst-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChromaticColorBurst-1.0.2.tar", last modified: Thu Feb 16 08:17:48 2023, max compression
+gzip compressed data, was "ChromaticColorBurst-1.0.3.tar", last modified: Tue Apr 18 13:02:15 2023, max compression
```

## Comparing `ChromaticColorBurst-1.0.2.tar` & `ChromaticColorBurst-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-02-16 08:17:48.406571 ChromaticColorBurst-1.0.2/
-drwxrwxrwx   0        0        0        0 2023-02-16 08:17:48.372548 ChromaticColorBurst-1.0.2/ChromaticColorBurst.egg-info/
--rw-rw-rw-   0        0        0    10693 2023-02-16 08:17:48.000000 ChromaticColorBurst-1.0.2/ChromaticColorBurst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-02-16 08:17:48.000000 ChromaticColorBurst-1.0.2/ChromaticColorBurst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-16 08:17:48.000000 ChromaticColorBurst-1.0.2/ChromaticColorBurst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-02-16 08:17:48.000000 ChromaticColorBurst-1.0.2/ChromaticColorBurst.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-16 08:17:48.403066 ChromaticColorBurst-1.0.2/ColorBurst/
--rw-rw-rw-   0        0        0     9343 2023-02-16 08:17:05.000000 ChromaticColorBurst-1.0.2/ColorBurst/ColorBurst.py
--rw-rw-rw-   0        0        0     1090 2023-02-15 12:55:36.000000 ChromaticColorBurst-1.0.2/ColorBurst/LISCENCE.md
--rw-rw-rw-   0        0        0       25 2023-02-15 05:56:44.000000 ChromaticColorBurst-1.0.2/ColorBurst/__init__.py
--rw-rw-rw-   0        0        0      611 2023-02-15 13:17:10.000000 ChromaticColorBurst-1.0.2/ColorBurst/test.py
--rw-rw-rw-   0        0        0    10693 2023-02-16 08:17:48.404560 ChromaticColorBurst-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    10152 2023-02-16 07:38:54.000000 ChromaticColorBurst-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-02-16 08:17:48.406571 ChromaticColorBurst-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      939 2023-02-16 08:17:35.000000 ChromaticColorBurst-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 13:02:15.831620 ChromaticColorBurst-1.0.3/
+drwxrwxrwx   0        0        0        0 2023-04-18 13:02:15.814873 ChromaticColorBurst-1.0.3/ChromaticColorBurst.egg-info/
+-rw-rw-rw-   0        0        0    10693 2023-04-18 13:02:15.000000 ChromaticColorBurst-1.0.3/ChromaticColorBurst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-04-18 13:02:15.000000 ChromaticColorBurst-1.0.3/ChromaticColorBurst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 13:02:15.000000 ChromaticColorBurst-1.0.3/ChromaticColorBurst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-18 13:02:15.000000 ChromaticColorBurst-1.0.3/ChromaticColorBurst.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 13:02:15.828611 ChromaticColorBurst-1.0.3/ColorBurst/
+-rw-rw-rw-   0        0        0     5002 2023-04-18 12:22:48.000000 ChromaticColorBurst-1.0.3/ColorBurst/ColorBurst.py
+-rw-rw-rw-   0        0        0     1023 2023-02-16 10:50:00.000000 ChromaticColorBurst-1.0.3/ColorBurst/LISCENCE.md
+-rw-rw-rw-   0        0        0       25 2023-04-18 13:01:20.000000 ChromaticColorBurst-1.0.3/ColorBurst/__init__.py
+-rw-rw-rw-   0        0        0     1990 2023-04-18 12:43:42.000000 ChromaticColorBurst-1.0.3/ColorBurst/classes.py
+-rw-rw-rw-   0        0        0    10693 2023-04-18 13:02:15.830620 ChromaticColorBurst-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10152 2023-02-16 07:38:54.000000 ChromaticColorBurst-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 13:02:15.831620 ChromaticColorBurst-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      939 2023-04-18 13:02:00.000000 ChromaticColorBurst-1.0.3/setup.py
```

### Comparing `ChromaticColorBurst-1.0.2/ChromaticColorBurst.egg-info/PKG-INFO` & `ChromaticColorBurst-1.0.3/ChromaticColorBurst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChromaticColorBurst
-Version: 1.0.2
+Version: 1.0.3
 Summary: You can now print styled TEXT to console/terminal without much of a hassel
 Home-page: https://github.com/sachin-acharya-projects/ColorBurst
 Author: Sachin Acharya
 Author-email: acharyaraj71+ColorBurst@gmail.com
 Keywords: colored_text console terminal style styled_text
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ChromaticColorBurst-1.0.2/ColorBurst/LISCENCE.md` & `ChromaticColorBurst-1.0.3/ColorBurst/LISCENCE.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 MIT License
 
 Copyright (c) 2022 Sachin Acharya
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
+to use, copy, modify, and merge and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
```

### Comparing `ChromaticColorBurst-1.0.2/PKG-INFO` & `ChromaticColorBurst-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChromaticColorBurst
-Version: 1.0.2
+Version: 1.0.3
 Summary: You can now print styled TEXT to console/terminal without much of a hassel
 Home-page: https://github.com/sachin-acharya-projects/ColorBurst
 Author: Sachin Acharya
 Author-email: acharyaraj71+ColorBurst@gmail.com
 Keywords: colored_text console terminal style styled_text
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ChromaticColorBurst-1.0.2/README.md` & `ChromaticColorBurst-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ChromaticColorBurst-1.0.2/setup.py` & `ChromaticColorBurst-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from pathlib import Path
 
 BASE = Path(__file__).parent
 LONG_DESCRIPTIONS = (BASE / "README.md").read_text()
 setup(
     name="ChromaticColorBurst",
-    version='1.0.2',
+    version='1.0.3',
     description="You can now print styled TEXT to console/terminal without much of a hassel",
     long_description=LONG_DESCRIPTIONS,
     long_description_content_type="text/markdown",
     keywords='colored_text console terminal style styled_text',
     author='Sachin Acharya',
     author_email='acharyaraj71+ColorBurst@gmail.com',
     packages=['ColorBurst'],
```

