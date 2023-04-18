# Comparing `tmp/krausening-15.tar.gz` & `tmp/krausening-16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krausening-15.tar", max compression
+gzip compressed data, was "krausening-16.tar", max compression
```

## Comparing `krausening-15.tar` & `krausening-16.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3893 2023-04-04 13:22:54.102596 krausening-15/README.md
--rw-r--r--   0        0        0      598 2023-04-04 14:21:49.650991 krausening-15/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-21 13:26:26.589762 krausening-15/src/krausening/__init__.py
--rw-r--r--   0        0        0       36 2022-11-21 13:26:26.589990 krausening-15/src/krausening/logging/__init__.py
--rw-r--r--   0        0        0      904 2022-11-21 13:26:26.590092 krausening-15/src/krausening/logging/log_manager.py
--rw-r--r--   0        0        0       96 2022-11-21 13:26:26.590189 krausening-15/src/krausening/properties/__init__.py
--rw-r--r--   0        0        0     2656 2022-11-21 13:26:26.590269 krausening-15/src/krausening/properties/property_encryptor.py
--rw-r--r--   0        0        0     8462 2023-04-04 13:22:54.102989 krausening-15/src/krausening/properties/property_manager.py
--rw-r--r--   0        0        0     4834 1970-01-01 00:00:00.000000 krausening-15/setup.py
--rw-r--r--   0        0        0     4686 1970-01-01 00:00:00.000000 krausening-15/PKG-INFO
+-rw-r--r--   0        0        0     3772 2023-04-18 18:44:32.709649 krausening-16/README.md
+-rw-r--r--   0        0        0      597 2023-04-18 18:44:32.710196 krausening-16/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-18 18:44:32.710376 krausening-16/src/krausening/__init__.py
+-rw-r--r--   0        0        0       36 2023-04-18 18:44:32.710567 krausening-16/src/krausening/logging/__init__.py
+-rw-r--r--   0        0        0      904 2023-04-18 18:44:32.710702 krausening-16/src/krausening/logging/log_manager.py
+-rw-r--r--   0        0        0       96 2023-04-18 18:44:32.710871 krausening-16/src/krausening/properties/__init__.py
+-rw-r--r--   0        0        0     2674 2023-04-18 18:44:32.711001 krausening-16/src/krausening/properties/property_encryptor.py
+-rw-r--r--   0        0        0     8486 2023-04-18 18:44:32.711176 krausening-16/src/krausening/properties/property_manager.py
+-rw-r--r--   0        0        0     4708 1970-01-01 00:00:00.000000 krausening-16/setup.py
+-rw-r--r--   0        0        0     4571 1970-01-01 00:00:00.000000 krausening-16/PKG-INFO
```

### Comparing `krausening-15/README.md` & `krausening-16/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 # Krausening Python - Externalized Property Management and Access for Python Projects #
+[![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://opensource.org/licenses/mit)
 [![PyPI](https://img.shields.io/pypi/v/krausening)](https://pypi.org/project/krausening/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/krausening)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/krausening)
-[![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://opensource.org/licenses/mit)
 
+Krausening property management and encryption for Python is packaged using the open-source Python Maven plugin [Habushu](https://bitbucket.org/cpointe/habushu) and made available as a [PyPI package](https://pypi.org/project/krausening/).  
 
- Krausening property management and encryption for Python is packaged using the open-source Python Maven plugin [Habushu](https://bitbucket.org/cpointe/habushu) and made available as a [PyPI package](https://pypi.org/project/krausening/).  
+## Distribution Channel
+
+Krausening Python is published to PyPI under the [krausening](https://pypi.org/project/krausening/) project and may be installed using any package installer/manager that leverages PyPI.  For example:
+
+* [Poetry](https://python-poetry.org/) - `poetry add krausening`
+* [pip](https://pip.pypa.io/) - `pip install krausening`
 
 ## Managing Properties with Krausening and Python
 
 Managing properties with Krausening's Python library utilizes a similar approach to that required by Krausening Java. Krausening Python expects that developers prime their target environment by configuring the following environment variables (which are named and leveraged in the same manner as the Java System Properties expected by Krausening Java):
 
 * `KRAUSENING_BASE`
 * `KRAUSENING_EXTENSIONS`
@@ -50,24 +56,14 @@
         if (integration_enable_str):
             integration_test_enable = (integration_enable_str == 'True')
         return integration_test_enable
     
     def reload(self):
         self.properties = PropertyManager.get_instance().get_properties('test.properties')
 ```
-
-**Note: Due to updates the M1 Apple Chip, we strongly recommend using Python >= 3.9 for compatibility reasons.**
-
-## Distribution Channel
-
-Krausening Python is published to PyPI under the [krausening](https://pypi.org/project/krausening/) project and may be installed using any package installer/manager that leverages PyPI.  For example:
-
-  * [Poetry](https://python-poetry.org/) - `poetry add krausening`
-  * [pip](https://pip.pypa.io/) - `pip install krausening`
-
 ## Releasing to PyPI
 
 Releasing Krausening Python integrates into the project's larger utilization of the `maven-release-plugin`, specifically publishing the package to PyPI during the `deploy` phase.  A [PyPI account](https://pypi.org/account/register/) with access to the [krausening](https://pypi.org/project/krausening/) project is required. PyPI account credentials should be specified in your `settings.xml` under the `<id>pypi</id>` `<server>` entry:
 
 ```xml
 <settings>
   <servers>
```

### Comparing `krausening-15/pyproject.toml` & `krausening-16/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "krausening"
-version = "15"
+version = "16"
 description = "Python implementation of Krausening"
-authors = ["Eric Konieczny <ekonieczny@cpointe-inc.com>"]
+authors = ["Eric Konieczny <ekoniec1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
-repository = "https://bitbucket.org/cpointe/krausening"
+repository = "https://github.com/TechnologyBrewery/krausening"
 
 keywords = ["properties", "configuration-management"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 javaproperties = "^0.8.1"
 cryptography = "^39.0.1"
```

### Comparing `krausening-15/src/krausening/logging/log_manager.py` & `krausening-16/src/krausening/logging/log_manager.py`

 * *Files identical despite different names*

### Comparing `krausening-15/src/krausening/properties/property_encryptor.py` & `krausening-16/src/krausening/properties/property_encryptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class PropertyEncryptor:
     """
     Provides property value encryption/decryption support via PBEWITHHMACSHA512ANDAES_256. This aligns with
     the same approach used for property encryption within the Krausening Java package.
 
     Reference: https://resultfor.dev/359470-implement-pbewithhmacsha512andaes-256-of-java-jasypt-in-python.
 
-    See https://bitbucket.org/cpointe/krausening/src/dev/ for details on encrypting values with Jasypt.
+    See https://github.com/TechnologyBrewery/krausening/tree/dev/krausening for details on encrypting values with Jasypt.
     """
 
     def encrypt(self, value_to_encrypt: str, password: bytes) -> bytes:
         return self.encrypt_pbe_with_hmac_sha512_aes_256(value_to_encrypt, password)
 
     def decrypt(self, encrypted_msg: str, password: bytes) -> str:
         return self.decrypt_pbe_with_hmac_sha512_aes_256(encrypted_msg, password)
```

### Comparing `krausening-15/src/krausening/properties/property_manager.py` & `krausening-16/src/krausening/properties/property_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 class EncryptableProperties(Properties):
     """
     Provides property value encryption/decryption support via PBEWITHHMACSHA512ANDAES_256. This aligns with
     the same approach used for property encryption within the Krausening Java package.
 
     Reference: https://resultfor.dev/359470-implement-pbewithhmacsha512andaes-256-of-java-jasypt-in-python.
 
-    See https://bitbucket.org/cpointe/krausening/src/dev/ for details on encrypting values with Jasypt.
+    See https:https://github.com/TechnologyBrewery/krausening/tree/dev/krausening for details on encrypting values with Jasypt.
     """
 
     def __init__(self, password: str) -> None:
         super().__init__()
         self.__propertyPrefix = "ENC("
         self.__propertySuffix = ")"
         self.__encryptor = PropertyEncryptor()
```

### Comparing `krausening-15/setup.py` & `krausening-16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 install_requires = \
 ['cryptography>=39.0.1,<40.0.0',
  'javaproperties>=0.8.1,<0.9.0',
  'watchdog>=2.1.9,<3.0.0']
 
 setup_kwargs = {
     'name': 'krausening',
-    'version': '15',
+    'version': '16',
     'description': 'Python implementation of Krausening',
-    'long_description': '# Krausening Python - Externalized Property Management and Access for Python Projects #\n[![PyPI](https://img.shields.io/pypi/v/krausening)](https://pypi.org/project/krausening/)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/krausening)\n![PyPI - Wheel](https://img.shields.io/pypi/wheel/krausening)\n[![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://opensource.org/licenses/mit)\n\n\n Krausening property management and encryption for Python is packaged using the open-source Python Maven plugin [Habushu](https://bitbucket.org/cpointe/habushu) and made available as a [PyPI package](https://pypi.org/project/krausening/).  \n\n## Managing Properties with Krausening and Python\n\nManaging properties with Krausening\'s Python library utilizes a similar approach to that required by Krausening Java. Krausening Python expects that developers prime their target environment by configuring the following environment variables (which are named and leveraged in the same manner as the Java System Properties expected by Krausening Java):\n\n* `KRAUSENING_BASE`\n* `KRAUSENING_EXTENSIONS`\n* `KRAUSENING_OVERRIDE_EXTENSIONS`\n* `KRAUSENING_PASSWORD`\n\nIn order to use the Krausening Python, developers may directly use `PropertyManager` or extend `PropertyManager` to provide a custom interface.  For example, developers may directly use the `PropertyManager` as such:\n\n```python\nfrom krausening.properties import PropertyManager\n\npropertyManager = PropertyManager.get_instance()\nproperties = None\nproperties = propertyManager.get_properties(\'my-property-file.properties\')\nassert properties[\'foo\'] == \'bar2\'\n```\n\nThis has the disadvantage that you must know the property keys in order to find the corresponding property values. To mitigate the need for all property file consumers to rely on specific property keys, consider wrapping the `PropertyManager` and writing your own custom methods to get the corresponding keys and values, abstracting away the exact key values:\n\n```python\nfrom krausening.properties import PropertyManager\n\nclass TestConfig():\n    """\n    Configurations utility class for being able to read in and reload properties\n    """\n\n    def __init__(self):\n        self.properties = None\n        self.reload()\n \n    def integration_test_enabled(self):\n        """\n        Returns whether the integration tests are enabled or not\n        """\n        integration_test_enable = False\n        integration_enable_str = self.properties[\'integration.test.enabled\']\n        if (integration_enable_str):\n            integration_test_enable = (integration_enable_str == \'True\')\n        return integration_test_enable\n    \n    def reload(self):\n        self.properties = PropertyManager.get_instance().get_properties(\'test.properties\')\n```\n\n**Note: Due to updates the M1 Apple Chip, we strongly recommend using Python >= 3.9 for compatibility reasons.**\n\n## Distribution Channel\n\nKrausening Python is published to PyPI under the [krausening](https://pypi.org/project/krausening/) project and may be installed using any package installer/manager that leverages PyPI.  For example:\n\n  * [Poetry](https://python-poetry.org/) - `poetry add krausening`\n  * [pip](https://pip.pypa.io/) - `pip install krausening`\n\n## Releasing to PyPI\n\nReleasing Krausening Python integrates into the project\'s larger utilization of the `maven-release-plugin`, specifically publishing the package to PyPI during the `deploy` phase.  A [PyPI account](https://pypi.org/account/register/) with access to the [krausening](https://pypi.org/project/krausening/) project is required. PyPI account credentials should be specified in your `settings.xml` under the `<id>pypi</id>` `<server>` entry:\n\n```xml\n<settings>\n  <servers>\n    <server>\n      <id>pypi</id>\n      <username>pypi-username</username>\n      <password>pypi-password</password>\n    </server>\n  </servers>\n</settings>\n```\n',
+    'long_description': '# Krausening Python - Externalized Property Management and Access for Python Projects #\n[![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://opensource.org/licenses/mit)\n[![PyPI](https://img.shields.io/pypi/v/krausening)](https://pypi.org/project/krausening/)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/krausening)\n![PyPI - Wheel](https://img.shields.io/pypi/wheel/krausening)\n\nKrausening property management and encryption for Python is packaged using the open-source Python Maven plugin [Habushu](https://bitbucket.org/cpointe/habushu) and made available as a [PyPI package](https://pypi.org/project/krausening/).  \n\n## Distribution Channel\n\nKrausening Python is published to PyPI under the [krausening](https://pypi.org/project/krausening/) project and may be installed using any package installer/manager that leverages PyPI.  For example:\n\n* [Poetry](https://python-poetry.org/) - `poetry add krausening`\n* [pip](https://pip.pypa.io/) - `pip install krausening`\n\n## Managing Properties with Krausening and Python\n\nManaging properties with Krausening\'s Python library utilizes a similar approach to that required by Krausening Java. Krausening Python expects that developers prime their target environment by configuring the following environment variables (which are named and leveraged in the same manner as the Java System Properties expected by Krausening Java):\n\n* `KRAUSENING_BASE`\n* `KRAUSENING_EXTENSIONS`\n* `KRAUSENING_OVERRIDE_EXTENSIONS`\n* `KRAUSENING_PASSWORD`\n\nIn order to use the Krausening Python, developers may directly use `PropertyManager` or extend `PropertyManager` to provide a custom interface.  For example, developers may directly use the `PropertyManager` as such:\n\n```python\nfrom krausening.properties import PropertyManager\n\npropertyManager = PropertyManager.get_instance()\nproperties = None\nproperties = propertyManager.get_properties(\'my-property-file.properties\')\nassert properties[\'foo\'] == \'bar2\'\n```\n\nThis has the disadvantage that you must know the property keys in order to find the corresponding property values. To mitigate the need for all property file consumers to rely on specific property keys, consider wrapping the `PropertyManager` and writing your own custom methods to get the corresponding keys and values, abstracting away the exact key values:\n\n```python\nfrom krausening.properties import PropertyManager\n\nclass TestConfig():\n    """\n    Configurations utility class for being able to read in and reload properties\n    """\n\n    def __init__(self):\n        self.properties = None\n        self.reload()\n \n    def integration_test_enabled(self):\n        """\n        Returns whether the integration tests are enabled or not\n        """\n        integration_test_enable = False\n        integration_enable_str = self.properties[\'integration.test.enabled\']\n        if (integration_enable_str):\n            integration_test_enable = (integration_enable_str == \'True\')\n        return integration_test_enable\n    \n    def reload(self):\n        self.properties = PropertyManager.get_instance().get_properties(\'test.properties\')\n```\n## Releasing to PyPI\n\nReleasing Krausening Python integrates into the project\'s larger utilization of the `maven-release-plugin`, specifically publishing the package to PyPI during the `deploy` phase.  A [PyPI account](https://pypi.org/account/register/) with access to the [krausening](https://pypi.org/project/krausening/) project is required. PyPI account credentials should be specified in your `settings.xml` under the `<id>pypi</id>` `<server>` entry:\n\n```xml\n<settings>\n  <servers>\n    <server>\n      <id>pypi</id>\n      <username>pypi-username</username>\n      <password>pypi-password</password>\n    </server>\n  </servers>\n</settings>\n```\n',
     'author': 'Eric Konieczny',
-    'author_email': 'ekonieczny@cpointe-inc.com',
+    'author_email': 'ekoniec1@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'https://bitbucket.org/cpointe/krausening',
+    'url': 'https://github.com/TechnologyBrewery/krausening',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.9,<4.0',
 }
```

### Comparing `krausening-15/PKG-INFO` & `krausening-16/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 Metadata-Version: 2.1
 Name: krausening
-Version: 15
+Version: 16
 Summary: Python implementation of Krausening
-Home-page: https://bitbucket.org/cpointe/krausening
+Home-page: https://github.com/TechnologyBrewery/krausening
 License: MIT
 Keywords: properties,configuration-management
 Author: Eric Konieczny
-Author-email: ekonieczny@cpointe-inc.com
+Author-email: ekoniec1@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cryptography (>=39.0.1,<40.0.0)
 Requires-Dist: javaproperties (>=0.8.1,<0.9.0)
 Requires-Dist: watchdog (>=2.1.9,<3.0.0)
-Project-URL: Repository, https://bitbucket.org/cpointe/krausening
+Project-URL: Repository, https://github.com/TechnologyBrewery/krausening
 Description-Content-Type: text/markdown
 
 # Krausening Python - Externalized Property Management and Access for Python Projects #
+[![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://opensource.org/licenses/mit)
 [![PyPI](https://img.shields.io/pypi/v/krausening)](https://pypi.org/project/krausening/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/krausening)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/krausening)
-[![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://opensource.org/licenses/mit)
 
+Krausening property management and encryption for Python is packaged using the open-source Python Maven plugin [Habushu](https://bitbucket.org/cpointe/habushu) and made available as a [PyPI package](https://pypi.org/project/krausening/).  
 
- Krausening property management and encryption for Python is packaged using the open-source Python Maven plugin [Habushu](https://bitbucket.org/cpointe/habushu) and made available as a [PyPI package](https://pypi.org/project/krausening/).  
+## Distribution Channel
+
+Krausening Python is published to PyPI under the [krausening](https://pypi.org/project/krausening/) project and may be installed using any package installer/manager that leverages PyPI.  For example:
+
+* [Poetry](https://python-poetry.org/) - `poetry add krausening`
+* [pip](https://pip.pypa.io/) - `pip install krausening`
 
 ## Managing Properties with Krausening and Python
 
 Managing properties with Krausening's Python library utilizes a similar approach to that required by Krausening Java. Krausening Python expects that developers prime their target environment by configuring the following environment variables (which are named and leveraged in the same manner as the Java System Properties expected by Krausening Java):
 
 * `KRAUSENING_BASE`
 * `KRAUSENING_EXTENSIONS`
@@ -71,24 +77,14 @@
         if (integration_enable_str):
             integration_test_enable = (integration_enable_str == 'True')
         return integration_test_enable
     
     def reload(self):
         self.properties = PropertyManager.get_instance().get_properties('test.properties')
 ```
-
-**Note: Due to updates the M1 Apple Chip, we strongly recommend using Python >= 3.9 for compatibility reasons.**
-
-## Distribution Channel
-
-Krausening Python is published to PyPI under the [krausening](https://pypi.org/project/krausening/) project and may be installed using any package installer/manager that leverages PyPI.  For example:
-
-  * [Poetry](https://python-poetry.org/) - `poetry add krausening`
-  * [pip](https://pip.pypa.io/) - `pip install krausening`
-
 ## Releasing to PyPI
 
 Releasing Krausening Python integrates into the project's larger utilization of the `maven-release-plugin`, specifically publishing the package to PyPI during the `deploy` phase.  A [PyPI account](https://pypi.org/account/register/) with access to the [krausening](https://pypi.org/project/krausening/) project is required. PyPI account credentials should be specified in your `settings.xml` under the `<id>pypi</id>` `<server>` entry:
 
 ```xml
 <settings>
   <servers>
```

