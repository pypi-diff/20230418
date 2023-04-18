# Comparing `tmp/PyNuclei-1.1.tar.gz` & `tmp/PyNuclei-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNuclei-1.1.tar", last modified: Mon Jun 13 15:17:24 2022, max compression
+gzip compressed data, was "PyNuclei-1.2.tar", last modified: Tue Apr 18 07:59:41 2023, max compression
```

## Comparing `PyNuclei-1.1.tar` & `PyNuclei-1.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 vaibhav   (1001) vaibhav   (1003)        0 2022-06-13 15:17:24.932689 PyNuclei-1.1/
--rw-r--r--   0 vaibhav   (1001) vaibhav   (1003)     1086 2022-06-12 15:49:23.000000 PyNuclei-1.1/LICENSE
--rw-r--r--   0 vaibhav   (1001) vaibhav   (1003)     2188 2022-06-13 15:17:24.932689 PyNuclei-1.1/PKG-INFO
-drwxr-xr-x   0 vaibhav   (1001) vaibhav   (1003)        0 2022-06-13 15:17:24.932689 PyNuclei-1.1/PyNuclei/
-drwxr-xr-x   0 vaibhav   (1001) vaibhav   (1003)        0 2022-06-13 15:17:24.932689 PyNuclei-1.1/PyNuclei/PyNuclei.egg-info/
--rw-r--r--   0 vaibhav   (1001) vaibhav   (1003)     2188 2022-06-13 15:17:24.000000 PyNuclei-1.1/PyNuclei/PyNuclei.egg-info/PKG-INFO
--rw-r--r--   0 vaibhav   (1001) vaibhav   (1003)      205 2022-06-13 15:17:24.000000 PyNuclei-1.1/PyNuclei/PyNuclei.egg-info/SOURCES.txt
--rw-r--r--   0 vaibhav   (1001) vaibhav   (1003)        1 2022-06-13 15:17:24.000000 PyNuclei-1.1/PyNuclei/PyNuclei.egg-info/dependency_links.txt
--rw-r--r--   0 vaibhav   (1001) vaibhav   (1003)        1 2022-06-13 15:17:24.000000 PyNuclei-1.1/PyNuclei/PyNuclei.egg-info/top_level.txt
--rw-r--r--   0 vaibhav   (1001) vaibhav   (1003)     1719 2022-06-13 06:32:40.000000 PyNuclei-1.1/README.md
--rw-r--r--   0 vaibhav   (1001) vaibhav   (1003)       89 2022-06-13 15:08:52.000000 PyNuclei-1.1/pyproject.toml
--rw-r--r--   0 vaibhav   (1001) vaibhav   (1003)       38 2022-06-13 15:17:24.932689 PyNuclei-1.1/setup.cfg
--rw-r--r--   0 vaibhav   (1001) vaibhav   (1003)      752 2022-06-13 15:17:15.000000 PyNuclei-1.1/setup.py
+drwxr-xr-x   0 vaibhav   (1001) vaibhav   (1003)        0 2023-04-18 07:59:41.004009 PyNuclei-1.2/
+-rw-r--r--   0 vaibhav   (1001) vaibhav   (1003)     3640 2023-04-18 07:59:41.000009 PyNuclei-1.2/PKG-INFO
+drwxr-xr-x   0 vaibhav   (1001) vaibhav   (1003)        0 2023-04-18 07:59:41.000009 PyNuclei-1.2/PyNuclei/
+drwxr-xr-x   0 vaibhav   (1001) vaibhav   (1003)        0 2023-04-18 07:59:41.000009 PyNuclei-1.2/PyNuclei/PyNuclei.egg-info/
+-rw-r--r--   0 vaibhav   (1001) vaibhav   (1003)     3640 2023-04-18 07:59:40.000000 PyNuclei-1.2/PyNuclei/PyNuclei.egg-info/PKG-INFO
+-rw-r--r--   0 vaibhav   (1001) vaibhav   (1003)      197 2023-04-18 07:59:40.000000 PyNuclei-1.2/PyNuclei/PyNuclei.egg-info/SOURCES.txt
+-rw-r--r--   0 vaibhav   (1001) vaibhav   (1003)        1 2023-04-18 07:59:40.000000 PyNuclei-1.2/PyNuclei/PyNuclei.egg-info/dependency_links.txt
+-rw-r--r--   0 vaibhav   (1001) vaibhav   (1003)        1 2023-04-18 07:59:40.000000 PyNuclei-1.2/PyNuclei/PyNuclei.egg-info/top_level.txt
+-rw-r--r--   0 vaibhav   (1001) vaibhav   (1003)     2521 2023-04-18 07:47:38.000000 PyNuclei-1.2/README.md
+-rw-r--r--   0 vaibhav   (1001) vaibhav   (1003)       89 2022-06-13 15:08:52.000000 PyNuclei-1.2/pyproject.toml
+-rw-r--r--   0 vaibhav   (1001) vaibhav   (1003)       38 2023-04-18 07:59:41.004009 PyNuclei-1.2/setup.cfg
+-rw-r--r--   0 vaibhav   (1001) vaibhav   (1003)      752 2023-04-18 07:59:36.000000 PyNuclei-1.2/setup.py
```

### Comparing `PyNuclei-1.1/PKG-INFO` & `PyNuclei-1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: PyNuclei
-Version: 1.1
-Summary: PyNuclei is an unofficial python library for Nuclei Scanner.
-Home-page: https://github.com/kushvaibhav/PyNuclei/
-Author: Vaibhav Kushwaha
-Author-email: vaibhavkush.007@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyNuclei
 
 PyNuclei is an unofficial Python library for Nuclei Scanner.
 
 ## Features
 - Run Nuclei Scans for all or selected templates
 - By default uses random User-Agents for every scan.
@@ -43,13 +29,50 @@
 """
 
 nucleiScanner = Nuclei()
 scanResult = nucleiScanner.scan("example.com", template=["cves","network", "ssl"], rateLimit=150))
 print(scanResult)
 ```
 
+### Templates
+```python
+from PyNuclei import Nuclei
+
+nucleiScanner = Nuclei()
+
+"""
+All active templates.
+"""
+print(nucleiScanner.nucleiTemplates)
+[
+    "cnvd", "cves", "default-logins", "exposed-panels",
+    "exposures", "file", "misconfiguration",
+    "miscellaneous", "takeovers", "technologies",
+    "token-spray", "vulnerabilities", "network", 
+    "dns", "iot", "ssl"
+]
+
+"""
+All ignored templates.
+"""
+print(nucleiScanner.ignoredTemplates)
+[
+    "headless", "fuzzing", "helpers", 
+]
+```
+NOTE: You can run ignored templates by passing them in the template parameter in ```nucleiScanner.scan(<host>, template=nucleiScanner.ignoredTemplates)```
+
+### Update Nuclei
+```python
+from PyNuclei import Nuclei
+"""
+This will update Nuclei engine & Nuclei Templates.
+"""
+Nuclei.updateNuclei(verbose=True)
+```
+
 ## Connect with me
 <p align="left">
 <a href="https://twitter.com/kushvaibhav_" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/twitter.svg" alt="kushvaibhav_" height="30" width="40" /></a>
 <a href="https://linkedin.com/in/kushvaibhav" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="kushvaibhav" height="30" width="40" /></a>
 <a href="https://instagram.com/kushvaibhav" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg" alt="kushvaibhav" height="30" width="40" /></a>
 </p>
```

#### html2text {}

```diff
@@ -1,20 +1,23 @@
-Metadata-Version: 2.1 Name: PyNuclei Version: 1.1 Summary: PyNuclei is an
-unofficial python library for Nuclei Scanner. Home-page: https://github.com/
-kushvaibhav/PyNuclei/ Author: Vaibhav Kushwaha Author-email:
-vaibhavkush.007@gmail.com Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.4 Description-Content-Type: text/
-markdown License-File: LICENSE # PyNuclei PyNuclei is an unofficial Python
-library for Nuclei Scanner. ## Features - Run Nuclei Scans for all or selected
-templates - By default uses random User-Agents for every scan. - User-defined
-rate limit (Default: 150) ## Installation ```sh pip3 install PyNuclei ``` ##
-Usage ```python from PyNuclei import Nuclei """ nucleiScanner.scan() Args: host
-[str]: The hostname of the target which Nuclei will run against templates
-[list][Optional]: If templates list not provided all nuclei templates from
-"nucleiTemplates" property will be executed userAgents [str][Optional]: If not
-provided random User-Agents will be used. rateLimit [int][Optional]: Defaults
-to 150. Returns: result [dict]: Scan result from all templates. """
-nucleiScanner = Nuclei() scanResult = nucleiScanner.scan("example.com",
-template=["cves","network", "ssl"], rateLimit=150)) print(scanResult) ``` ##
-Connect with me
+# PyNuclei PyNuclei is an unofficial Python library for Nuclei Scanner. ##
+Features - Run Nuclei Scans for all or selected templates - By default uses
+random User-Agents for every scan. - User-defined rate limit (Default: 150) ##
+Installation ```sh pip3 install PyNuclei ``` ## Usage ```python from PyNuclei
+import Nuclei """ nucleiScanner.scan() Args: host [str]: The hostname of the
+target which Nuclei will run against templates [list][Optional]: If templates
+list not provided all nuclei templates from "nucleiTemplates" property will be
+executed userAgents [str][Optional]: If not provided random User-Agents will be
+used. rateLimit [int][Optional]: Defaults to 150. Returns: result [dict]: Scan
+result from all templates. """ nucleiScanner = Nuclei() scanResult =
+nucleiScanner.scan("example.com", template=["cves","network", "ssl"],
+rateLimit=150)) print(scanResult) ``` ### Templates ```python from PyNuclei
+import Nuclei nucleiScanner = Nuclei() """ All active templates. """ print
+(nucleiScanner.nucleiTemplates) [ "cnvd", "cves", "default-logins", "exposed-
+panels", "exposures", "file", "misconfiguration", "miscellaneous", "takeovers",
+"technologies", "token-spray", "vulnerabilities", "network", "dns", "iot",
+"ssl" ] """ All ignored templates. """ print(nucleiScanner.ignoredTemplates)
+[ "headless", "fuzzing", "helpers", ] ``` NOTE: You can run ignored templates
+by passing them in the template parameter in ```nucleiScanner.scan(,
+template=nucleiScanner.ignoredTemplates)``` ### Update Nuclei ```python from
+PyNuclei import Nuclei """ This will update Nuclei engine & Nuclei Templates.
+""" Nuclei.updateNuclei(verbose=True) ``` ## Connect with me
 [kushvaibhav_] [kushvaibhav] [kushvaibhav]
```

### Comparing `PyNuclei-1.1/setup.py` & `PyNuclei-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyNuclei",
-    version="1.1",
+    version="1.2",
     author="Vaibhav Kushwaha",
     author_email="vaibhavkush.007@gmail.com",
     description="PyNuclei is an unofficial python library for Nuclei Scanner.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kushvaibhav/PyNuclei/",
     classifiers=[
```

