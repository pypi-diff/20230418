# Comparing `tmp/koku-nise-4.2.2.tar.gz` & `tmp/koku-nise-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koku-nise-4.2.2.tar", last modified: Wed Apr 12 16:17:03 2023, max compression
+gzip compressed data, was "koku-nise-4.2.3.tar", last modified: Tue Apr 18 16:58:50 2023, max compression
```

## Comparing `koku-nise-4.2.2.tar` & `koku-nise-4.2.3.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:03.211041 koku-nise-4.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-04-12 16:16:46.000000 koku-nise-4.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-12 16:16:46.000000 koku-nise-4.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-12 16:17:03.211041 koku-nise-4.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10526 2023-04-12 16:16:46.000000 koku-nise-4.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:03.203040 koku-nise-4.2.2/koku_nise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-12 16:17:03.000000 koku-nise-4.2.2/koku_nise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-12 16:17:03.000000 koku-nise-4.2.2/koku_nise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:17:03.000000 koku-nise-4.2.2/koku_nise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 16:17:03.000000 koku-nise-4.2.2/koku_nise.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:17:03.000000 koku-nise-4.2.2/koku_nise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-12 16:17:03.000000 koku-nise-4.2.2/koku_nise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-12 16:17:03.000000 koku-nise-4.2.2/koku_nise.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:03.203040 koku-nise-4.2.2/nise/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26044 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/aws-template-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:03.207041 koku-nise-4.2.2/nise/generators/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:03.207041 koku-nise-4.2.2/nise/generators/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/aws/aws_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13300 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/aws/aws_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/aws/data_transfer_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/aws/ebs_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/aws/ec2_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/aws/marketplace_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/aws/rds_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/aws/route53_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/aws/s3_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/aws/vpc_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:03.207041 koku-nise-4.2.2/nise/generators/azure/
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/azure/azure_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/azure/bandwidth_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/azure/ccsp_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/azure/sql_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/azure/storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/azure/virtual_machine_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/azure/virtual_network_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:03.207041 koku-nise-4.2.2/nise/generators/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/gcp/cloud_storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/gcp/compute_engine_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/gcp/gcp_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/gcp/gcp_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/gcp/gcp_network_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/gcp/hcs_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/gcp/project_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:03.207041 koku-nise-4.2.2/nise/generators/oci/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/oci/oci_block_storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/oci/oci_compute_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/oci/oci_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/oci/oci_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/oci/oci_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/oci/oci_network_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:03.207041 koku-nise-4.2.2/nise/generators/ocp/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/ocp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36824 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/generators/ocp/ocp_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/ocp-template-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)    52710 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:03.211041 koku-nise-4.2.2/nise/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/util/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:03.211041 koku-nise-4.2.2/nise/yaml_generators/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:03.211041 koku-nise-4.2.2/nise/yaml_generators/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71376 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/aws/ec2_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/aws/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/aws/rds_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/aws/regions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:03.211041 koku-nise-4.2.2/nise/yaml_generators/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/azure/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:03.211041 koku-nise-4.2.2/nise/yaml_generators/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/gcp/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:03.211041 koku-nise-4.2.2/nise/yaml_generators/oci/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/oci/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/oci/oci_yaml_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:03.211041 koku-nise-4.2.2/nise/yaml_generators/ocp/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/ocp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/ocp/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:03.211041 koku-nise-4.2.2/nise/yaml_generators/ocp_on_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/ocp_on_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/ocp_on_cloud/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:03.211041 koku-nise-4.2.2/nise/yaml_generators/static/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/static/aws_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/static/aws_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/static/azure_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/static/azure_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/static/gcp_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/static/gcp_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/static/oci_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/static/oci_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/static/ocp_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/static/ocp_on_cloud_options.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/static/ocp_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-04-12 16:16:46.000000 koku-nise-4.2.2/nise/yaml_generators/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 16:17:03.211041 koku-nise-4.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-12 16:16:46.000000 koku-nise-4.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.509495 koku-nise-4.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-04-18 16:58:28.000000 koku-nise-4.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-18 16:58:28.000000 koku-nise-4.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-18 16:58:50.509495 koku-nise-4.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10526 2023-04-18 16:58:28.000000 koku-nise-4.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.497495 koku-nise-4.2.3/koku_nise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-18 16:58:50.000000 koku-nise-4.2.3/koku_nise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-18 16:58:50.000000 koku-nise-4.2.3/koku_nise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:58:50.000000 koku-nise-4.2.3/koku_nise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-18 16:58:50.000000 koku-nise-4.2.3/koku_nise.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:58:50.000000 koku-nise-4.2.3/koku_nise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-18 16:58:50.000000 koku-nise-4.2.3/koku_nise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 16:58:50.000000 koku-nise-4.2.3/koku_nise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.501495 koku-nise-4.2.3/nise/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26044 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/aws-template-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.501495 koku-nise-4.2.3/nise/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.501495 koku-nise-4.2.3/nise/generators/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/aws_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/aws_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/data_transfer_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/ebs_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/ec2_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/marketplace_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/rds_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/route53_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/s3_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/vpc_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.501495 koku-nise-4.2.3/nise/generators/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/azure/azure_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/azure/bandwidth_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/azure/ccsp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/azure/sql_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/azure/storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/azure/virtual_machine_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/azure/virtual_network_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.501495 koku-nise-4.2.3/nise/generators/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/gcp/cloud_storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/gcp/compute_engine_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/gcp/gcp_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/gcp/gcp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/gcp/gcp_network_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/gcp/hcs_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/gcp/project_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.505495 koku-nise-4.2.3/nise/generators/oci/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/oci/oci_block_storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/oci/oci_compute_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/oci/oci_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/oci/oci_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/oci/oci_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/oci/oci_network_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.505495 koku-nise-4.2.3/nise/generators/ocp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/ocp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36824 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/ocp/ocp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/ocp-template-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)    52710 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.505495 koku-nise-4.2.3/nise/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/util/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.505495 koku-nise-4.2.3/nise/yaml_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.505495 koku-nise-4.2.3/nise/yaml_generators/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71376 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/aws/ec2_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/aws/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/aws/rds_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/aws/regions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.505495 koku-nise-4.2.3/nise/yaml_generators/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/azure/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.505495 koku-nise-4.2.3/nise/yaml_generators/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/gcp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.505495 koku-nise-4.2.3/nise/yaml_generators/oci/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/oci/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/oci/oci_yaml_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.505495 koku-nise-4.2.3/nise/yaml_generators/ocp/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/ocp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/ocp/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.505495 koku-nise-4.2.3/nise/yaml_generators/ocp_on_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/ocp_on_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/ocp_on_cloud/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.509495 koku-nise-4.2.3/nise/yaml_generators/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/aws_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/aws_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/azure_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/azure_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/gcp_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/gcp_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/oci_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/oci_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/ocp_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/ocp_on_cloud_options.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/ocp_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:58:50.509495 koku-nise-4.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-18 16:58:28.000000 koku-nise-4.2.3/setup.py
```

### Comparing `koku-nise-4.2.2/LICENSE` & `koku-nise-4.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/README.rst` & `koku-nise-4.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/koku_nise.egg-info/SOURCES.txt` & `koku-nise-4.2.3/koku_nise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/__main__.py` & `koku-nise-4.2.3/nise/__main__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/aws-template-manifest.json` & `koku-nise-4.2.3/nise/aws-template-manifest.json`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/copy.py` & `koku-nise-4.2.3/nise/copy.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/extract.py` & `koku-nise-4.2.3/nise/extract.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/aws/__init__.py` & `koku-nise-4.2.3/nise/generators/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/aws/aws_constants.py` & `koku-nise-4.2.3/nise/generators/aws/aws_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/aws/aws_generator.py` & `koku-nise-4.2.3/nise/generators/aws/aws_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,14 +225,15 @@
         "resourceTags/user:environment",
         "resourceTags/user:app",
         "resourceTags/user:version",
         "resourceTags/user:storageclass",
         "resourceTags/user:openshift_cluster",
         "resourceTags/user:openshift_project",
         "resourceTags/user:openshift_node",
+        "resourceTags/aws:createdBy",
     }
     COST_CATEGORY_COLS = {
         "costCategory/Charge type",
         "costCategory/CostCenter",
         "costCategory/OUs",
         "costCategory/Organization",
     }
@@ -244,20 +245,20 @@
         + PRICING_COLS
         + RESERVE_COLS
         + SAVINGS_COLS
         + tuple(RESOURCE_TAG_COLS)
         + tuple(COST_CATEGORY_COLS)
     )
 
-    def __init__(self, start_date, end_date, currency, payer_account, usage_accounts, attributes={}, tag_cols=None):
+    def __init__(self, start_date, end_date, currency, payer_account, usage_accounts, attributes=None, tag_cols=None):
         """Initialize the generator."""
         self.payer_account = payer_account
         self.currency = currency
         self.usage_accounts = usage_accounts
-        self.attributes = attributes
+        self.attributes = attributes if attributes else {}
         self._tags = None
         self._cost_category = None
         self.num_instances = 1 if attributes else randint(2, 60)
         if tag_cols:
             self.RESOURCE_TAG_COLS.update(tag_cols)
             self.AWS_COLUMNS.update(tag_cols)
         if attributes:
```

### Comparing `koku-nise-4.2.2/nise/generators/aws/data_transfer_generator.py` & `koku-nise-4.2.3/nise/generators/aws/data_transfer_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/aws/ebs_generator.py` & `koku-nise-4.2.3/nise/generators/aws/ebs_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/aws/ec2_generator.py` & `koku-nise-4.2.3/nise/generators/aws/ec2_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/aws/marketplace_generator.py` & `koku-nise-4.2.3/nise/generators/aws/marketplace_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,25 +30,26 @@
 
     MARKETPLACE_PRODUCTS = (
         "Red Hat OpenShift Service on AWS",
         "Red Hat Enterprise Linux 7",
         "Red Hat Enterprise Linux 8",
     )
 
-    def __init__(self, start_date, end_date, currency, payer_account, usage_accounts, attributes={}, tag_cols=None):
+    def __init__(self, start_date, end_date, currency, payer_account, usage_accounts, attributes=None, tag_cols=None):
         """Initialize the generator."""
         super().__init__(start_date, end_date, currency, payer_account, usage_accounts, attributes, tag_cols)
 
         self._amount = uniform(0.2, 300.99)
         self._rate = round(uniform(0.02, 0.16), 3)
         self._resource_id = "i-{}".format(self.fake.ean8())
         self._product_sku = self.fake.pystr(min_chars=12, max_chars=12).upper()
 
-        for attribute in self.attributes:
-            setattr(self, f"_{attribute}", self.attributes.get(attribute))
+        if self.attributes:
+            for attribute in self.attributes:
+                setattr(self, f"_{attribute}", self.attributes.get(attribute))
 
         if tag_cols:
             self.RESOURCE_TAG_COLS.update(tag_cols)
             self.AWS_COLUMNS.update(tag_cols)
 
     @property
     def rate_code(self):
```

### Comparing `koku-nise-4.2.2/nise/generators/aws/rds_generator.py` & `koku-nise-4.2.3/nise/generators/aws/rds_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/aws/route53_generator.py` & `koku-nise-4.2.3/nise/generators/aws/route53_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/aws/s3_generator.py` & `koku-nise-4.2.3/nise/generators/aws/s3_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/aws/vpc_generator.py` & `koku-nise-4.2.3/nise/generators/aws/vpc_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/azure/__init__.py` & `koku-nise-4.2.3/nise/generators/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/azure/azure_generator.py` & `koku-nise-4.2.3/nise/generators/azure/azure_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/azure/bandwidth_generator.py` & `koku-nise-4.2.3/nise/generators/azure/bandwidth_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/azure/ccsp_generator.py` & `koku-nise-4.2.3/nise/generators/azure/ccsp_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/azure/sql_database_generator.py` & `koku-nise-4.2.3/nise/generators/azure/sql_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/azure/storage_generator.py` & `koku-nise-4.2.3/nise/generators/azure/storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/azure/virtual_machine_generator.py` & `koku-nise-4.2.3/nise/generators/azure/virtual_machine_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/azure/virtual_network_generator.py` & `koku-nise-4.2.3/nise/generators/azure/virtual_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/gcp/__init__.py` & `koku-nise-4.2.3/nise/generators/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/gcp/cloud_storage_generator.py` & `koku-nise-4.2.3/nise/generators/gcp/cloud_storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/gcp/compute_engine_generator.py` & `koku-nise-4.2.3/nise/generators/gcp/compute_engine_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/gcp/gcp_database_generator.py` & `koku-nise-4.2.3/nise/generators/gcp/gcp_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/gcp/gcp_generator.py` & `koku-nise-4.2.3/nise/generators/gcp/gcp_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/gcp/gcp_network_generator.py` & `koku-nise-4.2.3/nise/generators/gcp/gcp_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/gcp/hcs_generator.py` & `koku-nise-4.2.3/nise/generators/gcp/hcs_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/gcp/project_generator.py` & `koku-nise-4.2.3/nise/generators/gcp/project_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/generator.py` & `koku-nise-4.2.3/nise/generators/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/oci/__init__.py` & `koku-nise-4.2.3/nise/generators/oci/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/oci/oci_block_storage_generator.py` & `koku-nise-4.2.3/nise/generators/oci/oci_block_storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/oci/oci_compute_generator.py` & `koku-nise-4.2.3/nise/generators/oci/oci_compute_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/oci/oci_constants.py` & `koku-nise-4.2.3/nise/generators/oci/oci_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/oci/oci_database_generator.py` & `koku-nise-4.2.3/nise/generators/oci/oci_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/oci/oci_generator.py` & `koku-nise-4.2.3/nise/generators/oci/oci_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/oci/oci_network_generator.py` & `koku-nise-4.2.3/nise/generators/oci/oci_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/ocp/__init__.py` & `koku-nise-4.2.3/nise/generators/ocp/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/generators/ocp/ocp_generator.py` & `koku-nise-4.2.3/nise/generators/ocp/ocp_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/manifest.py` & `koku-nise-4.2.3/nise/manifest.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/report.py` & `koku-nise-4.2.3/nise/report.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/upload.py` & `koku-nise-4.2.3/nise/upload.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/util/__init__.py` & `koku-nise-4.2.3/nise/util/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/util/log.py` & `koku-nise-4.2.3/nise/util/log.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_gen.py` & `koku-nise-4.2.3/nise/yaml_gen.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_generators/aws/ec2_instance_types.py` & `koku-nise-4.2.3/nise/yaml_generators/aws/ec2_instance_types.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_generators/aws/generator.py` & `koku-nise-4.2.3/nise/yaml_generators/aws/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_generators/aws/rds_instance_types.py` & `koku-nise-4.2.3/nise/yaml_generators/aws/rds_instance_types.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_generators/aws/regions.py` & `koku-nise-4.2.3/nise/yaml_generators/aws/regions.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_generators/azure/generator.py` & `koku-nise-4.2.3/nise/yaml_generators/azure/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_generators/gcp/generator.py` & `koku-nise-4.2.3/nise/yaml_generators/gcp/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_generators/generator.py` & `koku-nise-4.2.3/nise/yaml_generators/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_generators/oci/generator.py` & `koku-nise-4.2.3/nise/yaml_generators/oci/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_generators/oci/oci_yaml_constants.py` & `koku-nise-4.2.3/nise/yaml_generators/oci/oci_yaml_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_generators/ocp/generator.py` & `koku-nise-4.2.3/nise/yaml_generators/ocp/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_generators/ocp_on_cloud/generator.py` & `koku-nise-4.2.3/nise/yaml_generators/ocp_on_cloud/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_generators/static/aws_generator_config.yml` & `koku-nise-4.2.3/nise/yaml_generators/static/aws_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_generators/static/aws_static_data.yml.j2` & `koku-nise-4.2.3/nise/yaml_generators/static/aws_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_generators/static/azure_generator_config.yml` & `koku-nise-4.2.3/nise/yaml_generators/static/azure_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_generators/static/azure_static_data.yml.j2` & `koku-nise-4.2.3/nise/yaml_generators/static/azure_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_generators/static/gcp_static_data.yml.j2` & `koku-nise-4.2.3/nise/yaml_generators/static/gcp_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_generators/static/oci_static_data.yml.j2` & `koku-nise-4.2.3/nise/yaml_generators/static/oci_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_generators/static/ocp_generator_config.yml` & `koku-nise-4.2.3/nise/yaml_generators/static/ocp_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_generators/static/ocp_on_cloud_options.yml` & `koku-nise-4.2.3/nise/yaml_generators/static/ocp_on_cloud_options.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_generators/static/ocp_static_data.yml.j2` & `koku-nise-4.2.3/nise/yaml_generators/static/ocp_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/nise/yaml_generators/utils.py` & `koku-nise-4.2.3/nise/yaml_generators/utils.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.2/setup.py` & `koku-nise-4.2.3/setup.py`

 * *Files identical despite different names*

