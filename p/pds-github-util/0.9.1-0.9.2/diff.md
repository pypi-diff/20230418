# Comparing `tmp/pds_github_util-0.9.1.tar.gz` & `tmp/pds_github_util-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pds_github_util-0.9.1.tar", last modified: Thu Jul  9 23:16:00 2020, max compression
+gzip compressed data, was "dist/pds_github_util-0.9.2.tar", last modified: Thu Jul  9 23:56:54 2020, max compression
```

## Comparing `pds_github_util-0.9.1.tar` & `pds_github_util-0.9.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (116)     3779 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2366 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/pds_github_util/
--rw-r--r--   0 runner    (1001) docker     (116)       19 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/pds_github_util/branches/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/branches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1884 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/branches/git_actions.py
--rw-r--r--   0 runner    (1001) docker     (116)      812 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/branches/git_ping.py
--rw-r--r--   0 runner    (1001) docker     (116)      862 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/build_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/pds_github_util/corral/
--rw-r--r--   0 runner    (1001) docker     (116)       59 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/corral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4549 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/corral/cattle_head.py
--rw-r--r--   0 runner    (1001) docker     (116)     2593 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/corral/herd.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/pds_github_util/gh_pages/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/gh_pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2462 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/gh_pages/build_summaries.py
--rw-r--r--   0 runner    (1001) docker     (116)     2821 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/gh_pages/root_index.py
--rw-r--r--   0 runner    (1001) docker     (116)     1910 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/gh_pages/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/pds_github_util/html/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      696 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/html/md_to_html.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/pds_github_util/release/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1275 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/release/maven_snapshot_release.py
--rw-r--r--   0 runner    (1001) docker     (116)     3014 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/release/python_snapshot_release.py
--rw-r--r--   0 runner    (1001) docker     (116)     2111 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/release/snapshot_release.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/pds_github_util/requirements/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/requirements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1662 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/requirements/generate_requirements.py
--rw-r--r--   0 runner    (1001) docker     (116)     6179 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/requirements/requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/pds_github_util/tags/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1697 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/tags/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/pds_github_util/versions/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1383 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/pds_github_util/versions/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/pds_github_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3779 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/pds_github_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1687 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/pds_github_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/pds_github_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      431 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/pds_github_util.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      151 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/pds_github_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       22 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/pds_github_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       49 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2074 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/tests/branches/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/tests/branches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      457 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/tests/branches/git-actions_test.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/tests/corral/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/tests/corral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      437 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/tests/corral/grab_versions_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     1208 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/tests/corral/summary_test.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/tests/gh_pages/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/tests/gh_pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      283 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/tests/gh_pages/build_summaries_test.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/tests/releases/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/tests/releases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      705 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/tests/releases/maven_get_version_test.py
--rw-r--r--   0 runner    (1001) docker     (116)      771 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/tests/releases/python_get_version_test.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/tests/requirements/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/tests/requirements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1424 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/tests/requirements/requirements_test.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:16:00.000000 pds_github_util-0.9.1/tests/tags/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/tests/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      529 2020-07-09 23:14:48.000000 pds_github_util-0.9.1/tests/tags/tags_test.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (116)     3779 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2366 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/pds_github_util/
+-rw-r--r--   0 runner    (1001) docker     (116)       19 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/pds_github_util/branches/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/branches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1884 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/branches/git_actions.py
+-rw-r--r--   0 runner    (1001) docker     (116)      812 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/branches/git_ping.py
+-rw-r--r--   0 runner    (1001) docker     (116)      862 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/build_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/pds_github_util/corral/
+-rw-r--r--   0 runner    (1001) docker     (116)       59 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/corral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4549 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/corral/cattle_head.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2593 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/corral/herd.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/pds_github_util/gh_pages/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/gh_pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2462 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/gh_pages/build_summaries.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3030 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/gh_pages/root_index.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1910 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/gh_pages/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/pds_github_util/html/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      696 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/html/md_to_html.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/pds_github_util/release/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1275 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/release/maven_snapshot_release.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3014 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/release/python_snapshot_release.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2111 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/release/snapshot_release.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/pds_github_util/requirements/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/requirements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1662 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/requirements/generate_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6179 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/requirements/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/pds_github_util/tags/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1697 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/tags/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/pds_github_util/versions/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1383 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/pds_github_util/versions/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/pds_github_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     3779 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/pds_github_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1687 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/pds_github_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/pds_github_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      431 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/pds_github_util.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      151 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/pds_github_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       22 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/pds_github_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       49 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     2074 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/tests/branches/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/tests/branches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      457 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/tests/branches/git-actions_test.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/tests/corral/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/tests/corral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      437 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/tests/corral/grab_versions_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1208 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/tests/corral/summary_test.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/tests/gh_pages/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/tests/gh_pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      283 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/tests/gh_pages/build_summaries_test.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/tests/releases/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/tests/releases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      705 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/tests/releases/maven_get_version_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)      771 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/tests/releases/python_get_version_test.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/tests/requirements/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/tests/requirements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1424 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/tests/requirements/requirements_test.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 23:56:54.000000 pds_github_util-0.9.2/tests/tags/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/tests/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      529 2020-07-09 23:55:42.000000 pds_github_util-0.9.2/tests/tags/tags_test.py
```

### Comparing `pds_github_util-0.9.1/PKG-INFO` & `pds_github_util-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pds_github_util
-Version: 0.9.1
+Version: 0.9.2
 Summary: util functions for software life cycle enforcement on github
 Home-page: https://github.com/NASA-PDS/pds-github-util
 Author: thomas loubrieu
 Author-email: loubrieu@jpl.nasa.gov
 License: apache-2.0
 Download-URL: https://github.com/NASA-PDS/pds-github-util/releases/download/0.0.1/pds_github_util-0.0.1.tar.gz
 Description: # PDS utility function for github
```

### Comparing `pds_github_util-0.9.1/README.md` & `pds_github_util-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/pds_github_util/branches/git_actions.py` & `pds_github_util-0.9.2/pds_github_util/branches/git_actions.py`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/pds_github_util/branches/git_ping.py` & `pds_github_util-0.9.2/pds_github_util/branches/git_ping.py`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/pds_github_util/build_summary.py` & `pds_github_util-0.9.2/pds_github_util/build_summary.py`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/pds_github_util/corral/cattle_head.py` & `pds_github_util-0.9.2/pds_github_util/corral/cattle_head.py`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/pds_github_util/corral/herd.py` & `pds_github_util-0.9.2/pds_github_util/corral/herd.py`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/pds_github_util/gh_pages/build_summaries.py` & `pds_github_util-0.9.2/pds_github_util/gh_pages/build_summaries.py`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/pds_github_util/gh_pages/root_index.py` & `pds_github_util-0.9.2/pds_github_util/gh_pages/root_index.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 SEMANTIC_VERSION_REGEX = r'\d+\.\d+(-SNAPSHOT)?'
 
 
 def colored_datetime(d, colored=True, format='%Y-%m-%d'):
     d_str = d.strftime(format)
     if colored:
-        color =  'orange' if d>datetime.now() else 'green'
+        color = 'orange' if d > datetime.now() else 'green'
         return f'<span style="color:{color}">{d_str}</span>'
     else:
         return d_str
 
 
 class HerdTable:
     def __init__(self, columns):
@@ -20,67 +20,74 @@
         self.n_rows = 1
         self.n_columns = len(columns)
 
     def add_herd(self, h):
         v = h.get_shepard_version()
         build_link = f'[{v}](./{v})'
         self.table.extend([build_link,
-                      colored_datetime(h.get_release_datetime()),
-                      colored_datetime(h.get_update_datetime(), colored=False)])
+                           colored_datetime(h.get_release_datetime()),
+                           colored_datetime(h.get_update_datetime(), colored=False)])
         self.n_rows += 1
 
     def __len__(self):
         return self.n_rows - 1
 
     def write_to_md_file(self, md_file):
         md_file.new_table(columns=self.n_columns,
-                   rows=self.n_rows,
-                   text=self.table,
-                   text_align='center')
+                          rows=self.n_rows,
+                          text=self.table,
+                          text_align='center')
 
 
 def update_index(root_dir, herds):
     index_file_name = os.path.join(root_dir, 'index.md')
     index_md_file = mdutils.MdUtils(file_name=index_file_name, title=f'PDS Engineering Node software suite, builds')
 
     herds.sort(key=lambda x: x.get_release_datetime(), reverse=True)
     herds_iterator = iter(herds)
+
     now = datetime.now()
 
     # dev/uit releases
-    table_development_releases =  HerdTable(["build" , "planned release", "update"])
+    table_development_releases = HerdTable(["build", "planned release", "update"])
     while True:
         herd = next(herds_iterator)
-        if herd.get_release_datetime()>now:
+        if herd.get_release_datetime() > now:
             table_development_releases.add_herd(herd)
         else:
             break
 
     # stable release
-    table_latest_stable_release = HerdTable(["build" , "release", "update"])
+    table_latest_stable_release = HerdTable(["build", "release", "update"])
     table_latest_stable_release.add_herd(herd)
 
     # archived releases
-    table_archived_releases =  HerdTable(["build" , "release", "update"])
+    table_archived_releases = HerdTable(["build", "release", "update"])
     while True:
         try:
             herd = next(herds_iterator)
             table_archived_releases.add_herd(herd)
         except StopIteration as e:
             break
 
     if len(table_latest_stable_release):
-        index_md_file.new_paragraph("Latest stable release")
+        index_md_file.new_paragraph("Latest stable release:")
+        index_md_file.new_line('')
         table_latest_stable_release.write_to_md_file(index_md_file)
 
     if len(table_development_releases):
-        index_md_file.new_paragraph("Development releases")
+        index_md_file.new_line('')
+        index_md_file.new_paragraph("Development releases:")
+        index_md_file.new_line('')
         table_development_releases.write_to_md_file(index_md_file)
 
     if len(table_archived_releases):
-        index_md_file.new_paragraph("Archived stable releases")
+        index_md_file.new_line('')
+        index_md_file.new_paragraph("Archived stable releases:")
+        index_md_file.new_line('')
         table_archived_releases.write_to_md_file(index_md_file)
 
     img = index_md_file.new_inline_image('new PDS logo test', 'https://nasa-pds.github.io/pdsen-corral/images/logo.png')
     index_md_file.new_line(img)
 
     index_md_file.create_md_file()
+
```

### Comparing `pds_github_util-0.9.1/pds_github_util/gh_pages/summary.py` & `pds_github_util-0.9.2/pds_github_util/gh_pages/summary.py`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/pds_github_util/html/md_to_html.py` & `pds_github_util-0.9.2/pds_github_util/html/md_to_html.py`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/pds_github_util/release/maven_snapshot_release.py` & `pds_github_util-0.9.2/pds_github_util/release/maven_snapshot_release.py`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/pds_github_util/release/python_snapshot_release.py` & `pds_github_util-0.9.2/pds_github_util/release/python_snapshot_release.py`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/pds_github_util/release/snapshot_release.py` & `pds_github_util-0.9.2/pds_github_util/release/snapshot_release.py`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/pds_github_util/requirements/generate_requirements.py` & `pds_github_util-0.9.2/pds_github_util/requirements/generate_requirements.py`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/pds_github_util/requirements/requirements.py` & `pds_github_util-0.9.2/pds_github_util/requirements/requirements.py`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/pds_github_util/tags/tags.py` & `pds_github_util-0.9.2/pds_github_util/tags/tags.py`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/pds_github_util/versions/versions.py` & `pds_github_util-0.9.2/pds_github_util/versions/versions.py`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/pds_github_util.egg-info/PKG-INFO` & `pds_github_util-0.9.2/pds_github_util.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pds-github-util
-Version: 0.9.1
+Version: 0.9.2
 Summary: util functions for software life cycle enforcement on github
 Home-page: https://github.com/NASA-PDS/pds-github-util
 Author: thomas loubrieu
 Author-email: loubrieu@jpl.nasa.gov
 License: apache-2.0
 Download-URL: https://github.com/NASA-PDS/pds-github-util/releases/download/0.0.1/pds_github_util-0.0.1.tar.gz
 Description: # PDS utility function for github
```

### Comparing `pds_github_util-0.9.1/pds_github_util.egg-info/SOURCES.txt` & `pds_github_util-0.9.2/pds_github_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/setup.py` & `pds_github_util-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/tests/corral/summary_test.py` & `pds_github_util-0.9.2/tests/corral/summary_test.py`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/tests/releases/maven_get_version_test.py` & `pds_github_util-0.9.2/tests/releases/maven_get_version_test.py`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/tests/releases/python_get_version_test.py` & `pds_github_util-0.9.2/tests/releases/python_get_version_test.py`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/tests/requirements/requirements_test.py` & `pds_github_util-0.9.2/tests/requirements/requirements_test.py`

 * *Files identical despite different names*

### Comparing `pds_github_util-0.9.1/tests/tags/tags_test.py` & `pds_github_util-0.9.2/tests/tags/tags_test.py`

 * *Files identical despite different names*

