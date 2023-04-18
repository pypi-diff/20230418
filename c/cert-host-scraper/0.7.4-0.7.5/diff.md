# Comparing `tmp/cert_host_scraper-0.7.4.tar.gz` & `tmp/cert_host_scraper-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cert_host_scraper-0.7.4.tar", max compression
+gzip compressed data, was "cert_host_scraper-0.7.5.tar", max compression
```

## Comparing `cert_host_scraper-0.7.4.tar` & `cert_host_scraper-0.7.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-04-18 21:24:02.790647 cert_host_scraper-0.7.4/LICENSE
--rw-r--r--   0        0        0     1187 2023-04-18 21:24:02.790647 cert_host_scraper-0.7.4/README.md
--rw-r--r--   0        0        0      142 2023-04-18 21:24:02.790647 cert_host_scraper-0.7.4/cert_host_scraper/__init__.py
--rw-r--r--   0        0        0     3041 2023-04-18 21:24:02.790647 cert_host_scraper-0.7.4/cert_host_scraper/cli.py
--rw-r--r--   0        0        0     1723 2023-04-18 21:24:02.790647 cert_host_scraper-0.7.4/cert_host_scraper/scraper.py
--rw-r--r--   0        0        0      337 2023-04-18 21:24:02.790647 cert_host_scraper-0.7.4/cert_host_scraper/utils.py
--rw-r--r--   0        0        0      697 2023-04-18 21:24:02.790647 cert_host_scraper-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 cert_host_scraper-0.7.4/setup.py
--rw-r--r--   0        0        0     1884 1970-01-01 00:00:00.000000 cert_host_scraper-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-18 21:31:55.092769 cert_host_scraper-0.7.5/LICENSE
+-rw-r--r--   0        0        0     1187 2023-04-18 21:31:55.092769 cert_host_scraper-0.7.5/README.md
+-rw-r--r--   0        0        0      142 2023-04-18 21:31:55.092769 cert_host_scraper-0.7.5/cert_host_scraper/__init__.py
+-rw-r--r--   0        0        0     3077 2023-04-18 21:31:55.092769 cert_host_scraper-0.7.5/cert_host_scraper/cli.py
+-rw-r--r--   0        0        0     1723 2023-04-18 21:31:55.092769 cert_host_scraper-0.7.5/cert_host_scraper/scraper.py
+-rw-r--r--   0        0        0      337 2023-04-18 21:31:55.092769 cert_host_scraper-0.7.5/cert_host_scraper/utils.py
+-rw-r--r--   0        0        0      697 2023-04-18 21:31:55.092769 cert_host_scraper-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 cert_host_scraper-0.7.5/setup.py
+-rw-r--r--   0        0        0     1884 1970-01-01 00:00:00.000000 cert_host_scraper-0.7.5/PKG-INFO
```

### Comparing `cert_host_scraper-0.7.4/LICENSE` & `cert_host_scraper-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cert_host_scraper-0.7.4/README.md` & `cert_host_scraper-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `cert_host_scraper-0.7.4/cert_host_scraper/cli.py` & `cert_host_scraper-0.7.5/cert_host_scraper/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 def validate_status_code(
     _ctx: click.core.Context, _param: click.core.Option, value: str
 ):
     try:
         status_code = int(value)
         if not (100 <= status_code <= 599):
             raise click.BadParameter("status code must be between 100 and 599")
+        
+        return status_code
     except ValueError:
         raise click.BadParameter("must be an integer")
     except TypeError:
         return NO_STATUS_CODE_FILTER
 
 
 @click.group()
```

### Comparing `cert_host_scraper-0.7.4/cert_host_scraper/scraper.py` & `cert_host_scraper-0.7.5/cert_host_scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `cert_host_scraper-0.7.4/pyproject.toml` & `cert_host_scraper-0.7.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cert-host-scraper"
-version = "0.7.4"
+version = "0.7.5"
 description = ""
 authors = ["Malachi Soord <inverse.chi@gmail.com>"]
 license = "MIT"
 
 readme = "README.md"
 repository = "https://github.com/inverse/cert-host-scraper"
 homepage = "https://github.com/inverse/cert-host-scraper"
```

### Comparing `cert_host_scraper-0.7.4/setup.py` & `cert_host_scraper-0.7.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'single-source>=0.3.0,<0.4.0']
 
 entry_points = \
 {'console_scripts': ['cert-host-scraper = cert_host_scraper.cli:cli']}
 
 setup_kwargs = {
     'name': 'cert-host-scraper',
-    'version': '0.7.4',
+    'version': '0.7.5',
     'description': '',
     'long_description': '# Cert Host Scraper\n\n![CI](https://github.com/inverse/cert-host-scraper/workflows/CI/badge.svg)\n[![PyPI version](https://badge.fury.io/py/cert-host-scraper.svg)](https://badge.fury.io/py/cert-host-scraper)\n![PyPI downloads](https://img.shields.io/pypi/dm/cert-host-scraper?label=pypi%20downloads)\n[![License](https://img.shields.io/github/license/inverse/cert-host-scraper.svg)](LICENSE)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\nQuery the certificate transparency log from [crt.sh](https://crt.sh) by a given a keyword and returns the status code of the matched results. Optionally filtering the results by status code.\n\n<img alt="Demo of cert-host-scraper" src="https://i.imgur.com/Co3aTfO.gif" width="800" />\n\n## Usage\n\n```bash\ncert-host-scraper search your-domain.com [--status-code 200] [--clean/--no-clean]\n```\n\n## Installation\n\nWith pipx:\n\n```bash\npipx install cert-host-scraper\n```\n\nWith pip:\n\n```bash\npip install cert-host-scraper\n```\n\n## Development\n\nRequires [poetry][0] and Python 3.10.\n\n```\npoetry install\npoetry run python -m cert_host_scraper.cli\n```\n\n## License\n\nMIT\n\n[0]: https://python-poetry.org\n',
     'author': 'Malachi Soord',
     'author_email': 'inverse.chi@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/inverse/cert-host-scraper',
```

### Comparing `cert_host_scraper-0.7.4/PKG-INFO` & `cert_host_scraper-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cert-host-scraper
-Version: 0.7.4
+Version: 0.7.5
 Summary: 
 Home-page: https://github.com/inverse/cert-host-scraper
 License: MIT
 Author: Malachi Soord
 Author-email: inverse.chi@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

