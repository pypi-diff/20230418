# Comparing `tmp/eotdl-cli-0.0.1.tar.gz` & `tmp/eotdl_cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eotdl-cli-0.0.1.tar", max compression
+gzip compressed data, was "eotdl_cli-0.0.2.tar", max compression
```

## Comparing `eotdl-cli-0.0.1.tar` & `eotdl_cli-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,26 @@
--rw-r--r--   0        0        0       41 2023-03-08 12:35:13.904699 eotdl-cli-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-03-08 12:34:08.972622 eotdl-cli-0.0.1/eotdl_cli/__init__.py
--rw-r--r--   0        0        0      168 2023-03-08 12:39:08.629058 eotdl-cli-0.0.1/eotdl_cli/main.py
--rw-r--r--   0        0        0      475 2023-03-08 12:40:50.777244 eotdl-cli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 eotdl-cli-0.0.1/setup.py
--rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 eotdl-cli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       41 2023-03-08 12:48:38.254243 eotdl_cli-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-03-08 12:48:38.254243 eotdl_cli-0.0.2/eotdl_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-0.0.2/eotdl_cli/commands/__init__.py
+-rw-r--r--   0        0        0      920 2023-03-14 15:03:37.605233 eotdl_cli-0.0.2/eotdl_cli/commands/auth.py
+-rw-r--r--   0        0        0     1155 2023-04-11 08:30:40.653793 eotdl_cli-0.0.2/eotdl_cli/commands/datasets.py
+-rw-r--r--   0        0        0      302 2023-04-11 08:30:40.653793 eotdl_cli-0.0.2/eotdl_cli/main.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-0.0.2/eotdl_cli/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-0.0.2/eotdl_cli/src/errors/__init__.py
+-rw-r--r--   0        0        0      306 2023-03-14 08:10:21.438175 eotdl_cli-0.0.2/eotdl_cli/src/errors/auth.py
+-rw-r--r--   0        0        0     2076 2023-04-11 08:30:40.653793 eotdl_cli-0.0.2/eotdl_cli/src/repos/APIRepo.py
+-rw-r--r--   0        0        0      955 2023-04-11 08:30:40.653793 eotdl_cli-0.0.2/eotdl_cli/src/repos/AuthRepo.py
+-rw-r--r--   0        0        0       59 2023-03-14 08:10:21.442175 eotdl_cli-0.0.2/eotdl_cli/src/repos/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.442175 eotdl_cli-0.0.2/eotdl_cli/src/usecases/__init__.py
+-rw-r--r--   0        0        0     1587 2023-04-11 08:30:40.653793 eotdl_cli-0.0.2/eotdl_cli/src/usecases/auth/Auth.py
+-rw-r--r--   0        0        0      332 2023-03-14 08:10:21.442175 eotdl_cli-0.0.2/eotdl_cli/src/usecases/auth/IsLogged.py
+-rw-r--r--   0        0        0      420 2023-03-14 08:10:21.442175 eotdl_cli-0.0.2/eotdl_cli/src/usecases/auth/Logout.py
+-rw-r--r--   0        0        0       54 2023-03-14 08:10:21.442175 eotdl_cli-0.0.2/eotdl_cli/src/usecases/auth/__init__.py
+-rw-r--r--   0        0        0      725 2023-03-14 15:04:32.741573 eotdl_cli-0.0.2/eotdl_cli/src/usecases/auth/main.py
+-rw-r--r--   0        0        0      458 2023-04-11 08:30:40.653793 eotdl_cli-0.0.2/eotdl_cli/src/usecases/datasets/DownloadDataset.py
+-rw-r--r--   0        0        0      603 2023-04-11 08:30:40.657793 eotdl_cli-0.0.2/eotdl_cli/src/usecases/datasets/IngestDataset.py
+-rw-r--r--   0        0        0      489 2023-04-11 08:30:40.657793 eotdl_cli-0.0.2/eotdl_cli/src/usecases/datasets/RetrieveDataset.py
+-rw-r--r--   0        0        0      427 2023-04-11 08:30:40.657793 eotdl_cli-0.0.2/eotdl_cli/src/usecases/datasets/RetrieveDatasets.py
+-rw-r--r--   0        0        0       69 2023-04-11 08:30:40.657793 eotdl_cli-0.0.2/eotdl_cli/src/usecases/datasets/__init__.py
+-rw-r--r--   0        0        0     1072 2023-04-11 08:30:40.657793 eotdl_cli-0.0.2/eotdl_cli/src/usecases/datasets/main.py
+-rw-r--r--   0        0        0      604 2023-04-18 12:54:29.025717 eotdl_cli-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      747 1970-01-01 00:00:00.000000 eotdl_cli-0.0.2/PKG-INFO
```

