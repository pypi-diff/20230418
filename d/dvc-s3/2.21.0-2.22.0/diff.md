# Comparing `tmp/dvc-s3-2.21.0.tar.gz` & `tmp/dvc-s3-2.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-s3-2.21.0.tar", last modified: Thu Nov  3 14:59:36 2022, max compression
+gzip compressed data, was "dvc-s3-2.22.0.tar", last modified: Tue Apr 18 08:38:08 2023, max compression
```

## Comparing `dvc-s3-2.21.0.tar` & `dvc-s3-2.22.0.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-03 14:59:36.478433 dvc-s3-2.21.0/
--rw-r--r--   0 runner    (1001) docker     (116)      349 2022-11-03 14:59:16.000000 dvc-s3-2.21.0/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-03 14:59:36.470434 dvc-s3-2.21.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-03 14:59:36.474434 dvc-s3-2.21.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)      587 2022-11-03 14:59:16.000000 dvc-s3-2.21.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     2427 2022-11-03 14:59:16.000000 dvc-s3-2.21.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      634 2022-11-03 14:59:16.000000 dvc-s3-2.21.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     1827 2022-11-03 14:59:16.000000 dvc-s3-2.21.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     1297 2022-11-03 14:59:16.000000 dvc-s3-2.21.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2022-11-03 14:59:16.000000 dvc-s3-2.21.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      677 2022-11-03 14:59:36.478433 dvc-s3-2.21.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       26 2022-11-03 14:59:16.000000 dvc-s3-2.21.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-03 14:59:36.474434 dvc-s3-2.21.0/dvc_s3/
--rw-r--r--   0 runner    (1001) docker     (116)     7537 2022-11-03 14:59:16.000000 dvc-s3-2.21.0/dvc_s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      178 2022-11-03 14:59:36.000000 dvc-s3-2.21.0/dvc_s3/_dvc_s3_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     1656 2022-11-03 14:59:16.000000 dvc-s3-2.21.0/dvc_s3/path.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-03 14:59:36.478433 dvc-s3-2.21.0/dvc_s3/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-11-03 14:59:16.000000 dvc-s3-2.21.0/dvc_s3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2186 2022-11-03 14:59:16.000000 dvc-s3-2.21.0/dvc_s3/tests/cloud.py
--rw-r--r--   0 runner    (1001) docker     (116)      170 2022-11-03 14:59:16.000000 dvc-s3-2.21.0/dvc_s3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)       96 2022-11-03 14:59:16.000000 dvc-s3-2.21.0/dvc_s3/tests/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1919 2022-11-03 14:59:16.000000 dvc-s3-2.21.0/dvc_s3/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (116)     1292 2022-11-03 14:59:16.000000 dvc-s3-2.21.0/dvc_s3/tests/test_dvc.py
--rw-r--r--   0 runner    (1001) docker     (116)      713 2022-11-03 14:59:16.000000 dvc-s3-2.21.0/dvc_s3/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-03 14:59:36.478433 dvc-s3-2.21.0/dvc_s3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      677 2022-11-03 14:59:36.000000 dvc-s3-2.21.0/dvc_s3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      617 2022-11-03 14:59:36.000000 dvc-s3-2.21.0/dvc_s3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-03 14:59:36.000000 dvc-s3-2.21.0/dvc_s3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-03 14:59:36.000000 dvc-s3-2.21.0/dvc_s3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      538 2022-11-03 14:59:36.000000 dvc-s3-2.21.0/dvc_s3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2022-11-03 14:59:36.000000 dvc-s3-2.21.0/dvc_s3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2146 2022-11-03 14:59:16.000000 dvc-s3-2.21.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)     1693 2022-11-03 14:59:36.478433 dvc-s3-2.21.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-11-03 14:59:16.000000 dvc-s3-2.21.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 08:38:08.664608 dvc-s3-2.22.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 08:38:08.660608 dvc-s3-2.22.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 08:38:08.664608 dvc-s3-2.22.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1827 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-04-18 08:38:08.664608 dvc-s3-2.22.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 08:38:08.664608 dvc-s3-2.22.0/dvc_s3/
+-rw-r--r--   0 runner    (1001) docker     (122)     7537 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/dvc_s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-04-18 08:38:08.000000 dvc-s3-2.22.0/dvc_s3/_dvc_s3_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1656 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/dvc_s3/path.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 08:38:08.664608 dvc-s3-2.22.0/dvc_s3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/dvc_s3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/dvc_s3/tests/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/dvc_s3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/dvc_s3/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1935 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/dvc_s3/tests/test_dvc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      713 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/dvc_s3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 08:38:08.664608 dvc-s3-2.22.0/dvc_s3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-04-18 08:38:08.000000 dvc-s3-2.22.0/dvc_s3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-04-18 08:38:08.000000 dvc-s3-2.22.0/dvc_s3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-18 08:38:08.000000 dvc-s3-2.22.0/dvc_s3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-18 08:38:08.000000 dvc-s3-2.22.0/dvc_s3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      543 2023-04-18 08:38:08.000000 dvc-s3-2.22.0/dvc_s3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-18 08:38:08.000000 dvc-s3-2.22.0/dvc_s3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-04-18 08:38:08.664608 dvc-s3-2.22.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/setup.py
```

### Comparing `dvc-s3-2.21.0/.github/workflows/update-template.yaml` & `dvc-s3-2.22.0/.github/workflows/update-template.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 name: Update template
 
 on:
   schedule:
     - cron: '5 1 * * *'  # every day at 01:05
-
   workflow_dispatch:
 
 jobs:
   update:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Install deps
       run: pip install cruft
     - name: Update template
       id: update
       run: |
         cruft update -y
         echo "::set-output name=changes::$(git diff)"
     - name: Create PR
       if: ${{ steps.update.outputs.changes != '' }}
       uses: peter-evans/create-pull-request@v3
       with:
         commit-message: update template
         title: update template
         token: ${{ secrets.WORKFLOW_TOKEN }}
-
```

### Comparing `dvc-s3-2.21.0/.gitignore` & `dvc-s3-2.22.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-s3-2.21.0/.pre-commit-config.yaml` & `dvc-s3-2.22.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -19,24 +19,24 @@
           - ba,datas,fo,uptodate
     repo: https://github.com/codespell-project/codespell
     rev: v2.1.0
   - hooks:
       - id: isort
         language_version: python3
     repo: https://github.com/timothycrosley/isort
-    rev: 5.9.3
+    rev: 5.12.0
   - hooks:
       - id: flake8
         language_version: python3
         additional_dependencies:
           - flake8-bugbear
           - flake8-comprehensions
           - flake8-debugger
           - flake8-string-format
-    repo: https://gitlab.com/pycqa/flake8
+    repo: https://github.com/pycqa/flake8
     rev: 3.9.2
   - repo: local
     hooks:
     - id: mypy
       name: mypy
       entry: mypy
       files: ^dvc_s3/
```

### Comparing `dvc-s3-2.21.0/LICENSE` & `dvc-s3-2.22.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-s3-2.21.0/PKG-INFO` & `dvc-s3-2.22.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: dvc-s3
-Version: 2.21.0
+Version: 2.22.0
 Summary: s3 plugin for dvc
 Home-page: http://dvc.org
 Download-URL: https://github.com/iterative/dvc-s3
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Source, https://github.com/iterative/dvc-s3
 Keywords: dvc,s3
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 License-File: LICENSE
 
 dvc-s3
```

### Comparing `dvc-s3-2.21.0/dvc_s3/__init__.py` & `dvc-s3-2.22.0/dvc_s3/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-s3-2.21.0/dvc_s3/path.py` & `dvc-s3-2.22.0/dvc_s3/path.py`

 * *Files identical despite different names*

### Comparing `dvc-s3-2.21.0/dvc_s3/tests/cloud.py` & `dvc-s3-2.22.0/dvc_s3/tests/cloud.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,24 +3,20 @@
 import uuid
 
 from dvc.testing.cloud import Cloud
 from dvc.testing.path_info import CloudURLInfo
 from funcy import cached_property
 
 TEST_AWS_REPO_BUCKET = os.environ.get("DVC_TEST_AWS_REPO_BUCKET", "dvc-temp")
-TEST_AWS_ENDPOINT_URL = "http://127.0.0.1:{port}/"
 
 
 class S3(Cloud, CloudURLInfo):
-
-    TEST_AWS_ENDPOINT_URL = None
-
     @property
     def config(self):
-        return {"url": self.url, "endpointurl": self.TEST_AWS_ENDPOINT_URL}
+        return {"url": self.url}
 
     @staticmethod
     def _get_storagepath():
         return (
             TEST_AWS_REPO_BUCKET
             + "/"
             + "dvc_test_caches"
@@ -77,7 +73,27 @@
             encoding = locale.getpreferredencoding(False)
         assert errors is None
         return self.read_bytes().decode(encoding)
 
     @property
     def fs_path(self):
         return self.bucket + "/" + self.path.lstrip("/")
+
+
+class FakeS3(S3):
+    """Fake S3 client that is supposed to be using a mock server's endpoint"""
+
+    def __init__(self, *args, endpoint_url: str, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.endpoint_url = endpoint_url
+
+    def __truediv__(self, key):
+        ret = super().__truediv__(key)
+        ret.endpoint_url = self.endpoint_url
+        return ret
+
+    @property
+    def config(self):
+        return {"url": self.url, "endpointurl": self.endpoint_url}
+
+    def get_url(self):  # pylint: disable=arguments-differ
+        return str(self)
```

### Comparing `dvc-s3-2.21.0/dvc_s3/tests/test_utils.py` & `dvc-s3-2.22.0/dvc_s3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-s3-2.21.0/dvc_s3.egg-info/PKG-INFO` & `dvc-s3-2.22.0/dvc_s3.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: dvc-s3
-Version: 2.21.0
+Version: 2.22.0
 Summary: s3 plugin for dvc
 Home-page: http://dvc.org
 Download-URL: https://github.com/iterative/dvc-s3
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Source, https://github.com/iterative/dvc-s3
 Keywords: dvc,s3
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 License-File: LICENSE
 
 dvc-s3
```

### Comparing `dvc-s3-2.21.0/dvc_s3.egg-info/SOURCES.txt` & `dvc-s3-2.22.0/dvc_s3.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -17,11 +17,10 @@
 dvc_s3.egg-info/dependency_links.txt
 dvc_s3.egg-info/not-zip-safe
 dvc_s3.egg-info/requires.txt
 dvc_s3.egg-info/top_level.txt
 dvc_s3/tests/__init__.py
 dvc_s3/tests/cloud.py
 dvc_s3/tests/conftest.py
-dvc_s3/tests/docker-compose.yml
 dvc_s3/tests/fixtures.py
 dvc_s3/tests/test_dvc.py
 dvc_s3/tests/test_utils.py
```

### Comparing `dvc-s3-2.21.0/dvc_s3.egg-info/requires.txt` & `dvc-s3-2.22.0/dvc_s3.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 dvc[testing]
 pytest==6.2.5
 pytest-cov==3.0.0
 pytest-xdist==2.4.0
 pytest-mock==3.6.1
 pytest-lazy-fixture==0.6.3
 pytest-docker==0.10.3
+pytest-servers[s3]==0.2.0
 flaky==3.7.0
 mock==4.0.3
 wget==3.2
 filelock==3.3.2
 xmltodict==0.12.0
 Pygments==2.10.0
 collective.checkdocs==0.2
 pydocstyle==6.1.1
-pylint==2.11.1
-pylint-pytest==1.1.2
+pylint==2.15.9
 pylint-plugin-utils==0.6
-mypy==0.910
+mypy==0.991
 types-requests==2.25.11
 types-tabulate==0.8.3
 types-toml==0.10.1
 
 [tests:sys_platform == "win32"]
 pywin32>=225
```

### Comparing `dvc-s3-2.21.0/pyproject.toml` & `dvc-s3-2.22.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -50,20 +50,19 @@
 warn_redundant_casts = true
 warn_unreachable = true
 files = ["dvc_s3"]
 
 [tool.pylint.master]
 extension-pkg-whitelist = ["pygit2"]
 init-hook = "import sys; sys.path.append(str('tests'))"
-load-plugins = ["pylint_pytest"]
 
 [tool.pylint.message_control]
 disable = [
-    "format", "refactoring", "spelling", "design", "no-self-use",
-    "invalid-name", "misplaced-comparison-constant", "duplicate-code", "fixme",
+    "format", "refactoring", "spelling", "design",
+    "invalid-name", "duplicate-code", "fixme",
     "unused-wildcard-import", "cyclic-import", "wrong-import-order",
     "wrong-import-position", "ungrouped-imports", "multiple-imports",
     "logging-format-interpolation", "logging-fstring-interpolation",
     "missing-function-docstring", "missing-module-docstring",
     "missing-class-docstring", "raise-missing-from", "import-outside-toplevel",
 ]
 enable = ["c-extension-no-member", "no-else-return"]
```

### Comparing `dvc-s3-2.21.0/setup.cfg` & `dvc-s3-2.22.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 keywords = dvc, s3
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 setup_requires = 
 	setuptools>=48
 	setuptools_scm[toml]>=6.3.1
 python_requires = >=3.8
 zip_safe = False
@@ -38,37 +39,37 @@
 	dvc[testing]
 	pytest==6.2.5
 	pytest-cov==3.0.0
 	pytest-xdist==2.4.0
 	pytest-mock==3.6.1
 	pytest-lazy-fixture==0.6.3
 	pytest-docker==0.10.3
+	pytest-servers[s3]==0.2.0
 	flaky==3.7.0
 	mock==4.0.3
 	wget==3.2
 	filelock==3.3.2
 	xmltodict==0.12.0
 	Pygments==2.10.0
 	collective.checkdocs==0.2
 	pydocstyle==6.1.1
-	pylint==2.11.1
-	pylint-pytest==1.1.2
+	pylint==2.15.9
 	pylint-plugin-utils==0.6
-	mypy==0.910
+	mypy==0.991
 	types-requests==2.25.11
 	types-tabulate==0.8.3
 	types-toml==0.10.1
 	pywin32>=225; sys_platform == 'win32'
 
 [flake8]
 ignore = 
-	E203, # Whitespace before ':'
-	E266, # Too many leading '#' for block comment
-	W503, # Line break occurred before a binary operator
-	P1,  # unindexed parameters in the str.format, see:
+	E203,
+	E266,
+	W503,
+	P1,
 max_line_length = 79
 max-complexity = 15
 select = B,C,E,F,W,T4,B902,T,P
 show_source = true
 count = true
 
 [egg_info]
```

