# Comparing `tmp/certificates-1.1.0.tar.gz` & `tmp/certificates-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certificates-1.1.0.tar", max compression
+gzip compressed data, was "certificates-1.2.0.tar", max compression
```

## Comparing `certificates-1.1.0.tar` & `certificates-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    11357 2022-08-08 23:58:18.162426 certificates-1.1.0/LICENSE
--rw-r--r--   0        0        0      965 2022-08-08 23:58:18.162426 certificates-1.1.0/README.md
--rw-r--r--   0        0        0      809 2022-08-08 23:58:18.162426 certificates-1.1.0/certificates/__main__.py
--rw-r--r--   0        0        0     1416 2022-08-08 23:58:18.162426 certificates-1.1.0/certificates/certificates.py
--rw-r--r--   0        0        0      729 2022-08-08 23:58:18.162426 certificates-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1706 2022-08-08 23:58:30.804210 certificates-1.1.0/setup.py
--rw-r--r--   0        0        0     1532 2022-08-08 23:58:30.804484 certificates-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-17 23:24:44.279975 certificates-1.2.0/LICENSE
+-rw-r--r--   0        0        0      965 2023-04-17 23:24:44.279975 certificates-1.2.0/README.md
+-rw-r--r--   0        0        0      809 2023-04-17 23:24:44.279975 certificates-1.2.0/certificates/__main__.py
+-rw-r--r--   0        0        0     1416 2023-04-17 23:24:44.279975 certificates-1.2.0/certificates/certificates.py
+-rw-r--r--   0        0        0      731 2023-04-17 23:24:44.279975 certificates-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 certificates-1.2.0/PKG-INFO
```

### Comparing `certificates-1.1.0/LICENSE` & `certificates-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `certificates-1.1.0/README.md` & `certificates-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `certificates-1.1.0/certificates/__main__.py` & `certificates-1.2.0/certificates/__main__.py`

 * *Files identical despite different names*

### Comparing `certificates-1.1.0/certificates/certificates.py` & `certificates-1.2.0/certificates/certificates.py`

 * *Files identical despite different names*

### Comparing `certificates-1.1.0/pyproject.toml` & `certificates-1.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "certificates"
-version = "1.1.0"
+version = "1.2.0"
 description = "Generate event certificates easily."
 readme = "README.md"
 homepage = "https://github.com/cassiobotaro/certificates"
 authors = ["cassiobotaro <cassiobotaro@gmail.com>"]
 license = "Apache-2.0"
-packages = [{include = "certificates"}]
+packages = [{ include = "certificates" }]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 
 [tool.poetry.dev-dependencies]
-black = "^22.6"
+black = "^23.3"
 flake8 = "^5.0.4"
-isort = "^5.10.1"
-pytest = "^7.0.1"
-pytest-cov = "^3.0.0"
+isort = "^5.12.0"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
 
 [tool.poetry.scripts]
 certificates = "certificates.__main__:main"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `certificates-1.1.0/setup.py` & `certificates-1.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,57 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: certificates
+Version: 1.2.0
+Summary: Generate event certificates easily.
+Home-page: https://github.com/cassiobotaro/certificates
+License: Apache-2.0
+Author: cassiobotaro
+Author-email: cassiobotaro@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
 
-packages = \
-['certificates']
+#  Certificates
 
-package_data = \
-{'': ['*']}
+Generate event certificates easily.
 
-entry_points = \
-{'console_scripts': ['certificates = certificates.__main__:main']}
-
-setup_kwargs = {
-    'name': 'certificates',
-    'version': '1.1.0',
-    'description': 'Generate event certificates easily.',
-    'long_description': '#  Certificates\n\nGenerate event certificates easily.\n\n## Requirements\n\n* Inkscape (`apt install inkscape`)\n\n## Installation\n\nUse the package manager [pip](https://pip.pypa.io/en/stable/) to install certificates.\n\n```bash\npip install certificates\n```\n\n## Usage\n\n`certificates participants.csv template.svg`\n\n```\nusage: certificates [-h] [--output OUTPUT] participants template\n\npositional arguments:\n  participants          csv filaname containing participants\n  template              certificate template in svg format used to build\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --output OUTPUT, -o OUTPUT\n                        destination of the generated certificates\n```\n\n## Contributing\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nPlease make sure to update tests as appropriate.\n\n## License\n[Apache 2.0](https://choosealicense.com/licenses/apache-2.0/)\n',
-    'author': 'cassiobotaro',
-    'author_email': 'cassiobotaro@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/cassiobotaro/certificates',
-    'packages': packages,
-    'package_data': package_data,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+## Requirements
 
+* Inkscape (`apt install inkscape`)
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install certificates.
+
+```bash
+pip install certificates
+```
+
+## Usage
+
+`certificates participants.csv template.svg`
+
+```
+usage: certificates [-h] [--output OUTPUT] participants template
+
+positional arguments:
+  participants          csv filaname containing participants
+  template              certificate template in svg format used to build
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --output OUTPUT, -o OUTPUT
+                        destination of the generated certificates
+```
+
+## Contributing
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+Please make sure to update tests as appropriate.
+
+## License
+[Apache 2.0](https://choosealicense.com/licenses/apache-2.0/)
 
-setup(**setup_kwargs)
```

