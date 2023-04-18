# Comparing `tmp/ligo-gracedb-2.8.0.tar.gz` & `tmp/ligo-gracedb-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ligo-gracedb-2.8.0.tar", last modified: Thu Sep 22 22:48:17 2022, max compression
+gzip compressed data, was "ligo-gracedb-2.9.0.tar", last modified: Fri Nov 11 18:46:32 2022, max compression
```

## Comparing `ligo-gracedb-2.8.0.tar` & `ligo-gracedb-2.9.0.tar`

### file list

```diff
@@ -1,128 +1,159 @@
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2022-09-22 22:48:17.911783 ligo-gracedb-2.8.0/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    35149 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/LICENSE
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      107 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/MANIFEST.in
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1984 2022-09-22 22:48:17.911783 ligo-gracedb-2.8.0/PKG-INFO
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      861 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/README.rst
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2022-09-22 22:48:17.907783 ligo-gracedb-2.8.0/debian/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    15175 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/debian/changelog
--rw-rw-r--   0 duncan    (1001) duncan    (1001)        2 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/debian/compat
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1558 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/debian/control
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1126 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/debian/copyright
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       31 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/debian/ligo-gracedb.install
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       33 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/debian/python-ligo-gracedb.install
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       33 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/debian/python3-ligo-gracedb.install
--rwxrwxr-x   0 duncan    (1001) duncan    (1001)      670 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/debian/rules
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2022-09-22 22:48:17.907783 ligo-gracedb-2.8.0/debian/source/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       12 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/debian/source/format
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2022-09-22 22:48:17.907783 ligo-gracedb-2.8.0/ligo/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       56 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/__init__.py
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2022-09-22 22:48:17.907783 ligo-gracedb-2.8.0/ligo/gracedb/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      816 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/__init__.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     4238 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/adapter.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1728 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/alias.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     3525 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cert.py
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2022-09-22 22:48:17.907783 ligo-gracedb-2.8.0/ligo/gracedb/cli/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)        0 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/__init__.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     7792 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/client.py
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2022-09-22 22:48:17.907783 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      945 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/__init__.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     3035 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/add.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     6403 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/base.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    14162 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/create.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1943 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/delete.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     6489 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/get.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     3023 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/list.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     2313 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/remove.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     4221 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/search.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     5446 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/subcommands.py
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2022-09-22 22:48:17.907783 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)        0 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/__init__.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     2672 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_add.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    13068 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_create.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1397 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_delete.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     6321 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_get.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     3337 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_level1_commands.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     5827 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_level1_subcommands.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     2201 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_level2_subcommands_help.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     2307 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_list.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     2292 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_remove.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1875 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_search.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     5167 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_update.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     6031 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/update.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      577 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/conftest.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     5231 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/parsers.py
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2022-09-22 22:48:17.911783 ligo-gracedb-2.8.0/ligo/gracedb/cli/tests/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)        0 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/tests/__init__.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     2625 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/tests/test_cli.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     6284 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/tests/test_main.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1331 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/cli/utils.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     8733 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/client.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      407 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/exceptions.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     3965 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/logging.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    82675 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/rest.py
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2022-09-22 22:48:17.911783 ligo-gracedb-2.8.0/ligo/gracedb/test/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      724 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/__init__.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1863 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/conftest.py
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2022-09-22 22:48:17.911783 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      724 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/__init__.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     2589 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/conftest.py
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2022-09-22 22:48:17.911783 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)  2097152 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/big.data
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    37704 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/burst-cwb-old-format.txt
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     3882 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/burst-cwb-old-old-format.txt
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    81412 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/burst-cwb.txt
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    14021 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/cbc-lm-missing-entry.xml
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    10984 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/cbc-lm-no-ilwdchar.xml
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    14101 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/cbc-lm.xml
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    14101 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/cbc-lm2.xml
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    13447 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/cbc-mbta.gwf
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     6609 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/cbc-mbta.xml
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     5123 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/fermi-test.xml
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      545 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/olib-test.json
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     5474 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/sim-inj.xml
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    18338 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/spiir-test-no-ilwdchar.xml
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    21619 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/spiir-test.xml
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       23 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/test_file.txt
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       31 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/test_file2.txt
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       11 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/upload.data
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1419 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/upload.data.gz
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       11 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/upload2.data
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      546 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/test_api_root.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    30900 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/test_cli.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     2360 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/test_emobservations.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     8346 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/test_events.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     4380 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/test_files.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1918 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/test_labels.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     2473 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/test_logs.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    10300 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/test_superevents.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1631 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/test_update_grbevent.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     8996 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/integration/test_voevents.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     3774 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/test_certificate.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     8060 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/test_client.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     6532 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/test_emobservations.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    19252 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/test_events.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     5771 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/test_files.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     6106 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/test_labels.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1413 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/test_logging.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     7252 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/test_logs.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     2857 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/test_permissions.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1723 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/test_scitokens.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    10972 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/test_signoffs.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    10652 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/test_superevents.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     4811 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/test_tags.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1758 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/test_update_grbevent.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      880 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/test_utils.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     6056 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/test/test_voevents.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     2528 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/utils.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       22 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo/gracedb/version.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     2757 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/ligo-gracedb.spec
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2022-09-22 22:48:17.911783 ligo-gracedb-2.8.0/ligo_gracedb.egg-info/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1984 2022-09-22 22:48:17.000000 ligo-gracedb-2.8.0/ligo_gracedb.egg-info/PKG-INFO
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     4208 2022-09-22 22:48:17.000000 ligo-gracedb-2.8.0/ligo_gracedb.egg-info/SOURCES.txt
--rw-rw-r--   0 duncan    (1001) duncan    (1001)        1 2022-09-22 22:48:17.000000 ligo-gracedb-2.8.0/ligo_gracedb.egg-info/dependency_links.txt
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       57 2022-09-22 22:48:17.000000 ligo-gracedb-2.8.0/ligo_gracedb.egg-info/entry_points.txt
--rw-rw-r--   0 duncan    (1001) duncan    (1001)        5 2022-09-22 22:48:17.000000 ligo-gracedb-2.8.0/ligo_gracedb.egg-info/namespace_packages.txt
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      112 2022-09-22 22:48:17.000000 ligo-gracedb-2.8.0/ligo_gracedb.egg-info/requires.txt
--rw-rw-r--   0 duncan    (1001) duncan    (1001)        5 2022-09-22 22:48:17.000000 ligo-gracedb-2.8.0/ligo_gracedb.egg-info/top_level.txt
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      591 2022-09-22 22:48:17.911783 ligo-gracedb-2.8.0/setup.cfg
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     4088 2022-09-22 22:25:25.000000 ligo-gracedb-2.8.0/setup.py
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-11-11 18:46:32.458874 ligo-gracedb-2.9.0/
+-rw-r--r--   0 alex      (1010) admin       (80)    35149 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/LICENSE
+-rw-r--r--   0 alex      (1010) admin       (80)      107 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/MANIFEST.in
+-rw-r--r--   0 alex      (1010) admin       (80)     2003 2022-11-11 18:46:32.458945 ligo-gracedb-2.9.0/PKG-INFO
+-rw-r--r--   0 alex      (1010) admin       (80)      861 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/README.rst
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-11-11 18:46:32.444787 ligo-gracedb-2.9.0/debian/
+-rw-r--r--   0 alex      (1010) admin       (80)    15401 2022-11-11 18:46:16.000000 ligo-gracedb-2.9.0/debian/changelog
+-rw-r--r--   0 alex      (1010) admin       (80)        2 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/debian/compat
+-rw-r--r--   0 alex      (1010) admin       (80)     1558 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/debian/control
+-rw-r--r--   0 alex      (1010) admin       (80)     1126 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/debian/copyright
+-rw-r--r--   0 alex      (1010) admin       (80)       31 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/debian/ligo-gracedb.install
+-rw-r--r--   0 alex      (1010) admin       (80)       33 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/debian/python-ligo-gracedb.install
+-rw-r--r--   0 alex      (1010) admin       (80)       33 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/debian/python3-ligo-gracedb.install
+-rwxr-xr-x   0 alex      (1010) admin       (80)      670 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/debian/rules
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-11-11 18:46:32.444886 ligo-gracedb-2.9.0/debian/source/
+-rw-r--r--   0 alex      (1010) admin       (80)       12 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/debian/source/format
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-11-11 18:46:32.444985 ligo-gracedb-2.9.0/ligo/
+-rw-r--r--   0 alex      (1010) admin       (80)       56 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/__init__.py
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-11-11 18:46:32.445995 ligo-gracedb-2.9.0/ligo/gracedb/
+-rw-r--r--   0 alex      (1010) admin       (80)      816 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/__init__.py
+-rw-r--r--   0 alex      (1010) admin       (80)     4238 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/adapter.py
+-rw-r--r--   0 alex      (1010) admin       (80)     1728 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/alias.py
+-rw-r--r--   0 alex      (1010) admin       (80)     3525 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/cert.py
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-11-11 18:46:32.446480 ligo-gracedb-2.9.0/ligo/gracedb/cli/
+-rw-r--r--   0 alex      (1010) admin       (80)        0 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/__init__.py
+-rw-r--r--   0 alex      (1010) admin       (80)     7792 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/client.py
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-11-11 18:46:32.447520 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/
+-rw-r--r--   0 alex      (1010) admin       (80)      945 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/__init__.py
+-rw-r--r--   0 alex      (1010) admin       (80)     3035 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/add.py
+-rw-r--r--   0 alex      (1010) admin       (80)     6403 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/base.py
+-rw-r--r--   0 alex      (1010) admin       (80)    14162 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/create.py
+-rw-r--r--   0 alex      (1010) admin       (80)     1943 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/delete.py
+-rw-r--r--   0 alex      (1010) admin       (80)     6489 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/get.py
+-rw-r--r--   0 alex      (1010) admin       (80)     3023 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/list.py
+-rw-r--r--   0 alex      (1010) admin       (80)     2313 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/remove.py
+-rw-r--r--   0 alex      (1010) admin       (80)     4221 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/search.py
+-rw-r--r--   0 alex      (1010) admin       (80)     5628 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/subcommands.py
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-11-11 18:46:32.448670 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/
+-rw-r--r--   0 alex      (1010) admin       (80)        0 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/__init__.py
+-rw-r--r--   0 alex      (1010) admin       (80)     2672 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_add.py
+-rw-r--r--   0 alex      (1010) admin       (80)    13068 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_create.py
+-rw-r--r--   0 alex      (1010) admin       (80)     1397 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_delete.py
+-rw-r--r--   0 alex      (1010) admin       (80)     6321 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_get.py
+-rw-r--r--   0 alex      (1010) admin       (80)     3337 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_level1_commands.py
+-rw-r--r--   0 alex      (1010) admin       (80)     5827 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_level1_subcommands.py
+-rw-r--r--   0 alex      (1010) admin       (80)     2201 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_level2_subcommands_help.py
+-rw-r--r--   0 alex      (1010) admin       (80)     2307 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_list.py
+-rw-r--r--   0 alex      (1010) admin       (80)     2292 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_remove.py
+-rw-r--r--   0 alex      (1010) admin       (80)     1875 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_search.py
+-rw-r--r--   0 alex      (1010) admin       (80)     5167 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_update.py
+-rw-r--r--   0 alex      (1010) admin       (80)     6031 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/update.py
+-rw-r--r--   0 alex      (1010) admin       (80)      577 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/conftest.py
+-rw-r--r--   0 alex      (1010) admin       (80)     5389 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/parsers.py
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-11-11 18:46:32.448928 ligo-gracedb-2.9.0/ligo/gracedb/cli/tests/
+-rw-r--r--   0 alex      (1010) admin       (80)        0 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/tests/__init__.py
+-rw-r--r--   0 alex      (1010) admin       (80)     2625 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/tests/test_cli.py
+-rw-r--r--   0 alex      (1010) admin       (80)     6284 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/tests/test_main.py
+-rw-r--r--   0 alex      (1010) admin       (80)     1331 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/cli/utils.py
+-rw-r--r--   0 alex      (1010) admin       (80)     8733 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/client.py
+-rw-r--r--   0 alex      (1010) admin       (80)      407 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/exceptions.py
+-rw-r--r--   0 alex      (1010) admin       (80)     3965 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/logging.py
+-rw-r--r--   0 alex      (1010) admin       (80)    83036 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/rest.py
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-11-11 18:46:32.450733 ligo-gracedb-2.9.0/ligo/gracedb/test/
+-rw-r--r--   0 alex      (1010) admin       (80)      724 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/__init__.py
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-11-11 18:46:32.452477 ligo-gracedb-2.9.0/ligo/gracedb/test/__pycache__/
+-rw-r--r--   0 alex      (1010) admin       (80)      148 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)     2043 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/__pycache__/conftest.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)     4879 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/__pycache__/test_certificate.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)    18362 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/__pycache__/test_client.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)     9051 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/__pycache__/test_emobservations.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)    25285 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/__pycache__/test_events.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)    10120 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/__pycache__/test_files.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)     9001 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/__pycache__/test_labels.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)     2442 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/__pycache__/test_logging.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)    10651 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/__pycache__/test_logs.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)     5022 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/__pycache__/test_permissions.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)    14449 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/__pycache__/test_signoffs.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)    12368 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/__pycache__/test_superevents.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)     8408 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/__pycache__/test_tags.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)     2455 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/__pycache__/test_update_grbevent.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)     2071 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/__pycache__/test_utils.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)     8018 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/__pycache__/test_voevents.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)     1863 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/conftest.py
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-11-11 18:46:32.453721 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/
+-rw-r--r--   0 alex      (1010) admin       (80)      724 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/__init__.py
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-11-11 18:46:32.454965 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/__pycache__/
+-rw-r--r--   0 alex      (1010) admin       (80)      160 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)     2377 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/__pycache__/conftest.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)     1707 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/__pycache__/test_api_root.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)    49466 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/__pycache__/test_cli.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)     5205 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/__pycache__/test_emobservations.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)    15726 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/__pycache__/test_events.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)     8445 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/__pycache__/test_files.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)     4395 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/__pycache__/test_labels.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)     5187 2022-04-05 19:07:02.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/__pycache__/test_logs.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)    13992 2022-04-05 19:07:03.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/__pycache__/test_superevents.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)     2613 2022-04-05 19:07:03.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/__pycache__/test_update_grbevent.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)    12646 2022-04-05 19:07:03.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/__pycache__/test_voevents.cpython-39-pytest-7.0.1.pyc
+-rw-r--r--   0 alex      (1010) admin       (80)     2589 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/conftest.py
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-11-11 18:46:32.458138 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/
+-rw-r--r--   0 alex      (1010) admin       (80)  2097152 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/big.data
+-rw-r--r--   0 alex      (1010) admin       (80)    37704 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/burst-cwb-old-format.txt
+-rw-r--r--   0 alex      (1010) admin       (80)     3882 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/burst-cwb-old-old-format.txt
+-rw-r--r--   0 alex      (1010) admin       (80)    81412 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/burst-cwb.txt
+-rw-r--r--   0 alex      (1010) admin       (80)    14021 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/cbc-lm-missing-entry.xml
+-rw-r--r--   0 alex      (1010) admin       (80)    10984 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/cbc-lm-no-ilwdchar.xml
+-rw-r--r--   0 alex      (1010) admin       (80)    14101 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/cbc-lm.xml
+-rw-r--r--   0 alex      (1010) admin       (80)    14101 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/cbc-lm2.xml
+-rw-r--r--   0 alex      (1010) admin       (80)    13447 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/cbc-mbta.gwf
+-rw-r--r--   0 alex      (1010) admin       (80)     6609 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/cbc-mbta.xml
+-rw-r--r--   0 alex      (1010) admin       (80)     5123 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/fermi-test.xml
+-rw-r--r--   0 alex      (1010) admin       (80)      545 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/olib-test.json
+-rw-r--r--   0 alex      (1010) admin       (80)     5474 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/sim-inj.xml
+-rw-r--r--   0 alex      (1010) admin       (80)    18338 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/spiir-test-no-ilwdchar.xml
+-rw-r--r--   0 alex      (1010) admin       (80)    21619 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/spiir-test.xml
+-rw-r--r--   0 alex      (1010) admin       (80)       23 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/test_file.txt
+-rw-r--r--   0 alex      (1010) admin       (80)       31 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/test_file2.txt
+-rw-r--r--   0 alex      (1010) admin       (80)       11 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/upload.data
+-rw-r--r--   0 alex      (1010) admin       (80)     1419 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/upload.data.gz
+-rw-r--r--   0 alex      (1010) admin       (80)       11 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/upload2.data
+-rw-r--r--   0 alex      (1010) admin       (80)      546 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/test_api_root.py
+-rw-r--r--   0 alex      (1010) admin       (80)    30900 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/test_cli.py
+-rw-r--r--   0 alex      (1010) admin       (80)     2360 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/test_emobservations.py
+-rw-r--r--   0 alex      (1010) admin       (80)     8346 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/test_events.py
+-rw-r--r--   0 alex      (1010) admin       (80)     4380 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/test_files.py
+-rw-r--r--   0 alex      (1010) admin       (80)     1918 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/test_labels.py
+-rw-r--r--   0 alex      (1010) admin       (80)     2473 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/test_logs.py
+-rw-r--r--   0 alex      (1010) admin       (80)    10300 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/test_superevents.py
+-rw-r--r--   0 alex      (1010) admin       (80)     1631 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/test_update_grbevent.py
+-rw-r--r--   0 alex      (1010) admin       (80)     9023 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/integration/test_voevents.py
+-rw-r--r--   0 alex      (1010) admin       (80)     3774 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/test_certificate.py
+-rw-r--r--   0 alex      (1010) admin       (80)     8060 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/test_client.py
+-rw-r--r--   0 alex      (1010) admin       (80)     6532 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/test_emobservations.py
+-rw-r--r--   0 alex      (1010) admin       (80)    19262 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/test_events.py
+-rw-r--r--   0 alex      (1010) admin       (80)     5771 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/test_files.py
+-rw-r--r--   0 alex      (1010) admin       (80)     6106 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/test_labels.py
+-rw-r--r--   0 alex      (1010) admin       (80)     1413 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/test_logging.py
+-rw-r--r--   0 alex      (1010) admin       (80)     7252 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/test_logs.py
+-rw-r--r--   0 alex      (1010) admin       (80)     2857 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/test_permissions.py
+-rw-r--r--   0 alex      (1010) admin       (80)     1723 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/test_scitokens.py
+-rw-r--r--   0 alex      (1010) admin       (80)    10972 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/test_signoffs.py
+-rw-r--r--   0 alex      (1010) admin       (80)    10662 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/test_superevents.py
+-rw-r--r--   0 alex      (1010) admin       (80)     4811 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/test_tags.py
+-rw-r--r--   0 alex      (1010) admin       (80)     1758 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/test_update_grbevent.py
+-rw-r--r--   0 alex      (1010) admin       (80)      880 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/test_utils.py
+-rw-r--r--   0 alex      (1010) admin       (80)     6804 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/ligo/gracedb/test/test_voevents.py
+-rw-r--r--   0 alex      (1010) admin       (80)     2528 2022-04-05 18:57:23.000000 ligo-gracedb-2.9.0/ligo/gracedb/utils.py
+-rw-r--r--   0 alex      (1010) admin       (80)       22 2022-11-11 18:46:16.000000 ligo-gracedb-2.9.0/ligo/gracedb/version.py
+-rw-r--r--   0 alex      (1010) admin       (80)     2757 2022-11-11 18:46:16.000000 ligo-gracedb-2.9.0/ligo-gracedb.spec
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-11-11 18:46:32.458783 ligo-gracedb-2.9.0/ligo_gracedb.egg-info/
+-rw-r--r--   0 alex      (1010) admin       (80)     2003 2022-11-11 18:46:32.000000 ligo-gracedb-2.9.0/ligo_gracedb.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1010) admin       (80)     6395 2022-11-11 18:46:32.000000 ligo-gracedb-2.9.0/ligo_gracedb.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1010) admin       (80)        1 2022-11-11 18:46:32.000000 ligo-gracedb-2.9.0/ligo_gracedb.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1010) admin       (80)       57 2022-11-11 18:46:32.000000 ligo-gracedb-2.9.0/ligo_gracedb.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1010) admin       (80)        5 2022-11-11 18:46:32.000000 ligo-gracedb-2.9.0/ligo_gracedb.egg-info/namespace_packages.txt
+-rw-r--r--   0 alex      (1010) admin       (80)      112 2022-11-11 18:46:32.000000 ligo-gracedb-2.9.0/ligo_gracedb.egg-info/requires.txt
+-rw-r--r--   0 alex      (1010) admin       (80)        5 2022-11-11 18:46:32.000000 ligo-gracedb-2.9.0/ligo_gracedb.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1010) admin       (80)      591 2022-11-11 18:46:32.459211 ligo-gracedb-2.9.0/setup.cfg
+-rw-r--r--   0 alex      (1010) admin       (80)     4088 2022-11-11 18:34:50.000000 ligo-gracedb-2.9.0/setup.py
```

### Comparing `ligo-gracedb-2.8.0/LICENSE` & `ligo-gracedb-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/PKG-INFO` & `ligo-gracedb-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: ligo-gracedb
-Version: 2.8.0
+Version: 2.9.0
 Summary: A Python package for accessing the GraceDB API.
 Home-page: https://git.ligo.org/lscsoft/gracedb-client
 Author: Tanner Prestegard, Alexander Pace, Branson Stephens, Brian Moe, Patrick Brady
 Author-email: tanner.prestegard@ligo.org, alexander.pace@ligo.org
 License: GPL-3.0-or-later
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
@@ -43,7 +44,8 @@
 
 
 Contributing
 ------------
 Please fork this `repository <https://git.ligo.org/computing/gracedb/client/>`__ and submit a merge request if you wish to contribute to this package.
 
 See the `contributing documentation <https://ligo-gracedb.readthedocs.io//en/latest/contributing.html>`__ for more details.
+
```

### Comparing `ligo-gracedb-2.8.0/README.rst` & `ligo-gracedb-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/debian/changelog` & `ligo-gracedb-2.9.0/debian/changelog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+ligo-gracedb (2.9.0-1) unstable; urgency=low
+  * support HasMassGap instead of MassGap for VOEvents
+  * gw_id support for naming confirmed GWs
+
+ -- Alexander E. Pace <alexander.pace@ligo.org>  Fri, 11 Nov 2022 09:58:54 -0800
+
 ligo-gracedb (2.8.0-1) unstable; urgency=low
   * use igwn-auth-utils for credential finding
 
  -- Alexander E. Pace <alexander.pace@ligo.org>  Wed, 11 May 2022 10:11:30 -0700
 
 ligo-gracedb (2.7.8-1) unstable; urgency=low
   * pipeline-specific preferred event features
```

### Comparing `ligo-gracedb-2.8.0/debian/control` & `ligo-gracedb-2.9.0/debian/control`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/debian/copyright` & `ligo-gracedb-2.9.0/debian/copyright`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/debian/rules` & `ligo-gracedb-2.9.0/debian/rules`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/__init__.py` & `ligo-gracedb-2.9.0/ligo/gracedb/__init__.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/adapter.py` & `ligo-gracedb-2.9.0/ligo/gracedb/adapter.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/alias.py` & `ligo-gracedb-2.9.0/ligo/gracedb/alias.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cert.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cert.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/client.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/client.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/__init__.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/add.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/base.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/create.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/create.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/delete.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/delete.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/get.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/get.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/list.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/remove.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/search.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/subcommands.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/subcommands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import six
 import textwrap
 
 from .base import RegisteredSubCommandBase
-from ..parsers import superevent_id_parser
+from ..parsers import superevent_id_parser, gw_id_parser
 
 
 class ConfirmAsGwCommand(RegisteredSubCommandBase):
     name = "confirm_as_gw"
     description = "Confirm a superevent as a GW"
     long_description = textwrap.dedent("""\
         Confirm a superevent as a gravitational wave. Specific permissions are
         required to perform this action on non-Test superevents.
     """).rstrip()
-    parent_parsers = (superevent_id_parser,)
+    parent_parsers = (superevent_id_parser, gw_id_parser,)
 
     def run(self, client, args):
-        return client.confirm_superevent_as_gw(args.superevent_id)
+        if args.gw_id:
+            return client.confirm_superevent_as_gw(
+                args.superevent_id, args.gw_id
+            )
+        else:
+            return client.confirm_superevent_as_gw(args.superevent_id)
 
 
 class CredentialsCommand(RegisteredSubCommandBase):
     name = "credentials"
     description = "Display your credentials"
     long_description = textwrap.dedent("""\
         Display the credentials that the client will use to make API requests
```

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_add.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_create.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_delete.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_get.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_get.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_level1_commands.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_level1_commands.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_level1_subcommands.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_level1_subcommands.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_level2_subcommands_help.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_level2_subcommands_help.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_list.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_remove.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_remove.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_search.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/tests/test_update.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/commands/update.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/conftest.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/parsers.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,20 @@
     "object_id", type=str, help="Event graceid or superevent id"
 )
 
 # Graceid parser
 graceid_parser = argparse.ArgumentParser(add_help=False)
 graceid_parser.add_argument("graceid", type=str, help="Event graceid")
 
+# GW_id parser
+gw_id_parser = argparse.ArgumentParser(add_help=False)
+gw_id_parser.add_argument(
+    "gw_id", type=str, nargs='?', help="Superevent GW id"
+)
+
 # Superevent id parser
 superevent_id_parser = argparse.ArgumentParser(add_help=False)
 superevent_id_parser.add_argument(
     "superevent_id", type=str, help="Superevent id"
 )
 
 # Tag parser
```

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/tests/test_cli.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/tests/test_main.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/cli/utils.py` & `ligo-gracedb-2.9.0/ligo/gracedb/cli/utils.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/client.py` & `ligo-gracedb-2.9.0/ligo/gracedb/client.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/logging.py` & `ligo-gracedb-2.9.0/ligo/gracedb/logging.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/rest.py` & `ligo-gracedb-2.9.0/ligo/gracedb/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -977,15 +977,15 @@
                     return
                 # If columns are specified, only return specific values
                 if columns:
                     yield {k: superevent[k] for k in columns}
                 else:
                     yield superevent
 
-    def confirm_superevent_as_gw(self, superevent_id):
+    def confirm_superevent_as_gw(self, superevent_id, gw_id=None):
         """Upgrade a superevent's state to 'confirmed GW'.
 
         All LIGO-Virgo users can perform this action on test superevents,
         but special permissions are required for production and MDC
         superevents. This action cannot be undone!
 
         Args:
@@ -1003,15 +1003,20 @@
             >>> g = GraceDb()
             >>> r = confirm_superevent_as_gw('S181224a')
             >>> r.status_code
             204
         """
         template = self.templates['superevent-confirm-as-gw-template']
         uri = template.format(superevent_id=superevent_id)
-        return self.post(uri)
+
+        request_body = {}
+        if gw_id:
+            request_body = {'gw_id': gw_id}
+
+        return self.post(uri, data=request_body)
 
     @event_or_superevent
     def files(self, object_id, filename="", *args, **kwargs):
         """Get a list of files or download a file associated with an event or
         superevent.
 
         If ``filename`` is not provided, get a list of available files
@@ -1687,15 +1692,16 @@
     @event_or_superevent
     @alias('createVOEvent')
     def create_voevent(self, object_id, voevent_type, skymap_type=None,
                        skymap_filename=None, combined_skymap_filename=None,
                        internal=True, open_alert=False, raven_coinc=False,
                        hardware_inj=False, CoincComment=False, ProbHasNS=None,
                        ProbHasRemnant=None, BNS=None, NSBH=None, BBH=None,
-                       Terrestrial=None, MassGap=None, *args, **kwargs):
+                       Terrestrial=None, MassGap=None, HasMassGap=None,
+                       *args, **kwargs):
         r"""Create a new VOEvent.
 
         Args:
             object_id (str): event graceid or superevent ID.
             voevent_type (str): VOEvent type (choose from ``'preliminary'``,
                 ``'initial'``, ``'update'``, and ``'retraction'``).
             skymap_type (:obj:`str`, optional): skymap type. Required for
@@ -1726,15 +1732,15 @@
             NSBH (:obj:`float`, optional): probability that the source is a
                 neutron star-black hole merger (CBC events only).
             BBH (:obj:`float`, optional): probability that the source is a
                 binary black hole merger (CBC events only).
             Terrestrial (:obj:`float`, optional): probability that the source
                 is terrestrial (i.e., a background noise fluctuation or a
                 glitch) (CBC events only).
-            MassGap (:obj:`float`, optional): probability that at least one
+            HasMassGap (:obj:`float`, optional): probability that at least one
                 object in the binary has a mass between 3 and 5 M\ :sub:`sun`
                 (CBC events only).
 
         Returns:
             :class:`requests.models.Response`
 
         Raises:
@@ -1766,14 +1772,19 @@
 
         # Require skymaps for 'update' and 'initial'
         if voevent_type == 'IN':
             if not skymap_filename:
                 raise ValueError("Skymap file is required for 'initial' "
                                  "VOEvents")
 
+        # Inform user about MassGap-->HasMassGap:
+        if MassGap:
+            raise ValueError('"MassGap" parameter has been replaced by '
+                             'HasMassGap.')
+
         # Construct request body
         body = {
             'voevent_type': voevent_type,
             'internal': internal,
             'open_alert': open_alert,
             'hardware_inj': hardware_inj,
             'CoincComment': CoincComment,
@@ -1794,16 +1805,16 @@
             body['BNS'] = BNS
         if NSBH is not None:
             body['NSBH'] = NSBH
         if BBH is not None:
             body['BBH'] = BBH
         if Terrestrial is not None:
             body['Terrestrial'] = Terrestrial
-        if MassGap is not None:
-            body['MassGap'] = MassGap
+        if HasMassGap is not None:
+            body['HasMassGap'] = HasMassGap
 
         return self.post(uri, data=body)
 
     @event_or_superevent
     def permissions(self, object_id, *args, **kwargs):
         """Get a list of permissions for a superevent.
```

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/__init__.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/__init__.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/conftest.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/conftest.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/__init__.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/conftest.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/big.data` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/big.data`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/burst-cwb-old-format.txt` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/burst-cwb-old-format.txt`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/burst-cwb-old-old-format.txt` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/burst-cwb-old-old-format.txt`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/burst-cwb.txt` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/burst-cwb.txt`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/cbc-lm-missing-entry.xml` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/cbc-lm-missing-entry.xml`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/cbc-lm-no-ilwdchar.xml` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/cbc-lm-no-ilwdchar.xml`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/cbc-lm.xml` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/cbc-lm.xml`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/cbc-lm2.xml` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/cbc-lm2.xml`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/cbc-mbta.gwf` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/cbc-mbta.gwf`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/cbc-mbta.xml` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/cbc-mbta.xml`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/fermi-test.xml` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/fermi-test.xml`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/olib-test.json` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/olib-test.json`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/sim-inj.xml` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/sim-inj.xml`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/spiir-test-no-ilwdchar.xml` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/spiir-test-no-ilwdchar.xml`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/spiir-test.xml` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/spiir-test.xml`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/data/upload.data.gz` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/data/upload.data.gz`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/test_api_root.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/test_api_root.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/test_cli.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/test_emobservations.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/test_emobservations.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/test_events.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/test_events.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/test_files.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/test_files.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/test_labels.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/test_labels.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/test_logs.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/test_logs.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/test_superevents.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/test_superevents.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/test_update_grbevent.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/test_update_grbevent.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/integration/test_voevents.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/integration/test_voevents.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     'CoincComment': False,
     'ProbHasNS': 0.1,
     'ProbHasRemnant': 0.9,
     'BNS': 0.2,
     'NSBH': 0.3,
     'BBH': 0.4,
     'Terrestrial': 0.5,
-    'MassGap': 0.6,
+    'HasMassGap': 0.6,
 }
 
 INITIAL_VOEVENT_DATA = {
     'skymap_type': 'new',
     'skymap_filename': 'fake_skymap.txt',
     'internal': True,
     'hardware_inj': False,
@@ -34,15 +34,15 @@
     'CoincComment': False,
     'ProbHasNS': 0.1,
     'ProbHasRemnant': 0.9,
     'BNS': 0.2,
     'NSBH': 0.3,
     'BBH': 0.4,
     'Terrestrial': 0.5,
-    'MassGap': 0.6,
+    'HasMassGap': 0.6,
 }
 
 
 ###############################################################################
 # UTILITY FUNCTIONS ###########################################################
 ###############################################################################
 def get_citations_dict(obj_id, voevent_file_text):
@@ -77,15 +77,15 @@
     assert data['prob_has_ns'] == PRELIMINARY_VOEVENT_DATA['ProbHasNS']
     assert data['prob_has_remnant'] == \
         PRELIMINARY_VOEVENT_DATA['ProbHasRemnant']
     assert data['prob_bns'] == PRELIMINARY_VOEVENT_DATA['BNS']
     assert data['prob_nsbh'] == PRELIMINARY_VOEVENT_DATA['NSBH']
     assert data['prob_bbh'] == PRELIMINARY_VOEVENT_DATA['BBH']
     assert data['prob_terrestrial'] == PRELIMINARY_VOEVENT_DATA['Terrestrial']
-    assert data['prob_mass_gap'] == PRELIMINARY_VOEVENT_DATA['MassGap']
+    assert data['prob_has_mass_gap'] == PRELIMINARY_VOEVENT_DATA['HasMassGap']
 
 
 @pytest.mark.parametrize("obj_type", ['event', 'superevent'])
 def test_initial_voevent(client, create_obj, obj_type):
     # Create event or superevent
     obj, obj_id = create_obj(obj_type)
 
@@ -115,15 +115,15 @@
     assert data['coinc_comment'] == INITIAL_VOEVENT_DATA['CoincComment']
     assert data['prob_has_ns'] == INITIAL_VOEVENT_DATA['ProbHasNS']
     assert data['prob_has_remnant'] == INITIAL_VOEVENT_DATA['ProbHasRemnant']
     assert data['prob_bns'] == INITIAL_VOEVENT_DATA['BNS']
     assert data['prob_nsbh'] == INITIAL_VOEVENT_DATA['NSBH']
     assert data['prob_bbh'] == INITIAL_VOEVENT_DATA['BBH']
     assert data['prob_terrestrial'] == INITIAL_VOEVENT_DATA['Terrestrial']
-    assert data['prob_mass_gap'] == INITIAL_VOEVENT_DATA['MassGap']
+    assert data['prob_has_mass_gap'] == INITIAL_VOEVENT_DATA['HasMassGap']
 
     # Check citations
     response = client.files(obj_id, data['filename'])
     assert response.status_code == 200
     voevent_file_text = response.read()
     citations_dict = get_citations_dict(obj_id, voevent_file_text)
     assert len(citations_dict) == 1
@@ -167,15 +167,15 @@
     assert data['coinc_comment'] == INITIAL_VOEVENT_DATA['CoincComment']
     assert data['prob_has_ns'] == INITIAL_VOEVENT_DATA['ProbHasNS']
     assert data['prob_has_remnant'] == INITIAL_VOEVENT_DATA['ProbHasRemnant']
     assert data['prob_bns'] == INITIAL_VOEVENT_DATA['BNS']
     assert data['prob_nsbh'] == INITIAL_VOEVENT_DATA['NSBH']
     assert data['prob_bbh'] == INITIAL_VOEVENT_DATA['BBH']
     assert data['prob_terrestrial'] == INITIAL_VOEVENT_DATA['Terrestrial']
-    assert data['prob_mass_gap'] == INITIAL_VOEVENT_DATA['MassGap']
+    assert data['prob_has_mass_gap'] == INITIAL_VOEVENT_DATA['HasMassGap']
 
     # Check citations
     response = client.files(obj_id, data['filename'])
     assert response.status_code == 200
     voevent_file_text = response.read()
     citations_dict = get_citations_dict(obj_id, voevent_file_text)
     assert len(citations_dict) == 2
```

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/test_certificate.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/test_certificate.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/test_client.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/test_client.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/test_emobservations.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/test_emobservations.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/test_events.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/test_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -420,15 +420,15 @@
     template_prop = 'ligo.gracedb.rest.GraceDb.templates'
     with mock.patch('ligo.gracedb.rest.GraceDb.post') as mock_post, \
          mock.patch(template_prop, mock_template_dict):  # noqa: E127
         safe_client.confirm_superevent_as_gw(superevent_id)
 
     post_call_args, post_call_kwargs = mock_post.call_args
     assert len(post_call_args) == 1
-    assert post_call_kwargs == {}
+    assert post_call_kwargs == {'data': {}}
 
     template_call_args, template_call_kwargs = mock_template.format.call_args
     assert template_call_args == ()
     assert len(template_call_kwargs) == 1
     assert template_call_kwargs['superevent_id'] == superevent_id
```

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/test_files.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/test_files.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/test_labels.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/test_labels.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/test_logging.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/test_logs.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/test_logs.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/test_permissions.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/test_permissions.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/test_scitokens.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/test_scitokens.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/test_signoffs.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/test_signoffs.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/test_superevents.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/test_superevents.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,15 +242,15 @@
     template_prop = 'ligo.gracedb.rest.GraceDb.templates'
     with mock.patch('ligo.gracedb.rest.GraceDb.post') as mock_post, \
          mock.patch(template_prop, mock_template_dict):  # noqa: E127
         safe_client.confirm_superevent_as_gw(superevent_id)
 
     post_call_args, post_call_kwargs = mock_post.call_args
     assert len(post_call_args) == 1
-    assert post_call_kwargs == {}
+    assert post_call_kwargs == {'data': {}}
 
     template_call_args, template_call_kwargs = mock_template.format.call_args
     assert template_call_args == ()
     assert len(template_call_kwargs) == 1
     assert template_call_kwargs['superevent_id'] == superevent_id
```

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/test_tags.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/test_tags.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/test_update_grbevent.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/test_update_grbevent.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/test_utils.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/test/test_voevents.py` & `ligo-gracedb-2.9.0/ligo/gracedb/test/test_voevents.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         'CoincComment': False,
         'ProbHasNS': 0.6,
         'ProbHasRemnant': 0.7,
         'BNS': 0.1,
         'NSBH': 0.2,
         'BBH': 0.3,
         'Terrestrial': 0.4,
-        'MassGap': 0.5,
+        'HasMassGap': 0.5,
     }
 
     # Set up templates mock
     mock_template = mock.MagicMock()
     if is_event:
         template_key = 'voevent-list-template'
     else:
@@ -131,14 +131,36 @@
     if is_event:
         call_key = 'graceid'
     else:
         call_key = 'superevent_id'
     assert template_call_kwargs[call_key] == obj_id
 
 
+def test_create_voevent_massgap_superevent(safe_client):
+    obj_id = "TS121212abc"
+
+    # Generate data
+    voevent_type = 'PR'
+
+    # Set up templates mock
+    mock_template = mock.MagicMock()
+    template_key = 'superevent-voevent-list-template'
+    mock_template_dict = {template_key: mock_template}
+    template_prop = 'ligo.gracedb.rest.GraceDb.templates'
+
+    # Set up emgroup mock
+    si_prop = 'ligo.gracedb.rest.GraceDb.service_info'
+    mock_si_dict = {'voevent-types': {voevent_type: 'preliminary'}}
+
+    with mock.patch(si_prop, mock_si_dict), \
+         mock.patch(template_prop, mock_template_dict):  # noqa: E127
+        with pytest.raises(ValueError):
+            safe_client.create_voevent(obj_id, voevent_type, MassGap=1.0)
+
+
 def test_create_voevent_bad_voevent_type(safe_client):
     # Set up templates mock
     mock_template = mock.MagicMock()
     mock_template_dict = {'superevent-voevent-list-template': mock_template}
     template_prop = 'ligo.gracedb.rest.GraceDb.templates'
 
     # Set up emgroup mock
```

### Comparing `ligo-gracedb-2.8.0/ligo/gracedb/utils.py` & `ligo-gracedb-2.9.0/ligo/gracedb/utils.py`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/ligo-gracedb.spec` & `ligo-gracedb-2.9.0/ligo-gracedb.spec`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 %define srcname              ligo-gracedb
-%define version           2.8.0
-%define unmangled_version 2.8.0
+%define version           2.9.0
+%define unmangled_version 2.9.0
 %define release           1
 
 Summary:   Gravity Wave Candidate Event Database
 Name:      python-%{srcname}
 Version:   %{version}
 Release:   %{release}%{?dist}
 Source0:   %pypi_source
```

### Comparing `ligo-gracedb-2.8.0/ligo_gracedb.egg-info/PKG-INFO` & `ligo-gracedb-2.9.0/ligo_gracedb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: ligo-gracedb
-Version: 2.8.0
+Version: 2.9.0
 Summary: A Python package for accessing the GraceDB API.
 Home-page: https://git.ligo.org/lscsoft/gracedb-client
 Author: Tanner Prestegard, Alexander Pace, Branson Stephens, Brian Moe, Patrick Brady
 Author-email: tanner.prestegard@ligo.org, alexander.pace@ligo.org
 License: GPL-3.0-or-later
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
@@ -43,7 +44,8 @@
 
 
 Contributing
 ------------
 Please fork this `repository <https://git.ligo.org/computing/gracedb/client/>`__ and submit a merge request if you wish to contribute to this package.
 
 See the `contributing documentation <https://ligo-gracedb.readthedocs.io//en/latest/contributing.html>`__ for more details.
+
```

### Comparing `ligo-gracedb-2.8.0/setup.cfg` & `ligo-gracedb-2.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ligo-gracedb-2.8.0/setup.py` & `ligo-gracedb-2.9.0/setup.py`

 * *Files identical despite different names*

