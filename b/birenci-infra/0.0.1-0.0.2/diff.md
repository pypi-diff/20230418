# Comparing `tmp/birenci-infra-0.0.1.tar.gz` & `tmp/birenci-infra-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "birenci-infra-0.0.1.tar", last modified: Tue Apr 18 03:21:37 2023, max compression
+gzip compressed data, was "birenci-infra-0.0.2.tar", last modified: Tue Apr 18 03:47:26 2023, max compression
```

## Comparing `birenci-infra-0.0.1.tar` & `birenci-infra-0.0.2.tar`

### file list

```diff
@@ -1,45 +1,43 @@
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:21:37.820931 birenci-infra-0.0.1/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1077 2023-04-18 03:17:45.000000 birenci-infra-0.0.1/LICENSE.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      375 2023-04-18 03:21:37.820931 birenci-infra-0.0.1/PKG-INFO
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:16:29.000000 birenci-infra-0.0.1/README.md
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:21:37.816930 birenci-infra-0.0.1/birenci_infra.egg-info/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      375 2023-04-18 03:21:37.000000 birenci-infra-0.0.1/birenci_infra.egg-info/PKG-INFO
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      771 2023-04-18 03:21:37.000000 birenci-infra-0.0.1/birenci_infra.egg-info/SOURCES.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        1 2023-04-18 03:21:37.000000 birenci-infra-0.0.1/birenci_infra.egg-info/dependency_links.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        4 2023-04-18 03:21:37.000000 birenci-infra-0.0.1/birenci_infra.egg-info/top_level.txt
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:21:37.816930 birenci-infra-0.0.1/sdk/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/__init__.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:21:37.816930 birenci-infra-0.0.1/sdk/apis/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/apis/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1530 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/apis/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1631 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/apis/client.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     4188 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/apis/pdu.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1932 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/apis/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1291 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/apis/pr.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:21:37.816930 birenci-infra-0.0.1/sdk/config/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      378 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/config/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      175 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/config/develop.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      176 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/config/prod.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:21:37.816930 birenci-infra-0.0.1/sdk/handles/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/handles/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3694 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/handles/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3429 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/handles/pdu.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     7944 2023-04-17 06:54:45.000000 birenci-infra-0.0.1/sdk/handles/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1502 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/handles/pr.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3697 2023-04-17 06:21:23.000000 birenci-infra-0.0.1/sdk/run.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:21:37.816930 birenci-infra-0.0.1/sdk/schemas/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/schemas/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      499 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/schemas/jenkins.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      619 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/schemas/pull_request.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      144 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/schemas/pull_request_job.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       94 2023-04-17 06:54:19.000000 birenci-infra-0.0.1/sdk/schemas/test_case.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      540 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/test_hander_perf.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:21:37.820931 birenci-infra-0.0.1/sdk/utils/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/utils/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1292 2023-04-17 06:18:32.000000 birenci-infra-0.0.1/sdk/utils/csv_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      369 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/utils/file_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      269 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/utils/json_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       83 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/utils/pd_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      533 2023-04-12 09:21:26.000000 birenci-infra-0.0.1/sdk/utils/xml_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-04-18 03:21:37.820931 birenci-infra-0.0.1/setup.cfg
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      583 2023-04-18 03:20:42.000000 birenci-infra-0.0.1/setup.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:47:26.306518 birenci-infra-0.0.2/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1078 2023-04-18 03:41:13.000000 birenci-infra-0.0.2/LICENSE.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1975 2023-04-18 03:47:26.306518 birenci-infra-0.0.2/PKG-INFO
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1609 2023-04-18 03:36:01.000000 birenci-infra-0.0.2/README.md
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:47:26.302518 birenci-infra-0.0.2/apis/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/apis/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1530 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/apis/build.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1631 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/apis/client.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     4188 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/apis/pdu.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1932 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/apis/perf.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1291 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/apis/pr.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:47:26.302518 birenci-infra-0.0.2/birenci_infra.egg-info/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1975 2023-04-18 03:47:26.000000 birenci-infra-0.0.2/birenci_infra.egg-info/PKG-INFO
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      636 2023-04-18 03:47:26.000000 birenci-infra-0.0.2/birenci_infra.egg-info/SOURCES.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        1 2023-04-18 03:47:26.000000 birenci-infra-0.0.2/birenci_infra.egg-info/dependency_links.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-04-18 03:47:26.000000 birenci-infra-0.0.2/birenci_infra.egg-info/top_level.txt
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:47:26.302518 birenci-infra-0.0.2/config/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      378 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/config/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      175 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/config/develop.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      176 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/config/prod.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:47:26.306518 birenci-infra-0.0.2/handles/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/handles/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3694 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/handles/build.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3429 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/handles/pdu.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     7944 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/handles/perf.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1502 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/handles/pr.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:47:26.306518 birenci-infra-0.0.2/schemas/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/schemas/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      499 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/schemas/jenkins.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      619 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/schemas/pull_request.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      144 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/schemas/pull_request_job.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       94 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/schemas/test_case.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:47:26.306518 birenci-infra-0.0.2/sdk/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:40:10.000000 birenci-infra-0.0.2/sdk/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-04-18 03:47:26.306518 birenci-infra-0.0.2/setup.cfg
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      588 2023-04-18 03:47:24.000000 birenci-infra-0.0.2/setup.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:47:26.306518 birenci-infra-0.0.2/utils/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/utils/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1292 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/utils/csv_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      369 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/utils/file_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      269 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/utils/json_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       83 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/utils/pd_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      533 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/utils/xml_utils.py
```

### Comparing `birenci-infra-0.0.1/LICENSE.txt` & `birenci-infra-0.0.2/LICENSE.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
  
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `birenci-infra-0.0.1/sdk/apis/build.py` & `birenci-infra-0.0.2/apis/build.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.1/sdk/apis/client.py` & `birenci-infra-0.0.2/apis/client.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.1/sdk/apis/pdu.py` & `birenci-infra-0.0.2/apis/pdu.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.1/sdk/apis/perf.py` & `birenci-infra-0.0.2/apis/perf.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.1/sdk/apis/pr.py` & `birenci-infra-0.0.2/apis/pr.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.1/sdk/handles/build.py` & `birenci-infra-0.0.2/handles/build.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.1/sdk/handles/pdu.py` & `birenci-infra-0.0.2/handles/pdu.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.1/sdk/handles/perf.py` & `birenci-infra-0.0.2/handles/perf.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.1/sdk/handles/pr.py` & `birenci-infra-0.0.2/handles/pr.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.1/sdk/schemas/pull_request.py` & `birenci-infra-0.0.2/schemas/pull_request.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.1/sdk/utils/csv_utils.py` & `birenci-infra-0.0.2/utils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.1/sdk/utils/xml_utils.py` & `birenci-infra-0.0.2/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.1/setup.py` & `birenci-infra-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+
 import setuptools 
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="birenci-infra", 
-    version="0.0.1",    
-    author="infra team",   
+    version="0.0.2",    
+    author="br_infra",    
     author_email="br_infra@birentech.com",    
-    description="br_ci_db sdk",
+    description="biren ci sdk",
     long_description=long_description,    
     long_description_content_type="text/markdown",
-    url="https://gitlab.birentech.com/software/br_ci_db", 
+    url="https://gitlab.birentech.com/software/br_ci_db",    
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
-    python_requires='>=3.6', 
+    python_requires='>=3.6',   
 )
```

