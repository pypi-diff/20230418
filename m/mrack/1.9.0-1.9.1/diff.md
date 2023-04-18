# Comparing `tmp/mrack-1.9.0.tar.gz` & `tmp/mrack-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrack-1.9.0.tar", last modified: Wed Oct 12 14:08:18 2022, max compression
+gzip compressed data, was "mrack-1.9.1.tar", last modified: Thu Oct 20 11:34:16 2022, max compression
```

## Comparing `mrack-1.9.0.tar` & `mrack-1.9.1.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 14:08:18.569204 mrack-1.9.0/
--rw-r--r--   0 root         (0) root         (0)    10143 2022-10-12 14:08:00.000000 mrack-1.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       41 2022-10-12 14:08:00.000000 mrack-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8928 2022-10-12 14:08:18.569204 mrack-1.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8567 2022-10-12 14:08:00.000000 mrack-1.9.0/README.md
--rw-r--r--   0 root         (0) root         (0)      565 2022-10-12 14:08:00.000000 mrack-1.9.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      125 2022-10-12 14:08:00.000000 mrack-1.9.0/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 14:08:18.553204 mrack-1.9.0/scripts/
--rwxr-xr-x   0 root         (0) root         (0)      709 2022-10-12 14:08:00.000000 mrack-1.9.0/scripts/mrack
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-12 14:08:18.569204 mrack-1.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1831 2022-10-12 14:08:00.000000 mrack-1.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 14:08:18.549204 mrack-1.9.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 14:08:18.557204 mrack-1.9.0/src/mrack/
--rw-r--r--   0 root         (0) root         (0)      655 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 14:08:18.561204 mrack-1.9.0/src/mrack/actions/
--rw-r--r--   0 root         (0) root         (0)      599 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/actions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1885 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/actions/action.py
--rw-r--r--   0 root         (0) root         (0)     1934 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/actions/destroy.py
--rw-r--r--   0 root         (0) root         (0)     4853 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/actions/etchosts.py
--rw-r--r--   0 root         (0) root         (0)      941 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/actions/list.py
--rw-r--r--   0 root         (0) root         (0)     2422 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/actions/output.py
--rw-r--r--   0 root         (0) root         (0)     3713 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/actions/ssh.py
--rw-r--r--   0 root         (0) root         (0)     5060 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/actions/up.py
--rw-r--r--   0 root         (0) root         (0)     4571 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/config.py
--rw-r--r--   0 root         (0) root         (0)     3255 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 14:08:18.561204 mrack-1.9.0/src/mrack/data/
--rw-r--r--   0 root         (0) root         (0)      186 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/data/mrack.conf
--rw-r--r--   0 root         (0) root         (0)     6456 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/data/provisioning-config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 14:08:18.561204 mrack-1.9.0/src/mrack/dbdrivers/
--rw-r--r--   0 root         (0) root         (0)      713 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/dbdrivers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2444 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/dbdrivers/file.py
--rw-r--r--   0 root         (0) root         (0)     1714 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/errors.py
--rw-r--r--   0 root         (0) root         (0)     5207 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/host.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 14:08:18.561204 mrack-1.9.0/src/mrack/outputs/
--rw-r--r--   0 root         (0) root         (0)      671 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/outputs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7691 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/outputs/ansible_inventory.py
--rw-r--r--   0 root         (0) root         (0)     6071 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/outputs/pytest_multihost.py
--rw-r--r--   0 root         (0) root         (0)     1489 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/outputs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 14:08:18.565204 mrack-1.9.0/src/mrack/providers/
--rw-r--r--   0 root         (0) root         (0)     1752 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/providers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12614 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/providers/aws.py
--rw-r--r--   0 root         (0) root         (0)    14348 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/providers/beaker.py
--rw-r--r--   0 root         (0) root         (0)    28989 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/providers/openstack.py
--rw-r--r--   0 root         (0) root         (0)    10624 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/providers/podman.py
--rw-r--r--   0 root         (0) root         (0)    20065 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/providers/provider.py
--rw-r--r--   0 root         (0) root         (0)     3323 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/providers/static.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 14:08:18.565204 mrack-1.9.0/src/mrack/providers/utils/
--rw-r--r--   0 root         (0) root         (0)       64 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/providers/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2467 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/providers/utils/osapi.py
--rw-r--r--   0 root         (0) root         (0)     6229 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/providers/utils/podman.py
--rw-r--r--   0 root         (0) root         (0)     4688 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/providers/utils/testcloud.py
--rw-r--r--   0 root         (0) root         (0)     6993 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/providers/virt.py
--rw-r--r--   0 root         (0) root         (0)     7977 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 14:08:18.569204 mrack-1.9.0/src/mrack/transformers/
--rw-r--r--   0 root         (0) root         (0)     4020 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/transformers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2602 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/transformers/aws.py
--rw-r--r--   0 root         (0) root         (0)     7251 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/transformers/beaker.py
--rw-r--r--   0 root         (0) root         (0)     2890 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/transformers/openstack.py
--rw-r--r--   0 root         (0) root         (0)     2076 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/transformers/podman.py
--rw-r--r--   0 root         (0) root         (0)     1177 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/transformers/static.py
--rw-r--r--   0 root         (0) root         (0)     5394 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/transformers/transformer.py
--rw-r--r--   0 root         (0) root         (0)     2326 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/transformers/virt.py
--rw-r--r--   0 root         (0) root         (0)    11565 2022-10-12 14:08:00.000000 mrack-1.9.0/src/mrack/utils.py
--rw-r--r--   0 root         (0) root         (0)       47 2022-10-12 14:08:15.000000 mrack-1.9.0/src/mrack/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 14:08:18.557204 mrack-1.9.0/src/mrack.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8928 2022-10-12 14:08:18.000000 mrack-1.9.0/src/mrack.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1545 2022-10-12 14:08:18.000000 mrack-1.9.0/src/mrack.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-12 14:08:18.000000 mrack-1.9.0/src/mrack.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      125 2022-10-12 14:08:18.000000 mrack-1.9.0/src/mrack.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-10-12 14:08:18.000000 mrack-1.9.0/src/mrack.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 11:34:16.652416 mrack-1.9.1/
+-rw-r--r--   0 root         (0) root         (0)    24845 2022-10-20 11:34:14.000000 mrack-1.9.1/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    10143 2022-10-20 11:34:04.000000 mrack-1.9.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       62 2022-10-20 11:34:04.000000 mrack-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8926 2022-10-20 11:34:16.652416 mrack-1.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8565 2022-10-20 11:34:04.000000 mrack-1.9.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      563 2022-10-20 11:34:04.000000 mrack-1.9.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      125 2022-10-20 11:34:04.000000 mrack-1.9.1/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 11:34:16.644416 mrack-1.9.1/scripts/
+-rwxr-xr-x   0 root         (0) root         (0)      709 2022-10-20 11:34:04.000000 mrack-1.9.1/scripts/mrack
+-rw-r--r--   0 root         (0) root         (0)       38 2022-10-20 11:34:16.652416 mrack-1.9.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1831 2022-10-20 11:34:04.000000 mrack-1.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 11:34:16.640416 mrack-1.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 11:34:16.644416 mrack-1.9.1/src/mrack/
+-rw-r--r--   0 root         (0) root         (0)      655 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 11:34:16.648416 mrack-1.9.1/src/mrack/actions/
+-rw-r--r--   0 root         (0) root         (0)      599 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/actions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/actions/action.py
+-rw-r--r--   0 root         (0) root         (0)     1934 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/actions/destroy.py
+-rw-r--r--   0 root         (0) root         (0)     4853 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/actions/etchosts.py
+-rw-r--r--   0 root         (0) root         (0)      941 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/actions/list.py
+-rw-r--r--   0 root         (0) root         (0)     2422 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/actions/output.py
+-rw-r--r--   0 root         (0) root         (0)     3713 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/actions/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     5060 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/actions/up.py
+-rw-r--r--   0 root         (0) root         (0)     4571 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/config.py
+-rw-r--r--   0 root         (0) root         (0)     3255 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 11:34:16.648416 mrack-1.9.1/src/mrack/data/
+-rw-r--r--   0 root         (0) root         (0)      186 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/data/mrack.conf
+-rw-r--r--   0 root         (0) root         (0)     6456 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/data/provisioning-config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 11:34:16.648416 mrack-1.9.1/src/mrack/dbdrivers/
+-rw-r--r--   0 root         (0) root         (0)      713 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/dbdrivers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2444 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/dbdrivers/file.py
+-rw-r--r--   0 root         (0) root         (0)     1714 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5207 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/host.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 11:34:16.648416 mrack-1.9.1/src/mrack/outputs/
+-rw-r--r--   0 root         (0) root         (0)      671 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/outputs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7691 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/outputs/ansible_inventory.py
+-rw-r--r--   0 root         (0) root         (0)     6071 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/outputs/pytest_multihost.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/outputs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 11:34:16.648416 mrack-1.9.1/src/mrack/providers/
+-rw-r--r--   0 root         (0) root         (0)     1752 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/providers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12614 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/providers/aws.py
+-rw-r--r--   0 root         (0) root         (0)    15146 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/providers/beaker.py
+-rw-r--r--   0 root         (0) root         (0)    28989 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/providers/openstack.py
+-rw-r--r--   0 root         (0) root         (0)    10624 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/providers/podman.py
+-rw-r--r--   0 root         (0) root         (0)    20065 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/providers/provider.py
+-rw-r--r--   0 root         (0) root         (0)     3323 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/providers/static.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 11:34:16.648416 mrack-1.9.1/src/mrack/providers/utils/
+-rw-r--r--   0 root         (0) root         (0)       64 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/providers/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2467 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/providers/utils/osapi.py
+-rw-r--r--   0 root         (0) root         (0)     6229 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/providers/utils/podman.py
+-rw-r--r--   0 root         (0) root         (0)     4688 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/providers/utils/testcloud.py
+-rw-r--r--   0 root         (0) root         (0)     6993 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/providers/virt.py
+-rw-r--r--   0 root         (0) root         (0)     7977 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 11:34:16.652416 mrack-1.9.1/src/mrack/transformers/
+-rw-r--r--   0 root         (0) root         (0)     4020 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/transformers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2602 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/transformers/aws.py
+-rw-r--r--   0 root         (0) root         (0)     7251 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/transformers/beaker.py
+-rw-r--r--   0 root         (0) root         (0)     2890 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/transformers/openstack.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/transformers/podman.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/transformers/static.py
+-rw-r--r--   0 root         (0) root         (0)     5394 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/transformers/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     2326 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/transformers/virt.py
+-rw-r--r--   0 root         (0) root         (0)    11565 2022-10-20 11:34:04.000000 mrack-1.9.1/src/mrack/utils.py
+-rw-r--r--   0 root         (0) root         (0)       47 2022-10-20 11:34:14.000000 mrack-1.9.1/src/mrack/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 11:34:16.644416 mrack-1.9.1/src/mrack.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8926 2022-10-20 11:34:16.000000 mrack-1.9.1/src/mrack.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1558 2022-10-20 11:34:16.000000 mrack-1.9.1/src/mrack.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-10-20 11:34:16.000000 mrack-1.9.1/src/mrack.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      125 2022-10-20 11:34:16.000000 mrack-1.9.1/src/mrack.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2022-10-20 11:34:16.000000 mrack-1.9.1/src/mrack.egg-info/top_level.txt
```

### Comparing `mrack-1.9.0/LICENSE` & `mrack-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/PKG-INFO` & `mrack-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrack
-Version: 1.9.0
+Version: 1.9.1
 Summary: Multicloud use-case based multihost async provisioner for CIs and testing during development
 Home-page: https://github.com/neoave/mrack
 Author: Petr Vobornik
 Author-email: pvoborni@redhat.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -162,15 +162,15 @@
 To install only some of `mrack` providers you should install `python3-mrack-{provider_name}`.
 To install mrack command a package `mrack-cli` is required.
 
 ---
 
 ## Run mrack
 
-In order to use the mrack utility a mrack.conf (e.g. [mrack.conf] from the repository(repo/blob/master/src/mrack/data/mrack.conf)) is needed.
+In order to use the mrack utility a mrack.conf (e.g. [mrack.conf] from the repository(repo/blob/main/src/mrack/data/mrack.conf)) is needed.
 
 mrack looks for the config file in following order:
 - `./` actual directory
 - `~/.mrack/` home directory
 - `/etc/mrack/` system directory
 
 Values from the configuration file could be overriden using mrack utility
```

### Comparing `mrack-1.9.0/README.md` & `mrack-1.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 To install only some of `mrack` providers you should install `python3-mrack-{provider_name}`.
 To install mrack command a package `mrack-cli` is required.
 
 ---
 
 ## Run mrack
 
-In order to use the mrack utility a mrack.conf (e.g. [mrack.conf] from the repository(repo/blob/master/src/mrack/data/mrack.conf)) is needed.
+In order to use the mrack utility a mrack.conf (e.g. [mrack.conf] from the repository(repo/blob/main/src/mrack/data/mrack.conf)) is needed.
 
 mrack looks for the config file in following order:
 - `./` actual directory
 - `~/.mrack/` home directory
 - `/etc/mrack/` system directory
 
 Values from the configuration file could be overriden using mrack utility
```

### Comparing `mrack-1.9.0/pyproject.toml` & `mrack-1.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,10 +17,10 @@
 version_variable = [
     "src/mrack/version.py:VERSION",
     "docs/conf.py:release",
 ]
 version_pattern = [
     "mrack.spec:Version:\\s+{version}",
 ]
-branch = "master"
+branch = "main"
 commit = true
 tag = true
```

### Comparing `mrack-1.9.0/scripts/mrack` & `mrack-1.9.1/scripts/mrack`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/setup.py` & `mrack-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/__init__.py` & `mrack-1.9.1/src/mrack/__init__.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/actions/__init__.py` & `mrack-1.9.1/src/mrack/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/actions/action.py` & `mrack-1.9.1/src/mrack/actions/action.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/actions/destroy.py` & `mrack-1.9.1/src/mrack/actions/destroy.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/actions/etchosts.py` & `mrack-1.9.1/src/mrack/actions/etchosts.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/actions/list.py` & `mrack-1.9.1/src/mrack/actions/list.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/actions/output.py` & `mrack-1.9.1/src/mrack/actions/output.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/actions/ssh.py` & `mrack-1.9.1/src/mrack/actions/ssh.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/actions/up.py` & `mrack-1.9.1/src/mrack/actions/up.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/config.py` & `mrack-1.9.1/src/mrack/config.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/context.py` & `mrack-1.9.1/src/mrack/context.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/data/provisioning-config.yaml` & `mrack-1.9.1/src/mrack/data/provisioning-config.yaml`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/dbdrivers/__init__.py` & `mrack-1.9.1/src/mrack/dbdrivers/__init__.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/dbdrivers/file.py` & `mrack-1.9.1/src/mrack/dbdrivers/file.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/errors.py` & `mrack-1.9.1/src/mrack/errors.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/host.py` & `mrack-1.9.1/src/mrack/host.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/outputs/__init__.py` & `mrack-1.9.1/src/mrack/outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/outputs/ansible_inventory.py` & `mrack-1.9.1/src/mrack/outputs/ansible_inventory.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/outputs/pytest_multihost.py` & `mrack-1.9.1/src/mrack/outputs/pytest_multihost.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/outputs/utils.py` & `mrack-1.9.1/src/mrack/outputs/utils.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/providers/__init__.py` & `mrack-1.9.1/src/mrack/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/providers/aws.py` & `mrack-1.9.1/src/mrack/providers/aws.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/providers/beaker.py` & `mrack-1.9.1/src/mrack/providers/beaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from xml.dom.minidom import Document as xml_doc
 from xmlrpc.client import Fault
 
 from bkr.client import BeakerJob, BeakerRecipe, BeakerRecipeSet
 from bkr.common.hub import HubProxy
 from bkr.common.pyconfig import PyConfigParser
 from gssapi.exceptions import MissingCredentialsError
+from gssapi.raw.misc import GSSError
 
 from mrack.errors import NotAuthenticatedError, ProvisioningError, ValidationError
 from mrack.host import (
     STATUS_ACTIVE,
     STATUS_DELETED,
     STATUS_ERROR,
     STATUS_OTHER,
@@ -120,14 +121,18 @@
         try:
             self.hub = HubProxy(logger=logger, conf=self.conf)
         except MissingCredentialsError as kinit_err:
             raise NotAuthenticatedError(
                 f"{self.dsp_name} needs Kerberos ticket to authenticate to BeakerHub. "
                 "Run 'kinit $USER' command to obtain Kerberos credentials."
             ) from kinit_err
+        except GSSError as hub_err:
+            raise NotAuthenticatedError(
+                f"{self.dsp_name} Unable to Create session: {hub_err}"
+            ) from hub_err
 
         login_end = datetime.now()
         login_duration = login_end - login_start
         logger.info(f"{self.dsp_name} Init duration {login_duration}")
 
     async def validate_hosts(self, reqs):
         """Validate that host requirements are well specified."""
@@ -289,35 +294,47 @@
     async def wait_till_provisioned(self, resource):
         """Wait for Beaker provisioning result."""
         beaker_id, req = resource
         log_msg_start = f"{self.dsp_name} [{req.get('name')}]"
         bkr_res = {}
         prev_status = ""
         job_url = ""
+        hub_url = self.hub._hub_url  # pylint: disable=protected-access
 
         # let us use timeout variable which is in minutes to define
         # maximum time to wait for beaker recipe to provide VM
         timeout_time = datetime.now() + timedelta(minutes=self.timeout)
 
         while datetime.now() < timeout_time:
-            bkr_res = self._get_recipe_info(beaker_id, log_msg_start=log_msg_start)
-            status = bkr_res["status"]
-            job_url = (
-                f"{self.hub._hub_url}"  # pylint: disable=protected-access
-                f"/jobs/{bkr_res['id']}"
-            )
+            prev_bkr_res = bkr_res
+            try:
+                bkr_res = self._get_recipe_info(beaker_id, log_msg_start=log_msg_start)
+            except TimeoutError as timeout:
+                logger.warning(
+                    f"{log_msg_start} Can not connect to {hub_url}: {timeout}"
+                )
+                logger.debug(
+                    f"{log_msg_start} Using previous result "
+                    f"and retrying in {self.poll_sleep:.1f}s"
+                )
+                bkr_res = prev_bkr_res
+
+            status = bkr_res.get("status", "")
+            job_url = f"{hub_url}/jobs/{bkr_res.get('id', None)}"
 
-            if prev_status != status:
+            status_changed = prev_status != status
+            if status_changed:
                 logger.info(
                     f"{log_msg_start} Job {job_url} "
                     f"has changed status ({prev_status} -> {status})"
                 )
                 prev_status = status
 
-            if self.status_map.get(status) == STATUS_PROVISIONING:
+            # if we have problem contacting hub from beginning: status will not change
+            if self.status_map.get(status) == STATUS_PROVISIONING or not status_changed:
                 await asyncio.sleep(self.poll_sleep)
             elif self.status_map.get(status) == STATUS_ACTIVE:
                 break
             elif self.status_map.get(status) in [STATUS_ERROR, STATUS_DELETED]:
                 logger.warning(
                     f"{log_msg_start} Job {job_url} has errored with status "
                     f"{status} and result {bkr_res['result']}"
```

### Comparing `mrack-1.9.0/src/mrack/providers/openstack.py` & `mrack-1.9.1/src/mrack/providers/openstack.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/providers/podman.py` & `mrack-1.9.1/src/mrack/providers/podman.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/providers/provider.py` & `mrack-1.9.1/src/mrack/providers/provider.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/providers/static.py` & `mrack-1.9.1/src/mrack/providers/static.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/providers/utils/osapi.py` & `mrack-1.9.1/src/mrack/providers/utils/osapi.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/providers/utils/podman.py` & `mrack-1.9.1/src/mrack/providers/utils/podman.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/providers/utils/testcloud.py` & `mrack-1.9.1/src/mrack/providers/utils/testcloud.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/providers/virt.py` & `mrack-1.9.1/src/mrack/providers/virt.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/run.py` & `mrack-1.9.1/src/mrack/run.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/transformers/__init__.py` & `mrack-1.9.1/src/mrack/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/transformers/aws.py` & `mrack-1.9.1/src/mrack/transformers/aws.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/transformers/beaker.py` & `mrack-1.9.1/src/mrack/transformers/beaker.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/transformers/openstack.py` & `mrack-1.9.1/src/mrack/transformers/openstack.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/transformers/podman.py` & `mrack-1.9.1/src/mrack/transformers/podman.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/transformers/static.py` & `mrack-1.9.1/src/mrack/transformers/static.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/transformers/transformer.py` & `mrack-1.9.1/src/mrack/transformers/transformer.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/transformers/virt.py` & `mrack-1.9.1/src/mrack/transformers/virt.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack/utils.py` & `mrack-1.9.1/src/mrack/utils.py`

 * *Files identical despite different names*

### Comparing `mrack-1.9.0/src/mrack.egg-info/PKG-INFO` & `mrack-1.9.1/src/mrack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrack
-Version: 1.9.0
+Version: 1.9.1
 Summary: Multicloud use-case based multihost async provisioner for CIs and testing during development
 Home-page: https://github.com/neoave/mrack
 Author: Petr Vobornik
 Author-email: pvoborni@redhat.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -162,15 +162,15 @@
 To install only some of `mrack` providers you should install `python3-mrack-{provider_name}`.
 To install mrack command a package `mrack-cli` is required.
 
 ---
 
 ## Run mrack
 
-In order to use the mrack utility a mrack.conf (e.g. [mrack.conf] from the repository(repo/blob/master/src/mrack/data/mrack.conf)) is needed.
+In order to use the mrack utility a mrack.conf (e.g. [mrack.conf] from the repository(repo/blob/main/src/mrack/data/mrack.conf)) is needed.
 
 mrack looks for the config file in following order:
 - `./` actual directory
 - `~/.mrack/` home directory
 - `/etc/mrack/` system directory
 
 Values from the configuration file could be overriden using mrack utility
```

### Comparing `mrack-1.9.0/src/mrack.egg-info/SOURCES.txt` & `mrack-1.9.1/src/mrack.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 scripts/mrack
```

