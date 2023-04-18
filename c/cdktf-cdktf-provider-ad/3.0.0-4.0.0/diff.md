# Comparing `tmp/cdktf-cdktf-provider-ad-3.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-ad-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-ad-3.0.0.tar", last modified: Tue Jan 17 14:58:58 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-ad-4.0.0.tar", last modified: Tue Apr 18 20:33:40 2023, max compression
```

## Comparing `cdktf-cdktf-provider-ad-3.0.0.tar` & `cdktf-cdktf-provider-ad-4.0.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:58:58.643711 cdktf-cdktf-provider-ad-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-01-17 14:58:58.643711 cdktf-cdktf-provider-ad-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 14:58:58.643711 cdktf-cdktf-provider-ad-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:58:58.639711 cdktf-cdktf-provider-ad-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:58:58.639711 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:58:58.639711 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   179833 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/_jsii/provider-ad@3.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:58:58.639711 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/computer/
--rw-r--r--   0 runner    (1001) docker     (123)    24808 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/computer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:58:58.639711 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/data_ad_computer/
--rw-r--r--   0 runner    (1001) docker     (123)    22888 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/data_ad_computer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:58:58.639711 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/data_ad_gpo/
--rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/data_ad_gpo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:58:58.639711 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/data_ad_group/
--rw-r--r--   0 runner    (1001) docker     (123)    18807 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/data_ad_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:58:58.643711 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/data_ad_ou/
--rw-r--r--   0 runner    (1001) docker     (123)    24289 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/data_ad_ou/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:58:58.643711 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/data_ad_user/
--rw-r--r--   0 runner    (1001) docker     (123)    23284 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/data_ad_user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:58:58.643711 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/gplink/
--rw-r--r--   0 runner    (1001) docker     (123)    27314 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/gplink/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:58:58.643711 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/gpo/
--rw-r--r--   0 runner    (1001) docker     (123)    24075 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/gpo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:58:58.643711 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/gpo_security/
--rw-r--r--   0 runner    (1001) docker     (123)   256376 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/gpo_security/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:58:58.643711 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/group/
--rw-r--r--   0 runner    (1001) docker     (123)    28552 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:58:58.643711 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/group_membership/
--rw-r--r--   0 runner    (1001) docker     (123)    20241 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/group_membership/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:58:58.643711 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/ou/
--rw-r--r--   0 runner    (1001) docker     (123)    24343 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/ou/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:58:58.643711 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    40884 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:58:58.643711 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/user/
--rw-r--r--   0 runner    (1001) docker     (123)   115343 2023-01-17 14:58:46.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:58:58.639711 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-01-17 14:58:58.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-01-17 14:58:58.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:58:58.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-17 14:58:58.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-17 14:58:58.000000 cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:33:40.084511 cdktf-cdktf-provider-ad-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.076511 cdktf-cdktf-provider-ad-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.076511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.076511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   494225 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/_jsii/provider-ad@4.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/computer/
+-rw-r--r--   0 runner    (1001) docker     (123)    25621 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/computer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_computer/
+-rw-r--r--   0 runner    (1001) docker     (123)    23659 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_computer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_gpo/
+-rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_gpo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_group/
+-rw-r--r--   0 runner    (1001) docker     (123)    19386 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_ou/
+-rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_ou/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_user/
+-rw-r--r--   0 runner    (1001) docker     (123)    23863 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/gplink/
+-rw-r--r--   0 runner    (1001) docker     (123)    28214 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/gplink/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/gpo/
+-rw-r--r--   0 runner    (1001) docker     (123)    24888 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/gpo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/gpo_security/
+-rw-r--r--   0 runner    (1001) docker     (123)   261974 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/gpo_security/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/group/
+-rw-r--r--   0 runner    (1001) docker     (123)    29539 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/group_membership/
+-rw-r--r--   0 runner    (1001) docker     (123)    20880 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/group_membership/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/ou/
+-rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/ou/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    41829 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/user/
+-rw-r--r--   0 runner    (1001) docker     (123)   119114 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.076511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-18 20:33:40.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-18 20:33:40.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:33:40.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:33:40.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 20:33:40.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-ad-3.0.0/LICENSE` & `cdktf-cdktf-provider-ad-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-ad-3.0.0/PKG-INFO` & `cdktf-cdktf-provider-ad-4.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-ad
-Version: 3.0.0
+Version: 4.0.0
 Summary: Prebuilt ad Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-ad.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-ad.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -62,15 +62,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-ad-go`](https://github.com/cdktf/cdktf-provider-ad-go) package.
 
 `go get github.com/cdktf/cdktf-provider-ad-go/ad`
 
 ## Docs
 
-Find auto-generated docs for this provider here: [./API.md](./API.md)
+Find auto-generated docs for this provider here:
+
+* [Typescript](./docs/API.typescript.md)
+* [Python](./docs/API.python.md)
+* [Java](./docs/API.java.md)
+* [C#](./docs/API.csharp.md)
+* [Go](./docs/API.go.md)
+
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-ad).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform ad Provider version 1:1. In fact, it always tracks `latest` of `~> 0.4` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-ad-3.0.0/README.md` & `cdktf-cdktf-provider-ad-4.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -38,15 +38,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-ad-go`](https://github.com/cdktf/cdktf-provider-ad-go) package.
 
 `go get github.com/cdktf/cdktf-provider-ad-go/ad`
 
 ## Docs
 
-Find auto-generated docs for this provider here: [./API.md](./API.md)
+Find auto-generated docs for this provider here:
+
+* [Typescript](./docs/API.typescript.md)
+* [Python](./docs/API.python.md)
+* [Java](./docs/API.java.md)
+* [C#](./docs/API.csharp.md)
+* [Go](./docs/API.go.md)
+
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-ad).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform ad Provider version 1:1. In fact, it always tracks `latest` of `~> 0.4` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-ad-3.0.0/setup.py` & `cdktf-cdktf-provider-ad-4.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-ad",
-    "version": "3.0.0",
+    "version": "4.0.0",
     "description": "Prebuilt ad Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-ad.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -36,37 +36,38 @@
         "cdktf_cdktf_provider_ad.group_membership",
         "cdktf_cdktf_provider_ad.ou",
         "cdktf_cdktf_provider_ad.provider",
         "cdktf_cdktf_provider_ad.user"
     ],
     "package_data": {
         "cdktf_cdktf_provider_ad._jsii": [
-            "provider-ad@3.0.0.jsii.tgz"
+            "provider-ad@4.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_ad": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdktf>=0.15.0, <0.16.0",
+        "cdktf>=0.16.0, <0.17.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.73.0, <2.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/__init__.py` & `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-ad-go`](https://github.com/cdktf/cdktf-provider-ad-go) package.
 
 `go get github.com/cdktf/cdktf-provider-ad-go/ad`
 
 ## Docs
 
-Find auto-generated docs for this provider here: [./API.md](./API.md)
+Find auto-generated docs for this provider here:
+
+* [Typescript](./docs/API.typescript.md)
+* [Python](./docs/API.python.md)
+* [Java](./docs/API.java.md)
+* [C#](./docs/API.csharp.md)
+* [Go](./docs/API.go.md)
+
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-ad).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform ad Provider version 1:1. In fact, it always tracks `latest` of `~> 0.4` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/computer/__init__.py` & `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/computer/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `ad_computer`
 
-Refer to the Terraform Registory for docs: [`ad_computer`](https://www.terraform.io/docs/providers/ad/r/computer).
+Refer to the Terraform Registory for docs: [`ad_computer`](https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/computer).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,43 +22,43 @@
 
 
 class Computer(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-ad.computer.Computer",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/ad/r/computer ad_computer}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/computer ad_computer}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
         container: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         id: typing.Optional[builtins.str] = None,
         pre2_kname: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/ad/r/computer ad_computer} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/computer ad_computer} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: The name for the computer account. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/computer#name Computer#name}
-        :param container: The DN of the container used to hold the computer account. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/computer#container Computer#container}
-        :param description: Specifies a description of the object. This parameter sets the value of the Description property for the computer object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/computer#description Computer#description}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/computer#id Computer#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param pre2_kname: The pre-win2k name for the computer account. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/computer#pre2kname Computer#pre2kname}
+        :param name: The name for the computer account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/computer#name Computer#name}
+        :param container: The DN of the container used to hold the computer account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/computer#container Computer#container}
+        :param description: Specifies a description of the object. This parameter sets the value of the Description property for the computer object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/computer#description Computer#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/computer#id Computer#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param pre2_kname: The pre-win2k name for the computer account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/computer#pre2kname Computer#pre2kname}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -229,15 +229,15 @@
     },
 )
 class ComputerConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         name: builtins.str,
         container: typing.Optional[builtins.str] = None,
@@ -249,19 +249,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: The name for the computer account. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/computer#name Computer#name}
-        :param container: The DN of the container used to hold the computer account. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/computer#container Computer#container}
-        :param description: Specifies a description of the object. This parameter sets the value of the Description property for the computer object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/computer#description Computer#description}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/computer#id Computer#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param pre2_kname: The pre-win2k name for the computer account. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/computer#pre2kname Computer#pre2kname}
+        :param name: The name for the computer account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/computer#name Computer#name}
+        :param container: The DN of the container used to hold the computer account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/computer#container Computer#container}
+        :param description: Specifies a description of the object. This parameter sets the value of the Description property for the computer object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/computer#description Computer#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/computer#id Computer#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param pre2_kname: The pre-win2k name for the computer account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/computer#pre2kname Computer#pre2kname}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1a57ce3843c326552f98827bcdf7ed3e79ad1a397454981392a02743d6aff222)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -308,20 +308,22 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("connection")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]], result)
 
     @builtins.property
-    def count(self) -> typing.Optional[jsii.Number]:
+    def count(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]]:
         '''
         :stability: experimental
         '''
         result = self._values.get("count")
-        return typing.cast(typing.Optional[jsii.Number], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]], result)
 
     @builtins.property
     def depends_on(
         self,
     ) -> typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]]:
         '''
         :stability: experimental
@@ -363,53 +365,53 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name for the computer account.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/computer#name Computer#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/computer#name Computer#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def container(self) -> typing.Optional[builtins.str]:
         '''The DN of the container used to hold the computer account.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/computer#container Computer#container}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/computer#container Computer#container}
         '''
         result = self._values.get("container")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''Specifies a description of the object. This parameter sets the value of the Description property for the computer object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/computer#description Computer#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/computer#description Computer#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/computer#id Computer#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/computer#id Computer#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def pre2_kname(self) -> typing.Optional[builtins.str]:
         '''The pre-win2k name for the computer account.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/computer#pre2kname Computer#pre2kname}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/computer#pre2kname Computer#pre2kname}
         '''
         result = self._values.get("pre2_kname")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -435,15 +437,15 @@
     *,
     name: builtins.str,
     container: typing.Optional[builtins.str] = None,
     description: typing.Optional[builtins.str] = None,
     id: typing.Optional[builtins.str] = None,
     pre2_kname: typing.Optional[builtins.str] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
@@ -478,15 +480,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__1a57ce3843c326552f98827bcdf7ed3e79ad1a397454981392a02743d6aff222(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     name: builtins.str,
     container: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/data_ad_computer/__init__.py` & `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_computer/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_ad_computer`
 
-Refer to the Terraform Registory for docs: [`data_ad_computer`](https://www.terraform.io/docs/providers/ad/d/computer).
+Refer to the Terraform Registory for docs: [`data_ad_computer`](https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/computer).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,41 +22,41 @@
 
 
 class DataAdComputer(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-ad.dataAdComputer.DataAdComputer",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/ad/d/computer ad_computer}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/computer ad_computer}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         computer_id: typing.Optional[builtins.str] = None,
         dn: typing.Optional[builtins.str] = None,
         guid: typing.Optional[builtins.str] = None,
         id: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/ad/d/computer ad_computer} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/computer ad_computer} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param computer_id: The OU's identifier. It can be the OU's GUID, SID, Distinguished Name, or SAM Account Name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/computer#computer_id DataAdComputer#computer_id}
-        :param dn: The Distinguished Name of the computer object. This field is deprecated in favour of ``computer_id``. In the future this field will be read-only. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/computer#dn DataAdComputer#dn}
-        :param guid: The GUID of the computer object. This field is deprecated in favour of ``computer_id``. In the future this field will be read-only. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/computer#guid DataAdComputer#guid}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/computer#id DataAdComputer#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param computer_id: The OU's identifier. It can be the OU's GUID, SID, Distinguished Name, or SAM Account Name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/computer#computer_id DataAdComputer#computer_id}
+        :param dn: The Distinguished Name of the computer object. This field is deprecated in favour of ``computer_id``. In the future this field will be read-only. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/computer#dn DataAdComputer#dn}
+        :param guid: The GUID of the computer object. This field is deprecated in favour of ``computer_id``. In the future this field will be read-only. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/computer#guid DataAdComputer#guid}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/computer#id DataAdComputer#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -203,15 +203,15 @@
     },
 )
 class DataAdComputerConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         computer_id: typing.Optional[builtins.str] = None,
         dn: typing.Optional[builtins.str] = None,
@@ -222,18 +222,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param computer_id: The OU's identifier. It can be the OU's GUID, SID, Distinguished Name, or SAM Account Name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/computer#computer_id DataAdComputer#computer_id}
-        :param dn: The Distinguished Name of the computer object. This field is deprecated in favour of ``computer_id``. In the future this field will be read-only. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/computer#dn DataAdComputer#dn}
-        :param guid: The GUID of the computer object. This field is deprecated in favour of ``computer_id``. In the future this field will be read-only. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/computer#guid DataAdComputer#guid}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/computer#id DataAdComputer#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param computer_id: The OU's identifier. It can be the OU's GUID, SID, Distinguished Name, or SAM Account Name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/computer#computer_id DataAdComputer#computer_id}
+        :param dn: The Distinguished Name of the computer object. This field is deprecated in favour of ``computer_id``. In the future this field will be read-only. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/computer#dn DataAdComputer#dn}
+        :param guid: The GUID of the computer object. This field is deprecated in favour of ``computer_id``. In the future this field will be read-only. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/computer#guid DataAdComputer#guid}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/computer#id DataAdComputer#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__99fed6e6b524309f23fcb6aaf9d0ec6908a674b1c5e320735e009b74647722ec)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -277,20 +277,22 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("connection")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]], result)
 
     @builtins.property
-    def count(self) -> typing.Optional[jsii.Number]:
+    def count(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]]:
         '''
         :stability: experimental
         '''
         result = self._values.get("count")
-        return typing.cast(typing.Optional[jsii.Number], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]], result)
 
     @builtins.property
     def depends_on(
         self,
     ) -> typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]]:
         '''
         :stability: experimental
@@ -332,44 +334,44 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def computer_id(self) -> typing.Optional[builtins.str]:
         '''The OU's identifier. It can be the OU's GUID, SID, Distinguished Name, or SAM Account Name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/computer#computer_id DataAdComputer#computer_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/computer#computer_id DataAdComputer#computer_id}
         '''
         result = self._values.get("computer_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def dn(self) -> typing.Optional[builtins.str]:
         '''The Distinguished Name of the computer object.
 
         This field is deprecated in favour of ``computer_id``. In the future this field will be read-only.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/computer#dn DataAdComputer#dn}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/computer#dn DataAdComputer#dn}
         '''
         result = self._values.get("dn")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def guid(self) -> typing.Optional[builtins.str]:
         '''The GUID of the computer object.
 
         This field is deprecated in favour of ``computer_id``. In the future this field will be read-only.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/computer#guid DataAdComputer#guid}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/computer#guid DataAdComputer#guid}
         '''
         result = self._values.get("guid")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/computer#id DataAdComputer#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/computer#id DataAdComputer#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -397,15 +399,15 @@
     id_: builtins.str,
     *,
     computer_id: typing.Optional[builtins.str] = None,
     dn: typing.Optional[builtins.str] = None,
     guid: typing.Optional[builtins.str] = None,
     id: typing.Optional[builtins.str] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
@@ -434,15 +436,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__99fed6e6b524309f23fcb6aaf9d0ec6908a674b1c5e320735e009b74647722ec(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     computer_id: typing.Optional[builtins.str] = None,
     dn: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/data_ad_gpo/__init__.py` & `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_gpo/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_ad_gpo`
 
-Refer to the Terraform Registory for docs: [`data_ad_gpo`](https://www.terraform.io/docs/providers/ad/d/gpo).
+Refer to the Terraform Registory for docs: [`data_ad_gpo`](https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/gpo).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,39 +22,39 @@
 
 
 class DataAdGpo(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-ad.dataAdGpo.DataAdGpo",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/ad/d/gpo ad_gpo}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/gpo ad_gpo}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         guid: typing.Optional[builtins.str] = None,
         id: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/ad/d/gpo ad_gpo} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/gpo ad_gpo} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param guid: GUID of the GPO. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/gpo#guid DataAdGpo#guid}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/gpo#id DataAdGpo#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: Name of the GPO. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/gpo#name DataAdGpo#name}
+        :param guid: GUID of the GPO. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/gpo#guid DataAdGpo#guid}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/gpo#id DataAdGpo#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Name of the GPO. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/gpo#name DataAdGpo#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -173,15 +173,15 @@
     },
 )
 class DataAdGpoConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         guid: typing.Optional[builtins.str] = None,
         id: typing.Optional[builtins.str] = None,
@@ -191,17 +191,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param guid: GUID of the GPO. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/gpo#guid DataAdGpo#guid}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/gpo#id DataAdGpo#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: Name of the GPO. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/gpo#name DataAdGpo#name}
+        :param guid: GUID of the GPO. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/gpo#guid DataAdGpo#guid}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/gpo#id DataAdGpo#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Name of the GPO. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/gpo#name DataAdGpo#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__37318e96a09296ea768979d86ba30df7d6077238bd9c147f3e2df26c07f976ca)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -242,20 +242,22 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("connection")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]], result)
 
     @builtins.property
-    def count(self) -> typing.Optional[jsii.Number]:
+    def count(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]]:
         '''
         :stability: experimental
         '''
         result = self._values.get("count")
-        return typing.cast(typing.Optional[jsii.Number], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]], result)
 
     @builtins.property
     def depends_on(
         self,
     ) -> typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]]:
         '''
         :stability: experimental
@@ -297,34 +299,34 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def guid(self) -> typing.Optional[builtins.str]:
         '''GUID of the GPO.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/gpo#guid DataAdGpo#guid}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/gpo#guid DataAdGpo#guid}
         '''
         result = self._values.get("guid")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/gpo#id DataAdGpo#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/gpo#id DataAdGpo#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''Name of the GPO.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/gpo#name DataAdGpo#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/gpo#name DataAdGpo#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -348,15 +350,15 @@
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     guid: typing.Optional[builtins.str] = None,
     id: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
@@ -379,15 +381,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__37318e96a09296ea768979d86ba30df7d6077238bd9c147f3e2df26c07f976ca(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     guid: typing.Optional[builtins.str] = None,
     id: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/data_ad_group/__init__.py` & `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_group/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_ad_group`
 
-Refer to the Terraform Registory for docs: [`data_ad_group`](https://www.terraform.io/docs/providers/ad/d/group).
+Refer to the Terraform Registory for docs: [`data_ad_group`](https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/group).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,37 +22,37 @@
 
 
 class DataAdGroup(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-ad.dataAdGroup.DataAdGroup",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/ad/d/group ad_group}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/group ad_group}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         group_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/ad/d/group ad_group} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/group ad_group} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param group_id: The group's identifier. It can be the group's GUID, SID, Distinguished Name, or SAM Account Name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/group#group_id DataAdGroup#group_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/group#id DataAdGroup#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param group_id: The group's identifier. It can be the group's GUID, SID, Distinguished Name, or SAM Account Name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/group#group_id DataAdGroup#group_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/group#id DataAdGroup#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -184,15 +184,15 @@
     },
 )
 class DataAdGroupConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         group_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
@@ -201,16 +201,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param group_id: The group's identifier. It can be the group's GUID, SID, Distinguished Name, or SAM Account Name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/group#group_id DataAdGroup#group_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/group#id DataAdGroup#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param group_id: The group's identifier. It can be the group's GUID, SID, Distinguished Name, or SAM Account Name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/group#group_id DataAdGroup#group_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/group#id DataAdGroup#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__06d14ca1b088f7ed3fe7bab7642e8a713e7f68ae41eebabc0dfab3acceed09ce)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -248,20 +248,22 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("connection")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]], result)
 
     @builtins.property
-    def count(self) -> typing.Optional[jsii.Number]:
+    def count(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]]:
         '''
         :stability: experimental
         '''
         result = self._values.get("count")
-        return typing.cast(typing.Optional[jsii.Number], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]], result)
 
     @builtins.property
     def depends_on(
         self,
     ) -> typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]]:
         '''
         :stability: experimental
@@ -303,23 +305,23 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def group_id(self) -> builtins.str:
         '''The group's identifier. It can be the group's GUID, SID, Distinguished Name, or SAM Account Name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/group#group_id DataAdGroup#group_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/group#group_id DataAdGroup#group_id}
         '''
         result = self._values.get("group_id")
         assert result is not None, "Required property 'group_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/group#id DataAdGroup#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/group#id DataAdGroup#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -345,15 +347,15 @@
 def _typecheckingstub__836f34b91509610ed79a69160477283510d5fa0b908529518d1e3af5827b22a4(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     group_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
@@ -370,15 +372,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__06d14ca1b088f7ed3fe7bab7642e8a713e7f68ae41eebabc0dfab3acceed09ce(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     group_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/data_ad_ou/__init__.py` & `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_ou/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_ad_ou`
 
-Refer to the Terraform Registory for docs: [`data_ad_ou`](https://www.terraform.io/docs/providers/ad/d/ou).
+Refer to the Terraform Registory for docs: [`data_ad_ou`](https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/ou).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,43 +22,43 @@
 
 
 class DataAdOu(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-ad.dataAdOu.DataAdOu",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/ad/d/ou ad_ou}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/ou ad_ou}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         dn: typing.Optional[builtins.str] = None,
         id: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
         ou_id: typing.Optional[builtins.str] = None,
         path: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/ad/d/ou ad_ou} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/ou ad_ou} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param dn: Distinguished Name of the OU object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/ou#dn DataAdOu#dn}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/ou#id DataAdOu#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: Name of the OU object. If this is used then the ``path`` attribute needs to be set as well. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/ou#name DataAdOu#name}
-        :param ou_id: The OU's identifier. It can be the OU's GUID, SID, Distinguished Name, or SAM Account Name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/ou#ou_id DataAdOu#ou_id}
-        :param path: Path of the OU object. If this is used then the ``Name`` attribute needs to be set as well. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/ou#path DataAdOu#path}
+        :param dn: Distinguished Name of the OU object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/ou#dn DataAdOu#dn}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/ou#id DataAdOu#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Name of the OU object. If this is used then the ``path`` attribute needs to be set as well. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/ou#name DataAdOu#name}
+        :param ou_id: The OU's identifier. It can be the OU's GUID, SID, Distinguished Name, or SAM Account Name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/ou#ou_id DataAdOu#ou_id}
+        :param path: Path of the OU object. If this is used then the ``Name`` attribute needs to be set as well. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/ou#path DataAdOu#path}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -228,15 +228,15 @@
     },
 )
 class DataAdOuConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         dn: typing.Optional[builtins.str] = None,
         id: typing.Optional[builtins.str] = None,
@@ -248,19 +248,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param dn: Distinguished Name of the OU object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/ou#dn DataAdOu#dn}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/ou#id DataAdOu#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: Name of the OU object. If this is used then the ``path`` attribute needs to be set as well. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/ou#name DataAdOu#name}
-        :param ou_id: The OU's identifier. It can be the OU's GUID, SID, Distinguished Name, or SAM Account Name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/ou#ou_id DataAdOu#ou_id}
-        :param path: Path of the OU object. If this is used then the ``Name`` attribute needs to be set as well. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/ou#path DataAdOu#path}
+        :param dn: Distinguished Name of the OU object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/ou#dn DataAdOu#dn}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/ou#id DataAdOu#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Name of the OU object. If this is used then the ``path`` attribute needs to be set as well. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/ou#name DataAdOu#name}
+        :param ou_id: The OU's identifier. It can be the OU's GUID, SID, Distinguished Name, or SAM Account Name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/ou#ou_id DataAdOu#ou_id}
+        :param path: Path of the OU object. If this is used then the ``Name`` attribute needs to be set as well. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/ou#path DataAdOu#path}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ba02a306445478fdc908405d5449d21e57ca7519a9d42c11bcf2397fef6a38e0)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -307,20 +307,22 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("connection")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]], result)
 
     @builtins.property
-    def count(self) -> typing.Optional[jsii.Number]:
+    def count(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]]:
         '''
         :stability: experimental
         '''
         result = self._values.get("count")
-        return typing.cast(typing.Optional[jsii.Number], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]], result)
 
     @builtins.property
     def depends_on(
         self,
     ) -> typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]]:
         '''
         :stability: experimental
@@ -362,52 +364,52 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def dn(self) -> typing.Optional[builtins.str]:
         '''Distinguished Name of the OU object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/ou#dn DataAdOu#dn}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/ou#dn DataAdOu#dn}
         '''
         result = self._values.get("dn")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/ou#id DataAdOu#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/ou#id DataAdOu#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''Name of the OU object. If this is used then the ``path`` attribute needs to be set as well.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/ou#name DataAdOu#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/ou#name DataAdOu#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ou_id(self) -> typing.Optional[builtins.str]:
         '''The OU's identifier. It can be the OU's GUID, SID, Distinguished Name, or SAM Account Name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/ou#ou_id DataAdOu#ou_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/ou#ou_id DataAdOu#ou_id}
         '''
         result = self._values.get("ou_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def path(self) -> typing.Optional[builtins.str]:
         '''Path of the OU object. If this is used then the ``Name`` attribute needs to be set as well.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/ou#path DataAdOu#path}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/ou#path DataAdOu#path}
         '''
         result = self._values.get("path")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -433,15 +435,15 @@
     *,
     dn: typing.Optional[builtins.str] = None,
     id: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     ou_id: typing.Optional[builtins.str] = None,
     path: typing.Optional[builtins.str] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
@@ -476,15 +478,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__ba02a306445478fdc908405d5449d21e57ca7519a9d42c11bcf2397fef6a38e0(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     dn: typing.Optional[builtins.str] = None,
     id: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/data_ad_user/__init__.py` & `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_user/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_ad_user`
 
-Refer to the Terraform Registory for docs: [`data_ad_user`](https://www.terraform.io/docs/providers/ad/d/user).
+Refer to the Terraform Registory for docs: [`data_ad_user`](https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/user).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,37 +22,37 @@
 
 
 class DataAdUser(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-ad.dataAdUser.DataAdUser",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/ad/d/user ad_user}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/user ad_user}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         user_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/ad/d/user ad_user} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/user ad_user} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param user_id: The user's identifier. It can be the group's GUID, SID, Distinguished Name, or SAM Account Name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/user#user_id DataAdUser#user_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/user#id DataAdUser#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param user_id: The user's identifier. It can be the group's GUID, SID, Distinguished Name, or SAM Account Name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/user#user_id DataAdUser#user_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/user#id DataAdUser#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -309,15 +309,15 @@
     },
 )
 class DataAdUserConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         user_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
@@ -326,16 +326,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param user_id: The user's identifier. It can be the group's GUID, SID, Distinguished Name, or SAM Account Name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/user#user_id DataAdUser#user_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/user#id DataAdUser#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param user_id: The user's identifier. It can be the group's GUID, SID, Distinguished Name, or SAM Account Name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/user#user_id DataAdUser#user_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/user#id DataAdUser#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__30b34cd90650b626b56ea2ee4c7efea03d1bffc89befa03faa7d3b9785ca8a7b)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -373,20 +373,22 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("connection")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]], result)
 
     @builtins.property
-    def count(self) -> typing.Optional[jsii.Number]:
+    def count(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]]:
         '''
         :stability: experimental
         '''
         result = self._values.get("count")
-        return typing.cast(typing.Optional[jsii.Number], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]], result)
 
     @builtins.property
     def depends_on(
         self,
     ) -> typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]]:
         '''
         :stability: experimental
@@ -428,23 +430,23 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def user_id(self) -> builtins.str:
         '''The user's identifier. It can be the group's GUID, SID, Distinguished Name, or SAM Account Name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/user#user_id DataAdUser#user_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/user#user_id DataAdUser#user_id}
         '''
         result = self._values.get("user_id")
         assert result is not None, "Required property 'user_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/d/user#id DataAdUser#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/data-sources/user#id DataAdUser#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -470,15 +472,15 @@
 def _typecheckingstub__d77e494a80f6e7a00b6f82f36a342256b711105039fa33f51a0820eba123ba07(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     user_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
@@ -495,15 +497,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__30b34cd90650b626b56ea2ee4c7efea03d1bffc89befa03faa7d3b9785ca8a7b(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     user_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/gplink/__init__.py` & `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/gplink/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `ad_gplink`
 
-Refer to the Terraform Registory for docs: [`ad_gplink`](https://www.terraform.io/docs/providers/ad/r/gplink).
+Refer to the Terraform Registory for docs: [`ad_gplink`](https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gplink).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,45 +22,45 @@
 
 
 class Gplink(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-ad.gplink.Gplink",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/ad/r/gplink ad_gplink}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gplink ad_gplink}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         gpo_guid: builtins.str,
         target_dn: builtins.str,
         enabled: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         enforced: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         id: typing.Optional[builtins.str] = None,
         order: typing.Optional[jsii.Number] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/ad/r/gplink ad_gplink} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gplink ad_gplink} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param gpo_guid: The GUID of the GPO that will be linked to the container object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gplink#gpo_guid Gplink#gpo_guid}
-        :param target_dn: The DN of the object the GPO will be linked to. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gplink#target_dn Gplink#target_dn}
-        :param enabled: Controls the state of the GP link between a GPO and a container object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gplink#enabled Gplink#enabled}
-        :param enforced: If set to true, the GPO will be enforced on the container object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gplink#enforced Gplink#enforced}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gplink#id Gplink#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param order: Sets the precedence between multiple GPOs linked to the same container object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gplink#order Gplink#order}
+        :param gpo_guid: The GUID of the GPO that will be linked to the container object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gplink#gpo_guid Gplink#gpo_guid}
+        :param target_dn: The DN of the object the GPO will be linked to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gplink#target_dn Gplink#target_dn}
+        :param enabled: Controls the state of the GP link between a GPO and a container object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gplink#enabled Gplink#enabled}
+        :param enforced: If set to true, the GPO will be enforced on the container object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gplink#enforced Gplink#enforced}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gplink#id Gplink#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param order: Sets the precedence between multiple GPOs linked to the same container object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gplink#order Gplink#order}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -245,15 +245,15 @@
     },
 )
 class GplinkConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         gpo_guid: builtins.str,
         target_dn: builtins.str,
@@ -266,20 +266,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param gpo_guid: The GUID of the GPO that will be linked to the container object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gplink#gpo_guid Gplink#gpo_guid}
-        :param target_dn: The DN of the object the GPO will be linked to. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gplink#target_dn Gplink#target_dn}
-        :param enabled: Controls the state of the GP link between a GPO and a container object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gplink#enabled Gplink#enabled}
-        :param enforced: If set to true, the GPO will be enforced on the container object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gplink#enforced Gplink#enforced}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gplink#id Gplink#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param order: Sets the precedence between multiple GPOs linked to the same container object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gplink#order Gplink#order}
+        :param gpo_guid: The GUID of the GPO that will be linked to the container object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gplink#gpo_guid Gplink#gpo_guid}
+        :param target_dn: The DN of the object the GPO will be linked to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gplink#target_dn Gplink#target_dn}
+        :param enabled: Controls the state of the GP link between a GPO and a container object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gplink#enabled Gplink#enabled}
+        :param enforced: If set to true, the GPO will be enforced on the container object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gplink#enforced Gplink#enforced}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gplink#id Gplink#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param order: Sets the precedence between multiple GPOs linked to the same container object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gplink#order Gplink#order}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__75f903f148f9920b0fb8899b8fd1a2c547fc1ddc845cbc29028ab472f5ae2366)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -328,20 +328,22 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("connection")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]], result)
 
     @builtins.property
-    def count(self) -> typing.Optional[jsii.Number]:
+    def count(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]]:
         '''
         :stability: experimental
         '''
         result = self._values.get("count")
-        return typing.cast(typing.Optional[jsii.Number], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]], result)
 
     @builtins.property
     def depends_on(
         self,
     ) -> typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]]:
         '''
         :stability: experimental
@@ -383,67 +385,67 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def gpo_guid(self) -> builtins.str:
         '''The GUID of the GPO that will be linked to the container object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gplink#gpo_guid Gplink#gpo_guid}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gplink#gpo_guid Gplink#gpo_guid}
         '''
         result = self._values.get("gpo_guid")
         assert result is not None, "Required property 'gpo_guid' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def target_dn(self) -> builtins.str:
         '''The DN of the object the GPO will be linked to.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gplink#target_dn Gplink#target_dn}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gplink#target_dn Gplink#target_dn}
         '''
         result = self._values.get("target_dn")
         assert result is not None, "Required property 'target_dn' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Controls the state of the GP link between a GPO and a container object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gplink#enabled Gplink#enabled}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gplink#enabled Gplink#enabled}
         '''
         result = self._values.get("enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def enforced(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If set to true, the GPO will be enforced on the container object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gplink#enforced Gplink#enforced}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gplink#enforced Gplink#enforced}
         '''
         result = self._values.get("enforced")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gplink#id Gplink#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gplink#id Gplink#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def order(self) -> typing.Optional[jsii.Number]:
         '''Sets the precedence between multiple GPOs linked to the same container object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gplink#order Gplink#order}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gplink#order Gplink#order}
         '''
         result = self._values.get("order")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -470,15 +472,15 @@
     gpo_guid: builtins.str,
     target_dn: builtins.str,
     enabled: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     enforced: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     id: typing.Optional[builtins.str] = None,
     order: typing.Optional[jsii.Number] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
@@ -519,15 +521,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__75f903f148f9920b0fb8899b8fd1a2c547fc1ddc845cbc29028ab472f5ae2366(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     gpo_guid: builtins.str,
     target_dn: builtins.str,
```

### Comparing `cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/gpo/__init__.py` & `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/gpo/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `ad_gpo`
 
-Refer to the Terraform Registory for docs: [`ad_gpo`](https://www.terraform.io/docs/providers/ad/r/gpo).
+Refer to the Terraform Registory for docs: [`ad_gpo`](https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,43 +22,43 @@
 
 
 class Gpo(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-ad.gpo.Gpo",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/ad/r/gpo ad_gpo}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo ad_gpo}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
         description: typing.Optional[builtins.str] = None,
         domain: typing.Optional[builtins.str] = None,
         id: typing.Optional[builtins.str] = None,
         status: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/ad/r/gpo ad_gpo} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo ad_gpo} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Name of the GPO. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo#name Gpo#name}
-        :param description: Description of the GPO. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo#description Gpo#description}
-        :param domain: Domain of the GPO. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo#domain Gpo#domain}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo#id Gpo#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param status: Status of the GPO. Can be one of ``AllSettingsEnabled``, ``UserSettingsDisabled``, ``ComputerSettingsDisabled``, or ``AllSettingsDisabled`` (case sensitive). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo#status Gpo#status}
+        :param name: Name of the GPO. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo#name Gpo#name}
+        :param description: Description of the GPO. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo#description Gpo#description}
+        :param domain: Domain of the GPO. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo#domain Gpo#domain}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo#id Gpo#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param status: Status of the GPO. Can be one of ``AllSettingsEnabled``, ``UserSettingsDisabled``, ``ComputerSettingsDisabled``, or ``AllSettingsDisabled`` (case sensitive). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo#status Gpo#status}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -224,15 +224,15 @@
     },
 )
 class GpoConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         name: builtins.str,
         description: typing.Optional[builtins.str] = None,
@@ -244,19 +244,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Name of the GPO. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo#name Gpo#name}
-        :param description: Description of the GPO. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo#description Gpo#description}
-        :param domain: Domain of the GPO. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo#domain Gpo#domain}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo#id Gpo#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param status: Status of the GPO. Can be one of ``AllSettingsEnabled``, ``UserSettingsDisabled``, ``ComputerSettingsDisabled``, or ``AllSettingsDisabled`` (case sensitive). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo#status Gpo#status}
+        :param name: Name of the GPO. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo#name Gpo#name}
+        :param description: Description of the GPO. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo#description Gpo#description}
+        :param domain: Domain of the GPO. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo#domain Gpo#domain}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo#id Gpo#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param status: Status of the GPO. Can be one of ``AllSettingsEnabled``, ``UserSettingsDisabled``, ``ComputerSettingsDisabled``, or ``AllSettingsDisabled`` (case sensitive). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo#status Gpo#status}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ff38e9174722d5cb736224355208c8fb0f0785e01763771adb5eed969541ebe9)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -303,20 +303,22 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("connection")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]], result)
 
     @builtins.property
-    def count(self) -> typing.Optional[jsii.Number]:
+    def count(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]]:
         '''
         :stability: experimental
         '''
         result = self._values.get("count")
-        return typing.cast(typing.Optional[jsii.Number], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]], result)
 
     @builtins.property
     def depends_on(
         self,
     ) -> typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]]:
         '''
         :stability: experimental
@@ -358,53 +360,53 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''Name of the GPO.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo#name Gpo#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo#name Gpo#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''Description of the GPO.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo#description Gpo#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo#description Gpo#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def domain(self) -> typing.Optional[builtins.str]:
         '''Domain of the GPO.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo#domain Gpo#domain}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo#domain Gpo#domain}
         '''
         result = self._values.get("domain")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo#id Gpo#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo#id Gpo#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def status(self) -> typing.Optional[builtins.str]:
         '''Status of the GPO. Can be one of ``AllSettingsEnabled``, ``UserSettingsDisabled``, ``ComputerSettingsDisabled``, or ``AllSettingsDisabled`` (case sensitive).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo#status Gpo#status}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo#status Gpo#status}
         '''
         result = self._values.get("status")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -430,15 +432,15 @@
     *,
     name: builtins.str,
     description: typing.Optional[builtins.str] = None,
     domain: typing.Optional[builtins.str] = None,
     id: typing.Optional[builtins.str] = None,
     status: typing.Optional[builtins.str] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
@@ -473,15 +475,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__ff38e9174722d5cb736224355208c8fb0f0785e01763771adb5eed969541ebe9(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     name: builtins.str,
     description: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/gpo_security/__init__.py` & `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/gpo_security/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `ad_gpo_security`
 
-Refer to the Terraform Registory for docs: [`ad_gpo_security`](https://www.terraform.io/docs/providers/ad/r/gpo_security).
+Refer to the Terraform Registory for docs: [`ad_gpo_security`](https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class GpoSecurity(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-ad.gpoSecurity.GpoSecurity",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/ad/r/gpo_security ad_gpo_security}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security ad_gpo_security}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         gpo_container: builtins.str,
@@ -44,39 +44,39 @@
         password_policies: typing.Optional[typing.Union["GpoSecurityPasswordPolicies", typing.Dict[builtins.str, typing.Any]]] = None,
         registry_keys: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["GpoSecurityRegistryKeys", typing.Dict[builtins.str, typing.Any]]]]] = None,
         registry_values: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["GpoSecurityRegistryValues", typing.Dict[builtins.str, typing.Any]]]]] = None,
         restricted_groups: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["GpoSecurityRestrictedGroups", typing.Dict[builtins.str, typing.Any]]]]] = None,
         system_log: typing.Optional[typing.Union["GpoSecuritySystemLog", typing.Dict[builtins.str, typing.Any]]] = None,
         system_services: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["GpoSecuritySystemServices", typing.Dict[builtins.str, typing.Any]]]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/ad/r/gpo_security ad_gpo_security} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security ad_gpo_security} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param gpo_container: The GUID of the container the security settings belong to. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#gpo_container GpoSecurity#gpo_container}
-        :param account_lockout: account_lockout block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#account_lockout GpoSecurity#account_lockout}
-        :param application_log: application_log block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#application_log GpoSecurity#application_log}
-        :param audit_log: audit_log block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_log GpoSecurity#audit_log}
-        :param event_audit: event_audit block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#event_audit GpoSecurity#event_audit}
-        :param filesystem: filesystem block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#filesystem GpoSecurity#filesystem}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#id GpoSecurity#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param kerberos_policy: kerberos_policy block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#kerberos_policy GpoSecurity#kerberos_policy}
-        :param password_policies: password_policies block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#password_policies GpoSecurity#password_policies}
-        :param registry_keys: registry_keys block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#registry_keys GpoSecurity#registry_keys}
-        :param registry_values: registry_values block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#registry_values GpoSecurity#registry_values}
-        :param restricted_groups: restricted_groups block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#restricted_groups GpoSecurity#restricted_groups}
-        :param system_log: system_log block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#system_log GpoSecurity#system_log}
-        :param system_services: system_services block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#system_services GpoSecurity#system_services}
+        :param gpo_container: The GUID of the container the security settings belong to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#gpo_container GpoSecurity#gpo_container}
+        :param account_lockout: account_lockout block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#account_lockout GpoSecurity#account_lockout}
+        :param application_log: application_log block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#application_log GpoSecurity#application_log}
+        :param audit_log: audit_log block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_log GpoSecurity#audit_log}
+        :param event_audit: event_audit block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#event_audit GpoSecurity#event_audit}
+        :param filesystem: filesystem block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#filesystem GpoSecurity#filesystem}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#id GpoSecurity#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param kerberos_policy: kerberos_policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#kerberos_policy GpoSecurity#kerberos_policy}
+        :param password_policies: password_policies block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#password_policies GpoSecurity#password_policies}
+        :param registry_keys: registry_keys block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#registry_keys GpoSecurity#registry_keys}
+        :param registry_values: registry_values block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#registry_values GpoSecurity#registry_values}
+        :param restricted_groups: restricted_groups block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#restricted_groups GpoSecurity#restricted_groups}
+        :param system_log: system_log block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#system_log GpoSecurity#system_log}
+        :param system_services: system_services block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#system_services GpoSecurity#system_services}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -117,18 +117,18 @@
         *,
         force_logoff_when_hour_expire: typing.Optional[builtins.str] = None,
         lockout_bad_count: typing.Optional[builtins.str] = None,
         lockout_duration: typing.Optional[builtins.str] = None,
         reset_lockout_count: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param force_logoff_when_hour_expire: Disconnect SMB sessions when logon hours expire. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#force_logoff_when_hour_expire GpoSecurity#force_logoff_when_hour_expire}
-        :param lockout_bad_count: Number of failed logon attempts until a account is locked. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#lockout_bad_count GpoSecurity#lockout_bad_count}
-        :param lockout_duration: Number of minutes a locked out account must remain locked out. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#lockout_duration GpoSecurity#lockout_duration}
-        :param reset_lockout_count: Number of minutes a account will remain locked after a failed logon attempt. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#reset_lockout_count GpoSecurity#reset_lockout_count}
+        :param force_logoff_when_hour_expire: Disconnect SMB sessions when logon hours expire. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#force_logoff_when_hour_expire GpoSecurity#force_logoff_when_hour_expire}
+        :param lockout_bad_count: Number of failed logon attempts until a account is locked. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#lockout_bad_count GpoSecurity#lockout_bad_count}
+        :param lockout_duration: Number of minutes a locked out account must remain locked out. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#lockout_duration GpoSecurity#lockout_duration}
+        :param reset_lockout_count: Number of minutes a account will remain locked after a failed logon attempt. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#reset_lockout_count GpoSecurity#reset_lockout_count}
         '''
         value = GpoSecurityAccountLockout(
             force_logoff_when_hour_expire=force_logoff_when_hour_expire,
             lockout_bad_count=lockout_bad_count,
             lockout_duration=lockout_duration,
             reset_lockout_count=reset_lockout_count,
         )
@@ -141,18 +141,18 @@
         *,
         audit_log_retention_period: typing.Optional[builtins.str] = None,
         maximum_log_size: typing.Optional[builtins.str] = None,
         restrict_guest_access: typing.Optional[builtins.str] = None,
         retention_days: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param audit_log_retention_period: Control log retention. Values: 0: overwrite events as needed, 1: overwrite events as specified specified by ``retention_days``, 2: never overwrite events. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_log_retention_period GpoSecurity#audit_log_retention_period}
-        :param maximum_log_size: Maximum size of log in KiloBytes. (64-4194240). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#maximum_log_size GpoSecurity#maximum_log_size}
-        :param restrict_guest_access: Restrict access to logs for guest users. A non-zero value restricts access to guest users. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#restrict_guest_access GpoSecurity#restrict_guest_access}
-        :param retention_days: Number of days before new events overwrite old events. (1-365). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#retention_days GpoSecurity#retention_days}
+        :param audit_log_retention_period: Control log retention. Values: 0: overwrite events as needed, 1: overwrite events as specified specified by ``retention_days``, 2: never overwrite events. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_log_retention_period GpoSecurity#audit_log_retention_period}
+        :param maximum_log_size: Maximum size of log in KiloBytes. (64-4194240). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#maximum_log_size GpoSecurity#maximum_log_size}
+        :param restrict_guest_access: Restrict access to logs for guest users. A non-zero value restricts access to guest users. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#restrict_guest_access GpoSecurity#restrict_guest_access}
+        :param retention_days: Number of days before new events overwrite old events. (1-365). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#retention_days GpoSecurity#retention_days}
         '''
         value = GpoSecurityApplicationLog(
             audit_log_retention_period=audit_log_retention_period,
             maximum_log_size=maximum_log_size,
             restrict_guest_access=restrict_guest_access,
             retention_days=retention_days,
         )
@@ -165,18 +165,18 @@
         *,
         audit_log_retention_period: typing.Optional[builtins.str] = None,
         maximum_log_size: typing.Optional[builtins.str] = None,
         restrict_guest_access: typing.Optional[builtins.str] = None,
         retention_days: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param audit_log_retention_period: Control log retention. Values: 0: overwrite events as needed, 1: overwrite events as specified specified by ``retention_days``, 2: never overwrite events. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_log_retention_period GpoSecurity#audit_log_retention_period}
-        :param maximum_log_size: Maximum size of log in KiloBytes. (64-4194240). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#maximum_log_size GpoSecurity#maximum_log_size}
-        :param restrict_guest_access: Restrict access to logs for guest users. A non-zero value restricts access to guest users. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#restrict_guest_access GpoSecurity#restrict_guest_access}
-        :param retention_days: Number of days before new events overwrite old events. (1-365). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#retention_days GpoSecurity#retention_days}
+        :param audit_log_retention_period: Control log retention. Values: 0: overwrite events as needed, 1: overwrite events as specified specified by ``retention_days``, 2: never overwrite events. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_log_retention_period GpoSecurity#audit_log_retention_period}
+        :param maximum_log_size: Maximum size of log in KiloBytes. (64-4194240). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#maximum_log_size GpoSecurity#maximum_log_size}
+        :param restrict_guest_access: Restrict access to logs for guest users. A non-zero value restricts access to guest users. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#restrict_guest_access GpoSecurity#restrict_guest_access}
+        :param retention_days: Number of days before new events overwrite old events. (1-365). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#retention_days GpoSecurity#retention_days}
         '''
         value = GpoSecurityAuditLog(
             audit_log_retention_period=audit_log_retention_period,
             maximum_log_size=maximum_log_size,
             restrict_guest_access=restrict_guest_access,
             retention_days=retention_days,
         )
@@ -194,23 +194,23 @@
         audit_object_access: typing.Optional[builtins.str] = None,
         audit_policy_change: typing.Optional[builtins.str] = None,
         audit_privilege_use: typing.Optional[builtins.str] = None,
         audit_process_tracking: typing.Optional[builtins.str] = None,
         audit_system_events: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param audit_account_logon: Audit credential validation. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_account_logon GpoSecurity#audit_account_logon}
-        :param audit_account_manage: Audit account management events. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_account_manage GpoSecurity#audit_account_manage}
-        :param audit_ds_access: Audit access attempts to AD objects. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_ds_access GpoSecurity#audit_ds_access}
-        :param audit_logon_events: Audit logon events. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_logon_events GpoSecurity#audit_logon_events}
-        :param audit_object_access: Audit access attempts to non-AD objects. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_object_access GpoSecurity#audit_object_access}
-        :param audit_policy_change: Audit attempts to change a policy. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_policy_change GpoSecurity#audit_policy_change}
-        :param audit_privilege_use: Audit user attempts of exercising user rights. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_privilege_use GpoSecurity#audit_privilege_use}
-        :param audit_process_tracking: Audit process related events. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_process_tracking GpoSecurity#audit_process_tracking}
-        :param audit_system_events: Audit system events. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_system_events GpoSecurity#audit_system_events}
+        :param audit_account_logon: Audit credential validation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_account_logon GpoSecurity#audit_account_logon}
+        :param audit_account_manage: Audit account management events. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_account_manage GpoSecurity#audit_account_manage}
+        :param audit_ds_access: Audit access attempts to AD objects. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_ds_access GpoSecurity#audit_ds_access}
+        :param audit_logon_events: Audit logon events. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_logon_events GpoSecurity#audit_logon_events}
+        :param audit_object_access: Audit access attempts to non-AD objects. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_object_access GpoSecurity#audit_object_access}
+        :param audit_policy_change: Audit attempts to change a policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_policy_change GpoSecurity#audit_policy_change}
+        :param audit_privilege_use: Audit user attempts of exercising user rights. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_privilege_use GpoSecurity#audit_privilege_use}
+        :param audit_process_tracking: Audit process related events. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_process_tracking GpoSecurity#audit_process_tracking}
+        :param audit_system_events: Audit system events. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_system_events GpoSecurity#audit_system_events}
         '''
         value = GpoSecurityEventAudit(
             audit_account_logon=audit_account_logon,
             audit_account_manage=audit_account_manage,
             audit_ds_access=audit_ds_access,
             audit_logon_events=audit_logon_events,
             audit_object_access=audit_object_access,
@@ -242,19 +242,19 @@
         max_clock_skew: typing.Optional[builtins.str] = None,
         max_renew_age: typing.Optional[builtins.str] = None,
         max_service_age: typing.Optional[builtins.str] = None,
         max_ticket_age: typing.Optional[builtins.str] = None,
         ticket_validate_client: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param max_clock_skew: Maximum time difference, in minutes, between the client clock and the server clock. (0-99999). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#max_clock_skew GpoSecurity#max_clock_skew}
-        :param max_renew_age: Number of days during which a ticket-granting ticket can be renewed (0-99999). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#max_renew_age GpoSecurity#max_renew_age}
-        :param max_service_age: Maximum amount of minutes a ticket must be valid to access a service or resource. Minimum should be 10 and maximum should be equal to ``max_ticket_age``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#max_service_age GpoSecurity#max_service_age}
-        :param max_ticket_age: Maximum amount of hours a ticket-granting ticket is valid (0-99999). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#max_ticket_age GpoSecurity#max_ticket_age}
-        :param ticket_validate_client: Control if the session ticket is validated for every request. A non-zero value disables the policy. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#ticket_validate_client GpoSecurity#ticket_validate_client}
+        :param max_clock_skew: Maximum time difference, in minutes, between the client clock and the server clock. (0-99999). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#max_clock_skew GpoSecurity#max_clock_skew}
+        :param max_renew_age: Number of days during which a ticket-granting ticket can be renewed (0-99999). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#max_renew_age GpoSecurity#max_renew_age}
+        :param max_service_age: Maximum amount of minutes a ticket must be valid to access a service or resource. Minimum should be 10 and maximum should be equal to ``max_ticket_age``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#max_service_age GpoSecurity#max_service_age}
+        :param max_ticket_age: Maximum amount of hours a ticket-granting ticket is valid (0-99999). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#max_ticket_age GpoSecurity#max_ticket_age}
+        :param ticket_validate_client: Control if the session ticket is validated for every request. A non-zero value disables the policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#ticket_validate_client GpoSecurity#ticket_validate_client}
         '''
         value = GpoSecurityKerberosPolicy(
             max_clock_skew=max_clock_skew,
             max_renew_age=max_renew_age,
             max_service_age=max_service_age,
             max_ticket_age=max_ticket_age,
             ticket_validate_client=ticket_validate_client,
@@ -270,20 +270,20 @@
         maximum_password_age: typing.Optional[builtins.str] = None,
         minimum_password_age: typing.Optional[builtins.str] = None,
         minimum_password_length: typing.Optional[builtins.str] = None,
         password_complexity: typing.Optional[builtins.str] = None,
         password_history_size: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param clear_text_password: Store password with reversible encryption (0-2^16). The password will not be stored with reversible encryption if the value is set to 0. Reversible encryption will be used in any other case. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#clear_text_password GpoSecurity#clear_text_password}
-        :param maximum_password_age: Number of days before password expires (-1-999). If set to -1, it means the password never expires. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#maximum_password_age GpoSecurity#maximum_password_age}
-        :param minimum_password_age: Number of days a password must be used before changing it (0-999). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#minimum_password_age GpoSecurity#minimum_password_age}
-        :param minimum_password_length: Minimum number of characters used in a password (0-2^16). If set to 0, it means no password is required. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#minimum_password_length GpoSecurity#minimum_password_length}
-        :param password_complexity: Password must meet complexity requirements (0-2^16). If set to 0, then requirements do not apply, any other value means requirements are applied Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#password_complexity GpoSecurity#password_complexity}
-        :param password_history_size: The number of unique new passwords that are required before an old password can be reused in association with a user account (0-2^16). A value of 0 indicates that the password history is disabled. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#password_history_size GpoSecurity#password_history_size}
+        :param clear_text_password: Store password with reversible encryption (0-2^16). The password will not be stored with reversible encryption if the value is set to 0. Reversible encryption will be used in any other case. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#clear_text_password GpoSecurity#clear_text_password}
+        :param maximum_password_age: Number of days before password expires (-1-999). If set to -1, it means the password never expires. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#maximum_password_age GpoSecurity#maximum_password_age}
+        :param minimum_password_age: Number of days a password must be used before changing it (0-999). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#minimum_password_age GpoSecurity#minimum_password_age}
+        :param minimum_password_length: Minimum number of characters used in a password (0-2^16). If set to 0, it means no password is required. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#minimum_password_length GpoSecurity#minimum_password_length}
+        :param password_complexity: Password must meet complexity requirements (0-2^16). If set to 0, then requirements do not apply, any other value means requirements are applied Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#password_complexity GpoSecurity#password_complexity}
+        :param password_history_size: The number of unique new passwords that are required before an old password can be reused in association with a user account (0-2^16). A value of 0 indicates that the password history is disabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#password_history_size GpoSecurity#password_history_size}
         '''
         value = GpoSecurityPasswordPolicies(
             clear_text_password=clear_text_password,
             maximum_password_age=maximum_password_age,
             minimum_password_age=minimum_password_age,
             minimum_password_length=minimum_password_length,
             password_complexity=password_complexity,
@@ -337,18 +337,18 @@
         *,
         audit_log_retention_period: typing.Optional[builtins.str] = None,
         maximum_log_size: typing.Optional[builtins.str] = None,
         restrict_guest_access: typing.Optional[builtins.str] = None,
         retention_days: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param audit_log_retention_period: Control log retention. Values: 0: overwrite events as needed, 1: overwrite events as specified specified by ``retention_days``, 2: never overwrite events. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_log_retention_period GpoSecurity#audit_log_retention_period}
-        :param maximum_log_size: Maximum size of log in KiloBytes. (64-4194240). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#maximum_log_size GpoSecurity#maximum_log_size}
-        :param restrict_guest_access: Restrict access to logs for guest users. A non-zero value restricts access to guest users. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#restrict_guest_access GpoSecurity#restrict_guest_access}
-        :param retention_days: Number of days before new events overwrite old events. (1-365). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#retention_days GpoSecurity#retention_days}
+        :param audit_log_retention_period: Control log retention. Values: 0: overwrite events as needed, 1: overwrite events as specified specified by ``retention_days``, 2: never overwrite events. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_log_retention_period GpoSecurity#audit_log_retention_period}
+        :param maximum_log_size: Maximum size of log in KiloBytes. (64-4194240). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#maximum_log_size GpoSecurity#maximum_log_size}
+        :param restrict_guest_access: Restrict access to logs for guest users. A non-zero value restricts access to guest users. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#restrict_guest_access GpoSecurity#restrict_guest_access}
+        :param retention_days: Number of days before new events overwrite old events. (1-365). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#retention_days GpoSecurity#retention_days}
         '''
         value = GpoSecuritySystemLog(
             audit_log_retention_period=audit_log_retention_period,
             maximum_log_size=maximum_log_size,
             restrict_guest_access=restrict_guest_access,
             retention_days=retention_days,
         )
@@ -610,18 +610,18 @@
         *,
         force_logoff_when_hour_expire: typing.Optional[builtins.str] = None,
         lockout_bad_count: typing.Optional[builtins.str] = None,
         lockout_duration: typing.Optional[builtins.str] = None,
         reset_lockout_count: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param force_logoff_when_hour_expire: Disconnect SMB sessions when logon hours expire. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#force_logoff_when_hour_expire GpoSecurity#force_logoff_when_hour_expire}
-        :param lockout_bad_count: Number of failed logon attempts until a account is locked. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#lockout_bad_count GpoSecurity#lockout_bad_count}
-        :param lockout_duration: Number of minutes a locked out account must remain locked out. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#lockout_duration GpoSecurity#lockout_duration}
-        :param reset_lockout_count: Number of minutes a account will remain locked after a failed logon attempt. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#reset_lockout_count GpoSecurity#reset_lockout_count}
+        :param force_logoff_when_hour_expire: Disconnect SMB sessions when logon hours expire. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#force_logoff_when_hour_expire GpoSecurity#force_logoff_when_hour_expire}
+        :param lockout_bad_count: Number of failed logon attempts until a account is locked. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#lockout_bad_count GpoSecurity#lockout_bad_count}
+        :param lockout_duration: Number of minutes a locked out account must remain locked out. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#lockout_duration GpoSecurity#lockout_duration}
+        :param reset_lockout_count: Number of minutes a account will remain locked after a failed logon attempt. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#reset_lockout_count GpoSecurity#reset_lockout_count}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cacf0f22d18e2b8532d32516e2fd1a537c0c00aaee04dca03763d69b225ff8c1)
             check_type(argname="argument force_logoff_when_hour_expire", value=force_logoff_when_hour_expire, expected_type=type_hints["force_logoff_when_hour_expire"])
             check_type(argname="argument lockout_bad_count", value=lockout_bad_count, expected_type=type_hints["lockout_bad_count"])
             check_type(argname="argument lockout_duration", value=lockout_duration, expected_type=type_hints["lockout_duration"])
             check_type(argname="argument reset_lockout_count", value=reset_lockout_count, expected_type=type_hints["reset_lockout_count"])
@@ -635,42 +635,42 @@
         if reset_lockout_count is not None:
             self._values["reset_lockout_count"] = reset_lockout_count
 
     @builtins.property
     def force_logoff_when_hour_expire(self) -> typing.Optional[builtins.str]:
         '''Disconnect SMB sessions when logon hours expire.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#force_logoff_when_hour_expire GpoSecurity#force_logoff_when_hour_expire}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#force_logoff_when_hour_expire GpoSecurity#force_logoff_when_hour_expire}
         '''
         result = self._values.get("force_logoff_when_hour_expire")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def lockout_bad_count(self) -> typing.Optional[builtins.str]:
         '''Number of failed logon attempts until a account is locked.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#lockout_bad_count GpoSecurity#lockout_bad_count}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#lockout_bad_count GpoSecurity#lockout_bad_count}
         '''
         result = self._values.get("lockout_bad_count")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def lockout_duration(self) -> typing.Optional[builtins.str]:
         '''Number of minutes a locked out account must remain locked out.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#lockout_duration GpoSecurity#lockout_duration}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#lockout_duration GpoSecurity#lockout_duration}
         '''
         result = self._values.get("lockout_duration")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def reset_lockout_count(self) -> typing.Optional[builtins.str]:
         '''Number of minutes a account will remain locked after a failed logon attempt.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#reset_lockout_count GpoSecurity#reset_lockout_count}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#reset_lockout_count GpoSecurity#reset_lockout_count}
         '''
         result = self._values.get("reset_lockout_count")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -816,18 +816,18 @@
         *,
         audit_log_retention_period: typing.Optional[builtins.str] = None,
         maximum_log_size: typing.Optional[builtins.str] = None,
         restrict_guest_access: typing.Optional[builtins.str] = None,
         retention_days: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param audit_log_retention_period: Control log retention. Values: 0: overwrite events as needed, 1: overwrite events as specified specified by ``retention_days``, 2: never overwrite events. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_log_retention_period GpoSecurity#audit_log_retention_period}
-        :param maximum_log_size: Maximum size of log in KiloBytes. (64-4194240). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#maximum_log_size GpoSecurity#maximum_log_size}
-        :param restrict_guest_access: Restrict access to logs for guest users. A non-zero value restricts access to guest users. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#restrict_guest_access GpoSecurity#restrict_guest_access}
-        :param retention_days: Number of days before new events overwrite old events. (1-365). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#retention_days GpoSecurity#retention_days}
+        :param audit_log_retention_period: Control log retention. Values: 0: overwrite events as needed, 1: overwrite events as specified specified by ``retention_days``, 2: never overwrite events. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_log_retention_period GpoSecurity#audit_log_retention_period}
+        :param maximum_log_size: Maximum size of log in KiloBytes. (64-4194240). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#maximum_log_size GpoSecurity#maximum_log_size}
+        :param restrict_guest_access: Restrict access to logs for guest users. A non-zero value restricts access to guest users. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#restrict_guest_access GpoSecurity#restrict_guest_access}
+        :param retention_days: Number of days before new events overwrite old events. (1-365). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#retention_days GpoSecurity#retention_days}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e0d73debdd5e6d72575b43ce6044d3ea0513f21b83c4340353a0baa55419e7ca)
             check_type(argname="argument audit_log_retention_period", value=audit_log_retention_period, expected_type=type_hints["audit_log_retention_period"])
             check_type(argname="argument maximum_log_size", value=maximum_log_size, expected_type=type_hints["maximum_log_size"])
             check_type(argname="argument restrict_guest_access", value=restrict_guest_access, expected_type=type_hints["restrict_guest_access"])
             check_type(argname="argument retention_days", value=retention_days, expected_type=type_hints["retention_days"])
@@ -843,42 +843,42 @@
 
     @builtins.property
     def audit_log_retention_period(self) -> typing.Optional[builtins.str]:
         '''Control log retention.
 
         Values: 0: overwrite events as needed, 1: overwrite events as specified specified by ``retention_days``, 2: never overwrite events.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_log_retention_period GpoSecurity#audit_log_retention_period}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_log_retention_period GpoSecurity#audit_log_retention_period}
         '''
         result = self._values.get("audit_log_retention_period")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def maximum_log_size(self) -> typing.Optional[builtins.str]:
         '''Maximum size of log in KiloBytes. (64-4194240).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#maximum_log_size GpoSecurity#maximum_log_size}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#maximum_log_size GpoSecurity#maximum_log_size}
         '''
         result = self._values.get("maximum_log_size")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def restrict_guest_access(self) -> typing.Optional[builtins.str]:
         '''Restrict access to logs for guest users. A non-zero value restricts access to guest users.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#restrict_guest_access GpoSecurity#restrict_guest_access}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#restrict_guest_access GpoSecurity#restrict_guest_access}
         '''
         result = self._values.get("restrict_guest_access")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def retention_days(self) -> typing.Optional[builtins.str]:
         '''Number of days before new events overwrite old events. (1-365).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#retention_days GpoSecurity#retention_days}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#retention_days GpoSecurity#retention_days}
         '''
         result = self._values.get("retention_days")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1024,18 +1024,18 @@
         *,
         audit_log_retention_period: typing.Optional[builtins.str] = None,
         maximum_log_size: typing.Optional[builtins.str] = None,
         restrict_guest_access: typing.Optional[builtins.str] = None,
         retention_days: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param audit_log_retention_period: Control log retention. Values: 0: overwrite events as needed, 1: overwrite events as specified specified by ``retention_days``, 2: never overwrite events. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_log_retention_period GpoSecurity#audit_log_retention_period}
-        :param maximum_log_size: Maximum size of log in KiloBytes. (64-4194240). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#maximum_log_size GpoSecurity#maximum_log_size}
-        :param restrict_guest_access: Restrict access to logs for guest users. A non-zero value restricts access to guest users. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#restrict_guest_access GpoSecurity#restrict_guest_access}
-        :param retention_days: Number of days before new events overwrite old events. (1-365). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#retention_days GpoSecurity#retention_days}
+        :param audit_log_retention_period: Control log retention. Values: 0: overwrite events as needed, 1: overwrite events as specified specified by ``retention_days``, 2: never overwrite events. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_log_retention_period GpoSecurity#audit_log_retention_period}
+        :param maximum_log_size: Maximum size of log in KiloBytes. (64-4194240). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#maximum_log_size GpoSecurity#maximum_log_size}
+        :param restrict_guest_access: Restrict access to logs for guest users. A non-zero value restricts access to guest users. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#restrict_guest_access GpoSecurity#restrict_guest_access}
+        :param retention_days: Number of days before new events overwrite old events. (1-365). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#retention_days GpoSecurity#retention_days}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__85435532b75fbdc4dc1b2e8e371b20c3191694415025fee1e3e76c4cae5b9108)
             check_type(argname="argument audit_log_retention_period", value=audit_log_retention_period, expected_type=type_hints["audit_log_retention_period"])
             check_type(argname="argument maximum_log_size", value=maximum_log_size, expected_type=type_hints["maximum_log_size"])
             check_type(argname="argument restrict_guest_access", value=restrict_guest_access, expected_type=type_hints["restrict_guest_access"])
             check_type(argname="argument retention_days", value=retention_days, expected_type=type_hints["retention_days"])
@@ -1051,42 +1051,42 @@
 
     @builtins.property
     def audit_log_retention_period(self) -> typing.Optional[builtins.str]:
         '''Control log retention.
 
         Values: 0: overwrite events as needed, 1: overwrite events as specified specified by ``retention_days``, 2: never overwrite events.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_log_retention_period GpoSecurity#audit_log_retention_period}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_log_retention_period GpoSecurity#audit_log_retention_period}
         '''
         result = self._values.get("audit_log_retention_period")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def maximum_log_size(self) -> typing.Optional[builtins.str]:
         '''Maximum size of log in KiloBytes. (64-4194240).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#maximum_log_size GpoSecurity#maximum_log_size}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#maximum_log_size GpoSecurity#maximum_log_size}
         '''
         result = self._values.get("maximum_log_size")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def restrict_guest_access(self) -> typing.Optional[builtins.str]:
         '''Restrict access to logs for guest users. A non-zero value restricts access to guest users.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#restrict_guest_access GpoSecurity#restrict_guest_access}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#restrict_guest_access GpoSecurity#restrict_guest_access}
         '''
         result = self._values.get("restrict_guest_access")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def retention_days(self) -> typing.Optional[builtins.str]:
         '''Number of days before new events overwrite old events. (1-365).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#retention_days GpoSecurity#retention_days}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#retention_days GpoSecurity#retention_days}
         '''
         result = self._values.get("retention_days")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1244,15 +1244,15 @@
     },
 )
 class GpoSecurityConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         gpo_container: builtins.str,
         account_lockout: typing.Optional[typing.Union[GpoSecurityAccountLockout, typing.Dict[builtins.str, typing.Any]]] = None,
@@ -1273,28 +1273,28 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param gpo_container: The GUID of the container the security settings belong to. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#gpo_container GpoSecurity#gpo_container}
-        :param account_lockout: account_lockout block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#account_lockout GpoSecurity#account_lockout}
-        :param application_log: application_log block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#application_log GpoSecurity#application_log}
-        :param audit_log: audit_log block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_log GpoSecurity#audit_log}
-        :param event_audit: event_audit block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#event_audit GpoSecurity#event_audit}
-        :param filesystem: filesystem block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#filesystem GpoSecurity#filesystem}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#id GpoSecurity#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param kerberos_policy: kerberos_policy block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#kerberos_policy GpoSecurity#kerberos_policy}
-        :param password_policies: password_policies block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#password_policies GpoSecurity#password_policies}
-        :param registry_keys: registry_keys block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#registry_keys GpoSecurity#registry_keys}
-        :param registry_values: registry_values block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#registry_values GpoSecurity#registry_values}
-        :param restricted_groups: restricted_groups block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#restricted_groups GpoSecurity#restricted_groups}
-        :param system_log: system_log block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#system_log GpoSecurity#system_log}
-        :param system_services: system_services block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#system_services GpoSecurity#system_services}
+        :param gpo_container: The GUID of the container the security settings belong to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#gpo_container GpoSecurity#gpo_container}
+        :param account_lockout: account_lockout block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#account_lockout GpoSecurity#account_lockout}
+        :param application_log: application_log block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#application_log GpoSecurity#application_log}
+        :param audit_log: audit_log block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_log GpoSecurity#audit_log}
+        :param event_audit: event_audit block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#event_audit GpoSecurity#event_audit}
+        :param filesystem: filesystem block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#filesystem GpoSecurity#filesystem}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#id GpoSecurity#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param kerberos_policy: kerberos_policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#kerberos_policy GpoSecurity#kerberos_policy}
+        :param password_policies: password_policies block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#password_policies GpoSecurity#password_policies}
+        :param registry_keys: registry_keys block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#registry_keys GpoSecurity#registry_keys}
+        :param registry_values: registry_values block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#registry_values GpoSecurity#registry_values}
+        :param restricted_groups: restricted_groups block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#restricted_groups GpoSecurity#restricted_groups}
+        :param system_log: system_log block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#system_log GpoSecurity#system_log}
+        :param system_services: system_services block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#system_services GpoSecurity#system_services}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(account_lockout, dict):
             account_lockout = GpoSecurityAccountLockout(**account_lockout)
         if isinstance(application_log, dict):
             application_log = GpoSecurityApplicationLog(**application_log)
@@ -1382,20 +1382,22 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("connection")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]], result)
 
     @builtins.property
-    def count(self) -> typing.Optional[jsii.Number]:
+    def count(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]]:
         '''
         :stability: experimental
         '''
         result = self._values.get("count")
-        return typing.cast(typing.Optional[jsii.Number], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]], result)
 
     @builtins.property
     def depends_on(
         self,
     ) -> typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]]:
         '''
         :stability: experimental
@@ -1437,144 +1439,144 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def gpo_container(self) -> builtins.str:
         '''The GUID of the container the security settings belong to.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#gpo_container GpoSecurity#gpo_container}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#gpo_container GpoSecurity#gpo_container}
         '''
         result = self._values.get("gpo_container")
         assert result is not None, "Required property 'gpo_container' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def account_lockout(self) -> typing.Optional[GpoSecurityAccountLockout]:
         '''account_lockout block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#account_lockout GpoSecurity#account_lockout}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#account_lockout GpoSecurity#account_lockout}
         '''
         result = self._values.get("account_lockout")
         return typing.cast(typing.Optional[GpoSecurityAccountLockout], result)
 
     @builtins.property
     def application_log(self) -> typing.Optional[GpoSecurityApplicationLog]:
         '''application_log block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#application_log GpoSecurity#application_log}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#application_log GpoSecurity#application_log}
         '''
         result = self._values.get("application_log")
         return typing.cast(typing.Optional[GpoSecurityApplicationLog], result)
 
     @builtins.property
     def audit_log(self) -> typing.Optional[GpoSecurityAuditLog]:
         '''audit_log block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_log GpoSecurity#audit_log}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_log GpoSecurity#audit_log}
         '''
         result = self._values.get("audit_log")
         return typing.cast(typing.Optional[GpoSecurityAuditLog], result)
 
     @builtins.property
     def event_audit(self) -> typing.Optional["GpoSecurityEventAudit"]:
         '''event_audit block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#event_audit GpoSecurity#event_audit}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#event_audit GpoSecurity#event_audit}
         '''
         result = self._values.get("event_audit")
         return typing.cast(typing.Optional["GpoSecurityEventAudit"], result)
 
     @builtins.property
     def filesystem(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["GpoSecurityFilesystem"]]]:
         '''filesystem block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#filesystem GpoSecurity#filesystem}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#filesystem GpoSecurity#filesystem}
         '''
         result = self._values.get("filesystem")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["GpoSecurityFilesystem"]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#id GpoSecurity#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#id GpoSecurity#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def kerberos_policy(self) -> typing.Optional["GpoSecurityKerberosPolicy"]:
         '''kerberos_policy block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#kerberos_policy GpoSecurity#kerberos_policy}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#kerberos_policy GpoSecurity#kerberos_policy}
         '''
         result = self._values.get("kerberos_policy")
         return typing.cast(typing.Optional["GpoSecurityKerberosPolicy"], result)
 
     @builtins.property
     def password_policies(self) -> typing.Optional["GpoSecurityPasswordPolicies"]:
         '''password_policies block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#password_policies GpoSecurity#password_policies}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#password_policies GpoSecurity#password_policies}
         '''
         result = self._values.get("password_policies")
         return typing.cast(typing.Optional["GpoSecurityPasswordPolicies"], result)
 
     @builtins.property
     def registry_keys(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["GpoSecurityRegistryKeys"]]]:
         '''registry_keys block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#registry_keys GpoSecurity#registry_keys}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#registry_keys GpoSecurity#registry_keys}
         '''
         result = self._values.get("registry_keys")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["GpoSecurityRegistryKeys"]]], result)
 
     @builtins.property
     def registry_values(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["GpoSecurityRegistryValues"]]]:
         '''registry_values block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#registry_values GpoSecurity#registry_values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#registry_values GpoSecurity#registry_values}
         '''
         result = self._values.get("registry_values")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["GpoSecurityRegistryValues"]]], result)
 
     @builtins.property
     def restricted_groups(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["GpoSecurityRestrictedGroups"]]]:
         '''restricted_groups block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#restricted_groups GpoSecurity#restricted_groups}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#restricted_groups GpoSecurity#restricted_groups}
         '''
         result = self._values.get("restricted_groups")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["GpoSecurityRestrictedGroups"]]], result)
 
     @builtins.property
     def system_log(self) -> typing.Optional["GpoSecuritySystemLog"]:
         '''system_log block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#system_log GpoSecurity#system_log}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#system_log GpoSecurity#system_log}
         '''
         result = self._values.get("system_log")
         return typing.cast(typing.Optional["GpoSecuritySystemLog"], result)
 
     @builtins.property
     def system_services(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["GpoSecuritySystemServices"]]]:
         '''system_services block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#system_services GpoSecurity#system_services}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#system_services GpoSecurity#system_services}
         '''
         result = self._values.get("system_services")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["GpoSecuritySystemServices"]]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1613,23 +1615,23 @@
         audit_object_access: typing.Optional[builtins.str] = None,
         audit_policy_change: typing.Optional[builtins.str] = None,
         audit_privilege_use: typing.Optional[builtins.str] = None,
         audit_process_tracking: typing.Optional[builtins.str] = None,
         audit_system_events: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param audit_account_logon: Audit credential validation. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_account_logon GpoSecurity#audit_account_logon}
-        :param audit_account_manage: Audit account management events. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_account_manage GpoSecurity#audit_account_manage}
-        :param audit_ds_access: Audit access attempts to AD objects. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_ds_access GpoSecurity#audit_ds_access}
-        :param audit_logon_events: Audit logon events. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_logon_events GpoSecurity#audit_logon_events}
-        :param audit_object_access: Audit access attempts to non-AD objects. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_object_access GpoSecurity#audit_object_access}
-        :param audit_policy_change: Audit attempts to change a policy. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_policy_change GpoSecurity#audit_policy_change}
-        :param audit_privilege_use: Audit user attempts of exercising user rights. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_privilege_use GpoSecurity#audit_privilege_use}
-        :param audit_process_tracking: Audit process related events. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_process_tracking GpoSecurity#audit_process_tracking}
-        :param audit_system_events: Audit system events. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_system_events GpoSecurity#audit_system_events}
+        :param audit_account_logon: Audit credential validation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_account_logon GpoSecurity#audit_account_logon}
+        :param audit_account_manage: Audit account management events. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_account_manage GpoSecurity#audit_account_manage}
+        :param audit_ds_access: Audit access attempts to AD objects. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_ds_access GpoSecurity#audit_ds_access}
+        :param audit_logon_events: Audit logon events. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_logon_events GpoSecurity#audit_logon_events}
+        :param audit_object_access: Audit access attempts to non-AD objects. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_object_access GpoSecurity#audit_object_access}
+        :param audit_policy_change: Audit attempts to change a policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_policy_change GpoSecurity#audit_policy_change}
+        :param audit_privilege_use: Audit user attempts of exercising user rights. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_privilege_use GpoSecurity#audit_privilege_use}
+        :param audit_process_tracking: Audit process related events. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_process_tracking GpoSecurity#audit_process_tracking}
+        :param audit_system_events: Audit system events. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_system_events GpoSecurity#audit_system_events}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__04f36083c93644f3b8249fda0271cc7369ecb371f6324297bdf28af4eb49ed93)
             check_type(argname="argument audit_account_logon", value=audit_account_logon, expected_type=type_hints["audit_account_logon"])
             check_type(argname="argument audit_account_manage", value=audit_account_manage, expected_type=type_hints["audit_account_manage"])
             check_type(argname="argument audit_ds_access", value=audit_ds_access, expected_type=type_hints["audit_ds_access"])
             check_type(argname="argument audit_logon_events", value=audit_logon_events, expected_type=type_hints["audit_logon_events"])
@@ -1658,87 +1660,87 @@
         if audit_system_events is not None:
             self._values["audit_system_events"] = audit_system_events
 
     @builtins.property
     def audit_account_logon(self) -> typing.Optional[builtins.str]:
         '''Audit credential validation.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_account_logon GpoSecurity#audit_account_logon}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_account_logon GpoSecurity#audit_account_logon}
         '''
         result = self._values.get("audit_account_logon")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def audit_account_manage(self) -> typing.Optional[builtins.str]:
         '''Audit account management events.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_account_manage GpoSecurity#audit_account_manage}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_account_manage GpoSecurity#audit_account_manage}
         '''
         result = self._values.get("audit_account_manage")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def audit_ds_access(self) -> typing.Optional[builtins.str]:
         '''Audit access attempts to AD objects.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_ds_access GpoSecurity#audit_ds_access}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_ds_access GpoSecurity#audit_ds_access}
         '''
         result = self._values.get("audit_ds_access")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def audit_logon_events(self) -> typing.Optional[builtins.str]:
         '''Audit logon events.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_logon_events GpoSecurity#audit_logon_events}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_logon_events GpoSecurity#audit_logon_events}
         '''
         result = self._values.get("audit_logon_events")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def audit_object_access(self) -> typing.Optional[builtins.str]:
         '''Audit access attempts to non-AD objects.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_object_access GpoSecurity#audit_object_access}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_object_access GpoSecurity#audit_object_access}
         '''
         result = self._values.get("audit_object_access")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def audit_policy_change(self) -> typing.Optional[builtins.str]:
         '''Audit attempts to change a policy.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_policy_change GpoSecurity#audit_policy_change}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_policy_change GpoSecurity#audit_policy_change}
         '''
         result = self._values.get("audit_policy_change")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def audit_privilege_use(self) -> typing.Optional[builtins.str]:
         '''Audit user attempts of exercising user rights.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_privilege_use GpoSecurity#audit_privilege_use}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_privilege_use GpoSecurity#audit_privilege_use}
         '''
         result = self._values.get("audit_privilege_use")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def audit_process_tracking(self) -> typing.Optional[builtins.str]:
         '''Audit process related events.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_process_tracking GpoSecurity#audit_process_tracking}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_process_tracking GpoSecurity#audit_process_tracking}
         '''
         result = self._values.get("audit_process_tracking")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def audit_system_events(self) -> typing.Optional[builtins.str]:
         '''Audit system events.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_system_events GpoSecurity#audit_system_events}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_system_events GpoSecurity#audit_system_events}
         '''
         result = self._values.get("audit_system_events")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1983,17 +1985,17 @@
         self,
         *,
         acl: builtins.str,
         path: builtins.str,
         propagation_mode: builtins.str,
     ) -> None:
         '''
-        :param acl: Security descriptor to apply. (https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-dtyp/f4296d69-1c0f-491f-9587-a960b292d070). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#acl GpoSecurity#acl}
-        :param path: Path of the file or directory. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#path GpoSecurity#path}
-        :param propagation_mode: Control permission propagation. 0: Propagate permissions to all subfolders and files, 1: Replace existing permissions on all subfolders and files, 2: Do not allow permissions to be replaced. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#propagation_mode GpoSecurity#propagation_mode}
+        :param acl: Security descriptor to apply. (https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-dtyp/f4296d69-1c0f-491f-9587-a960b292d070). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#acl GpoSecurity#acl}
+        :param path: Path of the file or directory. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#path GpoSecurity#path}
+        :param propagation_mode: Control permission propagation. 0: Propagate permissions to all subfolders and files, 1: Replace existing permissions on all subfolders and files, 2: Do not allow permissions to be replaced. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#propagation_mode GpoSecurity#propagation_mode}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f1e47ad0df9ce1f0d0dca5122a3c2d58890a35639017d7ef682e0539a203733f)
             check_type(argname="argument acl", value=acl, expected_type=type_hints["acl"])
             check_type(argname="argument path", value=path, expected_type=type_hints["path"])
             check_type(argname="argument propagation_mode", value=propagation_mode, expected_type=type_hints["propagation_mode"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -2002,37 +2004,37 @@
             "propagation_mode": propagation_mode,
         }
 
     @builtins.property
     def acl(self) -> builtins.str:
         '''Security descriptor to apply. (https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-dtyp/f4296d69-1c0f-491f-9587-a960b292d070).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#acl GpoSecurity#acl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#acl GpoSecurity#acl}
         '''
         result = self._values.get("acl")
         assert result is not None, "Required property 'acl' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def path(self) -> builtins.str:
         '''Path of the file or directory.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#path GpoSecurity#path}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#path GpoSecurity#path}
         '''
         result = self._values.get("path")
         assert result is not None, "Required property 'path' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def propagation_mode(self) -> builtins.str:
         '''Control permission propagation.
 
         0: Propagate permissions to all subfolders and files, 1: Replace existing permissions on all subfolders and files, 2: Do not allow permissions to be replaced.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#propagation_mode GpoSecurity#propagation_mode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#propagation_mode GpoSecurity#propagation_mode}
         '''
         result = self._values.get("propagation_mode")
         assert result is not None, "Required property 'propagation_mode' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -2249,19 +2251,19 @@
         max_clock_skew: typing.Optional[builtins.str] = None,
         max_renew_age: typing.Optional[builtins.str] = None,
         max_service_age: typing.Optional[builtins.str] = None,
         max_ticket_age: typing.Optional[builtins.str] = None,
         ticket_validate_client: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param max_clock_skew: Maximum time difference, in minutes, between the client clock and the server clock. (0-99999). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#max_clock_skew GpoSecurity#max_clock_skew}
-        :param max_renew_age: Number of days during which a ticket-granting ticket can be renewed (0-99999). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#max_renew_age GpoSecurity#max_renew_age}
-        :param max_service_age: Maximum amount of minutes a ticket must be valid to access a service or resource. Minimum should be 10 and maximum should be equal to ``max_ticket_age``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#max_service_age GpoSecurity#max_service_age}
-        :param max_ticket_age: Maximum amount of hours a ticket-granting ticket is valid (0-99999). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#max_ticket_age GpoSecurity#max_ticket_age}
-        :param ticket_validate_client: Control if the session ticket is validated for every request. A non-zero value disables the policy. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#ticket_validate_client GpoSecurity#ticket_validate_client}
+        :param max_clock_skew: Maximum time difference, in minutes, between the client clock and the server clock. (0-99999). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#max_clock_skew GpoSecurity#max_clock_skew}
+        :param max_renew_age: Number of days during which a ticket-granting ticket can be renewed (0-99999). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#max_renew_age GpoSecurity#max_renew_age}
+        :param max_service_age: Maximum amount of minutes a ticket must be valid to access a service or resource. Minimum should be 10 and maximum should be equal to ``max_ticket_age``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#max_service_age GpoSecurity#max_service_age}
+        :param max_ticket_age: Maximum amount of hours a ticket-granting ticket is valid (0-99999). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#max_ticket_age GpoSecurity#max_ticket_age}
+        :param ticket_validate_client: Control if the session ticket is validated for every request. A non-zero value disables the policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#ticket_validate_client GpoSecurity#ticket_validate_client}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__02abc20895ee902d3e4eeb6d435b574318c54664742937967fdb55e9c67d803b)
             check_type(argname="argument max_clock_skew", value=max_clock_skew, expected_type=type_hints["max_clock_skew"])
             check_type(argname="argument max_renew_age", value=max_renew_age, expected_type=type_hints["max_renew_age"])
             check_type(argname="argument max_service_age", value=max_service_age, expected_type=type_hints["max_service_age"])
             check_type(argname="argument max_ticket_age", value=max_ticket_age, expected_type=type_hints["max_ticket_age"])
@@ -2278,53 +2280,53 @@
         if ticket_validate_client is not None:
             self._values["ticket_validate_client"] = ticket_validate_client
 
     @builtins.property
     def max_clock_skew(self) -> typing.Optional[builtins.str]:
         '''Maximum time difference, in minutes, between the client clock and the server clock. (0-99999).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#max_clock_skew GpoSecurity#max_clock_skew}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#max_clock_skew GpoSecurity#max_clock_skew}
         '''
         result = self._values.get("max_clock_skew")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def max_renew_age(self) -> typing.Optional[builtins.str]:
         '''Number of days during which a ticket-granting ticket can be renewed (0-99999).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#max_renew_age GpoSecurity#max_renew_age}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#max_renew_age GpoSecurity#max_renew_age}
         '''
         result = self._values.get("max_renew_age")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def max_service_age(self) -> typing.Optional[builtins.str]:
         '''Maximum amount of minutes a ticket must be valid to access a service or resource.
 
         Minimum should be 10 and maximum should be equal to ``max_ticket_age``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#max_service_age GpoSecurity#max_service_age}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#max_service_age GpoSecurity#max_service_age}
         '''
         result = self._values.get("max_service_age")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def max_ticket_age(self) -> typing.Optional[builtins.str]:
         '''Maximum amount of hours a ticket-granting ticket is valid (0-99999).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#max_ticket_age GpoSecurity#max_ticket_age}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#max_ticket_age GpoSecurity#max_ticket_age}
         '''
         result = self._values.get("max_ticket_age")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ticket_validate_client(self) -> typing.Optional[builtins.str]:
         '''Control if the session ticket is validated for every request. A non-zero value disables the policy.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#ticket_validate_client GpoSecurity#ticket_validate_client}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#ticket_validate_client GpoSecurity#ticket_validate_client}
         '''
         result = self._values.get("ticket_validate_client")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -2495,20 +2497,20 @@
         maximum_password_age: typing.Optional[builtins.str] = None,
         minimum_password_age: typing.Optional[builtins.str] = None,
         minimum_password_length: typing.Optional[builtins.str] = None,
         password_complexity: typing.Optional[builtins.str] = None,
         password_history_size: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param clear_text_password: Store password with reversible encryption (0-2^16). The password will not be stored with reversible encryption if the value is set to 0. Reversible encryption will be used in any other case. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#clear_text_password GpoSecurity#clear_text_password}
-        :param maximum_password_age: Number of days before password expires (-1-999). If set to -1, it means the password never expires. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#maximum_password_age GpoSecurity#maximum_password_age}
-        :param minimum_password_age: Number of days a password must be used before changing it (0-999). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#minimum_password_age GpoSecurity#minimum_password_age}
-        :param minimum_password_length: Minimum number of characters used in a password (0-2^16). If set to 0, it means no password is required. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#minimum_password_length GpoSecurity#minimum_password_length}
-        :param password_complexity: Password must meet complexity requirements (0-2^16). If set to 0, then requirements do not apply, any other value means requirements are applied Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#password_complexity GpoSecurity#password_complexity}
-        :param password_history_size: The number of unique new passwords that are required before an old password can be reused in association with a user account (0-2^16). A value of 0 indicates that the password history is disabled. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#password_history_size GpoSecurity#password_history_size}
+        :param clear_text_password: Store password with reversible encryption (0-2^16). The password will not be stored with reversible encryption if the value is set to 0. Reversible encryption will be used in any other case. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#clear_text_password GpoSecurity#clear_text_password}
+        :param maximum_password_age: Number of days before password expires (-1-999). If set to -1, it means the password never expires. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#maximum_password_age GpoSecurity#maximum_password_age}
+        :param minimum_password_age: Number of days a password must be used before changing it (0-999). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#minimum_password_age GpoSecurity#minimum_password_age}
+        :param minimum_password_length: Minimum number of characters used in a password (0-2^16). If set to 0, it means no password is required. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#minimum_password_length GpoSecurity#minimum_password_length}
+        :param password_complexity: Password must meet complexity requirements (0-2^16). If set to 0, then requirements do not apply, any other value means requirements are applied Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#password_complexity GpoSecurity#password_complexity}
+        :param password_history_size: The number of unique new passwords that are required before an old password can be reused in association with a user account (0-2^16). A value of 0 indicates that the password history is disabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#password_history_size GpoSecurity#password_history_size}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7e772677afd93a9ada091ed35eef2d3076c0e7452d28b59f4cadf651231179e0)
             check_type(argname="argument clear_text_password", value=clear_text_password, expected_type=type_hints["clear_text_password"])
             check_type(argname="argument maximum_password_age", value=maximum_password_age, expected_type=type_hints["maximum_password_age"])
             check_type(argname="argument minimum_password_age", value=minimum_password_age, expected_type=type_hints["minimum_password_age"])
             check_type(argname="argument minimum_password_length", value=minimum_password_length, expected_type=type_hints["minimum_password_length"])
@@ -2530,64 +2532,64 @@
 
     @builtins.property
     def clear_text_password(self) -> typing.Optional[builtins.str]:
         '''Store password with reversible encryption (0-2^16).
 
         The password will not be stored with reversible encryption if the value is set to 0. Reversible encryption will be used in any other case.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#clear_text_password GpoSecurity#clear_text_password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#clear_text_password GpoSecurity#clear_text_password}
         '''
         result = self._values.get("clear_text_password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def maximum_password_age(self) -> typing.Optional[builtins.str]:
         '''Number of days before password expires (-1-999). If set to -1, it means the password never expires.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#maximum_password_age GpoSecurity#maximum_password_age}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#maximum_password_age GpoSecurity#maximum_password_age}
         '''
         result = self._values.get("maximum_password_age")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def minimum_password_age(self) -> typing.Optional[builtins.str]:
         '''Number of days a password must be used before changing it (0-999).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#minimum_password_age GpoSecurity#minimum_password_age}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#minimum_password_age GpoSecurity#minimum_password_age}
         '''
         result = self._values.get("minimum_password_age")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def minimum_password_length(self) -> typing.Optional[builtins.str]:
         '''Minimum number of characters used in a password (0-2^16). If set to 0, it means no password is required.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#minimum_password_length GpoSecurity#minimum_password_length}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#minimum_password_length GpoSecurity#minimum_password_length}
         '''
         result = self._values.get("minimum_password_length")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def password_complexity(self) -> typing.Optional[builtins.str]:
         '''Password must meet complexity requirements (0-2^16).
 
         If set to 0, then requirements do not apply, any other value means requirements are applied
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#password_complexity GpoSecurity#password_complexity}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#password_complexity GpoSecurity#password_complexity}
         '''
         result = self._values.get("password_complexity")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def password_history_size(self) -> typing.Optional[builtins.str]:
         '''The number of unique new passwords that are required before an old password can be reused in association with a user account (0-2^16).
 
         A value of 0 indicates that the password history is disabled.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#password_history_size GpoSecurity#password_history_size}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#password_history_size GpoSecurity#password_history_size}
         '''
         result = self._values.get("password_history_size")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -2776,17 +2778,17 @@
         self,
         *,
         acl: builtins.str,
         key_name: builtins.str,
         propagation_mode: builtins.str,
     ) -> None:
         '''
-        :param acl: Security descriptor to apply. (https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-dtyp/f4296d69-1c0f-491f-9587-a960b292d070). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#acl GpoSecurity#acl}
-        :param key_name: Fully qualified name of the key (https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rrp/97587de7-3524-4291-8527-3951711 0c0eb). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#key_name GpoSecurity#key_name}
-        :param propagation_mode: Control permission propagation. 0: Propagate permissions to all subkeys, 1: Replace existing permissions on all subkeys, 2: Do not allow permissions to be replaced on the key. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#propagation_mode GpoSecurity#propagation_mode}
+        :param acl: Security descriptor to apply. (https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-dtyp/f4296d69-1c0f-491f-9587-a960b292d070). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#acl GpoSecurity#acl}
+        :param key_name: Fully qualified name of the key (https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rrp/97587de7-3524-4291-8527-3951711 0c0eb). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#key_name GpoSecurity#key_name}
+        :param propagation_mode: Control permission propagation. 0: Propagate permissions to all subkeys, 1: Replace existing permissions on all subkeys, 2: Do not allow permissions to be replaced on the key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#propagation_mode GpoSecurity#propagation_mode}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__fe2524f50e031da606c37d83319cf14a6e3f93f6fe4121cdb0bd21b257287ecf)
             check_type(argname="argument acl", value=acl, expected_type=type_hints["acl"])
             check_type(argname="argument key_name", value=key_name, expected_type=type_hints["key_name"])
             check_type(argname="argument propagation_mode", value=propagation_mode, expected_type=type_hints["propagation_mode"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -2795,37 +2797,37 @@
             "propagation_mode": propagation_mode,
         }
 
     @builtins.property
     def acl(self) -> builtins.str:
         '''Security descriptor to apply. (https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-dtyp/f4296d69-1c0f-491f-9587-a960b292d070).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#acl GpoSecurity#acl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#acl GpoSecurity#acl}
         '''
         result = self._values.get("acl")
         assert result is not None, "Required property 'acl' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def key_name(self) -> builtins.str:
         '''Fully qualified name of the key (https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rrp/97587de7-3524-4291-8527-3951711      0c0eb).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#key_name GpoSecurity#key_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#key_name GpoSecurity#key_name}
         '''
         result = self._values.get("key_name")
         assert result is not None, "Required property 'key_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def propagation_mode(self) -> builtins.str:
         '''Control permission propagation.
 
         0: Propagate permissions to all subkeys, 1: Replace existing permissions on all subkeys, 2: Do not allow permissions to be replaced on the key.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#propagation_mode GpoSecurity#propagation_mode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#propagation_mode GpoSecurity#propagation_mode}
         '''
         result = self._values.get("propagation_mode")
         assert result is not None, "Required property 'propagation_mode' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -3034,17 +3036,17 @@
         self,
         *,
         key_name: builtins.str,
         value: builtins.str,
         value_type: builtins.str,
     ) -> None:
         '''
-        :param key_name: Fully qualified name of the key (https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rrp/97587de7-3524-4291-8527-39517110c0eb). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#key_name GpoSecurity#key_name}
-        :param value: The value of the key, matching the type set in ``value_type``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#value GpoSecurity#value}
-        :param value_type: Data type of the key's value. 1: String, 2: Expand String, 3: Binary, 4: DWORD, 5: MULTI_SZ. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#value_type GpoSecurity#value_type}
+        :param key_name: Fully qualified name of the key (https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rrp/97587de7-3524-4291-8527-39517110c0eb). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#key_name GpoSecurity#key_name}
+        :param value: The value of the key, matching the type set in ``value_type``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#value GpoSecurity#value}
+        :param value_type: Data type of the key's value. 1: String, 2: Expand String, 3: Binary, 4: DWORD, 5: MULTI_SZ. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#value_type GpoSecurity#value_type}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__75bfb8fdde1f9e13205db062cd76b5fa0b133f6b623a99890f9f5cbbd069d3c6)
             check_type(argname="argument key_name", value=key_name, expected_type=type_hints["key_name"])
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             check_type(argname="argument value_type", value=value_type, expected_type=type_hints["value_type"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -3053,35 +3055,35 @@
             "value_type": value_type,
         }
 
     @builtins.property
     def key_name(self) -> builtins.str:
         '''Fully qualified name of the key (https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rrp/97587de7-3524-4291-8527-39517110c0eb).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#key_name GpoSecurity#key_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#key_name GpoSecurity#key_name}
         '''
         result = self._values.get("key_name")
         assert result is not None, "Required property 'key_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def value(self) -> builtins.str:
         '''The value of the key, matching the type set in ``value_type``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#value GpoSecurity#value}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#value GpoSecurity#value}
         '''
         result = self._values.get("value")
         assert result is not None, "Required property 'value' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def value_type(self) -> builtins.str:
         '''Data type of the key's value. 1: String, 2: Expand String, 3: Binary, 4: DWORD, 5: MULTI_SZ.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#value_type GpoSecurity#value_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#value_type GpoSecurity#value_type}
         '''
         result = self._values.get("value_type")
         assert result is not None, "Required property 'value_type' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -3294,17 +3296,17 @@
         self,
         *,
         group_memberof: builtins.str,
         group_members: builtins.str,
         group_name: builtins.str,
     ) -> None:
         '''
-        :param group_memberof: Comma separated list of group names or SIDs that this group belongs to. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#group_memberof GpoSecurity#group_memberof}
-        :param group_members: Comma separated list of group names or SIDs that are members of the group. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#group_members GpoSecurity#group_members}
-        :param group_name: Name of the group we are managing. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#group_name GpoSecurity#group_name}
+        :param group_memberof: Comma separated list of group names or SIDs that this group belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#group_memberof GpoSecurity#group_memberof}
+        :param group_members: Comma separated list of group names or SIDs that are members of the group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#group_members GpoSecurity#group_members}
+        :param group_name: Name of the group we are managing. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#group_name GpoSecurity#group_name}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4ce42a35443ab69779568df4c7a89ae66e130c3bcc77f1818bff49ca65bf24c6)
             check_type(argname="argument group_memberof", value=group_memberof, expected_type=type_hints["group_memberof"])
             check_type(argname="argument group_members", value=group_members, expected_type=type_hints["group_members"])
             check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -3313,35 +3315,35 @@
             "group_name": group_name,
         }
 
     @builtins.property
     def group_memberof(self) -> builtins.str:
         '''Comma separated list of group names or SIDs that this group belongs to.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#group_memberof GpoSecurity#group_memberof}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#group_memberof GpoSecurity#group_memberof}
         '''
         result = self._values.get("group_memberof")
         assert result is not None, "Required property 'group_memberof' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def group_members(self) -> builtins.str:
         '''Comma separated list of group names or SIDs that are members of the group.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#group_members GpoSecurity#group_members}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#group_members GpoSecurity#group_members}
         '''
         result = self._values.get("group_members")
         assert result is not None, "Required property 'group_members' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def group_name(self) -> builtins.str:
         '''Name of the group we are managing.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#group_name GpoSecurity#group_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#group_name GpoSecurity#group_name}
         '''
         result = self._values.get("group_name")
         assert result is not None, "Required property 'group_name' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -3556,18 +3558,18 @@
         *,
         audit_log_retention_period: typing.Optional[builtins.str] = None,
         maximum_log_size: typing.Optional[builtins.str] = None,
         restrict_guest_access: typing.Optional[builtins.str] = None,
         retention_days: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param audit_log_retention_period: Control log retention. Values: 0: overwrite events as needed, 1: overwrite events as specified specified by ``retention_days``, 2: never overwrite events. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_log_retention_period GpoSecurity#audit_log_retention_period}
-        :param maximum_log_size: Maximum size of log in KiloBytes. (64-4194240). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#maximum_log_size GpoSecurity#maximum_log_size}
-        :param restrict_guest_access: Restrict access to logs for guest users. A non-zero value restricts access to guest users. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#restrict_guest_access GpoSecurity#restrict_guest_access}
-        :param retention_days: Number of days before new events overwrite old events. (1-365). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#retention_days GpoSecurity#retention_days}
+        :param audit_log_retention_period: Control log retention. Values: 0: overwrite events as needed, 1: overwrite events as specified specified by ``retention_days``, 2: never overwrite events. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_log_retention_period GpoSecurity#audit_log_retention_period}
+        :param maximum_log_size: Maximum size of log in KiloBytes. (64-4194240). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#maximum_log_size GpoSecurity#maximum_log_size}
+        :param restrict_guest_access: Restrict access to logs for guest users. A non-zero value restricts access to guest users. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#restrict_guest_access GpoSecurity#restrict_guest_access}
+        :param retention_days: Number of days before new events overwrite old events. (1-365). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#retention_days GpoSecurity#retention_days}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1e76d4551a024fb277187dfd83ead93a052d42a6ad199ce2ded65afa58e6ce6d)
             check_type(argname="argument audit_log_retention_period", value=audit_log_retention_period, expected_type=type_hints["audit_log_retention_period"])
             check_type(argname="argument maximum_log_size", value=maximum_log_size, expected_type=type_hints["maximum_log_size"])
             check_type(argname="argument restrict_guest_access", value=restrict_guest_access, expected_type=type_hints["restrict_guest_access"])
             check_type(argname="argument retention_days", value=retention_days, expected_type=type_hints["retention_days"])
@@ -3583,42 +3585,42 @@
 
     @builtins.property
     def audit_log_retention_period(self) -> typing.Optional[builtins.str]:
         '''Control log retention.
 
         Values: 0: overwrite events as needed, 1: overwrite events as specified specified by ``retention_days``, 2: never overwrite events.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#audit_log_retention_period GpoSecurity#audit_log_retention_period}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#audit_log_retention_period GpoSecurity#audit_log_retention_period}
         '''
         result = self._values.get("audit_log_retention_period")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def maximum_log_size(self) -> typing.Optional[builtins.str]:
         '''Maximum size of log in KiloBytes. (64-4194240).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#maximum_log_size GpoSecurity#maximum_log_size}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#maximum_log_size GpoSecurity#maximum_log_size}
         '''
         result = self._values.get("maximum_log_size")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def restrict_guest_access(self) -> typing.Optional[builtins.str]:
         '''Restrict access to logs for guest users. A non-zero value restricts access to guest users.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#restrict_guest_access GpoSecurity#restrict_guest_access}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#restrict_guest_access GpoSecurity#restrict_guest_access}
         '''
         result = self._values.get("restrict_guest_access")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def retention_days(self) -> typing.Optional[builtins.str]:
         '''Number of days before new events overwrite old events. (1-365).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#retention_days GpoSecurity#retention_days}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#retention_days GpoSecurity#retention_days}
         '''
         result = self._values.get("retention_days")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -3762,17 +3764,17 @@
         self,
         *,
         acl: builtins.str,
         service_name: builtins.str,
         startup_mode: builtins.str,
     ) -> None:
         '''
-        :param acl: Security descriptor to apply. (https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-dtyp/f4296d69-1c0f-491f-9587-a960b292d070). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#acl GpoSecurity#acl}
-        :param service_name: Name of the service. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#service_name GpoSecurity#service_name}
-        :param startup_mode: Startup mode of the service. Possible values are 2: Automatic, 3: Manual, 4: Disabled. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#startup_mode GpoSecurity#startup_mode}
+        :param acl: Security descriptor to apply. (https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-dtyp/f4296d69-1c0f-491f-9587-a960b292d070). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#acl GpoSecurity#acl}
+        :param service_name: Name of the service. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#service_name GpoSecurity#service_name}
+        :param startup_mode: Startup mode of the service. Possible values are 2: Automatic, 3: Manual, 4: Disabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#startup_mode GpoSecurity#startup_mode}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2188d074c1f3c10a2818a60856846a4340c28f6588dcf5329ee38be44e09433a)
             check_type(argname="argument acl", value=acl, expected_type=type_hints["acl"])
             check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
             check_type(argname="argument startup_mode", value=startup_mode, expected_type=type_hints["startup_mode"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -3781,35 +3783,35 @@
             "startup_mode": startup_mode,
         }
 
     @builtins.property
     def acl(self) -> builtins.str:
         '''Security descriptor to apply. (https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-dtyp/f4296d69-1c0f-491f-9587-a960b292d070).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#acl GpoSecurity#acl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#acl GpoSecurity#acl}
         '''
         result = self._values.get("acl")
         assert result is not None, "Required property 'acl' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def service_name(self) -> builtins.str:
         '''Name of the service.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#service_name GpoSecurity#service_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#service_name GpoSecurity#service_name}
         '''
         result = self._values.get("service_name")
         assert result is not None, "Required property 'service_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def startup_mode(self) -> builtins.str:
         '''Startup mode of the service. Possible values are 2: Automatic, 3: Manual, 4: Disabled.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/gpo_security#startup_mode GpoSecurity#startup_mode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/gpo_security#startup_mode GpoSecurity#startup_mode}
         '''
         result = self._values.get("startup_mode")
         assert result is not None, "Required property 'startup_mode' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -4059,15 +4061,15 @@
     password_policies: typing.Optional[typing.Union[GpoSecurityPasswordPolicies, typing.Dict[builtins.str, typing.Any]]] = None,
     registry_keys: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[GpoSecurityRegistryKeys, typing.Dict[builtins.str, typing.Any]]]]] = None,
     registry_values: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[GpoSecurityRegistryValues, typing.Dict[builtins.str, typing.Any]]]]] = None,
     restricted_groups: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[GpoSecurityRestrictedGroups, typing.Dict[builtins.str, typing.Any]]]]] = None,
     system_log: typing.Optional[typing.Union[GpoSecuritySystemLog, typing.Dict[builtins.str, typing.Any]]] = None,
     system_services: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[GpoSecuritySystemServices, typing.Dict[builtins.str, typing.Any]]]]] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
@@ -4255,15 +4257,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__813fbf075deae0a8dfc08469b9da1745f51d18e18bfeb83aa92f4d8ad9e55094(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     gpo_container: builtins.str,
     account_lockout: typing.Optional[typing.Union[GpoSecurityAccountLockout, typing.Dict[builtins.str, typing.Any]]] = None,
```

### Comparing `cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/group/__init__.py` & `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/group/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `ad_group`
 
-Refer to the Terraform Registory for docs: [`ad_group`](https://www.terraform.io/docs/providers/ad/r/group).
+Refer to the Terraform Registory for docs: [`ad_group`](https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,47 +22,47 @@
 
 
 class Group(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-ad.group.Group",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/ad/r/group ad_group}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group ad_group}.'''
 
     def __init__(
         self,
         scope_: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         container: builtins.str,
         name: builtins.str,
         sam_account_name: builtins.str,
         category: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         id: typing.Optional[builtins.str] = None,
         scope: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/ad/r/group ad_group} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group ad_group} Resource.
 
         :param scope_: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param container: A DN of a container object holding the group. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group#container Group#container}
-        :param name: The name of the group. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group#name Group#name}
-        :param sam_account_name: The pre-win2k name of the group. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group#sam_account_name Group#sam_account_name}
-        :param category: The group's category. Can be one of ``distribution`` or ``security`` (case sensitive). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group#category Group#category}
-        :param description: Description of the Group. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group#description Group#description}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group#id Group#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param scope: The group's scope. Can be one of ``global``, ``domainlocal``, or ``universal`` (case sensitive). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group#scope Group#scope}
+        :param container: A DN of a container object holding the group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group#container Group#container}
+        :param name: The name of the group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group#name Group#name}
+        :param sam_account_name: The pre-win2k name of the group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group#sam_account_name Group#sam_account_name}
+        :param category: The group's category. Can be one of ``distribution`` or ``security`` (case sensitive). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group#category Group#category}
+        :param description: Description of the Group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group#description Group#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group#id Group#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param scope: The group's scope. Can be one of ``global``, ``domainlocal``, or ``universal`` (case sensitive). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group#scope Group#scope}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -266,15 +266,15 @@
     },
 )
 class GroupConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         container: builtins.str,
         name: builtins.str,
@@ -288,21 +288,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param container: A DN of a container object holding the group. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group#container Group#container}
-        :param name: The name of the group. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group#name Group#name}
-        :param sam_account_name: The pre-win2k name of the group. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group#sam_account_name Group#sam_account_name}
-        :param category: The group's category. Can be one of ``distribution`` or ``security`` (case sensitive). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group#category Group#category}
-        :param description: Description of the Group. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group#description Group#description}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group#id Group#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param scope: The group's scope. Can be one of ``global``, ``domainlocal``, or ``universal`` (case sensitive). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group#scope Group#scope}
+        :param container: A DN of a container object holding the group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group#container Group#container}
+        :param name: The name of the group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group#name Group#name}
+        :param sam_account_name: The pre-win2k name of the group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group#sam_account_name Group#sam_account_name}
+        :param category: The group's category. Can be one of ``distribution`` or ``security`` (case sensitive). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group#category Group#category}
+        :param description: Description of the Group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group#description Group#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group#id Group#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param scope: The group's scope. Can be one of ``global``, ``domainlocal``, or ``universal`` (case sensitive). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group#scope Group#scope}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6b1f7e2fdc2620c7b24ad6c8dfe97b3b893cb7081f0c10a804b7acf7e468b709)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -353,20 +353,22 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("connection")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]], result)
 
     @builtins.property
-    def count(self) -> typing.Optional[jsii.Number]:
+    def count(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]]:
         '''
         :stability: experimental
         '''
         result = self._values.get("count")
-        return typing.cast(typing.Optional[jsii.Number], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]], result)
 
     @builtins.property
     def depends_on(
         self,
     ) -> typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]]:
         '''
         :stability: experimental
@@ -408,73 +410,73 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def container(self) -> builtins.str:
         '''A DN of a container object holding the group.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group#container Group#container}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group#container Group#container}
         '''
         result = self._values.get("container")
         assert result is not None, "Required property 'container' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the group.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group#name Group#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group#name Group#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def sam_account_name(self) -> builtins.str:
         '''The pre-win2k name of the group.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group#sam_account_name Group#sam_account_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group#sam_account_name Group#sam_account_name}
         '''
         result = self._values.get("sam_account_name")
         assert result is not None, "Required property 'sam_account_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def category(self) -> typing.Optional[builtins.str]:
         '''The group's category. Can be one of ``distribution`` or ``security`` (case sensitive).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group#category Group#category}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group#category Group#category}
         '''
         result = self._values.get("category")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''Description of the Group.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group#description Group#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group#description Group#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group#id Group#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group#id Group#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def scope(self) -> typing.Optional[builtins.str]:
         '''The group's scope. Can be one of ``global``, ``domainlocal``, or ``universal`` (case sensitive).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group#scope Group#scope}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group#scope Group#scope}
         '''
         result = self._values.get("scope")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -502,15 +504,15 @@
     name: builtins.str,
     sam_account_name: builtins.str,
     category: typing.Optional[builtins.str] = None,
     description: typing.Optional[builtins.str] = None,
     id: typing.Optional[builtins.str] = None,
     scope: typing.Optional[builtins.str] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
@@ -557,15 +559,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__6b1f7e2fdc2620c7b24ad6c8dfe97b3b893cb7081f0c10a804b7acf7e468b709(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     container: builtins.str,
     name: builtins.str,
```

### Comparing `cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/group_membership/__init__.py` & `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/group_membership/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `ad_group_membership`
 
-Refer to the Terraform Registory for docs: [`ad_group_membership`](https://www.terraform.io/docs/providers/ad/r/group_membership).
+Refer to the Terraform Registory for docs: [`ad_group_membership`](https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group_membership).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,39 +22,39 @@
 
 
 class GroupMembership(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-ad.groupMembership.GroupMembership",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/ad/r/group_membership ad_group_membership}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group_membership ad_group_membership}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         group_id: builtins.str,
         group_members: typing.Sequence[builtins.str],
         id: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/ad/r/group_membership ad_group_membership} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group_membership ad_group_membership} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param group_id: The ID of the group. This can be a GUID, a SID, a Distinguished Name, or the SAM Account Name of the group. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group_membership#group_id GroupMembership#group_id}
-        :param group_members: A list of member AD Principals. Each principal can be identified by its GUID, SID, Distinguished Name, or SAM Account Name. Only one is required Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group_membership#group_members GroupMembership#group_members}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group_membership#id GroupMembership#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param group_id: The ID of the group. This can be a GUID, a SID, a Distinguished Name, or the SAM Account Name of the group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group_membership#group_id GroupMembership#group_id}
+        :param group_members: A list of member AD Principals. Each principal can be identified by its GUID, SID, Distinguished Name, or SAM Account Name. Only one is required Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group_membership#group_members GroupMembership#group_members}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group_membership#id GroupMembership#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -160,15 +160,15 @@
     },
 )
 class GroupMembershipConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         group_id: builtins.str,
         group_members: typing.Sequence[builtins.str],
@@ -178,17 +178,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param group_id: The ID of the group. This can be a GUID, a SID, a Distinguished Name, or the SAM Account Name of the group. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group_membership#group_id GroupMembership#group_id}
-        :param group_members: A list of member AD Principals. Each principal can be identified by its GUID, SID, Distinguished Name, or SAM Account Name. Only one is required Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group_membership#group_members GroupMembership#group_members}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group_membership#id GroupMembership#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param group_id: The ID of the group. This can be a GUID, a SID, a Distinguished Name, or the SAM Account Name of the group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group_membership#group_id GroupMembership#group_id}
+        :param group_members: A list of member AD Principals. Each principal can be identified by its GUID, SID, Distinguished Name, or SAM Account Name. Only one is required Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group_membership#group_members GroupMembership#group_members}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group_membership#id GroupMembership#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9e8f6eb422185bc245841712c30bf59088d7c5c7c4a11dd57a29dce214e33504)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -228,20 +228,22 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("connection")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]], result)
 
     @builtins.property
-    def count(self) -> typing.Optional[jsii.Number]:
+    def count(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]]:
         '''
         :stability: experimental
         '''
         result = self._values.get("count")
-        return typing.cast(typing.Optional[jsii.Number], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]], result)
 
     @builtins.property
     def depends_on(
         self,
     ) -> typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]]:
         '''
         :stability: experimental
@@ -285,35 +287,35 @@
 
     @builtins.property
     def group_id(self) -> builtins.str:
         '''The ID of the group.
 
         This can be a GUID, a SID, a Distinguished Name, or the SAM Account Name of the group.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group_membership#group_id GroupMembership#group_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group_membership#group_id GroupMembership#group_id}
         '''
         result = self._values.get("group_id")
         assert result is not None, "Required property 'group_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def group_members(self) -> typing.List[builtins.str]:
         '''A list of member AD Principals.
 
         Each principal can be identified by its GUID, SID, Distinguished Name, or SAM Account Name. Only one is required
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group_membership#group_members GroupMembership#group_members}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group_membership#group_members GroupMembership#group_members}
         '''
         result = self._values.get("group_members")
         assert result is not None, "Required property 'group_members' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/group_membership#id GroupMembership#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/group_membership#id GroupMembership#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -340,15 +342,15 @@
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     group_id: builtins.str,
     group_members: typing.Sequence[builtins.str],
     id: typing.Optional[builtins.str] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
@@ -371,15 +373,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__9e8f6eb422185bc245841712c30bf59088d7c5c7c4a11dd57a29dce214e33504(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     group_id: builtins.str,
     group_members: typing.Sequence[builtins.str],
```

### Comparing `cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/ou/__init__.py` & `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/ou/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `ad_ou`
 
-Refer to the Terraform Registory for docs: [`ad_ou`](https://www.terraform.io/docs/providers/ad/r/ou).
+Refer to the Terraform Registory for docs: [`ad_ou`](https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/ou).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,43 +22,43 @@
 
 
 class Ou(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-ad.ou.Ou",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/ad/r/ou ad_ou}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/ou ad_ou}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
         description: typing.Optional[builtins.str] = None,
         id: typing.Optional[builtins.str] = None,
         path: typing.Optional[builtins.str] = None,
         protected: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/ad/r/ou ad_ou} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/ou ad_ou} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Name of the OU. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/ou#name Ou#name}
-        :param description: Description of the OU. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/ou#description Ou#description}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/ou#id Ou#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param path: DN of the object that contains the OU. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/ou#path Ou#path}
-        :param protected: Protect this OU from being deleted accidentaly. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/ou#protected Ou#protected}
+        :param name: Name of the OU. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/ou#name Ou#name}
+        :param description: Description of the OU. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/ou#description Ou#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/ou#id Ou#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param path: DN of the object that contains the OU. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/ou#path Ou#path}
+        :param protected: Protect this OU from being deleted accidentaly. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/ou#protected Ou#protected}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -229,15 +229,15 @@
     },
 )
 class OuConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         name: builtins.str,
         description: typing.Optional[builtins.str] = None,
@@ -249,19 +249,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Name of the OU. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/ou#name Ou#name}
-        :param description: Description of the OU. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/ou#description Ou#description}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/ou#id Ou#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param path: DN of the object that contains the OU. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/ou#path Ou#path}
-        :param protected: Protect this OU from being deleted accidentaly. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/ou#protected Ou#protected}
+        :param name: Name of the OU. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/ou#name Ou#name}
+        :param description: Description of the OU. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/ou#description Ou#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/ou#id Ou#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param path: DN of the object that contains the OU. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/ou#path Ou#path}
+        :param protected: Protect this OU from being deleted accidentaly. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/ou#protected Ou#protected}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__db6d8b81b78ea4bb4172ffcb0ffb36fc7eb730b6ef2036a76631db90c7be4baf)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -308,20 +308,22 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("connection")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]], result)
 
     @builtins.property
-    def count(self) -> typing.Optional[jsii.Number]:
+    def count(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]]:
         '''
         :stability: experimental
         '''
         result = self._values.get("count")
-        return typing.cast(typing.Optional[jsii.Number], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]], result)
 
     @builtins.property
     def depends_on(
         self,
     ) -> typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]]:
         '''
         :stability: experimental
@@ -363,55 +365,55 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''Name of the OU.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/ou#name Ou#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/ou#name Ou#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''Description of the OU.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/ou#description Ou#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/ou#description Ou#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/ou#id Ou#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/ou#id Ou#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def path(self) -> typing.Optional[builtins.str]:
         '''DN of the object that contains the OU.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/ou#path Ou#path}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/ou#path Ou#path}
         '''
         result = self._values.get("path")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def protected(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Protect this OU from being deleted accidentaly.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/ou#protected Ou#protected}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/ou#protected Ou#protected}
         '''
         result = self._values.get("protected")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -437,15 +439,15 @@
     *,
     name: builtins.str,
     description: typing.Optional[builtins.str] = None,
     id: typing.Optional[builtins.str] = None,
     path: typing.Optional[builtins.str] = None,
     protected: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
@@ -480,15 +482,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__db6d8b81b78ea4bb4172ffcb0ffb36fc7eb730b6ef2036a76631db90c7be4baf(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     name: builtins.str,
     description: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/provider/__init__.py` & `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/provider/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`ad`](https://www.terraform.io/docs/providers/ad).
+Refer to the Terraform Registory for docs: [`ad`](https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class AdProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-ad.provider.AdProvider",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/ad ad}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs ad}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         winrm_hostname: builtins.str,
@@ -44,32 +44,32 @@
         krb_spn: typing.Optional[builtins.str] = None,
         winrm_insecure: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         winrm_pass_credentials: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         winrm_port: typing.Optional[jsii.Number] = None,
         winrm_proto: typing.Optional[builtins.str] = None,
         winrm_use_ntlm: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/ad ad} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs ad} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param winrm_hostname: The hostname of the server we will use to run powershell scripts over WinRM. (Environment variable: AD_HOSTNAME). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_hostname AdProvider#winrm_hostname}
-        :param winrm_password: The password used to authenticate to the server's WinRM service. (Environment variable: AD_PASSWORD). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_password AdProvider#winrm_password}
-        :param winrm_username: The username used to authenticate to the server's WinRM service. (Environment variable: AD_USER). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_username AdProvider#winrm_username}
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#alias AdProvider#alias}
-        :param domain_controller: Use a specific domain controller. (default: none, environment variable: AD_DC). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#domain_controller AdProvider#domain_controller}
-        :param krb_conf: Path to kerberos configuration file. (default: none, environment variable: AD_KRB_CONF). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#krb_conf AdProvider#krb_conf}
-        :param krb_keytab: Path to a keytab file to be used instead of a password. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#krb_keytab AdProvider#krb_keytab}
-        :param krb_realm: The name of the kerberos realm (domain) we will use for authentication. (default: "", environment variable: AD_KRB_REALM). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#krb_realm AdProvider#krb_realm}
-        :param krb_spn: Alternative Service Principal Name. (default: none, environment variable: AD_KRB_SPN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#krb_spn AdProvider#krb_spn}
-        :param winrm_insecure: Trust unknown certificates. (default: false, environment variable: AD_WINRM_INSECURE). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_insecure AdProvider#winrm_insecure}
-        :param winrm_pass_credentials: Pass credentials in WinRM session to create a System.Management.Automation.PSCredential. (default: false, environment variable: AD_WINRM_PASS_CREDENTIALS). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_pass_credentials AdProvider#winrm_pass_credentials}
-        :param winrm_port: The port WinRM is listening for connections. (default: 5985, environment variable: AD_PORT). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_port AdProvider#winrm_port}
-        :param winrm_proto: The WinRM protocol we will use. (default: http, environment variable: AD_PROTO). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_proto AdProvider#winrm_proto}
-        :param winrm_use_ntlm: Use NTLM authentication. (default: false, environment variable: AD_WINRM_USE_NTLM). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_use_ntlm AdProvider#winrm_use_ntlm}
+        :param winrm_hostname: The hostname of the server we will use to run powershell scripts over WinRM. (Environment variable: AD_HOSTNAME). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_hostname AdProvider#winrm_hostname}
+        :param winrm_password: The password used to authenticate to the server's WinRM service. (Environment variable: AD_PASSWORD). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_password AdProvider#winrm_password}
+        :param winrm_username: The username used to authenticate to the server's WinRM service. (Environment variable: AD_USER). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_username AdProvider#winrm_username}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#alias AdProvider#alias}
+        :param domain_controller: Use a specific domain controller. (default: none, environment variable: AD_DC). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#domain_controller AdProvider#domain_controller}
+        :param krb_conf: Path to kerberos configuration file. (default: none, environment variable: AD_KRB_CONF). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#krb_conf AdProvider#krb_conf}
+        :param krb_keytab: Path to a keytab file to be used instead of a password. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#krb_keytab AdProvider#krb_keytab}
+        :param krb_realm: The name of the kerberos realm (domain) we will use for authentication. (default: "", environment variable: AD_KRB_REALM). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#krb_realm AdProvider#krb_realm}
+        :param krb_spn: Alternative Service Principal Name. (default: none, environment variable: AD_KRB_SPN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#krb_spn AdProvider#krb_spn}
+        :param winrm_insecure: Trust unknown certificates. (default: false, environment variable: AD_WINRM_INSECURE). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_insecure AdProvider#winrm_insecure}
+        :param winrm_pass_credentials: Pass credentials in WinRM session to create a System.Management.Automation.PSCredential. (default: false, environment variable: AD_WINRM_PASS_CREDENTIALS). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_pass_credentials AdProvider#winrm_pass_credentials}
+        :param winrm_port: The port WinRM is listening for connections. (default: 5985, environment variable: AD_PORT). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_port AdProvider#winrm_port}
+        :param winrm_proto: The WinRM protocol we will use. (default: http, environment variable: AD_PROTO). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_proto AdProvider#winrm_proto}
+        :param winrm_use_ntlm: Use NTLM authentication. (default: false, environment variable: AD_WINRM_USE_NTLM). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_use_ntlm AdProvider#winrm_use_ntlm}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2810f24a129ff6cfcf42c046e694e9cf8fee8632d3175c9b6c0513b7b669f059)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = AdProviderConfig(
             winrm_hostname=winrm_hostname,
@@ -439,28 +439,28 @@
         winrm_insecure: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         winrm_pass_credentials: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         winrm_port: typing.Optional[jsii.Number] = None,
         winrm_proto: typing.Optional[builtins.str] = None,
         winrm_use_ntlm: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     ) -> None:
         '''
-        :param winrm_hostname: The hostname of the server we will use to run powershell scripts over WinRM. (Environment variable: AD_HOSTNAME). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_hostname AdProvider#winrm_hostname}
-        :param winrm_password: The password used to authenticate to the server's WinRM service. (Environment variable: AD_PASSWORD). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_password AdProvider#winrm_password}
-        :param winrm_username: The username used to authenticate to the server's WinRM service. (Environment variable: AD_USER). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_username AdProvider#winrm_username}
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#alias AdProvider#alias}
-        :param domain_controller: Use a specific domain controller. (default: none, environment variable: AD_DC). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#domain_controller AdProvider#domain_controller}
-        :param krb_conf: Path to kerberos configuration file. (default: none, environment variable: AD_KRB_CONF). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#krb_conf AdProvider#krb_conf}
-        :param krb_keytab: Path to a keytab file to be used instead of a password. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#krb_keytab AdProvider#krb_keytab}
-        :param krb_realm: The name of the kerberos realm (domain) we will use for authentication. (default: "", environment variable: AD_KRB_REALM). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#krb_realm AdProvider#krb_realm}
-        :param krb_spn: Alternative Service Principal Name. (default: none, environment variable: AD_KRB_SPN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#krb_spn AdProvider#krb_spn}
-        :param winrm_insecure: Trust unknown certificates. (default: false, environment variable: AD_WINRM_INSECURE). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_insecure AdProvider#winrm_insecure}
-        :param winrm_pass_credentials: Pass credentials in WinRM session to create a System.Management.Automation.PSCredential. (default: false, environment variable: AD_WINRM_PASS_CREDENTIALS). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_pass_credentials AdProvider#winrm_pass_credentials}
-        :param winrm_port: The port WinRM is listening for connections. (default: 5985, environment variable: AD_PORT). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_port AdProvider#winrm_port}
-        :param winrm_proto: The WinRM protocol we will use. (default: http, environment variable: AD_PROTO). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_proto AdProvider#winrm_proto}
-        :param winrm_use_ntlm: Use NTLM authentication. (default: false, environment variable: AD_WINRM_USE_NTLM). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_use_ntlm AdProvider#winrm_use_ntlm}
+        :param winrm_hostname: The hostname of the server we will use to run powershell scripts over WinRM. (Environment variable: AD_HOSTNAME). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_hostname AdProvider#winrm_hostname}
+        :param winrm_password: The password used to authenticate to the server's WinRM service. (Environment variable: AD_PASSWORD). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_password AdProvider#winrm_password}
+        :param winrm_username: The username used to authenticate to the server's WinRM service. (Environment variable: AD_USER). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_username AdProvider#winrm_username}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#alias AdProvider#alias}
+        :param domain_controller: Use a specific domain controller. (default: none, environment variable: AD_DC). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#domain_controller AdProvider#domain_controller}
+        :param krb_conf: Path to kerberos configuration file. (default: none, environment variable: AD_KRB_CONF). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#krb_conf AdProvider#krb_conf}
+        :param krb_keytab: Path to a keytab file to be used instead of a password. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#krb_keytab AdProvider#krb_keytab}
+        :param krb_realm: The name of the kerberos realm (domain) we will use for authentication. (default: "", environment variable: AD_KRB_REALM). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#krb_realm AdProvider#krb_realm}
+        :param krb_spn: Alternative Service Principal Name. (default: none, environment variable: AD_KRB_SPN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#krb_spn AdProvider#krb_spn}
+        :param winrm_insecure: Trust unknown certificates. (default: false, environment variable: AD_WINRM_INSECURE). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_insecure AdProvider#winrm_insecure}
+        :param winrm_pass_credentials: Pass credentials in WinRM session to create a System.Management.Automation.PSCredential. (default: false, environment variable: AD_WINRM_PASS_CREDENTIALS). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_pass_credentials AdProvider#winrm_pass_credentials}
+        :param winrm_port: The port WinRM is listening for connections. (default: 5985, environment variable: AD_PORT). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_port AdProvider#winrm_port}
+        :param winrm_proto: The WinRM protocol we will use. (default: http, environment variable: AD_PROTO). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_proto AdProvider#winrm_proto}
+        :param winrm_use_ntlm: Use NTLM authentication. (default: false, environment variable: AD_WINRM_USE_NTLM). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_use_ntlm AdProvider#winrm_use_ntlm}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ce43b7d56d27583b9b5b49565f771b310f201757fdee0f2987c1c866af84e910)
             check_type(argname="argument winrm_hostname", value=winrm_hostname, expected_type=type_hints["winrm_hostname"])
             check_type(argname="argument winrm_password", value=winrm_password, expected_type=type_hints["winrm_password"])
             check_type(argname="argument winrm_username", value=winrm_username, expected_type=type_hints["winrm_username"])
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
@@ -502,141 +502,141 @@
         if winrm_use_ntlm is not None:
             self._values["winrm_use_ntlm"] = winrm_use_ntlm
 
     @builtins.property
     def winrm_hostname(self) -> builtins.str:
         '''The hostname of the server we will use to run powershell scripts over WinRM. (Environment variable: AD_HOSTNAME).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_hostname AdProvider#winrm_hostname}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_hostname AdProvider#winrm_hostname}
         '''
         result = self._values.get("winrm_hostname")
         assert result is not None, "Required property 'winrm_hostname' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def winrm_password(self) -> builtins.str:
         '''The password used to authenticate to the server's WinRM service. (Environment variable: AD_PASSWORD).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_password AdProvider#winrm_password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_password AdProvider#winrm_password}
         '''
         result = self._values.get("winrm_password")
         assert result is not None, "Required property 'winrm_password' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def winrm_username(self) -> builtins.str:
         '''The username used to authenticate to the server's WinRM service. (Environment variable: AD_USER).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_username AdProvider#winrm_username}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_username AdProvider#winrm_username}
         '''
         result = self._values.get("winrm_username")
         assert result is not None, "Required property 'winrm_username' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#alias AdProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#alias AdProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def domain_controller(self) -> typing.Optional[builtins.str]:
         '''Use a specific domain controller. (default: none, environment variable: AD_DC).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#domain_controller AdProvider#domain_controller}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#domain_controller AdProvider#domain_controller}
         '''
         result = self._values.get("domain_controller")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def krb_conf(self) -> typing.Optional[builtins.str]:
         '''Path to kerberos configuration file. (default: none, environment variable: AD_KRB_CONF).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#krb_conf AdProvider#krb_conf}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#krb_conf AdProvider#krb_conf}
         '''
         result = self._values.get("krb_conf")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def krb_keytab(self) -> typing.Optional[builtins.str]:
         '''Path to a keytab file to be used instead of a password.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#krb_keytab AdProvider#krb_keytab}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#krb_keytab AdProvider#krb_keytab}
         '''
         result = self._values.get("krb_keytab")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def krb_realm(self) -> typing.Optional[builtins.str]:
         '''The name of the kerberos realm (domain) we will use for authentication. (default: "", environment variable: AD_KRB_REALM).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#krb_realm AdProvider#krb_realm}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#krb_realm AdProvider#krb_realm}
         '''
         result = self._values.get("krb_realm")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def krb_spn(self) -> typing.Optional[builtins.str]:
         '''Alternative Service Principal Name. (default: none, environment variable: AD_KRB_SPN).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#krb_spn AdProvider#krb_spn}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#krb_spn AdProvider#krb_spn}
         '''
         result = self._values.get("krb_spn")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def winrm_insecure(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Trust unknown certificates. (default: false, environment variable: AD_WINRM_INSECURE).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_insecure AdProvider#winrm_insecure}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_insecure AdProvider#winrm_insecure}
         '''
         result = self._values.get("winrm_insecure")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def winrm_pass_credentials(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Pass credentials in WinRM session to create a System.Management.Automation.PSCredential. (default: false, environment variable: AD_WINRM_PASS_CREDENTIALS).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_pass_credentials AdProvider#winrm_pass_credentials}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_pass_credentials AdProvider#winrm_pass_credentials}
         '''
         result = self._values.get("winrm_pass_credentials")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def winrm_port(self) -> typing.Optional[jsii.Number]:
         '''The port WinRM is listening for connections. (default: 5985, environment variable: AD_PORT).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_port AdProvider#winrm_port}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_port AdProvider#winrm_port}
         '''
         result = self._values.get("winrm_port")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def winrm_proto(self) -> typing.Optional[builtins.str]:
         '''The WinRM protocol we will use. (default: http, environment variable: AD_PROTO).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_proto AdProvider#winrm_proto}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_proto AdProvider#winrm_proto}
         '''
         result = self._values.get("winrm_proto")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def winrm_use_ntlm(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Use NTLM authentication. (default: false, environment variable: AD_WINRM_USE_NTLM).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad#winrm_use_ntlm AdProvider#winrm_use_ntlm}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs#winrm_use_ntlm AdProvider#winrm_use_ntlm}
         '''
         result = self._values.get("winrm_use_ntlm")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad/user/__init__.py` & `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/user/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `ad_user`
 
-Refer to the Terraform Registory for docs: [`ad_user`](https://www.terraform.io/docs/providers/ad/r/user).
+Refer to the Terraform Registory for docs: [`ad_user`](https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class User(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-ad.user.User",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/ad/r/user ad_user}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user ad_user}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         display_name: builtins.str,
@@ -69,64 +69,64 @@
         smart_card_logon_required: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         state: typing.Optional[builtins.str] = None,
         street_address: typing.Optional[builtins.str] = None,
         surname: typing.Optional[builtins.str] = None,
         title: typing.Optional[builtins.str] = None,
         trusted_for_delegation: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/ad/r/user ad_user} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user ad_user} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param display_name: The Display Name of an Active Directory user. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#display_name User#display_name}
-        :param principal_name: The Principal Name of an Active Directory user. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#principal_name User#principal_name}
-        :param sam_account_name: The pre-win2k user logon name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#sam_account_name User#sam_account_name}
-        :param cannot_change_password: If set to true, the user will not be allowed to change their password. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#cannot_change_password User#cannot_change_password}
-        :param city: Specifies the user's town or city. This parameter sets the City property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#city User#city}
-        :param company: Specifies the user's company. This parameter sets the Company property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#company User#company}
-        :param container: A DN of the container object that will be holding the user. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#container User#container}
-        :param country: Specifies the country by setting the country code (refer to ISO 3166). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#country User#country}
-        :param custom_attributes: JSON encoded map that represents key/value pairs for custom attributes. Please note that ``terraform import`` will not import these attributes. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#custom_attributes User#custom_attributes}
-        :param department: Specifies the user's department. This parameter sets the Department property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#department User#department}
-        :param description: Specifies a description of the object. This parameter sets the value of the Description property for the user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#description User#description}
-        :param division: Specifies the user's division. This parameter sets the Division property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#division User#division}
-        :param email_address: Specifies the user's e-mail address. This parameter sets the EmailAddress property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#email_address User#email_address}
-        :param employee_id: Specifies the user's employee ID. This parameter sets the EmployeeID property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#employee_id User#employee_id}
-        :param employee_number: Specifies the user's employee number. This parameter sets the EmployeeNumber property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#employee_number User#employee_number}
-        :param enabled: If set to false, the user will be disabled. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#enabled User#enabled}
-        :param fax: Specifies the user's fax phone number. This parameter sets the Fax property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#fax User#fax}
-        :param given_name: Specifies the user's given name. This parameter sets the GivenName property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#given_name User#given_name}
-        :param home_directory: Specifies a user's home directory. This parameter sets the HomeDirectory property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#home_directory User#home_directory}
-        :param home_drive: Specifies a drive that is associated with the UNC path defined by the HomeDirectory property. The drive letter is specified as : where indicates the letter of the drive to associate. The must be a single, uppercase letter and the colon is required. This parameter sets the HomeDrive property of the user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#home_drive User#home_drive}
-        :param home_page: Specifies the URL of the home page of the object. This parameter sets the homePage property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#home_page User#home_page}
-        :param home_phone: Specifies the user's home telephone number. This parameter sets the HomePhone property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#home_phone User#home_phone}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#id User#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param initial_password: The user's initial password. This will be set on creation but will *not* be enforced in subsequent plans. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#initial_password User#initial_password}
-        :param initials: Specifies the initials that represent part of a user's name. Maximum 6 char. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#initials User#initials}
-        :param mobile_phone: Specifies the user's mobile phone number. This parameter sets the MobilePhone property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#mobile_phone User#mobile_phone}
-        :param office: Specifies the location of the user's office or place of business. This parameter sets the Office property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#office User#office}
-        :param office_phone: Specifies the user's office telephone number. This parameter sets the OfficePhone property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#office_phone User#office_phone}
-        :param organization: Specifies the user's organization. This parameter sets the Organization property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#organization User#organization}
-        :param other_name: Specifies a name in addition to a user's given name and surname, such as the user's middle name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#other_name User#other_name}
-        :param password_never_expires: If set to true, the password for this user will not expire. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#password_never_expires User#password_never_expires}
-        :param po_box: Specifies the user's post office box number. This parameter sets the POBox property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#po_box User#po_box}
-        :param postal_code: Specifies the user's postal code or zip code. This parameter sets the PostalCode property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#postal_code User#postal_code}
-        :param smart_card_logon_required: If set to true, a smart card is required to logon. This parameter sets the SmartCardLoginRequired property for a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#smart_card_logon_required User#smart_card_logon_required}
-        :param state: Specifies the user's or Organizational Unit's state or province. This parameter sets the State property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#state User#state}
-        :param street_address: Specifies the user's street address. This parameter sets the StreetAddress property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#street_address User#street_address}
-        :param surname: Specifies the user's last name or surname. This parameter sets the Surname property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#surname User#surname}
-        :param title: Specifies the user's title. This parameter sets the Title property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#title User#title}
-        :param trusted_for_delegation: If set to true, the user account is trusted for Kerberos delegation. A service that runs under an account that is trusted for Kerberos delegation can assume the identity of a client requesting the service. This parameter sets the TrustedForDelegation property of an account object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#trusted_for_delegation User#trusted_for_delegation}
+        :param display_name: The Display Name of an Active Directory user. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#display_name User#display_name}
+        :param principal_name: The Principal Name of an Active Directory user. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#principal_name User#principal_name}
+        :param sam_account_name: The pre-win2k user logon name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#sam_account_name User#sam_account_name}
+        :param cannot_change_password: If set to true, the user will not be allowed to change their password. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#cannot_change_password User#cannot_change_password}
+        :param city: Specifies the user's town or city. This parameter sets the City property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#city User#city}
+        :param company: Specifies the user's company. This parameter sets the Company property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#company User#company}
+        :param container: A DN of the container object that will be holding the user. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#container User#container}
+        :param country: Specifies the country by setting the country code (refer to ISO 3166). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#country User#country}
+        :param custom_attributes: JSON encoded map that represents key/value pairs for custom attributes. Please note that ``terraform import`` will not import these attributes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#custom_attributes User#custom_attributes}
+        :param department: Specifies the user's department. This parameter sets the Department property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#department User#department}
+        :param description: Specifies a description of the object. This parameter sets the value of the Description property for the user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#description User#description}
+        :param division: Specifies the user's division. This parameter sets the Division property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#division User#division}
+        :param email_address: Specifies the user's e-mail address. This parameter sets the EmailAddress property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#email_address User#email_address}
+        :param employee_id: Specifies the user's employee ID. This parameter sets the EmployeeID property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#employee_id User#employee_id}
+        :param employee_number: Specifies the user's employee number. This parameter sets the EmployeeNumber property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#employee_number User#employee_number}
+        :param enabled: If set to false, the user will be disabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#enabled User#enabled}
+        :param fax: Specifies the user's fax phone number. This parameter sets the Fax property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#fax User#fax}
+        :param given_name: Specifies the user's given name. This parameter sets the GivenName property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#given_name User#given_name}
+        :param home_directory: Specifies a user's home directory. This parameter sets the HomeDirectory property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#home_directory User#home_directory}
+        :param home_drive: Specifies a drive that is associated with the UNC path defined by the HomeDirectory property. The drive letter is specified as : where indicates the letter of the drive to associate. The must be a single, uppercase letter and the colon is required. This parameter sets the HomeDrive property of the user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#home_drive User#home_drive}
+        :param home_page: Specifies the URL of the home page of the object. This parameter sets the homePage property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#home_page User#home_page}
+        :param home_phone: Specifies the user's home telephone number. This parameter sets the HomePhone property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#home_phone User#home_phone}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#id User#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param initial_password: The user's initial password. This will be set on creation but will *not* be enforced in subsequent plans. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#initial_password User#initial_password}
+        :param initials: Specifies the initials that represent part of a user's name. Maximum 6 char. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#initials User#initials}
+        :param mobile_phone: Specifies the user's mobile phone number. This parameter sets the MobilePhone property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#mobile_phone User#mobile_phone}
+        :param office: Specifies the location of the user's office or place of business. This parameter sets the Office property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#office User#office}
+        :param office_phone: Specifies the user's office telephone number. This parameter sets the OfficePhone property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#office_phone User#office_phone}
+        :param organization: Specifies the user's organization. This parameter sets the Organization property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#organization User#organization}
+        :param other_name: Specifies a name in addition to a user's given name and surname, such as the user's middle name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#other_name User#other_name}
+        :param password_never_expires: If set to true, the password for this user will not expire. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#password_never_expires User#password_never_expires}
+        :param po_box: Specifies the user's post office box number. This parameter sets the POBox property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#po_box User#po_box}
+        :param postal_code: Specifies the user's postal code or zip code. This parameter sets the PostalCode property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#postal_code User#postal_code}
+        :param smart_card_logon_required: If set to true, a smart card is required to logon. This parameter sets the SmartCardLoginRequired property for a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#smart_card_logon_required User#smart_card_logon_required}
+        :param state: Specifies the user's or Organizational Unit's state or province. This parameter sets the State property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#state User#state}
+        :param street_address: Specifies the user's street address. This parameter sets the StreetAddress property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#street_address User#street_address}
+        :param surname: Specifies the user's last name or surname. This parameter sets the Surname property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#surname User#surname}
+        :param title: Specifies the user's title. This parameter sets the Title property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#title User#title}
+        :param trusted_for_delegation: If set to true, the user account is trusted for Kerberos delegation. A service that runs under an account that is trusted for Kerberos delegation can assume the identity of a client requesting the service. This parameter sets the TrustedForDelegation property of an account object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#trusted_for_delegation User#trusted_for_delegation}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -1099,15 +1099,15 @@
     },
 )
 class UserConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         display_name: builtins.str,
         principal_name: builtins.str,
@@ -1153,53 +1153,53 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param display_name: The Display Name of an Active Directory user. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#display_name User#display_name}
-        :param principal_name: The Principal Name of an Active Directory user. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#principal_name User#principal_name}
-        :param sam_account_name: The pre-win2k user logon name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#sam_account_name User#sam_account_name}
-        :param cannot_change_password: If set to true, the user will not be allowed to change their password. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#cannot_change_password User#cannot_change_password}
-        :param city: Specifies the user's town or city. This parameter sets the City property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#city User#city}
-        :param company: Specifies the user's company. This parameter sets the Company property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#company User#company}
-        :param container: A DN of the container object that will be holding the user. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#container User#container}
-        :param country: Specifies the country by setting the country code (refer to ISO 3166). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#country User#country}
-        :param custom_attributes: JSON encoded map that represents key/value pairs for custom attributes. Please note that ``terraform import`` will not import these attributes. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#custom_attributes User#custom_attributes}
-        :param department: Specifies the user's department. This parameter sets the Department property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#department User#department}
-        :param description: Specifies a description of the object. This parameter sets the value of the Description property for the user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#description User#description}
-        :param division: Specifies the user's division. This parameter sets the Division property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#division User#division}
-        :param email_address: Specifies the user's e-mail address. This parameter sets the EmailAddress property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#email_address User#email_address}
-        :param employee_id: Specifies the user's employee ID. This parameter sets the EmployeeID property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#employee_id User#employee_id}
-        :param employee_number: Specifies the user's employee number. This parameter sets the EmployeeNumber property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#employee_number User#employee_number}
-        :param enabled: If set to false, the user will be disabled. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#enabled User#enabled}
-        :param fax: Specifies the user's fax phone number. This parameter sets the Fax property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#fax User#fax}
-        :param given_name: Specifies the user's given name. This parameter sets the GivenName property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#given_name User#given_name}
-        :param home_directory: Specifies a user's home directory. This parameter sets the HomeDirectory property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#home_directory User#home_directory}
-        :param home_drive: Specifies a drive that is associated with the UNC path defined by the HomeDirectory property. The drive letter is specified as : where indicates the letter of the drive to associate. The must be a single, uppercase letter and the colon is required. This parameter sets the HomeDrive property of the user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#home_drive User#home_drive}
-        :param home_page: Specifies the URL of the home page of the object. This parameter sets the homePage property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#home_page User#home_page}
-        :param home_phone: Specifies the user's home telephone number. This parameter sets the HomePhone property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#home_phone User#home_phone}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#id User#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param initial_password: The user's initial password. This will be set on creation but will *not* be enforced in subsequent plans. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#initial_password User#initial_password}
-        :param initials: Specifies the initials that represent part of a user's name. Maximum 6 char. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#initials User#initials}
-        :param mobile_phone: Specifies the user's mobile phone number. This parameter sets the MobilePhone property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#mobile_phone User#mobile_phone}
-        :param office: Specifies the location of the user's office or place of business. This parameter sets the Office property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#office User#office}
-        :param office_phone: Specifies the user's office telephone number. This parameter sets the OfficePhone property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#office_phone User#office_phone}
-        :param organization: Specifies the user's organization. This parameter sets the Organization property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#organization User#organization}
-        :param other_name: Specifies a name in addition to a user's given name and surname, such as the user's middle name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#other_name User#other_name}
-        :param password_never_expires: If set to true, the password for this user will not expire. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#password_never_expires User#password_never_expires}
-        :param po_box: Specifies the user's post office box number. This parameter sets the POBox property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#po_box User#po_box}
-        :param postal_code: Specifies the user's postal code or zip code. This parameter sets the PostalCode property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#postal_code User#postal_code}
-        :param smart_card_logon_required: If set to true, a smart card is required to logon. This parameter sets the SmartCardLoginRequired property for a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#smart_card_logon_required User#smart_card_logon_required}
-        :param state: Specifies the user's or Organizational Unit's state or province. This parameter sets the State property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#state User#state}
-        :param street_address: Specifies the user's street address. This parameter sets the StreetAddress property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#street_address User#street_address}
-        :param surname: Specifies the user's last name or surname. This parameter sets the Surname property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#surname User#surname}
-        :param title: Specifies the user's title. This parameter sets the Title property of a user object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#title User#title}
-        :param trusted_for_delegation: If set to true, the user account is trusted for Kerberos delegation. A service that runs under an account that is trusted for Kerberos delegation can assume the identity of a client requesting the service. This parameter sets the TrustedForDelegation property of an account object. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#trusted_for_delegation User#trusted_for_delegation}
+        :param display_name: The Display Name of an Active Directory user. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#display_name User#display_name}
+        :param principal_name: The Principal Name of an Active Directory user. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#principal_name User#principal_name}
+        :param sam_account_name: The pre-win2k user logon name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#sam_account_name User#sam_account_name}
+        :param cannot_change_password: If set to true, the user will not be allowed to change their password. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#cannot_change_password User#cannot_change_password}
+        :param city: Specifies the user's town or city. This parameter sets the City property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#city User#city}
+        :param company: Specifies the user's company. This parameter sets the Company property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#company User#company}
+        :param container: A DN of the container object that will be holding the user. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#container User#container}
+        :param country: Specifies the country by setting the country code (refer to ISO 3166). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#country User#country}
+        :param custom_attributes: JSON encoded map that represents key/value pairs for custom attributes. Please note that ``terraform import`` will not import these attributes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#custom_attributes User#custom_attributes}
+        :param department: Specifies the user's department. This parameter sets the Department property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#department User#department}
+        :param description: Specifies a description of the object. This parameter sets the value of the Description property for the user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#description User#description}
+        :param division: Specifies the user's division. This parameter sets the Division property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#division User#division}
+        :param email_address: Specifies the user's e-mail address. This parameter sets the EmailAddress property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#email_address User#email_address}
+        :param employee_id: Specifies the user's employee ID. This parameter sets the EmployeeID property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#employee_id User#employee_id}
+        :param employee_number: Specifies the user's employee number. This parameter sets the EmployeeNumber property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#employee_number User#employee_number}
+        :param enabled: If set to false, the user will be disabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#enabled User#enabled}
+        :param fax: Specifies the user's fax phone number. This parameter sets the Fax property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#fax User#fax}
+        :param given_name: Specifies the user's given name. This parameter sets the GivenName property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#given_name User#given_name}
+        :param home_directory: Specifies a user's home directory. This parameter sets the HomeDirectory property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#home_directory User#home_directory}
+        :param home_drive: Specifies a drive that is associated with the UNC path defined by the HomeDirectory property. The drive letter is specified as : where indicates the letter of the drive to associate. The must be a single, uppercase letter and the colon is required. This parameter sets the HomeDrive property of the user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#home_drive User#home_drive}
+        :param home_page: Specifies the URL of the home page of the object. This parameter sets the homePage property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#home_page User#home_page}
+        :param home_phone: Specifies the user's home telephone number. This parameter sets the HomePhone property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#home_phone User#home_phone}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#id User#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param initial_password: The user's initial password. This will be set on creation but will *not* be enforced in subsequent plans. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#initial_password User#initial_password}
+        :param initials: Specifies the initials that represent part of a user's name. Maximum 6 char. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#initials User#initials}
+        :param mobile_phone: Specifies the user's mobile phone number. This parameter sets the MobilePhone property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#mobile_phone User#mobile_phone}
+        :param office: Specifies the location of the user's office or place of business. This parameter sets the Office property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#office User#office}
+        :param office_phone: Specifies the user's office telephone number. This parameter sets the OfficePhone property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#office_phone User#office_phone}
+        :param organization: Specifies the user's organization. This parameter sets the Organization property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#organization User#organization}
+        :param other_name: Specifies a name in addition to a user's given name and surname, such as the user's middle name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#other_name User#other_name}
+        :param password_never_expires: If set to true, the password for this user will not expire. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#password_never_expires User#password_never_expires}
+        :param po_box: Specifies the user's post office box number. This parameter sets the POBox property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#po_box User#po_box}
+        :param postal_code: Specifies the user's postal code or zip code. This parameter sets the PostalCode property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#postal_code User#postal_code}
+        :param smart_card_logon_required: If set to true, a smart card is required to logon. This parameter sets the SmartCardLoginRequired property for a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#smart_card_logon_required User#smart_card_logon_required}
+        :param state: Specifies the user's or Organizational Unit's state or province. This parameter sets the State property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#state User#state}
+        :param street_address: Specifies the user's street address. This parameter sets the StreetAddress property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#street_address User#street_address}
+        :param surname: Specifies the user's last name or surname. This parameter sets the Surname property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#surname User#surname}
+        :param title: Specifies the user's title. This parameter sets the Title property of a user object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#title User#title}
+        :param trusted_for_delegation: If set to true, the user account is trusted for Kerberos delegation. A service that runs under an account that is trusted for Kerberos delegation can assume the identity of a client requesting the service. This parameter sets the TrustedForDelegation property of an account object. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#trusted_for_delegation User#trusted_for_delegation}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cf50c00353f44d35109a932cd7f15e60f3ccf4d10d6b4806022ab9ec39ddc3da)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -1346,20 +1346,22 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("connection")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]], result)
 
     @builtins.property
-    def count(self) -> typing.Optional[jsii.Number]:
+    def count(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]]:
         '''
         :stability: experimental
         '''
         result = self._values.get("count")
-        return typing.cast(typing.Optional[jsii.Number], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]], result)
 
     @builtins.property
     def depends_on(
         self,
     ) -> typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]]:
         '''
         :stability: experimental
@@ -1401,383 +1403,383 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def display_name(self) -> builtins.str:
         '''The Display Name of an Active Directory user.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#display_name User#display_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#display_name User#display_name}
         '''
         result = self._values.get("display_name")
         assert result is not None, "Required property 'display_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def principal_name(self) -> builtins.str:
         '''The Principal Name of an Active Directory user.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#principal_name User#principal_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#principal_name User#principal_name}
         '''
         result = self._values.get("principal_name")
         assert result is not None, "Required property 'principal_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def sam_account_name(self) -> builtins.str:
         '''The pre-win2k user logon name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#sam_account_name User#sam_account_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#sam_account_name User#sam_account_name}
         '''
         result = self._values.get("sam_account_name")
         assert result is not None, "Required property 'sam_account_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def cannot_change_password(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If set to true, the user will not be allowed to change their password.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#cannot_change_password User#cannot_change_password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#cannot_change_password User#cannot_change_password}
         '''
         result = self._values.get("cannot_change_password")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def city(self) -> typing.Optional[builtins.str]:
         '''Specifies the user's town or city. This parameter sets the City property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#city User#city}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#city User#city}
         '''
         result = self._values.get("city")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def company(self) -> typing.Optional[builtins.str]:
         '''Specifies the user's company. This parameter sets the Company property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#company User#company}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#company User#company}
         '''
         result = self._values.get("company")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def container(self) -> typing.Optional[builtins.str]:
         '''A DN of the container object that will be holding the user.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#container User#container}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#container User#container}
         '''
         result = self._values.get("container")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def country(self) -> typing.Optional[builtins.str]:
         '''Specifies the country by setting the country code (refer to ISO 3166).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#country User#country}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#country User#country}
         '''
         result = self._values.get("country")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def custom_attributes(self) -> typing.Optional[builtins.str]:
         '''JSON encoded map that represents key/value pairs for custom attributes.
 
         Please note that ``terraform import`` will not import these attributes.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#custom_attributes User#custom_attributes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#custom_attributes User#custom_attributes}
         '''
         result = self._values.get("custom_attributes")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def department(self) -> typing.Optional[builtins.str]:
         '''Specifies the user's department. This parameter sets the Department property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#department User#department}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#department User#department}
         '''
         result = self._values.get("department")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''Specifies a description of the object. This parameter sets the value of the Description property for the user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#description User#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#description User#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def division(self) -> typing.Optional[builtins.str]:
         '''Specifies the user's division. This parameter sets the Division property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#division User#division}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#division User#division}
         '''
         result = self._values.get("division")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def email_address(self) -> typing.Optional[builtins.str]:
         '''Specifies the user's e-mail address. This parameter sets the EmailAddress property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#email_address User#email_address}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#email_address User#email_address}
         '''
         result = self._values.get("email_address")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def employee_id(self) -> typing.Optional[builtins.str]:
         '''Specifies the user's employee ID. This parameter sets the EmployeeID property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#employee_id User#employee_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#employee_id User#employee_id}
         '''
         result = self._values.get("employee_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def employee_number(self) -> typing.Optional[builtins.str]:
         '''Specifies the user's employee number. This parameter sets the EmployeeNumber property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#employee_number User#employee_number}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#employee_number User#employee_number}
         '''
         result = self._values.get("employee_number")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If set to false, the user will be disabled.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#enabled User#enabled}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#enabled User#enabled}
         '''
         result = self._values.get("enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def fax(self) -> typing.Optional[builtins.str]:
         '''Specifies the user's fax phone number. This parameter sets the Fax property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#fax User#fax}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#fax User#fax}
         '''
         result = self._values.get("fax")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def given_name(self) -> typing.Optional[builtins.str]:
         '''Specifies the user's given name. This parameter sets the GivenName property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#given_name User#given_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#given_name User#given_name}
         '''
         result = self._values.get("given_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def home_directory(self) -> typing.Optional[builtins.str]:
         '''Specifies a user's home directory. This parameter sets the HomeDirectory property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#home_directory User#home_directory}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#home_directory User#home_directory}
         '''
         result = self._values.get("home_directory")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def home_drive(self) -> typing.Optional[builtins.str]:
         '''Specifies a drive that is associated with the UNC path defined by the HomeDirectory property.
 
         The drive letter is specified as : where  indicates the letter of the drive to associate. The  must be a single, uppercase letter and the colon is required. This parameter sets the HomeDrive property of the user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#home_drive User#home_drive}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#home_drive User#home_drive}
         '''
         result = self._values.get("home_drive")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def home_page(self) -> typing.Optional[builtins.str]:
         '''Specifies the URL of the home page of the object.
 
         This parameter sets the homePage property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#home_page User#home_page}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#home_page User#home_page}
         '''
         result = self._values.get("home_page")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def home_phone(self) -> typing.Optional[builtins.str]:
         '''Specifies the user's home telephone number. This parameter sets the HomePhone property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#home_phone User#home_phone}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#home_phone User#home_phone}
         '''
         result = self._values.get("home_phone")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#id User#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#id User#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def initial_password(self) -> typing.Optional[builtins.str]:
         '''The user's initial password. This will be set on creation but will *not* be enforced in subsequent plans.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#initial_password User#initial_password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#initial_password User#initial_password}
         '''
         result = self._values.get("initial_password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def initials(self) -> typing.Optional[builtins.str]:
         '''Specifies the initials that represent part of a user's name. Maximum 6 char.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#initials User#initials}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#initials User#initials}
         '''
         result = self._values.get("initials")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def mobile_phone(self) -> typing.Optional[builtins.str]:
         '''Specifies the user's mobile phone number. This parameter sets the MobilePhone property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#mobile_phone User#mobile_phone}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#mobile_phone User#mobile_phone}
         '''
         result = self._values.get("mobile_phone")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def office(self) -> typing.Optional[builtins.str]:
         '''Specifies the location of the user's office or place of business.
 
         This parameter sets the Office property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#office User#office}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#office User#office}
         '''
         result = self._values.get("office")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def office_phone(self) -> typing.Optional[builtins.str]:
         '''Specifies the user's office telephone number. This parameter sets the OfficePhone property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#office_phone User#office_phone}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#office_phone User#office_phone}
         '''
         result = self._values.get("office_phone")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
         '''Specifies the user's organization. This parameter sets the Organization property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#organization User#organization}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#organization User#organization}
         '''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def other_name(self) -> typing.Optional[builtins.str]:
         '''Specifies a name in addition to a user's given name and surname, such as the user's middle name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#other_name User#other_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#other_name User#other_name}
         '''
         result = self._values.get("other_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def password_never_expires(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If set to true, the password for this user will not expire.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#password_never_expires User#password_never_expires}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#password_never_expires User#password_never_expires}
         '''
         result = self._values.get("password_never_expires")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def po_box(self) -> typing.Optional[builtins.str]:
         '''Specifies the user's post office box number. This parameter sets the POBox property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#po_box User#po_box}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#po_box User#po_box}
         '''
         result = self._values.get("po_box")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def postal_code(self) -> typing.Optional[builtins.str]:
         '''Specifies the user's postal code or zip code. This parameter sets the PostalCode property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#postal_code User#postal_code}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#postal_code User#postal_code}
         '''
         result = self._values.get("postal_code")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def smart_card_logon_required(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If set to true, a smart card is required to logon.
 
         This parameter sets the SmartCardLoginRequired property for a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#smart_card_logon_required User#smart_card_logon_required}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#smart_card_logon_required User#smart_card_logon_required}
         '''
         result = self._values.get("smart_card_logon_required")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def state(self) -> typing.Optional[builtins.str]:
         '''Specifies the user's or Organizational Unit's state or province. This parameter sets the State property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#state User#state}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#state User#state}
         '''
         result = self._values.get("state")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def street_address(self) -> typing.Optional[builtins.str]:
         '''Specifies the user's street address. This parameter sets the StreetAddress property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#street_address User#street_address}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#street_address User#street_address}
         '''
         result = self._values.get("street_address")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def surname(self) -> typing.Optional[builtins.str]:
         '''Specifies the user's last name or surname. This parameter sets the Surname property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#surname User#surname}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#surname User#surname}
         '''
         result = self._values.get("surname")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def title(self) -> typing.Optional[builtins.str]:
         '''Specifies the user's title. This parameter sets the Title property of a user object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#title User#title}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#title User#title}
         '''
         result = self._values.get("title")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def trusted_for_delegation(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If set to true, the user account is trusted for Kerberos delegation.
 
         A service that runs under an account that is trusted for Kerberos delegation can assume the identity of a client requesting the service. This parameter sets the TrustedForDelegation property of an account object.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/ad/r/user#trusted_for_delegation User#trusted_for_delegation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/ad/0.4.4/docs/resources/user#trusted_for_delegation User#trusted_for_delegation}
         '''
         result = self._values.get("trusted_for_delegation")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1837,15 +1839,15 @@
     smart_card_logon_required: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     state: typing.Optional[builtins.str] = None,
     street_address: typing.Optional[builtins.str] = None,
     surname: typing.Optional[builtins.str] = None,
     title: typing.Optional[builtins.str] = None,
     trusted_for_delegation: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
@@ -2084,15 +2086,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__cf50c00353f44d35109a932cd7f15e60f3ccf4d10d6b4806022ab9ec39ddc3da(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     display_name: builtins.str,
     principal_name: builtins.str,
```

### Comparing `cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad.egg-info/PKG-INFO` & `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-ad
-Version: 3.0.0
+Version: 4.0.0
 Summary: Prebuilt ad Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-ad.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-ad.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -62,15 +62,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-ad-go`](https://github.com/cdktf/cdktf-provider-ad-go) package.
 
 `go get github.com/cdktf/cdktf-provider-ad-go/ad`
 
 ## Docs
 
-Find auto-generated docs for this provider here: [./API.md](./API.md)
+Find auto-generated docs for this provider here:
+
+* [Typescript](./docs/API.typescript.md)
+* [Python](./docs/API.python.md)
+* [Java](./docs/API.java.md)
+* [C#](./docs/API.csharp.md)
+* [Go](./docs/API.go.md)
+
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-ad).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform ad Provider version 1:1. In fact, it always tracks `latest` of `~> 0.4` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-ad-3.0.0/src/cdktf_cdktf_provider_ad.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_ad/py.typed
 src/cdktf_cdktf_provider_ad.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_ad.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_ad.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_ad.egg-info/requires.txt
 src/cdktf_cdktf_provider_ad.egg-info/top_level.txt
 src/cdktf_cdktf_provider_ad/_jsii/__init__.py
-src/cdktf_cdktf_provider_ad/_jsii/provider-ad@3.0.0.jsii.tgz
+src/cdktf_cdktf_provider_ad/_jsii/provider-ad@4.0.0.jsii.tgz
 src/cdktf_cdktf_provider_ad/computer/__init__.py
 src/cdktf_cdktf_provider_ad/data_ad_computer/__init__.py
 src/cdktf_cdktf_provider_ad/data_ad_gpo/__init__.py
 src/cdktf_cdktf_provider_ad/data_ad_group/__init__.py
 src/cdktf_cdktf_provider_ad/data_ad_ou/__init__.py
 src/cdktf_cdktf_provider_ad/data_ad_user/__init__.py
 src/cdktf_cdktf_provider_ad/gplink/__init__.py
```

