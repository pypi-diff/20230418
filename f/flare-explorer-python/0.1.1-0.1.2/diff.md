# Comparing `tmp/flare_explorer_python-0.1.1.tar.gz` & `tmp/flare_explorer_python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flare_explorer_python-0.1.1.tar", max compression
+gzip compressed data, was "flare_explorer_python-0.1.2.tar", max compression
```

## Comparing `flare_explorer_python-0.1.1.tar` & `flare_explorer_python-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-01-22 16:09:45.273284 flare_explorer_python-0.1.1/LICENSE
--rw-r--r--   0        0        0     3020 2023-01-28 18:54:49.193517 flare_explorer_python-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-01-28 15:16:13.115891 flare_explorer_python-0.1.1/flare_explorer/__init__.py
--rw-r--r--   0        0        0     2342 2023-01-28 15:28:53.079821 flare_explorer_python-0.1.1/flare_explorer/address.py
--rw-r--r--   0        0        0     1110 2023-01-28 09:56:49.468982 flare_explorer_python-0.1.1/flare_explorer/block.py
--rw-r--r--   0        0        0      527 2023-01-28 12:11:20.604044 flare_explorer_python-0.1.1/flare_explorer/exceptions.py
--rw-r--r--   0        0        0     1392 2023-01-27 21:58:23.671943 flare_explorer_python-0.1.1/flare_explorer/gql_client.py
--rw-r--r--   0        0        0     1974 2023-01-27 21:57:15.211992 flare_explorer_python-0.1.1/flare_explorer/token_transfers.py
--rw-r--r--   0        0        0     5768 2023-01-28 17:48:10.167514 flare_explorer_python-0.1.1/flare_explorer/transaction.py
--rw-r--r--   0        0        0     1189 2023-01-28 18:55:01.660179 flare_explorer_python-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3870 1970-01-01 00:00:00.000000 flare_explorer_python-0.1.1/setup.py
--rw-r--r--   0        0        0     4013 1970-01-01 00:00:00.000000 flare_explorer_python-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-01-22 16:09:45.273284 flare_explorer_python-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3020 2023-04-18 04:13:14.853407 flare_explorer_python-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-01-28 15:16:13.115891 flare_explorer_python-0.1.2/flare_explorer/__init__.py
+-rw-r--r--   0        0        0     2342 2023-01-31 17:29:51.953472 flare_explorer_python-0.1.2/flare_explorer/address.py
+-rw-r--r--   0        0        0     1110 2023-01-28 09:56:49.468982 flare_explorer_python-0.1.2/flare_explorer/block.py
+-rw-r--r--   0        0        0      386 2023-04-18 04:13:14.853927 flare_explorer_python-0.1.2/flare_explorer/exceptions.py
+-rw-r--r--   0        0        0     1513 2023-04-18 04:13:14.854282 flare_explorer_python-0.1.2/flare_explorer/gql_client.py
+-rw-r--r--   0        0        0     1974 2023-02-03 18:56:57.596469 flare_explorer_python-0.1.2/flare_explorer/token_transfers.py
+-rw-r--r--   0        0        0     5768 2023-01-28 17:48:10.167514 flare_explorer_python-0.1.2/flare_explorer/transaction.py
+-rw-r--r--   0        0        0     1397 2023-04-18 04:58:48.241752 flare_explorer_python-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4101 1970-01-01 00:00:00.000000 flare_explorer_python-0.1.2/PKG-INFO
```

### Comparing `flare_explorer_python-0.1.1/LICENSE` & `flare_explorer_python-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flare_explorer_python-0.1.1/README.md` & `flare_explorer_python-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -82,13 +82,13 @@
 - websocket support
 - fast mode (no pydantic serialization)
 
 ## Testing / Contributing
 Any contributions or issue raising is welcomed. If you wish to contribute then:
 1. fork/clone this repo
 2. make changes on a branch taken from main
-3. sumbit a pull request against main
+3. submit a pull request against main
 
 Pull requests will be blocked from merging automatically if:
 - less than 100% coverage
 - there are failing tests
 - linting rules have been violated.
```

#### html2text {}

```diff
@@ -27,10 +27,10 @@
 import get_block block = get_block(4463469) ``` ### Token transfers ``` python
 from flare_explorer.token_transfers import get_token_transfers token_transfers,
 page_info = get_token_transfers( "token_contract_address_hash",
 previous_cursor="previous_page_last_cursor" ) ``` ## Upcoming features -
 asyncio support - websocket support - fast mode (no pydantic serialization) ##
 Testing / Contributing Any contributions or issue raising is welcomed. If you
 wish to contribute then: 1. fork/clone this repo 2. make changes on a branch
-taken from main 3. sumbit a pull request against main Pull requests will be
+taken from main 3. submit a pull request against main Pull requests will be
 blocked from merging automatically if: - less than 100% coverage - there are
 failing tests - linting rules have been violated.
```

### Comparing `flare_explorer_python-0.1.1/flare_explorer/address.py` & `flare_explorer_python-0.1.2/flare_explorer/address.py`

 * *Files identical despite different names*

### Comparing `flare_explorer_python-0.1.1/flare_explorer/block.py` & `flare_explorer_python-0.1.2/flare_explorer/block.py`

 * *Files identical despite different names*

### Comparing `flare_explorer_python-0.1.1/flare_explorer/token_transfers.py` & `flare_explorer_python-0.1.2/flare_explorer/token_transfers.py`

 * *Files identical despite different names*

### Comparing `flare_explorer_python-0.1.1/flare_explorer/transaction.py` & `flare_explorer_python-0.1.2/flare_explorer/transaction.py`

 * *Files identical despite different names*

### Comparing `flare_explorer_python-0.1.1/pyproject.toml` & `flare_explorer_python-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flare-explorer-python"
-version = "0.1.1"
+version = "0.1.2"
 description = "A lightweight library that works as a connector to the Flare explorer api"
 authors = ["James Davis <jamesecd@gmail.com>"]
 keywords = ["flare-explorer", "flare", "network", "api", "crypto", "blockchain"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -20,25 +20,38 @@
 ]
 packages = [{include = "flare_explorer"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.28.2"
 pydantic = "^1.10.4"
+gql = "^3.4.0"
+requests-toolbelt = "^0.10.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 pytest = "^7.2.1"
 aiohttp = "^3.8.3"
 requests-mock = "^1.10.0"
-isort = "^5.11.4"
-codecov = "^2.1.12"
-flake8 = "^6.0.0"
 pytest-cov = "^4.0.0"
+ruff = "^0.0.237"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.isort]
-profile = "black"
+[tool.ruff]
+select = ["E", "F"]
+ignore = ["E501"]
+fixable = []
+unfixable = ["B"]
+exclude = [
+    ".git",
+    "__pypackages__",
+    "_build",
+    "build",
+    "dist",
+]
+per-file-ignores = {}
+line-length = 88
+target-version = "py310"
```

### Comparing `flare_explorer_python-0.1.1/setup.py` & `flare_explorer_python-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,120 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: flare-explorer-python
+Version: 0.1.2
+Summary: A lightweight library that works as a connector to the Flare explorer api
+Home-page: https://github.com/james-ecd/flare-explorer-python
+License: MIT
+Keywords: flare-explorer,flare,network,api,crypto,blockchain
+Author: James Davis
+Author-email: jamesecd@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: gql (>=3.4.0,<4.0.0)
+Requires-Dist: pydantic (>=1.10.4,<2.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: requests-toolbelt (>=0.10.1,<0.11.0)
+Project-URL: Repository, https://github.com/james-ecd/flare-explorer-python
+Description-Content-Type: text/markdown
+
+# Flare explorer python
+<a href="https://pypi.org/project/flare-explorer-python" target="_blank"><img src="https://img.shields.io/pypi/v/flare-explorer-python?color=%2334D058&label=pypi%20package" alt="Package version"></a>
+[![Linting and tests](https://github.com/james-ecd/flare-explorer-python/actions/workflows/tests-and-linting.yml/badge.svg?branch=main)](https://github.com/james-ecd/flare-explorer-python/actions/workflows/tests-and-linting.yml)
+[![codecov](https://codecov.io/gh/james-ecd/flare-explorer-python/branch/main/graph/badge.svg?token=XOBC0UK00V)](https://codecov.io/gh/james-ecd/flare-explorer-python)
+<a href="https://pypi.org/project/flare-explorer-python" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/flare-explorer-python.svg?color=%2334D058" alt="Supported Python versions">
+</a>
+[![Code Style](https://img.shields.io/badge/code_style-black-black)](https://black.readthedocs.io/en/stable/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+A lightweight library that works as a connector to the [Flare explorer api](https://flare-explorer.flare.network/graphiql)
+
+If you came here looking for the flare network, then go [here](https://flare.network/). If you want to query flares blockchain using python then stick around.
+
+## Installation
+flare-explorer-python is available on PYPI. Install with pip or poetry:
+
+```
+pip install flare-explorer-python
+```
+```
+poetry add flare-explorer-python
+```
+
+## Usage
+### Transactions
+``` python
+from flare_explorer.transaction import (
+    get_internal_transactions,
+    get_transaction,
+    get_transactions_from_address,
+)
+
+transaction = get_transaction("transaction_hash")
+
+internal_transactions, page_info = get_internal_transactions(
+    "transaction_hash",
+    previous_cursor="previous_page_last_cursor"
+)
+
+transactions, page_info = get_transactions_from_address(
+    "address_hash",
+    previous_cursor="previous_page_last_cursor"
+)
+```
+
+### Addresses
+``` python
+from flare_explorer.address import get_address, get_addresses
+
+address = get_address(
+    "address_hash",
+)
+
+addresses = get_addresses(
+    [
+        "address_hash_1",
+        "address_hash_2",
+    ]
+)
+```
+
+### Blocks
+``` python
+from flare_explorer.block import get_block
+
+block = get_block(4463469)
+```
+
+### Token transfers
+``` python
+from flare_explorer.token_transfers import get_token_transfers
+
+token_transfers, page_info = get_token_transfers(
+    "token_contract_address_hash",
+    previous_cursor="previous_page_last_cursor"
+)
+```
+
+## Upcoming features
+- asyncio support
+- websocket support
+- fast mode (no pydantic serialization)
+
+## Testing / Contributing
+Any contributions or issue raising is welcomed. If you wish to contribute then:
+1. fork/clone this repo
+2. make changes on a branch taken from main
+3. submit a pull request against main
+
+Pull requests will be blocked from merging automatically if:
+- less than 100% coverage
+- there are failing tests
+- linting rules have been violated.
 
-packages = \
-['flare_explorer']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pydantic>=1.10.4,<2.0.0', 'requests>=2.28.2,<3.0.0']
-
-setup_kwargs = {
-    'name': 'flare-explorer-python',
-    'version': '0.1.1',
-    'description': 'A lightweight library that works as a connector to the Flare explorer api',
-    'long_description': '# Flare explorer python\n<a href="https://pypi.org/project/flare-explorer-python" target="_blank"><img src="https://img.shields.io/pypi/v/flare-explorer-python?color=%2334D058&label=pypi%20package" alt="Package version"></a>\n[![Linting and tests](https://github.com/james-ecd/flare-explorer-python/actions/workflows/tests-and-linting.yml/badge.svg?branch=main)](https://github.com/james-ecd/flare-explorer-python/actions/workflows/tests-and-linting.yml)\n[![codecov](https://codecov.io/gh/james-ecd/flare-explorer-python/branch/main/graph/badge.svg?token=XOBC0UK00V)](https://codecov.io/gh/james-ecd/flare-explorer-python)\n<a href="https://pypi.org/project/flare-explorer-python" target="_blank">\n    <img src="https://img.shields.io/pypi/pyversions/flare-explorer-python.svg?color=%2334D058" alt="Supported Python versions">\n</a>\n[![Code Style](https://img.shields.io/badge/code_style-black-black)](https://black.readthedocs.io/en/stable/)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n\nA lightweight library that works as a connector to the [Flare explorer api](https://flare-explorer.flare.network/graphiql)\n\nIf you came here looking for the flare network, then go [here](https://flare.network/). If you want to query flares blockchain using python then stick around.\n\n## Installation\nflare-explorer-python is available on PYPI. Install with pip or poetry:\n\n```\npip install flare-explorer-python\n```\n```\npoetry add flare-explorer-python\n```\n\n## Usage\n### Transactions\n``` python\nfrom flare_explorer.transaction import (\n    get_internal_transactions,\n    get_transaction,\n    get_transactions_from_address,\n)\n\ntransaction = get_transaction("transaction_hash")\n\ninternal_transactions, page_info = get_internal_transactions(\n    "transaction_hash",\n    previous_cursor="previous_page_last_cursor"\n)\n\ntransactions, page_info = get_transactions_from_address(\n    "address_hash",\n    previous_cursor="previous_page_last_cursor"\n)\n```\n\n### Addresses\n``` python\nfrom flare_explorer.address import get_address, get_addresses\n\naddress = get_address(\n    "address_hash",\n)\n\naddresses = get_addresses(\n    [\n        "address_hash_1",\n        "address_hash_2",\n    ]\n)\n```\n\n### Blocks\n``` python\nfrom flare_explorer.block import get_block\n\nblock = get_block(4463469)\n```\n\n### Token transfers\n``` python\nfrom flare_explorer.token_transfers import get_token_transfers\n\ntoken_transfers, page_info = get_token_transfers(\n    "token_contract_address_hash",\n    previous_cursor="previous_page_last_cursor"\n)\n```\n\n## Upcoming features\n- asyncio support\n- websocket support\n- fast mode (no pydantic serialization)\n\n## Testing / Contributing\nAny contributions or issue raising is welcomed. If you wish to contribute then:\n1. fork/clone this repo\n2. make changes on a branch taken from main\n3. sumbit a pull request against main\n\nPull requests will be blocked from merging automatically if:\n- less than 100% coverage\n- there are failing tests\n- linting rules have been violated.\n',
-    'author': 'James Davis',
-    'author_email': 'jamesecd@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/james-ecd/flare-explorer-python',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,48 +1,50 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['flare_explorer'] package_data = \ {'': ['*']} install_requires = \
-['pydantic>=1.10.4,<2.0.0', 'requests>=2.28.2,<3.0.0'] setup_kwargs = { 'name':
-'flare-explorer-python', 'version': '0.1.1', 'description': 'A lightweight
-library that works as a connector to the Flare explorer api',
-'long_description': '# Flare explorer python\n[Package_version]\n[![Linting and
-tests](https://github.com/james-ecd/flare-explorer-python/actions/workflows/
-tests-and-linting.yml/badge.svg?branch=main)](https://github.com/james-ecd/
-flare-explorer-python/actions/workflows/tests-and-linting.yml)\n[![codecov]
-(https://codecov.io/gh/james-ecd/flare-explorer-python/branch/main/graph/
+Metadata-Version: 2.1 Name: flare-explorer-python Version: 0.1.2 Summary: A
+lightweight library that works as a connector to the Flare explorer api Home-
+page: https://github.com/james-ecd/flare-explorer-python License: MIT Keywords:
+flare-explorer,flare,network,api,crypto,blockchain Author: James Davis Author-
+email: jamesecd@gmail.com Requires-Python: >=3.10,<4.0 Classifier: Development
+Status :: 5 - Production/Stable Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3 Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Requires-Dist: gql (>=3.4.0,<4.0.0) Requires-Dist: pydantic
+(>=1.10.4,<2.0.0) Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist:
+requests-toolbelt (>=0.10.1,<0.11.0) Project-URL: Repository, https://
+github.com/james-ecd/flare-explorer-python Description-Content-Type: text/
+markdown # Flare explorer python [Package_version] [![Linting and tests](https:
+//github.com/james-ecd/flare-explorer-python/actions/workflows/tests-and-
+linting.yml/badge.svg?branch=main)](https://github.com/james-ecd/flare-
+explorer-python/actions/workflows/tests-and-linting.yml) [![codecov](https://
+codecov.io/gh/james-ecd/flare-explorer-python/branch/main/graph/
 badge.svg?token=XOBC0UK00V)](https://codecov.io/gh/james-ecd/flare-explorer-
-python)\n\n_[Supported_Python_versions]\n\n[![Code Style](https://
-img.shields.io/badge/code_style-black-black)](https://black.readthedocs.io/en/
-stable/)\n[![License: MIT](https://img.shields.io/badge/License-MIT-
-yellow.svg)](https://opensource.org/licenses/MIT)\n\nA lightweight library that
-works as a connector to the [Flare explorer api](https://flare-
-explorer.flare.network/graphiql)\n\nIf you came here looking for the flare
-network, then go [here](https://flare.network/). If you want to query flares
-blockchain using python then stick around.\n\n## Installation\nflare-explorer-
-python is available on PYPI. Install with pip or poetry:\n\n```\npip install
-flare-explorer-python\n```\n```\npoetry add flare-explorer-python\n```\n\n##
-Usage\n### Transactions\n``` python\nfrom flare_explorer.transaction import (\n
-get_internal_transactions,\n get_transaction,\n
-get_transactions_from_address,\n)\n\ntransaction = get_transaction
-("transaction_hash")\n\ninternal_transactions, page_info =
-get_internal_transactions(\n "transaction_hash",\n
-previous_cursor="previous_page_last_cursor"\n)\n\ntransactions, page_info =
-get_transactions_from_address(\n "address_hash",\n
-previous_cursor="previous_page_last_cursor"\n)\n```\n\n### Addresses\n```
-python\nfrom flare_explorer.address import get_address,
-get_addresses\n\naddress = get_address(\n "address_hash",\n)\n\naddresses =
-get_addresses(\n [\n "address_hash_1",\n "address_hash_2",\n ]\n)\n```\n\n###
-Blocks\n``` python\nfrom flare_explorer.block import get_block\n\nblock =
-get_block(4463469)\n```\n\n### Token transfers\n``` python\nfrom
-flare_explorer.token_transfers import get_token_transfers\n\ntoken_transfers,
-page_info = get_token_transfers(\n "token_contract_address_hash",\n
-previous_cursor="previous_page_last_cursor"\n)\n```\n\n## Upcoming features\n-
-asyncio support\n- websocket support\n- fast mode (no pydantic
-serialization)\n\n## Testing / Contributing\nAny contributions or issue raising
-is welcomed. If you wish to contribute then:\n1. fork/clone this repo\n2. make
-changes on a branch taken from main\n3. sumbit a pull request against
-main\n\nPull requests will be blocked from merging automatically if:\n- less
-than 100% coverage\n- there are failing tests\n- linting rules have been
-violated.\n', 'author': 'James Davis', 'author_email': 'jamesecd@gmail.com',
-'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://github.com/
-james-ecd/flare-explorer-python', 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'python_requires':
-'>=3.10,<4.0', } setup(**setup_kwargs)
+python) [Supported_Python_versions] [![Code Style](https://img.shields.io/
+badge/code_style-black-black)](https://black.readthedocs.io/en/stable/) [!
+[License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
+opensource.org/licenses/MIT) A lightweight library that works as a connector to
+the [Flare explorer api](https://flare-explorer.flare.network/graphiql) If you
+came here looking for the flare network, then go [here](https://flare.network/
+). If you want to query flares blockchain using python then stick around. ##
+Installation flare-explorer-python is available on PYPI. Install with pip or
+poetry: ``` pip install flare-explorer-python ``` ``` poetry add flare-
+explorer-python ``` ## Usage ### Transactions ``` python from
+flare_explorer.transaction import ( get_internal_transactions, get_transaction,
+get_transactions_from_address, ) transaction = get_transaction
+("transaction_hash") internal_transactions, page_info =
+get_internal_transactions( "transaction_hash",
+previous_cursor="previous_page_last_cursor" ) transactions, page_info =
+get_transactions_from_address( "address_hash",
+previous_cursor="previous_page_last_cursor" ) ``` ### Addresses ``` python from
+flare_explorer.address import get_address, get_addresses address = get_address
+( "address_hash", ) addresses = get_addresses( [ "address_hash_1",
+"address_hash_2", ] ) ``` ### Blocks ``` python from flare_explorer.block
+import get_block block = get_block(4463469) ``` ### Token transfers ``` python
+from flare_explorer.token_transfers import get_token_transfers token_transfers,
+page_info = get_token_transfers( "token_contract_address_hash",
+previous_cursor="previous_page_last_cursor" ) ``` ## Upcoming features -
+asyncio support - websocket support - fast mode (no pydantic serialization) ##
+Testing / Contributing Any contributions or issue raising is welcomed. If you
+wish to contribute then: 1. fork/clone this repo 2. make changes on a branch
+taken from main 3. submit a pull request against main Pull requests will be
+blocked from merging automatically if: - less than 100% coverage - there are
+failing tests - linting rules have been violated.
```

