# Comparing `tmp/ansible-modules-hashivault-5.0.0.tar.gz` & `tmp/ansible-modules-hashivault-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-modules-hashivault-5.0.0.tar", last modified: Tue Nov  8 11:30:09 2022, max compression
+gzip compressed data, was "ansible-modules-hashivault-5.1.0.tar", last modified: Tue Apr 18 18:54:10 2023, max compression
```

## Comparing `ansible-modules-hashivault-5.0.0.tar` & `ansible-modules-hashivault-5.1.0.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2022-11-08 11:30:09.303420 ansible-modules-hashivault-5.0.0/
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)       36 2020-11-06 20:49:46.000000 ansible-modules-hashivault-5.0.0/AUTHORS
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)    28309 2022-11-08 11:29:58.000000 ansible-modules-hashivault-5.0.0/CHANGELOG.rst
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1079 2020-11-06 20:49:46.000000 ansible-modules-hashivault-5.0.0/LICENSE
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)      114 2020-11-06 20:49:46.000000 ansible-modules-hashivault-5.0.0/MANIFEST.in
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     6733 2022-11-08 11:30:09.303634 ansible-modules-hashivault-5.0.0/PKG-INFO
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     6376 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/README.rst
-drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2022-11-08 11:30:09.212302 ansible-modules-hashivault-5.0.0/ansible/
-drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2022-11-08 11:30:09.216673 ansible-modules-hashivault-5.0.0/ansible/module_utils/
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)    13379 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/ansible/module_utils/hashivault.py
-drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2022-11-08 11:30:09.212084 ansible-modules-hashivault-5.0.0/ansible/modules/
-drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2022-11-08 11:30:09.295192 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)        0 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/__init__.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7661 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_approle_role.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1673 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_approle_role_get.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1762 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_approle_role_id.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1565 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_approle_role_list.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4722 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_approle_role_secret.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2069 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_approle_role_secret_accessor_get.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2312 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_approle_role_secret_get.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1970 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_approle_role_secret_list.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2933 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_audit.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1228 2022-11-07 21:30:40.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_audit_list.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)    10086 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_auth_ldap.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1289 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_auth_list.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4124 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_auth_method.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3499 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_aws_auth_config.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7274 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_aws_auth_role.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4182 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_azure_auth_config.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7090 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_azure_auth_role.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4184 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_azure_secret_engine_config.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3745 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_azure_secret_engine_role.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2112 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_cluster_status.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2688 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_consul_secret_engine_config.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     5362 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_consul_secret_engine_role.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7073 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_db_secret_engine_config.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     6299 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_db_secret_engine_role.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     3247 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_delete.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1536 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_generate_root.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1435 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_generate_root_cancel.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2125 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_generate_root_init.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1172 2022-10-22 13:30:33.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_generate_root_status.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     5903 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_identity_entity.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7527 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_identity_entity_alias.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     9178 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_identity_group.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7489 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_identity_group_alias.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3901 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_init.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4121 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_k8s_auth_config.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     6187 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_k8s_auth_role.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4059 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_ldap_group.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1203 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_leader.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3967 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_list.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2487 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_namespace.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     5366 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_oidc_auth_method_config.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     9357 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_oidc_auth_role.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)    11153 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_ca.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2728 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_ca_set.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2065 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_cert_get.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     6029 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_cert_issue.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1828 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_cert_list.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2314 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_cert_revoke.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     6865 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_cert_sign.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2708 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_crl.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1987 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_crl_get.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1965 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_crl_rotate.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)    19029 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_role.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2115 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_role_get.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1839 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_role_list.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2948 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_set_signed.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     3198 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_tidy.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     3359 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_url.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1942 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_url_get.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2946 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_policy.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1588 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_policy_get.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1458 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_policy_list.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1796 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_read.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1251 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_read_to_file.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1789 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_rekey.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1337 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_rekey_cancel.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3530 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_rekey_init.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1152 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_rekey_status.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1702 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_rekey_verify.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1276 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_seal.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     5971 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_secret.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     9290 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_secret_engine.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1364 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_secret_list.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)    18577 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_ssh_role.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2267 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_ssh_role_list.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1189 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_status.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4688 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_token_create.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2140 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_token_lookup.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2531 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_token_renew.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2088 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_token_revoke.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)    12376 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_token_role.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2237 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_token_role_list.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1392 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_unseal.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     5748 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_userpass.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     5301 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_write.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)      979 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_write_from_file.py
-drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2022-11-08 11:30:09.212916 ansible-modules-hashivault-5.0.0/ansible/plugins/
-drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2022-11-08 11:30:09.297116 ansible-modules-hashivault-5.0.0/ansible/plugins/action/
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     5319 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/plugins/action/hashivault_read_to_file.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2108 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/plugins/action/hashivault_write_from_file.py
-drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2022-11-08 11:30:09.298024 ansible-modules-hashivault-5.0.0/ansible/plugins/doc_fragments/
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2695 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/plugins/doc_fragments/hashivault.py
-drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2022-11-08 11:30:09.299047 ansible-modules-hashivault-5.0.0/ansible/plugins/lookup/
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2846 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.0.0/ansible/plugins/lookup/hashivault.py
-drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2022-11-08 11:30:09.302944 ansible-modules-hashivault-5.0.0/ansible_modules_hashivault.egg-info/
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     6733 2022-11-08 11:30:08.000000 ansible-modules-hashivault-5.0.0/ansible_modules_hashivault.egg-info/PKG-INFO
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     5306 2022-11-08 11:30:09.000000 ansible-modules-hashivault-5.0.0/ansible_modules_hashivault.egg-info/SOURCES.txt
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)        1 2022-11-08 11:30:08.000000 ansible-modules-hashivault-5.0.0/ansible_modules_hashivault.egg-info/dependency_links.txt
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)       36 2022-11-08 11:30:09.000000 ansible-modules-hashivault-5.0.0/ansible_modules_hashivault.egg-info/requires.txt
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)      231 2022-11-08 11:30:09.000000 ansible-modules-hashivault-5.0.0/ansible_modules_hashivault.egg-info/top_level.txt
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)      119 2022-11-08 11:30:09.304522 ansible-modules-hashivault-5.0.0/setup.cfg
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)      894 2022-11-08 11:26:58.000000 ansible-modules-hashivault-5.0.0/setup.py
+drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-04-18 18:54:10.866017 ansible-modules-hashivault-5.1.0/
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)       36 2020-11-06 20:49:46.000000 ansible-modules-hashivault-5.1.0/AUTHORS
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)    29188 2023-04-18 18:54:02.000000 ansible-modules-hashivault-5.1.0/CHANGELOG.rst
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1079 2020-11-06 20:49:46.000000 ansible-modules-hashivault-5.1.0/LICENSE
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)      114 2020-11-06 20:49:46.000000 ansible-modules-hashivault-5.1.0/MANIFEST.in
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     6733 2023-04-18 18:54:10.866146 ansible-modules-hashivault-5.1.0/PKG-INFO
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     6376 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/README.rst
+drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-04-18 18:54:10.795088 ansible-modules-hashivault-5.1.0/ansible/
+drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-04-18 18:54:10.800615 ansible-modules-hashivault-5.1.0/ansible/module_utils/
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)    14241 2023-03-11 12:45:43.000000 ansible-modules-hashivault-5.1.0/ansible/module_utils/hashivault.py
+drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-04-18 18:54:10.794902 ansible-modules-hashivault-5.1.0/ansible/modules/
+drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-04-18 18:54:10.861614 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)        0 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/__init__.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7661 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1673 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_get.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1762 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_id.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1565 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_list.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4722 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_secret.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2069 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_secret_accessor_get.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2312 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_secret_get.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1970 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_secret_list.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2933 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_audit.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1228 2022-11-07 21:30:40.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_audit_list.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)    10086 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_auth_ldap.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1289 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_auth_list.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4973 2023-04-18 18:08:46.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_auth_method.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3499 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_aws_auth_config.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7274 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_aws_auth_role.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4221 2023-03-31 13:47:48.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_azure_auth_config.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7090 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_azure_auth_role.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4184 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_azure_secret_engine_config.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3745 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_azure_secret_engine_role.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2112 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_cluster_status.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2688 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_consul_secret_engine_config.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     5362 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_consul_secret_engine_role.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7073 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_db_secret_engine_config.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     6299 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_db_secret_engine_role.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     3247 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_delete.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1536 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_generate_root.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1435 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_generate_root_cancel.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2125 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_generate_root_init.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1172 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_generate_root_status.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     5903 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_identity_entity.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7527 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_identity_entity_alias.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     9178 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_identity_group.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7489 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_identity_group_alias.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3901 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_init.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4121 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_k8s_auth_config.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     6187 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_k8s_auth_role.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4059 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_ldap_group.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1203 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_leader.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3967 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_list.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2487 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_namespace.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     5426 2023-04-18 18:08:46.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_oidc_auth_method_config.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     9444 2023-04-18 18:08:46.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_oidc_auth_role.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)    11153 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_ca.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2728 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_ca_set.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2065 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_cert_get.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     6029 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_cert_issue.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1828 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_cert_list.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2314 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_cert_revoke.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     6865 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_cert_sign.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2708 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_crl.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1987 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_crl_get.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1965 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_crl_rotate.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)    18694 2023-03-11 12:45:43.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_role.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2115 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_role_get.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1839 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_role_list.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2948 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_set_signed.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     3198 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_tidy.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     3359 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_url.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1942 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_url_get.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3455 2023-04-18 18:08:46.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_policy.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1588 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_policy_get.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1458 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_policy_list.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1796 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_read.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1251 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_read_to_file.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1789 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_rekey.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1337 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_rekey_cancel.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3530 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_rekey_init.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1152 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_rekey_status.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1702 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_rekey_verify.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1276 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_seal.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     5971 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_secret.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     9583 2023-04-18 18:08:46.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_secret_engine.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1364 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_secret_list.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)    18577 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_ssh_role.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2267 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_ssh_role_list.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1189 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_status.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4688 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_create.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2140 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_lookup.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2531 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_renew.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2088 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_revoke.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)    12376 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_role.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2237 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_role_list.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1392 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_unseal.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     5748 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_userpass.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     5301 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_write.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)      979 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_write_from_file.py
+drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-04-18 18:54:10.795572 ansible-modules-hashivault-5.1.0/ansible/plugins/
+drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-04-18 18:54:10.862752 ansible-modules-hashivault-5.1.0/ansible/plugins/action/
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     5319 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/plugins/action/hashivault_read_to_file.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2108 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/plugins/action/hashivault_write_from_file.py
+drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-04-18 18:54:10.863361 ansible-modules-hashivault-5.1.0/ansible/plugins/doc_fragments/
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2695 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/plugins/doc_fragments/hashivault.py
+drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-04-18 18:54:10.863803 ansible-modules-hashivault-5.1.0/ansible/plugins/lookup/
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2846 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/plugins/lookup/hashivault.py
+drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-04-18 18:54:10.865780 ansible-modules-hashivault-5.1.0/ansible_modules_hashivault.egg-info/
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     6733 2023-04-18 18:54:10.000000 ansible-modules-hashivault-5.1.0/ansible_modules_hashivault.egg-info/PKG-INFO
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     5306 2023-04-18 18:54:10.000000 ansible-modules-hashivault-5.1.0/ansible_modules_hashivault.egg-info/SOURCES.txt
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)        1 2023-04-18 18:54:10.000000 ansible-modules-hashivault-5.1.0/ansible_modules_hashivault.egg-info/dependency_links.txt
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)       36 2023-04-18 18:54:10.000000 ansible-modules-hashivault-5.1.0/ansible_modules_hashivault.egg-info/requires.txt
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)      231 2023-04-18 18:54:10.000000 ansible-modules-hashivault-5.1.0/ansible_modules_hashivault.egg-info/top_level.txt
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)      119 2023-04-18 18:54:10.866608 ansible-modules-hashivault-5.1.0/setup.cfg
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)      894 2023-04-18 18:53:07.000000 ansible-modules-hashivault-5.1.0/setup.py
```

### Comparing `ansible-modules-hashivault-5.0.0/CHANGELOG.rst` & `ansible-modules-hashivault-5.1.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 Changelog
 =========
 
 
+5.1.0 (2023-04-18)
+------------------
+- Refactor policy module. [Cees Moerkerken]
+- Add diff, fixes #439. [Cees Moerkerken]
+- Add path to return values. [Cees Moerkerken]
+- Fix line length linting. [Cees Moerkerken]
+- Only call enable or tune when changed. add comments. [Cees Moerkerken]
+- Add result to return values, fixes #435. [Cees Moerkerken]
+- Add diff, fixes #436. [Cees Moerkerken]
+- Replace whitelist_externals with allowlist_externals. [Cees
+  Moerkerken]
+- Prevent keyerror on inconsistencies between the current and desired
+  state. [Cees Moerkerken]
+- Add diff and enable check mode support. [Cees Moerkerken]
+- Warn user when an unknown value is processed by the option
+  normalization. [Benjamin Demarteau]
+- Extract option normalisation to module_utils and reverse logic to
+  allow for unknown options. [Benjamin Demarteau]
+- Create SECURITY.md. [Terry Howe]
+
+
 5.0.0 (2022-11-08)
 ------------------
 - Remove deprecated modules. [Terry Howe]
   * hashivault_approle_role_create
   * hashivault_approle_role_secret_create
   * hashivault_approle_role_secret_delete
   * hashivault_audit_enable
```

### Comparing `ansible-modules-hashivault-5.0.0/LICENSE` & `ansible-modules-hashivault-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/PKG-INFO` & `ansible-modules-hashivault-5.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-modules-hashivault
-Version: 5.0.0
+Version: 5.1.0
 Summary: Ansible Modules for Hashicorp Vault
 Home-page: https://github.com/TerryHowe/ansible-modules-hashivault
 Author: Terry Howe
 Author-email: terrylhowe@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/x-rst
```

### Comparing `ansible-modules-hashivault-5.0.0/README.rst` & `ansible-modules-hashivault-5.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/module_utils/hashivault.py` & `ansible-modules-hashivault-5.1.0/ansible/module_utils/hashivault.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 
 import hvac
 import requests
 from ansible.module_utils.basic import AnsibleModule, env_fallback
 from hvac.exceptions import InvalidPath
 
+normalize = {'list': list, 'str': str, 'dict': dict, 'bool': bool, 'int': int, 'duration': str}
+
 
 def hashivault_argspec():
     argument_spec = dict(
         url=dict(required=False, default=os.environ.get('VAULT_ADDR', ''), type='str'),
         ca_cert=dict(required=False, default=os.environ.get('VAULT_CACERT', ''), type='str'),
         ca_path=dict(required=False, default=os.environ.get('VAULT_CAPATH', ''), type='str'),
         client_cert=dict(required=False, default=os.environ.get('VAULT_CLIENT_CERT', ''), type='str'),
@@ -38,14 +40,33 @@
     module.no_log_values.discard(1)
     module.no_log_values.discard(True)
     module.no_log_values.discard(False)
     module.no_log_values.discard('ttl')
     return module
 
 
+def hashivault_normalize_from_doc(module, options, documentation):
+    desired_state = {}
+    for key, value in options.items():
+        config_type = documentation.get(key, {}).get('type')
+        if config_type is None:
+            module.warn('Unknown option "{}". Make sure this is not a typo, if it is not, please open an '
+                        'issue at https://github.com/TerryHowe/ansible-modules-hashivault/issues.'.format(key))
+        else:
+            try:
+                value = normalize[config_type](value)
+            except Exception:
+                return {'changed': False, 'failed': True,
+                        'msg': 'config item \'{}\' has wrong data format'.format(key)}
+
+        desired_state[key] = value
+
+    return desired_state
+
+
 def get_ec2_iam_role():
     request = requests.get(url='http://169.254.169.254/latest/meta-data/iam/security-credentials/')
     request.raise_for_status()
     return request.content
 
 
 def get_ec2_iam_credentials(header_value, role_id):
```

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_approle_role.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_approle_role_get.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_get.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_approle_role_id.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_id.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_approle_role_list.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_approle_role_secret.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_secret.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_approle_role_secret_accessor_get.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_secret_accessor_get.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_approle_role_secret_get.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_secret_get.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_approle_role_secret_list.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_secret_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_audit.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_audit.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_audit_list.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_audit_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_auth_ldap.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_auth_ldap.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_auth_list.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_auth_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_auth_method.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_ldap_group.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,124 +1,127 @@
 #!/usr/bin/env python
-from ansible.module_utils.hashivault import is_state_changed
 from ansible.module_utils.hashivault import hashivault_argspec
 from ansible.module_utils.hashivault import hashivault_auth_client
 from ansible.module_utils.hashivault import hashivault_init
 from ansible.module_utils.hashivault import hashiwrapper
 
 ANSIBLE_METADATA = {'status': ['stableinterface'], 'supported_by': 'community', 'version': '1.1'}
 DOCUMENTATION = '''
 ---
-module: hashivault_auth_method
-version_added: "3.17.7"
-short_description: Hashicorp Vault auth module
+module: hashivault_ldap_group
+version_added: "3.18.3"
+short_description: Hashicorp Vault LDAP group configuration module
 description:
-    - Module to enable or disable authentication methods in Hashicorp Vault.
+    - Module to configure LDAP groups in Hashicorp Vault.
 options:
-    method_type:
+    mount_point:
         description:
-            - name of auth method. [required]
-    description:
+            - location where this method/backend is mounted. also known as "path"
+        default: ldap
+    name:
         description:
-            - description of authenticator
-    mount_point:
+            - name of the group
+        default: None
+    policies:
         description:
-            - location where this auth_method will be mounted. also known as "path"
+            - policies to be tied to the group
+        default: None
     state:
         description:
-            - should auth mount be enabled or disabled
-        default: enabled
-    config:
-        description:
-            - configuration set on auth method. expects a dict
-        default: "{'default_lease_ttl': 2764800, 'max_lease_ttl': 2764800, 'force_no_cache':False,
-                  'token_type': 'default-service'}"
+            - whether create/update or delete the entity
 extends_documentation_fragment: hashivault
 '''
 EXAMPLES = '''
 ---
 - hosts: localhost
   tasks:
-    - hashivault_auth_method:
-        method_type: userpass
+    - hashivault_ldap_group:
+        name: 'my-group'
+        policies:
+            - 'my-policy'
+        token: "{{ vault_token }}"
+        url: "{{ vault_url }}"
 '''
 
-DEFAULT_TTL = 2764800
-DEFAULT_CONFIG = {
-    'default_lease_ttl': DEFAULT_TTL,
-    'max_lease_ttl': DEFAULT_TTL,
-    'force_no_cache': False,
-    'token_type': 'default-service'
-}
-
 
 def main():
     argspec = hashivault_argspec()
-    argspec['method_type'] = dict(required=True, type='str')
-    argspec['description'] = dict(required=False, type='str', default='')
-    argspec['state'] = dict(required=False, type='str', default='enabled',
-                            choices=['enabled', 'disabled', 'enable', 'disable'])
-    argspec['mount_point'] = dict(required=False, type='str', default=None)
-    argspec['config'] = dict(required=False, type='dict',
-                             default=DEFAULT_CONFIG)
-    module = hashivault_init(argspec, supports_check_mode=True)
-    result = hashivault_auth_method(module)
+    argspec['name'] = dict(required=True, type='str', default=None)
+    argspec['mount_point'] = dict(required=False, type='str', default='ldap')
+    argspec['policies'] = dict(required=False, type='list', default=[])
+    argspec['state'] = dict(required=False, choices=['present', 'absent'], default='present')
+    module = hashivault_init(argspec)
+    result = hashivault_ldap_group(module.params)
     if result.get('failed'):
         module.fail_json(**result)
     else:
         module.exit_json(**result)
 
 
-@hashiwrapper
-def hashivault_auth_method(module):
-    params = module.params
+def hashivault_ldap_group_update(group_details, client, group_name, group_policies, mount_point):
+    changed = False
+
+    # existing policies
+    if group_details['policies'] is not None:
+        if set(group_details['policies']) != set(group_policies):
+            changed = True
+    # new policies and none existing
+    elif len(group_policies) > 0:
+        changed = True
+
+    if changed:
+        try:
+            response = client.auth.ldap.create_or_update_group(
+                name=group_name,
+                policies=group_policies,
+                mount_point=mount_point
+            )
+        except Exception as e:
+            return {'failed': True, 'msg': str(e)}
+        if response.status_code == 204:
+            return {'changed': True}
+        return {'changed': True, 'data': response}
+    return {'changed': False}
+
+
+def hashivault_ldap_group_create_or_update(params):
     client = hashivault_auth_client(params)
-    method_type = params.get('method_type')
-    description = params.get('description')
+    group_name = params.get('name')
     mount_point = params.get('mount_point')
-    config = params.get('config')
-    if params.get('state') in ['enabled', 'enable']:
-        state = 'enabled'
-    else:
-        state = 'disabled'
-    exists = False
-    changed = False
-    create = False
+    group_policies = params.get('policies')
+    try:
+        group_details = client.auth.ldap.read_group(name=group_name, mount_point=mount_point)
+    except Exception:
+        client.auth.ldap.create_or_update_group(
+            name=group_name,
+            policies=group_policies,
+            mount_point=mount_point
+        )
+        return {'changed': True}
+    return hashivault_ldap_group_update(group_details['data'], client, group_name=group_name,
+                                        group_policies=group_policies,
+                                        mount_point=mount_point)
 
-    if mount_point is None:
-        mount_point = method_type
+
+def hashivault_ldap_group_delete(params):
+    client = hashivault_auth_client(params)
+    group_name = params.get('name')
 
     try:
-        result = client.sys.list_auth_methods()
-        auth_methods = result.get('data', result)
-        if (mount_point + u"/") in auth_methods:
-            exists = True
+        client.auth.ldap.read_group(name=group_name)
     except Exception:
-        pass
+        return {'changed': False}
+    client.auth.ldap.delete_group(name=group_name)
+    return {'changed': True}
 
-    if state == 'enabled' and not exists:
-        changed = True
-        create = True
-    elif state == 'disabled' and exists:
-        changed = True
-    elif exists and state == 'enabled':
-        current_state = auth_methods[mount_point + u"/"]
-        changed = description != current_state['description'] or is_state_changed(config, current_state['config'])
-
-    if module.check_mode:
-        return {'changed': changed, 'created': create, 'state': state}
-    if not changed:
-        return {'changed': changed, 'created': False, 'state': state}
-
-    if state == 'enabled':
-        if create:
-            client.sys.enable_auth_method(method_type, description=description, path=mount_point, config=config)
-        else:
-            client.sys.tune_auth_method(description=description, path=mount_point, **config)
-    if state == 'disabled':
-        client.sys.disable_auth_method(path=mount_point)
 
-    return {'changed': changed, 'created': create}
+@hashiwrapper
+def hashivault_ldap_group(params):
+    state = params.get('state')
+    if state == 'present':
+        return hashivault_ldap_group_create_or_update(params)
+    elif state == 'absent':
+        return hashivault_ldap_group_delete(params)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_aws_auth_config.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_aws_auth_config.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_aws_auth_role.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_aws_auth_role.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_azure_auth_config.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_azure_auth_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,16 +101,17 @@
     try:
         current_state = client.auth.azure.read_config()
     except Exception:
         changed = True
 
     # check if current config matches desired config values, if they dont match, set changed true
     for k, v in current_state.items():
-        if v != desired_state[k]:
-            changed = True
+        if k in desired_state:
+            if v != desired_state[k]:
+                changed = True
 
     # if configs dont match and checkmode is off, complete the change
     if changed and not module.check_mode:
         client.auth.azure.configure(mount_point=mount_point, **desired_state)
 
     return {'changed': changed}
```

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_azure_auth_role.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_azure_auth_role.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_azure_secret_engine_config.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_azure_secret_engine_config.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_azure_secret_engine_role.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_azure_secret_engine_role.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_cluster_status.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_cluster_status.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_consul_secret_engine_config.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_consul_secret_engine_config.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_consul_secret_engine_role.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_consul_secret_engine_role.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_db_secret_engine_config.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_db_secret_engine_config.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_db_secret_engine_role.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_db_secret_engine_role.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_delete.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_delete.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_generate_root.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_generate_root.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_generate_root_cancel.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_generate_root_cancel.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_generate_root_init.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_generate_root_init.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_generate_root_status.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_generate_root_status.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_identity_entity.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_identity_entity.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_identity_entity_alias.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_identity_entity_alias.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_identity_group.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_identity_group.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_identity_group_alias.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_identity_group_alias.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_init.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_init.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_k8s_auth_config.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_k8s_auth_config.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_k8s_auth_role.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_k8s_auth_role.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_leader.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_leader.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_list.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_namespace.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_namespace.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_oidc_auth_method_config.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_oidc_auth_method_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,12 +128,18 @@
         current_value = current_state.get(key, None)
         if current_value is not None and current_value != desired_state[key]:
             changed = True
             break
 
     if changed and not module.check_mode:
         client.auth.oidc.configure(**desired_state)
-    return {'changed': changed, 'old_state': current_state, 'new_state': desired_state}
+    return {
+        'changed': changed,
+        "diff": {
+            "before": current_state,
+            "after": desired_state,
+        }
+    }
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_oidc_auth_role.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_oidc_auth_role.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
     argspec['token_period'] = dict(required=False, type='int', default=0)
     argspec['token_type'] = dict(required=False, type='str', default='default')
     argspec['clock_skew_leeway'] = dict(required=False, type='int', default=0)
     argspec['expiration_leeway'] = dict(required=False, type='int', default=0)
     argspec['not_before_leeway'] = dict(required=False, type='int', default=0)
     argspec['role_type'] = dict(required=False, type='str', default='oidc', choices=['oidc', 'jwt'])
 
-    module = hashivault_init(argspec)
+    module = hashivault_init(argspec, supports_check_mode=True)
     result = hashivault_oidc_auth_role(module)
     if result.get('failed'):
         module.fail_json(**result)
     else:
         module.exit_json(**result)
 
 
@@ -200,12 +200,19 @@
             break
 
     if changed and not module.check_mode:
         if not current_state and state == 'present':
             client.auth.oidc.create_role(name=name, **desired_state)
         elif current_state and state == 'absent':
             client.auth.oidc.delete_role(name=name)
-    return {'changed': changed, 'old_state': current_state, 'new_state': desired_state}
+
+    return {
+        'changed': changed,
+        "diff": {
+            "before": current_state,
+            "after": desired_state,
+        }
+    }
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_ca.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_ca.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_ca_set.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_ca_set.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_cert_get.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_cert_get.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_cert_issue.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_cert_issue.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_cert_list.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_cert_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_cert_revoke.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_cert_revoke.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_cert_sign.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_cert_sign.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_crl.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_crl.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_crl_get.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_crl_get.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_crl_rotate.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_crl_rotate.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_role.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_role.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
-from ansible.module_utils.hashivault import hashivault_auth_client
 from ansible.module_utils.hashivault import hashivault_argspec
+from ansible.module_utils.hashivault import hashivault_auth_client
 from ansible.module_utils.hashivault import hashivault_init
-from ansible.module_utils.hashivault import is_state_changed
+from ansible.module_utils.hashivault import hashivault_normalize_from_doc
 from ansible.module_utils.hashivault import hashiwrapper
+from ansible.module_utils.hashivault import is_state_changed
 
 ANSIBLE_METADATA = {'status': ['preview'], 'supported_by': 'community', 'version': '1.1'}
 DOCUMENTATION = r'''
 ---
 module: hashivault_pki_role
 version_added: "4.5.0"
 short_description: Hashicorp Vault PKI Create/Update/Delete Role
@@ -305,15 +306,14 @@
             allow_subdomains: true
 
     - hashivault_pki_role:
         name: tester
         role_file: "/opt/vault/etc/roles/pki-tester.json"
         state: "present"
 '''
-normalize = {'list': list, 'str': str, 'dict': dict, 'bool': bool, 'int': int, 'duration': str}
 
 
 def main():
     argspec = hashivault_argspec()
     argspec['name'] = dict(required=True, type='str')
     argspec['state'] = dict(required=False, type='str', default='present', choices=['present', 'absent'])
     argspec['mount_point'] = dict(required=False, type='str', default='pki')
@@ -347,23 +347,16 @@
 
     if role_file:
         import json
         desired_state = json.loads(open(role_file, 'r').read())
     elif config:
         import yaml
         doc = yaml.safe_load(DOCUMENTATION)
-        args = doc.get('options').get('config').get('suboptions').items()
-        for key, value in args:
-            arg = config.get(key)
-            if arg is not None:
-                try:
-                    desired_state[key] = normalize[value.get('type')](arg)
-                except Exception:
-                    return {'changed': False, 'failed': True,
-                            'msg': 'config item \'{}\' has wrong data format'.format(key)}
+        args = doc.get('options').get('config').get('suboptions')
+        desired_state = hashivault_normalize_from_doc(module, config, args)
 
     changed = False
     try:
         current_state = client.secrets.pki.read_role(name=name, mount_point=mount_point).get('data')
     except Exception:
         current_state = {}
     if current_state:
```

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_role_get.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_role_get.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_role_list.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_role_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_set_signed.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_set_signed.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_tidy.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_tidy.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_url.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_url.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_pki_url_get.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_url_get.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_policy.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_policy.py`

 * *Files 22% similar despite different names*

```diff
@@ -43,49 +43,74 @@
 def main():
     argspec = hashivault_argspec()
     argspec['name'] = dict(required=True, type='str')
     argspec['rules'] = dict(required=False, type='str')
     argspec['rules_file'] = dict(required=False, type='str')
     argspec['state'] = dict(required=False, choices=['present', 'absent'], default='present')
     mutually_exclusive = [['rules', 'rules_file']]
-    module = hashivault_init(argspec, mutually_exclusive=mutually_exclusive)
-    result = hashivault_policy(module.params)
+    module = hashivault_init(argspec, mutually_exclusive=mutually_exclusive, supports_check_mode=True)
+    result = hashivault_policy(module)
     if result.get('failed'):
         module.fail_json(**result)
     else:
         module.exit_json(**result)
 
 
 @hashiwrapper
-def hashivault_policy(params):
+def hashivault_policy(module):
+    params = module.params
     client = hashivault_auth_client(params)
     state = params.get('state')
     name = params.get('name')
-    if state == 'present':
-        rules_file = params.get('rules_file')
-        if rules_file:
-            try:
-                rules = open(rules_file, 'r').read()
-            except Exception as e:
-                return {'changed': False,
-                        'failed': True,
-                        'msg': 'Error opening rules file <%s>: %s' % (rules_file, str(e))}
-        else:
-            rules = params.get('rules')
-        current = client.get_policy(name)
-        if current == rules:
-            return {'changed': False}
-        client.sys.create_or_update_policy(name, rules)
-        return {'changed': True}
+    exists = False
+    changed = False
+    current_state = {}
+    desired_state = {}
 
+    # get current policies
     current_policies = client.sys.list_policies()
     if isinstance(current_policies, dict):
-        current_policies = current_policies.get('data', current_policies)
         current_policies = current_policies.get('policies', current_policies)
-    if name not in current_policies:
-        return {'changed': False}
-    client.sys.delete_policy(name)
-    return {'changed': True}
+    if name in current_policies:
+        exists = True
+        current_state = client.get_policy(name)
+
+    # Define desired rules
+    rules_file = params.get('rules_file')
+    if rules_file:
+        try:
+            desired_state = open(rules_file, 'r').read()
+        except Exception as e:
+            return {'changed': False,
+                    'failed': True,
+                    'msg': 'Error opening rules file <%s>: %s' % (rules_file, str(e))}
+    else:
+        desired_state = params.get('rules')
+
+    # Check required actions
+    if state == 'present' and not exists:
+        changed = True
+    elif state == 'absent' and exists:
+        changed = True
+    elif state == 'present' and exists:
+        if current_state != desired_state:
+            changed = True
+
+    if changed and not module.check_mode:
+        # create or update
+        if state == 'present':
+            client.sys.create_or_update_policy(name, desired_state)
+        # delete
+        elif state == 'absent':
+            client.sys.delete_policy(name)
+
+    return {
+        "changed": changed,
+        "diff": {
+            "before": current_state,
+            "after": desired_state,
+        },
+    }
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_policy_get.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_policy_get.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_policy_list.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_policy_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_read.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_read.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_read_to_file.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_read_to_file.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_rekey.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_rekey.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_rekey_cancel.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_rekey_cancel.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_rekey_init.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_rekey_init.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_rekey_status.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_rekey_status.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_rekey_verify.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_rekey_verify.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_seal.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_seal.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_secret.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_secret.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_secret_engine.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_secret_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,15 +100,15 @@
                                                                    'max_lease_ttl': DEFAULT_TTL,
                                                                    'force_no_cache': False})
     argspec['state'] = dict(required=False, type='str', choices=['present', 'enabled', 'absent', 'disabled'],
                             default='present')
     argspec['options'] = dict(required=False, type='dict', default={})
     argspec['cas_required'] = dict(required=False, type='bool')
     argspec['max_versions'] = dict(required=False, type='int')
-    module = hashivault_init(argspec)
+    module = hashivault_init(argspec, supports_check_mode=True)
     result = hashivault_secret_engine(module)
     if result.get('failed'):
         module.fail_json(**result)
     else:
         module.exit_json(**result)
 
 
@@ -169,14 +169,20 @@
         configuration = client.sys.read_mount_configuration(path=name)
         current_state = configuration['data']
         exists = True
     except Exception:
         # doesn't exist
         pass
 
+    desired_state = {
+        **config,
+        'options': options if 'version' in options else {},
+        'description': description
+    }
+
     # doesnt exist and should or does exist and shouldnt
     if (exists and state == 'disabled'):
         changed = True
     elif (not exists and state == 'enabled'):
         changed = True
     elif state == 'enabled':
         if 'version' in options:
@@ -225,12 +231,19 @@
         else:
             client.sys.tune_mount_configuration(path=name, description=description, **config)
 
     # delete
     elif changed and state == 'disabled' and not module.check_mode:
         client.sys.disable_secrets_engine(path=name)
 
-    return {'changed': changed, 'created': created}
+    return {
+        "changed": changed,
+        "created": created,
+        "diff": {
+            "before": current_state,
+            "after": desired_state,
+        },
+    }
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_secret_list.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_secret_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_ssh_role.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_ssh_role.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_ssh_role_list.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_ssh_role_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_status.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_status.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_token_create.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_create.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_token_lookup.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_lookup.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_token_renew.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_renew.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_token_revoke.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_revoke.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_token_role.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_role.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_token_role_list.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_role_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_unseal.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_unseal.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_userpass.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_userpass.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_write.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_write.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/modules/hashivault/hashivault_write_from_file.py` & `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_write_from_file.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/plugins/action/hashivault_read_to_file.py` & `ansible-modules-hashivault-5.1.0/ansible/plugins/action/hashivault_read_to_file.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/plugins/action/hashivault_write_from_file.py` & `ansible-modules-hashivault-5.1.0/ansible/plugins/action/hashivault_write_from_file.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/plugins/doc_fragments/hashivault.py` & `ansible-modules-hashivault-5.1.0/ansible/plugins/doc_fragments/hashivault.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible/plugins/lookup/hashivault.py` & `ansible-modules-hashivault-5.1.0/ansible/plugins/lookup/hashivault.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/ansible_modules_hashivault.egg-info/PKG-INFO` & `ansible-modules-hashivault-5.1.0/ansible_modules_hashivault.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-modules-hashivault
-Version: 5.0.0
+Version: 5.1.0
 Summary: Ansible Modules for Hashicorp Vault
 Home-page: https://github.com/TerryHowe/ansible-modules-hashivault
 Author: Terry Howe
 Author-email: terrylhowe@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/x-rst
```

### Comparing `ansible-modules-hashivault-5.0.0/ansible_modules_hashivault.egg-info/SOURCES.txt` & `ansible-modules-hashivault-5.1.0/ansible_modules_hashivault.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.0.0/setup.py` & `ansible-modules-hashivault-5.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "ansible/modules/hashivault",
 ]
 
 long_description = open('README.rst', 'r').read()
 
 setup(
     name='ansible-modules-hashivault',
-    version='5.0.0',
+    version='5.1.0',
     description='Ansible Modules for Hashicorp Vault',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Terry Howe',
     author_email='terrylhowe@example.com',
     url='https://github.com/TerryHowe/ansible-modules-hashivault',
     py_modules=py_files,
```

