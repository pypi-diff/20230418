# Comparing `tmp/nx5d-0.3.1.tar.gz` & `tmp/nx5d-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nx5d-0.3.1.tar", last modified: Mon Apr 17 15:48:04 2023, max compression
+gzip compressed data, was "nx5d-0.3.2.tar", last modified: Tue Apr 18 08:04:42 2023, max compression
```

## Comparing `nx5d-0.3.1.tar` & `nx5d-0.3.2.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.474620 nx5d-0.3.1/
--rw-r--r--   0 florin    (1000) florin    (1000)       72 2023-04-13 14:23:04.000000 nx5d-0.3.1/.gitignore
--rw-r--r--   0 florin    (1000) florin    (1000)     3261 2023-04-12 13:31:40.000000 nx5d-0.3.1/.gitlab-ci.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      227 2023-03-15 11:10:41.000000 nx5d-0.3.1/.readthedocs.yaml
--rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-14 11:33:48.000000 nx5d-0.3.1/COPYING.md
--rw-r--r--   0 florin    (1000) florin    (1000)     3449 2023-04-17 15:48:04.474620 nx5d-0.3.1/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)     2724 2023-03-27 10:49:57.000000 nx5d-0.3.1/README.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.454620 nx5d-0.3.1/doc/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.456620 nx5d-0.3.1/doc/mkdocs/
--rw-r--r--   0 florin    (1000) florin    (1000)       11 2023-03-15 10:15:42.000000 nx5d-0.3.1/doc/mkdocs/about.md
--rw-r--r--   0 florin    (1000) florin    (1000)      147 2023-04-12 12:52:07.000000 nx5d-0.3.1/doc/mkdocs/api.md
--rw-r--r--   0 florin    (1000) florin    (1000)    27046 2023-03-27 10:25:44.000000 nx5d-0.3.1/doc/mkdocs/concepts.md
--rw-r--r--   0 florin    (1000) florin    (1000)     5970 2023-03-25 14:27:00.000000 nx5d-0.3.1/doc/mkdocs/frame.svg
--rw-r--r--   0 florin    (1000) florin    (1000)     2482 2023-03-27 10:54:07.000000 nx5d-0.3.1/doc/mkdocs/index.md
--rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-15 10:32:22.000000 nx5d-0.3.1/doc/mkdocs/license.md
--rw-r--r--   0 florin    (1000) florin    (1000)      723 2023-03-27 10:50:49.000000 nx5d-0.3.1/doc/mkdocs/module-nx.md
--rw-r--r--   0 florin    (1000) florin    (1000)    36207 2023-03-25 14:25:35.000000 nx5d-0.3.1/doc/mkdocs/scan.svg
--rw-r--r--   0 florin    (1000) florin    (1000)    25024 2023-03-25 14:49:22.000000 nx5d-0.3.1/doc/mkdocs/streak1.svg
--rw-r--r--   0 florin    (1000) florin    (1000)    11491 2023-03-25 14:49:37.000000 nx5d-0.3.1/doc/mkdocs/streak2.svg
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.456620 nx5d-0.3.1/doc/mkdocs/tutorials/
--rw-r--r--   0 florin    (1000) florin    (1000)      516 2023-03-15 10:35:31.000000 nx5d-0.3.1/doc/mkdocs/tutorials/index.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.457620 nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/
--rw-------   0 florin    (1000) florin    (1000)    44315 2023-03-14 14:52:34.000000 nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md
--rw-------   0 florin    (1000) florin    (1000)    19430 2023-03-14 14:52:34.000000 nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png
--rw-------   0 florin    (1000) florin    (1000)    25263 2023-03-14 14:52:34.000000 nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png
--rw-------   0 florin    (1000) florin    (1000)    23184 2023-03-14 14:52:34.000000 nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png
--rw-------   0 florin    (1000) florin    (1000)    13289 2023-03-14 14:52:34.000000 nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png
--rw-------   0 florin    (1000) florin    (1000)    16038 2023-03-14 14:52:34.000000 nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.457620 nx5d-0.3.1/doc/mkdocs/tutorials/scansource-howto/
--rw-r--r--   0 florin    (1000) florin    (1000)     8968 2023-03-14 12:31:08.000000 nx5d-0.3.1/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.457620 nx5d-0.3.1/doc/mkdocs/user-guide/
--rw-r--r--   0 florin    (1000) florin    (1000)      322 2023-04-12 12:48:11.000000 nx5d-0.3.1/doc/mkdocs/user-guide/index.md
--rw-r--r--   0 florin    (1000) florin    (1000)      513 2023-03-15 14:06:55.000000 nx5d-0.3.1/doc/mkdocs.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      273 2023-03-15 10:49:21.000000 nx5d-0.3.1/mkdocs.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      280 2023-03-14 11:33:48.000000 nx5d-0.3.1/pyproject.toml
--rw-r--r--   0 florin    (1000) florin    (1000)     2974 2022-08-02 20:02:56.000000 nx5d-0.3.1/scratch.org
--rw-r--r--   0 florin    (1000) florin    (1000)      900 2023-04-17 15:48:04.475620 nx5d-0.3.1/setup.cfg
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.452620 nx5d-0.3.1/src/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.458620 nx5d-0.3.1/src/nx5d/
--rw-r--r--   0 florin    (1000) florin    (1000)      117 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)      160 2023-04-17 15:48:04.000000 nx5d-0.3.1/src/nx5d/_version.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     7559 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/edf.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.459620 nx5d-0.3.1/src/nx5d/h5like/
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-04-12 12:44:54.000000 nx5d-0.3.1/src/nx5d/h5like/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)     5686 2023-04-17 15:45:54.000000 nx5d-0.3.1/src/nx5d/h5like/pypod.py
--rw-r--r--   0 florin    (1000) florin    (1000)    10778 2023-04-17 15:45:54.000000 nx5d-0.3.1/src/nx5d/h5like/tools.py
--rw-r--r--   0 florin    (1000) florin    (1000)    31529 2023-04-13 15:04:17.000000 nx5d-0.3.1/src/nx5d/h5like/xfel.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)    15796 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/nx.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     7585 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/runlog.py
--rw-r--r--   0 florin    (1000) florin    (1000)    13662 2023-04-17 15:45:54.000000 nx5d-0.3.1/src/nx5d/scan.py
--rw-r--r--   0 florin    (1000) florin    (1000)     7572 2023-04-17 15:45:54.000000 nx5d-0.3.1/src/nx5d/streaks.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.461620 nx5d-0.3.1/src/nx5d/xrd/
--rw-r--r--   0 florin    (1000) florin    (1000)      756 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/xrd/ColonelSandersFinest.py
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/xrd/__init__.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     4859 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/xrd/analysis.py
--rw-r--r--   0 florin    (1000) florin    (1000)      972 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/xrd/esrf_id09.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1481 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/xrd/experiment-xpp.yml
--rw-r--r--   0 florin    (1000) florin    (1000)     4201 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/xrd/experiment.py
--rw-r--r--   0 florin    (1000) florin    (1000)    13272 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/xrd/kmc3.py
--rw-r--r--   0 florin    (1000) florin    (1000)     4316 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/xrd/roi.py
--rw-r--r--   0 florin    (1000) florin    (1000)    18117 2023-04-17 15:45:54.000000 nx5d-0.3.1/src/nx5d/xrd/signal.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1223 2023-04-17 15:45:54.000000 nx5d-0.3.1/src/nx5d/xrd/xfel.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     3960 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/xrd/xraytest.py
--rw-r--r--   0 florin    (1000) florin    (1000)    15899 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/xrd/xrd_helpers.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.459620 nx5d-0.3.1/src/nx5d.egg-info/
--rw-r--r--   0 florin    (1000) florin    (1000)     3449 2023-04-17 15:48:04.000000 nx5d-0.3.1/src/nx5d.egg-info/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)     7583 2023-04-17 15:48:04.000000 nx5d-0.3.1/src/nx5d.egg-info/SOURCES.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        1 2023-04-17 15:48:04.000000 nx5d-0.3.1/src/nx5d.egg-info/dependency_links.txt
--rw-r--r--   0 florin    (1000) florin    (1000)      113 2023-04-17 15:48:04.000000 nx5d-0.3.1/src/nx5d.egg-info/requires.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        5 2023-04-17 15:48:04.000000 nx5d-0.3.1/src/nx5d.egg-info/top_level.txt
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.462620 nx5d-0.3.1/tests/
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/.gitignore
--rw-r--r--   0 florin    (1000) florin    (1000)      961 2023-04-17 15:45:54.000000 nx5d-0.3.1/tests/pabst_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1559 2023-04-17 15:45:54.000000 nx5d-0.3.1/tests/pypod_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1342 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/runlog_test.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.453620 nx5d-0.3.1/tests/test_data/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.466620 nx5d-0.3.1/tests/test_data/runfile/
--rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/run04.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10599 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/run105.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/run105_brokendata1.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/run105_brokendata2.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/run105_brokenheader.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10588 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/run105_simple.log
--rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04.log
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0001.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0002.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0003.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0004.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0005.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0006.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0007.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0008.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0009.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0010.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0011.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0012.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0013.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0014.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0015.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0016.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0017.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0018.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0019.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0020.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0021.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0022.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0023.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0024.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0025.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0026.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0027.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0028.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0029.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0030.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0031.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0032.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0033.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0034.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0035.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0036.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0037.edf
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.453620 nx5d-0.3.1/tests/test_data/spech5/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.466620 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/
--rw-r--r--   0 florin    (1000) florin    (1000)  1374025 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.453620 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.468620 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/
--rw-r--r--   0 florin    (1000) florin    (1000)    32118 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.474620 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/
--rw-r--r--   0 florin    (1000) florin    (1000)     2133 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2204 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3368 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3429 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3609 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3668 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3827 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4037 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4216 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4322 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4305 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2228 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4165 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3937 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3842 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3835 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3592 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3479 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3270 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3221 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3065 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2427 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2901 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2931 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2707 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2548 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2512 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2306 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2260 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2162 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2078 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2026 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2556 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2013 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2654 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2786 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2845 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3019 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3164 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3341 2023-04-13 14:23:04.000000 nx5d-0.3.1/tests/xfel_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1059 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/xrd_data_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)      915 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/xrd_kmc3_test.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-18 08:04:42.412311 nx5d-0.3.2/
+-rw-r--r--   0 florin    (1000) florin    (1000)       72 2023-04-13 14:23:04.000000 nx5d-0.3.2/.gitignore
+-rw-r--r--   0 florin    (1000) florin    (1000)     3261 2023-04-12 13:31:40.000000 nx5d-0.3.2/.gitlab-ci.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      227 2023-03-15 11:10:41.000000 nx5d-0.3.2/.readthedocs.yaml
+-rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-14 11:33:48.000000 nx5d-0.3.2/COPYING.md
+-rw-r--r--   0 florin    (1000) florin    (1000)     3449 2023-04-18 08:04:42.412311 nx5d-0.3.2/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)     2724 2023-03-27 10:49:57.000000 nx5d-0.3.2/README.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-18 08:04:42.398311 nx5d-0.3.2/doc/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-18 08:04:42.399311 nx5d-0.3.2/doc/mkdocs/
+-rw-r--r--   0 florin    (1000) florin    (1000)       11 2023-03-15 10:15:42.000000 nx5d-0.3.2/doc/mkdocs/about.md
+-rw-r--r--   0 florin    (1000) florin    (1000)      147 2023-04-12 12:52:07.000000 nx5d-0.3.2/doc/mkdocs/api.md
+-rw-r--r--   0 florin    (1000) florin    (1000)    27046 2023-03-27 10:25:44.000000 nx5d-0.3.2/doc/mkdocs/concepts.md
+-rw-r--r--   0 florin    (1000) florin    (1000)     5970 2023-03-25 14:27:00.000000 nx5d-0.3.2/doc/mkdocs/frame.svg
+-rw-r--r--   0 florin    (1000) florin    (1000)     2482 2023-03-27 10:54:07.000000 nx5d-0.3.2/doc/mkdocs/index.md
+-rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-15 10:32:22.000000 nx5d-0.3.2/doc/mkdocs/license.md
+-rw-r--r--   0 florin    (1000) florin    (1000)      723 2023-03-27 10:50:49.000000 nx5d-0.3.2/doc/mkdocs/module-nx.md
+-rw-r--r--   0 florin    (1000) florin    (1000)    36207 2023-03-25 14:25:35.000000 nx5d-0.3.2/doc/mkdocs/scan.svg
+-rw-r--r--   0 florin    (1000) florin    (1000)    25024 2023-03-25 14:49:22.000000 nx5d-0.3.2/doc/mkdocs/streak1.svg
+-rw-r--r--   0 florin    (1000) florin    (1000)    11491 2023-03-25 14:49:37.000000 nx5d-0.3.2/doc/mkdocs/streak2.svg
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-18 08:04:42.400311 nx5d-0.3.2/doc/mkdocs/tutorials/
+-rw-r--r--   0 florin    (1000) florin    (1000)      516 2023-03-15 10:35:31.000000 nx5d-0.3.2/doc/mkdocs/tutorials/index.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-18 08:04:42.400311 nx5d-0.3.2/doc/mkdocs/tutorials/kmc3-data-processing-howto/
+-rw-------   0 florin    (1000) florin    (1000)    44315 2023-03-14 14:52:34.000000 nx5d-0.3.2/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md
+-rw-------   0 florin    (1000) florin    (1000)    19430 2023-03-14 14:52:34.000000 nx5d-0.3.2/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png
+-rw-------   0 florin    (1000) florin    (1000)    25263 2023-03-14 14:52:34.000000 nx5d-0.3.2/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png
+-rw-------   0 florin    (1000) florin    (1000)    23184 2023-03-14 14:52:34.000000 nx5d-0.3.2/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png
+-rw-------   0 florin    (1000) florin    (1000)    13289 2023-03-14 14:52:34.000000 nx5d-0.3.2/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png
+-rw-------   0 florin    (1000) florin    (1000)    16038 2023-03-14 14:52:34.000000 nx5d-0.3.2/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-18 08:04:42.400311 nx5d-0.3.2/doc/mkdocs/tutorials/scansource-howto/
+-rw-r--r--   0 florin    (1000) florin    (1000)     8968 2023-03-14 12:31:08.000000 nx5d-0.3.2/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-18 08:04:42.400311 nx5d-0.3.2/doc/mkdocs/user-guide/
+-rw-r--r--   0 florin    (1000) florin    (1000)      322 2023-04-12 12:48:11.000000 nx5d-0.3.2/doc/mkdocs/user-guide/index.md
+-rw-r--r--   0 florin    (1000) florin    (1000)      513 2023-03-15 14:06:55.000000 nx5d-0.3.2/doc/mkdocs.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      273 2023-03-15 10:49:21.000000 nx5d-0.3.2/mkdocs.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      280 2023-03-14 11:33:48.000000 nx5d-0.3.2/pyproject.toml
+-rw-r--r--   0 florin    (1000) florin    (1000)     2974 2022-08-02 20:02:56.000000 nx5d-0.3.2/scratch.org
+-rw-r--r--   0 florin    (1000) florin    (1000)      900 2023-04-18 08:04:42.412311 nx5d-0.3.2/setup.cfg
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-18 08:04:42.397311 nx5d-0.3.2/src/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-18 08:04:42.401311 nx5d-0.3.2/src/nx5d/
+-rw-r--r--   0 florin    (1000) florin    (1000)      117 2023-03-14 11:33:48.000000 nx5d-0.3.2/src/nx5d/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      160 2023-04-18 08:04:42.000000 nx5d-0.3.2/src/nx5d/_version.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     7559 2023-03-14 11:33:48.000000 nx5d-0.3.2/src/nx5d/edf.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-18 08:04:42.402311 nx5d-0.3.2/src/nx5d/h5like/
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-04-12 12:44:54.000000 nx5d-0.3.2/src/nx5d/h5like/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     5686 2023-04-17 15:45:54.000000 nx5d-0.3.2/src/nx5d/h5like/pypod.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    11246 2023-04-18 08:03:50.000000 nx5d-0.3.2/src/nx5d/h5like/tools.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    31529 2023-04-13 15:04:17.000000 nx5d-0.3.2/src/nx5d/h5like/xfel.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)    15796 2023-03-14 11:33:48.000000 nx5d-0.3.2/src/nx5d/nx.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     7585 2023-03-14 11:33:48.000000 nx5d-0.3.2/src/nx5d/runlog.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    13662 2023-04-17 15:45:54.000000 nx5d-0.3.2/src/nx5d/scan.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     7572 2023-04-17 15:45:54.000000 nx5d-0.3.2/src/nx5d/streaks.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-18 08:04:42.403311 nx5d-0.3.2/src/nx5d/xrd/
+-rw-r--r--   0 florin    (1000) florin    (1000)      756 2023-03-14 11:33:48.000000 nx5d-0.3.2/src/nx5d/xrd/ColonelSandersFinest.py
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-14 11:33:48.000000 nx5d-0.3.2/src/nx5d/xrd/__init__.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     4859 2023-03-14 11:33:48.000000 nx5d-0.3.2/src/nx5d/xrd/analysis.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      972 2023-03-14 11:33:48.000000 nx5d-0.3.2/src/nx5d/xrd/esrf_id09.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1481 2023-03-14 11:33:48.000000 nx5d-0.3.2/src/nx5d/xrd/experiment-xpp.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)     4201 2023-03-14 11:33:48.000000 nx5d-0.3.2/src/nx5d/xrd/experiment.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    13272 2023-03-14 11:33:48.000000 nx5d-0.3.2/src/nx5d/xrd/kmc3.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     4316 2023-03-14 11:33:48.000000 nx5d-0.3.2/src/nx5d/xrd/roi.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    18254 2023-04-18 08:03:50.000000 nx5d-0.3.2/src/nx5d/xrd/signal.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1223 2023-04-18 08:03:50.000000 nx5d-0.3.2/src/nx5d/xrd/xfel.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     3960 2023-03-14 11:33:48.000000 nx5d-0.3.2/src/nx5d/xrd/xraytest.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    15899 2023-03-14 11:33:48.000000 nx5d-0.3.2/src/nx5d/xrd/xrd_helpers.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-18 08:04:42.401311 nx5d-0.3.2/src/nx5d.egg-info/
+-rw-r--r--   0 florin    (1000) florin    (1000)     3449 2023-04-18 08:04:42.000000 nx5d-0.3.2/src/nx5d.egg-info/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)     7583 2023-04-18 08:04:42.000000 nx5d-0.3.2/src/nx5d.egg-info/SOURCES.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        1 2023-04-18 08:04:42.000000 nx5d-0.3.2/src/nx5d.egg-info/dependency_links.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)      113 2023-04-18 08:04:42.000000 nx5d-0.3.2/src/nx5d.egg-info/requires.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        5 2023-04-18 08:04:42.000000 nx5d-0.3.2/src/nx5d.egg-info/top_level.txt
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-18 08:04:42.403311 nx5d-0.3.2/tests/
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/.gitignore
+-rw-r--r--   0 florin    (1000) florin    (1000)      961 2023-04-17 15:45:54.000000 nx5d-0.3.2/tests/pabst_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1559 2023-04-17 15:45:54.000000 nx5d-0.3.2/tests/pypod_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1342 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/runlog_test.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-18 08:04:42.397311 nx5d-0.3.2/tests/test_data/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-18 08:04:42.407311 nx5d-0.3.2/tests/test_data/runfile/
+-rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/run04.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10599 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/run105.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/run105_brokendata1.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/run105_brokendata2.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/run105_brokenheader.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10588 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/run105_simple.log
+-rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04.log
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0001.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0002.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0003.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0004.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0005.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0006.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0007.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0008.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0009.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0010.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0011.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0012.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0013.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0014.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0015.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0016.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0017.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0018.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0019.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0020.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0021.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0022.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0023.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0024.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0025.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0026.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0027.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0028.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0029.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0030.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0031.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0032.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0033.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0034.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0035.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0036.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/runfile/short_run04_0037.edf
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-18 08:04:42.397311 nx5d-0.3.2/tests/test_data/spech5/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-18 08:04:42.407311 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/
+-rw-r--r--   0 florin    (1000) florin    (1000)  1374025 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-18 08:04:42.397311 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-18 08:04:42.408311 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/
+-rw-r--r--   0 florin    (1000) florin    (1000)    32118 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-18 08:04:42.412311 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/
+-rw-r--r--   0 florin    (1000) florin    (1000)     2133 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2204 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3368 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3429 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3609 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3668 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3827 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4037 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4216 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4322 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4305 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2228 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4165 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3937 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3842 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3835 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3592 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3479 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3270 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3221 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3065 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2427 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2901 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2931 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2707 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2548 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2512 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2306 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2260 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2162 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2078 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2026 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2556 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2013 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2654 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2786 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2845 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3019 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3164 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3341 2023-04-13 14:23:04.000000 nx5d-0.3.2/tests/xfel_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1059 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/xrd_data_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      915 2023-03-14 11:33:48.000000 nx5d-0.3.2/tests/xrd_kmc3_test.py
```

### Comparing `nx5d-0.3.1/.gitlab-ci.yml` & `nx5d-0.3.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/COPYING.md` & `nx5d-0.3.2/COPYING.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/PKG-INFO` & `nx5d-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nx5d
-Version: 0.3.1
+Version: 0.3.2
 Summary: NX5 Duct Tape
 Author: Florin Boariu
 Author-email: florin.pt@rootshell.ro
 Project-URL: Source Code, https://gitlab.com/codedump2/nx5d
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/nx5d/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `nx5d-0.3.1/README.md` & `nx5d-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/doc/mkdocs/concepts.md` & `nx5d-0.3.2/doc/mkdocs/concepts.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/doc/mkdocs/frame.svg` & `nx5d-0.3.2/doc/mkdocs/frame.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/doc/mkdocs/index.md` & `nx5d-0.3.2/doc/mkdocs/index.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/doc/mkdocs/license.md` & `nx5d-0.3.2/doc/mkdocs/license.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/doc/mkdocs/module-nx.md` & `nx5d-0.3.2/doc/mkdocs/module-nx.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/doc/mkdocs/scan.svg` & `nx5d-0.3.2/doc/mkdocs/scan.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/doc/mkdocs/streak1.svg` & `nx5d-0.3.2/doc/mkdocs/streak1.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/doc/mkdocs/streak2.svg` & `nx5d-0.3.2/doc/mkdocs/streak2.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/doc/mkdocs/tutorials/index.md` & `nx5d-0.3.2/doc/mkdocs/tutorials/index.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md` & `nx5d-0.3.2/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png` & `nx5d-0.3.2/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png` & `nx5d-0.3.2/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png` & `nx5d-0.3.2/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png` & `nx5d-0.3.2/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png` & `nx5d-0.3.2/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md` & `nx5d-0.3.2/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/doc/mkdocs.yml` & `nx5d-0.3.2/doc/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/scratch.org` & `nx5d-0.3.2/scratch.org`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/setup.cfg` & `nx5d-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/src/nx5d/edf.py` & `nx5d-0.3.2/src/nx5d/edf.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/src/nx5d/h5like/pypod.py` & `nx5d-0.3.2/src/nx5d/h5like/pypod.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/src/nx5d/h5like/tools.py` & `nx5d-0.3.2/src/nx5d/h5like/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,32 +176,42 @@
 
 
         if isinstance(value, str):
             # The main feature: loading data from HDF5 if we encounter an "@..." string.
             # FIXME: need to actually rewrite this and base this on the __call__() feature
             # (see below). This will simplify many things.
 
-            if len(value) == 0 or value[0] != '@':
+            if (len(value) == 0) or (value[0] not in  ['@', '$']):
                 return value
+
+            # Only HDF5 addresses prefixed with '@' will be subject to slicing.
+            # Prefix '$' will take the data verbatim, no slicing.
+            doSlicing = (value[0] == '@')
             
             nodeAddrFmt = value[1:]
             
             try:
                 nodeAddr = nodeAddrFmt.format(**fmtKeys)
 
                 node = h5like[nodeAddr]
 
                 logging.debug("Loading data from %s (only node: %r)" % (nodeAddr, opts.get('nodeOnly', False)))
                 
                 if opts.get('nodeOnly', False):
                     return node
                 else:
                     try:
-                        s = tuple(my_slicer[:len(node.shape)]) if isinstance(my_slicer, tuple) else my_slicer
-                        data = node[s]
+                        if doSlicing:
+                            s = tuple(my_slicer[:len(node.shape)]) if isinstance(my_slicer, tuple) else my_slicer
+                            data = node[s]
+                            #print("Slicing %s: %r" % (value, data))
+                        else:
+                            data = node[()]
+                            #print("Not slicing %s: %r" % (value, data))
+
                         if data.shape[0] == 0 and not opts.get('allowEmpty', False):
                             raise DatasetEmpty
                         return data
                     #except TypeError:  # ...not sure when this happens (?)
                     #    return node
                     except ValueError: # This happens when value is a scalar and needs to be sliced by ()
                         return node[()]
```

### Comparing `nx5d-0.3.1/src/nx5d/h5like/xfel.py` & `nx5d-0.3.2/src/nx5d/h5like/xfel.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/src/nx5d/nx.py` & `nx5d-0.3.2/src/nx5d/nx.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/src/nx5d/runlog.py` & `nx5d-0.3.2/src/nx5d/runlog.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/src/nx5d/scan.py` & `nx5d-0.3.2/src/nx5d/scan.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/src/nx5d/streaks.py` & `nx5d-0.3.2/src/nx5d/streaks.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/src/nx5d/xrd/ColonelSandersFinest.py` & `nx5d-0.3.2/src/nx5d/xrd/ColonelSandersFinest.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/src/nx5d/xrd/analysis.py` & `nx5d-0.3.2/src/nx5d/xrd/analysis.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/src/nx5d/xrd/esrf_id09.py` & `nx5d-0.3.2/src/nx5d/xrd/esrf_id09.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/src/nx5d/xrd/experiment-xpp.yml` & `nx5d-0.3.2/src/nx5d/xrd/experiment-xpp.yml`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/src/nx5d/xrd/experiment.py` & `nx5d-0.3.2/src/nx5d/xrd/experiment.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/src/nx5d/xrd/kmc3.py` & `nx5d-0.3.2/src/nx5d/xrd/kmc3.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/src/nx5d/xrd/roi.py` & `nx5d-0.3.2/src/nx5d/xrd/roi.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/src/nx5d/xrd/signal.py` & `nx5d-0.3.2/src/nx5d/xrd/signal.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,21 +264,23 @@
           - from an array or tuple (2, N)
         '''
         if not hasattr(data, "__len__"):
             raise RuntimeError("%s: needs to be a 2-tuple" % name)
         
         if len(data) == 2:
             if hasattr(data[0], "__len__"):
-                return np.array([data[0][0], data[1][0]])
+                return ([data[0][0], data[1][0]])
             else:
-                return np.array([data[0], data[1]])
+                return ([data[0], data[1]])
 
         if len(data) > 2:
             return data[0]
 
+        raise RuntimeError("Oops: don't know how to handle %s: %r" % (name, data))
+
         
 
 
     def __init_experiment(self, setup):
         '''
         Initializes the Experiment part (i.e. xrayutilities HXRD object etc)
         with specified device and sample geometry. The optional parameter `roi`
@@ -306,16 +308,16 @@
         hxrd = xu.HXRD(idir=setup['beamDirection'],
                        ndir=setup['sampleNormal'],
                        sampleor=setup['sampleFaceUp'],
                        qconv=qconv,
                        # Workaround for buggy xrayutilities: repeat the beam energy
                        en=beamEnergy)
 
-        imageCenter = self.__2tuple(setup['imageCenter'])
-        imageSize = self.__2tuple(setup['imageSize'])
+        imageCenter = self.__2tuple(setup['imageCenter'], 'imageCenter')
+        imageSize = self.__2tuple(setup['imageSize'], 'imageSize')
         imageDistance = setup['imageDistance'][0] \
             if hasattr(setup['imageDistance'], "__len__") \
                else setup['imageDistance']
 
         logging.debug("image distance %r, size %r, center at %r" % (imageDistance, imageSize, imageCenter))
         
         if imageCenter[0] <= 1 and imageCenter[1] <= 1:
@@ -329,23 +331,23 @@
             assert imgs[0] is not None
             assert imgs[1] is not None            
             imageCenter = tuple([c*s for c,s in zip(setup['imageCenter'], imgs)])
 
         chSizeParm = {}
         if ('imageChannelSpan' in setup) and (setup['imageChannelSpan'] is not None):
             # channelSpan is degrees/channel, but we need to pass channels/degree to Ang2Q
-            imageChannelSize = self.__2tuple(setup['imageChannelSpan'])
+            imageChannelSize = self.__2tuple(setup['imageChannelSpan'], 'imageChannelSpan')
             chSizeParm = {'chpdeg1': 1.0/imageChannelSpan[0],
                           'chpdeg1': 1.0/imageChannelSpan[1] }
 
         elif ('imageChannelSize' in setup) and (setup['imageChannelSize'] is not None):
             # Ang2Q takes one explicit distance parameter, but we're assuming that channelSize
             # is relative to the distance itself (putting the distance always at 1.0 units)
-            imageChannelSize = self.__2tuple(setup['imageChannelSize'])
-            logging.warn("pixel size: %r" % (imageChannelSize,))
+            imageChannelSize = self.__2tuple(setup['imageChannelSize'], 'imageChannelSize')
+            logging.debug("pixel size: %r" % (imageChannelSize,))
             chSizeParm = { 'pwidth1':  imageChannelSize[0],
                            'pwidth2':  imageChannelSize[1],
                            'distance': imageDistance }
 
         else:
             raise RuntimeError("Experiment setup needs either the channel span or channel size")
```

### Comparing `nx5d-0.3.1/src/nx5d/xrd/xfel.py` & `nx5d-0.3.2/src/nx5d/xrd/xfel.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     "goniometerAxes": ('y-', 'z+', 'x+'),
     
     "detectorTARAxes": ('x+', None, None),
 
     # These were correct for the AGIPD1M detector at one point in time.
     # Might change over time, so you might need to adjust them.
     "imageAxes": ("x+", "y-"),
-    "imageSize": "@/detector_size",
-    "imageCenter": "@/detector_centre",
+    "imageSize": "$/detector_size",
+    "imageCenter": "$/detector_centre",
 
     # same unit as imageChannelSize
     "imageDistance": "@/sdd",
 
     # same unit as imageDistance (mm)    
     "imageChannelSize": ("@/pixel_size", "@/pixel_size"),
 
@@ -32,16 +32,16 @@
     "beamDirection": (0, 1, 0),
     
     "sampleNormal": (0, 0, 1),
     
     "beamEnergy": "@/photon_energy",
 
     "goniometerAngles": {
-        'omega': '@/omega',
+        '2theta': '@/twotheta',
         'chi': '@/chi',
         'phi': '@/phi',
     },
 
     "detectorTARAngles": {
-        '2theta': '@/twotheta',
+        'omega': '@/omega',
     },
 }
```

### Comparing `nx5d-0.3.1/src/nx5d/xrd/xraytest.py` & `nx5d-0.3.2/src/nx5d/xrd/xraytest.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/src/nx5d/xrd/xrd_helpers.py` & `nx5d-0.3.2/src/nx5d/xrd/xrd_helpers.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/src/nx5d.egg-info/PKG-INFO` & `nx5d-0.3.2/src/nx5d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nx5d
-Version: 0.3.1
+Version: 0.3.2
 Summary: NX5 Duct Tape
 Author: Florin Boariu
 Author-email: florin.pt@rootshell.ro
 Project-URL: Source Code, https://gitlab.com/codedump2/nx5d
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/nx5d/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `nx5d-0.3.1/src/nx5d.egg-info/SOURCES.txt` & `nx5d-0.3.2/src/nx5d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/pabst_test.py` & `nx5d-0.3.2/tests/pabst_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/pypod_test.py` & `nx5d-0.3.2/tests/pypod_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/runlog_test.py` & `nx5d-0.3.2/tests/runlog_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/run04.log` & `nx5d-0.3.2/tests/test_data/runfile/run04.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/run105.log` & `nx5d-0.3.2/tests/test_data/runfile/run105.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/run105_brokendata1.log` & `nx5d-0.3.2/tests/test_data/runfile/run105_brokendata1.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/run105_brokendata2.log` & `nx5d-0.3.2/tests/test_data/runfile/run105_brokendata2.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/run105_brokenheader.log` & `nx5d-0.3.2/tests/test_data/runfile/run105_brokenheader.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/run105_simple.log` & `nx5d-0.3.2/tests/test_data/runfile/run105_simple.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04.log` & `nx5d-0.3.2/tests/test_data/runfile/short_run04.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0001.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0001.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0002.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0002.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0003.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0003.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0004.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0004.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0005.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0005.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0006.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0006.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0007.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0007.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0008.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0008.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0009.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0009.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0010.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0010.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0011.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0011.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0012.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0012.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0013.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0013.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0014.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0014.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0015.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0015.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0016.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0016.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0017.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0017.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0018.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0018.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0019.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0019.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0020.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0020.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0021.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0021.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0022.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0022.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0023.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0023.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0024.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0024.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0025.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0025.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0026.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0026.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0027.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0027.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0028.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0028.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0029.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0029.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0030.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0030.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0031.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0031.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0032.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0032.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0033.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0033.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0034.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0034.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0035.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0035.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0036.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0036.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/runfile/short_run04_0037.edf` & `nx5d-0.3.2/tests/test_data/runfile/short_run04_0037.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif` & `nx5d-0.3.2/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/xfel_test.py` & `nx5d-0.3.2/tests/xfel_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/xrd_data_test.py` & `nx5d-0.3.2/tests/xrd_data_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.1/tests/xrd_kmc3_test.py` & `nx5d-0.3.2/tests/xrd_kmc3_test.py`

 * *Files identical despite different names*

