# Comparing `tmp/cdktf-cdktf-provider-hcp-3.0.3.tar.gz` & `tmp/cdktf-cdktf-provider-hcp-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-hcp-3.0.3.tar", last modified: Tue Apr  4 07:23:14 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-hcp-4.0.0.tar", last modified: Tue Apr 18 20:43:20 2023, max compression
```

## Comparing `cdktf-cdktf-provider-hcp-3.0.3.tar` & `cdktf-cdktf-provider-hcp-4.0.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.884648 cdktf-cdktf-provider-hcp-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-04 07:23:14.884648 cdktf-cdktf-provider-hcp-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 07:23:14.884648 cdktf-cdktf-provider-hcp-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.868648 cdktf-cdktf-provider-hcp-3.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.872648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.876648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1132881 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/_jsii/provider-hcp@3.0.3.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.876648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/aws_network_peering/
--rw-r--r--   0 runner    (1001) docker     (123)    39869 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/aws_network_peering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.876648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/aws_transit_gateway_attachment/
--rw-r--r--   0 runner    (1001) docker     (123)    41319 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/aws_transit_gateway_attachment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.876648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/azure_peering_connection/
--rw-r--r--   0 runner    (1001) docker     (123)    46007 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/azure_peering_connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.876648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/boundary_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)    34892 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/boundary_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.876648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/consul_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)    80043 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/consul_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.876648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/consul_cluster_root_token/
--rw-r--r--   0 runner    (1001) docker     (123)    26437 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/consul_cluster_root_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.880648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/consul_snapshot/
--rw-r--r--   0 runner    (1001) docker     (123)    35057 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/consul_snapshot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.880648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_aws_network_peering/
--rw-r--r--   0 runner    (1001) docker     (123)    33323 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_aws_network_peering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.880648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_aws_transit_gateway_attachment/
--rw-r--r--   0 runner    (1001) docker     (123)    34679 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_aws_transit_gateway_attachment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.880648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_azure_peering_connection/
--rw-r--r--   0 runner    (1001) docker     (123)    34436 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_azure_peering_connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.880648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_boundary_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)    26244 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_boundary_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.880648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_helm_config/
--rw-r--r--   0 runner    (1001) docker     (123)    32227 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_helm_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.880648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_kubernetes_secret/
--rw-r--r--   0 runner    (1001) docker     (123)    26728 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_kubernetes_secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.880648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)    39351 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.880648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_versions/
--rw-r--r--   0 runner    (1001) docker     (123)    24090 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.880648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_hvn/
--rw-r--r--   0 runner    (1001) docker     (123)    26438 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_hvn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.880648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_peering_connection/
--rw-r--r--   0 runner    (1001) docker     (123)    31214 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_peering_connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.880648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_route/
--rw-r--r--   0 runner    (1001) docker     (123)    28302 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_route/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.880648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image/
--rw-r--r--   0 runner    (1001) docker     (123)    39296 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.880648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image_iteration/
--rw-r--r--   0 runner    (1001) docker     (123)    49506 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image_iteration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.880648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_packer_iteration/
--rw-r--r--   0 runner    (1001) docker     (123)    29600 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_packer_iteration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.880648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_vault_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)    67987 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_vault_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.884648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/hvn/
--rw-r--r--   0 runner    (1001) docker     (123)    36459 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/hvn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.884648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/hvn_peering_connection/
--rw-r--r--   0 runner    (1001) docker     (123)    33124 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/hvn_peering_connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.884648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/hvn_route/
--rw-r--r--   0 runner    (1001) docker     (123)    36610 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/hvn_route/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.884648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/packer_channel/
--rw-r--r--   0 runner    (1001) docker     (123)    48424 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/packer_channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.884648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.884648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/vault_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)   114048 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/vault_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.884648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/vault_cluster_admin_token/
--rw-r--r--   0 runner    (1001) docker     (123)    30409 2023-04-04 07:22:59.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/vault_cluster_admin_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:23:14.876648 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-04 07:23:14.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-04 07:23:14.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 07:23:14.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-04 07:23:14.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-04 07:23:14.000000 cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.309649 cdktf-cdktf-provider-hcp-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-18 20:43:20.309649 cdktf-cdktf-provider-hcp-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:43:20.309649 cdktf-cdktf-provider-hcp-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.301649 cdktf-cdktf-provider-hcp-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.301649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.305649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1133045 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/_jsii/provider-hcp@4.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.305649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/aws_network_peering/
+-rw-r--r--   0 runner    (1001) docker     (123)    41150 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/aws_network_peering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.305649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/aws_transit_gateway_attachment/
+-rw-r--r--   0 runner    (1001) docker     (123)    42510 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/aws_transit_gateway_attachment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.305649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/azure_peering_connection/
+-rw-r--r--   0 runner    (1001) docker     (123)    47468 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/azure_peering_connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.305649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/boundary_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)    35993 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/boundary_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.305649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/consul_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)    82074 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/consul_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.305649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/consul_cluster_root_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    27178 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/consul_cluster_root_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.305649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/consul_snapshot/
+-rw-r--r--   0 runner    (1001) docker     (123)    36158 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/consul_snapshot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.305649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_aws_network_peering/
+-rw-r--r--   0 runner    (1001) docker     (123)    34307 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_aws_network_peering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.305649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_aws_transit_gateway_attachment/
+-rw-r--r--   0 runner    (1001) docker     (123)    35663 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_aws_transit_gateway_attachment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.305649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_azure_peering_connection/
+-rw-r--r--   0 runner    (1001) docker     (123)    35420 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_azure_peering_connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.305649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_boundary_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)    27030 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_boundary_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.305649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_helm_config/
+-rw-r--r--   0 runner    (1001) docker     (123)    33211 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_helm_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.305649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_kubernetes_secret/
+-rw-r--r--   0 runner    (1001) docker     (123)    27514 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_kubernetes_secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.305649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)    40137 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.305649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_versions/
+-rw-r--r--   0 runner    (1001) docker     (123)    24777 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.305649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_hvn/
+-rw-r--r--   0 runner    (1001) docker     (123)    27224 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_hvn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.309649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_peering_connection/
+-rw-r--r--   0 runner    (1001) docker     (123)    32198 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_peering_connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.309649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_route/
+-rw-r--r--   0 runner    (1001) docker     (123)    29187 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_route/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.309649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image/
+-rw-r--r--   0 runner    (1001) docker     (123)    40577 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.309649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image_iteration/
+-rw-r--r--   0 runner    (1001) docker     (123)    50391 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image_iteration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.309649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_packer_iteration/
+-rw-r--r--   0 runner    (1001) docker     (123)    30485 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_packer_iteration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.309649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_vault_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)    68971 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_vault_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.309649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/hvn/
+-rw-r--r--   0 runner    (1001) docker     (123)    37650 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/hvn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.309649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/hvn_peering_connection/
+-rw-r--r--   0 runner    (1001) docker     (123)    34135 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/hvn_peering_connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.309649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/hvn_route/
+-rw-r--r--   0 runner    (1001) docker     (123)    37801 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/hvn_route/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.309649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/packer_channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    49885 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/packer_channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.309649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.309649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/vault_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)   117399 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/vault_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.309649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/vault_cluster_admin_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    31330 2023-04-18 20:43:08.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/vault_cluster_admin_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:43:20.305649 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-18 20:43:20.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-18 20:43:20.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:43:20.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:43:20.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 20:43:20.000000 cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/LICENSE` & `cdktf-cdktf-provider-hcp-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/PKG-INFO` & `cdktf-cdktf-provider-hcp-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-hcp
-Version: 3.0.3
+Version: 4.0.0
 Summary: Prebuilt hcp Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-hcp.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-hcp.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/README.md` & `cdktf-cdktf-provider-hcp-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/setup.py` & `cdktf-cdktf-provider-hcp-4.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-hcp",
-    "version": "3.0.3",
+    "version": "4.0.0",
     "description": "Prebuilt hcp Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-hcp.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -51,25 +51,25 @@
         "cdktf_cdktf_provider_hcp.packer_channel",
         "cdktf_cdktf_provider_hcp.provider",
         "cdktf_cdktf_provider_hcp.vault_cluster",
         "cdktf_cdktf_provider_hcp.vault_cluster_admin_token"
     ],
     "package_data": {
         "cdktf_cdktf_provider_hcp._jsii": [
-            "provider-hcp@3.0.3.jsii.tgz"
+            "provider-hcp@4.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_hcp": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdktf>=0.15.0, <0.16.0",
+        "cdktf>=0.16.0, <0.17.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.79.0, <2.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/aws_network_peering/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/aws_network_peering/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_aws_network_peering`
 
-Refer to the Terraform Registory for docs: [`hcp_aws_network_peering`](https://www.terraform.io/docs/providers/hcp/r/aws_network_peering).
+Refer to the Terraform Registory for docs: [`hcp_aws_network_peering`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,47 +22,47 @@
 
 
 class AwsNetworkPeering(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.awsNetworkPeering.AwsNetworkPeering",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering hcp_aws_network_peering}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering hcp_aws_network_peering}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         hvn_id: builtins.str,
         peer_account_id: builtins.str,
         peering_id: builtins.str,
         peer_vpc_id: builtins.str,
         peer_vpc_region: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["AwsNetworkPeeringTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering hcp_aws_network_peering} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering hcp_aws_network_peering} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#hvn_id AwsNetworkPeering#hvn_id}
-        :param peer_account_id: The account ID of the peer VPC in AWS. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#peer_account_id AwsNetworkPeering#peer_account_id}
-        :param peering_id: The ID of the network peering. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#peering_id AwsNetworkPeering#peering_id}
-        :param peer_vpc_id: The ID of the peer VPC in AWS. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#peer_vpc_id AwsNetworkPeering#peer_vpc_id}
-        :param peer_vpc_region: The region of the peer VPC in AWS. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#peer_vpc_region AwsNetworkPeering#peer_vpc_region}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#id AwsNetworkPeering#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#timeouts AwsNetworkPeering#timeouts}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#hvn_id AwsNetworkPeering#hvn_id}
+        :param peer_account_id: The account ID of the peer VPC in AWS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#peer_account_id AwsNetworkPeering#peer_account_id}
+        :param peering_id: The ID of the network peering. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#peering_id AwsNetworkPeering#peering_id}
+        :param peer_vpc_id: The ID of the peer VPC in AWS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#peer_vpc_id AwsNetworkPeering#peer_vpc_id}
+        :param peer_vpc_region: The region of the peer VPC in AWS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#peer_vpc_region AwsNetworkPeering#peer_vpc_region}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#id AwsNetworkPeering#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#timeouts AwsNetworkPeering#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -95,17 +95,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#create AwsNetworkPeering#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#default AwsNetworkPeering#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#delete AwsNetworkPeering#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#create AwsNetworkPeering#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#default AwsNetworkPeering#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#delete AwsNetworkPeering#delete}.
         '''
         value = AwsNetworkPeeringTimeouts(
             create=create, default=default, delete=delete
         )
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
@@ -297,15 +297,15 @@
     },
 )
 class AwsNetworkPeeringConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         hvn_id: builtins.str,
         peer_account_id: builtins.str,
@@ -319,21 +319,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#hvn_id AwsNetworkPeering#hvn_id}
-        :param peer_account_id: The account ID of the peer VPC in AWS. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#peer_account_id AwsNetworkPeering#peer_account_id}
-        :param peering_id: The ID of the network peering. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#peering_id AwsNetworkPeering#peering_id}
-        :param peer_vpc_id: The ID of the peer VPC in AWS. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#peer_vpc_id AwsNetworkPeering#peer_vpc_id}
-        :param peer_vpc_region: The region of the peer VPC in AWS. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#peer_vpc_region AwsNetworkPeering#peer_vpc_region}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#id AwsNetworkPeering#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#timeouts AwsNetworkPeering#timeouts}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#hvn_id AwsNetworkPeering#hvn_id}
+        :param peer_account_id: The account ID of the peer VPC in AWS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#peer_account_id AwsNetworkPeering#peer_account_id}
+        :param peering_id: The ID of the network peering. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#peering_id AwsNetworkPeering#peering_id}
+        :param peer_vpc_id: The ID of the peer VPC in AWS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#peer_vpc_id AwsNetworkPeering#peer_vpc_id}
+        :param peer_vpc_region: The region of the peer VPC in AWS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#peer_vpc_region AwsNetworkPeering#peer_vpc_region}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#id AwsNetworkPeering#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#timeouts AwsNetworkPeering#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = AwsNetworkPeeringTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b9c17948df4b1bafb7d97d68e6ba1b74034b5b1e7e0ed633ac481576c3f6d8b4)
@@ -384,20 +384,22 @@
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
@@ -439,75 +441,75 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def hvn_id(self) -> builtins.str:
         '''The ID of the HashiCorp Virtual Network (HVN).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#hvn_id AwsNetworkPeering#hvn_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#hvn_id AwsNetworkPeering#hvn_id}
         '''
         result = self._values.get("hvn_id")
         assert result is not None, "Required property 'hvn_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peer_account_id(self) -> builtins.str:
         '''The account ID of the peer VPC in AWS.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#peer_account_id AwsNetworkPeering#peer_account_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#peer_account_id AwsNetworkPeering#peer_account_id}
         '''
         result = self._values.get("peer_account_id")
         assert result is not None, "Required property 'peer_account_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peering_id(self) -> builtins.str:
         '''The ID of the network peering.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#peering_id AwsNetworkPeering#peering_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#peering_id AwsNetworkPeering#peering_id}
         '''
         result = self._values.get("peering_id")
         assert result is not None, "Required property 'peering_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peer_vpc_id(self) -> builtins.str:
         '''The ID of the peer VPC in AWS.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#peer_vpc_id AwsNetworkPeering#peer_vpc_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#peer_vpc_id AwsNetworkPeering#peer_vpc_id}
         '''
         result = self._values.get("peer_vpc_id")
         assert result is not None, "Required property 'peer_vpc_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peer_vpc_region(self) -> builtins.str:
         '''The region of the peer VPC in AWS.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#peer_vpc_region AwsNetworkPeering#peer_vpc_region}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#peer_vpc_region AwsNetworkPeering#peer_vpc_region}
         '''
         result = self._values.get("peer_vpc_region")
         assert result is not None, "Required property 'peer_vpc_region' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#id AwsNetworkPeering#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#id AwsNetworkPeering#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["AwsNetworkPeeringTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#timeouts AwsNetworkPeering#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#timeouts AwsNetworkPeering#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["AwsNetworkPeeringTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -530,17 +532,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#create AwsNetworkPeering#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#default AwsNetworkPeering#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#delete AwsNetworkPeering#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#create AwsNetworkPeering#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#default AwsNetworkPeering#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#delete AwsNetworkPeering#delete}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b0806ef2cb0a231646e95e4e369115a214ea50b4cb68f673ea8486daac15fe09)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -549,27 +551,27 @@
         if default is not None:
             self._values["default"] = default
         if delete is not None:
             self._values["delete"] = delete
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#create AwsNetworkPeering#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#create AwsNetworkPeering#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#default AwsNetworkPeering#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#default AwsNetworkPeering#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_network_peering#delete AwsNetworkPeering#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_network_peering#delete AwsNetworkPeering#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -699,15 +701,15 @@
     peer_account_id: builtins.str,
     peering_id: builtins.str,
     peer_vpc_id: builtins.str,
     peer_vpc_region: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[AwsNetworkPeeringTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -748,15 +750,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__b9c17948df4b1bafb7d97d68e6ba1b74034b5b1e7e0ed633ac481576c3f6d8b4(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     hvn_id: builtins.str,
     peer_account_id: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/aws_transit_gateway_attachment/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/aws_transit_gateway_attachment/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_aws_transit_gateway_attachment`
 
-Refer to the Terraform Registory for docs: [`hcp_aws_transit_gateway_attachment`](https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment).
+Refer to the Terraform Registory for docs: [`hcp_aws_transit_gateway_attachment`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,45 +22,45 @@
 
 
 class AwsTransitGatewayAttachment(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.awsTransitGatewayAttachment.AwsTransitGatewayAttachment",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment hcp_aws_transit_gateway_attachment}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment hcp_aws_transit_gateway_attachment}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         hvn_id: builtins.str,
         resource_share_arn: builtins.str,
         transit_gateway_attachment_id: builtins.str,
         transit_gateway_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["AwsTransitGatewayAttachmentTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment hcp_aws_transit_gateway_attachment} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment hcp_aws_transit_gateway_attachment} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#hvn_id AwsTransitGatewayAttachment#hvn_id}
-        :param resource_share_arn: The Amazon Resource Name (ARN) of the Resource Share that is needed to grant HCP access to the transit gateway in AWS. The Resource Share should be associated with the HCP AWS account principal (see `aws_ram_principal_association <https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ram_principal_association>`_) and the transit gateway resource (see `aws_ram_resource_association <https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ram_resource_association>`_) Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#resource_share_arn AwsTransitGatewayAttachment#resource_share_arn}
-        :param transit_gateway_attachment_id: The user-settable name of the transit gateway attachment in HCP. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#transit_gateway_attachment_id AwsTransitGatewayAttachment#transit_gateway_attachment_id}
-        :param transit_gateway_id: The ID of the user-owned transit gateway in AWS. The AWS region of the transit gateway must match the HVN. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#transit_gateway_id AwsTransitGatewayAttachment#transit_gateway_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#id AwsTransitGatewayAttachment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#timeouts AwsTransitGatewayAttachment#timeouts}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#hvn_id AwsTransitGatewayAttachment#hvn_id}
+        :param resource_share_arn: The Amazon Resource Name (ARN) of the Resource Share that is needed to grant HCP access to the transit gateway in AWS. The Resource Share should be associated with the HCP AWS account principal (see `aws_ram_principal_association <https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ram_principal_association>`_) and the transit gateway resource (see `aws_ram_resource_association <https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ram_resource_association>`_) Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#resource_share_arn AwsTransitGatewayAttachment#resource_share_arn}
+        :param transit_gateway_attachment_id: The user-settable name of the transit gateway attachment in HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#transit_gateway_attachment_id AwsTransitGatewayAttachment#transit_gateway_attachment_id}
+        :param transit_gateway_id: The ID of the user-owned transit gateway in AWS. The AWS region of the transit gateway must match the HVN. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#transit_gateway_id AwsTransitGatewayAttachment#transit_gateway_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#id AwsTransitGatewayAttachment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#timeouts AwsTransitGatewayAttachment#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -92,17 +92,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#create AwsTransitGatewayAttachment#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#default AwsTransitGatewayAttachment#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#delete AwsTransitGatewayAttachment#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#create AwsTransitGatewayAttachment#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#default AwsTransitGatewayAttachment#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#delete AwsTransitGatewayAttachment#delete}.
         '''
         value = AwsTransitGatewayAttachmentTimeouts(
             create=create, default=default, delete=delete
         )
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
@@ -276,15 +276,15 @@
     },
 )
 class AwsTransitGatewayAttachmentConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         hvn_id: builtins.str,
         resource_share_arn: builtins.str,
@@ -297,20 +297,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#hvn_id AwsTransitGatewayAttachment#hvn_id}
-        :param resource_share_arn: The Amazon Resource Name (ARN) of the Resource Share that is needed to grant HCP access to the transit gateway in AWS. The Resource Share should be associated with the HCP AWS account principal (see `aws_ram_principal_association <https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ram_principal_association>`_) and the transit gateway resource (see `aws_ram_resource_association <https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ram_resource_association>`_) Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#resource_share_arn AwsTransitGatewayAttachment#resource_share_arn}
-        :param transit_gateway_attachment_id: The user-settable name of the transit gateway attachment in HCP. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#transit_gateway_attachment_id AwsTransitGatewayAttachment#transit_gateway_attachment_id}
-        :param transit_gateway_id: The ID of the user-owned transit gateway in AWS. The AWS region of the transit gateway must match the HVN. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#transit_gateway_id AwsTransitGatewayAttachment#transit_gateway_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#id AwsTransitGatewayAttachment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#timeouts AwsTransitGatewayAttachment#timeouts}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#hvn_id AwsTransitGatewayAttachment#hvn_id}
+        :param resource_share_arn: The Amazon Resource Name (ARN) of the Resource Share that is needed to grant HCP access to the transit gateway in AWS. The Resource Share should be associated with the HCP AWS account principal (see `aws_ram_principal_association <https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ram_principal_association>`_) and the transit gateway resource (see `aws_ram_resource_association <https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ram_resource_association>`_) Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#resource_share_arn AwsTransitGatewayAttachment#resource_share_arn}
+        :param transit_gateway_attachment_id: The user-settable name of the transit gateway attachment in HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#transit_gateway_attachment_id AwsTransitGatewayAttachment#transit_gateway_attachment_id}
+        :param transit_gateway_id: The ID of the user-owned transit gateway in AWS. The AWS region of the transit gateway must match the HVN. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#transit_gateway_id AwsTransitGatewayAttachment#transit_gateway_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#id AwsTransitGatewayAttachment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#timeouts AwsTransitGatewayAttachment#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = AwsTransitGatewayAttachmentTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e20715d2f0d81810af99b1e2ec8ab5ff9b9100521407d7dfa1313b227c18af53)
@@ -359,20 +359,22 @@
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
@@ -414,69 +416,69 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def hvn_id(self) -> builtins.str:
         '''The ID of the HashiCorp Virtual Network (HVN).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#hvn_id AwsTransitGatewayAttachment#hvn_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#hvn_id AwsTransitGatewayAttachment#hvn_id}
         '''
         result = self._values.get("hvn_id")
         assert result is not None, "Required property 'hvn_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def resource_share_arn(self) -> builtins.str:
         '''The Amazon Resource Name (ARN) of the Resource Share that is needed to grant HCP access to the transit gateway in AWS.
 
         The Resource Share should be associated with the HCP AWS account principal (see `aws_ram_principal_association <https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ram_principal_association>`_) and the transit gateway resource (see `aws_ram_resource_association <https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ram_resource_association>`_)
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#resource_share_arn AwsTransitGatewayAttachment#resource_share_arn}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#resource_share_arn AwsTransitGatewayAttachment#resource_share_arn}
         '''
         result = self._values.get("resource_share_arn")
         assert result is not None, "Required property 'resource_share_arn' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def transit_gateway_attachment_id(self) -> builtins.str:
         '''The user-settable name of the transit gateway attachment in HCP.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#transit_gateway_attachment_id AwsTransitGatewayAttachment#transit_gateway_attachment_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#transit_gateway_attachment_id AwsTransitGatewayAttachment#transit_gateway_attachment_id}
         '''
         result = self._values.get("transit_gateway_attachment_id")
         assert result is not None, "Required property 'transit_gateway_attachment_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def transit_gateway_id(self) -> builtins.str:
         '''The ID of the user-owned transit gateway in AWS.
 
         The AWS region of the transit gateway must match the HVN.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#transit_gateway_id AwsTransitGatewayAttachment#transit_gateway_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#transit_gateway_id AwsTransitGatewayAttachment#transit_gateway_id}
         '''
         result = self._values.get("transit_gateway_id")
         assert result is not None, "Required property 'transit_gateway_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#id AwsTransitGatewayAttachment#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#id AwsTransitGatewayAttachment#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["AwsTransitGatewayAttachmentTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#timeouts AwsTransitGatewayAttachment#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#timeouts AwsTransitGatewayAttachment#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["AwsTransitGatewayAttachmentTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -499,17 +501,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#create AwsTransitGatewayAttachment#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#default AwsTransitGatewayAttachment#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#delete AwsTransitGatewayAttachment#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#create AwsTransitGatewayAttachment#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#default AwsTransitGatewayAttachment#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#delete AwsTransitGatewayAttachment#delete}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ccdd66f27acdf06d50d9f4079bbf0ba1b927640ff31a49119b05b5c03c92f45d)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -518,27 +520,27 @@
         if default is not None:
             self._values["default"] = default
         if delete is not None:
             self._values["delete"] = delete
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#create AwsTransitGatewayAttachment#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#create AwsTransitGatewayAttachment#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#default AwsTransitGatewayAttachment#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#default AwsTransitGatewayAttachment#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/aws_transit_gateway_attachment#delete AwsTransitGatewayAttachment#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/aws_transit_gateway_attachment#delete AwsTransitGatewayAttachment#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -667,15 +669,15 @@
     hvn_id: builtins.str,
     resource_share_arn: builtins.str,
     transit_gateway_attachment_id: builtins.str,
     transit_gateway_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[AwsTransitGatewayAttachmentTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -710,15 +712,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__e20715d2f0d81810af99b1e2ec8ab5ff9b9100521407d7dfa1313b227c18af53(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     hvn_id: builtins.str,
     resource_share_arn: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/azure_peering_connection/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/azure_peering_connection/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_azure_peering_connection`
 
-Refer to the Terraform Registory for docs: [`hcp_azure_peering_connection`](https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection).
+Refer to the Terraform Registory for docs: [`hcp_azure_peering_connection`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class AzurePeeringConnection(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.azurePeeringConnection.AzurePeeringConnection",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection hcp_azure_peering_connection}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection hcp_azure_peering_connection}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         hvn_link: builtins.str,
@@ -39,34 +39,34 @@
         peer_subscription_id: builtins.str,
         peer_tenant_id: builtins.str,
         peer_vnet_name: builtins.str,
         peer_vnet_region: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["AzurePeeringConnectionTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection hcp_azure_peering_connection} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection hcp_azure_peering_connection} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#hvn_link AzurePeeringConnection#hvn_link}
-        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#peering_id AzurePeeringConnection#peering_id}
-        :param peer_resource_group_name: The resource group name of the peer VNet in Azure. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#peer_resource_group_name AzurePeeringConnection#peer_resource_group_name}
-        :param peer_subscription_id: The subscription ID of the peer VNet in Azure. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#peer_subscription_id AzurePeeringConnection#peer_subscription_id}
-        :param peer_tenant_id: The tenant ID of the peer VNet in Azure. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#peer_tenant_id AzurePeeringConnection#peer_tenant_id}
-        :param peer_vnet_name: The name of the peer VNet in Azure. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#peer_vnet_name AzurePeeringConnection#peer_vnet_name}
-        :param peer_vnet_region: The region of the peer VNet in Azure. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#peer_vnet_region AzurePeeringConnection#peer_vnet_region}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#id AzurePeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#timeouts AzurePeeringConnection#timeouts}
+        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#hvn_link AzurePeeringConnection#hvn_link}
+        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#peering_id AzurePeeringConnection#peering_id}
+        :param peer_resource_group_name: The resource group name of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#peer_resource_group_name AzurePeeringConnection#peer_resource_group_name}
+        :param peer_subscription_id: The subscription ID of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#peer_subscription_id AzurePeeringConnection#peer_subscription_id}
+        :param peer_tenant_id: The tenant ID of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#peer_tenant_id AzurePeeringConnection#peer_tenant_id}
+        :param peer_vnet_name: The name of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#peer_vnet_name AzurePeeringConnection#peer_vnet_name}
+        :param peer_vnet_region: The region of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#peer_vnet_region AzurePeeringConnection#peer_vnet_region}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#id AzurePeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#timeouts AzurePeeringConnection#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -101,17 +101,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#create AzurePeeringConnection#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#default AzurePeeringConnection#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#delete AzurePeeringConnection#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#create AzurePeeringConnection#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#default AzurePeeringConnection#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#delete AzurePeeringConnection#delete}.
         '''
         value = AzurePeeringConnectionTimeouts(
             create=create, default=default, delete=delete
         )
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
@@ -344,15 +344,15 @@
     },
 )
 class AzurePeeringConnectionConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         hvn_link: builtins.str,
         peering_id: builtins.str,
@@ -368,23 +368,23 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#hvn_link AzurePeeringConnection#hvn_link}
-        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#peering_id AzurePeeringConnection#peering_id}
-        :param peer_resource_group_name: The resource group name of the peer VNet in Azure. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#peer_resource_group_name AzurePeeringConnection#peer_resource_group_name}
-        :param peer_subscription_id: The subscription ID of the peer VNet in Azure. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#peer_subscription_id AzurePeeringConnection#peer_subscription_id}
-        :param peer_tenant_id: The tenant ID of the peer VNet in Azure. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#peer_tenant_id AzurePeeringConnection#peer_tenant_id}
-        :param peer_vnet_name: The name of the peer VNet in Azure. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#peer_vnet_name AzurePeeringConnection#peer_vnet_name}
-        :param peer_vnet_region: The region of the peer VNet in Azure. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#peer_vnet_region AzurePeeringConnection#peer_vnet_region}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#id AzurePeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#timeouts AzurePeeringConnection#timeouts}
+        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#hvn_link AzurePeeringConnection#hvn_link}
+        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#peering_id AzurePeeringConnection#peering_id}
+        :param peer_resource_group_name: The resource group name of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#peer_resource_group_name AzurePeeringConnection#peer_resource_group_name}
+        :param peer_subscription_id: The subscription ID of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#peer_subscription_id AzurePeeringConnection#peer_subscription_id}
+        :param peer_tenant_id: The tenant ID of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#peer_tenant_id AzurePeeringConnection#peer_tenant_id}
+        :param peer_vnet_name: The name of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#peer_vnet_name AzurePeeringConnection#peer_vnet_name}
+        :param peer_vnet_region: The region of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#peer_vnet_region AzurePeeringConnection#peer_vnet_region}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#id AzurePeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#timeouts AzurePeeringConnection#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = AzurePeeringConnectionTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__fdeca02ceccf49e104c97dbf97368fcb5bf7c3b9bdbe2658f3fe03d7beaf4990)
@@ -439,20 +439,22 @@
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
@@ -494,95 +496,95 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def hvn_link(self) -> builtins.str:
         '''The ``self_link`` of the HashiCorp Virtual Network (HVN).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#hvn_link AzurePeeringConnection#hvn_link}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#hvn_link AzurePeeringConnection#hvn_link}
         '''
         result = self._values.get("hvn_link")
         assert result is not None, "Required property 'hvn_link' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peering_id(self) -> builtins.str:
         '''The ID of the peering connection.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#peering_id AzurePeeringConnection#peering_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#peering_id AzurePeeringConnection#peering_id}
         '''
         result = self._values.get("peering_id")
         assert result is not None, "Required property 'peering_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peer_resource_group_name(self) -> builtins.str:
         '''The resource group name of the peer VNet in Azure.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#peer_resource_group_name AzurePeeringConnection#peer_resource_group_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#peer_resource_group_name AzurePeeringConnection#peer_resource_group_name}
         '''
         result = self._values.get("peer_resource_group_name")
         assert result is not None, "Required property 'peer_resource_group_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peer_subscription_id(self) -> builtins.str:
         '''The subscription ID of the peer VNet in Azure.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#peer_subscription_id AzurePeeringConnection#peer_subscription_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#peer_subscription_id AzurePeeringConnection#peer_subscription_id}
         '''
         result = self._values.get("peer_subscription_id")
         assert result is not None, "Required property 'peer_subscription_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peer_tenant_id(self) -> builtins.str:
         '''The tenant ID of the peer VNet in Azure.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#peer_tenant_id AzurePeeringConnection#peer_tenant_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#peer_tenant_id AzurePeeringConnection#peer_tenant_id}
         '''
         result = self._values.get("peer_tenant_id")
         assert result is not None, "Required property 'peer_tenant_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peer_vnet_name(self) -> builtins.str:
         '''The name of the peer VNet in Azure.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#peer_vnet_name AzurePeeringConnection#peer_vnet_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#peer_vnet_name AzurePeeringConnection#peer_vnet_name}
         '''
         result = self._values.get("peer_vnet_name")
         assert result is not None, "Required property 'peer_vnet_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peer_vnet_region(self) -> builtins.str:
         '''The region of the peer VNet in Azure.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#peer_vnet_region AzurePeeringConnection#peer_vnet_region}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#peer_vnet_region AzurePeeringConnection#peer_vnet_region}
         '''
         result = self._values.get("peer_vnet_region")
         assert result is not None, "Required property 'peer_vnet_region' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#id AzurePeeringConnection#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#id AzurePeeringConnection#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["AzurePeeringConnectionTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#timeouts AzurePeeringConnection#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#timeouts AzurePeeringConnection#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["AzurePeeringConnectionTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -605,17 +607,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#create AzurePeeringConnection#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#default AzurePeeringConnection#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#delete AzurePeeringConnection#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#create AzurePeeringConnection#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#default AzurePeeringConnection#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#delete AzurePeeringConnection#delete}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__127f56bb37ab835fef1b18188f7621a124d0fb401d1e629d1300d24f99ad3d39)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -624,27 +626,27 @@
         if default is not None:
             self._values["default"] = default
         if delete is not None:
             self._values["delete"] = delete
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#create AzurePeeringConnection#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#create AzurePeeringConnection#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#default AzurePeeringConnection#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#default AzurePeeringConnection#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/azure_peering_connection#delete AzurePeeringConnection#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/azure_peering_connection#delete AzurePeeringConnection#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -776,15 +778,15 @@
     peer_subscription_id: builtins.str,
     peer_tenant_id: builtins.str,
     peer_vnet_name: builtins.str,
     peer_vnet_region: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[AzurePeeringConnectionTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -837,15 +839,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__fdeca02ceccf49e104c97dbf97368fcb5bf7c3b9bdbe2658f3fe03d7beaf4990(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     hvn_link: builtins.str,
     peering_id: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/boundary_cluster/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/boundary_cluster/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_boundary_cluster`
 
-Refer to the Terraform Registory for docs: [`hcp_boundary_cluster`](https://www.terraform.io/docs/providers/hcp/r/boundary_cluster).
+Refer to the Terraform Registory for docs: [`hcp_boundary_cluster`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,43 +22,43 @@
 
 
 class BoundaryCluster(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.boundaryCluster.BoundaryCluster",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster hcp_boundary_cluster}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster hcp_boundary_cluster}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_id: builtins.str,
         password: builtins.str,
         username: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["BoundaryClusterTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster hcp_boundary_cluster} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster hcp_boundary_cluster} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_id: The ID of the Boundary cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#cluster_id BoundaryCluster#cluster_id}
-        :param password: The password of the initial admin user. This must be at least 8 characters in length. Note that this may show up in logs, and it will be stored in the state file. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#password BoundaryCluster#password}
-        :param username: The username of the initial admin user. This must be at least 3 characters in length, alphanumeric, hyphen, or period. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#username BoundaryCluster#username}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#id BoundaryCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#timeouts BoundaryCluster#timeouts}
+        :param cluster_id: The ID of the Boundary cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#cluster_id BoundaryCluster#cluster_id}
+        :param password: The password of the initial admin user. This must be at least 8 characters in length. Note that this may show up in logs, and it will be stored in the state file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#password BoundaryCluster#password}
+        :param username: The username of the initial admin user. This must be at least 3 characters in length, alphanumeric, hyphen, or period. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#username BoundaryCluster#username}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#id BoundaryCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#timeouts BoundaryCluster#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -89,17 +89,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#create BoundaryCluster#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#default BoundaryCluster#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#delete BoundaryCluster#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#create BoundaryCluster#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#default BoundaryCluster#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#delete BoundaryCluster#delete}.
         '''
         value = BoundaryClusterTimeouts(create=create, default=default, delete=delete)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -233,15 +233,15 @@
     },
 )
 class BoundaryClusterConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         cluster_id: builtins.str,
         password: builtins.str,
@@ -253,19 +253,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_id: The ID of the Boundary cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#cluster_id BoundaryCluster#cluster_id}
-        :param password: The password of the initial admin user. This must be at least 8 characters in length. Note that this may show up in logs, and it will be stored in the state file. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#password BoundaryCluster#password}
-        :param username: The username of the initial admin user. This must be at least 3 characters in length, alphanumeric, hyphen, or period. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#username BoundaryCluster#username}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#id BoundaryCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#timeouts BoundaryCluster#timeouts}
+        :param cluster_id: The ID of the Boundary cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#cluster_id BoundaryCluster#cluster_id}
+        :param password: The password of the initial admin user. This must be at least 8 characters in length. Note that this may show up in logs, and it will be stored in the state file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#password BoundaryCluster#password}
+        :param username: The username of the initial admin user. This must be at least 3 characters in length, alphanumeric, hyphen, or period. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#username BoundaryCluster#username}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#id BoundaryCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#timeouts BoundaryCluster#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = BoundaryClusterTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d6a42c8435422f6174ef4b14850c898cf15aef2c0f59ff51f8537eff8217911b)
@@ -312,20 +312,22 @@
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
@@ -367,59 +369,59 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cluster_id(self) -> builtins.str:
         '''The ID of the Boundary cluster.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#cluster_id BoundaryCluster#cluster_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#cluster_id BoundaryCluster#cluster_id}
         '''
         result = self._values.get("cluster_id")
         assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def password(self) -> builtins.str:
         '''The password of the initial admin user.
 
         This must be at least 8 characters in length. Note that this may show up in logs, and it will be stored in the state file.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#password BoundaryCluster#password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#password BoundaryCluster#password}
         '''
         result = self._values.get("password")
         assert result is not None, "Required property 'password' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def username(self) -> builtins.str:
         '''The username of the initial admin user.
 
         This must be at least 3 characters in length, alphanumeric, hyphen, or period.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#username BoundaryCluster#username}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#username BoundaryCluster#username}
         '''
         result = self._values.get("username")
         assert result is not None, "Required property 'username' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#id BoundaryCluster#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#id BoundaryCluster#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["BoundaryClusterTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#timeouts BoundaryCluster#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#timeouts BoundaryCluster#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["BoundaryClusterTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -442,17 +444,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#create BoundaryCluster#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#default BoundaryCluster#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#delete BoundaryCluster#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#create BoundaryCluster#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#default BoundaryCluster#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#delete BoundaryCluster#delete}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f1df35e6c2ce2e7de0ee92af3344b57d6ac6a21e84b62284e97df14a42ec523f)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -461,27 +463,27 @@
         if default is not None:
             self._values["default"] = default
         if delete is not None:
             self._values["delete"] = delete
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#create BoundaryCluster#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#create BoundaryCluster#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#default BoundaryCluster#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#default BoundaryCluster#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/boundary_cluster#delete BoundaryCluster#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/boundary_cluster#delete BoundaryCluster#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -609,15 +611,15 @@
     *,
     cluster_id: builtins.str,
     password: builtins.str,
     username: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[BoundaryClusterTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -646,15 +648,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__d6a42c8435422f6174ef4b14850c898cf15aef2c0f59ff51f8537eff8217911b(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     cluster_id: builtins.str,
     password: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/consul_cluster/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/consul_cluster/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_consul_cluster`
 
-Refer to the Terraform Registory for docs: [`hcp_consul_cluster`](https://www.terraform.io/docs/providers/hcp/r/consul_cluster).
+Refer to the Terraform Registory for docs: [`hcp_consul_cluster`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class ConsulCluster(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.consulCluster.ConsulCluster",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster hcp_consul_cluster}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster hcp_consul_cluster}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_id: builtins.str,
@@ -43,38 +43,38 @@
         ip_allowlist: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["ConsulClusterIpAllowlist", typing.Dict[builtins.str, typing.Any]]]]] = None,
         min_consul_version: typing.Optional[builtins.str] = None,
         primary_link: typing.Optional[builtins.str] = None,
         public_endpoint: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         size: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["ConsulClusterTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster hcp_consul_cluster} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster hcp_consul_cluster} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#cluster_id ConsulCluster#cluster_id}
-        :param hvn_id: The ID of the HVN this HCP Consul cluster is associated to. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#hvn_id ConsulCluster#hvn_id}
-        :param tier: The tier that the HCP Consul cluster will be provisioned as. Only ``development``, ``standard`` and ``plus`` are available at this time. See `pricing information <https://www.hashicorp.com/products/consul/pricing>`_. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#tier ConsulCluster#tier}
-        :param auto_hvn_to_hvn_peering: Enables automatic HVN to HVN peering when creating a secondary cluster in a federation. The alternative to using the auto-accept feature is to create an ```hcp_hvn_peering_connection`` <hvn_peering_connection.md>`_ resource that explicitly defines the HVN resources that are allowed to communicate with each other. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#auto_hvn_to_hvn_peering ConsulCluster#auto_hvn_to_hvn_peering}
-        :param connect_enabled: Denotes the Consul connect feature should be enabled for this cluster. Default to true. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#connect_enabled ConsulCluster#connect_enabled}
-        :param datacenter: The Consul data center name of the cluster. If not specified, it is defaulted to the value of ``cluster_id``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#datacenter ConsulCluster#datacenter}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#id ConsulCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param ip_allowlist: ip_allowlist block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#ip_allowlist ConsulCluster#ip_allowlist}
-        :param min_consul_version: The minimum Consul patch version of the cluster. Allows only the rightmost version component to increment (E.g: ``1.13.0`` will allow installation of ``1.13.2`` and ``1.13.3`` etc., but not ``1.14.0``). If not specified, it is defaulted to the version that is currently recommended by HCP. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#min_consul_version ConsulCluster#min_consul_version}
-        :param primary_link: The ``self_link`` of the HCP Consul cluster which is the primary in the federation setup with this HCP Consul cluster. If not specified, it is a standalone cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#primary_link ConsulCluster#primary_link}
-        :param public_endpoint: Denotes that the cluster has a public endpoint for the Consul UI. Defaults to false. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#public_endpoint ConsulCluster#public_endpoint}
-        :param size: The t-shirt size representation of each server VM that this Consul cluster is provisioned with. Valid option for development tier - ``x_small``. Valid options for other tiers - ``small``, ``medium``, ``large``. For more details - https://cloud.hashicorp.com/pricing/consul. Upgrading the size of a cluster after creation is allowed. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#size ConsulCluster#size}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#timeouts ConsulCluster#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#cluster_id ConsulCluster#cluster_id}
+        :param hvn_id: The ID of the HVN this HCP Consul cluster is associated to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#hvn_id ConsulCluster#hvn_id}
+        :param tier: The tier that the HCP Consul cluster will be provisioned as. Only ``development``, ``standard`` and ``plus`` are available at this time. See `pricing information <https://www.hashicorp.com/products/consul/pricing>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#tier ConsulCluster#tier}
+        :param auto_hvn_to_hvn_peering: Enables automatic HVN to HVN peering when creating a secondary cluster in a federation. The alternative to using the auto-accept feature is to create an ```hcp_hvn_peering_connection`` <hvn_peering_connection.md>`_ resource that explicitly defines the HVN resources that are allowed to communicate with each other. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#auto_hvn_to_hvn_peering ConsulCluster#auto_hvn_to_hvn_peering}
+        :param connect_enabled: Denotes the Consul connect feature should be enabled for this cluster. Default to true. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#connect_enabled ConsulCluster#connect_enabled}
+        :param datacenter: The Consul data center name of the cluster. If not specified, it is defaulted to the value of ``cluster_id``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#datacenter ConsulCluster#datacenter}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#id ConsulCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param ip_allowlist: ip_allowlist block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#ip_allowlist ConsulCluster#ip_allowlist}
+        :param min_consul_version: The minimum Consul patch version of the cluster. Allows only the rightmost version component to increment (E.g: ``1.13.0`` will allow installation of ``1.13.2`` and ``1.13.3`` etc., but not ``1.14.0``). If not specified, it is defaulted to the version that is currently recommended by HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#min_consul_version ConsulCluster#min_consul_version}
+        :param primary_link: The ``self_link`` of the HCP Consul cluster which is the primary in the federation setup with this HCP Consul cluster. If not specified, it is a standalone cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#primary_link ConsulCluster#primary_link}
+        :param public_endpoint: Denotes that the cluster has a public endpoint for the Consul UI. Defaults to false. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#public_endpoint ConsulCluster#public_endpoint}
+        :param size: The t-shirt size representation of each server VM that this Consul cluster is provisioned with. Valid option for development tier - ``x_small``. Valid options for other tiers - ``small``, ``medium``, ``large``. For more details - https://cloud.hashicorp.com/pricing/consul. Upgrading the size of a cluster after creation is allowed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#size ConsulCluster#size}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#timeouts ConsulCluster#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -127,18 +127,18 @@
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#create ConsulCluster#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#default ConsulCluster#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#delete ConsulCluster#delete}.
-        :param update: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#update ConsulCluster#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#create ConsulCluster#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#default ConsulCluster#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#delete ConsulCluster#delete}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#update ConsulCluster#update}.
         '''
         value = ConsulClusterTimeouts(
             create=create, default=default, delete=delete, update=update
         )
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
@@ -536,15 +536,15 @@
     },
 )
 class ConsulClusterConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         cluster_id: builtins.str,
         hvn_id: builtins.str,
@@ -564,27 +564,27 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#cluster_id ConsulCluster#cluster_id}
-        :param hvn_id: The ID of the HVN this HCP Consul cluster is associated to. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#hvn_id ConsulCluster#hvn_id}
-        :param tier: The tier that the HCP Consul cluster will be provisioned as. Only ``development``, ``standard`` and ``plus`` are available at this time. See `pricing information <https://www.hashicorp.com/products/consul/pricing>`_. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#tier ConsulCluster#tier}
-        :param auto_hvn_to_hvn_peering: Enables automatic HVN to HVN peering when creating a secondary cluster in a federation. The alternative to using the auto-accept feature is to create an ```hcp_hvn_peering_connection`` <hvn_peering_connection.md>`_ resource that explicitly defines the HVN resources that are allowed to communicate with each other. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#auto_hvn_to_hvn_peering ConsulCluster#auto_hvn_to_hvn_peering}
-        :param connect_enabled: Denotes the Consul connect feature should be enabled for this cluster. Default to true. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#connect_enabled ConsulCluster#connect_enabled}
-        :param datacenter: The Consul data center name of the cluster. If not specified, it is defaulted to the value of ``cluster_id``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#datacenter ConsulCluster#datacenter}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#id ConsulCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param ip_allowlist: ip_allowlist block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#ip_allowlist ConsulCluster#ip_allowlist}
-        :param min_consul_version: The minimum Consul patch version of the cluster. Allows only the rightmost version component to increment (E.g: ``1.13.0`` will allow installation of ``1.13.2`` and ``1.13.3`` etc., but not ``1.14.0``). If not specified, it is defaulted to the version that is currently recommended by HCP. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#min_consul_version ConsulCluster#min_consul_version}
-        :param primary_link: The ``self_link`` of the HCP Consul cluster which is the primary in the federation setup with this HCP Consul cluster. If not specified, it is a standalone cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#primary_link ConsulCluster#primary_link}
-        :param public_endpoint: Denotes that the cluster has a public endpoint for the Consul UI. Defaults to false. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#public_endpoint ConsulCluster#public_endpoint}
-        :param size: The t-shirt size representation of each server VM that this Consul cluster is provisioned with. Valid option for development tier - ``x_small``. Valid options for other tiers - ``small``, ``medium``, ``large``. For more details - https://cloud.hashicorp.com/pricing/consul. Upgrading the size of a cluster after creation is allowed. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#size ConsulCluster#size}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#timeouts ConsulCluster#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#cluster_id ConsulCluster#cluster_id}
+        :param hvn_id: The ID of the HVN this HCP Consul cluster is associated to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#hvn_id ConsulCluster#hvn_id}
+        :param tier: The tier that the HCP Consul cluster will be provisioned as. Only ``development``, ``standard`` and ``plus`` are available at this time. See `pricing information <https://www.hashicorp.com/products/consul/pricing>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#tier ConsulCluster#tier}
+        :param auto_hvn_to_hvn_peering: Enables automatic HVN to HVN peering when creating a secondary cluster in a federation. The alternative to using the auto-accept feature is to create an ```hcp_hvn_peering_connection`` <hvn_peering_connection.md>`_ resource that explicitly defines the HVN resources that are allowed to communicate with each other. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#auto_hvn_to_hvn_peering ConsulCluster#auto_hvn_to_hvn_peering}
+        :param connect_enabled: Denotes the Consul connect feature should be enabled for this cluster. Default to true. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#connect_enabled ConsulCluster#connect_enabled}
+        :param datacenter: The Consul data center name of the cluster. If not specified, it is defaulted to the value of ``cluster_id``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#datacenter ConsulCluster#datacenter}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#id ConsulCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param ip_allowlist: ip_allowlist block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#ip_allowlist ConsulCluster#ip_allowlist}
+        :param min_consul_version: The minimum Consul patch version of the cluster. Allows only the rightmost version component to increment (E.g: ``1.13.0`` will allow installation of ``1.13.2`` and ``1.13.3`` etc., but not ``1.14.0``). If not specified, it is defaulted to the version that is currently recommended by HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#min_consul_version ConsulCluster#min_consul_version}
+        :param primary_link: The ``self_link`` of the HCP Consul cluster which is the primary in the federation setup with this HCP Consul cluster. If not specified, it is a standalone cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#primary_link ConsulCluster#primary_link}
+        :param public_endpoint: Denotes that the cluster has a public endpoint for the Consul UI. Defaults to false. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#public_endpoint ConsulCluster#public_endpoint}
+        :param size: The t-shirt size representation of each server VM that this Consul cluster is provisioned with. Valid option for development tier - ``x_small``. Valid options for other tiers - ``small``, ``medium``, ``large``. For more details - https://cloud.hashicorp.com/pricing/consul. Upgrading the size of a cluster after creation is allowed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#size ConsulCluster#size}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#timeouts ConsulCluster#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = ConsulClusterTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e15a4aa3c9e2c590b1a7243a86035a6b7c3197aaded71d8b2ef48bed209d4f0a)
@@ -655,20 +655,22 @@
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
@@ -710,145 +712,145 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cluster_id(self) -> builtins.str:
         '''The ID of the HCP Consul cluster.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#cluster_id ConsulCluster#cluster_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#cluster_id ConsulCluster#cluster_id}
         '''
         result = self._values.get("cluster_id")
         assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def hvn_id(self) -> builtins.str:
         '''The ID of the HVN this HCP Consul cluster is associated to.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#hvn_id ConsulCluster#hvn_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#hvn_id ConsulCluster#hvn_id}
         '''
         result = self._values.get("hvn_id")
         assert result is not None, "Required property 'hvn_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def tier(self) -> builtins.str:
         '''The tier that the HCP Consul cluster will be provisioned as.
 
         Only ``development``, ``standard`` and ``plus`` are available at this time. See `pricing information <https://www.hashicorp.com/products/consul/pricing>`_.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#tier ConsulCluster#tier}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#tier ConsulCluster#tier}
         '''
         result = self._values.get("tier")
         assert result is not None, "Required property 'tier' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def auto_hvn_to_hvn_peering(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Enables automatic HVN to HVN peering when creating a secondary cluster in a federation.
 
         The alternative to using the auto-accept feature is to create an ```hcp_hvn_peering_connection`` <hvn_peering_connection.md>`_ resource that explicitly defines the HVN resources that are allowed to communicate with each other.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#auto_hvn_to_hvn_peering ConsulCluster#auto_hvn_to_hvn_peering}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#auto_hvn_to_hvn_peering ConsulCluster#auto_hvn_to_hvn_peering}
         '''
         result = self._values.get("auto_hvn_to_hvn_peering")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def connect_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Denotes the Consul connect feature should be enabled for this cluster.  Default to true.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#connect_enabled ConsulCluster#connect_enabled}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#connect_enabled ConsulCluster#connect_enabled}
         '''
         result = self._values.get("connect_enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def datacenter(self) -> typing.Optional[builtins.str]:
         '''The Consul data center name of the cluster. If not specified, it is defaulted to the value of ``cluster_id``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#datacenter ConsulCluster#datacenter}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#datacenter ConsulCluster#datacenter}
         '''
         result = self._values.get("datacenter")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#id ConsulCluster#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#id ConsulCluster#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ip_allowlist(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ConsulClusterIpAllowlist"]]]:
         '''ip_allowlist block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#ip_allowlist ConsulCluster#ip_allowlist}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#ip_allowlist ConsulCluster#ip_allowlist}
         '''
         result = self._values.get("ip_allowlist")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ConsulClusterIpAllowlist"]]], result)
 
     @builtins.property
     def min_consul_version(self) -> typing.Optional[builtins.str]:
         '''The minimum Consul patch version of the cluster.
 
         Allows only the rightmost version component to increment (E.g: ``1.13.0`` will allow installation of ``1.13.2`` and ``1.13.3`` etc., but not ``1.14.0``). If not specified, it is defaulted to the version that is currently recommended by HCP.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#min_consul_version ConsulCluster#min_consul_version}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#min_consul_version ConsulCluster#min_consul_version}
         '''
         result = self._values.get("min_consul_version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def primary_link(self) -> typing.Optional[builtins.str]:
         '''The ``self_link`` of the HCP Consul cluster which is the primary in the federation setup with this HCP Consul cluster.
 
         If not specified, it is a standalone cluster.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#primary_link ConsulCluster#primary_link}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#primary_link ConsulCluster#primary_link}
         '''
         result = self._values.get("primary_link")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def public_endpoint(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Denotes that the cluster has a public endpoint for the Consul UI. Defaults to false.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#public_endpoint ConsulCluster#public_endpoint}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#public_endpoint ConsulCluster#public_endpoint}
         '''
         result = self._values.get("public_endpoint")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def size(self) -> typing.Optional[builtins.str]:
         '''The t-shirt size representation of each server VM that this Consul cluster is provisioned with.
 
         Valid option for development tier - ``x_small``. Valid options for other tiers - ``small``, ``medium``, ``large``. For more details - https://cloud.hashicorp.com/pricing/consul. Upgrading the size of a cluster after creation is allowed.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#size ConsulCluster#size}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#size ConsulCluster#size}
         '''
         result = self._values.get("size")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["ConsulClusterTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#timeouts ConsulCluster#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#timeouts ConsulCluster#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["ConsulClusterTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -870,16 +872,16 @@
     def __init__(
         self,
         *,
         address: builtins.str,
         description: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param address: IP address range in CIDR notation. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#address ConsulCluster#address}
-        :param description: Description to help identify source (maximum 255 chars). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#description ConsulCluster#description}
+        :param address: IP address range in CIDR notation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#address ConsulCluster#address}
+        :param description: Description to help identify source (maximum 255 chars). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#description ConsulCluster#description}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5930d5372f601a65bf165fe531bcc46f44dc92b49c5e477afe81fb26d98a42e5)
             check_type(argname="argument address", value=address, expected_type=type_hints["address"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "address": address,
@@ -887,25 +889,25 @@
         if description is not None:
             self._values["description"] = description
 
     @builtins.property
     def address(self) -> builtins.str:
         '''IP address range in CIDR notation.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#address ConsulCluster#address}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#address ConsulCluster#address}
         '''
         result = self._values.get("address")
         assert result is not None, "Required property 'address' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''Description to help identify source (maximum 255 chars).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#description ConsulCluster#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#description ConsulCluster#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1106,18 +1108,18 @@
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#create ConsulCluster#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#default ConsulCluster#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#delete ConsulCluster#delete}.
-        :param update: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#update ConsulCluster#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#create ConsulCluster#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#default ConsulCluster#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#delete ConsulCluster#delete}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#update ConsulCluster#update}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8f659835463a84e60ea15cd993c4c5de4055fb363e403183b9791dcfc6d21d85)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
             check_type(argname="argument update", value=update, expected_type=type_hints["update"])
@@ -1129,33 +1131,33 @@
         if delete is not None:
             self._values["delete"] = delete
         if update is not None:
             self._values["update"] = update
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#create ConsulCluster#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#create ConsulCluster#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#default ConsulCluster#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#default ConsulCluster#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#delete ConsulCluster#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#delete ConsulCluster#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def update(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster#update ConsulCluster#update}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster#update ConsulCluster#update}.'''
         result = self._values.get("update")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -1315,15 +1317,15 @@
     ip_allowlist: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[ConsulClusterIpAllowlist, typing.Dict[builtins.str, typing.Any]]]]] = None,
     min_consul_version: typing.Optional[builtins.str] = None,
     primary_link: typing.Optional[builtins.str] = None,
     public_endpoint: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     size: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[ConsulClusterTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -1400,15 +1402,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__e15a4aa3c9e2c590b1a7243a86035a6b7c3197aaded71d8b2ef48bed209d4f0a(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     cluster_id: builtins.str,
     hvn_id: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/consul_cluster_root_token/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/consul_cluster_root_token/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_consul_cluster_root_token`
 
-Refer to the Terraform Registory for docs: [`hcp_consul_cluster_root_token`](https://www.terraform.io/docs/providers/hcp/r/consul_cluster_root_token).
+Refer to the Terraform Registory for docs: [`hcp_consul_cluster_root_token`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster_root_token).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,39 +22,39 @@
 
 
 class ConsulClusterRootToken(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.consulClusterRootToken.ConsulClusterRootToken",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster_root_token hcp_consul_cluster_root_token}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster_root_token hcp_consul_cluster_root_token}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["ConsulClusterRootTokenTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster_root_token hcp_consul_cluster_root_token} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster_root_token hcp_consul_cluster_root_token} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster_root_token#cluster_id ConsulClusterRootToken#cluster_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster_root_token#id ConsulClusterRootToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster_root_token#timeouts ConsulClusterRootToken#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster_root_token#cluster_id ConsulClusterRootToken#cluster_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster_root_token#id ConsulClusterRootToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster_root_token#timeouts ConsulClusterRootToken#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -77,15 +77,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster_root_token#default ConsulClusterRootToken#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster_root_token#default ConsulClusterRootToken#default}.
         '''
         value = ConsulClusterRootTokenTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -183,15 +183,15 @@
     },
 )
 class ConsulClusterRootTokenConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         cluster_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
@@ -201,17 +201,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster_root_token#cluster_id ConsulClusterRootToken#cluster_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster_root_token#id ConsulClusterRootToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster_root_token#timeouts ConsulClusterRootToken#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster_root_token#cluster_id ConsulClusterRootToken#cluster_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster_root_token#id ConsulClusterRootToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster_root_token#timeouts ConsulClusterRootToken#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = ConsulClusterRootTokenTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0926c56dc948940e26333b91643ad320e4464a38f99d953c37e4f5a86c59f395)
@@ -254,20 +254,22 @@
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
@@ -309,35 +311,35 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cluster_id(self) -> builtins.str:
         '''The ID of the HCP Consul cluster.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster_root_token#cluster_id ConsulClusterRootToken#cluster_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster_root_token#cluster_id ConsulClusterRootToken#cluster_id}
         '''
         result = self._values.get("cluster_id")
         assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster_root_token#id ConsulClusterRootToken#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster_root_token#id ConsulClusterRootToken#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["ConsulClusterRootTokenTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster_root_token#timeouts ConsulClusterRootToken#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster_root_token#timeouts ConsulClusterRootToken#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["ConsulClusterRootTokenTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -354,26 +356,26 @@
     jsii_type="@cdktf/provider-hcp.consulClusterRootToken.ConsulClusterRootTokenTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class ConsulClusterRootTokenTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster_root_token#default ConsulClusterRootToken#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster_root_token#default ConsulClusterRootToken#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d87a29510dda71b964e144ecd9ecd4c1a0d3c0b0f6eeacaf4c54503c6adea5cb)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_cluster_root_token#default ConsulClusterRootToken#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_cluster_root_token#default ConsulClusterRootToken#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -457,15 +459,15 @@
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     cluster_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[ConsulClusterRootTokenTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
 
 def _typecheckingstub__0926c56dc948940e26333b91643ad320e4464a38f99d953c37e4f5a86c59f395(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     cluster_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/consul_snapshot/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/consul_snapshot/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_consul_snapshot`
 
-Refer to the Terraform Registory for docs: [`hcp_consul_snapshot`](https://www.terraform.io/docs/providers/hcp/r/consul_snapshot).
+Refer to the Terraform Registory for docs: [`hcp_consul_snapshot`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,41 +22,41 @@
 
 
 class ConsulSnapshot(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.consulSnapshot.ConsulSnapshot",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot hcp_consul_snapshot}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot hcp_consul_snapshot}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_id: builtins.str,
         snapshot_name: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["ConsulSnapshotTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot hcp_consul_snapshot} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot hcp_consul_snapshot} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#cluster_id ConsulSnapshot#cluster_id}
-        :param snapshot_name: The name of the snapshot. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#snapshot_name ConsulSnapshot#snapshot_name}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#id ConsulSnapshot#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#timeouts ConsulSnapshot#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#cluster_id ConsulSnapshot#cluster_id}
+        :param snapshot_name: The name of the snapshot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#snapshot_name ConsulSnapshot#snapshot_name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#id ConsulSnapshot#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#timeouts ConsulSnapshot#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -87,18 +87,18 @@
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#create ConsulSnapshot#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#default ConsulSnapshot#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#delete ConsulSnapshot#delete}.
-        :param update: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#update ConsulSnapshot#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#create ConsulSnapshot#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#default ConsulSnapshot#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#delete ConsulSnapshot#delete}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#update ConsulSnapshot#update}.
         '''
         value = ConsulSnapshotTimeouts(
             create=create, default=default, delete=delete, update=update
         )
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
@@ -236,15 +236,15 @@
     },
 )
 class ConsulSnapshotConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         cluster_id: builtins.str,
         snapshot_name: builtins.str,
@@ -255,18 +255,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#cluster_id ConsulSnapshot#cluster_id}
-        :param snapshot_name: The name of the snapshot. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#snapshot_name ConsulSnapshot#snapshot_name}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#id ConsulSnapshot#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#timeouts ConsulSnapshot#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#cluster_id ConsulSnapshot#cluster_id}
+        :param snapshot_name: The name of the snapshot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#snapshot_name ConsulSnapshot#snapshot_name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#id ConsulSnapshot#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#timeouts ConsulSnapshot#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = ConsulSnapshotTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__407e2d5ef4ee09855675a8e1850926e063e9aa9defd2c3d0404764b6ddaf9375)
@@ -311,20 +311,22 @@
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
@@ -366,45 +368,45 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cluster_id(self) -> builtins.str:
         '''The ID of the HCP Consul cluster.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#cluster_id ConsulSnapshot#cluster_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#cluster_id ConsulSnapshot#cluster_id}
         '''
         result = self._values.get("cluster_id")
         assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def snapshot_name(self) -> builtins.str:
         '''The name of the snapshot.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#snapshot_name ConsulSnapshot#snapshot_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#snapshot_name ConsulSnapshot#snapshot_name}
         '''
         result = self._values.get("snapshot_name")
         assert result is not None, "Required property 'snapshot_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#id ConsulSnapshot#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#id ConsulSnapshot#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["ConsulSnapshotTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#timeouts ConsulSnapshot#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#timeouts ConsulSnapshot#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["ConsulSnapshotTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -433,18 +435,18 @@
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#create ConsulSnapshot#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#default ConsulSnapshot#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#delete ConsulSnapshot#delete}.
-        :param update: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#update ConsulSnapshot#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#create ConsulSnapshot#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#default ConsulSnapshot#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#delete ConsulSnapshot#delete}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#update ConsulSnapshot#update}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4e975142f34042561381f5a0050fa61ee7531532c88761b85e444bbe42f2fa5a)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
             check_type(argname="argument update", value=update, expected_type=type_hints["update"])
@@ -456,33 +458,33 @@
         if delete is not None:
             self._values["delete"] = delete
         if update is not None:
             self._values["update"] = update
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#create ConsulSnapshot#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#create ConsulSnapshot#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#default ConsulSnapshot#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#default ConsulSnapshot#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#delete ConsulSnapshot#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#delete ConsulSnapshot#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def update(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/consul_snapshot#update ConsulSnapshot#update}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/consul_snapshot#update ConsulSnapshot#update}.'''
         result = self._values.get("update")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -630,15 +632,15 @@
     id_: builtins.str,
     *,
     cluster_id: builtins.str,
     snapshot_name: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[ConsulSnapshotTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -661,15 +663,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__407e2d5ef4ee09855675a8e1850926e063e9aa9defd2c3d0404764b6ddaf9375(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     cluster_id: builtins.str,
     snapshot_name: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_aws_network_peering/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_aws_network_peering/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_aws_network_peering`
 
-Refer to the Terraform Registory for docs: [`data_hcp_aws_network_peering`](https://www.terraform.io/docs/providers/hcp/d/aws_network_peering).
+Refer to the Terraform Registory for docs: [`data_hcp_aws_network_peering`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_network_peering).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,43 +22,43 @@
 
 
 class DataHcpAwsNetworkPeering(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpAwsNetworkPeering.DataHcpAwsNetworkPeering",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/d/aws_network_peering hcp_aws_network_peering}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_network_peering hcp_aws_network_peering}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         hvn_id: builtins.str,
         peering_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcpAwsNetworkPeeringTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         wait_for_active_state: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/d/aws_network_peering hcp_aws_network_peering} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_network_peering hcp_aws_network_peering} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_network_peering#hvn_id DataHcpAwsNetworkPeering#hvn_id}
-        :param peering_id: The ID of the network peering. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_network_peering#peering_id DataHcpAwsNetworkPeering#peering_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_network_peering#id DataHcpAwsNetworkPeering#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_network_peering#timeouts DataHcpAwsNetworkPeering#timeouts}
-        :param wait_for_active_state: If ``true``, Terraform will wait for the network peering to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_network_peering#wait_for_active_state DataHcpAwsNetworkPeering#wait_for_active_state}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_network_peering#hvn_id DataHcpAwsNetworkPeering#hvn_id}
+        :param peering_id: The ID of the network peering. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_network_peering#peering_id DataHcpAwsNetworkPeering#peering_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_network_peering#id DataHcpAwsNetworkPeering#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_network_peering#timeouts DataHcpAwsNetworkPeering#timeouts}
+        :param wait_for_active_state: If ``true``, Terraform will wait for the network peering to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_network_peering#wait_for_active_state DataHcpAwsNetworkPeering#wait_for_active_state}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -83,15 +83,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, read: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param read: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_network_peering#read DataHcpAwsNetworkPeering#read}.
+        :param read: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_network_peering#read DataHcpAwsNetworkPeering#read}.
         '''
         value = DataHcpAwsNetworkPeeringTimeouts(read=read)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -271,15 +271,15 @@
     },
 )
 class DataHcpAwsNetworkPeeringConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         hvn_id: builtins.str,
         peering_id: builtins.str,
@@ -291,19 +291,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_network_peering#hvn_id DataHcpAwsNetworkPeering#hvn_id}
-        :param peering_id: The ID of the network peering. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_network_peering#peering_id DataHcpAwsNetworkPeering#peering_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_network_peering#id DataHcpAwsNetworkPeering#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_network_peering#timeouts DataHcpAwsNetworkPeering#timeouts}
-        :param wait_for_active_state: If ``true``, Terraform will wait for the network peering to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_network_peering#wait_for_active_state DataHcpAwsNetworkPeering#wait_for_active_state}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_network_peering#hvn_id DataHcpAwsNetworkPeering#hvn_id}
+        :param peering_id: The ID of the network peering. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_network_peering#peering_id DataHcpAwsNetworkPeering#peering_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_network_peering#id DataHcpAwsNetworkPeering#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_network_peering#timeouts DataHcpAwsNetworkPeering#timeouts}
+        :param wait_for_active_state: If ``true``, Terraform will wait for the network peering to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_network_peering#wait_for_active_state DataHcpAwsNetworkPeering#wait_for_active_state}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpAwsNetworkPeeringTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__43949da3b11b0b9444af24cc57bdefdbcb02dc379fe0bee2128f98454251c2d5)
@@ -351,20 +351,22 @@
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
@@ -406,56 +408,56 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def hvn_id(self) -> builtins.str:
         '''The ID of the HashiCorp Virtual Network (HVN).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_network_peering#hvn_id DataHcpAwsNetworkPeering#hvn_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_network_peering#hvn_id DataHcpAwsNetworkPeering#hvn_id}
         '''
         result = self._values.get("hvn_id")
         assert result is not None, "Required property 'hvn_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peering_id(self) -> builtins.str:
         '''The ID of the network peering.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_network_peering#peering_id DataHcpAwsNetworkPeering#peering_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_network_peering#peering_id DataHcpAwsNetworkPeering#peering_id}
         '''
         result = self._values.get("peering_id")
         assert result is not None, "Required property 'peering_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_network_peering#id DataHcpAwsNetworkPeering#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_network_peering#id DataHcpAwsNetworkPeering#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpAwsNetworkPeeringTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_network_peering#timeouts DataHcpAwsNetworkPeering#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_network_peering#timeouts DataHcpAwsNetworkPeering#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpAwsNetworkPeeringTimeouts"], result)
 
     @builtins.property
     def wait_for_active_state(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If ``true``, Terraform will wait for the network peering to reach an ``ACTIVE`` state before continuing. Default ``false``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_network_peering#wait_for_active_state DataHcpAwsNetworkPeering#wait_for_active_state}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_network_peering#wait_for_active_state DataHcpAwsNetworkPeering#wait_for_active_state}
         '''
         result = self._values.get("wait_for_active_state")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -472,26 +474,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpAwsNetworkPeering.DataHcpAwsNetworkPeeringTimeouts",
     jsii_struct_bases=[],
     name_mapping={"read": "read"},
 )
 class DataHcpAwsNetworkPeeringTimeouts:
     def __init__(self, *, read: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param read: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_network_peering#read DataHcpAwsNetworkPeering#read}.
+        :param read: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_network_peering#read DataHcpAwsNetworkPeering#read}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4a4732455394dadd0b7d3991531e7ed17f2ce34ec0f53c7143fde4246e7972f2)
             check_type(argname="argument read", value=read, expected_type=type_hints["read"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if read is not None:
             self._values["read"] = read
 
     @builtins.property
     def read(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_network_peering#read DataHcpAwsNetworkPeering#read}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_network_peering#read DataHcpAwsNetworkPeering#read}.'''
         result = self._values.get("read")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -577,15 +579,15 @@
     *,
     hvn_id: builtins.str,
     peering_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcpAwsNetworkPeeringTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
     wait_for_active_state: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
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
@@ -614,15 +616,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__43949da3b11b0b9444af24cc57bdefdbcb02dc379fe0bee2128f98454251c2d5(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     hvn_id: builtins.str,
     peering_id: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_aws_transit_gateway_attachment/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_aws_transit_gateway_attachment/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_aws_transit_gateway_attachment`
 
-Refer to the Terraform Registory for docs: [`data_hcp_aws_transit_gateway_attachment`](https://www.terraform.io/docs/providers/hcp/d/aws_transit_gateway_attachment).
+Refer to the Terraform Registory for docs: [`data_hcp_aws_transit_gateway_attachment`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_transit_gateway_attachment).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,43 +22,43 @@
 
 
 class DataHcpAwsTransitGatewayAttachment(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpAwsTransitGatewayAttachment.DataHcpAwsTransitGatewayAttachment",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/d/aws_transit_gateway_attachment hcp_aws_transit_gateway_attachment}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_transit_gateway_attachment hcp_aws_transit_gateway_attachment}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         hvn_id: builtins.str,
         transit_gateway_attachment_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcpAwsTransitGatewayAttachmentTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         wait_for_active_state: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/d/aws_transit_gateway_attachment hcp_aws_transit_gateway_attachment} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_transit_gateway_attachment hcp_aws_transit_gateway_attachment} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_transit_gateway_attachment#hvn_id DataHcpAwsTransitGatewayAttachment#hvn_id}
-        :param transit_gateway_attachment_id: The user-settable name of the transit gateway attachment in HCP. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_transit_gateway_attachment#transit_gateway_attachment_id DataHcpAwsTransitGatewayAttachment#transit_gateway_attachment_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_transit_gateway_attachment#id DataHcpAwsTransitGatewayAttachment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_transit_gateway_attachment#timeouts DataHcpAwsTransitGatewayAttachment#timeouts}
-        :param wait_for_active_state: If ``true``, Terraform will wait for the transit gateway attachment to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_transit_gateway_attachment#wait_for_active_state DataHcpAwsTransitGatewayAttachment#wait_for_active_state}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_transit_gateway_attachment#hvn_id DataHcpAwsTransitGatewayAttachment#hvn_id}
+        :param transit_gateway_attachment_id: The user-settable name of the transit gateway attachment in HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_transit_gateway_attachment#transit_gateway_attachment_id DataHcpAwsTransitGatewayAttachment#transit_gateway_attachment_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_transit_gateway_attachment#id DataHcpAwsTransitGatewayAttachment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_transit_gateway_attachment#timeouts DataHcpAwsTransitGatewayAttachment#timeouts}
+        :param wait_for_active_state: If ``true``, Terraform will wait for the transit gateway attachment to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_transit_gateway_attachment#wait_for_active_state DataHcpAwsTransitGatewayAttachment#wait_for_active_state}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -83,15 +83,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_transit_gateway_attachment#default DataHcpAwsTransitGatewayAttachment#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_transit_gateway_attachment#default DataHcpAwsTransitGatewayAttachment#default}.
         '''
         value = DataHcpAwsTransitGatewayAttachmentTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -261,15 +261,15 @@
     },
 )
 class DataHcpAwsTransitGatewayAttachmentConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         hvn_id: builtins.str,
         transit_gateway_attachment_id: builtins.str,
@@ -281,19 +281,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_transit_gateway_attachment#hvn_id DataHcpAwsTransitGatewayAttachment#hvn_id}
-        :param transit_gateway_attachment_id: The user-settable name of the transit gateway attachment in HCP. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_transit_gateway_attachment#transit_gateway_attachment_id DataHcpAwsTransitGatewayAttachment#transit_gateway_attachment_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_transit_gateway_attachment#id DataHcpAwsTransitGatewayAttachment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_transit_gateway_attachment#timeouts DataHcpAwsTransitGatewayAttachment#timeouts}
-        :param wait_for_active_state: If ``true``, Terraform will wait for the transit gateway attachment to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_transit_gateway_attachment#wait_for_active_state DataHcpAwsTransitGatewayAttachment#wait_for_active_state}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_transit_gateway_attachment#hvn_id DataHcpAwsTransitGatewayAttachment#hvn_id}
+        :param transit_gateway_attachment_id: The user-settable name of the transit gateway attachment in HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_transit_gateway_attachment#transit_gateway_attachment_id DataHcpAwsTransitGatewayAttachment#transit_gateway_attachment_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_transit_gateway_attachment#id DataHcpAwsTransitGatewayAttachment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_transit_gateway_attachment#timeouts DataHcpAwsTransitGatewayAttachment#timeouts}
+        :param wait_for_active_state: If ``true``, Terraform will wait for the transit gateway attachment to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_transit_gateway_attachment#wait_for_active_state DataHcpAwsTransitGatewayAttachment#wait_for_active_state}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpAwsTransitGatewayAttachmentTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__363ded0d2931637094a88761d374e1998f400853e0f9fe567af0bc1d8931a7a2)
@@ -341,20 +341,22 @@
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
@@ -396,56 +398,56 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def hvn_id(self) -> builtins.str:
         '''The ID of the HashiCorp Virtual Network (HVN).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_transit_gateway_attachment#hvn_id DataHcpAwsTransitGatewayAttachment#hvn_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_transit_gateway_attachment#hvn_id DataHcpAwsTransitGatewayAttachment#hvn_id}
         '''
         result = self._values.get("hvn_id")
         assert result is not None, "Required property 'hvn_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def transit_gateway_attachment_id(self) -> builtins.str:
         '''The user-settable name of the transit gateway attachment in HCP.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_transit_gateway_attachment#transit_gateway_attachment_id DataHcpAwsTransitGatewayAttachment#transit_gateway_attachment_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_transit_gateway_attachment#transit_gateway_attachment_id DataHcpAwsTransitGatewayAttachment#transit_gateway_attachment_id}
         '''
         result = self._values.get("transit_gateway_attachment_id")
         assert result is not None, "Required property 'transit_gateway_attachment_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_transit_gateway_attachment#id DataHcpAwsTransitGatewayAttachment#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_transit_gateway_attachment#id DataHcpAwsTransitGatewayAttachment#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpAwsTransitGatewayAttachmentTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_transit_gateway_attachment#timeouts DataHcpAwsTransitGatewayAttachment#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_transit_gateway_attachment#timeouts DataHcpAwsTransitGatewayAttachment#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpAwsTransitGatewayAttachmentTimeouts"], result)
 
     @builtins.property
     def wait_for_active_state(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If ``true``, Terraform will wait for the transit gateway attachment to reach an ``ACTIVE`` state before continuing. Default ``false``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_transit_gateway_attachment#wait_for_active_state DataHcpAwsTransitGatewayAttachment#wait_for_active_state}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_transit_gateway_attachment#wait_for_active_state DataHcpAwsTransitGatewayAttachment#wait_for_active_state}
         '''
         result = self._values.get("wait_for_active_state")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -462,26 +464,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpAwsTransitGatewayAttachment.DataHcpAwsTransitGatewayAttachmentTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpAwsTransitGatewayAttachmentTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_transit_gateway_attachment#default DataHcpAwsTransitGatewayAttachment#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_transit_gateway_attachment#default DataHcpAwsTransitGatewayAttachment#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7f1272ea3ccd49ce428f535dea4ad39e95f9fe501d9aca38228c5aecea5b85f5)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/aws_transit_gateway_attachment#default DataHcpAwsTransitGatewayAttachment#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/aws_transit_gateway_attachment#default DataHcpAwsTransitGatewayAttachment#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -567,15 +569,15 @@
     *,
     hvn_id: builtins.str,
     transit_gateway_attachment_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcpAwsTransitGatewayAttachmentTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
     wait_for_active_state: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
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
@@ -604,15 +606,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__363ded0d2931637094a88761d374e1998f400853e0f9fe567af0bc1d8931a7a2(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     hvn_id: builtins.str,
     transit_gateway_attachment_id: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_azure_peering_connection/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_azure_peering_connection/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_azure_peering_connection`
 
-Refer to the Terraform Registory for docs: [`data_hcp_azure_peering_connection`](https://www.terraform.io/docs/providers/hcp/d/azure_peering_connection).
+Refer to the Terraform Registory for docs: [`data_hcp_azure_peering_connection`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/azure_peering_connection).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,43 +22,43 @@
 
 
 class DataHcpAzurePeeringConnection(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpAzurePeeringConnection.DataHcpAzurePeeringConnection",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/d/azure_peering_connection hcp_azure_peering_connection}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/azure_peering_connection hcp_azure_peering_connection}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         hvn_link: builtins.str,
         peering_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcpAzurePeeringConnectionTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         wait_for_active_state: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/d/azure_peering_connection hcp_azure_peering_connection} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/azure_peering_connection hcp_azure_peering_connection} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/azure_peering_connection#hvn_link DataHcpAzurePeeringConnection#hvn_link}
-        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/azure_peering_connection#peering_id DataHcpAzurePeeringConnection#peering_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/azure_peering_connection#id DataHcpAzurePeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/azure_peering_connection#timeouts DataHcpAzurePeeringConnection#timeouts}
-        :param wait_for_active_state: If ``true``, Terraform will wait for the peering connection to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/azure_peering_connection#wait_for_active_state DataHcpAzurePeeringConnection#wait_for_active_state}
+        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/azure_peering_connection#hvn_link DataHcpAzurePeeringConnection#hvn_link}
+        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/azure_peering_connection#peering_id DataHcpAzurePeeringConnection#peering_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/azure_peering_connection#id DataHcpAzurePeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/azure_peering_connection#timeouts DataHcpAzurePeeringConnection#timeouts}
+        :param wait_for_active_state: If ``true``, Terraform will wait for the peering connection to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/azure_peering_connection#wait_for_active_state DataHcpAzurePeeringConnection#wait_for_active_state}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -83,15 +83,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, read: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param read: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/azure_peering_connection#read DataHcpAzurePeeringConnection#read}.
+        :param read: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/azure_peering_connection#read DataHcpAzurePeeringConnection#read}.
         '''
         value = DataHcpAzurePeeringConnectionTimeouts(read=read)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -286,15 +286,15 @@
     },
 )
 class DataHcpAzurePeeringConnectionConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         hvn_link: builtins.str,
         peering_id: builtins.str,
@@ -306,19 +306,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/azure_peering_connection#hvn_link DataHcpAzurePeeringConnection#hvn_link}
-        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/azure_peering_connection#peering_id DataHcpAzurePeeringConnection#peering_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/azure_peering_connection#id DataHcpAzurePeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/azure_peering_connection#timeouts DataHcpAzurePeeringConnection#timeouts}
-        :param wait_for_active_state: If ``true``, Terraform will wait for the peering connection to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/azure_peering_connection#wait_for_active_state DataHcpAzurePeeringConnection#wait_for_active_state}
+        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/azure_peering_connection#hvn_link DataHcpAzurePeeringConnection#hvn_link}
+        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/azure_peering_connection#peering_id DataHcpAzurePeeringConnection#peering_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/azure_peering_connection#id DataHcpAzurePeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/azure_peering_connection#timeouts DataHcpAzurePeeringConnection#timeouts}
+        :param wait_for_active_state: If ``true``, Terraform will wait for the peering connection to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/azure_peering_connection#wait_for_active_state DataHcpAzurePeeringConnection#wait_for_active_state}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpAzurePeeringConnectionTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__bd4aba9c40f32574afd6b9f7bfd3bb022ad0157924dba691af2463b7fa0e49bd)
@@ -366,20 +366,22 @@
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
@@ -421,56 +423,56 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def hvn_link(self) -> builtins.str:
         '''The ``self_link`` of the HashiCorp Virtual Network (HVN).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/azure_peering_connection#hvn_link DataHcpAzurePeeringConnection#hvn_link}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/azure_peering_connection#hvn_link DataHcpAzurePeeringConnection#hvn_link}
         '''
         result = self._values.get("hvn_link")
         assert result is not None, "Required property 'hvn_link' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peering_id(self) -> builtins.str:
         '''The ID of the peering connection.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/azure_peering_connection#peering_id DataHcpAzurePeeringConnection#peering_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/azure_peering_connection#peering_id DataHcpAzurePeeringConnection#peering_id}
         '''
         result = self._values.get("peering_id")
         assert result is not None, "Required property 'peering_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/azure_peering_connection#id DataHcpAzurePeeringConnection#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/azure_peering_connection#id DataHcpAzurePeeringConnection#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpAzurePeeringConnectionTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/azure_peering_connection#timeouts DataHcpAzurePeeringConnection#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/azure_peering_connection#timeouts DataHcpAzurePeeringConnection#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpAzurePeeringConnectionTimeouts"], result)
 
     @builtins.property
     def wait_for_active_state(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If ``true``, Terraform will wait for the peering connection to reach an ``ACTIVE`` state before continuing. Default ``false``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/azure_peering_connection#wait_for_active_state DataHcpAzurePeeringConnection#wait_for_active_state}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/azure_peering_connection#wait_for_active_state DataHcpAzurePeeringConnection#wait_for_active_state}
         '''
         result = self._values.get("wait_for_active_state")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -487,26 +489,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpAzurePeeringConnection.DataHcpAzurePeeringConnectionTimeouts",
     jsii_struct_bases=[],
     name_mapping={"read": "read"},
 )
 class DataHcpAzurePeeringConnectionTimeouts:
     def __init__(self, *, read: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param read: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/azure_peering_connection#read DataHcpAzurePeeringConnection#read}.
+        :param read: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/azure_peering_connection#read DataHcpAzurePeeringConnection#read}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__898b38c26d5c9a0e94ffd813a9d9bfba170550beaa5a58cee10657e5e66c4981)
             check_type(argname="argument read", value=read, expected_type=type_hints["read"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if read is not None:
             self._values["read"] = read
 
     @builtins.property
     def read(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/azure_peering_connection#read DataHcpAzurePeeringConnection#read}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/azure_peering_connection#read DataHcpAzurePeeringConnection#read}.'''
         result = self._values.get("read")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -592,15 +594,15 @@
     *,
     hvn_link: builtins.str,
     peering_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcpAzurePeeringConnectionTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
     wait_for_active_state: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
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
@@ -629,15 +631,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__bd4aba9c40f32574afd6b9f7bfd3bb022ad0157924dba691af2463b7fa0e49bd(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     hvn_link: builtins.str,
     peering_id: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_boundary_cluster/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_boundary_cluster/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_boundary_cluster`
 
-Refer to the Terraform Registory for docs: [`data_hcp_boundary_cluster`](https://www.terraform.io/docs/providers/hcp/d/boundary_cluster).
+Refer to the Terraform Registory for docs: [`data_hcp_boundary_cluster`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/boundary_cluster).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,39 +22,39 @@
 
 
 class DataHcpBoundaryCluster(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpBoundaryCluster.DataHcpBoundaryCluster",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/d/boundary_cluster hcp_boundary_cluster}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/boundary_cluster hcp_boundary_cluster}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcpBoundaryClusterTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/d/boundary_cluster hcp_boundary_cluster} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/boundary_cluster hcp_boundary_cluster} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_id: The ID of the Boundary cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/boundary_cluster#cluster_id DataHcpBoundaryCluster#cluster_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/boundary_cluster#id DataHcpBoundaryCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/boundary_cluster#timeouts DataHcpBoundaryCluster#timeouts}
+        :param cluster_id: The ID of the Boundary cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/boundary_cluster#cluster_id DataHcpBoundaryCluster#cluster_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/boundary_cluster#id DataHcpBoundaryCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/boundary_cluster#timeouts DataHcpBoundaryCluster#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -77,15 +77,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/boundary_cluster#default DataHcpBoundaryCluster#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/boundary_cluster#default DataHcpBoundaryCluster#default}.
         '''
         value = DataHcpBoundaryClusterTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -183,15 +183,15 @@
     },
 )
 class DataHcpBoundaryClusterConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         cluster_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
@@ -201,17 +201,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_id: The ID of the Boundary cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/boundary_cluster#cluster_id DataHcpBoundaryCluster#cluster_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/boundary_cluster#id DataHcpBoundaryCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/boundary_cluster#timeouts DataHcpBoundaryCluster#timeouts}
+        :param cluster_id: The ID of the Boundary cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/boundary_cluster#cluster_id DataHcpBoundaryCluster#cluster_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/boundary_cluster#id DataHcpBoundaryCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/boundary_cluster#timeouts DataHcpBoundaryCluster#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpBoundaryClusterTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1913eb550d7af1c0dfbcde15980d6a32f450b17c9b36190718614e6f68d1327c)
@@ -254,20 +254,22 @@
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
@@ -309,35 +311,35 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cluster_id(self) -> builtins.str:
         '''The ID of the Boundary cluster.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/boundary_cluster#cluster_id DataHcpBoundaryCluster#cluster_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/boundary_cluster#cluster_id DataHcpBoundaryCluster#cluster_id}
         '''
         result = self._values.get("cluster_id")
         assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/boundary_cluster#id DataHcpBoundaryCluster#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/boundary_cluster#id DataHcpBoundaryCluster#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpBoundaryClusterTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/boundary_cluster#timeouts DataHcpBoundaryCluster#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/boundary_cluster#timeouts DataHcpBoundaryCluster#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpBoundaryClusterTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -354,26 +356,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpBoundaryCluster.DataHcpBoundaryClusterTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpBoundaryClusterTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/boundary_cluster#default DataHcpBoundaryCluster#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/boundary_cluster#default DataHcpBoundaryCluster#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__fbef6012e860ebe04f146d9896c229e6efec69de6b4a4c1c99a92fcd23d124a6)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/boundary_cluster#default DataHcpBoundaryCluster#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/boundary_cluster#default DataHcpBoundaryCluster#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -457,15 +459,15 @@
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     cluster_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcpBoundaryClusterTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
 
 def _typecheckingstub__1913eb550d7af1c0dfbcde15980d6a32f450b17c9b36190718614e6f68d1327c(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     cluster_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_helm_config/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_helm_config/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_consul_agent_helm_config`
 
-Refer to the Terraform Registory for docs: [`data_hcp_consul_agent_helm_config`](https://www.terraform.io/docs/providers/hcp/d/consul_agent_helm_config).
+Refer to the Terraform Registory for docs: [`data_hcp_consul_agent_helm_config`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_helm_config).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,43 +22,43 @@
 
 
 class DataHcpConsulAgentHelmConfig(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpConsulAgentHelmConfig.DataHcpConsulAgentHelmConfig",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_helm_config hcp_consul_agent_helm_config}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_helm_config hcp_consul_agent_helm_config}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_id: builtins.str,
         kubernetes_endpoint: builtins.str,
         expose_gossip_ports: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcpConsulAgentHelmConfigTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_helm_config hcp_consul_agent_helm_config} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_helm_config hcp_consul_agent_helm_config} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_helm_config#cluster_id DataHcpConsulAgentHelmConfig#cluster_id}
-        :param kubernetes_endpoint: The FQDN for the Kubernetes API. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_helm_config#kubernetes_endpoint DataHcpConsulAgentHelmConfig#kubernetes_endpoint}
-        :param expose_gossip_ports: Denotes that the gossip ports should be exposed. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_helm_config#expose_gossip_ports DataHcpConsulAgentHelmConfig#expose_gossip_ports}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_helm_config#id DataHcpConsulAgentHelmConfig#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_helm_config#timeouts DataHcpConsulAgentHelmConfig#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_helm_config#cluster_id DataHcpConsulAgentHelmConfig#cluster_id}
+        :param kubernetes_endpoint: The FQDN for the Kubernetes API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_helm_config#kubernetes_endpoint DataHcpConsulAgentHelmConfig#kubernetes_endpoint}
+        :param expose_gossip_ports: Denotes that the gossip ports should be exposed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_helm_config#expose_gossip_ports DataHcpConsulAgentHelmConfig#expose_gossip_ports}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_helm_config#id DataHcpConsulAgentHelmConfig#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_helm_config#timeouts DataHcpConsulAgentHelmConfig#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -83,15 +83,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_helm_config#default DataHcpConsulAgentHelmConfig#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_helm_config#default DataHcpConsulAgentHelmConfig#default}.
         '''
         value = DataHcpConsulAgentHelmConfigTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetExposeGossipPorts")
     def reset_expose_gossip_ports(self) -> None:
@@ -226,15 +226,15 @@
     },
 )
 class DataHcpConsulAgentHelmConfigConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         cluster_id: builtins.str,
         kubernetes_endpoint: builtins.str,
@@ -246,19 +246,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_helm_config#cluster_id DataHcpConsulAgentHelmConfig#cluster_id}
-        :param kubernetes_endpoint: The FQDN for the Kubernetes API. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_helm_config#kubernetes_endpoint DataHcpConsulAgentHelmConfig#kubernetes_endpoint}
-        :param expose_gossip_ports: Denotes that the gossip ports should be exposed. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_helm_config#expose_gossip_ports DataHcpConsulAgentHelmConfig#expose_gossip_ports}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_helm_config#id DataHcpConsulAgentHelmConfig#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_helm_config#timeouts DataHcpConsulAgentHelmConfig#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_helm_config#cluster_id DataHcpConsulAgentHelmConfig#cluster_id}
+        :param kubernetes_endpoint: The FQDN for the Kubernetes API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_helm_config#kubernetes_endpoint DataHcpConsulAgentHelmConfig#kubernetes_endpoint}
+        :param expose_gossip_ports: Denotes that the gossip ports should be exposed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_helm_config#expose_gossip_ports DataHcpConsulAgentHelmConfig#expose_gossip_ports}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_helm_config#id DataHcpConsulAgentHelmConfig#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_helm_config#timeouts DataHcpConsulAgentHelmConfig#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpConsulAgentHelmConfigTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__47dec92eef00aad8d588b88d58009be6faf64a357be06fe065859618bd4d3c59)
@@ -306,20 +306,22 @@
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
@@ -361,56 +363,56 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cluster_id(self) -> builtins.str:
         '''The ID of the HCP Consul cluster.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_helm_config#cluster_id DataHcpConsulAgentHelmConfig#cluster_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_helm_config#cluster_id DataHcpConsulAgentHelmConfig#cluster_id}
         '''
         result = self._values.get("cluster_id")
         assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def kubernetes_endpoint(self) -> builtins.str:
         '''The FQDN for the Kubernetes API.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_helm_config#kubernetes_endpoint DataHcpConsulAgentHelmConfig#kubernetes_endpoint}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_helm_config#kubernetes_endpoint DataHcpConsulAgentHelmConfig#kubernetes_endpoint}
         '''
         result = self._values.get("kubernetes_endpoint")
         assert result is not None, "Required property 'kubernetes_endpoint' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def expose_gossip_ports(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Denotes that the gossip ports should be exposed.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_helm_config#expose_gossip_ports DataHcpConsulAgentHelmConfig#expose_gossip_ports}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_helm_config#expose_gossip_ports DataHcpConsulAgentHelmConfig#expose_gossip_ports}
         '''
         result = self._values.get("expose_gossip_ports")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_helm_config#id DataHcpConsulAgentHelmConfig#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_helm_config#id DataHcpConsulAgentHelmConfig#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpConsulAgentHelmConfigTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_helm_config#timeouts DataHcpConsulAgentHelmConfig#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_helm_config#timeouts DataHcpConsulAgentHelmConfig#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpConsulAgentHelmConfigTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -427,26 +429,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpConsulAgentHelmConfig.DataHcpConsulAgentHelmConfigTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpConsulAgentHelmConfigTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_helm_config#default DataHcpConsulAgentHelmConfig#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_helm_config#default DataHcpConsulAgentHelmConfig#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5fea9574e4bcb25213a3bf7392a0f4ad548eb6e2edf296edabf437732e15d0f0)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_helm_config#default DataHcpConsulAgentHelmConfig#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_helm_config#default DataHcpConsulAgentHelmConfig#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -532,15 +534,15 @@
     *,
     cluster_id: builtins.str,
     kubernetes_endpoint: builtins.str,
     expose_gossip_ports: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcpConsulAgentHelmConfigTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -569,15 +571,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__47dec92eef00aad8d588b88d58009be6faf64a357be06fe065859618bd4d3c59(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     cluster_id: builtins.str,
     kubernetes_endpoint: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_kubernetes_secret/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_kubernetes_secret/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_consul_agent_kubernetes_secret`
 
-Refer to the Terraform Registory for docs: [`data_hcp_consul_agent_kubernetes_secret`](https://www.terraform.io/docs/providers/hcp/d/consul_agent_kubernetes_secret).
+Refer to the Terraform Registory for docs: [`data_hcp_consul_agent_kubernetes_secret`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_kubernetes_secret).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,39 +22,39 @@
 
 
 class DataHcpConsulAgentKubernetesSecret(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpConsulAgentKubernetesSecret.DataHcpConsulAgentKubernetesSecret",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_kubernetes_secret hcp_consul_agent_kubernetes_secret}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_kubernetes_secret hcp_consul_agent_kubernetes_secret}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcpConsulAgentKubernetesSecretTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_kubernetes_secret hcp_consul_agent_kubernetes_secret} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_kubernetes_secret hcp_consul_agent_kubernetes_secret} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_kubernetes_secret#cluster_id DataHcpConsulAgentKubernetesSecret#cluster_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_kubernetes_secret#id DataHcpConsulAgentKubernetesSecret#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_kubernetes_secret#timeouts DataHcpConsulAgentKubernetesSecret#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_kubernetes_secret#cluster_id DataHcpConsulAgentKubernetesSecret#cluster_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_kubernetes_secret#id DataHcpConsulAgentKubernetesSecret#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_kubernetes_secret#timeouts DataHcpConsulAgentKubernetesSecret#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -77,15 +77,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_kubernetes_secret#default DataHcpConsulAgentKubernetesSecret#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_kubernetes_secret#default DataHcpConsulAgentKubernetesSecret#default}.
         '''
         value = DataHcpConsulAgentKubernetesSecretTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -173,15 +173,15 @@
     },
 )
 class DataHcpConsulAgentKubernetesSecretConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         cluster_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
@@ -191,17 +191,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_kubernetes_secret#cluster_id DataHcpConsulAgentKubernetesSecret#cluster_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_kubernetes_secret#id DataHcpConsulAgentKubernetesSecret#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_kubernetes_secret#timeouts DataHcpConsulAgentKubernetesSecret#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_kubernetes_secret#cluster_id DataHcpConsulAgentKubernetesSecret#cluster_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_kubernetes_secret#id DataHcpConsulAgentKubernetesSecret#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_kubernetes_secret#timeouts DataHcpConsulAgentKubernetesSecret#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpConsulAgentKubernetesSecretTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__be3c31d62c3a82506dcabb7d451bc380c751bf95c7a2298998776362da97a950)
@@ -244,20 +244,22 @@
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
@@ -299,35 +301,35 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cluster_id(self) -> builtins.str:
         '''The ID of the HCP Consul cluster.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_kubernetes_secret#cluster_id DataHcpConsulAgentKubernetesSecret#cluster_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_kubernetes_secret#cluster_id DataHcpConsulAgentKubernetesSecret#cluster_id}
         '''
         result = self._values.get("cluster_id")
         assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_kubernetes_secret#id DataHcpConsulAgentKubernetesSecret#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_kubernetes_secret#id DataHcpConsulAgentKubernetesSecret#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpConsulAgentKubernetesSecretTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_kubernetes_secret#timeouts DataHcpConsulAgentKubernetesSecret#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_kubernetes_secret#timeouts DataHcpConsulAgentKubernetesSecret#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpConsulAgentKubernetesSecretTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -344,26 +346,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpConsulAgentKubernetesSecret.DataHcpConsulAgentKubernetesSecretTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpConsulAgentKubernetesSecretTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_kubernetes_secret#default DataHcpConsulAgentKubernetesSecret#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_kubernetes_secret#default DataHcpConsulAgentKubernetesSecret#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3df70bd5a73802b3268610283263f56fafc818d7a8202339d48801ee49e63fa4)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_agent_kubernetes_secret#default DataHcpConsulAgentKubernetesSecret#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_agent_kubernetes_secret#default DataHcpConsulAgentKubernetesSecret#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -447,15 +449,15 @@
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     cluster_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcpConsulAgentKubernetesSecretTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -472,15 +474,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__be3c31d62c3a82506dcabb7d451bc380c751bf95c7a2298998776362da97a950(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     cluster_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_cluster/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_cluster/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_consul_cluster`
 
-Refer to the Terraform Registory for docs: [`data_hcp_consul_cluster`](https://www.terraform.io/docs/providers/hcp/d/consul_cluster).
+Refer to the Terraform Registory for docs: [`data_hcp_consul_cluster`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_cluster).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,39 +22,39 @@
 
 
 class DataHcpConsulCluster(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpConsulCluster.DataHcpConsulCluster",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/d/consul_cluster hcp_consul_cluster}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_cluster hcp_consul_cluster}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcpConsulClusterTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/d/consul_cluster hcp_consul_cluster} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_cluster hcp_consul_cluster} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_cluster#cluster_id DataHcpConsulCluster#cluster_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_cluster#id DataHcpConsulCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_cluster#timeouts DataHcpConsulCluster#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_cluster#cluster_id DataHcpConsulCluster#cluster_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_cluster#id DataHcpConsulCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_cluster#timeouts DataHcpConsulCluster#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -77,15 +77,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_cluster#default DataHcpConsulCluster#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_cluster#default DataHcpConsulCluster#default}.
         '''
         value = DataHcpConsulClusterTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -288,15 +288,15 @@
     },
 )
 class DataHcpConsulClusterConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         cluster_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
@@ -306,17 +306,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_cluster#cluster_id DataHcpConsulCluster#cluster_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_cluster#id DataHcpConsulCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_cluster#timeouts DataHcpConsulCluster#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_cluster#cluster_id DataHcpConsulCluster#cluster_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_cluster#id DataHcpConsulCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_cluster#timeouts DataHcpConsulCluster#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpConsulClusterTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__19684549a8d13e15136e636a89284757a67861c6b2b39b4bf12ae186931f5bfc)
@@ -359,20 +359,22 @@
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
@@ -414,35 +416,35 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cluster_id(self) -> builtins.str:
         '''The ID of the HCP Consul cluster.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_cluster#cluster_id DataHcpConsulCluster#cluster_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_cluster#cluster_id DataHcpConsulCluster#cluster_id}
         '''
         result = self._values.get("cluster_id")
         assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_cluster#id DataHcpConsulCluster#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_cluster#id DataHcpConsulCluster#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpConsulClusterTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_cluster#timeouts DataHcpConsulCluster#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_cluster#timeouts DataHcpConsulCluster#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpConsulClusterTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -608,26 +610,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpConsulCluster.DataHcpConsulClusterTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpConsulClusterTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_cluster#default DataHcpConsulCluster#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_cluster#default DataHcpConsulCluster#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c7161f129504bca3297102710546c4a3e54ea686e16b8260793ad0548b5feb0d)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_cluster#default DataHcpConsulCluster#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_cluster#default DataHcpConsulCluster#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -714,15 +716,15 @@
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     cluster_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcpConsulClusterTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -739,15 +741,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__19684549a8d13e15136e636a89284757a67861c6b2b39b4bf12ae186931f5bfc(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     cluster_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_versions/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_versions/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_consul_versions`
 
-Refer to the Terraform Registory for docs: [`data_hcp_consul_versions`](https://www.terraform.io/docs/providers/hcp/d/consul_versions).
+Refer to the Terraform Registory for docs: [`data_hcp_consul_versions`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_versions).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,37 +22,37 @@
 
 
 class DataHcpConsulVersions(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpConsulVersions.DataHcpConsulVersions",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/d/consul_versions hcp_consul_versions}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_versions hcp_consul_versions}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcpConsulVersionsTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/d/consul_versions hcp_consul_versions} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_versions hcp_consul_versions} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_versions#id DataHcpConsulVersions#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_versions#timeouts DataHcpConsulVersions#timeouts}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_versions#id DataHcpConsulVersions#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_versions#timeouts DataHcpConsulVersions#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -74,15 +74,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_versions#default DataHcpConsulVersions#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_versions#default DataHcpConsulVersions#default}.
         '''
         value = DataHcpConsulVersionsTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -162,15 +162,15 @@
     },
 )
 class DataHcpConsulVersionsConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         timeouts: typing.Optional[typing.Union["DataHcpConsulVersionsTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
@@ -179,16 +179,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_versions#id DataHcpConsulVersions#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_versions#timeouts DataHcpConsulVersions#timeouts}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_versions#id DataHcpConsulVersions#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_versions#timeouts DataHcpConsulVersions#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpConsulVersionsTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ce4ec732e9d19fd84371964dd0535e9577854e1ca55940960301bcb99e1b9c2a)
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
@@ -281,27 +283,27 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_versions#id DataHcpConsulVersions#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_versions#id DataHcpConsulVersions#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpConsulVersionsTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_versions#timeouts DataHcpConsulVersions#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_versions#timeouts DataHcpConsulVersions#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpConsulVersionsTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -318,26 +320,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpConsulVersions.DataHcpConsulVersionsTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpConsulVersionsTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_versions#default DataHcpConsulVersions#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_versions#default DataHcpConsulVersions#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ed5af9126b62d7113ddbc82d2866619e910bd9a40ebdd4661b031b030fd73381)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/consul_versions#default DataHcpConsulVersions#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/consul_versions#default DataHcpConsulVersions#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -420,15 +422,15 @@
 def _typecheckingstub__708b33e2166982944a250a3c67a9ae61c103b8a167b9c5b072820800aade7e4d(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcpConsulVersionsTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -439,15 +441,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__ce4ec732e9d19fd84371964dd0535e9577854e1ca55940960301bcb99e1b9c2a(
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
     timeouts: typing.Optional[typing.Union[DataHcpConsulVersionsTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_hvn/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_hvn/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_hvn`
 
-Refer to the Terraform Registory for docs: [`data_hcp_hvn`](https://www.terraform.io/docs/providers/hcp/d/hvn).
+Refer to the Terraform Registory for docs: [`data_hcp_hvn`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,39 +22,39 @@
 
 
 class DataHcpHvn(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpHvn.DataHcpHvn",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/d/hvn hcp_hvn}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn hcp_hvn}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         hvn_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcpHvnTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/d/hvn hcp_hvn} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn hcp_hvn} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn#hvn_id DataHcpHvn#hvn_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn#id DataHcpHvn#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn#timeouts DataHcpHvn#timeouts}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn#hvn_id DataHcpHvn#hvn_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn#id DataHcpHvn#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn#timeouts DataHcpHvn#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -77,15 +77,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn#default DataHcpHvn#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn#default DataHcpHvn#default}.
         '''
         value = DataHcpHvnTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -213,15 +213,15 @@
     },
 )
 class DataHcpHvnConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         hvn_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
@@ -231,17 +231,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn#hvn_id DataHcpHvn#hvn_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn#id DataHcpHvn#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn#timeouts DataHcpHvn#timeouts}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn#hvn_id DataHcpHvn#hvn_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn#id DataHcpHvn#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn#timeouts DataHcpHvn#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpHvnTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__453ff1b7bb2a6010c49d2b5b38f47ec9027f2eda8d8bfe47db04286175f886d2)
@@ -284,20 +284,22 @@
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
@@ -339,35 +341,35 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def hvn_id(self) -> builtins.str:
         '''The ID of the HashiCorp Virtual Network (HVN).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn#hvn_id DataHcpHvn#hvn_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn#hvn_id DataHcpHvn#hvn_id}
         '''
         result = self._values.get("hvn_id")
         assert result is not None, "Required property 'hvn_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn#id DataHcpHvn#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn#id DataHcpHvn#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpHvnTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn#timeouts DataHcpHvn#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn#timeouts DataHcpHvn#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpHvnTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -384,26 +386,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpHvn.DataHcpHvnTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpHvnTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn#default DataHcpHvn#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn#default DataHcpHvn#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9467b305aebd65c6d36c9d0a374293e0e94ab466fb5e32c9ca7a3f68955d8e8b)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn#default DataHcpHvn#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn#default DataHcpHvn#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -487,15 +489,15 @@
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     hvn_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcpHvnTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -512,15 +514,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__453ff1b7bb2a6010c49d2b5b38f47ec9027f2eda8d8bfe47db04286175f886d2(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     hvn_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_peering_connection/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_peering_connection/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_hvn_peering_connection`
 
-Refer to the Terraform Registory for docs: [`data_hcp_hvn_peering_connection`](https://www.terraform.io/docs/providers/hcp/d/hvn_peering_connection).
+Refer to the Terraform Registory for docs: [`data_hcp_hvn_peering_connection`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_peering_connection).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,43 +22,43 @@
 
 
 class DataHcpHvnPeeringConnection(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpHvnPeeringConnection.DataHcpHvnPeeringConnection",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/d/hvn_peering_connection hcp_hvn_peering_connection}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_peering_connection hcp_hvn_peering_connection}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         hvn1: builtins.str,
         hvn2: builtins.str,
         peering_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcpHvnPeeringConnectionTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/d/hvn_peering_connection hcp_hvn_peering_connection} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_peering_connection hcp_hvn_peering_connection} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param hvn1: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_peering_connection#hvn_1 DataHcpHvnPeeringConnection#hvn_1}
-        :param hvn2: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_peering_connection#hvn_2 DataHcpHvnPeeringConnection#hvn_2}
-        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_peering_connection#peering_id DataHcpHvnPeeringConnection#peering_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_peering_connection#id DataHcpHvnPeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_peering_connection#timeouts DataHcpHvnPeeringConnection#timeouts}
+        :param hvn1: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_peering_connection#hvn_1 DataHcpHvnPeeringConnection#hvn_1}
+        :param hvn2: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_peering_connection#hvn_2 DataHcpHvnPeeringConnection#hvn_2}
+        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_peering_connection#peering_id DataHcpHvnPeeringConnection#peering_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_peering_connection#id DataHcpHvnPeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_peering_connection#timeouts DataHcpHvnPeeringConnection#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -83,15 +83,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_peering_connection#default DataHcpHvnPeeringConnection#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_peering_connection#default DataHcpHvnPeeringConnection#default}.
         '''
         value = DataHcpHvnPeeringConnectionTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -240,15 +240,15 @@
     },
 )
 class DataHcpHvnPeeringConnectionConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         hvn1: builtins.str,
         hvn2: builtins.str,
@@ -260,19 +260,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param hvn1: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_peering_connection#hvn_1 DataHcpHvnPeeringConnection#hvn_1}
-        :param hvn2: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_peering_connection#hvn_2 DataHcpHvnPeeringConnection#hvn_2}
-        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_peering_connection#peering_id DataHcpHvnPeeringConnection#peering_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_peering_connection#id DataHcpHvnPeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_peering_connection#timeouts DataHcpHvnPeeringConnection#timeouts}
+        :param hvn1: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_peering_connection#hvn_1 DataHcpHvnPeeringConnection#hvn_1}
+        :param hvn2: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_peering_connection#hvn_2 DataHcpHvnPeeringConnection#hvn_2}
+        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_peering_connection#peering_id DataHcpHvnPeeringConnection#peering_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_peering_connection#id DataHcpHvnPeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_peering_connection#timeouts DataHcpHvnPeeringConnection#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpHvnPeeringConnectionTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__64fce66989d09d9766300ce08a1b3a8dc5342d493a037f8bf2715a94a6016b1a)
@@ -319,20 +319,22 @@
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
@@ -374,55 +376,55 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def hvn1(self) -> builtins.str:
         '''The unique URL of one of the HVNs being peered.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_peering_connection#hvn_1 DataHcpHvnPeeringConnection#hvn_1}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_peering_connection#hvn_1 DataHcpHvnPeeringConnection#hvn_1}
         '''
         result = self._values.get("hvn1")
         assert result is not None, "Required property 'hvn1' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def hvn2(self) -> builtins.str:
         '''The unique URL of one of the HVNs being peered.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_peering_connection#hvn_2 DataHcpHvnPeeringConnection#hvn_2}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_peering_connection#hvn_2 DataHcpHvnPeeringConnection#hvn_2}
         '''
         result = self._values.get("hvn2")
         assert result is not None, "Required property 'hvn2' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peering_id(self) -> builtins.str:
         '''The ID of the peering connection.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_peering_connection#peering_id DataHcpHvnPeeringConnection#peering_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_peering_connection#peering_id DataHcpHvnPeeringConnection#peering_id}
         '''
         result = self._values.get("peering_id")
         assert result is not None, "Required property 'peering_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_peering_connection#id DataHcpHvnPeeringConnection#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_peering_connection#id DataHcpHvnPeeringConnection#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpHvnPeeringConnectionTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_peering_connection#timeouts DataHcpHvnPeeringConnection#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_peering_connection#timeouts DataHcpHvnPeeringConnection#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpHvnPeeringConnectionTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -439,26 +441,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpHvnPeeringConnection.DataHcpHvnPeeringConnectionTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpHvnPeeringConnectionTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_peering_connection#default DataHcpHvnPeeringConnection#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_peering_connection#default DataHcpHvnPeeringConnection#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c57c224aebaac18dfcc2bfb2fab6ec74b8879a2f03b6640da399adc636b20345)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_peering_connection#default DataHcpHvnPeeringConnection#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_peering_connection#default DataHcpHvnPeeringConnection#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -544,15 +546,15 @@
     *,
     hvn1: builtins.str,
     hvn2: builtins.str,
     peering_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcpHvnPeeringConnectionTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -581,15 +583,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__64fce66989d09d9766300ce08a1b3a8dc5342d493a037f8bf2715a94a6016b1a(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     hvn1: builtins.str,
     hvn2: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_route/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_route/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_hvn_route`
 
-Refer to the Terraform Registory for docs: [`data_hcp_hvn_route`](https://www.terraform.io/docs/providers/hcp/d/hvn_route).
+Refer to the Terraform Registory for docs: [`data_hcp_hvn_route`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_route).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,41 +22,41 @@
 
 
 class DataHcpHvnRoute(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpHvnRoute.DataHcpHvnRoute",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/d/hvn_route hcp_hvn_route}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_route hcp_hvn_route}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         hvn_link: builtins.str,
         hvn_route_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcpHvnRouteTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/d/hvn_route hcp_hvn_route} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_route hcp_hvn_route} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_route#hvn_link DataHcpHvnRoute#hvn_link}
-        :param hvn_route_id: The ID of the HVN route. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_route#hvn_route_id DataHcpHvnRoute#hvn_route_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_route#id DataHcpHvnRoute#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_route#timeouts DataHcpHvnRoute#timeouts}
+        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_route#hvn_link DataHcpHvnRoute#hvn_link}
+        :param hvn_route_id: The ID of the HVN route. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_route#hvn_route_id DataHcpHvnRoute#hvn_route_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_route#id DataHcpHvnRoute#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_route#timeouts DataHcpHvnRoute#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -80,15 +80,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_route#default DataHcpHvnRoute#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_route#default DataHcpHvnRoute#default}.
         '''
         value = DataHcpHvnRouteTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -214,15 +214,15 @@
     },
 )
 class DataHcpHvnRouteConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         hvn_link: builtins.str,
         hvn_route_id: builtins.str,
@@ -233,18 +233,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_route#hvn_link DataHcpHvnRoute#hvn_link}
-        :param hvn_route_id: The ID of the HVN route. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_route#hvn_route_id DataHcpHvnRoute#hvn_route_id}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_route#id DataHcpHvnRoute#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_route#timeouts DataHcpHvnRoute#timeouts}
+        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_route#hvn_link DataHcpHvnRoute#hvn_link}
+        :param hvn_route_id: The ID of the HVN route. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_route#hvn_route_id DataHcpHvnRoute#hvn_route_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_route#id DataHcpHvnRoute#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_route#timeouts DataHcpHvnRoute#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpHvnRouteTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7d998d291388f4b581ac447f8245e6ae3a3b6b66449802a6f662426ff3f18163)
@@ -289,20 +289,22 @@
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
@@ -344,45 +346,45 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def hvn_link(self) -> builtins.str:
         '''The ``self_link`` of the HashiCorp Virtual Network (HVN).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_route#hvn_link DataHcpHvnRoute#hvn_link}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_route#hvn_link DataHcpHvnRoute#hvn_link}
         '''
         result = self._values.get("hvn_link")
         assert result is not None, "Required property 'hvn_link' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def hvn_route_id(self) -> builtins.str:
         '''The ID of the HVN route.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_route#hvn_route_id DataHcpHvnRoute#hvn_route_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_route#hvn_route_id DataHcpHvnRoute#hvn_route_id}
         '''
         result = self._values.get("hvn_route_id")
         assert result is not None, "Required property 'hvn_route_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_route#id DataHcpHvnRoute#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_route#id DataHcpHvnRoute#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpHvnRouteTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_route#timeouts DataHcpHvnRoute#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_route#timeouts DataHcpHvnRoute#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpHvnRouteTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -399,26 +401,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpHvnRoute.DataHcpHvnRouteTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpHvnRouteTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_route#default DataHcpHvnRoute#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_route#default DataHcpHvnRoute#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f0f604582e5a2eb35eace86bd6d3db0862d78e9a132e9be96ebbe04ee856c19b)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/hvn_route#default DataHcpHvnRoute#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/hvn_route#default DataHcpHvnRoute#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -503,15 +505,15 @@
     id_: builtins.str,
     *,
     hvn_link: builtins.str,
     hvn_route_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcpHvnRouteTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -534,15 +536,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__7d998d291388f4b581ac447f8245e6ae3a3b6b66449802a6f662426ff3f18163(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     hvn_link: builtins.str,
     hvn_route_id: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/hvn/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# `data_hcp_packer_image`
+# `hcp_hvn`
 
-Refer to the Terraform Registory for docs: [`data_hcp_packer_image`](https://www.terraform.io/docs/providers/hcp/d/packer_image).
+Refer to the Terraform Registory for docs: [`hcp_hvn`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -17,378 +17,320 @@
 
 from .._jsii import *
 
 import cdktf as _cdktf_9a9027ec
 import constructs as _constructs_77d1e7e8
 
 
-class DataHcpPackerImage(
-    _cdktf_9a9027ec.TerraformDataSource,
+class Hvn(
+    _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-hcp.dataHcpPackerImage.DataHcpPackerImage",
+    jsii_type="@cdktf/provider-hcp.hvn.Hvn",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/d/packer_image hcp_packer_image}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn hcp_hvn}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
-        bucket_name: builtins.str,
         cloud_provider: builtins.str,
+        hvn_id: builtins.str,
         region: builtins.str,
-        channel: typing.Optional[builtins.str] = None,
-        component_type: typing.Optional[builtins.str] = None,
+        cidr_block: typing.Optional[builtins.str] = None,
         id: typing.Optional[builtins.str] = None,
-        iteration_id: typing.Optional[builtins.str] = None,
-        timeouts: typing.Optional[typing.Union["DataHcpPackerImageTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
+        timeouts: typing.Optional[typing.Union["HvnTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/d/packer_image hcp_packer_image} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn hcp_hvn} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#bucket_name DataHcpPackerImage#bucket_name}
-        :param cloud_provider: Name of the cloud provider this image is stored-in. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#cloud_provider DataHcpPackerImage#cloud_provider}
-        :param region: Region this image is stored in, if any. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#region DataHcpPackerImage#region}
-        :param channel: The channel that points to the version of the image being retrieved. Either this or ``iteration_id`` must be specified. Note: will incur a billable request Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#channel DataHcpPackerImage#channel}
-        :param component_type: Name of the builder that built this image. Ex: ``amazon-ebs.example``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#component_type DataHcpPackerImage#component_type}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#id DataHcpPackerImage#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param iteration_id: The iteration from which to get the image. Either this or ``channel`` must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#iteration_id DataHcpPackerImage#iteration_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#timeouts DataHcpPackerImage#timeouts}
+        :param cloud_provider: The provider where the HVN is located. The provider 'aws' is generally available and 'azure' is in public beta. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#cloud_provider Hvn#cloud_provider}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#hvn_id Hvn#hvn_id}
+        :param region: The region where the HVN is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#region Hvn#region}
+        :param cidr_block: The CIDR range of the HVN. If this is not provided, the service will provide a default value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#cidr_block Hvn#cidr_block}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#id Hvn#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#timeouts Hvn#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__cc6c7caad008e83a00f4b8e66ad31c0f6a0402f000262976b1b3474e28f8d9ce)
+            type_hints = typing.get_type_hints(_typecheckingstub__d9c0b08caea8368b936671060ab06f3ecff3c2acd1bdb71cae9606506c352a28)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
-        config = DataHcpPackerImageConfig(
-            bucket_name=bucket_name,
+        config = HvnConfig(
             cloud_provider=cloud_provider,
+            hvn_id=hvn_id,
             region=region,
-            channel=channel,
-            component_type=component_type,
+            cidr_block=cidr_block,
             id=id,
-            iteration_id=iteration_id,
             timeouts=timeouts,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
-    def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
+    def put_timeouts(
+        self,
+        *,
+        create: typing.Optional[builtins.str] = None,
+        default: typing.Optional[builtins.str] = None,
+        delete: typing.Optional[builtins.str] = None,
+    ) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#default DataHcpPackerImage#default}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#create Hvn#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#default Hvn#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#delete Hvn#delete}.
         '''
-        value = DataHcpPackerImageTimeouts(default=default)
+        value = HvnTimeouts(create=create, default=default, delete=delete)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
-    @jsii.member(jsii_name="resetChannel")
-    def reset_channel(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetChannel", []))
-
-    @jsii.member(jsii_name="resetComponentType")
-    def reset_component_type(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetComponentType", []))
+    @jsii.member(jsii_name="resetCidrBlock")
+    def reset_cidr_block(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetCidrBlock", []))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetId", []))
 
-    @jsii.member(jsii_name="resetIterationId")
-    def reset_iteration_id(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetIterationId", []))
-
     @jsii.member(jsii_name="resetTimeouts")
     def reset_timeouts(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetTimeouts", []))
 
     @jsii.member(jsii_name="synthesizeAttributes")
     def _synthesize_attributes(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "synthesizeAttributes", []))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
-    @jsii.member(jsii_name="buildId")
-    def build_id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "buildId"))
-
-    @builtins.property
-    @jsii.member(jsii_name="cloudImageId")
-    def cloud_image_id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "cloudImageId"))
-
-    @builtins.property
     @jsii.member(jsii_name="createdAt")
     def created_at(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "createdAt"))
 
     @builtins.property
-    @jsii.member(jsii_name="labels")
-    def labels(self) -> _cdktf_9a9027ec.StringMap:
-        return typing.cast(_cdktf_9a9027ec.StringMap, jsii.get(self, "labels"))
-
-    @builtins.property
     @jsii.member(jsii_name="organizationId")
     def organization_id(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "organizationId"))
 
     @builtins.property
-    @jsii.member(jsii_name="packerRunUuid")
-    def packer_run_uuid(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "packerRunUuid"))
-
-    @builtins.property
     @jsii.member(jsii_name="projectId")
     def project_id(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "projectId"))
 
     @builtins.property
-    @jsii.member(jsii_name="revokeAt")
-    def revoke_at(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "revokeAt"))
+    @jsii.member(jsii_name="providerAccountId")
+    def provider_account_id(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "providerAccountId"))
 
     @builtins.property
-    @jsii.member(jsii_name="timeouts")
-    def timeouts(self) -> "DataHcpPackerImageTimeoutsOutputReference":
-        return typing.cast("DataHcpPackerImageTimeoutsOutputReference", jsii.get(self, "timeouts"))
+    @jsii.member(jsii_name="selfLink")
+    def self_link(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "selfLink"))
+
+    @builtins.property
+    @jsii.member(jsii_name="state")
+    def state(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "state"))
 
     @builtins.property
-    @jsii.member(jsii_name="bucketNameInput")
-    def bucket_name_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "bucketNameInput"))
+    @jsii.member(jsii_name="timeouts")
+    def timeouts(self) -> "HvnTimeoutsOutputReference":
+        return typing.cast("HvnTimeoutsOutputReference", jsii.get(self, "timeouts"))
 
     @builtins.property
-    @jsii.member(jsii_name="channelInput")
-    def channel_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "channelInput"))
+    @jsii.member(jsii_name="cidrBlockInput")
+    def cidr_block_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "cidrBlockInput"))
 
     @builtins.property
     @jsii.member(jsii_name="cloudProviderInput")
     def cloud_provider_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "cloudProviderInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="componentTypeInput")
-    def component_type_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "componentTypeInput"))
+    @jsii.member(jsii_name="hvnIdInput")
+    def hvn_id_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "hvnIdInput"))
 
     @builtins.property
     @jsii.member(jsii_name="idInput")
     def id_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="iterationIdInput")
-    def iteration_id_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "iterationIdInput"))
-
-    @builtins.property
     @jsii.member(jsii_name="regionInput")
     def region_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "regionInput"))
 
     @builtins.property
     @jsii.member(jsii_name="timeoutsInput")
     def timeouts_input(
         self,
-    ) -> typing.Optional[typing.Union["DataHcpPackerImageTimeouts", _cdktf_9a9027ec.IResolvable]]:
-        return typing.cast(typing.Optional[typing.Union["DataHcpPackerImageTimeouts", _cdktf_9a9027ec.IResolvable]], jsii.get(self, "timeoutsInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="bucketName")
-    def bucket_name(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "bucketName"))
-
-    @bucket_name.setter
-    def bucket_name(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__670ac0b627c06a19adafde3135dc758c09c3cdcdfe00019e1c6a779c84cab8ef)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "bucketName", value)
+    ) -> typing.Optional[typing.Union["HvnTimeouts", _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union["HvnTimeouts", _cdktf_9a9027ec.IResolvable]], jsii.get(self, "timeoutsInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="channel")
-    def channel(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "channel"))
+    @jsii.member(jsii_name="cidrBlock")
+    def cidr_block(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "cidrBlock"))
 
-    @channel.setter
-    def channel(self, value: builtins.str) -> None:
+    @cidr_block.setter
+    def cidr_block(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__47f7f89ae3780d0838f0402b320bcc5920246dcb2dd58b3134313b095fbcd02f)
+            type_hints = typing.get_type_hints(_typecheckingstub__01eea2c7326bb3ea8ab024b1ede34acb60a071dcfef3ab4beb99ae85a90090a4)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "channel", value)
+        jsii.set(self, "cidrBlock", value)
 
     @builtins.property
     @jsii.member(jsii_name="cloudProvider")
     def cloud_provider(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "cloudProvider"))
 
     @cloud_provider.setter
     def cloud_provider(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a16003bf630186465fa54a08f5c4f9454b30e7a035b33bd0ae6aee1972174ecc)
+            type_hints = typing.get_type_hints(_typecheckingstub__1e8d462e6ddd72e6a026cfa9c0e9f7a2ec7529b3bbbc6141a40192c50df98150)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cloudProvider", value)
 
     @builtins.property
-    @jsii.member(jsii_name="componentType")
-    def component_type(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "componentType"))
+    @jsii.member(jsii_name="hvnId")
+    def hvn_id(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "hvnId"))
 
-    @component_type.setter
-    def component_type(self, value: builtins.str) -> None:
+    @hvn_id.setter
+    def hvn_id(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__06e904c39415dfc257bf3618c70f4493c54e27bf0377326fb6cb41e86eae29ec)
+            type_hints = typing.get_type_hints(_typecheckingstub__7466dd4240d89ce97202456c249c13b379fdb07e8c9fe6fda8eb9c0a0f737634)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "componentType", value)
+        jsii.set(self, "hvnId", value)
 
     @builtins.property
     @jsii.member(jsii_name="id")
     def id(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "id"))
 
     @id.setter
     def id(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b187756316217e3e2e71bea2cff1b84961e65057de1e6130033387dea9fe473f)
+            type_hints = typing.get_type_hints(_typecheckingstub__a5ba3730911d8c28a965bf96d41dde6d044d6080b9168018993c8d716e860289)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "id", value)
 
     @builtins.property
-    @jsii.member(jsii_name="iterationId")
-    def iteration_id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "iterationId"))
-
-    @iteration_id.setter
-    def iteration_id(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__55ac89d21189644f47369f6c73a0c5d57f224a8af39ba8aacba36dd1d3e7dc60)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "iterationId", value)
-
-    @builtins.property
     @jsii.member(jsii_name="region")
     def region(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "region"))
 
     @region.setter
     def region(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__aa0762e2ee1b9b1e3072737097fa1eb6b5554862504cb9458278c82dd32d31fa)
+            type_hints = typing.get_type_hints(_typecheckingstub__87022c9cf10bd5feb0e7b700780a06e4f8dd44488210c29f05f7d6918bb6363e)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "region", value)
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-hcp.dataHcpPackerImage.DataHcpPackerImageConfig",
+    jsii_type="@cdktf/provider-hcp.hvn.HvnConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
-        "bucket_name": "bucketName",
         "cloud_provider": "cloudProvider",
+        "hvn_id": "hvnId",
         "region": "region",
-        "channel": "channel",
-        "component_type": "componentType",
+        "cidr_block": "cidrBlock",
         "id": "id",
-        "iteration_id": "iterationId",
         "timeouts": "timeouts",
     },
 )
-class DataHcpPackerImageConfig(_cdktf_9a9027ec.TerraformMetaArguments):
+class HvnConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
-        bucket_name: builtins.str,
         cloud_provider: builtins.str,
+        hvn_id: builtins.str,
         region: builtins.str,
-        channel: typing.Optional[builtins.str] = None,
-        component_type: typing.Optional[builtins.str] = None,
+        cidr_block: typing.Optional[builtins.str] = None,
         id: typing.Optional[builtins.str] = None,
-        iteration_id: typing.Optional[builtins.str] = None,
-        timeouts: typing.Optional[typing.Union["DataHcpPackerImageTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
+        timeouts: typing.Optional[typing.Union["HvnTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#bucket_name DataHcpPackerImage#bucket_name}
-        :param cloud_provider: Name of the cloud provider this image is stored-in. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#cloud_provider DataHcpPackerImage#cloud_provider}
-        :param region: Region this image is stored in, if any. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#region DataHcpPackerImage#region}
-        :param channel: The channel that points to the version of the image being retrieved. Either this or ``iteration_id`` must be specified. Note: will incur a billable request Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#channel DataHcpPackerImage#channel}
-        :param component_type: Name of the builder that built this image. Ex: ``amazon-ebs.example``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#component_type DataHcpPackerImage#component_type}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#id DataHcpPackerImage#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param iteration_id: The iteration from which to get the image. Either this or ``channel`` must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#iteration_id DataHcpPackerImage#iteration_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#timeouts DataHcpPackerImage#timeouts}
+        :param cloud_provider: The provider where the HVN is located. The provider 'aws' is generally available and 'azure' is in public beta. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#cloud_provider Hvn#cloud_provider}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#hvn_id Hvn#hvn_id}
+        :param region: The region where the HVN is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#region Hvn#region}
+        :param cidr_block: The CIDR range of the HVN. If this is not provided, the service will provide a default value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#cidr_block Hvn#cidr_block}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#id Hvn#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#timeouts Hvn#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
-            timeouts = DataHcpPackerImageTimeouts(**timeouts)
+            timeouts = HvnTimeouts(**timeouts)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d493367e1c5b95af729f26e73812da9655a869bb22c8f88270fbf9a025718631)
+            type_hints = typing.get_type_hints(_typecheckingstub__d25a7fdd7ab2372e1a2e11563d24055e64416bf11f211460edfc9e4cac4b0545)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
-            check_type(argname="argument bucket_name", value=bucket_name, expected_type=type_hints["bucket_name"])
             check_type(argname="argument cloud_provider", value=cloud_provider, expected_type=type_hints["cloud_provider"])
+            check_type(argname="argument hvn_id", value=hvn_id, expected_type=type_hints["hvn_id"])
             check_type(argname="argument region", value=region, expected_type=type_hints["region"])
-            check_type(argname="argument channel", value=channel, expected_type=type_hints["channel"])
-            check_type(argname="argument component_type", value=component_type, expected_type=type_hints["component_type"])
+            check_type(argname="argument cidr_block", value=cidr_block, expected_type=type_hints["cidr_block"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument iteration_id", value=iteration_id, expected_type=type_hints["iteration_id"])
             check_type(argname="argument timeouts", value=timeouts, expected_type=type_hints["timeouts"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
-            "bucket_name": bucket_name,
             "cloud_provider": cloud_provider,
+            "hvn_id": hvn_id,
             "region": region,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
         if depends_on is not None:
@@ -397,42 +339,40 @@
             self._values["for_each"] = for_each
         if lifecycle is not None:
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
-        if channel is not None:
-            self._values["channel"] = channel
-        if component_type is not None:
-            self._values["component_type"] = component_type
+        if cidr_block is not None:
+            self._values["cidr_block"] = cidr_block
         if id is not None:
             self._values["id"] = id
-        if iteration_id is not None:
-            self._values["iteration_id"] = iteration_id
         if timeouts is not None:
             self._values["timeouts"] = timeouts
 
     @builtins.property
     def connection(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]]:
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
@@ -471,310 +411,356 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
-    def bucket_name(self) -> builtins.str:
-        '''The slug of the HCP Packer Registry image bucket to pull from.
+    def cloud_provider(self) -> builtins.str:
+        '''The provider where the HVN is located. The provider 'aws' is generally available and 'azure' is in public beta.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#bucket_name DataHcpPackerImage#bucket_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#cloud_provider Hvn#cloud_provider}
         '''
-        result = self._values.get("bucket_name")
-        assert result is not None, "Required property 'bucket_name' is missing"
+        result = self._values.get("cloud_provider")
+        assert result is not None, "Required property 'cloud_provider' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def cloud_provider(self) -> builtins.str:
-        '''Name of the cloud provider this image is stored-in.
+    def hvn_id(self) -> builtins.str:
+        '''The ID of the HashiCorp Virtual Network (HVN).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#cloud_provider DataHcpPackerImage#cloud_provider}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#hvn_id Hvn#hvn_id}
         '''
-        result = self._values.get("cloud_provider")
-        assert result is not None, "Required property 'cloud_provider' is missing"
+        result = self._values.get("hvn_id")
+        assert result is not None, "Required property 'hvn_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def region(self) -> builtins.str:
-        '''Region this image is stored in, if any.
+        '''The region where the HVN is located.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#region DataHcpPackerImage#region}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#region Hvn#region}
         '''
         result = self._values.get("region")
         assert result is not None, "Required property 'region' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def channel(self) -> typing.Optional[builtins.str]:
-        '''The channel that points to the version of the image being retrieved.
+    def cidr_block(self) -> typing.Optional[builtins.str]:
+        '''The CIDR range of the HVN. If this is not provided, the service will provide a default value.
 
-        Either this or ``iteration_id`` must be specified. Note: will incur a billable request
-
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#channel DataHcpPackerImage#channel}
-        '''
-        result = self._values.get("channel")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    @builtins.property
-    def component_type(self) -> typing.Optional[builtins.str]:
-        '''Name of the builder that built this image. Ex: ``amazon-ebs.example``.
-
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#component_type DataHcpPackerImage#component_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#cidr_block Hvn#cidr_block}
         '''
-        result = self._values.get("component_type")
+        result = self._values.get("cidr_block")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#id DataHcpPackerImage#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#id Hvn#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def iteration_id(self) -> typing.Optional[builtins.str]:
-        '''The iteration from which to get the image. Either this or ``channel`` must be specified.
-
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#iteration_id DataHcpPackerImage#iteration_id}
-        '''
-        result = self._values.get("iteration_id")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    @builtins.property
-    def timeouts(self) -> typing.Optional["DataHcpPackerImageTimeouts"]:
+    def timeouts(self) -> typing.Optional["HvnTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#timeouts DataHcpPackerImage#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#timeouts Hvn#timeouts}
         '''
         result = self._values.get("timeouts")
-        return typing.cast(typing.Optional["DataHcpPackerImageTimeouts"], result)
+        return typing.cast(typing.Optional["HvnTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataHcpPackerImageConfig(%s)" % ", ".join(
+        return "HvnConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-hcp.dataHcpPackerImage.DataHcpPackerImageTimeouts",
+    jsii_type="@cdktf/provider-hcp.hvn.HvnTimeouts",
     jsii_struct_bases=[],
-    name_mapping={"default": "default"},
+    name_mapping={"create": "create", "default": "default", "delete": "delete"},
 )
-class DataHcpPackerImageTimeouts:
-    def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
+class HvnTimeouts:
+    def __init__(
+        self,
+        *,
+        create: typing.Optional[builtins.str] = None,
+        default: typing.Optional[builtins.str] = None,
+        delete: typing.Optional[builtins.str] = None,
+    ) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#default DataHcpPackerImage#default}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#create Hvn#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#default Hvn#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#delete Hvn#delete}.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4be11f84de0716029be04a7daa0df27f4151e6a0bf1e56cb08c563b3a95bdd94)
+            type_hints = typing.get_type_hints(_typecheckingstub__c6735e0b1a893f99c663fcdd555521d20556b1c3aac0d53912d420fd1bc74eaa)
+            check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
+            check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if create is not None:
+            self._values["create"] = create
         if default is not None:
             self._values["default"] = default
+        if delete is not None:
+            self._values["delete"] = delete
+
+    @builtins.property
+    def create(self) -> typing.Optional[builtins.str]:
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#create Hvn#create}.'''
+        result = self._values.get("create")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image#default DataHcpPackerImage#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#default Hvn#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
+    @builtins.property
+    def delete(self) -> typing.Optional[builtins.str]:
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn#delete Hvn#delete}.'''
+        result = self._values.get("delete")
+        return typing.cast(typing.Optional[builtins.str], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataHcpPackerImageTimeouts(%s)" % ", ".join(
+        return "HvnTimeouts(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataHcpPackerImageTimeoutsOutputReference(
+class HvnTimeoutsOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-hcp.dataHcpPackerImage.DataHcpPackerImageTimeoutsOutputReference",
+    jsii_type="@cdktf/provider-hcp.hvn.HvnTimeoutsOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ede3a5dff4ab5e7059531426b1b7f7442fa254278883b44fd6bd52e4115c002e)
+            type_hints = typing.get_type_hints(_typecheckingstub__a3029689df0bee70166788261ce529a2b33cef6edc47c3aa8cf863428e56e831)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
+    @jsii.member(jsii_name="resetCreate")
+    def reset_create(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetCreate", []))
+
     @jsii.member(jsii_name="resetDefault")
     def reset_default(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetDefault", []))
 
+    @jsii.member(jsii_name="resetDelete")
+    def reset_delete(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetDelete", []))
+
+    @builtins.property
+    @jsii.member(jsii_name="createInput")
+    def create_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "createInput"))
+
     @builtins.property
     @jsii.member(jsii_name="defaultInput")
     def default_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "defaultInput"))
 
     @builtins.property
+    @jsii.member(jsii_name="deleteInput")
+    def delete_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "deleteInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="create")
+    def create(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "create"))
+
+    @create.setter
+    def create(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__e4050c1bd51bac1ab061ff525d74d6390eb721b7829bed69184bf9fb70f1bde8)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "create", value)
+
+    @builtins.property
     @jsii.member(jsii_name="default")
     def default(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "default"))
 
     @default.setter
     def default(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__29fdef3bf79ad06147e87370c3d8331606ad41dc83f716b2b7ac552bfb3c2551)
+            type_hints = typing.get_type_hints(_typecheckingstub__b655a6b03433b43424170f1d1932d655bb37314d862daca043722c5f529e3eed)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "default", value)
 
     @builtins.property
+    @jsii.member(jsii_name="delete")
+    def delete(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "delete"))
+
+    @delete.setter
+    def delete(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__20fc95bdf5da2f082b8394ef5d339ab454fbecbec66fa59a109ff0eb0677bd6f)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "delete", value)
+
+    @builtins.property
     @jsii.member(jsii_name="internalValue")
     def internal_value(
         self,
-    ) -> typing.Optional[typing.Union[DataHcpPackerImageTimeouts, _cdktf_9a9027ec.IResolvable]]:
-        return typing.cast(typing.Optional[typing.Union[DataHcpPackerImageTimeouts, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "internalValue"))
+    ) -> typing.Optional[typing.Union[HvnTimeouts, _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union[HvnTimeouts, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[typing.Union[DataHcpPackerImageTimeouts, _cdktf_9a9027ec.IResolvable]],
+        value: typing.Optional[typing.Union[HvnTimeouts, _cdktf_9a9027ec.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__1c169efc18af613e8740b26ca4a19b64797fbebc90b9ec07734b99a60494813f)
+            type_hints = typing.get_type_hints(_typecheckingstub__f324f70a650ffb69ab131ae27f6d459090bdcc9e2bc948c722f0d9b1c2fdc6e7)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 __all__ = [
-    "DataHcpPackerImage",
-    "DataHcpPackerImageConfig",
-    "DataHcpPackerImageTimeouts",
-    "DataHcpPackerImageTimeoutsOutputReference",
+    "Hvn",
+    "HvnConfig",
+    "HvnTimeouts",
+    "HvnTimeoutsOutputReference",
 ]
 
 publication.publish()
 
-def _typecheckingstub__cc6c7caad008e83a00f4b8e66ad31c0f6a0402f000262976b1b3474e28f8d9ce(
+def _typecheckingstub__d9c0b08caea8368b936671060ab06f3ecff3c2acd1bdb71cae9606506c352a28(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
-    bucket_name: builtins.str,
     cloud_provider: builtins.str,
+    hvn_id: builtins.str,
     region: builtins.str,
-    channel: typing.Optional[builtins.str] = None,
-    component_type: typing.Optional[builtins.str] = None,
+    cidr_block: typing.Optional[builtins.str] = None,
     id: typing.Optional[builtins.str] = None,
-    iteration_id: typing.Optional[builtins.str] = None,
-    timeouts: typing.Optional[typing.Union[DataHcpPackerImageTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
+    timeouts: typing.Optional[typing.Union[HvnTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
     pass
 
-def _typecheckingstub__670ac0b627c06a19adafde3135dc758c09c3cdcdfe00019e1c6a779c84cab8ef(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__47f7f89ae3780d0838f0402b320bcc5920246dcb2dd58b3134313b095fbcd02f(
+def _typecheckingstub__01eea2c7326bb3ea8ab024b1ede34acb60a071dcfef3ab4beb99ae85a90090a4(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__a16003bf630186465fa54a08f5c4f9454b30e7a035b33bd0ae6aee1972174ecc(
+def _typecheckingstub__1e8d462e6ddd72e6a026cfa9c0e9f7a2ec7529b3bbbc6141a40192c50df98150(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__06e904c39415dfc257bf3618c70f4493c54e27bf0377326fb6cb41e86eae29ec(
+def _typecheckingstub__7466dd4240d89ce97202456c249c13b379fdb07e8c9fe6fda8eb9c0a0f737634(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__b187756316217e3e2e71bea2cff1b84961e65057de1e6130033387dea9fe473f(
+def _typecheckingstub__a5ba3730911d8c28a965bf96d41dde6d044d6080b9168018993c8d716e860289(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__55ac89d21189644f47369f6c73a0c5d57f224a8af39ba8aacba36dd1d3e7dc60(
+def _typecheckingstub__87022c9cf10bd5feb0e7b700780a06e4f8dd44488210c29f05f7d6918bb6363e(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__aa0762e2ee1b9b1e3072737097fa1eb6b5554862504cb9458278c82dd32d31fa(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__d493367e1c5b95af729f26e73812da9655a869bb22c8f88270fbf9a025718631(
+def _typecheckingstub__d25a7fdd7ab2372e1a2e11563d24055e64416bf11f211460edfc9e4cac4b0545(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
-    bucket_name: builtins.str,
     cloud_provider: builtins.str,
+    hvn_id: builtins.str,
     region: builtins.str,
-    channel: typing.Optional[builtins.str] = None,
-    component_type: typing.Optional[builtins.str] = None,
+    cidr_block: typing.Optional[builtins.str] = None,
     id: typing.Optional[builtins.str] = None,
-    iteration_id: typing.Optional[builtins.str] = None,
-    timeouts: typing.Optional[typing.Union[DataHcpPackerImageTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
+    timeouts: typing.Optional[typing.Union[HvnTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__4be11f84de0716029be04a7daa0df27f4151e6a0bf1e56cb08c563b3a95bdd94(
+def _typecheckingstub__c6735e0b1a893f99c663fcdd555521d20556b1c3aac0d53912d420fd1bc74eaa(
     *,
+    create: typing.Optional[builtins.str] = None,
     default: typing.Optional[builtins.str] = None,
+    delete: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__ede3a5dff4ab5e7059531426b1b7f7442fa254278883b44fd6bd52e4115c002e(
+def _typecheckingstub__a3029689df0bee70166788261ce529a2b33cef6edc47c3aa8cf863428e56e831(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__29fdef3bf79ad06147e87370c3d8331606ad41dc83f716b2b7ac552bfb3c2551(
+def _typecheckingstub__e4050c1bd51bac1ab061ff525d74d6390eb721b7829bed69184bf9fb70f1bde8(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b655a6b03433b43424170f1d1932d655bb37314d862daca043722c5f529e3eed(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__20fc95bdf5da2f082b8394ef5d339ab454fbecbec66fa59a109ff0eb0677bd6f(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__1c169efc18af613e8740b26ca4a19b64797fbebc90b9ec07734b99a60494813f(
-    value: typing.Optional[typing.Union[DataHcpPackerImageTimeouts, _cdktf_9a9027ec.IResolvable]],
+def _typecheckingstub__f324f70a650ffb69ab131ae27f6d459090bdcc9e2bc948c722f0d9b1c2fdc6e7(
+    value: typing.Optional[typing.Union[HvnTimeouts, _cdktf_9a9027ec.IResolvable]],
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image_iteration/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image_iteration/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_packer_image_iteration`
 
-Refer to the Terraform Registory for docs: [`data_hcp_packer_image_iteration`](https://www.terraform.io/docs/providers/hcp/d/packer_image_iteration).
+Refer to the Terraform Registory for docs: [`data_hcp_packer_image_iteration`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_image_iteration).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,41 +22,41 @@
 
 
 class DataHcpPackerImageIteration(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpPackerImageIteration.DataHcpPackerImageIteration",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/d/packer_image_iteration hcp_packer_image_iteration}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_image_iteration hcp_packer_image_iteration}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         bucket_name: builtins.str,
         channel: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcpPackerImageIterationTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/d/packer_image_iteration hcp_packer_image_iteration} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_image_iteration hcp_packer_image_iteration} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image_iteration#bucket_name DataHcpPackerImageIteration#bucket_name}
-        :param channel: The channel that points to the version of the image you want. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image_iteration#channel DataHcpPackerImageIteration#channel}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image_iteration#id DataHcpPackerImageIteration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image_iteration#timeouts DataHcpPackerImageIteration#timeouts}
+        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_image_iteration#bucket_name DataHcpPackerImageIteration#bucket_name}
+        :param channel: The channel that points to the version of the image you want. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_image_iteration#channel DataHcpPackerImageIteration#channel}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_image_iteration#id DataHcpPackerImageIteration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_image_iteration#timeouts DataHcpPackerImageIteration#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -80,15 +80,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image_iteration#default DataHcpPackerImageIteration#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_image_iteration#default DataHcpPackerImageIteration#default}.
         '''
         value = DataHcpPackerImageIterationTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -564,15 +564,15 @@
     },
 )
 class DataHcpPackerImageIterationConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         bucket_name: builtins.str,
         channel: builtins.str,
@@ -583,18 +583,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image_iteration#bucket_name DataHcpPackerImageIteration#bucket_name}
-        :param channel: The channel that points to the version of the image you want. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image_iteration#channel DataHcpPackerImageIteration#channel}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image_iteration#id DataHcpPackerImageIteration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image_iteration#timeouts DataHcpPackerImageIteration#timeouts}
+        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_image_iteration#bucket_name DataHcpPackerImageIteration#bucket_name}
+        :param channel: The channel that points to the version of the image you want. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_image_iteration#channel DataHcpPackerImageIteration#channel}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_image_iteration#id DataHcpPackerImageIteration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_image_iteration#timeouts DataHcpPackerImageIteration#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpPackerImageIterationTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d58fea42b2c52a22d4572e002560d14dfa31818c38be7a84f5c652d433d3bf0c)
@@ -639,20 +639,22 @@
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
@@ -694,45 +696,45 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def bucket_name(self) -> builtins.str:
         '''The slug of the HCP Packer Registry image bucket to pull from.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image_iteration#bucket_name DataHcpPackerImageIteration#bucket_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_image_iteration#bucket_name DataHcpPackerImageIteration#bucket_name}
         '''
         result = self._values.get("bucket_name")
         assert result is not None, "Required property 'bucket_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def channel(self) -> builtins.str:
         '''The channel that points to the version of the image you want.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image_iteration#channel DataHcpPackerImageIteration#channel}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_image_iteration#channel DataHcpPackerImageIteration#channel}
         '''
         result = self._values.get("channel")
         assert result is not None, "Required property 'channel' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image_iteration#id DataHcpPackerImageIteration#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_image_iteration#id DataHcpPackerImageIteration#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpPackerImageIterationTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image_iteration#timeouts DataHcpPackerImageIteration#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_image_iteration#timeouts DataHcpPackerImageIteration#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpPackerImageIterationTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -749,26 +751,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpPackerImageIteration.DataHcpPackerImageIterationTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpPackerImageIterationTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image_iteration#default DataHcpPackerImageIteration#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_image_iteration#default DataHcpPackerImageIteration#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a7466533aa9f1828ae820a0ceadf3b9186cde9924c22191d7503f192b4a00a64)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_image_iteration#default DataHcpPackerImageIteration#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_image_iteration#default DataHcpPackerImageIteration#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -859,15 +861,15 @@
     id_: builtins.str,
     *,
     bucket_name: builtins.str,
     channel: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcpPackerImageIterationTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -984,15 +986,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__d58fea42b2c52a22d4572e002560d14dfa31818c38be7a84f5c652d433d3bf0c(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     bucket_name: builtins.str,
     channel: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_packer_iteration/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_packer_iteration/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_packer_iteration`
 
-Refer to the Terraform Registory for docs: [`data_hcp_packer_iteration`](https://www.terraform.io/docs/providers/hcp/d/packer_iteration).
+Refer to the Terraform Registory for docs: [`data_hcp_packer_iteration`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_iteration).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,41 +22,41 @@
 
 
 class DataHcpPackerIteration(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpPackerIteration.DataHcpPackerIteration",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/d/packer_iteration hcp_packer_iteration}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_iteration hcp_packer_iteration}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         bucket_name: builtins.str,
         channel: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcpPackerIterationTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/d/packer_iteration hcp_packer_iteration} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_iteration hcp_packer_iteration} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_iteration#bucket_name DataHcpPackerIteration#bucket_name}
-        :param channel: The channel that points to the version of the image you want. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_iteration#channel DataHcpPackerIteration#channel}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_iteration#id DataHcpPackerIteration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_iteration#timeouts DataHcpPackerIteration#timeouts}
+        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_iteration#bucket_name DataHcpPackerIteration#bucket_name}
+        :param channel: The channel that points to the version of the image you want. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_iteration#channel DataHcpPackerIteration#channel}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_iteration#id DataHcpPackerIteration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_iteration#timeouts DataHcpPackerIteration#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -80,15 +80,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_iteration#default DataHcpPackerIteration#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_iteration#default DataHcpPackerIteration#default}.
         '''
         value = DataHcpPackerIterationTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -234,15 +234,15 @@
     },
 )
 class DataHcpPackerIterationConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         bucket_name: builtins.str,
         channel: builtins.str,
@@ -253,18 +253,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_iteration#bucket_name DataHcpPackerIteration#bucket_name}
-        :param channel: The channel that points to the version of the image you want. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_iteration#channel DataHcpPackerIteration#channel}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_iteration#id DataHcpPackerIteration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_iteration#timeouts DataHcpPackerIteration#timeouts}
+        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_iteration#bucket_name DataHcpPackerIteration#bucket_name}
+        :param channel: The channel that points to the version of the image you want. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_iteration#channel DataHcpPackerIteration#channel}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_iteration#id DataHcpPackerIteration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_iteration#timeouts DataHcpPackerIteration#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpPackerIterationTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b1907b3a3bbaf110973ff3896d69eb2ee23ee8aa755c517c2430a72823955f9f)
@@ -309,20 +309,22 @@
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
@@ -364,45 +366,45 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def bucket_name(self) -> builtins.str:
         '''The slug of the HCP Packer Registry image bucket to pull from.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_iteration#bucket_name DataHcpPackerIteration#bucket_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_iteration#bucket_name DataHcpPackerIteration#bucket_name}
         '''
         result = self._values.get("bucket_name")
         assert result is not None, "Required property 'bucket_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def channel(self) -> builtins.str:
         '''The channel that points to the version of the image you want.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_iteration#channel DataHcpPackerIteration#channel}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_iteration#channel DataHcpPackerIteration#channel}
         '''
         result = self._values.get("channel")
         assert result is not None, "Required property 'channel' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_iteration#id DataHcpPackerIteration#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_iteration#id DataHcpPackerIteration#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpPackerIterationTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_iteration#timeouts DataHcpPackerIteration#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_iteration#timeouts DataHcpPackerIteration#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpPackerIterationTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -419,26 +421,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpPackerIteration.DataHcpPackerIterationTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpPackerIterationTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_iteration#default DataHcpPackerIteration#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_iteration#default DataHcpPackerIteration#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__bc56ebde634d6984041a03ea104026e4f9ae111de199ff8f95ab8447a5a1e05a)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/packer_iteration#default DataHcpPackerIteration#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/packer_iteration#default DataHcpPackerIteration#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -523,15 +525,15 @@
     id_: builtins.str,
     *,
     bucket_name: builtins.str,
     channel: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcpPackerIterationTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -554,15 +556,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__b1907b3a3bbaf110973ff3896d69eb2ee23ee8aa755c517c2430a72823955f9f(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     bucket_name: builtins.str,
     channel: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_vault_cluster/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_vault_cluster/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_vault_cluster`
 
-Refer to the Terraform Registory for docs: [`data_hcp_vault_cluster`](https://www.terraform.io/docs/providers/hcp/d/vault_cluster).
+Refer to the Terraform Registory for docs: [`data_hcp_vault_cluster`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/vault_cluster).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,43 +22,43 @@
 
 
 class DataHcpVaultCluster(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpVaultCluster.DataHcpVaultCluster",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/d/vault_cluster hcp_vault_cluster}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/vault_cluster hcp_vault_cluster}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_id: builtins.str,
         audit_log_config: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataHcpVaultClusterAuditLogConfig", typing.Dict[builtins.str, typing.Any]]]]] = None,
         id: typing.Optional[builtins.str] = None,
         metrics_config: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataHcpVaultClusterMetricsConfig", typing.Dict[builtins.str, typing.Any]]]]] = None,
         timeouts: typing.Optional[typing.Union["DataHcpVaultClusterTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/d/vault_cluster hcp_vault_cluster} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/vault_cluster hcp_vault_cluster} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/vault_cluster#cluster_id DataHcpVaultCluster#cluster_id}
-        :param audit_log_config: audit_log_config block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/vault_cluster#audit_log_config DataHcpVaultCluster#audit_log_config}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/vault_cluster#id DataHcpVaultCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param metrics_config: metrics_config block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/vault_cluster#metrics_config DataHcpVaultCluster#metrics_config}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/vault_cluster#timeouts DataHcpVaultCluster#timeouts}
+        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/vault_cluster#cluster_id DataHcpVaultCluster#cluster_id}
+        :param audit_log_config: audit_log_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/vault_cluster#audit_log_config DataHcpVaultCluster#audit_log_config}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/vault_cluster#id DataHcpVaultCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param metrics_config: metrics_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/vault_cluster#metrics_config DataHcpVaultCluster#metrics_config}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/vault_cluster#timeouts DataHcpVaultCluster#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -109,15 +109,15 @@
             type_hints = typing.get_type_hints(_typecheckingstub__0f2ed9f26c2e43f2268a672c7574d1dd5434bde5b170e1e29bd79d306680414c)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast(None, jsii.invoke(self, "putMetricsConfig", [value]))
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/vault_cluster#default DataHcpVaultCluster#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/vault_cluster#default DataHcpVaultCluster#default}.
         '''
         value = DataHcpVaultClusterTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetAuditLogConfig")
     def reset_audit_log_config(self) -> None:
@@ -504,15 +504,15 @@
     },
 )
 class DataHcpVaultClusterConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         cluster_id: builtins.str,
         audit_log_config: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataHcpVaultClusterAuditLogConfig, typing.Dict[builtins.str, typing.Any]]]]] = None,
@@ -524,19 +524,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/vault_cluster#cluster_id DataHcpVaultCluster#cluster_id}
-        :param audit_log_config: audit_log_config block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/vault_cluster#audit_log_config DataHcpVaultCluster#audit_log_config}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/vault_cluster#id DataHcpVaultCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param metrics_config: metrics_config block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/vault_cluster#metrics_config DataHcpVaultCluster#metrics_config}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/vault_cluster#timeouts DataHcpVaultCluster#timeouts}
+        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/vault_cluster#cluster_id DataHcpVaultCluster#cluster_id}
+        :param audit_log_config: audit_log_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/vault_cluster#audit_log_config DataHcpVaultCluster#audit_log_config}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/vault_cluster#id DataHcpVaultCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param metrics_config: metrics_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/vault_cluster#metrics_config DataHcpVaultCluster#metrics_config}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/vault_cluster#timeouts DataHcpVaultCluster#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpVaultClusterTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__da593314112c29f9ed1ae10bbea6751cfa957166b81160e91502af33eb797ec5)
@@ -585,20 +585,22 @@
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
@@ -640,57 +642,57 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cluster_id(self) -> builtins.str:
         '''The ID of the HCP Vault cluster.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/vault_cluster#cluster_id DataHcpVaultCluster#cluster_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/vault_cluster#cluster_id DataHcpVaultCluster#cluster_id}
         '''
         result = self._values.get("cluster_id")
         assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def audit_log_config(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataHcpVaultClusterAuditLogConfig]]]:
         '''audit_log_config block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/vault_cluster#audit_log_config DataHcpVaultCluster#audit_log_config}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/vault_cluster#audit_log_config DataHcpVaultCluster#audit_log_config}
         '''
         result = self._values.get("audit_log_config")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataHcpVaultClusterAuditLogConfig]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/vault_cluster#id DataHcpVaultCluster#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/vault_cluster#id DataHcpVaultCluster#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def metrics_config(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataHcpVaultClusterMetricsConfig"]]]:
         '''metrics_config block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/vault_cluster#metrics_config DataHcpVaultCluster#metrics_config}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/vault_cluster#metrics_config DataHcpVaultCluster#metrics_config}
         '''
         result = self._values.get("metrics_config")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataHcpVaultClusterMetricsConfig"]]], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpVaultClusterTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/vault_cluster#timeouts DataHcpVaultCluster#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/vault_cluster#timeouts DataHcpVaultCluster#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpVaultClusterTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1041,26 +1043,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpVaultCluster.DataHcpVaultClusterTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpVaultClusterTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/vault_cluster#default DataHcpVaultCluster#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/vault_cluster#default DataHcpVaultCluster#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__dc864ae2e4ef57eb0c4d269f34764f9957a907ec6662655189f9cec1dfa0b305)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/d/vault_cluster#default DataHcpVaultCluster#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/data-sources/vault_cluster#default DataHcpVaultCluster#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -1155,15 +1157,15 @@
     *,
     cluster_id: builtins.str,
     audit_log_config: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataHcpVaultClusterAuditLogConfig, typing.Dict[builtins.str, typing.Any]]]]] = None,
     id: typing.Optional[builtins.str] = None,
     metrics_config: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataHcpVaultClusterMetricsConfig, typing.Dict[builtins.str, typing.Any]]]]] = None,
     timeouts: typing.Optional[typing.Union[DataHcpVaultClusterTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -1245,15 +1247,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__da593314112c29f9ed1ae10bbea6751cfa957166b81160e91502af33eb797ec5(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     cluster_id: builtins.str,
     audit_log_config: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataHcpVaultClusterAuditLogConfig, typing.Dict[builtins.str, typing.Any]]]]] = None,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/hvn/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/hvn_route/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# `hcp_hvn`
+# `hcp_hvn_route`
 
-Refer to the Terraform Registory for docs: [`hcp_hvn`](https://www.terraform.io/docs/providers/hcp/r/hvn).
+Refer to the Terraform Registory for docs: [`hcp_hvn_route`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -17,67 +17,67 @@
 
 from .._jsii import *
 
 import cdktf as _cdktf_9a9027ec
 import constructs as _constructs_77d1e7e8
 
 
-class Hvn(
+class HvnRoute(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-hcp.hvn.Hvn",
+    jsii_type="@cdktf/provider-hcp.hvnRoute.HvnRoute",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/r/hvn hcp_hvn}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route hcp_hvn_route}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
-        cloud_provider: builtins.str,
-        hvn_id: builtins.str,
-        region: builtins.str,
-        cidr_block: typing.Optional[builtins.str] = None,
+        destination_cidr: builtins.str,
+        hvn_link: builtins.str,
+        hvn_route_id: builtins.str,
+        target_link: builtins.str,
         id: typing.Optional[builtins.str] = None,
-        timeouts: typing.Optional[typing.Union["HvnTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
+        timeouts: typing.Optional[typing.Union["HvnRouteTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/r/hvn hcp_hvn} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route hcp_hvn_route} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cloud_provider: The provider where the HVN is located. The provider 'aws' is generally available and 'azure' is in public beta. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#cloud_provider Hvn#cloud_provider}
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#hvn_id Hvn#hvn_id}
-        :param region: The region where the HVN is located. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#region Hvn#region}
-        :param cidr_block: The CIDR range of the HVN. If this is not provided, the service will provide a default value. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#cidr_block Hvn#cidr_block}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#id Hvn#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#timeouts Hvn#timeouts}
+        :param destination_cidr: The destination CIDR of the HVN route. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#destination_cidr HvnRoute#destination_cidr}
+        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#hvn_link HvnRoute#hvn_link}
+        :param hvn_route_id: The ID of the HVN route. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#hvn_route_id HvnRoute#hvn_route_id}
+        :param target_link: A unique URL identifying the target of the HVN route. Examples of the target: ```aws_network_peering`` <aws_network_peering.md>`_, ```aws_transit_gateway_attachment`` <aws_transit_gateway_attachment.md>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#target_link HvnRoute#target_link}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#id HvnRoute#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#timeouts HvnRoute#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d9c0b08caea8368b936671060ab06f3ecff3c2acd1bdb71cae9606506c352a28)
+            type_hints = typing.get_type_hints(_typecheckingstub__1a17d6b8cf3db69b7342f70da2c474c2d1d7611598e9a7fff081727517345746)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
-        config = HvnConfig(
-            cloud_provider=cloud_provider,
-            hvn_id=hvn_id,
-            region=region,
-            cidr_block=cidr_block,
+        config = HvnRouteConfig(
+            destination_cidr=destination_cidr,
+            hvn_link=hvn_link,
+            hvn_route_id=hvn_route_id,
+            target_link=target_link,
             id=id,
             timeouts=timeouts,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
@@ -92,26 +92,22 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#create Hvn#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#default Hvn#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#delete Hvn#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#create HvnRoute#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#default HvnRoute#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#delete HvnRoute#delete}.
         '''
-        value = HvnTimeouts(create=create, default=default, delete=delete)
+        value = HvnRouteTimeouts(create=create, default=default, delete=delete)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
-    @jsii.member(jsii_name="resetCidrBlock")
-    def reset_cidr_block(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetCidrBlock", []))
-
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetId", []))
 
     @jsii.member(jsii_name="resetTimeouts")
     def reset_timeouts(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetTimeouts", []))
@@ -127,211 +123,197 @@
 
     @builtins.property
     @jsii.member(jsii_name="createdAt")
     def created_at(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "createdAt"))
 
     @builtins.property
-    @jsii.member(jsii_name="organizationId")
-    def organization_id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "organizationId"))
-
-    @builtins.property
-    @jsii.member(jsii_name="projectId")
-    def project_id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "projectId"))
-
-    @builtins.property
-    @jsii.member(jsii_name="providerAccountId")
-    def provider_account_id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "providerAccountId"))
-
-    @builtins.property
     @jsii.member(jsii_name="selfLink")
     def self_link(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "selfLink"))
 
     @builtins.property
     @jsii.member(jsii_name="state")
     def state(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "state"))
 
     @builtins.property
     @jsii.member(jsii_name="timeouts")
-    def timeouts(self) -> "HvnTimeoutsOutputReference":
-        return typing.cast("HvnTimeoutsOutputReference", jsii.get(self, "timeouts"))
+    def timeouts(self) -> "HvnRouteTimeoutsOutputReference":
+        return typing.cast("HvnRouteTimeoutsOutputReference", jsii.get(self, "timeouts"))
 
     @builtins.property
-    @jsii.member(jsii_name="cidrBlockInput")
-    def cidr_block_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "cidrBlockInput"))
+    @jsii.member(jsii_name="destinationCidrInput")
+    def destination_cidr_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "destinationCidrInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="cloudProviderInput")
-    def cloud_provider_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "cloudProviderInput"))
+    @jsii.member(jsii_name="hvnLinkInput")
+    def hvn_link_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "hvnLinkInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="hvnIdInput")
-    def hvn_id_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "hvnIdInput"))
+    @jsii.member(jsii_name="hvnRouteIdInput")
+    def hvn_route_id_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "hvnRouteIdInput"))
 
     @builtins.property
     @jsii.member(jsii_name="idInput")
     def id_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="regionInput")
-    def region_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "regionInput"))
+    @jsii.member(jsii_name="targetLinkInput")
+    def target_link_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "targetLinkInput"))
 
     @builtins.property
     @jsii.member(jsii_name="timeoutsInput")
     def timeouts_input(
         self,
-    ) -> typing.Optional[typing.Union["HvnTimeouts", _cdktf_9a9027ec.IResolvable]]:
-        return typing.cast(typing.Optional[typing.Union["HvnTimeouts", _cdktf_9a9027ec.IResolvable]], jsii.get(self, "timeoutsInput"))
+    ) -> typing.Optional[typing.Union["HvnRouteTimeouts", _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union["HvnRouteTimeouts", _cdktf_9a9027ec.IResolvable]], jsii.get(self, "timeoutsInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="cidrBlock")
-    def cidr_block(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "cidrBlock"))
+    @jsii.member(jsii_name="destinationCidr")
+    def destination_cidr(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "destinationCidr"))
 
-    @cidr_block.setter
-    def cidr_block(self, value: builtins.str) -> None:
+    @destination_cidr.setter
+    def destination_cidr(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__01eea2c7326bb3ea8ab024b1ede34acb60a071dcfef3ab4beb99ae85a90090a4)
+            type_hints = typing.get_type_hints(_typecheckingstub__4a9e54d9ff0c25dc1f1cb4902ccd6d30f010d64704c3318fdd368ea9bcbc7af1)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "cidrBlock", value)
+        jsii.set(self, "destinationCidr", value)
 
     @builtins.property
-    @jsii.member(jsii_name="cloudProvider")
-    def cloud_provider(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "cloudProvider"))
+    @jsii.member(jsii_name="hvnLink")
+    def hvn_link(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "hvnLink"))
 
-    @cloud_provider.setter
-    def cloud_provider(self, value: builtins.str) -> None:
+    @hvn_link.setter
+    def hvn_link(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__1e8d462e6ddd72e6a026cfa9c0e9f7a2ec7529b3bbbc6141a40192c50df98150)
+            type_hints = typing.get_type_hints(_typecheckingstub__69bf3c339aa87cb6cf9e1aa5514a14a9054c44a02f4fc1fc2551ca3d8c1f3968)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "cloudProvider", value)
+        jsii.set(self, "hvnLink", value)
 
     @builtins.property
-    @jsii.member(jsii_name="hvnId")
-    def hvn_id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "hvnId"))
+    @jsii.member(jsii_name="hvnRouteId")
+    def hvn_route_id(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "hvnRouteId"))
 
-    @hvn_id.setter
-    def hvn_id(self, value: builtins.str) -> None:
+    @hvn_route_id.setter
+    def hvn_route_id(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7466dd4240d89ce97202456c249c13b379fdb07e8c9fe6fda8eb9c0a0f737634)
+            type_hints = typing.get_type_hints(_typecheckingstub__476e4cd36b551871725bf628ba44765524cd4e581d6a66d0b64b254a5f73c7c9)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "hvnId", value)
+        jsii.set(self, "hvnRouteId", value)
 
     @builtins.property
     @jsii.member(jsii_name="id")
     def id(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "id"))
 
     @id.setter
     def id(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a5ba3730911d8c28a965bf96d41dde6d044d6080b9168018993c8d716e860289)
+            type_hints = typing.get_type_hints(_typecheckingstub__814a0ed126b8900e8fc119cf255c6c2b059877d571ac1f4c9dfc3344a38bbeb8)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "id", value)
 
     @builtins.property
-    @jsii.member(jsii_name="region")
-    def region(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "region"))
+    @jsii.member(jsii_name="targetLink")
+    def target_link(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "targetLink"))
 
-    @region.setter
-    def region(self, value: builtins.str) -> None:
+    @target_link.setter
+    def target_link(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__87022c9cf10bd5feb0e7b700780a06e4f8dd44488210c29f05f7d6918bb6363e)
+            type_hints = typing.get_type_hints(_typecheckingstub__c9509f91d22ed6edebfeba29a3d564c1df05a2ee9b04281706fdba99514e5a6a)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "region", value)
+        jsii.set(self, "targetLink", value)
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-hcp.hvn.HvnConfig",
+    jsii_type="@cdktf/provider-hcp.hvnRoute.HvnRouteConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
-        "cloud_provider": "cloudProvider",
-        "hvn_id": "hvnId",
-        "region": "region",
-        "cidr_block": "cidrBlock",
+        "destination_cidr": "destinationCidr",
+        "hvn_link": "hvnLink",
+        "hvn_route_id": "hvnRouteId",
+        "target_link": "targetLink",
         "id": "id",
         "timeouts": "timeouts",
     },
 )
-class HvnConfig(_cdktf_9a9027ec.TerraformMetaArguments):
+class HvnRouteConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
-        cloud_provider: builtins.str,
-        hvn_id: builtins.str,
-        region: builtins.str,
-        cidr_block: typing.Optional[builtins.str] = None,
+        destination_cidr: builtins.str,
+        hvn_link: builtins.str,
+        hvn_route_id: builtins.str,
+        target_link: builtins.str,
         id: typing.Optional[builtins.str] = None,
-        timeouts: typing.Optional[typing.Union["HvnTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
+        timeouts: typing.Optional[typing.Union["HvnRouteTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cloud_provider: The provider where the HVN is located. The provider 'aws' is generally available and 'azure' is in public beta. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#cloud_provider Hvn#cloud_provider}
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#hvn_id Hvn#hvn_id}
-        :param region: The region where the HVN is located. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#region Hvn#region}
-        :param cidr_block: The CIDR range of the HVN. If this is not provided, the service will provide a default value. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#cidr_block Hvn#cidr_block}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#id Hvn#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#timeouts Hvn#timeouts}
+        :param destination_cidr: The destination CIDR of the HVN route. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#destination_cidr HvnRoute#destination_cidr}
+        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#hvn_link HvnRoute#hvn_link}
+        :param hvn_route_id: The ID of the HVN route. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#hvn_route_id HvnRoute#hvn_route_id}
+        :param target_link: A unique URL identifying the target of the HVN route. Examples of the target: ```aws_network_peering`` <aws_network_peering.md>`_, ```aws_transit_gateway_attachment`` <aws_transit_gateway_attachment.md>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#target_link HvnRoute#target_link}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#id HvnRoute#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#timeouts HvnRoute#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
-            timeouts = HvnTimeouts(**timeouts)
+            timeouts = HvnRouteTimeouts(**timeouts)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d25a7fdd7ab2372e1a2e11563d24055e64416bf11f211460edfc9e4cac4b0545)
+            type_hints = typing.get_type_hints(_typecheckingstub__a0f8a11ad97253aa3b4db1898b778709d07fdea552ee920fe7548e933e30e5f3)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
-            check_type(argname="argument cloud_provider", value=cloud_provider, expected_type=type_hints["cloud_provider"])
-            check_type(argname="argument hvn_id", value=hvn_id, expected_type=type_hints["hvn_id"])
-            check_type(argname="argument region", value=region, expected_type=type_hints["region"])
-            check_type(argname="argument cidr_block", value=cidr_block, expected_type=type_hints["cidr_block"])
+            check_type(argname="argument destination_cidr", value=destination_cidr, expected_type=type_hints["destination_cidr"])
+            check_type(argname="argument hvn_link", value=hvn_link, expected_type=type_hints["hvn_link"])
+            check_type(argname="argument hvn_route_id", value=hvn_route_id, expected_type=type_hints["hvn_route_id"])
+            check_type(argname="argument target_link", value=target_link, expected_type=type_hints["target_link"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument timeouts", value=timeouts, expected_type=type_hints["timeouts"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
-            "cloud_provider": cloud_provider,
-            "hvn_id": hvn_id,
-            "region": region,
+            "destination_cidr": destination_cidr,
+            "hvn_link": hvn_link,
+            "hvn_route_id": hvn_route_id,
+            "target_link": target_link,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
         if depends_on is not None:
             self._values["depends_on"] = depends_on
@@ -339,16 +321,14 @@
             self._values["for_each"] = for_each
         if lifecycle is not None:
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
-        if cidr_block is not None:
-            self._values["cidr_block"] = cidr_block
         if id is not None:
             self._values["id"] = id
         if timeouts is not None:
             self._values["timeouts"] = timeouts
 
     @builtins.property
     def connection(
@@ -357,20 +337,22 @@
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
@@ -409,160 +391,161 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
-    def cloud_provider(self) -> builtins.str:
-        '''The provider where the HVN is located. The provider 'aws' is generally available and 'azure' is in public beta.
+    def destination_cidr(self) -> builtins.str:
+        '''The destination CIDR of the HVN route.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#cloud_provider Hvn#cloud_provider}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#destination_cidr HvnRoute#destination_cidr}
         '''
-        result = self._values.get("cloud_provider")
-        assert result is not None, "Required property 'cloud_provider' is missing"
+        result = self._values.get("destination_cidr")
+        assert result is not None, "Required property 'destination_cidr' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def hvn_id(self) -> builtins.str:
-        '''The ID of the HashiCorp Virtual Network (HVN).
+    def hvn_link(self) -> builtins.str:
+        '''The ``self_link`` of the HashiCorp Virtual Network (HVN).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#hvn_id Hvn#hvn_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#hvn_link HvnRoute#hvn_link}
         '''
-        result = self._values.get("hvn_id")
-        assert result is not None, "Required property 'hvn_id' is missing"
+        result = self._values.get("hvn_link")
+        assert result is not None, "Required property 'hvn_link' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def region(self) -> builtins.str:
-        '''The region where the HVN is located.
+    def hvn_route_id(self) -> builtins.str:
+        '''The ID of the HVN route.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#region Hvn#region}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#hvn_route_id HvnRoute#hvn_route_id}
         '''
-        result = self._values.get("region")
-        assert result is not None, "Required property 'region' is missing"
+        result = self._values.get("hvn_route_id")
+        assert result is not None, "Required property 'hvn_route_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def cidr_block(self) -> typing.Optional[builtins.str]:
-        '''The CIDR range of the HVN. If this is not provided, the service will provide a default value.
+    def target_link(self) -> builtins.str:
+        '''A unique URL identifying the target of the HVN route. Examples of the target: ```aws_network_peering`` <aws_network_peering.md>`_, ```aws_transit_gateway_attachment`` <aws_transit_gateway_attachment.md>`_.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#cidr_block Hvn#cidr_block}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#target_link HvnRoute#target_link}
         '''
-        result = self._values.get("cidr_block")
-        return typing.cast(typing.Optional[builtins.str], result)
+        result = self._values.get("target_link")
+        assert result is not None, "Required property 'target_link' is missing"
+        return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#id Hvn#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#id HvnRoute#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def timeouts(self) -> typing.Optional["HvnTimeouts"]:
+    def timeouts(self) -> typing.Optional["HvnRouteTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#timeouts Hvn#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#timeouts HvnRoute#timeouts}
         '''
         result = self._values.get("timeouts")
-        return typing.cast(typing.Optional["HvnTimeouts"], result)
+        return typing.cast(typing.Optional["HvnRouteTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "HvnConfig(%s)" % ", ".join(
+        return "HvnRouteConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-hcp.hvn.HvnTimeouts",
+    jsii_type="@cdktf/provider-hcp.hvnRoute.HvnRouteTimeouts",
     jsii_struct_bases=[],
     name_mapping={"create": "create", "default": "default", "delete": "delete"},
 )
-class HvnTimeouts:
+class HvnRouteTimeouts:
     def __init__(
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#create Hvn#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#default Hvn#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#delete Hvn#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#create HvnRoute#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#default HvnRoute#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#delete HvnRoute#delete}.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c6735e0b1a893f99c663fcdd555521d20556b1c3aac0d53912d420fd1bc74eaa)
+            type_hints = typing.get_type_hints(_typecheckingstub__c7530df28c80a750f79162999178fa310eed9eb7c994ca81b4125415b6563456)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if create is not None:
             self._values["create"] = create
         if default is not None:
             self._values["default"] = default
         if delete is not None:
             self._values["delete"] = delete
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#create Hvn#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#create HvnRoute#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#default Hvn#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#default HvnRoute#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn#delete Hvn#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_route#delete HvnRoute#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "HvnTimeouts(%s)" % ", ".join(
+        return "HvnRouteTimeouts(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class HvnTimeoutsOutputReference(
+class HvnRouteTimeoutsOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-hcp.hvn.HvnTimeoutsOutputReference",
+    jsii_type="@cdktf/provider-hcp.hvnRoute.HvnRouteTimeoutsOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a3029689df0bee70166788261ce529a2b33cef6edc47c3aa8cf863428e56e831)
+            type_hints = typing.get_type_hints(_typecheckingstub__3b1f97ab1af4061452a808fd4c975168cc528b0b07ed5bc50b193b7f6b9bf89f)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
     @jsii.member(jsii_name="resetCreate")
     def reset_create(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetCreate", []))
@@ -594,171 +577,171 @@
     @jsii.member(jsii_name="create")
     def create(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "create"))
 
     @create.setter
     def create(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e4050c1bd51bac1ab061ff525d74d6390eb721b7829bed69184bf9fb70f1bde8)
+            type_hints = typing.get_type_hints(_typecheckingstub__43af6be95b0212e893e55f68b02652485eb6a9600db72dc93729c83f27363079)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "create", value)
 
     @builtins.property
     @jsii.member(jsii_name="default")
     def default(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "default"))
 
     @default.setter
     def default(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b655a6b03433b43424170f1d1932d655bb37314d862daca043722c5f529e3eed)
+            type_hints = typing.get_type_hints(_typecheckingstub__9de3b04ca1058744988b9dcdcc913790323dabfebc326ef626467a956a5086ec)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "default", value)
 
     @builtins.property
     @jsii.member(jsii_name="delete")
     def delete(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "delete"))
 
     @delete.setter
     def delete(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__20fc95bdf5da2f082b8394ef5d339ab454fbecbec66fa59a109ff0eb0677bd6f)
+            type_hints = typing.get_type_hints(_typecheckingstub__be9a4c69b9870a24e0632381de585b5fb99537cba3ffba103bc7b803905aabaa)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "delete", value)
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
     def internal_value(
         self,
-    ) -> typing.Optional[typing.Union[HvnTimeouts, _cdktf_9a9027ec.IResolvable]]:
-        return typing.cast(typing.Optional[typing.Union[HvnTimeouts, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "internalValue"))
+    ) -> typing.Optional[typing.Union[HvnRouteTimeouts, _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union[HvnRouteTimeouts, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[typing.Union[HvnTimeouts, _cdktf_9a9027ec.IResolvable]],
+        value: typing.Optional[typing.Union[HvnRouteTimeouts, _cdktf_9a9027ec.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f324f70a650ffb69ab131ae27f6d459090bdcc9e2bc948c722f0d9b1c2fdc6e7)
+            type_hints = typing.get_type_hints(_typecheckingstub__0da6313a3e738335a80309b378e5bd9531ef61b3b919209eb26fa623b1e148b0)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 __all__ = [
-    "Hvn",
-    "HvnConfig",
-    "HvnTimeouts",
-    "HvnTimeoutsOutputReference",
+    "HvnRoute",
+    "HvnRouteConfig",
+    "HvnRouteTimeouts",
+    "HvnRouteTimeoutsOutputReference",
 ]
 
 publication.publish()
 
-def _typecheckingstub__d9c0b08caea8368b936671060ab06f3ecff3c2acd1bdb71cae9606506c352a28(
+def _typecheckingstub__1a17d6b8cf3db69b7342f70da2c474c2d1d7611598e9a7fff081727517345746(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
-    cloud_provider: builtins.str,
-    hvn_id: builtins.str,
-    region: builtins.str,
-    cidr_block: typing.Optional[builtins.str] = None,
+    destination_cidr: builtins.str,
+    hvn_link: builtins.str,
+    hvn_route_id: builtins.str,
+    target_link: builtins.str,
     id: typing.Optional[builtins.str] = None,
-    timeouts: typing.Optional[typing.Union[HvnTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
+    timeouts: typing.Optional[typing.Union[HvnRouteTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
     pass
 
-def _typecheckingstub__01eea2c7326bb3ea8ab024b1ede34acb60a071dcfef3ab4beb99ae85a90090a4(
+def _typecheckingstub__4a9e54d9ff0c25dc1f1cb4902ccd6d30f010d64704c3318fdd368ea9bcbc7af1(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__1e8d462e6ddd72e6a026cfa9c0e9f7a2ec7529b3bbbc6141a40192c50df98150(
+def _typecheckingstub__69bf3c339aa87cb6cf9e1aa5514a14a9054c44a02f4fc1fc2551ca3d8c1f3968(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__7466dd4240d89ce97202456c249c13b379fdb07e8c9fe6fda8eb9c0a0f737634(
+def _typecheckingstub__476e4cd36b551871725bf628ba44765524cd4e581d6a66d0b64b254a5f73c7c9(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__a5ba3730911d8c28a965bf96d41dde6d044d6080b9168018993c8d716e860289(
+def _typecheckingstub__814a0ed126b8900e8fc119cf255c6c2b059877d571ac1f4c9dfc3344a38bbeb8(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__87022c9cf10bd5feb0e7b700780a06e4f8dd44488210c29f05f7d6918bb6363e(
+def _typecheckingstub__c9509f91d22ed6edebfeba29a3d564c1df05a2ee9b04281706fdba99514e5a6a(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__d25a7fdd7ab2372e1a2e11563d24055e64416bf11f211460edfc9e4cac4b0545(
+def _typecheckingstub__a0f8a11ad97253aa3b4db1898b778709d07fdea552ee920fe7548e933e30e5f3(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
-    cloud_provider: builtins.str,
-    hvn_id: builtins.str,
-    region: builtins.str,
-    cidr_block: typing.Optional[builtins.str] = None,
+    destination_cidr: builtins.str,
+    hvn_link: builtins.str,
+    hvn_route_id: builtins.str,
+    target_link: builtins.str,
     id: typing.Optional[builtins.str] = None,
-    timeouts: typing.Optional[typing.Union[HvnTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
+    timeouts: typing.Optional[typing.Union[HvnRouteTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__c6735e0b1a893f99c663fcdd555521d20556b1c3aac0d53912d420fd1bc74eaa(
+def _typecheckingstub__c7530df28c80a750f79162999178fa310eed9eb7c994ca81b4125415b6563456(
     *,
     create: typing.Optional[builtins.str] = None,
     default: typing.Optional[builtins.str] = None,
     delete: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__a3029689df0bee70166788261ce529a2b33cef6edc47c3aa8cf863428e56e831(
+def _typecheckingstub__3b1f97ab1af4061452a808fd4c975168cc528b0b07ed5bc50b193b7f6b9bf89f(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__e4050c1bd51bac1ab061ff525d74d6390eb721b7829bed69184bf9fb70f1bde8(
+def _typecheckingstub__43af6be95b0212e893e55f68b02652485eb6a9600db72dc93729c83f27363079(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__b655a6b03433b43424170f1d1932d655bb37314d862daca043722c5f529e3eed(
+def _typecheckingstub__9de3b04ca1058744988b9dcdcc913790323dabfebc326ef626467a956a5086ec(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__20fc95bdf5da2f082b8394ef5d339ab454fbecbec66fa59a109ff0eb0677bd6f(
+def _typecheckingstub__be9a4c69b9870a24e0632381de585b5fb99537cba3ffba103bc7b803905aabaa(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__f324f70a650ffb69ab131ae27f6d459090bdcc9e2bc948c722f0d9b1c2fdc6e7(
-    value: typing.Optional[typing.Union[HvnTimeouts, _cdktf_9a9027ec.IResolvable]],
+def _typecheckingstub__0da6313a3e738335a80309b378e5bd9531ef61b3b919209eb26fa623b1e148b0(
+    value: typing.Optional[typing.Union[HvnRouteTimeouts, _cdktf_9a9027ec.IResolvable]],
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/hvn_peering_connection/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/hvn_peering_connection/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_hvn_peering_connection`
 
-Refer to the Terraform Registory for docs: [`hcp_hvn_peering_connection`](https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection).
+Refer to the Terraform Registory for docs: [`hcp_hvn_peering_connection`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,41 +22,41 @@
 
 
 class HvnPeeringConnection(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.hvnPeeringConnection.HvnPeeringConnection",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection hcp_hvn_peering_connection}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection hcp_hvn_peering_connection}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         hvn1: builtins.str,
         hvn2: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["HvnPeeringConnectionTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection hcp_hvn_peering_connection} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection hcp_hvn_peering_connection} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param hvn1: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection#hvn_1 HvnPeeringConnection#hvn_1}
-        :param hvn2: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection#hvn_2 HvnPeeringConnection#hvn_2}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection#id HvnPeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection#timeouts HvnPeeringConnection#timeouts}
+        :param hvn1: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection#hvn_1 HvnPeeringConnection#hvn_1}
+        :param hvn2: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection#hvn_2 HvnPeeringConnection#hvn_2}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection#id HvnPeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection#timeouts HvnPeeringConnection#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -86,17 +86,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection#create HvnPeeringConnection#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection#default HvnPeeringConnection#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection#delete HvnPeeringConnection#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection#create HvnPeeringConnection#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection#default HvnPeeringConnection#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection#delete HvnPeeringConnection#delete}.
         '''
         value = HvnPeeringConnectionTimeouts(
             create=create, default=default, delete=delete
         )
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
@@ -234,15 +234,15 @@
     },
 )
 class HvnPeeringConnectionConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         hvn1: builtins.str,
         hvn2: builtins.str,
@@ -253,18 +253,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param hvn1: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection#hvn_1 HvnPeeringConnection#hvn_1}
-        :param hvn2: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection#hvn_2 HvnPeeringConnection#hvn_2}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection#id HvnPeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection#timeouts HvnPeeringConnection#timeouts}
+        :param hvn1: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection#hvn_1 HvnPeeringConnection#hvn_1}
+        :param hvn2: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection#hvn_2 HvnPeeringConnection#hvn_2}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection#id HvnPeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection#timeouts HvnPeeringConnection#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = HvnPeeringConnectionTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__78dd0c35c825813a5a19efd778b3a9008690809616f2a6c869b89e19d3ad99c3)
@@ -309,20 +309,22 @@
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
@@ -364,45 +366,45 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def hvn1(self) -> builtins.str:
         '''The unique URL of one of the HVNs being peered.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection#hvn_1 HvnPeeringConnection#hvn_1}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection#hvn_1 HvnPeeringConnection#hvn_1}
         '''
         result = self._values.get("hvn1")
         assert result is not None, "Required property 'hvn1' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def hvn2(self) -> builtins.str:
         '''The unique URL of one of the HVNs being peered.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection#hvn_2 HvnPeeringConnection#hvn_2}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection#hvn_2 HvnPeeringConnection#hvn_2}
         '''
         result = self._values.get("hvn2")
         assert result is not None, "Required property 'hvn2' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection#id HvnPeeringConnection#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection#id HvnPeeringConnection#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["HvnPeeringConnectionTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection#timeouts HvnPeeringConnection#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection#timeouts HvnPeeringConnection#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["HvnPeeringConnectionTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -425,17 +427,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection#create HvnPeeringConnection#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection#default HvnPeeringConnection#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection#delete HvnPeeringConnection#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection#create HvnPeeringConnection#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection#default HvnPeeringConnection#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection#delete HvnPeeringConnection#delete}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6d89673ab7be9279ee2024c9587ecdae2ebfc5be5a751caaa32e70ba4ca3975f)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -444,27 +446,27 @@
         if default is not None:
             self._values["default"] = default
         if delete is not None:
             self._values["delete"] = delete
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection#create HvnPeeringConnection#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection#create HvnPeeringConnection#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection#default HvnPeeringConnection#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection#default HvnPeeringConnection#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_peering_connection#delete HvnPeeringConnection#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/hvn_peering_connection#delete HvnPeeringConnection#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -591,15 +593,15 @@
     id_: builtins.str,
     *,
     hvn1: builtins.str,
     hvn2: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[HvnPeeringConnectionTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -622,15 +624,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__78dd0c35c825813a5a19efd778b3a9008690809616f2a6c869b89e19d3ad99c3(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     hvn1: builtins.str,
     hvn2: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/hvn_route/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/vault_cluster_admin_token/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# `hcp_hvn_route`
+# `hcp_vault_cluster_admin_token`
 
-Refer to the Terraform Registory for docs: [`hcp_hvn_route`](https://www.terraform.io/docs/providers/hcp/r/hvn_route).
+Refer to the Terraform Registory for docs: [`hcp_vault_cluster_admin_token`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster_admin_token).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -17,67 +17,58 @@
 
 from .._jsii import *
 
 import cdktf as _cdktf_9a9027ec
 import constructs as _constructs_77d1e7e8
 
 
-class HvnRoute(
+class VaultClusterAdminToken(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-hcp.hvnRoute.HvnRoute",
+    jsii_type="@cdktf/provider-hcp.vaultClusterAdminToken.VaultClusterAdminToken",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route hcp_hvn_route}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster_admin_token hcp_vault_cluster_admin_token}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
-        destination_cidr: builtins.str,
-        hvn_link: builtins.str,
-        hvn_route_id: builtins.str,
-        target_link: builtins.str,
+        cluster_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
-        timeouts: typing.Optional[typing.Union["HvnRouteTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
+        timeouts: typing.Optional[typing.Union["VaultClusterAdminTokenTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route hcp_hvn_route} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster_admin_token hcp_vault_cluster_admin_token} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param destination_cidr: The destination CIDR of the HVN route. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#destination_cidr HvnRoute#destination_cidr}
-        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#hvn_link HvnRoute#hvn_link}
-        :param hvn_route_id: The ID of the HVN route. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#hvn_route_id HvnRoute#hvn_route_id}
-        :param target_link: A unique URL identifying the target of the HVN route. Examples of the target: ```aws_network_peering`` <aws_network_peering.md>`_, ```aws_transit_gateway_attachment`` <aws_transit_gateway_attachment.md>`_. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#target_link HvnRoute#target_link}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#id HvnRoute#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#timeouts HvnRoute#timeouts}
+        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster_admin_token#cluster_id VaultClusterAdminToken#cluster_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster_admin_token#id VaultClusterAdminToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster_admin_token#timeouts VaultClusterAdminToken#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__1a17d6b8cf3db69b7342f70da2c474c2d1d7611598e9a7fff081727517345746)
+            type_hints = typing.get_type_hints(_typecheckingstub__a5f8b29e232f21f17cb5b1144d8fe521a550d4d67069f03a590e7aec0a072552)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
-        config = HvnRouteConfig(
-            destination_cidr=destination_cidr,
-            hvn_link=hvn_link,
-            hvn_route_id=hvn_route_id,
-            target_link=target_link,
+        config = VaultClusterAdminTokenConfig(
+            cluster_id=cluster_id,
             id=id,
             timeouts=timeouts,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
@@ -88,23 +79,23 @@
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(
         self,
         *,
         create: typing.Optional[builtins.str] = None,
-        default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
+        read: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#create HvnRoute#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#default HvnRoute#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#delete HvnRoute#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster_admin_token#create VaultClusterAdminToken#create}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster_admin_token#delete VaultClusterAdminToken#delete}.
+        :param read: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster_admin_token#read VaultClusterAdminToken#read}.
         '''
-        value = HvnRouteTimeouts(create=create, default=default, delete=delete)
+        value = VaultClusterAdminTokenTimeouts(create=create, delete=delete, read=read)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetId", []))
 
@@ -123,197 +114,126 @@
 
     @builtins.property
     @jsii.member(jsii_name="createdAt")
     def created_at(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "createdAt"))
 
     @builtins.property
-    @jsii.member(jsii_name="selfLink")
-    def self_link(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "selfLink"))
-
-    @builtins.property
-    @jsii.member(jsii_name="state")
-    def state(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "state"))
-
-    @builtins.property
     @jsii.member(jsii_name="timeouts")
-    def timeouts(self) -> "HvnRouteTimeoutsOutputReference":
-        return typing.cast("HvnRouteTimeoutsOutputReference", jsii.get(self, "timeouts"))
-
-    @builtins.property
-    @jsii.member(jsii_name="destinationCidrInput")
-    def destination_cidr_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "destinationCidrInput"))
+    def timeouts(self) -> "VaultClusterAdminTokenTimeoutsOutputReference":
+        return typing.cast("VaultClusterAdminTokenTimeoutsOutputReference", jsii.get(self, "timeouts"))
 
     @builtins.property
-    @jsii.member(jsii_name="hvnLinkInput")
-    def hvn_link_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "hvnLinkInput"))
+    @jsii.member(jsii_name="token")
+    def token(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "token"))
 
     @builtins.property
-    @jsii.member(jsii_name="hvnRouteIdInput")
-    def hvn_route_id_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "hvnRouteIdInput"))
+    @jsii.member(jsii_name="clusterIdInput")
+    def cluster_id_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "clusterIdInput"))
 
     @builtins.property
     @jsii.member(jsii_name="idInput")
     def id_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="targetLinkInput")
-    def target_link_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "targetLinkInput"))
-
-    @builtins.property
     @jsii.member(jsii_name="timeoutsInput")
     def timeouts_input(
         self,
-    ) -> typing.Optional[typing.Union["HvnRouteTimeouts", _cdktf_9a9027ec.IResolvable]]:
-        return typing.cast(typing.Optional[typing.Union["HvnRouteTimeouts", _cdktf_9a9027ec.IResolvable]], jsii.get(self, "timeoutsInput"))
+    ) -> typing.Optional[typing.Union["VaultClusterAdminTokenTimeouts", _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union["VaultClusterAdminTokenTimeouts", _cdktf_9a9027ec.IResolvable]], jsii.get(self, "timeoutsInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="destinationCidr")
-    def destination_cidr(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "destinationCidr"))
+    @jsii.member(jsii_name="clusterId")
+    def cluster_id(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "clusterId"))
 
-    @destination_cidr.setter
-    def destination_cidr(self, value: builtins.str) -> None:
+    @cluster_id.setter
+    def cluster_id(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4a9e54d9ff0c25dc1f1cb4902ccd6d30f010d64704c3318fdd368ea9bcbc7af1)
+            type_hints = typing.get_type_hints(_typecheckingstub__a5b411e34dd90efc5b743f58062e093a6161d76f4b9d3bcc3977064c9a18c734)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "destinationCidr", value)
-
-    @builtins.property
-    @jsii.member(jsii_name="hvnLink")
-    def hvn_link(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "hvnLink"))
-
-    @hvn_link.setter
-    def hvn_link(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__69bf3c339aa87cb6cf9e1aa5514a14a9054c44a02f4fc1fc2551ca3d8c1f3968)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "hvnLink", value)
-
-    @builtins.property
-    @jsii.member(jsii_name="hvnRouteId")
-    def hvn_route_id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "hvnRouteId"))
-
-    @hvn_route_id.setter
-    def hvn_route_id(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__476e4cd36b551871725bf628ba44765524cd4e581d6a66d0b64b254a5f73c7c9)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "hvnRouteId", value)
+        jsii.set(self, "clusterId", value)
 
     @builtins.property
     @jsii.member(jsii_name="id")
     def id(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "id"))
 
     @id.setter
     def id(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__814a0ed126b8900e8fc119cf255c6c2b059877d571ac1f4c9dfc3344a38bbeb8)
+            type_hints = typing.get_type_hints(_typecheckingstub__9eeeaa88556995a85150bab5b8ea50a8d37aebb46c401e1f864b66f494cd6e7f)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "id", value)
 
-    @builtins.property
-    @jsii.member(jsii_name="targetLink")
-    def target_link(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "targetLink"))
-
-    @target_link.setter
-    def target_link(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c9509f91d22ed6edebfeba29a3d564c1df05a2ee9b04281706fdba99514e5a6a)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "targetLink", value)
-
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-hcp.hvnRoute.HvnRouteConfig",
+    jsii_type="@cdktf/provider-hcp.vaultClusterAdminToken.VaultClusterAdminTokenConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
-        "destination_cidr": "destinationCidr",
-        "hvn_link": "hvnLink",
-        "hvn_route_id": "hvnRouteId",
-        "target_link": "targetLink",
+        "cluster_id": "clusterId",
         "id": "id",
         "timeouts": "timeouts",
     },
 )
-class HvnRouteConfig(_cdktf_9a9027ec.TerraformMetaArguments):
+class VaultClusterAdminTokenConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
-        destination_cidr: builtins.str,
-        hvn_link: builtins.str,
-        hvn_route_id: builtins.str,
-        target_link: builtins.str,
+        cluster_id: builtins.str,
         id: typing.Optional[builtins.str] = None,
-        timeouts: typing.Optional[typing.Union["HvnRouteTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
+        timeouts: typing.Optional[typing.Union["VaultClusterAdminTokenTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param destination_cidr: The destination CIDR of the HVN route. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#destination_cidr HvnRoute#destination_cidr}
-        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#hvn_link HvnRoute#hvn_link}
-        :param hvn_route_id: The ID of the HVN route. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#hvn_route_id HvnRoute#hvn_route_id}
-        :param target_link: A unique URL identifying the target of the HVN route. Examples of the target: ```aws_network_peering`` <aws_network_peering.md>`_, ```aws_transit_gateway_attachment`` <aws_transit_gateway_attachment.md>`_. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#target_link HvnRoute#target_link}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#id HvnRoute#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#timeouts HvnRoute#timeouts}
+        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster_admin_token#cluster_id VaultClusterAdminToken#cluster_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster_admin_token#id VaultClusterAdminToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster_admin_token#timeouts VaultClusterAdminToken#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
-            timeouts = HvnRouteTimeouts(**timeouts)
+            timeouts = VaultClusterAdminTokenTimeouts(**timeouts)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a0f8a11ad97253aa3b4db1898b778709d07fdea552ee920fe7548e933e30e5f3)
+            type_hints = typing.get_type_hints(_typecheckingstub__83e679d92c18871e7ba585dbaa17bf175d7732a6c8292545e7d48798de47cf92)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
-            check_type(argname="argument destination_cidr", value=destination_cidr, expected_type=type_hints["destination_cidr"])
-            check_type(argname="argument hvn_link", value=hvn_link, expected_type=type_hints["hvn_link"])
-            check_type(argname="argument hvn_route_id", value=hvn_route_id, expected_type=type_hints["hvn_route_id"])
-            check_type(argname="argument target_link", value=target_link, expected_type=type_hints["target_link"])
+            check_type(argname="argument cluster_id", value=cluster_id, expected_type=type_hints["cluster_id"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument timeouts", value=timeouts, expected_type=type_hints["timeouts"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
-            "destination_cidr": destination_cidr,
-            "hvn_link": hvn_link,
-            "hvn_route_id": hvn_route_id,
-            "target_link": target_link,
+            "cluster_id": cluster_id,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
         if depends_on is not None:
             self._values["depends_on"] = depends_on
@@ -337,20 +257,22 @@
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
@@ -389,357 +311,303 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
-    def destination_cidr(self) -> builtins.str:
-        '''The destination CIDR of the HVN route.
-
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#destination_cidr HvnRoute#destination_cidr}
-        '''
-        result = self._values.get("destination_cidr")
-        assert result is not None, "Required property 'destination_cidr' is missing"
-        return typing.cast(builtins.str, result)
-
-    @builtins.property
-    def hvn_link(self) -> builtins.str:
-        '''The ``self_link`` of the HashiCorp Virtual Network (HVN).
-
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#hvn_link HvnRoute#hvn_link}
-        '''
-        result = self._values.get("hvn_link")
-        assert result is not None, "Required property 'hvn_link' is missing"
-        return typing.cast(builtins.str, result)
-
-    @builtins.property
-    def hvn_route_id(self) -> builtins.str:
-        '''The ID of the HVN route.
-
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#hvn_route_id HvnRoute#hvn_route_id}
-        '''
-        result = self._values.get("hvn_route_id")
-        assert result is not None, "Required property 'hvn_route_id' is missing"
-        return typing.cast(builtins.str, result)
-
-    @builtins.property
-    def target_link(self) -> builtins.str:
-        '''A unique URL identifying the target of the HVN route. Examples of the target: ```aws_network_peering`` <aws_network_peering.md>`_, ```aws_transit_gateway_attachment`` <aws_transit_gateway_attachment.md>`_.
+    def cluster_id(self) -> builtins.str:
+        '''The ID of the HCP Vault cluster.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#target_link HvnRoute#target_link}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster_admin_token#cluster_id VaultClusterAdminToken#cluster_id}
         '''
-        result = self._values.get("target_link")
-        assert result is not None, "Required property 'target_link' is missing"
+        result = self._values.get("cluster_id")
+        assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#id HvnRoute#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster_admin_token#id VaultClusterAdminToken#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def timeouts(self) -> typing.Optional["HvnRouteTimeouts"]:
+    def timeouts(self) -> typing.Optional["VaultClusterAdminTokenTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#timeouts HvnRoute#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster_admin_token#timeouts VaultClusterAdminToken#timeouts}
         '''
         result = self._values.get("timeouts")
-        return typing.cast(typing.Optional["HvnRouteTimeouts"], result)
+        return typing.cast(typing.Optional["VaultClusterAdminTokenTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "HvnRouteConfig(%s)" % ", ".join(
+        return "VaultClusterAdminTokenConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-hcp.hvnRoute.HvnRouteTimeouts",
+    jsii_type="@cdktf/provider-hcp.vaultClusterAdminToken.VaultClusterAdminTokenTimeouts",
     jsii_struct_bases=[],
-    name_mapping={"create": "create", "default": "default", "delete": "delete"},
+    name_mapping={"create": "create", "delete": "delete", "read": "read"},
 )
-class HvnRouteTimeouts:
+class VaultClusterAdminTokenTimeouts:
     def __init__(
         self,
         *,
         create: typing.Optional[builtins.str] = None,
-        default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
+        read: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#create HvnRoute#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#default HvnRoute#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#delete HvnRoute#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster_admin_token#create VaultClusterAdminToken#create}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster_admin_token#delete VaultClusterAdminToken#delete}.
+        :param read: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster_admin_token#read VaultClusterAdminToken#read}.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c7530df28c80a750f79162999178fa310eed9eb7c994ca81b4125415b6563456)
+            type_hints = typing.get_type_hints(_typecheckingstub__7b913c5a37226d68faee27ca7806a92620ab10ea5f6187e16ee77f2822bc1d2d)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
-            check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
+            check_type(argname="argument read", value=read, expected_type=type_hints["read"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if create is not None:
             self._values["create"] = create
-        if default is not None:
-            self._values["default"] = default
         if delete is not None:
             self._values["delete"] = delete
+        if read is not None:
+            self._values["read"] = read
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#create HvnRoute#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster_admin_token#create VaultClusterAdminToken#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#default HvnRoute#default}.'''
-        result = self._values.get("default")
+    def delete(self) -> typing.Optional[builtins.str]:
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster_admin_token#delete VaultClusterAdminToken#delete}.'''
+        result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/hvn_route#delete HvnRoute#delete}.'''
-        result = self._values.get("delete")
+    def read(self) -> typing.Optional[builtins.str]:
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster_admin_token#read VaultClusterAdminToken#read}.'''
+        result = self._values.get("read")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "HvnRouteTimeouts(%s)" % ", ".join(
+        return "VaultClusterAdminTokenTimeouts(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class HvnRouteTimeoutsOutputReference(
+class VaultClusterAdminTokenTimeoutsOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-hcp.hvnRoute.HvnRouteTimeoutsOutputReference",
+    jsii_type="@cdktf/provider-hcp.vaultClusterAdminToken.VaultClusterAdminTokenTimeoutsOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__3b1f97ab1af4061452a808fd4c975168cc528b0b07ed5bc50b193b7f6b9bf89f)
+            type_hints = typing.get_type_hints(_typecheckingstub__20ffdfbe029215c187d51ae037057685bfd69f2a8ca3110566b71f0d977f6ea7)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
     @jsii.member(jsii_name="resetCreate")
     def reset_create(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetCreate", []))
 
-    @jsii.member(jsii_name="resetDefault")
-    def reset_default(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetDefault", []))
-
     @jsii.member(jsii_name="resetDelete")
     def reset_delete(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetDelete", []))
 
+    @jsii.member(jsii_name="resetRead")
+    def reset_read(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetRead", []))
+
     @builtins.property
     @jsii.member(jsii_name="createInput")
     def create_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "createInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="defaultInput")
-    def default_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "defaultInput"))
-
-    @builtins.property
     @jsii.member(jsii_name="deleteInput")
     def delete_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "deleteInput"))
 
     @builtins.property
+    @jsii.member(jsii_name="readInput")
+    def read_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "readInput"))
+
+    @builtins.property
     @jsii.member(jsii_name="create")
     def create(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "create"))
 
     @create.setter
     def create(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__43af6be95b0212e893e55f68b02652485eb6a9600db72dc93729c83f27363079)
+            type_hints = typing.get_type_hints(_typecheckingstub__d5291d129796399619f6096866f63458c1954193aa3497539396b2e4f571d371)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "create", value)
 
     @builtins.property
-    @jsii.member(jsii_name="default")
-    def default(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "default"))
-
-    @default.setter
-    def default(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__9de3b04ca1058744988b9dcdcc913790323dabfebc326ef626467a956a5086ec)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "default", value)
-
-    @builtins.property
     @jsii.member(jsii_name="delete")
     def delete(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "delete"))
 
     @delete.setter
     def delete(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__be9a4c69b9870a24e0632381de585b5fb99537cba3ffba103bc7b803905aabaa)
+            type_hints = typing.get_type_hints(_typecheckingstub__ffe47e4bbec2ac695f05f28eb6b3779ae411a4490e454cb359d51d28a9ed0d38)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "delete", value)
 
     @builtins.property
+    @jsii.member(jsii_name="read")
+    def read(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "read"))
+
+    @read.setter
+    def read(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__f1caa623946819cc777acae2b9421024ae3504f189dabd8b302744214facaa2b)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "read", value)
+
+    @builtins.property
     @jsii.member(jsii_name="internalValue")
     def internal_value(
         self,
-    ) -> typing.Optional[typing.Union[HvnRouteTimeouts, _cdktf_9a9027ec.IResolvable]]:
-        return typing.cast(typing.Optional[typing.Union[HvnRouteTimeouts, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "internalValue"))
+    ) -> typing.Optional[typing.Union[VaultClusterAdminTokenTimeouts, _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union[VaultClusterAdminTokenTimeouts, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[typing.Union[HvnRouteTimeouts, _cdktf_9a9027ec.IResolvable]],
+        value: typing.Optional[typing.Union[VaultClusterAdminTokenTimeouts, _cdktf_9a9027ec.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0da6313a3e738335a80309b378e5bd9531ef61b3b919209eb26fa623b1e148b0)
+            type_hints = typing.get_type_hints(_typecheckingstub__1d511258a846a731c9603c6d9a77d0bc88f34d7825b2e33a92b372a86e48c2dc)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 __all__ = [
-    "HvnRoute",
-    "HvnRouteConfig",
-    "HvnRouteTimeouts",
-    "HvnRouteTimeoutsOutputReference",
+    "VaultClusterAdminToken",
+    "VaultClusterAdminTokenConfig",
+    "VaultClusterAdminTokenTimeouts",
+    "VaultClusterAdminTokenTimeoutsOutputReference",
 ]
 
 publication.publish()
 
-def _typecheckingstub__1a17d6b8cf3db69b7342f70da2c474c2d1d7611598e9a7fff081727517345746(
+def _typecheckingstub__a5f8b29e232f21f17cb5b1144d8fe521a550d4d67069f03a590e7aec0a072552(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
-    destination_cidr: builtins.str,
-    hvn_link: builtins.str,
-    hvn_route_id: builtins.str,
-    target_link: builtins.str,
+    cluster_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
-    timeouts: typing.Optional[typing.Union[HvnRouteTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
+    timeouts: typing.Optional[typing.Union[VaultClusterAdminTokenTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
     pass
 
-def _typecheckingstub__4a9e54d9ff0c25dc1f1cb4902ccd6d30f010d64704c3318fdd368ea9bcbc7af1(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__69bf3c339aa87cb6cf9e1aa5514a14a9054c44a02f4fc1fc2551ca3d8c1f3968(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__476e4cd36b551871725bf628ba44765524cd4e581d6a66d0b64b254a5f73c7c9(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__814a0ed126b8900e8fc119cf255c6c2b059877d571ac1f4c9dfc3344a38bbeb8(
+def _typecheckingstub__a5b411e34dd90efc5b743f58062e093a6161d76f4b9d3bcc3977064c9a18c734(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__c9509f91d22ed6edebfeba29a3d564c1df05a2ee9b04281706fdba99514e5a6a(
+def _typecheckingstub__9eeeaa88556995a85150bab5b8ea50a8d37aebb46c401e1f864b66f494cd6e7f(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__a0f8a11ad97253aa3b4db1898b778709d07fdea552ee920fe7548e933e30e5f3(
+def _typecheckingstub__83e679d92c18871e7ba585dbaa17bf175d7732a6c8292545e7d48798de47cf92(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
-    destination_cidr: builtins.str,
-    hvn_link: builtins.str,
-    hvn_route_id: builtins.str,
-    target_link: builtins.str,
+    cluster_id: builtins.str,
     id: typing.Optional[builtins.str] = None,
-    timeouts: typing.Optional[typing.Union[HvnRouteTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
+    timeouts: typing.Optional[typing.Union[VaultClusterAdminTokenTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__c7530df28c80a750f79162999178fa310eed9eb7c994ca81b4125415b6563456(
+def _typecheckingstub__7b913c5a37226d68faee27ca7806a92620ab10ea5f6187e16ee77f2822bc1d2d(
     *,
     create: typing.Optional[builtins.str] = None,
-    default: typing.Optional[builtins.str] = None,
     delete: typing.Optional[builtins.str] = None,
+    read: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__3b1f97ab1af4061452a808fd4c975168cc528b0b07ed5bc50b193b7f6b9bf89f(
+def _typecheckingstub__20ffdfbe029215c187d51ae037057685bfd69f2a8ca3110566b71f0d977f6ea7(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__43af6be95b0212e893e55f68b02652485eb6a9600db72dc93729c83f27363079(
+def _typecheckingstub__d5291d129796399619f6096866f63458c1954193aa3497539396b2e4f571d371(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__9de3b04ca1058744988b9dcdcc913790323dabfebc326ef626467a956a5086ec(
+def _typecheckingstub__ffe47e4bbec2ac695f05f28eb6b3779ae411a4490e454cb359d51d28a9ed0d38(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__be9a4c69b9870a24e0632381de585b5fb99537cba3ffba103bc7b803905aabaa(
+def _typecheckingstub__f1caa623946819cc777acae2b9421024ae3504f189dabd8b302744214facaa2b(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__0da6313a3e738335a80309b378e5bd9531ef61b3b919209eb26fa623b1e148b0(
-    value: typing.Optional[typing.Union[HvnRouteTimeouts, _cdktf_9a9027ec.IResolvable]],
+def _typecheckingstub__1d511258a846a731c9603c6d9a77d0bc88f34d7825b2e33a92b372a86e48c2dc(
+    value: typing.Optional[typing.Union[VaultClusterAdminTokenTimeouts, _cdktf_9a9027ec.IResolvable]],
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/packer_channel/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/packer_channel/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_packer_channel`
 
-Refer to the Terraform Registory for docs: [`hcp_packer_channel`](https://www.terraform.io/docs/providers/hcp/r/packer_channel).
+Refer to the Terraform Registory for docs: [`hcp_packer_channel`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,43 +22,43 @@
 
 
 class PackerChannel(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.packerChannel.PackerChannel",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel hcp_packer_channel}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel hcp_packer_channel}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         bucket_name: builtins.str,
         name: builtins.str,
         id: typing.Optional[builtins.str] = None,
         iteration: typing.Optional[typing.Union["PackerChannelIteration", typing.Dict[builtins.str, typing.Any]]] = None,
         timeouts: typing.Optional[typing.Union["PackerChannelTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel hcp_packer_channel} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel hcp_packer_channel} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param bucket_name: The slug of the HCP Packer Registry image bucket where the channel should be created in. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#bucket_name PackerChannel#bucket_name}
-        :param name: The name of the channel being managed. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#name PackerChannel#name}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#id PackerChannel#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param iteration: iteration block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#iteration PackerChannel#iteration}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#timeouts PackerChannel#timeouts}
+        :param bucket_name: The slug of the HCP Packer Registry image bucket where the channel should be created in. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#bucket_name PackerChannel#bucket_name}
+        :param name: The name of the channel being managed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#name PackerChannel#name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#id PackerChannel#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param iteration: iteration block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#iteration PackerChannel#iteration}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#timeouts PackerChannel#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -89,17 +89,17 @@
         self,
         *,
         fingerprint: typing.Optional[builtins.str] = None,
         id: typing.Optional[builtins.str] = None,
         incremental_version: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
-        :param fingerprint: The fingerprint of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#fingerprint PackerChannel#fingerprint}
-        :param id: The ID of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#id PackerChannel#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param incremental_version: The incremental_version of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#incremental_version PackerChannel#incremental_version}
+        :param fingerprint: The fingerprint of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#fingerprint PackerChannel#fingerprint}
+        :param id: The ID of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#id PackerChannel#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param incremental_version: The incremental_version of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#incremental_version PackerChannel#incremental_version}
         '''
         value = PackerChannelIteration(
             fingerprint=fingerprint, id=id, incremental_version=incremental_version
         )
 
         return typing.cast(None, jsii.invoke(self, "putIteration", [value]))
 
@@ -109,18 +109,18 @@
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#create PackerChannel#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#default PackerChannel#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#delete PackerChannel#delete}.
-        :param update: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#update PackerChannel#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#create PackerChannel#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#default PackerChannel#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#delete PackerChannel#delete}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#update PackerChannel#update}.
         '''
         value = PackerChannelTimeouts(
             create=create, default=default, delete=delete, update=update
         )
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
@@ -263,15 +263,15 @@
     },
 )
 class PackerChannelConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         bucket_name: builtins.str,
         name: builtins.str,
@@ -283,19 +283,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param bucket_name: The slug of the HCP Packer Registry image bucket where the channel should be created in. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#bucket_name PackerChannel#bucket_name}
-        :param name: The name of the channel being managed. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#name PackerChannel#name}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#id PackerChannel#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param iteration: iteration block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#iteration PackerChannel#iteration}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#timeouts PackerChannel#timeouts}
+        :param bucket_name: The slug of the HCP Packer Registry image bucket where the channel should be created in. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#bucket_name PackerChannel#bucket_name}
+        :param name: The name of the channel being managed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#name PackerChannel#name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#id PackerChannel#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param iteration: iteration block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#iteration PackerChannel#iteration}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#timeouts PackerChannel#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(iteration, dict):
             iteration = PackerChannelIteration(**iteration)
         if isinstance(timeouts, dict):
             timeouts = PackerChannelTimeouts(**timeouts)
@@ -345,20 +345,22 @@
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
@@ -400,54 +402,54 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def bucket_name(self) -> builtins.str:
         '''The slug of the HCP Packer Registry image bucket where the channel should be created in.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#bucket_name PackerChannel#bucket_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#bucket_name PackerChannel#bucket_name}
         '''
         result = self._values.get("bucket_name")
         assert result is not None, "Required property 'bucket_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the channel being managed.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#name PackerChannel#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#name PackerChannel#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#id PackerChannel#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#id PackerChannel#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def iteration(self) -> typing.Optional["PackerChannelIteration"]:
         '''iteration block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#iteration PackerChannel#iteration}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#iteration PackerChannel#iteration}
         '''
         result = self._values.get("iteration")
         return typing.cast(typing.Optional["PackerChannelIteration"], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["PackerChannelTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#timeouts PackerChannel#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#timeouts PackerChannel#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["PackerChannelTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -474,17 +476,17 @@
         self,
         *,
         fingerprint: typing.Optional[builtins.str] = None,
         id: typing.Optional[builtins.str] = None,
         incremental_version: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
-        :param fingerprint: The fingerprint of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#fingerprint PackerChannel#fingerprint}
-        :param id: The ID of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#id PackerChannel#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param incremental_version: The incremental_version of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#incremental_version PackerChannel#incremental_version}
+        :param fingerprint: The fingerprint of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#fingerprint PackerChannel#fingerprint}
+        :param id: The ID of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#id PackerChannel#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param incremental_version: The incremental_version of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#incremental_version PackerChannel#incremental_version}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ab35d949073c20a9975f8d59dbcea56f6019586d8d17c87198ed9b73d8da416c)
             check_type(argname="argument fingerprint", value=fingerprint, expected_type=type_hints["fingerprint"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument incremental_version", value=incremental_version, expected_type=type_hints["incremental_version"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -495,36 +497,36 @@
         if incremental_version is not None:
             self._values["incremental_version"] = incremental_version
 
     @builtins.property
     def fingerprint(self) -> typing.Optional[builtins.str]:
         '''The fingerprint of the iteration assigned to the channel.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#fingerprint PackerChannel#fingerprint}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#fingerprint PackerChannel#fingerprint}
         '''
         result = self._values.get("fingerprint")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
         '''The ID of the iteration assigned to the channel.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#id PackerChannel#id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#id PackerChannel#id}
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def incremental_version(self) -> typing.Optional[jsii.Number]:
         '''The incremental_version of the iteration assigned to the channel.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#incremental_version PackerChannel#incremental_version}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#incremental_version PackerChannel#incremental_version}
         '''
         result = self._values.get("incremental_version")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -649,18 +651,18 @@
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#create PackerChannel#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#default PackerChannel#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#delete PackerChannel#delete}.
-        :param update: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#update PackerChannel#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#create PackerChannel#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#default PackerChannel#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#delete PackerChannel#delete}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#update PackerChannel#update}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__fe787a15b951abd7c6a540834a0577806e60d41fed9c893cef64fa1dabed3638)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
             check_type(argname="argument update", value=update, expected_type=type_hints["update"])
@@ -672,33 +674,33 @@
         if delete is not None:
             self._values["delete"] = delete
         if update is not None:
             self._values["update"] = update
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#create PackerChannel#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#create PackerChannel#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#default PackerChannel#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#default PackerChannel#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#delete PackerChannel#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#delete PackerChannel#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def update(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/packer_channel#update PackerChannel#update}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/packer_channel#update PackerChannel#update}.'''
         result = self._values.get("update")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -849,15 +851,15 @@
     *,
     bucket_name: builtins.str,
     name: builtins.str,
     id: typing.Optional[builtins.str] = None,
     iteration: typing.Optional[typing.Union[PackerChannelIteration, typing.Dict[builtins.str, typing.Any]]] = None,
     timeouts: typing.Optional[typing.Union[PackerChannelTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -880,15 +882,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__d477df52b7c60b14dc1bee079bed7a6b984f2086c59e5444cea18401d935f420(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     bucket_name: builtins.str,
     name: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/provider/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/provider/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`hcp`](https://www.terraform.io/docs/providers/hcp).
+Refer to the Terraform Registory for docs: [`hcp`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,32 +22,32 @@
 
 
 class HcpProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.provider.HcpProvider",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp hcp}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs hcp}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias: typing.Optional[builtins.str] = None,
         client_id: typing.Optional[builtins.str] = None,
         client_secret: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp hcp} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs hcp} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp#alias HcpProvider#alias}
-        :param client_id: The OAuth2 Client ID for API operations. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp#client_id HcpProvider#client_id}
-        :param client_secret: The OAuth2 Client Secret for API operations. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp#client_secret HcpProvider#client_secret}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs#alias HcpProvider#alias}
+        :param client_id: The OAuth2 Client ID for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs#client_id HcpProvider#client_id}
+        :param client_secret: The OAuth2 Client Secret for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs#client_secret HcpProvider#client_secret}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9962aa89ee76b9284f3c61b4b164aa99145fa8bddda7ed708d531d776d163687)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = HcpProviderConfig(
             alias=alias, client_id=client_id, client_secret=client_secret
@@ -142,17 +142,17 @@
         self,
         *,
         alias: typing.Optional[builtins.str] = None,
         client_id: typing.Optional[builtins.str] = None,
         client_secret: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp#alias HcpProvider#alias}
-        :param client_id: The OAuth2 Client ID for API operations. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp#client_id HcpProvider#client_id}
-        :param client_secret: The OAuth2 Client Secret for API operations. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp#client_secret HcpProvider#client_secret}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs#alias HcpProvider#alias}
+        :param client_id: The OAuth2 Client ID for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs#client_id HcpProvider#client_id}
+        :param client_secret: The OAuth2 Client Secret for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs#client_secret HcpProvider#client_secret}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8d6d52a2ef8cb5413ad5a8ca3a6605f03df54b36c17588f9157418d93854016b)
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
             check_type(argname="argument client_id", value=client_id, expected_type=type_hints["client_id"])
             check_type(argname="argument client_secret", value=client_secret, expected_type=type_hints["client_secret"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -163,33 +163,33 @@
         if client_secret is not None:
             self._values["client_secret"] = client_secret
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp#alias HcpProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs#alias HcpProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def client_id(self) -> typing.Optional[builtins.str]:
         '''The OAuth2 Client ID for API operations.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp#client_id HcpProvider#client_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs#client_id HcpProvider#client_id}
         '''
         result = self._values.get("client_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def client_secret(self) -> typing.Optional[builtins.str]:
         '''The OAuth2 Client Secret for API operations.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp#client_secret HcpProvider#client_secret}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs#client_secret HcpProvider#client_secret}
         '''
         result = self._values.get("client_secret")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp/vault_cluster/__init__.py` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp/vault_cluster/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_vault_cluster`
 
-Refer to the Terraform Registory for docs: [`hcp_vault_cluster`](https://www.terraform.io/docs/providers/hcp/r/vault_cluster).
+Refer to the Terraform Registory for docs: [`hcp_vault_cluster`](https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class VaultCluster(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.vaultCluster.VaultCluster",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster hcp_vault_cluster}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster hcp_vault_cluster}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_id: builtins.str,
@@ -42,37 +42,37 @@
         min_vault_version: typing.Optional[builtins.str] = None,
         paths_filter: typing.Optional[typing.Sequence[builtins.str]] = None,
         primary_link: typing.Optional[builtins.str] = None,
         public_endpoint: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         tier: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["VaultClusterTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster hcp_vault_cluster} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster hcp_vault_cluster} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#cluster_id VaultCluster#cluster_id}
-        :param hvn_id: The ID of the HVN this HCP Vault cluster is associated to. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#hvn_id VaultCluster#hvn_id}
-        :param audit_log_config: audit_log_config block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#audit_log_config VaultCluster#audit_log_config}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#id VaultCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param major_version_upgrade_config: major_version_upgrade_config block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#major_version_upgrade_config VaultCluster#major_version_upgrade_config}
-        :param metrics_config: metrics_config block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#metrics_config VaultCluster#metrics_config}
-        :param min_vault_version: The minimum Vault version to use when creating the cluster. If not specified, it is defaulted to the version that is currently recommended by HCP. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#min_vault_version VaultCluster#min_vault_version}
-        :param paths_filter: The performance replication `paths filter <https://developer.hashicorp.com/vault/tutorials/cloud-ops/vault-replication-terraform>`_. Applies to performance replication secondaries only and operates in "deny" mode only. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#paths_filter VaultCluster#paths_filter}
-        :param primary_link: The ``self_link`` of the HCP Vault Plus tier cluster which is the primary in the performance replication setup with this HCP Vault Plus tier cluster. If not specified, it is a standalone Plus tier HCP Vault cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#primary_link VaultCluster#primary_link}
-        :param public_endpoint: Denotes that the cluster has a public endpoint. Defaults to false. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#public_endpoint VaultCluster#public_endpoint}
-        :param tier: Tier of the HCP Vault cluster. Valid options for tiers - ``dev``, ``starter_small``, ``standard_small``, ``standard_medium``, ``standard_large``, ``plus_small``, ``plus_medium``, ``plus_large``. See `pricing information <https://www.hashicorp.com/products/vault/pricing>`_. Changing a cluster's size or tier is only available to admins. See `Scale a cluster <https://registry.terraform.io/providers/hashicorp/hcp/latest/docs/guides/vault-scaling>`_. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#tier VaultCluster#tier}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#timeouts VaultCluster#timeouts}
+        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#cluster_id VaultCluster#cluster_id}
+        :param hvn_id: The ID of the HVN this HCP Vault cluster is associated to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#hvn_id VaultCluster#hvn_id}
+        :param audit_log_config: audit_log_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#audit_log_config VaultCluster#audit_log_config}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#id VaultCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param major_version_upgrade_config: major_version_upgrade_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#major_version_upgrade_config VaultCluster#major_version_upgrade_config}
+        :param metrics_config: metrics_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#metrics_config VaultCluster#metrics_config}
+        :param min_vault_version: The minimum Vault version to use when creating the cluster. If not specified, it is defaulted to the version that is currently recommended by HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#min_vault_version VaultCluster#min_vault_version}
+        :param paths_filter: The performance replication `paths filter <https://developer.hashicorp.com/vault/tutorials/cloud-ops/vault-replication-terraform>`_. Applies to performance replication secondaries only and operates in "deny" mode only. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#paths_filter VaultCluster#paths_filter}
+        :param primary_link: The ``self_link`` of the HCP Vault Plus tier cluster which is the primary in the performance replication setup with this HCP Vault Plus tier cluster. If not specified, it is a standalone Plus tier HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#primary_link VaultCluster#primary_link}
+        :param public_endpoint: Denotes that the cluster has a public endpoint. Defaults to false. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#public_endpoint VaultCluster#public_endpoint}
+        :param tier: Tier of the HCP Vault cluster. Valid options for tiers - ``dev``, ``starter_small``, ``standard_small``, ``standard_medium``, ``standard_large``, ``plus_small``, ``plus_medium``, ``plus_large``. See `pricing information <https://www.hashicorp.com/products/vault/pricing>`_. Changing a cluster's size or tier is only available to admins. See `Scale a cluster <https://registry.terraform.io/providers/hashicorp/hcp/latest/docs/guides/vault-scaling>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#tier VaultCluster#tier}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#timeouts VaultCluster#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -114,21 +114,21 @@
         grafana_endpoint: typing.Optional[builtins.str] = None,
         grafana_password: typing.Optional[builtins.str] = None,
         grafana_user: typing.Optional[builtins.str] = None,
         splunk_hecendpoint: typing.Optional[builtins.str] = None,
         splunk_token: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param datadog_api_key: Datadog api key for streaming audit logs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
-        :param datadog_region: Datadog region for streaming audit logs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#datadog_region VaultCluster#datadog_region}
-        :param grafana_endpoint: Grafana endpoint for streaming audit logs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
-        :param grafana_password: Grafana password for streaming audit logs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#grafana_password VaultCluster#grafana_password}
-        :param grafana_user: Grafana user for streaming audit logs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#grafana_user VaultCluster#grafana_user}
-        :param splunk_hecendpoint: Splunk endpoint for streaming audit logs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
-        :param splunk_token: Splunk token for streaming audit logs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#splunk_token VaultCluster#splunk_token}
+        :param datadog_api_key: Datadog api key for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
+        :param datadog_region: Datadog region for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#datadog_region VaultCluster#datadog_region}
+        :param grafana_endpoint: Grafana endpoint for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
+        :param grafana_password: Grafana password for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#grafana_password VaultCluster#grafana_password}
+        :param grafana_user: Grafana user for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#grafana_user VaultCluster#grafana_user}
+        :param splunk_hecendpoint: Splunk endpoint for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
+        :param splunk_token: Splunk token for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#splunk_token VaultCluster#splunk_token}
         '''
         value = VaultClusterAuditLogConfig(
             datadog_api_key=datadog_api_key,
             datadog_region=datadog_region,
             grafana_endpoint=grafana_endpoint,
             grafana_password=grafana_password,
             grafana_user=grafana_user,
@@ -143,17 +143,17 @@
         self,
         *,
         upgrade_type: builtins.str,
         maintenance_window_day: typing.Optional[builtins.str] = None,
         maintenance_window_time: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param upgrade_type: The major upgrade type for the cluster. Valid options for upgrade type - ``AUTOMATIC``, ``SCHEDULED``, ``MANUAL``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#upgrade_type VaultCluster#upgrade_type}
-        :param maintenance_window_day: The maintenance day of the week for scheduled upgrades. Valid options for maintenance window day - ``MONDAY``, ``TUESDAY``, ``WEDNESDAY``, ``THURSDAY``, ``FRIDAY``, ``SATURDAY``, ``SUNDAY`` Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#maintenance_window_day VaultCluster#maintenance_window_day}
-        :param maintenance_window_time: The maintenance time frame for scheduled upgrades. Valid options for maintenance window time - ``WINDOW_12AM_4AM``, ``WINDOW_6AM_10AM``, ``WINDOW_12PM_4PM``, ``WINDOW_6PM_10PM``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#maintenance_window_time VaultCluster#maintenance_window_time}
+        :param upgrade_type: The major upgrade type for the cluster. Valid options for upgrade type - ``AUTOMATIC``, ``SCHEDULED``, ``MANUAL``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#upgrade_type VaultCluster#upgrade_type}
+        :param maintenance_window_day: The maintenance day of the week for scheduled upgrades. Valid options for maintenance window day - ``MONDAY``, ``TUESDAY``, ``WEDNESDAY``, ``THURSDAY``, ``FRIDAY``, ``SATURDAY``, ``SUNDAY`` Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#maintenance_window_day VaultCluster#maintenance_window_day}
+        :param maintenance_window_time: The maintenance time frame for scheduled upgrades. Valid options for maintenance window time - ``WINDOW_12AM_4AM``, ``WINDOW_6AM_10AM``, ``WINDOW_12PM_4PM``, ``WINDOW_6PM_10PM``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#maintenance_window_time VaultCluster#maintenance_window_time}
         '''
         value = VaultClusterMajorVersionUpgradeConfig(
             upgrade_type=upgrade_type,
             maintenance_window_day=maintenance_window_day,
             maintenance_window_time=maintenance_window_time,
         )
 
@@ -168,21 +168,21 @@
         grafana_endpoint: typing.Optional[builtins.str] = None,
         grafana_password: typing.Optional[builtins.str] = None,
         grafana_user: typing.Optional[builtins.str] = None,
         splunk_hecendpoint: typing.Optional[builtins.str] = None,
         splunk_token: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param datadog_api_key: Datadog api key for streaming metrics. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
-        :param datadog_region: Datadog region for streaming metrics. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#datadog_region VaultCluster#datadog_region}
-        :param grafana_endpoint: Grafana endpoint for streaming metrics. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
-        :param grafana_password: Grafana password for streaming metrics. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#grafana_password VaultCluster#grafana_password}
-        :param grafana_user: Grafana user for streaming metrics. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#grafana_user VaultCluster#grafana_user}
-        :param splunk_hecendpoint: Splunk endpoint for streaming metrics. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
-        :param splunk_token: Splunk token for streaming metrics. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#splunk_token VaultCluster#splunk_token}
+        :param datadog_api_key: Datadog api key for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
+        :param datadog_region: Datadog region for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#datadog_region VaultCluster#datadog_region}
+        :param grafana_endpoint: Grafana endpoint for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
+        :param grafana_password: Grafana password for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#grafana_password VaultCluster#grafana_password}
+        :param grafana_user: Grafana user for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#grafana_user VaultCluster#grafana_user}
+        :param splunk_hecendpoint: Splunk endpoint for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
+        :param splunk_token: Splunk token for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#splunk_token VaultCluster#splunk_token}
         '''
         value = VaultClusterMetricsConfig(
             datadog_api_key=datadog_api_key,
             datadog_region=datadog_region,
             grafana_endpoint=grafana_endpoint,
             grafana_password=grafana_password,
             grafana_user=grafana_user,
@@ -198,18 +198,18 @@
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#create VaultCluster#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#default VaultCluster#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#delete VaultCluster#delete}.
-        :param update: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#update VaultCluster#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#create VaultCluster#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#default VaultCluster#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#delete VaultCluster#delete}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#update VaultCluster#update}.
         '''
         value = VaultClusterTimeouts(
             create=create, default=default, delete=delete, update=update
         )
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
@@ -529,21 +529,21 @@
         grafana_endpoint: typing.Optional[builtins.str] = None,
         grafana_password: typing.Optional[builtins.str] = None,
         grafana_user: typing.Optional[builtins.str] = None,
         splunk_hecendpoint: typing.Optional[builtins.str] = None,
         splunk_token: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param datadog_api_key: Datadog api key for streaming audit logs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
-        :param datadog_region: Datadog region for streaming audit logs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#datadog_region VaultCluster#datadog_region}
-        :param grafana_endpoint: Grafana endpoint for streaming audit logs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
-        :param grafana_password: Grafana password for streaming audit logs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#grafana_password VaultCluster#grafana_password}
-        :param grafana_user: Grafana user for streaming audit logs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#grafana_user VaultCluster#grafana_user}
-        :param splunk_hecendpoint: Splunk endpoint for streaming audit logs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
-        :param splunk_token: Splunk token for streaming audit logs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#splunk_token VaultCluster#splunk_token}
+        :param datadog_api_key: Datadog api key for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
+        :param datadog_region: Datadog region for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#datadog_region VaultCluster#datadog_region}
+        :param grafana_endpoint: Grafana endpoint for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
+        :param grafana_password: Grafana password for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#grafana_password VaultCluster#grafana_password}
+        :param grafana_user: Grafana user for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#grafana_user VaultCluster#grafana_user}
+        :param splunk_hecendpoint: Splunk endpoint for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
+        :param splunk_token: Splunk token for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#splunk_token VaultCluster#splunk_token}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__945e965e9dab450573c42b8a5cc975ed8d0713bf41d459bead13f88051d0a34e)
             check_type(argname="argument datadog_api_key", value=datadog_api_key, expected_type=type_hints["datadog_api_key"])
             check_type(argname="argument datadog_region", value=datadog_region, expected_type=type_hints["datadog_region"])
             check_type(argname="argument grafana_endpoint", value=grafana_endpoint, expected_type=type_hints["grafana_endpoint"])
             check_type(argname="argument grafana_password", value=grafana_password, expected_type=type_hints["grafana_password"])
@@ -566,69 +566,69 @@
         if splunk_token is not None:
             self._values["splunk_token"] = splunk_token
 
     @builtins.property
     def datadog_api_key(self) -> typing.Optional[builtins.str]:
         '''Datadog api key for streaming audit logs.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
         '''
         result = self._values.get("datadog_api_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def datadog_region(self) -> typing.Optional[builtins.str]:
         '''Datadog region for streaming audit logs.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#datadog_region VaultCluster#datadog_region}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#datadog_region VaultCluster#datadog_region}
         '''
         result = self._values.get("datadog_region")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def grafana_endpoint(self) -> typing.Optional[builtins.str]:
         '''Grafana endpoint for streaming audit logs.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
         '''
         result = self._values.get("grafana_endpoint")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def grafana_password(self) -> typing.Optional[builtins.str]:
         '''Grafana password for streaming audit logs.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#grafana_password VaultCluster#grafana_password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#grafana_password VaultCluster#grafana_password}
         '''
         result = self._values.get("grafana_password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def grafana_user(self) -> typing.Optional[builtins.str]:
         '''Grafana user for streaming audit logs.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#grafana_user VaultCluster#grafana_user}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#grafana_user VaultCluster#grafana_user}
         '''
         result = self._values.get("grafana_user")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def splunk_hecendpoint(self) -> typing.Optional[builtins.str]:
         '''Splunk endpoint for streaming audit logs.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
         '''
         result = self._values.get("splunk_hecendpoint")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def splunk_token(self) -> typing.Optional[builtins.str]:
         '''Splunk token for streaming audit logs.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#splunk_token VaultCluster#splunk_token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#splunk_token VaultCluster#splunk_token}
         '''
         result = self._values.get("splunk_token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -850,15 +850,15 @@
     },
 )
 class VaultClusterConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         cluster_id: builtins.str,
         hvn_id: builtins.str,
@@ -877,26 +877,26 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#cluster_id VaultCluster#cluster_id}
-        :param hvn_id: The ID of the HVN this HCP Vault cluster is associated to. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#hvn_id VaultCluster#hvn_id}
-        :param audit_log_config: audit_log_config block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#audit_log_config VaultCluster#audit_log_config}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#id VaultCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param major_version_upgrade_config: major_version_upgrade_config block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#major_version_upgrade_config VaultCluster#major_version_upgrade_config}
-        :param metrics_config: metrics_config block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#metrics_config VaultCluster#metrics_config}
-        :param min_vault_version: The minimum Vault version to use when creating the cluster. If not specified, it is defaulted to the version that is currently recommended by HCP. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#min_vault_version VaultCluster#min_vault_version}
-        :param paths_filter: The performance replication `paths filter <https://developer.hashicorp.com/vault/tutorials/cloud-ops/vault-replication-terraform>`_. Applies to performance replication secondaries only and operates in "deny" mode only. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#paths_filter VaultCluster#paths_filter}
-        :param primary_link: The ``self_link`` of the HCP Vault Plus tier cluster which is the primary in the performance replication setup with this HCP Vault Plus tier cluster. If not specified, it is a standalone Plus tier HCP Vault cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#primary_link VaultCluster#primary_link}
-        :param public_endpoint: Denotes that the cluster has a public endpoint. Defaults to false. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#public_endpoint VaultCluster#public_endpoint}
-        :param tier: Tier of the HCP Vault cluster. Valid options for tiers - ``dev``, ``starter_small``, ``standard_small``, ``standard_medium``, ``standard_large``, ``plus_small``, ``plus_medium``, ``plus_large``. See `pricing information <https://www.hashicorp.com/products/vault/pricing>`_. Changing a cluster's size or tier is only available to admins. See `Scale a cluster <https://registry.terraform.io/providers/hashicorp/hcp/latest/docs/guides/vault-scaling>`_. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#tier VaultCluster#tier}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#timeouts VaultCluster#timeouts}
+        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#cluster_id VaultCluster#cluster_id}
+        :param hvn_id: The ID of the HVN this HCP Vault cluster is associated to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#hvn_id VaultCluster#hvn_id}
+        :param audit_log_config: audit_log_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#audit_log_config VaultCluster#audit_log_config}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#id VaultCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param major_version_upgrade_config: major_version_upgrade_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#major_version_upgrade_config VaultCluster#major_version_upgrade_config}
+        :param metrics_config: metrics_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#metrics_config VaultCluster#metrics_config}
+        :param min_vault_version: The minimum Vault version to use when creating the cluster. If not specified, it is defaulted to the version that is currently recommended by HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#min_vault_version VaultCluster#min_vault_version}
+        :param paths_filter: The performance replication `paths filter <https://developer.hashicorp.com/vault/tutorials/cloud-ops/vault-replication-terraform>`_. Applies to performance replication secondaries only and operates in "deny" mode only. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#paths_filter VaultCluster#paths_filter}
+        :param primary_link: The ``self_link`` of the HCP Vault Plus tier cluster which is the primary in the performance replication setup with this HCP Vault Plus tier cluster. If not specified, it is a standalone Plus tier HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#primary_link VaultCluster#primary_link}
+        :param public_endpoint: Denotes that the cluster has a public endpoint. Defaults to false. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#public_endpoint VaultCluster#public_endpoint}
+        :param tier: Tier of the HCP Vault cluster. Valid options for tiers - ``dev``, ``starter_small``, ``standard_small``, ``standard_medium``, ``standard_large``, ``plus_small``, ``plus_medium``, ``plus_large``. See `pricing information <https://www.hashicorp.com/products/vault/pricing>`_. Changing a cluster's size or tier is only available to admins. See `Scale a cluster <https://registry.terraform.io/providers/hashicorp/hcp/latest/docs/guides/vault-scaling>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#tier VaultCluster#tier}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#timeouts VaultCluster#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(audit_log_config, dict):
             audit_log_config = VaultClusterAuditLogConfig(**audit_log_config)
         if isinstance(major_version_upgrade_config, dict):
             major_version_upgrade_config = VaultClusterMajorVersionUpgradeConfig(**major_version_upgrade_config)
@@ -971,20 +971,22 @@
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
@@ -1026,127 +1028,127 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cluster_id(self) -> builtins.str:
         '''The ID of the HCP Vault cluster.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#cluster_id VaultCluster#cluster_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#cluster_id VaultCluster#cluster_id}
         '''
         result = self._values.get("cluster_id")
         assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def hvn_id(self) -> builtins.str:
         '''The ID of the HVN this HCP Vault cluster is associated to.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#hvn_id VaultCluster#hvn_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#hvn_id VaultCluster#hvn_id}
         '''
         result = self._values.get("hvn_id")
         assert result is not None, "Required property 'hvn_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def audit_log_config(self) -> typing.Optional[VaultClusterAuditLogConfig]:
         '''audit_log_config block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#audit_log_config VaultCluster#audit_log_config}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#audit_log_config VaultCluster#audit_log_config}
         '''
         result = self._values.get("audit_log_config")
         return typing.cast(typing.Optional[VaultClusterAuditLogConfig], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#id VaultCluster#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#id VaultCluster#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def major_version_upgrade_config(
         self,
     ) -> typing.Optional["VaultClusterMajorVersionUpgradeConfig"]:
         '''major_version_upgrade_config block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#major_version_upgrade_config VaultCluster#major_version_upgrade_config}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#major_version_upgrade_config VaultCluster#major_version_upgrade_config}
         '''
         result = self._values.get("major_version_upgrade_config")
         return typing.cast(typing.Optional["VaultClusterMajorVersionUpgradeConfig"], result)
 
     @builtins.property
     def metrics_config(self) -> typing.Optional["VaultClusterMetricsConfig"]:
         '''metrics_config block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#metrics_config VaultCluster#metrics_config}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#metrics_config VaultCluster#metrics_config}
         '''
         result = self._values.get("metrics_config")
         return typing.cast(typing.Optional["VaultClusterMetricsConfig"], result)
 
     @builtins.property
     def min_vault_version(self) -> typing.Optional[builtins.str]:
         '''The minimum Vault version to use when creating the cluster.
 
         If not specified, it is defaulted to the version that is currently recommended by HCP.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#min_vault_version VaultCluster#min_vault_version}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#min_vault_version VaultCluster#min_vault_version}
         '''
         result = self._values.get("min_vault_version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def paths_filter(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The performance replication `paths filter <https://developer.hashicorp.com/vault/tutorials/cloud-ops/vault-replication-terraform>`_. Applies to performance replication secondaries only and operates in "deny" mode only.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#paths_filter VaultCluster#paths_filter}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#paths_filter VaultCluster#paths_filter}
         '''
         result = self._values.get("paths_filter")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def primary_link(self) -> typing.Optional[builtins.str]:
         '''The ``self_link`` of the HCP Vault Plus tier cluster which is the primary in the performance replication setup with this HCP Vault Plus tier cluster.
 
         If not specified, it is a standalone Plus tier HCP Vault cluster.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#primary_link VaultCluster#primary_link}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#primary_link VaultCluster#primary_link}
         '''
         result = self._values.get("primary_link")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def public_endpoint(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Denotes that the cluster has a public endpoint. Defaults to false.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#public_endpoint VaultCluster#public_endpoint}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#public_endpoint VaultCluster#public_endpoint}
         '''
         result = self._values.get("public_endpoint")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def tier(self) -> typing.Optional[builtins.str]:
         '''Tier of the HCP Vault cluster.
 
         Valid options for tiers - ``dev``, ``starter_small``, ``standard_small``, ``standard_medium``, ``standard_large``, ``plus_small``, ``plus_medium``, ``plus_large``. See `pricing information <https://www.hashicorp.com/products/vault/pricing>`_. Changing a cluster's size or tier is only available to admins. See `Scale a cluster <https://registry.terraform.io/providers/hashicorp/hcp/latest/docs/guides/vault-scaling>`_.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#tier VaultCluster#tier}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#tier VaultCluster#tier}
         '''
         result = self._values.get("tier")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["VaultClusterTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#timeouts VaultCluster#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#timeouts VaultCluster#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["VaultClusterTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1173,17 +1175,17 @@
         self,
         *,
         upgrade_type: builtins.str,
         maintenance_window_day: typing.Optional[builtins.str] = None,
         maintenance_window_time: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param upgrade_type: The major upgrade type for the cluster. Valid options for upgrade type - ``AUTOMATIC``, ``SCHEDULED``, ``MANUAL``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#upgrade_type VaultCluster#upgrade_type}
-        :param maintenance_window_day: The maintenance day of the week for scheduled upgrades. Valid options for maintenance window day - ``MONDAY``, ``TUESDAY``, ``WEDNESDAY``, ``THURSDAY``, ``FRIDAY``, ``SATURDAY``, ``SUNDAY`` Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#maintenance_window_day VaultCluster#maintenance_window_day}
-        :param maintenance_window_time: The maintenance time frame for scheduled upgrades. Valid options for maintenance window time - ``WINDOW_12AM_4AM``, ``WINDOW_6AM_10AM``, ``WINDOW_12PM_4PM``, ``WINDOW_6PM_10PM``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#maintenance_window_time VaultCluster#maintenance_window_time}
+        :param upgrade_type: The major upgrade type for the cluster. Valid options for upgrade type - ``AUTOMATIC``, ``SCHEDULED``, ``MANUAL``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#upgrade_type VaultCluster#upgrade_type}
+        :param maintenance_window_day: The maintenance day of the week for scheduled upgrades. Valid options for maintenance window day - ``MONDAY``, ``TUESDAY``, ``WEDNESDAY``, ``THURSDAY``, ``FRIDAY``, ``SATURDAY``, ``SUNDAY`` Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#maintenance_window_day VaultCluster#maintenance_window_day}
+        :param maintenance_window_time: The maintenance time frame for scheduled upgrades. Valid options for maintenance window time - ``WINDOW_12AM_4AM``, ``WINDOW_6AM_10AM``, ``WINDOW_12PM_4PM``, ``WINDOW_6PM_10PM``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#maintenance_window_time VaultCluster#maintenance_window_time}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f4962f49b844cabab740d8df01f3b70a715d3f1306b60fec54b6272426400d44)
             check_type(argname="argument upgrade_type", value=upgrade_type, expected_type=type_hints["upgrade_type"])
             check_type(argname="argument maintenance_window_day", value=maintenance_window_day, expected_type=type_hints["maintenance_window_day"])
             check_type(argname="argument maintenance_window_time", value=maintenance_window_time, expected_type=type_hints["maintenance_window_time"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -1194,36 +1196,36 @@
         if maintenance_window_time is not None:
             self._values["maintenance_window_time"] = maintenance_window_time
 
     @builtins.property
     def upgrade_type(self) -> builtins.str:
         '''The major upgrade type for the cluster. Valid options for upgrade type - ``AUTOMATIC``, ``SCHEDULED``, ``MANUAL``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#upgrade_type VaultCluster#upgrade_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#upgrade_type VaultCluster#upgrade_type}
         '''
         result = self._values.get("upgrade_type")
         assert result is not None, "Required property 'upgrade_type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def maintenance_window_day(self) -> typing.Optional[builtins.str]:
         '''The maintenance day of the week for scheduled upgrades.
 
         Valid options for maintenance window day - ``MONDAY``, ``TUESDAY``, ``WEDNESDAY``, ``THURSDAY``, ``FRIDAY``, ``SATURDAY``, ``SUNDAY``
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#maintenance_window_day VaultCluster#maintenance_window_day}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#maintenance_window_day VaultCluster#maintenance_window_day}
         '''
         result = self._values.get("maintenance_window_day")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def maintenance_window_time(self) -> typing.Optional[builtins.str]:
         '''The maintenance time frame for scheduled upgrades. Valid options for maintenance window time - ``WINDOW_12AM_4AM``, ``WINDOW_6AM_10AM``, ``WINDOW_12PM_4PM``, ``WINDOW_6PM_10PM``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#maintenance_window_time VaultCluster#maintenance_window_time}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#maintenance_window_time VaultCluster#maintenance_window_time}
         '''
         result = self._values.get("maintenance_window_time")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1353,21 +1355,21 @@
         grafana_endpoint: typing.Optional[builtins.str] = None,
         grafana_password: typing.Optional[builtins.str] = None,
         grafana_user: typing.Optional[builtins.str] = None,
         splunk_hecendpoint: typing.Optional[builtins.str] = None,
         splunk_token: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param datadog_api_key: Datadog api key for streaming metrics. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
-        :param datadog_region: Datadog region for streaming metrics. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#datadog_region VaultCluster#datadog_region}
-        :param grafana_endpoint: Grafana endpoint for streaming metrics. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
-        :param grafana_password: Grafana password for streaming metrics. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#grafana_password VaultCluster#grafana_password}
-        :param grafana_user: Grafana user for streaming metrics. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#grafana_user VaultCluster#grafana_user}
-        :param splunk_hecendpoint: Splunk endpoint for streaming metrics. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
-        :param splunk_token: Splunk token for streaming metrics. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#splunk_token VaultCluster#splunk_token}
+        :param datadog_api_key: Datadog api key for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
+        :param datadog_region: Datadog region for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#datadog_region VaultCluster#datadog_region}
+        :param grafana_endpoint: Grafana endpoint for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
+        :param grafana_password: Grafana password for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#grafana_password VaultCluster#grafana_password}
+        :param grafana_user: Grafana user for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#grafana_user VaultCluster#grafana_user}
+        :param splunk_hecendpoint: Splunk endpoint for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
+        :param splunk_token: Splunk token for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#splunk_token VaultCluster#splunk_token}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e41328d9c30b2160db3534c4e47502c0f13855650febdfb88b239dcb6d6ee814)
             check_type(argname="argument datadog_api_key", value=datadog_api_key, expected_type=type_hints["datadog_api_key"])
             check_type(argname="argument datadog_region", value=datadog_region, expected_type=type_hints["datadog_region"])
             check_type(argname="argument grafana_endpoint", value=grafana_endpoint, expected_type=type_hints["grafana_endpoint"])
             check_type(argname="argument grafana_password", value=grafana_password, expected_type=type_hints["grafana_password"])
@@ -1390,69 +1392,69 @@
         if splunk_token is not None:
             self._values["splunk_token"] = splunk_token
 
     @builtins.property
     def datadog_api_key(self) -> typing.Optional[builtins.str]:
         '''Datadog api key for streaming metrics.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
         '''
         result = self._values.get("datadog_api_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def datadog_region(self) -> typing.Optional[builtins.str]:
         '''Datadog region for streaming metrics.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#datadog_region VaultCluster#datadog_region}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#datadog_region VaultCluster#datadog_region}
         '''
         result = self._values.get("datadog_region")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def grafana_endpoint(self) -> typing.Optional[builtins.str]:
         '''Grafana endpoint for streaming metrics.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
         '''
         result = self._values.get("grafana_endpoint")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def grafana_password(self) -> typing.Optional[builtins.str]:
         '''Grafana password for streaming metrics.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#grafana_password VaultCluster#grafana_password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#grafana_password VaultCluster#grafana_password}
         '''
         result = self._values.get("grafana_password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def grafana_user(self) -> typing.Optional[builtins.str]:
         '''Grafana user for streaming metrics.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#grafana_user VaultCluster#grafana_user}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#grafana_user VaultCluster#grafana_user}
         '''
         result = self._values.get("grafana_user")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def splunk_hecendpoint(self) -> typing.Optional[builtins.str]:
         '''Splunk endpoint for streaming metrics.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
         '''
         result = self._values.get("splunk_hecendpoint")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def splunk_token(self) -> typing.Optional[builtins.str]:
         '''Splunk token for streaming metrics.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#splunk_token VaultCluster#splunk_token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#splunk_token VaultCluster#splunk_token}
         '''
         result = self._values.get("splunk_token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1661,18 +1663,18 @@
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#create VaultCluster#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#default VaultCluster#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#delete VaultCluster#delete}.
-        :param update: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#update VaultCluster#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#create VaultCluster#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#default VaultCluster#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#delete VaultCluster#delete}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#update VaultCluster#update}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__85ee5e56e863fb68b056cf0c52c11694127fd2447b2109705c1c013124bc122b)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
             check_type(argname="argument update", value=update, expected_type=type_hints["update"])
@@ -1684,33 +1686,33 @@
         if delete is not None:
             self._values["delete"] = delete
         if update is not None:
             self._values["update"] = update
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#create VaultCluster#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#create VaultCluster#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#default VaultCluster#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#default VaultCluster#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#delete VaultCluster#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#delete VaultCluster#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def update(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcp/r/vault_cluster#update VaultCluster#update}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.56.0/docs/resources/vault_cluster#update VaultCluster#update}.'''
         result = self._values.get("update")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -1872,15 +1874,15 @@
     min_vault_version: typing.Optional[builtins.str] = None,
     paths_filter: typing.Optional[typing.Sequence[builtins.str]] = None,
     primary_link: typing.Optional[builtins.str] = None,
     public_endpoint: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     tier: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[VaultClusterTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -2001,15 +2003,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__f8a47be8c3817c70555bc777416f18db7e158d5f4a408d5a70bef49dc6666cf0(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     cluster_id: builtins.str,
     hvn_id: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp.egg-info/PKG-INFO` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-hcp
-Version: 3.0.3
+Version: 4.0.0
 Summary: Prebuilt hcp Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-hcp.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-hcp.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-hcp-3.0.3/src/cdktf_cdktf_provider_hcp.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-hcp-4.0.0/src/cdktf_cdktf_provider_hcp.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_hcp/py.typed
 src/cdktf_cdktf_provider_hcp.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_hcp.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_hcp.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_hcp.egg-info/requires.txt
 src/cdktf_cdktf_provider_hcp.egg-info/top_level.txt
 src/cdktf_cdktf_provider_hcp/_jsii/__init__.py
-src/cdktf_cdktf_provider_hcp/_jsii/provider-hcp@3.0.3.jsii.tgz
+src/cdktf_cdktf_provider_hcp/_jsii/provider-hcp@4.0.0.jsii.tgz
 src/cdktf_cdktf_provider_hcp/aws_network_peering/__init__.py
 src/cdktf_cdktf_provider_hcp/aws_transit_gateway_attachment/__init__.py
 src/cdktf_cdktf_provider_hcp/azure_peering_connection/__init__.py
 src/cdktf_cdktf_provider_hcp/boundary_cluster/__init__.py
 src/cdktf_cdktf_provider_hcp/consul_cluster/__init__.py
 src/cdktf_cdktf_provider_hcp/consul_cluster_root_token/__init__.py
 src/cdktf_cdktf_provider_hcp/consul_snapshot/__init__.py
```

