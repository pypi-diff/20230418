# Comparing `tmp/ephysiopy-1.8.97.tar.gz` & `tmp/ephysiopy-1.8.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephysiopy-1.8.97.tar", last modified: Thu Apr  6 14:50:32 2023, max compression
+gzip compressed data, was "ephysiopy-1.8.98.tar", last modified: Tue Apr 18 15:56:53 2023, max compression
```

## Comparing `ephysiopy-1.8.97.tar` & `ephysiopy-1.8.98.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:50:32.900210 ephysiopy-1.8.97/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-06 14:50:32.900210 ephysiopy-1.8.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:50:32.896209 ephysiopy-1.8.97/ephysiopy/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:50:32.896209 ephysiopy-1.8.97/ephysiopy/axona/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/axona/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/axona/axonaIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/axona/file_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/axona/tetrode_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/axona/tintcolours.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:50:32.896209 ephysiopy-1.8.97/ephysiopy/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31243 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/common/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/common/ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/common/fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/common/gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/common/mle_von_mises_vals.py
--rw-r--r--   0 runner    (1001) docker     (123)    49463 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/common/phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/common/rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)    28784 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/common/spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/common/statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:50:32.896209 ephysiopy-1.8.97/ephysiopy/format_converters/
--rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/format_converters/OE_Axona.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/format_converters/OE_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/format_converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:50:32.896209 ephysiopy-1.8.97/ephysiopy/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21861 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/io/recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:50:32.896209 ephysiopy-1.8.97/ephysiopy/openephys2py/
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/openephys2py/KiloSort.py
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/openephys2py/OESettings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/openephys2py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:50:32.900210 ephysiopy-1.8.97/ephysiopy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/tests/test_axona_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/tests/test_axona_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/tests/test_binning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/tests/test_dacq2py.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/tests/test_ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/tests/test_fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/tests/test_gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/tests/test_openephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/tests/test_phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/tests/test_rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/tests/test_spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/tests/test_statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:50:32.900210 ephysiopy-1.8.97/ephysiopy/visualise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/visualise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31481 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/ephysiopy/visualise/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:50:32.896209 ephysiopy-1.8.97/ephysiopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-06 14:50:32.000000 ephysiopy-1.8.97/ephysiopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-06 14:50:32.000000 ephysiopy-1.8.97/ephysiopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 14:50:32.000000 ephysiopy-1.8.97/ephysiopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-06 14:50:32.000000 ephysiopy-1.8.97/ephysiopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-06 14:50:32.000000 ephysiopy-1.8.97/ephysiopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-06 14:50:32.900210 ephysiopy-1.8.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-06 14:50:24.000000 ephysiopy-1.8.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:53.204770 ephysiopy-1.8.98/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-18 15:56:53.204770 ephysiopy-1.8.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:53.200770 ephysiopy-1.8.98/ephysiopy/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:53.200770 ephysiopy-1.8.98/ephysiopy/axona/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/axona/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/axona/axonaIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/axona/file_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/axona/tetrode_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/axona/tintcolours.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:53.200770 ephysiopy-1.8.98/ephysiopy/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31243 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/mle_von_mises_vals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49463 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28784 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:53.200770 ephysiopy-1.8.98/ephysiopy/format_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/format_converters/OE_Axona.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/format_converters/OE_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/format_converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:53.200770 ephysiopy-1.8.98/ephysiopy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21861 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/io/recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:53.200770 ephysiopy-1.8.98/ephysiopy/openephys2py/
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/openephys2py/KiloSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/openephys2py/OESettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/openephys2py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:53.204770 ephysiopy-1.8.98/ephysiopy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_axona_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_axona_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_dacq2py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_openephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:53.204770 ephysiopy-1.8.98/ephysiopy/visualise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/visualise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32398 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/visualise/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:53.200770 ephysiopy-1.8.98/ephysiopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-18 15:56:53.000000 ephysiopy-1.8.98/ephysiopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-18 15:56:53.000000 ephysiopy-1.8.98/ephysiopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:56:53.000000 ephysiopy-1.8.98/ephysiopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-18 15:56:53.000000 ephysiopy-1.8.98/ephysiopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 15:56:53.000000 ephysiopy-1.8.98/ephysiopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-18 15:56:53.204770 ephysiopy-1.8.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/setup.py
```

### Comparing `ephysiopy-1.8.97/LICENSE` & `ephysiopy-1.8.98/LICENSE`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/PKG-INFO` & `ephysiopy-1.8.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.8.97
+Version: 1.8.98
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.8.97/README.md` & `ephysiopy-1.8.98/README.md`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/axona/axonaIO.py` & `ephysiopy-1.8.98/ephysiopy/axona/axonaIO.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/axona/file_headers.py` & `ephysiopy-1.8.98/ephysiopy/axona/file_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/axona/tetrode_dict.py` & `ephysiopy-1.8.98/ephysiopy/axona/tetrode_dict.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/axona/tintcolours.py` & `ephysiopy-1.8.98/ephysiopy/axona/tintcolours.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/common/binning.py` & `ephysiopy-1.8.98/ephysiopy/common/binning.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/common/ephys_generic.py` & `ephysiopy-1.8.98/ephysiopy/common/ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/common/fieldcalcs.py` & `ephysiopy-1.8.98/ephysiopy/common/fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/common/gridcell.py` & `ephysiopy-1.8.98/ephysiopy/common/gridcell.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/common/mle_von_mises_vals.py` & `ephysiopy-1.8.98/ephysiopy/common/mle_von_mises_vals.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/common/phasecoding.py` & `ephysiopy-1.8.98/ephysiopy/common/phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/common/rhythmicity.py` & `ephysiopy-1.8.98/ephysiopy/common/rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/common/spikecalcs.py` & `ephysiopy-1.8.98/ephysiopy/common/spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/common/statscalcs.py` & `ephysiopy-1.8.98/ephysiopy/common/statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/common/utils.py` & `ephysiopy-1.8.98/ephysiopy/common/utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/format_converters/OE_Axona.py` & `ephysiopy-1.8.98/ephysiopy/format_converters/OE_Axona.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/format_converters/OE_numpy.py` & `ephysiopy-1.8.98/ephysiopy/format_converters/OE_numpy.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/io/recording.py` & `ephysiopy-1.8.98/ephysiopy/io/recording.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/openephys2py/KiloSort.py` & `ephysiopy-1.8.98/ephysiopy/openephys2py/KiloSort.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/openephys2py/OESettings.py` & `ephysiopy-1.8.98/ephysiopy/openephys2py/OESettings.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/tests/conftest.py` & `ephysiopy-1.8.98/ephysiopy/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/tests/test_axona_headers.py` & `ephysiopy-1.8.98/ephysiopy/tests/test_axona_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/tests/test_axona_io.py` & `ephysiopy-1.8.98/ephysiopy/tests/test_axona_io.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/tests/test_binning.py` & `ephysiopy-1.8.98/ephysiopy/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/tests/test_dacq2py.py` & `ephysiopy-1.8.98/ephysiopy/tests/test_dacq2py.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/tests/test_ephys_generic.py` & `ephysiopy-1.8.98/ephysiopy/tests/test_ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/tests/test_fieldcalcs.py` & `ephysiopy-1.8.98/ephysiopy/tests/test_fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/tests/test_gridcell.py` & `ephysiopy-1.8.98/ephysiopy/tests/test_gridcell.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/tests/test_phasecoding.py` & `ephysiopy-1.8.98/ephysiopy/tests/test_phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/tests/test_rhythmicity.py` & `ephysiopy-1.8.98/ephysiopy/tests/test_rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/tests/test_spikecalcs.py` & `ephysiopy-1.8.98/ephysiopy/tests/test_spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/tests/test_statscalcs.py` & `ephysiopy-1.8.98/ephysiopy/tests/test_statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/tests/test_utils.py` & `ephysiopy-1.8.98/ephysiopy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/ephysiopy/visualise/plotting.py` & `ephysiopy-1.8.98/ephysiopy/visualise/plotting.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-import matplotlib.pylab as plt
+import functools
+
 import matplotlib
+import matplotlib.pylab as plt
+import matplotlib.transforms as transforms
 import numpy as np
-import functools
+from matplotlib.patches import Rectangle
+from mpl_toolkits.axes_grid1 import make_axes_locatable
+
+from ephysiopy.axona import tintcolours as tcols
 from ephysiopy.common.binning import RateMap
 from ephysiopy.common.spikecalcs import SpikeCalcsGeneric
-from ephysiopy.axona import tintcolours as tcols
-from mpl_toolkits.axes_grid1 import make_axes_locatable
-import matplotlib.transforms as transforms
-from matplotlib.patches import Rectangle
 
 
 # Decorators
 def stripAxes(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         ax = func(*args, **kwargs)
@@ -550,14 +552,17 @@
         all_ax.set_ylim((inDict['dist_to_centre'].shape[0]-.5, -.5))
         return ax
 
     def plotSpectrogramByDepth(self,
                                nchannels: int = 384,
                                nseconds: int = 100,
                                maxFreq: int = 125,
+                               channels: list = [],
+                               frequencies: list = [],
+                               frequencyIncrement: int = 1,
                                **kwargs):
         """
         Plots a heat map spectrogram of the LFP for each channel.
         Line plots of power per frequency band and power on a subset of
         channels are also displayed to the right and above the main plot.
         Parameters
         ----------
@@ -566,14 +571,22 @@
         nseconds : int, optional
             How long in seconds from the start of the trial to do
             the spectrogram for (for speed).
             Default 100
         maxFreq : int
             The maximum frequency in Hz to plot the spectrogram out to.
             Maximum 1250. Default 125
+        channels: list
+            The channels to plot separately on the top plot
+        frequencies: list
+            The specific frequencies to examine across
+            all channels. The mean from frequency: frequency+frequencyIncrement
+            is calculated and plotted on the left hand side of the plot
+        frequencyIncrement: int
+            The amount to add to each value of the frequencies list above
         kwargs: valid key value pairs:
             "saveas" - save the figure to this location, needs absolute
             path and filename
 
         Notes
         -----
         Should also allow kwargs to specify exactly which channels
@@ -629,33 +642,43 @@
         meanfreq_powerAx = divider.append_axes("right",
                                                1.2,
                                                pad=0.1,
                                                sharey=spectoAx)
         plt.setp(channel_spectoAx.get_xticklabels() +
                  meanfreq_powerAx.get_yticklabels(), visible=False)
 
+        # plot mean power across some channels
         mn_power = np.mean(spec_data, 0)
-        cols = iter(cm.rainbow(np.linspace(0, 1, (nchannels//60)+1)))
-        for i in range(0, spec_data.shape[0], 60):
+        if not channels:
+            channels = range(1, nchannels, 60)
+        cols = iter(cm.rainbow(np.linspace(0, 1, len(channels))))
+        for chan in channels:
             c = next(cols)
             channel_spectoAx.plot(E.freqs[0::50],
-                                  10*np.log10(spec_data[i, :]/mn_power),
+                                  10*np.log10(spec_data[chan, :]/mn_power),
                                   c=c,
-                                  label=str(i))
+                                  label=str(chan))
 
         channel_spectoAx.set_ylabel('Channel power(dB)')
         channel_spectoAx.legend(bbox_to_anchor=(0., 1.02, 1., .102),
                                 loc='lower left',
                                 mode='expand',
                                 fontsize='x-small',
                                 ncol=4)
 
-        freq_inc = 6
-        lower_freqs = np.arange(1, maxFreq-freq_inc, freq_inc)
-        upper_freqs = np.arange(1+freq_inc, maxFreq, freq_inc)
+        # plot mean frequencies across all channels
+        if not frequencyIncrement:
+            freq_inc = 6
+        else:
+            freq_inc = frequencyIncrement
+        if not frequencies:
+            lower_freqs = np.arange(1, maxFreq-freq_inc, freq_inc)
+        else:
+            lower_freqs = frequencies
+        upper_freqs = [f + freq_inc for f in lower_freqs]
         cols = iter(cm.nipy_spectral(np.linspace(0, 1, len(upper_freqs))))
         mn_power = np.mean(spec_data, 1)
         for freqs in zip(lower_freqs, upper_freqs):
             freq_mask = np.logical_and(
                 E.freqs[0::50] > freqs[0], E.freqs[0::50] < freqs[1])
             mean_power = 10*np.log10(
                 np.mean(spec_data[:, freq_mask], 1) / mn_power)
```

### Comparing `ephysiopy-1.8.97/ephysiopy.egg-info/PKG-INFO` & `ephysiopy-1.8.98/ephysiopy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.8.97
+Version: 1.8.98
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.8.97/ephysiopy.egg-info/SOURCES.txt` & `ephysiopy-1.8.98/ephysiopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.97/setup.py` & `ephysiopy-1.8.98/setup.py`

 * *Files identical despite different names*

