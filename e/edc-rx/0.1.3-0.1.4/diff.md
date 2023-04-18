# Comparing `tmp/edc-rx-0.1.3.tar.gz` & `tmp/edc-rx-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-rx-0.1.3.tar", last modified: Fri Mar 31 01:08:47 2023, max compression
+gzip compressed data, was "edc-rx-0.1.4.tar", last modified: Tue Apr 18 01:41:33 2023, max compression
```

## Comparing `edc-rx-0.1.3.tar` & `edc-rx-0.1.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 01:08:47.103233 edc-rx-0.1.3/
--rw-r--r--   0 erikvw     (501) staff       (20)       78 2022-11-29 04:55:26.000000 edc-rx-0.1.3/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-29 04:55:26.000000 edc-rx-0.1.3/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 01:08:47.093778 edc-rx-0.1.3/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 01:08:47.097249 edc-rx-0.1.3/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1639 2022-11-29 04:55:26.000000 edc-rx-0.1.3/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-11-29 04:55:26.000000 edc-rx-0.1.3/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-11-29 04:55:26.000000 edc-rx-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-29 04:55:26.000000 edc-rx-0.1.3/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.3/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.3/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-29 03:26:32.000000 edc-rx-0.1.3/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-11-29 04:55:26.000000 edc-rx-0.1.3/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1410 2023-03-31 01:08:47.103346 edc-rx-0.1.3/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      613 2022-11-29 04:55:26.000000 edc-rx-0.1.3/README.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 01:08:47.098136 edc-rx-0.1.3/edc_rx/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      157 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      270 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/apps.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 01:08:47.099616 edc-rx-0.1.3/edc_rx/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)     5180 2022-11-29 06:36:26.000000 edc-rx-0.1.3/edc_rx/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 06:36:26.000000 edc-rx-0.1.3/edc_rx/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 01:08:47.100517 edc-rx-0.1.3/edc_rx/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      181 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1558 2023-03-31 01:06:02.000000 edc-rx-0.1.3/edc_rx/model_mixins/drug_refill_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      866 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/model_mixins/drug_supply_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1250 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/model_mixins/treatment_pay_methods.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 01:08:47.101038 edc-rx-0.1.3/edc_rx/modeladmin_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/modeladmin_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1158 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      731 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 01:08:47.101382 edc-rx-0.1.3/edc_rx/modelform_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)       73 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/modelform_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1915 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      440 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 01:08:47.101550 edc-rx-0.1.3/edc_rx/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.3/edc_rx/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 01:08:47.102860 edc-rx-0.1.3/edc_rx/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/tests/etc/user-salt-restricted.key
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 01:08:47.103022 edc-rx-0.1.3/edc_rx/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.3/edc_rx/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      277 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      900 2022-11-29 04:55:26.000000 edc-rx-0.1.3/edc_rx/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 01:08:47.099195 edc-rx-0.1.3/edc_rx.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1410 2023-03-31 01:08:47.000000 edc-rx-0.1.3/edc_rx.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1302 2023-03-31 01:08:47.000000 edc-rx-0.1.3/edc_rx.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-03-31 01:08:47.000000 edc-rx-0.1.3/edc_rx.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-29 04:55:34.000000 edc-rx-0.1.3/edc_rx.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)        7 2023-03-31 01:08:47.000000 edc-rx-0.1.3/edc_rx.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1592 2022-11-29 04:55:26.000000 edc-rx-0.1.3/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1106 2023-03-31 01:08:39.000000 edc-rx-0.1.3/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1100 2023-03-31 01:08:47.103701 edc-rx-0.1.3/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.467733 edc-rx-0.1.4/
+-rw-r--r--   0 erikvw     (501) staff       (20)       78 2022-11-29 04:55:26.000000 edc-rx-0.1.4/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-29 04:55:26.000000 edc-rx-0.1.4/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.459466 edc-rx-0.1.4/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.462997 edc-rx-0.1.4/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1645 2023-04-18 01:41:25.000000 edc-rx-0.1.4/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-11-29 04:55:26.000000 edc-rx-0.1.4/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-04-18 01:41:25.000000 edc-rx-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-29 04:55:26.000000 edc-rx-0.1.4/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.4/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.4/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-29 03:26:32.000000 edc-rx-0.1.4/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-11-29 04:55:26.000000 edc-rx-0.1.4/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1461 2023-04-18 01:41:33.467826 edc-rx-0.1.4/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      613 2022-11-29 04:55:26.000000 edc-rx-0.1.4/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.463885 edc-rx-0.1.4/edc_rx/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      157 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      270 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/apps.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.464930 edc-rx-0.1.4/edc_rx/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)     5179 2023-04-18 01:41:25.000000 edc-rx-0.1.4/edc_rx/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 06:36:26.000000 edc-rx-0.1.4/edc_rx/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.465579 edc-rx-0.1.4/edc_rx/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      181 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1558 2023-03-31 01:06:02.000000 edc-rx-0.1.4/edc_rx/model_mixins/drug_refill_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      865 2023-04-18 01:41:25.000000 edc-rx-0.1.4/edc_rx/model_mixins/drug_supply_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1249 2023-04-18 01:41:25.000000 edc-rx-0.1.4/edc_rx/model_mixins/treatment_pay_methods.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.466018 edc-rx-0.1.4/edc_rx/modeladmin_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/modeladmin_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1158 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      730 2023-04-18 01:41:25.000000 edc-rx-0.1.4/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.466283 edc-rx-0.1.4/edc_rx/modelform_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)       73 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/modelform_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1914 2023-04-18 01:41:25.000000 edc-rx-0.1.4/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      440 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.466406 edc-rx-0.1.4/edc_rx/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.4/edc_rx/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.467513 edc-rx-0.1.4/edc_rx/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/tests/etc/user-salt-restricted.key
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.467651 edc-rx-0.1.4/edc_rx/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.4/edc_rx/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      277 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      900 2022-11-29 04:55:26.000000 edc-rx-0.1.4/edc_rx/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-18 01:41:33.464680 edc-rx-0.1.4/edc_rx.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1461 2023-04-18 01:41:33.000000 edc-rx-0.1.4/edc_rx.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1302 2023-04-18 01:41:33.000000 edc-rx-0.1.4/edc_rx.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-04-18 01:41:33.000000 edc-rx-0.1.4/edc_rx.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-29 04:55:34.000000 edc-rx-0.1.4/edc_rx.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)        7 2023-04-18 01:41:33.000000 edc-rx-0.1.4/edc_rx.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1679 2023-04-18 01:41:25.000000 edc-rx-0.1.4/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1106 2023-03-31 01:08:39.000000 edc-rx-0.1.4/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1140 2023-04-18 01:41:33.468159 edc-rx-0.1.4/setup.cfg
```

### Comparing `edc-rx-0.1.3/.github/workflows/build.yml` & `edc-rx-0.1.4/.github/workflows/build.yml`

 * *Files 10% similar despite different names*

```diff
@@ -7,37 +7,37 @@
   build:
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.10']
+        python-version: ['3.10', '3.11']
         django-version: ['4.1', 'dev']
 
     steps:
       - name: Install pycups and words dependency
         run: |
           sudo sed -i 's/azure\.//' /etc/apt/sources.list
           sudo apt-get -y update
           sudo apt-get install libcups2-dev wamerican
 
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Get pip cache dir
         id: pip-cache
         run: |
-          echo "::set-output name=dir::$(pip cache dir)"
+          echo "dir=$(pip cache dir)" >>$GITHUB_OUTPUT
 
       - name: Cache
-        uses: actions/cache@v2
+        uses: actions/cache@v3
         with:
           path: ${{ steps.pip-cache.outputs.dir }}
           key:
             ${{ matrix.python-version }}-v1-${{ hashFiles('**/setup.py') }}-${{ hashFiles('**/tox.ini') }}
           restore-keys: |
             ${{ matrix.python-version }}-v1-
 
@@ -50,10 +50,10 @@
       - name: Tox tests
         run: |
           tox -v
         env:
           DJANGO: ${{ matrix.django-version }}
 
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v2
+        uses: codecov/codecov-action@v3
         with:
           name: Python ${{ matrix.python-version }}
```

### Comparing `edc-rx-0.1.3/.gitignore` & `edc-rx-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.3/.pre-commit-config.yaml` & `edc-rx-0.1.4/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 ---
 exclude: tests/etc/user-*
 
 repos:
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.4
+    rev: 1.7.5
     hooks:
       - id: bandit
         args:
           - "-x *test*.py"
 
   - repo: https://github.com/psf/black
-    rev: 22.6.0
+    rev: 23.3.0
     hooks:
       - id: black
         language_version: python3.9
 
   - repo: https://github.com/pycqa/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
       - id: flake8
         args:
           - "--config=setup.cfg"
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: requirements-txt-fixer
         files: requirements/.*\.txt$
       - id: trailing-whitespace
       - id: check-added-large-files
       - id: fix-byte-order-marker
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
       - id: detect-private-key
 
   - repo: https://github.com/adrienverge/yamllint
-    rev: v1.27.1
+    rev: v1.30.0
     hooks:
       - id: yamllint
         args:
           - "--strict"
```

### Comparing `edc-rx-0.1.3/LICENSE` & `edc-rx-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.3/PKG-INFO` & `edc-rx-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: edc-rx
-Version: 0.1.3
+Version: 0.1.4
 Summary: Microcopy model mixins in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-rx
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc rx-refill,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |codecov| |downloads|
```

### Comparing `edc-rx-0.1.3/README.rst` & `edc-rx-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.3/edc_rx/migrations/0001_initial.py` & `edc-rx-0.1.4/edc_rx/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 4.1.2 on 2022-11-29 05:42
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="RxModificationReasons",
```

### Comparing `edc-rx-0.1.3/edc_rx/model_mixins/drug_refill_model_mixin.py` & `edc-rx-0.1.4/edc_rx/model_mixins/drug_refill_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.3/edc_rx/model_mixins/drug_supply_model_mixin.py` & `edc-rx-0.1.4/edc_rx/model_mixins/drug_supply_model_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from django.core.validators import MaxValueValidator, MinValueValidator
 from django.db import models
 
 
 class DrugSupplyModelMixin(models.Model):
-
     clinic_days = models.IntegerField(
         verbose_name="Clinic",
         validators=[MinValueValidator(0), MaxValueValidator(180)],
         help_text="days",
     )
 
     club_days = models.IntegerField(
```

### Comparing `edc-rx-0.1.3/edc_rx/model_mixins/treatment_pay_methods.py` & `edc-rx-0.1.4/edc_rx/model_mixins/treatment_pay_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from django.core.validators import MinValueValidator
 from django.db import models
 from edc_constants.choices import YES_NO
 from edc_constants.constants import UNKNOWN
 
 
 class TreatmentPayMethodsModelMixin(models.Model):
-
     health_insurance = models.CharField(
         verbose_name="Does the patient have any private or work-place health insurance?",
         max_length=15,
         choices=YES_NO,
         default=UNKNOWN,
     )
```

### Comparing `edc-rx-0.1.3/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py` & `edc-rx-0.1.4/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.3/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py` & `edc-rx-0.1.4/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 class DrugSupplyInlineMixin:
-
     extra = 1
     view_on_site = False
 
     min_num = 1
     insert_after = "return_in_days"
 
     fieldsets = (
```

### Comparing `edc-rx-0.1.3/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py` & `edc-rx-0.1.4/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from django import forms
 
 from ..utils import TotalDaysMismatch, validate_total_days
 
 
 class DrugSupplyNcdModelFormMixin:
-
     list_model_cls = None
 
     def clean(self):
         cleaned_data = super().clean()
         data = dict(self.data.lists())
         rx = self.list_model_cls.objects.filter(id__in=data.get("rx") or [])
         rx_names = [obj.display_name for obj in rx]
```

### Comparing `edc-rx-0.1.3/edc_rx/tests/etc/user-rsa-local-private.pem` & `edc-rx-0.1.4/edc_rx/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.3/edc_rx/tests/etc/user-rsa-restricted-private.pem` & `edc-rx-0.1.4/edc_rx/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.3/edc_rx/utils.py` & `edc-rx-0.1.4/edc_rx/utils.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.3/edc_rx.egg-info/PKG-INFO` & `edc-rx-0.1.4/edc_rx.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: edc-rx
-Version: 0.1.3
+Version: 0.1.4
 Summary: Microcopy model mixins in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-rx
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc rx-refill,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |codecov| |downloads|
```

### Comparing `edc-rx-0.1.3/edc_rx.egg-info/SOURCES.txt` & `edc-rx-0.1.4/edc_rx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.3/pyproject.toml` & `edc-rx-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,47 +3,52 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "_version.py"
 
 [tool.black]
 line-length = 95
-target-version = ["py39"]
+target-version = ["py310"]
 extend-exclude = '''^(.*\/)*\b(migrations)\b($|\/.*$)'''
 
 [tool.isort]
 profile = "black"
-py_version = "39"
+py_version = "310"
 skip = [".tox", ".eggs", "migrations"]
 
 [tool.coverage.run]
 parallel = true
 branch = true
 source = ["edc_rx"]
 
 [tool.coverage.paths]
 source = ["edc_rx"]
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 omit = ["requirements.txt"]
+exclude_lines = [
+  "pragma: no cover",
+  "if TYPE_CHECKING:",
+]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    py{310}-dj{41,dev},
+    py{310,311}-dj{41,dev},
     lint
 
 isolated_build = true
 
 [gh-actions]
 python =
-    3.10: py310, lint
+    3.10: py310
+    3.11: py311, lint
 
 [gh-actions:env]
 DJANGO =
     4.1: dj41, lint
     dev: djdev
 
 [testenv]
```

### Comparing `edc-rx-0.1.3/runtests.py` & `edc-rx-0.1.4/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.3/setup.cfg` & `edc-rx-0.1.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 4.1
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 
 [options]
 python_requires = >=3.10
 zip_safe = False
 include_package_data = True
 packages = find:
```

