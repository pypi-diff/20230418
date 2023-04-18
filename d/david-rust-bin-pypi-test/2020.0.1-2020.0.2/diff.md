# Comparing `tmp/david-rust-bin-pypi-test-2020.0.1.tar.gz` & `tmp/david-rust-bin-pypi-test-2020.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "david-rust-bin-pypi-test-2020.0.1.tar", last modified: Tue Apr 18 05:02:21 2023, max compression
+gzip compressed data, was "david-rust-bin-pypi-test-2020.0.2.tar", last modified: Tue Apr 18 05:07:01 2023, max compression
```

## Comparing `david-rust-bin-pypi-test-2020.0.1.tar` & `david-rust-bin-pypi-test-2020.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 05:02:21.544100 david-rust-bin-pypi-test-2020.0.1/
--rw-rw-rw-   0        0        0       74 2023-04-18 05:02:21.540384 david-rust-bin-pypi-test-2020.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-04-18 04:58:43.000000 david-rust-bin-pypi-test-2020.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 05:02:21.544100 david-rust-bin-pypi-test-2020.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-18 05:02:21.506068 david-rust-bin-pypi-test-2020.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-18 05:02:21.537365 david-rust-bin-pypi-test-2020.0.1/src/david_rust_bin_pypi_test.egg-info/
--rw-rw-rw-   0        0        0       74 2023-04-18 05:02:21.000000 david-rust-bin-pypi-test-2020.0.1/src/david_rust_bin_pypi_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-04-18 05:02:21.000000 david-rust-bin-pypi-test-2020.0.1/src/david_rust_bin_pypi_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 05:02:21.000000 david-rust-bin-pypi-test-2020.0.1/src/david_rust_bin_pypi_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 05:02:21.000000 david-rust-bin-pypi-test-2020.0.1/src/david_rust_bin_pypi_test.egg-info/top_level.txt
--rwxrwxrwx   0        0        0   160256 2023-04-18 01:46:57.000000 david-rust-bin-pypi-test-2020.0.1/src/rust_proj.exe
+drwxrwxrwx   0        0        0        0 2023-04-18 05:07:01.883387 david-rust-bin-pypi-test-2020.0.2/
+-rw-rw-rw-   0        0        0       74 2023-04-18 05:07:01.882373 david-rust-bin-pypi-test-2020.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-04-18 05:06:22.000000 david-rust-bin-pypi-test-2020.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 05:07:01.884370 david-rust-bin-pypi-test-2020.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 05:07:01.848420 david-rust-bin-pypi-test-2020.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 05:07:01.878131 david-rust-bin-pypi-test-2020.0.2/src/david_rust_bin_pypi_test.egg-info/
+-rw-rw-rw-   0        0        0       74 2023-04-18 05:07:01.000000 david-rust-bin-pypi-test-2020.0.2/src/david_rust_bin_pypi_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-04-18 05:07:01.000000 david-rust-bin-pypi-test-2020.0.2/src/david_rust_bin_pypi_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 05:07:01.000000 david-rust-bin-pypi-test-2020.0.2/src/david_rust_bin_pypi_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 05:07:01.000000 david-rust-bin-pypi-test-2020.0.2/src/david_rust_bin_pypi_test.egg-info/top_level.txt
+-rwxrwxrwx   0        0        0   160256 2023-04-18 01:46:57.000000 david-rust-bin-pypi-test-2020.0.2/src/rust_proj.exe
```

### Comparing `david-rust-bin-pypi-test-2020.0.1/src/rust_proj.exe` & `david-rust-bin-pypi-test-2020.0.2/src/rust_proj.exe`

 * *Files identical despite different names*

