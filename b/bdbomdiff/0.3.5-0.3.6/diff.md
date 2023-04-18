# Comparing `tmp/bdbomdiff-0.3.5.tar.gz` & `tmp/bdbomdiff-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdbomdiff-0.3.5.tar", max compression
+gzip compressed data, was "bdbomdiff-0.3.6.tar", max compression
```

## Comparing `bdbomdiff-0.3.5.tar` & `bdbomdiff-0.3.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    12803 2022-11-25 20:28:57.291231 bdbomdiff-0.3.5/bdbomdiff/__init__.py
--rw-r--r--   0        0        0    49192 2022-10-16 14:02:55.406721 bdbomdiff-0.3.5/bdbomdiff/template_aosd_new.xlsx
--rw-r--r--   0        0        0     1068 2022-10-16 14:02:55.337718 bdbomdiff-0.3.5/LICENSE
--rw-r--r--   0        0        0      516 2022-11-25 20:28:48.177055 bdbomdiff-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     1835 2022-11-25 20:30:02.066854 bdbomdiff-0.3.5/README.md
--rw-r--r--   0        0        0     2712 2022-11-25 20:31:32.940063 bdbomdiff-0.3.5/setup.py
--rw-r--r--   0        0        0     2338 2022-11-25 20:31:32.940063 bdbomdiff-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    12806 2023-04-18 16:39:49.911126 bdbomdiff-0.3.6/bdbomdiff/__init__.py
+-rw-r--r--   0        0        0    49192 2022-10-16 14:02:55.406721 bdbomdiff-0.3.6/bdbomdiff/template_aosd_new.xlsx
+-rw-r--r--   0        0        0     1068 2022-10-16 14:02:55.337718 bdbomdiff-0.3.6/LICENSE
+-rw-r--r--   0        0        0      516 2023-04-18 16:33:28.916142 bdbomdiff-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     1835 2022-11-25 20:30:02.066854 bdbomdiff-0.3.6/README.md
+-rw-r--r--   0        0        0     2712 2023-04-18 16:40:00.461338 bdbomdiff-0.3.6/setup.py
+-rw-r--r--   0        0        0     2338 2023-04-18 16:40:00.461338 bdbomdiff-0.3.6/PKG-INFO
```

### Comparing `bdbomdiff-0.3.5/bdbomdiff/__init__.py` & `bdbomdiff-0.3.6/bdbomdiff/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,17 +213,16 @@
                                 cl = (
                                     f'{l.get("spdxId","NA")}'
                                     if len(licenses) == 1
                                     else f'{cl}, {l.get("spdxId","============")}'
                                 )
                         co = ""
                         if origins:
-                            copyright_infos = []
                             for o in origins:
-
+                                copyright_infos = []
                                 origin_url = hub.get_link(o, "origin")
                                 origin_details = hub.execute_get(origin_url).json()
                                 url = hub.get_link(origin_details, "file-copyrights")
                                 copyright_info = (
                                     hub.execute_get(url).json().get("items", [])
                                 )
                                 if len(copyright_info) > 0:
```

### Comparing `bdbomdiff-0.3.5/bdbomdiff/template_aosd_new.xlsx` & `bdbomdiff-0.3.6/bdbomdiff/template_aosd_new.xlsx`

 * *Files identical despite different names*

### Comparing `bdbomdiff-0.3.5/LICENSE` & `bdbomdiff-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bdbomdiff-0.3.5/pyproject.toml` & `bdbomdiff-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bdbomdiff"
-version = "0.3.5"
+version = "0.3.6"
 description = "Blackduck BOM Diff to excel for AOSD import"
 authors = ["dineshr93gmail.com"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `bdbomdiff-0.3.5/README.md` & `bdbomdiff-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `bdbomdiff-0.3.5/setup.py` & `bdbomdiff-0.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'openpyxl>=3.0.10,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['bdbomdiff = bdbomdiff:main']}
 
 setup_kwargs = {
     'name': 'bdbomdiff',
-    'version': '0.3.5',
+    'version': '0.3.6',
     'description': 'Blackduck BOM Diff to excel for AOSD import',
     'long_description': '# BDBOMDIFF\n\nBlackduck BOM Diff to excel for AOSD import\n\n## Description\n\nThis is intended for finding new OSS component to be imported into AOSD\n\n## Getting Started\n\n### Dependencies\n\n- Blackduck\n- importlib-resources\n- openpyxl\n\n### Installing\n\n- pip install bdbomdiff\n\n### Executing program\n\n- How to run the program\n\n```\n<!-- on the folder it is running place this blackduck config file for blackduck library-->\n.restconfig.json\n{\n    <!-- make sure Blackduck_url should not end with slash -->\n  "baseurl": "Blackduck_url",\n  "api_token": "API_KEY",\n  "insecure": true,\n  "debug": false\n}\n\nbdbomdiff PROJECT_NAME NEW_VERSION OLD_VERSION -o OUTPUT_DIR\n\n```\n\n## Help\n\nAny advise for common problems or issues.\n\n```\n>bdbomdiff -h\nusage: Retreive BOM component info for the given project and version [-h] -o O [-l LIMIT | -u | -r] [-v] [-c] project_name version oldversion\n\npositional arguments:\n  project_name\n  version\n  oldversion\n\noptions:\n  -h, --help            show this help message and exit\n  -o O                  Output directory\n  -l LIMIT, --limit LIMIT\n                        Set limit on number of components to retrieve\n  -u, --unreviewed\n  -r, --reviewed\n  -v, --vulnerabilities\n                        Get the vulnerability info for each of the components\n  -c, --custom_fields   Get the custom field info for each of the components\n```\n\n## Authors\n\nDinesh Ravi\n\n## Version History\n\n- 0.3.0\n  - get license, homepage url, description, copyright and files info,\n- 0.2.0\n  - Documentation update\n- 0.1.0\n  - Initial Release\n\n## License\n\nThis project is licensed under the MIT License - see the [MIT](LICENSE) file for details\n\n## Acknowledgments\n\n- [openpyxl](https://pypi.org/project/openpyxl/)\n- [Blackduck](https://pypi.org/project/blackduck/)\n- [importlib-resources](https://pypi.org/project/importlib-resources/)\n',
     'author': 'dineshr93gmail.com',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `bdbomdiff-0.3.5/PKG-INFO` & `bdbomdiff-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdbomdiff
-Version: 0.3.5
+Version: 0.3.6
 Summary: Blackduck BOM Diff to excel for AOSD import
 License: MIT
 Author: dineshr93gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

