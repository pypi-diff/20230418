# Comparing `tmp/artifacts-20221219.tar.gz` & `tmp/artifacts-20230413.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artifacts-20221219.tar", last modified: Mon Dec 19 17:49:47 2022, max compression
+gzip compressed data, was "artifacts-20230413.tar", last modified: Tue Apr 18 03:49:47 2023, max compression
```

## Comparing `artifacts-20221219.tar` & `artifacts-20230413.tar`

### file list

```diff
@@ -1,128 +1,130 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-19 17:49:47.326697 artifacts-20221219/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-19 17:49:47.181697 artifacts-20221219/.github/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-19 17:49:47.230697 artifacts-20221219/.github/workflows/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2493 2022-12-19 17:49:28.000000 artifacts-20221219/.github/workflows/test_docker.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1343 2022-12-19 17:49:28.000000 artifacts-20221219/.github/workflows/test_docs.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1643 2022-12-19 17:49:28.000000 artifacts-20221219/.github/workflows/test_tox.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21003 2022-12-19 17:28:46.000000 artifacts-20221219/.pylintrc
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      149 2022-03-20 08:05:24.000000 artifacts-20221219/.yamllint.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      151 2021-11-01 18:53:11.000000 artifacts-20221219/ACKNOWLEDGEMENTS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      488 2014-11-26 17:20:08.000000 artifacts-20221219/AUTHORS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11325 2014-11-19 19:52:15.000000 artifacts-20221219/LICENSE
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      609 2022-03-20 08:05:24.000000 artifacts-20221219/MANIFEST.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      674 2022-12-19 17:49:47.327697 artifacts-20221219/PKG-INFO
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      303 2021-11-15 13:27:42.000000 artifacts-20221219/README
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      932 2021-11-15 13:27:49.000000 artifacts-20221219/README.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2022-12-19 17:28:46.000000 artifacts-20221219/appveyor.yml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-19 17:49:47.232697 artifacts-20221219/artifacts/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       99 2022-12-19 17:49:28.000000 artifacts-20221219/artifacts/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3274 2022-10-09 16:01:05.000000 artifacts-20221219/artifacts/artifact.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      946 2022-10-09 14:10:43.000000 artifacts-20221219/artifacts/definitions.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      387 2018-03-18 07:06:42.000000 artifacts-20221219/artifacts/errors.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10920 2022-10-09 16:01:05.000000 artifacts-20221219/artifacts/reader.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8516 2022-10-09 16:01:05.000000 artifacts-20221219/artifacts/registry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13704 2022-10-09 16:01:05.000000 artifacts-20221219/artifacts/source_type.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2733 2022-06-05 09:55:00.000000 artifacts-20221219/artifacts/writer.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-19 17:49:47.233697 artifacts-20221219/artifacts.egg-info/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      674 2022-12-19 17:49:45.000000 artifacts-20221219/artifacts.egg-info/PKG-INFO
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2438 2022-12-19 17:49:47.000000 artifacts-20221219/artifacts.egg-info/SOURCES.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2022-12-19 17:49:45.000000 artifacts-20221219/artifacts.egg-info/dependency_links.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-12-19 17:49:45.000000 artifacts-20221219/artifacts.egg-info/requires.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       10 2022-12-19 17:49:45.000000 artifacts-20221219/artifacts.egg-info/top_level.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      529 2021-11-15 13:27:42.000000 artifacts-20221219/artifacts.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-19 17:49:47.182697 artifacts-20221219/config/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-19 17:49:47.234697 artifacts-20221219/config/appveyor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      758 2022-12-19 17:49:28.000000 artifacts-20221219/config/appveyor/install.ps1
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2022-12-19 17:28:46.000000 artifacts-20221219/config/appveyor/install.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2022-12-19 17:28:46.000000 artifacts-20221219/config/appveyor/runtests.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-19 17:49:47.284697 artifacts-20221219/config/dpkg/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       21 2017-05-20 19:17:24.000000 artifacts-20221219/config/dpkg/artifacts-data.dirs
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       27 2017-07-01 08:08:23.000000 artifacts-20221219/config/dpkg/artifacts-data.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        8 2017-05-21 20:05:37.000000 artifacts-20221219/config/dpkg/artifacts-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      159 2022-12-19 17:49:28.000000 artifacts-20221219/config/dpkg/changelog
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       22 2017-05-20 19:17:24.000000 artifacts-20221219/config/dpkg/clean
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2022-12-19 17:28:46.000000 artifacts-20221219/config/dpkg/compat
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2022-12-19 17:28:46.000000 artifacts-20221219/config/dpkg/control
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1017 2017-05-13 17:01:46.000000 artifacts-20221219/config/dpkg/copyright
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       99 2017-05-20 19:17:24.000000 artifacts-20221219/config/dpkg/python3-artifacts.install
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2022-12-19 17:28:46.000000 artifacts-20221219/config/dpkg/rules
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-19 17:49:47.284697 artifacts-20221219/config/dpkg/source/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2017-05-20 19:17:24.000000 artifacts-20221219/config/dpkg/source/format
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-19 17:49:47.302697 artifacts-20221219/data/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6762 2022-11-21 18:38:28.000000 artifacts-20221219/data/antivirus.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4248 2022-11-21 18:57:08.000000 artifacts-20221219/data/applications.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2787 2022-11-21 18:57:08.000000 artifacts-20221219/data/cloud_services.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1664 2022-11-21 18:38:28.000000 artifacts-20221219/data/config_files.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      812 2022-11-21 18:38:28.000000 artifacts-20221219/data/containerd.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6324 2022-11-21 18:38:28.000000 artifacts-20221219/data/database_servers.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      522 2022-11-21 18:38:28.000000 artifacts-20221219/data/docker.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3602 2022-11-21 18:38:28.000000 artifacts-20221219/data/esxi.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1030 2022-11-21 18:38:28.000000 artifacts-20221219/data/file_systems.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1258 2022-11-21 18:38:28.000000 artifacts-20221219/data/hadoop.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1958 2022-12-19 16:43:19.000000 artifacts-20221219/data/installed_module_paths.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5243 2022-11-21 18:38:28.000000 artifacts-20221219/data/installed_modules.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2022-11-21 18:57:08.000000 artifacts-20221219/data/instant_messaging.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      558 2022-11-21 18:38:28.000000 artifacts-20221219/data/java.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5174 2022-11-21 18:38:28.000000 artifacts-20221219/data/kaspersky_careto.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5223 2022-11-21 18:38:28.000000 artifacts-20221219/data/kubernetes.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2743 2022-11-21 18:38:28.000000 artifacts-20221219/data/legacy.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24977 2022-12-16 20:19:10.000000 artifacts-20221219/data/linux.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5117 2022-11-21 18:38:28.000000 artifacts-20221219/data/linux_proc.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2022-11-21 18:38:28.000000 artifacts-20221219/data/linux_services.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27715 2022-11-21 18:57:08.000000 artifacts-20221219/data/macos.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8373 2022-11-21 18:57:08.000000 artifacts-20221219/data/shell.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4201 2022-11-21 18:38:28.000000 artifacts-20221219/data/tomcat.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8988 2022-11-21 18:38:28.000000 artifacts-20221219/data/triage.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2522 2022-11-21 18:38:28.000000 artifacts-20221219/data/unix_common.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      896 2022-11-21 18:57:08.000000 artifacts-20221219/data/user.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    65574 2022-12-16 20:19:10.000000 artifacts-20221219/data/webbrowser.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2884 2022-11-21 18:38:28.000000 artifacts-20221219/data/webservers.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   167852 2022-11-21 18:57:08.000000 artifacts-20221219/data/windows.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6174 2022-11-21 18:38:28.000000 artifacts-20221219/data/windows_dll_hijacking.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8549 2022-11-21 18:57:08.000000 artifacts-20221219/data/wmi.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      150 2021-11-01 18:53:11.000000 artifacts-20221219/dependencies.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-19 17:49:47.310697 artifacts-20221219/docs/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       88 2021-11-15 13:27:42.000000 artifacts-20221219/docs/Artifacts definition format and style guide.asciidoc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2022-12-19 17:49:28.000000 artifacts-20221219/docs/conf.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      673 2022-03-20 08:05:24.000000 artifacts-20221219/docs/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2022-12-19 17:28:55.000000 artifacts-20221219/docs/requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-19 17:49:47.310697 artifacts-20221219/docs/sources/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15892 2022-07-10 06:36:45.000000 artifacts-20221219/docs/sources/Format-specification.md
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-19 17:49:47.311697 artifacts-20221219/docs/sources/api/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1176 2021-11-15 13:27:43.000000 artifacts-20221219/docs/sources/api/artifacts.rst
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       64 2021-11-15 13:27:43.000000 artifacts-20221219/docs/sources/api/modules.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-19 17:49:47.312697 artifacts-20221219/docs/sources/background/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      726 2022-12-19 17:49:28.000000 artifacts-20221219/docs/sources/background/Stats.md
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      873 2021-11-15 13:27:43.000000 artifacts-20221219/docs/sources/background/Terminology.md
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1276 2021-11-15 13:27:43.000000 artifacts-20221219/docs/sources/background/index.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-19 17:49:47.312697 artifacts-20221219/docs/sources/user/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2021-11-15 13:27:43.000000 artifacts-20221219/docs/sources/user/Installation-instructions.md
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      311 2021-11-15 13:27:43.000000 artifacts-20221219/docs/sources/user/index.rst
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       28 2022-12-19 17:28:46.000000 artifacts-20221219/requirements.txt
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1018 2022-10-09 16:01:05.000000 artifacts-20221219/run_tests.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      320 2022-12-19 17:49:47.327697 artifacts-20221219/setup.cfg
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7313 2022-12-19 17:28:46.000000 artifacts-20221219/setup.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-19 17:49:47.313697 artifacts-20221219/test_data/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2422 2022-07-10 06:36:45.000000 artifacts-20221219/test_data/definitions.json
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2312 2022-07-10 06:36:45.000000 artifacts-20221219/test_data/definitions.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-19 17:49:28.000000 artifacts-20221219/test_dependencies.ini
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-19 17:49:28.000000 artifacts-20221219/test_requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-19 17:49:47.315697 artifacts-20221219/tests/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2021-11-01 18:53:11.000000 artifacts-20221219/tests/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11907 2022-10-09 16:01:05.000000 artifacts-20221219/tests/reader_test.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4906 2022-07-10 06:36:45.000000 artifacts-20221219/tests/registry_test.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5365 2022-03-20 08:05:24.000000 artifacts-20221219/tests/source_type_test.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1720 2022-10-09 16:01:05.000000 artifacts-20221219/tests/test_lib.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1135 2022-10-09 16:01:05.000000 artifacts-20221219/tests/validator_test.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1837 2022-03-20 08:05:24.000000 artifacts-20221219/tests/writer_test.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-19 17:49:47.315697 artifacts-20221219/tools/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       46 2021-11-01 18:53:12.000000 artifacts-20221219/tools/__init__.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3740 2022-10-19 17:44:16.000000 artifacts-20221219/tools/stats.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    21201 2022-10-09 16:01:05.000000 artifacts-20221219/tools/validator.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2022-12-19 17:28:46.000000 artifacts-20221219/tox.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-19 17:49:47.326697 artifacts-20221219/utils/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        0 2018-03-18 07:06:41.000000 artifacts-20221219/utils/__init__.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2022-12-19 17:28:46.000000 artifacts-20221219/utils/check_dependencies.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2022-12-19 17:28:46.000000 artifacts-20221219/utils/dependencies.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9073 2015-05-07 21:05:55.000000 artifacts-20221219/utils/pylintrc
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      675 2022-03-20 08:05:24.000000 artifacts-20221219/utils/update_release.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-18 03:49:47.215101 artifacts-20230413/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-18 03:49:46.955101 artifacts-20230413/.github/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-18 03:49:47.053101 artifacts-20230413/.github/workflows/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2515 2023-04-13 07:50:17.000000 artifacts-20230413/.github/workflows/test_docker.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-04-13 07:50:17.000000 artifacts-20230413/.github/workflows/test_docs.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4068 2023-04-13 07:50:17.000000 artifacts-20230413/.github/workflows/test_tox.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21911 2023-04-13 06:58:50.000000 artifacts-20230413/.pylintrc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      149 2022-12-20 18:52:11.000000 artifacts-20230413/.yamllint.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      151 2021-11-01 18:53:11.000000 artifacts-20230413/ACKNOWLEDGEMENTS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      488 2014-11-26 17:20:08.000000 artifacts-20230413/AUTHORS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11325 2014-11-19 19:52:15.000000 artifacts-20230413/LICENSE
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      609 2022-12-20 18:52:11.000000 artifacts-20230413/MANIFEST.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      674 2023-04-18 03:49:47.215101 artifacts-20230413/PKG-INFO
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      303 2022-12-20 18:52:11.000000 artifacts-20230413/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      932 2022-12-20 18:52:11.000000 artifacts-20230413/README.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-04-13 06:58:50.000000 artifacts-20230413/appveyor.yml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-18 03:49:47.055101 artifacts-20230413/artifacts/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       99 2023-04-18 03:49:23.000000 artifacts-20230413/artifacts/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3274 2022-12-20 18:52:11.000000 artifacts-20230413/artifacts/artifact.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      946 2022-12-20 18:52:11.000000 artifacts-20230413/artifacts/definitions.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      387 2018-03-18 07:06:42.000000 artifacts-20230413/artifacts/errors.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10920 2022-12-20 18:52:11.000000 artifacts-20230413/artifacts/reader.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8516 2022-12-20 18:52:11.000000 artifacts-20230413/artifacts/registry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13704 2022-12-20 18:52:11.000000 artifacts-20230413/artifacts/source_type.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2733 2022-12-20 18:52:11.000000 artifacts-20230413/artifacts/writer.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-18 03:49:47.056101 artifacts-20230413/artifacts.egg-info/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      674 2023-04-18 03:49:44.000000 artifacts-20230413/artifacts.egg-info/PKG-INFO
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2475 2023-04-18 03:49:46.000000 artifacts-20230413/artifacts.egg-info/SOURCES.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-04-18 03:49:44.000000 artifacts-20230413/artifacts.egg-info/dependency_links.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-04-18 03:49:44.000000 artifacts-20230413/artifacts.egg-info/requires.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       10 2023-04-18 03:49:44.000000 artifacts-20230413/artifacts.egg-info/top_level.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      529 2022-12-20 18:52:11.000000 artifacts-20230413/artifacts.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-18 03:49:46.956101 artifacts-20230413/config/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-18 03:49:47.057101 artifacts-20230413/config/appveyor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      834 2023-04-13 06:58:50.000000 artifacts-20230413/config/appveyor/install.ps1
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2023-04-13 06:58:50.000000 artifacts-20230413/config/appveyor/install.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2023-04-13 06:58:50.000000 artifacts-20230413/config/appveyor/runtests.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-18 03:49:47.106101 artifacts-20230413/config/dpkg/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       21 2017-05-20 19:17:24.000000 artifacts-20230413/config/dpkg/artifacts-data.dirs
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       27 2017-07-01 08:08:23.000000 artifacts-20230413/config/dpkg/artifacts-data.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        8 2017-05-21 20:05:37.000000 artifacts-20230413/config/dpkg/artifacts-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      159 2023-04-18 03:49:23.000000 artifacts-20230413/config/dpkg/changelog
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       22 2017-05-20 19:17:24.000000 artifacts-20230413/config/dpkg/clean
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2023-04-13 06:58:50.000000 artifacts-20230413/config/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2023-04-13 06:58:50.000000 artifacts-20230413/config/dpkg/control
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1017 2017-05-13 17:01:46.000000 artifacts-20230413/config/dpkg/copyright
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       99 2017-05-20 19:17:24.000000 artifacts-20230413/config/dpkg/python3-artifacts.install
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2023-04-13 06:58:50.000000 artifacts-20230413/config/dpkg/rules
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-18 03:49:47.107101 artifacts-20230413/config/dpkg/source/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2017-05-20 19:17:24.000000 artifacts-20230413/config/dpkg/source/format
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-18 03:49:47.148101 artifacts-20230413/data/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16384 2023-01-30 18:02:06.000000 artifacts-20230413/data/.windows.yaml.swp
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6762 2022-12-20 18:52:11.000000 artifacts-20230413/data/antivirus.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4248 2022-12-20 18:52:11.000000 artifacts-20230413/data/applications.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2787 2022-12-20 18:52:11.000000 artifacts-20230413/data/cloud_services.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1664 2022-12-20 18:52:11.000000 artifacts-20230413/data/config_files.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      812 2022-12-20 18:52:11.000000 artifacts-20230413/data/containerd.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6324 2022-12-20 18:52:11.000000 artifacts-20230413/data/database_servers.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      522 2022-12-20 18:52:11.000000 artifacts-20230413/data/docker.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3602 2022-12-20 18:52:11.000000 artifacts-20230413/data/esxi.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1030 2022-12-20 18:52:11.000000 artifacts-20230413/data/file_systems.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1258 2022-12-20 18:52:11.000000 artifacts-20230413/data/hadoop.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2023-01-30 17:22:48.000000 artifacts-20230413/data/ics.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1958 2022-12-20 18:52:11.000000 artifacts-20230413/data/installed_module_paths.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5243 2022-12-20 18:52:11.000000 artifacts-20230413/data/installed_modules.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2316 2023-01-30 17:22:48.000000 artifacts-20230413/data/instant_messaging.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      558 2022-12-20 18:52:11.000000 artifacts-20230413/data/java.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5174 2022-12-20 18:52:11.000000 artifacts-20230413/data/kaspersky_careto.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5223 2022-12-20 18:52:11.000000 artifacts-20230413/data/kubernetes.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2743 2022-12-20 18:52:11.000000 artifacts-20230413/data/legacy.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24973 2023-01-30 17:22:48.000000 artifacts-20230413/data/linux.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5117 2022-12-20 18:52:11.000000 artifacts-20230413/data/linux_proc.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2022-12-20 18:52:11.000000 artifacts-20230413/data/linux_services.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27748 2023-01-30 17:22:48.000000 artifacts-20230413/data/macos.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8373 2022-12-20 18:52:11.000000 artifacts-20230413/data/shell.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4201 2022-12-20 18:52:11.000000 artifacts-20230413/data/tomcat.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8988 2022-12-20 18:52:11.000000 artifacts-20230413/data/triage.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2522 2022-12-20 18:52:11.000000 artifacts-20230413/data/unix_common.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      892 2023-01-30 17:22:48.000000 artifacts-20230413/data/user.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    71374 2023-04-13 03:32:57.000000 artifacts-20230413/data/webbrowser.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2884 2022-12-20 18:52:11.000000 artifacts-20230413/data/webservers.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   167680 2022-12-20 18:52:11.000000 artifacts-20230413/data/windows.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6174 2022-12-20 18:52:11.000000 artifacts-20230413/data/windows_dll_hijacking.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8549 2022-12-20 18:52:11.000000 artifacts-20230413/data/wmi.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      150 2021-11-01 18:53:11.000000 artifacts-20230413/dependencies.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-18 03:49:47.168101 artifacts-20230413/docs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       88 2022-12-20 18:52:11.000000 artifacts-20230413/docs/Artifacts definition format and style guide.asciidoc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2023-04-13 06:58:50.000000 artifacts-20230413/docs/conf.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      673 2022-12-20 18:52:11.000000 artifacts-20230413/docs/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2023-04-13 06:59:04.000000 artifacts-20230413/docs/requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-18 03:49:47.180101 artifacts-20230413/docs/sources/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15892 2022-12-20 18:52:11.000000 artifacts-20230413/docs/sources/Format-specification.md
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-18 03:49:47.181101 artifacts-20230413/docs/sources/api/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1176 2022-12-20 18:52:11.000000 artifacts-20230413/docs/sources/api/artifacts.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       64 2022-12-20 18:52:11.000000 artifacts-20230413/docs/sources/api/modules.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-18 03:49:47.181101 artifacts-20230413/docs/sources/background/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      726 2023-04-18 03:49:23.000000 artifacts-20230413/docs/sources/background/Stats.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      873 2022-12-20 18:52:11.000000 artifacts-20230413/docs/sources/background/Terminology.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1276 2022-12-20 18:52:11.000000 artifacts-20230413/docs/sources/background/index.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-18 03:49:47.182101 artifacts-20230413/docs/sources/user/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2022-12-20 18:52:11.000000 artifacts-20230413/docs/sources/user/Installation-instructions.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      311 2022-12-20 18:52:11.000000 artifacts-20230413/docs/sources/user/index.rst
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       28 2023-04-13 06:58:50.000000 artifacts-20230413/requirements.txt
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1018 2022-12-20 18:52:11.000000 artifacts-20230413/run_tests.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      320 2023-04-18 03:49:47.216101 artifacts-20230413/setup.cfg
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7313 2023-04-13 06:58:50.000000 artifacts-20230413/setup.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-18 03:49:47.182101 artifacts-20230413/test_data/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2422 2022-12-20 18:52:11.000000 artifacts-20230413/test_data/definitions.json
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2312 2022-12-20 18:52:11.000000 artifacts-20230413/test_data/definitions.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-20 18:52:11.000000 artifacts-20230413/test_dependencies.ini
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-13 06:58:50.000000 artifacts-20230413/test_requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-18 03:49:47.195101 artifacts-20230413/tests/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2021-11-01 18:53:11.000000 artifacts-20230413/tests/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11907 2022-12-20 18:52:11.000000 artifacts-20230413/tests/reader_test.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4906 2022-12-20 18:52:11.000000 artifacts-20230413/tests/registry_test.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5365 2022-12-20 18:52:11.000000 artifacts-20230413/tests/source_type_test.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1720 2022-12-20 18:52:11.000000 artifacts-20230413/tests/test_lib.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1135 2022-12-20 18:52:11.000000 artifacts-20230413/tests/validator_test.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1837 2022-12-20 18:52:11.000000 artifacts-20230413/tests/writer_test.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-18 03:49:47.201101 artifacts-20230413/tools/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       46 2021-11-01 18:53:12.000000 artifacts-20230413/tools/__init__.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3740 2022-12-20 18:52:11.000000 artifacts-20230413/tools/stats.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    21201 2022-12-20 18:52:11.000000 artifacts-20230413/tools/validator.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1257 2023-04-13 07:50:17.000000 artifacts-20230413/tox.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-18 03:49:47.215101 artifacts-20230413/utils/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        0 2018-03-18 07:06:41.000000 artifacts-20230413/utils/__init__.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2023-04-13 06:58:50.000000 artifacts-20230413/utils/check_dependencies.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2023-04-13 06:58:50.000000 artifacts-20230413/utils/dependencies.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9073 2015-05-07 21:05:55.000000 artifacts-20230413/utils/pylintrc
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      675 2022-12-20 18:52:11.000000 artifacts-20230413/utils/update_release.sh
```

### Comparing `artifacts-20221219/.github/workflows/test_docker.yml` & `artifacts-20230413/.github/workflows/test_docker.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Run tests on Fedora and Ubuntu Docker images using GIFT CORP and GIFT PPA on commit
 name: test_docker
 on: [push]
+permissions: read-all
 jobs:
   test_fedora:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        version: ['36']
+        version: ['37']
     container:
       image: registry.fedoraproject.org/fedora:${{ matrix.version }}
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up container
       run: |
         dnf install -y dnf-plugins-core langpacks-en
     - name: Install dependencies
       run: |
         dnf copr -y enable @gift/dev
         dnf install -y @development-tools python3 python3-devel python3-pyyaml python3-setuptools
@@ -40,15 +41,15 @@
     runs-on: ubuntu-latest
     strategy:
       matrix:
         version: ['22.04']
     container:
       image: ubuntu:${{ matrix.version }}
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
```

### Comparing `artifacts-20221219/.github/workflows/test_docs.yml` & `artifacts-20230413/.github/workflows/test_docs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 on:
   pull_request:
     branches:
     - main
   push:
     branches:
     - main
+permissions: read-all
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         include:
         - python-version: '3.8'
           toxenv: 'docs'
     container:
       image: ubuntu:22.04
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
```

### Comparing `artifacts-20221219/.pylintrc` & `artifacts-20230413/.pylintrc`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,30 @@
-# Pylint 2.10.x configuration file
+# Pylint 2.14.x configuration file
 #
 # This file is generated by l2tdevtools update-dependencies.py, any dependency
 # related changes should be made in dependencies.ini.
-[MASTER]
+[MAIN]
+
+# Analyse import fallback blocks. This can be used to support both Python 2 and
+# 3 compatible code, which means that the block might have code that exists
+# only in one or another interpreter, leading to false positives when analysed.
+analyse-fallback-blocks=no
+
+# Load and enable all available extensions. Use --list-extensions to see a list
+# all available extensions.
+#enable-all-extensions=
+
+# In error mode, messages with a category besides ERROR or FATAL are
+# suppressed, and no reports are done by default. Error mode is compatible with
+# disabling specific errors.
+#errors-only=
+
+# Always return a 0 (non-error) status code, even if lint errors are found.
+# This is primarily useful in continuous integration scripts.
+#exit-zero=
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code.
 extension-pkg-allow-list=
 
 # A comma-separated list of package or module names from where C extensions may
@@ -17,70 +35,116 @@
 
 # Return non-zero exit code if any of these messages/categories are detected,
 # even if score is above --fail-under value. Syntax same as enable. Messages
 # specified are enabled, while categories only check already-enabled messages.
 fail-on=
 
 # Specify a score threshold to be exceeded before program exits with error.
-fail-under=10.0
+fail-under=10
+
+# Interpret the stdin as a python script, whose filename needs to be passed as
+# the module_or_package argument.
+#from-stdin=
 
 # Files or directories to be skipped. They should be base names, not paths.
 ignore=CVS
 
 # Add files or directories matching the regex patterns to the ignore-list. The
 # regex matches against paths and can be in Posix or Windows format.
 ignore-paths=
 
 # Files or directories matching the regex patterns are skipped. The regex
-# matches against base names, not paths. The default value ignores emacs file
+# matches against base names, not paths. The default value ignores Emacs file
 # locks
 ignore-patterns=^\.#
 
+# List of module names for which member attributes should not be checked
+# (useful for modules/projects where namespaces are manipulated during runtime
+# and thus existing member attributes cannot be deduced by static analysis). It
+# supports qualified module names, as well as Unix pattern matching.
+ignored-modules=
+
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
 # Use multiple processes to speed up Pylint. Specifying 0 will auto-detect the
-# number of processors available to use.
+# number of processors available to use, and will cap the count on Windows to
+# avoid hangs.
 jobs=1
 
 # Control the amount of potential inferred values when inferring a single
 # object. This can help the performance when dealing with large functions or
 # complex, nested conditions.
 limit-inference-results=100
 
 # List of plugins (as comma separated values of python module names) to load,
 # usually to register additional checkers.
+# load-plugins=
 load-plugins=pylint.extensions.docparams
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Minimum Python version to use for version dependent checks. Will default to
 # the version used to run pylint.
-py-version=3.10
+py-version=3.11
 
 # Discover python modules and packages in the file system subtree.
+# recursive=no
 recursive=yes
 
 # When enabled, pylint would attempt to guess common misconfiguration and emit
 # user-friendly hints instead of false-positive error messages.
 suggestion-mode=yes
 
 # Allow loading of arbitrary C extensions. Extensions are imported into the
 # active Python interpreter and may run arbitrary code.
 unsafe-load-any-extension=no
 
+# In verbose mode, extra non-checker-related info will be displayed.
+#verbose=
+
+
+[REPORTS]
+
+# Python expression which should return a score less than or equal to 10. You
+# have access to the variables 'fatal', 'error', 'warning', 'refactor',
+# 'convention', and 'info' which contain the number of messages in each
+# category, as well as 'statement' which is the total number of statements
+# analyzed. This score is used by the global evaluation report (RP0004).
+evaluation=max(0, 0 if fatal else 10.0 - ((float(5 * error + warning + refactor + convention) / statement) * 10))
+
+# Template used to display messages. This is a python new-style format string
+# used to format the message information. See doc for all details.
+msg-template=
+
+# Set the output format. Available formats are text, parseable, colorized, json
+# and msvs (visual studio). You can also give a reporter class, e.g.
+# mypackage.mymodule.MyReporterClass.
+#output-format=
+
+# Tells whether to display a full report or only the messages.
+reports=no
+
+# Activate the evaluation score.
+# score=yes
+score=no
+
 
 [MESSAGES CONTROL]
 
 # Only show warnings with the listed confidence levels. Leave empty to show
 # all. Valid levels: HIGH, CONTROL_FLOW, INFERENCE, INFERENCE_FAILURE,
 # UNDEFINED.
-confidence=
+confidence=HIGH,
+           CONTROL_FLOW,
+           INFERENCE,
+           INFERENCE_FAILURE,
+           UNDEFINED
 
 # Disable the message, report, category or checker with the given id(s). You
 # can either give multiple identifiers separated by comma (,) or put this
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once). You can also use "--disable=all" to
 # disable everything first and then re-enable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
@@ -88,26 +152,20 @@
 # no Warning level messages displayed, use "--disable=all --enable=classes
 # --disable=W".
 disable=assignment-from-none,
         bad-inline-option,
         consider-using-f-string,
         deprecated-pragma,
         duplicate-code,
-        eq-without-hash,
         file-ignored,
         fixme,
         locally-disabled,
-        locally-enabled,
         logging-format-interpolation,
         logging-fstring-interpolation,
-        metaclass-assignment,
         missing-param-doc,
-        no-absolute-import,
-        no-self-use,
-        parameter-unpacking,
         raise-missing-from,
         raw-checker-failed,
         super-with-arguments,
         suppressed-message,
         too-few-public-methods,
         too-many-ancestors,
         too-many-boolean-expressions,
@@ -126,51 +184,14 @@
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=c-extension-no-member
 
 
-[REPORTS]
-
-# Python expression which should return a score less than or equal to 10. You
-# have access to the variables 'fatal', 'error', 'warning', 'refactor',
-# 'convention', and 'info' which contain the number of messages in each
-# category, as well as 'statement' which is the total number of statements
-# analyzed. This score is used by the global evaluation report (RP0004).
-evaluation=max(0, 0 if fatal else 10.0 - ((float(5 * error + warning + refactor + convention) / statement) * 10))
-
-# Template used to display messages. This is a python new-style format string
-# used to format the message information. See doc for all details.
-#msg-template=
-
-# Set the output format. Available formats are text, parseable, colorized, json
-# and msvs (visual studio). You can also give a reporter class, e.g.
-# mypackage.mymodule.MyReporterClass.
-output-format=text
-
-# Tells whether to display a full report or only the messages.
-reports=no
-
-# Activate the evaluation score.
-score=no
-
-
-[REFACTORING]
-
-# Maximum number of nested blocks for function / method body
-max-nested-blocks=5
-
-# Complete name of functions that never returns. When checking for
-# inconsistent-return-statements if a never returning function is called then
-# it will be considered as an explicit return statement and no message will be
-# printed.
-never-returning-functions=sys.exit,argparse.parse_error
-
-
 [VARIABLES]
 
 # List of additional names supposed to be defined in builtins. Remember that
 # you should avoid defining new builtins when possible.
 additional-builtins=
 
 # Tells whether unused global variables should be treated as a violation.
@@ -208,55 +229,50 @@
 contextmanager-decorators=contextlib.contextmanager
 
 # List of members which are set dynamically and missed by pylint inference
 # system, and so shouldn't trigger E1101 when accessed. Python regular
 # expressions are accepted.
 generated-members=
 
-# Tells whether missing members accessed in mixin class should be ignored. A
-# class is considered mixin if its name matches the mixin-class-rgx option.
-ignore-mixin-members=yes
-
 # Tells whether to warn about missing members when the owner of the attribute
 # is inferred to be None.
 ignore-none=yes
 
 # This flag controls whether pylint should warn about no-member and similar
 # checks whenever an opaque object is returned when inferring. The inference
 # can return multiple potential results while evaluating a Python object, but
 # some branches might not be evaluated, which results in partial inference. In
 # that case, it might be useful to still emit no-member and other checks for
 # the rest of the inferred objects.
 ignore-on-opaque-inference=yes
 
+# List of symbolic message names to ignore for Mixin members.
+ignored-checks-for-mixins=no-member,
+                          not-async-context-manager,
+                          not-context-manager,
+                          attribute-defined-outside-init
+
 # List of class names for which member attributes should not be checked (useful
 # for classes with dynamically set attributes). This supports the use of
 # qualified names.
-ignored-classes=optparse.Values,thread._local,_thread._local
-
-# List of module names for which member attributes should not be checked
-# (useful for modules/projects where namespaces are manipulated during runtime
-# and thus existing member attributes cannot be deduced by static analysis). It
-# supports qualified module names, as well as Unix pattern matching.
-ignored-modules=
+ignored-classes=optparse.Values,thread._local,_thread._local,argparse.Namespace
 
 # Show a hint with possible names when a member name was not found. The aspect
 # of finding the hint is based on edit distance.
 missing-member-hint=yes
 
 # The minimum edit distance a name should have in order to be considered a
 # similar match for a missing member name.
 missing-member-hint-distance=1
 
 # The total number of similar names that should be taken in consideration when
 # showing a hint for a missing member.
 missing-member-max-choices=1
 
-# Regex pattern to define which classes are considered mixins ignore-mixin-
-# members is set to 'yes'
+# Regex pattern to define which classes are considered mixins.
 mixin-class-rgx=.*[Mm]ixin
 
 # List of decorators that change the signature of a decorated function.
 signature-mutators=
 
 
 [LOGGING]
@@ -266,30 +282,74 @@
 logging-format-style=old
 
 # Logging modules to check that the string format arguments are in logging
 # function parameter format.
 logging-modules=logging
 
 
+[DESIGN]
+
+# List of regular expressions of class ancestor names to ignore when counting
+# public methods (see R0903)
+exclude-too-few-public-methods=
+
+# List of qualified class names to ignore when counting class parents (see
+# R0901)
+ignored-parents=
+
+# Maximum number of arguments for function / method.
+# max-args=5
+max-args=10
+
+# Maximum number of attributes for a class (see R0902).
+max-attributes=7
+
+# Maximum number of boolean expressions in an if statement (see R0916).
+max-bool-expr=5
+
+# Maximum number of branch for function / method body.
+max-branches=12
+
+# Maximum number of locals for function / method body.
+max-locals=15
+
+# Maximum number of parents for a class (see R0901).
+max-parents=7
+
+# Maximum number of public methods for a class (see R0904).
+max-public-methods=20
+
+# Maximum number of return / yield for function / method body.
+max-returns=6
+
+# Maximum number of statements in function / method body.
+max-statements=50
+
+# Minimum number of public methods for a class (see R0903).
+min-public-methods=2
+
+
 [BASIC]
 
 # Naming style matching correct argument names.
 argument-naming-style=snake_case
 
 # Regular expression matching correct argument names. Overrides argument-
 # naming-style. If left empty, argument names will be checked with the set
 # naming style.
+#argument-rgx=
 argument-rgx=(([a-z][a-z0-9_]*)|(_[a-z0-9_]*))$
 
 # Naming style matching correct attribute names.
 attr-naming-style=snake_case
 
 # Regular expression matching correct attribute names. Overrides attr-naming-
 # style. If left empty, attribute names will be checked with the set naming
 # style.
+#attr-rgx=
 attr-rgx=(([a-z][a-z0-9_]*)|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma.
 bad-names=foo,
           bar,
           baz,
           toto,
@@ -302,14 +362,15 @@
 
 # Naming style matching correct class attribute names.
 class-attribute-naming-style=any
 
 # Regular expression matching correct class attribute names. Overrides class-
 # attribute-naming-style. If left empty, class attribute names will be checked
 # with the set naming style.
+#class-attribute-rgx=
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]*|(__.*__))$
 
 # Naming style matching correct class constant names.
 class-const-naming-style=UPPER_CASE
 
 # Regular expression matching correct class constant names. Overrides class-
 # const-naming-style. If left empty, class constant names will be checked with
@@ -317,34 +378,37 @@
 #class-const-rgx=
 
 # Naming style matching correct class names.
 class-naming-style=PascalCase
 
 # Regular expression matching correct class names. Overrides class-naming-
 # style. If left empty, class names will be checked with the set naming style.
+#class-rgx=
 class-rgx=[A-Z_][a-zA-Z0-9]+$
 
 # Naming style matching correct constant names.
 const-naming-style=UPPER_CASE
 
 # Regular expression matching correct constant names. Overrides const-naming-
 # style. If left empty, constant names will be checked with the set naming
 # style.
+#const-rgx=
 const-rgx=(([a-zA-Z_][a-zA-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
 # Naming style matching correct function names.
 function-naming-style=snake_case
 
 # Regular expression matching correct function names. Overrides function-
 # naming-style. If left empty, function names will be checked with the set
 # naming style.
+#function-rgx=
 function-rgx=[A-Z_][a-zA-Z0-9_]*$
 
 # Good variable names which should always be accepted, separated by a comma.
 good-names=i,
            j,
            k,
            ex,
@@ -360,28 +424,31 @@
 
 # Naming style matching correct inline iteration names.
 inlinevar-naming-style=any
 
 # Regular expression matching correct inline iteration names. Overrides
 # inlinevar-naming-style. If left empty, inline iteration names will be checked
 # with the set naming style.
+#inlinevar-rgx=
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
 # Naming style matching correct method names.
 method-naming-style=snake_case
 
 # Regular expression matching correct method names. Overrides method-naming-
 # style. If left empty, method names will be checked with the set naming style.
+#method-rgx=
 method-rgx=(test|[A-Z_])[a-zA-Z0-9_]*$
 
 # Naming style matching correct module names.
 module-naming-style=snake_case
 
 # Regular expression matching correct module names. Overrides module-naming-
 # style. If left empty, module names will be checked with the set naming style.
+#module-rgx=
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
 # Regular expression which should only match function or class names that do
@@ -399,26 +466,60 @@
 
 # Naming style matching correct variable names.
 variable-naming-style=snake_case
 
 # Regular expression matching correct variable names. Overrides variable-
 # naming-style. If left empty, variable names will be checked with the set
 # naming style.
+#variable-rgx=
 variable-rgx=(([a-z][a-z0-9_]*)|(_[a-z0-9_]*))$
 
 
+[EXCEPTIONS]
+
+# Exceptions that will emit a warning when caught.
+overgeneral-exceptions=BaseException,
+                       Exception
+
+
+[CLASSES]
+
+# Warn about protected attribute access inside special methods
+check-protected-access-in-special-methods=no
+
+# List of method names used to declare (i.e. assign) instance attributes.
+defining-attr-methods=__init__,
+                      __new__,
+                      setUp,
+                      __post_init__
+
+# List of member names, which should be excluded from the protected access
+# warning.
+exclude-protected=_asdict,
+                  _fields,
+                  _replace,
+                  _source,
+                  _make
+
+# List of valid names for the first argument in a class method.
+valid-classmethod-first-arg=cls
+
+# List of valid names for the first argument in a metaclass class method.
+valid-metaclass-classmethod-first-arg=cls
+
+
 [MISCELLANEOUS]
 
 # List of note tags to take in consideration, separated by a comma.
 notes=FIXME,
       XXX,
       TODO
 
 # Regular expression of note tags to take in consideration.
-#notes-rgx=
+notes-rgx=
 
 
 [FORMAT]
 
 # Expected format of line ending, e.g. empty (any line ending), LF or CRLF.
 expected-line-ending-format=
 
@@ -426,17 +527,19 @@
 ignore-long-lines=^\s*(# )?<?https?://\S+>?$
 
 # Number of spaces of indent required inside a hanging or continued line.
 indent-after-paren=4
 
 # String used as indentation unit. This is usually "    " (4 spaces) or "\t" (1
 # tab).
+# indent-string='    '
 indent-string='  '
 
 # Maximum number of characters on a single line.
+# max-line-length=100
 max-line-length=80
 
 # Maximum number of lines in a module.
 max-module-lines=1000
 
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
@@ -458,15 +561,15 @@
 # (hunspell), en_IE (hunspell), en_IN (hunspell), en_JM (hunspell), en_MW
 # (hunspell), en_NA (hunspell), en_NG (hunspell), en_NZ (hunspell), en_PH
 # (hunspell), en_SG (hunspell), en_TT (hunspell), en_US (hunspell), en_ZA
 # (hunspell), en_ZM (hunspell), en_ZW (hunspell).
 spelling-dict=
 
 # List of comma separated words that should be considered directives if they
-# appear and the beginning of a comment and should not be checked.
+# appear at the beginning of a comment and should not be checked.
 spelling-ignore-comment-directives=fmt: on,fmt: off,noqa:,noqa,nosec,isort:skip,mypy:
 
 # List of comma separated words that should not be checked.
 spelling-ignore-words=
 
 # A path to a file that contains the private dictionary; one word per line.
 spelling-private-dict-file=
@@ -481,18 +584,18 @@
 # Comments are removed from the similarity computation
 ignore-comments=yes
 
 # Docstrings are removed from the similarity computation
 ignore-docstrings=yes
 
 # Imports are removed from the similarity computation
-ignore-imports=no
+ignore-imports=yes
 
 # Signatures are removed from the similarity computation
-ignore-signatures=no
+ignore-signatures=yes
 
 # Minimum lines number of a similarity.
 min-similarity-lines=4
 
 
 [STRING]
 
@@ -501,97 +604,25 @@
 check-quote-consistency=no
 
 # This flag controls whether the implicit-str-concat should generate a warning
 # on implicit string concatenation in sequences defined over several lines.
 check-str-concat-over-line-jumps=no
 
 
-[DESIGN]
-
-# List of regular expressions of class ancestor names to ignore when counting
-# public methods (see R0903)
-exclude-too-few-public-methods=
-
-# List of qualified class names to ignore when counting class parents (see
-# R0901)
-ignored-parents=
-
-# Maximum number of arguments for function / method.
-max-args=10
-
-# Maximum number of attributes for a class (see R0902).
-max-attributes=7
-
-# Maximum number of boolean expressions in an if statement (see R0916).
-max-bool-expr=5
-
-# Maximum number of branch for function / method body.
-max-branches=12
-
-# Maximum number of locals for function / method body.
-max-locals=15
-
-# Maximum number of parents for a class (see R0901).
-max-parents=7
-
-# Maximum number of public methods for a class (see R0904).
-max-public-methods=20
-
-# Maximum number of return / yield for function / method body.
-max-returns=6
-
-# Maximum number of statements in function / method body.
-max-statements=50
-
-# Minimum number of public methods for a class (see R0903).
-min-public-methods=2
-
-
-[CLASSES]
-
-# Warn about protected attribute access inside special methods
-check-protected-access-in-special-methods=no
-
-# List of method names used to declare (i.e. assign) instance attributes.
-defining-attr-methods=__init__,
-                      __new__,
-                      setUp,
-                      __post_init__
-
-# List of member names, which should be excluded from the protected access
-# warning.
-exclude-protected=_asdict,
-                  _fields,
-                  _replace,
-                  _source,
-                  _make
-
-# List of valid names for the first argument in a class method.
-valid-classmethod-first-arg=cls
-
-# List of valid names for the first argument in a metaclass class method.
-valid-metaclass-classmethod-first-arg=cls
-
-
 [IMPORTS]
 
 # List of modules that can be imported at any level, not just the top level
 # one.
 allow-any-import-level=
 
 # Allow wildcard imports from modules that define __all__.
 allow-wildcard-with-all=no
 
-# Analyse import fallback blocks. This can be used to support both Python 2 and
-# 3 compatible code, which means that the block might have code that exists
-# only in one or another interpreter, leading to false positives when analysed.
-analyse-fallback-blocks=no
-
 # Deprecated modules which should not be used, separated by a comma.
-deprecated-modules=optparse,tkinter.tix
+deprecated-modules=
 
 # Output a graph (.gv or any supported image format) of external dependencies
 # to the given file (report RP0402 must not be disabled).
 ext-import-graph=
 
 # Output a graph (.gv or any supported image format) of all (i.e. internal and
 # external) dependencies to the given file (report RP0402 must not be
@@ -609,13 +640,17 @@
 # Force import order to recognize a module as part of a third party library.
 known-third-party=enchant
 
 # Couples of modules and preferred modules, separated by a comma.
 preferred-modules=
 
 
-[EXCEPTIONS]
+[REFACTORING]
 
-# Exceptions that will emit a warning when being caught. Defaults to
-# "BaseException, Exception".
-overgeneral-exceptions=BaseException,
-                       Exception
+# Maximum number of nested blocks for function / method body
+max-nested-blocks=5
+
+# Complete name of functions that never returns. When checking for
+# inconsistent-return-statements if a never returning function is called then
+# it will be considered as an explicit return statement and no message will be
+# printed.
+never-returning-functions=sys.exit,argparse.parse_error
```

### Comparing `artifacts-20221219/LICENSE` & `artifacts-20230413/LICENSE`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/MANIFEST.in` & `artifacts-20230413/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/PKG-INFO` & `artifacts-20230413/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artifacts
-Version: 20221219
+Version: 20230413
 Summary: ForensicArtifacts.com Artifact Repository.
 Home-page: https://github.com/ForensicArtifacts/artifacts
 Maintainer: Forensic artifacts
 Maintainer-email: forensicartifacts@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `artifacts-20221219/README.md` & `artifacts-20230413/README.md`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/appveyor.yml` & `artifacts-20230413/appveyor.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 environment:
   matrix:
-  - DESCRIPTION: "Windows with 32-bit Python 3.10"
+  - DESCRIPTION: "Windows with 32-bit Python 3.11"
     MACHINE_TYPE: "x86"
-    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2019
-    PYTHON: "C:\\Python310"
-    PYTHON_VERSION: "3.10"
+    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2022
+    PYTHON: "C:\\Python311"
+    PYTHON_VERSION: "3.11"
     L2TBINARIES_TRACK: "dev"
-  - DESCRIPTION: "Windows with 64-bit Python 3.10"
+  - DESCRIPTION: "Windows with 64-bit Python 3.11"
     MACHINE_TYPE: "amd64"
-    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2019
-    PYTHON: "C:\\Python310-x64"
-    PYTHON_VERSION: "3.10"
+    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2022
+    PYTHON: "C:\\Python311-x64"
+    PYTHON_VERSION: "3.11"
     L2TBINARIES_TRACK: "dev"
   - DESCRIPTION: "Mac OS with Python 3.11"
     APPVEYOR_BUILD_WORKER_IMAGE: macos-monterey
     HOMEBREW_NO_INSTALL_CLEANUP: 1
 
 install:
 - cmd: "%PYTHON%\\python.exe -m pip install -U pip setuptools twine wheel"
```

### Comparing `artifacts-20221219/artifacts/artifact.py` & `artifacts-20230413/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/artifacts/definitions.py` & `artifacts-20230413/artifacts/definitions.py`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/artifacts/reader.py` & `artifacts-20230413/artifacts/reader.py`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/artifacts/registry.py` & `artifacts-20230413/artifacts/registry.py`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/artifacts/source_type.py` & `artifacts-20230413/artifacts/source_type.py`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/artifacts/writer.py` & `artifacts-20230413/artifacts/writer.py`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/artifacts.egg-info/PKG-INFO` & `artifacts-20230413/artifacts.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artifacts
-Version: 20221219
+Version: 20230413
 Summary: ForensicArtifacts.com Artifact Repository.
 Home-page: https://github.com/ForensicArtifacts/artifacts
 Maintainer: Forensic artifacts
 Maintainer-email: forensicartifacts@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `artifacts-20221219/artifacts.egg-info/SOURCES.txt` & `artifacts-20230413/artifacts.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -42,24 +42,26 @@
 config/dpkg/clean
 config/dpkg/compat
 config/dpkg/control
 config/dpkg/copyright
 config/dpkg/python3-artifacts.install
 config/dpkg/rules
 config/dpkg/source/format
+data/.windows.yaml.swp
 data/antivirus.yaml
 data/applications.yaml
 data/cloud_services.yaml
 data/config_files.yaml
 data/containerd.yaml
 data/database_servers.yaml
 data/docker.yaml
 data/esxi.yaml
 data/file_systems.yaml
 data/hadoop.yaml
+data/ics.yaml
 data/installed_module_paths.yaml
 data/installed_modules.yaml
 data/instant_messaging.yaml
 data/java.yaml
 data/kaspersky_careto.yaml
 data/kubernetes.yaml
 data/legacy.yaml
```

### Comparing `artifacts-20221219/artifacts.ini` & `artifacts-20230413/artifacts.ini`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/config/appveyor/install.ps1` & `artifacts-20230413/config/appveyor/install.ps1`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # Script to set up tests on AppVeyor Windows.
 
 $Dependencies = "PyYAML"
-$Dependencies = ${Dependencies} -split " "
 
-$Output = Invoke-Expression -Command "git clone https://github.com/log2timeline/l2tdevtools.git ..\l2tdevtools 2>&1"
-Write-Host (${Output} | Out-String)
-
-If ($env:APPVEYOR_REPO_BRANCH -eq "main")
-{
-	$Track = "stable"
-}
-Else
+If ($Dependencies.Length -gt 0)
 {
-	$Track = $env:APPVEYOR_REPO_BRANCH
-}
-New-Item -ItemType "directory" -Name "dependencies"
+	$Dependencies = ${Dependencies} -split " "
 
-$env:PYTHONPATH = "..\l2tdevtools"
+	$Output = Invoke-Expression -Command "git clone https://github.com/log2timeline/l2tdevtools.git ..\l2tdevtools 2>&1" | %{ "$_" }
+	Write-Host (${Output} | Out-String)
 
-$Output = Invoke-Expression -Command "& '${env:PYTHON}\python.exe' ..\l2tdevtools\tools\update.py --download-directory dependencies --machine-type ${env:MACHINE_TYPE} --msi-targetdir ${env:PYTHON} --track ${env:L2TBINARIES_TRACK} ${Dependencies} 2>&1"
-Write-Host (${Output} | Out-String)
+	If ($env:APPVEYOR_REPO_BRANCH -eq "main")
+	{
+		$Track = "stable"
+	}
+	Else
+	{
+		$Track = $env:APPVEYOR_REPO_BRANCH
+	}
+	New-Item -ItemType "directory" -Name "dependencies"
+
+	$env:PYTHONPATH = "..\l2tdevtools"
+
+	$Output = Invoke-Expression -Command "& '${env:PYTHON}\python.exe' ..\l2tdevtools\tools\update.py --download-directory dependencies --machine-type ${env:MACHINE_TYPE} --msi-targetdir ${env:PYTHON} --track ${env:L2TBINARIES_TRACK} ${Dependencies} 2>&1" | %{ "$_" }
+	Write-Host (${Output} | Out-String)
+}
```

### Comparing `artifacts-20221219/config/appveyor/runtests.sh` & `artifacts-20230413/config/appveyor/runtests.sh`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/config/dpkg/control` & `artifacts-20230413/config/dpkg/control`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/config/dpkg/copyright` & `artifacts-20230413/config/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/antivirus.yaml` & `artifacts-20230413/data/antivirus.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/applications.yaml` & `artifacts-20230413/data/applications.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     paths:
     - '%%users.appdata%%\Microsoft\Word\**'
     - '%%users.appdata%%\Microsoft\Excel\**'
     - '%%users.appdata%%\Microsoft\Powerpoint\**'
     - '%%users.appdata%%\Microsoft\Publisher\**'
     separator: '\'
 supported_os: [Windows]
-urls: ['https://forensics.wiki/windows#microsoft_office_autosave']
+urls: ['https://forensics.wiki/windows#microsoft-office-autosave']
 ---
 name: MicrosoftOfficeMRU
 doc: Microsoft Office Most Recently Used
 sources:
 - type: FILE
   attributes:
     paths:
```

### Comparing `artifacts-20221219/data/cloud_services.yaml` & `artifacts-20230413/data/cloud_services.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -72,8 +72,8 @@
     - '%%users.localappdata%%\Microsoft\SkyDrive\setup\logs\*.log'
     - '%%users.localappdata%%\Microsoft\SkyDrive\settings\ApplicationSettings.xml'
     - '%%users.localappdata%%\Microsoft\SkyDrive\settings\*.dat'
     - '%%users.localappdata%%\Microsoft\SkyDrive\settings\*.ini'
     separator: '\'
   supported_os: [Windows]
 supported_os: [Windows]
-urls: ['https://forensics.wiki/one_drive#sky_drive_client']
+urls: ['https://forensics.wiki/one_drive#sky-drive-client']
```

### Comparing `artifacts-20221219/data/config_files.yaml` & `artifacts-20230413/data/config_files.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/containerd.yaml` & `artifacts-20230413/data/containerd.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/database_servers.yaml` & `artifacts-20230413/data/database_servers.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/docker.yaml` & `artifacts-20230413/data/docker.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/esxi.yaml` & `artifacts-20230413/data/esxi.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/file_systems.yaml` & `artifacts-20230413/data/file_systems.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/hadoop.yaml` & `artifacts-20230413/data/hadoop.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/installed_module_paths.yaml` & `artifacts-20230413/data/installed_module_paths.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/installed_modules.yaml` & `artifacts-20230413/data/installed_modules.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/instant_messaging.yaml` & `artifacts-20230413/data/instant_messaging.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 doc: Chat Sync Directory
 sources:
 - type: FILE
   attributes:
     paths: ['%%users.homedir%%/Library/Application Support/Skype/*/chatsync/*']
   supported_os: [Darwin]
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#skype']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#skype']
 ---
 name: SkypeDb
 doc: Main Skype database
 sources:
 - type: FILE
   attributes:
     paths: ['%%users.homedir%%/Library/Application Support/Skype/*/Main.db']
   supported_os: [Darwin]
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#skype']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#skype']
 ---
 name: SkypeMainDirectory
 doc: Skype Directory
 sources:
 - type: PATH
   attributes:
     paths: ['%%users.homedir%%/Library/Application Support/Skype/*']
@@ -33,25 +33,25 @@
 doc: Skype Preferences and Recent Searches
 sources:
 - type: FILE
   attributes:
     paths: ['%%users.homedir%%/Library/Preferences/com.skype.skype.plist']
   supported_os: [Darwin]
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#skype']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#skype']
 ---
 name: SkypeUserProfile
 doc: Skype User profile
 sources:
 - type: FILE
   attributes:
     paths: ['%%users.homedir%%/Library/Application Support/Skype/*/*']
   supported_os: [Darwin]
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#skype']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#skype']
 ---
 name: SignalApplicationContent
 doc: Signal Application Content and Configuration
 sources:
 - type: FILE
   attributes:
     paths:
```

### Comparing `artifacts-20221219/data/java.yaml` & `artifacts-20230413/data/java.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/kaspersky_careto.yaml` & `artifacts-20230413/data/kaspersky_careto.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/kubernetes.yaml` & `artifacts-20230413/data/kubernetes.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/legacy.yaml` & `artifacts-20230413/data/legacy.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/linux.yaml` & `artifacts-20230413/data/linux.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,15 @@
 name: LinuxAuthLogs
 doc: Linux authentication log files.
 sources:
 - type: FILE
   attributes:
     paths:
     - '/var/log/auth.log*'
-    - '/var/log/secure.log*'
+    - '/var/log/secure*'
 supported_os: [Linux]
 ---
 name: LinuxCACertificatesConfiguration
 doc: Linux CA Certificates configuration file.
 sources:
 - type: FILE
   attributes:
```

### Comparing `artifacts-20221219/data/linux_proc.yaml` & `artifacts-20230413/data/linux_proc.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/linux_services.yaml` & `artifacts-20230413/data/linux_services.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/macos.yaml` & `artifacts-20230413/data/macos.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -15,115 +15,119 @@
 sources:
 - type: FILE
   attributes:
     paths:
     - '/private/var/db/.AppleSetupDone'
     - '/var/db/.AppleSetupDone'
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#system_settings_and_informations']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-settings-and-informations']
 ---
 name: MacOSAppleSystemLogFile
 aliases: [MacOSAppleSystemLogFiles]
 doc: Apple system log (ASL) files.
 sources:
 - type: FILE
   attributes:
     paths:
     - '/private/var/log/asl/*.asl'
+    - '/private/var/log/DiagnosticMessages/*.asl'
     - '/var/log/asl/*.asl'
+    - '/var/log/DiagnosticMessages/*.asl'
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#system_logs']
+urls:
+- 'https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-logs'
+- 'https://support.apple.com/guide/console/reports-cnsl664be99a/mac'
 ---
 name: MacOSApplicationsDirectory
 aliases: [MacOSApplications]
 doc: Contents of the Applications directory.
 sources:
 - type: PATH
   attributes: {paths: ['/Applications/*']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#user_directories']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#user-directories']
 ---
 name: MacOSApplicationsRecentItems
 doc: Recent Items application specific
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Preferences/*.LSSharedFileList.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#recent_items']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#recent-items']
 ---
 name: MacOSAtJobs
 doc: MacOS at jobs
 sources:
 - type: FILE
   attributes: {paths: ['/usr/lib/cron/jobs/*']}
 supported_os: [Darwin]
 urls:
-- 'https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#system_info_misc'
+- 'https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-info-misc'
 - 'https://developer.apple.com/library/mac/documentation/Darwin/Reference/ManPages/man1/at.1.html#//apple_ref/doc/man/1/at'
 ---
 name: MacOSAuditLogFile
 aliases: [MacOSAuditLogFiles]
 doc: Audit log files.
 sources:
 - type: FILE
   attributes:
     paths:
     # Name of the file consists of "startime.stoptime" where each time is formatted as:
     # "YYYYMMDDhhmmss". For example: "20141130081343.20141130081943".
     - '/private/var/audit/[0-9]*.[0-9]*'
     - '/var/audit/[0-9]*.[0-9]*'
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#system_logs']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-logs']
 ---
 name: MacOSBluetoothPlistFile
 doc: Bluetooth preferences and paired device information property list (plist) file
 sources:
 - type: FILE
   attributes: {paths: ['/Library/Preferences/com.apple.Bluetooth.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#system_preferences']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-preferences']
 ---
 name: MacOSCoreAnalyticsFile
 aliases: [MacOSCoreAnalyticsFiles]
 doc: CoreAnalytics log files.
 sources:
 - type: FILE
   attributes:
     paths:
     - '/Library/Logs/DiagnosticReports/*.core_analytics'
     - '/private/var/db/analyticsd/aggregates/*'
     - '/var/db/analyticsd/aggregates/*'
 supported_os: [Darwin]
 urls:
-- 'https://forensics.wiki/mac_os_x#diagnostic_reports'
+- 'https://forensics.wiki/mac_os_x#diagnostic-reports'
 - 'https://www.crowdstrike.com/blog/i-know-what-you-did-last-month-a-new-artifact-of-execution-on-macos-10-13/'
 ---
 name: MacOSCronTabs
 doc: Cron tabs
 sources:
 - type: FILE
   attributes:
     paths:
     - '/etc/crontab'
     - '/private/etc/crontab'
     - '/usr/lib/cron/tabs/*'
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#system_info_misc']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-info-misc']
 ---
 name: MacOSDockConfigurationPlistFile
 aliases: [MacOSDock]
 doc: |
   Dock configuration property list (plist) file.
 
   This property list contains information about the configuration of a user's Dock.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Preferences/com.apple.Dock.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#preferences']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#preferences']
 ---
 name: MacOSDuetKnowledgeBase
 doc: KnowledgeC User and Application usage database.
 sources:
 - type: FILE
   attributes:
     paths:
@@ -147,98 +151,98 @@
   Global preferences property list (plist) file.
 
   This property list contains information about the system's locale and time zone.
 sources:
 - type: FILE
   attributes: {paths: ['/Library/Preferences/.GlobalPreferences.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#system_preferences']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-preferences']
 ---
 name: MacOSiCloudAccounts
 doc: iCloud Accounts
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Application Support/iCloud/Accounts/*']}
 supported_os: [Darwin]
 ---
 name: MacOSiCloudPreferences
 doc: iCloud user preferences
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Preferences/MobileMeAccounts.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#preferences']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#preferences']
 ---
 name: MacOSiDevices
 doc: Attached iDevices
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Preferences/com.apple.iPod.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#preferences']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#preferences']
 ---
 name: MacOSInstallationHistoryPlistFile
 aliases: [MacOSInstallationHistory]
 doc: Software installation history property list (plist) file.
 sources:
 - type: FILE
   attributes: {paths: ['/Library/Receipts/InstallHistory.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#software_installation']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#software-installation']
 ---
 name: MacOSInstallationLogFile
 doc: Software installation log file
 sources:
 - type: FILE
   attributes:
     paths:
     - '/private/var/log/install.log'
     - '/var/log/install.log'
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#system_logs']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-logs']
 ---
 name: MacOSiOSBackupInfo
 doc: iOS device backup information
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Application Support/MobileSync/Backup/*/info.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#idevice_backup']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#idevice-backup']
 ---
 name: MacOSiOSBackupManifest
 doc: iOS device backup apps information
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Application Support/MobileSync/Backup/*/Manifest.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#idevice_backup']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#idevice-backup']
 ---
 name: MacOSiOSBackupMbdb
 doc: iOS device backup files information
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Application Support/MobileSync/Backup/*/Manifest.mdbd']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#idevice_backup']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#idevice-backup']
 ---
 name: MacOSiOSBackupsMainDirectory
 doc: iOS device backups directory
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Application Support/MobileSync/Backup/*']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#idevice_backup']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#idevice-backup']
 ---
 name: MacOSiOSBackupStatus
 doc: iOS device backup status information.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Application Support/MobileSync/Backup/*/Status.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#idevice_backup']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#idevice-backup']
 ---
 name: MacOSKeyboardLayoutPlistFile
 doc: Keyboard layout property list (plist) file.
 sources:
 - type: FILE
   attributes: {paths: ['/Library/Preferences/com.apple.HIToolbox.plist']}
 supported_os: [Darwin]
@@ -249,15 +253,15 @@
 sources:
 - type: FILE
   attributes:
     paths:
     - '/Library/Extensions/*'
     - '/System/Library/Extensions/*'
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#kernel_extension']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#kernel-extension']
 ---
 name: MacOSLastlogFile
 doc: Lastlog file.
 sources:
 - type: FILE
   attributes:
     paths:
@@ -272,28 +276,28 @@
 - type: FILE
   attributes:
     paths:
     - '/Library/LaunchAgents/*.plist'
     - '/System/Library/LaunchAgents/*.plist'
     - '%%users.homedir%%/Library/LaunchAgents/*.plist'
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#autorun_locations']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#autorun-locations']
 ---
 name: MacOSLaunchDaemonsPlistFile
 aliases: [MacOSLaunchDaemonsPlistFiles]
 doc: Launch Daemons property list (plist) files.
 sources:
 - type: FILE
   attributes:
     paths:
     - '/Library/LaunchDaemons/*.plist'
     - '/System/Library/LaunchDaemons/*.plist'
     - '%%users.homedir%%/Library/LaunchDaemons/*.plist'
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#autorun_locations']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#autorun-locations']
 ---
 name: MacOSLoadedKexts
 doc: MacOS Loaded Kernel Extensions.
 sources:
 - type: COMMAND
   attributes:
     args: []
@@ -303,119 +307,119 @@
 name: MacOSLogFile
 aliases: [MacOSMiscLogs]
 doc: Miscellaneous system log files.
 sources:
 - type: FILE
   attributes: {paths: ['/Library/Logs/*']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#logs']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#logs']
 ---
 name: MacOSLoginWindowPlistFile
 doc: Log-in window information property list (plist) file
 sources:
 - type: FILE
   attributes: {paths: ['/Library/Preferences/com.apple.loginwindow.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#system_preferences']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-preferences']
 ---
 name: MacOSMailAccounts
 doc: Mail Accounts. Until now only V2, V3 and V5 have been observed.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Mail/V[0-9]/MailData/Accounts.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#mail']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#mail']
 ---
 name: MacOSMailBackupTOC
 doc: Mail Backup Table of Content. Until now only V2, V3 and V5 have been observed.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Mail/V[0-9]/MailData/BackupTOC.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#mail']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#mail']
 ---
 name: MacOSMailboxes
 doc: Mail Mailbox Directory. Until now only V2, V3 and V5 have been observed.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Mail/V[0-9]/Mailboxes/*']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#mail']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#mail']
 ---
 name: MacOSMailDownloadAttachments
 doc: Mail Downloads Directory
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Containers/com.apple.mail/Data/Library/Mail Downloads/*']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#mail']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#mail']
 ---
 name: MacOSMailEnvelopIndex
 doc: Mail Envelope Index. Until now only V2, V3 and V5 have been observed.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Mail/V[0-9]/MailData/Envelope Index']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#mail']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#mail']
 ---
 name: MacOSMailIMAP
 doc: Mail IMAP Synched Mailboxes. Until now only V2, V3 and V5 have been observed.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Mail/V[0-9]/IMAP-*/*']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#mail']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#mail']
 ---
 name: MacOSMailMainDirectory
 doc: Mail Main Folder. Until now only V2, V3 and V5 have been observed.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Mail/V[0-9]/*']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#mail']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#mail']
 ---
 name: MacOSMailOpenedAttachments
 doc: Mail Opened Attachments
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Mail/V[0-9]/MailData/OpenedAttachmentsV2.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#mail']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#mail']
 ---
 name: MacOSMailPOP
 doc: Mail POP Synched Mailboxes. Until now only V2, V3 and V5 have been observed.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Mail/V[0-9]/POP-*/*']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#mail']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#mail']
 ---
 name: MacOSMailPreferences
 doc: Mail Preferences
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Preferences/com.apple.Mail.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#mail']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#mail']
 ---
 name: MacOSMailRecentContacts
 doc: Mail Recent Contacts
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Application Support/AddressBook/MailRecents-v4.abcdmr']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#mail']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#mail']
 ---
 name: MacOSMailSignatures
 doc: Mail Signatures by Account. Until now only V2, V3 and V5 have been observed.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Mail/V[0-9]/MailData/Signatures/*']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#mail']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#mail']
 ---
 name: MacOSMountedDMGs
 doc: MacOS Mounted DMG files.
 sources:
 - type: COMMAND
   attributes:
     args: ['info']
@@ -462,38 +466,38 @@
     - '/private/etc/periodic/daily/*'
     - '/private/etc/periodic/monthly/*'
     - '/private/etc/periodic/weekly/*'
     - '/private/etc/weekly.local/*'
     - '/usr/local/etc/periodic/**2'
 supported_os: [Darwin]
 urls:
-- 'https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#system_info_misc'
+- 'https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-info-misc'
 - 'https://www.freebsd.org/cgi/man.cgi?periodic'
 - 'https://www.freebsd.org/cgi/man.cgi?periodic.conf'
 ---
 name: MacOSQuarantineEventsSQLiteDatabaseFile
 aliases: [MacOSQuarantineEvents]
 doc: Quarantine events SQLite database file.
 sources:
 - type: FILE
   attributes:
     paths:
     - '%%users.homedir%%/Library/Preferences/com.apple.LaunchServices.QuarantineEvents'
     - '%%users.homedir%%/Library/Preferences/com.apple.LaunchServices.QuarantineEventsV2'
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#preferences']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#preferences']
 ---
 name: MacOSRecentItemsPlistFile
 aliases: [MacOSRecentItems]
 doc: Recent items property list (plist) file.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Preferences/com.apple.recentitems.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#recent_items']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#recent-items']
 ---
 name: MacOSRemoteDesktopAdministratorSystem
 doc: Apple Remote Desktop (ARD) was first released in 2002 and is Apple’s desktop management system for software distribution, asset management, and remote assistance.
 sources:
 - type: FILE
   attributes:
     paths:
@@ -532,59 +536,59 @@
 sources:
 - type: FILE
   attributes:
     paths:
     - '%%users.homedir%%/Library/Preferences/com.apple.sidebarlists.plist'
     - '%%users.homedir%%/Preferences/com.apple.sidebarlists.plist'
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#preferences']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#preferences']
 ---
 name: MacOSSleepimageFile
 doc: Sleepimage file which contains the content of memory before going to sleep
 sources:
 - type: FILE
   attributes:
     paths:
     - '/private/var/vm/sleepimage'
     - '/var/vm/sleepimage'
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#sleep.2fhibernate_and_swap_image_file']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#sleep.2fhibernate-and-swap-image-file']
 ---
 name: MacOSSoftwareUpdatePreferencesPlistFile
 aliases: [MacOSUpdate]
 doc: Software update preferences property list (plist) files.
 sources:
 - type: FILE
   attributes: {paths: ['/Library/Preferences/com.apple.SoftwareUpdate.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#software_installation']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#software-installation']
 ---
 name: MacOSStartupItemsPlistFile
 aliases: [MacOSStartupItemsPlistFiles]
 doc: Startup Items property list (plist) files.
 sources:
 - type: FILE
   attributes:
     paths:
     - '/Library/StartupItems/*.plist'
     - '/System/Library/StartupItems/*.plist'
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#autorun_locations']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#autorun-locations']
 ---
 name: MacOSSwapFile
 aliases: [MacOSSwapFiles]
 doc: Swap files
 sources:
 - type: FILE
   attributes:
     paths:
     - '/private/var/vm/swapfile[0-9]'
     - '/var/vm/swapfile[0-9]'
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#sleep.2fhibernate_and_swap_image_file']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#sleep.2fhibernate-and-swap-image-file']
 ---
 name: MacOSSystemConfigurationPreferencesPlistFile
 doc: System configuration preferences property list (plist) file
 sources:
 - type: FILE
   attributes: {paths: ['/Library/Preferences/SystemConfiguration/preferences.plist']}
 supported_os: [Darwin]
@@ -595,32 +599,32 @@
 sources:
 - type: FILE
   attributes:
     paths:
     - '/private/var/log/*'
     - '/var/log/*'
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#system_logs']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-logs']
 ---
 name: MacOSSystemPreferencesPlistFile
 aliases: [MacOSSystemPreferencesPlistFiles]
 doc: System Preferences property list (plist) files
 sources:
 - type: FILE
   attributes: {paths: ['/Library/Preferences/**/*.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#system_preferences']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-preferences']
 ---
 name: MacOSSystemVersionPlistFile
 doc: Operating system name and version property list (plist) file
 sources:
 - type: FILE
   attributes: {paths: ['/System/Library/CoreServices/SystemVersion.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#system_settings_and_informations']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-settings-and-informations']
 ---
 name: MacOSTCCSQLiteDatabaseFile
 aliases: [MacOSTCC]
 doc: Transparency, Consent, Control (TCC) framework SQLite database files.
 sources:
 - type: FILE
   attributes:
@@ -632,15 +636,15 @@
 ---
 name: MacOSTimeMachinePlistFile
 doc: Time Machine information property list (plist) file
 sources:
 - type: FILE
   attributes: {paths: ['/Library/Preferences/com.apple.TimeMachine.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#system_preferences']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-preferences']
 ---
 name: MacOSUnifiedLogging
 doc: Apple Unified Logging and Activity Tracing
 sources:
 - type: FILE
   attributes:
     paths:
@@ -656,151 +660,151 @@
 name: MacOSUserApplicationLogFile
 aliases: [MacOSUserApplicationLogs]
 doc: User applications log files.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Logs/*.log']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#logs']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#logs']
 ---
 name: MacOSUserApplicationSupportDirectory
 aliases: [MacOSApplicationSupport]
 doc: Contents of the user Application Support directories.
 sources:
 - type: PATH
   attributes: {paths: ['%%users.homedir%%/Library/Application Support/*']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#misc']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#misc']
 ---
 name: MacOSUserDesktopDirectory
 doc: Contents of the user Desktop directories.
 sources:
 - type: PATH
   attributes: {paths: ['%%users.homedir%%/Desktop/*']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#user_directories']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#user-directories']
 ---
 name: MacOSUserDocumentsDirectory
 doc: Contents of the user Documents directories.
 sources:
 - type: PATH
   attributes: {paths: ['%%users.homedir%%/Documents/*']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#user_directories']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#user-directories']
 ---
 name: MacOSUserGlobalPreferencesPlistFile
 aliases: [MacOSUserGlobalPreferences]
 doc: User global preferences property list (plist) file.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Preferences/.GlobalPreferences.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#preferences']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#preferences']
 ---
 name: MacOSUserKeychainFile
 aliases: [MacOSKeychains]
 doc: User keychain files.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Keychains/*.keychain']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#misc']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#misc']
 ---
 name: MacOSUserLibraryDirectory
 doc: Contents of the user Library directories.
 sources:
 - type: PATH
   attributes: {paths: ['%%users.homedir%%/Library/*']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#user_directories']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#user-directories']
 ---
 name: MacOSUserLoginItemsPlistFile
 aliases: [MacOSUserLoginItems]
 doc: User login items property list (plist) file.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Preferences/com.apple.loginitems.plist']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#autorun_locations_2']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#autorun-locations-2']
 ---
 name: MacOSUserMoviesDirectory
 doc: Contents of the user Movies directories.
 sources:
 - type: PATH
   attributes: {paths: ['%%users.homedir%%/Movies/*']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#user_directories']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#user-directories']
 ---
 name: MacOSUserMusicDirectory
 doc: Contents of the user Music directories.
 sources:
 - type: PATH
   attributes: {paths: ['%%users.homedir%%/Music/*']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#user_directories']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#user-directories']
 ---
 name: MacOSUserPasswordHashesPlistFile
 aliases: [MacOSUserPasswordHashesPlistFiles]
 doc: User password hashes property list (plist) files.
 sources:
 - type: FILE
   attributes:
     paths:
     - '/private/var/db/dslocal/nodes/Default/users/*.plist'
     - '/var/db/dslocal/nodes/Default/users/*.plist'
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#system_settings_and_informations']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-settings-and-informations']
 ---
 name: MacOSUserPicturesDirectory
 doc: Contents of the user Pictures directories.
 sources:
 - type: PATH
   attributes: {paths: ['%%users.homedir%%/Pictures/*']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#user_directories']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#user-directories']
 ---
 name: MacOSUserPreferencesDirectory
 aliases: [MacOSUserPreferences]
 doc: Contents of the user Preferences directories.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Preferences/*']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#preferences']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#preferences']
 ---
 name: MacOSUserPublicDirectory
 doc: Contents of the user Public directories.
 sources:
 - type: PATH
   attributes: {paths: ['%%users.homedir%%/Public/*']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#user_directories']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#user-directories']
 ---
 name: MacOSUserAccountsSQLiteDatabaseFile
 aliases: [MacOSUserSocialAccounts]
 doc: User Accounts SQLite database files.
 sources:
 - type: FILE
   attributes:
     paths:
     - '%%users.homedir%%/Library/Accounts/Accounts3.sqlite'
     - '%%users.homedir%%/Library/Accounts/Accounts3.sqlite-wal'
     - '%%users.homedir%%/Library/Accounts/Accounts4.sqlite'
     - '%%users.homedir%%/Library/Accounts/Accounts4.sqlite-wal'
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#user.27s_accounts']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#user.27s-accounts']
 ---
 name: MacOSUserTrashDirectory
 aliases: [MacOSUserTrash]
 doc: Contents of the user Trash directories.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/.Trash/*']}
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#misc']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#misc']
 ---
 name: MacOSUtmpxFile
 doc: Utmpx login record file.
 sources:
 - type: FILE
   attributes:
     paths:
```

### Comparing `artifacts-20221219/data/shell.yaml` & `artifacts-20230413/data/shell.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/tomcat.yaml` & `artifacts-20230413/data/tomcat.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/triage.yaml` & `artifacts-20230413/data/triage.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/unix_common.yaml` & `artifacts-20230413/data/unix_common.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/user.yaml` & `artifacts-20230413/data/user.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 aliases: [MacOSUsers, MacOSUsersDirectory, OSXUsers, UserHomeDirectory]
 doc: Contents of the Users directory.
 sources:
 - type: PATH
   attributes: {paths: ['/Users/*']}
 supported_os: [Darwin]
 provides: [users.username]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#users']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#users']
 ---
 name: UserDownloadsDirectory
 aliases: [MacOSUserDownloadsDirectory, UserDownloads, WindowsUserDownloadsDirectory]
 doc: Contents of user Downloads directories.
 sources:
 - type: PATH
   attributes:
@@ -20,8 +20,8 @@
   supported_os: [Darwin, Linux]
 - type: PATH
   attributes:
     paths: ['%%users.userprofile%%\Downloads\*']
     separator: '\'
   supported_os: [Windows]
 supported_os: [Darwin, Linux, Windows]
-urls: ['https://forensics.wiki/mac_os_x_10.9_-_artifacts_location#user_directories']
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#user-directories']
```

### Comparing `artifacts-20221219/data/webbrowser.yaml` & `artifacts-20230413/data/webbrowser.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -64,25 +64,29 @@
   * PNaCl translation cache
 sources:
 - type: FILE
   attributes:
     paths:
     - '%%users.localappdata%%\Google\Chrome\User Data\*\Application Cache\Cache\*'
     - '%%users.localappdata%%\Google\Chrome\User Data\*\Cache\*'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\Cache\Cache_Data\*'
     - '%%users.localappdata%%\Google\Chrome\User Data\*\Media Cache\*'
     - '%%users.localappdata%%\Google\Chrome\User Data\*\GPUCache\*'
     - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Application Cache\Cache\*'
     - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Cache\*'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Cache\Cache_Data\*'
     - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Media Cache\*'
     - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\GPUCache\*'
     - '%%users.localappdata%%\Chromium\User Data\*\Application Cache\Cache\*'
     - '%%users.localappdata%%\Chromium\User Data\*\Cache\*'
+    - '%%users.localappdata%%\Chromium\User Data\*\Cache\Cache_Data\*'
     - '%%users.localappdata%%\Chromium\User Data\*\Media Cache\*'
     - '%%users.localappdata%%\Chromium\User Data\*\GPUCache\*'
     - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Cache\*'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Cache\Cache_Data\*'
     - '%%users.localappdata%%\Microsoft\Edge\User Data\*\GPUCache\*'
     separator: '\'
   supported_os: [Windows]
 - type: FILE
   attributes:
     paths:
     - '%%users.homedir%%/Caches/Google/Chrome/*/Cache/*'
@@ -103,46 +107,56 @@
     - '%%users.homedir%%/Library/Application Support/Chromium/*/Application Cache/Cache/*'
     - '%%users.homedir%%/Library/Application Support/Chromium/*/GPUCache/*'
     - '%%users.homedir%%/Library/Caches/Chromium/PnaclTranslationCache/*'
   supported_os: [Darwin]
 - type: FILE
   attributes:
     paths:
+    - '%%users.homedir%%/.cache/BraveSoftware/Brave-Browser/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.cache/google-chrome/Cache/*'
     - '%%users.homedir%%/.cache/google-chrome/*/Cache/*'
+    - '%%users.homedir%%/.cache/google-chrome/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.cache/google-chrome/*/Media Cache/*'
     - '%%users.homedir%%/.cache/google-chrome/PnaclTranslationCache/*'
     - '%%users.homedir%%/.config/google-chrome/*/Application Cache/*'
     - '%%users.homedir%%/.config/google-chrome/*/Cache/*'
+    - '%%users.homedir%%/.config/google-chrome/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.config/google-chrome/*/Media Cache/*'
     - '%%users.homedir%%/.config/google-chrome/*/GPUCache/*'
     - '%%users.homedir%%/.cache/chromium/Cache/*'
     - '%%users.homedir%%/.cache/chromium/*/Cache/*'
+    - '%%users.homedir%%/.cache/chromium/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.cache/chromium/*/Media Cache/*'
     - '%%users.homedir%%/.cache/chromium/PnaclTranslationCache/*'
     - '%%users.homedir%%/.config/chromium/*/Application Cache/*'
     - '%%users.homedir%%/.config/chromium/*/Cache/*'
+    - '%%users.homedir%%/.config/chromium/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.config/chromium/*/Media Cache/*'
     - '%%users.homedir%%/.config/chromium/*/GPUCache/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-profile/Cache/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-profile/*/Cache/*'
+    - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-profile/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-profile/*/Media Cache/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-profile/PnaclTranslationCache/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-config/google-chrome/Cache/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-config/google-chrome/*/Cache/*'
+    - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-config/google-chrome/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-config/google-chrome/*/Media Cache/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-config/google-chrome/PnaclTranslationCache/*'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Application Cache/*'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Cache/*'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Media Cache/*'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/GPUCache/*'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Application Cache/*'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Cache/*'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Media Cache/*'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/GPUCache/*'
+    - '%%users.homedir%%/.cache/microsoft-edge/*/Cache/Cache_Data/*'
   supported_os: [Linux]
 supported_os: [Darwin, Linux, Windows]
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/webbrowser/ChromeCache.html']
 ---
 name: ChromiumBasedBrowsersCache
 doc: |
   Caches of multiple Chromium-based browsers (Google Chrome, Brave, Chromium,
@@ -155,46 +169,61 @@
   * PNaCl translation cache
 sources:
 - type: FILE
   attributes:
     paths:
     - '%%users.appdata%%\Brave\*\Application Cache\Cache\*'
     - '%%users.appdata%%\Brave\*\Cache\*'
+    - '%%users.appdata%%\Brave\*\Cache\Cache_Data\*'
     - '%%users.appdata%%\Brave\*\GPUCache\*'
     - '%%users.appdata%%\Brave\*\Media Cache\*'
     - '%%users.appdata%%\Opera Software\Opera Stable\*\Application Cache\Cache\*'
     - '%%users.appdata%%\Opera Software\Opera Stable\*\Cache\*'
+    - '%%users.appdata%%\Opera Software\Opera Stable\*\Cache\Cache_Data\*'
     - '%%users.appdata%%\Opera Software\Opera Stable\*\GPUCache\*'
     - '%%users.appdata%%\Opera Software\Opera Stable\*\Media Cache\*'
+    - '%%users.localappdata%%\BraveSoftware\Brave-Browser\User Data\*\Application Cache\Cache\*'
+    - '%%users.localappdata%%\BraveSoftware\Brave-Browser\User Data\*\Cache\*'
+    - '%%users.localappdata%%\BraveSoftware\Brave-Browser\User Data\*\Cache\Cache_Data\*'
+    - '%%users.localappdata%%\BraveSoftware\Brave-Browser\User Data\*\GPUCache\*'
+    - '%%users.localappdata%%\BraveSoftware\Brave-Browser\User Data\*\Media Cache\*'
     - '%%users.localappdata%%\Chromium\*\Application Cache\Cache\*'
     - '%%users.localappdata%%\Chromium\*\Cache\*'
+    - '%%users.localappdata%%\Chromium\*\Cache\Cache_Data\*'
     - '%%users.localappdata%%\Chromium\*\GPUCache\*'
     - '%%users.localappdata%%\Chromium\*\Media Cache\*'
     - '%%users.localappdata%%\Chromium\User Data\*\Application Cache\Cache\*'
     - '%%users.localappdata%%\Chromium\User Data\*\Cache\*'
+    - '%%users.localappdata%%\Chromium\User Data\*\Cache\Cache_Data\*'
     - '%%users.localappdata%%\Chromium\User Data\*\GPUCache\*'
     - '%%users.localappdata%%\Chromium\User Data\*\Media Cache\*'
     - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Application Cache\Cache\*'
     - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Cache\*'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Cache\Cache_Data\*'
     - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\GPUCache\*'
     - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Media Cache\*'
     - '%%users.localappdata%%\Google\Chrome\User Data\*\Application Cache\Cache\*'
     - '%%users.localappdata%%\Google\Chrome\User Data\*\Cache\*'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\Cache\Cache_Data\*'
     - '%%users.localappdata%%\Google\Chrome\User Data\*\GPUCache\*'
     - '%%users.localappdata%%\Google\Chrome\User Data\*\Media Cache\*'
     - '%%users.localappdata%%\Microsoft\Edge Beta\User Data\*\Application Cache\Cache\*'
     - '%%users.localappdata%%\Microsoft\Edge Beta\User Data\*\Cache\*'
+    - '%%users.localappdata%%\Microsoft\Edge Beta\User Data\*\Cache\Cache_Data\*'
     - '%%users.localappdata%%\Microsoft\Edge Beta\User Data\*\GPUCache\*'
     - '%%users.localappdata%%\Microsoft\Edge Beta\User Data\*\Media Cache\*'
     - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Application Cache\Cache\*'
     - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Cache\*'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Cache\Cache_Data\*'
     - '%%users.localappdata%%\Microsoft\Edge\User Data\*\GPUCache\*'
     - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Media Cache\*'
+    - '%%users.localappdata%%\Opera Software\Opera Stable\*\Cache_Data\*'
     - '%%users.localappdata%%\Yandex\YandexBrowser\User Data\*\Application Cache\Cache\*'
     - '%%users.localappdata%%\Yandex\YandexBrowser\User Data\*\Cache\*'
+    - '%%users.localappdata%%\Yandex\YandexBrowser\User Data\*\Cache\Cache_Data\*'
     - '%%users.localappdata%%\Yandex\YandexBrowser\User Data\*\GPUCache\*'
     - '%%users.localappdata%%\Yandex\YandexBrowser\User Data\*\Media Cache\*'
     separator: '\'
   supported_os: [Windows]
 - type: FILE
   attributes:
     paths:
@@ -263,30 +292,37 @@
     - '%%users.homedir%%/Library/Caches/Google/Chrome/*/Media Cache/*'
     - '%%users.homedir%%/Library/Caches/Google/Chrome/Cache/*'
     - '%%users.homedir%%/Library/Caches/Google/Chrome/PnaclTranslationCache/*'
   supported_os: [Darwin]
 - type: FILE
   attributes:
     paths:
+    - '%%users.homedir%%/.cache/BraveSoftware/Brave-Browser/Cache/Cache_Data/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-config/google-chrome/*/Cache/*'
+    - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-config/google-chrome/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-config/google-chrome/*/Media Cache/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-config/google-chrome/Cache/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-config/google-chrome/PnaclTranslationCache/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-profile/*/Cache/*'
+    - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-profile/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-profile/*/Media Cache/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-profile/Cache/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-profile/PnaclTranslationCache/*'
     - '%%users.homedir%%/.cache/chromium/*/Cache/*'
+    - '%%users.homedir%%/.cache/chromium/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.cache/chromium/*/Media Cache/*'
     - '%%users.homedir%%/.cache/chromium/Cache/*'
     - '%%users.homedir%%/.cache/chromium/PnaclTranslationCache/*'
     - '%%users.homedir%%/.cache/google-chrome/*/Cache/*'
+    - '%%users.homedir%%/.cache/google-chrome/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.cache/google-chrome/*/Media Cache/*'
     - '%%users.homedir%%/.cache/google-chrome/Cache/*'
     - '%%users.homedir%%/.cache/google-chrome/PnaclTranslationCache/*'
+    - '%%users.homedir%%/.cache/microsoft-edge/*/Cache/Cache_Data/*'
+    - '%%users.homedir%%/.cache/opera/*/Cache_Data/*'
     - '%%users.homedir%%/.config/BraveSoftware/Brave-Browser/*/Application Cache/*'
     - '%%users.homedir%%/.config/BraveSoftware/Brave-Browser/*/Cache/*'
     - '%%users.homedir%%/.config/BraveSoftware/Brave-Browser/*/GPUCache/*'
     - '%%users.homedir%%/.config/BraveSoftware/Brave-Browser/*/Media Cache/*'
     - '%%users.homedir%%/.config/BraveSoftware/Brave-Browser/Cache/*'
     - '%%users.homedir%%/.config/BraveSoftware/Brave-Browser/PnaclTranslationCache/*'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Application Cache/*'
@@ -315,19 +351,21 @@
     - '%%users.homedir%%/.config/google-chrome-beta/PnaclTranslationCache/*'
     - '%%users.homedir%%/.config/google-chrome/*/Application Cache/*'
     - '%%users.homedir%%/.config/google-chrome/*/Cache/*'
     - '%%users.homedir%%/.config/google-chrome/*/GPUCache/*'
     - '%%users.homedir%%/.config/google-chrome/*/Media Cache/*'
     - '%%users.homedir%%/.config/google-chrome/Cache/*'
     - '%%users.homedir%%/.config/google-chrome/PnaclTranslationCache/*'
+    - '%%users.homedir%%/.config/microsoft-edge/*/GPUCache/*'
     - '%%users.homedir%%/.config/opera/*/Application Cache/*'
     - '%%users.homedir%%/.config/opera/*/Cache/*'
     - '%%users.homedir%%/.config/opera/*/GPUCache/*'
     - '%%users.homedir%%/.config/opera/*/Media Cache/*'
     - '%%users.homedir%%/.config/opera/Cache/*'
+    - '%%users.homedir%%/.config/opera/GPUCache/*'
     - '%%users.homedir%%/.config/opera/PnaclTranslationCache/*'
     - '%%users.homedir%%/.config/yandex-browser-beta/*/Application Cache/*'
     - '%%users.homedir%%/.config/yandex-browser-beta/*/Cache/*'
     - '%%users.homedir%%/.config/yandex-browser-beta/*/GPUCache/*'
     - '%%users.homedir%%/.config/yandex-browser-beta/*/Media Cache/*'
     - '%%users.homedir%%/.config/yandex-browser-beta/Cache/*'
     - '%%users.homedir%%/.config/yandex-browser-beta/PnaclTranslationCache/*'
@@ -343,33 +381,41 @@
 ---
 name: ChromeCookies
 doc: Chrome Cookies database.
 sources:
 - type: FILE
   attributes:
     paths:
+    - '%%users.localappdata%%\BraveSoftware\Brave-Browser\User Data\*\Network\Cookies'
+    - '%%users.localappdata%%\BraveSoftware\Brave-Browser\User Data\*\Network\Cookies-journal'
     - '%%users.localappdata%%\Chromium\User Data\*\Cookies'
     - '%%users.localappdata%%\Chromium\User Data\*\Cookies-journal'
     - '%%users.localappdata%%\Chromium\User Data\*\Network\Cookies'
     - '%%users.localappdata%%\Chromium\User Data\*\Network\Cookies-journal'
     - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Cookies'
     - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Cookies-journal'
     - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Network\Cookies'
     - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Network\Cookies-journal'
     - '%%users.localappdata%%\Google\Chrome\User Data\*\Cookies'
     - '%%users.localappdata%%\Google\Chrome\User Data\*\Cookies-journal'
     - '%%users.localappdata%%\Google\Chrome\User Data\*\Network\Cookies'
     - '%%users.localappdata%%\Google\Chrome\User Data\*\Network\Cookies-journal'
     - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Cookies'
     - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Cookies-journal'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Network\Cookies'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Network\Cookies-journal'
+    - '%%users.appdata%%\Opera Software\Opera Stable\Network\Cookies'
+    - '%%users.appdata%%\Opera Software\Opera Stable\Network\Cookies-journal'
     separator: '\'
   supported_os: [Windows]
 - type: FILE
   attributes:
     paths:
+    - '%%users.homedir%%/.config/BraveSoftware/Brave-Browser/*/Cookies'
+    - '%%users.homedir%%/.config/BraveSoftware/Brave-Browser/*/Cookies-journal'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Cookies'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Cookies-journal'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Network/Cookies'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Network/Cookies-journal'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Cookies'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Cookies-journal'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Network/Cookies'
@@ -382,14 +428,18 @@
     - '%%users.homedir%%/.config/google-chrome-beta/*/Cookies-journal'
     - '%%users.homedir%%/.config/google-chrome-beta/*/Network/Cookies'
     - '%%users.homedir%%/.config/google-chrome-beta/*/Network/Cookies-journal'
     - '%%users.homedir%%/.config/google-chrome/*/Cookies'
     - '%%users.homedir%%/.config/google-chrome/*/Cookies-journal'
     - '%%users.homedir%%/.config/google-chrome/*/Network/Cookies'
     - '%%users.homedir%%/.config/google-chrome/*/Network/Cookies-journal'
+    - '%%users.homedir%%/.config/microsoft-edge/*/Cookies'
+    - '%%users.homedir%%/.config/microsoft-edge/*/Cookies-journal'
+    - '%%users.homedir%%/.config/opera/Cookies'
+    - '%%users.homedir%%/.config/opera/Cookies-journal'
   supported_os: [Linux]
 - type: FILE
   attributes:
     paths:
     - '%%users.homedir%%/Library/Application Support/Chromium/*/Cookies'
     - '%%users.homedir%%/Library/Application Support/Chromium/*/Cookies-journal'
     - '%%users.homedir%%/Library/Application Support/Chromium/*/Network/Cookies'
@@ -448,16 +498,16 @@
     - '%%users.localappdata%%\Microsoft\Edge Beta\User Data\*\Extensions\**10'
     - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Extensions\**10'
     - '%%users.localappdata%%\Yandex\YandexBrowser\User Data\*\Extensions\**10'
     separator: '\'
   supported_os: [Windows]
 supported_os: [Darwin, Linux, Windows]
 urls:
+- 'https://forensics.wiki/google_chrome#chromium-based-browsers'
 - 'https://forensics.wiki/google_chrome#extensions'
-- 'https://forensics.wiki/google_chrome#chromium-based_browsers'
 ---
 name: ChromiumBasedBrowsersExtensionActivitySQLiteDatabaseFile
 aliases: [ChromeExtensionActivity, ChromiumBasedBrowsersExtensionActivity]
 doc: |
   Browser Extension Activity SQLite database file for Chromium-based browsers,
   such as Google Chrome, Brave, Chromium, Yandex, Opera, Edge, EdgeBeta.
 sources:
@@ -498,16 +548,16 @@
     - '%%users.localappdata%%\Microsoft\Edge Beta\User Data\*\Extension Activity'
     - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Extension Activity'
     - '%%users.localappdata%%\Yandex\YandexBrowser\User Data\*\Extension Activity'
     separator: '\'
   supported_os: [Windows]
 supported_os: [Darwin, Linux, Windows]
 urls:
-- 'https://forensics.wiki/google_chrome#extension_activity_database'
-- 'https://forensics.wiki/google_chrome#chromium-based_browsers'
+- 'https://forensics.wiki/google_chrome#chromium-based-browsers'
+- 'https://forensics.wiki/google_chrome#extension-activity-database'
 ---
 name: ChromeExtensionRegistryKeys
 doc: Chrome extensions installed by writing windows registry keys.
 sources:
 - type: REGISTRY_KEY
   attributes:
     keys:
@@ -621,14 +671,18 @@
     - '%%users.homedir%%/.config/google-chrome-beta/*/Archived History-journal'
     - '%%users.homedir%%/.config/google-chrome-beta/*/History'
     - '%%users.homedir%%/.config/google-chrome-beta/*/History-journal'
     - '%%users.homedir%%/.config/google-chrome/*/Archived History'
     - '%%users.homedir%%/.config/google-chrome/*/Archived History-journal'
     - '%%users.homedir%%/.config/google-chrome/*/History'
     - '%%users.homedir%%/.config/google-chrome/*/History-journal'
+    - '%%users.homedir%%/.config/microsoft-edge/*/Archived History'
+    - '%%users.homedir%%/.config/microsoft-edge/*/Archived History-journal'
+    - '%%users.homedir%%/.config/microsoft-edge/*/History'
+    - '%%users.homedir%%/.config/microsoft-edge/*/History-journal'
     - '%%users.homedir%%/.config/opera/*/Archived History'
     - '%%users.homedir%%/.config/opera/*/Archived History-journal'
     - '%%users.homedir%%/.config/opera/*/History'
     - '%%users.homedir%%/.config/opera/*/History-journal'
     - '%%users.homedir%%/.config/yandex-browser-beta/*/Archived History'
     - '%%users.homedir%%/.config/yandex-browser-beta/*/Archived History-journal'
     - '%%users.homedir%%/.config/yandex-browser-beta/*/History'
@@ -641,14 +695,16 @@
 - type: FILE
   attributes:
     paths:
     - '%%users.appdata%%\Brave\*\Archived History'
     - '%%users.appdata%%\Brave\*\Archived History-journal'
     - '%%users.appdata%%\Brave\*\History'
     - '%%users.appdata%%\Brave\*\History-journal'
+    - '%%users.appdata%%\BraveSoftware\Brave-Browser\User Data\*\History'
+    - '%%users.appdata%%\BraveSoftware\Brave-Browser\User Data\*\History-journal'
     - '%%users.appdata%%\Opera Software\Opera Stable\*\Archived History'
     - '%%users.appdata%%\Opera Software\Opera Stable\*\Archived History-journal'
     - '%%users.appdata%%\Opera Software\Opera Stable\*\History'
     - '%%users.appdata%%\Opera Software\Opera Stable\*\History-journal'
     - '%%users.localappdata%%\Chromium\*\Archived History'
     - '%%users.localappdata%%\Chromium\*\Archived History-journal'
     - '%%users.localappdata%%\Chromium\*\History'
@@ -678,15 +734,15 @@
     - '%%users.localappdata%%\Yandex\YandexBrowser\User Data\*\History'
     - '%%users.localappdata%%\Yandex\YandexBrowser\User Data\*\History-journal'
     separator: '\'
   supported_os: [Windows]
 supported_os: [Darwin, Linux, Windows]
 urls:
 - 'https://forensics.wiki/google_chrome'
-- 'https://forensics.wiki/google_chrome#chromium-based_browsers'
+- 'https://forensics.wiki/google_chrome#chromium-based-browsers'
 ---
 name: ChromeIndexedDB
 doc: |
   Google Chrome, Canary and Chromium IndexedDB files.
 
   The IndexedDB directory contains one directory per origin that uses
   IndexedDB, named like https_www.example.com_0.indexeddb.leveldb,
@@ -876,22 +932,38 @@
   attributes:
     paths:
     - '%%users.homedir%%/.mozilla/firefox/*.default/Cache/*'
     - '%%users.homedir%%/.cache/mozilla/firefox/*.default/Cache/*'
     - '%%users.homedir%%/.cache/mozilla/firefox/*.default/cache2/*'
     - '%%users.homedir%%/.cache/mozilla/firefox/*.default/cache2/doomed/*'
     - '%%users.homedir%%/.cache/mozilla/firefox/*.default/cache2/entries/*'
+    - '%%users.homedir%%/.cache/mozilla/firefox/*.default-*/Cache/*'
+    - '%%users.homedir%%/.cache/mozilla/firefox/*.default-*/cache2/*'
+    - '%%users.homedir%%/.cache/mozilla/firefox/*.default-*/cache2/doomed/*'
+    - '%%users.homedir%%/.cache/mozilla/firefox/*.default-*/cache2/entries/*'
+    - '%%users.homedir%%/snap/firefox/common/.cache/mozilla/firefox/*.default/Cache/*'
+    - '%%users.homedir%%/snap/firefox/common/.cache/mozilla/firefox/*.default/cache2/*'
+    - '%%users.homedir%%/snap/firefox/common/.cache/mozilla/firefox/*.default/cache2/doomed/*'
+    - '%%users.homedir%%/snap/firefox/common/.cache/mozilla/firefox/*.default/cache2/entries/*'
+    - '%%users.homedir%%/snap/firefox/common/.cache/mozilla/firefox/*.default-*/Cache/*'
+    - '%%users.homedir%%/snap/firefox/common/.cache/mozilla/firefox/*.default-*/cache2/*'
+    - '%%users.homedir%%/snap/firefox/common/.cache/mozilla/firefox/*.default-*/cache2/doomed/*'
+    - '%%users.homedir%%/snap/firefox/common/.cache/mozilla/firefox/*.default-*/cache2/entries/*'
   supported_os: [Linux]
 - type: FILE
   attributes:
     paths:
     - '%%users.localappdata%%\Mozilla\Firefox\Profiles\*.default\Cache\*'
     - '%%users.localappdata%%\Mozilla\Firefox\Profiles\*.default\cache2\*'
     - '%%users.localappdata%%\Mozilla\Firefox\Profiles\*.default\cache2\doomed\*'
     - '%%users.localappdata%%\Mozilla\Firefox\Profiles\*.default\cache2\entries\*'
+    - '%%users.localappdata%%\Mozilla\Firefox\Profiles\*.default-*\Cache\*'
+    - '%%users.localappdata%%\Mozilla\Firefox\Profiles\*.default-*\cache2\*'
+    - '%%users.localappdata%%\Mozilla\Firefox\Profiles\*.default-*\cache2\doomed\*'
+    - '%%users.localappdata%%\Mozilla\Firefox\Profiles\*.default-*\cache2\entries\*'
     separator: '\'
   supported_os: [Windows]
 supported_os: [Darwin, Linux, Windows]
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/webbrowser/FirefoxCache.html']
 ---
 name: FirefoxDownloads
 doc: Firefox browser downloads (downloads.sqlite).
@@ -930,14 +1002,16 @@
     - '%%users.homedir%%/Library/Application Support/Firefox/Profiles/*/places.sqlite-wal'
   supported_os: [Darwin]
 - type: FILE
   attributes:
     paths:
     - '%%users.homedir%%/.mozilla/firefox/*/places.sqlite'
     - '%%users.homedir%%/.mozilla/firefox/*/places.sqlite-wal'
+    - '%%users.homedir%%/snap/firefox/common/.mozilla/firefox/*/places.sqlite'
+    - '%%users.homedir%%/snap/firefox/common/.mozilla/firefox/*/places.sqlite-wal'
   supported_os: [Linux]
 - type: FILE
   attributes:
     paths:
     - '%%users.localappdata%%\Mozilla\Firefox\Profiles\*\places.sqlite'
     - '%%users.localappdata%%\Mozilla\Firefox\Profiles\*\places.sqlite-wal'
     - '%%users.appdata%%\Mozilla\Firefox\Profiles\*\places.sqlite'
@@ -1129,15 +1203,15 @@
 ---
 name: InternetExplorerTypedURLsKeys
 doc: Microsoft Internet Explorer TypedUrls keys.
 sources:
 - type: REGISTRY_KEY
   attributes: {keys: ['HKEY_USERS\%%users.sid%%\Software\Microsoft\Internet Explorer\TypedURLs\*']}
 supported_os: [Windows]
-urls: ['https://forensics.wiki/internet_explorer#typed_urls']
+urls: ['https://forensics.wiki/internet_explorer#typed-urls']
 ---
 name: OperaHistoryFile
 aliases: [OperaHistory]
 doc: Opera browser history (global_history.dat) file.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Opera/global_history.dat']}
@@ -1146,14 +1220,15 @@
   attributes: {paths: ['%%users.homedir%%/.opera/global_history.dat']}
   supported_os: [Linux]
 - type: FILE
   attributes:
     paths:
     - '%%users.appdata%%\Opera\Opera\global_history.dat'
     - '%%users.appdata%%\Opera Software\Opera Stable\History'
+    - '%%users.appdata%%\Opera Software\Opera Stable\History-journal'
     separator: '\'
   supported_os: [Windows]
 supported_os: [Darwin, Linux, Windows]
 urls: ['https://forensics.wiki/opera']
 ---
 name: SafariCacheSQLiteDatabaseFile
 aliases: [SafariCache]
```

### Comparing `artifacts-20221219/data/webservers.yaml` & `artifacts-20230413/data/webservers.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/windows.yaml` & `artifacts-20230413/data/windows.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -602,15 +602,15 @@
     - '%%environ_systemroot%%\System32\config\systemprofile\AppData\Local\Temp\*.dmp'
     - '%%environ_systemroot%%\Temp\*.dmp'
     - '%%users.localappdata%%\CrashDumps\**'
     - '%%users.localappdata%%\Microsoft\Windows\WER\**'
     - '%%users.localappdata%%\Temp\*.dmp'
     separator: '\'
 supported_os: [Windows]
-urls: ['https://forensics.wiki/windows#crash_and_minidumps']
+urls: ['https://forensics.wiki/windows#crash-and-minidumps']
 ---
 name: WindowsCredentialProviderFilters
 doc: Windows Credential Provider Filters
 sources:
 - type: REGISTRY_KEY
   attributes:
     keys:
@@ -646,15 +646,15 @@
   attributes:
     paths:
     - '%%environ_systemroot%%\System32\config\systemprofile\AppData\LocalLow\Microsoft\CryptnetUrlCache\MetaData\*'
     - '%%environ_systemroot%%\SysWOW64\config\systemprofile\AppData\LocalLow\Microsoft\CryptnetUrlCache\MetaData\*'
     - '%%users.userprofile%%\AppData\LocalLow\Microsoft\CryptnetUrlCache\MetaData\*'
     separator: '\'
 supported_os: [Windows]
-urls: ['https://forensics.wiki/windows#cryptnet_url_cache']
+urls: ['https://forensics.wiki/windows#cryptnet-url-cache']
 ---
 name: WindowsCryptnetUrlCacheContent
 doc: |
   Content of a Windows cache of files downloaded from the internet.
 
   Helpful when investigating the use of "Living of the Land" tools that allow
   attackers to download arbitrary files from the internet, such as
@@ -664,15 +664,15 @@
   attributes:
     paths:
     - '%%environ_systemroot%%\System32\config\systemprofile\AppData\LocalLow\Microsoft\CryptnetUrlCache\Content\*'
     - '%%environ_systemroot%%\SysWOW64\config\systemprofile\AppData\LocalLow\Microsoft\CryptnetUrlCache\Content\*'
     - '%%users.userprofile%%\AppData\LocalLow\Microsoft\CryptnetUrlCache\Content\*'
     separator: '\'
 supported_os: [Windows]
-urls: ['https://forensics.wiki/windows#cryptnet_url_cache']
+urls: ['https://forensics.wiki/windows#cryptnet-url-cache']
 ---
 name: WindowsCurrentVersion
 doc: The Windows current version
 sources:
 - type: REGISTRY_VALUE
   attributes: {key_value_pairs: [{key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion', value: 'CurrentVersion'}]}
 supported_os: [Windows]
@@ -1505,28 +1505,24 @@
 name: WindowsOpenSaveMRU
 doc: Information about files opened or saved in a Windows shell dialog.
 sources:
 - type: REGISTRY_KEY
   attributes:
     keys: ['HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Explorer\ComDIg32\OpenSaveMRU\*\*']
 supported_os: [Windows]
-urls:
-- 'https://forensics.wiki/opensavemru'
-- 'https://digital-forensics.sans.org/blog/2010/04/02/openrunsavemru-lastvisitedmru'
+urls: ['https://forensics.wiki/opensavemru']
 ---
 name: WindowsOpenSavePidlMRU
 doc: Information about files opened or saved in a Windows shell dialog.
 sources:
 - type: REGISTRY_KEY
   attributes:
     keys: ['HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Explorer\ComDlg32\OpenSavePidlMRU\*\*']
 supported_os: [Windows]
-urls:
-- 'https://digital-forensics.sans.org/blog/2010/04/02/openrunsavemru-lastvisitedmru'
-- 'https://forensics.wiki/opensavepidlmru'
+urls: ['https://forensics.wiki/opensavepidlmru']
 ---
 name: WindowsPendingFileRenames
 doc: Windows Pending file renames on reboot
 sources:
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
@@ -1822,27 +1818,27 @@
 - type: FILE
   attributes:
     paths:
     - '\$Recycle.Bin\**'
     - '\Recycler\**'
     separator: '\'
 supported_os: [Windows]
-urls: ['https://forensics.wiki/windows#recycle_bin']
+urls: ['https://forensics.wiki/windows#recycle-bin']
 ---
 name: WindowsRecycleBinMetadata
 doc: Windows Recycle Bin (Recyler, $Recycle.Bin) metadata files only.
 sources:
 - type: FILE
   attributes:
     paths:
     - '\$Recycle.Bin\*\$I*'
     - '\Recycler\*\INFO2'
     separator: '\'
 supported_os: [Windows]
-urls: ['https://forensics.wiki/windows#recycle_bin']
+urls: ['https://forensics.wiki/windows#recycle-bin']
 ---
 name: WindowsRegistryCurrentControlSet
 aliases: [CurrentControlSet]
 doc: The current control set of the Windows Registry.
 sources:
 - type: REGISTRY_VALUE
   attributes: {key_value_pairs: [{key: 'HKEY_LOCAL_MACHINE\System\Select', value: 'Current'}]}
@@ -1989,15 +1985,15 @@
   attributes:
     paths:
     - '%%environ_systemroot%%\Tasks\**10'
     - '%%environ_systemroot%%\System32\Tasks\**10'
     - '%%environ_systemroot%%\SysWow64\Tasks\**10'
     separator: '\'
 supported_os: [Windows]
-urls: ['https://forensics.wiki/windows#scheduled_tasks']
+urls: ['https://forensics.wiki/windows#scheduled-tasks']
 ---
 name: WindowsScreenSaverExecutable
 doc: ScreenSaver Executable
 sources:
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
@@ -3027,15 +3023,15 @@
 doc: Artifacts of RDP connection contents
 sources:
 - type: FILE
   attributes:
     paths: ['%%users.localappdata%%\Microsoft\Terminal Server Client\Cache\*.*']
     separator: '\'
 supported_os: [Windows]
-urls: ['https://forensics.wiki/windows#rdp_bitmap_cache']
+urls: ['https://forensics.wiki/windows#rdp-bitmap-cache']
 ---
 name: WindowsActiveSyncAutoStart
 doc: Windows ActiveSync AutoStart entries
 sources:
 - type: REGISTRY_KEY
   attributes:
     keys:
@@ -3471,28 +3467,28 @@
   process info, among other things.
 sources:
 - type: FILE
   attributes:
     paths: ['%%environ_systemroot%%\System32\WDI\LogFiles\StartupInfo\*.xml']
     separator: '\'
 supported_os: [Windows]
-urls: ['https://forensics.wiki/windows#startup_info']
+urls: ['https://forensics.wiki/windows#startup-info']
 ---
 name: WindowsTileDataLayerDatabase
 doc: |
   Windows tile data layer database (vedatamodel.edb)
 
   The tile data layer database is used to store information about Start Tiles.
 sources:
 - type: FILE
   attributes:
     paths: ['%%users.localappdata%%\TileDataLayer\Database\vedatamodel.edb']
     separator: '\'
 supported_os: [Windows]
-urls: ['https://forensics.wiki/extensible_storage_engine_(ese)_database_file_(edb)_format#tile_data_layer_database']
+urls: ['https://forensics.wiki/extensible_storage_engine_(ese)_database_file_(edb)_format#tile-data-layer-database']
 ---
 name: WindowsUserAccessLogging
 doc: |
   User Access Logging (UAL) databases.
 
   UAL is a local data aggregation feature (enabled by default) on Windows
   Servers 2012 and above, recording client usage by role and product on each
@@ -3501,15 +3497,15 @@
   "<GUID>.mdb").
 sources:
 - type: FILE
   attributes:
     paths: ['%%environ_systemroot%%\System32\LogFiles\SUM\*.mdb']
     separator: '\'
 supported_os: [Windows]
-urls: ['https://forensics.wiki/windows#user_access_logging_(ual)']
+urls: ['https://forensics.wiki/windows#user-access-logging-ual']
 ---
 name: WindowsWordWheelQueryRegistryKey
 doc: Keywords searched in from the Windows start menu, potentially resulting in files or folders access or program executions.
 sources:
 - type: REGISTRY_KEY
   attributes:
     keys: ['HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Explorer\WordWheelQuery\*']
```

### Comparing `artifacts-20221219/data/windows_dll_hijacking.yaml` & `artifacts-20230413/data/windows_dll_hijacking.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/data/wmi.yaml` & `artifacts-20230413/data/wmi.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -225,8 +225,8 @@
 ---
 name: WMICCMRUA
 doc: Enumerate instances of CCM_RecentlyUsedApps.
 sources:
 - type: WMI
   attributes: {query: SELECT * FROM CCM_RecentlyUsedApps, base_object: 'winmgmts:\root\ccm\SoftwareMeteringAgent'}
 supported_os: [Windows]
-urls: ['https://forensics.wiki/windows#ccm_recentlyusedapps']
+urls: ['https://forensics.wiki/windows#ccm-recentlyusedapps']
```

### Comparing `artifacts-20221219/docs/conf.py` & `artifacts-20230413/docs/conf.py`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/docs/index.rst` & `artifacts-20230413/docs/index.rst`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/docs/sources/Format-specification.md` & `artifacts-20230413/docs/sources/Format-specification.md`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/docs/sources/api/artifacts.rst` & `artifacts-20230413/docs/sources/api/artifacts.rst`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/docs/sources/background/Stats.md` & `artifacts-20230413/docs/sources/background/Stats.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 ## Statistics
 
 The artifact definitions can be found in the
 [data directory](https://github.com/ForensicArtifacts/artifacts/tree/main/data) and the format is described in detail
 in the [Style Guide](https://artifacts.readthedocs.io/en/latest/sources/Format-specification.html).
 
-Status of the repository as of 2022-12-19
+Status of the repository as of 2023-04-13
 
 Description | Number
 --- | ---
-Number of artifact definitions: | 756
-Number of file paths: | 1885
+Number of artifact definitions: | 757
+Number of file paths: | 1970
 Number of Windows Registry key paths: | 677
 
 ### Artifact definition source types
 
 Identifier | Number
 --- | ---
 ARTIFACT_GROUP | 47
 COMMAND | 10
-FILE | 471
+FILE | 472
 PATH | 28
 REGISTRY_KEY | 57
 REGISTRY_VALUE | 116
 WMI | 27
 
 ### Operating systems
```

### Comparing `artifacts-20221219/docs/sources/background/Terminology.md` & `artifacts-20230413/docs/sources/background/Terminology.md`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/docs/sources/background/index.rst` & `artifacts-20230413/docs/sources/background/index.rst`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/docs/sources/user/Installation-instructions.md` & `artifacts-20230413/docs/sources/user/Installation-instructions.md`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/run_tests.py` & `artifacts-20230413/run_tests.py`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/setup.py` & `artifacts-20230413/setup.py`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/test_data/definitions.json` & `artifacts-20230413/test_data/definitions.json`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/test_data/definitions.yaml` & `artifacts-20230413/test_data/definitions.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/tests/reader_test.py` & `artifacts-20230413/tests/reader_test.py`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/tests/registry_test.py` & `artifacts-20230413/tests/registry_test.py`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/tests/source_type_test.py` & `artifacts-20230413/tests/source_type_test.py`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/tests/test_lib.py` & `artifacts-20230413/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/tests/validator_test.py` & `artifacts-20230413/tests/validator_test.py`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/tests/writer_test.py` & `artifacts-20230413/tests/writer_test.py`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/tools/stats.py` & `artifacts-20230413/tools/stats.py`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/tools/validator.py` & `artifacts-20230413/tools/validator.py`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/utils/dependencies.py` & `artifacts-20230413/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/utils/pylintrc` & `artifacts-20230413/utils/pylintrc`

 * *Files identical despite different names*

### Comparing `artifacts-20221219/utils/update_release.sh` & `artifacts-20230413/utils/update_release.sh`

 * *Files identical despite different names*

