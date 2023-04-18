# Comparing `tmp/ledger_bitcoin-0.2.0.tar.gz` & `tmp/ledger_bitcoin-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ledger_bitcoin-0.2.0.tar", last modified: Mon Apr  3 08:17:51 2023, max compression
+gzip compressed data, was "ledger_bitcoin-0.2.1.tar", last modified: Tue Apr 18 14:25:56 2023, max compression
```

## Comparing `ledger_bitcoin-0.2.0.tar` & `ledger_bitcoin-0.2.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-04-03 08:17:51.245973 ledger_bitcoin-0.2.0/
--rw-rw-r--   0 singala   (1000) singala   (1000)    11357 2023-01-28 15:06:45.000000 ledger_bitcoin-0.2.0/LICENSE
--rw-rw-r--   0 singala   (1000) singala   (1000)     5812 2023-04-03 08:17:51.245973 ledger_bitcoin-0.2.0/PKG-INFO
--rw-rw-r--   0 singala   (1000) singala   (1000)     5260 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.0/README.md
-drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-04-03 08:17:51.241973 ledger_bitcoin-0.2.0/ledger_bitcoin/
--rw-rw-r--   0 singala   (1000) singala   (1000)      450 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/__init__.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     4051 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/_base58.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     4265 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/_script.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     6661 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/_serialize.py
-drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-04-03 08:17:51.241973 ledger_bitcoin-0.2.0/ledger_bitcoin/btchip/
--rw-rw-r--   0 singala   (1000) singala   (1000)      855 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/btchip/__init__.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     4874 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/btchip/bitcoinTransaction.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     2025 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/btchip/bitcoinVarint.py
--rw-rw-r--   0 singala   (1000) singala   (1000)    16475 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/btchip/btchip.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     4795 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/btchip/btchipComm.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     1020 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/btchip/btchipException.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     2713 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/btchip/btchipHelpers.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     3416 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/btchip/btchipUtils.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     3224 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/btchip/ledgerWrapper.py
--rw-rw-r--   0 singala   (1000) singala   (1000)    10607 2023-04-03 08:13:57.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/client.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     9267 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/client_base.py
--rw-rw-r--   0 singala   (1000) singala   (1000)    11336 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/client_command.py
--rw-rw-r--   0 singala   (1000) singala   (1000)    15428 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/client_legacy.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     5937 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/command_builder.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     4688 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/common.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     7153 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/errors.py
-drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-04-03 08:17:51.245973 ledger_bitcoin-0.2.0/ledger_bitcoin/exception/
--rw-rw-r--   0 singala   (1000) singala   (1000)      806 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/exception/__init__.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     1251 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/exception/device_exception.py
--rw-rw-r--   0 singala   (1000) singala   (1000)      652 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/exception/errors.py
--rw-rw-r--   0 singala   (1000) singala   (1000)    15997 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/key.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     8383 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/merkle.py
--rw-rw-r--   0 singala   (1000) singala   (1000)    47567 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/psbt.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     4206 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/ripemd.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     7623 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/transport.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     9191 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/tx.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     4397 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.0/ledger_bitcoin/wallet.py
-drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-04-03 08:17:51.241973 ledger_bitcoin-0.2.0/ledger_bitcoin.egg-info/
--rw-rw-r--   0 singala   (1000) singala   (1000)     5812 2023-04-03 08:17:51.000000 ledger_bitcoin-0.2.0/ledger_bitcoin.egg-info/PKG-INFO
--rw-rw-r--   0 singala   (1000) singala   (1000)     1427 2023-04-03 08:17:51.000000 ledger_bitcoin-0.2.0/ledger_bitcoin.egg-info/SOURCES.txt
--rw-rw-r--   0 singala   (1000) singala   (1000)        1 2023-04-03 08:17:51.000000 ledger_bitcoin-0.2.0/ledger_bitcoin.egg-info/dependency_links.txt
--rw-rw-r--   0 singala   (1000) singala   (1000)       84 2023-04-03 08:17:51.000000 ledger_bitcoin-0.2.0/ledger_bitcoin.egg-info/requires.txt
--rw-rw-r--   0 singala   (1000) singala   (1000)       15 2023-04-03 08:17:51.000000 ledger_bitcoin-0.2.0/ledger_bitcoin.egg-info/top_level.txt
--rw-rw-r--   0 singala   (1000) singala   (1000)      159 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/pyproject.toml
--rw-rw-r--   0 singala   (1000) singala   (1000)      812 2023-04-03 08:17:51.245973 ledger_bitcoin-0.2.0/setup.cfg
-drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-04-03 08:17:51.245973 ledger_bitcoin-0.2.0/tests/
--rw-rw-r--   0 singala   (1000) singala   (1000)      431 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.0/tests/test_client_legacy.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     1289 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/tests/test_get_extended_pubkey_legacyapp.py
--rw-rw-r--   0 singala   (1000) singala   (1000)      259 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/tests/test_get_master_fingerprint_legacyapp.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     1823 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.0/tests/test_get_wallet_address_legacyapp.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     1050 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.0/tests/test_ripemd160.py
--rw-rw-r--   0 singala   (1000) singala   (1000)      447 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.0/tests/test_sign_message_legacyapp.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     5504 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.0/tests/test_sign_psbt_legacyapp.py
+drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-04-18 14:25:56.907050 ledger_bitcoin-0.2.1/
+-rw-rw-r--   0 singala   (1000) singala   (1000)    11357 2023-04-18 14:24:56.000000 ledger_bitcoin-0.2.1/LICENSE
+-rw-rw-r--   0 singala   (1000) singala   (1000)     5812 2023-04-18 14:25:56.907050 ledger_bitcoin-0.2.1/PKG-INFO
+-rw-rw-r--   0 singala   (1000) singala   (1000)     5260 2023-04-18 14:24:56.000000 ledger_bitcoin-0.2.1/README.md
+drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-04-18 14:25:56.903050 ledger_bitcoin-0.2.1/ledger_bitcoin/
+-rw-rw-r--   0 singala   (1000) singala   (1000)      450 2023-04-18 14:25:09.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/__init__.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     4051 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/_base58.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     4265 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/_script.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     6661 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/_serialize.py
+drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-04-18 14:25:56.907050 ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/
+-rw-rw-r--   0 singala   (1000) singala   (1000)      855 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/__init__.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     4874 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/bitcoinTransaction.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     2025 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/bitcoinVarint.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)    16475 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/btchip.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     4795 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/btchipComm.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     1020 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/btchipException.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     2713 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/btchipHelpers.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     3416 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/btchipUtils.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     3224 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/ledgerWrapper.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)    11466 2023-04-18 14:25:09.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/client.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     9267 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/client_base.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)    11336 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/client_command.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)    15428 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/client_legacy.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     5937 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/command_builder.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     4688 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/common.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     7153 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/errors.py
+drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-04-18 14:25:56.907050 ledger_bitcoin-0.2.1/ledger_bitcoin/exception/
+-rw-rw-r--   0 singala   (1000) singala   (1000)      806 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/exception/__init__.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     1251 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/exception/device_exception.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)      652 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/exception/errors.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)    15997 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/key.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     8383 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/merkle.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)    47567 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/psbt.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     4206 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/ripemd.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     7623 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/transport.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     9191 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/tx.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     4397 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/wallet.py
+drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-04-18 14:25:56.903050 ledger_bitcoin-0.2.1/ledger_bitcoin.egg-info/
+-rw-rw-r--   0 singala   (1000) singala   (1000)     5812 2023-04-18 14:25:56.000000 ledger_bitcoin-0.2.1/ledger_bitcoin.egg-info/PKG-INFO
+-rw-rw-r--   0 singala   (1000) singala   (1000)     1427 2023-04-18 14:25:56.000000 ledger_bitcoin-0.2.1/ledger_bitcoin.egg-info/SOURCES.txt
+-rw-rw-r--   0 singala   (1000) singala   (1000)        1 2023-04-18 14:25:56.000000 ledger_bitcoin-0.2.1/ledger_bitcoin.egg-info/dependency_links.txt
+-rw-rw-r--   0 singala   (1000) singala   (1000)       84 2023-04-18 14:25:56.000000 ledger_bitcoin-0.2.1/ledger_bitcoin.egg-info/requires.txt
+-rw-rw-r--   0 singala   (1000) singala   (1000)       15 2023-04-18 14:25:56.000000 ledger_bitcoin-0.2.1/ledger_bitcoin.egg-info/top_level.txt
+-rw-rw-r--   0 singala   (1000) singala   (1000)      159 2023-04-18 14:24:56.000000 ledger_bitcoin-0.2.1/pyproject.toml
+-rw-rw-r--   0 singala   (1000) singala   (1000)      812 2023-04-18 14:25:56.907050 ledger_bitcoin-0.2.1/setup.cfg
+drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-04-18 14:25:56.907050 ledger_bitcoin-0.2.1/tests/
+-rw-rw-r--   0 singala   (1000) singala   (1000)      431 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/tests/test_client_legacy.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     1289 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/tests/test_get_extended_pubkey_legacyapp.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)      259 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/tests/test_get_master_fingerprint_legacyapp.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     1823 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/tests/test_get_wallet_address_legacyapp.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     1050 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/tests/test_ripemd160.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)      447 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/tests/test_sign_message_legacyapp.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     5504 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/tests/test_sign_psbt_legacyapp.py
```

### Comparing `ledger_bitcoin-0.2.0/LICENSE` & `ledger_bitcoin-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/PKG-INFO` & `ledger_bitcoin-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledger_bitcoin
-Version: 0.2.0
+Version: 0.2.1
 Summary: Client for Ledger Nano Bitcoin application
 Home-page: https://github.com/LedgerHQ/app-bitcoin-new
 Author: Ledger
 Author-email: hello@ledger.fr
 Project-URL: Bug Tracker, https://github.com/LedgerHQ/app-bitcoin-new/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ledger_bitcoin-0.2.0/README.md` & `ledger_bitcoin-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/_base58.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/_base58.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/_script.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/_script.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/_serialize.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/_serialize.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/btchip/__init__.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/__init__.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/btchip/bitcoinTransaction.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/bitcoinTransaction.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/btchip/bitcoinVarint.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/bitcoinVarint.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/btchip/btchip.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/btchip.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/btchip/btchipComm.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/btchipComm.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/btchip/btchipException.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/btchipException.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/btchip/btchipHelpers.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/btchipHelpers.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/btchip/btchipUtils.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/btchipUtils.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/btchip/ledgerWrapper.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/ledgerWrapper.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/client.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from packaging.version import parse as parse_version
 from typing import Tuple, List, Mapping, Optional, Union
 import base64
 from io import BytesIO, BufferedReader
+import re
 
 from .command_builder import BitcoinCommandBuilder, BitcoinInsType
 from .common import Chain, read_uint, read_varint
 from .client_command import ClientCommandInterpreter
 from .client_base import Client, TransportClient, PartialSignature
 from .client_legacy import LegacyClient
 from .exception import DeviceException
@@ -47,14 +48,19 @@
 
         if len(pubkey_augm) not in [32, 33]:
             raise UnknownDeviceError(f"Invalid pubkey length returned: {len(pubkey_augm)}")
 
         return PartialSignature(signature=signature, pubkey=pubkey_augm)
 
 
+def _contains_a_fragment(desc_tmp: str) -> bool:
+    """Returns true if the given descriptor template contains the `a:` fragment."""
+    return any('a' in match for match in re.findall(r'[asctdvjnlu]+:', desc_tmp))
+
+
 class NewClient(Client):
     # internal use for testing: if set to True, sign_psbt will not clone the psbt before converting to psbt version 2
     _no_clone_psbt: bool = False
 
     def __init__(self, comm_client: TransportClient, chain: Chain = Chain.MAIN, debug: bool = False) -> None:
         super().__init__(comm_client, chain, debug)
         self.builder = BitcoinCommandBuilder()
@@ -84,14 +90,16 @@
 
         return response.decode()
 
     def register_wallet(self, wallet: WalletPolicy) -> Tuple[bytes, bytes]:
         if wallet.version not in [WalletType.WALLET_POLICY_V1, WalletType.WALLET_POLICY_V2]:
             raise ValueError("invalid wallet policy version")
 
+        self._validate_policy(wallet)
+
         client_intepreter = ClientCommandInterpreter()
         client_intepreter.add_known_preimage(wallet.serialize())
         client_intepreter.add_known_list([k.encode() for k in wallet.keys_info])
 
         # necessary for version 1 of the protocol (introduced in version 2.1.0)
         client_intepreter.add_known_preimage(wallet.descriptor_template.encode())
 
@@ -121,14 +129,16 @@
 
         if not isinstance(wallet, WalletPolicy) or wallet.version not in [WalletType.WALLET_POLICY_V1, WalletType.WALLET_POLICY_V2]:
             raise ValueError("wallet type must be WalletPolicy, with version either WALLET_POLICY_V1 or WALLET_POLICY_V2")
 
         if change != 0 and change != 1:
             raise ValueError("Invalid change")
 
+        self._validate_policy(wallet)
+
         client_intepreter = ClientCommandInterpreter()
         client_intepreter.add_known_list([k.encode() for k in wallet.keys_info])
         client_intepreter.add_known_preimage(wallet.serialize())
 
         # necessary for version 1 of the protocol (introduced in version 2.1.0)
         client_intepreter.add_known_preimage(wallet.descriptor_template.encode())
 
@@ -141,14 +151,17 @@
 
         if sw != 0x9000:
             raise DeviceException(error_code=sw, ins=BitcoinInsType.GET_WALLET_ADDRESS)
 
         return response.decode()
 
     def sign_psbt(self, psbt: Union[PSBT, bytes, str], wallet: WalletPolicy, wallet_hmac: Optional[bytes]) -> List[Tuple[int, PartialSignature]]:
+
+        self._validate_policy(wallet)
+
         psbt = normalize_psbt(psbt)
 
         if psbt.version != 2:
             if self._no_clone_psbt:
                 psbt.convert_to_v2()
                 psbt_v2 = psbt
             else:
@@ -248,14 +261,23 @@
         sw, response = self._make_request(self.builder.sign_message(message_bytes, bip32_path), client_intepreter)
 
         if sw != 0x9000:
             raise DeviceException(error_code=sw, ins=BitcoinInsType.SIGN_MESSAGE)
 
         return base64.b64encode(response).decode('utf-8')
 
+    def _validate_policy(self, wallet_policy: WalletPolicy):
+        """Performs any additional checks before we use a wallet policy"""
+        if _contains_a_fragment(wallet_policy.descriptor_template):
+            _, app_version, _ = self.get_version()
+            if app_version in ["2.1.0", "2.1.1"]:
+                # Versions 2.1.0 and 2.1.1 produced incorrect scripts for policies containing
+                # the `a:` fragment.
+                raise RuntimeError("Please update your Ledger Bitcoin app.")
+
 
 def createClient(comm_client: Optional[TransportClient] = None, chain: Chain = Chain.MAIN, debug: bool = False) -> Union[LegacyClient, NewClient]:
     if comm_client is None:
         comm_client = TransportClient("hid")
 
     base_client = Client(comm_client, chain, debug)
     app_name, app_version, _ = base_client.get_version()
```

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/client_base.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/client_base.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/client_command.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/client_command.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/client_legacy.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/client_legacy.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/command_builder.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/command_builder.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/common.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/common.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/errors.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/errors.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/exception/__init__.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/exception/device_exception.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/exception/device_exception.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/exception/errors.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/exception/errors.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/key.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/key.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/merkle.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/merkle.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/psbt.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/psbt.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/ripemd.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/ripemd.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/transport.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/transport.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/tx.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/tx.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin/wallet.py` & `ledger_bitcoin-0.2.1/ledger_bitcoin/wallet.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin.egg-info/PKG-INFO` & `ledger_bitcoin-0.2.1/ledger_bitcoin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledger-bitcoin
-Version: 0.2.0
+Version: 0.2.1
 Summary: Client for Ledger Nano Bitcoin application
 Home-page: https://github.com/LedgerHQ/app-bitcoin-new
 Author: Ledger
 Author-email: hello@ledger.fr
 Project-URL: Bug Tracker, https://github.com/LedgerHQ/app-bitcoin-new/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ledger_bitcoin-0.2.0/ledger_bitcoin.egg-info/SOURCES.txt` & `ledger_bitcoin-0.2.1/ledger_bitcoin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/setup.cfg` & `ledger_bitcoin-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/tests/test_get_extended_pubkey_legacyapp.py` & `ledger_bitcoin-0.2.1/tests/test_get_extended_pubkey_legacyapp.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/tests/test_get_wallet_address_legacyapp.py` & `ledger_bitcoin-0.2.1/tests/test_get_wallet_address_legacyapp.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/tests/test_ripemd160.py` & `ledger_bitcoin-0.2.1/tests/test_ripemd160.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.0/tests/test_sign_psbt_legacyapp.py` & `ledger_bitcoin-0.2.1/tests/test_sign_psbt_legacyapp.py`

 * *Files identical despite different names*

