# Comparing `tmp/vmware-nsxlib-19.2.4.tar.gz` & `tmp/vmware-nsxlib-19.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmware-nsxlib-19.2.4.tar", last modified: Tue Apr 18 01:23:37 2023, max compression
+gzip compressed data, was "vmware-nsxlib-19.3.0.tar", last modified: Mon Apr  3 21:23:15 2023, max compression
```

## Comparing `vmware-nsxlib-19.2.4.tar` & `vmware-nsxlib-19.3.0.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:37.500251 vmware-nsxlib-19.2.4/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1850 2023-04-18 01:23:37.000000 vmware-nsxlib-19.2.4/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36593 2023-04-18 01:23:37.000000 vmware-nsxlib-19.2.4/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1069 2023-04-18 01:23:37.500251 vmware-nsxlib-19.2.4/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/babel.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:37.488251 vmware-nsxlib-19.2.4/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:37.488251 vmware-nsxlib-19.2.4/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2463 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/doc/source/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/doc/source/readme.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/doc/source/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:37.484251 vmware-nsxlib-19.2.4/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:37.488251 vmware-nsxlib-19.2.4/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/releasenotes/notes/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:37.488251 vmware-nsxlib-19.2.4/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:37.488251 vmware-nsxlib-19.2.4/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:37.488251 vmware-nsxlib-19.2.4/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9050 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7980 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/run_tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1320 2023-04-18 01:23:37.500251 vmware-nsxlib-19.2.4/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3461 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:37.492251 vmware-nsxlib-19.2.4/vmware_nsxlib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1089 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/_i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:37.492251 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:37.492251 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:37.492251 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8272 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/mocks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15186 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/nsxlib_testcase.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:37.496251 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/policy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/policy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1385 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/policy/policy_testcase.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1505 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/policy/test_alb_auth_token_provider.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18601 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/policy/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28725 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/policy/test_ipsec_vpn_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    85381 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/policy/test_lb_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   307987 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/policy/test_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27223 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/policy/test_transaction.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12798 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_cert.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14792 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25132 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1049 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_cluster_management.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23560 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30338 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_load_balancer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7433 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_native_dhcp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8249 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_ns_group_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12060 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_qos_switching_profile.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   114892 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19717 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_router.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29487 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_security.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3403 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_trust_management.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25449 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14669 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_vpn_ipsec.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:37.500251 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10813 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16955 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12546 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/client_cert.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36269 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/cluster_management.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14235 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4972 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45071 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/core_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1833 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/debug_retry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7654 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16620 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/lib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21966 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/load_balancer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3199 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/native_dhcp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6043 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/ns_group_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6561 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/nsx_constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:37.500251 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11579 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/alb_auth_token_provider.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3361 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    92602 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/core_defs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   224874 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/core_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9618 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/ipsec_vpn_defs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21062 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/ipsec_vpn_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19214 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/lb_defs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    57323 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/lb_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8336 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/transaction.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33384 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15738 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/router.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25997 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/security.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1420 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/token_provider.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5643 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/trust_management.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29341 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15442 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/v3/vpn_ipsec.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      684 2023-04-18 01:23:00.000000 vmware-nsxlib-19.2.4/vmware_nsxlib/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 01:23:37.492251 vmware-nsxlib-19.2.4/vmware_nsxlib.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1069 2023-04-18 01:23:37.000000 vmware-nsxlib-19.2.4/vmware_nsxlib.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3398 2023-04-18 01:23:37.000000 vmware-nsxlib-19.2.4/vmware_nsxlib.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-18 01:23:37.000000 vmware-nsxlib-19.2.4/vmware_nsxlib.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-18 01:23:37.000000 vmware-nsxlib-19.2.4/vmware_nsxlib.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-04-18 01:23:37.000000 vmware-nsxlib-19.2.4/vmware_nsxlib.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2023-04-18 01:23:37.000000 vmware-nsxlib-19.2.4/vmware_nsxlib.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2023-04-18 01:23:37.000000 vmware-nsxlib-19.2.4/vmware_nsxlib.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.485784 vmware-nsxlib-19.3.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1893 2023-04-03 21:23:15.000000 vmware-nsxlib-19.3.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36983 2023-04-03 21:23:15.000000 vmware-nsxlib-19.3.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2023-04-03 21:23:15.485784 vmware-nsxlib-19.3.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/babel.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.465784 vmware-nsxlib-19.3.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.465784 vmware-nsxlib-19.3.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2463 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/doc/source/readme.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/doc/source/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.461784 vmware-nsxlib-19.3.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.465784 vmware-nsxlib-19.3.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/releasenotes/notes/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.465784 vmware-nsxlib-19.3.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.465784 vmware-nsxlib-19.3.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.469784 vmware-nsxlib-19.3.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9050 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7980 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/run_tests.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1249 2023-04-03 21:23:15.485784 vmware-nsxlib-19.3.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3496 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.469784 vmware-nsxlib-19.3.0/vmware_nsxlib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1089 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/_i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.469784 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.469784 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.473784 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8272 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/mocks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15186 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/nsxlib_testcase.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.477784 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1385 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/policy_testcase.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1505 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_alb_auth_token_provider.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18601 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28725 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_ipsec_vpn_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    85381 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_lb_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   309672 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27223 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_transaction.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12798 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_cert.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14792 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25132 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1049 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_cluster_management.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23560 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30338 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_load_balancer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7433 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_native_dhcp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8249 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_ns_group_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12060 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_qos_switching_profile.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   114892 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19717 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_router.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29487 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_security.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3403 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_trust_management.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25449 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14669 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_vpn_ipsec.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.481784 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10813 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16955 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12546 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/client_cert.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36269 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/cluster_management.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14235 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4972 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    45071 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/core_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1833 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/debug_retry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7654 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16620 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/lib.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21966 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/load_balancer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3199 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/native_dhcp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6043 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/ns_group_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6617 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/nsx_constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.485784 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11579 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/alb_auth_token_provider.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3361 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    93127 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/core_defs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   225612 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/core_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9618 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/ipsec_vpn_defs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21062 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/ipsec_vpn_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19214 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/lb_defs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    57319 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/lb_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8336 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/transaction.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33384 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15738 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/router.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25997 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/security.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1420 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/token_provider.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5643 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/trust_management.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29341 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15442 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/vpn_ipsec.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      684 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.469784 vmware-nsxlib-19.3.0/vmware_nsxlib.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2023-04-03 21:23:15.000000 vmware-nsxlib-19.3.0/vmware_nsxlib.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3398 2023-04-03 21:23:15.000000 vmware-nsxlib-19.3.0/vmware_nsxlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-03 21:23:15.000000 vmware-nsxlib-19.3.0/vmware_nsxlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-03 21:23:15.000000 vmware-nsxlib-19.3.0/vmware_nsxlib.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-04-03 21:23:15.000000 vmware-nsxlib-19.3.0/vmware_nsxlib.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2023-04-03 21:23:15.000000 vmware-nsxlib-19.3.0/vmware_nsxlib.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2023-04-03 21:23:15.000000 vmware-nsxlib-19.3.0/vmware_nsxlib.egg-info/top_level.txt
```

### Comparing `vmware-nsxlib-19.2.4/AUTHORS` & `vmware-nsxlib-19.3.0/AUTHORS`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 Mengdie Song <songm@vmware.com>
 Michal Kelner Mishali <mkelnermishal@vmware.com>
 Qian Sun <sunq@vmware.com>
 Quan Tian <qtian@vmware.com>
 Ran Gu <gran@vmware.com>
 Roey Chen <roeyc@vmware.com>
 Rongrong_Miao <rmiao@vmware.com>
+Salvatore Orlando <salv.orlando@gmail.com>
 Salvatore Orlando <sorlando@vmware.com>
 Sean <ranp@vmware.com>
 Shawn Wang <wshaoquan@vmware.com>
 Shih-Hao Li <shihli@vmware.com>
 Spark Fan <yfan@vmware.com>
 Tao Zou <tazou@vmware.com>
 Tong Liu <tongl@vmware.com>
```

### Comparing `vmware-nsxlib-19.2.4/CONTRIBUTING.rst` & `vmware-nsxlib-19.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/ChangeLog` & `vmware-nsxlib-19.3.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,56 +1,44 @@
 CHANGES
 =======
 
-19.2.4
-------
-
-* Enable H-API delete for Policy Tier1 Api
-
-19.2.3
+19.3.0
 ------
 
+* Update version check to use POST API when restore vif
+* Revert "Revert "Add sync\_realization while creating ip-pool/ip-subnet for nsx-keeper""
+* Add ip\_release\_delay when creating IpPool
+* Revert "Add sync\_realization while creating ip-pool/ip-subnet for nsx-keeper"
 * Add version check to use POST API when restore vif
-
-19.2.2
-------
-
+* Add sync\_realization while creating ip-pool/ip-subnet for nsx-keeper
+* Fix issues with tox 4.2.4
 * Use POST API when restore vif
-* Get all certificates from NSX
 * Drop lower-constraints job
-
-19.2.1
-------
-
 * Allow using force option to create and release IPBlockSubnets
 * [tox] Make pass\_env compatible with tox4
-
-19.2.0
-------
-
 * Support large IPv6 subnet via NSX IPAM
+* Get all certificates from NSX
 * lower-constraints: bump pyopenssl to 21.0.0
+* Update vs/lbpool delete api to support hierarchical API
 * Restore FEATURE\_ROUTER\_FIREWALL, remove nat\_pass usage
+* Extending Overwrite Header for different PI in T1 Static routes
 * Remove FEATURE\_ROUTER\_FIREWALL support since 4.0.1
 * Add NsxInvalidPath exception for error code 500012
-* Extending Overwrite Header for different PI in T1 Static routes
 * Support two json decoder exception
 * Add resource\_type for NsxPolicyLoadBalancerSourceIpPersistenceProfileApi update
-* Handle response is not a json format
+* Add definition for 3.2.1 and 4.0.0
 * [MP] Support firewall\_match for NAT rules
-
-19.0.0
-------
-
+* Handle response is not a json format
+* Drop py36 and py37 from zuul gate test
+* Revert "Support multiple ca certificates"
+* Support multiple ca certificates
 * Operator field invalid if Scope\_operator field is present
 * Handle bad XSRF token in exception handler
 * Fix the logical port created twice
-* Drop py36 and py37 from zuul gate test
 * Add force update of Policy T1 Adv Rules
-* Fix garbage text in README file
 * Remove debug log statements
 * Accept locale\_service\_id to get seg interfaces on T1
 * Fix typo in exception name
 * Reduce page\_size if too large response size for search api
 * Bump minimum pyOpenSSL to 20.0.0
 * Add all\_results param in get\_ip\_subnet\_realization\_info
 * Adding scope\_operator support for NSX 3.2 API
```

### Comparing `vmware-nsxlib-19.2.4/LICENSE` & `vmware-nsxlib-19.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/PKG-INFO` & `vmware-nsxlib-19.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 1.1
 Name: vmware-nsxlib
-Version: 19.2.4
-Summary: A common library that interfaces with NSX
+Version: 19.3.0
+Summary: A common library that interfaces with VMware NSX
 Home-page: https://opendev.org/x/vmware-nsxlib
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
-Description: =============
+Description: TESt:wq
+        
+        
+        =============
         vmware-nsxlib
         =============
         
         * Free software: Apache license
         * Source: https://opendev.org/x/vmware-nsxlib
         
         Features
@@ -25,9 +28,7 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vmware-nsxlib-19.2.4/doc/source/conf.py` & `vmware-nsxlib-19.3.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/releasenotes/source/conf.py` & `vmware-nsxlib-19.3.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/requirements.txt` & `vmware-nsxlib-19.3.0/requirements.txt`

 * *Files 15% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 decorator>=4.4.1 # BSD
 eventlet>=0.24.1 # MIT
 netaddr>=0.7.18 # BSD
 tenacity>=6.0.0 # Apache-2.0
 oslo.i18n>=3.20.0 # Apache-2.0
 oslo.log>=4.2.1;python_version=='3.6'
 oslo.log>=4.2.1;python_version=='3.7'
-oslo.log>=4.6.0;python_version=='3.8'
+oslo.log>=5.0.0;python_version=='3.8'
 oslo.serialization>=2.28.1 # Apache-2.0
 oslo.service>=1.31.0 # Apache-2.0
 oslo.utils>=4.4.0 # Apache-2.0
 pyOpenSSL>=20.0.0 # Apache-2.0
```

### Comparing `vmware-nsxlib-19.2.4/run_tests.sh` & `vmware-nsxlib-19.3.0/run_tests.sh`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/setup.cfg` & `vmware-nsxlib-19.3.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vmware-nsxlib
-summary = A common library that interfaces with NSX
+summary = A common library that interfaces with VMware NSX
 description-file = 
 	README.rst
 author = OpenStack
 author-email = openstack-discuss@lists.openstack.org
 home-page = https://opendev.org/x/vmware-nsxlib
 classifier = 
 	Environment :: OpenStack
@@ -12,16 +12,14 @@
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
 
 [files]
 packages = 
 	vmware_nsxlib
 
 [build_sphinx]
 source-dir = doc/source
```

### Comparing `vmware-nsxlib-19.2.4/setup.py` & `vmware-nsxlib-19.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/test-requirements.txt` & `vmware-nsxlib-19.3.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/tox.ini` & `vmware-nsxlib-19.3.0/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [tox]
-envlist = py37,pep8
+envlist = py38,pep8
 minversion = 2.0
 skipsdist = True
+ignore_base_python_conflict = True
 
 [testenv]
 install_command = pip install {opts} {packages}
 basepython = python3
 setenv = VIRTUAL_ENV={envdir}
          PYTHONWARNINGS=default::DeprecationWarning
 passenv =
```

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/__init__.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/__init__.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/_i18n.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/_i18n.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/base.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/base.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/mocks.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/mocks.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/nsxlib_testcase.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/nsxlib_testcase.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/policy/policy_testcase.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/policy_testcase.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/policy/test_alb_auth_token_provider.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_alb_auth_token_provider.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/policy/test_api.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_api.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/policy/test_ipsec_vpn_resources.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_ipsec_vpn_resources.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/policy/test_lb_resources.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_lb_resources.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/policy/test_resources.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -4893,25 +4893,28 @@
         super(TestPolicyIpPool, self).setUp()
         self.resourceApi = self.policy_lib.ip_pool
 
     def test_create(self):
         name = 'test'
         description = 'desc'
         ip_pool_id = '111'
+        ip_release_delay = 10
 
         with mock.patch.object(self.policy_api,
                                "create_or_update") as api_call:
             result = self.resourceApi.create_or_overwrite(
                 name, ip_pool_id, description=description,
+                ip_release_delay=ip_release_delay,
                 tenant=TEST_TENANT)
 
             expected_def = core_defs.IpPoolDef(
                 ip_pool_id=ip_pool_id,
                 name=name,
                 description=description,
+                ip_release_delay=ip_release_delay,
                 tenant=TEST_TENANT)
 
             self.assert_called_with_def(api_call, expected_def)
             self.assertEqual(ip_pool_id, result)
 
     def test_delete(self):
         ip_pool_id = '111'
@@ -5001,14 +5004,42 @@
                 ip_block_id=ip_block_id,
                 ip_subnet_id=ip_subnet_id,
                 size=size,
                 tenant=TEST_TENANT,
                 start_ip=start_ip)
             self.assert_called_with_def(api_call, expected_def)
 
+    def test_allocate_block_subnet_sync_realization(self):
+        ip_pool_id = '111'
+        ip_block_id = 'block-id'
+        size = 256
+        ip_subnet_id = 'subnet-id'
+        start_ip = '192.168.1.0'
+        sync_realization = True
+
+        with mock.patch.object(
+                self.policy_api, "create_or_update") as api_call, \
+                mock.patch.object(self.resourceApi, 'version',
+                                  nsx_constants.NSX_VERSION_4_1_1):
+            self.resourceApi.allocate_block_subnet(
+                ip_pool_id, ip_block_id, size, ip_subnet_id,
+                tenant=TEST_TENANT, start_ip=start_ip,
+                sync_realization=sync_realization)
+
+            expected_def = core_defs.IpPoolBlockSubnetDef(
+                nsx_version=nsx_constants.NSX_VERSION_4_1_1,
+                ip_pool_id=ip_pool_id,
+                ip_block_id=ip_block_id,
+                ip_subnet_id=ip_subnet_id,
+                subnet_size='%s' % size,
+                tenant=TEST_TENANT,
+                start_ip=start_ip,
+                sync_realization=sync_realization)
+            self.assert_called_with_def(api_call, expected_def)
+
     def test_allocate_block_subnet_with_unsupported_attribute(self):
         ip_pool_id = '111'
         ip_block_id = 'block-id'
         size = 256
         ip_subnet_id = 'subnet-id'
         start_ip = '192.168.1.0'
 
@@ -5417,89 +5448,93 @@
         traffic_tag = 10
         allocate_addresses = "BOTH"
         tags = [{'scope': 'a', 'tag': 'b'}]
         hyperbus_mode = 'DISABLE'
         admin_state = True
         init_state = 'RESTORE_VIF'
 
-        with mock.patch.object(
-            self.policy_api.client, "url_post") as api_post, \
-            mock.patch.object(self.resourceApi, 'version',
-                              nsx_constants.NSX_VERSION_4_1_0):
-            result = self.resourceApi.create_or_overwrite(
-                name, segment_id, port_id=port_id, description=description,
-                address_bindings=address_bindings,
-                attachment_type=attachment_type, vif_id=vif_id, app_id=app_id,
-                context_id=context_id, traffic_tag=traffic_tag,
-                allocate_addresses=allocate_addresses,
-                hyperbus_mode=hyperbus_mode, admin_state=admin_state,
-                tags=tags,
-                tenant=TEST_TENANT,
-                init_state=init_state)
-
-            expected_def = core_defs.SegmentPortDef(
-                nsx_version=nsx_constants.NSX_VERSION_4_1_0,
-                segment_id=segment_id,
-                port_id=port_id,
-                name=name,
-                description=description,
-                address_bindings=address_bindings,
-                attachment_type=attachment_type,
-                vif_id=vif_id,
-                app_id=app_id,
-                context_id=context_id,
-                traffic_tag=traffic_tag,
-                allocate_addresses=allocate_addresses,
-                admin_state=admin_state,
-                tags=tags,
-                tenant=TEST_TENANT,
-                hyperbus_mode=hyperbus_mode,
-                init_state=init_state)
-
-            api_post.assert_called_once_with(
-                expected_def.get_resource_path(),
-                expected_def.get_obj_dict(), headers=None,
-                expected_results=None, retry_confirm=False)
-            self.assertIsNotNone(result)
-
-        with mock.patch.object(
-            self.policy_api, "create_or_update") as api_call, \
-            mock.patch.object(self.resourceApi, 'version',
-                              nsxlib_testcase.LATEST_VERSION):
-            result = self.resourceApi.create_or_overwrite(
-                name, segment_id, port_id=port_id, description=description,
-                address_bindings=address_bindings,
-                attachment_type=attachment_type, vif_id=vif_id, app_id=app_id,
-                context_id=context_id, traffic_tag=traffic_tag,
-                allocate_addresses=allocate_addresses,
-                hyperbus_mode=hyperbus_mode, admin_state=admin_state,
-                tags=tags,
-                tenant=TEST_TENANT,
-                init_state=init_state)
-
-            expected_def = core_defs.SegmentPortDef(
-                nsx_version=nsxlib_testcase.LATEST_VERSION,
-                segment_id=segment_id,
-                port_id=port_id,
-                name=name,
-                description=description,
-                address_bindings=address_bindings,
-                attachment_type=attachment_type,
-                vif_id=vif_id,
-                app_id=app_id,
-                context_id=context_id,
-                traffic_tag=traffic_tag,
-                allocate_addresses=allocate_addresses,
-                admin_state=admin_state,
-                tags=tags,
-                tenant=TEST_TENANT,
-                hyperbus_mode=hyperbus_mode,
-                init_state=init_state)
-            self.assert_called_with_def(api_call, expected_def)
-            self.assertIsNotNone(result)
+        for version in [nsx_constants.NSX_VERSION_3_2_3,
+                        nsx_constants.NSX_VERSION_4_1_0]:
+            with mock.patch.object(
+                self.policy_api.client, "url_post") as api_post, \
+                mock.patch.object(self.resourceApi, 'version', version):
+                result = self.resourceApi.create_or_overwrite(
+                    name, segment_id, port_id=port_id, description=description,
+                    address_bindings=address_bindings,
+                    attachment_type=attachment_type,
+                    vif_id=vif_id, app_id=app_id,
+                    context_id=context_id, traffic_tag=traffic_tag,
+                    allocate_addresses=allocate_addresses,
+                    hyperbus_mode=hyperbus_mode, admin_state=admin_state,
+                    tags=tags,
+                    tenant=TEST_TENANT,
+                    init_state=init_state)
+
+                expected_def = core_defs.SegmentPortDef(
+                    nsx_version=version,
+                    segment_id=segment_id,
+                    port_id=port_id,
+                    name=name,
+                    description=description,
+                    address_bindings=address_bindings,
+                    attachment_type=attachment_type,
+                    vif_id=vif_id,
+                    app_id=app_id,
+                    context_id=context_id,
+                    traffic_tag=traffic_tag,
+                    allocate_addresses=allocate_addresses,
+                    admin_state=admin_state,
+                    tags=tags,
+                    tenant=TEST_TENANT,
+                    hyperbus_mode=hyperbus_mode,
+                    init_state=init_state)
+
+                api_post.assert_called_once_with(
+                    expected_def.get_resource_path(),
+                    expected_def.get_obj_dict(), headers=None,
+                    expected_results=None, retry_confirm=False)
+                self.assertIsNotNone(result)
+
+        for version in [nsx_constants.NSX_VERSION_3_2_1,
+                        nsx_constants.NSX_VERSION_4_0_0]:
+            with mock.patch.object(
+                self.policy_api, "create_or_update") as api_call, \
+                mock.patch.object(self.resourceApi, 'version', version):
+                result = self.resourceApi.create_or_overwrite(
+                    name, segment_id, port_id=port_id, description=description,
+                    address_bindings=address_bindings,
+                    attachment_type=attachment_type,
+                    vif_id=vif_id, app_id=app_id,
+                    context_id=context_id, traffic_tag=traffic_tag,
+                    allocate_addresses=allocate_addresses,
+                    hyperbus_mode=hyperbus_mode, admin_state=admin_state,
+                    tags=tags,
+                    tenant=TEST_TENANT,
+                    init_state=init_state)
+
+                expected_def = core_defs.SegmentPortDef(
+                    nsx_version=version,
+                    segment_id=segment_id,
+                    port_id=port_id,
+                    name=name,
+                    description=description,
+                    address_bindings=address_bindings,
+                    attachment_type=attachment_type,
+                    vif_id=vif_id,
+                    app_id=app_id,
+                    context_id=context_id,
+                    traffic_tag=traffic_tag,
+                    allocate_addresses=allocate_addresses,
+                    admin_state=admin_state,
+                    tags=tags,
+                    tenant=TEST_TENANT,
+                    hyperbus_mode=hyperbus_mode,
+                    init_state=init_state)
+                self.assert_called_with_def(api_call, expected_def)
+                self.assertIsNotNone(result)
 
     def test_create_with_unsupported_attribute(self):
         name = 'test'
         description = 'desc'
         segment_id = "segment"
         address_bindings = []
         attachment_type = "CHILD"
```

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/policy/test_transaction.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_transaction.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_cert.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_cert.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_client.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_client.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_cluster.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_cluster.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_cluster_management.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_cluster_management.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_constants.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_constants.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_load_balancer.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_load_balancer.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_native_dhcp.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_native_dhcp.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_ns_group_manager.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_ns_group_manager.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_qos_switching_profile.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_qos_switching_profile.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_resources.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_resources.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_router.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_router.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_security.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_security.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_trust_management.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_trust_management.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_utils.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_utils.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/tests/unit/v3/test_vpn_ipsec.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_vpn_ipsec.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/__init__.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/client.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/client.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/client_cert.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/client_cert.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/cluster.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/cluster.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/cluster_management.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/cluster_management.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/config.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/config.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/constants.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/constants.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/core_resources.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/core_resources.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/debug_retry.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/debug_retry.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/exceptions.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/exceptions.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/lib.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/lib.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/load_balancer.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/load_balancer.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/native_dhcp.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/native_dhcp.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/ns_group_manager.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/ns_group_manager.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/nsx_constants.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/nsx_constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -160,16 +160,18 @@
 NSX_VERSION_2_4_0 = '2.4.0'
 NSX_VERSION_2_5_0 = '2.5.0'
 NSX_VERSION_3_0_0 = '3.0.0'
 NSX_VERSION_3_0_2 = '3.0.2'
 NSX_VERSION_3_1_0 = '3.1.0'
 NSX_VERSION_3_2_0 = '3.2.0'
 NSX_VERSION_3_2_1 = '3.2.1'
+NSX_VERSION_3_2_3 = '3.2.3'
 NSX_VERSION_4_0_0 = '4.0.0'
 NSX_VERSION_4_1_0 = '4.1.0'
+NSX_VERSION_4_1_1 = '4.1.1'
 
 # Features available depending on the NSX Manager backend version
 FEATURE_MAC_LEARNING = 'MAC Learning'
 FEATURE_DYNAMIC_CRITERIA = 'Dynamic criteria'
 FEATURE_EXCLUDE_PORT_BY_TAG = 'Exclude Port by Tag'
 FEATURE_ROUTER_FIREWALL = 'Router Firewall'
 FEATURE_LOAD_BALANCER = 'Load Balancer'
```

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/__init__.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/alb_auth_token_provider.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/alb_auth_token_provider.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/constants.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/constants.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/core_defs.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/core_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1518,14 +1518,24 @@
     @staticmethod
     def resource_type():
         return 'IpAddressPool'
 
     def path_defs(self):
         return (TenantDef,)
 
+    def get_obj_dict(self):
+        body = super(IpPoolDef, self).get_obj_dict()
+        self._set_attr_if_specified(body, 'ip_release_delay')
+        self._set_attr_if_supported(body, 'sync_realization')
+        return body
+
+    @property
+    def version_dependant_attr_map(self):
+        return {'sync_realization': nsx_constants.NSX_VERSION_4_1_1}
+
 
 class IpPoolAllocationDef(ResourceDef):
     '''Infra IpPoolAllocation'''
 
     @property
     def path_pattern(self):
         return IP_POOLS_PATH_PATTERN + "%s/ip-allocations/"
@@ -1586,25 +1596,29 @@
                 body, 'ip_block_id', body_attr='ip_block_path',
                 value=ip_block_path)
         # Attrs supported from NSX 3.0.0
         self._set_attr_if_supported(body, 'start_ip')
         # Attrs supported from NSX 4.1.0
         self._set_attrs_if_supported(body, ['subnet_size',
                                             'allocation_range'])
+        # Attrs supported from NSX 4.1.1
+        self._set_attr_if_supported(body, 'sync_realization')
         # Attribute "subnet size" is replacement for "size" attribute
         # thus, removing redundancy
         if 'subnet_size' in body:
             body.pop('size', None)
         return body
 
     @property
     def version_dependant_attr_map(self):
-        return {'start_ip': nsx_constants.NSX_VERSION_3_0_0,
-                'subnet_size': nsx_constants.NSX_VERSION_4_1_0,
-                'allocation_range': nsx_constants.NSX_VERSION_4_1_0}
+        return {
+            'start_ip': nsx_constants.NSX_VERSION_3_0_0,
+            'subnet_size': nsx_constants.NSX_VERSION_4_1_0,
+            'allocation_range': nsx_constants.NSX_VERSION_4_1_0,
+            'sync_realization': nsx_constants.NSX_VERSION_4_1_1}
 
 
 class IpPoolStaticSubnetDef(IpPoolSubnetDef):
     '''Infra IpPool static subnet'''
 
     @staticmethod
     def resource_type():
```

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/core_resources.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/core_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1132,15 +1132,15 @@
                                    tenant=tenant)
 
         self._create_or_store(tier1_def)
         return tier1_id
 
     def delete(self, tier1_id, tenant=constants.POLICY_INFRA_TENANT):
         tier1_def = self.entry_def(tier1_id=tier1_id, tenant=tenant)
-        self._delete_or_store(tier1_def)
+        self._delete_with_retry(tier1_def)
 
     def get(self, tier1_id, tenant=constants.POLICY_INFRA_TENANT,
             silent=False):
         tier1_def = self.entry_def(tier1_id=tier1_id, tenant=tenant)
         return self.policy_api.get(tier1_def, silent=silent)
 
     def get_path(self, tier1_id, tenant=constants.POLICY_INFRA_TENANT):
@@ -2544,14 +2544,18 @@
                                   admin_state=admin_state,
                                   init_state=init_state,
                                   extra_configs=extra_configs,
                                   tags=tags,
                                   tenant=tenant)
         if init_state == nsx_constants.INIT_STATE_RESTORE_VIF:
             if (version.LooseVersion(self.version) >=
+                version.LooseVersion(nsx_constants.NSX_VERSION_3_2_3) and
+                version.LooseVersion(self.version) <
+                version.LooseVersion(nsx_constants.NSX_VERSION_4_0_0) or
+                version.LooseVersion(self.version) >=
                 version.LooseVersion(nsx_constants.NSX_VERSION_4_1_0)):
                 path = port_def.get_resource_path()
                 body = port_def.get_obj_dict()
                 self.policy_api.client.create(path, body=body)
             else:
                 self._create_or_store(port_def)
         else:
@@ -3346,21 +3350,26 @@
     def entry_def(self):
         return core_defs.IpPoolDef
 
     def create_or_overwrite(self, name,
                             ip_pool_id=None,
                             description=IGNORE,
                             tags=IGNORE,
+                            ip_release_delay=IGNORE,
+                            sync_realization=False,
                             tenant=constants.POLICY_INFRA_TENANT):
 
         ip_pool_id = self._init_obj_uuid(ip_pool_id)
+
         ip_pool_def = self._init_def(ip_pool_id=ip_pool_id,
                                      name=name,
                                      description=description,
                                      tags=tags,
+                                     ip_release_delay=ip_release_delay,
+                                     sync_realization=sync_realization,
                                      tenant=tenant)
         self._create_or_store(ip_pool_def)
         return ip_pool_id
 
     def delete(self, ip_pool_id, tenant=constants.POLICY_INFRA_TENANT):
         ip_pool_def = self.entry_def(ip_pool_id=ip_pool_id,
                                      tenant=tenant)
@@ -3428,29 +3437,33 @@
         return self.policy_api.get(ip_allocation_def)
 
     def allocate_block_subnet(self, ip_pool_id, ip_block_id, size,
                               ip_subnet_id=None, auto_assign_gateway=IGNORE,
                               name=IGNORE, description=IGNORE, tags=IGNORE,
                               tenant=constants.POLICY_INFRA_TENANT,
                               start_ip=IGNORE, v6_allocation_range=IGNORE,
-                              force=False):
+                              force=False, sync_realization=False):
         ip_subnet_id = self._init_obj_uuid(ip_subnet_id)
+        # suppose all NSXT 4.1.0 build support sync_realization
+        # else we need to check if it supports sync_realization
+        # it's just a temp patch
         args = self._get_user_args(
             ip_pool_id=ip_pool_id,
             ip_block_id=ip_block_id,
             ip_subnet_id=ip_subnet_id,
             size=size,
             auto_assign_gateway=auto_assign_gateway,
             name=name,
             description=description,
             tags=tags,
             tenant=tenant,
             start_ip=start_ip,
             subnet_size=str(size),
-            allocation_range=v6_allocation_range)
+            allocation_range=v6_allocation_range,
+            sync_realization=sync_realization)
 
         ip_subnet_def = core_defs.IpPoolBlockSubnetDef(
             nsx_version=self.version, **args)
         self._create_or_store(ip_subnet_def, force=force)
 
     def release_block_subnet(self, ip_pool_id, ip_subnet_id,
                              tenant=constants.POLICY_INFRA_TENANT,
```

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/ipsec_vpn_defs.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/ipsec_vpn_defs.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/ipsec_vpn_resources.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/ipsec_vpn_resources.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/lb_defs.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/lb_defs.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/lb_resources.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/lb_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -497,15 +497,15 @@
         self._create_or_store(lb_pool_def)
         return lb_pool_id
 
     def delete(self, lb_pool_id,
                tenant=constants.POLICY_INFRA_TENANT):
         lb_pool_def = self.entry_def(
             lb_pool_id=lb_pool_id, tenant=tenant)
-        self._delete_with_retry(lb_pool_def)
+        self._delete_or_store(lb_pool_def)
 
     def get(self, lb_pool_id, tenant=constants.POLICY_INFRA_TENANT,
             silent=False):
         lb_pool_def = self.entry_def(
             lb_pool_id=lb_pool_id, tenant=tenant)
         return self.policy_api.get(lb_pool_def, silent=silent)
 
@@ -825,15 +825,15 @@
         self._create_or_store(lbvs_def)
         return virtual_server_id
 
     def delete(self, virtual_server_id,
                tenant=constants.POLICY_INFRA_TENANT):
         lbvs_def = self.entry_def(
             virtual_server_id=virtual_server_id, tenant=tenant)
-        self._delete_with_retry(lbvs_def)
+        self._delete_or_store(lbvs_def)
 
     def get(self, virtual_server_id,
             tenant=constants.POLICY_INFRA_TENANT, silent=False):
         lbvs_def = self.entry_def(
             virtual_server_id=virtual_server_id, tenant=tenant)
         return self.policy_api.get(lbvs_def, silent=silent)
```

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/transaction.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/transaction.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/policy/utils.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/utils.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/resources.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/resources.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/router.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/router.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/security.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/security.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/token_provider.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/token_provider.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/trust_management.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/trust_management.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/utils.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/utils.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/v3/vpn_ipsec.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/vpn_ipsec.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib/version.py` & `vmware-nsxlib-19.3.0/vmware_nsxlib/version.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib.egg-info/PKG-INFO` & `vmware-nsxlib-19.3.0/vmware_nsxlib.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 1.1
 Name: vmware-nsxlib
-Version: 19.2.4
-Summary: A common library that interfaces with NSX
+Version: 19.3.0
+Summary: A common library that interfaces with VMware NSX
 Home-page: https://opendev.org/x/vmware-nsxlib
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
-Description: =============
+Description: TESt:wq
+        
+        
+        =============
         vmware-nsxlib
         =============
         
         * Free software: Apache license
         * Source: https://opendev.org/x/vmware-nsxlib
         
         Features
@@ -25,9 +28,7 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vmware-nsxlib-19.2.4/vmware_nsxlib.egg-info/SOURCES.txt` & `vmware-nsxlib-19.3.0/vmware_nsxlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

