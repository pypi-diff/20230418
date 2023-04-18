# Comparing `tmp/faker-security-0.2.0.tar.gz` & `tmp/faker_security-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faker-security-0.2.0.tar", max compression
+gzip compressed data, was "faker_security-0.3.1.tar", max compression
```

## Comparing `faker-security-0.2.0.tar` & `faker_security-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      550 2022-03-22 16:37:01.069428 faker-security-0.2.0/LICENSE
--rw-r--r--   0        0        0     1101 2022-03-22 16:37:01.069428 faker-security-0.2.0/README.md
--rw-r--r--   0        0        0     2631 2022-03-22 16:37:01.069428 faker-security-0.2.0/faker_security/providers.py
--rw-r--r--   0        0        0      826 2022-03-22 16:37:01.069428 faker-security-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1822 2022-03-22 16:37:28.130840 faker-security-0.2.0/setup.py
--rw-r--r--   0        0        0     1791 2022-03-22 16:37:28.131188 faker-security-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      550 2023-04-18 16:42:59.742859 faker_security-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1569 2023-04-18 16:42:59.742859 faker_security-0.3.1/README.md
+-rw-r--r--   0        0        0     2972 2023-04-18 16:42:59.742859 faker_security-0.3.1/faker_security/providers.py
+-rw-r--r--   0        0        0      826 2023-04-18 16:42:59.742859 faker_security-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2299 1970-01-01 00:00:00.000000 faker_security-0.3.1/setup.py
+-rw-r--r--   0        0        0     2310 1970-01-01 00:00:00.000000 faker_security-0.3.1/PKG-INFO
```

### Comparing `faker-security-0.2.0/LICENSE` & `faker_security-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `faker-security-0.2.0/faker_security/providers.py` & `faker_security-0.3.1/faker_security/providers.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,29 +2,38 @@
 Custom providers for the Faker library that help generate random data within
 our factories.
 """
 
 import random
 from typing import Tuple
 
+from faker import Faker
 from faker.providers import BaseProvider
 
+fake = Faker()
+
 
 class SecurityProvider(BaseProvider):
     def version(
         self,
         major_range: Tuple[int, int] = (1, 10),
         minor_range: Tuple[int, int] = (1, 10),
         patch_range: Tuple[int, int] = (1, 10),
     ):
         major = random.randint(*major_range)
         minor = random.randint(*minor_range)
         patch = random.randint(*patch_range)
         return f"{major}.{minor}.{patch}"
 
+    def snyk_id(self, suffix_range: Tuple[int, int] = (1000, 90000)):
+        ecosystem = random.choice(["python", "java", "ruby", "dotnet"]).upper()
+        slug = fake.slug().replace("-", "").upper()
+        suffix = random.randint(*suffix_range)
+        return f"SNYK-{ecosystem}-{slug}-{suffix}"
+
     def npm_semver_range(self):
         version = self.version()
         operator = random.choice(["=", "<", ">", "<=", ">="])
         return f"{operator}{version}"
 
     def cwe(self, range: Tuple[int, int] = (1, 1000)):
         value = random.randint(*range)
```

### Comparing `faker-security-0.2.0/pyproject.toml` & `faker_security-0.3.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "faker-security"
-version = "0.2.0"
+version = "0.3.1"
 description = "Faker provider for security related data"
 authors = ["Snyk Security R&D <security-engineering@snyk.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/snyk/faker-security"
 repository = "https://github.com/snyk/faker-security"
 keywords = ["faker"]
```

### Comparing `faker-security-0.2.0/setup.py` & `faker_security-0.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 {'': ['*']}
 
 install_requires = \
 ['faker>=8.2.1']
 
 setup_kwargs = {
     'name': 'faker-security',
-    'version': '0.2.0',
+    'version': '0.3.1',
     'description': 'Faker provider for security related data',
-    'long_description': '# Faker-Security\n\nProvider for [Faker](https://github.com/joke2k/faker)\nto generate random/fake data related to security.\n\n## Requirements\n\n- Faker\n- Python 3.9+\n\n## Installation and Usage\n\n- Add `faker-security` to your requirements\n- Install `faker-security` using `pip` or whatever package manager you use\n- Add the `SecurityProvider` during tests or wherever you use Faker\n\n```python\nfrom faker import Faker\nfrom faker_security.providers import SecurityProvider\n\nfake = Faker()\nfake.add_provider(SecurityProvider)\n\n# generate a CVSSv3 vector\nfake.cvss3()\n```\n\n## Provider Features\n\n- `cvss3`: generates a CVSS v3 vector\n- `cvss2`: generates a CVSS v2 vector\n- `version`: generates a [semver version number](https://semver.org/)\n- `npm_semver_range`: generates a [npm compatible semver version range](https://docs.npmjs.com/about-semantic-versioning)\n- `cwe`: generates a CWE identifier\n- `cve`: generates a CVE identifier\n\n## Developing\n\n- Install `poetry` and run `poetry install`\n- Install `pre-commit` and run `pre-commit install --install-hooks`\n\n## Testing\n\n`poetry run pytest` to run tests.\n',
+    'long_description': "# Faker-Security\n\n[![Pypi](https://badge.fury.io/py/faker-security.svg)](https://pypi.org/project/faker-security/)\n[![CircleCI](https://circleci.com/gh/snyk/faker-security/tree/main.svg?style=svg)](https://circleci.com/gh/snyk/faker-security/tree/main)\n\nProvider for [Faker](https://github.com/joke2k/faker)\nto generate random/fake data related to security.\n\n## Requirements\n\n- Faker\n- Python 3.8+\n\n## Installation and Usage\n\nIf you want to use `faker-security` within your project, add it to your dependency file of choice.\n\nThis is typically your project's `requirements.txt` file. If you are using a higher-level package manager like `poetry` or `pipenv`, follow their instructions for adding new packages.\n\nOnce installed, you need to setup `Faker` to make use of the `SecurityProvider`. An example of how that could be done is shown below:\n\n```python\nfrom faker import Faker\nfrom faker_security.providers import SecurityProvider\n\nfake = Faker()\nfake.add_provider(SecurityProvider)\n\n# generate a CVSSv3 vector\nfake.cvss3()\n```\n\n## Provider Features\n\n- `cvss3`: generates a CVSS v3 vector\n- `cvss2`: generates a CVSS v2 vector\n- `version`: generates a [semver version number](https://semver.org/)\n- `npm_semver_range`: generates a [npm compatible semver version range](https://docs.npmjs.com/about-semantic-versioning)\n- `cwe`: generates a CWE identifier\n- `cve`: generates a CVE identifier\n\n## Developing\n\n- Install `poetry` and run `poetry install`\n- Install `pre-commit` and run `pre-commit install --install-hooks`\n\n## Testing\n\n`poetry run pytest` to run tests.\n",
     'author': 'Snyk Security R&D',
     'author_email': 'security-engineering@snyk.io',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/snyk/faker-security',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `faker-security-0.2.0/PKG-INFO` & `faker_security-0.3.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 Metadata-Version: 2.1
 Name: faker-security
-Version: 0.2.0
+Version: 0.3.1
 Summary: Faker provider for security related data
 Home-page: https://github.com/snyk/faker-security
 License: Apache-2.0
 Keywords: faker
 Author: Snyk Security R&D
 Author-email: security-engineering@snyk.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: faker (>=8.2.1)
 Project-URL: Repository, https://github.com/snyk/faker-security
 Description-Content-Type: text/markdown
 
 # Faker-Security
 
+[![Pypi](https://badge.fury.io/py/faker-security.svg)](https://pypi.org/project/faker-security/)
+[![CircleCI](https://circleci.com/gh/snyk/faker-security/tree/main.svg?style=svg)](https://circleci.com/gh/snyk/faker-security/tree/main)
+
 Provider for [Faker](https://github.com/joke2k/faker)
 to generate random/fake data related to security.
 
 ## Requirements
 
 - Faker
-- Python 3.9+
+- Python 3.8+
 
 ## Installation and Usage
 
-- Add `faker-security` to your requirements
-- Install `faker-security` using `pip` or whatever package manager you use
-- Add the `SecurityProvider` during tests or wherever you use Faker
+If you want to use `faker-security` within your project, add it to your dependency file of choice.
+
+This is typically your project's `requirements.txt` file. If you are using a higher-level package manager like `poetry` or `pipenv`, follow their instructions for adding new packages.
+
+Once installed, you need to setup `Faker` to make use of the `SecurityProvider`. An example of how that could be done is shown below:
 
 ```python
 from faker import Faker
 from faker_security.providers import SecurityProvider
 
 fake = Faker()
 fake.add_provider(SecurityProvider)
```

