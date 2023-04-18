# Comparing `tmp/cdk-extensions-0.0.56.tar.gz` & `tmp/cdk-extensions-0.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-extensions-0.0.56.tar", last modified: Mon Apr 17 17:31:34 2023, max compression
+gzip compressed data, was "cdk-extensions-0.0.57.tar", last modified: Tue Apr 18 19:03:26 2023, max compression
```

## Comparing `cdk-extensions-0.0.56.tar` & `cdk-extensions-0.0.57.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.344279 cdk-extensions-0.0.56/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-17 17:31:34.344279 cdk-extensions-0.0.56/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 17:31:34.344279 cdk-extensions-0.0.56/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.332279 cdk-extensions-0.0.56/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.336279 cdk-extensions-0.0.56/src/cdk_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.336279 cdk-extensions-0.0.56/src/cdk_extensions/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.336279 cdk-extensions-0.0.56/src/cdk_extensions/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/_jsii/bin/init-aws.sh
--rw-r--r--   0 runner    (1001) docker     (123)  1548042 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/_jsii/cdk-extensions@0.0.56.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.336279 cdk-extensions-0.0.56/src/cdk_extensions/aps/
--rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/aps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.340279 cdk-extensions-0.0.56/src/cdk_extensions/asserts/
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/asserts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.340279 cdk-extensions-0.0.56/src/cdk_extensions/athena/
--rw-r--r--   0 runner    (1001) docker     (123)   100087 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/athena/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.340279 cdk-extensions-0.0.56/src/cdk_extensions/core/
--rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.340279 cdk-extensions-0.0.56/src/cdk_extensions/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)   661251 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/ec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.340279 cdk-extensions-0.0.56/src/cdk_extensions/ec2_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)   159980 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/ec2_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.340279 cdk-extensions-0.0.56/src/cdk_extensions/eks_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)    95667 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/eks_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.340279 cdk-extensions-0.0.56/src/cdk_extensions/glue/
--rw-r--r--   0 runner    (1001) docker     (123)   507583 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/glue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.340279 cdk-extensions-0.0.56/src/cdk_extensions/glue_tables/
--rw-r--r--   0 runner    (1001) docker     (123)   140852 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/glue_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.340279 cdk-extensions-0.0.56/src/cdk_extensions/k8s_aws/
--rw-r--r--   0 runner    (1001) docker     (123)   692448 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/k8s_aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.340279 cdk-extensions-0.0.56/src/cdk_extensions/k8s_fargate/
--rw-r--r--   0 runner    (1001) docker     (123)    25868 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/k8s_fargate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.340279 cdk-extensions-0.0.56/src/cdk_extensions/kinesis_firehose/
--rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/kinesis_firehose/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.344279 cdk-extensions-0.0.56/src/cdk_extensions/lambda_/
--rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/lambda_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.344279 cdk-extensions-0.0.56/src/cdk_extensions/networkmanager/
--rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/networkmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.344279 cdk-extensions-0.0.56/src/cdk_extensions/ram/
--rw-r--r--   0 runner    (1001) docker     (123)    42370 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/ram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.344279 cdk-extensions-0.0.56/src/cdk_extensions/ram_resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/ram_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.344279 cdk-extensions-0.0.56/src/cdk_extensions/rds/
--rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/rds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.344279 cdk-extensions-0.0.56/src/cdk_extensions/route53/
--rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/route53/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.344279 cdk-extensions-0.0.56/src/cdk_extensions/s3_buckets/
--rw-r--r--   0 runner    (1001) docker     (123)   215302 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/s3_buckets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.344279 cdk-extensions-0.0.56/src/cdk_extensions/sso/
--rw-r--r--   0 runner    (1001) docker     (123)   130481 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/sso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.344279 cdk-extensions-0.0.56/src/cdk_extensions/stacks/
--rw-r--r--   0 runner    (1001) docker     (123)    58263 2023-04-17 17:31:23.000000 cdk-extensions-0.0.56/src/cdk_extensions/stacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:34.336279 cdk-extensions-0.0.56/src/cdk_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-17 17:31:34.000000 cdk-extensions-0.0.56/src/cdk_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-17 17:31:34.000000 cdk-extensions-0.0.56/src/cdk_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:31:34.000000 cdk-extensions-0.0.56/src/cdk_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-17 17:31:34.000000 cdk-extensions-0.0.56/src/cdk_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 17:31:34.000000 cdk-extensions-0.0.56/src/cdk_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.093843 cdk-extensions-0.0.57/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-18 19:03:26.093843 cdk-extensions-0.0.57/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 19:03:26.093843 cdk-extensions-0.0.57/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.081843 cdk-extensions-0.0.57/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.085843 cdk-extensions-0.0.57/src/cdk_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.085843 cdk-extensions-0.0.57/src/cdk_extensions/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.085843 cdk-extensions-0.0.57/src/cdk_extensions/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/_jsii/bin/init-aws.sh
+-rw-r--r--   0 runner    (1001) docker     (123)  1548296 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/_jsii/cdk-extensions@0.0.57.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.085843 cdk-extensions-0.0.57/src/cdk_extensions/aps/
+-rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/aps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.085843 cdk-extensions-0.0.57/src/cdk_extensions/asserts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/asserts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.085843 cdk-extensions-0.0.57/src/cdk_extensions/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)   100087 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/athena/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.085843 cdk-extensions-0.0.57/src/cdk_extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.085843 cdk-extensions-0.0.57/src/cdk_extensions/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)   661251 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/ec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.089843 cdk-extensions-0.0.57/src/cdk_extensions/ec2_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)   162099 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/ec2_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.089843 cdk-extensions-0.0.57/src/cdk_extensions/eks_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)    95667 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/eks_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.089843 cdk-extensions-0.0.57/src/cdk_extensions/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)   507583 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/glue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.089843 cdk-extensions-0.0.57/src/cdk_extensions/glue_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)   140852 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/glue_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.089843 cdk-extensions-0.0.57/src/cdk_extensions/k8s_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)   692448 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/k8s_aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.089843 cdk-extensions-0.0.57/src/cdk_extensions/k8s_fargate/
+-rw-r--r--   0 runner    (1001) docker     (123)    25868 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/k8s_fargate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.089843 cdk-extensions-0.0.57/src/cdk_extensions/kinesis_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/kinesis_firehose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.089843 cdk-extensions-0.0.57/src/cdk_extensions/lambda_/
+-rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/lambda_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.089843 cdk-extensions-0.0.57/src/cdk_extensions/networkmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/networkmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.089843 cdk-extensions-0.0.57/src/cdk_extensions/ram/
+-rw-r--r--   0 runner    (1001) docker     (123)    42370 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/ram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.089843 cdk-extensions-0.0.57/src/cdk_extensions/ram_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/ram_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.089843 cdk-extensions-0.0.57/src/cdk_extensions/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/rds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.089843 cdk-extensions-0.0.57/src/cdk_extensions/route53/
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/route53/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.089843 cdk-extensions-0.0.57/src/cdk_extensions/s3_buckets/
+-rw-r--r--   0 runner    (1001) docker     (123)   215302 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/s3_buckets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.093843 cdk-extensions-0.0.57/src/cdk_extensions/sso/
+-rw-r--r--   0 runner    (1001) docker     (123)   130481 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/sso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.093843 cdk-extensions-0.0.57/src/cdk_extensions/stacks/
+-rw-r--r--   0 runner    (1001) docker     (123)    58263 2023-04-18 19:03:14.000000 cdk-extensions-0.0.57/src/cdk_extensions/stacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:26.085843 cdk-extensions-0.0.57/src/cdk_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-18 19:03:26.000000 cdk-extensions-0.0.57/src/cdk_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-18 19:03:26.000000 cdk-extensions-0.0.57/src/cdk_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:03:26.000000 cdk-extensions-0.0.57/src/cdk_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-18 19:03:26.000000 cdk-extensions-0.0.57/src/cdk_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 19:03:26.000000 cdk-extensions-0.0.57/src/cdk_extensions.egg-info/top_level.txt
```

### Comparing `cdk-extensions-0.0.56/LICENSE` & `cdk-extensions-0.0.57/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/PKG-INFO` & `cdk-extensions-0.0.57/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.56
+Version: 0.0.57
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.56/README.md` & `cdk-extensions-0.0.57/README.md`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/setup.py` & `cdk-extensions-0.0.57/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-extensions",
-    "version": "0.0.56",
+    "version": "0.0.57",
     "description": "cdk-extensions",
     "license": "Apache-2.0",
     "url": "https://github.com/vibe-io/cdk-extensions.git",
     "long_description_content_type": "text/markdown",
     "author": "Kevin Lucas<kevinluc08@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -43,15 +43,15 @@
         "cdk_extensions.route53",
         "cdk_extensions.s3_buckets",
         "cdk_extensions.sso",
         "cdk_extensions.stacks"
     ],
     "package_data": {
         "cdk_extensions._jsii": [
-            "cdk-extensions@0.0.56.jsii.tgz"
+            "cdk-extensions@0.0.57.jsii.tgz"
         ],
         "cdk_extensions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/aps/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/aps/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/asserts/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/asserts/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/athena/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/core/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/ec2/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/ec2_patterns/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/ec2_patterns/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,29 +31,57 @@
     ResourceShare as _ResourceShare_f0180713,
 )
 
 
 @jsii.data_type(
     jsii_type="cdk-extensions.ec2_patterns.AddNetworkOptions",
     jsii_struct_bases=[],
-    name_mapping={"netmask": "netmask"},
+    name_mapping={
+        "availability_zones": "availabilityZones",
+        "max_azs": "maxAzs",
+        "netmask": "netmask",
+    },
 )
 class AddNetworkOptions:
-    def __init__(self, *, netmask: typing.Optional[jsii.Number] = None) -> None:
+    def __init__(
+        self,
+        *,
+        availability_zones: typing.Optional[typing.Sequence[builtins.str]] = None,
+        max_azs: typing.Optional[jsii.Number] = None,
+        netmask: typing.Optional[jsii.Number] = None,
+    ) -> None:
         '''
+        :param availability_zones: 
+        :param max_azs: 
         :param netmask: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__24d3c1346e4e259fee32303499f123223b892ff23852cdfdf5a57bf21cad7680)
+            check_type(argname="argument availability_zones", value=availability_zones, expected_type=type_hints["availability_zones"])
+            check_type(argname="argument max_azs", value=max_azs, expected_type=type_hints["max_azs"])
             check_type(argname="argument netmask", value=netmask, expected_type=type_hints["netmask"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if availability_zones is not None:
+            self._values["availability_zones"] = availability_zones
+        if max_azs is not None:
+            self._values["max_azs"] = max_azs
         if netmask is not None:
             self._values["netmask"] = netmask
 
     @builtins.property
+    def availability_zones(self) -> typing.Optional[typing.List[builtins.str]]:
+        result = self._values.get("availability_zones")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+
+    @builtins.property
+    def max_azs(self) -> typing.Optional[jsii.Number]:
+        result = self._values.get("max_azs")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
     def netmask(self) -> typing.Optional[jsii.Number]:
         result = self._values.get("netmask")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -2203,47 +2231,59 @@
 
     @jsii.member(jsii_name="addHub")
     def add_hub(
         self,
         scope: _constructs_77d1e7e8.IConstruct,
         id: builtins.str,
         *,
+        availability_zones: typing.Optional[typing.Sequence[builtins.str]] = None,
+        max_azs: typing.Optional[jsii.Number] = None,
         netmask: typing.Optional[jsii.Number] = None,
     ) -> FourTierNetworkHub:
         '''
         :param scope: -
         :param id: -
+        :param availability_zones: 
+        :param max_azs: 
         :param netmask: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__74ba1ec928c092f33aeb546fda189638c35c356996133e040cb167d089e3f343)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        options = AddNetworkOptions(netmask=netmask)
+        options = AddNetworkOptions(
+            availability_zones=availability_zones, max_azs=max_azs, netmask=netmask
+        )
 
         return typing.cast(FourTierNetworkHub, jsii.invoke(self, "addHub", [scope, id, options]))
 
     @jsii.member(jsii_name="addSpoke")
     def add_spoke(
         self,
         scope: _constructs_77d1e7e8.IConstruct,
         id: builtins.str,
         *,
+        availability_zones: typing.Optional[typing.Sequence[builtins.str]] = None,
+        max_azs: typing.Optional[jsii.Number] = None,
         netmask: typing.Optional[jsii.Number] = None,
     ) -> FourTierNetworkSpoke:
         '''
         :param scope: -
         :param id: -
+        :param availability_zones: 
+        :param max_azs: 
         :param netmask: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f39726d5378c607c7d2408b015e8aed7d5f87a4d39b2235dbde97aa46e8daba2)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        options = AddNetworkOptions(netmask=netmask)
+        options = AddNetworkOptions(
+            availability_zones=availability_zones, max_azs=max_azs, netmask=netmask
+        )
 
         return typing.cast(FourTierNetworkSpoke, jsii.invoke(self, "addSpoke", [scope, id, options]))
 
     @jsii.member(jsii_name="registerAccount")
     def _register_account(self, account: builtins.str) -> None:
         '''
         :param account: -
@@ -2648,14 +2688,16 @@
     "TransitGatewaySpokeConfiguration",
 ]
 
 publication.publish()
 
 def _typecheckingstub__24d3c1346e4e259fee32303499f123223b892ff23852cdfdf5a57bf21cad7680(
     *,
+    availability_zones: typing.Optional[typing.Sequence[builtins.str]] = None,
+    max_azs: typing.Optional[jsii.Number] = None,
     netmask: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__bafe93fe5666e81af7b6555c6e0b02d696c2267310d93ce406cc5b16333a1449(
     *,
@@ -2998,23 +3040,27 @@
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__74ba1ec928c092f33aeb546fda189638c35c356996133e040cb167d089e3f343(
     scope: _constructs_77d1e7e8.IConstruct,
     id: builtins.str,
     *,
+    availability_zones: typing.Optional[typing.Sequence[builtins.str]] = None,
+    max_azs: typing.Optional[jsii.Number] = None,
     netmask: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__f39726d5378c607c7d2408b015e8aed7d5f87a4d39b2235dbde97aa46e8daba2(
     scope: _constructs_77d1e7e8.IConstruct,
     id: builtins.str,
     *,
+    availability_zones: typing.Optional[typing.Sequence[builtins.str]] = None,
+    max_azs: typing.Optional[jsii.Number] = None,
     netmask: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__7a94042b91cf18ea51b81a0607a52121519d15828b001d7f2a7c825c4dc5c4f9(
     account: builtins.str,
```

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/eks_patterns/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/eks_patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/glue/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/glue/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/glue_tables/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/glue_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/k8s_aws/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/k8s_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/k8s_fargate/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/k8s_fargate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/kinesis_firehose/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/kinesis_firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/lambda_/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/networkmanager/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/networkmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/ram/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/ram_resources/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/ram_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/rds/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/rds/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/route53/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/s3_buckets/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/s3_buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/sso/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/sso/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions/stacks/__init__.py` & `cdk-extensions-0.0.57/src/cdk_extensions/stacks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions.egg-info/PKG-INFO` & `cdk-extensions-0.0.57/src/cdk_extensions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.56
+Version: 0.0.57
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.56/src/cdk_extensions.egg-info/SOURCES.txt` & `cdk-extensions-0.0.57/src/cdk_extensions.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdk_extensions/py.typed
 src/cdk_extensions.egg-info/PKG-INFO
 src/cdk_extensions.egg-info/SOURCES.txt
 src/cdk_extensions.egg-info/dependency_links.txt
 src/cdk_extensions.egg-info/requires.txt
 src/cdk_extensions.egg-info/top_level.txt
 src/cdk_extensions/_jsii/__init__.py
-src/cdk_extensions/_jsii/cdk-extensions@0.0.56.jsii.tgz
+src/cdk_extensions/_jsii/cdk-extensions@0.0.57.jsii.tgz
 src/cdk_extensions/_jsii/bin/init-aws.sh
 src/cdk_extensions/aps/__init__.py
 src/cdk_extensions/asserts/__init__.py
 src/cdk_extensions/athena/__init__.py
 src/cdk_extensions/core/__init__.py
 src/cdk_extensions/ec2/__init__.py
 src/cdk_extensions/ec2_patterns/__init__.py
```

