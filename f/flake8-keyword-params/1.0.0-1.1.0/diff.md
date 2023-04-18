# Comparing `tmp/flake8-keyword-params-1.0.0.tar.gz` & `tmp/flake8-keyword-params-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-keyword-params-1.0.0.tar", last modified: Sun Apr 16 01:02:04 2023, max compression
+gzip compressed data, was "flake8-keyword-params-1.1.0.tar", last modified: Tue Apr 18 01:43:36 2023, max compression
```

## Comparing `flake8-keyword-params-1.0.0.tar` & `flake8-keyword-params-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 01:02:04.168822 flake8-keyword-params-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-04-16 00:54:26.000000 flake8-keyword-params-1.0.0/.editorconfig
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-04-16 00:54:26.000000 flake8-keyword-params-1.0.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-04-16 00:54:26.000000 flake8-keyword-params-1.0.0/.gitlab-ci.env
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-16 00:54:26.000000 flake8-keyword-params-1.0.0/.gitlab-ci.yaml
--rw-rw-rw-   0 root         (0) root         (0)      260 2023-04-16 00:54:26.000000 flake8-keyword-params-1.0.0/.yamllint.yaml
--rw-r--r--   0 root         (0) root         (0)     1783 2023-04-16 01:02:04.168822 flake8-keyword-params-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      700 2023-04-16 01:00:42.000000 flake8-keyword-params-1.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-16 00:54:26.000000 flake8-keyword-params-1.0.0/flake8-keyword-params.sublime-project
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 01:02:04.164822 flake8-keyword-params-1.0.0/flake8_keyword_params/
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-16 00:54:26.000000 flake8-keyword-params-1.0.0/flake8_keyword_params/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3969 2023-04-16 00:54:26.000000 flake8-keyword-params-1.0.0/flake8_keyword_params/checker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 01:02:04.168822 flake8-keyword-params-1.0.0/flake8_keyword_params.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1783 2023-04-16 01:02:04.000000 flake8-keyword-params-1.0.0/flake8_keyword_params.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2023-04-16 01:02:04.000000 flake8-keyword-params-1.0.0/flake8_keyword_params.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 01:02:04.000000 flake8-keyword-params-1.0.0/flake8_keyword_params.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-04-16 01:02:04.000000 flake8-keyword-params-1.0.0/flake8_keyword_params.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-04-16 01:02:04.000000 flake8-keyword-params-1.0.0/flake8_keyword_params.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-16 01:02:04.000000 flake8-keyword-params-1.0.0/flake8_keyword_params.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2293 2023-04-16 00:54:26.000000 flake8-keyword-params-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 01:02:04.168822 flake8-keyword-params-1.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:43:36.611959 flake8-keyword-params-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.0/.editorconfig
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.0/.gitlab-ci.env
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.0/.gitlab-ci.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      260 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.0/.yamllint.yaml
+-rw-r--r--   0 root         (0) root         (0)     3475 2023-04-18 01:43:36.611959 flake8-keyword-params-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2392 2023-04-18 01:40:25.000000 flake8-keyword-params-1.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.0/flake8-keyword-params.sublime-project
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:43:36.607959 flake8-keyword-params-1.1.0/flake8_keyword_params/
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.0/flake8_keyword_params/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7182 2023-04-18 01:40:25.000000 flake8-keyword-params-1.1.0/flake8_keyword_params/checker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:43:36.611959 flake8-keyword-params-1.1.0/flake8_keyword_params.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3475 2023-04-18 01:43:36.000000 flake8-keyword-params-1.1.0/flake8_keyword_params.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2023-04-18 01:43:36.000000 flake8-keyword-params-1.1.0/flake8_keyword_params.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 01:43:36.000000 flake8-keyword-params-1.1.0/flake8_keyword_params.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-04-18 01:43:36.000000 flake8-keyword-params-1.1.0/flake8_keyword_params.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-04-18 01:43:36.000000 flake8-keyword-params-1.1.0/flake8_keyword_params.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-18 01:43:36.000000 flake8-keyword-params-1.1.0/flake8_keyword_params.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2293 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 01:43:36.611959 flake8-keyword-params-1.1.0/setup.cfg
```

### Comparing `flake8-keyword-params-1.0.0/pyproject.toml` & `flake8-keyword-params-1.1.0/pyproject.toml`

 * *Files identical despite different names*

