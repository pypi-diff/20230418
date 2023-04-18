# Comparing `tmp/eotdl_cli-0.0.3.tar.gz` & `tmp/eotdl_cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eotdl_cli-0.0.3.tar", max compression
+gzip compressed data, was "eotdl_cli-0.0.4.tar", max compression
```

## Comparing `eotdl_cli-0.0.3.tar` & `eotdl_cli-0.0.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0       41 2023-03-08 12:48:38.254243 eotdl_cli-0.0.3/README.md
--rw-r--r--   0        0        0       37 2023-03-08 13:10:34.433708 eotdl_cli-0.0.3/eotdl_cli/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-03-08 13:10:34.433708 eotdl_cli-0.0.3/eotdl_cli/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2023-03-08 13:10:34.433708 eotdl_cli-0.0.3/eotdl_cli/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2023-03-08 13:10:34.433708 eotdl_cli-0.0.3/eotdl_cli/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-03-09 16:40:11.561505 eotdl_cli-0.0.3/eotdl_cli/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2023-03-08 12:48:38.254243 eotdl_cli-0.0.3/eotdl_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-0.0.3/eotdl_cli/commands/__init__.py
--rw-r--r--   0        0        0      150 2023-03-14 14:46:50.348018 eotdl_cli-0.0.3/eotdl_cli/commands/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1167 2023-03-14 15:03:45.145281 eotdl_cli-0.0.3/eotdl_cli/commands/__pycache__/auth.cpython-38.pyc
--rw-r--r--   0        0        0     1476 2023-04-18 12:58:34.462517 eotdl_cli-0.0.3/eotdl_cli/commands/__pycache__/datasets.cpython-38.pyc
--rw-r--r--   0        0        0      920 2023-03-14 15:03:37.605233 eotdl_cli-0.0.3/eotdl_cli/commands/auth.py
--rw-r--r--   0        0        0     1155 2023-04-11 08:30:40.653793 eotdl_cli-0.0.3/eotdl_cli/commands/datasets.py
--rw-r--r--   0        0        0      312 2023-04-18 13:01:29.135065 eotdl_cli-0.0.3/eotdl_cli/main.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-0.0.3/eotdl_cli/src/__init__.py
--rw-r--r--   0        0        0      145 2023-03-14 14:46:50.348018 eotdl_cli-0.0.3/eotdl_cli/src/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2457 2023-03-09 15:57:18.356803 eotdl_cli-0.0.3/eotdl_cli/src/__pycache__/auth.cpython-38.pyc
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-0.0.3/eotdl_cli/src/errors/__init__.py
--rw-r--r--   0        0        0      152 2023-03-14 14:46:50.416018 eotdl_cli-0.0.3/eotdl_cli/src/errors/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      831 2023-03-14 14:46:50.416018 eotdl_cli-0.0.3/eotdl_cli/src/errors/__pycache__/auth.cpython-38.pyc
--rw-r--r--   0        0        0      306 2023-03-14 08:10:21.438175 eotdl_cli-0.0.3/eotdl_cli/src/errors/auth.py
--rw-r--r--   0        0        0     2076 2023-04-11 08:30:40.653793 eotdl_cli-0.0.3/eotdl_cli/src/repos/APIRepo.py
--rw-r--r--   0        0        0      955 2023-04-11 08:30:40.653793 eotdl_cli-0.0.3/eotdl_cli/src/repos/AuthRepo.py
--rw-r--r--   0        0        0       59 2023-03-14 08:10:21.442175 eotdl_cli-0.0.3/eotdl_cli/src/repos/__init__.py
--rw-r--r--   0        0        0     2587 2023-04-18 12:58:34.402517 eotdl_cli-0.0.3/eotdl_cli/src/repos/__pycache__/APIRepo.cpython-38.pyc
--rw-r--r--   0        0        0     1505 2023-04-18 12:58:34.382517 eotdl_cli-0.0.3/eotdl_cli/src/repos/__pycache__/AuthRepo.cpython-38.pyc
--rw-r--r--   0        0        0      212 2023-03-14 14:46:50.348018 eotdl_cli-0.0.3/eotdl_cli/src/repos/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.442175 eotdl_cli-0.0.3/eotdl_cli/src/usecases/__init__.py
--rw-r--r--   0        0        0      154 2023-03-14 14:46:50.348018 eotdl_cli-0.0.3/eotdl_cli/src/usecases/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1851 2023-03-09 16:08:40.611573 eotdl_cli-0.0.3/eotdl_cli/src/usecases/__pycache__/auth.cpython-38.pyc
--rw-r--r--   0        0        0     1587 2023-04-11 08:30:40.653793 eotdl_cli-0.0.3/eotdl_cli/src/usecases/auth/Auth.py
--rw-r--r--   0        0        0      332 2023-03-14 08:10:21.442175 eotdl_cli-0.0.3/eotdl_cli/src/usecases/auth/IsLogged.py
--rw-r--r--   0        0        0      420 2023-03-14 08:10:21.442175 eotdl_cli-0.0.3/eotdl_cli/src/usecases/auth/Logout.py
--rw-r--r--   0        0        0       54 2023-03-14 08:10:21.442175 eotdl_cli-0.0.3/eotdl_cli/src/usecases/auth/__init__.py
--rw-r--r--   0        0        0     1792 2023-04-18 12:58:34.462517 eotdl_cli-0.0.3/eotdl_cli/src/usecases/auth/__pycache__/Auth.cpython-38.pyc
--rw-r--r--   0        0        0     1036 2023-03-14 14:46:50.396018 eotdl_cli-0.0.3/eotdl_cli/src/usecases/auth/__pycache__/IsLogged.cpython-38.pyc
--rw-r--r--   0        0        0     1061 2023-03-14 14:46:50.416018 eotdl_cli-0.0.3/eotdl_cli/src/usecases/auth/__pycache__/Logout.cpython-38.pyc
--rw-r--r--   0        0        0      242 2023-03-14 14:46:50.348018 eotdl_cli-0.0.3/eotdl_cli/src/usecases/auth/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      953 2023-03-14 15:04:39.669615 eotdl_cli-0.0.3/eotdl_cli/src/usecases/auth/__pycache__/main.cpython-38.pyc
--rw-r--r--   0        0        0      725 2023-03-14 15:04:32.741573 eotdl_cli-0.0.3/eotdl_cli/src/usecases/auth/main.py
--rw-r--r--   0        0        0      458 2023-04-11 08:30:40.653793 eotdl_cli-0.0.3/eotdl_cli/src/usecases/datasets/DownloadDataset.py
--rw-r--r--   0        0        0      603 2023-04-11 08:30:40.657793 eotdl_cli-0.0.3/eotdl_cli/src/usecases/datasets/IngestDataset.py
--rw-r--r--   0        0        0      489 2023-04-11 08:30:40.657793 eotdl_cli-0.0.3/eotdl_cli/src/usecases/datasets/RetrieveDataset.py
--rw-r--r--   0        0        0      427 2023-04-11 08:30:40.657793 eotdl_cli-0.0.3/eotdl_cli/src/usecases/datasets/RetrieveDatasets.py
--rw-r--r--   0        0        0       69 2023-04-11 08:30:40.657793 eotdl_cli-0.0.3/eotdl_cli/src/usecases/datasets/__init__.py
--rw-r--r--   0        0        0     1199 2023-04-18 12:58:34.466517 eotdl_cli-0.0.3/eotdl_cli/src/usecases/datasets/__pycache__/DownloadDataset.cpython-38.pyc
--rw-r--r--   0        0        0     1307 2023-04-18 12:58:34.466517 eotdl_cli-0.0.3/eotdl_cli/src/usecases/datasets/__pycache__/IngestDataset.cpython-38.pyc
--rw-r--r--   0        0        0     1211 2023-04-18 12:58:34.466517 eotdl_cli-0.0.3/eotdl_cli/src/usecases/datasets/__pycache__/RetrieveDataset.cpython-38.pyc
--rw-r--r--   0        0        0     1314 2023-04-18 12:58:34.462517 eotdl_cli-0.0.3/eotdl_cli/src/usecases/datasets/__pycache__/RetrieveDatasets.cpython-38.pyc
--rw-r--r--   0        0        0      261 2023-04-18 12:58:34.462517 eotdl_cli-0.0.3/eotdl_cli/src/usecases/datasets/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1287 2023-04-18 12:58:34.462517 eotdl_cli-0.0.3/eotdl_cli/src/usecases/datasets/__pycache__/main.cpython-38.pyc
--rw-r--r--   0        0        0     1072 2023-04-11 08:30:40.657793 eotdl_cli-0.0.3/eotdl_cli/src/usecases/datasets/main.py
--rw-r--r--   0        0        0      604 2023-04-18 13:01:37.299090 eotdl_cli-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      747 1970-01-01 00:00:00.000000 eotdl_cli-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       41 2023-03-08 12:48:38.254243 eotdl_cli-0.0.4/README.md
+-rw-r--r--   0        0        0       37 2023-03-08 13:10:34.433708 eotdl_cli-0.0.4/eotdl_cli/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-03-08 13:10:34.433708 eotdl_cli-0.0.4/eotdl_cli/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2023-03-08 13:10:34.433708 eotdl_cli-0.0.4/eotdl_cli/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2023-03-08 13:10:34.433708 eotdl_cli-0.0.4/eotdl_cli/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-03-09 16:40:11.561505 eotdl_cli-0.0.4/eotdl_cli/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2023-03-08 12:48:38.254243 eotdl_cli-0.0.4/eotdl_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-0.0.4/eotdl_cli/commands/__init__.py
+-rw-r--r--   0        0        0      150 2023-03-14 14:46:50.348018 eotdl_cli-0.0.4/eotdl_cli/commands/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1167 2023-03-14 15:03:45.145281 eotdl_cli-0.0.4/eotdl_cli/commands/__pycache__/auth.cpython-38.pyc
+-rw-r--r--   0        0        0     1476 2023-04-18 12:58:34.462517 eotdl_cli-0.0.4/eotdl_cli/commands/__pycache__/datasets.cpython-38.pyc
+-rw-r--r--   0        0        0      940 2023-04-18 13:03:59.183525 eotdl_cli-0.0.4/eotdl_cli/commands/auth.py
+-rw-r--r--   0        0        0     1175 2023-04-18 13:04:05.455544 eotdl_cli-0.0.4/eotdl_cli/commands/datasets.py
+-rw-r--r--   0        0        0      312 2023-04-18 13:03:47.587490 eotdl_cli-0.0.4/eotdl_cli/main.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-0.0.4/eotdl_cli/src/__init__.py
+-rw-r--r--   0        0        0      145 2023-03-14 14:46:50.348018 eotdl_cli-0.0.4/eotdl_cli/src/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2457 2023-03-09 15:57:18.356803 eotdl_cli-0.0.4/eotdl_cli/src/__pycache__/auth.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-0.0.4/eotdl_cli/src/errors/__init__.py
+-rw-r--r--   0        0        0      152 2023-03-14 14:46:50.416018 eotdl_cli-0.0.4/eotdl_cli/src/errors/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      831 2023-03-14 14:46:50.416018 eotdl_cli-0.0.4/eotdl_cli/src/errors/__pycache__/auth.cpython-38.pyc
+-rw-r--r--   0        0        0      306 2023-03-14 08:10:21.438175 eotdl_cli-0.0.4/eotdl_cli/src/errors/auth.py
+-rw-r--r--   0        0        0     2076 2023-04-11 08:30:40.653793 eotdl_cli-0.0.4/eotdl_cli/src/repos/APIRepo.py
+-rw-r--r--   0        0        0      955 2023-04-11 08:30:40.653793 eotdl_cli-0.0.4/eotdl_cli/src/repos/AuthRepo.py
+-rw-r--r--   0        0        0       59 2023-03-14 08:10:21.442175 eotdl_cli-0.0.4/eotdl_cli/src/repos/__init__.py
+-rw-r--r--   0        0        0     2587 2023-04-18 12:58:34.402517 eotdl_cli-0.0.4/eotdl_cli/src/repos/__pycache__/APIRepo.cpython-38.pyc
+-rw-r--r--   0        0        0     1505 2023-04-18 12:58:34.382517 eotdl_cli-0.0.4/eotdl_cli/src/repos/__pycache__/AuthRepo.cpython-38.pyc
+-rw-r--r--   0        0        0      212 2023-03-14 14:46:50.348018 eotdl_cli-0.0.4/eotdl_cli/src/repos/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.442175 eotdl_cli-0.0.4/eotdl_cli/src/usecases/__init__.py
+-rw-r--r--   0        0        0      154 2023-03-14 14:46:50.348018 eotdl_cli-0.0.4/eotdl_cli/src/usecases/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1851 2023-03-09 16:08:40.611573 eotdl_cli-0.0.4/eotdl_cli/src/usecases/__pycache__/auth.cpython-38.pyc
+-rw-r--r--   0        0        0     1587 2023-04-11 08:30:40.653793 eotdl_cli-0.0.4/eotdl_cli/src/usecases/auth/Auth.py
+-rw-r--r--   0        0        0      332 2023-03-14 08:10:21.442175 eotdl_cli-0.0.4/eotdl_cli/src/usecases/auth/IsLogged.py
+-rw-r--r--   0        0        0      420 2023-03-14 08:10:21.442175 eotdl_cli-0.0.4/eotdl_cli/src/usecases/auth/Logout.py
+-rw-r--r--   0        0        0       54 2023-03-14 08:10:21.442175 eotdl_cli-0.0.4/eotdl_cli/src/usecases/auth/__init__.py
+-rw-r--r--   0        0        0     1792 2023-04-18 12:58:34.462517 eotdl_cli-0.0.4/eotdl_cli/src/usecases/auth/__pycache__/Auth.cpython-38.pyc
+-rw-r--r--   0        0        0     1036 2023-03-14 14:46:50.396018 eotdl_cli-0.0.4/eotdl_cli/src/usecases/auth/__pycache__/IsLogged.cpython-38.pyc
+-rw-r--r--   0        0        0     1061 2023-03-14 14:46:50.416018 eotdl_cli-0.0.4/eotdl_cli/src/usecases/auth/__pycache__/Logout.cpython-38.pyc
+-rw-r--r--   0        0        0      242 2023-03-14 14:46:50.348018 eotdl_cli-0.0.4/eotdl_cli/src/usecases/auth/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      953 2023-03-14 15:04:39.669615 eotdl_cli-0.0.4/eotdl_cli/src/usecases/auth/__pycache__/main.cpython-38.pyc
+-rw-r--r--   0        0        0      725 2023-03-14 15:04:32.741573 eotdl_cli-0.0.4/eotdl_cli/src/usecases/auth/main.py
+-rw-r--r--   0        0        0      458 2023-04-11 08:30:40.653793 eotdl_cli-0.0.4/eotdl_cli/src/usecases/datasets/DownloadDataset.py
+-rw-r--r--   0        0        0      603 2023-04-11 08:30:40.657793 eotdl_cli-0.0.4/eotdl_cli/src/usecases/datasets/IngestDataset.py
+-rw-r--r--   0        0        0      489 2023-04-11 08:30:40.657793 eotdl_cli-0.0.4/eotdl_cli/src/usecases/datasets/RetrieveDataset.py
+-rw-r--r--   0        0        0      427 2023-04-11 08:30:40.657793 eotdl_cli-0.0.4/eotdl_cli/src/usecases/datasets/RetrieveDatasets.py
+-rw-r--r--   0        0        0       69 2023-04-11 08:30:40.657793 eotdl_cli-0.0.4/eotdl_cli/src/usecases/datasets/__init__.py
+-rw-r--r--   0        0        0     1199 2023-04-18 12:58:34.466517 eotdl_cli-0.0.4/eotdl_cli/src/usecases/datasets/__pycache__/DownloadDataset.cpython-38.pyc
+-rw-r--r--   0        0        0     1307 2023-04-18 12:58:34.466517 eotdl_cli-0.0.4/eotdl_cli/src/usecases/datasets/__pycache__/IngestDataset.cpython-38.pyc
+-rw-r--r--   0        0        0     1211 2023-04-18 12:58:34.466517 eotdl_cli-0.0.4/eotdl_cli/src/usecases/datasets/__pycache__/RetrieveDataset.cpython-38.pyc
+-rw-r--r--   0        0        0     1314 2023-04-18 12:58:34.462517 eotdl_cli-0.0.4/eotdl_cli/src/usecases/datasets/__pycache__/RetrieveDatasets.cpython-38.pyc
+-rw-r--r--   0        0        0      261 2023-04-18 12:58:34.462517 eotdl_cli-0.0.4/eotdl_cli/src/usecases/datasets/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1287 2023-04-18 12:58:34.462517 eotdl_cli-0.0.4/eotdl_cli/src/usecases/datasets/__pycache__/main.cpython-38.pyc
+-rw-r--r--   0        0        0     1072 2023-04-11 08:30:40.657793 eotdl_cli-0.0.4/eotdl_cli/src/usecases/datasets/main.py
+-rw-r--r--   0        0        0      604 2023-04-18 13:05:02.075716 eotdl_cli-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      747 1970-01-01 00:00:00.000000 eotdl_cli-0.0.4/PKG-INFO
```

### Comparing `eotdl_cli-0.0.3/eotdl_cli/commands/__pycache__/auth.cpython-38.pyc` & `eotdl_cli-0.0.4/eotdl_cli/commands/__pycache__/auth.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/eotdl_cli/commands/__pycache__/datasets.cpython-38.pyc` & `eotdl_cli-0.0.4/eotdl_cli/commands/__pycache__/datasets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/eotdl_cli/commands/auth.py` & `eotdl_cli-0.0.4/eotdl_cli/commands/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typer
-from src.usecases.auth import is_logged, auth, generate_logout_url
-from src.errors.auth import LoginError
+from eotdl_cli.src.usecases.auth import is_logged, auth, generate_logout_url
+from eotdl_cli.src.errors.auth import LoginError
 
 app = typer.Typer()
 
 @app.command()
 def login():
     """
     Login to your account
```

### Comparing `eotdl_cli-0.0.3/eotdl_cli/commands/datasets.py` & `eotdl_cli-0.0.4/eotdl_cli/commands/datasets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typer
-from src.usecases.datasets import retrieve_datasets, download_dataset, ingest_dataset
-from src.usecases.auth import auth
+from eotdl_cli.src.usecases.datasets import retrieve_datasets, download_dataset, ingest_dataset
+from eotdl_cli.src.usecases.auth import auth
 
 app = typer.Typer()
 
 @app.command()
 def list():
     """
     List all datasets
```

### Comparing `eotdl_cli-0.0.3/eotdl_cli/src/__pycache__/auth.cpython-38.pyc` & `eotdl_cli-0.0.4/eotdl_cli/src/__pycache__/auth.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/eotdl_cli/src/errors/__pycache__/auth.cpython-38.pyc` & `eotdl_cli-0.0.4/eotdl_cli/src/errors/__pycache__/auth.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/eotdl_cli/src/repos/APIRepo.py` & `eotdl_cli-0.0.4/eotdl_cli/src/repos/APIRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/eotdl_cli/src/repos/AuthRepo.py` & `eotdl_cli-0.0.4/eotdl_cli/src/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/eotdl_cli/src/repos/__pycache__/APIRepo.cpython-38.pyc` & `eotdl_cli-0.0.4/eotdl_cli/src/repos/__pycache__/APIRepo.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/eotdl_cli/src/repos/__pycache__/AuthRepo.cpython-38.pyc` & `eotdl_cli-0.0.4/eotdl_cli/src/repos/__pycache__/AuthRepo.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/eotdl_cli/src/usecases/__pycache__/auth.cpython-38.pyc` & `eotdl_cli-0.0.4/eotdl_cli/src/usecases/__pycache__/auth.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/eotdl_cli/src/usecases/auth/Auth.py` & `eotdl_cli-0.0.4/eotdl_cli/src/usecases/auth/Auth.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/eotdl_cli/src/usecases/auth/__pycache__/Auth.cpython-38.pyc` & `eotdl_cli-0.0.4/eotdl_cli/src/usecases/auth/__pycache__/Auth.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/eotdl_cli/src/usecases/auth/__pycache__/IsLogged.cpython-38.pyc` & `eotdl_cli-0.0.4/eotdl_cli/src/usecases/auth/__pycache__/IsLogged.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/eotdl_cli/src/usecases/auth/__pycache__/Logout.cpython-38.pyc` & `eotdl_cli-0.0.4/eotdl_cli/src/usecases/auth/__pycache__/Logout.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/eotdl_cli/src/usecases/auth/__pycache__/main.cpython-38.pyc` & `eotdl_cli-0.0.4/eotdl_cli/src/usecases/auth/__pycache__/main.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/eotdl_cli/src/usecases/auth/main.py` & `eotdl_cli-0.0.4/eotdl_cli/src/usecases/auth/main.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/eotdl_cli/src/usecases/datasets/IngestDataset.py` & `eotdl_cli-0.0.4/eotdl_cli/src/usecases/datasets/IngestDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/eotdl_cli/src/usecases/datasets/__pycache__/DownloadDataset.cpython-38.pyc` & `eotdl_cli-0.0.4/eotdl_cli/src/usecases/datasets/__pycache__/DownloadDataset.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/eotdl_cli/src/usecases/datasets/__pycache__/IngestDataset.cpython-38.pyc` & `eotdl_cli-0.0.4/eotdl_cli/src/usecases/datasets/__pycache__/IngestDataset.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/eotdl_cli/src/usecases/datasets/__pycache__/RetrieveDataset.cpython-38.pyc` & `eotdl_cli-0.0.4/eotdl_cli/src/usecases/datasets/__pycache__/RetrieveDataset.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/eotdl_cli/src/usecases/datasets/__pycache__/RetrieveDatasets.cpython-38.pyc` & `eotdl_cli-0.0.4/eotdl_cli/src/usecases/datasets/__pycache__/RetrieveDatasets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/eotdl_cli/src/usecases/datasets/__pycache__/main.cpython-38.pyc` & `eotdl_cli-0.0.4/eotdl_cli/src/usecases/datasets/__pycache__/main.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/eotdl_cli/src/usecases/datasets/main.py` & `eotdl_cli-0.0.4/eotdl_cli/src/usecases/datasets/main.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.3/pyproject.toml` & `eotdl_cli-0.0.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eotdl-cli"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 authors = ["EarthPulse <it@earthpulse.es>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "eotdl_cli"}]
 
 [tool.poetry.scripts]
```

### Comparing `eotdl_cli-0.0.3/PKG-INFO` & `eotdl_cli-0.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eotdl-cli
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 License: MIT
 Author: EarthPulse
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

