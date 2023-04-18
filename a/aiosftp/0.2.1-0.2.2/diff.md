# Comparing `tmp/aiosftp-0.2.1.tar.gz` & `tmp/aiosftp-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosftp-0.2.1.tar", last modified: Wed Mar  8 20:54:13 2023, max compression
+gzip compressed data, was "aiosftp-0.2.2.tar", last modified: Tue Apr 18 16:22:12 2023, max compression
```

## Comparing `aiosftp-0.2.1.tar` & `aiosftp-0.2.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-03-08 20:54:13.676931 aiosftp-0.2.1/
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-03-08 20:54:13.668931 aiosftp-0.2.1/.github/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      125 2022-11-09 21:24:33.000000 aiosftp-0.2.1/.github/dependabot.yml
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-03-08 20:54:13.668931 aiosftp-0.2.1/.github/workflows/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2731 2022-11-09 23:53:30.000000 aiosftp-0.2.1/.github/workflows/codeql-analysis.yml
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      833 2023-03-08 18:43:37.000000 aiosftp-0.2.1/.github/workflows/release.yml
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1838 2022-11-29 01:22:18.000000 aiosftp-0.2.1/.gitignore
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      174 2022-11-09 21:00:12.000000 aiosftp-0.2.1/.isort.cfg
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       37 2022-11-09 20:59:27.000000 aiosftp-0.2.1/.mypy.ini
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    20245 2022-11-09 20:59:39.000000 aiosftp-0.2.1/.pylintrc
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      329 2022-11-09 20:56:46.000000 aiosftp-0.2.1/CHANGELOG.md
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3225 2022-11-09 20:59:54.000000 aiosftp-0.2.1/CODE_OF_CONDUCT.md
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    11357 2022-11-09 20:54:25.000000 aiosftp-0.2.1/LICENSE
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      568 2023-03-08 18:18:46.000000 aiosftp-0.2.1/Makefile
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2963 2023-03-08 20:54:13.676931 aiosftp-0.2.1/PKG-INFO
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1629 2022-11-09 23:28:12.000000 aiosftp-0.2.1/README.md
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-03-08 20:54:13.668931 aiosftp-0.2.1/aiosftp/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       93 2022-11-09 21:36:43.000000 aiosftp-0.2.1/aiosftp/__init__.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2505 2022-11-09 22:42:22.000000 aiosftp-0.2.1/aiosftp/__main__.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2006 2022-11-09 22:27:33.000000 aiosftp-0.2.1/aiosftp/conf.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5894 2022-11-09 22:45:17.000000 aiosftp-0.2.1/aiosftp/ftp.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6792 2022-11-09 23:04:57.000000 aiosftp-0.2.1/aiosftp/scp.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1992 2022-11-09 22:57:34.000000 aiosftp-0.2.1/aiosftp/user.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      546 2023-03-08 20:50:09.000000 aiosftp-0.2.1/aiosftp/version.py
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-03-08 20:54:13.672931 aiosftp-0.2.1/aiosftp.egg-info/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2963 2023-03-08 20:54:13.000000 aiosftp-0.2.1/aiosftp.egg-info/PKG-INFO
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      898 2023-03-08 20:54:13.000000 aiosftp-0.2.1/aiosftp.egg-info/SOURCES.txt
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)        1 2023-03-08 20:54:13.000000 aiosftp-0.2.1/aiosftp.egg-info/dependency_links.txt
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       49 2023-03-08 20:54:13.000000 aiosftp-0.2.1/aiosftp.egg-info/entry_points.txt
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      148 2023-03-08 20:54:13.000000 aiosftp-0.2.1/aiosftp.egg-info/requires.txt
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)        8 2023-03-08 20:54:13.000000 aiosftp-0.2.1/aiosftp.egg-info/top_level.txt
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-03-08 20:54:13.672931 aiosftp-0.2.1/docs/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      299 2023-03-08 18:17:22.000000 aiosftp-0.2.1/docs/requirements-dev.txt
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1163 2022-11-09 22:36:21.000000 aiosftp-0.2.1/docs/sql-ftpusers.sql
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-03-08 20:54:13.672931 aiosftp-0.2.1/docs/ssl/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      756 2022-11-09 21:51:47.000000 aiosftp-0.2.1/docs/ssl/known_hosts
--rw-------   0 jesuslara  (1000) jesuslara  (1000)     1381 2022-11-09 21:51:47.000000 aiosftp-0.2.1/docs/ssl/ssh_host_dsa_key
--rw-r--r--   0 jesuslara  (1000) jesuslara  (1000)      606 2022-11-09 21:51:47.000000 aiosftp-0.2.1/docs/ssl/ssh_host_dsa_key.pub
--rw-------   0 jesuslara  (1000) jesuslara  (1000)      736 2022-11-09 21:51:47.000000 aiosftp-0.2.1/docs/ssl/ssh_host_ecdsa_key
--rw-r--r--   0 jesuslara  (1000) jesuslara  (1000)      270 2022-11-09 21:51:47.000000 aiosftp-0.2.1/docs/ssl/ssh_host_ecdsa_key.pub
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2602 2022-11-09 21:51:47.000000 aiosftp-0.2.1/docs/ssl/ssh_host_rsa_key
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      570 2022-11-09 21:51:47.000000 aiosftp-0.2.1/docs/ssl/ssh_host_rsa_key.pub
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      134 2022-11-09 21:52:15.000000 aiosftp-0.2.1/docs/ssl/sshd-banner
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3266 2022-11-09 21:51:47.000000 aiosftp-0.2.1/docs/ssl/sshd_config
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1708 2022-11-09 21:51:47.000000 aiosftp-0.2.1/docs/ssl/ssl-cert-snakeoil.key
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1074 2022-11-09 21:51:47.000000 aiosftp-0.2.1/docs/ssl/ssl-cert-snakeoil.pem
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1405 2023-03-08 20:41:56.000000 aiosftp-0.2.1/pyproject.toml
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       70 2022-11-09 21:00:03.000000 aiosftp-0.2.1/pytest.ini
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       38 2023-03-08 20:54:13.676931 aiosftp-0.2.1/setup.cfg
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3481 2023-03-08 20:41:28.000000 aiosftp-0.2.1/setup.py
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-03-08 20:54:13.672931 aiosftp-0.2.1/tests/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)        0 2022-11-09 20:57:52.000000 aiosftp-0.2.1/tests/__init__.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-18 16:22:12.656221 aiosftp-0.2.2/
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-18 16:22:12.652222 aiosftp-0.2.2/.github/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      125 2022-11-09 21:24:33.000000 aiosftp-0.2.2/.github/dependabot.yml
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-18 16:22:12.652222 aiosftp-0.2.2/.github/workflows/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2731 2022-11-09 23:53:30.000000 aiosftp-0.2.2/.github/workflows/codeql-analysis.yml
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      833 2023-03-08 18:43:37.000000 aiosftp-0.2.2/.github/workflows/release.yml
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1838 2022-11-29 01:22:18.000000 aiosftp-0.2.2/.gitignore
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      174 2022-11-09 21:00:12.000000 aiosftp-0.2.2/.isort.cfg
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       37 2022-11-09 20:59:27.000000 aiosftp-0.2.2/.mypy.ini
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    20245 2022-11-09 20:59:39.000000 aiosftp-0.2.2/.pylintrc
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      329 2022-11-09 20:56:46.000000 aiosftp-0.2.2/CHANGELOG.md
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3225 2022-11-09 20:59:54.000000 aiosftp-0.2.2/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    11357 2022-11-09 20:54:25.000000 aiosftp-0.2.2/LICENSE
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      568 2023-03-08 18:18:46.000000 aiosftp-0.2.2/Makefile
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2986 2023-04-18 16:22:12.656221 aiosftp-0.2.2/PKG-INFO
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1629 2022-11-09 23:28:12.000000 aiosftp-0.2.2/README.md
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-18 16:22:12.652222 aiosftp-0.2.2/aiosftp/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       93 2022-11-09 21:36:43.000000 aiosftp-0.2.2/aiosftp/__init__.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2500 2023-04-18 16:17:46.000000 aiosftp-0.2.2/aiosftp/__main__.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2006 2022-11-09 22:27:33.000000 aiosftp-0.2.2/aiosftp/conf.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5894 2022-11-09 22:45:17.000000 aiosftp-0.2.2/aiosftp/ftp.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6792 2022-11-09 23:04:57.000000 aiosftp-0.2.2/aiosftp/scp.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1992 2022-11-09 22:57:34.000000 aiosftp-0.2.2/aiosftp/user.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      546 2023-04-18 16:08:48.000000 aiosftp-0.2.2/aiosftp/version.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-18 16:22:12.652222 aiosftp-0.2.2/aiosftp.egg-info/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2986 2023-04-18 16:22:12.000000 aiosftp-0.2.2/aiosftp.egg-info/PKG-INFO
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      898 2023-04-18 16:22:12.000000 aiosftp-0.2.2/aiosftp.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)        1 2023-04-18 16:22:12.000000 aiosftp-0.2.2/aiosftp.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       49 2023-04-18 16:22:12.000000 aiosftp-0.2.2/aiosftp.egg-info/entry_points.txt
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      158 2023-04-18 16:22:12.000000 aiosftp-0.2.2/aiosftp.egg-info/requires.txt
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)        8 2023-04-18 16:22:12.000000 aiosftp-0.2.2/aiosftp.egg-info/top_level.txt
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-18 16:22:12.656221 aiosftp-0.2.2/docs/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      299 2023-03-08 18:17:22.000000 aiosftp-0.2.2/docs/requirements-dev.txt
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1163 2022-11-09 22:36:21.000000 aiosftp-0.2.2/docs/sql-ftpusers.sql
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-18 16:22:12.656221 aiosftp-0.2.2/docs/ssl/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      756 2022-11-09 21:51:47.000000 aiosftp-0.2.2/docs/ssl/known_hosts
+-rw-------   0 jesuslara  (1000) jesuslara  (1000)     1381 2022-11-09 21:51:47.000000 aiosftp-0.2.2/docs/ssl/ssh_host_dsa_key
+-rw-r--r--   0 jesuslara  (1000) jesuslara  (1000)      606 2022-11-09 21:51:47.000000 aiosftp-0.2.2/docs/ssl/ssh_host_dsa_key.pub
+-rw-------   0 jesuslara  (1000) jesuslara  (1000)      736 2022-11-09 21:51:47.000000 aiosftp-0.2.2/docs/ssl/ssh_host_ecdsa_key
+-rw-r--r--   0 jesuslara  (1000) jesuslara  (1000)      270 2022-11-09 21:51:47.000000 aiosftp-0.2.2/docs/ssl/ssh_host_ecdsa_key.pub
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2602 2022-11-09 21:51:47.000000 aiosftp-0.2.2/docs/ssl/ssh_host_rsa_key
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      570 2022-11-09 21:51:47.000000 aiosftp-0.2.2/docs/ssl/ssh_host_rsa_key.pub
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      134 2022-11-09 21:52:15.000000 aiosftp-0.2.2/docs/ssl/sshd-banner
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3266 2022-11-09 21:51:47.000000 aiosftp-0.2.2/docs/ssl/sshd_config
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1708 2022-11-09 21:51:47.000000 aiosftp-0.2.2/docs/ssl/ssl-cert-snakeoil.key
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1074 2022-11-09 21:51:47.000000 aiosftp-0.2.2/docs/ssl/ssl-cert-snakeoil.pem
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1405 2023-04-18 16:11:33.000000 aiosftp-0.2.2/pyproject.toml
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       70 2022-11-09 21:00:03.000000 aiosftp-0.2.2/pytest.ini
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       38 2023-04-18 16:22:12.656221 aiosftp-0.2.2/setup.cfg
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3544 2023-04-18 16:15:01.000000 aiosftp-0.2.2/setup.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-18 16:22:12.656221 aiosftp-0.2.2/tests/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)        0 2022-11-09 20:57:52.000000 aiosftp-0.2.2/tests/__init__.py
```

### Comparing `aiosftp-0.2.1/.github/workflows/codeql-analysis.yml` & `aiosftp-0.2.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/.github/workflows/release.yml` & `aiosftp-0.2.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/.gitignore` & `aiosftp-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/.pylintrc` & `aiosftp-0.2.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/CODE_OF_CONDUCT.md` & `aiosftp-0.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/LICENSE` & `aiosftp-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/Makefile` & `aiosftp-0.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/PKG-INFO` & `aiosftp-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosftp
-Version: 0.2.1
+Version: 0.2.2
 Summary: FTP/SSH/sFTP Server implementation built on to of Asyncio.Facility to deploy SSH server easily inside any project.
 Home-page: https://github.com/phenobarbital/aiosftp
 Author: Jesus Lara
 Author-email: jesuslara@phenobarbital.info
 License: Apache-2
 Project-URL: Source, https://github.com/phenobarbital/aiosftp
 Project-URL: Funding, https://paypal.me/phenobarbital
@@ -22,14 +22,15 @@
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: AsyncIO
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
+Provides-Extra: uvloop
 License-File: LICENSE
 
 # aioSFTP #
 
 [![pypi](https://img.shields.io/pypi/v/aiosftp?style=plastic)](https://pypi.org/project/aiosftp/)
 [![status](https://img.shields.io/pypi/status/aiosftp?style=plastic)](https://pypi.org/project/aiosftp/)
 [![versions](https://img.shields.io/pypi/pyversions/blacksheep.svg?style=plastic)](https://github.com/phenobarbital/naiosftp)
```

### Comparing `aiosftp-0.2.1/README.md` & `aiosftp-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/aiosftp/__main__.py` & `aiosftp-0.2.2/aiosftp/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         loop.run_until_complete(
             ftp.start()
         )
         loop.run_until_complete(
             scp.start()
         )
         loop.run_forever()
-    except Exception as e:
+    except Exception:
         raise
     except KeyboardInterrupt:
         loop.run_until_complete(ftp.close())
         loop.run_until_complete(scp.close())
         print('Closing (s)FTP Connections ...')
     finally:
         loop.close()
```

### Comparing `aiosftp-0.2.1/aiosftp/conf.py` & `aiosftp-0.2.2/aiosftp/conf.py`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/aiosftp/ftp.py` & `aiosftp-0.2.2/aiosftp/ftp.py`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/aiosftp/scp.py` & `aiosftp-0.2.2/aiosftp/scp.py`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/aiosftp/user.py` & `aiosftp-0.2.2/aiosftp/user.py`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/aiosftp/version.py` & `aiosftp-0.2.2/aiosftp/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """aioSFTP Meta information.
    FTP/SSH Servers implementation.
 """
 
 __title__ = 'aiosftp'
 __description__ = ('FTP/SSH/sFTP Server implementation built on to of Asyncio.'
                    'Facility to deploy SSH server easily inside any project.')
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 __author__ = 'Jesus Lara'
 __author_email__ = 'jesuslara@phenoarbital.info'
 __license__ = 'Apache-2'
 
 def get_version() -> tuple: # pragma: no cover
    """
    Get aiosftp server version as a tuple.
```

### Comparing `aiosftp-0.2.1/aiosftp.egg-info/PKG-INFO` & `aiosftp-0.2.2/aiosftp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosftp
-Version: 0.2.1
+Version: 0.2.2
 Summary: FTP/SSH/sFTP Server implementation built on to of Asyncio.Facility to deploy SSH server easily inside any project.
 Home-page: https://github.com/phenobarbital/aiosftp
 Author: Jesus Lara
 Author-email: jesuslara@phenobarbital.info
 License: Apache-2
 Project-URL: Source, https://github.com/phenobarbital/aiosftp
 Project-URL: Funding, https://paypal.me/phenobarbital
@@ -22,14 +22,15 @@
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: AsyncIO
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
+Provides-Extra: uvloop
 License-File: LICENSE
 
 # aioSFTP #
 
 [![pypi](https://img.shields.io/pypi/v/aiosftp?style=plastic)](https://pypi.org/project/aiosftp/)
 [![status](https://img.shields.io/pypi/status/aiosftp?style=plastic)](https://pypi.org/project/aiosftp/)
 [![versions](https://img.shields.io/pypi/pyversions/blacksheep.svg?style=plastic)](https://github.com/phenobarbital/naiosftp)
```

### Comparing `aiosftp-0.2.1/aiosftp.egg-info/SOURCES.txt` & `aiosftp-0.2.2/aiosftp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/docs/sql-ftpusers.sql` & `aiosftp-0.2.2/docs/sql-ftpusers.sql`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/docs/ssl/known_hosts` & `aiosftp-0.2.2/docs/ssl/known_hosts`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/docs/ssl/ssh_host_dsa_key` & `aiosftp-0.2.2/docs/ssl/ssh_host_dsa_key`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/docs/ssl/ssh_host_dsa_key.pub` & `aiosftp-0.2.2/docs/ssl/ssh_host_dsa_key.pub`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/docs/ssl/ssh_host_ecdsa_key` & `aiosftp-0.2.2/docs/ssl/ssh_host_ecdsa_key`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/docs/ssl/ssh_host_rsa_key` & `aiosftp-0.2.2/docs/ssl/ssh_host_rsa_key`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/docs/ssl/ssh_host_rsa_key.pub` & `aiosftp-0.2.2/docs/ssl/ssh_host_rsa_key.pub`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/docs/ssl/sshd_config` & `aiosftp-0.2.2/docs/ssl/sshd_config`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/docs/ssl/ssl-cert-snakeoil.key` & `aiosftp-0.2.2/docs/ssl/ssl-cert-snakeoil.key`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/docs/ssl/ssl-cert-snakeoil.pem` & `aiosftp-0.2.2/docs/ssl/ssl-cert-snakeoil.pem`

 * *Files identical despite different names*

### Comparing `aiosftp-0.2.1/pyproject.toml` & `aiosftp-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = [
-    'setuptools==67.5.1',
+    'setuptools==67.6.1',
     'setuptools-scm',
     'Cython==0.29.33',
-    'wheel==0.38.4',
+    'wheel==0.40.0',
     'flit'
 ]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [tool.flit.metadata]
 module = "aiosftp"
 author = "Jesus Lara Gimenez"
```

### Comparing `aiosftp-0.2.1/setup.py` & `aiosftp-0.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,28 +73,32 @@
         'Framework :: AsyncIO'
     ],
     author='Jesus Lara',
     author_email='jesuslara@phenobarbital.info',
     packages=find_packages(exclude=["contrib", "docs", "tests", "settings"]),
     include_package_data=True,
     setup_requires=[
-        'wheel==0.38.4',
+        'wheel==0.40.0',
         'cython==0.29.33'
     ],
     install_requires=[
-        'wheel==0.38.4',
+        'wheel==0.40.0',
         "aiohttp==3.8.4",
         "asyncio==3.4.3",
-        "uvloop==0.17.0",
         "asyncdb>=2.2.0",
         "navconfig[default]>=1.1.0",
         "aioftp==0.21.4",
         "siosocks>=0.3.0",
         "asyncssh==2.13.1",
     ],
+    extras_require={
+        "uvloop": [
+            "uvloop==0.17.0",
+        ],
+    },
     entry_points={
         'console_scripts': [
             'aioftp = aiosftp.__main__:main'
         ]
     },
     project_urls={  # Optional
         'Source': 'https://github.com/phenobarbital/aiosftp',
```

