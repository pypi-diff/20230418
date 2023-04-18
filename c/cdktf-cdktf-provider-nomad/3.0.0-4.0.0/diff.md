# Comparing `tmp/cdktf-cdktf-provider-nomad-3.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-nomad-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-nomad-3.0.0.tar", last modified: Tue Jan 17 14:56:48 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-nomad-4.0.0.tar", last modified: Tue Apr 18 20:48:56 2023, max compression
```

## Comparing `cdktf-cdktf-provider-nomad-3.0.0.tar` & `cdktf-cdktf-provider-nomad-4.0.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.277680 cdktf-cdktf-provider-nomad-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-01-17 14:56:48.277680 cdktf-cdktf-provider-nomad-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 14:56:48.277680 cdktf-cdktf-provider-nomad-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.269680 cdktf-cdktf-provider-nomad-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.273680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.273680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   291112 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/_jsii/provider-nomad@3.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.273680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/acl_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/acl_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.273680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/acl_role/
--rw-r--r--   0 runner    (1001) docker     (123)    33951 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/acl_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.273680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/acl_token/
--rw-r--r--   0 runner    (1001) docker     (123)    43526 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/acl_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.273680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policies/
--rw-r--r--   0 runner    (1001) docker     (123)    26729 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.273680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    17435 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.273680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_role/
--rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.273680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_roles/
--rw-r--r--   0 runner    (1001) docker     (123)    35766 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_roles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.273680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_token/
--rw-r--r--   0 runner    (1001) docker     (123)    27881 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.273680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_tokens/
--rw-r--r--   0 runner    (1001) docker     (123)    36759 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_tokens/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.273680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_datacenters/
--rw-r--r--   0 runner    (1001) docker     (123)    21128 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_datacenters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.273680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_deployments/
--rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_deployments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.273680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_job/
--rw-r--r--   0 runner    (1001) docker     (123)    78876 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_job/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.273680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_job_parser/
--rw-r--r--   0 runner    (1001) docker     (123)    20538 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_job_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.273680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_namespace/
--rw-r--r--   0 runner    (1001) docker     (123)    26981 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_namespace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.277680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_namespaces/
--rw-r--r--   0 runner    (1001) docker     (123)    15449 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_namespaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.277680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)    34460 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.277680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)    17548 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.277680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_regions/
--rw-r--r--   0 runner    (1001) docker     (123)    15371 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_regions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.277680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policies/
--rw-r--r--   0 runner    (1001) docker     (123)    29633 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.277680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.277680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_scheduler_config/
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_scheduler_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.277680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_volumes/
--rw-r--r--   0 runner    (1001) docker     (123)    24372 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_volumes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.277680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/external_volume/
--rw-r--r--   0 runner    (1001) docker     (123)   131540 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/external_volume/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.277680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/job/
--rw-r--r--   0 runner    (1001) docker     (123)   102081 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/job/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.277680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/namespace/
--rw-r--r--   0 runner    (1001) docker     (123)    35549 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/namespace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.277680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    43922 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.277680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/quota_specification/
--rw-r--r--   0 runner    (1001) docker     (123)    44596 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/quota_specification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.277680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/scheduler_config/
--rw-r--r--   0 runner    (1001) docker     (123)    25563 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/scheduler_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.277680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/sentinel_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    26039 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/sentinel_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.277680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/volume/
--rw-r--r--   0 runner    (1001) docker     (123)   110023 2023-01-17 14:56:36.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/volume/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:56:48.273680 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-01-17 14:56:47.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-01-17 14:56:48.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:56:47.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-17 14:56:48.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-17 14:56:48.000000 cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.527063 cdktf-cdktf-provider-nomad-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-18 20:48:56.527063 cdktf-cdktf-provider-nomad-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:48:56.527063 cdktf-cdktf-provider-nomad-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.515063 cdktf-cdktf-provider-nomad-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.519063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.519063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   981392 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/_jsii/provider-nomad@4.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/acl_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    22421 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/acl_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/acl_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    34752 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/acl_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/acl_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    44597 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/acl_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policies/
+-rw-r--r--   0 runner    (1001) docker     (123)    27317 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    24820 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)    36354 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_roles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    28469 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_tokens/
+-rw-r--r--   0 runner    (1001) docker     (123)    37347 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_tokens/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_datacenters/
+-rw-r--r--   0 runner    (1001) docker     (123)    21815 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_datacenters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_deployments/
+-rw-r--r--   0 runner    (1001) docker     (123)    15972 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_deployments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_job/
+-rw-r--r--   0 runner    (1001) docker     (123)    79563 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_job/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_job_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)    21225 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_job_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_namespace/
+-rw-r--r--   0 runner    (1001) docker     (123)    27569 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_namespace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_namespaces/
+-rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_namespaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)    35246 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_regions/
+-rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_regions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policies/
+-rw-r--r--   0 runner    (1001) docker     (123)    30320 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    16686 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_scheduler_config/
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_scheduler_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)    25257 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_volumes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.523063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/external_volume/
+-rw-r--r--   0 runner    (1001) docker     (123)   134051 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/external_volume/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.527063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/job/
+-rw-r--r--   0 runner    (1001) docker     (123)   103992 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/job/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.527063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/namespace/
+-rw-r--r--   0 runner    (1001) docker     (123)    36650 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/namespace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.527063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    45066 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.527063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/quota_specification/
+-rw-r--r--   0 runner    (1001) docker     (123)    45637 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/quota_specification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.527063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/scheduler_config/
+-rw-r--r--   0 runner    (1001) docker     (123)    26304 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/scheduler_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.527063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/sentinel_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    26960 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/sentinel_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.527063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/volume/
+-rw-r--r--   0 runner    (1001) docker     (123)   112384 2023-04-18 20:48:43.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/volume/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:56.519063 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-18 20:48:56.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-18 20:48:56.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:48:56.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:48:56.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 20:48:56.000000 cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/LICENSE` & `cdktf-cdktf-provider-nomad-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/PKG-INFO` & `cdktf-cdktf-provider-nomad-4.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-nomad
-Version: 3.0.0
+Version: 4.0.0
 Summary: Prebuilt nomad Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-nomad.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-nomad.git
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
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-nomad-go`](https://github.com/cdktf/cdktf-provider-nomad-go) package.
 
 `go get github.com/cdktf/cdktf-provider-nomad-go/nomad`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-nomad).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform nomad Provider version 1:1. In fact, it always tracks `latest` of `~> 1.4` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/README.md` & `cdktf-cdktf-provider-nomad-4.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-nomad-go`](https://github.com/cdktf/cdktf-provider-nomad-go) package.
 
 `go get github.com/cdktf/cdktf-provider-nomad-go/nomad`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-nomad).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform nomad Provider version 1:1. In fact, it always tracks `latest` of `~> 1.4` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/setup.py` & `cdktf-cdktf-provider-nomad-4.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-nomad",
-    "version": "3.0.0",
+    "version": "4.0.0",
     "description": "Prebuilt nomad Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-nomad.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -52,37 +52,38 @@
         "cdktf_cdktf_provider_nomad.quota_specification",
         "cdktf_cdktf_provider_nomad.scheduler_config",
         "cdktf_cdktf_provider_nomad.sentinel_policy",
         "cdktf_cdktf_provider_nomad.volume"
     ],
     "package_data": {
         "cdktf_cdktf_provider_nomad._jsii": [
-            "provider-nomad@3.0.0.jsii.tgz"
+            "provider-nomad@4.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_nomad": [
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

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-nomad-go`](https://github.com/cdktf/cdktf-provider-nomad-go) package.
 
 `go get github.com/cdktf/cdktf-provider-nomad-go/nomad`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-nomad).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform nomad Provider version 1:1. In fact, it always tracks `latest` of `~> 1.4` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/acl_policy/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/acl_policy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `nomad_acl_policy`
 
-Refer to the Terraform Registory for docs: [`nomad_acl_policy`](https://www.terraform.io/docs/providers/nomad/r/acl_policy).
+Refer to the Terraform Registory for docs: [`nomad_acl_policy`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_policy).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,41 +22,41 @@
 
 
 class AclPolicy(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.aclPolicy.AclPolicy",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/r/acl_policy nomad_acl_policy}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_policy nomad_acl_policy}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
         rules_hcl: builtins.str,
         description: typing.Optional[builtins.str] = None,
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
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/r/acl_policy nomad_acl_policy} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_policy nomad_acl_policy} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Unique name for this policy. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_policy#name AclPolicy#name}
-        :param rules_hcl: HCL or JSON representation of the rules to enforce on this policy. Use file() to specify a file as input. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_policy#rules_hcl AclPolicy#rules_hcl}
-        :param description: Description for this policy. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_policy#description AclPolicy#description}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_policy#id AclPolicy#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Unique name for this policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_policy#name AclPolicy#name}
+        :param rules_hcl: HCL or JSON representation of the rules to enforce on this policy. Use file() to specify a file as input. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_policy#rules_hcl AclPolicy#rules_hcl}
+        :param description: Description for this policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_policy#description AclPolicy#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_policy#id AclPolicy#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -185,15 +185,15 @@
     },
 )
 class AclPolicyConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         rules_hcl: builtins.str,
@@ -204,18 +204,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Unique name for this policy. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_policy#name AclPolicy#name}
-        :param rules_hcl: HCL or JSON representation of the rules to enforce on this policy. Use file() to specify a file as input. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_policy#rules_hcl AclPolicy#rules_hcl}
-        :param description: Description for this policy. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_policy#description AclPolicy#description}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_policy#id AclPolicy#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Unique name for this policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_policy#name AclPolicy#name}
+        :param rules_hcl: HCL or JSON representation of the rules to enforce on this policy. Use file() to specify a file as input. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_policy#rules_hcl AclPolicy#rules_hcl}
+        :param description: Description for this policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_policy#description AclPolicy#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_policy#id AclPolicy#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c9dd74b156bc04292051b30dce551bee4be12595022fa30fd6b4c7bdc7334298)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -258,20 +258,22 @@
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
@@ -313,44 +315,44 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''Unique name for this policy.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_policy#name AclPolicy#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_policy#name AclPolicy#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def rules_hcl(self) -> builtins.str:
         '''HCL or JSON representation of the rules to enforce on this policy.
 
         Use file() to specify a file as input.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_policy#rules_hcl AclPolicy#rules_hcl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_policy#rules_hcl AclPolicy#rules_hcl}
         '''
         result = self._values.get("rules_hcl")
         assert result is not None, "Required property 'rules_hcl' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''Description for this policy.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_policy#description AclPolicy#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_policy#description AclPolicy#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_policy#id AclPolicy#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_policy#id AclPolicy#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -378,15 +380,15 @@
     id_: builtins.str,
     *,
     name: builtins.str,
     rules_hcl: builtins.str,
     description: typing.Optional[builtins.str] = None,
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
@@ -415,15 +417,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__c9dd74b156bc04292051b30dce551bee4be12595022fa30fd6b4c7bdc7334298(
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
     rules_hcl: builtins.str,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/acl_role/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/acl_role/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `nomad_acl_role`
 
-Refer to the Terraform Registory for docs: [`nomad_acl_role`](https://www.terraform.io/docs/providers/nomad/r/acl_role).
+Refer to the Terraform Registory for docs: [`nomad_acl_role`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_role).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,41 +22,41 @@
 
 
 class AclRole(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.aclRole.AclRole",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/r/acl_role nomad_acl_role}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_role nomad_acl_role}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
         policy: typing.Union[typing.Sequence[typing.Union["AclRolePolicy", typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable],
         description: typing.Optional[builtins.str] = None,
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
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/r/acl_role nomad_acl_role} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_role nomad_acl_role} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Unique name for this ACL role. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_role#name AclRole#name}
-        :param policy: policy block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_role#policy AclRole#policy}
-        :param description: Description for this ACL role. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_role#description AclRole#description}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_role#id AclRole#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Unique name for this ACL role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_role#name AclRole#name}
+        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_role#policy AclRole#policy}
+        :param description: Description for this ACL role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_role#description AclRole#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_role#id AclRole#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -193,15 +193,15 @@
     },
 )
 class AclRoleConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         policy: typing.Union[typing.Sequence[typing.Union["AclRolePolicy", typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable],
@@ -212,18 +212,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Unique name for this ACL role. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_role#name AclRole#name}
-        :param policy: policy block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_role#policy AclRole#policy}
-        :param description: Description for this ACL role. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_role#description AclRole#description}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_role#id AclRole#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Unique name for this ACL role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_role#name AclRole#name}
+        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_role#policy AclRole#policy}
+        :param description: Description for this ACL role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_role#description AclRole#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_role#id AclRole#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__00a078397c19bf37a1ce639f57206f0924696d5c214414806605104c17fff840)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -266,20 +266,22 @@
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
@@ -321,44 +323,44 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''Unique name for this ACL role.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_role#name AclRole#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_role#name AclRole#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def policy(
         self,
     ) -> typing.Union[typing.List["AclRolePolicy"], _cdktf_9a9027ec.IResolvable]:
         '''policy block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_role#policy AclRole#policy}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_role#policy AclRole#policy}
         '''
         result = self._values.get("policy")
         assert result is not None, "Required property 'policy' is missing"
         return typing.cast(typing.Union[typing.List["AclRolePolicy"], _cdktf_9a9027ec.IResolvable], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''Description for this ACL role.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_role#description AclRole#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_role#description AclRole#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_role#id AclRole#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_role#id AclRole#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -378,28 +380,28 @@
     jsii_type="@cdktf/provider-nomad.aclRole.AclRolePolicy",
     jsii_struct_bases=[],
     name_mapping={"name": "name"},
 )
 class AclRolePolicy:
     def __init__(self, *, name: builtins.str) -> None:
         '''
-        :param name: The name of the ACL policy to link. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_role#name AclRole#name}
+        :param name: The name of the ACL policy to link. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_role#name AclRole#name}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a091de4c363c10633aceeaf1802821125a53573ba932314f6cbb7044e6d684b0)
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "name": name,
         }
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the ACL policy to link.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_role#name AclRole#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_role#name AclRole#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -579,15 +581,15 @@
     id_: builtins.str,
     *,
     name: builtins.str,
     policy: typing.Union[typing.Sequence[typing.Union[AclRolePolicy, typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable],
     description: typing.Optional[builtins.str] = None,
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
@@ -616,15 +618,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__00a078397c19bf37a1ce639f57206f0924696d5c214414806605104c17fff840(
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
     policy: typing.Union[typing.Sequence[typing.Union[AclRolePolicy, typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable],
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/acl_token/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/acl_token/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `nomad_acl_token`
 
-Refer to the Terraform Registory for docs: [`nomad_acl_token`](https://www.terraform.io/docs/providers/nomad/r/acl_token).
+Refer to the Terraform Registory for docs: [`nomad_acl_token`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,47 +22,47 @@
 
 
 class AclToken(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.aclToken.AclToken",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/r/acl_token nomad_acl_token}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token nomad_acl_token}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         type: builtins.str,
         expiration_ttl: typing.Optional[builtins.str] = None,
         global_: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         id: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
         policies: typing.Optional[typing.Sequence[builtins.str]] = None,
         role: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["AclTokenRole", typing.Dict[builtins.str, typing.Any]]]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/r/acl_token nomad_acl_token} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token nomad_acl_token} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param type: The type of token to create, 'client' or 'management'. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#type AclToken#type}
-        :param expiration_ttl: Provides a TTL for the token in the form of a time duration such as "5m" or "1h". Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#expiration_ttl AclToken#expiration_ttl}
-        :param global_: Whether the token should be replicated to all regions or not. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#global AclToken#global}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#id AclToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: Human-readable name for this token. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#name AclToken#name}
-        :param policies: The ACL policies to associate with the token, if it's a 'client' type. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#policies AclToken#policies}
-        :param role: role block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#role AclToken#role}
+        :param type: The type of token to create, 'client' or 'management'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#type AclToken#type}
+        :param expiration_ttl: Provides a TTL for the token in the form of a time duration such as "5m" or "1h". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#expiration_ttl AclToken#expiration_ttl}
+        :param global_: Whether the token should be replicated to all regions or not. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#global AclToken#global}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#id AclToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Human-readable name for this token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#name AclToken#name}
+        :param policies: The ACL policies to associate with the token, if it's a 'client' type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#policies AclToken#policies}
+        :param role: role block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#role AclToken#role}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -297,15 +297,15 @@
     },
 )
 class AclTokenConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         type: builtins.str,
         expiration_ttl: typing.Optional[builtins.str] = None,
@@ -319,21 +319,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param type: The type of token to create, 'client' or 'management'. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#type AclToken#type}
-        :param expiration_ttl: Provides a TTL for the token in the form of a time duration such as "5m" or "1h". Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#expiration_ttl AclToken#expiration_ttl}
-        :param global_: Whether the token should be replicated to all regions or not. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#global AclToken#global}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#id AclToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: Human-readable name for this token. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#name AclToken#name}
-        :param policies: The ACL policies to associate with the token, if it's a 'client' type. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#policies AclToken#policies}
-        :param role: role block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#role AclToken#role}
+        :param type: The type of token to create, 'client' or 'management'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#type AclToken#type}
+        :param expiration_ttl: Provides a TTL for the token in the form of a time duration such as "5m" or "1h". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#expiration_ttl AclToken#expiration_ttl}
+        :param global_: Whether the token should be replicated to all regions or not. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#global AclToken#global}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#id AclToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Human-readable name for this token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#name AclToken#name}
+        :param policies: The ACL policies to associate with the token, if it's a 'client' type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#policies AclToken#policies}
+        :param role: role block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#role AclToken#role}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3ed26cf3b8c1be89d8a5826386350923bbaecdcf77b0b46424c0e40866d03998)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -386,20 +386,22 @@
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
@@ -441,75 +443,75 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def type(self) -> builtins.str:
         '''The type of token to create, 'client' or 'management'.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#type AclToken#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#type AclToken#type}
         '''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def expiration_ttl(self) -> typing.Optional[builtins.str]:
         '''Provides a TTL for the token in the form of a time duration such as "5m" or "1h".
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#expiration_ttl AclToken#expiration_ttl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#expiration_ttl AclToken#expiration_ttl}
         '''
         result = self._values.get("expiration_ttl")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def global_(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether the token should be replicated to all regions or not.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#global AclToken#global}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#global AclToken#global}
         '''
         result = self._values.get("global_")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#id AclToken#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#id AclToken#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''Human-readable name for this token.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#name AclToken#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#name AclToken#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def policies(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The ACL policies to associate with the token, if it's a 'client' type.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#policies AclToken#policies}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#policies AclToken#policies}
         '''
         result = self._values.get("policies")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def role(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["AclTokenRole"]]]:
         '''role block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#role AclToken#role}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#role AclToken#role}
         '''
         result = self._values.get("role")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["AclTokenRole"]]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -526,28 +528,28 @@
     jsii_type="@cdktf/provider-nomad.aclToken.AclTokenRole",
     jsii_struct_bases=[],
     name_mapping={"id": "id"},
 )
 class AclTokenRole:
     def __init__(self, *, id: builtins.str) -> None:
         '''
-        :param id: The ID of the ACL role to link. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#id AclToken#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: The ID of the ACL role to link. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#id AclToken#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__196f11e7fdca8879341cc445d394ca47f5eabf62fa3bad01e26119a9c77f1c33)
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "id": id,
         }
 
     @builtins.property
     def id(self) -> builtins.str:
         '''The ID of the ACL role to link.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/acl_token#id AclToken#id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/acl_token#id AclToken#id}
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         assert result is not None, "Required property 'id' is missing"
         return typing.cast(builtins.str, result)
@@ -738,15 +740,15 @@
     expiration_ttl: typing.Optional[builtins.str] = None,
     global_: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     id: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     policies: typing.Optional[typing.Sequence[builtins.str]] = None,
     role: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[AclTokenRole, typing.Dict[builtins.str, typing.Any]]]]] = None,
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
@@ -793,15 +795,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__3ed26cf3b8c1be89d8a5826386350923bbaecdcf77b0b46424c0e40866d03998(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     type: builtins.str,
     expiration_ttl: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policies/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policies/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_nomad_acl_policies`
 
-Refer to the Terraform Registory for docs: [`data_nomad_acl_policies`](https://www.terraform.io/docs/providers/nomad/d/acl_policies).
+Refer to the Terraform Registory for docs: [`data_nomad_acl_policies`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_policies).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,37 +22,37 @@
 
 
 class DataNomadAclPolicies(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.dataNomadAclPolicies.DataNomadAclPolicies",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/d/acl_policies nomad_acl_policies}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_policies nomad_acl_policies}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: typing.Optional[builtins.str] = None,
         prefix: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/d/acl_policies nomad_acl_policies} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_policies nomad_acl_policies} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_policies#id DataNomadAclPolicies#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param prefix: ACL Policy Name Prefix. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_policies#prefix DataNomadAclPolicies#prefix}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_policies#id DataNomadAclPolicies#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param prefix: ACL Policy Name Prefix. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_policies#prefix DataNomadAclPolicies#prefix}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -148,15 +148,15 @@
     },
 )
 class DataNomadAclPoliciesConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         id: typing.Optional[builtins.str] = None,
         prefix: typing.Optional[builtins.str] = None,
@@ -165,16 +165,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_policies#id DataNomadAclPolicies#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param prefix: ACL Policy Name Prefix. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_policies#prefix DataNomadAclPolicies#prefix}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_policies#id DataNomadAclPolicies#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param prefix: ACL Policy Name Prefix. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_policies#prefix DataNomadAclPolicies#prefix}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4c473dc5e4d524001478fa016e33a6c7e01e19fe432a8d0b3ef9bddf03bf5a0e)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -212,20 +212,22 @@
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
@@ -265,27 +267,27 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_policies#id DataNomadAclPolicies#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_policies#id DataNomadAclPolicies#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def prefix(self) -> typing.Optional[builtins.str]:
         '''ACL Policy Name Prefix.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_policies#prefix DataNomadAclPolicies#prefix}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_policies#prefix DataNomadAclPolicies#prefix}
         '''
         result = self._values.get("prefix")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -457,15 +459,15 @@
 def _typecheckingstub__99d1b3832e23778e28591d3ad8e81bdea5e4ec9365468afdeb35fafbf572288f(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     id: typing.Optional[builtins.str] = None,
     prefix: typing.Optional[builtins.str] = None,
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
@@ -482,15 +484,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__4c473dc5e4d524001478fa016e33a6c7e01e19fe432a8d0b3ef9bddf03bf5a0e(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     id: typing.Optional[builtins.str] = None,
     prefix: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policy/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_nomad_acl_policy`
 
-Refer to the Terraform Registory for docs: [`data_nomad_acl_policy`](https://www.terraform.io/docs/providers/nomad/d/acl_policy).
+Refer to the Terraform Registory for docs: [`data_nomad_acl_policy`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_policy).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,37 +22,37 @@
 
 
 class DataNomadAclPolicy(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.dataNomadAclPolicy.DataNomadAclPolicy",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/d/acl_policy nomad_acl_policy}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_policy nomad_acl_policy}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
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
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/d/acl_policy nomad_acl_policy} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_policy nomad_acl_policy} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_policy#name DataNomadAclPolicy#name}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_policy#id DataNomadAclPolicy#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_policy#name DataNomadAclPolicy#name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_policy#id DataNomadAclPolicy#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -149,15 +149,15 @@
     },
 )
 class DataNomadAclPolicyConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         id: typing.Optional[builtins.str] = None,
@@ -166,16 +166,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_policy#name DataNomadAclPolicy#name}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_policy#id DataNomadAclPolicy#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_policy#name DataNomadAclPolicy#name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_policy#id DataNomadAclPolicy#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__018dde363310928fc9da982d1844c154ed4944629dd860eaf1d1a9fecdcfe02c)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -213,20 +213,22 @@
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
@@ -268,23 +270,23 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''Name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_policy#name DataNomadAclPolicy#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_policy#name DataNomadAclPolicy#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_policy#id DataNomadAclPolicy#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_policy#id DataNomadAclPolicy#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -310,15 +312,15 @@
 def _typecheckingstub__481db60ddc7e24d58fbbffcc4b9a1d4fa1e6f9d4620075c58901770b963d3761(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     name: builtins.str,
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
@@ -335,15 +337,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__018dde363310928fc9da982d1844c154ed4944629dd860eaf1d1a9fecdcfe02c(
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
     id: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_role/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_role/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_nomad_acl_role`
 
-Refer to the Terraform Registory for docs: [`data_nomad_acl_role`](https://www.terraform.io/docs/providers/nomad/d/acl_role).
+Refer to the Terraform Registory for docs: [`data_nomad_acl_role`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_role).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,35 +22,35 @@
 
 
 class DataNomadAclRole(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.dataNomadAclRole.DataNomadAclRole",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/d/acl_role nomad_acl_role}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_role nomad_acl_role}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: builtins.str,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/d/acl_role nomad_acl_role} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_role nomad_acl_role} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: The ACL Role unique identifier. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_role#id DataNomadAclRole#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: The ACL Role unique identifier. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_role#id DataNomadAclRole#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -129,15 +129,15 @@
     },
 )
 class DataNomadAclRoleConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         id: builtins.str,
     ) -> None:
@@ -145,15 +145,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: The ACL Role unique identifier. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_role#id DataNomadAclRole#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: The ACL Role unique identifier. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_role#id DataNomadAclRole#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0aad8ffa522dbbc60abe11e298e2aa447ab4c96c2ba7aa9cd9d1bd66be43fd4e)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -188,20 +188,22 @@
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
@@ -243,15 +245,15 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> builtins.str:
         '''The ACL Role unique identifier.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_role#id DataNomadAclRole#id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_role#id DataNomadAclRole#id}
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         assert result is not None, "Required property 'id' is missing"
         return typing.cast(builtins.str, result)
@@ -418,15 +420,15 @@
 
 def _typecheckingstub__33984ba4bed2a6fe922c84cee04cfea7fed8255793212323dc34c4bead1463ad(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     id: builtins.str,
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
@@ -437,15 +439,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__0aad8ffa522dbbc60abe11e298e2aa447ab4c96c2ba7aa9cd9d1bd66be43fd4e(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     id: builtins.str,
 ) -> None:
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_roles/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_roles/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_nomad_acl_roles`
 
-Refer to the Terraform Registory for docs: [`data_nomad_acl_roles`](https://www.terraform.io/docs/providers/nomad/d/acl_roles).
+Refer to the Terraform Registory for docs: [`data_nomad_acl_roles`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_roles).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,37 +22,37 @@
 
 
 class DataNomadAclRoles(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.dataNomadAclRoles.DataNomadAclRoles",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/d/acl_roles nomad_acl_roles}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_roles nomad_acl_roles}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: typing.Optional[builtins.str] = None,
         prefix: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/d/acl_roles nomad_acl_roles} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_roles nomad_acl_roles} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_roles#id DataNomadAclRoles#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param prefix: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_roles#prefix DataNomadAclRoles#prefix}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_roles#id DataNomadAclRoles#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param prefix: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_roles#prefix DataNomadAclRoles#prefix}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -445,15 +445,15 @@
     },
 )
 class DataNomadAclRolesConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         id: typing.Optional[builtins.str] = None,
         prefix: typing.Optional[builtins.str] = None,
@@ -462,16 +462,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_roles#id DataNomadAclRoles#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param prefix: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_roles#prefix DataNomadAclRoles#prefix}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_roles#id DataNomadAclRoles#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param prefix: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_roles#prefix DataNomadAclRoles#prefix}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ae442f4d72521b3841219b6976d9f63d1786deaa362aeaf5e2c55cd28dca8184)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -509,20 +509,22 @@
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
@@ -562,25 +564,25 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_roles#id DataNomadAclRoles#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_roles#id DataNomadAclRoles#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def prefix(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_roles#prefix DataNomadAclRoles#prefix}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_roles#prefix DataNomadAclRoles#prefix}.'''
         result = self._values.get("prefix")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -608,15 +610,15 @@
 def _typecheckingstub__63c4aaae6a4b7e8fe6e5594f5441154c9b87fa91723f3d338d9d65aba4c8ea42(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     id: typing.Optional[builtins.str] = None,
     prefix: typing.Optional[builtins.str] = None,
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
@@ -727,15 +729,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__ae442f4d72521b3841219b6976d9f63d1786deaa362aeaf5e2c55cd28dca8184(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     id: typing.Optional[builtins.str] = None,
     prefix: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_token/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_token/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_nomad_acl_token`
 
-Refer to the Terraform Registory for docs: [`data_nomad_acl_token`](https://www.terraform.io/docs/providers/nomad/d/acl_token).
+Refer to the Terraform Registory for docs: [`data_nomad_acl_token`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_token).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,37 +22,37 @@
 
 
 class DataNomadAclToken(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.dataNomadAclToken.DataNomadAclToken",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/d/acl_token nomad_acl_token}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_token nomad_acl_token}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         accessor_id: builtins.str,
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
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/d/acl_token nomad_acl_token} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_token nomad_acl_token} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param accessor_id: Non-sensitive identifier for this token. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_token#accessor_id DataNomadAclToken#accessor_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_token#id DataNomadAclToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param accessor_id: Non-sensitive identifier for this token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_token#accessor_id DataNomadAclToken#accessor_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_token#id DataNomadAclToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
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
 class DataNomadAclTokenConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         accessor_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
@@ -201,16 +201,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param accessor_id: Non-sensitive identifier for this token. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_token#accessor_id DataNomadAclToken#accessor_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_token#id DataNomadAclToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param accessor_id: Non-sensitive identifier for this token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_token#accessor_id DataNomadAclToken#accessor_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_token#id DataNomadAclToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__efaed7a6c029ffedd571b623dd5e20f94d6b979caee33a6c8df03940b75332e6)
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
     def accessor_id(self) -> builtins.str:
         '''Non-sensitive identifier for this token.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_token#accessor_id DataNomadAclToken#accessor_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_token#accessor_id DataNomadAclToken#accessor_id}
         '''
         result = self._values.get("accessor_id")
         assert result is not None, "Required property 'accessor_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_token#id DataNomadAclToken#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_token#id DataNomadAclToken#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -491,15 +493,15 @@
 def _typecheckingstub__ebafd7dc059ad1cace26d49d00b03f59cd867e125e2665faa509017f11921a7e(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     accessor_id: builtins.str,
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
@@ -516,15 +518,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__efaed7a6c029ffedd571b623dd5e20f94d6b979caee33a6c8df03940b75332e6(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     accessor_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_tokens/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_acl_tokens/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_nomad_acl_tokens`
 
-Refer to the Terraform Registory for docs: [`data_nomad_acl_tokens`](https://www.terraform.io/docs/providers/nomad/d/acl_tokens).
+Refer to the Terraform Registory for docs: [`data_nomad_acl_tokens`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_tokens).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,37 +22,37 @@
 
 
 class DataNomadAclTokens(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.dataNomadAclTokens.DataNomadAclTokens",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/d/acl_tokens nomad_acl_tokens}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_tokens nomad_acl_tokens}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: typing.Optional[builtins.str] = None,
         prefix: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/d/acl_tokens nomad_acl_tokens} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_tokens nomad_acl_tokens} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_tokens#id DataNomadAclTokens#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param prefix: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_tokens#prefix DataNomadAclTokens#prefix}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_tokens#id DataNomadAclTokens#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param prefix: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_tokens#prefix DataNomadAclTokens#prefix}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -473,15 +473,15 @@
     },
 )
 class DataNomadAclTokensConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         id: typing.Optional[builtins.str] = None,
         prefix: typing.Optional[builtins.str] = None,
@@ -490,16 +490,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_tokens#id DataNomadAclTokens#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param prefix: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_tokens#prefix DataNomadAclTokens#prefix}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_tokens#id DataNomadAclTokens#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param prefix: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_tokens#prefix DataNomadAclTokens#prefix}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d7e8beab2879f9bb6f5e5fe1aa897f18358a77c34988ee8801144c5d45fe0e6f)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -537,20 +537,22 @@
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
@@ -590,25 +592,25 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_tokens#id DataNomadAclTokens#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_tokens#id DataNomadAclTokens#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def prefix(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/acl_tokens#prefix DataNomadAclTokens#prefix}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/acl_tokens#prefix DataNomadAclTokens#prefix}.'''
         result = self._values.get("prefix")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -636,15 +638,15 @@
 def _typecheckingstub__23ccb4853d8e73ea8ab615eb9212abd25cd5f4fa8372f7d7d87b298e95e06251(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     id: typing.Optional[builtins.str] = None,
     prefix: typing.Optional[builtins.str] = None,
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
@@ -755,15 +757,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__d7e8beab2879f9bb6f5e5fe1aa897f18358a77c34988ee8801144c5d45fe0e6f(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     id: typing.Optional[builtins.str] = None,
     prefix: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_datacenters/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_datacenters/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_nomad_datacenters`
 
-Refer to the Terraform Registory for docs: [`data_nomad_datacenters`](https://www.terraform.io/docs/providers/nomad/d/datacenters).
+Refer to the Terraform Registory for docs: [`data_nomad_datacenters`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/datacenters).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,39 +22,39 @@
 
 
 class DataNomadDatacenters(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.dataNomadDatacenters.DataNomadDatacenters",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/d/datacenters nomad_datacenters}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/datacenters nomad_datacenters}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: typing.Optional[builtins.str] = None,
         ignore_down_nodes: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         prefix: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/d/datacenters nomad_datacenters} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/datacenters nomad_datacenters} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/datacenters#id DataNomadDatacenters#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param ignore_down_nodes: If enabled, this flag will ignore nodes that are down when listing datacenters. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/datacenters#ignore_down_nodes DataNomadDatacenters#ignore_down_nodes}
-        :param prefix: Prefix value used for filtering results. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/datacenters#prefix DataNomadDatacenters#prefix}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/datacenters#id DataNomadDatacenters#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param ignore_down_nodes: If enabled, this flag will ignore nodes that are down when listing datacenters. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/datacenters#ignore_down_nodes DataNomadDatacenters#ignore_down_nodes}
+        :param prefix: Prefix value used for filtering results. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/datacenters#prefix DataNomadDatacenters#prefix}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -180,15 +180,15 @@
     },
 )
 class DataNomadDatacentersConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         id: typing.Optional[builtins.str] = None,
         ignore_down_nodes: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
@@ -198,17 +198,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/datacenters#id DataNomadDatacenters#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param ignore_down_nodes: If enabled, this flag will ignore nodes that are down when listing datacenters. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/datacenters#ignore_down_nodes DataNomadDatacenters#ignore_down_nodes}
-        :param prefix: Prefix value used for filtering results. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/datacenters#prefix DataNomadDatacenters#prefix}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/datacenters#id DataNomadDatacenters#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param ignore_down_nodes: If enabled, this flag will ignore nodes that are down when listing datacenters. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/datacenters#ignore_down_nodes DataNomadDatacenters#ignore_down_nodes}
+        :param prefix: Prefix value used for filtering results. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/datacenters#prefix DataNomadDatacenters#prefix}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__baa347359ec5c81f44beedb94b3631ca3974400dc5f28332ab000f4aa5fdff5a)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -249,20 +249,22 @@
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
@@ -302,38 +304,38 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/datacenters#id DataNomadDatacenters#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/datacenters#id DataNomadDatacenters#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ignore_down_nodes(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If enabled, this flag will ignore nodes that are down when listing datacenters.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/datacenters#ignore_down_nodes DataNomadDatacenters#ignore_down_nodes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/datacenters#ignore_down_nodes DataNomadDatacenters#ignore_down_nodes}
         '''
         result = self._values.get("ignore_down_nodes")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def prefix(self) -> typing.Optional[builtins.str]:
         '''Prefix value used for filtering results.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/datacenters#prefix DataNomadDatacenters#prefix}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/datacenters#prefix DataNomadDatacenters#prefix}
         '''
         result = self._values.get("prefix")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -357,15 +359,15 @@
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     id: typing.Optional[builtins.str] = None,
     ignore_down_nodes: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     prefix: typing.Optional[builtins.str] = None,
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
@@ -388,15 +390,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__baa347359ec5c81f44beedb94b3631ca3974400dc5f28332ab000f4aa5fdff5a(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     id: typing.Optional[builtins.str] = None,
     ignore_down_nodes: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_deployments/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_deployments/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_nomad_deployments`
 
-Refer to the Terraform Registory for docs: [`data_nomad_deployments`](https://www.terraform.io/docs/providers/nomad/d/deployments).
+Refer to the Terraform Registory for docs: [`data_nomad_deployments`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/deployments).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,35 +22,35 @@
 
 
 class DataNomadDeployments(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.dataNomadDeployments.DataNomadDeployments",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/d/deployments nomad_deployments}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/deployments nomad_deployments}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
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
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/d/deployments nomad_deployments} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/deployments nomad_deployments} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/deployments#id DataNomadDeployments#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/deployments#id DataNomadDeployments#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -123,15 +123,15 @@
     },
 )
 class DataNomadDeploymentsConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         id: typing.Optional[builtins.str] = None,
     ) -> None:
@@ -139,15 +139,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/deployments#id DataNomadDeployments#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/deployments#id DataNomadDeployments#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__58b776b8f0a5075d5d60581d7f9ba45117d8ae3cf307b5ddfccdcbea19c05d79)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -182,20 +182,22 @@
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
@@ -235,15 +237,15 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/deployments#id DataNomadDeployments#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/deployments#id DataNomadDeployments#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -268,15 +270,15 @@
 
 def _typecheckingstub__bd2c5966b4fe2f6ca4e93a7201a581d256b888f072f1b630c52de9390e8c5c80(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
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
@@ -287,15 +289,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__58b776b8f0a5075d5d60581d7f9ba45117d8ae3cf307b5ddfccdcbea19c05d79(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     id: typing.Optional[builtins.str] = None,
 ) -> None:
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_job/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_job/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_nomad_job`
 
-Refer to the Terraform Registory for docs: [`data_nomad_job`](https://www.terraform.io/docs/providers/nomad/d/job).
+Refer to the Terraform Registory for docs: [`data_nomad_job`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,39 +22,39 @@
 
 
 class DataNomadJob(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.dataNomadJob.DataNomadJob",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/d/job nomad_job}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job nomad_job}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         job_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
         namespace: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/d/job nomad_job} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job nomad_job} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param job_id: Job ID. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/job#job_id DataNomadJob#job_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/job#id DataNomadJob#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param namespace: Job Namespace. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/job#namespace DataNomadJob#namespace}
+        :param job_id: Job ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job#job_id DataNomadJob#job_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job#id DataNomadJob#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param namespace: Job Namespace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job#namespace DataNomadJob#namespace}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -259,15 +259,15 @@
     },
 )
 class DataNomadJobConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         job_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
@@ -277,17 +277,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param job_id: Job ID. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/job#job_id DataNomadJob#job_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/job#id DataNomadJob#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param namespace: Job Namespace. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/job#namespace DataNomadJob#namespace}
+        :param job_id: Job ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job#job_id DataNomadJob#job_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job#id DataNomadJob#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param namespace: Job Namespace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job#namespace DataNomadJob#namespace}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ac5285161a6cb42ba4e7cb2c387e0a4a8b91b20306141b8eb5e3d73517359c0b)
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
@@ -383,35 +385,35 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def job_id(self) -> builtins.str:
         '''Job ID.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/job#job_id DataNomadJob#job_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job#job_id DataNomadJob#job_id}
         '''
         result = self._values.get("job_id")
         assert result is not None, "Required property 'job_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/job#id DataNomadJob#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job#id DataNomadJob#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def namespace(self) -> typing.Optional[builtins.str]:
         '''Job Namespace.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/job#namespace DataNomadJob#namespace}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job#namespace DataNomadJob#namespace}
         '''
         result = self._values.get("namespace")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1386,15 +1388,15 @@
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     job_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
     namespace: typing.Optional[builtins.str] = None,
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
@@ -1417,15 +1419,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__ac5285161a6cb42ba4e7cb2c387e0a4a8b91b20306141b8eb5e3d73517359c0b(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     job_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_job_parser/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_job_parser/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_nomad_job_parser`
 
-Refer to the Terraform Registory for docs: [`data_nomad_job_parser`](https://www.terraform.io/docs/providers/nomad/d/job_parser).
+Refer to the Terraform Registory for docs: [`data_nomad_job_parser`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job_parser).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,39 +22,39 @@
 
 
 class DataNomadJobParser(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.dataNomadJobParser.DataNomadJobParser",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/d/job_parser nomad_job_parser}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job_parser nomad_job_parser}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         hcl: builtins.str,
         canonicalize: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
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
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/d/job_parser nomad_job_parser} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job_parser nomad_job_parser} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param hcl: Specifies the HCL definition of the job encoded in a JSON string. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/job_parser#hcl DataNomadJobParser#hcl}
-        :param canonicalize: Flag to enable setting any unset fields to their default values. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/job_parser#canonicalize DataNomadJobParser#canonicalize}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/job_parser#id DataNomadJobParser#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param hcl: Specifies the HCL definition of the job encoded in a JSON string. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job_parser#hcl DataNomadJobParser#hcl}
+        :param canonicalize: Flag to enable setting any unset fields to their default values. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job_parser#canonicalize DataNomadJobParser#canonicalize}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job_parser#id DataNomadJobParser#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -174,15 +174,15 @@
     },
 )
 class DataNomadJobParserConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         hcl: builtins.str,
         canonicalize: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
@@ -192,17 +192,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param hcl: Specifies the HCL definition of the job encoded in a JSON string. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/job_parser#hcl DataNomadJobParser#hcl}
-        :param canonicalize: Flag to enable setting any unset fields to their default values. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/job_parser#canonicalize DataNomadJobParser#canonicalize}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/job_parser#id DataNomadJobParser#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param hcl: Specifies the HCL definition of the job encoded in a JSON string. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job_parser#hcl DataNomadJobParser#hcl}
+        :param canonicalize: Flag to enable setting any unset fields to their default values. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job_parser#canonicalize DataNomadJobParser#canonicalize}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job_parser#id DataNomadJobParser#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0fadd74699e47513de3c6eacc468c717dc2b36cf878b91aadf7c1da7f4d09534)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -243,20 +243,22 @@
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
@@ -298,34 +300,34 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def hcl(self) -> builtins.str:
         '''Specifies the HCL definition of the job encoded in a JSON string.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/job_parser#hcl DataNomadJobParser#hcl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job_parser#hcl DataNomadJobParser#hcl}
         '''
         result = self._values.get("hcl")
         assert result is not None, "Required property 'hcl' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def canonicalize(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Flag to enable setting any unset fields to their default values.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/job_parser#canonicalize DataNomadJobParser#canonicalize}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job_parser#canonicalize DataNomadJobParser#canonicalize}
         '''
         result = self._values.get("canonicalize")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/job_parser#id DataNomadJobParser#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/job_parser#id DataNomadJobParser#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -352,15 +354,15 @@
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     hcl: builtins.str,
     canonicalize: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
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
@@ -383,15 +385,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__0fadd74699e47513de3c6eacc468c717dc2b36cf878b91aadf7c1da7f4d09534(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     hcl: builtins.str,
     canonicalize: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_namespace/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_namespace/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_nomad_namespace`
 
-Refer to the Terraform Registory for docs: [`data_nomad_namespace`](https://www.terraform.io/docs/providers/nomad/d/namespace).
+Refer to the Terraform Registory for docs: [`data_nomad_namespace`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/namespace).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,37 +22,37 @@
 
 
 class DataNomadNamespace(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.dataNomadNamespace.DataNomadNamespace",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/d/namespace nomad_namespace}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/namespace nomad_namespace}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
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
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/d/namespace nomad_namespace} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/namespace nomad_namespace} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/namespace#name DataNomadNamespace#name}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/namespace#id DataNomadNamespace#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/namespace#name DataNomadNamespace#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/namespace#id DataNomadNamespace#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -308,15 +308,15 @@
     },
 )
 class DataNomadNamespaceConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         id: typing.Optional[builtins.str] = None,
@@ -325,16 +325,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/namespace#name DataNomadNamespace#name}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/namespace#id DataNomadNamespace#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/namespace#name DataNomadNamespace#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/namespace#id DataNomadNamespace#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__494e2120d48a3e41c0624c41c109c43145962d975bc11ca3df6b156567d1c2cb)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -372,20 +372,22 @@
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
@@ -425,22 +427,22 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/namespace#name DataNomadNamespace#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/namespace#name DataNomadNamespace#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/namespace#id DataNomadNamespace#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/namespace#id DataNomadNamespace#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -469,15 +471,15 @@
 def _typecheckingstub__62e3a34045887dab9fc9579f5fe1d7382cd2810b350ee0c089322c47d22a743d(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     name: builtins.str,
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
@@ -541,15 +543,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__494e2120d48a3e41c0624c41c109c43145962d975bc11ca3df6b156567d1c2cb(
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
     id: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_namespaces/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_namespaces/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_nomad_namespaces`
 
-Refer to the Terraform Registory for docs: [`data_nomad_namespaces`](https://www.terraform.io/docs/providers/nomad/d/namespaces).
+Refer to the Terraform Registory for docs: [`data_nomad_namespaces`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/namespaces).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,35 +22,35 @@
 
 
 class DataNomadNamespaces(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.dataNomadNamespaces.DataNomadNamespaces",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/d/namespaces nomad_namespaces}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/namespaces nomad_namespaces}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
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
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/d/namespaces nomad_namespaces} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/namespaces nomad_namespaces} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/namespaces#id DataNomadNamespaces#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/namespaces#id DataNomadNamespaces#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -123,15 +123,15 @@
     },
 )
 class DataNomadNamespacesConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         id: typing.Optional[builtins.str] = None,
     ) -> None:
@@ -139,15 +139,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/namespaces#id DataNomadNamespaces#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/namespaces#id DataNomadNamespaces#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4181cf0cc40d8776f4e4e35972d25964fb3d5544f6a10169bcfb121c92bf567f)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -182,20 +182,22 @@
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
@@ -235,15 +237,15 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/namespaces#id DataNomadNamespaces#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/namespaces#id DataNomadNamespaces#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -268,15 +270,15 @@
 
 def _typecheckingstub__72bf090d2d0140765055fc4ebace9396ff6901570c05dbbe038520e1624ad081(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
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
@@ -287,15 +289,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__4181cf0cc40d8776f4e4e35972d25964fb3d5544f6a10169bcfb121c92bf567f(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     id: typing.Optional[builtins.str] = None,
 ) -> None:
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_plugin/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_plugin/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_nomad_plugin`
 
-Refer to the Terraform Registory for docs: [`data_nomad_plugin`](https://www.terraform.io/docs/providers/nomad/d/plugin).
+Refer to the Terraform Registory for docs: [`data_nomad_plugin`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugin).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,41 +22,41 @@
 
 
 class DataNomadPlugin(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.dataNomadPlugin.DataNomadPlugin",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/d/plugin nomad_plugin}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugin nomad_plugin}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         plugin_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
         wait_for_healthy: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         wait_for_registration: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/d/plugin nomad_plugin} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugin nomad_plugin} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param plugin_id: Plugin ID. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/plugin#plugin_id DataNomadPlugin#plugin_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/plugin#id DataNomadPlugin#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param wait_for_healthy: Wait for to be backed by a specified number of controllers. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/plugin#wait_for_healthy DataNomadPlugin#wait_for_healthy}
-        :param wait_for_registration: Wait for the plugin to be registered in Noamd. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/plugin#wait_for_registration DataNomadPlugin#wait_for_registration}
+        :param plugin_id: Plugin ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugin#plugin_id DataNomadPlugin#plugin_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugin#id DataNomadPlugin#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param wait_for_healthy: Wait for to be backed by a specified number of controllers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugin#wait_for_healthy DataNomadPlugin#wait_for_healthy}
+        :param wait_for_registration: Wait for the plugin to be registered in Noamd. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugin#wait_for_registration DataNomadPlugin#wait_for_registration}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -243,15 +243,15 @@
     },
 )
 class DataNomadPluginConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         plugin_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
@@ -262,18 +262,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param plugin_id: Plugin ID. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/plugin#plugin_id DataNomadPlugin#plugin_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/plugin#id DataNomadPlugin#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param wait_for_healthy: Wait for to be backed by a specified number of controllers. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/plugin#wait_for_healthy DataNomadPlugin#wait_for_healthy}
-        :param wait_for_registration: Wait for the plugin to be registered in Noamd. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/plugin#wait_for_registration DataNomadPlugin#wait_for_registration}
+        :param plugin_id: Plugin ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugin#plugin_id DataNomadPlugin#plugin_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugin#id DataNomadPlugin#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param wait_for_healthy: Wait for to be backed by a specified number of controllers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugin#wait_for_healthy DataNomadPlugin#wait_for_healthy}
+        :param wait_for_registration: Wait for the plugin to be registered in Noamd. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugin#wait_for_registration DataNomadPlugin#wait_for_registration}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__68692a1a631ac34086920f116c918372fa6961ce1e679518ee021c81e2fae3ea)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -317,20 +317,22 @@
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
@@ -372,48 +374,48 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def plugin_id(self) -> builtins.str:
         '''Plugin ID.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/plugin#plugin_id DataNomadPlugin#plugin_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugin#plugin_id DataNomadPlugin#plugin_id}
         '''
         result = self._values.get("plugin_id")
         assert result is not None, "Required property 'plugin_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/plugin#id DataNomadPlugin#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugin#id DataNomadPlugin#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def wait_for_healthy(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Wait for to be backed by a specified number of controllers.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/plugin#wait_for_healthy DataNomadPlugin#wait_for_healthy}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugin#wait_for_healthy DataNomadPlugin#wait_for_healthy}
         '''
         result = self._values.get("wait_for_healthy")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def wait_for_registration(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Wait for the plugin to be registered in Noamd.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/plugin#wait_for_registration DataNomadPlugin#wait_for_registration}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugin#wait_for_registration DataNomadPlugin#wait_for_registration}
         '''
         result = self._values.get("wait_for_registration")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -589,15 +591,15 @@
     id_: builtins.str,
     *,
     plugin_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
     wait_for_healthy: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     wait_for_registration: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
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
@@ -626,15 +628,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__68692a1a631ac34086920f116c918372fa6961ce1e679518ee021c81e2fae3ea(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     plugin_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_plugins/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_plugins/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_nomad_plugins`
 
-Refer to the Terraform Registory for docs: [`data_nomad_plugins`](https://www.terraform.io/docs/providers/nomad/d/plugins).
+Refer to the Terraform Registory for docs: [`data_nomad_plugins`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugins).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,37 +22,37 @@
 
 
 class DataNomadPlugins(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.dataNomadPlugins.DataNomadPlugins",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/d/plugins nomad_plugins}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugins nomad_plugins}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: typing.Optional[builtins.str] = None,
         type: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/d/plugins nomad_plugins} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugins nomad_plugins} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/plugins#id DataNomadPlugins#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param type: Volume Type (currently only 'csi'). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/plugins#type DataNomadPlugins#type}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugins#id DataNomadPlugins#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param type: Volume Type (currently only 'csi'). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugins#type DataNomadPlugins#type}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -148,15 +148,15 @@
     },
 )
 class DataNomadPluginsConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         id: typing.Optional[builtins.str] = None,
         type: typing.Optional[builtins.str] = None,
@@ -165,16 +165,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/plugins#id DataNomadPlugins#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param type: Volume Type (currently only 'csi'). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/plugins#type DataNomadPlugins#type}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugins#id DataNomadPlugins#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param type: Volume Type (currently only 'csi'). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugins#type DataNomadPlugins#type}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__528691e1aeb913541e94efbed9b44d60c8dfab87377894b4280a8bf8b44ca055)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -212,20 +212,22 @@
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
@@ -265,27 +267,27 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/plugins#id DataNomadPlugins#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugins#id DataNomadPlugins#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
         '''Volume Type (currently only 'csi').
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/plugins#type DataNomadPlugins#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/plugins#type DataNomadPlugins#type}
         '''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -308,15 +310,15 @@
 def _typecheckingstub__166971278a2d93e7fce1c4f93f53b5e49b79432bf8f8d821249a145ed14934eb(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     id: typing.Optional[builtins.str] = None,
     type: typing.Optional[builtins.str] = None,
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
@@ -333,15 +335,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__528691e1aeb913541e94efbed9b44d60c8dfab87377894b4280a8bf8b44ca055(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     id: typing.Optional[builtins.str] = None,
     type: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_regions/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_regions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_nomad_regions`
 
-Refer to the Terraform Registory for docs: [`data_nomad_regions`](https://www.terraform.io/docs/providers/nomad/d/regions).
+Refer to the Terraform Registory for docs: [`data_nomad_regions`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/regions).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,35 +22,35 @@
 
 
 class DataNomadRegions(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.dataNomadRegions.DataNomadRegions",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/d/regions nomad_regions}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/regions nomad_regions}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
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
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/d/regions nomad_regions} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/regions nomad_regions} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/regions#id DataNomadRegions#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/regions#id DataNomadRegions#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -123,15 +123,15 @@
     },
 )
 class DataNomadRegionsConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         id: typing.Optional[builtins.str] = None,
     ) -> None:
@@ -139,15 +139,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/regions#id DataNomadRegions#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/regions#id DataNomadRegions#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cd70805bebf2c3edc3c4ade9360949d621fef945bce118aafdf8e0cabf94195e)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -182,20 +182,22 @@
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
@@ -235,15 +237,15 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/regions#id DataNomadRegions#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/regions#id DataNomadRegions#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -268,15 +270,15 @@
 
 def _typecheckingstub__397366386cfb664e056ecc1c067824c40ed93ecc94dea2bcbb2ccae27c5f8aae(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
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
@@ -287,15 +289,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__cd70805bebf2c3edc3c4ade9360949d621fef945bce118aafdf8e0cabf94195e(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     id: typing.Optional[builtins.str] = None,
 ) -> None:
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policies/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policies/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_nomad_scaling_policies`
 
-Refer to the Terraform Registory for docs: [`data_nomad_scaling_policies`](https://www.terraform.io/docs/providers/nomad/d/scaling_policies).
+Refer to the Terraform Registory for docs: [`data_nomad_scaling_policies`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scaling_policies).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,39 +22,39 @@
 
 
 class DataNomadScalingPolicies(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.dataNomadScalingPolicies.DataNomadScalingPolicies",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/d/scaling_policies nomad_scaling_policies}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scaling_policies nomad_scaling_policies}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: typing.Optional[builtins.str] = None,
         job_id: typing.Optional[builtins.str] = None,
         type: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/d/scaling_policies nomad_scaling_policies} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scaling_policies nomad_scaling_policies} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/scaling_policies#id DataNomadScalingPolicies#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param job_id: Job ID to use to filter scaling policies. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/scaling_policies#job_id DataNomadScalingPolicies#job_id}
-        :param type: Scaling policy type used to filter scaling policies. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/scaling_policies#type DataNomadScalingPolicies#type}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scaling_policies#id DataNomadScalingPolicies#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param job_id: Job ID to use to filter scaling policies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scaling_policies#job_id DataNomadScalingPolicies#job_id}
+        :param type: Scaling policy type used to filter scaling policies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scaling_policies#type DataNomadScalingPolicies#type}
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
 class DataNomadScalingPoliciesConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         id: typing.Optional[builtins.str] = None,
         job_id: typing.Optional[builtins.str] = None,
@@ -191,17 +191,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/scaling_policies#id DataNomadScalingPolicies#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param job_id: Job ID to use to filter scaling policies. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/scaling_policies#job_id DataNomadScalingPolicies#job_id}
-        :param type: Scaling policy type used to filter scaling policies. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/scaling_policies#type DataNomadScalingPolicies#type}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scaling_policies#id DataNomadScalingPolicies#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param job_id: Job ID to use to filter scaling policies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scaling_policies#job_id DataNomadScalingPolicies#job_id}
+        :param type: Scaling policy type used to filter scaling policies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scaling_policies#type DataNomadScalingPolicies#type}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5dc967c5232b19645884d56f1d28cd08dbe2b611c611c05d371ccc53223454e8)
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
@@ -295,36 +297,36 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/scaling_policies#id DataNomadScalingPolicies#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scaling_policies#id DataNomadScalingPolicies#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def job_id(self) -> typing.Optional[builtins.str]:
         '''Job ID to use to filter scaling policies.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/scaling_policies#job_id DataNomadScalingPolicies#job_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scaling_policies#job_id DataNomadScalingPolicies#job_id}
         '''
         result = self._values.get("job_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
         '''Scaling policy type used to filter scaling policies.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/scaling_policies#type DataNomadScalingPolicies#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scaling_policies#type DataNomadScalingPolicies#type}
         '''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -510,15 +512,15 @@
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     id: typing.Optional[builtins.str] = None,
     job_id: typing.Optional[builtins.str] = None,
     type: typing.Optional[builtins.str] = None,
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
@@ -541,15 +543,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__5dc967c5232b19645884d56f1d28cd08dbe2b611c611c05d371ccc53223454e8(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     id: typing.Optional[builtins.str] = None,
     job_id: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policy/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policy/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_nomad_scaling_policy`
 
-Refer to the Terraform Registory for docs: [`data_nomad_scaling_policy`](https://www.terraform.io/docs/providers/nomad/d/scaling_policy).
+Refer to the Terraform Registory for docs: [`data_nomad_scaling_policy`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scaling_policy).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,35 +22,35 @@
 
 
 class DataNomadScalingPolicy(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.dataNomadScalingPolicy.DataNomadScalingPolicy",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/d/scaling_policy nomad_scaling_policy}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scaling_policy nomad_scaling_policy}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: builtins.str,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/d/scaling_policy nomad_scaling_policy} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scaling_policy nomad_scaling_policy} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: The scaling policy ID. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/scaling_policy#id DataNomadScalingPolicy#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: The scaling policy ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scaling_policy#id DataNomadScalingPolicy#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -144,15 +144,15 @@
     },
 )
 class DataNomadScalingPolicyConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         id: builtins.str,
     ) -> None:
@@ -160,15 +160,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: The scaling policy ID. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/scaling_policy#id DataNomadScalingPolicy#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: The scaling policy ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scaling_policy#id DataNomadScalingPolicy#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__058d4e842b9b389e091f3dcbc504fc5c7e6e76a9104590795619b49f73e270c1)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -203,20 +203,22 @@
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
@@ -258,15 +260,15 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> builtins.str:
         '''The scaling policy ID.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/scaling_policy#id DataNomadScalingPolicy#id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scaling_policy#id DataNomadScalingPolicy#id}
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         assert result is not None, "Required property 'id' is missing"
         return typing.cast(builtins.str, result)
@@ -292,15 +294,15 @@
 
 def _typecheckingstub__99c20fa3e79ab77f1c43f44c39d0ad132789bd82980aaa3d921db6e1f5abe277(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     id: builtins.str,
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
@@ -311,15 +313,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__058d4e842b9b389e091f3dcbc504fc5c7e6e76a9104590795619b49f73e270c1(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     id: builtins.str,
 ) -> None:
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_scheduler_config/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_scheduler_config/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_nomad_scheduler_config`
 
-Refer to the Terraform Registory for docs: [`data_nomad_scheduler_config`](https://www.terraform.io/docs/providers/nomad/d/scheduler_config).
+Refer to the Terraform Registory for docs: [`data_nomad_scheduler_config`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scheduler_config).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,35 +22,35 @@
 
 
 class DataNomadSchedulerConfig(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.dataNomadSchedulerConfig.DataNomadSchedulerConfig",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/d/scheduler_config nomad_scheduler_config}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scheduler_config nomad_scheduler_config}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
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
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/d/scheduler_config nomad_scheduler_config} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scheduler_config nomad_scheduler_config} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/scheduler_config#id DataNomadSchedulerConfig#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scheduler_config#id DataNomadSchedulerConfig#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -133,15 +133,15 @@
     },
 )
 class DataNomadSchedulerConfigConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         id: typing.Optional[builtins.str] = None,
     ) -> None:
@@ -149,15 +149,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/scheduler_config#id DataNomadSchedulerConfig#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scheduler_config#id DataNomadSchedulerConfig#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7084dea75f06f7236849103af5128257940fff820adc8ee844c705fec196dc5b)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -192,20 +192,22 @@
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
@@ -245,15 +247,15 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/scheduler_config#id DataNomadSchedulerConfig#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/scheduler_config#id DataNomadSchedulerConfig#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -278,15 +280,15 @@
 
 def _typecheckingstub__d9bf53f7dd96e9a5d5c48f319514a60c7420b10134bae6d1b025567a9721e8cb(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
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
@@ -297,15 +299,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__7084dea75f06f7236849103af5128257940fff820adc8ee844c705fec196dc5b(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     id: typing.Optional[builtins.str] = None,
 ) -> None:
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_volumes/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/data_nomad_volumes/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_nomad_volumes`
 
-Refer to the Terraform Registory for docs: [`data_nomad_volumes`](https://www.terraform.io/docs/providers/nomad/d/volumes).
+Refer to the Terraform Registory for docs: [`data_nomad_volumes`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/volumes).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,43 +22,43 @@
 
 
 class DataNomadVolumes(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.dataNomadVolumes.DataNomadVolumes",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/d/volumes nomad_volumes}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/volumes nomad_volumes}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: typing.Optional[builtins.str] = None,
         namespace: typing.Optional[builtins.str] = None,
         node_id: typing.Optional[builtins.str] = None,
         plugin_id: typing.Optional[builtins.str] = None,
         type: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/d/volumes nomad_volumes} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/volumes nomad_volumes} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/volumes#id DataNomadVolumes#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param namespace: Volume namespace filter. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/volumes#namespace DataNomadVolumes#namespace}
-        :param node_id: Volume node filter. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/volumes#node_id DataNomadVolumes#node_id}
-        :param plugin_id: Plugin ID filter. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/volumes#plugin_id DataNomadVolumes#plugin_id}
-        :param type: Volume Type (currently only 'csi'). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/volumes#type DataNomadVolumes#type}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/volumes#id DataNomadVolumes#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param namespace: Volume namespace filter. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/volumes#namespace DataNomadVolumes#namespace}
+        :param node_id: Volume node filter. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/volumes#node_id DataNomadVolumes#node_id}
+        :param plugin_id: Plugin ID filter. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/volumes#plugin_id DataNomadVolumes#plugin_id}
+        :param type: Volume Type (currently only 'csi'). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/volumes#type DataNomadVolumes#type}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -223,15 +223,15 @@
     },
 )
 class DataNomadVolumesConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         id: typing.Optional[builtins.str] = None,
         namespace: typing.Optional[builtins.str] = None,
@@ -243,19 +243,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/volumes#id DataNomadVolumes#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param namespace: Volume namespace filter. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/volumes#namespace DataNomadVolumes#namespace}
-        :param node_id: Volume node filter. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/volumes#node_id DataNomadVolumes#node_id}
-        :param plugin_id: Plugin ID filter. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/volumes#plugin_id DataNomadVolumes#plugin_id}
-        :param type: Volume Type (currently only 'csi'). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/volumes#type DataNomadVolumes#type}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/volumes#id DataNomadVolumes#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param namespace: Volume namespace filter. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/volumes#namespace DataNomadVolumes#namespace}
+        :param node_id: Volume node filter. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/volumes#node_id DataNomadVolumes#node_id}
+        :param plugin_id: Plugin ID filter. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/volumes#plugin_id DataNomadVolumes#plugin_id}
+        :param type: Volume Type (currently only 'csi'). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/volumes#type DataNomadVolumes#type}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__27c5bc3ee5c30d37acef2d722fd146b0ae225e4748fcefa8a6cdf43d67bb1a03)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -302,20 +302,22 @@
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
@@ -355,54 +357,54 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/volumes#id DataNomadVolumes#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/volumes#id DataNomadVolumes#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def namespace(self) -> typing.Optional[builtins.str]:
         '''Volume namespace filter.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/volumes#namespace DataNomadVolumes#namespace}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/volumes#namespace DataNomadVolumes#namespace}
         '''
         result = self._values.get("namespace")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def node_id(self) -> typing.Optional[builtins.str]:
         '''Volume node filter.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/volumes#node_id DataNomadVolumes#node_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/volumes#node_id DataNomadVolumes#node_id}
         '''
         result = self._values.get("node_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def plugin_id(self) -> typing.Optional[builtins.str]:
         '''Plugin ID filter.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/volumes#plugin_id DataNomadVolumes#plugin_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/volumes#plugin_id DataNomadVolumes#plugin_id}
         '''
         result = self._values.get("plugin_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
         '''Volume Type (currently only 'csi').
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/d/volumes#type DataNomadVolumes#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/data-sources/volumes#type DataNomadVolumes#type}
         '''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -428,15 +430,15 @@
     *,
     id: typing.Optional[builtins.str] = None,
     namespace: typing.Optional[builtins.str] = None,
     node_id: typing.Optional[builtins.str] = None,
     plugin_id: typing.Optional[builtins.str] = None,
     type: typing.Optional[builtins.str] = None,
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
@@ -471,15 +473,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__27c5bc3ee5c30d37acef2d722fd146b0ae225e4748fcefa8a6cdf43d67bb1a03(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     id: typing.Optional[builtins.str] = None,
     namespace: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/external_volume/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/external_volume/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `nomad_external_volume`
 
-Refer to the Terraform Registory for docs: [`nomad_external_volume`](https://www.terraform.io/docs/providers/nomad/r/external_volume).
+Refer to the Terraform Registory for docs: [`nomad_external_volume`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class ExternalVolume(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.externalVolume.ExternalVolume",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/r/external_volume nomad_external_volume}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume nomad_external_volume}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         capability: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["ExternalVolumeCapability", typing.Dict[builtins.str, typing.Any]]]],
@@ -45,40 +45,40 @@
         namespace: typing.Optional[builtins.str] = None,
         parameters: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         secrets: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         snapshot_id: typing.Optional[builtins.str] = None,
         topology_request: typing.Optional[typing.Union["ExternalVolumeTopologyRequest", typing.Dict[builtins.str, typing.Any]]] = None,
         type: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/r/external_volume nomad_external_volume} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume nomad_external_volume} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param capability: capability block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#capability ExternalVolume#capability}
-        :param name: The display name of the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#name ExternalVolume#name}
-        :param plugin_id: The ID of the CSI plugin that manages this volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#plugin_id ExternalVolume#plugin_id}
-        :param volume_id: The unique ID of the volume, how jobs will refer to the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#volume_id ExternalVolume#volume_id}
-        :param capacity_max: Defines how large the volume can be. The storage provider may return a volume that is smaller than this value. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#capacity_max ExternalVolume#capacity_max}
-        :param capacity_min: Defines how small the volume can be. The storage provider may return a volume that is larger than this value. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#capacity_min ExternalVolume#capacity_min}
-        :param clone_id: The volume ID to clone when creating this volume. Storage provider must support cloning. Conflicts with 'snapshot_id'. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#clone_id ExternalVolume#clone_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#id ExternalVolume#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param mount_options: mount_options block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#mount_options ExternalVolume#mount_options}
-        :param namespace: The namespace in which to create the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#namespace ExternalVolume#namespace}
-        :param parameters: An optional key-value map of strings passed directly to the CSI plugin to configure the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#parameters ExternalVolume#parameters}
-        :param secrets: An optional key-value map of strings used as credentials for publishing and unpublishing volumes. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#secrets ExternalVolume#secrets}
-        :param snapshot_id: The snapshot ID to restore when creating this volume. Storage provider must support snapshots. Conflicts with 'clone_id'. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#snapshot_id ExternalVolume#snapshot_id}
-        :param topology_request: topology_request block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#topology_request ExternalVolume#topology_request}
-        :param type: The type of the volume. Currently, only 'csi' is supported. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#type ExternalVolume#type}
+        :param capability: capability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#capability ExternalVolume#capability}
+        :param name: The display name of the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#name ExternalVolume#name}
+        :param plugin_id: The ID of the CSI plugin that manages this volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#plugin_id ExternalVolume#plugin_id}
+        :param volume_id: The unique ID of the volume, how jobs will refer to the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#volume_id ExternalVolume#volume_id}
+        :param capacity_max: Defines how large the volume can be. The storage provider may return a volume that is smaller than this value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#capacity_max ExternalVolume#capacity_max}
+        :param capacity_min: Defines how small the volume can be. The storage provider may return a volume that is larger than this value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#capacity_min ExternalVolume#capacity_min}
+        :param clone_id: The volume ID to clone when creating this volume. Storage provider must support cloning. Conflicts with 'snapshot_id'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#clone_id ExternalVolume#clone_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#id ExternalVolume#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param mount_options: mount_options block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#mount_options ExternalVolume#mount_options}
+        :param namespace: The namespace in which to create the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#namespace ExternalVolume#namespace}
+        :param parameters: An optional key-value map of strings passed directly to the CSI plugin to configure the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#parameters ExternalVolume#parameters}
+        :param secrets: An optional key-value map of strings used as credentials for publishing and unpublishing volumes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#secrets ExternalVolume#secrets}
+        :param snapshot_id: The snapshot ID to restore when creating this volume. Storage provider must support snapshots. Conflicts with 'clone_id'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#snapshot_id ExternalVolume#snapshot_id}
+        :param topology_request: topology_request block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#topology_request ExternalVolume#topology_request}
+        :param type: The type of the volume. Currently, only 'csi' is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#type ExternalVolume#type}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -131,31 +131,31 @@
     def put_mount_options(
         self,
         *,
         fs_type: typing.Optional[builtins.str] = None,
         mount_flags: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param fs_type: The file system type. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#fs_type ExternalVolume#fs_type}
-        :param mount_flags: The flags passed to mount. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#mount_flags ExternalVolume#mount_flags}
+        :param fs_type: The file system type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#fs_type ExternalVolume#fs_type}
+        :param mount_flags: The flags passed to mount. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#mount_flags ExternalVolume#mount_flags}
         '''
         value = ExternalVolumeMountOptions(fs_type=fs_type, mount_flags=mount_flags)
 
         return typing.cast(None, jsii.invoke(self, "putMountOptions", [value]))
 
     @jsii.member(jsii_name="putTopologyRequest")
     def put_topology_request(
         self,
         *,
         preferred: typing.Optional[typing.Union["ExternalVolumeTopologyRequestPreferred", typing.Dict[builtins.str, typing.Any]]] = None,
         required: typing.Optional[typing.Union["ExternalVolumeTopologyRequestRequired", typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
-        :param preferred: preferred block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#preferred ExternalVolume#preferred}
-        :param required: required block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#required ExternalVolume#required}
+        :param preferred: preferred block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#preferred ExternalVolume#preferred}
+        :param required: required block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#required ExternalVolume#required}
         '''
         value = ExternalVolumeTopologyRequest(preferred=preferred, required=required)
 
         return typing.cast(None, jsii.invoke(self, "putTopologyRequest", [value]))
 
     @jsii.member(jsii_name="resetCapacityMax")
     def reset_capacity_max(self) -> None:
@@ -507,41 +507,41 @@
     def __init__(
         self,
         *,
         access_mode: builtins.str,
         attachment_mode: builtins.str,
     ) -> None:
         '''
-        :param access_mode: Defines whether a volume should be available concurrently. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#access_mode ExternalVolume#access_mode}
-        :param attachment_mode: The storage API that will be used by the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#attachment_mode ExternalVolume#attachment_mode}
+        :param access_mode: Defines whether a volume should be available concurrently. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#access_mode ExternalVolume#access_mode}
+        :param attachment_mode: The storage API that will be used by the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#attachment_mode ExternalVolume#attachment_mode}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__eef56ee2021e0f6b876e4088399075c751c2c52807eec2b390180c9cae5303ba)
             check_type(argname="argument access_mode", value=access_mode, expected_type=type_hints["access_mode"])
             check_type(argname="argument attachment_mode", value=attachment_mode, expected_type=type_hints["attachment_mode"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "access_mode": access_mode,
             "attachment_mode": attachment_mode,
         }
 
     @builtins.property
     def access_mode(self) -> builtins.str:
         '''Defines whether a volume should be available concurrently.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#access_mode ExternalVolume#access_mode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#access_mode ExternalVolume#access_mode}
         '''
         result = self._values.get("access_mode")
         assert result is not None, "Required property 'access_mode' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def attachment_mode(self) -> builtins.str:
         '''The storage API that will be used by the volume.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#attachment_mode ExternalVolume#attachment_mode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#attachment_mode ExternalVolume#attachment_mode}
         '''
         result = self._values.get("attachment_mode")
         assert result is not None, "Required property 'attachment_mode' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -752,15 +752,15 @@
     },
 )
 class ExternalVolumeConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         capability: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[ExternalVolumeCapability, typing.Dict[builtins.str, typing.Any]]]],
         name: builtins.str,
@@ -782,29 +782,29 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param capability: capability block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#capability ExternalVolume#capability}
-        :param name: The display name of the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#name ExternalVolume#name}
-        :param plugin_id: The ID of the CSI plugin that manages this volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#plugin_id ExternalVolume#plugin_id}
-        :param volume_id: The unique ID of the volume, how jobs will refer to the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#volume_id ExternalVolume#volume_id}
-        :param capacity_max: Defines how large the volume can be. The storage provider may return a volume that is smaller than this value. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#capacity_max ExternalVolume#capacity_max}
-        :param capacity_min: Defines how small the volume can be. The storage provider may return a volume that is larger than this value. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#capacity_min ExternalVolume#capacity_min}
-        :param clone_id: The volume ID to clone when creating this volume. Storage provider must support cloning. Conflicts with 'snapshot_id'. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#clone_id ExternalVolume#clone_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#id ExternalVolume#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param mount_options: mount_options block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#mount_options ExternalVolume#mount_options}
-        :param namespace: The namespace in which to create the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#namespace ExternalVolume#namespace}
-        :param parameters: An optional key-value map of strings passed directly to the CSI plugin to configure the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#parameters ExternalVolume#parameters}
-        :param secrets: An optional key-value map of strings used as credentials for publishing and unpublishing volumes. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#secrets ExternalVolume#secrets}
-        :param snapshot_id: The snapshot ID to restore when creating this volume. Storage provider must support snapshots. Conflicts with 'clone_id'. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#snapshot_id ExternalVolume#snapshot_id}
-        :param topology_request: topology_request block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#topology_request ExternalVolume#topology_request}
-        :param type: The type of the volume. Currently, only 'csi' is supported. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#type ExternalVolume#type}
+        :param capability: capability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#capability ExternalVolume#capability}
+        :param name: The display name of the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#name ExternalVolume#name}
+        :param plugin_id: The ID of the CSI plugin that manages this volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#plugin_id ExternalVolume#plugin_id}
+        :param volume_id: The unique ID of the volume, how jobs will refer to the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#volume_id ExternalVolume#volume_id}
+        :param capacity_max: Defines how large the volume can be. The storage provider may return a volume that is smaller than this value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#capacity_max ExternalVolume#capacity_max}
+        :param capacity_min: Defines how small the volume can be. The storage provider may return a volume that is larger than this value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#capacity_min ExternalVolume#capacity_min}
+        :param clone_id: The volume ID to clone when creating this volume. Storage provider must support cloning. Conflicts with 'snapshot_id'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#clone_id ExternalVolume#clone_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#id ExternalVolume#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param mount_options: mount_options block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#mount_options ExternalVolume#mount_options}
+        :param namespace: The namespace in which to create the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#namespace ExternalVolume#namespace}
+        :param parameters: An optional key-value map of strings passed directly to the CSI plugin to configure the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#parameters ExternalVolume#parameters}
+        :param secrets: An optional key-value map of strings used as credentials for publishing and unpublishing volumes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#secrets ExternalVolume#secrets}
+        :param snapshot_id: The snapshot ID to restore when creating this volume. Storage provider must support snapshots. Conflicts with 'clone_id'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#snapshot_id ExternalVolume#snapshot_id}
+        :param topology_request: topology_request block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#topology_request ExternalVolume#topology_request}
+        :param type: The type of the volume. Currently, only 'csi' is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#type ExternalVolume#type}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(mount_options, dict):
             mount_options = ExternalVolumeMountOptions(**mount_options)
         if isinstance(topology_request, dict):
             topology_request = ExternalVolumeTopologyRequest(**topology_request)
@@ -882,20 +882,22 @@
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
@@ -939,150 +941,150 @@
 
     @builtins.property
     def capability(
         self,
     ) -> typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[ExternalVolumeCapability]]:
         '''capability block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#capability ExternalVolume#capability}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#capability ExternalVolume#capability}
         '''
         result = self._values.get("capability")
         assert result is not None, "Required property 'capability' is missing"
         return typing.cast(typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[ExternalVolumeCapability]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The display name of the volume.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#name ExternalVolume#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#name ExternalVolume#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def plugin_id(self) -> builtins.str:
         '''The ID of the CSI plugin that manages this volume.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#plugin_id ExternalVolume#plugin_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#plugin_id ExternalVolume#plugin_id}
         '''
         result = self._values.get("plugin_id")
         assert result is not None, "Required property 'plugin_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def volume_id(self) -> builtins.str:
         '''The unique ID of the volume, how jobs will refer to the volume.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#volume_id ExternalVolume#volume_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#volume_id ExternalVolume#volume_id}
         '''
         result = self._values.get("volume_id")
         assert result is not None, "Required property 'volume_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def capacity_max(self) -> typing.Optional[builtins.str]:
         '''Defines how large the volume can be.
 
         The storage provider may return a volume that is smaller than this value.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#capacity_max ExternalVolume#capacity_max}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#capacity_max ExternalVolume#capacity_max}
         '''
         result = self._values.get("capacity_max")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def capacity_min(self) -> typing.Optional[builtins.str]:
         '''Defines how small the volume can be.
 
         The storage provider may return a volume that is larger than this value.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#capacity_min ExternalVolume#capacity_min}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#capacity_min ExternalVolume#capacity_min}
         '''
         result = self._values.get("capacity_min")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def clone_id(self) -> typing.Optional[builtins.str]:
         '''The volume ID to clone when creating this volume. Storage provider must support cloning. Conflicts with 'snapshot_id'.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#clone_id ExternalVolume#clone_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#clone_id ExternalVolume#clone_id}
         '''
         result = self._values.get("clone_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#id ExternalVolume#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#id ExternalVolume#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def mount_options(self) -> typing.Optional["ExternalVolumeMountOptions"]:
         '''mount_options block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#mount_options ExternalVolume#mount_options}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#mount_options ExternalVolume#mount_options}
         '''
         result = self._values.get("mount_options")
         return typing.cast(typing.Optional["ExternalVolumeMountOptions"], result)
 
     @builtins.property
     def namespace(self) -> typing.Optional[builtins.str]:
         '''The namespace in which to create the volume.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#namespace ExternalVolume#namespace}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#namespace ExternalVolume#namespace}
         '''
         result = self._values.get("namespace")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def parameters(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#parameters ExternalVolume#parameters}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#parameters ExternalVolume#parameters}
         '''
         result = self._values.get("parameters")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def secrets(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#secrets ExternalVolume#secrets}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#secrets ExternalVolume#secrets}
         '''
         result = self._values.get("secrets")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def snapshot_id(self) -> typing.Optional[builtins.str]:
         '''The snapshot ID to restore when creating this volume. Storage provider must support snapshots. Conflicts with 'clone_id'.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#snapshot_id ExternalVolume#snapshot_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#snapshot_id ExternalVolume#snapshot_id}
         '''
         result = self._values.get("snapshot_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def topology_request(self) -> typing.Optional["ExternalVolumeTopologyRequest"]:
         '''topology_request block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#topology_request ExternalVolume#topology_request}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#topology_request ExternalVolume#topology_request}
         '''
         result = self._values.get("topology_request")
         return typing.cast(typing.Optional["ExternalVolumeTopologyRequest"], result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
         '''The type of the volume. Currently, only 'csi' is supported.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#type ExternalVolume#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#type ExternalVolume#type}
         '''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1104,16 +1106,16 @@
     def __init__(
         self,
         *,
         fs_type: typing.Optional[builtins.str] = None,
         mount_flags: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param fs_type: The file system type. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#fs_type ExternalVolume#fs_type}
-        :param mount_flags: The flags passed to mount. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#mount_flags ExternalVolume#mount_flags}
+        :param fs_type: The file system type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#fs_type ExternalVolume#fs_type}
+        :param mount_flags: The flags passed to mount. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#mount_flags ExternalVolume#mount_flags}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cae5722437a1cfcfaa567da19c8e0e2145693d4846fd79bff0dd3deb4c599539)
             check_type(argname="argument fs_type", value=fs_type, expected_type=type_hints["fs_type"])
             check_type(argname="argument mount_flags", value=mount_flags, expected_type=type_hints["mount_flags"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if fs_type is not None:
@@ -1121,24 +1123,24 @@
         if mount_flags is not None:
             self._values["mount_flags"] = mount_flags
 
     @builtins.property
     def fs_type(self) -> typing.Optional[builtins.str]:
         '''The file system type.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#fs_type ExternalVolume#fs_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#fs_type ExternalVolume#fs_type}
         '''
         result = self._values.get("fs_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def mount_flags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The flags passed to mount.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#mount_flags ExternalVolume#mount_flags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#mount_flags ExternalVolume#mount_flags}
         '''
         result = self._values.get("mount_flags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1376,16 +1378,16 @@
     def __init__(
         self,
         *,
         preferred: typing.Optional[typing.Union["ExternalVolumeTopologyRequestPreferred", typing.Dict[builtins.str, typing.Any]]] = None,
         required: typing.Optional[typing.Union["ExternalVolumeTopologyRequestRequired", typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
-        :param preferred: preferred block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#preferred ExternalVolume#preferred}
-        :param required: required block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#required ExternalVolume#required}
+        :param preferred: preferred block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#preferred ExternalVolume#preferred}
+        :param required: required block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#required ExternalVolume#required}
         '''
         if isinstance(preferred, dict):
             preferred = ExternalVolumeTopologyRequestPreferred(**preferred)
         if isinstance(required, dict):
             required = ExternalVolumeTopologyRequestRequired(**required)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ef1b6ead6360f02853486c7deb75cccaae2e27685d9367fc7e90d66274b1451e)
@@ -1397,24 +1399,24 @@
         if required is not None:
             self._values["required"] = required
 
     @builtins.property
     def preferred(self) -> typing.Optional["ExternalVolumeTopologyRequestPreferred"]:
         '''preferred block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#preferred ExternalVolume#preferred}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#preferred ExternalVolume#preferred}
         '''
         result = self._values.get("preferred")
         return typing.cast(typing.Optional["ExternalVolumeTopologyRequestPreferred"], result)
 
     @builtins.property
     def required(self) -> typing.Optional["ExternalVolumeTopologyRequestRequired"]:
         '''required block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#required ExternalVolume#required}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#required ExternalVolume#required}
         '''
         result = self._values.get("required")
         return typing.cast(typing.Optional["ExternalVolumeTopologyRequestRequired"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1450,28 +1452,28 @@
     @jsii.member(jsii_name="putPreferred")
     def put_preferred(
         self,
         *,
         topology: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["ExternalVolumeTopologyRequestPreferredTopology", typing.Dict[builtins.str, typing.Any]]]],
     ) -> None:
         '''
-        :param topology: topology block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#topology ExternalVolume#topology}
+        :param topology: topology block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#topology ExternalVolume#topology}
         '''
         value = ExternalVolumeTopologyRequestPreferred(topology=topology)
 
         return typing.cast(None, jsii.invoke(self, "putPreferred", [value]))
 
     @jsii.member(jsii_name="putRequired")
     def put_required(
         self,
         *,
         topology: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["ExternalVolumeTopologyRequestRequiredTopology", typing.Dict[builtins.str, typing.Any]]]],
     ) -> None:
         '''
-        :param topology: topology block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#topology ExternalVolume#topology}
+        :param topology: topology block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#topology ExternalVolume#topology}
         '''
         value = ExternalVolumeTopologyRequestRequired(topology=topology)
 
         return typing.cast(None, jsii.invoke(self, "putRequired", [value]))
 
     @jsii.member(jsii_name="resetPreferred")
     def reset_preferred(self) -> None:
@@ -1529,30 +1531,30 @@
 class ExternalVolumeTopologyRequestPreferred:
     def __init__(
         self,
         *,
         topology: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["ExternalVolumeTopologyRequestPreferredTopology", typing.Dict[builtins.str, typing.Any]]]],
     ) -> None:
         '''
-        :param topology: topology block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#topology ExternalVolume#topology}
+        :param topology: topology block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#topology ExternalVolume#topology}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c616ba5dc0196f03bfd1c72737cb2901e2b87697e063c7b78149dc628622b834)
             check_type(argname="argument topology", value=topology, expected_type=type_hints["topology"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "topology": topology,
         }
 
     @builtins.property
     def topology(
         self,
     ) -> typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ExternalVolumeTopologyRequestPreferredTopology"]]:
         '''topology block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#topology ExternalVolume#topology}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#topology ExternalVolume#topology}
         '''
         result = self._values.get("topology")
         assert result is not None, "Required property 'topology' is missing"
         return typing.cast(typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ExternalVolumeTopologyRequestPreferredTopology"]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -1631,28 +1633,28 @@
     jsii_type="@cdktf/provider-nomad.externalVolume.ExternalVolumeTopologyRequestPreferredTopology",
     jsii_struct_bases=[],
     name_mapping={"segments": "segments"},
 )
 class ExternalVolumeTopologyRequestPreferredTopology:
     def __init__(self, *, segments: typing.Mapping[builtins.str, builtins.str]) -> None:
         '''
-        :param segments: Define the attributes for the topology request. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#segments ExternalVolume#segments}
+        :param segments: Define the attributes for the topology request. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#segments ExternalVolume#segments}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5d674a9a46dee127dbe9c0207fe6d4794cda9b6448fcb4d1e51c9a69b10e9323)
             check_type(argname="argument segments", value=segments, expected_type=type_hints["segments"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "segments": segments,
         }
 
     @builtins.property
     def segments(self) -> typing.Mapping[builtins.str, builtins.str]:
         '''Define the attributes for the topology request.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#segments ExternalVolume#segments}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#segments ExternalVolume#segments}
         '''
         result = self._values.get("segments")
         assert result is not None, "Required property 'segments' is missing"
         return typing.cast(typing.Mapping[builtins.str, builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -1830,30 +1832,30 @@
 class ExternalVolumeTopologyRequestRequired:
     def __init__(
         self,
         *,
         topology: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["ExternalVolumeTopologyRequestRequiredTopology", typing.Dict[builtins.str, typing.Any]]]],
     ) -> None:
         '''
-        :param topology: topology block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#topology ExternalVolume#topology}
+        :param topology: topology block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#topology ExternalVolume#topology}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__52be38be32d7d459be054e61bd9a9b9bc78006d5d7882c83e29057eec38c296a)
             check_type(argname="argument topology", value=topology, expected_type=type_hints["topology"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "topology": topology,
         }
 
     @builtins.property
     def topology(
         self,
     ) -> typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ExternalVolumeTopologyRequestRequiredTopology"]]:
         '''topology block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#topology ExternalVolume#topology}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#topology ExternalVolume#topology}
         '''
         result = self._values.get("topology")
         assert result is not None, "Required property 'topology' is missing"
         return typing.cast(typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ExternalVolumeTopologyRequestRequiredTopology"]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -1932,28 +1934,28 @@
     jsii_type="@cdktf/provider-nomad.externalVolume.ExternalVolumeTopologyRequestRequiredTopology",
     jsii_struct_bases=[],
     name_mapping={"segments": "segments"},
 )
 class ExternalVolumeTopologyRequestRequiredTopology:
     def __init__(self, *, segments: typing.Mapping[builtins.str, builtins.str]) -> None:
         '''
-        :param segments: Define the attributes for the topology request. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#segments ExternalVolume#segments}
+        :param segments: Define the attributes for the topology request. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#segments ExternalVolume#segments}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__72f2114a9abbe766b99886b0f86178779fc416a5e2faa2a5cc77252daf54c6f5)
             check_type(argname="argument segments", value=segments, expected_type=type_hints["segments"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "segments": segments,
         }
 
     @builtins.property
     def segments(self) -> typing.Mapping[builtins.str, builtins.str]:
         '''Define the attributes for the topology request.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/external_volume#segments ExternalVolume#segments}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/external_volume#segments ExternalVolume#segments}
         '''
         result = self._values.get("segments")
         assert result is not None, "Required property 'segments' is missing"
         return typing.cast(typing.Mapping[builtins.str, builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -2166,15 +2168,15 @@
     namespace: typing.Optional[builtins.str] = None,
     parameters: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     secrets: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     snapshot_id: typing.Optional[builtins.str] = None,
     topology_request: typing.Optional[typing.Union[ExternalVolumeTopologyRequest, typing.Dict[builtins.str, typing.Any]]] = None,
     type: typing.Optional[builtins.str] = None,
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
@@ -2330,15 +2332,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__9b7e1ab3b5b3e528078e47a1078a3235f757c4ded1c3e28f98f2bf52b3c6ce05(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     capability: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[ExternalVolumeCapability, typing.Dict[builtins.str, typing.Any]]]],
     name: builtins.str,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/job/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/job/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `nomad_job`
 
-Refer to the Terraform Registory for docs: [`nomad_job`](https://www.terraform.io/docs/providers/nomad/r/job).
+Refer to the Terraform Registory for docs: [`nomad_job`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Job(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.job.Job",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/r/job nomad_job}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job nomad_job}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         jobspec: builtins.str,
@@ -42,37 +42,37 @@
         id: typing.Optional[builtins.str] = None,
         json: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         policy_override: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         purge_on_destroy: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         timeouts: typing.Optional[typing.Union["JobTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         vault_token: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/r/job nomad_job} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job nomad_job} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param jobspec: Job specification. If you want to point to a file use the file() function. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#jobspec Job#jobspec}
-        :param consul_token: The Consul token used to submit this job. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#consul_token Job#consul_token}
-        :param deregister_on_destroy: If true, the job will be deregistered on destroy. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#deregister_on_destroy Job#deregister_on_destroy}
-        :param deregister_on_id_change: If true, the job will be deregistered when the job ID changes. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#deregister_on_id_change Job#deregister_on_id_change}
-        :param detach: If true, the provider will return immediately after creating or updating, instead of monitoring. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#detach Job#detach}
-        :param hcl2: hcl2 block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#hcl2 Job#hcl2}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#id Job#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param json: If true, the ``jobspec`` will be parsed as json instead of HCL. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#json Job#json}
-        :param policy_override: Override any soft-mandatory Sentinel policies that fail. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#policy_override Job#policy_override}
-        :param purge_on_destroy: Whether to purge the job when the resource is destroyed. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#purge_on_destroy Job#purge_on_destroy}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#timeouts Job#timeouts}
-        :param vault_token: The Vault token used to submit this job. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#vault_token Job#vault_token}
+        :param jobspec: Job specification. If you want to point to a file use the file() function. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#jobspec Job#jobspec}
+        :param consul_token: The Consul token used to submit this job. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#consul_token Job#consul_token}
+        :param deregister_on_destroy: If true, the job will be deregistered on destroy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#deregister_on_destroy Job#deregister_on_destroy}
+        :param deregister_on_id_change: If true, the job will be deregistered when the job ID changes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#deregister_on_id_change Job#deregister_on_id_change}
+        :param detach: If true, the provider will return immediately after creating or updating, instead of monitoring. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#detach Job#detach}
+        :param hcl2: hcl2 block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#hcl2 Job#hcl2}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#id Job#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param json: If true, the ``jobspec`` will be parsed as json instead of HCL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#json Job#json}
+        :param policy_override: Override any soft-mandatory Sentinel policies that fail. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#policy_override Job#policy_override}
+        :param purge_on_destroy: Whether to purge the job when the resource is destroyed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#purge_on_destroy Job#purge_on_destroy}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#timeouts Job#timeouts}
+        :param vault_token: The Vault token used to submit this job. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#vault_token Job#vault_token}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -110,32 +110,32 @@
         self,
         *,
         allow_fs: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         enabled: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         vars: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     ) -> None:
         '''
-        :param allow_fs: If true, HCL2 file system functions will be enabled when parsing the ``jobspec``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#allow_fs Job#allow_fs}
-        :param enabled: If true, the ``jobspec`` will be parsed as HCL2 instead of HCL. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#enabled Job#enabled}
-        :param vars: Additional variables to use when templating the job with HCL2. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#vars Job#vars}
+        :param allow_fs: If true, HCL2 file system functions will be enabled when parsing the ``jobspec``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#allow_fs Job#allow_fs}
+        :param enabled: If true, the ``jobspec`` will be parsed as HCL2 instead of HCL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#enabled Job#enabled}
+        :param vars: Additional variables to use when templating the job with HCL2. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#vars Job#vars}
         '''
         value = JobHcl2(allow_fs=allow_fs, enabled=enabled, vars=vars)
 
         return typing.cast(None, jsii.invoke(self, "putHcl2", [value]))
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#create Job#create}.
-        :param update: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#update Job#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#create Job#create}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#update Job#update}.
         '''
         value = JobTimeouts(create=create, update=update)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetConsulToken")
     def reset_consul_token(self) -> None:
@@ -497,15 +497,15 @@
     },
 )
 class JobConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         jobspec: builtins.str,
         consul_token: typing.Optional[builtins.str] = None,
@@ -524,26 +524,26 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param jobspec: Job specification. If you want to point to a file use the file() function. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#jobspec Job#jobspec}
-        :param consul_token: The Consul token used to submit this job. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#consul_token Job#consul_token}
-        :param deregister_on_destroy: If true, the job will be deregistered on destroy. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#deregister_on_destroy Job#deregister_on_destroy}
-        :param deregister_on_id_change: If true, the job will be deregistered when the job ID changes. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#deregister_on_id_change Job#deregister_on_id_change}
-        :param detach: If true, the provider will return immediately after creating or updating, instead of monitoring. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#detach Job#detach}
-        :param hcl2: hcl2 block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#hcl2 Job#hcl2}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#id Job#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param json: If true, the ``jobspec`` will be parsed as json instead of HCL. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#json Job#json}
-        :param policy_override: Override any soft-mandatory Sentinel policies that fail. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#policy_override Job#policy_override}
-        :param purge_on_destroy: Whether to purge the job when the resource is destroyed. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#purge_on_destroy Job#purge_on_destroy}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#timeouts Job#timeouts}
-        :param vault_token: The Vault token used to submit this job. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#vault_token Job#vault_token}
+        :param jobspec: Job specification. If you want to point to a file use the file() function. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#jobspec Job#jobspec}
+        :param consul_token: The Consul token used to submit this job. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#consul_token Job#consul_token}
+        :param deregister_on_destroy: If true, the job will be deregistered on destroy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#deregister_on_destroy Job#deregister_on_destroy}
+        :param deregister_on_id_change: If true, the job will be deregistered when the job ID changes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#deregister_on_id_change Job#deregister_on_id_change}
+        :param detach: If true, the provider will return immediately after creating or updating, instead of monitoring. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#detach Job#detach}
+        :param hcl2: hcl2 block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#hcl2 Job#hcl2}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#id Job#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param json: If true, the ``jobspec`` will be parsed as json instead of HCL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#json Job#json}
+        :param policy_override: Override any soft-mandatory Sentinel policies that fail. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#policy_override Job#policy_override}
+        :param purge_on_destroy: Whether to purge the job when the resource is destroyed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#purge_on_destroy Job#purge_on_destroy}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#timeouts Job#timeouts}
+        :param vault_token: The Vault token used to submit this job. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#vault_token Job#vault_token}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(hcl2, dict):
             hcl2 = JobHcl2(**hcl2)
         if isinstance(timeouts, dict):
             timeouts = JobTimeouts(**timeouts)
@@ -615,20 +615,22 @@
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
@@ -670,128 +672,128 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def jobspec(self) -> builtins.str:
         '''Job specification. If you want to point to a file use the file() function.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#jobspec Job#jobspec}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#jobspec Job#jobspec}
         '''
         result = self._values.get("jobspec")
         assert result is not None, "Required property 'jobspec' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def consul_token(self) -> typing.Optional[builtins.str]:
         '''The Consul token used to submit this job.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#consul_token Job#consul_token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#consul_token Job#consul_token}
         '''
         result = self._values.get("consul_token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def deregister_on_destroy(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If true, the job will be deregistered on destroy.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#deregister_on_destroy Job#deregister_on_destroy}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#deregister_on_destroy Job#deregister_on_destroy}
         '''
         result = self._values.get("deregister_on_destroy")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def deregister_on_id_change(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If true, the job will be deregistered when the job ID changes.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#deregister_on_id_change Job#deregister_on_id_change}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#deregister_on_id_change Job#deregister_on_id_change}
         '''
         result = self._values.get("deregister_on_id_change")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def detach(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If true, the provider will return immediately after creating or updating, instead of monitoring.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#detach Job#detach}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#detach Job#detach}
         '''
         result = self._values.get("detach")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def hcl2(self) -> typing.Optional["JobHcl2"]:
         '''hcl2 block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#hcl2 Job#hcl2}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#hcl2 Job#hcl2}
         '''
         result = self._values.get("hcl2")
         return typing.cast(typing.Optional["JobHcl2"], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#id Job#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#id Job#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def json(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If true, the ``jobspec`` will be parsed as json instead of HCL.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#json Job#json}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#json Job#json}
         '''
         result = self._values.get("json")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def policy_override(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Override any soft-mandatory Sentinel policies that fail.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#policy_override Job#policy_override}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#policy_override Job#policy_override}
         '''
         result = self._values.get("policy_override")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def purge_on_destroy(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether to purge the job when the resource is destroyed.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#purge_on_destroy Job#purge_on_destroy}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#purge_on_destroy Job#purge_on_destroy}
         '''
         result = self._values.get("purge_on_destroy")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["JobTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#timeouts Job#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#timeouts Job#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["JobTimeouts"], result)
 
     @builtins.property
     def vault_token(self) -> typing.Optional[builtins.str]:
         '''The Vault token used to submit this job.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#vault_token Job#vault_token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#vault_token Job#vault_token}
         '''
         result = self._values.get("vault_token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -814,17 +816,17 @@
         self,
         *,
         allow_fs: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         enabled: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         vars: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     ) -> None:
         '''
-        :param allow_fs: If true, HCL2 file system functions will be enabled when parsing the ``jobspec``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#allow_fs Job#allow_fs}
-        :param enabled: If true, the ``jobspec`` will be parsed as HCL2 instead of HCL. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#enabled Job#enabled}
-        :param vars: Additional variables to use when templating the job with HCL2. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#vars Job#vars}
+        :param allow_fs: If true, HCL2 file system functions will be enabled when parsing the ``jobspec``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#allow_fs Job#allow_fs}
+        :param enabled: If true, the ``jobspec`` will be parsed as HCL2 instead of HCL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#enabled Job#enabled}
+        :param vars: Additional variables to use when templating the job with HCL2. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#vars Job#vars}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__00bd4c654c786dcc73121f9f1442771d83e52e3edaefba4adf383affd6577100)
             check_type(argname="argument allow_fs", value=allow_fs, expected_type=type_hints["allow_fs"])
             check_type(argname="argument enabled", value=enabled, expected_type=type_hints["enabled"])
             check_type(argname="argument vars", value=vars, expected_type=type_hints["vars"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -837,35 +839,35 @@
 
     @builtins.property
     def allow_fs(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If true, HCL2 file system functions will be enabled when parsing the ``jobspec``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#allow_fs Job#allow_fs}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#allow_fs Job#allow_fs}
         '''
         result = self._values.get("allow_fs")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If true, the ``jobspec`` will be parsed as HCL2 instead of HCL.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#enabled Job#enabled}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#enabled Job#enabled}
         '''
         result = self._values.get("enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def vars(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''Additional variables to use when templating the job with HCL2.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#vars Job#vars}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#vars Job#vars}
         '''
         result = self._values.get("vars")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1608,36 +1610,36 @@
     def __init__(
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#create Job#create}.
-        :param update: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#update Job#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#create Job#create}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#update Job#update}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__80fdd78a4b76365a4ff7e85aea94e40ea25256faa32e8e589a49bb86705cfab2)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument update", value=update, expected_type=type_hints["update"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if create is not None:
             self._values["create"] = create
         if update is not None:
             self._values["update"] = update
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#create Job#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#create Job#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def update(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/job#update Job#update}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/job#update Job#update}.'''
         result = self._values.get("update")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -1765,15 +1767,15 @@
     id: typing.Optional[builtins.str] = None,
     json: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     policy_override: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     purge_on_destroy: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     timeouts: typing.Optional[typing.Union[JobTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
     vault_token: typing.Optional[builtins.str] = None,
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
@@ -1838,15 +1840,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__37af447459ed11d3aaa370e639e90e5dbccbaa7ec090fc274ebbf6a048d1f698(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     jobspec: builtins.str,
     consul_token: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/namespace/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/namespace/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `nomad_namespace`
 
-Refer to the Terraform Registory for docs: [`nomad_namespace`](https://www.terraform.io/docs/providers/nomad/r/namespace).
+Refer to the Terraform Registory for docs: [`nomad_namespace`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,45 +22,45 @@
 
 
 class Namespace(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.namespace.Namespace",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/r/namespace nomad_namespace}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace nomad_namespace}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
         capabilities: typing.Optional[typing.Union["NamespaceCapabilities", typing.Dict[builtins.str, typing.Any]]] = None,
         description: typing.Optional[builtins.str] = None,
         id: typing.Optional[builtins.str] = None,
         meta: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         quota: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/r/namespace nomad_namespace} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace nomad_namespace} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Unique name for this namespace. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#name Namespace#name}
-        :param capabilities: capabilities block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#capabilities Namespace#capabilities}
-        :param description: Description for this namespace. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#description Namespace#description}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#id Namespace#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param meta: Metadata associated with the namespace. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#meta Namespace#meta}
-        :param quota: Quota to set for this namespace. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#quota Namespace#quota}
+        :param name: Unique name for this namespace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#name Namespace#name}
+        :param capabilities: capabilities block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#capabilities Namespace#capabilities}
+        :param description: Description for this namespace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#description Namespace#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#id Namespace#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param meta: Metadata associated with the namespace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#meta Namespace#meta}
+        :param quota: Quota to set for this namespace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#quota Namespace#quota}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -91,16 +91,16 @@
     def put_capabilities(
         self,
         *,
         disabled_task_drivers: typing.Optional[typing.Sequence[builtins.str]] = None,
         enabled_task_drivers: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param disabled_task_drivers: Disabled task drivers for the namespace. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#disabled_task_drivers Namespace#disabled_task_drivers}
-        :param enabled_task_drivers: Enabled task drivers for the namespace. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#enabled_task_drivers Namespace#enabled_task_drivers}
+        :param disabled_task_drivers: Disabled task drivers for the namespace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#disabled_task_drivers Namespace#disabled_task_drivers}
+        :param enabled_task_drivers: Enabled task drivers for the namespace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#enabled_task_drivers Namespace#enabled_task_drivers}
         '''
         value = NamespaceCapabilities(
             disabled_task_drivers=disabled_task_drivers,
             enabled_task_drivers=enabled_task_drivers,
         )
 
         return typing.cast(None, jsii.invoke(self, "putCapabilities", [value]))
@@ -242,16 +242,16 @@
     def __init__(
         self,
         *,
         disabled_task_drivers: typing.Optional[typing.Sequence[builtins.str]] = None,
         enabled_task_drivers: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param disabled_task_drivers: Disabled task drivers for the namespace. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#disabled_task_drivers Namespace#disabled_task_drivers}
-        :param enabled_task_drivers: Enabled task drivers for the namespace. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#enabled_task_drivers Namespace#enabled_task_drivers}
+        :param disabled_task_drivers: Disabled task drivers for the namespace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#disabled_task_drivers Namespace#disabled_task_drivers}
+        :param enabled_task_drivers: Enabled task drivers for the namespace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#enabled_task_drivers Namespace#enabled_task_drivers}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a3379bc61ce22be5e8f5f099b1c0b081234e86c61100cda567dba8e72745663b)
             check_type(argname="argument disabled_task_drivers", value=disabled_task_drivers, expected_type=type_hints["disabled_task_drivers"])
             check_type(argname="argument enabled_task_drivers", value=enabled_task_drivers, expected_type=type_hints["enabled_task_drivers"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if disabled_task_drivers is not None:
@@ -259,24 +259,24 @@
         if enabled_task_drivers is not None:
             self._values["enabled_task_drivers"] = enabled_task_drivers
 
     @builtins.property
     def disabled_task_drivers(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Disabled task drivers for the namespace.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#disabled_task_drivers Namespace#disabled_task_drivers}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#disabled_task_drivers Namespace#disabled_task_drivers}
         '''
         result = self._values.get("disabled_task_drivers")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def enabled_task_drivers(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Enabled task drivers for the namespace.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#enabled_task_drivers Namespace#enabled_task_drivers}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#enabled_task_drivers Namespace#enabled_task_drivers}
         '''
         result = self._values.get("enabled_task_drivers")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -384,15 +384,15 @@
     },
 )
 class NamespaceConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         capabilities: typing.Optional[typing.Union[NamespaceCapabilities, typing.Dict[builtins.str, typing.Any]]] = None,
@@ -405,20 +405,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Unique name for this namespace. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#name Namespace#name}
-        :param capabilities: capabilities block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#capabilities Namespace#capabilities}
-        :param description: Description for this namespace. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#description Namespace#description}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#id Namespace#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param meta: Metadata associated with the namespace. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#meta Namespace#meta}
-        :param quota: Quota to set for this namespace. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#quota Namespace#quota}
+        :param name: Unique name for this namespace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#name Namespace#name}
+        :param capabilities: capabilities block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#capabilities Namespace#capabilities}
+        :param description: Description for this namespace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#description Namespace#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#id Namespace#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param meta: Metadata associated with the namespace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#meta Namespace#meta}
+        :param quota: Quota to set for this namespace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#quota Namespace#quota}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(capabilities, dict):
             capabilities = NamespaceCapabilities(**capabilities)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a81352aa4fd2f5d9a2d30390572fa3baecc6fbd2f02319884c8eccc39bcb5e2e)
@@ -470,20 +470,22 @@
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
@@ -525,62 +527,62 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''Unique name for this namespace.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#name Namespace#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#name Namespace#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def capabilities(self) -> typing.Optional[NamespaceCapabilities]:
         '''capabilities block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#capabilities Namespace#capabilities}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#capabilities Namespace#capabilities}
         '''
         result = self._values.get("capabilities")
         return typing.cast(typing.Optional[NamespaceCapabilities], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''Description for this namespace.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#description Namespace#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#description Namespace#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#id Namespace#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#id Namespace#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def meta(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''Metadata associated with the namespace.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#meta Namespace#meta}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#meta Namespace#meta}
         '''
         result = self._values.get("meta")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def quota(self) -> typing.Optional[builtins.str]:
         '''Quota to set for this namespace.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/namespace#quota Namespace#quota}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/namespace#quota Namespace#quota}
         '''
         result = self._values.get("quota")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -609,15 +611,15 @@
     name: builtins.str,
     capabilities: typing.Optional[typing.Union[NamespaceCapabilities, typing.Dict[builtins.str, typing.Any]]] = None,
     description: typing.Optional[builtins.str] = None,
     id: typing.Optional[builtins.str] = None,
     meta: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     quota: typing.Optional[builtins.str] = None,
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
@@ -685,15 +687,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__a81352aa4fd2f5d9a2d30390572fa3baecc6fbd2f02319884c8eccc39bcb5e2e(
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
     capabilities: typing.Optional[typing.Union[NamespaceCapabilities, typing.Dict[builtins.str, typing.Any]]] = None,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/provider/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/provider/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`nomad`](https://www.terraform.io/docs/providers/nomad).
+Refer to the Terraform Registory for docs: [`nomad`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class NomadProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.provider.NomadProvider",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad nomad}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs nomad}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         address: builtins.str,
@@ -45,33 +45,33 @@
         ignore_env_vars: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]] = None,
         key_file: typing.Optional[builtins.str] = None,
         key_pem: typing.Optional[builtins.str] = None,
         region: typing.Optional[builtins.str] = None,
         secret_id: typing.Optional[builtins.str] = None,
         vault_token: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad nomad} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs nomad} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param address: URL of the root of the target Nomad agent. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#address NomadProvider#address}
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#alias NomadProvider#alias}
-        :param ca_file: A path to a PEM-encoded certificate authority used to verify the remote agent's certificate. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#ca_file NomadProvider#ca_file}
-        :param ca_pem: PEM-encoded certificate authority used to verify the remote agent's certificate. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#ca_pem NomadProvider#ca_pem}
-        :param cert_file: A path to a PEM-encoded certificate provided to the remote agent; requires use of key_file or key_pem. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#cert_file NomadProvider#cert_file}
-        :param cert_pem: PEM-encoded certificate provided to the remote agent; requires use of key_file or key_pem. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#cert_pem NomadProvider#cert_pem}
-        :param consul_token: Consul token to validate Consul Connect Service Identity policies specified in the job file. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#consul_token NomadProvider#consul_token}
-        :param headers: headers block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#headers NomadProvider#headers}
-        :param http_auth: HTTP basic auth configuration. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#http_auth NomadProvider#http_auth}
-        :param ignore_env_vars: A set of environment variables that are ignored by the provider when configuring the Nomad API client. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#ignore_env_vars NomadProvider#ignore_env_vars}
-        :param key_file: A path to a PEM-encoded private key, required if cert_file or cert_pem is specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#key_file NomadProvider#key_file}
-        :param key_pem: PEM-encoded private key, required if cert_file or cert_pem is specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#key_pem NomadProvider#key_pem}
-        :param region: Region of the target Nomad agent. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#region NomadProvider#region}
-        :param secret_id: ACL token secret for API requests. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#secret_id NomadProvider#secret_id}
-        :param vault_token: Vault token if policies are specified in the job file. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#vault_token NomadProvider#vault_token}
+        :param address: URL of the root of the target Nomad agent. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#address NomadProvider#address}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#alias NomadProvider#alias}
+        :param ca_file: A path to a PEM-encoded certificate authority used to verify the remote agent's certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#ca_file NomadProvider#ca_file}
+        :param ca_pem: PEM-encoded certificate authority used to verify the remote agent's certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#ca_pem NomadProvider#ca_pem}
+        :param cert_file: A path to a PEM-encoded certificate provided to the remote agent; requires use of key_file or key_pem. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#cert_file NomadProvider#cert_file}
+        :param cert_pem: PEM-encoded certificate provided to the remote agent; requires use of key_file or key_pem. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#cert_pem NomadProvider#cert_pem}
+        :param consul_token: Consul token to validate Consul Connect Service Identity policies specified in the job file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#consul_token NomadProvider#consul_token}
+        :param headers: headers block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#headers NomadProvider#headers}
+        :param http_auth: HTTP basic auth configuration. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#http_auth NomadProvider#http_auth}
+        :param ignore_env_vars: A set of environment variables that are ignored by the provider when configuring the Nomad API client. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#ignore_env_vars NomadProvider#ignore_env_vars}
+        :param key_file: A path to a PEM-encoded private key, required if cert_file or cert_pem is specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#key_file NomadProvider#key_file}
+        :param key_pem: PEM-encoded private key, required if cert_file or cert_pem is specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#key_pem NomadProvider#key_pem}
+        :param region: Region of the target Nomad agent. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#region NomadProvider#region}
+        :param secret_id: ACL token secret for API requests. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#secret_id NomadProvider#secret_id}
+        :param vault_token: Vault token if policies are specified in the job file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#vault_token NomadProvider#vault_token}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__fa1135b3e0a6e5d3f7edfef684226a9a3ae7c144ae366e8b37d5ae425d916fff)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = NomadProviderConfig(
             address=address,
@@ -466,29 +466,29 @@
         key_file: typing.Optional[builtins.str] = None,
         key_pem: typing.Optional[builtins.str] = None,
         region: typing.Optional[builtins.str] = None,
         secret_id: typing.Optional[builtins.str] = None,
         vault_token: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param address: URL of the root of the target Nomad agent. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#address NomadProvider#address}
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#alias NomadProvider#alias}
-        :param ca_file: A path to a PEM-encoded certificate authority used to verify the remote agent's certificate. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#ca_file NomadProvider#ca_file}
-        :param ca_pem: PEM-encoded certificate authority used to verify the remote agent's certificate. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#ca_pem NomadProvider#ca_pem}
-        :param cert_file: A path to a PEM-encoded certificate provided to the remote agent; requires use of key_file or key_pem. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#cert_file NomadProvider#cert_file}
-        :param cert_pem: PEM-encoded certificate provided to the remote agent; requires use of key_file or key_pem. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#cert_pem NomadProvider#cert_pem}
-        :param consul_token: Consul token to validate Consul Connect Service Identity policies specified in the job file. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#consul_token NomadProvider#consul_token}
-        :param headers: headers block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#headers NomadProvider#headers}
-        :param http_auth: HTTP basic auth configuration. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#http_auth NomadProvider#http_auth}
-        :param ignore_env_vars: A set of environment variables that are ignored by the provider when configuring the Nomad API client. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#ignore_env_vars NomadProvider#ignore_env_vars}
-        :param key_file: A path to a PEM-encoded private key, required if cert_file or cert_pem is specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#key_file NomadProvider#key_file}
-        :param key_pem: PEM-encoded private key, required if cert_file or cert_pem is specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#key_pem NomadProvider#key_pem}
-        :param region: Region of the target Nomad agent. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#region NomadProvider#region}
-        :param secret_id: ACL token secret for API requests. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#secret_id NomadProvider#secret_id}
-        :param vault_token: Vault token if policies are specified in the job file. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#vault_token NomadProvider#vault_token}
+        :param address: URL of the root of the target Nomad agent. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#address NomadProvider#address}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#alias NomadProvider#alias}
+        :param ca_file: A path to a PEM-encoded certificate authority used to verify the remote agent's certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#ca_file NomadProvider#ca_file}
+        :param ca_pem: PEM-encoded certificate authority used to verify the remote agent's certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#ca_pem NomadProvider#ca_pem}
+        :param cert_file: A path to a PEM-encoded certificate provided to the remote agent; requires use of key_file or key_pem. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#cert_file NomadProvider#cert_file}
+        :param cert_pem: PEM-encoded certificate provided to the remote agent; requires use of key_file or key_pem. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#cert_pem NomadProvider#cert_pem}
+        :param consul_token: Consul token to validate Consul Connect Service Identity policies specified in the job file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#consul_token NomadProvider#consul_token}
+        :param headers: headers block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#headers NomadProvider#headers}
+        :param http_auth: HTTP basic auth configuration. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#http_auth NomadProvider#http_auth}
+        :param ignore_env_vars: A set of environment variables that are ignored by the provider when configuring the Nomad API client. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#ignore_env_vars NomadProvider#ignore_env_vars}
+        :param key_file: A path to a PEM-encoded private key, required if cert_file or cert_pem is specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#key_file NomadProvider#key_file}
+        :param key_pem: PEM-encoded private key, required if cert_file or cert_pem is specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#key_pem NomadProvider#key_pem}
+        :param region: Region of the target Nomad agent. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#region NomadProvider#region}
+        :param secret_id: ACL token secret for API requests. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#secret_id NomadProvider#secret_id}
+        :param vault_token: Vault token if policies are specified in the job file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#vault_token NomadProvider#vault_token}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e759273490438086fe5dd3d88c084b63217b1cc6e133fcd010a5f3e4c7a37ada)
             check_type(argname="argument address", value=address, expected_type=type_hints["address"])
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
             check_type(argname="argument ca_file", value=ca_file, expected_type=type_hints["ca_file"])
             check_type(argname="argument ca_pem", value=ca_pem, expected_type=type_hints["ca_pem"])
@@ -535,146 +535,146 @@
         if vault_token is not None:
             self._values["vault_token"] = vault_token
 
     @builtins.property
     def address(self) -> builtins.str:
         '''URL of the root of the target Nomad agent.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#address NomadProvider#address}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#address NomadProvider#address}
         '''
         result = self._values.get("address")
         assert result is not None, "Required property 'address' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#alias NomadProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#alias NomadProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ca_file(self) -> typing.Optional[builtins.str]:
         '''A path to a PEM-encoded certificate authority used to verify the remote agent's certificate.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#ca_file NomadProvider#ca_file}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#ca_file NomadProvider#ca_file}
         '''
         result = self._values.get("ca_file")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ca_pem(self) -> typing.Optional[builtins.str]:
         '''PEM-encoded certificate authority used to verify the remote agent's certificate.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#ca_pem NomadProvider#ca_pem}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#ca_pem NomadProvider#ca_pem}
         '''
         result = self._values.get("ca_pem")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def cert_file(self) -> typing.Optional[builtins.str]:
         '''A path to a PEM-encoded certificate provided to the remote agent; requires use of key_file or key_pem.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#cert_file NomadProvider#cert_file}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#cert_file NomadProvider#cert_file}
         '''
         result = self._values.get("cert_file")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def cert_pem(self) -> typing.Optional[builtins.str]:
         '''PEM-encoded certificate provided to the remote agent; requires use of key_file or key_pem.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#cert_pem NomadProvider#cert_pem}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#cert_pem NomadProvider#cert_pem}
         '''
         result = self._values.get("cert_pem")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def consul_token(self) -> typing.Optional[builtins.str]:
         '''Consul token to validate Consul Connect Service Identity policies specified in the job file.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#consul_token NomadProvider#consul_token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#consul_token NomadProvider#consul_token}
         '''
         result = self._values.get("consul_token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def headers(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["NomadProviderHeaders"]]]:
         '''headers block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#headers NomadProvider#headers}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#headers NomadProvider#headers}
         '''
         result = self._values.get("headers")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["NomadProviderHeaders"]]], result)
 
     @builtins.property
     def http_auth(self) -> typing.Optional[builtins.str]:
         '''HTTP basic auth configuration.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#http_auth NomadProvider#http_auth}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#http_auth NomadProvider#http_auth}
         '''
         result = self._values.get("http_auth")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ignore_env_vars(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]]:
         '''A set of environment variables that are ignored by the provider when configuring the Nomad API client.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#ignore_env_vars NomadProvider#ignore_env_vars}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#ignore_env_vars NomadProvider#ignore_env_vars}
         '''
         result = self._values.get("ignore_env_vars")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]], result)
 
     @builtins.property
     def key_file(self) -> typing.Optional[builtins.str]:
         '''A path to a PEM-encoded private key, required if cert_file or cert_pem is specified.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#key_file NomadProvider#key_file}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#key_file NomadProvider#key_file}
         '''
         result = self._values.get("key_file")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def key_pem(self) -> typing.Optional[builtins.str]:
         '''PEM-encoded private key, required if cert_file or cert_pem is specified.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#key_pem NomadProvider#key_pem}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#key_pem NomadProvider#key_pem}
         '''
         result = self._values.get("key_pem")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def region(self) -> typing.Optional[builtins.str]:
         '''Region of the target Nomad agent.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#region NomadProvider#region}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#region NomadProvider#region}
         '''
         result = self._values.get("region")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def secret_id(self) -> typing.Optional[builtins.str]:
         '''ACL token secret for API requests.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#secret_id NomadProvider#secret_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#secret_id NomadProvider#secret_id}
         '''
         result = self._values.get("secret_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def vault_token(self) -> typing.Optional[builtins.str]:
         '''Vault token if policies are specified in the job file.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#vault_token NomadProvider#vault_token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#vault_token NomadProvider#vault_token}
         '''
         result = self._values.get("vault_token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -691,41 +691,41 @@
     jsii_type="@cdktf/provider-nomad.provider.NomadProviderHeaders",
     jsii_struct_bases=[],
     name_mapping={"name": "name", "value": "value"},
 )
 class NomadProviderHeaders:
     def __init__(self, *, name: builtins.str, value: builtins.str) -> None:
         '''
-        :param name: The header name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#name NomadProvider#name}
-        :param value: The header value. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#value NomadProvider#value}
+        :param name: The header name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#name NomadProvider#name}
+        :param value: The header value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#value NomadProvider#value}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__55e77394e5bf2f9bd34a37f003dbe588118fddb6f74338ed48dcede78167deb3)
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "name": name,
             "value": value,
         }
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The header name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#name NomadProvider#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#name NomadProvider#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def value(self) -> builtins.str:
         '''The header value.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad#value NomadProvider#value}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs#value NomadProvider#value}
         '''
         result = self._values.get("value")
         assert result is not None, "Required property 'value' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/quota_specification/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/quota_specification/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `nomad_quota_specification`
 
-Refer to the Terraform Registory for docs: [`nomad_quota_specification`](https://www.terraform.io/docs/providers/nomad/r/quota_specification).
+Refer to the Terraform Registory for docs: [`nomad_quota_specification`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,41 +22,41 @@
 
 
 class QuotaSpecification(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.quotaSpecification.QuotaSpecification",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification nomad_quota_specification}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification nomad_quota_specification}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         limits: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["QuotaSpecificationLimits", typing.Dict[builtins.str, typing.Any]]]],
         name: builtins.str,
         description: typing.Optional[builtins.str] = None,
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
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification nomad_quota_specification} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification nomad_quota_specification} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param limits: limits block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#limits QuotaSpecification#limits}
-        :param name: Unique name for this quota specification. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#name QuotaSpecification#name}
-        :param description: Description for this quota specification. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#description QuotaSpecification#description}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#id QuotaSpecification#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param limits: limits block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#limits QuotaSpecification#limits}
+        :param name: Unique name for this quota specification. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#name QuotaSpecification#name}
+        :param description: Description for this quota specification. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#description QuotaSpecification#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#id QuotaSpecification#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -193,15 +193,15 @@
     },
 )
 class QuotaSpecificationConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         limits: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["QuotaSpecificationLimits", typing.Dict[builtins.str, typing.Any]]]],
         name: builtins.str,
@@ -212,18 +212,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param limits: limits block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#limits QuotaSpecification#limits}
-        :param name: Unique name for this quota specification. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#name QuotaSpecification#name}
-        :param description: Description for this quota specification. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#description QuotaSpecification#description}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#id QuotaSpecification#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param limits: limits block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#limits QuotaSpecification#limits}
+        :param name: Unique name for this quota specification. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#name QuotaSpecification#name}
+        :param description: Description for this quota specification. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#description QuotaSpecification#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#id QuotaSpecification#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9bbacac1608669777de5aa925508b8baa491a0beaf6e872b0375040fbf806252)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -266,20 +266,22 @@
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
@@ -323,42 +325,42 @@
 
     @builtins.property
     def limits(
         self,
     ) -> typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["QuotaSpecificationLimits"]]:
         '''limits block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#limits QuotaSpecification#limits}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#limits QuotaSpecification#limits}
         '''
         result = self._values.get("limits")
         assert result is not None, "Required property 'limits' is missing"
         return typing.cast(typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["QuotaSpecificationLimits"]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''Unique name for this quota specification.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#name QuotaSpecification#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#name QuotaSpecification#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''Description for this quota specification.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#description QuotaSpecification#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#description QuotaSpecification#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#id QuotaSpecification#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#id QuotaSpecification#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -383,16 +385,16 @@
     def __init__(
         self,
         *,
         region: builtins.str,
         region_limit: typing.Union["QuotaSpecificationLimitsRegionLimit", typing.Dict[builtins.str, typing.Any]],
     ) -> None:
         '''
-        :param region: Region in which this limit has affect. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#region QuotaSpecification#region}
-        :param region_limit: region_limit block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#region_limit QuotaSpecification#region_limit}
+        :param region: Region in which this limit has affect. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#region QuotaSpecification#region}
+        :param region_limit: region_limit block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#region_limit QuotaSpecification#region_limit}
         '''
         if isinstance(region_limit, dict):
             region_limit = QuotaSpecificationLimitsRegionLimit(**region_limit)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__046cab3db18bfd2e688094ffdf93d01951feb11939f6d207109d226b05318751)
             check_type(argname="argument region", value=region, expected_type=type_hints["region"])
             check_type(argname="argument region_limit", value=region_limit, expected_type=type_hints["region_limit"])
@@ -401,25 +403,25 @@
             "region_limit": region_limit,
         }
 
     @builtins.property
     def region(self) -> builtins.str:
         '''Region in which this limit has affect.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#region QuotaSpecification#region}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#region QuotaSpecification#region}
         '''
         result = self._values.get("region")
         assert result is not None, "Required property 'region' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def region_limit(self) -> "QuotaSpecificationLimitsRegionLimit":
         '''region_limit block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#region_limit QuotaSpecification#region_limit}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#region_limit QuotaSpecification#region_limit}
         '''
         result = self._values.get("region_limit")
         assert result is not None, "Required property 'region_limit' is missing"
         return typing.cast("QuotaSpecificationLimitsRegionLimit", result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -553,16 +555,16 @@
     def put_region_limit(
         self,
         *,
         cpu: typing.Optional[jsii.Number] = None,
         memory_mb: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
-        :param cpu: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#cpu QuotaSpecification#cpu}.
-        :param memory_mb: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#memory_mb QuotaSpecification#memory_mb}.
+        :param cpu: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#cpu QuotaSpecification#cpu}.
+        :param memory_mb: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#memory_mb QuotaSpecification#memory_mb}.
         '''
         value = QuotaSpecificationLimitsRegionLimit(cpu=cpu, memory_mb=memory_mb)
 
         return typing.cast(None, jsii.invoke(self, "putRegionLimit", [value]))
 
     @builtins.property
     @jsii.member(jsii_name="regionLimit")
@@ -620,36 +622,36 @@
     def __init__(
         self,
         *,
         cpu: typing.Optional[jsii.Number] = None,
         memory_mb: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
-        :param cpu: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#cpu QuotaSpecification#cpu}.
-        :param memory_mb: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#memory_mb QuotaSpecification#memory_mb}.
+        :param cpu: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#cpu QuotaSpecification#cpu}.
+        :param memory_mb: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#memory_mb QuotaSpecification#memory_mb}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__fb2c774fec44fdef15550af04c0defda44df7373af4c89bbbe5ca8ecc225a88f)
             check_type(argname="argument cpu", value=cpu, expected_type=type_hints["cpu"])
             check_type(argname="argument memory_mb", value=memory_mb, expected_type=type_hints["memory_mb"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if cpu is not None:
             self._values["cpu"] = cpu
         if memory_mb is not None:
             self._values["memory_mb"] = memory_mb
 
     @builtins.property
     def cpu(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#cpu QuotaSpecification#cpu}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#cpu QuotaSpecification#cpu}.'''
         result = self._values.get("cpu")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def memory_mb(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/quota_specification#memory_mb QuotaSpecification#memory_mb}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/quota_specification#memory_mb QuotaSpecification#memory_mb}.'''
         result = self._values.get("memory_mb")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -756,15 +758,15 @@
     id_: builtins.str,
     *,
     limits: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[QuotaSpecificationLimits, typing.Dict[builtins.str, typing.Any]]]],
     name: builtins.str,
     description: typing.Optional[builtins.str] = None,
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
@@ -793,15 +795,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__9bbacac1608669777de5aa925508b8baa491a0beaf6e872b0375040fbf806252(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     limits: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[QuotaSpecificationLimits, typing.Dict[builtins.str, typing.Any]]]],
     name: builtins.str,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/scheduler_config/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/scheduler_config/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `nomad_scheduler_config`
 
-Refer to the Terraform Registory for docs: [`nomad_scheduler_config`](https://www.terraform.io/docs/providers/nomad/r/scheduler_config).
+Refer to the Terraform Registory for docs: [`nomad_scheduler_config`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/scheduler_config).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,41 +22,41 @@
 
 
 class SchedulerConfig(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.schedulerConfig.SchedulerConfig",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/r/scheduler_config nomad_scheduler_config}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/scheduler_config nomad_scheduler_config}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: typing.Optional[builtins.str] = None,
         memory_oversubscription_enabled: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         preemption_config: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]] = None,
         scheduler_algorithm: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/r/scheduler_config nomad_scheduler_config} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/scheduler_config nomad_scheduler_config} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/scheduler_config#id SchedulerConfig#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param memory_oversubscription_enabled: When true, tasks may exceed their reserved memory limit. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/scheduler_config#memory_oversubscription_enabled SchedulerConfig#memory_oversubscription_enabled}
-        :param preemption_config: Options to enable preemption for various schedulers. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/scheduler_config#preemption_config SchedulerConfig#preemption_config}
-        :param scheduler_algorithm: Specifies whether scheduler binpacks or spreads allocations on available nodes. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/scheduler_config#scheduler_algorithm SchedulerConfig#scheduler_algorithm}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/scheduler_config#id SchedulerConfig#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param memory_oversubscription_enabled: When true, tasks may exceed their reserved memory limit. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/scheduler_config#memory_oversubscription_enabled SchedulerConfig#memory_oversubscription_enabled}
+        :param preemption_config: Options to enable preemption for various schedulers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/scheduler_config#preemption_config SchedulerConfig#preemption_config}
+        :param scheduler_algorithm: Specifies whether scheduler binpacks or spreads allocations on available nodes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/scheduler_config#scheduler_algorithm SchedulerConfig#scheduler_algorithm}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -207,15 +207,15 @@
     },
 )
 class SchedulerConfigConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         id: typing.Optional[builtins.str] = None,
         memory_oversubscription_enabled: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
@@ -226,18 +226,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/scheduler_config#id SchedulerConfig#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param memory_oversubscription_enabled: When true, tasks may exceed their reserved memory limit. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/scheduler_config#memory_oversubscription_enabled SchedulerConfig#memory_oversubscription_enabled}
-        :param preemption_config: Options to enable preemption for various schedulers. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/scheduler_config#preemption_config SchedulerConfig#preemption_config}
-        :param scheduler_algorithm: Specifies whether scheduler binpacks or spreads allocations on available nodes. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/scheduler_config#scheduler_algorithm SchedulerConfig#scheduler_algorithm}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/scheduler_config#id SchedulerConfig#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param memory_oversubscription_enabled: When true, tasks may exceed their reserved memory limit. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/scheduler_config#memory_oversubscription_enabled SchedulerConfig#memory_oversubscription_enabled}
+        :param preemption_config: Options to enable preemption for various schedulers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/scheduler_config#preemption_config SchedulerConfig#preemption_config}
+        :param scheduler_algorithm: Specifies whether scheduler binpacks or spreads allocations on available nodes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/scheduler_config#scheduler_algorithm SchedulerConfig#scheduler_algorithm}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2960b8e7114f79c41b18bc71a4082adc1d3a78d0fc7ff1561eedd88b1584ba4b)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -281,20 +281,22 @@
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
@@ -334,49 +336,49 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/scheduler_config#id SchedulerConfig#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/scheduler_config#id SchedulerConfig#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def memory_oversubscription_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''When true, tasks may exceed their reserved memory limit.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/scheduler_config#memory_oversubscription_enabled SchedulerConfig#memory_oversubscription_enabled}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/scheduler_config#memory_oversubscription_enabled SchedulerConfig#memory_oversubscription_enabled}
         '''
         result = self._values.get("memory_oversubscription_enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def preemption_config(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]]:
         '''Options to enable preemption for various schedulers.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/scheduler_config#preemption_config SchedulerConfig#preemption_config}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/scheduler_config#preemption_config SchedulerConfig#preemption_config}
         '''
         result = self._values.get("preemption_config")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]], result)
 
     @builtins.property
     def scheduler_algorithm(self) -> typing.Optional[builtins.str]:
         '''Specifies whether scheduler binpacks or spreads allocations on available nodes.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/scheduler_config#scheduler_algorithm SchedulerConfig#scheduler_algorithm}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/scheduler_config#scheduler_algorithm SchedulerConfig#scheduler_algorithm}
         '''
         result = self._values.get("scheduler_algorithm")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -401,15 +403,15 @@
     id_: builtins.str,
     *,
     id: typing.Optional[builtins.str] = None,
     memory_oversubscription_enabled: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     preemption_config: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]] = None,
     scheduler_algorithm: typing.Optional[builtins.str] = None,
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
@@ -438,15 +440,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__2960b8e7114f79c41b18bc71a4082adc1d3a78d0fc7ff1561eedd88b1584ba4b(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     id: typing.Optional[builtins.str] = None,
     memory_oversubscription_enabled: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/sentinel_policy/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/sentinel_policy/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `nomad_sentinel_policy`
 
-Refer to the Terraform Registory for docs: [`nomad_sentinel_policy`](https://www.terraform.io/docs/providers/nomad/r/sentinel_policy).
+Refer to the Terraform Registory for docs: [`nomad_sentinel_policy`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/sentinel_policy).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,45 +22,45 @@
 
 
 class SentinelPolicy(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.sentinelPolicy.SentinelPolicy",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/r/sentinel_policy nomad_sentinel_policy}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/sentinel_policy nomad_sentinel_policy}.'''
 
     def __init__(
         self,
         scope_: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         enforcement_level: builtins.str,
         name: builtins.str,
         policy: builtins.str,
         scope: builtins.str,
         description: typing.Optional[builtins.str] = None,
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
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/r/sentinel_policy nomad_sentinel_policy} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/sentinel_policy nomad_sentinel_policy} Resource.
 
         :param scope_: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param enforcement_level: Specifies the enforcement level of the policy. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/sentinel_policy#enforcement_level SentinelPolicy#enforcement_level}
-        :param name: Unique name for this policy. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/sentinel_policy#name SentinelPolicy#name}
-        :param policy: The Sentinel policy. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/sentinel_policy#policy SentinelPolicy#policy}
-        :param scope: Specifies the scope for this policy. Only 'submit-job' is currently supported. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/sentinel_policy#scope SentinelPolicy#scope}
-        :param description: Description for this policy. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/sentinel_policy#description SentinelPolicy#description}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/sentinel_policy#id SentinelPolicy#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param enforcement_level: Specifies the enforcement level of the policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/sentinel_policy#enforcement_level SentinelPolicy#enforcement_level}
+        :param name: Unique name for this policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/sentinel_policy#name SentinelPolicy#name}
+        :param policy: The Sentinel policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/sentinel_policy#policy SentinelPolicy#policy}
+        :param scope: Specifies the scope for this policy. Only 'submit-job' is currently supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/sentinel_policy#scope SentinelPolicy#scope}
+        :param description: Description for this policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/sentinel_policy#description SentinelPolicy#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/sentinel_policy#id SentinelPolicy#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -227,15 +227,15 @@
     },
 )
 class SentinelPolicyConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         enforcement_level: builtins.str,
         name: builtins.str,
@@ -248,20 +248,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param enforcement_level: Specifies the enforcement level of the policy. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/sentinel_policy#enforcement_level SentinelPolicy#enforcement_level}
-        :param name: Unique name for this policy. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/sentinel_policy#name SentinelPolicy#name}
-        :param policy: The Sentinel policy. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/sentinel_policy#policy SentinelPolicy#policy}
-        :param scope: Specifies the scope for this policy. Only 'submit-job' is currently supported. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/sentinel_policy#scope SentinelPolicy#scope}
-        :param description: Description for this policy. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/sentinel_policy#description SentinelPolicy#description}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/sentinel_policy#id SentinelPolicy#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param enforcement_level: Specifies the enforcement level of the policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/sentinel_policy#enforcement_level SentinelPolicy#enforcement_level}
+        :param name: Unique name for this policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/sentinel_policy#name SentinelPolicy#name}
+        :param policy: The Sentinel policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/sentinel_policy#policy SentinelPolicy#policy}
+        :param scope: Specifies the scope for this policy. Only 'submit-job' is currently supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/sentinel_policy#scope SentinelPolicy#scope}
+        :param description: Description for this policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/sentinel_policy#description SentinelPolicy#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/sentinel_policy#id SentinelPolicy#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__474e5918a2ed72211e6b5e4a4e6cc6c981b4c8a615a348a72e607a1cafb946dd)
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
@@ -363,62 +365,62 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def enforcement_level(self) -> builtins.str:
         '''Specifies the enforcement level of the policy.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/sentinel_policy#enforcement_level SentinelPolicy#enforcement_level}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/sentinel_policy#enforcement_level SentinelPolicy#enforcement_level}
         '''
         result = self._values.get("enforcement_level")
         assert result is not None, "Required property 'enforcement_level' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''Unique name for this policy.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/sentinel_policy#name SentinelPolicy#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/sentinel_policy#name SentinelPolicy#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def policy(self) -> builtins.str:
         '''The Sentinel policy.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/sentinel_policy#policy SentinelPolicy#policy}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/sentinel_policy#policy SentinelPolicy#policy}
         '''
         result = self._values.get("policy")
         assert result is not None, "Required property 'policy' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def scope(self) -> builtins.str:
         '''Specifies the scope for this policy. Only 'submit-job' is currently supported.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/sentinel_policy#scope SentinelPolicy#scope}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/sentinel_policy#scope SentinelPolicy#scope}
         '''
         result = self._values.get("scope")
         assert result is not None, "Required property 'scope' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''Description for this policy.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/sentinel_policy#description SentinelPolicy#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/sentinel_policy#description SentinelPolicy#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/sentinel_policy#id SentinelPolicy#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/sentinel_policy#id SentinelPolicy#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -448,15 +450,15 @@
     enforcement_level: builtins.str,
     name: builtins.str,
     policy: builtins.str,
     scope: builtins.str,
     description: typing.Optional[builtins.str] = None,
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
@@ -497,15 +499,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__474e5918a2ed72211e6b5e4a4e6cc6c981b4c8a615a348a72e607a1cafb946dd(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     enforcement_level: builtins.str,
     name: builtins.str,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad/volume/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad/volume/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `nomad_volume`
 
-Refer to the Terraform Registory for docs: [`nomad_volume`](https://www.terraform.io/docs/providers/nomad/r/volume).
+Refer to the Terraform Registory for docs: [`nomad_volume`](https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Volume(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-nomad.volume.Volume",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/nomad/r/volume nomad_volume}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume nomad_volume}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         external_id: builtins.str,
@@ -46,41 +46,41 @@
         mount_options: typing.Optional[typing.Union["VolumeMountOptions", typing.Dict[builtins.str, typing.Any]]] = None,
         namespace: typing.Optional[builtins.str] = None,
         parameters: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         secrets: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         topology_request: typing.Optional[typing.Union["VolumeTopologyRequest", typing.Dict[builtins.str, typing.Any]]] = None,
         type: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/nomad/r/volume nomad_volume} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume nomad_volume} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param external_id: The ID of the physical volume from the storage provider. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#external_id Volume#external_id}
-        :param name: The display name of the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#name Volume#name}
-        :param plugin_id: The ID of the CSI plugin that manages this volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#plugin_id Volume#plugin_id}
-        :param volume_id: The unique ID of the volume, how jobs will refer to the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#volume_id Volume#volume_id}
-        :param access_mode: Defines whether a volume should be available concurrently. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#access_mode Volume#access_mode}
-        :param attachment_mode: The storage API that will be used by the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#attachment_mode Volume#attachment_mode}
-        :param capability: capability block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#capability Volume#capability}
-        :param context: An optional key-value map of strings passed directly to the CSI plugin to validate the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#context Volume#context}
-        :param deregister_on_destroy: If true, the volume will be deregistered on destroy. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#deregister_on_destroy Volume#deregister_on_destroy}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#id Volume#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param mount_options: mount_options block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#mount_options Volume#mount_options}
-        :param namespace: The namespace in which to create the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#namespace Volume#namespace}
-        :param parameters: An optional key-value map of strings passed directly to the CSI plugin to configure the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#parameters Volume#parameters}
-        :param secrets: An optional key-value map of strings used as credentials for publishing and unpublishing volumes. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#secrets Volume#secrets}
-        :param topology_request: topology_request block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#topology_request Volume#topology_request}
-        :param type: The type of the volume. Currently, only 'csi' is supported. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#type Volume#type}
+        :param external_id: The ID of the physical volume from the storage provider. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#external_id Volume#external_id}
+        :param name: The display name of the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#name Volume#name}
+        :param plugin_id: The ID of the CSI plugin that manages this volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#plugin_id Volume#plugin_id}
+        :param volume_id: The unique ID of the volume, how jobs will refer to the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#volume_id Volume#volume_id}
+        :param access_mode: Defines whether a volume should be available concurrently. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#access_mode Volume#access_mode}
+        :param attachment_mode: The storage API that will be used by the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#attachment_mode Volume#attachment_mode}
+        :param capability: capability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#capability Volume#capability}
+        :param context: An optional key-value map of strings passed directly to the CSI plugin to validate the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#context Volume#context}
+        :param deregister_on_destroy: If true, the volume will be deregistered on destroy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#deregister_on_destroy Volume#deregister_on_destroy}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#id Volume#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param mount_options: mount_options block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#mount_options Volume#mount_options}
+        :param namespace: The namespace in which to create the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#namespace Volume#namespace}
+        :param parameters: An optional key-value map of strings passed directly to the CSI plugin to configure the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#parameters Volume#parameters}
+        :param secrets: An optional key-value map of strings used as credentials for publishing and unpublishing volumes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#secrets Volume#secrets}
+        :param topology_request: topology_request block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#topology_request Volume#topology_request}
+        :param type: The type of the volume. Currently, only 'csi' is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#type Volume#type}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -134,29 +134,29 @@
     def put_mount_options(
         self,
         *,
         fs_type: typing.Optional[builtins.str] = None,
         mount_flags: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param fs_type: The file system type. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#fs_type Volume#fs_type}
-        :param mount_flags: The flags passed to mount. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#mount_flags Volume#mount_flags}
+        :param fs_type: The file system type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#fs_type Volume#fs_type}
+        :param mount_flags: The flags passed to mount. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#mount_flags Volume#mount_flags}
         '''
         value = VolumeMountOptions(fs_type=fs_type, mount_flags=mount_flags)
 
         return typing.cast(None, jsii.invoke(self, "putMountOptions", [value]))
 
     @jsii.member(jsii_name="putTopologyRequest")
     def put_topology_request(
         self,
         *,
         required: typing.Optional[typing.Union["VolumeTopologyRequestRequired", typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
-        :param required: required block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#required Volume#required}
+        :param required: required block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#required Volume#required}
         '''
         value = VolumeTopologyRequest(required=required)
 
         return typing.cast(None, jsii.invoke(self, "putTopologyRequest", [value]))
 
     @jsii.member(jsii_name="resetAccessMode")
     def reset_access_mode(self) -> None:
@@ -536,41 +536,41 @@
     def __init__(
         self,
         *,
         access_mode: builtins.str,
         attachment_mode: builtins.str,
     ) -> None:
         '''
-        :param access_mode: Defines whether a volume should be available concurrently. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#access_mode Volume#access_mode}
-        :param attachment_mode: The storage API that will be used by the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#attachment_mode Volume#attachment_mode}
+        :param access_mode: Defines whether a volume should be available concurrently. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#access_mode Volume#access_mode}
+        :param attachment_mode: The storage API that will be used by the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#attachment_mode Volume#attachment_mode}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__82ff8d33b081ea2e1dd4c0781d9b593bc38991532a7cb78bfea7b13ccf673154)
             check_type(argname="argument access_mode", value=access_mode, expected_type=type_hints["access_mode"])
             check_type(argname="argument attachment_mode", value=attachment_mode, expected_type=type_hints["attachment_mode"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "access_mode": access_mode,
             "attachment_mode": attachment_mode,
         }
 
     @builtins.property
     def access_mode(self) -> builtins.str:
         '''Defines whether a volume should be available concurrently.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#access_mode Volume#access_mode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#access_mode Volume#access_mode}
         '''
         result = self._values.get("access_mode")
         assert result is not None, "Required property 'access_mode' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def attachment_mode(self) -> builtins.str:
         '''The storage API that will be used by the volume.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#attachment_mode Volume#attachment_mode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#attachment_mode Volume#attachment_mode}
         '''
         result = self._values.get("attachment_mode")
         assert result is not None, "Required property 'attachment_mode' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -782,15 +782,15 @@
     },
 )
 class VolumeConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         external_id: builtins.str,
         name: builtins.str,
@@ -813,30 +813,30 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param external_id: The ID of the physical volume from the storage provider. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#external_id Volume#external_id}
-        :param name: The display name of the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#name Volume#name}
-        :param plugin_id: The ID of the CSI plugin that manages this volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#plugin_id Volume#plugin_id}
-        :param volume_id: The unique ID of the volume, how jobs will refer to the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#volume_id Volume#volume_id}
-        :param access_mode: Defines whether a volume should be available concurrently. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#access_mode Volume#access_mode}
-        :param attachment_mode: The storage API that will be used by the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#attachment_mode Volume#attachment_mode}
-        :param capability: capability block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#capability Volume#capability}
-        :param context: An optional key-value map of strings passed directly to the CSI plugin to validate the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#context Volume#context}
-        :param deregister_on_destroy: If true, the volume will be deregistered on destroy. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#deregister_on_destroy Volume#deregister_on_destroy}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#id Volume#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param mount_options: mount_options block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#mount_options Volume#mount_options}
-        :param namespace: The namespace in which to create the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#namespace Volume#namespace}
-        :param parameters: An optional key-value map of strings passed directly to the CSI plugin to configure the volume. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#parameters Volume#parameters}
-        :param secrets: An optional key-value map of strings used as credentials for publishing and unpublishing volumes. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#secrets Volume#secrets}
-        :param topology_request: topology_request block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#topology_request Volume#topology_request}
-        :param type: The type of the volume. Currently, only 'csi' is supported. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#type Volume#type}
+        :param external_id: The ID of the physical volume from the storage provider. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#external_id Volume#external_id}
+        :param name: The display name of the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#name Volume#name}
+        :param plugin_id: The ID of the CSI plugin that manages this volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#plugin_id Volume#plugin_id}
+        :param volume_id: The unique ID of the volume, how jobs will refer to the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#volume_id Volume#volume_id}
+        :param access_mode: Defines whether a volume should be available concurrently. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#access_mode Volume#access_mode}
+        :param attachment_mode: The storage API that will be used by the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#attachment_mode Volume#attachment_mode}
+        :param capability: capability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#capability Volume#capability}
+        :param context: An optional key-value map of strings passed directly to the CSI plugin to validate the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#context Volume#context}
+        :param deregister_on_destroy: If true, the volume will be deregistered on destroy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#deregister_on_destroy Volume#deregister_on_destroy}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#id Volume#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param mount_options: mount_options block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#mount_options Volume#mount_options}
+        :param namespace: The namespace in which to create the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#namespace Volume#namespace}
+        :param parameters: An optional key-value map of strings passed directly to the CSI plugin to configure the volume. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#parameters Volume#parameters}
+        :param secrets: An optional key-value map of strings used as credentials for publishing and unpublishing volumes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#secrets Volume#secrets}
+        :param topology_request: topology_request block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#topology_request Volume#topology_request}
+        :param type: The type of the volume. Currently, only 'csi' is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#type Volume#type}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(mount_options, dict):
             mount_options = VolumeMountOptions(**mount_options)
         if isinstance(topology_request, dict):
             topology_request = VolumeTopologyRequest(**topology_request)
@@ -917,20 +917,22 @@
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
@@ -972,159 +974,159 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def external_id(self) -> builtins.str:
         '''The ID of the physical volume from the storage provider.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#external_id Volume#external_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#external_id Volume#external_id}
         '''
         result = self._values.get("external_id")
         assert result is not None, "Required property 'external_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The display name of the volume.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#name Volume#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#name Volume#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def plugin_id(self) -> builtins.str:
         '''The ID of the CSI plugin that manages this volume.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#plugin_id Volume#plugin_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#plugin_id Volume#plugin_id}
         '''
         result = self._values.get("plugin_id")
         assert result is not None, "Required property 'plugin_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def volume_id(self) -> builtins.str:
         '''The unique ID of the volume, how jobs will refer to the volume.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#volume_id Volume#volume_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#volume_id Volume#volume_id}
         '''
         result = self._values.get("volume_id")
         assert result is not None, "Required property 'volume_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def access_mode(self) -> typing.Optional[builtins.str]:
         '''Defines whether a volume should be available concurrently.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#access_mode Volume#access_mode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#access_mode Volume#access_mode}
         '''
         result = self._values.get("access_mode")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def attachment_mode(self) -> typing.Optional[builtins.str]:
         '''The storage API that will be used by the volume.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#attachment_mode Volume#attachment_mode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#attachment_mode Volume#attachment_mode}
         '''
         result = self._values.get("attachment_mode")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def capability(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[VolumeCapability]]]:
         '''capability block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#capability Volume#capability}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#capability Volume#capability}
         '''
         result = self._values.get("capability")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[VolumeCapability]]], result)
 
     @builtins.property
     def context(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''An optional key-value map of strings passed directly to the CSI plugin to validate the volume.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#context Volume#context}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#context Volume#context}
         '''
         result = self._values.get("context")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def deregister_on_destroy(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If true, the volume will be deregistered on destroy.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#deregister_on_destroy Volume#deregister_on_destroy}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#deregister_on_destroy Volume#deregister_on_destroy}
         '''
         result = self._values.get("deregister_on_destroy")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#id Volume#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#id Volume#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def mount_options(self) -> typing.Optional["VolumeMountOptions"]:
         '''mount_options block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#mount_options Volume#mount_options}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#mount_options Volume#mount_options}
         '''
         result = self._values.get("mount_options")
         return typing.cast(typing.Optional["VolumeMountOptions"], result)
 
     @builtins.property
     def namespace(self) -> typing.Optional[builtins.str]:
         '''The namespace in which to create the volume.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#namespace Volume#namespace}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#namespace Volume#namespace}
         '''
         result = self._values.get("namespace")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def parameters(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#parameters Volume#parameters}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#parameters Volume#parameters}
         '''
         result = self._values.get("parameters")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def secrets(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#secrets Volume#secrets}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#secrets Volume#secrets}
         '''
         result = self._values.get("secrets")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def topology_request(self) -> typing.Optional["VolumeTopologyRequest"]:
         '''topology_request block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#topology_request Volume#topology_request}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#topology_request Volume#topology_request}
         '''
         result = self._values.get("topology_request")
         return typing.cast(typing.Optional["VolumeTopologyRequest"], result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
         '''The type of the volume. Currently, only 'csi' is supported.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#type Volume#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#type Volume#type}
         '''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1146,16 +1148,16 @@
     def __init__(
         self,
         *,
         fs_type: typing.Optional[builtins.str] = None,
         mount_flags: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param fs_type: The file system type. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#fs_type Volume#fs_type}
-        :param mount_flags: The flags passed to mount. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#mount_flags Volume#mount_flags}
+        :param fs_type: The file system type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#fs_type Volume#fs_type}
+        :param mount_flags: The flags passed to mount. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#mount_flags Volume#mount_flags}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9d7feb5a469c8fcd95c95dd231c420df4eedfcc8ed690da67dc74a1596d722cf)
             check_type(argname="argument fs_type", value=fs_type, expected_type=type_hints["fs_type"])
             check_type(argname="argument mount_flags", value=mount_flags, expected_type=type_hints["mount_flags"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if fs_type is not None:
@@ -1163,24 +1165,24 @@
         if mount_flags is not None:
             self._values["mount_flags"] = mount_flags
 
     @builtins.property
     def fs_type(self) -> typing.Optional[builtins.str]:
         '''The file system type.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#fs_type Volume#fs_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#fs_type Volume#fs_type}
         '''
         result = self._values.get("fs_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def mount_flags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The flags passed to mount.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#mount_flags Volume#mount_flags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#mount_flags Volume#mount_flags}
         '''
         result = self._values.get("mount_flags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1414,30 +1416,30 @@
 class VolumeTopologyRequest:
     def __init__(
         self,
         *,
         required: typing.Optional[typing.Union["VolumeTopologyRequestRequired", typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
-        :param required: required block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#required Volume#required}
+        :param required: required block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#required Volume#required}
         '''
         if isinstance(required, dict):
             required = VolumeTopologyRequestRequired(**required)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4d3276426c5991d2601f38dcf5b1a34b9623cb79308256f951807d43a9e3dd55)
             check_type(argname="argument required", value=required, expected_type=type_hints["required"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if required is not None:
             self._values["required"] = required
 
     @builtins.property
     def required(self) -> typing.Optional["VolumeTopologyRequestRequired"]:
         '''required block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#required Volume#required}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#required Volume#required}
         '''
         result = self._values.get("required")
         return typing.cast(typing.Optional["VolumeTopologyRequestRequired"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1473,15 +1475,15 @@
     @jsii.member(jsii_name="putRequired")
     def put_required(
         self,
         *,
         topology: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["VolumeTopologyRequestRequiredTopology", typing.Dict[builtins.str, typing.Any]]]],
     ) -> None:
         '''
-        :param topology: topology block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#topology Volume#topology}
+        :param topology: topology block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#topology Volume#topology}
         '''
         value = VolumeTopologyRequestRequired(topology=topology)
 
         return typing.cast(None, jsii.invoke(self, "putRequired", [value]))
 
     @jsii.member(jsii_name="resetRequired")
     def reset_required(self) -> None:
@@ -1518,30 +1520,30 @@
 class VolumeTopologyRequestRequired:
     def __init__(
         self,
         *,
         topology: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["VolumeTopologyRequestRequiredTopology", typing.Dict[builtins.str, typing.Any]]]],
     ) -> None:
         '''
-        :param topology: topology block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#topology Volume#topology}
+        :param topology: topology block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#topology Volume#topology}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d615fe70e0d6d70420c0b22f988cf927fdb46da96f73255b57b88c4510cf61a0)
             check_type(argname="argument topology", value=topology, expected_type=type_hints["topology"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "topology": topology,
         }
 
     @builtins.property
     def topology(
         self,
     ) -> typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["VolumeTopologyRequestRequiredTopology"]]:
         '''topology block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#topology Volume#topology}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#topology Volume#topology}
         '''
         result = self._values.get("topology")
         assert result is not None, "Required property 'topology' is missing"
         return typing.cast(typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["VolumeTopologyRequestRequiredTopology"]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -1620,28 +1622,28 @@
     jsii_type="@cdktf/provider-nomad.volume.VolumeTopologyRequestRequiredTopology",
     jsii_struct_bases=[],
     name_mapping={"segments": "segments"},
 )
 class VolumeTopologyRequestRequiredTopology:
     def __init__(self, *, segments: typing.Mapping[builtins.str, builtins.str]) -> None:
         '''
-        :param segments: Define attributes for the topology request. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#segments Volume#segments}
+        :param segments: Define attributes for the topology request. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#segments Volume#segments}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4562a0ac1b734aed0d2e5fa885ebfe69f6b4249b485c956c66468125c09a9f1d)
             check_type(argname="argument segments", value=segments, expected_type=type_hints["segments"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "segments": segments,
         }
 
     @builtins.property
     def segments(self) -> typing.Mapping[builtins.str, builtins.str]:
         '''Define attributes for the topology request.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/nomad/r/volume#segments Volume#segments}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/nomad/1.4.19/docs/resources/volume#segments Volume#segments}
         '''
         result = self._values.get("segments")
         assert result is not None, "Required property 'segments' is missing"
         return typing.cast(typing.Mapping[builtins.str, builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -1850,15 +1852,15 @@
     mount_options: typing.Optional[typing.Union[VolumeMountOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     namespace: typing.Optional[builtins.str] = None,
     parameters: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     secrets: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     topology_request: typing.Optional[typing.Union[VolumeTopologyRequest, typing.Dict[builtins.str, typing.Any]]] = None,
     type: typing.Optional[builtins.str] = None,
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
@@ -2020,15 +2022,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__52babf881cfea79050bb811ab5834626eb980a40882a415da94157a451771d85(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     external_id: builtins.str,
     name: builtins.str,
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad.egg-info/PKG-INFO` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-nomad
-Version: 3.0.0
+Version: 4.0.0
 Summary: Prebuilt nomad Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-nomad.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-nomad.git
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
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-nomad-go`](https://github.com/cdktf/cdktf-provider-nomad-go) package.
 
 `go get github.com/cdktf/cdktf-provider-nomad-go/nomad`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-nomad).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform nomad Provider version 1:1. In fact, it always tracks `latest` of `~> 1.4` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-nomad-3.0.0/src/cdktf_cdktf_provider_nomad.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-nomad-4.0.0/src/cdktf_cdktf_provider_nomad.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_nomad/py.typed
 src/cdktf_cdktf_provider_nomad.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_nomad.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_nomad.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_nomad.egg-info/requires.txt
 src/cdktf_cdktf_provider_nomad.egg-info/top_level.txt
 src/cdktf_cdktf_provider_nomad/_jsii/__init__.py
-src/cdktf_cdktf_provider_nomad/_jsii/provider-nomad@3.0.0.jsii.tgz
+src/cdktf_cdktf_provider_nomad/_jsii/provider-nomad@4.0.0.jsii.tgz
 src/cdktf_cdktf_provider_nomad/acl_policy/__init__.py
 src/cdktf_cdktf_provider_nomad/acl_role/__init__.py
 src/cdktf_cdktf_provider_nomad/acl_token/__init__.py
 src/cdktf_cdktf_provider_nomad/data_nomad_acl_policies/__init__.py
 src/cdktf_cdktf_provider_nomad/data_nomad_acl_policy/__init__.py
 src/cdktf_cdktf_provider_nomad/data_nomad_acl_role/__init__.py
 src/cdktf_cdktf_provider_nomad/data_nomad_acl_roles/__init__.py
```

