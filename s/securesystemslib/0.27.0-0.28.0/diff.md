# Comparing `tmp/securesystemslib-0.27.0.tar.gz` & `tmp/securesystemslib-0.28.0.tar.gz`

## Comparing `securesystemslib-0.27.0.tar` & `securesystemslib-0.28.0.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/.coveragerc
--rw-r--r--   0        0        0    15251 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/CHANGELOG.md
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/mypy.ini
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/pylintrc
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/requirements-dev.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/requirements-kms.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/requirements-lint.txt
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/requirements-pinned.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/requirements-sigstore.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/requirements-test.txt
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/requirements.txt
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tox.ini
--rwxr-xr-x   0        0        0      824 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/__init__.py
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/dsse.py
--rwxr-xr-x   0        0        0    17697 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/ecdsa_keys.py
--rwxr-xr-x   0        0        0    13303 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/ed25519_keys.py
--rwxr-xr-x   0        0        0     3404 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/exceptions.py
--rwxr-xr-x   0        0        0    25146 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/formats.py
--rwxr-xr-x   0        0        0    14051 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/hash.py
--rw-r--r--   0        0        0    39147 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/interface.py
--rwxr-xr-x   0        0        0    69439 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/keys.py
--rwxr-xr-x   0        0        0    44363 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/rsa_keys.py
--rwxr-xr-x   0        0        0    32217 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/schema.py
--rwxr-xr-x   0        0        0     1340 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/settings.py
--rwxr-xr-x   0        0        0     2911 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/sphincs_keys.py
--rw-r--r--   0        0        0     9911 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/storage.py
--rwxr-xr-x   0        0        0     4182 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/unittest_toolbox.py
--rw-r--r--   0        0        0    14050 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/util.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/_internal/utils.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/_vendor/README.md
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/_vendor/__init__.py
--rwxr-xr-x   0        0        0     1026 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/_vendor/test-ed25519-upstream.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/_vendor/ed25519/.gitignore
--rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/_vendor/ed25519/LICENSE
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/_vendor/ed25519/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/_vendor/ed25519/__init__.py
--rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/_vendor/ed25519/ed25519.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/_vendor/ed25519/science.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/_vendor/ed25519/test_ed25519.py
--rw-r--r--   0        0        0  2427904 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/_vendor/ed25519/test_data/ed25519
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/gpg/__init__.py
--rw-r--r--   0        0        0    35971 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/gpg/common.py
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/gpg/constants.py
--rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/gpg/dsa.py
--rw-r--r--   0        0        0     7647 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/gpg/eddsa.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/gpg/exceptions.py
--rw-r--r--   0        0        0    11954 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/gpg/functions.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/gpg/handlers.py
--rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/gpg/rsa.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/gpg/util.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/signer/__init__.py
--rw-r--r--   0        0        0     7464 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/signer/_gcp_signer.py
--rw-r--r--   0        0        0     7858 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/signer/_gpg_signer.py
--rw-r--r--   0        0        0    13345 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/signer/_hsm_signer.py
--rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/signer/_key.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/signer/_signature.py
--rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/signer/_signer.py
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/securesystemslib/signer/_sigstore_signer.py
--rwxr-xr-x   0        0        0        1 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/__init__.py
--rwxr-xr-x   0        0        0      729 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/aggregate_tests.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/check_gpg_available.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/check_kms_signers.py
--rw-r--r--   0        0        0    15135 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/check_public_interfaces.py
--rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/check_public_interfaces_gpg.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/check_sigstore_signer.py
--rw-r--r--   0        0        0     5551 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/test_dsse.py
--rwxr-xr-x   0        0        0     7348 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/test_ecdsa_keys.py
--rwxr-xr-x   0        0        0     5782 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/test_ed25519_keys.py
--rwxr-xr-x   0        0        0     1314 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/test_exceptions.py
--rwxr-xr-x   0        0        0    14755 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/test_formats.py
--rw-r--r--   0        0        0    36713 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/test_gpg.py
--rwxr-xr-x   0        0        0    12542 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/test_hash.py
--rw-r--r--   0        0        0     6078 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/test_hsm_signer.py
--rwxr-xr-x   0        0        0    39040 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/test_interface.py
--rwxr-xr-x   0        0        0    33187 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/test_keys.py
--rwxr-xr-x   0        0        0    14765 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/test_rsa_keys.py
--rwxr-xr-x   0        0        0    17839 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/test_schema.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/test_signer.py
--rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/test_storage.py
--rw-r--r--   0        0        0    14283 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/test_util.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/data/keystore/ecdsa_key
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/data/keystore/ecdsa_key.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/data/keystore/ed25519_key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/data/keystore/ed25519_key.pub
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/data/keystore/no_key
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/data/keystore/rsa_key
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/data/keystore/rsa_key.pub
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.pem
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/dsa/pubring.gpg
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/dsa/random_seed
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/dsa/secring.gpg
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/dsa/trustdb.gpg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/eddsa/pubring.gpg
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/eddsa/pubring.kbx
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/eddsa/pubring.kbx~
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/eddsa/short.sig
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/eddsa/trustdb.gpg
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/eddsa/openpgp-revocs.d/4E630F84838BF6F7447B830B22692F5FEA9E2DD2.rev
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/eddsa/private-keys-v1.d/672E9A973B33784B4579F316820434E5631C086A.key
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/rsa/7B3ABB26B97B655AB9296BD15B0BD02E1C768C43.ssh
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/rsa/8288EF560ED3795F9DF2C0DB56193089B285DA58.ssh
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/rsa/8465A1E2E0FB2B40ADB2478E18FB3F537E0C8A17.ssh
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/rsa/E8AC80C924116DABB51D4B987CB07D6D2C199C7C.raw
--rw-r--r--   0        0        0     6792 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/rsa/F557D0FF451DEF45372591429EA70BD13D883381.raw
--rw-r--r--   0        0        0    17740 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/rsa/pubring.gpg
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/rsa/random_seed
--rw-r--r--   0        0        0    27893 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/rsa/secring.gpg
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/tests/gpg_keyrings/rsa/trustdb.gpg
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/LICENSE
--rw-r--r--   0        0        0    12082 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/README.rst
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/pyproject.toml
--rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 securesystemslib-0.27.0/PKG-INFO
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/.coveragerc
+-rw-r--r--   0        0        0    15820 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/CHANGELOG.md
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/mypy.ini
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/pylintrc
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/requirements-dev.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/requirements-kms.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/requirements-lint.txt
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/requirements-pinned.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/requirements-sigstore.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/requirements-test.txt
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/requirements.txt
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tox.ini
+-rwxr-xr-x   0        0        0      824 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/__init__.py
+-rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/dsse.py
+-rwxr-xr-x   0        0        0    17697 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/ecdsa_keys.py
+-rwxr-xr-x   0        0        0    13303 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/ed25519_keys.py
+-rwxr-xr-x   0        0        0     3404 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/exceptions.py
+-rwxr-xr-x   0        0        0    24992 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/formats.py
+-rwxr-xr-x   0        0        0    13945 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/hash.py
+-rw-r--r--   0        0        0    39124 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/interface.py
+-rwxr-xr-x   0        0        0    69322 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/keys.py
+-rwxr-xr-x   0        0        0    44340 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/rsa_keys.py
+-rwxr-xr-x   0        0        0    32194 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/schema.py
+-rwxr-xr-x   0        0        0     1317 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/settings.py
+-rwxr-xr-x   0        0        0     2911 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/sphincs_keys.py
+-rw-r--r--   0        0        0     9911 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/storage.py
+-rwxr-xr-x   0        0        0     4182 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/unittest_toolbox.py
+-rw-r--r--   0        0        0    14050 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/util.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/_internal/utils.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/_vendor/README.md
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/_vendor/__init__.py
+-rwxr-xr-x   0        0        0     1026 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/_vendor/test-ed25519-upstream.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/_vendor/ed25519/.gitignore
+-rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/_vendor/ed25519/LICENSE
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/_vendor/ed25519/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/_vendor/ed25519/__init__.py
+-rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/_vendor/ed25519/ed25519.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/_vendor/ed25519/science.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/_vendor/ed25519/test_ed25519.py
+-rw-r--r--   0        0        0  2427904 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/_vendor/ed25519/test_data/ed25519
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/gpg/__init__.py
+-rw-r--r--   0        0        0    35971 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/gpg/common.py
+-rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/gpg/constants.py
+-rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/gpg/dsa.py
+-rw-r--r--   0        0        0     7647 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/gpg/eddsa.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/gpg/exceptions.py
+-rw-r--r--   0        0        0    11954 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/gpg/functions.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/gpg/handlers.py
+-rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/gpg/rsa.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/gpg/util.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/signer/__init__.py
+-rw-r--r--   0        0        0     7423 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/signer/_gcp_signer.py
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/signer/_gpg_signer.py
+-rw-r--r--   0        0        0    13280 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/signer/_hsm_signer.py
+-rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/signer/_key.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/signer/_signature.py
+-rw-r--r--   0        0        0     8390 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/signer/_signer.py
+-rw-r--r--   0        0        0     7456 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/securesystemslib/signer/_sigstore_signer.py
+-rwxr-xr-x   0        0        0      333 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/__init__.py
+-rwxr-xr-x   0        0        0      706 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/aggregate_tests.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/check_gpg_available.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/check_kms_signers.py
+-rw-r--r--   0        0        0    16578 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/check_public_interfaces.py
+-rw-r--r--   0        0        0     8395 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/check_public_interfaces_gpg.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/check_sigstore_signer.py
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/test_dsse.py
+-rwxr-xr-x   0        0        0     7324 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/test_ecdsa_keys.py
+-rwxr-xr-x   0        0        0     5758 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/test_ed25519_keys.py
+-rwxr-xr-x   0        0        0     1291 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/test_exceptions.py
+-rwxr-xr-x   0        0        0    14102 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/test_formats.py
+-rw-r--r--   0        0        0    36690 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/test_gpg.py
+-rwxr-xr-x   0        0        0    11694 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/test_hash.py
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/test_hsm_signer.py
+-rwxr-xr-x   0        0        0    39239 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/test_interface.py
+-rwxr-xr-x   0        0        0    33164 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/test_keys.py
+-rwxr-xr-x   0        0        0    14742 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/test_rsa_keys.py
+-rwxr-xr-x   0        0        0    17816 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/test_schema.py
+-rw-r--r--   0        0        0    29482 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/test_signer.py
+-rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/test_storage.py
+-rw-r--r--   0        0        0    14260 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/test_util.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/data/keystore/ecdsa_key
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/data/keystore/ecdsa_key.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/data/keystore/ed25519_key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/data/keystore/ed25519_key.pub
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/data/keystore/no_key
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/data/keystore/rsa_key
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/data/keystore/rsa_key.pub
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.pem
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/dsa/pubring.gpg
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/dsa/random_seed
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/dsa/secring.gpg
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/dsa/trustdb.gpg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/eddsa/pubring.gpg
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/eddsa/pubring.kbx
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/eddsa/pubring.kbx~
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/eddsa/short.sig
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/eddsa/trustdb.gpg
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/eddsa/openpgp-revocs.d/4E630F84838BF6F7447B830B22692F5FEA9E2DD2.rev
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/eddsa/private-keys-v1.d/672E9A973B33784B4579F316820434E5631C086A.key
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/rsa/7B3ABB26B97B655AB9296BD15B0BD02E1C768C43.ssh
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/rsa/8288EF560ED3795F9DF2C0DB56193089B285DA58.ssh
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/rsa/8465A1E2E0FB2B40ADB2478E18FB3F537E0C8A17.ssh
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/rsa/E8AC80C924116DABB51D4B987CB07D6D2C199C7C.raw
+-rw-r--r--   0        0        0     6792 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/rsa/F557D0FF451DEF45372591429EA70BD13D883381.raw
+-rw-r--r--   0        0        0    17740 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/rsa/pubring.gpg
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/rsa/random_seed
+-rw-r--r--   0        0        0    27893 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/rsa/secring.gpg
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/tests/gpg_keyrings/rsa/trustdb.gpg
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/LICENSE
+-rw-r--r--   0        0        0    12082 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/README.rst
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/pyproject.toml
+-rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 securesystemslib-0.28.0/PKG-INFO
```

### Comparing `securesystemslib-0.27.0/CHANGELOG.md` & `securesystemslib-0.28.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,31 @@
 # Changelog
 
+## securesystemslib v0.28.0
+
+### Added
+* Signer: auto-keyid helper (#557)
+* Signer: de/serialization helpers (#558)
+* Signer: tests (#555, #556)
+* Sigstore Signer: import methods (#535)
+
+### Changed
+* HSMSigner: pre-hash data (#548)
+* GCP Signer, HSM Signer: auto-keyid computation (#557)
+* DSSE: serialize signature data as base64 for compliance (#565)
+
+### Removed
+* Obsolete shebangs (#544, #545)
+* Outdated schemes: md5, sha1 (#554)
+
+### Fixed
+* Various test and CI fixes (#538, #541, #542, #543, #546)
+* Minor SSlibKey.verify_signature error handling bug (#556)
+
+
 ## securesystemslib v0.27.0
 
 ### Added
 * EXPERIMENTAL DSSE implementation (#487)
 * EXPERIMENTAL sigstore signer and verifier (#522)
 * Minimal TUF/in-toto spec-compliant GPG verifier (#488)
 * API-typical 'import' and 'from URI' GPG signer methods (#488)
```

### Comparing `securesystemslib-0.27.0/mypy.ini` & `securesystemslib-0.28.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/pylintrc` & `securesystemslib-0.28.0/pylintrc`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/requirements-pinned.txt` & `securesystemslib-0.28.0/requirements-pinned.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 asn1crypto==1.5.1
     # via -r requirements.txt
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
     #   pyspx
-cryptography==39.0.2
+cryptography==40.0.2
     # via -r requirements.txt
 pycparser==2.21
     # via cffi
-pykcs11==1.5.11
+pykcs11==1.5.12
     # via -r requirements.txt
 pynacl==1.5.0
     # via -r requirements.txt
 pyspx==0.5.0 ; platform_system != "Windows"
     # via -r requirements.txt
```

### Comparing `securesystemslib-0.27.0/tox.ini` & `securesystemslib-0.28.0/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 deps =
     -r{toxinidir}/requirements-pinned.txt
     -r{toxinidir}/requirements-test.txt
 
 commands =
     python -m tests.check_gpg_available
     coverage run tests/aggregate_tests.py
-    coverage report -m --fail-under 90
+    coverage report -m --fail-under 85
 
 [testenv:purepy311]
 deps =
 
 commands =
     python -m tests.check_gpg_available
     python -m tests.check_public_interfaces
```

### Comparing `securesystemslib-0.27.0/securesystemslib/__init__.py` & `securesystemslib-0.28.0/securesystemslib/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=missing-module-docstring
 import logging
 
-__version__ = "0.27.0"
+__version__ = "0.28.0"
 
 # Configure a basic 'securesystemslib' top-level logger with a StreamHandler
 # (print to console) and the WARNING log level (print messages of type
 # warning, error or critical). This is similar to what 'logging.basicConfig'
 # would do with the root logger. All 'securesystemslib.*' loggers default to
 # this top-level logger and thus may be configured (e.g. formatted, silenced,
 # etc.) with it. It can be accessed via logging.getLogger('securesystemslib').
```

### Comparing `securesystemslib-0.27.0/securesystemslib/dsse.py` & `securesystemslib-0.28.0/securesystemslib/dsse.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,29 +54,34 @@
         Returns:
             A "Envelope" instance.
         """
 
         payload = b64dec(data["payload"])
         payload_type = data["payloadType"]
 
-        signatures = [
-            Signature.from_dict(signature) for signature in data["signatures"]
-        ]
+        signatures = []
+        for signature in data["signatures"]:
+            signature["sig"] = b64dec(signature["sig"]).hex()
+            signatures.append(Signature.from_dict(signature))
 
         return cls(payload, payload_type, signatures)
 
     def to_dict(self) -> dict:
         """Returns the JSON-serializable dictionary representation of self."""
 
+        signatures = []
+        for signature in self.signatures:
+            sig_dict = signature.to_dict()
+            sig_dict["sig"] = b64enc(bytes.fromhex(sig_dict["sig"]))
+            signatures.append(sig_dict)
+
         return {
             "payload": b64enc(self.payload),
             "payloadType": self.payload_type,
-            "signatures": [
-                signature.to_dict() for signature in self.signatures
-            ],
+            "signatures": signatures,
         }
 
     def pae(self) -> bytes:
         """Pre-Auth-Encoding byte sequence of self."""
 
         return b"DSSEv1 %d %b %d %b" % (
             len(self.payload_type),
```

### Comparing `securesystemslib-0.27.0/securesystemslib/ecdsa_keys.py` & `securesystemslib-0.28.0/securesystemslib/ecdsa_keys.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/ed25519_keys.py` & `securesystemslib-0.28.0/securesystemslib/ed25519_keys.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/exceptions.py` & `securesystemslib-0.28.0/securesystemslib/exceptions.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/formats.py` & `securesystemslib-0.28.0/securesystemslib/formats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """
 <Program Name>
   formats.py
 
 <Author>
   Geremy Condra
   Vladimir Diaz <vladimir.v.diaz@gmail.com>
@@ -139,16 +137,14 @@
 # A text string.  For instance, a string entered by the user.
 TEXT_SCHEMA = SCHEMA.AnyString()
 
 # Supported hash algorithms.
 HASHALGORITHMS_SCHEMA = SCHEMA.ListOf(
     SCHEMA.OneOf(
         [
-            SCHEMA.String("md5"),
-            SCHEMA.String("sha1"),
             SCHEMA.String("sha224"),
             SCHEMA.String("sha256"),
             SCHEMA.String("sha384"),
             SCHEMA.String("sha512"),
             SCHEMA.String("blake2s"),
             SCHEMA.String("blake2b"),
             SCHEMA.String("blake2b-256"),
@@ -250,20 +246,16 @@
 
 # A list of securesystemslib key objects.
 ANYKEYLIST_SCHEMA = SCHEMA.ListOf(ANYKEY_SCHEMA)
 
 # RSA signature schemes.
 RSA_SCHEME_SCHEMA = SCHEMA.OneOf(
     [
-        SCHEMA.RegularExpression(
-            r"rsassa-pss-(md5|sha1|sha224|sha256|sha384|sha512)"
-        ),
-        SCHEMA.RegularExpression(
-            r"rsa-pkcs1v15-(md5|sha1|sha224|sha256|sha384|sha512)"
-        ),
+        SCHEMA.RegularExpression(r"rsassa-pss-(sha224|sha256|sha384|sha512)"),
+        SCHEMA.RegularExpression(r"rsa-pkcs1v15-(sha224|sha256|sha384|sha512)"),
     ]
 )
 
 # An RSA securesystemslib key.
 RSAKEY_SCHEMA = SCHEMA.Object(
     object_name="RSAKEY_SCHEMA",
     keytype=SCHEMA.String("rsa"),
```

### Comparing `securesystemslib-0.27.0/securesystemslib/hash.py` & `securesystemslib-0.28.0/securesystemslib/hash.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python2
 """
 <Program Name>
   hash.py
 
 <Author>
   Vladimir Diaz <vladimir.v.diaz@gmail.com>
 
@@ -38,16 +37,14 @@
     import binascii
 
     from cryptography.hazmat.backends import default_backend
     from cryptography.hazmat.primitives import hashes as _pyca_hashes
 
     # Dictionary of `pyca/cryptography` supported hash algorithms.
     PYCA_DIGEST_OBJECTS_CACHE = {
-        "md5": _pyca_hashes.MD5,
-        "sha1": _pyca_hashes.SHA1,
         "sha224": _pyca_hashes.SHA224,
         "sha256": _pyca_hashes.SHA256,
         "sha384": _pyca_hashes.SHA384,
         "sha512": _pyca_hashes.SHA512,
     }
 
     SUPPORTED_LIBRARIES.append("pyca_crypto")
@@ -139,15 +136,15 @@
 
       # Added hash routines by this module.
       digest_object = securesystemslib.hash.digest_fileobject(file_object)
       digest_object = securesystemslib.hash.digest_filename(filename)
 
     <Arguments>
       algorithm:
-        The hash algorithm (e.g., 'md5', 'sha1', 'sha256').
+        The hash algorithm (e.g., 'sha256', 'sha512').
 
       hash_library:
         The crypto library to use for the given hash algorithm (e.g., 'hashlib').
 
     <Exceptions>
       securesystemslib.exceptions.FormatError, if the arguments are
       improperly formatted.
@@ -227,15 +224,15 @@
 
     <Arguments>
       file_object:
         File object whose contents will be used as the data
         to update the hash of a digest object to be returned.
 
       algorithm:
-        The hash algorithm (e.g., 'md5', 'sha1', 'sha256').
+        The hash algorithm (e.g., 'sha256', 'sha512').
 
       hash_library:
         The library providing the hash algorithms (e.g., 'hashlib').
 
       normalize_line_endings: (default False)
         Whether or not to normalize line endings for cross-platform support.
         Note that this results in ambiguous hashes (e.g. 'abc\n' and 'abc\r\n'
@@ -326,15 +323,15 @@
       specified by filename, and then return it to the caller.
 
     <Arguments>
       filename:
         The filename belonging to the file object to be used.
 
       algorithm:
-        The hash algorithm (e.g., 'md5', 'sha1', 'sha256').
+        The hash algorithm (e.g., 'sha256', 'sha512').
 
       hash_library:
         The library providing the hash algorithms (e.g., 'hashlib').
 
       normalize_line_endings:
         Whether or not to normalize line endings for cross-platform support.
```

### Comparing `securesystemslib-0.27.0/securesystemslib/interface.py` & `securesystemslib-0.28.0/securesystemslib/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """
 <Program Name>
   interface.py
 
 <Author>
   Vladimir Diaz <vladimir.v.diaz@gmail.com>
```

### Comparing `securesystemslib-0.27.0/securesystemslib/keys.py` & `securesystemslib-0.28.0/securesystemslib/keys.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """
 <Program Name>
   keys.py
 
 <Author>
   Vladimir Diaz <vladimir.v.diaz@gmail.com>
 
@@ -71,22 +69,18 @@
 # http://www.emc.com/emc-plus/rsa-labs/historical/twirl-and-rsa-key-size.htm#table1
 # According to the document above, revised May 6, 2003, RSA keys of
 # size 3072 provide security through 2031 and beyond.
 _DEFAULT_RSA_KEY_BITS = 3072
 
 
 RSA_SIGNATURE_SCHEMES = [
-    "rsassa-pss-md5",
-    "rsassa-pss-sha1",
     "rsassa-pss-sha224",
     "rsassa-pss-sha256",
     "rsassa-pss-sha384",
     "rsassa-pss-sha512",
-    "rsa-pkcs1v15-md5",
-    "rsa-pkcs1v15-sha1",
     "rsa-pkcs1v15-sha224",
     "rsa-pkcs1v15-sha256",
     "rsa-pkcs1v15-sha384",
     "rsa-pkcs1v15-sha512",
 ]
 
 logger = logging.getLogger(__name__)
```

### Comparing `securesystemslib-0.27.0/securesystemslib/rsa_keys.py` & `securesystemslib-0.28.0/securesystemslib/rsa_keys.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """
 <Program Name>
   rsa_keys.py
 
 <Author>
   Vladimir Diaz <vladimir.v.diaz@gmail.com>
```

### Comparing `securesystemslib-0.27.0/securesystemslib/schema.py` & `securesystemslib-0.28.0/securesystemslib/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """
 <Program Name>
   schema.py
 
 <Author>
   Geremy Condra
   Vladimir Diaz <vladimir.v.diaz@gmail.com>
```

### Comparing `securesystemslib-0.27.0/securesystemslib/settings.py` & `securesystemslib-0.28.0/securesystemslib/settings.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """
 <Program Name>
   settings.py
 
 <Author>
   Vladimir Diaz <vladimir.v.diaz@gmail.com>
```

### Comparing `securesystemslib-0.27.0/securesystemslib/sphincs_keys.py` & `securesystemslib-0.28.0/securesystemslib/sphincs_keys.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/storage.py` & `securesystemslib-0.28.0/securesystemslib/storage.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/unittest_toolbox.py` & `securesystemslib-0.28.0/securesystemslib/unittest_toolbox.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/util.py` & `securesystemslib-0.28.0/securesystemslib/util.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/_internal/utils.py` & `securesystemslib-0.28.0/securesystemslib/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/_vendor/README.md` & `securesystemslib-0.28.0/securesystemslib/_vendor/README.md`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/_vendor/test-ed25519-upstream.sh` & `securesystemslib-0.28.0/securesystemslib/_vendor/test-ed25519-upstream.sh`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/_vendor/ed25519/LICENSE` & `securesystemslib-0.28.0/securesystemslib/_vendor/ed25519/LICENSE`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/_vendor/ed25519/README.rst` & `securesystemslib-0.28.0/securesystemslib/_vendor/ed25519/README.rst`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/_vendor/ed25519/ed25519.py` & `securesystemslib-0.28.0/securesystemslib/_vendor/ed25519/ed25519.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/_vendor/ed25519/science.py` & `securesystemslib-0.28.0/securesystemslib/_vendor/ed25519/science.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/_vendor/ed25519/test_ed25519.py` & `securesystemslib-0.28.0/securesystemslib/_vendor/ed25519/test_ed25519.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/_vendor/ed25519/test_data/ed25519` & `securesystemslib-0.28.0/securesystemslib/_vendor/ed25519/test_data/ed25519`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/gpg/__init__.py` & `securesystemslib-0.28.0/securesystemslib/gpg/__init__.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/gpg/common.py` & `securesystemslib-0.28.0/securesystemslib/gpg/common.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/gpg/constants.py` & `securesystemslib-0.28.0/securesystemslib/gpg/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,24 +16,27 @@
   handling
 """
 import functools
 import logging
 import os
 import shlex
 import subprocess  # nosec
-from typing import List
+from typing import List, Optional
 
 log = logging.getLogger(__name__)
 
 GPG_TIMEOUT = 10
 
 
 @functools.lru_cache(maxsize=3)
-def is_available_gnupg(gnupg: str, timeout=GPG_TIMEOUT) -> bool:
+def is_available_gnupg(gnupg: str, timeout: Optional[int] = None) -> bool:
     """Returns whether gnupg points to a gpg binary."""
+    if timeout is None:
+        timeout = GPG_TIMEOUT
+
     gpg_version_cmd = shlex.split(f"{gnupg} --version")
     try:
         subprocess.run(  # nosec
             gpg_version_cmd,
             capture_output=True,
             timeout=timeout,
             check=True,
```

### Comparing `securesystemslib-0.27.0/securesystemslib/gpg/dsa.py` & `securesystemslib-0.28.0/securesystemslib/gpg/dsa.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/gpg/eddsa.py` & `securesystemslib-0.28.0/securesystemslib/gpg/eddsa.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/gpg/exceptions.py` & `securesystemslib-0.28.0/securesystemslib/gpg/exceptions.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/gpg/functions.py` & `securesystemslib-0.28.0/securesystemslib/gpg/functions.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/gpg/handlers.py` & `securesystemslib-0.28.0/securesystemslib/gpg/handlers.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/gpg/rsa.py` & `securesystemslib-0.28.0/securesystemslib/gpg/rsa.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/gpg/util.py` & `securesystemslib-0.28.0/securesystemslib/gpg/util.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/signer/__init__.py` & `securesystemslib-0.28.0/securesystemslib/signer/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,22 +32,18 @@
 KEY_FOR_TYPE_AND_SCHEME.update(
     {
         ("ecdsa", "ecdsa-sha2-nistp256"): SSlibKey,
         ("ecdsa", "ecdsa-sha2-nistp384"): SSlibKey,
         ("ecdsa-sha2-nistp256", "ecdsa-sha2-nistp256"): SSlibKey,
         ("ecdsa-sha2-nistp384", "ecdsa-sha2-nistp384"): SSlibKey,
         ("ed25519", "ed25519"): SSlibKey,
-        ("rsa", "rsassa-pss-md5"): SSlibKey,
-        ("rsa", "rsassa-pss-sha1"): SSlibKey,
         ("rsa", "rsassa-pss-sha224"): SSlibKey,
         ("rsa", "rsassa-pss-sha256"): SSlibKey,
         ("rsa", "rsassa-pss-sha384"): SSlibKey,
         ("rsa", "rsassa-pss-sha512"): SSlibKey,
-        ("rsa", "rsa-pkcs1v15-md5"): SSlibKey,
-        ("rsa", "rsa-pkcs1v15-sha1"): SSlibKey,
         ("rsa", "rsa-pkcs1v15-sha224"): SSlibKey,
         ("rsa", "rsa-pkcs1v15-sha256"): SSlibKey,
         ("rsa", "rsa-pkcs1v15-sha384"): SSlibKey,
         ("rsa", "rsa-pkcs1v15-sha512"): SSlibKey,
         ("sphincs", "sphincs-shake-128s"): SSlibKey,
         ("rsa", "pgp+rsa-pkcsv1.5"): GPGKey,
         ("dsa", "pgp+dsa-fips-180-2"): GPGKey,
```

### Comparing `securesystemslib-0.27.0/securesystemslib/signer/_gcp_signer.py` & `securesystemslib-0.28.0/securesystemslib/signer/_gcp_signer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import logging
 from typing import Optional, Tuple
 from urllib import parse
 
 import securesystemslib.hash as sslib_hash
 from securesystemslib import exceptions
-from securesystemslib.keys import _get_keyid
 from securesystemslib.signer._key import Key
 from securesystemslib.signer._signer import (
     SecretsHandler,
     Signature,
     Signer,
     SSlibKey,
 )
@@ -100,15 +99,15 @@
             keytype, scheme = cls._get_keytype_and_scheme(kms_pubkey.algorithm)
         except KeyError as e:
             raise exceptions.UnsupportedAlgorithmError(
                 f"{kms_pubkey.algorithm} is not a supported signing algorithm"
             ) from e
 
         keyval = {"public": kms_pubkey.pem}
-        keyid = _get_keyid(keytype, scheme, keyval)
+        keyid = cls._get_keyid(keytype, scheme, keyval)
         public_key = SSlibKey(keyid, keytype, scheme, keyval)
 
         return f"{cls.SCHEME}:{gcp_keyid}", public_key
 
     @staticmethod
     def _get_keytype_and_scheme(algorithm: int) -> Tuple[str, str]:
         """Return keytype and scheme for the KMS algorithm enum"""
```

### Comparing `securesystemslib-0.27.0/securesystemslib/signer/_gpg_signer.py` & `securesystemslib-0.28.0/securesystemslib/signer/_gpg_signer.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,27 +28,19 @@
         keyval: Opaque key content.
         unrecognized_fields: Dictionary of all attributes that are not managed
             by Securesystemslib
     """
 
     @classmethod
     def from_dict(cls, keyid: str, key_dict: Dict[str, Any]) -> "GPGKey":
-        keytype = key_dict.pop("keytype")
-        scheme = key_dict.pop("scheme")
-        keyval = key_dict.pop("keyval")
-
+        keytype, scheme, keyval = cls._from_dict(key_dict)
         return cls(keyid, keytype, scheme, keyval, key_dict)
 
     def to_dict(self) -> Dict:
-        return {
-            "keytype": self.keytype,
-            "scheme": self.scheme,
-            "keyval": self.keyval,
-            **self.unrecognized_fields,
-        }
+        return self._to_dict()
 
     def verify_signature(self, signature: Signature, data: bytes) -> None:
         try:
             if not gpg.verify_signature(
                 GPGSigner._sig_to_legacy_dict(  # pylint: disable=protected-access
                     signature
                 ),
```

### Comparing `securesystemslib-0.27.0/securesystemslib/signer/_hsm_signer.py` & `securesystemslib-0.28.0/securesystemslib/signer/_hsm_signer.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import binascii
 from contextlib import contextmanager
 from typing import Dict, Iterator, List, Optional, Tuple
 from urllib import parse
 
 from securesystemslib import KEY_TYPE_ECDSA
 from securesystemslib.exceptions import UnsupportedLibraryError
-from securesystemslib.keys import _get_keyid
+from securesystemslib.hash import digest
 from securesystemslib.signer._key import Key, SSlibKey
 from securesystemslib.signer._signature import Signature
 from securesystemslib.signer._signer import SecretsHandler, Signer
 
 # pylint: disable=wrong-import-position
 CRYPTO_IMPORT_ERROR = None
 try:
@@ -40,21 +40,14 @@
 
 except ImportError:
     CRYPTO_IMPORT_ERROR = "'cryptography' required"
 
 PYKCS11_IMPORT_ERROR = None
 try:
     from PyKCS11 import PyKCS11
-
-    # TODO: Don't hardcode schemes
-    _MECHANISM_FOR_SCHEME = {
-        "ecdsa-sha2-nistp256": PyKCS11.Mechanism(PyKCS11.CKM_ECDSA_SHA256),
-        "ecdsa-sha2-nistp384": PyKCS11.Mechanism(PyKCS11.CKM_ECDSA_SHA384),
-    }
-
 except ImportError:
     PYKCS11_IMPORT_ERROR = "'PyKCS11' required"
 
 ASN1_IMPORT_ERROR = None
 try:
     from asn1crypto.keys import (  # pylint: disable=import-error
         ECDomainParameters,
@@ -137,18 +130,20 @@
     ):
         if CRYPTO_IMPORT_ERROR:
             raise UnsupportedLibraryError(CRYPTO_IMPORT_ERROR)
 
         if PYKCS11_IMPORT_ERROR:
             raise UnsupportedLibraryError(PYKCS11_IMPORT_ERROR)
 
-        if public_key.scheme not in _MECHANISM_FOR_SCHEME:
+        if public_key.scheme not in [
+            "ecdsa-sha2-nistp256",
+            "ecdsa-sha2-nistp384",
+        ]:
             raise ValueError(f"unsupported scheme {public_key.scheme}")
 
-        self._mechanism = _MECHANISM_FOR_SCHEME[public_key.scheme]
         self.hsm_keyid = hsm_keyid
         self.token_filter = token_filter
         self.public_key = public_key
         self.pin_handler = pin_handler
 
     @staticmethod
     def _find_pkcs_slot(filters: Dict[str, str]) -> int:
@@ -322,15 +317,15 @@
                 serialization.PublicFormat.SubjectPublicKeyInfo,
             )
             .decode()
         )
 
         keyval = {"public": public_pem}
         scheme = _SCHEME_FOR_CURVE[curve]
-        keyid = _get_keyid(KEY_TYPE_ECDSA, scheme, keyval)
+        keyid = cls._get_keyid(KEY_TYPE_ECDSA, scheme, keyval)
         key = SSlibKey(keyid, KEY_TYPE_ECDSA, scheme, keyval)
 
         return uri, key
 
     @classmethod
     def from_priv_key_uri(
         cls,
@@ -363,21 +358,26 @@
         Raises:
             ValueError: No compatible key for ``hsm_keyid`` found on HSM.
             PyKCS11.PyKCS11Error: Various HSM communication errors.
 
         Returns:
             Signature.
         """
+
+        hasher = digest(algorithm=f"sha{self.public_key.scheme[-3:]}")
+        hasher.update(payload)
+
         pin = self.pin_handler(self.SECRETS_HANDLER_MSG)
         with self._get_session(self.token_filter) as session:
             session.login(pin)
             key = self._find_key(
                 session, self.hsm_keyid, PyKCS11.CKO_PRIVATE_KEY
             )
-            signature = session.sign(key, payload, self._mechanism)
+            mechanism = PyKCS11.Mechanism(PyKCS11.CKM_ECDSA)
+            signature = session.sign(key, hasher.digest(), mechanism)
             session.logout()
 
         # The PKCS11 signature octets correspond to the concatenation of the ECDSA
         # values r and s, both represented as an octet string of equal length of at
         # most nLen with the most significant byte first (i.e. big endian)
         # https://docs.oasis-open.org/pkcs11/pkcs11-curr/v3.0/cs01/pkcs11-curr-v3.0-cs01.html#_Toc30061178
         r_s_len = int(len(signature) / 2)
```

### Comparing `securesystemslib-0.27.0/securesystemslib/signer/_key.py` & `securesystemslib-0.28.0/securesystemslib/signer/_key.py`

 * *Files 12% similar despite different names*

```diff
@@ -97,14 +97,40 @@
     def to_dict(self) -> Dict[str, Any]:
         """Returns a serialization dict.
 
         Key implementations must override this serialization helper.
         """
         raise NotImplementedError
 
+    def _to_dict(self) -> Dict[str, Any]:
+        """Serialization helper to add base Key fields to a dict.
+
+        Key implementations may call this in their to_dict, which they must
+        still provide, in order to avoid unnoticed serialization accidents.
+        """
+        return {
+            "keytype": self.keytype,
+            "scheme": self.scheme,
+            "keyval": self.keyval,
+            **self.unrecognized_fields,
+        }
+
+    @staticmethod
+    def _from_dict(key_dict: Dict[str, Any]) -> Tuple[str, str, Dict[str, Any]]:
+        """Deserialization helper to pop base Key fields off the dict.
+
+        Key implementations may call this in their from_dict, in order to parse
+        out common fields. But they have to create the Key instance themselves.
+        """
+        keytype = key_dict.pop("keytype")
+        scheme = key_dict.pop("scheme")
+        keyval = key_dict.pop("keyval")
+
+        return keytype, scheme, keyval
+
     @abstractmethod
     def verify_signature(self, signature: Signature, data: bytes) -> None:
         """Raises if verification of signature over data fails.
 
         Args:
             signature: Signature object.
             data: Payload bytes.
@@ -139,31 +165,24 @@
             key_dict["keytype"],
             key_dict["scheme"],
             {"public": key_dict["keyval"]["public"]},
         )
 
     @classmethod
     def from_dict(cls, keyid: str, key_dict: Dict[str, Any]) -> "SSlibKey":
-        keytype = key_dict.pop("keytype")
-        scheme = key_dict.pop("scheme")
-        keyval = key_dict.pop("keyval")
+        keytype, scheme, keyval = cls._from_dict(key_dict)
 
         if "public" not in keyval or not isinstance(keyval["public"], str):
             raise ValueError(f"public key string required for scheme {scheme}")
 
         # All fields left in the key_dict are unrecognized.
         return cls(keyid, keytype, scheme, keyval, key_dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        return {
-            "keytype": self.keytype,
-            "scheme": self.scheme,
-            "keyval": self.keyval,
-            **self.unrecognized_fields,
-        }
+        return self._to_dict()
 
     def verify_signature(self, signature: Signature, data: bytes) -> None:
         try:
             if not sslib_keys.verify_signature(
                 self.to_securesystemslib_key(),
                 signature.to_dict(),
                 data,
@@ -171,12 +190,13 @@
                 raise exceptions.UnverifiedSignatureError(
                     f"Failed to verify signature by {self.keyid}"
                 )
         except (
             exceptions.CryptoError,
             exceptions.FormatError,
             exceptions.UnsupportedAlgorithmError,
+            exceptions.UnsupportedLibraryError,
         ) as e:
             logger.info("Key %s failed to verify sig: %s", self.keyid, str(e))
             raise exceptions.VerificationError(
                 f"Unknown failure to verify signature by {self.keyid}"
             ) from e
```

### Comparing `securesystemslib-0.27.0/securesystemslib/signer/_signature.py` & `securesystemslib-0.28.0/securesystemslib/signer/_signature.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/securesystemslib/signer/_signer.py` & `securesystemslib-0.28.0/securesystemslib/signer/_signer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Signer interface and the default implementations"""
 
 import logging
 import os
 from abc import ABCMeta, abstractmethod
-from typing import Callable, Dict, Optional, Type
+from typing import Any, Callable, Dict, Optional, Type
 from urllib import parse
 
 import securesystemslib.keys as sslib_keys
+from securesystemslib.formats import encode_canonical
+from securesystemslib.hash import digest
 from securesystemslib.signer._key import Key, SSlibKey
 from securesystemslib.signer._signature import Signature
 
 logger = logging.getLogger(__name__)
 
 # NOTE Signer dispatch table is defined here so it's usable by Signer,
 # but is populated in __init__.py (and can be appended by users).
@@ -113,14 +115,28 @@
             raise ValueError(f"Unsupported private key scheme {scheme}")
 
         signer = SIGNER_FOR_URI_SCHEME[scheme]
         return signer.from_priv_key_uri(
             priv_key_uri, public_key, secrets_handler
         )
 
+    @staticmethod
+    def _get_keyid(keytype: str, scheme, keyval: Dict[str, Any]) -> str:
+        """Get keyid as sha256 hexdigest of the cjson representation of key fields."""
+        data = encode_canonical(
+            {
+                "keytype": keytype,
+                "scheme": scheme,
+                "keyval": keyval,
+            }
+        ).encode("utf-8")
+        hasher = digest("sha256")
+        hasher.update(data)
+        return hasher.hexdigest()
+
 
 class SSlibSigner(Signer):
     """A securesystemslib signer implementation.
 
     Provides a sign method to generate a cryptographic signature with a
     securesystemslib-style rsa, ed25519 or ecdsa key. See keys module
     for the supported types, schemes and hash algorithms.
```

### Comparing `securesystemslib-0.27.0/tests/check_gpg_available.py` & `securesystemslib-0.28.0/tests/check_gpg_available.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """
 <Program Name>
   check_gpg_available.py
 
 <Author>
   Zack Newman <zjn@chainguard.dev>
```

### Comparing `securesystemslib-0.27.0/tests/check_kms_signers.py` & `securesystemslib-0.28.0/tests/check_kms_signers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """
 This module confirms that signing using KMS keys works.
 
 The purpose is to do a smoke test, not to exhaustively test every possible
 key and environment combination.
 
 For Google Cloud (GCP), the requirements to successfully test are:
@@ -21,15 +19,15 @@
 from securesystemslib.signer import GCPSigner, Key, Signer
 
 
 class TestKMSKeys(unittest.TestCase):
     """Test that KMS keys can be used to sign."""
 
     pubkey = Key.from_dict(
-        "218611b80052667026c221f8774249b0f6b8b310d30a5c45a3b878aa3a02f39e",
+        "ab45d8d98992a4128efaea284c7ef0459557db199aeadf237ae41b915b9b5a1c",
         {
             "keytype": "ecdsa",
             "scheme": "ecdsa-sha2-nistp256",
             "keyval": {
                 "public": "-----BEGIN PUBLIC KEY-----\nMFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAE/ptvrXYuUc2ZaKssHhtg/IKNbO1X\ncDWlbKqLNpaK62MKdOwDz1qlp5AGHZkTY9tO09iq1F16SvVot1BQ9FJ2dw==\n-----END PUBLIC KEY-----\n"
             },
         },
```

### Comparing `securesystemslib-0.27.0/tests/check_public_interfaces.py` & `securesystemslib-0.28.0/tests/check_public_interfaces.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """
 <Program Name>
   check_public_interfaces.py
 
 <Author>
   Joshua Lock <jlock@vmware.com>
 
@@ -41,15 +39,16 @@
 import securesystemslib.gpg.util  # pylint: disable=wrong-import-position
 import securesystemslib.interface  # pylint: disable=wrong-import-position
 import securesystemslib.keys  # pylint: disable=wrong-import-position
 from securesystemslib.exceptions import (
     UnsupportedLibraryError,
     VerificationError,
 )
-from securesystemslib.signer import GPGKey, Signature
+from securesystemslib.signer import GPGKey, Key, Signature, SSlibKey
+from securesystemslib.signer._sigstore_signer import SigstoreKey
 
 
 class TestPublicInterfaces(
     unittest.TestCase
 ):  # pylint: disable=missing-class-docstring
     @classmethod
     def setUpClass(cls):
@@ -315,18 +314,63 @@
             securesystemslib.gpg.functions.verify_signature(None, "f00", "bar")
         self.assertEqual(expected_error_msg, str(ctx.exception))
 
         with self.assertRaises(expected_error) as ctx:
             securesystemslib.gpg.functions.export_pubkey("f00")
         self.assertEqual(expected_error_msg, str(ctx.exception))
 
-    def test_signer(self):
+    def test_signer_verify(self):
         """Assert generic VerificationError from UnsupportedLibraryError."""
-        key = GPGKey("aa", "rsa", "pgp+rsa-pkcsv1.5", {"public": "val"})
-        sig = Signature("aa", "aaaaaaa", {"other_headers": "aaaaaa"})
-        with self.assertRaises(VerificationError) as ctx:
-            key.verify_signature(sig, b"data")
-        self.assertIsInstance(ctx.exception.__cause__, UnsupportedLibraryError)
+        keyid = "aa"
+        sig = Signature(keyid, "aaaaaaaa", {"other_headers": "aaaaaa"})
+
+        keys = [
+            GPGKey(keyid, "rsa", "pgp+rsa-pkcsv1.5", {"public": "val"}),
+            SSlibKey(keyid, "rsa", "rsa-pkcs1v15-sha512", {"public": "val"}),
+            SigstoreKey(
+                keyid,
+                "sigstore-oidc",
+                "Fulcio",
+                {"identity": "val", "issuer": "val"},
+            ),
+        ]
+
+        for key in keys:
+            with self.assertRaises(VerificationError) as ctx:
+                key.verify_signature(sig, b"data")
+
+            self.assertIsInstance(
+                ctx.exception.__cause__, (UnsupportedLibraryError, ImportError)
+            )
+
+    def test_signer_ed25519_fallback(self):
+        """Assert ed25519 signature verification works in pure Python."""
+        data = b"The quick brown fox jumps over the lazy dog"
+        keyid = "aaa"
+        sig = Signature.from_dict(
+            {
+                "keyid": keyid,
+                "sig": "2ec7a5e295fa6265e10f3da7f1a432e7742f041f081b4faecab3a12bf0fc8f366c919c90c267e9ed1dfdeb7a7556b959a96dd0dcfea17da358622d39af36bf09",
+            }
+        )
+
+        key = Key.from_dict(
+            keyid,
+            {
+                "keytype": "ed25519",
+                "scheme": "ed25519",
+                "keyval": {
+                    "public": "beb75c268206554e963c45dcbf3c004140d1cb69bbfe9370ef736f19388c9b26"
+                },
+            },
+        )
+
+        self.assertIsNone(key.verify_signature(sig, data))
+
+        with self.assertRaises(
+            securesystemslib.exceptions.UnverifiedSignatureError
+        ):
+            key.verify_signature(sig, b"NOT DATA")
 
 
 if __name__ == "__main__":
     unittest.main(verbosity=1, buffer=True)
```

### Comparing `securesystemslib-0.27.0/tests/check_public_interfaces_gpg.py` & `securesystemslib-0.28.0/tests/check_public_interfaces_gpg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 """
 <Program Name>
   check_public_interfaces_gpg.py
 
 <Author>
   Lukas Puehringer <lukas.puehringer@nyu.edu>
```

### Comparing `securesystemslib-0.27.0/tests/check_sigstore_signer.py` & `securesystemslib-0.28.0/tests/check_sigstore_signer.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,63 +4,42 @@
 NOTE: The filename prefix is check_ instead of test_ so that tests are
 only run when explicitly invoked in a suited environment.
 
 """
 import os
 import unittest
 
-from sigstore.oidc import detect_credential  # pylint: disable=import-error
-
 from securesystemslib.signer import (
-    KEY_FOR_TYPE_AND_SCHEME,
-    Key,
-    SigstoreKey,
+    SIGNER_FOR_URI_SCHEME,
+    Signer,
     SigstoreSigner,
 )
 
-KEY_FOR_TYPE_AND_SCHEME.update(
-    {
-        ("sigstore-oidc", "Fulcio"): SigstoreKey,
-    }
-)
+SIGNER_FOR_URI_SCHEME[SigstoreSigner.SCHEME] = SigstoreSigner
 
 
 class TestSigstoreSigner(unittest.TestCase):
     """Test public key parsing, signature creation and verification.
 
     Requires ambient credentials for signing (e.g. from GitHub Action).
 
     See sigstore-python docs for more infos about ambient credentials:
     https://github.com/sigstore/sigstore-python#signing-with-ambient-credentials
 
     See securesystemslib SigstoreSigner docs for how to test locally.
     """
 
     def test_sign(self):
-        token = detect_credential()
-        self.assertIsNotNone(token, "ambient credentials required")
-
         identity = os.getenv("CERT_ID")
-        self.assertIsNotNone(token, "certificate identity required")
-
+        self.assertIsNotNone(identity, "certificate identity required")
         issuer = os.getenv("CERT_ISSUER")
-        self.assertIsNotNone(token, "OIDC issuer required")
+        self.assertIsNotNone(issuer, "OIDC issuer required")
 
-        public_key = Key.from_dict(
-            "abcdef",
-            {
-                "keytype": "sigstore-oidc",
-                "scheme": "Fulcio",
-                "keyval": {
-                    "issuer": issuer,
-                    "identity": identity,
-                },
-            },
-        )
+        uri, public_key = SigstoreSigner.import_(identity, issuer)
+        signer = Signer.from_priv_key_uri(uri, public_key)
 
-        signer = SigstoreSigner(token, public_key)
         sig = signer.sign(b"data")
         public_key.verify_signature(sig, b"data")
 
 
 if __name__ == "__main__":
     unittest.main(verbosity=4, buffer=False)
```

### Comparing `securesystemslib-0.27.0/tests/test_dsse.py` & `securesystemslib-0.28.0/tests/test_dsse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """Test cases for "metadata.py". """
 
 import copy
 import unittest
 
 import securesystemslib.keys as KEYS
 from securesystemslib.dsse import Envelope
@@ -24,15 +22,15 @@
             KEYS.generate_rsa_key(),
             KEYS.generate_ed25519_key(),
             KEYS.generate_ecdsa_key(),
         ]
 
         cls.signature_dict = {
             "keyid": "11fa391a0ed7a447",
-            "sig": "30460221009342e4566528fcecf6a7a5",
+            "sig": "MEYCIQCTQuRWZSj87PanpQ==",
         }
         cls.envelope_dict = {
             "payload": "aGVsbG8gd29ybGQ=",
             "payloadType": "http://example.com/HelloWorld",
             "signatures": [cls.signature_dict],
         }
         cls.pae = b"DSSEv1 29 http://example.com/HelloWorld 11 hello world"
```

### Comparing `securesystemslib-0.27.0/tests/test_ecdsa_keys.py` & `securesystemslib-0.28.0/tests/test_ecdsa_keys.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env/ python
-
 """
 <Program Name>
   test_ecdsa_keys.py
 
 <Author>
   Vladimir Diaz <vladimir.v.diaz@gmail.com>
```

### Comparing `securesystemslib-0.27.0/tests/test_ed25519_keys.py` & `securesystemslib-0.28.0/tests/test_ed25519_keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env/ python
-
 """
 <Program Name>
   test_ed25519_keys.py
 
 <Author>
   Vladimir Diaz <vladimir.v.diaz@gmail.com>
```

### Comparing `securesystemslib-0.27.0/tests/test_exceptions.py` & `securesystemslib-0.28.0/tests/test_exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """
 <Program Name>
   test_exceptions.py
 
 <Author>
   Vladimir Diaz
```

### Comparing `securesystemslib-0.27.0/tests/test_formats.py` & `securesystemslib-0.28.0/tests/test_formats.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """
 <Program Name>
   test_formats.py
 
 <Author>
   Vladimir Diaz <vladimir.v.diaz@gmail.com>
 
@@ -106,57 +104,41 @@
             ),
             "PUBLIC_KEYVAL_SCHEMA2": (
                 securesystemslib.formats.PUBLIC_KEYVAL_SCHEMA,
                 {"public": "pubkey", "private": ""},
             ),
             "RSA_SCHEME_SCHEMA_RSASSA_PSS": (
                 securesystemslib.formats.RSA_SCHEME_SCHEMA,
-                "rsassa-pss-md5",
-            ),
-            "RSA_SCHEME_SCHEMA_RSASSA_PSS_2": (
-                securesystemslib.formats.RSA_SCHEME_SCHEMA,
-                "rsassa-pss-sha1",
-            ),
-            "RSA_SCHEME_SCHEMA_RSASSA_PSS_3": (
-                securesystemslib.formats.RSA_SCHEME_SCHEMA,
                 "rsassa-pss-sha224",
             ),
-            "RSA_SCHEME_SCHEMA_RSASSA_PSS_4": (
+            "RSA_SCHEME_SCHEMA_RSASSA_PSS_2": (
                 securesystemslib.formats.RSA_SCHEME_SCHEMA,
                 "rsassa-pss-sha256",
             ),
-            "RSA_SCHEME_SCHEMA_RSASSA_PSS_5": (
+            "RSA_SCHEME_SCHEMA_RSASSA_PSS_3": (
                 securesystemslib.formats.RSA_SCHEME_SCHEMA,
                 "rsassa-pss-sha384",
             ),
-            "RSA_SCHEME_SCHEMA_RSASSA_PSS_6": (
+            "RSA_SCHEME_SCHEMA_RSASSA_PSS_4": (
                 securesystemslib.formats.RSA_SCHEME_SCHEMA,
                 "rsassa-pss-sha512",
             ),
             "RSA_SCHEME_SCHEMA_PKCS1v15": (
                 securesystemslib.formats.RSA_SCHEME_SCHEMA,
-                "rsa-pkcs1v15-md5",
-            ),
-            "RSA_SCHEME_SCHEMA_PKCS1v15_2": (
-                securesystemslib.formats.RSA_SCHEME_SCHEMA,
-                "rsa-pkcs1v15-sha1",
-            ),
-            "RSA_SCHEME_SCHEMA_PKCS1v15_3": (
-                securesystemslib.formats.RSA_SCHEME_SCHEMA,
                 "rsa-pkcs1v15-sha224",
             ),
-            "RSA_SCHEME_SCHEMA_PKCS1v15_4": (
+            "RSA_SCHEME_SCHEMA_PKCS1v15_2": (
                 securesystemslib.formats.RSA_SCHEME_SCHEMA,
                 "rsa-pkcs1v15-sha256",
             ),
-            "RSA_SCHEME_SCHEMA_PKCS1v15_5": (
+            "RSA_SCHEME_SCHEMA_PKCS1v15_3": (
                 securesystemslib.formats.RSA_SCHEME_SCHEMA,
                 "rsa-pkcs1v15-sha384",
             ),
-            "RSA_SCHEME_SCHEMA_PKCS1v15_6": (
+            "RSA_SCHEME_SCHEMA_PKCS1v15_4": (
                 securesystemslib.formats.RSA_SCHEME_SCHEMA,
                 "rsa-pkcs1v15-sha512",
             ),
             "KEY_SCHEMA": (
                 securesystemslib.formats.KEY_SCHEMA,
                 {
                     "keytype": "rsa",
```

### Comparing `securesystemslib-0.27.0/tests/test_gpg.py` & `securesystemslib-0.28.0/tests/test_gpg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """
 <Program Name>
   test_gpg.py
 
 <Author>
   Santiago Torres-Arias <santiago@nyu.edu>
   Lukas Puehringer <lukas.puehringer@nyu.edu>
```

### Comparing `securesystemslib-0.27.0/tests/test_hash.py` & `securesystemslib-0.28.0/tests/test_hash.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """
 <Program Name>
   test_hash.py
 
 <Authors>
   Geremy Condra
   Vladimir Diaz <vladimir.v.diaz@gmail.com>
@@ -48,16 +46,14 @@
                 return False
         return True
 
     def _run_with_all_algos_and_libs(
         self, test_func
     ):  # pylint: disable=missing-function-docstring
         algorithms = [
-            "md5",
-            "sha1",
             "sha224",
             "sha256",
             "sha384",
             "sha512",
             "blake2b-256",
             "blake2b",
             "blake2s",
@@ -95,26 +91,14 @@
             ],
             "blake2s": [
                 "69217a3079908094e11121d042354a7c1f55b6482ca1a51e1b250dfd1ed0eef9",
                 "4a0d129873403037c2cd9b9048203687f6233fb6738956e0349bd4320fec3e90",
                 "2b68156e70f71280f7ad021f74620446ee49613a7ed34f5220da7b1dbae9adb2",
                 "2b68156e70f71280f7ad021f74620446ee49613a7ed34f5220da7b1dbae9adb2",
             ],
-            "md5": [
-                "d41d8cd98f00b204e9800998ecf8427e",
-                "0cc175b9c0f1b6a831c399e269772661",
-                "f034e93091235adbb5d2781908e2b313",
-                "f034e93091235adbb5d2781908e2b313",
-            ],
-            "sha1": [
-                "da39a3ee5e6b4b0d3255bfef95601890afd80709",
-                "86f7e437faa5a7fce15d1ddcb9eaeaea377667b8",
-                "d7bfa42fc62b697bf6cf1cda9af1fb7f40a27817",
-                "d7bfa42fc62b697bf6cf1cda9af1fb7f40a27817",
-            ],
             "sha224": [
                 "d14a028c2a3a2bc9476102bb288234c415a2b01f828ea62ac5b3e42f",
                 "abd37534c7d9a2efb9465de931cd7055ffdb8879563ae98078d6d6d5",
                 "ab1342f31c2a6f242d9a3cefb503fb49465c95eb255c16ad791d688c",
                 "ab1342f31c2a6f242d9a3cefb503fb49465c95eb255c16ad791d688c",
             ],
             "sha256": [
@@ -153,20 +137,14 @@
         self._run_with_all_hash_libraries(self._do_algorithm_update, "blake2b")
 
     def test_blake2b_256_update(self):
         self._run_with_all_hash_libraries(
             self._do_algorithm_update, "blake2b-256"
         )
 
-    def test_md5_update(self):
-        self._run_with_all_hash_libraries(self._do_algorithm_update, "md5")
-
-    def test_sha1_update(self):
-        self._run_with_all_hash_libraries(self._do_algorithm_update, "sha1")
-
     def test_sha224_update(self):
         self._run_with_all_hash_libraries(self._do_algorithm_update, "sha224")
 
     def test_sha256_update(self):
         self._run_with_all_hash_libraries(self._do_algorithm_update, "sha256")
 
     def test_sha384_update(self):
@@ -191,16 +169,14 @@
     def test_digest_size(self):
         self._run_with_all_algos_and_libs(self._do_digest_size)
 
     def _do_digest_size(
         self, library, algorithm
     ):  # pylint: disable=missing-function-docstring
         digest_sizes = {
-            "md5": 16,
-            "sha1": 20,
             "sha224": 28,
             "sha256": 32,
             "sha384": 48,
             "sha512": 64,
             "blake2b-256": 32,
             "blake2b": 64,
             "blake2s": 32,
```

### Comparing `securesystemslib-0.27.0/tests/test_hsm_signer.py` & `securesystemslib-0.28.0/tests/test_hsm_signer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,50 +1,29 @@
-#!/usr/bin/env python
 """Test HSMSigner
 """
 import os
 import shutil
 import tempfile
 import unittest
-from unittest.mock import patch
 
 from asn1crypto.keys import (  # pylint: disable=import-error
     ECDomainParameters,
     NamedCurve,
 )
 from cryptography.hazmat.primitives.asymmetric.ec import SECP256R1, SECP384R1
 from PyKCS11 import PyKCS11
 
 from securesystemslib.exceptions import UnverifiedSignatureError
-from securesystemslib.hash import digest
 from securesystemslib.signer import HSMSigner, Signer
 from securesystemslib.signer._hsm_signer import PYKCS11LIB
 
-_orig_sign = HSMSigner.sign
-
-
-def _sign(self, data):
-    """Wraps HSMSigner sign method for testing
-
-    HSMSigner supports CKM_ECDSA_SHA256 and CKM_ECDSA_SHA384 mechanisms. But SoftHSM
-    only supports CKM_ECDSA. For testing we patch the HSMSigner mechanism attribute and
-    pre-hash the data.
-    """
-    self._mechanism = PyKCS11.Mechanism(  # pylint: disable=protected-access
-        PyKCS11.CKM_ECDSA
-    )
-    hasher = digest(algorithm=f"sha{self.public_key.scheme[-3:]}")
-    hasher.update(data)
-    return _orig_sign(self, hasher.digest())
-
 
 @unittest.skipUnless(
     os.environ.get("PYKCS11LIB"), "set PYKCS11LIB to SoftHSM lib path"
 )
-@patch.object(HSMSigner, "sign", _sign)
 class TestHSM(unittest.TestCase):
     """Test HSMSigner with SoftHSM
 
     Requirements:
     - install SoftHSM2
     - set environment variable ``PYKCS11LIB`` to SoftHSM library path
```

### Comparing `securesystemslib-0.27.0/tests/test_interface.py` & `securesystemslib-0.28.0/tests/test_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """
 <Program Name>
   test_interface.py
 
 <Author>
   Vladimir Diaz <vladimir.v.diaz@gmail.com>
 
@@ -272,21 +270,14 @@
                 # Error on encrypted but empty pw passed
                 (
                     [fn_encrypted],
                     {"password": ""},
                     CryptoError,
                     "Password was not given but private key is encrypted",
                 ),
-                # Error on encrypted but bad pw passed
-                (
-                    [fn_encrypted],
-                    {"password": "bad pw"},
-                    CryptoError,
-                    "Bad decrypt. Incorrect password?",
-                ),
                 # Error on pw and prompt
                 (
                     [fn_default],
                     {"password": pw, "prompt": True},
                     ValueError,
                     "passing 'password' and 'prompt=True' is not allowed",
                 ),
@@ -303,14 +294,26 @@
             self.assertTrue(
                 err_msg in str(ctx.exception),
                 "expected: '{}' got: '{}' (row {})".format(  # pylint: disable=consider-using-f-string
                     err_msg, ctx.exception, idx
                 ),
             )
 
+        # Error on encrypted but bad pw passed
+        # NOTE: for some key+pw combos the error differs, see pyca/cryptography#8563
+        with self.assertRaises(CryptoError) as ctx:
+            import_rsa_privatekey_from_file(fn_encrypted, password="bad pw")
+
+        error = str(ctx.exception)
+        self.assertTrue(
+            "Bad decrypt. Incorrect password?" in error
+            or "Could not deserialize key data" in error,
+            f"unexpected: {error}",
+        )
+
         # Error on encrypted but bad pw prompted
         err_msg = "Password was not given but private key is encrypted"
         with self.assertRaises(CryptoError) as ctx, mock.patch(
             "securesystemslib.interface.get_password", return_value="bad_pw"
         ):
             import_rsa_privatekey_from_file(fn_encrypted)
```

### Comparing `securesystemslib-0.27.0/tests/test_keys.py` & `securesystemslib-0.28.0/tests/test_keys.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """
 <Program Name>
   test_keys.py
 
 <Author>
   Vladimir Diaz
```

### Comparing `securesystemslib-0.27.0/tests/test_rsa_keys.py` & `securesystemslib-0.28.0/tests/test_rsa_keys.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """
 <Program Name>
   test_rsa_keys.py
 
 <Author>
   Vladimir Diaz <vladimir.v.diaz@gmail.com>
```

### Comparing `securesystemslib-0.27.0/tests/test_schema.py` & `securesystemslib-0.28.0/tests/test_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """
 <Program Name>
   test_schema.py
 
 <Author>
   Vladimir Diaz <vladimir.v.diaz@gmail.com>
```

### Comparing `securesystemslib-0.27.0/tests/test_storage.py` & `securesystemslib-0.28.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/tests/test_util.py` & `securesystemslib-0.28.0/tests/test_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """
 <Program Name>
   test_util.py
 
 <Author>
   Konstantin Andrianov.
```

### Comparing `securesystemslib-0.27.0/tests/data/keystore/ecdsa_key` & `securesystemslib-0.28.0/tests/data/keystore/ecdsa_key`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/tests/data/keystore/ed25519_key` & `securesystemslib-0.28.0/tests/data/keystore/ed25519_key`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/tests/data/keystore/rsa_key` & `securesystemslib-0.28.0/tests/data/keystore/rsa_key`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/tests/data/keystore/rsa_key.pub` & `securesystemslib-0.28.0/tests/data/keystore/rsa_key.pub`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.pem` & `securesystemslib-0.28.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.pem`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh` & `securesystemslib-0.28.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/tests/gpg_keyrings/dsa/pubring.gpg` & `securesystemslib-0.28.0/tests/gpg_keyrings/dsa/pubring.gpg`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/tests/gpg_keyrings/dsa/random_seed` & `securesystemslib-0.28.0/tests/gpg_keyrings/dsa/random_seed`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/tests/gpg_keyrings/dsa/secring.gpg` & `securesystemslib-0.28.0/tests/gpg_keyrings/dsa/secring.gpg`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/tests/gpg_keyrings/dsa/trustdb.gpg` & `securesystemslib-0.28.0/tests/gpg_keyrings/dsa/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/tests/gpg_keyrings/eddsa/trustdb.gpg` & `securesystemslib-0.28.0/tests/gpg_keyrings/eddsa/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/tests/gpg_keyrings/eddsa/openpgp-revocs.d/4E630F84838BF6F7447B830B22692F5FEA9E2DD2.rev` & `securesystemslib-0.28.0/tests/gpg_keyrings/eddsa/openpgp-revocs.d/4E630F84838BF6F7447B830B22692F5FEA9E2DD2.rev`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/tests/gpg_keyrings/rsa/E8AC80C924116DABB51D4B987CB07D6D2C199C7C.raw` & `securesystemslib-0.28.0/tests/gpg_keyrings/rsa/E8AC80C924116DABB51D4B987CB07D6D2C199C7C.raw`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/tests/gpg_keyrings/rsa/F557D0FF451DEF45372591429EA70BD13D883381.raw` & `securesystemslib-0.28.0/tests/gpg_keyrings/rsa/F557D0FF451DEF45372591429EA70BD13D883381.raw`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/tests/gpg_keyrings/rsa/pubring.gpg` & `securesystemslib-0.28.0/tests/gpg_keyrings/rsa/pubring.gpg`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/tests/gpg_keyrings/rsa/random_seed` & `securesystemslib-0.28.0/tests/gpg_keyrings/rsa/random_seed`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/tests/gpg_keyrings/rsa/secring.gpg` & `securesystemslib-0.28.0/tests/gpg_keyrings/rsa/secring.gpg`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/tests/gpg_keyrings/rsa/trustdb.gpg` & `securesystemslib-0.28.0/tests/gpg_keyrings/rsa/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/LICENSE` & `securesystemslib-0.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/README.rst` & `securesystemslib-0.28.0/README.rst`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/pyproject.toml` & `securesystemslib-0.28.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.27.0/PKG-INFO` & `securesystemslib-0.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: securesystemslib
-Version: 0.27.0
+Version: 0.28.0
 Summary: A library that provides cryptographic and general-purpose routines for Secure Systems Lab projects at NYU
 Project-URL: Homepage, https://github.com/secure-systems-lab/securesystemslib
 Project-URL: Source, https://github.com/secure-systems-lab/securesystemslib
 Project-URL: Issues, https://github.com/secure-systems-lab/securesystemslib/issues
 Author-email: "https://www.updateframework.com" <theupdateframework@googlegroups.com>
 License: MIT
 License-File: LICENSE
```

