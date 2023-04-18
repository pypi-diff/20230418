# Comparing `tmp/glustercli-0.8.4.tar.gz` & `tmp/glustercli-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glustercli-0.8.4.tar", last modified: Wed Apr 12 16:12:29 2023, max compression
+gzip compressed data, was "glustercli-0.8.5.tar", last modified: Tue Apr 18 06:17:01 2023, max compression
```

## Comparing `glustercli-0.8.4.tar` & `glustercli-0.8.5.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:29.187635 glustercli-0.8.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:29.179635 glustercli-0.8.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:29.183635 glustercli-0.8.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-12 16:12:20.000000 glustercli-0.8.4/.github/workflows/on-release-tag.yml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-12 16:12:20.000000 glustercli-0.8.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-12 16:12:20.000000 glustercli-0.8.4/COPYING-GPLV2
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-12 16:12:20.000000 glustercli-0.8.4/COPYING-LGPLV3
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-12 16:12:20.000000 glustercli-0.8.4/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-12 16:12:20.000000 glustercli-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-12 16:12:20.000000 glustercli-0.8.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-12 16:12:29.187635 glustercli-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-12 16:12:20.000000 glustercli-0.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:29.183635 glustercli-0.8.4/debian/
--rwxr-xr-x   0 runner    (1001) docker     (123)      156 2023-04-12 16:12:20.000000 glustercli-0.8.4/debian/changelog
--rwxr-xr-x   0 runner    (1001) docker     (123)        3 2023-04-12 16:12:20.000000 glustercli-0.8.4/debian/compat
--rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-04-12 16:12:20.000000 glustercli-0.8.4/debian/control
--rwxr-xr-x   0 runner    (1001) docker     (123)     2032 2023-04-12 16:12:20.000000 glustercli-0.8.4/debian/copyright
--rwxr-xr-x   0 runner    (1001) docker     (123)      410 2023-04-12 16:12:20.000000 glustercli-0.8.4/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:29.183635 glustercli-0.8.4/debian/source/
--rwxr-xr-x   0 runner    (1001) docker     (123)       12 2023-04-12 16:12:20.000000 glustercli-0.8.4/debian/source/format
--rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-04-12 16:12:20.000000 glustercli-0.8.4/debian/source/options
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:29.183635 glustercli-0.8.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/bitrot.md
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/bricks.md
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/georep.md
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/heal.md
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/local_diskstats.md
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/local_processes.md
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/local_utilization.md
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/nfs_ganesha.md
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/peer.md
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/quota.md
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/rebalance.md
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/snapshot.md
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/utils.md
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/volume.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:29.183635 glustercli-0.8.4/glustercli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 16:12:29.000000 glustercli-0.8.4/glustercli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:29.187635 glustercli-0.8.4/glustercli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/bitrot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/bricks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/georep.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/gluster_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/heal.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/nfs_ganesha.py
--rw-r--r--   0 runner    (1001) docker     (123)    27409 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/quota.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/rebalance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:29.187635 glustercli-0.8.4/glustercli/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/metrics/cmdlineparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/metrics/diskstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/metrics/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/metrics/utilization.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:29.183635 glustercli-0.8.4/glustercli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-12 16:12:29.000000 glustercli-0.8.4/glustercli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-12 16:12:29.000000 glustercli-0.8.4/glustercli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:12:29.000000 glustercli-0.8.4/glustercli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 16:12:29.000000 glustercli-0.8.4/glustercli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 16:12:29.000000 glustercli-0.8.4/glustercli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-12 16:12:20.000000 glustercli-0.8.4/pydocmd.yml
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-12 16:12:20.000000 glustercli-0.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 16:12:29.187635 glustercli-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-12 16:12:20.000000 glustercli-0.8.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-12 16:12:20.000000 glustercli-0.8.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:17:01.305531 glustercli-0.8.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:17:01.293531 glustercli-0.8.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:17:01.297531 glustercli-0.8.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-18 06:16:48.000000 glustercli-0.8.5/.github/workflows/on-release-tag.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-18 06:16:48.000000 glustercli-0.8.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-18 06:16:48.000000 glustercli-0.8.5/COPYING-GPLV2
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-18 06:16:48.000000 glustercli-0.8.5/COPYING-LGPLV3
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-18 06:16:48.000000 glustercli-0.8.5/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-18 06:16:48.000000 glustercli-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-18 06:16:48.000000 glustercli-0.8.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-18 06:17:01.301531 glustercli-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-18 06:16:48.000000 glustercli-0.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:17:01.297531 glustercli-0.8.5/debian/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      156 2023-04-18 06:16:48.000000 glustercli-0.8.5/debian/changelog
+-rwxr-xr-x   0 runner    (1001) docker     (123)        3 2023-04-18 06:16:48.000000 glustercli-0.8.5/debian/compat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-04-18 06:16:48.000000 glustercli-0.8.5/debian/control
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2032 2023-04-18 06:16:48.000000 glustercli-0.8.5/debian/copyright
+-rwxr-xr-x   0 runner    (1001) docker     (123)      410 2023-04-18 06:16:48.000000 glustercli-0.8.5/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:17:01.297531 glustercli-0.8.5/debian/source/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       12 2023-04-18 06:16:48.000000 glustercli-0.8.5/debian/source/format
+-rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-04-18 06:16:48.000000 glustercli-0.8.5/debian/source/options
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:17:01.297531 glustercli-0.8.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/bitrot.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/bricks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/georep.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/heal.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/local_diskstats.md
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/local_processes.md
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/local_utilization.md
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/nfs_ganesha.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/peer.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/quota.md
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/rebalance.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/snapshot.md
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-04-18 06:16:48.000000 glustercli-0.8.5/docs/volume.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:17:01.297531 glustercli-0.8.5/glustercli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 06:17:01.000000 glustercli-0.8.5/glustercli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:17:01.301531 glustercli-0.8.5/glustercli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/bitrot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/bricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/georep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/gluster_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/heal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/nfs_ganesha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27551 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/quota.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/rebalance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/cli/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:17:01.301531 glustercli-0.8.5/glustercli/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/metrics/cmdlineparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/metrics/diskstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/metrics/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/metrics/utilization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-18 06:16:48.000000 glustercli-0.8.5/glustercli/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:17:01.301531 glustercli-0.8.5/glustercli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-18 06:17:01.000000 glustercli-0.8.5/glustercli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-18 06:17:01.000000 glustercli-0.8.5/glustercli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 06:17:01.000000 glustercli-0.8.5/glustercli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 06:17:01.000000 glustercli-0.8.5/glustercli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 06:17:01.000000 glustercli-0.8.5/glustercli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-18 06:16:48.000000 glustercli-0.8.5/pydocmd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-18 06:16:48.000000 glustercli-0.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 06:17:01.305531 glustercli-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-18 06:16:48.000000 glustercli-0.8.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-18 06:16:48.000000 glustercli-0.8.5/tox.ini
```

### Comparing `glustercli-0.8.4/.github/workflows/on-release-tag.yml` & `glustercli-0.8.5/.github/workflows/on-release-tag.yml`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/COPYING-GPLV2` & `glustercli-0.8.5/COPYING-GPLV2`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/COPYING-LGPLV3` & `glustercli-0.8.5/COPYING-LGPLV3`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/MAINTAINERS` & `glustercli-0.8.5/MAINTAINERS`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/Makefile` & `glustercli-0.8.5/Makefile`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/PKG-INFO` & `glustercli-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glustercli
-Version: 0.8.4
+Version: 0.8.5
 Summary: Python bindings for GlusterFS CLI and Metrics collection
 Home-page: https://github.com/gluster/glustercli-python
 Author: Aravinda Vishwanathapura
 Author-email: aravinda@kadalu.io
 License: GPLv2 or LGPLv3+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `glustercli-0.8.4/README.md` & `glustercli-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/debian/control` & `glustercli-0.8.5/debian/control`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/debian/copyright` & `glustercli-0.8.5/debian/copyright`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/docs/README.md` & `glustercli-0.8.5/docs/README.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/docs/bitrot.md` & `glustercli-0.8.5/docs/bitrot.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/docs/bricks.md` & `glustercli-0.8.5/docs/bricks.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/docs/georep.md` & `glustercli-0.8.5/docs/georep.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/docs/heal.md` & `glustercli-0.8.5/docs/heal.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/docs/local_diskstats.md` & `glustercli-0.8.5/docs/local_diskstats.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/docs/local_utilization.md` & `glustercli-0.8.5/docs/local_utilization.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/docs/peer.md` & `glustercli-0.8.5/docs/peer.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/docs/quota.md` & `glustercli-0.8.5/docs/quota.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/docs/rebalance.md` & `glustercli-0.8.5/docs/rebalance.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/docs/snapshot.md` & `glustercli-0.8.5/docs/snapshot.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/docs/volume.md` & `glustercli-0.8.5/docs/volume.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/glustercli/cli/__init__.py` & `glustercli-0.8.5/glustercli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/glustercli/cli/bitrot.py` & `glustercli-0.8.5/glustercli/cli/bitrot.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/glustercli/cli/bricks.py` & `glustercli-0.8.5/glustercli/cli/bricks.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/glustercli/cli/georep.py` & `glustercli-0.8.5/glustercli/cli/georep.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/glustercli/cli/heal.py` & `glustercli-0.8.5/glustercli/cli/heal.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/glustercli/cli/nfs_ganesha.py` & `glustercli-0.8.5/glustercli/cli/nfs_ganesha.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/glustercli/cli/parsers.py` & `glustercli-0.8.5/glustercli/cli/parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -497,47 +497,47 @@
     gstatus = {}
 
     try:
         tree = etree.fromstring(data)
         # Get All Sessions
         for volume_el in tree.findall("geoRep/volume"):
             sessions_el = volume_el.find("sessions")
-            # Master Volume name if multiple Volumes
-            mvol = volume_el.find("name").text
+            # Primary Volume name if multiple Volumes
+            pvol = volume_el.find("name").text
 
             # For each session, collect the details
             for session in sessions_el.findall("session"):
-                session_slave = "{0}:{1}".format(mvol, session.find(
-                    "session_slave").text)
-                session_keys.add(session_slave)
-                gstatus[session_slave] = {}
+                session_secondary = "{0}:{1}".format(pvol, session.find(
+                    "session_secondary").text)
+                session_keys.add(session_secondary)
+                gstatus[session_secondary] = {}
 
                 for pair in session.findall('pair'):
-                    master_brick = "{0}:{1}".format(
-                        pair.find("master_node").text,
-                        pair.find("master_brick").text
+                    primary_brick = "{0}:{1}".format(
+                        pair.find("primary_node").text,
+                        pair.find("primary_brick").text
                     )
 
-                    gstatus[session_slave][master_brick] = {
-                        "mastervol": mvol,
-                        "slavevol": pair.find("slave").text.split("::")[-1],
-                        "master_node": pair.find("master_node").text,
-                        "master_brick": pair.find("master_brick").text,
-                        "slave_user": pair.find("slave_user").text,
-                        "slave": pair.find("slave").text,
-                        "slave_node": pair.find("slave_node").text,
+                    gstatus[session_secondary][primary_brick] = {
+                        "primary_volume": pvol,
+                        "secondary_volume": pair.find("secondary").text.split("::")[-1],
+                        "primary_node": pair.find("primary_node").text,
+                        "primary_brick": pair.find("primary_brick").text,
+                        "secondary_user": pair.find("secondary_user").text,
+                        "secondary": pair.find("secondary").text,
+                        "secondary_node": pair.find("secondary_node").text,
                         "status": pair.find("status").text,
                         "crawl_status": pair.find("crawl_status").text,
                         "entry": pair.find("entry").text,
                         "data": pair.find("data").text,
                         "meta": pair.find("meta").text,
                         "failures": pair.find("failures").text,
                         "checkpoint_completed": pair.find(
                             "checkpoint_completed").text,
-                        "master_node_uuid": pair.find("master_node_uuid").text,
+                        "primary_node_uuid": pair.find("primary_node_uuid").text,
                         "last_synced": pair.find("last_synced").text,
                         "checkpoint_time": pair.find("checkpoint_time").text,
                         "checkpoint_completion_time":
                         pair.find("checkpoint_completion_time").text
                     }
     except (ParseError, AttributeError, ValueError) as err:
         raise GlusterCmdOutputParseError(err)
@@ -547,46 +547,46 @@
     for vol in volinfo:
         all_bricks[vol["name"]] = vol["bricks"]
 
     # For Each session Get Bricks info for the Volume and Populate
     # Geo-rep status for that Brick
     out = []
     for session in session_keys:
-        mvol, _, slave = session.split(":", 2)
-        slave = slave.replace("ssh://", "")
-        master_bricks = all_bricks[mvol]
+        pvol, _, secondary = session.split(":", 2)
+        secondary = secondary.replace("ssh://", "")
+        primary_bricks = all_bricks[pvol]
         out.append([])
-        for brick in master_bricks:
+        for brick in primary_bricks:
             bname = brick["name"]
             if gstatus.get(session) and gstatus[session].get(bname, None):
                 out[-1].append(gstatus[session][bname])
             else:
                 # Offline Status
                 node, brick_path = bname.split(":")
-                if "@" not in slave:
-                    slave_user = "root"
+                if "@" not in secondary:
+                    secondary_user = "root"
                 else:
-                    slave_user, _ = slave.split("@")
+                    secondary_user, _ = secondary.split("@")
 
                 out[-1].append({
-                    "mastervol": mvol,
-                    "slavevol": slave.split("::")[-1],
-                    "master_node": node,
-                    "master_brick": brick_path,
-                    "slave_user": slave_user,
-                    "slave": slave,
-                    "slave_node": "N/A",
+                    "primary_volume": pvol,
+                    "secondary_volume": secondary.split("::")[-1],
+                    "primary_node": node,
+                    "primary_brick": brick_path,
+                    "secondary_user": secondary_user,
+                    "secondary": secondary,
+                    "secondary_node": "N/A",
                     "status": "Offline",
                     "crawl_status": "N/A",
                     "entry": "N/A",
                     "data": "N/A",
                     "meta": "N/A",
                     "failures": "N/A",
                     "checkpoint_completed": "N/A",
-                    "master_node_uuid": brick["uuid"],
+                    "primary_node_uuid": brick["uuid"],
                     "last_synced": "N/A",
                     "checkpoint_time": "N/A",
                     "checkpoint_completion_time": "N/A"
                 })
     return out
```

### Comparing `glustercli-0.8.4/glustercli/cli/peer.py` & `glustercli-0.8.5/glustercli/cli/peer.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/glustercli/cli/quota.py` & `glustercli-0.8.5/glustercli/cli/quota.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/glustercli/cli/rebalance.py` & `glustercli-0.8.5/glustercli/cli/rebalance.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/glustercli/cli/snapshot.py` & `glustercli-0.8.5/glustercli/cli/snapshot.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/glustercli/cli/utils.py` & `glustercli-0.8.5/glustercli/cli/utils.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/glustercli/cli/volume.py` & `glustercli-0.8.5/glustercli/cli/volume.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/glustercli/metrics/cmdlineparser.py` & `glustercli-0.8.5/glustercli/metrics/cmdlineparser.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/glustercli/metrics/diskstats.py` & `glustercli-0.8.5/glustercli/metrics/diskstats.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/glustercli/metrics/process.py` & `glustercli-0.8.5/glustercli/metrics/process.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/glustercli/metrics/utilization.py` & `glustercli-0.8.5/glustercli/metrics/utilization.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/glustercli/metrics/utils.py` & `glustercli-0.8.5/glustercli/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/glustercli.egg-info/PKG-INFO` & `glustercli-0.8.5/glustercli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glustercli
-Version: 0.8.4
+Version: 0.8.5
 Summary: Python bindings for GlusterFS CLI and Metrics collection
 Home-page: https://github.com/gluster/glustercli-python
 Author: Aravinda Vishwanathapura
 Author-email: aravinda@kadalu.io
 License: GPLv2 or LGPLv3+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `glustercli-0.8.4/glustercli.egg-info/SOURCES.txt` & `glustercli-0.8.5/glustercli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/pydocmd.yml` & `glustercli-0.8.5/pydocmd.yml`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.4/setup.py` & `glustercli-0.8.5/setup.py`

 * *Files identical despite different names*

