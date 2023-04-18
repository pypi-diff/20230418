# Comparing `tmp/cdktf-cdktf-provider-dns-3.0.1.tar.gz` & `tmp/cdktf-cdktf-provider-dns-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-dns-3.0.1.tar", last modified: Thu Feb  9 14:06:15 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-dns-4.0.0.tar", last modified: Tue Apr 18 20:37:26 2023, max compression
```

## Comparing `cdktf-cdktf-provider-dns-3.0.1.tar` & `cdktf-cdktf-provider-dns-4.0.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.541317 cdktf-cdktf-provider-dns-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-02-09 14:06:15.541317 cdktf-cdktf-provider-dns-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 14:06:15.541317 cdktf-cdktf-provider-dns-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.537317 cdktf-cdktf-provider-dns-3.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.537317 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.537317 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    88197 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/_jsii/provider-dns@3.0.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.537317 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/a_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    23067 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/a_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.541317 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/aaaa_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/aaaa_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.541317 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/cname_record/
--rw-r--r--   0 runner    (1001) docker     (123)    22544 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/cname_record/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.541317 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_a_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_a_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.541317 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_aaaa_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    17314 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_aaaa_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.541317 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_cname_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    17317 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_cname_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.541317 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_mx_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    26162 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_mx_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.541317 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_ns_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    17274 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_ns_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.541317 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_ptr_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_ptr_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.541317 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_srv_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    26576 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_srv_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.541317 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_txt_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    17457 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_txt_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.541317 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/mx_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    37225 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/mx_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.541317 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/ns_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    22936 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/ns_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.541317 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.541317 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/ptr_record/
--rw-r--r--   0 runner    (1001) docker     (123)    22628 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/ptr_record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.541317 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/srv_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    40305 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/srv_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.541317 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/txt_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    22963 2023-02-09 14:06:00.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/txt_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:06:15.537317 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-02-09 14:06:15.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-02-09 14:06:15.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 14:06:15.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-09 14:06:15.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-09 14:06:15.000000 cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.957090 cdktf-cdktf-provider-dns-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-18 20:37:26.953090 cdktf-cdktf-provider-dns-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:37:26.957090 cdktf-cdktf-provider-dns-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.949090 cdktf-cdktf-provider-dns-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.953090 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.953090 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   316414 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/_jsii/provider-dns@4.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.953090 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/a_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    24858 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/a_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.953090 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/aaaa_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    24999 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/aaaa_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.953090 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/cname_record/
+-rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/cname_record/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.953090 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_a_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_a_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.953090 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_aaaa_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    15083 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_aaaa_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.953090 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_cname_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_cname_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.953090 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_mx_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    23949 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_mx_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.953090 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_ns_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    15055 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_ns_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.953090 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_ptr_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_ptr_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.953090 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_srv_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    24360 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_srv_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.953090 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_txt_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    15232 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_txt_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.953090 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/mx_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    36579 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/mx_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.953090 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/ns_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    21884 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/ns_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.953090 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.953090 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/ptr_record/
+-rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/ptr_record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.953090 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/srv_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    39920 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/srv_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.953090 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/txt_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    21911 2023-04-18 20:37:15.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/txt_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:26.953090 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-18 20:37:26.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-18 20:37:26.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:37:26.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:37:26.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 20:37:26.000000 cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-dns-3.0.1/LICENSE` & `cdktf-cdktf-provider-dns-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-3.0.1/PKG-INFO` & `cdktf-cdktf-provider-dns-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-dns
-Version: 3.0.1
+Version: 4.0.0
 Summary: Prebuilt dns Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-dns.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-dns.git
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
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-dns-go`](https://github.com/cdktf/cdktf-provider-dns-go) package.
 
 `go get github.com/cdktf/cdktf-provider-dns-go/dns`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-dns).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform dns Provider version 1:1. In fact, it always tracks `latest` of `~> 3.2` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-dns-3.0.1/README.md` & `cdktf-cdktf-provider-dns-4.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-dns-go`](https://github.com/cdktf/cdktf-provider-dns-go) package.
 
 `go get github.com/cdktf/cdktf-provider-dns-go/dns`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-dns).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform dns Provider version 1:1. In fact, it always tracks `latest` of `~> 3.2` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-dns-3.0.1/setup.py` & `cdktf-cdktf-provider-dns-4.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-dns",
-    "version": "3.0.1",
+    "version": "4.0.0",
     "description": "Prebuilt dns Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-dns.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -39,37 +39,38 @@
         "cdktf_cdktf_provider_dns.provider",
         "cdktf_cdktf_provider_dns.ptr_record",
         "cdktf_cdktf_provider_dns.srv_record_set",
         "cdktf_cdktf_provider_dns.txt_record_set"
     ],
     "package_data": {
         "cdktf_cdktf_provider_dns._jsii": [
-            "provider-dns@3.0.1.jsii.tgz"
+            "provider-dns@4.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_dns": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdktf>=0.15.0, <0.16.0",
+        "cdktf>=0.16.0, <0.17.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.74.0, <2.0.0",
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

### Comparing `cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/__init__.py` & `cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-dns-go`](https://github.com/cdktf/cdktf-provider-dns-go) package.
 
 `go get github.com/cdktf/cdktf-provider-dns-go/dns`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-dns).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform dns Provider version 1:1. In fact, it always tracks `latest` of `~> 3.2` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/a_record_set/__init__.py` & `cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/txt_record_set/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# `dns_a_record_set`
+# `dns_txt_record_set`
 
-Refer to the Terraform Registory for docs: [`dns_a_record_set`](https://www.terraform.io/docs/providers/dns/r/a_record_set).
+Refer to the Terraform Registory for docs: [`dns_txt_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/txt_record_set).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -17,80 +17,73 @@
 
 from .._jsii import *
 
 import cdktf as _cdktf_9a9027ec
 import constructs as _constructs_77d1e7e8
 
 
-class ARecordSet(
+class TxtRecordSet(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-dns.aRecordSet.ARecordSet",
+    jsii_type="@cdktf/provider-dns.txtRecordSet.TxtRecordSet",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dns/r/a_record_set dns_a_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/txt_record_set dns_txt_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
-        id_: builtins.str,
+        id: builtins.str,
         *,
-        addresses: typing.Sequence[builtins.str],
+        txt: typing.Sequence[builtins.str],
         zone: builtins.str,
-        id: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
         ttl: typing.Optional[jsii.Number] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dns/r/a_record_set dns_a_record_set} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/txt_record_set dns_txt_record_set} Resource.
 
         :param scope: The scope in which to define this construct.
-        :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param addresses: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/a_record_set#addresses ARecordSet#addresses}.
-        :param zone: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/a_record_set#zone ARecordSet#zone}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/a_record_set#id ARecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/a_record_set#name ARecordSet#name}.
-        :param ttl: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/a_record_set#ttl ARecordSet#ttl}.
+        :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
+        :param txt: The text records this record set will be set to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/txt_record_set#txt TxtRecordSet#txt}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/txt_record_set#zone TxtRecordSet#zone}
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/txt_record_set#name TxtRecordSet#name}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/txt_record_set#ttl TxtRecordSet#ttl}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__56309216a4932d58e61b48abbe057388f9f67f265044ec885a18b7d609453396)
+            type_hints = typing.get_type_hints(_typecheckingstub__a51e4003b74cde103c0047a30c686a2c5cc17d4ee313d7059a1382df0018c934)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
-        config = ARecordSetConfig(
-            addresses=addresses,
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        config = TxtRecordSetConfig(
+            txt=txt,
             zone=zone,
-            id=id,
             name=name,
             ttl=ttl,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
         )
 
-        jsii.create(self.__class__, self, [scope, id_, config])
-
-    @jsii.member(jsii_name="resetId")
-    def reset_id(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetId", []))
+        jsii.create(self.__class__, self, [scope, id, config])
 
     @jsii.member(jsii_name="resetName")
     def reset_name(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetName", []))
 
     @jsii.member(jsii_name="resetTtl")
     def reset_ttl(self) -> None:
@@ -102,166 +95,150 @@
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
-    @jsii.member(jsii_name="addressesInput")
-    def addresses_input(self) -> typing.Optional[typing.List[builtins.str]]:
-        return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "addressesInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="idInput")
-    def id_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
+    @jsii.member(jsii_name="id")
+    def id(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "id"))
 
     @builtins.property
     @jsii.member(jsii_name="nameInput")
     def name_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "nameInput"))
 
     @builtins.property
     @jsii.member(jsii_name="ttlInput")
     def ttl_input(self) -> typing.Optional[jsii.Number]:
         return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "ttlInput"))
 
     @builtins.property
+    @jsii.member(jsii_name="txtInput")
+    def txt_input(self) -> typing.Optional[typing.List[builtins.str]]:
+        return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "txtInput"))
+
+    @builtins.property
     @jsii.member(jsii_name="zoneInput")
     def zone_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "zoneInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="addresses")
-    def addresses(self) -> typing.List[builtins.str]:
-        return typing.cast(typing.List[builtins.str], jsii.get(self, "addresses"))
-
-    @addresses.setter
-    def addresses(self, value: typing.List[builtins.str]) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e5b8c95116689fc96412dd6b6649d2ad69c784bb68f50aa570b4fb7b18d1e219)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "addresses", value)
-
-    @builtins.property
-    @jsii.member(jsii_name="id")
-    def id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "id"))
-
-    @id.setter
-    def id(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__12e33e8e68bcbe8ed279da1d3458df2cd27e0f22d6a3d8c4cea7e7ce92e04706)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "id", value)
-
-    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__58a1e2aa02a1572a7ad576339b6bd1f9fa6378bd0cb3185c14c01290573e52eb)
+            type_hints = typing.get_type_hints(_typecheckingstub__ae6a03f672c9c35a2b3d592a782166274ba5483a5a784b659d4ed5938f4e2ee0)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
     @builtins.property
     @jsii.member(jsii_name="ttl")
     def ttl(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "ttl"))
 
     @ttl.setter
     def ttl(self, value: jsii.Number) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__bce949f9faf94d2947f660e79005c86116a6c8c11f0387502874040832565921)
+            type_hints = typing.get_type_hints(_typecheckingstub__d2398a91b02be48a801a3aa711874ccc4d44c72e74591d884f15b92d788f7b78)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ttl", value)
 
     @builtins.property
+    @jsii.member(jsii_name="txt")
+    def txt(self) -> typing.List[builtins.str]:
+        return typing.cast(typing.List[builtins.str], jsii.get(self, "txt"))
+
+    @txt.setter
+    def txt(self, value: typing.List[builtins.str]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__49378e0e2763440a0134210dcb932295719151ebbccdf593cc0a86ba0dba5908)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "txt", value)
+
+    @builtins.property
     @jsii.member(jsii_name="zone")
     def zone(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "zone"))
 
     @zone.setter
     def zone(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b4cca80a49f5ba81b2deb9eb060d0d4bd07176dcbabc69f114b2cc8fe77e9466)
+            type_hints = typing.get_type_hints(_typecheckingstub__853cb1fa1788f9020175e03e4bfbda61223cf282852f9f417d1bb98965d45519)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zone", value)
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-dns.aRecordSet.ARecordSetConfig",
+    jsii_type="@cdktf/provider-dns.txtRecordSet.TxtRecordSetConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
-        "addresses": "addresses",
+        "txt": "txt",
         "zone": "zone",
-        "id": "id",
         "name": "name",
         "ttl": "ttl",
     },
 )
-class ARecordSetConfig(_cdktf_9a9027ec.TerraformMetaArguments):
+class TxtRecordSetConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
-        addresses: typing.Sequence[builtins.str],
+        txt: typing.Sequence[builtins.str],
         zone: builtins.str,
-        id: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
         ttl: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param addresses: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/a_record_set#addresses ARecordSet#addresses}.
-        :param zone: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/a_record_set#zone ARecordSet#zone}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/a_record_set#id ARecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/a_record_set#name ARecordSet#name}.
-        :param ttl: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/a_record_set#ttl ARecordSet#ttl}.
+        :param txt: The text records this record set will be set to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/txt_record_set#txt TxtRecordSet#txt}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/txt_record_set#zone TxtRecordSet#zone}
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/txt_record_set#name TxtRecordSet#name}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/txt_record_set#ttl TxtRecordSet#ttl}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__15cff60de25b8724a41dea37bad793e750c7efcacadb8bc6470dbb98cec4342f)
+            type_hints = typing.get_type_hints(_typecheckingstub__d17e9bfe665b6b04383b6279df11401d9213158e0dd640fa26830d2ae7466fbd)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
-            check_type(argname="argument addresses", value=addresses, expected_type=type_hints["addresses"])
+            check_type(argname="argument txt", value=txt, expected_type=type_hints["txt"])
             check_type(argname="argument zone", value=zone, expected_type=type_hints["zone"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument ttl", value=ttl, expected_type=type_hints["ttl"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
-            "addresses": addresses,
+            "txt": txt,
             "zone": zone,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
         if depends_on is not None:
@@ -270,16 +247,14 @@
             self._values["for_each"] = for_each
         if lifecycle is not None:
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
-        if id is not None:
-            self._values["id"] = id
         if name is not None:
             self._values["name"] = name
         if ttl is not None:
             self._values["ttl"] = ttl
 
     @builtins.property
     def connection(
@@ -288,20 +263,22 @@
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
@@ -340,128 +317,124 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
-    def addresses(self) -> typing.List[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/a_record_set#addresses ARecordSet#addresses}.'''
-        result = self._values.get("addresses")
-        assert result is not None, "Required property 'addresses' is missing"
+    def txt(self) -> typing.List[builtins.str]:
+        '''The text records this record set will be set to.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/txt_record_set#txt TxtRecordSet#txt}
+        '''
+        result = self._values.get("txt")
+        assert result is not None, "Required property 'txt' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def zone(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/a_record_set#zone ARecordSet#zone}.'''
+        '''DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/txt_record_set#zone TxtRecordSet#zone}
+        '''
         result = self._values.get("zone")
         assert result is not None, "Required property 'zone' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/a_record_set#id ARecordSet#id}.
+    def name(self) -> typing.Optional[builtins.str]:
+        '''The name of the record set.
 
-        Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
-        If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        '''
-        result = self._values.get("id")
-        return typing.cast(typing.Optional[builtins.str], result)
+        The ``zone`` argument will be appended to this value to create the full record path.
 
-    @builtins.property
-    def name(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/a_record_set#name ARecordSet#name}.'''
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/txt_record_set#name TxtRecordSet#name}
+        '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ttl(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/a_record_set#ttl ARecordSet#ttl}.'''
+        '''The TTL of the record set. Defaults to ``3600``.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/txt_record_set#ttl TxtRecordSet#ttl}
+        '''
         result = self._values.get("ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "ARecordSetConfig(%s)" % ", ".join(
+        return "TxtRecordSetConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
-    "ARecordSet",
-    "ARecordSetConfig",
+    "TxtRecordSet",
+    "TxtRecordSetConfig",
 ]
 
 publication.publish()
 
-def _typecheckingstub__56309216a4932d58e61b48abbe057388f9f67f265044ec885a18b7d609453396(
+def _typecheckingstub__a51e4003b74cde103c0047a30c686a2c5cc17d4ee313d7059a1382df0018c934(
     scope: _constructs_77d1e7e8.Construct,
-    id_: builtins.str,
+    id: builtins.str,
     *,
-    addresses: typing.Sequence[builtins.str],
+    txt: typing.Sequence[builtins.str],
     zone: builtins.str,
-    id: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     ttl: typing.Optional[jsii.Number] = None,
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
 
-def _typecheckingstub__e5b8c95116689fc96412dd6b6649d2ad69c784bb68f50aa570b4fb7b18d1e219(
-    value: typing.List[builtins.str],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__12e33e8e68bcbe8ed279da1d3458df2cd27e0f22d6a3d8c4cea7e7ce92e04706(
+def _typecheckingstub__ae6a03f672c9c35a2b3d592a782166274ba5483a5a784b659d4ed5938f4e2ee0(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__58a1e2aa02a1572a7ad576339b6bd1f9fa6378bd0cb3185c14c01290573e52eb(
-    value: builtins.str,
+def _typecheckingstub__d2398a91b02be48a801a3aa711874ccc4d44c72e74591d884f15b92d788f7b78(
+    value: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__bce949f9faf94d2947f660e79005c86116a6c8c11f0387502874040832565921(
-    value: jsii.Number,
+def _typecheckingstub__49378e0e2763440a0134210dcb932295719151ebbccdf593cc0a86ba0dba5908(
+    value: typing.List[builtins.str],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__b4cca80a49f5ba81b2deb9eb060d0d4bd07176dcbabc69f114b2cc8fe77e9466(
+def _typecheckingstub__853cb1fa1788f9020175e03e4bfbda61223cf282852f9f417d1bb98965d45519(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__15cff60de25b8724a41dea37bad793e750c7efcacadb8bc6470dbb98cec4342f(
+def _typecheckingstub__d17e9bfe665b6b04383b6279df11401d9213158e0dd640fa26830d2ae7466fbd(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
-    addresses: typing.Sequence[builtins.str],
+    txt: typing.Sequence[builtins.str],
     zone: builtins.str,
-    id: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     ttl: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/aaaa_record_set/__init__.py` & `cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/a_record_set/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# `dns_aaaa_record_set`
+# `dns_a_record_set`
 
-Refer to the Terraform Registory for docs: [`dns_aaaa_record_set`](https://www.terraform.io/docs/providers/dns/r/aaaa_record_set).
+Refer to the Terraform Registory for docs: [`dns_a_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/a_record_set).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -17,61 +17,61 @@
 
 from .._jsii import *
 
 import cdktf as _cdktf_9a9027ec
 import constructs as _constructs_77d1e7e8
 
 
-class AaaaRecordSet(
+class ARecordSet(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-dns.aaaaRecordSet.AaaaRecordSet",
+    jsii_type="@cdktf/provider-dns.aRecordSet.ARecordSet",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dns/r/aaaa_record_set dns_aaaa_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/a_record_set dns_a_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         addresses: typing.Sequence[builtins.str],
         zone: builtins.str,
         id: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
         ttl: typing.Optional[jsii.Number] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dns/r/aaaa_record_set dns_aaaa_record_set} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/a_record_set dns_a_record_set} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param addresses: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/aaaa_record_set#addresses AaaaRecordSet#addresses}.
-        :param zone: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/aaaa_record_set#zone AaaaRecordSet#zone}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/aaaa_record_set#id AaaaRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/aaaa_record_set#name AaaaRecordSet#name}.
-        :param ttl: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/aaaa_record_set#ttl AaaaRecordSet#ttl}.
+        :param addresses: The IPv4 addresses this record set will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/a_record_set#addresses ARecordSet#addresses}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/a_record_set#zone ARecordSet#zone}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/a_record_set#id ARecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/a_record_set#name ARecordSet#name}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/a_record_set#ttl ARecordSet#ttl}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f95a77e839b028e1ec4b902d403800b8b2681cb3c7db96ab08cc03ebda128881)
+            type_hints = typing.get_type_hints(_typecheckingstub__56309216a4932d58e61b48abbe057388f9f67f265044ec885a18b7d609453396)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
-        config = AaaaRecordSetConfig(
+        config = ARecordSetConfig(
             addresses=addresses,
             zone=zone,
             id=id,
             name=name,
             ttl=ttl,
             connection=connection,
             count=count,
@@ -134,69 +134,69 @@
     @jsii.member(jsii_name="addresses")
     def addresses(self) -> typing.List[builtins.str]:
         return typing.cast(typing.List[builtins.str], jsii.get(self, "addresses"))
 
     @addresses.setter
     def addresses(self, value: typing.List[builtins.str]) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c3e59b87eff2656f0de40996521f03d742ff8265b83569ec1fd4b8a6056ad4c0)
+            type_hints = typing.get_type_hints(_typecheckingstub__e5b8c95116689fc96412dd6b6649d2ad69c784bb68f50aa570b4fb7b18d1e219)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "addresses", value)
 
     @builtins.property
     @jsii.member(jsii_name="id")
     def id(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "id"))
 
     @id.setter
     def id(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c7fecdfc9eeccee6c52b39b5837a4e230fe597c52ba820d55aff7f8ac1b7b580)
+            type_hints = typing.get_type_hints(_typecheckingstub__12e33e8e68bcbe8ed279da1d3458df2cd27e0f22d6a3d8c4cea7e7ce92e04706)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "id", value)
 
     @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__969155f00d50bb4a786f2c8022e08a5844dc4a210099603a0c7efbed716c6639)
+            type_hints = typing.get_type_hints(_typecheckingstub__58a1e2aa02a1572a7ad576339b6bd1f9fa6378bd0cb3185c14c01290573e52eb)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
     @builtins.property
     @jsii.member(jsii_name="ttl")
     def ttl(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "ttl"))
 
     @ttl.setter
     def ttl(self, value: jsii.Number) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__2ce4b77d7d883f7cc36d31ff4f98f93b768f356d6bfb3d47277b1b80fdb2f192)
+            type_hints = typing.get_type_hints(_typecheckingstub__bce949f9faf94d2947f660e79005c86116a6c8c11f0387502874040832565921)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ttl", value)
 
     @builtins.property
     @jsii.member(jsii_name="zone")
     def zone(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "zone"))
 
     @zone.setter
     def zone(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__76ee0b7f55beb4e085448a399443bf4cb34ccba38c7001a5de482dcd9df78fcb)
+            type_hints = typing.get_type_hints(_typecheckingstub__b4cca80a49f5ba81b2deb9eb060d0d4bd07176dcbabc69f114b2cc8fe77e9466)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zone", value)
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-dns.aaaaRecordSet.AaaaRecordSetConfig",
+    jsii_type="@cdktf/provider-dns.aRecordSet.ARecordSetConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
@@ -205,20 +205,20 @@
         "addresses": "addresses",
         "zone": "zone",
         "id": "id",
         "name": "name",
         "ttl": "ttl",
     },
 )
-class AaaaRecordSetConfig(_cdktf_9a9027ec.TerraformMetaArguments):
+class ARecordSetConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         addresses: typing.Sequence[builtins.str],
         zone: builtins.str,
@@ -230,24 +230,24 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param addresses: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/aaaa_record_set#addresses AaaaRecordSet#addresses}.
-        :param zone: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/aaaa_record_set#zone AaaaRecordSet#zone}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/aaaa_record_set#id AaaaRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/aaaa_record_set#name AaaaRecordSet#name}.
-        :param ttl: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/aaaa_record_set#ttl AaaaRecordSet#ttl}.
+        :param addresses: The IPv4 addresses this record set will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/a_record_set#addresses ARecordSet#addresses}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/a_record_set#zone ARecordSet#zone}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/a_record_set#id ARecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/a_record_set#name ARecordSet#name}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/a_record_set#ttl ARecordSet#ttl}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7b02504a909c79d4df8654eda870cd6b0da805b48d848ba6bc32daaa4249e3a3)
+            type_hints = typing.get_type_hints(_typecheckingstub__15cff60de25b8724a41dea37bad793e750c7efcacadb8bc6470dbb98cec4342f)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
@@ -288,20 +288,22 @@
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
@@ -341,121 +343,135 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def addresses(self) -> typing.List[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/aaaa_record_set#addresses AaaaRecordSet#addresses}.'''
+        '''The IPv4 addresses this record set will point to.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/a_record_set#addresses ARecordSet#addresses}
+        '''
         result = self._values.get("addresses")
         assert result is not None, "Required property 'addresses' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def zone(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/aaaa_record_set#zone AaaaRecordSet#zone}.'''
+        '''DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/a_record_set#zone ARecordSet#zone}
+        '''
         result = self._values.get("zone")
         assert result is not None, "Required property 'zone' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/aaaa_record_set#id AaaaRecordSet#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/a_record_set#id ARecordSet#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/aaaa_record_set#name AaaaRecordSet#name}.'''
+        '''The name of the record set.
+
+        The ``zone`` argument will be appended to this value to create the full record path.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/a_record_set#name ARecordSet#name}
+        '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ttl(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/aaaa_record_set#ttl AaaaRecordSet#ttl}.'''
+        '''The TTL of the record set. Defaults to ``3600``.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/a_record_set#ttl ARecordSet#ttl}
+        '''
         result = self._values.get("ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "AaaaRecordSetConfig(%s)" % ", ".join(
+        return "ARecordSetConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
-    "AaaaRecordSet",
-    "AaaaRecordSetConfig",
+    "ARecordSet",
+    "ARecordSetConfig",
 ]
 
 publication.publish()
 
-def _typecheckingstub__f95a77e839b028e1ec4b902d403800b8b2681cb3c7db96ab08cc03ebda128881(
+def _typecheckingstub__56309216a4932d58e61b48abbe057388f9f67f265044ec885a18b7d609453396(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     addresses: typing.Sequence[builtins.str],
     zone: builtins.str,
     id: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     ttl: typing.Optional[jsii.Number] = None,
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
 
-def _typecheckingstub__c3e59b87eff2656f0de40996521f03d742ff8265b83569ec1fd4b8a6056ad4c0(
+def _typecheckingstub__e5b8c95116689fc96412dd6b6649d2ad69c784bb68f50aa570b4fb7b18d1e219(
     value: typing.List[builtins.str],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__c7fecdfc9eeccee6c52b39b5837a4e230fe597c52ba820d55aff7f8ac1b7b580(
+def _typecheckingstub__12e33e8e68bcbe8ed279da1d3458df2cd27e0f22d6a3d8c4cea7e7ce92e04706(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__969155f00d50bb4a786f2c8022e08a5844dc4a210099603a0c7efbed716c6639(
+def _typecheckingstub__58a1e2aa02a1572a7ad576339b6bd1f9fa6378bd0cb3185c14c01290573e52eb(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__2ce4b77d7d883f7cc36d31ff4f98f93b768f356d6bfb3d47277b1b80fdb2f192(
+def _typecheckingstub__bce949f9faf94d2947f660e79005c86116a6c8c11f0387502874040832565921(
     value: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__76ee0b7f55beb4e085448a399443bf4cb34ccba38c7001a5de482dcd9df78fcb(
+def _typecheckingstub__b4cca80a49f5ba81b2deb9eb060d0d4bd07176dcbabc69f114b2cc8fe77e9466(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__7b02504a909c79d4df8654eda870cd6b0da805b48d848ba6bc32daaa4249e3a3(
+def _typecheckingstub__15cff60de25b8724a41dea37bad793e750c7efcacadb8bc6470dbb98cec4342f(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     addresses: typing.Sequence[builtins.str],
     zone: builtins.str,
```

### Comparing `cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/cname_record/__init__.py` & `cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/cname_record/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `dns_cname_record`
 
-Refer to the Terraform Registory for docs: [`dns_cname_record`](https://www.terraform.io/docs/providers/dns/r/cname_record).
+Refer to the Terraform Registory for docs: [`dns_cname_record`](https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/cname_record).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,75 +22,68 @@
 
 
 class CnameRecord(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.cnameRecord.CnameRecord",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dns/r/cname_record dns_cname_record}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/cname_record dns_cname_record}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
-        id_: builtins.str,
+        id: builtins.str,
         *,
         cname: builtins.str,
         name: builtins.str,
         zone: builtins.str,
-        id: typing.Optional[builtins.str] = None,
         ttl: typing.Optional[jsii.Number] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dns/r/cname_record dns_cname_record} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/cname_record dns_cname_record} Resource.
 
         :param scope: The scope in which to define this construct.
-        :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cname: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/cname_record#cname CnameRecord#cname}.
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/cname_record#name CnameRecord#name}.
-        :param zone: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/cname_record#zone CnameRecord#zone}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/cname_record#id CnameRecord#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param ttl: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/cname_record#ttl CnameRecord#ttl}.
+        :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
+        :param cname: The canonical name this record will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/cname_record#cname CnameRecord#cname}
+        :param name: The name of the record. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/cname_record#name CnameRecord#name}
+        :param zone: DNS zone the record belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/cname_record#zone CnameRecord#zone}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/cname_record#ttl CnameRecord#ttl}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d150e95dadfb18e11b6fd53a8b64e6a7d5d15e4edb8126e9a55d2b9d1afbd52f)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = CnameRecordConfig(
             cname=cname,
             name=name,
             zone=zone,
-            id=id,
             ttl=ttl,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
         )
 
-        jsii.create(self.__class__, self, [scope, id_, config])
-
-    @jsii.member(jsii_name="resetId")
-    def reset_id(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetId", []))
+        jsii.create(self.__class__, self, [scope, id, config])
 
     @jsii.member(jsii_name="resetTtl")
     def reset_ttl(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetTtl", []))
 
     @jsii.member(jsii_name="synthesizeAttributes")
     def _synthesize_attributes(self) -> typing.Mapping[builtins.str, typing.Any]:
@@ -98,24 +91,24 @@
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
+    @jsii.member(jsii_name="id")
+    def id(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "id"))
+
+    @builtins.property
     @jsii.member(jsii_name="cnameInput")
     def cname_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "cnameInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="idInput")
-    def id_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
-
-    @builtins.property
     @jsii.member(jsii_name="nameInput")
     def name_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "nameInput"))
 
     @builtins.property
     @jsii.member(jsii_name="ttlInput")
     def ttl_input(self) -> typing.Optional[jsii.Number]:
@@ -135,26 +128,14 @@
     def cname(self, value: builtins.str) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5cc27d7a064cf5b4efdf9f23f9df74e237942138159edc2ed31e4443db47f586)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cname", value)
 
     @builtins.property
-    @jsii.member(jsii_name="id")
-    def id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "id"))
-
-    @id.setter
-    def id(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__da9ff513c58042944a1ad599e84f4a17c3df0770af4c56a12fb96e2cbbeee0f6)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "id", value)
-
-    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: builtins.str) -> None:
         if __debug__:
@@ -197,48 +178,45 @@
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
         "cname": "cname",
         "name": "name",
         "zone": "zone",
-        "id": "id",
         "ttl": "ttl",
     },
 )
 class CnameRecordConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         cname: builtins.str,
         name: builtins.str,
         zone: builtins.str,
-        id: typing.Optional[builtins.str] = None,
         ttl: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cname: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/cname_record#cname CnameRecord#cname}.
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/cname_record#name CnameRecord#name}.
-        :param zone: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/cname_record#zone CnameRecord#zone}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/cname_record#id CnameRecord#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param ttl: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/cname_record#ttl CnameRecord#ttl}.
+        :param cname: The canonical name this record will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/cname_record#cname CnameRecord#cname}
+        :param name: The name of the record. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/cname_record#name CnameRecord#name}
+        :param zone: DNS zone the record belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/cname_record#zone CnameRecord#zone}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/cname_record#ttl CnameRecord#ttl}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__85ab3d3a662907f40b18ce9ac321aedec0c7f81fc9368400c9f94ee960050a8a)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -246,15 +224,14 @@
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
             check_type(argname="argument cname", value=cname, expected_type=type_hints["cname"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument zone", value=zone, expected_type=type_hints["zone"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument ttl", value=ttl, expected_type=type_hints["ttl"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "cname": cname,
             "name": name,
             "zone": zone,
         }
         if connection is not None:
@@ -267,36 +244,36 @@
             self._values["for_each"] = for_each
         if lifecycle is not None:
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
-        if id is not None:
-            self._values["id"] = id
         if ttl is not None:
             self._values["ttl"] = ttl
 
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
@@ -336,46 +313,50 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cname(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/cname_record#cname CnameRecord#cname}.'''
+        '''The canonical name this record will point to.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/cname_record#cname CnameRecord#cname}
+        '''
         result = self._values.get("cname")
         assert result is not None, "Required property 'cname' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/cname_record#name CnameRecord#name}.'''
+        '''The name of the record.
+
+        The ``zone`` argument will be appended to this value to create the full record path.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/cname_record#name CnameRecord#name}
+        '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def zone(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/cname_record#zone CnameRecord#zone}.'''
+        '''DNS zone the record belongs to. It must be an FQDN, that is, include the trailing dot.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/cname_record#zone CnameRecord#zone}
+        '''
         result = self._values.get("zone")
         assert result is not None, "Required property 'zone' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/cname_record#id CnameRecord#id}.
+    def ttl(self) -> typing.Optional[jsii.Number]:
+        '''The TTL of the record set. Defaults to ``3600``.
 
-        Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
-        If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/cname_record#ttl CnameRecord#ttl}
         '''
-        result = self._values.get("id")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    @builtins.property
-    def ttl(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/cname_record#ttl CnameRecord#ttl}.'''
         result = self._values.get("ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -392,23 +373,22 @@
     "CnameRecordConfig",
 ]
 
 publication.publish()
 
 def _typecheckingstub__d150e95dadfb18e11b6fd53a8b64e6a7d5d15e4edb8126e9a55d2b9d1afbd52f(
     scope: _constructs_77d1e7e8.Construct,
-    id_: builtins.str,
+    id: builtins.str,
     *,
     cname: builtins.str,
     name: builtins.str,
     zone: builtins.str,
-    id: typing.Optional[builtins.str] = None,
     ttl: typing.Optional[jsii.Number] = None,
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
@@ -416,20 +396,14 @@
 
 def _typecheckingstub__5cc27d7a064cf5b4efdf9f23f9df74e237942138159edc2ed31e4443db47f586(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__da9ff513c58042944a1ad599e84f4a17c3df0770af4c56a12fb96e2cbbeee0f6(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
 def _typecheckingstub__3a9f51b803e003e161bc2b89444744e689478618cefb14241915b35901b97ea7(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__b4810bce4a4eb8592ed5ba1ef584f87939a9d42213aac7ed03695f00a190b4af(
@@ -443,21 +417,20 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__85ab3d3a662907f40b18ce9ac321aedec0c7f81fc9368400c9f94ee960050a8a(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     cname: builtins.str,
     name: builtins.str,
     zone: builtins.str,
-    id: typing.Optional[builtins.str] = None,
     ttl: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_a_record_set/__init__.py` & `cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_cname_record_set/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# `data_dns_a_record_set`
+# `data_dns_cname_record_set`
 
-Refer to the Terraform Registory for docs: [`data_dns_a_record_set`](https://www.terraform.io/docs/providers/dns/d/a_record_set).
+Refer to the Terraform Registory for docs: [`data_dns_cname_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/cname_record_set).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -17,174 +17,151 @@
 
 from .._jsii import *
 
 import cdktf as _cdktf_9a9027ec
 import constructs as _constructs_77d1e7e8
 
 
-class DataDnsARecordSet(
+class DataDnsCnameRecordSet(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-dns.dataDnsARecordSet.DataDnsARecordSet",
+    jsii_type="@cdktf/provider-dns.dataDnsCnameRecordSet.DataDnsCnameRecordSet",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dns/d/a_record_set dns_a_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/cname_record_set dns_cname_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
-        id_: builtins.str,
+        id: builtins.str,
         *,
         host: builtins.str,
-        id: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dns/d/a_record_set dns_a_record_set} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/cname_record_set dns_cname_record_set} Data Source.
 
         :param scope: The scope in which to define this construct.
-        :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param host: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/a_record_set#host DataDnsARecordSet#host}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/a_record_set#id DataDnsARecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
+        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/cname_record_set#host DataDnsCnameRecordSet#host}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__631408f625d64bf3db9be59419947b4dc4cf3a6a5990bf875ff1ce7302fc0533)
+            type_hints = typing.get_type_hints(_typecheckingstub__da9253a2dfad571733a41afc5003bff2268ccdb1634a7e31482e60f491d7d9ec)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
-        config = DataDnsARecordSetConfig(
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        config = DataDnsCnameRecordSetConfig(
             host=host,
-            id=id,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
         )
 
-        jsii.create(self.__class__, self, [scope, id_, config])
-
-    @jsii.member(jsii_name="resetId")
-    def reset_id(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetId", []))
+        jsii.create(self.__class__, self, [scope, id, config])
 
     @jsii.member(jsii_name="synthesizeAttributes")
     def _synthesize_attributes(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "synthesizeAttributes", []))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
-    @jsii.member(jsii_name="addrs")
-    def addrs(self) -> typing.List[builtins.str]:
-        return typing.cast(typing.List[builtins.str], jsii.get(self, "addrs"))
+    @jsii.member(jsii_name="cname")
+    def cname(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "cname"))
+
+    @builtins.property
+    @jsii.member(jsii_name="id")
+    def id(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "id"))
 
     @builtins.property
     @jsii.member(jsii_name="hostInput")
     def host_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "hostInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="idInput")
-    def id_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
-
-    @builtins.property
     @jsii.member(jsii_name="host")
     def host(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "host"))
 
     @host.setter
     def host(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__611e0f44e1562ef59d44b555fbad36c2a1c2c50a1db5ed8d19ffe895e684406a)
+            type_hints = typing.get_type_hints(_typecheckingstub__b3c085eb03f77a7649e8c2316d0fbbbae41f4bb6c1a463744edbaa84ccd8ae81)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "host", value)
 
-    @builtins.property
-    @jsii.member(jsii_name="id")
-    def id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "id"))
-
-    @id.setter
-    def id(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__9ea121013066562e4731737dec803d9c40891354c715a5341151fc504fe06e5e)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "id", value)
-
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-dns.dataDnsARecordSet.DataDnsARecordSetConfig",
+    jsii_type="@cdktf/provider-dns.dataDnsCnameRecordSet.DataDnsCnameRecordSetConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
         "host": "host",
-        "id": "id",
     },
 )
-class DataDnsARecordSetConfig(_cdktf_9a9027ec.TerraformMetaArguments):
+class DataDnsCnameRecordSetConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         host: builtins.str,
-        id: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param host: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/a_record_set#host DataDnsARecordSet#host}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/a_record_set#id DataDnsARecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/cname_record_set#host DataDnsCnameRecordSet#host}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4392563f6d6ca59db53a3f1e6c445df6f633bba1c3bced497176d8a70eb282ed)
+            type_hints = typing.get_type_hints(_typecheckingstub__3d1a77e5261d74d2f0b88c8a59df0d2ff76c2bdc029e41e1cfdd2cabeb567e46)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
             check_type(argname="argument host", value=host, expected_type=type_hints["host"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "host": host,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
@@ -194,34 +171,34 @@
             self._values["for_each"] = for_each
         if lifecycle is not None:
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
-        if id is not None:
-            self._values["id"] = id
 
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
@@ -261,84 +238,69 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def host(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/a_record_set#host DataDnsARecordSet#host}.'''
+        '''Host to look up.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/cname_record_set#host DataDnsCnameRecordSet#host}
+        '''
         result = self._values.get("host")
         assert result is not None, "Required property 'host' is missing"
         return typing.cast(builtins.str, result)
 
-    @builtins.property
-    def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/a_record_set#id DataDnsARecordSet#id}.
-
-        Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
-        If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        '''
-        result = self._values.get("id")
-        return typing.cast(typing.Optional[builtins.str], result)
-
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataDnsARecordSetConfig(%s)" % ", ".join(
+        return "DataDnsCnameRecordSetConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
-    "DataDnsARecordSet",
-    "DataDnsARecordSetConfig",
+    "DataDnsCnameRecordSet",
+    "DataDnsCnameRecordSetConfig",
 ]
 
 publication.publish()
 
-def _typecheckingstub__631408f625d64bf3db9be59419947b4dc4cf3a6a5990bf875ff1ce7302fc0533(
+def _typecheckingstub__da9253a2dfad571733a41afc5003bff2268ccdb1634a7e31482e60f491d7d9ec(
     scope: _constructs_77d1e7e8.Construct,
-    id_: builtins.str,
+    id: builtins.str,
     *,
     host: builtins.str,
-    id: typing.Optional[builtins.str] = None,
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
 
-def _typecheckingstub__611e0f44e1562ef59d44b555fbad36c2a1c2c50a1db5ed8d19ffe895e684406a(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__9ea121013066562e4731737dec803d9c40891354c715a5341151fc504fe06e5e(
+def _typecheckingstub__b3c085eb03f77a7649e8c2316d0fbbbae41f4bb6c1a463744edbaa84ccd8ae81(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__4392563f6d6ca59db53a3f1e6c445df6f633bba1c3bced497176d8a70eb282ed(
+def _typecheckingstub__3d1a77e5261d74d2f0b88c8a59df0d2ff76c2bdc029e41e1cfdd2cabeb567e46(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     host: builtins.str,
-    id: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_aaaa_record_set/__init__.py` & `cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_ptr_record_set/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# `data_dns_aaaa_record_set`
+# `data_dns_ptr_record_set`
 
-Refer to the Terraform Registory for docs: [`data_dns_aaaa_record_set`](https://www.terraform.io/docs/providers/dns/d/aaaa_record_set).
+Refer to the Terraform Registory for docs: [`data_dns_ptr_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/ptr_record_set).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -17,176 +17,153 @@
 
 from .._jsii import *
 
 import cdktf as _cdktf_9a9027ec
 import constructs as _constructs_77d1e7e8
 
 
-class DataDnsAaaaRecordSet(
+class DataDnsPtrRecordSet(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-dns.dataDnsAaaaRecordSet.DataDnsAaaaRecordSet",
+    jsii_type="@cdktf/provider-dns.dataDnsPtrRecordSet.DataDnsPtrRecordSet",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dns/d/aaaa_record_set dns_aaaa_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/ptr_record_set dns_ptr_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
-        id_: builtins.str,
+        id: builtins.str,
         *,
-        host: builtins.str,
-        id: typing.Optional[builtins.str] = None,
+        ip_address: builtins.str,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dns/d/aaaa_record_set dns_aaaa_record_set} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/ptr_record_set dns_ptr_record_set} Data Source.
 
         :param scope: The scope in which to define this construct.
-        :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param host: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/aaaa_record_set#host DataDnsAaaaRecordSet#host}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/aaaa_record_set#id DataDnsAaaaRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
+        :param ip_address: IP address to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/ptr_record_set#ip_address DataDnsPtrRecordSet#ip_address}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7c5b6c9236742afbf3551e98db9f779338baacbc53bc50e3b91145a96a8bb0f2)
+            type_hints = typing.get_type_hints(_typecheckingstub__fda41c0faffb5e35e54a3ebc013b5cc6d3805ee4f3a1eeb1e50f268ab9f5d9bc)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
-        config = DataDnsAaaaRecordSetConfig(
-            host=host,
-            id=id,
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        config = DataDnsPtrRecordSetConfig(
+            ip_address=ip_address,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
         )
 
-        jsii.create(self.__class__, self, [scope, id_, config])
-
-    @jsii.member(jsii_name="resetId")
-    def reset_id(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetId", []))
+        jsii.create(self.__class__, self, [scope, id, config])
 
     @jsii.member(jsii_name="synthesizeAttributes")
     def _synthesize_attributes(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "synthesizeAttributes", []))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
-    @jsii.member(jsii_name="addrs")
-    def addrs(self) -> typing.List[builtins.str]:
-        return typing.cast(typing.List[builtins.str], jsii.get(self, "addrs"))
-
-    @builtins.property
-    @jsii.member(jsii_name="hostInput")
-    def host_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "hostInput"))
+    @jsii.member(jsii_name="id")
+    def id(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "id"))
 
     @builtins.property
-    @jsii.member(jsii_name="idInput")
-    def id_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
+    @jsii.member(jsii_name="ptr")
+    def ptr(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "ptr"))
 
     @builtins.property
-    @jsii.member(jsii_name="host")
-    def host(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "host"))
-
-    @host.setter
-    def host(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d2c01f0d1f97e5a5cf351e400fcb19bf53b7ad147feee0699ed05080f89616e2)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "host", value)
+    @jsii.member(jsii_name="ipAddressInput")
+    def ip_address_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "ipAddressInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="id")
-    def id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "id"))
+    @jsii.member(jsii_name="ipAddress")
+    def ip_address(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "ipAddress"))
 
-    @id.setter
-    def id(self, value: builtins.str) -> None:
+    @ip_address.setter
+    def ip_address(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8b25fcb806e3239a0ae4f3a0674d2572d45d8ff40175e4232d983924f4a5972a)
+            type_hints = typing.get_type_hints(_typecheckingstub__c64a8750ea2f9542ec3363181593443c5cd79849a6d6de816341d419d1b638ec)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "id", value)
+        jsii.set(self, "ipAddress", value)
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-dns.dataDnsAaaaRecordSet.DataDnsAaaaRecordSetConfig",
+    jsii_type="@cdktf/provider-dns.dataDnsPtrRecordSet.DataDnsPtrRecordSetConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
-        "host": "host",
-        "id": "id",
+        "ip_address": "ipAddress",
     },
 )
-class DataDnsAaaaRecordSetConfig(_cdktf_9a9027ec.TerraformMetaArguments):
+class DataDnsPtrRecordSetConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
-        host: builtins.str,
-        id: typing.Optional[builtins.str] = None,
+        ip_address: builtins.str,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param host: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/aaaa_record_set#host DataDnsAaaaRecordSet#host}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/aaaa_record_set#id DataDnsAaaaRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param ip_address: IP address to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/ptr_record_set#ip_address DataDnsPtrRecordSet#ip_address}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__908caa216afdc6eb58e4534363fab765aca58abf2556163688267bf57a2baf0a)
+            type_hints = typing.get_type_hints(_typecheckingstub__fcf1fd55b23b7e629d56697ab8a11be420526958500797f4bdec98583deded00)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
-            check_type(argname="argument host", value=host, expected_type=type_hints["host"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument ip_address", value=ip_address, expected_type=type_hints["ip_address"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
-            "host": host,
+            "ip_address": ip_address,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
         if depends_on is not None:
             self._values["depends_on"] = depends_on
@@ -194,34 +171,34 @@
             self._values["for_each"] = for_each
         if lifecycle is not None:
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
-        if id is not None:
-            self._values["id"] = id
 
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
@@ -260,85 +237,70 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
-    def host(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/aaaa_record_set#host DataDnsAaaaRecordSet#host}.'''
-        result = self._values.get("host")
-        assert result is not None, "Required property 'host' is missing"
-        return typing.cast(builtins.str, result)
-
-    @builtins.property
-    def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/aaaa_record_set#id DataDnsAaaaRecordSet#id}.
+    def ip_address(self) -> builtins.str:
+        '''IP address to look up.
 
-        Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
-        If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/ptr_record_set#ip_address DataDnsPtrRecordSet#ip_address}
         '''
-        result = self._values.get("id")
-        return typing.cast(typing.Optional[builtins.str], result)
+        result = self._values.get("ip_address")
+        assert result is not None, "Required property 'ip_address' is missing"
+        return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataDnsAaaaRecordSetConfig(%s)" % ", ".join(
+        return "DataDnsPtrRecordSetConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
-    "DataDnsAaaaRecordSet",
-    "DataDnsAaaaRecordSetConfig",
+    "DataDnsPtrRecordSet",
+    "DataDnsPtrRecordSetConfig",
 ]
 
 publication.publish()
 
-def _typecheckingstub__7c5b6c9236742afbf3551e98db9f779338baacbc53bc50e3b91145a96a8bb0f2(
+def _typecheckingstub__fda41c0faffb5e35e54a3ebc013b5cc6d3805ee4f3a1eeb1e50f268ab9f5d9bc(
     scope: _constructs_77d1e7e8.Construct,
-    id_: builtins.str,
+    id: builtins.str,
     *,
-    host: builtins.str,
-    id: typing.Optional[builtins.str] = None,
+    ip_address: builtins.str,
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
 
-def _typecheckingstub__d2c01f0d1f97e5a5cf351e400fcb19bf53b7ad147feee0699ed05080f89616e2(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__8b25fcb806e3239a0ae4f3a0674d2572d45d8ff40175e4232d983924f4a5972a(
+def _typecheckingstub__c64a8750ea2f9542ec3363181593443c5cd79849a6d6de816341d419d1b638ec(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__908caa216afdc6eb58e4534363fab765aca58abf2556163688267bf57a2baf0a(
+def _typecheckingstub__fcf1fd55b23b7e629d56697ab8a11be420526958500797f4bdec98583deded00(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
-    host: builtins.str,
-    id: typing.Optional[builtins.str] = None,
+    ip_address: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_cname_record_set/__init__.py` & `cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/ns_record_set/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# `data_dns_cname_record_set`
+# `dns_ns_record_set`
 
-Refer to the Terraform Registory for docs: [`data_dns_cname_record_set`](https://www.terraform.io/docs/providers/dns/d/cname_record_set).
+Refer to the Terraform Registory for docs: [`dns_ns_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ns_record_set).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -17,176 +17,226 @@
 
 from .._jsii import *
 
 import cdktf as _cdktf_9a9027ec
 import constructs as _constructs_77d1e7e8
 
 
-class DataDnsCnameRecordSet(
-    _cdktf_9a9027ec.TerraformDataSource,
+class NsRecordSet(
+    _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-dns.dataDnsCnameRecordSet.DataDnsCnameRecordSet",
+    jsii_type="@cdktf/provider-dns.nsRecordSet.NsRecordSet",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dns/d/cname_record_set dns_cname_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ns_record_set dns_ns_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
-        id_: builtins.str,
+        id: builtins.str,
         *,
-        host: builtins.str,
-        id: typing.Optional[builtins.str] = None,
+        name: builtins.str,
+        nameservers: typing.Sequence[builtins.str],
+        zone: builtins.str,
+        ttl: typing.Optional[jsii.Number] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dns/d/cname_record_set dns_cname_record_set} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ns_record_set dns_ns_record_set} Resource.
 
         :param scope: The scope in which to define this construct.
-        :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param host: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/cname_record_set#host DataDnsCnameRecordSet#host}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/cname_record_set#id DataDnsCnameRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ns_record_set#name NsRecordSet#name}
+        :param nameservers: The nameservers this record set will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ns_record_set#nameservers NsRecordSet#nameservers}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ns_record_set#zone NsRecordSet#zone}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ns_record_set#ttl NsRecordSet#ttl}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__da9253a2dfad571733a41afc5003bff2268ccdb1634a7e31482e60f491d7d9ec)
+            type_hints = typing.get_type_hints(_typecheckingstub__509f309cc2ac8c5a7e7e52d7cc690641f019a292fc46e109472e09179e6721b0)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
-        config = DataDnsCnameRecordSetConfig(
-            host=host,
-            id=id,
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        config = NsRecordSetConfig(
+            name=name,
+            nameservers=nameservers,
+            zone=zone,
+            ttl=ttl,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
         )
 
-        jsii.create(self.__class__, self, [scope, id_, config])
+        jsii.create(self.__class__, self, [scope, id, config])
 
-    @jsii.member(jsii_name="resetId")
-    def reset_id(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetId", []))
+    @jsii.member(jsii_name="resetTtl")
+    def reset_ttl(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetTtl", []))
 
     @jsii.member(jsii_name="synthesizeAttributes")
     def _synthesize_attributes(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "synthesizeAttributes", []))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
-    @jsii.member(jsii_name="cname")
-    def cname(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "cname"))
+    @jsii.member(jsii_name="id")
+    def id(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "id"))
+
+    @builtins.property
+    @jsii.member(jsii_name="nameInput")
+    def name_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "nameInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="hostInput")
-    def host_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "hostInput"))
+    @jsii.member(jsii_name="nameserversInput")
+    def nameservers_input(self) -> typing.Optional[typing.List[builtins.str]]:
+        return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "nameserversInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="idInput")
-    def id_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
+    @jsii.member(jsii_name="ttlInput")
+    def ttl_input(self) -> typing.Optional[jsii.Number]:
+        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "ttlInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="host")
-    def host(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "host"))
+    @jsii.member(jsii_name="zoneInput")
+    def zone_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "zoneInput"))
 
-    @host.setter
-    def host(self, value: builtins.str) -> None:
+    @builtins.property
+    @jsii.member(jsii_name="name")
+    def name(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "name"))
+
+    @name.setter
+    def name(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b3c085eb03f77a7649e8c2316d0fbbbae41f4bb6c1a463744edbaa84ccd8ae81)
+            type_hints = typing.get_type_hints(_typecheckingstub__31f585b9bd18e4dac0600b5da866ef4caeebe89a886776bddbe5956f5b256076)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "host", value)
+        jsii.set(self, "name", value)
 
     @builtins.property
-    @jsii.member(jsii_name="id")
-    def id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "id"))
+    @jsii.member(jsii_name="nameservers")
+    def nameservers(self) -> typing.List[builtins.str]:
+        return typing.cast(typing.List[builtins.str], jsii.get(self, "nameservers"))
 
-    @id.setter
-    def id(self, value: builtins.str) -> None:
+    @nameservers.setter
+    def nameservers(self, value: typing.List[builtins.str]) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__1a7b04d329a75b07daa2ad4c28880f4aeeb756ca0f269d2fa4c1ab82e1839bf0)
+            type_hints = typing.get_type_hints(_typecheckingstub__eda6be7152f2c47d8c6e1b2468138cf373970f2d271619e5c0641b5071411f84)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "id", value)
+        jsii.set(self, "nameservers", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="ttl")
+    def ttl(self) -> jsii.Number:
+        return typing.cast(jsii.Number, jsii.get(self, "ttl"))
+
+    @ttl.setter
+    def ttl(self, value: jsii.Number) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__9dfb7611269b3993e4ed448bf64d9c468f39dd3cc7b5e721b685e67eae5ef214)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "ttl", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="zone")
+    def zone(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "zone"))
+
+    @zone.setter
+    def zone(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__a63d9123b8105fe544190f89f83ac56cd44bfc410b7f4dff0c505daf9774c5e6)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "zone", value)
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-dns.dataDnsCnameRecordSet.DataDnsCnameRecordSetConfig",
+    jsii_type="@cdktf/provider-dns.nsRecordSet.NsRecordSetConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
-        "host": "host",
-        "id": "id",
+        "name": "name",
+        "nameservers": "nameservers",
+        "zone": "zone",
+        "ttl": "ttl",
     },
 )
-class DataDnsCnameRecordSetConfig(_cdktf_9a9027ec.TerraformMetaArguments):
+class NsRecordSetConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
-        host: builtins.str,
-        id: typing.Optional[builtins.str] = None,
+        name: builtins.str,
+        nameservers: typing.Sequence[builtins.str],
+        zone: builtins.str,
+        ttl: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param host: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/cname_record_set#host DataDnsCnameRecordSet#host}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/cname_record_set#id DataDnsCnameRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ns_record_set#name NsRecordSet#name}
+        :param nameservers: The nameservers this record set will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ns_record_set#nameservers NsRecordSet#nameservers}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ns_record_set#zone NsRecordSet#zone}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ns_record_set#ttl NsRecordSet#ttl}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__3d1a77e5261d74d2f0b88c8a59df0d2ff76c2bdc029e41e1cfdd2cabeb567e46)
+            type_hints = typing.get_type_hints(_typecheckingstub__f6a1231a3a6a7ab541c206eb7f9e24e0c86f26ee0a5c23e6f66eb0bb66fe6cd3)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
-            check_type(argname="argument host", value=host, expected_type=type_hints["host"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument nameservers", value=nameservers, expected_type=type_hints["nameservers"])
+            check_type(argname="argument zone", value=zone, expected_type=type_hints["zone"])
+            check_type(argname="argument ttl", value=ttl, expected_type=type_hints["ttl"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
-            "host": host,
+            "name": name,
+            "nameservers": nameservers,
+            "zone": zone,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
         if depends_on is not None:
             self._values["depends_on"] = depends_on
@@ -194,34 +244,36 @@
             self._values["for_each"] = for_each
         if lifecycle is not None:
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
-        if id is not None:
-            self._values["id"] = id
+        if ttl is not None:
+            self._values["ttl"] = ttl
 
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
@@ -260,85 +312,125 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
-    def host(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/cname_record_set#host DataDnsCnameRecordSet#host}.'''
-        result = self._values.get("host")
-        assert result is not None, "Required property 'host' is missing"
+    def name(self) -> builtins.str:
+        '''The name of the record set.
+
+        The ``zone`` argument will be appended to this value to create the full record path.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ns_record_set#name NsRecordSet#name}
+        '''
+        result = self._values.get("name")
+        assert result is not None, "Required property 'name' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def nameservers(self) -> typing.List[builtins.str]:
+        '''The nameservers this record set will point to.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ns_record_set#nameservers NsRecordSet#nameservers}
+        '''
+        result = self._values.get("nameservers")
+        assert result is not None, "Required property 'nameservers' is missing"
+        return typing.cast(typing.List[builtins.str], result)
+
+    @builtins.property
+    def zone(self) -> builtins.str:
+        '''DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ns_record_set#zone NsRecordSet#zone}
+        '''
+        result = self._values.get("zone")
+        assert result is not None, "Required property 'zone' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/cname_record_set#id DataDnsCnameRecordSet#id}.
+    def ttl(self) -> typing.Optional[jsii.Number]:
+        '''The TTL of the record set. Defaults to ``3600``.
 
-        Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
-        If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ns_record_set#ttl NsRecordSet#ttl}
         '''
-        result = self._values.get("id")
-        return typing.cast(typing.Optional[builtins.str], result)
+        result = self._values.get("ttl")
+        return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataDnsCnameRecordSetConfig(%s)" % ", ".join(
+        return "NsRecordSetConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
-    "DataDnsCnameRecordSet",
-    "DataDnsCnameRecordSetConfig",
+    "NsRecordSet",
+    "NsRecordSetConfig",
 ]
 
 publication.publish()
 
-def _typecheckingstub__da9253a2dfad571733a41afc5003bff2268ccdb1634a7e31482e60f491d7d9ec(
+def _typecheckingstub__509f309cc2ac8c5a7e7e52d7cc690641f019a292fc46e109472e09179e6721b0(
     scope: _constructs_77d1e7e8.Construct,
-    id_: builtins.str,
+    id: builtins.str,
     *,
-    host: builtins.str,
-    id: typing.Optional[builtins.str] = None,
+    name: builtins.str,
+    nameservers: typing.Sequence[builtins.str],
+    zone: builtins.str,
+    ttl: typing.Optional[jsii.Number] = None,
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
 
-def _typecheckingstub__b3c085eb03f77a7649e8c2316d0fbbbae41f4bb6c1a463744edbaa84ccd8ae81(
+def _typecheckingstub__31f585b9bd18e4dac0600b5da866ef4caeebe89a886776bddbe5956f5b256076(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__1a7b04d329a75b07daa2ad4c28880f4aeeb756ca0f269d2fa4c1ab82e1839bf0(
+def _typecheckingstub__eda6be7152f2c47d8c6e1b2468138cf373970f2d271619e5c0641b5071411f84(
+    value: typing.List[builtins.str],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__9dfb7611269b3993e4ed448bf64d9c468f39dd3cc7b5e721b685e67eae5ef214(
+    value: jsii.Number,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__a63d9123b8105fe544190f89f83ac56cd44bfc410b7f4dff0c505daf9774c5e6(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__3d1a77e5261d74d2f0b88c8a59df0d2ff76c2bdc029e41e1cfdd2cabeb567e46(
+def _typecheckingstub__f6a1231a3a6a7ab541c206eb7f9e24e0c86f26ee0a5c23e6f66eb0bb66fe6cd3(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
-    host: builtins.str,
-    id: typing.Optional[builtins.str] = None,
+    name: builtins.str,
+    nameservers: typing.Sequence[builtins.str],
+    zone: builtins.str,
+    ttl: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_mx_record_set/__init__.py` & `cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_mx_record_set/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_dns_mx_record_set`
 
-Refer to the Terraform Registory for docs: [`data_dns_mx_record_set`](https://www.terraform.io/docs/providers/dns/d/mx_record_set).
+Refer to the Terraform Registory for docs: [`data_dns_mx_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/mx_record_set).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,169 +22,146 @@
 
 
 class DataDnsMxRecordSet(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.dataDnsMxRecordSet.DataDnsMxRecordSet",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dns/d/mx_record_set dns_mx_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/mx_record_set dns_mx_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
-        id_: builtins.str,
+        id: builtins.str,
         *,
         domain: builtins.str,
-        id: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dns/d/mx_record_set dns_mx_record_set} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/mx_record_set dns_mx_record_set} Data Source.
 
         :param scope: The scope in which to define this construct.
-        :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param domain: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/mx_record_set#domain DataDnsMxRecordSet#domain}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/mx_record_set#id DataDnsMxRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
+        :param domain: Domain to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/mx_record_set#domain DataDnsMxRecordSet#domain}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__257fe484da590469942f26adbc57258b7b2b329a329638494bf14593c7ed4e9e)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = DataDnsMxRecordSetConfig(
             domain=domain,
-            id=id,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
         )
 
-        jsii.create(self.__class__, self, [scope, id_, config])
-
-    @jsii.member(jsii_name="resetId")
-    def reset_id(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetId", []))
+        jsii.create(self.__class__, self, [scope, id, config])
 
     @jsii.member(jsii_name="synthesizeAttributes")
     def _synthesize_attributes(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "synthesizeAttributes", []))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
+    @jsii.member(jsii_name="id")
+    def id(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "id"))
+
+    @builtins.property
     @jsii.member(jsii_name="mx")
     def mx(self) -> "DataDnsMxRecordSetMxList":
         return typing.cast("DataDnsMxRecordSetMxList", jsii.get(self, "mx"))
 
     @builtins.property
     @jsii.member(jsii_name="domainInput")
     def domain_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "domainInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="idInput")
-    def id_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
-
-    @builtins.property
     @jsii.member(jsii_name="domain")
     def domain(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "domain"))
 
     @domain.setter
     def domain(self, value: builtins.str) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1e70dcc0f7287152b7ec8d79499cbe0e6181bc6335e6e88de9f6f45172db1d47)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "domain", value)
 
-    @builtins.property
-    @jsii.member(jsii_name="id")
-    def id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "id"))
-
-    @id.setter
-    def id(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__1c958e38da90864c8c26f541b56ea4bbdc6f811b08c8a82ae30c41cb309b5e6c)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "id", value)
-
 
 @jsii.data_type(
     jsii_type="@cdktf/provider-dns.dataDnsMxRecordSet.DataDnsMxRecordSetConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
         "domain": "domain",
-        "id": "id",
     },
 )
 class DataDnsMxRecordSetConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         domain: builtins.str,
-        id: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param domain: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/mx_record_set#domain DataDnsMxRecordSet#domain}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/mx_record_set#id DataDnsMxRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param domain: Domain to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/mx_record_set#domain DataDnsMxRecordSet#domain}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__112b631474f3656d4096e3a10b250e7363827fdc3f044c40f9d5c97caf0f0ec4)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
             check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "domain": domain,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
@@ -194,34 +171,34 @@
             self._values["for_each"] = for_each
         if lifecycle is not None:
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
-        if id is not None:
-            self._values["id"] = id
 
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
@@ -261,29 +238,22 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def domain(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/mx_record_set#domain DataDnsMxRecordSet#domain}.'''
+        '''Domain to look up.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/mx_record_set#domain DataDnsMxRecordSet#domain}
+        '''
         result = self._values.get("domain")
         assert result is not None, "Required property 'domain' is missing"
         return typing.cast(builtins.str, result)
 
-    @builtins.property
-    def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/mx_record_set#id DataDnsMxRecordSet#id}.
-
-        Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
-        If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        '''
-        result = self._values.get("id")
-        return typing.cast(typing.Optional[builtins.str], result)
-
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -443,20 +413,19 @@
     "DataDnsMxRecordSetMxOutputReference",
 ]
 
 publication.publish()
 
 def _typecheckingstub__257fe484da590469942f26adbc57258b7b2b329a329638494bf14593c7ed4e9e(
     scope: _constructs_77d1e7e8.Construct,
-    id_: builtins.str,
+    id: builtins.str,
     *,
     domain: builtins.str,
-    id: typing.Optional[builtins.str] = None,
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
@@ -464,31 +433,24 @@
 
 def _typecheckingstub__1e70dcc0f7287152b7ec8d79499cbe0e6181bc6335e6e88de9f6f45172db1d47(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__1c958e38da90864c8c26f541b56ea4bbdc6f811b08c8a82ae30c41cb309b5e6c(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
 def _typecheckingstub__112b631474f3656d4096e3a10b250e7363827fdc3f044c40f9d5c97caf0f0ec4(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     domain: builtins.str,
-    id: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__869f6c881fa368f4c76089b957608b8f73c77b259d825dbb077940f786728f7d(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
```

### Comparing `cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_ns_record_set/__init__.py` & `cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_ns_record_set/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_dns_ns_record_set`
 
-Refer to the Terraform Registory for docs: [`data_dns_ns_record_set`](https://www.terraform.io/docs/providers/dns/d/ns_record_set).
+Refer to the Terraform Registory for docs: [`data_dns_ns_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/ns_record_set).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,169 +22,146 @@
 
 
 class DataDnsNsRecordSet(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.dataDnsNsRecordSet.DataDnsNsRecordSet",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dns/d/ns_record_set dns_ns_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/ns_record_set dns_ns_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
-        id_: builtins.str,
+        id: builtins.str,
         *,
         host: builtins.str,
-        id: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dns/d/ns_record_set dns_ns_record_set} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/ns_record_set dns_ns_record_set} Data Source.
 
         :param scope: The scope in which to define this construct.
-        :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param host: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/ns_record_set#host DataDnsNsRecordSet#host}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/ns_record_set#id DataDnsNsRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
+        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/ns_record_set#host DataDnsNsRecordSet#host}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__258bb366eda1e34d0ddde3fcc62f652a8ff8e6a5712d15ff2246f1bd312d6b44)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = DataDnsNsRecordSetConfig(
             host=host,
-            id=id,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
         )
 
-        jsii.create(self.__class__, self, [scope, id_, config])
-
-    @jsii.member(jsii_name="resetId")
-    def reset_id(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetId", []))
+        jsii.create(self.__class__, self, [scope, id, config])
 
     @jsii.member(jsii_name="synthesizeAttributes")
     def _synthesize_attributes(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "synthesizeAttributes", []))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
+    @jsii.member(jsii_name="id")
+    def id(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "id"))
+
+    @builtins.property
     @jsii.member(jsii_name="nameservers")
     def nameservers(self) -> typing.List[builtins.str]:
         return typing.cast(typing.List[builtins.str], jsii.get(self, "nameservers"))
 
     @builtins.property
     @jsii.member(jsii_name="hostInput")
     def host_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "hostInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="idInput")
-    def id_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
-
-    @builtins.property
     @jsii.member(jsii_name="host")
     def host(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "host"))
 
     @host.setter
     def host(self, value: builtins.str) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6131c6510bedd973e083181f50860f0aa2f001d8150824387770dca865656adc)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "host", value)
 
-    @builtins.property
-    @jsii.member(jsii_name="id")
-    def id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "id"))
-
-    @id.setter
-    def id(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c5605ab1d8ca79c4ef14b5cb15094b36bde8081990ea02ae50b27acb2345fedb)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "id", value)
-
 
 @jsii.data_type(
     jsii_type="@cdktf/provider-dns.dataDnsNsRecordSet.DataDnsNsRecordSetConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
         "host": "host",
-        "id": "id",
     },
 )
 class DataDnsNsRecordSetConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         host: builtins.str,
-        id: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param host: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/ns_record_set#host DataDnsNsRecordSet#host}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/ns_record_set#id DataDnsNsRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/ns_record_set#host DataDnsNsRecordSet#host}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__83f15275c0d7535be3797ec071f20244f1d9cf271ac24f43dc5fe373457644e3)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
             check_type(argname="argument host", value=host, expected_type=type_hints["host"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "host": host,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
@@ -194,34 +171,34 @@
             self._values["for_each"] = for_each
         if lifecycle is not None:
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
-        if id is not None:
-            self._values["id"] = id
 
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
@@ -261,29 +238,22 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def host(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/ns_record_set#host DataDnsNsRecordSet#host}.'''
+        '''Host to look up.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/ns_record_set#host DataDnsNsRecordSet#host}
+        '''
         result = self._values.get("host")
         assert result is not None, "Required property 'host' is missing"
         return typing.cast(builtins.str, result)
 
-    @builtins.property
-    def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/ns_record_set#id DataDnsNsRecordSet#id}.
-
-        Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
-        If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        '''
-        result = self._values.get("id")
-        return typing.cast(typing.Optional[builtins.str], result)
-
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -297,20 +267,19 @@
     "DataDnsNsRecordSetConfig",
 ]
 
 publication.publish()
 
 def _typecheckingstub__258bb366eda1e34d0ddde3fcc62f652a8ff8e6a5712d15ff2246f1bd312d6b44(
     scope: _constructs_77d1e7e8.Construct,
-    id_: builtins.str,
+    id: builtins.str,
     *,
     host: builtins.str,
-    id: typing.Optional[builtins.str] = None,
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
@@ -318,27 +287,20 @@
 
 def _typecheckingstub__6131c6510bedd973e083181f50860f0aa2f001d8150824387770dca865656adc(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__c5605ab1d8ca79c4ef14b5cb15094b36bde8081990ea02ae50b27acb2345fedb(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
 def _typecheckingstub__83f15275c0d7535be3797ec071f20244f1d9cf271ac24f43dc5fe373457644e3(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     host: builtins.str,
-    id: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_ptr_record_set/__init__.py` & `cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_aaaa_record_set/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# `data_dns_ptr_record_set`
+# `data_dns_aaaa_record_set`
 
-Refer to the Terraform Registory for docs: [`data_dns_ptr_record_set`](https://www.terraform.io/docs/providers/dns/d/ptr_record_set).
+Refer to the Terraform Registory for docs: [`data_dns_aaaa_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/aaaa_record_set).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -17,176 +17,153 @@
 
 from .._jsii import *
 
 import cdktf as _cdktf_9a9027ec
 import constructs as _constructs_77d1e7e8
 
 
-class DataDnsPtrRecordSet(
+class DataDnsAaaaRecordSet(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-dns.dataDnsPtrRecordSet.DataDnsPtrRecordSet",
+    jsii_type="@cdktf/provider-dns.dataDnsAaaaRecordSet.DataDnsAaaaRecordSet",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dns/d/ptr_record_set dns_ptr_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/aaaa_record_set dns_aaaa_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
-        id_: builtins.str,
+        id: builtins.str,
         *,
-        ip_address: builtins.str,
-        id: typing.Optional[builtins.str] = None,
+        host: builtins.str,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dns/d/ptr_record_set dns_ptr_record_set} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/aaaa_record_set dns_aaaa_record_set} Data Source.
 
         :param scope: The scope in which to define this construct.
-        :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param ip_address: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/ptr_record_set#ip_address DataDnsPtrRecordSet#ip_address}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/ptr_record_set#id DataDnsPtrRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
+        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/aaaa_record_set#host DataDnsAaaaRecordSet#host}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__fda41c0faffb5e35e54a3ebc013b5cc6d3805ee4f3a1eeb1e50f268ab9f5d9bc)
+            type_hints = typing.get_type_hints(_typecheckingstub__7c5b6c9236742afbf3551e98db9f779338baacbc53bc50e3b91145a96a8bb0f2)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
-        config = DataDnsPtrRecordSetConfig(
-            ip_address=ip_address,
-            id=id,
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        config = DataDnsAaaaRecordSetConfig(
+            host=host,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
         )
 
-        jsii.create(self.__class__, self, [scope, id_, config])
-
-    @jsii.member(jsii_name="resetId")
-    def reset_id(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetId", []))
+        jsii.create(self.__class__, self, [scope, id, config])
 
     @jsii.member(jsii_name="synthesizeAttributes")
     def _synthesize_attributes(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "synthesizeAttributes", []))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
-    @jsii.member(jsii_name="ptr")
-    def ptr(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "ptr"))
-
-    @builtins.property
-    @jsii.member(jsii_name="idInput")
-    def id_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="ipAddressInput")
-    def ip_address_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "ipAddressInput"))
+    @jsii.member(jsii_name="addrs")
+    def addrs(self) -> typing.List[builtins.str]:
+        return typing.cast(typing.List[builtins.str], jsii.get(self, "addrs"))
 
     @builtins.property
     @jsii.member(jsii_name="id")
     def id(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "id"))
 
-    @id.setter
-    def id(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4804da93c71956da89856d1b9f7b702f3edfacd50ab23840252d84fbb79e340e)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "id", value)
+    @builtins.property
+    @jsii.member(jsii_name="hostInput")
+    def host_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "hostInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="ipAddress")
-    def ip_address(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "ipAddress"))
+    @jsii.member(jsii_name="host")
+    def host(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "host"))
 
-    @ip_address.setter
-    def ip_address(self, value: builtins.str) -> None:
+    @host.setter
+    def host(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c64a8750ea2f9542ec3363181593443c5cd79849a6d6de816341d419d1b638ec)
+            type_hints = typing.get_type_hints(_typecheckingstub__d2c01f0d1f97e5a5cf351e400fcb19bf53b7ad147feee0699ed05080f89616e2)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "ipAddress", value)
+        jsii.set(self, "host", value)
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-dns.dataDnsPtrRecordSet.DataDnsPtrRecordSetConfig",
+    jsii_type="@cdktf/provider-dns.dataDnsAaaaRecordSet.DataDnsAaaaRecordSetConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
-        "ip_address": "ipAddress",
-        "id": "id",
+        "host": "host",
     },
 )
-class DataDnsPtrRecordSetConfig(_cdktf_9a9027ec.TerraformMetaArguments):
+class DataDnsAaaaRecordSetConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
-        ip_address: builtins.str,
-        id: typing.Optional[builtins.str] = None,
+        host: builtins.str,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param ip_address: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/ptr_record_set#ip_address DataDnsPtrRecordSet#ip_address}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/ptr_record_set#id DataDnsPtrRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/aaaa_record_set#host DataDnsAaaaRecordSet#host}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__fcf1fd55b23b7e629d56697ab8a11be420526958500797f4bdec98583deded00)
+            type_hints = typing.get_type_hints(_typecheckingstub__908caa216afdc6eb58e4534363fab765aca58abf2556163688267bf57a2baf0a)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
-            check_type(argname="argument ip_address", value=ip_address, expected_type=type_hints["ip_address"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument host", value=host, expected_type=type_hints["host"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
-            "ip_address": ip_address,
+            "host": host,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
         if depends_on is not None:
             self._values["depends_on"] = depends_on
@@ -194,34 +171,34 @@
             self._values["for_each"] = for_each
         if lifecycle is not None:
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
-        if id is not None:
-            self._values["id"] = id
 
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
@@ -260,85 +237,70 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
-    def ip_address(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/ptr_record_set#ip_address DataDnsPtrRecordSet#ip_address}.'''
-        result = self._values.get("ip_address")
-        assert result is not None, "Required property 'ip_address' is missing"
-        return typing.cast(builtins.str, result)
+    def host(self) -> builtins.str:
+        '''Host to look up.
 
-    @builtins.property
-    def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/ptr_record_set#id DataDnsPtrRecordSet#id}.
-
-        Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
-        If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/aaaa_record_set#host DataDnsAaaaRecordSet#host}
         '''
-        result = self._values.get("id")
-        return typing.cast(typing.Optional[builtins.str], result)
+        result = self._values.get("host")
+        assert result is not None, "Required property 'host' is missing"
+        return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataDnsPtrRecordSetConfig(%s)" % ", ".join(
+        return "DataDnsAaaaRecordSetConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
-    "DataDnsPtrRecordSet",
-    "DataDnsPtrRecordSetConfig",
+    "DataDnsAaaaRecordSet",
+    "DataDnsAaaaRecordSetConfig",
 ]
 
 publication.publish()
 
-def _typecheckingstub__fda41c0faffb5e35e54a3ebc013b5cc6d3805ee4f3a1eeb1e50f268ab9f5d9bc(
+def _typecheckingstub__7c5b6c9236742afbf3551e98db9f779338baacbc53bc50e3b91145a96a8bb0f2(
     scope: _constructs_77d1e7e8.Construct,
-    id_: builtins.str,
+    id: builtins.str,
     *,
-    ip_address: builtins.str,
-    id: typing.Optional[builtins.str] = None,
+    host: builtins.str,
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
 
-def _typecheckingstub__4804da93c71956da89856d1b9f7b702f3edfacd50ab23840252d84fbb79e340e(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__c64a8750ea2f9542ec3363181593443c5cd79849a6d6de816341d419d1b638ec(
+def _typecheckingstub__d2c01f0d1f97e5a5cf351e400fcb19bf53b7ad147feee0699ed05080f89616e2(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__fcf1fd55b23b7e629d56697ab8a11be420526958500797f4bdec98583deded00(
+def _typecheckingstub__908caa216afdc6eb58e4534363fab765aca58abf2556163688267bf57a2baf0a(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
-    ip_address: builtins.str,
-    id: typing.Optional[builtins.str] = None,
+    host: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_srv_record_set/__init__.py` & `cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_srv_record_set/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_dns_srv_record_set`
 
-Refer to the Terraform Registory for docs: [`data_dns_srv_record_set`](https://www.terraform.io/docs/providers/dns/d/srv_record_set).
+Refer to the Terraform Registory for docs: [`data_dns_srv_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/srv_record_set).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,104 +22,85 @@
 
 
 class DataDnsSrvRecordSet(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.dataDnsSrvRecordSet.DataDnsSrvRecordSet",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dns/d/srv_record_set dns_srv_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/srv_record_set dns_srv_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
-        id_: builtins.str,
+        id: builtins.str,
         *,
         service: builtins.str,
-        id: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dns/d/srv_record_set dns_srv_record_set} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/srv_record_set dns_srv_record_set} Data Source.
 
         :param scope: The scope in which to define this construct.
-        :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param service: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/srv_record_set#service DataDnsSrvRecordSet#service}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/srv_record_set#id DataDnsSrvRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
+        :param service: Service to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/srv_record_set#service DataDnsSrvRecordSet#service}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__900efa013f09ac2e7c2d59a5ca95b23f1e060ed453df1921852fbba50c77cc67)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = DataDnsSrvRecordSetConfig(
             service=service,
-            id=id,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
         )
 
-        jsii.create(self.__class__, self, [scope, id_, config])
-
-    @jsii.member(jsii_name="resetId")
-    def reset_id(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetId", []))
+        jsii.create(self.__class__, self, [scope, id, config])
 
     @jsii.member(jsii_name="synthesizeAttributes")
     def _synthesize_attributes(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "synthesizeAttributes", []))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
+    @jsii.member(jsii_name="id")
+    def id(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "id"))
+
+    @builtins.property
     @jsii.member(jsii_name="srv")
     def srv(self) -> "DataDnsSrvRecordSetSrvList":
         return typing.cast("DataDnsSrvRecordSetSrvList", jsii.get(self, "srv"))
 
     @builtins.property
-    @jsii.member(jsii_name="idInput")
-    def id_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
-
-    @builtins.property
     @jsii.member(jsii_name="serviceInput")
     def service_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "serviceInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="id")
-    def id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "id"))
-
-    @id.setter
-    def id(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b16232a6357bf4484eb8e3413ca36e93dba5814cabc7834793a4c0be4f3cf0b8)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "id", value)
-
-    @builtins.property
     @jsii.member(jsii_name="service")
     def service(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "service"))
 
     @service.setter
     def service(self, value: builtins.str) -> None:
         if __debug__:
@@ -136,55 +117,51 @@
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
         "service": "service",
-        "id": "id",
     },
 )
 class DataDnsSrvRecordSetConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         service: builtins.str,
-        id: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param service: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/srv_record_set#service DataDnsSrvRecordSet#service}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/srv_record_set#id DataDnsSrvRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param service: Service to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/srv_record_set#service DataDnsSrvRecordSet#service}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e8e5d88426be0b98ea34a69b2a05888d2eb35258075775c0b01206258ff94272)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
             check_type(argname="argument service", value=service, expected_type=type_hints["service"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "service": service,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
@@ -194,34 +171,34 @@
             self._values["for_each"] = for_each
         if lifecycle is not None:
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
-        if id is not None:
-            self._values["id"] = id
 
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
@@ -261,29 +238,22 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def service(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/srv_record_set#service DataDnsSrvRecordSet#service}.'''
+        '''Service to look up.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/srv_record_set#service DataDnsSrvRecordSet#service}
+        '''
         result = self._values.get("service")
         assert result is not None, "Required property 'service' is missing"
         return typing.cast(builtins.str, result)
 
-    @builtins.property
-    def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/srv_record_set#id DataDnsSrvRecordSet#id}.
-
-        Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
-        If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        '''
-        result = self._values.get("id")
-        return typing.cast(typing.Optional[builtins.str], result)
-
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -453,52 +423,44 @@
     "DataDnsSrvRecordSetSrvOutputReference",
 ]
 
 publication.publish()
 
 def _typecheckingstub__900efa013f09ac2e7c2d59a5ca95b23f1e060ed453df1921852fbba50c77cc67(
     scope: _constructs_77d1e7e8.Construct,
-    id_: builtins.str,
+    id: builtins.str,
     *,
     service: builtins.str,
-    id: typing.Optional[builtins.str] = None,
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
 
-def _typecheckingstub__b16232a6357bf4484eb8e3413ca36e93dba5814cabc7834793a4c0be4f3cf0b8(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
 def _typecheckingstub__f844407d7eb727a4a7e7f86a3c2e399928d921cf373b91f306d2f596c0c82fdd(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__e8e5d88426be0b98ea34a69b2a05888d2eb35258075775c0b01206258ff94272(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     service: builtins.str,
-    id: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__271da12d1a633c7498a91a1f2515fb56b3cf5ef22a14e0de88cab8cb24b24f33(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
```

### Comparing `cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/data_dns_txt_record_set/__init__.py` & `cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/data_dns_txt_record_set/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_dns_txt_record_set`
 
-Refer to the Terraform Registory for docs: [`data_dns_txt_record_set`](https://www.terraform.io/docs/providers/dns/d/txt_record_set).
+Refer to the Terraform Registory for docs: [`data_dns_txt_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/txt_record_set).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,77 +22,75 @@
 
 
 class DataDnsTxtRecordSet(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.dataDnsTxtRecordSet.DataDnsTxtRecordSet",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dns/d/txt_record_set dns_txt_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/txt_record_set dns_txt_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
-        id_: builtins.str,
+        id: builtins.str,
         *,
         host: builtins.str,
-        id: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dns/d/txt_record_set dns_txt_record_set} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/txt_record_set dns_txt_record_set} Data Source.
 
         :param scope: The scope in which to define this construct.
-        :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param host: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/txt_record_set#host DataDnsTxtRecordSet#host}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/txt_record_set#id DataDnsTxtRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
+        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/txt_record_set#host DataDnsTxtRecordSet#host}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c37126296a8eaf7c5e802e35c4d3a81ae3454af6345aba3e10406fa000114e94)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = DataDnsTxtRecordSetConfig(
             host=host,
-            id=id,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
         )
 
-        jsii.create(self.__class__, self, [scope, id_, config])
-
-    @jsii.member(jsii_name="resetId")
-    def reset_id(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetId", []))
+        jsii.create(self.__class__, self, [scope, id, config])
 
     @jsii.member(jsii_name="synthesizeAttributes")
     def _synthesize_attributes(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "synthesizeAttributes", []))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
+    @jsii.member(jsii_name="id")
+    def id(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "id"))
+
+    @builtins.property
     @jsii.member(jsii_name="record")
     def record(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "record"))
 
     @builtins.property
     @jsii.member(jsii_name="records")
     def records(self) -> typing.List[builtins.str]:
@@ -100,96 +98,75 @@
 
     @builtins.property
     @jsii.member(jsii_name="hostInput")
     def host_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "hostInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="idInput")
-    def id_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
-
-    @builtins.property
     @jsii.member(jsii_name="host")
     def host(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "host"))
 
     @host.setter
     def host(self, value: builtins.str) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4f73226430bf565db8b62466b52455c6a93e8e0b4895ab72417e1df36431ac0f)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "host", value)
 
-    @builtins.property
-    @jsii.member(jsii_name="id")
-    def id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "id"))
-
-    @id.setter
-    def id(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__9d230d57b97a16ae4d74f5a2d537e6fe309a84ce4e2d1f0e7dad0ce766a1a9e8)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "id", value)
-
 
 @jsii.data_type(
     jsii_type="@cdktf/provider-dns.dataDnsTxtRecordSet.DataDnsTxtRecordSetConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
         "host": "host",
-        "id": "id",
     },
 )
 class DataDnsTxtRecordSetConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         host: builtins.str,
-        id: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param host: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/txt_record_set#host DataDnsTxtRecordSet#host}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/txt_record_set#id DataDnsTxtRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/txt_record_set#host DataDnsTxtRecordSet#host}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f61abd6fb273d5267b36dde3dc223e24b8418c0ecba25b1d1c82dafbe200648f)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
             check_type(argname="argument host", value=host, expected_type=type_hints["host"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "host": host,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
@@ -199,34 +176,34 @@
             self._values["for_each"] = for_each
         if lifecycle is not None:
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
-        if id is not None:
-            self._values["id"] = id
 
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
@@ -266,29 +243,22 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def host(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/txt_record_set#host DataDnsTxtRecordSet#host}.'''
+        '''Host to look up.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/data-sources/txt_record_set#host DataDnsTxtRecordSet#host}
+        '''
         result = self._values.get("host")
         assert result is not None, "Required property 'host' is missing"
         return typing.cast(builtins.str, result)
 
-    @builtins.property
-    def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/d/txt_record_set#id DataDnsTxtRecordSet#id}.
-
-        Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
-        If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        '''
-        result = self._values.get("id")
-        return typing.cast(typing.Optional[builtins.str], result)
-
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -302,20 +272,19 @@
     "DataDnsTxtRecordSetConfig",
 ]
 
 publication.publish()
 
 def _typecheckingstub__c37126296a8eaf7c5e802e35c4d3a81ae3454af6345aba3e10406fa000114e94(
     scope: _constructs_77d1e7e8.Construct,
-    id_: builtins.str,
+    id: builtins.str,
     *,
     host: builtins.str,
-    id: typing.Optional[builtins.str] = None,
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
@@ -323,27 +292,20 @@
 
 def _typecheckingstub__4f73226430bf565db8b62466b52455c6a93e8e0b4895ab72417e1df36431ac0f(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__9d230d57b97a16ae4d74f5a2d537e6fe309a84ce4e2d1f0e7dad0ce766a1a9e8(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
 def _typecheckingstub__f61abd6fb273d5267b36dde3dc223e24b8418c0ecba25b1d1c82dafbe200648f(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     host: builtins.str,
-    id: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/mx_record_set/__init__.py` & `cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/mx_record_set/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `dns_mx_record_set`
 
-Refer to the Terraform Registory for docs: [`dns_mx_record_set`](https://www.terraform.io/docs/providers/dns/r/mx_record_set).
+Refer to the Terraform Registory for docs: [`dns_mx_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/mx_record_set).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,88 +22,85 @@
 
 
 class MxRecordSet(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.mxRecordSet.MxRecordSet",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dns/r/mx_record_set dns_mx_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/mx_record_set dns_mx_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
-        id_: builtins.str,
+        id: builtins.str,
         *,
-        mx: typing.Union[typing.Sequence[typing.Union["MxRecordSetMx", typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable],
         zone: builtins.str,
-        id: typing.Optional[builtins.str] = None,
+        mx: typing.Optional[typing.Union[typing.Sequence[typing.Union["MxRecordSetMx", typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable]] = None,
         name: typing.Optional[builtins.str] = None,
         ttl: typing.Optional[jsii.Number] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dns/r/mx_record_set dns_mx_record_set} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/mx_record_set dns_mx_record_set} Resource.
 
         :param scope: The scope in which to define this construct.
-        :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param mx: mx block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/mx_record_set#mx MxRecordSet#mx}
-        :param zone: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/mx_record_set#zone MxRecordSet#zone}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/mx_record_set#id MxRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/mx_record_set#name MxRecordSet#name}.
-        :param ttl: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/mx_record_set#ttl MxRecordSet#ttl}.
+        :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/mx_record_set#zone MxRecordSet#zone}
+        :param mx: mx block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/mx_record_set#mx MxRecordSet#mx}
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/mx_record_set#name MxRecordSet#name}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/mx_record_set#ttl MxRecordSet#ttl}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__28fb84e84b50a4f4ae8352b9c2e99694ed2c33de0d1735733d284ee6b9a232d8)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = MxRecordSetConfig(
-            mx=mx,
             zone=zone,
-            id=id,
+            mx=mx,
             name=name,
             ttl=ttl,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
         )
 
-        jsii.create(self.__class__, self, [scope, id_, config])
+        jsii.create(self.__class__, self, [scope, id, config])
 
     @jsii.member(jsii_name="putMx")
     def put_mx(
         self,
         value: typing.Union[typing.Sequence[typing.Union["MxRecordSetMx", typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable],
     ) -> None:
         '''
         :param value: -
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c4077b9e8d32998e5ee328daf6edd5e49e77050924a32ce8d7089a0be0eaecd8)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast(None, jsii.invoke(self, "putMx", [value]))
 
-    @jsii.member(jsii_name="resetId")
-    def reset_id(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetId", []))
+    @jsii.member(jsii_name="resetMx")
+    def reset_mx(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetMx", []))
 
     @jsii.member(jsii_name="resetName")
     def reset_name(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetName", []))
 
     @jsii.member(jsii_name="resetTtl")
     def reset_ttl(self) -> None:
@@ -115,24 +112,24 @@
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
+    @jsii.member(jsii_name="id")
+    def id(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "id"))
+
+    @builtins.property
     @jsii.member(jsii_name="mx")
     def mx(self) -> "MxRecordSetMxList":
         return typing.cast("MxRecordSetMxList", jsii.get(self, "mx"))
 
     @builtins.property
-    @jsii.member(jsii_name="idInput")
-    def id_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
-
-    @builtins.property
     @jsii.member(jsii_name="mxInput")
     def mx_input(
         self,
     ) -> typing.Optional[typing.Union[typing.List["MxRecordSetMx"], _cdktf_9a9027ec.IResolvable]]:
         return typing.cast(typing.Optional[typing.Union[typing.List["MxRecordSetMx"], _cdktf_9a9027ec.IResolvable]], jsii.get(self, "mxInput"))
 
     @builtins.property
@@ -147,26 +144,14 @@
 
     @builtins.property
     @jsii.member(jsii_name="zoneInput")
     def zone_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "zoneInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="id")
-    def id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "id"))
-
-    @id.setter
-    def id(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__549dedf2b65fdf6f1d56be771e73cd93a9bab3587c9d5dbe4e85a0a533d9cfbe)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "id", value)
-
-    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: builtins.str) -> None:
         if __debug__:
@@ -206,70 +191,65 @@
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
-        "mx": "mx",
         "zone": "zone",
-        "id": "id",
+        "mx": "mx",
         "name": "name",
         "ttl": "ttl",
     },
 )
 class MxRecordSetConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
-        mx: typing.Union[typing.Sequence[typing.Union["MxRecordSetMx", typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable],
         zone: builtins.str,
-        id: typing.Optional[builtins.str] = None,
+        mx: typing.Optional[typing.Union[typing.Sequence[typing.Union["MxRecordSetMx", typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable]] = None,
         name: typing.Optional[builtins.str] = None,
         ttl: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param mx: mx block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/mx_record_set#mx MxRecordSet#mx}
-        :param zone: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/mx_record_set#zone MxRecordSet#zone}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/mx_record_set#id MxRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/mx_record_set#name MxRecordSet#name}.
-        :param ttl: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/mx_record_set#ttl MxRecordSet#ttl}.
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/mx_record_set#zone MxRecordSet#zone}
+        :param mx: mx block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/mx_record_set#mx MxRecordSet#mx}
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/mx_record_set#name MxRecordSet#name}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/mx_record_set#ttl MxRecordSet#ttl}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ec52a97ad6f232299e279d08e298f4d1d15ec84a55f739a2354b185a4ac6f39c)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
-            check_type(argname="argument mx", value=mx, expected_type=type_hints["mx"])
             check_type(argname="argument zone", value=zone, expected_type=type_hints["zone"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument mx", value=mx, expected_type=type_hints["mx"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument ttl", value=ttl, expected_type=type_hints["ttl"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
-            "mx": mx,
             "zone": zone,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
         if depends_on is not None:
@@ -278,16 +258,16 @@
             self._values["for_each"] = for_each
         if lifecycle is not None:
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
-        if id is not None:
-            self._values["id"] = id
+        if mx is not None:
+            self._values["mx"] = mx
         if name is not None:
             self._values["name"] = name
         if ttl is not None:
             self._values["ttl"] = ttl
 
     @builtins.property
     def connection(
@@ -296,20 +276,22 @@
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
@@ -348,51 +330,51 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
-    def mx(
-        self,
-    ) -> typing.Union[typing.List["MxRecordSetMx"], _cdktf_9a9027ec.IResolvable]:
-        '''mx block.
+    def zone(self) -> builtins.str:
+        '''DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/mx_record_set#mx MxRecordSet#mx}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/mx_record_set#zone MxRecordSet#zone}
         '''
-        result = self._values.get("mx")
-        assert result is not None, "Required property 'mx' is missing"
-        return typing.cast(typing.Union[typing.List["MxRecordSetMx"], _cdktf_9a9027ec.IResolvable], result)
-
-    @builtins.property
-    def zone(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/mx_record_set#zone MxRecordSet#zone}.'''
         result = self._values.get("zone")
         assert result is not None, "Required property 'zone' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/mx_record_set#id MxRecordSet#id}.
+    def mx(
+        self,
+    ) -> typing.Optional[typing.Union[typing.List["MxRecordSetMx"], _cdktf_9a9027ec.IResolvable]]:
+        '''mx block.
 
-        Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
-        If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/mx_record_set#mx MxRecordSet#mx}
         '''
-        result = self._values.get("id")
-        return typing.cast(typing.Optional[builtins.str], result)
+        result = self._values.get("mx")
+        return typing.cast(typing.Optional[typing.Union[typing.List["MxRecordSetMx"], _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/mx_record_set#name MxRecordSet#name}.'''
+        '''The name of the record set.
+
+        The ``zone`` argument will be appended to this value to create the full record path.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/mx_record_set#name MxRecordSet#name}
+        '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ttl(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/mx_record_set#ttl MxRecordSet#ttl}.'''
+        '''The TTL of the record set. Defaults to ``3600``.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/mx_record_set#ttl MxRecordSet#ttl}
+        '''
         result = self._values.get("ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -408,36 +390,42 @@
     jsii_type="@cdktf/provider-dns.mxRecordSet.MxRecordSetMx",
     jsii_struct_bases=[],
     name_mapping={"exchange": "exchange", "preference": "preference"},
 )
 class MxRecordSetMx:
     def __init__(self, *, exchange: builtins.str, preference: jsii.Number) -> None:
         '''
-        :param exchange: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/mx_record_set#exchange MxRecordSet#exchange}.
-        :param preference: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/mx_record_set#preference MxRecordSet#preference}.
+        :param exchange: The FQDN of the mail exchange, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/mx_record_set#exchange MxRecordSet#exchange}
+        :param preference: The preference for the record. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/mx_record_set#preference MxRecordSet#preference}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__62db89f8cd7dfd80d666fc650cddbbb0d8c9a8866c7654e8b7a20dc912ebb67a)
             check_type(argname="argument exchange", value=exchange, expected_type=type_hints["exchange"])
             check_type(argname="argument preference", value=preference, expected_type=type_hints["preference"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "exchange": exchange,
             "preference": preference,
         }
 
     @builtins.property
     def exchange(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/mx_record_set#exchange MxRecordSet#exchange}.'''
+        '''The FQDN of the mail exchange, include the trailing dot.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/mx_record_set#exchange MxRecordSet#exchange}
+        '''
         result = self._values.get("exchange")
         assert result is not None, "Required property 'exchange' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def preference(self) -> jsii.Number:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/mx_record_set#preference MxRecordSet#preference}.'''
+        '''The preference for the record.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/mx_record_set#preference MxRecordSet#preference}
+        '''
         result = self._values.get("preference")
         assert result is not None, "Required property 'preference' is missing"
         return typing.cast(jsii.Number, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -626,23 +614,22 @@
     "MxRecordSetMxOutputReference",
 ]
 
 publication.publish()
 
 def _typecheckingstub__28fb84e84b50a4f4ae8352b9c2e99694ed2c33de0d1735733d284ee6b9a232d8(
     scope: _constructs_77d1e7e8.Construct,
-    id_: builtins.str,
+    id: builtins.str,
     *,
-    mx: typing.Union[typing.Sequence[typing.Union[MxRecordSetMx, typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable],
     zone: builtins.str,
-    id: typing.Optional[builtins.str] = None,
+    mx: typing.Optional[typing.Union[typing.Sequence[typing.Union[MxRecordSetMx, typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable]] = None,
     name: typing.Optional[builtins.str] = None,
     ttl: typing.Optional[jsii.Number] = None,
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
@@ -650,20 +637,14 @@
 
 def _typecheckingstub__c4077b9e8d32998e5ee328daf6edd5e49e77050924a32ce8d7089a0be0eaecd8(
     value: typing.Union[typing.Sequence[typing.Union[MxRecordSetMx, typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__549dedf2b65fdf6f1d56be771e73cd93a9bab3587c9d5dbe4e85a0a533d9cfbe(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
 def _typecheckingstub__7695431eb02123d6ddacd7392cb32c3197caf57fd5718939645faec883c35da8(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__1bffdd2e2715d126f7a69a0e5f48d06c487b74cbde5ccaca6df905d74d319716(
@@ -677,23 +658,22 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__ec52a97ad6f232299e279d08e298f4d1d15ec84a55f739a2354b185a4ac6f39c(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
-    mx: typing.Union[typing.Sequence[typing.Union[MxRecordSetMx, typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable],
     zone: builtins.str,
-    id: typing.Optional[builtins.str] = None,
+    mx: typing.Optional[typing.Union[typing.Sequence[typing.Union[MxRecordSetMx, typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable]] = None,
     name: typing.Optional[builtins.str] = None,
     ttl: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__62db89f8cd7dfd80d666fc650cddbbb0d8c9a8866c7654e8b7a20dc912ebb67a(
```

### Comparing `cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/ns_record_set/__init__.py` & `cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/ptr_record/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# `dns_ns_record_set`
+# `dns_ptr_record`
 
-Refer to the Terraform Registory for docs: [`dns_ns_record_set`](https://www.terraform.io/docs/providers/dns/r/ns_record_set).
+Refer to the Terraform Registory for docs: [`dns_ptr_record`](https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ptr_record).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -17,80 +17,77 @@
 
 from .._jsii import *
 
 import cdktf as _cdktf_9a9027ec
 import constructs as _constructs_77d1e7e8
 
 
-class NsRecordSet(
+class PtrRecord(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-dns.nsRecordSet.NsRecordSet",
+    jsii_type="@cdktf/provider-dns.ptrRecord.PtrRecord",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dns/r/ns_record_set dns_ns_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ptr_record dns_ptr_record}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
-        id_: builtins.str,
+        id: builtins.str,
         *,
-        name: builtins.str,
-        nameservers: typing.Sequence[builtins.str],
+        ptr: builtins.str,
         zone: builtins.str,
-        id: typing.Optional[builtins.str] = None,
+        name: typing.Optional[builtins.str] = None,
         ttl: typing.Optional[jsii.Number] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dns/r/ns_record_set dns_ns_record_set} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ptr_record dns_ptr_record} Resource.
 
         :param scope: The scope in which to define this construct.
-        :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ns_record_set#name NsRecordSet#name}.
-        :param nameservers: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ns_record_set#nameservers NsRecordSet#nameservers}.
-        :param zone: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ns_record_set#zone NsRecordSet#zone}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ns_record_set#id NsRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param ttl: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ns_record_set#ttl NsRecordSet#ttl}.
+        :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
+        :param ptr: The canonical name this record will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ptr_record#ptr PtrRecord#ptr}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ptr_record#zone PtrRecord#zone}
+        :param name: The name of the record. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ptr_record#name PtrRecord#name}
+        :param ttl: The TTL of the record. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ptr_record#ttl PtrRecord#ttl}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__509f309cc2ac8c5a7e7e52d7cc690641f019a292fc46e109472e09179e6721b0)
+            type_hints = typing.get_type_hints(_typecheckingstub__8a13e50b6d262793ee60c0eaaaf61802dd1cc57db91c11e1ed7a4c0b0aeec0a5)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
-        config = NsRecordSetConfig(
-            name=name,
-            nameservers=nameservers,
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        config = PtrRecordConfig(
+            ptr=ptr,
             zone=zone,
-            id=id,
+            name=name,
             ttl=ttl,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
         )
 
-        jsii.create(self.__class__, self, [scope, id_, config])
+        jsii.create(self.__class__, self, [scope, id, config])
 
-    @jsii.member(jsii_name="resetId")
-    def reset_id(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetId", []))
+    @jsii.member(jsii_name="resetName")
+    def reset_name(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetName", []))
 
     @jsii.member(jsii_name="resetTtl")
     def reset_ttl(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetTtl", []))
 
     @jsii.member(jsii_name="synthesizeAttributes")
     def _synthesize_attributes(self) -> typing.Mapping[builtins.str, typing.Any]:
@@ -98,167 +95,150 @@
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
-    @jsii.member(jsii_name="idInput")
-    def id_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
+    @jsii.member(jsii_name="id")
+    def id(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "id"))
 
     @builtins.property
     @jsii.member(jsii_name="nameInput")
     def name_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "nameInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="nameserversInput")
-    def nameservers_input(self) -> typing.Optional[typing.List[builtins.str]]:
-        return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "nameserversInput"))
+    @jsii.member(jsii_name="ptrInput")
+    def ptr_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "ptrInput"))
 
     @builtins.property
     @jsii.member(jsii_name="ttlInput")
     def ttl_input(self) -> typing.Optional[jsii.Number]:
         return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "ttlInput"))
 
     @builtins.property
     @jsii.member(jsii_name="zoneInput")
     def zone_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "zoneInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="id")
-    def id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "id"))
-
-    @id.setter
-    def id(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__02aababa885ae064e0b70a8e7f51acc48895ce9e19238c990adac02f835497dc)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "id", value)
-
-    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__31f585b9bd18e4dac0600b5da866ef4caeebe89a886776bddbe5956f5b256076)
+            type_hints = typing.get_type_hints(_typecheckingstub__91ddbbef594a63c73b27cbd90c9efa478f85d9ea8369993f5ceb9d37e93cd98c)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
     @builtins.property
-    @jsii.member(jsii_name="nameservers")
-    def nameservers(self) -> typing.List[builtins.str]:
-        return typing.cast(typing.List[builtins.str], jsii.get(self, "nameservers"))
+    @jsii.member(jsii_name="ptr")
+    def ptr(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "ptr"))
 
-    @nameservers.setter
-    def nameservers(self, value: typing.List[builtins.str]) -> None:
+    @ptr.setter
+    def ptr(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__eda6be7152f2c47d8c6e1b2468138cf373970f2d271619e5c0641b5071411f84)
+            type_hints = typing.get_type_hints(_typecheckingstub__cdc3e5836ec4da323bd622209b7504fa2028817da005b9fac2b428d05f484f1a)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "nameservers", value)
+        jsii.set(self, "ptr", value)
 
     @builtins.property
     @jsii.member(jsii_name="ttl")
     def ttl(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "ttl"))
 
     @ttl.setter
     def ttl(self, value: jsii.Number) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__9dfb7611269b3993e4ed448bf64d9c468f39dd3cc7b5e721b685e67eae5ef214)
+            type_hints = typing.get_type_hints(_typecheckingstub__a8cf42b82165bcaf8c02d3d87ae15b67c63e49f0fd14f0151610124f8880271e)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ttl", value)
 
     @builtins.property
     @jsii.member(jsii_name="zone")
     def zone(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "zone"))
 
     @zone.setter
     def zone(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a63d9123b8105fe544190f89f83ac56cd44bfc410b7f4dff0c505daf9774c5e6)
+            type_hints = typing.get_type_hints(_typecheckingstub__4d61cd8c75254c10c41be2fcce4399e144c08effea1359f2f097e81d27846f3e)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zone", value)
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-dns.nsRecordSet.NsRecordSetConfig",
+    jsii_type="@cdktf/provider-dns.ptrRecord.PtrRecordConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
-        "name": "name",
-        "nameservers": "nameservers",
+        "ptr": "ptr",
         "zone": "zone",
-        "id": "id",
+        "name": "name",
         "ttl": "ttl",
     },
 )
-class NsRecordSetConfig(_cdktf_9a9027ec.TerraformMetaArguments):
+class PtrRecordConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
-        name: builtins.str,
-        nameservers: typing.Sequence[builtins.str],
+        ptr: builtins.str,
         zone: builtins.str,
-        id: typing.Optional[builtins.str] = None,
+        name: typing.Optional[builtins.str] = None,
         ttl: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ns_record_set#name NsRecordSet#name}.
-        :param nameservers: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ns_record_set#nameservers NsRecordSet#nameservers}.
-        :param zone: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ns_record_set#zone NsRecordSet#zone}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ns_record_set#id NsRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param ttl: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ns_record_set#ttl NsRecordSet#ttl}.
+        :param ptr: The canonical name this record will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ptr_record#ptr PtrRecord#ptr}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ptr_record#zone PtrRecord#zone}
+        :param name: The name of the record. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ptr_record#name PtrRecord#name}
+        :param ttl: The TTL of the record. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ptr_record#ttl PtrRecord#ttl}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f6a1231a3a6a7ab541c206eb7f9e24e0c86f26ee0a5c23e6f66eb0bb66fe6cd3)
+            type_hints = typing.get_type_hints(_typecheckingstub__b49158521f7275c89a62a7ef19fe09213221f904f5b6b549c8cbf760fa926d3b)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
-            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
-            check_type(argname="argument nameservers", value=nameservers, expected_type=type_hints["nameservers"])
+            check_type(argname="argument ptr", value=ptr, expected_type=type_hints["ptr"])
             check_type(argname="argument zone", value=zone, expected_type=type_hints["zone"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument ttl", value=ttl, expected_type=type_hints["ttl"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
-            "name": name,
-            "nameservers": nameservers,
+            "ptr": ptr,
             "zone": zone,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
         if depends_on is not None:
@@ -267,36 +247,38 @@
             self._values["for_each"] = for_each
         if lifecycle is not None:
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
-        if id is not None:
-            self._values["id"] = id
+        if name is not None:
+            self._values["name"] = name
         if ttl is not None:
             self._values["ttl"] = ttl
 
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
@@ -335,129 +317,124 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
-    def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ns_record_set#name NsRecordSet#name}.'''
-        result = self._values.get("name")
-        assert result is not None, "Required property 'name' is missing"
-        return typing.cast(builtins.str, result)
+    def ptr(self) -> builtins.str:
+        '''The canonical name this record will point to.
 
-    @builtins.property
-    def nameservers(self) -> typing.List[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ns_record_set#nameservers NsRecordSet#nameservers}.'''
-        result = self._values.get("nameservers")
-        assert result is not None, "Required property 'nameservers' is missing"
-        return typing.cast(typing.List[builtins.str], result)
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ptr_record#ptr PtrRecord#ptr}
+        '''
+        result = self._values.get("ptr")
+        assert result is not None, "Required property 'ptr' is missing"
+        return typing.cast(builtins.str, result)
 
     @builtins.property
     def zone(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ns_record_set#zone NsRecordSet#zone}.'''
+        '''DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ptr_record#zone PtrRecord#zone}
+        '''
         result = self._values.get("zone")
         assert result is not None, "Required property 'zone' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ns_record_set#id NsRecordSet#id}.
+    def name(self) -> typing.Optional[builtins.str]:
+        '''The name of the record.
+
+        The ``zone`` argument will be appended to this value to create the full record path.
 
-        Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
-        If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ptr_record#name PtrRecord#name}
         '''
-        result = self._values.get("id")
+        result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ttl(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ns_record_set#ttl NsRecordSet#ttl}.'''
+        '''The TTL of the record. Defaults to ``3600``.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/ptr_record#ttl PtrRecord#ttl}
+        '''
         result = self._values.get("ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "NsRecordSetConfig(%s)" % ", ".join(
+        return "PtrRecordConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
-    "NsRecordSet",
-    "NsRecordSetConfig",
+    "PtrRecord",
+    "PtrRecordConfig",
 ]
 
 publication.publish()
 
-def _typecheckingstub__509f309cc2ac8c5a7e7e52d7cc690641f019a292fc46e109472e09179e6721b0(
+def _typecheckingstub__8a13e50b6d262793ee60c0eaaaf61802dd1cc57db91c11e1ed7a4c0b0aeec0a5(
     scope: _constructs_77d1e7e8.Construct,
-    id_: builtins.str,
+    id: builtins.str,
     *,
-    name: builtins.str,
-    nameservers: typing.Sequence[builtins.str],
+    ptr: builtins.str,
     zone: builtins.str,
-    id: typing.Optional[builtins.str] = None,
+    name: typing.Optional[builtins.str] = None,
     ttl: typing.Optional[jsii.Number] = None,
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
 
-def _typecheckingstub__02aababa885ae064e0b70a8e7f51acc48895ce9e19238c990adac02f835497dc(
+def _typecheckingstub__91ddbbef594a63c73b27cbd90c9efa478f85d9ea8369993f5ceb9d37e93cd98c(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__31f585b9bd18e4dac0600b5da866ef4caeebe89a886776bddbe5956f5b256076(
+def _typecheckingstub__cdc3e5836ec4da323bd622209b7504fa2028817da005b9fac2b428d05f484f1a(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__eda6be7152f2c47d8c6e1b2468138cf373970f2d271619e5c0641b5071411f84(
-    value: typing.List[builtins.str],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__9dfb7611269b3993e4ed448bf64d9c468f39dd3cc7b5e721b685e67eae5ef214(
+def _typecheckingstub__a8cf42b82165bcaf8c02d3d87ae15b67c63e49f0fd14f0151610124f8880271e(
     value: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__a63d9123b8105fe544190f89f83ac56cd44bfc410b7f4dff0c505daf9774c5e6(
+def _typecheckingstub__4d61cd8c75254c10c41be2fcce4399e144c08effea1359f2f097e81d27846f3e(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__f6a1231a3a6a7ab541c206eb7f9e24e0c86f26ee0a5c23e6f66eb0bb66fe6cd3(
+def _typecheckingstub__b49158521f7275c89a62a7ef19fe09213221f904f5b6b549c8cbf760fa926d3b(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
-    name: builtins.str,
-    nameservers: typing.Sequence[builtins.str],
+    ptr: builtins.str,
     zone: builtins.str,
-    id: typing.Optional[builtins.str] = None,
+    name: typing.Optional[builtins.str] = None,
     ttl: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/ptr_record/__init__.py` & `cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/aaaa_record_set/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# `dns_ptr_record`
+# `dns_aaaa_record_set`
 
-Refer to the Terraform Registory for docs: [`dns_ptr_record`](https://www.terraform.io/docs/providers/dns/r/ptr_record).
+Refer to the Terraform Registory for docs: [`dns_aaaa_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/aaaa_record_set).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -17,62 +17,62 @@
 
 from .._jsii import *
 
 import cdktf as _cdktf_9a9027ec
 import constructs as _constructs_77d1e7e8
 
 
-class PtrRecord(
+class AaaaRecordSet(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-dns.ptrRecord.PtrRecord",
+    jsii_type="@cdktf/provider-dns.aaaaRecordSet.AaaaRecordSet",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dns/r/ptr_record dns_ptr_record}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/aaaa_record_set dns_aaaa_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
-        ptr: builtins.str,
+        addresses: typing.Sequence[builtins.str],
         zone: builtins.str,
         id: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
         ttl: typing.Optional[jsii.Number] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dns/r/ptr_record dns_ptr_record} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/aaaa_record_set dns_aaaa_record_set} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param ptr: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ptr_record#ptr PtrRecord#ptr}.
-        :param zone: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ptr_record#zone PtrRecord#zone}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ptr_record#id PtrRecord#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ptr_record#name PtrRecord#name}.
-        :param ttl: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ptr_record#ttl PtrRecord#ttl}.
+        :param addresses: The IPv6 addresses this record set will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/aaaa_record_set#addresses AaaaRecordSet#addresses}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/aaaa_record_set#zone AaaaRecordSet#zone}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/aaaa_record_set#id AaaaRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/aaaa_record_set#name AaaaRecordSet#name}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/aaaa_record_set#ttl AaaaRecordSet#ttl}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8a13e50b6d262793ee60c0eaaaf61802dd1cc57db91c11e1ed7a4c0b0aeec0a5)
+            type_hints = typing.get_type_hints(_typecheckingstub__f95a77e839b028e1ec4b902d403800b8b2681cb3c7db96ab08cc03ebda128881)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
-        config = PtrRecordConfig(
-            ptr=ptr,
+        config = AaaaRecordSetConfig(
+            addresses=addresses,
             zone=zone,
             id=id,
             name=name,
             ttl=ttl,
             connection=connection,
             count=count,
             depends_on=depends_on,
@@ -102,166 +102,166 @@
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
+    @jsii.member(jsii_name="addressesInput")
+    def addresses_input(self) -> typing.Optional[typing.List[builtins.str]]:
+        return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "addressesInput"))
+
+    @builtins.property
     @jsii.member(jsii_name="idInput")
     def id_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
 
     @builtins.property
     @jsii.member(jsii_name="nameInput")
     def name_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "nameInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="ptrInput")
-    def ptr_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "ptrInput"))
-
-    @builtins.property
     @jsii.member(jsii_name="ttlInput")
     def ttl_input(self) -> typing.Optional[jsii.Number]:
         return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "ttlInput"))
 
     @builtins.property
     @jsii.member(jsii_name="zoneInput")
     def zone_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "zoneInput"))
 
     @builtins.property
+    @jsii.member(jsii_name="addresses")
+    def addresses(self) -> typing.List[builtins.str]:
+        return typing.cast(typing.List[builtins.str], jsii.get(self, "addresses"))
+
+    @addresses.setter
+    def addresses(self, value: typing.List[builtins.str]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__c3e59b87eff2656f0de40996521f03d742ff8265b83569ec1fd4b8a6056ad4c0)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "addresses", value)
+
+    @builtins.property
     @jsii.member(jsii_name="id")
     def id(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "id"))
 
     @id.setter
     def id(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8be20a22ed5f43bc84f24657428cb3acaed86e3af7c64d03cfd4e6e46bcd8b9f)
+            type_hints = typing.get_type_hints(_typecheckingstub__c7fecdfc9eeccee6c52b39b5837a4e230fe597c52ba820d55aff7f8ac1b7b580)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "id", value)
 
     @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__91ddbbef594a63c73b27cbd90c9efa478f85d9ea8369993f5ceb9d37e93cd98c)
+            type_hints = typing.get_type_hints(_typecheckingstub__969155f00d50bb4a786f2c8022e08a5844dc4a210099603a0c7efbed716c6639)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
     @builtins.property
-    @jsii.member(jsii_name="ptr")
-    def ptr(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "ptr"))
-
-    @ptr.setter
-    def ptr(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__cdc3e5836ec4da323bd622209b7504fa2028817da005b9fac2b428d05f484f1a)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "ptr", value)
-
-    @builtins.property
     @jsii.member(jsii_name="ttl")
     def ttl(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "ttl"))
 
     @ttl.setter
     def ttl(self, value: jsii.Number) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a8cf42b82165bcaf8c02d3d87ae15b67c63e49f0fd14f0151610124f8880271e)
+            type_hints = typing.get_type_hints(_typecheckingstub__2ce4b77d7d883f7cc36d31ff4f98f93b768f356d6bfb3d47277b1b80fdb2f192)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ttl", value)
 
     @builtins.property
     @jsii.member(jsii_name="zone")
     def zone(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "zone"))
 
     @zone.setter
     def zone(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4d61cd8c75254c10c41be2fcce4399e144c08effea1359f2f097e81d27846f3e)
+            type_hints = typing.get_type_hints(_typecheckingstub__76ee0b7f55beb4e085448a399443bf4cb34ccba38c7001a5de482dcd9df78fcb)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zone", value)
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-dns.ptrRecord.PtrRecordConfig",
+    jsii_type="@cdktf/provider-dns.aaaaRecordSet.AaaaRecordSetConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
-        "ptr": "ptr",
+        "addresses": "addresses",
         "zone": "zone",
         "id": "id",
         "name": "name",
         "ttl": "ttl",
     },
 )
-class PtrRecordConfig(_cdktf_9a9027ec.TerraformMetaArguments):
+class AaaaRecordSetConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
-        ptr: builtins.str,
+        addresses: typing.Sequence[builtins.str],
         zone: builtins.str,
         id: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
         ttl: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param ptr: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ptr_record#ptr PtrRecord#ptr}.
-        :param zone: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ptr_record#zone PtrRecord#zone}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ptr_record#id PtrRecord#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ptr_record#name PtrRecord#name}.
-        :param ttl: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ptr_record#ttl PtrRecord#ttl}.
+        :param addresses: The IPv6 addresses this record set will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/aaaa_record_set#addresses AaaaRecordSet#addresses}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/aaaa_record_set#zone AaaaRecordSet#zone}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/aaaa_record_set#id AaaaRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/aaaa_record_set#name AaaaRecordSet#name}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/aaaa_record_set#ttl AaaaRecordSet#ttl}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b49158521f7275c89a62a7ef19fe09213221f904f5b6b549c8cbf760fa926d3b)
+            type_hints = typing.get_type_hints(_typecheckingstub__7b02504a909c79d4df8654eda870cd6b0da805b48d848ba6bc32daaa4249e3a3)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
-            check_type(argname="argument ptr", value=ptr, expected_type=type_hints["ptr"])
+            check_type(argname="argument addresses", value=addresses, expected_type=type_hints["addresses"])
             check_type(argname="argument zone", value=zone, expected_type=type_hints["zone"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument ttl", value=ttl, expected_type=type_hints["ttl"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
-            "ptr": ptr,
+            "addresses": addresses,
             "zone": zone,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
         if depends_on is not None:
@@ -288,20 +288,22 @@
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
@@ -340,128 +342,142 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
-    def ptr(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ptr_record#ptr PtrRecord#ptr}.'''
-        result = self._values.get("ptr")
-        assert result is not None, "Required property 'ptr' is missing"
-        return typing.cast(builtins.str, result)
+    def addresses(self) -> typing.List[builtins.str]:
+        '''The IPv6 addresses this record set will point to.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/aaaa_record_set#addresses AaaaRecordSet#addresses}
+        '''
+        result = self._values.get("addresses")
+        assert result is not None, "Required property 'addresses' is missing"
+        return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def zone(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ptr_record#zone PtrRecord#zone}.'''
+        '''DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/aaaa_record_set#zone AaaaRecordSet#zone}
+        '''
         result = self._values.get("zone")
         assert result is not None, "Required property 'zone' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ptr_record#id PtrRecord#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/aaaa_record_set#id AaaaRecordSet#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ptr_record#name PtrRecord#name}.'''
+        '''The name of the record set.
+
+        The ``zone`` argument will be appended to this value to create the full record path.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/aaaa_record_set#name AaaaRecordSet#name}
+        '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ttl(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/ptr_record#ttl PtrRecord#ttl}.'''
+        '''The TTL of the record set. Defaults to ``3600``.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/aaaa_record_set#ttl AaaaRecordSet#ttl}
+        '''
         result = self._values.get("ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "PtrRecordConfig(%s)" % ", ".join(
+        return "AaaaRecordSetConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
-    "PtrRecord",
-    "PtrRecordConfig",
+    "AaaaRecordSet",
+    "AaaaRecordSetConfig",
 ]
 
 publication.publish()
 
-def _typecheckingstub__8a13e50b6d262793ee60c0eaaaf61802dd1cc57db91c11e1ed7a4c0b0aeec0a5(
+def _typecheckingstub__f95a77e839b028e1ec4b902d403800b8b2681cb3c7db96ab08cc03ebda128881(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
-    ptr: builtins.str,
+    addresses: typing.Sequence[builtins.str],
     zone: builtins.str,
     id: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     ttl: typing.Optional[jsii.Number] = None,
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
 
-def _typecheckingstub__8be20a22ed5f43bc84f24657428cb3acaed86e3af7c64d03cfd4e6e46bcd8b9f(
-    value: builtins.str,
+def _typecheckingstub__c3e59b87eff2656f0de40996521f03d742ff8265b83569ec1fd4b8a6056ad4c0(
+    value: typing.List[builtins.str],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__91ddbbef594a63c73b27cbd90c9efa478f85d9ea8369993f5ceb9d37e93cd98c(
+def _typecheckingstub__c7fecdfc9eeccee6c52b39b5837a4e230fe597c52ba820d55aff7f8ac1b7b580(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__cdc3e5836ec4da323bd622209b7504fa2028817da005b9fac2b428d05f484f1a(
+def _typecheckingstub__969155f00d50bb4a786f2c8022e08a5844dc4a210099603a0c7efbed716c6639(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__a8cf42b82165bcaf8c02d3d87ae15b67c63e49f0fd14f0151610124f8880271e(
+def _typecheckingstub__2ce4b77d7d883f7cc36d31ff4f98f93b768f356d6bfb3d47277b1b80fdb2f192(
     value: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__4d61cd8c75254c10c41be2fcce4399e144c08effea1359f2f097e81d27846f3e(
+def _typecheckingstub__76ee0b7f55beb4e085448a399443bf4cb34ccba38c7001a5de482dcd9df78fcb(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__b49158521f7275c89a62a7ef19fe09213221f904f5b6b549c8cbf760fa926d3b(
+def _typecheckingstub__7b02504a909c79d4df8654eda870cd6b0da805b48d848ba6bc32daaa4249e3a3(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
-    ptr: builtins.str,
+    addresses: typing.Sequence[builtins.str],
     zone: builtins.str,
     id: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     ttl: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns/srv_record_set/__init__.py` & `cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns/srv_record_set/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `dns_srv_record_set`
 
-Refer to the Terraform Registory for docs: [`dns_srv_record_set`](https://www.terraform.io/docs/providers/dns/r/srv_record_set).
+Refer to the Terraform Registory for docs: [`dns_srv_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,88 +22,85 @@
 
 
 class SrvRecordSet(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.srvRecordSet.SrvRecordSet",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set dns_srv_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set dns_srv_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
-        id_: builtins.str,
+        id: builtins.str,
         *,
         name: builtins.str,
-        srv: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["SrvRecordSetSrv", typing.Dict[builtins.str, typing.Any]]]],
         zone: builtins.str,
-        id: typing.Optional[builtins.str] = None,
+        srv: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["SrvRecordSetSrv", typing.Dict[builtins.str, typing.Any]]]]] = None,
         ttl: typing.Optional[jsii.Number] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set dns_srv_record_set} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set dns_srv_record_set} Resource.
 
         :param scope: The scope in which to define this construct.
-        :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#name SrvRecordSet#name}.
-        :param srv: srv block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#srv SrvRecordSet#srv}
-        :param zone: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#zone SrvRecordSet#zone}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#id SrvRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param ttl: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#ttl SrvRecordSet#ttl}.
+        :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set#name SrvRecordSet#name}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set#zone SrvRecordSet#zone}
+        :param srv: srv block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set#srv SrvRecordSet#srv}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set#ttl SrvRecordSet#ttl}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a7e53ee7bbad1e23f45b47594e2b0a1caa7300b9c2488c1cae72f4ff4d5c738d)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = SrvRecordSetConfig(
             name=name,
-            srv=srv,
             zone=zone,
-            id=id,
+            srv=srv,
             ttl=ttl,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
         )
 
-        jsii.create(self.__class__, self, [scope, id_, config])
+        jsii.create(self.__class__, self, [scope, id, config])
 
     @jsii.member(jsii_name="putSrv")
     def put_srv(
         self,
         value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["SrvRecordSetSrv", typing.Dict[builtins.str, typing.Any]]]],
     ) -> None:
         '''
         :param value: -
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5e0117747aa1bf787eb1a72418573dadd646361b3fff4daf3764b794a606c513)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast(None, jsii.invoke(self, "putSrv", [value]))
 
-    @jsii.member(jsii_name="resetId")
-    def reset_id(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetId", []))
+    @jsii.member(jsii_name="resetSrv")
+    def reset_srv(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetSrv", []))
 
     @jsii.member(jsii_name="resetTtl")
     def reset_ttl(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetTtl", []))
 
     @jsii.member(jsii_name="synthesizeAttributes")
     def _synthesize_attributes(self) -> typing.Mapping[builtins.str, typing.Any]:
@@ -111,24 +108,24 @@
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
+    @jsii.member(jsii_name="id")
+    def id(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "id"))
+
+    @builtins.property
     @jsii.member(jsii_name="srv")
     def srv(self) -> "SrvRecordSetSrvList":
         return typing.cast("SrvRecordSetSrvList", jsii.get(self, "srv"))
 
     @builtins.property
-    @jsii.member(jsii_name="idInput")
-    def id_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
-
-    @builtins.property
     @jsii.member(jsii_name="nameInput")
     def name_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "nameInput"))
 
     @builtins.property
     @jsii.member(jsii_name="srvInput")
     def srv_input(
@@ -143,26 +140,14 @@
 
     @builtins.property
     @jsii.member(jsii_name="zoneInput")
     def zone_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "zoneInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="id")
-    def id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "id"))
-
-    @id.setter
-    def id(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__fac91d36439f5afd12fde7aac6c1853ca0bb34b60f9a54dd87d9b35d45baf9f0)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "id", value)
-
-    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: builtins.str) -> None:
         if __debug__:
@@ -203,70 +188,65 @@
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
         "name": "name",
-        "srv": "srv",
         "zone": "zone",
-        "id": "id",
+        "srv": "srv",
         "ttl": "ttl",
     },
 )
 class SrvRecordSetConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
-        srv: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["SrvRecordSetSrv", typing.Dict[builtins.str, typing.Any]]]],
         zone: builtins.str,
-        id: typing.Optional[builtins.str] = None,
+        srv: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["SrvRecordSetSrv", typing.Dict[builtins.str, typing.Any]]]]] = None,
         ttl: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#name SrvRecordSet#name}.
-        :param srv: srv block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#srv SrvRecordSet#srv}
-        :param zone: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#zone SrvRecordSet#zone}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#id SrvRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param ttl: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#ttl SrvRecordSet#ttl}.
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set#name SrvRecordSet#name}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set#zone SrvRecordSet#zone}
+        :param srv: srv block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set#srv SrvRecordSet#srv}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set#ttl SrvRecordSet#ttl}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a6cead32c63515d033c83d20cbbfcf8c7bcd53fa2262ec6c1d0833d054ff2ada)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
-            check_type(argname="argument srv", value=srv, expected_type=type_hints["srv"])
             check_type(argname="argument zone", value=zone, expected_type=type_hints["zone"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument srv", value=srv, expected_type=type_hints["srv"])
             check_type(argname="argument ttl", value=ttl, expected_type=type_hints["ttl"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "name": name,
-            "srv": srv,
             "zone": zone,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
         if depends_on is not None:
@@ -275,36 +255,38 @@
             self._values["for_each"] = for_each
         if lifecycle is not None:
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
-        if id is not None:
-            self._values["id"] = id
+        if srv is not None:
+            self._values["srv"] = srv
         if ttl is not None:
             self._values["ttl"] = ttl
 
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
@@ -344,51 +326,51 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#name SrvRecordSet#name}.'''
+        '''The name of the record set.
+
+        The ``zone`` argument will be appended to this value to create the full record path.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set#name SrvRecordSet#name}
+        '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def srv(
-        self,
-    ) -> typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SrvRecordSetSrv"]]:
-        '''srv block.
+    def zone(self) -> builtins.str:
+        '''DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#srv SrvRecordSet#srv}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set#zone SrvRecordSet#zone}
         '''
-        result = self._values.get("srv")
-        assert result is not None, "Required property 'srv' is missing"
-        return typing.cast(typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SrvRecordSetSrv"]], result)
-
-    @builtins.property
-    def zone(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#zone SrvRecordSet#zone}.'''
         result = self._values.get("zone")
         assert result is not None, "Required property 'zone' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#id SrvRecordSet#id}.
+    def srv(
+        self,
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SrvRecordSetSrv"]]]:
+        '''srv block.
 
-        Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
-        If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set#srv SrvRecordSet#srv}
         '''
-        result = self._values.get("id")
-        return typing.cast(typing.Optional[builtins.str], result)
+        result = self._values.get("srv")
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SrvRecordSetSrv"]]], result)
 
     @builtins.property
     def ttl(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#ttl SrvRecordSet#ttl}.'''
+        '''The TTL of the record set. Defaults to ``3600``.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set#ttl SrvRecordSet#ttl}
+        '''
         result = self._values.get("ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -416,18 +398,18 @@
         *,
         port: jsii.Number,
         priority: jsii.Number,
         target: builtins.str,
         weight: jsii.Number,
     ) -> None:
         '''
-        :param port: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#port SrvRecordSet#port}.
-        :param priority: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#priority SrvRecordSet#priority}.
-        :param target: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#target SrvRecordSet#target}.
-        :param weight: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#weight SrvRecordSet#weight}.
+        :param port: The port for the service on the target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set#port SrvRecordSet#port}
+        :param priority: The priority for the record. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set#priority SrvRecordSet#priority}
+        :param target: The FQDN of the target, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set#target SrvRecordSet#target}
+        :param weight: The weight for the record. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set#weight SrvRecordSet#weight}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8e3b61e2f863fa4a109ee13e90a0ecff126e73fce1309591ec6e079b4f7ad5f6)
             check_type(argname="argument port", value=port, expected_type=type_hints["port"])
             check_type(argname="argument priority", value=priority, expected_type=type_hints["priority"])
             check_type(argname="argument target", value=target, expected_type=type_hints["target"])
             check_type(argname="argument weight", value=weight, expected_type=type_hints["weight"])
@@ -436,36 +418,48 @@
             "priority": priority,
             "target": target,
             "weight": weight,
         }
 
     @builtins.property
     def port(self) -> jsii.Number:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#port SrvRecordSet#port}.'''
+        '''The port for the service on the target.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set#port SrvRecordSet#port}
+        '''
         result = self._values.get("port")
         assert result is not None, "Required property 'port' is missing"
         return typing.cast(jsii.Number, result)
 
     @builtins.property
     def priority(self) -> jsii.Number:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#priority SrvRecordSet#priority}.'''
+        '''The priority for the record.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set#priority SrvRecordSet#priority}
+        '''
         result = self._values.get("priority")
         assert result is not None, "Required property 'priority' is missing"
         return typing.cast(jsii.Number, result)
 
     @builtins.property
     def target(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#target SrvRecordSet#target}.'''
+        '''The FQDN of the target, include the trailing dot.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set#target SrvRecordSet#target}
+        '''
         result = self._values.get("target")
         assert result is not None, "Required property 'target' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def weight(self) -> jsii.Number:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dns/r/srv_record_set#weight SrvRecordSet#weight}.'''
+        '''The weight for the record.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.3.0/docs/resources/srv_record_set#weight SrvRecordSet#weight}
+        '''
         result = self._values.get("weight")
         assert result is not None, "Required property 'weight' is missing"
         return typing.cast(jsii.Number, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -688,23 +682,22 @@
     "SrvRecordSetSrvOutputReference",
 ]
 
 publication.publish()
 
 def _typecheckingstub__a7e53ee7bbad1e23f45b47594e2b0a1caa7300b9c2488c1cae72f4ff4d5c738d(
     scope: _constructs_77d1e7e8.Construct,
-    id_: builtins.str,
+    id: builtins.str,
     *,
     name: builtins.str,
-    srv: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[SrvRecordSetSrv, typing.Dict[builtins.str, typing.Any]]]],
     zone: builtins.str,
-    id: typing.Optional[builtins.str] = None,
+    srv: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[SrvRecordSetSrv, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ttl: typing.Optional[jsii.Number] = None,
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
@@ -712,20 +705,14 @@
 
 def _typecheckingstub__5e0117747aa1bf787eb1a72418573dadd646361b3fff4daf3764b794a606c513(
     value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[SrvRecordSetSrv, typing.Dict[builtins.str, typing.Any]]]],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__fac91d36439f5afd12fde7aac6c1853ca0bb34b60f9a54dd87d9b35d45baf9f0(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
 def _typecheckingstub__8829f8ec5d8a8e5e138d029a8a6093887d31d312b18831087bdadb9a43af23a7(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__6192b6100c812f5490ccaa01ef3c5f9da2353df039934b2491c44e91b4da1b91(
@@ -739,24 +726,23 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__a6cead32c63515d033c83d20cbbfcf8c7bcd53fa2262ec6c1d0833d054ff2ada(
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
-    srv: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[SrvRecordSetSrv, typing.Dict[builtins.str, typing.Any]]]],
     zone: builtins.str,
-    id: typing.Optional[builtins.str] = None,
+    srv: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[SrvRecordSetSrv, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ttl: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__8e3b61e2f863fa4a109ee13e90a0ecff126e73fce1309591ec6e079b4f7ad5f6(
     *,
```

### Comparing `cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns.egg-info/PKG-INFO` & `cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-dns
-Version: 3.0.1
+Version: 4.0.0
 Summary: Prebuilt dns Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-dns.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-dns.git
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
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-dns-go`](https://github.com/cdktf/cdktf-provider-dns-go) package.
 
 `go get github.com/cdktf/cdktf-provider-dns-go/dns`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-dns).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform dns Provider version 1:1. In fact, it always tracks `latest` of `~> 3.2` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-dns-3.0.1/src/cdktf_cdktf_provider_dns.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-dns-4.0.0/src/cdktf_cdktf_provider_dns.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_dns/py.typed
 src/cdktf_cdktf_provider_dns.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_dns.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_dns.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_dns.egg-info/requires.txt
 src/cdktf_cdktf_provider_dns.egg-info/top_level.txt
 src/cdktf_cdktf_provider_dns/_jsii/__init__.py
-src/cdktf_cdktf_provider_dns/_jsii/provider-dns@3.0.1.jsii.tgz
+src/cdktf_cdktf_provider_dns/_jsii/provider-dns@4.0.0.jsii.tgz
 src/cdktf_cdktf_provider_dns/a_record_set/__init__.py
 src/cdktf_cdktf_provider_dns/aaaa_record_set/__init__.py
 src/cdktf_cdktf_provider_dns/cname_record/__init__.py
 src/cdktf_cdktf_provider_dns/data_dns_a_record_set/__init__.py
 src/cdktf_cdktf_provider_dns/data_dns_aaaa_record_set/__init__.py
 src/cdktf_cdktf_provider_dns/data_dns_cname_record_set/__init__.py
 src/cdktf_cdktf_provider_dns/data_dns_mx_record_set/__init__.py
```

