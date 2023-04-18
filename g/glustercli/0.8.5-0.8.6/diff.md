# Comparing `tmp/glustercli-0.8.5.tar.gz` & `tmp/glustercli-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glustercli-0.8.5.tar", last modified: Tue Apr 18 06:17:01 2023, max compression
+gzip compressed data, was "glustercli-0.8.6.tar", last modified: Tue Apr 18 16:07:25 2023, max compression
```

## Comparing `glustercli-0.8.5.tar` & `glustercli-0.8.6.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:17:01.305531 glustercli-0.8.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:17:01.293531 glustercli-0.8.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:17:01.297531 glustercli-0.8.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-18 06:16:48.000000 glustercli-0.8.5/.github/workflows/on-release-tag.yml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-18 06:16:48.000000 glustercli-0.8.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-18 06:16:48.000000 glustercli-0.8.5/COPYING-GPLV2
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-18 06:16:48.000000 glustercli-0.8.5/COPYING-LGPLV3
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-18 06:16:48.000000 glustercli-0.8.5/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-18 06:16:48.000000 glustercli-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-18 06:16:48.000000 glustercli-0.8.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-18 06:17:01.301531 glustercli-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-18 06:16:48.000000 glustercli-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:17:01.297531 glustercli-0.8.5/debian/
--rwxr-xr-x   0 runner    (1001) docker     (123)      156 2023-04-18 06:16:48.000000 glustercli-0.8.5/debian/changelog
--rwxr-xr-x   0 runner    (1001) docker     (123)        3 2023-04-18 06:16:48.000000 glustercli-0.8.5/debian/compat
--rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-04-18 06:16:48.000000 glustercli-0.8.5/debian/control
--rwxr-xr-x   0 runner    (1001) docker     (123)     2032 2023-04-18 06:16:48.000000 glustercli-0.8.5/debian/copyright
--rwxr-xr-x   0 runner    (1001) docker     (123)      410 2023-04-18 06:16:48.000000 glustercli-0.8.5/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:17:01.297531 glustercli-0.8.5/debian/source/
--rwxr-xr-x   0 runner    (1001) docker     (123)       12 2023-04-18 06:16:48.000000 glustercli-0.8.5/debian/source/format
--rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-04-18 06:16:48.000000 glustercli-0.8.5/debian/source/options
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:17:01.297531 glustercli-0.8.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/bitrot.md
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/bricks.md
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/georep.md
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/heal.md
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/local_diskstats.md
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/local_processes.md
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/local_utilization.md
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/nfs_ganesha.md
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/peer.md
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/quota.md
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/rebalance.md
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/snapshot.md
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/utils.md
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/volume.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:17:01.297531 glustercli-0.8.5/glustercli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 06:17:01.000000 glustercli-0.8.5/glustercli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:17:01.301531 glustercli-0.8.5/glustercli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/bitrot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/bricks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/georep.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/gluster_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/heal.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/nfs_ganesha.py
--rw-r--r--   0 runner    (1001) docker     (123)    27551 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/quota.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/rebalance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:17:01.301531 glustercli-0.8.5/glustercli/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/metrics/cmdlineparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/metrics/diskstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/metrics/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/metrics/utilization.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:17:01.301531 glustercli-0.8.5/glustercli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-18 06:17:01.000000 glustercli-0.8.5/glustercli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-18 06:17:01.000000 glustercli-0.8.5/glustercli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 06:17:01.000000 glustercli-0.8.5/glustercli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 06:17:01.000000 glustercli-0.8.5/glustercli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 06:17:01.000000 glustercli-0.8.5/glustercli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-18 06:16:48.000000 glustercli-0.8.5/pydocmd.yml
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-18 06:16:48.000000 glustercli-0.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 06:17:01.305531 glustercli-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-18 06:16:48.000000 glustercli-0.8.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-18 06:16:48.000000 glustercli-0.8.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:07:25.462441 glustercli-0.8.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:07:25.458441 glustercli-0.8.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:07:25.458441 glustercli-0.8.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-18 16:07:11.000000 glustercli-0.8.6/.github/workflows/on-release-tag.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-18 16:07:11.000000 glustercli-0.8.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-18 16:07:11.000000 glustercli-0.8.6/COPYING-GPLV2
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-18 16:07:11.000000 glustercli-0.8.6/COPYING-LGPLV3
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-18 16:07:11.000000 glustercli-0.8.6/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-18 16:07:11.000000 glustercli-0.8.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-18 16:07:11.000000 glustercli-0.8.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-18 16:07:25.462441 glustercli-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-18 16:07:11.000000 glustercli-0.8.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:07:25.458441 glustercli-0.8.6/debian/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      156 2023-04-18 16:07:11.000000 glustercli-0.8.6/debian/changelog
+-rwxr-xr-x   0 runner    (1001) docker     (123)        3 2023-04-18 16:07:11.000000 glustercli-0.8.6/debian/compat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-04-18 16:07:11.000000 glustercli-0.8.6/debian/control
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2032 2023-04-18 16:07:11.000000 glustercli-0.8.6/debian/copyright
+-rwxr-xr-x   0 runner    (1001) docker     (123)      410 2023-04-18 16:07:11.000000 glustercli-0.8.6/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:07:25.458441 glustercli-0.8.6/debian/source/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       12 2023-04-18 16:07:11.000000 glustercli-0.8.6/debian/source/format
+-rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-04-18 16:07:11.000000 glustercli-0.8.6/debian/source/options
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:07:25.462441 glustercli-0.8.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-18 16:07:11.000000 glustercli-0.8.6/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-18 16:07:11.000000 glustercli-0.8.6/docs/bitrot.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-18 16:07:11.000000 glustercli-0.8.6/docs/bricks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-04-18 16:07:11.000000 glustercli-0.8.6/docs/georep.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-18 16:07:11.000000 glustercli-0.8.6/docs/heal.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-18 16:07:11.000000 glustercli-0.8.6/docs/local_diskstats.md
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 16:07:11.000000 glustercli-0.8.6/docs/local_processes.md
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-18 16:07:11.000000 glustercli-0.8.6/docs/local_utilization.md
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-18 16:07:11.000000 glustercli-0.8.6/docs/nfs_ganesha.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-18 16:07:11.000000 glustercli-0.8.6/docs/peer.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-18 16:07:11.000000 glustercli-0.8.6/docs/quota.md
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-18 16:07:11.000000 glustercli-0.8.6/docs/rebalance.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-18 16:07:11.000000 glustercli-0.8.6/docs/snapshot.md
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-18 16:07:11.000000 glustercli-0.8.6/docs/utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-04-18 16:07:11.000000 glustercli-0.8.6/docs/volume.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:07:25.462441 glustercli-0.8.6/glustercli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 16:07:25.000000 glustercli-0.8.6/glustercli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:07:25.462441 glustercli-0.8.6/glustercli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/cli/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/cli/bitrot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/cli/bricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/cli/georep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/cli/gluster_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/cli/heal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/cli/nfs_ganesha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27551 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/cli/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/cli/peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/cli/quota.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/cli/rebalance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/cli/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/cli/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:07:25.462441 glustercli-0.8.6/glustercli/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/metrics/cmdlineparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/metrics/diskstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/metrics/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/metrics/utilization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-18 16:07:11.000000 glustercli-0.8.6/glustercli/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:07:25.462441 glustercli-0.8.6/glustercli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-18 16:07:25.000000 glustercli-0.8.6/glustercli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-18 16:07:25.000000 glustercli-0.8.6/glustercli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:07:25.000000 glustercli-0.8.6/glustercli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 16:07:25.000000 glustercli-0.8.6/glustercli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 16:07:25.000000 glustercli-0.8.6/glustercli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-18 16:07:11.000000 glustercli-0.8.6/pydocmd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-18 16:07:11.000000 glustercli-0.8.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:07:25.462441 glustercli-0.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-18 16:07:11.000000 glustercli-0.8.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-18 16:07:11.000000 glustercli-0.8.6/tox.ini
```

### Comparing `glustercli-0.8.5/.github/workflows/on-release-tag.yml` & `glustercli-0.8.6/.github/workflows/on-release-tag.yml`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/COPYING-GPLV2` & `glustercli-0.8.6/COPYING-GPLV2`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/COPYING-LGPLV3` & `glustercli-0.8.6/COPYING-LGPLV3`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/MAINTAINERS` & `glustercli-0.8.6/MAINTAINERS`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/Makefile` & `glustercli-0.8.6/Makefile`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/PKG-INFO` & `glustercli-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glustercli
-Version: 0.8.5
+Version: 0.8.6
 Summary: Python bindings for GlusterFS CLI and Metrics collection
 Home-page: https://github.com/gluster/glustercli-python
 Author: Aravinda Vishwanathapura
 Author-email: aravinda@kadalu.io
 License: GPLv2 or LGPLv3+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `glustercli-0.8.5/README.md` & `glustercli-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/debian/control` & `glustercli-0.8.6/debian/control`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/debian/copyright` & `glustercli-0.8.6/debian/copyright`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/docs/README.md` & `glustercli-0.8.6/docs/README.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/docs/bitrot.md` & `glustercli-0.8.6/docs/bitrot.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/docs/bricks.md` & `glustercli-0.8.6/docs/bricks.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/docs/georep.md` & `glustercli-0.8.6/docs/volume.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,211 +1,272 @@
 
-# glustercli.cli.georep
+# glustercli.cli.volume
 
 
-## gsec_create
+## start
 ```python
-gsec_create(ssh_key_prefix=True)
+start(volname, force=False)
 ```
 
-Generate Geo-replication SSH Keys
+Start Gluster Volume
 
-:param ssh_key_prefix: True|False Command prefix in generated public keys
-:returns: Output of gsec_create command, raises
+:param volname: Volume Name
+:param force: (True|False) Start Volume with Force option
+:returns: Output of Start command, raises
+ GlusterCmdException((rc, out, err)) on error
+
+
+## stop
+```python
+stop(volname, force=False)
+```
+
+Stop Gluster Volume
+
+:param volname: Volume Name
+:param force: (True|False) Stop Volume with Force option
+:returns: Output of Stop command, raises
+ GlusterCmdException((rc, out, err)) on error
+
+
+## restart
+```python
+restart(volname, force=False)
+```
+
+Restart Gluster Volume, Wrapper around two calls stop and start
+
+:param volname: Volume Name
+:param force: (True|False) Restart Volume with Force option
+:returns: Output of Start command, raises
+ GlusterCmdException((rc, out, err)) on error
+
+
+## delete
+```python
+delete(volname)
+```
+
+Delete Gluster Volume
+
+:param volname: Volume Name
+:returns: Output of Delete command, raises
  GlusterCmdException((rc, out, err)) on error
 
 
 ## create
 ```python
 create(volname,
-       slave_host,
-       slave_vol,
-       slave_user='root',
-       push_pem=True,
-       no_verify=False,
-       force=False,
-       ssh_port=22)
-```
-
-Create Geo-replication Session
-
-:param volname: Master Volume Name
-:param slave_host: Slave Hostname or IP
-:param slave_vol: Slave Volume
-:param slave_user: Slave User, default is "root"
-:param push_pem: True|False Push SSH keys to Slave
-:param no_verify: True|False Skip the Slave Verification
- process before create
-:param force: True|False Force Create Session
-:param ssh_port: SSH Port, Default is 22
+       volbricks,
+       replica=0,
+       stripe=0,
+       arbiter=0,
+       disperse=0,
+       disperse_data=0,
+       redundancy=0,
+       transport='tcp',
+       force=False)
+```
+
+Create Gluster Volume
+
+:param volname: Volume Name
+:param volbricks: List of Brick paths(HOSTNAME:PATH)
+:param replica: Number of Replica bricks
+:param stripe: Number of Stripe bricks
+:param arbiter: Number of Arbiter bricks
+:param disperse: Number of disperse bricks
+:param disperse_data: Number of disperse data bricks
+:param redundancy: Number of Redundancy bricks
+:param transport: Transport mode(tcp|rdma|tcp,rdma)
+:param force: (True|False) Create Volume with Force option
 :returns: Output of Create command, raises
  GlusterCmdException((rc, out, err)) on error
 
 
-## start
+## info
 ```python
-start(volname, slave_host, slave_vol, slave_user='root', force=False)
+info(volname=None, group_subvols=False)
 ```
 
-Start Geo-replication Session
+Get Gluster Volume Info
 
-:param volname: Master Volume Name
-:param slave_host: Slave Hostname or IP
-:param slave_vol: Slave Volume
-:param slave_user: Slave User, default is "root"
-:param force: True|False Force Start the Session
-:returns: Output of Start command, raises
+:param volname: Volume Name
+:param group_subvols: Show Subvolume Information in Groups
+:returns: Returns Volume Info, raises
  GlusterCmdException((rc, out, err)) on error
 
 
-## stop
+## status_detail
 ```python
-stop(volname, slave_host, slave_vol, slave_user='root', force=False)
+status_detail(volname=None, group_subvols=False)
 ```
 
-Stop Geo-replication Session
+Get Gluster Volume Status
 
-:param volname: Master Volume Name
-:param slave_host: Slave Hostname or IP
-:param slave_vol: Slave Volume
-:param slave_user: Slave User, default is "root"
-:param force: True|False Force Stop the Session
-:returns: Output of Stop command, raises
+:param volname: Volume Name
+:param group_subvols: Show Subvolume Information in Groups
+:returns: Returns Volume Status, raises
  GlusterCmdException((rc, out, err)) on error
 
 
-## restart
+## optset
 ```python
-restart(volname, slave_host, slave_vol, slave_user='root', force=False)
+optset(volname, opts)
 ```
 
-Restart Geo-replication Session
+Set Volume Options
 
-:param volname: Master Volume Name
-:param slave_host: Slave Hostname or IP
-:param slave_vol: Slave Volume
-:param slave_user: Slave User, default is "root"
-:param force: True|False Force Start the Session
-:returns: Output of Start command, raises
+:param volname: Volume Name
+:param opts: Dict with config key as dict key and config value as value
+:returns: Output of Volume Set command, raises
  GlusterCmdException((rc, out, err)) on error
 
 
-## delete
+## optget
 ```python
-delete(volname,
-       slave_host,
-       slave_vol,
-       slave_user='root',
-       reset_sync_time=None)
+optget(volname, opt='all')
 ```
 
-Delete Geo-replication Session
-
-:param volname: Master Volume Name
-:param slave_host: Slave Hostname or IP
-:param slave_vol: Slave Volume
-:param slave_user: Slave User, default is "root"
-:param reset_sync_time: True|False Reset Sync time on delete
-:returns: Output of Start command, raises
+Get Volume Options
+
+:param volname: Volume Name
+:param opt: Option Name
+:returns: List of Volume Options, raises
+ GlusterCmdException((rc, out, err)) on error
+
+
+## optreset
+```python
+optreset(volname, opt=None, force=False)
+```
+
+Reset Volume Options
+
+:param volname: Volume Name
+:param opt: Option name to reset, else reset all
+:param force: Force reset options
+:returns: Output of Volume Reset command, raises
+ GlusterCmdException((rc, out, err)) on error
+
+
+## vollist
+```python
+vollist()
+```
+
+Volumes List
+
+:returns: List of Volumes, raises
+ GlusterCmdException((rc, out, err)) on error
+
+
+## log_rotate
+```python
+log_rotate(volname, brick)
+```
+
+Brick log rotate
+
+:param volname: Volume Name
+:param brick: Brick Path
+:returns: Output of Log rotate command, raises
+ GlusterCmdException((rc, out, err)) on error
+
+
+## sync
+```python
+sync(hostname, volname=None)
+```
+
+Sync the volume information from a peer
+
+:param hostname: Hostname to sync from
+:param volname: Volume Name
+:returns: Output of Sync command, raises
  GlusterCmdException((rc, out, err)) on error
 
 
-## pause
+## clear_locks
 ```python
-pause(volname, slave_host, slave_vol, slave_user='root', force=False)
+clear_locks(volname,
+            path,
+            kind,
+            inode_range=None,
+            entry_basename=None,
+            posix_range=None)
 ```
 
-Pause Geo-replication Session
+Clear locks held on path
 
-:param volname: Master Volume Name
-:param slave_host: Slave Hostname or IP
-:param slave_vol: Slave Volume
-:param slave_user: Slave User, default is "root"
-:param force: True|False Force Pause Session
-:returns: Output of Pause command, raises
+:param volname: Volume Name
+:param path: Locked Path
+:param kind: Lock Kind(blocked|granted|all)
+:param inode_range: Inode Range
+:param entry_basename: Entry Basename
+:param posix_range: Posix Range
+:returns: Output of Clear locks command, raises
  GlusterCmdException((rc, out, err)) on error
 
 
-## resume
+## barrier_enable
 ```python
-resume(volname, slave_host, slave_vol, slave_user='root', force=False)
+barrier_enable(volname)
 ```
 
-Resume Geo-replication Session
+Enable Barrier
 
-:param volname: Master Volume Name
-:param slave_host: Slave Hostname or IP
-:param slave_vol: Slave Volume
-:param slave_user: Slave User, default is "root"
-:param force: True|False Force Resume Session
-:returns: Output of Resume command, raises
+:param volname: Volume Name
+:returns: Output of Barrier command, raises
  GlusterCmdException((rc, out, err)) on error
 
 
-## config_set
+## barrier_disable
 ```python
-config_set(volname,
-           slave_host,
-           slave_vol,
-           key,
-           value,
-           slave_user='root')
+barrier_disable(volname)
 ```
 
-Set Config of a Geo-replication Session
+Disable Barrier
 
-:param volname: Master Volume Name
-:param slave_host: Slave Hostname or IP
-:param slave_vol: Slave Volume
-:param slave_user: Slave User, default is "root"
-:param key: Config Key
-:param value: Config Value
-:returns: Output of Config set command, raises
+:param volname: Volume Name
+:returns: Output of Barrier command, raises
  GlusterCmdException((rc, out, err)) on error
 
 
-## config_reset
+## profile_start
 ```python
-config_reset(volname, slave_host, slave_vol, key, slave_user='root')
+profile_start(volname)
 ```
 
-Reset configuration of Geo-replication Session
+Start Profile
 
-:param volname: Master Volume Name
-:param slave_host: Slave Hostname or IP
-:param slave_vol: Slave Volume
-:param slave_user: Slave User, default is "root"
-:param key: Config Key
-:returns: Output of Config reset command, raises
+:param volname: Volume Name
+:return: Output of Profile command, raises
  GlusterCmdException((rc, out, err)) on error
 
 
-## config_get
+## profile_stop
 ```python
-config_get(volname, slave_host, slave_vol, key=None, slave_user='root')
+profile_stop(volname)
 ```
 
-Get Configuration of Geo-replication Session
+Stop Profile
 
-:param volname: Master Volume Name
-:param slave_host: Slave Hostname or IP
-:param slave_vol: Slave Volume
-:param slave_user: Slave User, default is "root"
-:param key: Config Key
-:returns: Geo-rep session Config Values, raises
+:param volname: Volume Name
+:return: Output of Profile command, raises
  GlusterCmdException((rc, out, err)) on error
 
 
-## status
+## profile_info
 ```python
-status(volname=None, slave_host=None, slave_vol=None, slave_user='root')
+profile_info(volname, opt, peek=False)
 ```
 
-Status of Geo-replication Session
+Get Profile info
 
-:param volname: Master Volume Name
-:param slave_host: Slave Hostname or IP
-:param slave_vol: Slave Volume
-:param slave_user: Slave User, default is "root"
-:returns: Geo-replication Status, raises
+:param volname: Volume Name
+:param opt: Operation type of info,
+ like peek, incremental, cumulative, clear
+:param peek: Use peek or not, default is False
+:return: Return profile info, raises
  GlusterCmdException((rc, out, err)) on error
```

### Comparing `glustercli-0.8.5/docs/heal.md` & `glustercli-0.8.6/docs/heal.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/docs/local_diskstats.md` & `glustercli-0.8.6/docs/local_diskstats.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/docs/local_utilization.md` & `glustercli-0.8.6/docs/local_utilization.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/docs/peer.md` & `glustercli-0.8.6/docs/peer.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/docs/quota.md` & `glustercli-0.8.6/docs/quota.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/docs/rebalance.md` & `glustercli-0.8.6/docs/rebalance.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/docs/snapshot.md` & `glustercli-0.8.6/docs/snapshot.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/glustercli/cli/__init__.py` & `glustercli-0.8.6/glustercli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/glustercli/cli/bitrot.py` & `glustercli-0.8.6/glustercli/cli/bitrot.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/glustercli/cli/bricks.py` & `glustercli-0.8.6/glustercli/cli/bricks.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/glustercli/cli/heal.py` & `glustercli-0.8.6/glustercli/cli/heal.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/glustercli/cli/nfs_ganesha.py` & `glustercli-0.8.6/glustercli/cli/nfs_ganesha.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/glustercli/cli/parsers.py` & `glustercli-0.8.6/glustercli/cli/parsers.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/glustercli/cli/peer.py` & `glustercli-0.8.6/glustercli/cli/peer.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/glustercli/cli/quota.py` & `glustercli-0.8.6/glustercli/cli/quota.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/glustercli/cli/rebalance.py` & `glustercli-0.8.6/glustercli/cli/rebalance.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/glustercli/cli/snapshot.py` & `glustercli-0.8.6/glustercli/cli/snapshot.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/glustercli/cli/utils.py` & `glustercli-0.8.6/glustercli/cli/utils.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/glustercli/cli/volume.py` & `glustercli-0.8.6/glustercli/cli/volume.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/glustercli/metrics/cmdlineparser.py` & `glustercli-0.8.6/glustercli/metrics/cmdlineparser.py`

 * *Files 14% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     if "--feedback-fd" in args:
         data["role"] = "worker"
     elif "--agent" in args:
         data["role"] = "agent"
     elif "--monitor" in args:
         data["role"] = "monitor"
     elif "--listen" in args:
-        data["role"] = "slave"
+        data["role"] = "secondary"
 
     return data
 
 
 def parse_cmdline_glustereventsd(args):
     return {
         "name": "glustereventsd",
```

### Comparing `glustercli-0.8.5/glustercli/metrics/diskstats.py` & `glustercli-0.8.6/glustercli/metrics/diskstats.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/glustercli/metrics/process.py` & `glustercli-0.8.6/glustercli/metrics/process.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/glustercli/metrics/utilization.py` & `glustercli-0.8.6/glustercli/metrics/utilization.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/glustercli/metrics/utils.py` & `glustercli-0.8.6/glustercli/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/glustercli.egg-info/PKG-INFO` & `glustercli-0.8.6/glustercli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glustercli
-Version: 0.8.5
+Version: 0.8.6
 Summary: Python bindings for GlusterFS CLI and Metrics collection
 Home-page: https://github.com/gluster/glustercli-python
 Author: Aravinda Vishwanathapura
 Author-email: aravinda@kadalu.io
 License: GPLv2 or LGPLv3+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `glustercli-0.8.5/glustercli.egg-info/SOURCES.txt` & `glustercli-0.8.6/glustercli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/pydocmd.yml` & `glustercli-0.8.6/pydocmd.yml`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.5/setup.py` & `glustercli-0.8.6/setup.py`

 * *Files identical despite different names*

