# Comparing `tmp/basicnanoclient-0.0.2.tar.gz` & `tmp/basicnanoclient-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basicnanoclient-0.0.2.tar", last modified: Tue Apr 18 03:15:34 2023, max compression
+gzip compressed data, was "basicnanoclient-0.0.4.tar", last modified: Tue Apr 18 03:43:59 2023, max compression
```

## Comparing `basicnanoclient-0.0.2.tar` & `basicnanoclient-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-18 03:15:34.569754 basicnanoclient-0.0.2/
--rw-r--r--   0 nate       (501) staff       (20)     1211 2023-04-18 02:36:25.000000 basicnanoclient-0.0.2/LICENSE
--rw-r--r--   0 nate       (501) staff       (20)     2756 2023-04-18 03:15:34.569631 basicnanoclient-0.0.2/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)      844 2023-04-18 03:14:16.000000 basicnanoclient-0.0.2/README.md
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-18 03:15:34.569493 basicnanoclient-0.0.2/basicnanoclient.egg-info/
--rw-r--r--   0 nate       (501) staff       (20)     2756 2023-04-18 03:15:34.000000 basicnanoclient-0.0.2/basicnanoclient.egg-info/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)      235 2023-04-18 03:15:34.000000 basicnanoclient-0.0.2/basicnanoclient.egg-info/SOURCES.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-18 03:15:34.000000 basicnanoclient-0.0.2/basicnanoclient.egg-info/dependency_links.txt
--rw-r--r--   0 nate       (501) staff       (20)        9 2023-04-18 03:15:34.000000 basicnanoclient-0.0.2/basicnanoclient.egg-info/requires.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-18 03:15:34.000000 basicnanoclient-0.0.2/basicnanoclient.egg-info/top_level.txt
--rw-r--r--   0 nate       (501) staff       (20)      592 2023-04-18 03:14:29.000000 basicnanoclient-0.0.2/pyproject.toml
--rw-r--r--   0 nate       (501) staff       (20)       38 2023-04-18 03:15:34.569784 basicnanoclient-0.0.2/setup.cfg
--rw-r--r--   0 nate       (501) staff       (20)      942 2023-04-18 03:14:22.000000 basicnanoclient-0.0.2/setup.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-18 03:43:59.174596 basicnanoclient-0.0.4/
+-rw-r--r--   0 nate       (501) staff       (20)     1211 2023-04-18 02:36:25.000000 basicnanoclient-0.0.4/LICENSE
+-rw-r--r--   0 nate       (501) staff       (20)     2762 2023-04-18 03:43:59.174480 basicnanoclient-0.0.4/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)      844 2023-04-18 03:14:16.000000 basicnanoclient-0.0.4/README.md
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-18 03:43:59.174331 basicnanoclient-0.0.4/basicnanoclient.egg-info/
+-rw-r--r--   0 nate       (501) staff       (20)     2762 2023-04-18 03:43:59.000000 basicnanoclient-0.0.4/basicnanoclient.egg-info/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)      235 2023-04-18 03:43:59.000000 basicnanoclient-0.0.4/basicnanoclient.egg-info/SOURCES.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-18 03:43:59.000000 basicnanoclient-0.0.4/basicnanoclient.egg-info/dependency_links.txt
+-rw-r--r--   0 nate       (501) staff       (20)       99 2023-04-18 03:43:59.000000 basicnanoclient-0.0.4/basicnanoclient.egg-info/requires.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-18 03:43:59.000000 basicnanoclient-0.0.4/basicnanoclient.egg-info/top_level.txt
+-rw-r--r--   0 nate       (501) staff       (20)      728 2023-04-18 03:43:04.000000 basicnanoclient-0.0.4/pyproject.toml
+-rw-r--r--   0 nate       (501) staff       (20)       38 2023-04-18 03:43:59.174629 basicnanoclient-0.0.4/setup.cfg
+-rw-r--r--   0 nate       (501) staff       (20)      943 2023-04-18 03:39:55.000000 basicnanoclient-0.0.4/setup.py
```

### Comparing `basicnanoclient-0.0.2/LICENSE` & `basicnanoclient-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `basicnanoclient-0.0.2/PKG-INFO` & `basicnanoclient-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicnanoclient
-Version: 0.0.2
+Version: 0.0.4
 Summary: Nano RPC python client
 Home-page: https://github.com/nanoswap/basicnanoclient
 Author: Nathaniel Schultz
 Author-email: Nathaniel Schultz <nate@nanoswap.finance>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
@@ -26,18 +26,18 @@
         IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
         OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
         ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
         OTHER DEALINGS IN THE SOFTWARE.
         
         For more information, please refer to <https://unlicense.org>
         
-Project-URL: Bug Tracker, https://github.com/nanoswap/nanoclient/issues
+Project-URL: Bug Tracker, https://github.com/nanoswap/basicnanoclient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
-Requires-Python: >=3.6
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # basicnanoclient
 
 A nano (XNO) cryptocurrency RPC python client
```

### Comparing `basicnanoclient-0.0.2/README.md` & `basicnanoclient-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `basicnanoclient-0.0.2/basicnanoclient.egg-info/PKG-INFO` & `basicnanoclient-0.0.4/basicnanoclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicnanoclient
-Version: 0.0.2
+Version: 0.0.4
 Summary: Nano RPC python client
 Home-page: https://github.com/nanoswap/basicnanoclient
 Author: Nathaniel Schultz
 Author-email: Nathaniel Schultz <nate@nanoswap.finance>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
@@ -26,18 +26,18 @@
         IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
         OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
         ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
         OTHER DEALINGS IN THE SOFTWARE.
         
         For more information, please refer to <https://unlicense.org>
         
-Project-URL: Bug Tracker, https://github.com/nanoswap/nanoclient/issues
+Project-URL: Bug Tracker, https://github.com/nanoswap/basicnanoclient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
-Requires-Python: >=3.6
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # basicnanoclient
 
 A nano (XNO) cryptocurrency RPC python client
```

### Comparing `basicnanoclient-0.0.2/setup.py` & `basicnanoclient-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     """Convert README.md to a string."""
     with open(filename, "r", encoding="utf-8") as f:
         return f.read()
 
 
 setup(
     name="basicnanoclient",
-    version="0.0.2",
+    version="0.0.4",
     author="Nathaniel Schultz",
     author_email="nate@nanoswap.finance",
     description="Nano Cryptocurrency RPC Client",
     long_description=load_long_description("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/nanoswap/basicnanoclient",
     project_urls={
@@ -22,9 +22,9 @@
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: The Unlicense (Unlicense)"
     ],
     package_dir={'basicnanoclient': "basicnanoclient"},
     packages=find_packages("basicnanoclient"),
-    python_requires=">=3.6"
+    python_requires=">=3.11"
 )
```

