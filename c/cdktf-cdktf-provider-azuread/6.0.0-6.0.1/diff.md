# Comparing `tmp/cdktf-cdktf-provider-azuread-6.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-azuread-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-azuread-6.0.0.tar", last modified: Fri Apr 14 03:15:55 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-azuread-6.0.1.tar", last modified: Tue Apr 18 03:15:44 2023, max compression
```

## Comparing `cdktf-cdktf-provider-azuread-6.0.0.tar` & `cdktf-cdktf-provider-azuread-6.0.1.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.963014 cdktf-cdktf-provider-azuread-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-04-14 03:15:55.963014 cdktf-cdktf-provider-azuread-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 03:15:55.963014 cdktf-cdktf-provider-azuread-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.947014 cdktf-cdktf-provider-azuread-6.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.951014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/
--rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.951014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2454082 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/_jsii/provider-azuread@6.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.951014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package/
--rw-r--r--   0 runner    (1001) docker     (123)    38947 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.951014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package_assignment_policy/
--rw-r--r--   0 runner    (1001) docker     (123)   312905 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package_assignment_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)    41133 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package_catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package_resource_catalog_association/
--rw-r--r--   0 runner    (1001) docker     (123)    37366 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package_resource_catalog_association/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package_resource_package_association/
--rw-r--r--   0 runner    (1001) docker     (123)    37722 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package_resource_package_association/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit/
--rw-r--r--   0 runner    (1001) docker     (123)    44934 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit_member/
--rw-r--r--   0 runner    (1001) docker     (123)    36110 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit_role_member/
--rw-r--r--   0 runner    (1001) docker     (123)    38281 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit_role_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/app_role_assignment/
--rw-r--r--   0 runner    (1001) docker     (123)    35528 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/app_role_assignment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application/
--rw-r--r--   0 runner    (1001) docker     (123)   339995 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    51104 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_federated_identity_credential/
--rw-r--r--   0 runner    (1001) docker     (123)    47523 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_federated_identity_credential/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_password/
--rw-r--r--   0 runner    (1001) docker     (123)    47170 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_password/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_pre_authorized/
--rw-r--r--   0 runner    (1001) docker     (123)    38158 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_pre_authorized/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/claims_mapping_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    20133 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/claims_mapping_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/conditional_access_policy/
--rw-r--r--   0 runner    (1001) docker     (123)   159595 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/conditional_access_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/custom_directory_role/
--rw-r--r--   0 runner    (1001) docker     (123)    58656 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/custom_directory_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_access_package/
--rw-r--r--   0 runner    (1001) docker     (123)    31337 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_access_package/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_access_package_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)    29683 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_access_package_catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_administrative_unit/
--rw-r--r--   0 runner    (1001) docker     (123)    35968 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_administrative_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application/
--rw-r--r--   0 runner    (1001) docker     (123)   171414 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application_published_app_ids/
--rw-r--r--   0 runner    (1001) docker     (123)    24645 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application_published_app_ids/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application_template/
--rw-r--r--   0 runner    (1001) docker     (123)    30259 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_client_config/
--rw-r--r--   0 runner    (1001) docker     (123)    24063 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_client_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_directory_object/
--rw-r--r--   0 runner    (1001) docker     (123)    26028 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_directory_object/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_directory_roles/
--rw-r--r--   0 runner    (1001) docker     (123)    33738 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_directory_roles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_domains/
--rw-r--r--   0 runner    (1001) docker     (123)    52583 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_domains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_group/
--rw-r--r--   0 runner    (1001) docker     (123)    48521 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_groups/
--rw-r--r--   0 runner    (1001) docker     (123)    43649 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_groups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_service_principal/
--rw-r--r--   0 runner    (1001) docker     (123)    85954 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_service_principal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_service_principals/
--rw-r--r--   0 runner    (1001) docker     (123)    50940 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_service_principals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_user/
--rw-r--r--   0 runner    (1001) docker     (123)    40255 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_users/
--rw-r--r--   0 runner    (1001) docker     (123)    48498 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_users/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/directory_role/
--rw-r--r--   0 runner    (1001) docker     (123)    34780 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/directory_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/directory_role_assignment/
--rw-r--r--   0 runner    (1001) docker     (123)    46418 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/directory_role_assignment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/directory_role_member/
--rw-r--r--   0 runner    (1001) docker     (123)    35113 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/directory_role_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/group/
--rw-r--r--   0 runner    (1001) docker     (123)   104726 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/group_member/
--rw-r--r--   0 runner    (1001) docker     (123)    34251 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/group_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/invitation/
--rw-r--r--   0 runner    (1001) docker     (123)    52285 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/invitation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/named_location/
--rw-r--r--   0 runner    (1001) docker     (123)    53279 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/named_location/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    57813 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal/
--rw-r--r--   0 runner    (1001) docker     (123)   148246 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    51492 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_claims_mapping_policy_assignment/
--rw-r--r--   0 runner    (1001) docker     (123)    21574 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_claims_mapping_policy_assignment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_delegated_permission_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    43680 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_delegated_permission_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_password/
--rw-r--r--   0 runner    (1001) docker     (123)    47768 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_password/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_token_signing_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    40516 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_token_signing_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/synchronization_job/
--rw-r--r--   0 runner    (1001) docker     (123)    47076 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/synchronization_job/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/synchronization_secret/
--rw-r--r--   0 runner    (1001) docker     (123)    50249 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/synchronization_secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/user/
--rw-r--r--   0 runner    (1001) docker     (123)   124438 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.963014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/user_flow_attribute/
--rw-r--r--   0 runner    (1001) docker     (123)    36734 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/user_flow_attribute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.951014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-04-14 03:15:55.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-14 03:15:55.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:15:55.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 03:15:55.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-14 03:15:55.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.279675 cdktf-cdktf-provider-azuread-6.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-04-18 03:15:44.279675 cdktf-cdktf-provider-azuread-6.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 03:15:44.279675 cdktf-cdktf-provider-azuread-6.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.263675 cdktf-cdktf-provider-azuread-6.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.267675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/
+-rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.267675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2464522 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/_jsii/provider-azuread@6.0.1.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.271675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/access_package/
+-rw-r--r--   0 runner    (1001) docker     (123)    38947 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/access_package/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.271675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/access_package_assignment_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)   312905 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/access_package_assignment_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.271675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/access_package_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    41133 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/access_package_catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.271675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/access_package_resource_catalog_association/
+-rw-r--r--   0 runner    (1001) docker     (123)    37366 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/access_package_resource_catalog_association/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.271675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/access_package_resource_package_association/
+-rw-r--r--   0 runner    (1001) docker     (123)    37722 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/access_package_resource_package_association/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.271675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/administrative_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)    44934 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/administrative_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.271675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/administrative_unit_member/
+-rw-r--r--   0 runner    (1001) docker     (123)    36110 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/administrative_unit_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.271675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/administrative_unit_role_member/
+-rw-r--r--   0 runner    (1001) docker     (123)    38281 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/administrative_unit_role_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.271675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/app_role_assignment/
+-rw-r--r--   0 runner    (1001) docker     (123)    35528 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/app_role_assignment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.271675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/application/
+-rw-r--r--   0 runner    (1001) docker     (123)   339995 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.271675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/application_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    51104 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/application_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/application_federated_identity_credential/
+-rw-r--r--   0 runner    (1001) docker     (123)    47523 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/application_federated_identity_credential/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/application_password/
+-rw-r--r--   0 runner    (1001) docker     (123)    47170 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/application_password/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/application_pre_authorized/
+-rw-r--r--   0 runner    (1001) docker     (123)    38158 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/application_pre_authorized/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/claims_mapping_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    20133 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/claims_mapping_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/conditional_access_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)   159595 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/conditional_access_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/custom_directory_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    58656 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/custom_directory_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_access_package/
+-rw-r--r--   0 runner    (1001) docker     (123)    31337 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_access_package/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_access_package_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    29683 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_access_package_catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_administrative_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)    35968 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_administrative_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_application/
+-rw-r--r--   0 runner    (1001) docker     (123)   171414 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_application_published_app_ids/
+-rw-r--r--   0 runner    (1001) docker     (123)    24645 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_application_published_app_ids/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_application_template/
+-rw-r--r--   0 runner    (1001) docker     (123)    30259 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_application_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_client_config/
+-rw-r--r--   0 runner    (1001) docker     (123)    24063 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_client_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_directory_object/
+-rw-r--r--   0 runner    (1001) docker     (123)    26028 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_directory_object/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_directory_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)    33738 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_directory_roles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_domains/
+-rw-r--r--   0 runner    (1001) docker     (123)    52583 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_domains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_group/
+-rw-r--r--   0 runner    (1001) docker     (123)    48521 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)    43649 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_groups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_service_principal/
+-rw-r--r--   0 runner    (1001) docker     (123)    85954 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_service_principal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_service_principals/
+-rw-r--r--   0 runner    (1001) docker     (123)    50940 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_service_principals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_user/
+-rw-r--r--   0 runner    (1001) docker     (123)    40255 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_users/
+-rw-r--r--   0 runner    (1001) docker     (123)    48498 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_users/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/directory_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    34780 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/directory_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/directory_role_assignment/
+-rw-r--r--   0 runner    (1001) docker     (123)    46418 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/directory_role_assignment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/directory_role_member/
+-rw-r--r--   0 runner    (1001) docker     (123)    35113 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/directory_role_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.275675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/group/
+-rw-r--r--   0 runner    (1001) docker     (123)   104726 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.279675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/group_member/
+-rw-r--r--   0 runner    (1001) docker     (123)    34251 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/group_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.279675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/invitation/
+-rw-r--r--   0 runner    (1001) docker     (123)    52285 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/invitation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.279675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/named_location/
+-rw-r--r--   0 runner    (1001) docker     (123)    53279 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/named_location/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.279675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    57813 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.279675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/service_principal/
+-rw-r--r--   0 runner    (1001) docker     (123)   148246 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/service_principal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.279675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/service_principal_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    51492 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/service_principal_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.279675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/service_principal_claims_mapping_policy_assignment/
+-rw-r--r--   0 runner    (1001) docker     (123)    21574 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/service_principal_claims_mapping_policy_assignment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.279675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/service_principal_delegated_permission_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    43680 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/service_principal_delegated_permission_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.279675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/service_principal_password/
+-rw-r--r--   0 runner    (1001) docker     (123)    47768 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/service_principal_password/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.279675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/service_principal_token_signing_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    40516 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/service_principal_token_signing_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.279675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/synchronization_job/
+-rw-r--r--   0 runner    (1001) docker     (123)    47076 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/synchronization_job/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.279675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/synchronization_secret/
+-rw-r--r--   0 runner    (1001) docker     (123)    50249 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/synchronization_secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.279675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/user/
+-rw-r--r--   0 runner    (1001) docker     (123)   124438 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.279675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/user_flow_attribute/
+-rw-r--r--   0 runner    (1001) docker     (123)    36734 2023-04-18 03:15:30.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/user_flow_attribute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:15:44.267675 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-04-18 03:15:44.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-18 03:15:44.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 03:15:44.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 03:15:44.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-18 03:15:44.000000 cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/LICENSE` & `cdktf-cdktf-provider-azuread-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/PKG-INFO` & `cdktf-cdktf-provider-azuread-6.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-azuread
-Version: 6.0.0
+Version: 6.0.1
 Summary: Prebuilt azuread Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-azuread.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-azuread.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/README.md` & `cdktf-cdktf-provider-azuread-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/setup.py` & `cdktf-cdktf-provider-azuread-6.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-azuread",
-    "version": "6.0.0",
+    "version": "6.0.1",
     "description": "Prebuilt azuread Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-azuread.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -73,15 +73,15 @@
         "cdktf_cdktf_provider_azuread.synchronization_job",
         "cdktf_cdktf_provider_azuread.synchronization_secret",
         "cdktf_cdktf_provider_azuread.user",
         "cdktf_cdktf_provider_azuread.user_flow_attribute"
     ],
     "package_data": {
         "cdktf_cdktf_provider_azuread._jsii": [
-            "provider-azuread@6.0.0.jsii.tgz"
+            "provider-azuread@6.0.1.jsii.tgz"
         ],
         "cdktf_cdktf_provider_azuread": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/access_package/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package_assignment_policy/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/access_package_assignment_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package_catalog/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/access_package_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package_resource_catalog_association/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/access_package_resource_catalog_association/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package_resource_package_association/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/access_package_resource_package_association/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/administrative_unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit_member/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/administrative_unit_member/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit_role_member/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/administrative_unit_role_member/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/app_role_assignment/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/app_role_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/application/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_certificate/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/application_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_federated_identity_credential/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/application_federated_identity_credential/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_password/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/application_password/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_pre_authorized/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/application_pre_authorized/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/claims_mapping_policy/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/claims_mapping_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/conditional_access_policy/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/conditional_access_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/custom_directory_role/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/custom_directory_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_access_package/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_access_package/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_access_package_catalog/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_access_package_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_administrative_unit/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_administrative_unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_application/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application_published_app_ids/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_application_published_app_ids/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application_template/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_application_template/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_client_config/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_client_config/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_directory_object/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_directory_object/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_directory_roles/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_directory_roles/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_domains/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_domains/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_group/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_groups/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_service_principal/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_service_principal/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_service_principals/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_service_principals/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_user/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_users/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/data_azuread_users/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/directory_role/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/directory_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/directory_role_assignment/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/directory_role_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/directory_role_member/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/directory_role_member/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/group/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/group_member/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/group_member/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/invitation/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/invitation/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/named_location/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/named_location/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/provider/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/service_principal/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_certificate/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/service_principal_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_claims_mapping_policy_assignment/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/service_principal_claims_mapping_policy_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_delegated_permission_grant/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/service_principal_delegated_permission_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_password/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/service_principal_password/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_token_signing_certificate/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/service_principal_token_signing_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/synchronization_job/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/synchronization_job/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/synchronization_secret/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/synchronization_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/user/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/user_flow_attribute/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread/user_flow_attribute/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread.egg-info/PKG-INFO` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-azuread
-Version: 6.0.0
+Version: 6.0.1
 Summary: Prebuilt azuread Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-azuread.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-azuread.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-azuread-6.0.1/src/cdktf_cdktf_provider_azuread.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_azuread/py.typed
 src/cdktf_cdktf_provider_azuread.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_azuread.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_azuread.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_azuread.egg-info/requires.txt
 src/cdktf_cdktf_provider_azuread.egg-info/top_level.txt
 src/cdktf_cdktf_provider_azuread/_jsii/__init__.py
-src/cdktf_cdktf_provider_azuread/_jsii/provider-azuread@6.0.0.jsii.tgz
+src/cdktf_cdktf_provider_azuread/_jsii/provider-azuread@6.0.1.jsii.tgz
 src/cdktf_cdktf_provider_azuread/access_package/__init__.py
 src/cdktf_cdktf_provider_azuread/access_package_assignment_policy/__init__.py
 src/cdktf_cdktf_provider_azuread/access_package_catalog/__init__.py
 src/cdktf_cdktf_provider_azuread/access_package_resource_catalog_association/__init__.py
 src/cdktf_cdktf_provider_azuread/access_package_resource_package_association/__init__.py
 src/cdktf_cdktf_provider_azuread/administrative_unit/__init__.py
 src/cdktf_cdktf_provider_azuread/administrative_unit_member/__init__.py
```

