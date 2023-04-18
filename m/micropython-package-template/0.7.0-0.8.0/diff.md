# Comparing `tmp/micropython-package-template-0.7.0.tar.gz` & `tmp/micropython-package-template-0.8.0.tar.gz`

## Comparing `micropython-package-template-0.7.0.tar` & `micropython-package-template-0.8.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-17 09:59:12.000000 micropython-package-template-0.7.0/be_upy_blink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-17 09:59:12.000000 micropython-package-template-0.7.0/be_upy_blink/blink.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-17 09:59:22.000000 micropython-package-template-0.7.0/be_upy_blink/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9809 2023-03-17 09:59:23.000000 micropython-package-template-0.7.0/micropython_package_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-18 20:38:13.000000 micropython-package-template-0.8.0/be_upy_blink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-18 20:38:13.000000 micropython-package-template-0.8.0/be_upy_blink/blink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-18 20:38:22.000000 micropython-package-template-0.8.0/be_upy_blink/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-04-18 20:38:23.000000 micropython-package-template-0.8.0/micropython_package_template.egg-info/PKG-INFO
```

### Comparing `micropython-package-template-0.7.0/be_upy_blink/blink.py` & `micropython-package-template-0.8.0/be_upy_blink/blink.py`

 * *Files identical despite different names*

### Comparing `micropython-package-template-0.7.0/micropython_package_template.egg-info/PKG-INFO` & `micropython-package-template-0.8.0/micropython_package_template.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: micropython-package-template
-Version: 0.7.0
+Version: 0.8.0
 Summary: MicroPython PyPi package template project with auto deploy
 Home-page: https://github.com/brainelectronics/micropython-package-template
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 License: MIT
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-package-template/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-package-template
 Keywords: micropython,template
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # MicroPython package template
 
 [![Downloads](https://pepy.tech/badge/micropython-package-template)](https://pepy.tech/project/micropython-package-template)
 ![Release](https://img.shields.io/github/v/release/brainelectronics/micropython-package-template?include_prereleases&color=success)
```

