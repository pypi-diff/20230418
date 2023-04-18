# Comparing `tmp/david-rust-bin-pypi-test-2020.0.0.tar.gz` & `tmp/david-rust-bin-pypi-test-2020.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "david-rust-bin-pypi-test-2020.0.0.tar", last modified: Tue Apr 18 04:49:02 2023, max compression
+gzip compressed data, was "david-rust-bin-pypi-test-2020.0.1.tar", last modified: Tue Apr 18 05:02:21 2023, max compression
```

## Comparing `david-rust-bin-pypi-test-2020.0.0.tar` & `david-rust-bin-pypi-test-2020.0.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 04:49:02.768582 david-rust-bin-pypi-test-2020.0.0/
--rw-rw-rw-   0        0        0       21 2023-04-18 04:43:32.000000 david-rust-bin-pypi-test-2020.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0       74 2023-04-18 04:49:02.766469 david-rust-bin-pypi-test-2020.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-04-18 03:04:05.000000 david-rust-bin-pypi-test-2020.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 04:49:02.768582 david-rust-bin-pypi-test-2020.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-18 04:49:02.745953 david-rust-bin-pypi-test-2020.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-18 04:49:02.763648 david-rust-bin-pypi-test-2020.0.0/src/david_rust_bin_pypi_test.egg-info/
--rw-rw-rw-   0        0        0       74 2023-04-18 04:49:02.000000 david-rust-bin-pypi-test-2020.0.0/src/david_rust_bin_pypi_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-04-18 04:49:02.000000 david-rust-bin-pypi-test-2020.0.0/src/david_rust_bin_pypi_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 04:49:02.000000 david-rust-bin-pypi-test-2020.0.0/src/david_rust_bin_pypi_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 04:49:02.000000 david-rust-bin-pypi-test-2020.0.0/src/david_rust_bin_pypi_test.egg-info/top_level.txt
--rwxrwxrwx   0        0        0   160256 2023-04-18 01:46:57.000000 david-rust-bin-pypi-test-2020.0.0/src/rust_proj.exe
+drwxrwxrwx   0        0        0        0 2023-04-18 05:02:21.544100 david-rust-bin-pypi-test-2020.0.1/
+-rw-rw-rw-   0        0        0       74 2023-04-18 05:02:21.540384 david-rust-bin-pypi-test-2020.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-04-18 04:58:43.000000 david-rust-bin-pypi-test-2020.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 05:02:21.544100 david-rust-bin-pypi-test-2020.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 05:02:21.506068 david-rust-bin-pypi-test-2020.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 05:02:21.537365 david-rust-bin-pypi-test-2020.0.1/src/david_rust_bin_pypi_test.egg-info/
+-rw-rw-rw-   0        0        0       74 2023-04-18 05:02:21.000000 david-rust-bin-pypi-test-2020.0.1/src/david_rust_bin_pypi_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-04-18 05:02:21.000000 david-rust-bin-pypi-test-2020.0.1/src/david_rust_bin_pypi_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 05:02:21.000000 david-rust-bin-pypi-test-2020.0.1/src/david_rust_bin_pypi_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 05:02:21.000000 david-rust-bin-pypi-test-2020.0.1/src/david_rust_bin_pypi_test.egg-info/top_level.txt
+-rwxrwxrwx   0        0        0   160256 2023-04-18 01:46:57.000000 david-rust-bin-pypi-test-2020.0.1/src/rust_proj.exe
```

### Comparing `david-rust-bin-pypi-test-2020.0.0/src/rust_proj.exe` & `david-rust-bin-pypi-test-2020.0.1/src/rust_proj.exe`

 * *Files identical despite different names*

