# Comparing `tmp/mainnet-1.1.0.tar.gz` & `tmp/mainnet-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mainnet-1.1.0.tar", last modified: Thu Mar 30 19:02:29 2023, max compression
+gzip compressed data, was "dist/mainnet-1.1.1.tar", last modified: Tue Apr 18 12:07:47 2023, max compression
```

## Comparing `mainnet-1.1.0.tar` & `mainnet-1.1.1.tar`

### file list

```diff
@@ -1,332 +1,332 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:02:29.000000 mainnet-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-03-30 19:02:29.000000 mainnet-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26894 2023-03-30 19:02:26.000000 mainnet-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:02:29.000000 mainnet-1.1.0/mainnet/
--rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:02:29.000000 mainnet-1.1.0/mainnet/api/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25449 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/api/contract_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25435 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/api/contract_escrow_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    31418 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/api/faucet_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/api/mine_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33291 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/api/smartbch_contract_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    59169 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/api/smartbch_sep20_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    55918 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/api/smartbch_wallet_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18228 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/api/util_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   154253 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/api/wallet_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/api/wallet_bcmr_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/api/wallet_signed_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    86668 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/api/wallet_slp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/api/wallet_util_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/api/webhook_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27388 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:02:29.000000 mainnet-1.1.0/mainnet/models/
--rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/auth_chain_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/balance_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/balance_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/cashscript_receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/contract_fn_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/contract_fn_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/contract_info_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/contract_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/contract_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/contract_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/convert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/create_signed_message_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/deposit_address_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/electrum_raw_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/electrum_raw_transaction_script_pub_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/electrum_raw_transaction_script_sig.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/electrum_raw_transaction_vin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/electrum_raw_transaction_vout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/encode_transaction_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/encode_transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/escrow_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/escrow_fn_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/escrow_info_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/escrow_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/escrow_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/escrow_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/get_addresses_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/get_addrs_by_xpub_key_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/get_testnet_bch_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/get_testnet_bch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/get_testnet_sbch_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/get_testnet_sbch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/get_testnet_sep20_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/get_testnet_sep20_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/get_testnet_slp_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/get_testnet_slp_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/get_xpub_key_info_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/get_xpub_key_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/history_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/history_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/inline_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/inline_object1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/inline_object2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/inline_object3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/inline_object4.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/max_amount_to_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/mine_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/network_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/op_return_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/scalable_vector_graphic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/send_max_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/send_max_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/send_request_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/send_request_item_any_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    13441 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/send_request_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/send_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/serialized_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/signed_message_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/signed_message_response_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/signed_message_response_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/slp_balance_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/slp_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/slp_deposit_address_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/slp_genesis_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/slp_genesis_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/slp_mint_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/slp_mint_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/slp_outpoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/slp_send_max_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/slp_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/slp_send_request_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/slp_send_request_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/slp_send_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/slp_token_info_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/slp_token_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/slp_utxo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/slp_utxo_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_contract_deploy_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_contract_deploy_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_contract_estimate_gas_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_contract_estimate_gas_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_contract_fn_call_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_contract_fn_call_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_contract_info_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_contract_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_contract_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_contract_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_deposit_address_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_max_amount_to_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_send_max_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_send_request_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_send_request_item_any_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_send_request_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_send_response_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_sep20_all_balances_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_sep20_balance_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_sep20_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_sep20_genesis_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_sep20_genesis_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_sep20_mint_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_sep20_mint_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_sep20_send_max_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_sep20_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_sep20_send_request_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_sep20_token_info_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_sep20_token_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    18359 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/smart_bch_transaction_receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/submit_transaction_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/submit_transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     9588 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/token_burn_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/token_genesis_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/token_mint_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/token_mint_request_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/token_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/transaction_history_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/unit_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/util_decode_transaction_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/utxo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/utxo_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/verify_signed_message_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/verify_signed_message_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/verify_signed_message_response_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/wallet_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/wallet_mnemonic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/wallet_named_exists_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/wallet_replace_named_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/wallet_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/wallet_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/wallet_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/watch_address_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/watch_address_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/wif.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/x_pub_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/x_pub_key_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/x_pub_key_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/models/zero_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-03-30 19:02:26.000000 mainnet-1.1.0/mainnet/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:02:29.000000 mainnet-1.1.0/mainnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-03-30 19:02:29.000000 mainnet-1.1.0/mainnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-03-30 19:02:29.000000 mainnet-1.1.0/mainnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 19:02:29.000000 mainnet-1.1.0/mainnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-30 19:02:29.000000 mainnet-1.1.0/mainnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-30 19:02:29.000000 mainnet-1.1.0/mainnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-30 19:02:29.000000 mainnet-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-30 19:02:29.000000 mainnet-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:02:29.000000 mainnet-1.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_auth_chain_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_balance_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_cashscript_receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_contract_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_contract_escrow_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_contract_fn_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_contract_fn_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_contract_info_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_contract_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_contract_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_contract_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_convert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_create_signed_message_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_deposit_address_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_electrum_raw_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_electrum_raw_transaction_script_pub_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_electrum_raw_transaction_script_sig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_electrum_raw_transaction_vin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_electrum_raw_transaction_vout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_encode_transaction_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_encode_transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_escrow_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_escrow_fn_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_escrow_info_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_escrow_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_escrow_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_escrow_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_faucet_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_get_addresses_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_get_addrs_by_xpub_key_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_get_testnet_bch_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_get_testnet_bch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_get_testnet_sbch_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_get_testnet_sbch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_get_testnet_sep20_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_get_testnet_sep20_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_get_testnet_slp_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_get_testnet_slp_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_get_xpub_key_info_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_get_xpub_key_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_history_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_history_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_inline_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_inline_object1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_inline_object2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_inline_object3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_inline_object4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_max_amount_to_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_mine_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_mine_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_network_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_op_return_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_scalable_vector_graphic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_send_max_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_send_max_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_send_request_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_send_request_item_any_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_send_request_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_send_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_serialized_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_signed_message_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_signed_message_response_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_signed_message_response_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_slp_balance_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_slp_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_slp_deposit_address_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_slp_genesis_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_slp_genesis_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_slp_mint_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_slp_mint_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_slp_outpoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_slp_send_max_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_slp_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_slp_send_request_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_slp_send_request_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_slp_send_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_slp_token_info_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_slp_token_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_slp_utxo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_slp_utxo_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_contract_deploy_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_contract_deploy_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_contract_estimate_gas_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_contract_estimate_gas_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_contract_fn_call_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_contract_fn_call_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_contract_info_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_contract_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_contract_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_contract_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_deposit_address_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_max_amount_to_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_send_max_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_send_request_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_send_request_item_any_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_send_request_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_send_response_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_sep20_all_balances_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_sep20_balance_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_sep20_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_sep20_genesis_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_sep20_genesis_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_sep20_mint_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_sep20_mint_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_sep20_send_max_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_sep20_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_sep20_send_request_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_sep20_token_info_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_sep20_token_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smart_bch_transaction_receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smartbch_contract_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smartbch_sep20_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_smartbch_wallet_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_submit_transaction_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_submit_transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_token_burn_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_token_genesis_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_token_mint_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_token_mint_request_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_token_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_transaction_history_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_unit_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_util_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_util_decode_transaction_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_utxo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_utxo_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_verify_signed_message_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_verify_signed_message_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_verify_signed_message_response_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_wallet_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_wallet_bcmr_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_wallet_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_wallet_mnemonic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_wallet_named_exists_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_wallet_replace_named_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_wallet_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_wallet_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_wallet_signed_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_wallet_slp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_wallet_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_wallet_util_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_watch_address_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_watch_address_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_webhook_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_wif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_x_pub_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_x_pub_key_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_x_pub_key_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-03-30 19:02:26.000000 mainnet-1.1.0/test/test_zero_balance_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:07:47.000000 mainnet-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-18 12:07:47.000000 mainnet-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26887 2023-04-18 12:07:44.000000 mainnet-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:07:47.000000 mainnet-1.1.1/mainnet/
+-rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:07:47.000000 mainnet-1.1.1/mainnet/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25442 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/api/contract_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25428 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/api/contract_escrow_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31417 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/api/faucet_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/api/mine_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/api/smartbch_contract_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59168 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/api/smartbch_sep20_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55917 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/api/smartbch_wallet_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18227 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/api/util_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154240 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/api/wallet_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43177 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/api/wallet_bcmr_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/api/wallet_signed_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86667 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/api/wallet_slp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13613 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/api/wallet_util_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/api/webhook_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16450 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:07:47.000000 mainnet-1.1.1/mainnet/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    10495 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/auth_chain_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/balance_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/cashscript_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16948 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/contract_fn_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/contract_fn_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/contract_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/contract_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/contract_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/contract_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/convert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/create_signed_message_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/deposit_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/electrum_raw_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/electrum_raw_transaction_script_pub_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/electrum_raw_transaction_script_sig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/electrum_raw_transaction_vin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/electrum_raw_transaction_vout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/encode_transaction_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/encode_transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/escrow_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/escrow_fn_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/escrow_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10302 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/escrow_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/escrow_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/escrow_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/get_addresses_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/get_addrs_by_xpub_key_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/get_testnet_bch_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/get_testnet_bch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/get_testnet_sbch_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/get_testnet_sbch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/get_testnet_sep20_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/get_testnet_sep20_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/get_testnet_slp_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/get_testnet_slp_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/get_xpub_key_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/get_xpub_key_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/history_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/history_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/inline_object1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/inline_object2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/inline_object3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/inline_object4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/max_amount_to_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/mine_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/network_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/op_return_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/scalable_vector_graphic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/send_max_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/send_max_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/send_request_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/send_request_item_any_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/send_request_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/send_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/serialized_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/signed_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/signed_message_response_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/signed_message_response_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/slp_balance_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/slp_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/slp_deposit_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14019 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/slp_genesis_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/slp_genesis_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/slp_mint_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/slp_mint_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/slp_outpoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/slp_send_max_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/slp_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/slp_send_request_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/slp_send_request_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/slp_send_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/slp_token_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/slp_token_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/slp_utxo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/slp_utxo_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_contract_deploy_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_contract_deploy_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_contract_estimate_gas_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_contract_estimate_gas_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_contract_fn_call_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_contract_fn_call_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_contract_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_contract_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_contract_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_contract_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_deposit_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_max_amount_to_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_send_max_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_send_request_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_send_request_item_any_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_send_request_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_send_response_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_sep20_all_balances_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_sep20_balance_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_sep20_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11666 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_sep20_genesis_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_sep20_genesis_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_sep20_mint_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_sep20_mint_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_sep20_send_max_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_sep20_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_sep20_send_request_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_sep20_token_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_sep20_token_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18358 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/smart_bch_transaction_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/submit_transaction_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/submit_transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/token_burn_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9714 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/token_genesis_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/token_mint_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/token_mint_request_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/token_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/transaction_history_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/unit_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/util_decode_transaction_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/utxo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/utxo_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/verify_signed_message_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/verify_signed_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/verify_signed_message_response_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/wallet_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/wallet_mnemonic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/wallet_named_exists_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/wallet_replace_named_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/wallet_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/wallet_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/watch_address_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/watch_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/wif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/x_pub_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/x_pub_key_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/x_pub_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/models/zero_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-04-18 12:07:44.000000 mainnet-1.1.1/mainnet/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:07:47.000000 mainnet-1.1.1/mainnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-18 12:07:47.000000 mainnet-1.1.1/mainnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-04-18 12:07:47.000000 mainnet-1.1.1/mainnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 12:07:47.000000 mainnet-1.1.1/mainnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-18 12:07:47.000000 mainnet-1.1.1/mainnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 12:07:47.000000 mainnet-1.1.1/mainnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-18 12:07:47.000000 mainnet-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-18 12:07:46.000000 mainnet-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:07:47.000000 mainnet-1.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_auth_chain_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_balance_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_cashscript_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_contract_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_contract_escrow_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_contract_fn_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_contract_fn_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_contract_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_contract_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_contract_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_contract_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_convert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_create_signed_message_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_deposit_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_electrum_raw_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_electrum_raw_transaction_script_pub_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_electrum_raw_transaction_script_sig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_electrum_raw_transaction_vin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_electrum_raw_transaction_vout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_encode_transaction_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_encode_transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_escrow_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_escrow_fn_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_escrow_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_escrow_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_escrow_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_escrow_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_faucet_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_get_addresses_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_get_addrs_by_xpub_key_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_get_testnet_bch_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_get_testnet_bch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_get_testnet_sbch_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_get_testnet_sbch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_get_testnet_sep20_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_get_testnet_sep20_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_get_testnet_slp_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_get_testnet_slp_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_get_xpub_key_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_get_xpub_key_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_history_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_inline_object1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_inline_object2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_inline_object3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_inline_object4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_max_amount_to_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_mine_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_mine_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_network_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_op_return_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_scalable_vector_graphic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_send_max_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_send_max_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_send_request_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_send_request_item_any_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_send_request_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_send_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_serialized_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_signed_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_signed_message_response_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_signed_message_response_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_slp_balance_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_slp_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_slp_deposit_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_slp_genesis_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_slp_genesis_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_slp_mint_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_slp_mint_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_slp_outpoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_slp_send_max_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_slp_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_slp_send_request_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_slp_send_request_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_slp_send_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_slp_token_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_slp_token_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_slp_utxo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_slp_utxo_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_contract_deploy_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_contract_deploy_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_contract_estimate_gas_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_contract_estimate_gas_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_contract_fn_call_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_contract_fn_call_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_contract_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_contract_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_contract_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_contract_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_deposit_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_max_amount_to_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_send_max_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_send_request_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_send_request_item_any_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_send_request_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_send_response_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_sep20_all_balances_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_sep20_balance_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_sep20_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_sep20_genesis_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_sep20_genesis_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_sep20_mint_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_sep20_mint_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_sep20_send_max_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_sep20_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_sep20_send_request_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_sep20_token_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_sep20_token_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smart_bch_transaction_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smartbch_contract_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smartbch_sep20_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_smartbch_wallet_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_submit_transaction_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_submit_transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_token_burn_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_token_genesis_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_token_mint_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_token_mint_request_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_token_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_transaction_history_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_unit_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_util_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_util_decode_transaction_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_utxo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_utxo_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_verify_signed_message_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_verify_signed_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_verify_signed_message_response_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_wallet_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_wallet_bcmr_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_wallet_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_wallet_mnemonic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_wallet_named_exists_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_wallet_replace_named_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_wallet_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_wallet_signed_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_wallet_slp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_wallet_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_wallet_util_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_watch_address_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_watch_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_webhook_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_wif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_x_pub_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_x_pub_key_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_x_pub_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-18 12:07:44.000000 mainnet-1.1.1/test/test_zero_balance_response.py
```

### Comparing `mainnet-1.1.0/README.md` & `mainnet-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 This API is currently in *active* development, breaking changes may
 be made prior to official release of version 1.0.0.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.18
+- API version: 1.1.0
 - Package version: 1.0.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -308,15 +308,15 @@
  - [TokenMintRequest](docs/TokenMintRequest.md)
  - [TokenMintRequestRequests](docs/TokenMintRequestRequests.md)
  - [TokenSendRequest](docs/TokenSendRequest.md)
  - [TransactionHistoryItem](docs/TransactionHistoryItem.md)
  - [UnitType](docs/UnitType.md)
  - [UtilDecodeTransactionRequest](docs/UtilDecodeTransactionRequest.md)
  - [Utxo](docs/Utxo.md)
- - [UtxoResponse](docs/UtxoResponse.md)
+ - [UtxoToken](docs/UtxoToken.md)
  - [VerifySignedMessageRequest](docs/VerifySignedMessageRequest.md)
  - [VerifySignedMessageResponse](docs/VerifySignedMessageResponse.md)
  - [VerifySignedMessageResponseDetails](docs/VerifySignedMessageResponseDetails.md)
  - [WalletInfo](docs/WalletInfo.md)
  - [WalletMnemonic](docs/WalletMnemonic.md)
  - [WalletNamedExistsRequest](docs/WalletNamedExistsRequest.md)
  - [WalletReplaceNamedRequest](docs/WalletReplaceNamedRequest.md)
```

### Comparing `mainnet-1.1.0/mainnet/__init__.py` & `mainnet-1.1.1/mainnet/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -162,15 +162,15 @@
 from mainnet.models.token_mint_request import TokenMintRequest
 from mainnet.models.token_mint_request_requests import TokenMintRequestRequests
 from mainnet.models.token_send_request import TokenSendRequest
 from mainnet.models.transaction_history_item import TransactionHistoryItem
 from mainnet.models.unit_type import UnitType
 from mainnet.models.util_decode_transaction_request import UtilDecodeTransactionRequest
 from mainnet.models.utxo import Utxo
-from mainnet.models.utxo_response import UtxoResponse
+from mainnet.models.utxo_token import UtxoToken
 from mainnet.models.verify_signed_message_request import VerifySignedMessageRequest
 from mainnet.models.verify_signed_message_response import VerifySignedMessageResponse
 from mainnet.models.verify_signed_message_response_details import VerifySignedMessageResponseDetails
 from mainnet.models.wallet_info import WalletInfo
 from mainnet.models.wallet_mnemonic import WalletMnemonic
 from mainnet.models.wallet_named_exists_request import WalletNamedExistsRequest
 from mainnet.models.wallet_replace_named_request import WalletReplaceNamedRequest
```

### Comparing `mainnet-1.1.0/mainnet/api/__init__.py` & `mainnet-1.1.1/mainnet/api/__init__.py`

 * *Files identical despite different names*

### Comparing `mainnet-1.1.0/mainnet/api/contract_api.py` & `mainnet-1.1.1/mainnet/api/contract_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -324,15 +324,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: UtxoResponse
+        :rtype: list[Utxo]
         """
         kwargs['_return_http_data_only'] = True
         return self.contract_utxos_with_http_info(contract, **kwargs)  # noqa: E501
 
     def contract_utxos_with_http_info(self, contract, **kwargs):  # noqa: E501
         """List specific utxos on any contract  # noqa: E501
 
@@ -361,15 +361,15 @@
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(UtxoResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(list[Utxo], status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
             'contract'
         ]
@@ -425,15 +425,15 @@
             '/contract/utxos', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='UtxoResponse',  # noqa: E501
+            response_type='list[Utxo]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
```

### Comparing `mainnet-1.1.0/mainnet/api/contract_escrow_api.py` & `mainnet-1.1.1/mainnet/api/contract_escrow_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -457,15 +457,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: UtxoResponse
+        :rtype: list[Utxo]
         """
         kwargs['_return_http_data_only'] = True
         return self.escrow_utxos_with_http_info(escrow_contract, **kwargs)  # noqa: E501
 
     def escrow_utxos_with_http_info(self, escrow_contract, **kwargs):  # noqa: E501
         """List specific utxos on any escrow contract  # noqa: E501
 
@@ -494,15 +494,15 @@
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(UtxoResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(list[Utxo], status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
             'escrow_contract'
         ]
@@ -558,15 +558,15 @@
             '/contract/escrow/utxos', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='UtxoResponse',  # noqa: E501
+            response_type='list[Utxo]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
```

### Comparing `mainnet-1.1.0/mainnet/api/faucet_api.py` & `mainnet-1.1.1/mainnet/api/faucet_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/mainnet/api/mine_api.py` & `mainnet-1.1.1/mainnet/api/mine_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/mainnet/api/smartbch_contract_api.py` & `mainnet-1.1.1/mainnet/api/smartbch_contract_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/mainnet/api/smartbch_sep20_api.py` & `mainnet-1.1.1/mainnet/api/smartbch_sep20_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/mainnet/api/smartbch_wallet_api.py` & `mainnet-1.1.1/mainnet/api/smartbch_wallet_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/mainnet/api/util_api.py` & `mainnet-1.1.1/mainnet/api/util_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/mainnet/api/wallet_api.py` & `mainnet-1.1.1/mainnet/api/wallet_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -1387,15 +1387,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: UtxoResponse
+        :rtype: list[Utxo]
         """
         kwargs['_return_http_data_only'] = True
         return self.get_token_utxos_with_http_info(inline_object, **kwargs)  # noqa: E501
 
     def get_token_utxos_with_http_info(self, inline_object, **kwargs):  # noqa: E501
         """Get token utxos  # noqa: E501
 
@@ -1423,15 +1423,15 @@
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(UtxoResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(list[Utxo], status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
             'inline_object'
         ]
@@ -1487,15 +1487,15 @@
             '/wallet/get_token_utxos', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='UtxoResponse',  # noqa: E501
+            response_type='list[Utxo]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
@@ -3116,15 +3116,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: UtxoResponse
+        :rtype: list[Utxo]
         """
         kwargs['_return_http_data_only'] = True
         return self.utxos_with_http_info(serialized_wallet, **kwargs)  # noqa: E501
 
     def utxos_with_http_info(self, serialized_wallet, **kwargs):  # noqa: E501
         """Get detailed information about unspent outputs (utxos)  # noqa: E501
 
@@ -3152,15 +3152,15 @@
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(UtxoResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(list[Utxo], status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
             'serialized_wallet'
         ]
@@ -3216,15 +3216,15 @@
             '/wallet/utxo', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='UtxoResponse',  # noqa: E501
+            response_type='list[Utxo]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
```

### Comparing `mainnet-1.1.0/mainnet/api/wallet_bcmr_api.py` & `mainnet-1.1.1/mainnet/api/wallet_bcmr_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/mainnet/api/wallet_signed_api.py` & `mainnet-1.1.1/mainnet/api/wallet_signed_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/mainnet/api/wallet_slp_api.py` & `mainnet-1.1.1/mainnet/api/wallet_slp_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/mainnet/api/wallet_util_api.py` & `mainnet-1.1.1/mainnet/api/wallet_util_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/mainnet/api/webhook_api.py` & `mainnet-1.1.1/mainnet/api/webhook_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/mainnet/api_client.py` & `mainnet-1.1.1/mainnet/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
```

### Comparing `mainnet-1.1.0/mainnet/configuration.py` & `mainnet-1.1.1/mainnet/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -378,15 +378,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.18\n"\
+               "Version of the API: 1.1.0\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `mainnet-1.1.0/mainnet/exceptions.py` & `mainnet-1.1.1/mainnet/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `mainnet-1.1.0/mainnet/models/__init__.py` & `mainnet-1.1.1/mainnet/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -134,15 +134,15 @@
 from mainnet.models.token_mint_request import TokenMintRequest
 from mainnet.models.token_mint_request_requests import TokenMintRequestRequests
 from mainnet.models.token_send_request import TokenSendRequest
 from mainnet.models.transaction_history_item import TransactionHistoryItem
 from mainnet.models.unit_type import UnitType
 from mainnet.models.util_decode_transaction_request import UtilDecodeTransactionRequest
 from mainnet.models.utxo import Utxo
-from mainnet.models.utxo_response import UtxoResponse
+from mainnet.models.utxo_token import UtxoToken
 from mainnet.models.verify_signed_message_request import VerifySignedMessageRequest
 from mainnet.models.verify_signed_message_response import VerifySignedMessageResponse
 from mainnet.models.verify_signed_message_response_details import VerifySignedMessageResponseDetails
 from mainnet.models.wallet_info import WalletInfo
 from mainnet.models.wallet_mnemonic import WalletMnemonic
 from mainnet.models.wallet_named_exists_request import WalletNamedExistsRequest
 from mainnet.models.wallet_replace_named_request import WalletReplaceNamedRequest
```

### Comparing `mainnet-1.1.0/mainnet/models/auth_chain_element.py` & `mainnet-1.1.1/mainnet/models/auth_chain_element.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/balance_request.py` & `mainnet-1.1.1/mainnet/models/balance_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/balance_response.py` & `mainnet-1.1.1/mainnet/models/balance_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/cashscript_receipt.py` & `mainnet-1.1.1/mainnet/models/cashscript_receipt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/contract.py` & `mainnet-1.1.1/mainnet/models/contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/contract_fn_request.py` & `mainnet-1.1.1/mainnet/models/contract_fn_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/contract_fn_response.py` & `mainnet-1.1.1/mainnet/models/contract_fn_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/contract_info_request.py` & `mainnet-1.1.1/mainnet/models/contract_info_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/contract_info_response.py` & `mainnet-1.1.1/mainnet/models/contract_info_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -33,44 +33,49 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'contract_id': 'str',
         'script': 'str',
         'parameters': 'list[str]',
-        'cashaddr': 'str'
+        'cashaddr': 'str',
+        'tokenaddr': 'str'
     }
 
     attribute_map = {
         'contract_id': 'contractId',
         'script': 'script',
         'parameters': 'parameters',
-        'cashaddr': 'cashaddr'
+        'cashaddr': 'cashaddr',
+        'tokenaddr': 'tokenaddr'
     }
 
-    def __init__(self, contract_id=None, script=None, parameters=None, cashaddr=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, contract_id=None, script=None, parameters=None, cashaddr=None, tokenaddr=None, local_vars_configuration=None):  # noqa: E501
         """ContractInfoResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._contract_id = None
         self._script = None
         self._parameters = None
         self._cashaddr = None
+        self._tokenaddr = None
         self.discriminator = None
 
         if contract_id is not None:
             self.contract_id = contract_id
         if script is not None:
             self.script = script
         if parameters is not None:
             self.parameters = parameters
         if cashaddr is not None:
             self.cashaddr = cashaddr
+        if tokenaddr is not None:
+            self.tokenaddr = tokenaddr
 
     @property
     def contract_id(self):
         """Gets the contract_id of this ContractInfoResponse.  # noqa: E501
 
         serialized contract   # noqa: E501
 
@@ -154,14 +159,35 @@
 
         :param cashaddr: The cashaddr of this ContractInfoResponse.  # noqa: E501
         :type cashaddr: str
         """
 
         self._cashaddr = cashaddr
 
+    @property
+    def tokenaddr(self):
+        """Gets the tokenaddr of this ContractInfoResponse.  # noqa: E501
+
+
+        :return: The tokenaddr of this ContractInfoResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._tokenaddr
+
+    @tokenaddr.setter
+    def tokenaddr(self, tokenaddr):
+        """Sets the tokenaddr of this ContractInfoResponse.
+
+
+        :param tokenaddr: The tokenaddr of this ContractInfoResponse.  # noqa: E501
+        :type tokenaddr: str
+        """
+
+        self._tokenaddr = tokenaddr
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `mainnet-1.1.0/mainnet/models/contract_request.py` & `mainnet-1.1.1/mainnet/models/contract_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/contract_response.py` & `mainnet-1.1.1/mainnet/models/contract_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/convert_request.py` & `mainnet-1.1.1/mainnet/models/convert_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/create_signed_message_request.py` & `mainnet-1.1.1/mainnet/models/create_signed_message_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/deposit_address_response.py` & `mainnet-1.1.1/mainnet/models/deposit_address_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/electrum_raw_transaction.py` & `mainnet-1.1.1/mainnet/models/electrum_raw_transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/electrum_raw_transaction_script_pub_key.py` & `mainnet-1.1.1/mainnet/models/electrum_raw_transaction_script_pub_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/electrum_raw_transaction_script_sig.py` & `mainnet-1.1.1/mainnet/models/electrum_raw_transaction_script_sig.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/electrum_raw_transaction_vin.py` & `mainnet-1.1.1/mainnet/models/electrum_raw_transaction_vin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/electrum_raw_transaction_vout.py` & `mainnet-1.1.1/mainnet/models/electrum_raw_transaction_vout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/encode_transaction_request.py` & `mainnet-1.1.1/mainnet/models/encode_transaction_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/encode_transaction_response.py` & `mainnet-1.1.1/mainnet/models/encode_transaction_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/error.py` & `mainnet-1.1.1/mainnet/models/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/escrow_contract.py` & `mainnet-1.1.1/mainnet/models/escrow_contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/escrow_fn_request.py` & `mainnet-1.1.1/mainnet/models/escrow_fn_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/escrow_info_request.py` & `mainnet-1.1.1/mainnet/models/escrow_info_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/escrow_info_response.py` & `mainnet-1.1.1/mainnet/models/escrow_info_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/escrow_request.py` & `mainnet-1.1.1/mainnet/models/escrow_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/escrow_response.py` & `mainnet-1.1.1/mainnet/models/escrow_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/get_addresses_response.py` & `mainnet-1.1.1/mainnet/models/get_addresses_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/get_addrs_by_xpub_key_request.py` & `mainnet-1.1.1/mainnet/models/get_addrs_by_xpub_key_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/get_testnet_bch_request.py` & `mainnet-1.1.1/mainnet/models/get_testnet_bch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/get_testnet_bch_response.py` & `mainnet-1.1.1/mainnet/models/get_testnet_bch_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/get_testnet_sbch_request.py` & `mainnet-1.1.1/mainnet/models/get_testnet_sbch_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/get_testnet_sbch_response.py` & `mainnet-1.1.1/mainnet/models/get_testnet_sbch_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/get_testnet_sep20_request.py` & `mainnet-1.1.1/mainnet/models/get_testnet_sep20_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/get_testnet_sep20_response.py` & `mainnet-1.1.1/mainnet/models/get_testnet_sep20_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/get_testnet_slp_request.py` & `mainnet-1.1.1/mainnet/models/get_testnet_slp_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/get_testnet_slp_response.py` & `mainnet-1.1.1/mainnet/models/get_testnet_slp_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/get_xpub_key_info_request.py` & `mainnet-1.1.1/mainnet/models/get_xpub_key_info_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/get_xpub_key_info_response.py` & `mainnet-1.1.1/mainnet/models/get_xpub_key_info_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/history_request.py` & `mainnet-1.1.1/mainnet/models/history_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/history_response.py` & `mainnet-1.1.1/mainnet/models/history_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/inline_object.py` & `mainnet-1.1.1/mainnet/models/inline_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/inline_object1.py` & `mainnet-1.1.1/mainnet/models/inline_object1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/inline_object2.py` & `mainnet-1.1.1/mainnet/models/inline_object2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/inline_object3.py` & `mainnet-1.1.1/mainnet/models/inline_object3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/inline_object4.py` & `mainnet-1.1.1/mainnet/models/inline_object4.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/max_amount_to_send_request.py` & `mainnet-1.1.1/mainnet/models/max_amount_to_send_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/mine_request.py` & `mainnet-1.1.1/mainnet/models/mine_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/network_enum.py` & `mainnet-1.1.1/mainnet/models/network_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/op_return_data.py` & `mainnet-1.1.1/mainnet/models/op_return_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/scalable_vector_graphic.py` & `mainnet-1.1.1/mainnet/models/scalable_vector_graphic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/send_max_request.py` & `mainnet-1.1.1/mainnet/models/send_max_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/send_max_response.py` & `mainnet-1.1.1/mainnet/models/send_max_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/send_request.py` & `mainnet-1.1.1/mainnet/models/send_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/send_request_item.py` & `mainnet-1.1.1/mainnet/models/send_request_item.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/send_request_item_any_of.py` & `mainnet-1.1.1/mainnet/models/send_request_item_any_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/send_request_options.py` & `mainnet-1.1.1/mainnet/models/send_request_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/send_response.py` & `mainnet-1.1.1/mainnet/models/send_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/serialized_wallet.py` & `mainnet-1.1.1/mainnet/models/serialized_wallet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/signed_message_response.py` & `mainnet-1.1.1/mainnet/models/signed_message_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/signed_message_response_details.py` & `mainnet-1.1.1/mainnet/models/signed_message_response_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/signed_message_response_raw.py` & `mainnet-1.1.1/mainnet/models/signed_message_response_raw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/slp_balance_request.py` & `mainnet-1.1.1/mainnet/models/slp_balance_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/slp_balance_response.py` & `mainnet-1.1.1/mainnet/models/slp_balance_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/slp_deposit_address_response.py` & `mainnet-1.1.1/mainnet/models/slp_deposit_address_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/slp_genesis_request.py` & `mainnet-1.1.1/mainnet/models/slp_genesis_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/slp_genesis_response.py` & `mainnet-1.1.1/mainnet/models/slp_genesis_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/slp_mint_request.py` & `mainnet-1.1.1/mainnet/models/slp_mint_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/slp_mint_response.py` & `mainnet-1.1.1/mainnet/models/slp_mint_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/slp_outpoints_response.py` & `mainnet-1.1.1/mainnet/models/slp_outpoints_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/slp_send_max_request.py` & `mainnet-1.1.1/mainnet/models/slp_send_max_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/slp_send_request.py` & `mainnet-1.1.1/mainnet/models/slp_send_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/slp_send_request_item.py` & `mainnet-1.1.1/mainnet/models/slp_send_request_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/slp_send_request_options.py` & `mainnet-1.1.1/mainnet/models/slp_send_request_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/slp_send_response.py` & `mainnet-1.1.1/mainnet/models/slp_send_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/slp_token_info_request.py` & `mainnet-1.1.1/mainnet/models/slp_token_info_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/slp_token_info_response.py` & `mainnet-1.1.1/mainnet/models/slp_token_info_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/slp_utxo.py` & `mainnet-1.1.1/mainnet/models/slp_utxo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/slp_utxo_response.py` & `mainnet-1.1.1/mainnet/models/slp_utxo_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_contract_deploy_request.py` & `mainnet-1.1.1/mainnet/models/smart_bch_contract_deploy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_contract_deploy_response.py` & `mainnet-1.1.1/mainnet/models/smart_bch_contract_deploy_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_contract_estimate_gas_request.py` & `mainnet-1.1.1/mainnet/models/smart_bch_contract_estimate_gas_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_contract_estimate_gas_response.py` & `mainnet-1.1.1/mainnet/models/smart_bch_contract_estimate_gas_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_contract_fn_call_request.py` & `mainnet-1.1.1/mainnet/models/smart_bch_contract_fn_call_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_contract_fn_call_response.py` & `mainnet-1.1.1/mainnet/models/smart_bch_contract_fn_call_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_contract_info_request.py` & `mainnet-1.1.1/mainnet/models/smart_bch_contract_info_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_contract_info_response.py` & `mainnet-1.1.1/mainnet/models/smart_bch_contract_info_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_contract_request.py` & `mainnet-1.1.1/mainnet/models/smart_bch_contract_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_contract_response.py` & `mainnet-1.1.1/mainnet/models/smart_bch_contract_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_deposit_address_response.py` & `mainnet-1.1.1/mainnet/models/smart_bch_deposit_address_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_max_amount_to_send_request.py` & `mainnet-1.1.1/mainnet/models/smart_bch_max_amount_to_send_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_overrides.py` & `mainnet-1.1.1/mainnet/models/smart_bch_overrides.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_send_max_request.py` & `mainnet-1.1.1/mainnet/models/smart_bch_send_max_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_send_request.py` & `mainnet-1.1.1/mainnet/models/smart_bch_send_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_send_request_item.py` & `mainnet-1.1.1/mainnet/models/smart_bch_send_request_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_send_request_item_any_of.py` & `mainnet-1.1.1/mainnet/models/smart_bch_send_request_item_any_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_send_request_options.py` & `mainnet-1.1.1/mainnet/models/smart_bch_send_request_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_send_response_item.py` & `mainnet-1.1.1/mainnet/models/smart_bch_send_response_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_sep20_all_balances_request.py` & `mainnet-1.1.1/mainnet/models/smart_bch_sep20_all_balances_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_sep20_balance_request.py` & `mainnet-1.1.1/mainnet/models/smart_bch_sep20_balance_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_sep20_balance_response.py` & `mainnet-1.1.1/mainnet/models/smart_bch_sep20_balance_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_sep20_genesis_request.py` & `mainnet-1.1.1/mainnet/models/smart_bch_sep20_genesis_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_sep20_genesis_response.py` & `mainnet-1.1.1/mainnet/models/smart_bch_sep20_genesis_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_sep20_mint_request.py` & `mainnet-1.1.1/mainnet/models/smart_bch_sep20_mint_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_sep20_mint_response.py` & `mainnet-1.1.1/mainnet/models/smart_bch_sep20_mint_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_sep20_send_max_request.py` & `mainnet-1.1.1/mainnet/models/smart_bch_sep20_send_max_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_sep20_send_request.py` & `mainnet-1.1.1/mainnet/models/smart_bch_sep20_send_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_sep20_send_request_item.py` & `mainnet-1.1.1/mainnet/models/smart_bch_sep20_send_request_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_sep20_token_info_request.py` & `mainnet-1.1.1/mainnet/models/smart_bch_sep20_token_info_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_sep20_token_info_response.py` & `mainnet-1.1.1/mainnet/models/smart_bch_sep20_token_info_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/smart_bch_transaction_receipt.py` & `mainnet-1.1.1/mainnet/models/smart_bch_transaction_receipt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/submit_transaction_request.py` & `mainnet-1.1.1/mainnet/models/submit_transaction_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/submit_transaction_response.py` & `mainnet-1.1.1/mainnet/models/submit_transaction_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/token_burn_request.py` & `mainnet-1.1.1/mainnet/models/token_burn_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/token_genesis_request.py` & `mainnet-1.1.1/mainnet/models/token_genesis_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/token_mint_request.py` & `mainnet-1.1.1/mainnet/models/token_mint_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/token_mint_request_requests.py` & `mainnet-1.1.1/mainnet/models/token_mint_request_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/token_send_request.py` & `mainnet-1.1.1/mainnet/models/token_send_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/transaction_history_item.py` & `mainnet-1.1.1/mainnet/models/transaction_history_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/unit_type.py` & `mainnet-1.1.1/mainnet/models/unit_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -38,15 +38,14 @@
     }
 
     attribute_map = {
         'unit': 'unit'
     }
 
     discriminator_value_class_map = {
-        'Utxo': 'Utxo',
         'BalanceRequest': 'BalanceRequest'
     }
 
     def __init__(self, unit=None, local_vars_configuration=None):  # noqa: E501
         """UnitType - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
```

### Comparing `mainnet-1.1.0/mainnet/models/util_decode_transaction_request.py` & `mainnet-1.1.1/mainnet/models/util_decode_transaction_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/utxo.py` & `mainnet-1.1.1/mainnet/models/utxo.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -30,138 +30,135 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'index': 'float',
-        'tx_id': 'str',
-        'value': 'float',
-        'utxo_id': 'str'
+        'vout': 'float',
+        'txid': 'str',
+        'satoshis': 'float',
+        'token': 'UtxoToken'
     }
 
     attribute_map = {
-        'index': 'index',
-        'tx_id': 'txId',
-        'value': 'value',
-        'utxo_id': 'utxoId'
+        'vout': 'vout',
+        'txid': 'txid',
+        'satoshis': 'satoshis',
+        'token': 'token'
     }
 
-    def __init__(self, index=None, tx_id=None, value=None, utxo_id=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, vout=None, txid=None, satoshis=None, token=None, local_vars_configuration=None):  # noqa: E501
         """Utxo - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._index = None
-        self._tx_id = None
-        self._value = None
-        self._utxo_id = None
+        self._vout = None
+        self._txid = None
+        self._satoshis = None
+        self._token = None
         self.discriminator = None
 
-        if index is not None:
-            self.index = index
-        self.tx_id = tx_id
-        self.value = value
-        self.utxo_id = utxo_id
+        self.vout = vout
+        self.txid = txid
+        self.satoshis = satoshis
+        self.token = token
 
     @property
-    def index(self):
-        """Gets the index of this Utxo.  # noqa: E501
+    def vout(self):
+        """Gets the vout of this Utxo.  # noqa: E501
 
 
-        :return: The index of this Utxo.  # noqa: E501
+        :return: The vout of this Utxo.  # noqa: E501
         :rtype: float
         """
-        return self._index
+        return self._vout
 
-    @index.setter
-    def index(self, index):
-        """Sets the index of this Utxo.
+    @vout.setter
+    def vout(self, vout):
+        """Sets the vout of this Utxo.
 
 
-        :param index: The index of this Utxo.  # noqa: E501
-        :type index: float
+        :param vout: The vout of this Utxo.  # noqa: E501
+        :type vout: float
         """
+        if self.local_vars_configuration.client_side_validation and vout is None:  # noqa: E501
+            raise ValueError("Invalid value for `vout`, must not be `None`")  # noqa: E501
 
-        self._index = index
+        self._vout = vout
 
     @property
-    def tx_id(self):
-        """Gets the tx_id of this Utxo.  # noqa: E501
+    def txid(self):
+        """Gets the txid of this Utxo.  # noqa: E501
 
         The hash of a transaction  # noqa: E501
 
-        :return: The tx_id of this Utxo.  # noqa: E501
+        :return: The txid of this Utxo.  # noqa: E501
         :rtype: str
         """
-        return self._tx_id
+        return self._txid
 
-    @tx_id.setter
-    def tx_id(self, tx_id):
-        """Sets the tx_id of this Utxo.
+    @txid.setter
+    def txid(self, txid):
+        """Sets the txid of this Utxo.
 
         The hash of a transaction  # noqa: E501
 
-        :param tx_id: The tx_id of this Utxo.  # noqa: E501
-        :type tx_id: str
+        :param txid: The txid of this Utxo.  # noqa: E501
+        :type txid: str
         """
-        if self.local_vars_configuration.client_side_validation and tx_id is None:  # noqa: E501
-            raise ValueError("Invalid value for `tx_id`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and txid is None:  # noqa: E501
+            raise ValueError("Invalid value for `txid`, must not be `None`")  # noqa: E501
 
-        self._tx_id = tx_id
+        self._txid = txid
 
     @property
-    def value(self):
-        """Gets the value of this Utxo.  # noqa: E501
+    def satoshis(self):
+        """Gets the satoshis of this Utxo.  # noqa: E501
 
 
-        :return: The value of this Utxo.  # noqa: E501
+        :return: The satoshis of this Utxo.  # noqa: E501
         :rtype: float
         """
-        return self._value
+        return self._satoshis
 
-    @value.setter
-    def value(self, value):
-        """Sets the value of this Utxo.
+    @satoshis.setter
+    def satoshis(self, satoshis):
+        """Sets the satoshis of this Utxo.
 
 
-        :param value: The value of this Utxo.  # noqa: E501
-        :type value: float
+        :param satoshis: The satoshis of this Utxo.  # noqa: E501
+        :type satoshis: float
         """
-        if self.local_vars_configuration.client_side_validation and value is None:  # noqa: E501
-            raise ValueError("Invalid value for `value`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and satoshis is None:  # noqa: E501
+            raise ValueError("Invalid value for `satoshis`, must not be `None`")  # noqa: E501
 
-        self._value = value
+        self._satoshis = satoshis
 
     @property
-    def utxo_id(self):
-        """Gets the utxo_id of this Utxo.  # noqa: E501
+    def token(self):
+        """Gets the token of this Utxo.  # noqa: E501
 
-        serialized outpoint  # noqa: E501
 
-        :return: The utxo_id of this Utxo.  # noqa: E501
-        :rtype: str
+        :return: The token of this Utxo.  # noqa: E501
+        :rtype: UtxoToken
         """
-        return self._utxo_id
+        return self._token
 
-    @utxo_id.setter
-    def utxo_id(self, utxo_id):
-        """Sets the utxo_id of this Utxo.
+    @token.setter
+    def token(self, token):
+        """Sets the token of this Utxo.
 
-        serialized outpoint  # noqa: E501
 
-        :param utxo_id: The utxo_id of this Utxo.  # noqa: E501
-        :type utxo_id: str
+        :param token: The token of this Utxo.  # noqa: E501
+        :type token: UtxoToken
         """
-        if self.local_vars_configuration.client_side_validation and utxo_id is None:  # noqa: E501
-            raise ValueError("Invalid value for `utxo_id`, must not be `None`")  # noqa: E501
 
-        self._utxo_id = utxo_id
+        self._token = token
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
```

### Comparing `mainnet-1.1.0/mainnet/models/utxo_response.py` & `mainnet-1.1.1/mainnet/models/wif.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,82 +1,84 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from mainnet.configuration import Configuration
 
 
-class UtxoResponse(object):
+class Wif(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'utxos': 'list[Utxo]'
+        'wif': 'str'
     }
 
     attribute_map = {
-        'utxos': 'utxos'
+        'wif': 'wif'
     }
 
-    def __init__(self, utxos=None, local_vars_configuration=None):  # noqa: E501
-        """UtxoResponse - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, wif=None, local_vars_configuration=None):  # noqa: E501
+        """Wif - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._utxos = None
+        self._wif = None
         self.discriminator = None
 
-        if utxos is not None:
-            self.utxos = utxos
+        if wif is not None:
+            self.wif = wif
 
     @property
-    def utxos(self):
-        """Gets the utxos of this UtxoResponse.  # noqa: E501
+    def wif(self):
+        """Gets the wif of this Wif.  # noqa: E501
 
+        The wallet in Wallet Import Format (WIF)   # noqa: E501
 
-        :return: The utxos of this UtxoResponse.  # noqa: E501
-        :rtype: list[Utxo]
+        :return: The wif of this Wif.  # noqa: E501
+        :rtype: str
         """
-        return self._utxos
+        return self._wif
 
-    @utxos.setter
-    def utxos(self, utxos):
-        """Sets the utxos of this UtxoResponse.
+    @wif.setter
+    def wif(self, wif):
+        """Sets the wif of this Wif.
 
+        The wallet in Wallet Import Format (WIF)   # noqa: E501
 
-        :param utxos: The utxos of this UtxoResponse.  # noqa: E501
-        :type utxos: list[Utxo]
+        :param wif: The wif of this Wif.  # noqa: E501
+        :type wif: str
         """
 
-        self._utxos = utxos
+        self._wif = wif
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -104,18 +106,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UtxoResponse):
+        if not isinstance(other, Wif):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, UtxoResponse):
+        if not isinstance(other, Wif):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `mainnet-1.1.0/mainnet/models/verify_signed_message_request.py` & `mainnet-1.1.1/mainnet/models/verify_signed_message_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/verify_signed_message_response.py` & `mainnet-1.1.1/mainnet/models/verify_signed_message_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/verify_signed_message_response_details.py` & `mainnet-1.1.1/mainnet/models/verify_signed_message_response_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/wallet_info.py` & `mainnet-1.1.1/mainnet/models/wallet_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/wallet_mnemonic.py` & `mainnet-1.1.1/mainnet/models/wallet_mnemonic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/wallet_named_exists_request.py` & `mainnet-1.1.1/mainnet/models/wallet_named_exists_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/wallet_replace_named_request.py` & `mainnet-1.1.1/mainnet/models/wallet_replace_named_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/wallet_request.py` & `mainnet-1.1.1/mainnet/models/wallet_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/wallet_response.py` & `mainnet-1.1.1/mainnet/models/wallet_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/wallet_type.py` & `mainnet-1.1.1/mainnet/models/wallet_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/watch_address_request.py` & `mainnet-1.1.1/mainnet/models/watch_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/watch_address_response.py` & `mainnet-1.1.1/mainnet/models/watch_address_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/wif.py` & `mainnet-1.1.1/mainnet/models/x_pub_key_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,84 +1,82 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from mainnet.configuration import Configuration
 
 
-class Wif(object):
+class XPubKeyResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'wif': 'str'
+        'xpubkeys': 'list[XPubKey]'
     }
 
     attribute_map = {
-        'wif': 'wif'
+        'xpubkeys': 'xpubkeys'
     }
 
-    def __init__(self, wif=None, local_vars_configuration=None):  # noqa: E501
-        """Wif - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, xpubkeys=None, local_vars_configuration=None):  # noqa: E501
+        """XPubKeyResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._wif = None
+        self._xpubkeys = None
         self.discriminator = None
 
-        if wif is not None:
-            self.wif = wif
+        if xpubkeys is not None:
+            self.xpubkeys = xpubkeys
 
     @property
-    def wif(self):
-        """Gets the wif of this Wif.  # noqa: E501
+    def xpubkeys(self):
+        """Gets the xpubkeys of this XPubKeyResponse.  # noqa: E501
 
-        The wallet in Wallet Import Format (WIF)   # noqa: E501
 
-        :return: The wif of this Wif.  # noqa: E501
-        :rtype: str
+        :return: The xpubkeys of this XPubKeyResponse.  # noqa: E501
+        :rtype: list[XPubKey]
         """
-        return self._wif
+        return self._xpubkeys
 
-    @wif.setter
-    def wif(self, wif):
-        """Sets the wif of this Wif.
+    @xpubkeys.setter
+    def xpubkeys(self, xpubkeys):
+        """Sets the xpubkeys of this XPubKeyResponse.
 
-        The wallet in Wallet Import Format (WIF)   # noqa: E501
 
-        :param wif: The wif of this Wif.  # noqa: E501
-        :type wif: str
+        :param xpubkeys: The xpubkeys of this XPubKeyResponse.  # noqa: E501
+        :type xpubkeys: list[XPubKey]
         """
 
-        self._wif = wif
+        self._xpubkeys = xpubkeys
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -106,18 +104,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Wif):
+        if not isinstance(other, XPubKeyResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Wif):
+        if not isinstance(other, XPubKeyResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `mainnet-1.1.0/mainnet/models/x_pub_key.py` & `mainnet-1.1.1/mainnet/models/x_pub_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/x_pub_key_request.py` & `mainnet-1.1.1/mainnet/models/x_pub_key_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/models/zero_balance_response.py` & `mainnet-1.1.1/mainnet/models/zero_balance_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `mainnet-1.1.0/mainnet/rest.py` & `mainnet-1.1.1/mainnet/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/mainnet.egg-info/SOURCES.txt` & `mainnet-1.1.1/mainnet.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 mainnet/models/token_mint_request.py
 mainnet/models/token_mint_request_requests.py
 mainnet/models/token_send_request.py
 mainnet/models/transaction_history_item.py
 mainnet/models/unit_type.py
 mainnet/models/util_decode_transaction_request.py
 mainnet/models/utxo.py
-mainnet/models/utxo_response.py
+mainnet/models/utxo_token.py
 mainnet/models/verify_signed_message_request.py
 mainnet/models/verify_signed_message_response.py
 mainnet/models/verify_signed_message_response_details.py
 mainnet/models/wallet_info.py
 mainnet/models/wallet_mnemonic.py
 mainnet/models/wallet_named_exists_request.py
 mainnet/models/wallet_replace_named_request.py
@@ -295,15 +295,15 @@
 test/test_token_mint_request_requests.py
 test/test_token_send_request.py
 test/test_transaction_history_item.py
 test/test_unit_type.py
 test/test_util_api.py
 test/test_util_decode_transaction_request.py
 test/test_utxo.py
-test/test_utxo_response.py
+test/test_utxo_token.py
 test/test_verify_signed_message_request.py
 test/test_verify_signed_message_response.py
 test/test_verify_signed_message_response_details.py
 test/test_wallet_api.py
 test/test_wallet_bcmr_api.py
 test/test_wallet_info.py
 test/test_wallet_mnemonic.py
```

### Comparing `mainnet-1.1.0/setup.py` & `mainnet-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
-    A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.1.0.   # noqa: E501
+    A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.1.1.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "mainnet"
-VERSION = "1.1.0"
+VERSION = "1.1.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -33,10 +33,10 @@
     url="",
     keywords=["OpenAPI", "OpenAPI-Generator", "Mainnet Cash"],
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     license="MIT Licence",
     long_description="""\
-    A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.1.0.   # noqa: E501
+    A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.1.1.   # noqa: E501
     """
 )
```

### Comparing `mainnet-1.1.0/test/test_auth_chain_element.py` & `mainnet-1.1.1/test/test_auth_chain_element.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_balance_request.py` & `mainnet-1.1.1/test/test_balance_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_balance_response.py` & `mainnet-1.1.1/test/test_balance_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_cashscript_receipt.py` & `mainnet-1.1.1/test/test_cashscript_receipt.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_contract.py` & `mainnet-1.1.1/test/test_contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_contract_api.py` & `mainnet-1.1.1/test/test_contract_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_contract_escrow_api.py` & `mainnet-1.1.1/test/test_contract_escrow_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_contract_fn_request.py` & `mainnet-1.1.1/test/test_contract_fn_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_contract_fn_response.py` & `mainnet-1.1.1/test/test_contract_fn_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_contract_info_request.py` & `mainnet-1.1.1/test/test_contract_info_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_contract_info_response.py` & `mainnet-1.1.1/test/test_smart_bch_contract_info_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import mainnet
-from mainnet.models.contract_info_response import ContractInfoResponse  # noqa: E501
+from mainnet.models.smart_bch_contract_info_response import SmartBchContractInfoResponse  # noqa: E501
 from mainnet.rest import ApiException
 
-class TestContractInfoResponse(unittest.TestCase):
-    """ContractInfoResponse unit test stubs"""
+class TestSmartBchContractInfoResponse(unittest.TestCase):
+    """SmartBchContractInfoResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test ContractInfoResponse
+        """Test SmartBchContractInfoResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = mainnet.models.contract_info_response.ContractInfoResponse()  # noqa: E501
+        # model = mainnet.models.smart_bch_contract_info_response.SmartBchContractInfoResponse()  # noqa: E501
         if include_optional :
-            return ContractInfoResponse(
+            return SmartBchContractInfoResponse(
                 contract_id = '0', 
-                script = 'contract TransferWithTimeout(pubkey sender, pubkey recipient, int timeout) {
-    function transfer(sig recipientSig) {
-        require(checkSig(recipientSig, recipient));
-    }
-
-    function timeout(sig senderSig) {
-        require(checkSig(senderSig, sender));
-        require(tx.time >= timeout);
-    }
-}            
+                address = '0', 
+                abi = - ["function name() view returns (string)"]
+- ["function symbol() view returns (string)"]
+, 
+                script = '// SPDX-License-Identifier: MIT
+pragma solidity ^0.8.2;
+
+import "@openzeppelin/contracts/token/SEP20/SEP20.sol";
+
+contract MyToken is SEP20 {
+  constructor(string memory name, string memory symbol) SEP20(name, symbol) {}
+}
 ', 
-                parameters = ["03410ef048b3da351793f6ed14cc2fde460becc5b658d9138443b9a3000707a6a7","034978ac464f358b235f11212eb6e017af90215b90b1ff7471d9ae2abb5e09263b",215], 
-                cashaddr = 'bchtest:qpalhxhl05mlhms3ys43u76rn0ttdv3qg2usm4nm7t'
+                parameters = ["MyToken","MTK"]
             )
         else :
-            return ContractInfoResponse(
+            return SmartBchContractInfoResponse(
         )
 
-    def testContractInfoResponse(self):
-        """Test ContractInfoResponse"""
+    def testSmartBchContractInfoResponse(self):
+        """Test SmartBchContractInfoResponse"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mainnet-1.1.0/test/test_contract_request.py` & `mainnet-1.1.1/test/test_contract_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_contract_response.py` & `mainnet-1.1.1/test/test_contract_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_convert_request.py` & `mainnet-1.1.1/test/test_convert_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_create_signed_message_request.py` & `mainnet-1.1.1/test/test_create_signed_message_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_deposit_address_response.py` & `mainnet-1.1.1/test/test_deposit_address_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_electrum_raw_transaction.py` & `mainnet-1.1.1/test/test_electrum_raw_transaction.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_electrum_raw_transaction_script_pub_key.py` & `mainnet-1.1.1/test/test_electrum_raw_transaction_script_pub_key.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_electrum_raw_transaction_script_sig.py` & `mainnet-1.1.1/test/test_electrum_raw_transaction_script_sig.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_electrum_raw_transaction_vin.py` & `mainnet-1.1.1/test/test_electrum_raw_transaction_vin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_electrum_raw_transaction_vout.py` & `mainnet-1.1.1/test/test_electrum_raw_transaction_vout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_encode_transaction_request.py` & `mainnet-1.1.1/test/test_encode_transaction_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_encode_transaction_response.py` & `mainnet-1.1.1/test/test_encode_transaction_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_error.py` & `mainnet-1.1.1/test/test_mine_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import mainnet
-from mainnet.models.error import Error  # noqa: E501
+from mainnet.models.mine_request import MineRequest  # noqa: E501
 from mainnet.rest import ApiException
 
-class TestError(unittest.TestCase):
-    """Error unit test stubs"""
+class TestMineRequest(unittest.TestCase):
+    """MineRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test Error
+        """Test MineRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = mainnet.models.error.Error()  # noqa: E501
+        # model = mainnet.models.mine_request.MineRequest()  # noqa: E501
         if include_optional :
-            return Error(
-                message = '0', 
-                code = 1.337
+            return MineRequest(
+                cashaddr = 'bchreg:qpttdv3qg2usm4nm7talhxhl05mlhms3ys43u76rn0', 
+                blocks = 105
             )
         else :
-            return Error(
+            return MineRequest(
         )
 
-    def testError(self):
-        """Test Error"""
+    def testMineRequest(self):
+        """Test MineRequest"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mainnet-1.1.0/test/test_escrow_contract.py` & `mainnet-1.1.1/test/test_escrow_contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_escrow_fn_request.py` & `mainnet-1.1.1/test/test_escrow_fn_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_escrow_info_request.py` & `mainnet-1.1.1/test/test_escrow_info_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_escrow_info_response.py` & `mainnet-1.1.1/test/test_escrow_info_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -54,15 +54,15 @@
         require(hash160(signingPk) == arbiterPkh||hash160(signingPk) == sellerPkh);
         require(checkSig(s, signingPk));
         require(amount >= contractAmount);
         require(nonce == contractNonce);
         bytes34 output = new OutputP2PKH(bytes8(amount), buyerPkh);
         require(hash256(output) == tx.hashOutputs);
     }
-}            
+}
 ', 
                 parameters = ["9ef0d8bf4c1f62a68c4c647beb404ec1d458f3c5","e7fe7119a6bb73409a087e0ac46cefada815b69f","a01c11c6deea905d25b487698f1140e0c53396c8",10000,1996128042], 
                 cashaddr = 'bchtest:prxla49zwqm8m2nzgn82qza3ssrqnpt8vgv60hlwm2', 
                 buyer_addr = bchtest:qrnluuge56ahxsy6pplq43rva7k6s9dknu4p5278ah, 
                 arbiter_addr = bchtest:qzspcywxmm4fqhf9kjrknrc3grsv2vukeqyjqla0nt, 
                 seller_addr = bchtest:qz00pk9lfs0k9f5vf3j8h66qfmqagk8nc56elq4dv2, 
                 amount = 10000,
```

### Comparing `mainnet-1.1.0/test/test_escrow_request.py` & `mainnet-1.1.1/test/test_escrow_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_escrow_response.py` & `mainnet-1.1.1/test/test_escrow_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_faucet_api.py` & `mainnet-1.1.1/test/test_faucet_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_get_addresses_response.py` & `mainnet-1.1.1/test/test_get_addresses_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_get_addrs_by_xpub_key_request.py` & `mainnet-1.1.1/test/test_get_addrs_by_xpub_key_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_get_testnet_bch_request.py` & `mainnet-1.1.1/test/test_get_testnet_sbch_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import mainnet
-from mainnet.models.get_testnet_bch_request import GetTestnetBchRequest  # noqa: E501
+from mainnet.models.get_testnet_sbch_request import GetTestnetSbchRequest  # noqa: E501
 from mainnet.rest import ApiException
 
-class TestGetTestnetBchRequest(unittest.TestCase):
-    """GetTestnetBchRequest unit test stubs"""
+class TestGetTestnetSbchRequest(unittest.TestCase):
+    """GetTestnetSbchRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test GetTestnetBchRequest
+        """Test GetTestnetSbchRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = mainnet.models.get_testnet_bch_request.GetTestnetBchRequest()  # noqa: E501
+        # model = mainnet.models.get_testnet_sbch_request.GetTestnetSbchRequest()  # noqa: E501
         if include_optional :
-            return GetTestnetBchRequest(
-                cashaddr = '0'
+            return GetTestnetSbchRequest(
+                address = '0'
             )
         else :
-            return GetTestnetBchRequest(
+            return GetTestnetSbchRequest(
         )
 
-    def testGetTestnetBchRequest(self):
-        """Test GetTestnetBchRequest"""
+    def testGetTestnetSbchRequest(self):
+        """Test GetTestnetSbchRequest"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mainnet-1.1.0/test/test_get_testnet_bch_response.py` & `mainnet-1.1.1/test/test_get_testnet_bch_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_get_testnet_sbch_request.py` & `mainnet-1.1.1/test/test_get_testnet_sbch_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import mainnet
-from mainnet.models.get_testnet_sbch_request import GetTestnetSbchRequest  # noqa: E501
+from mainnet.models.get_testnet_sbch_response import GetTestnetSbchResponse  # noqa: E501
 from mainnet.rest import ApiException
 
-class TestGetTestnetSbchRequest(unittest.TestCase):
-    """GetTestnetSbchRequest unit test stubs"""
+class TestGetTestnetSbchResponse(unittest.TestCase):
+    """GetTestnetSbchResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test GetTestnetSbchRequest
+        """Test GetTestnetSbchResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = mainnet.models.get_testnet_sbch_request.GetTestnetSbchRequest()  # noqa: E501
+        # model = mainnet.models.get_testnet_sbch_response.GetTestnetSbchResponse()  # noqa: E501
         if include_optional :
-            return GetTestnetSbchRequest(
-                address = '0'
+            return GetTestnetSbchResponse(
+                success = True
             )
         else :
-            return GetTestnetSbchRequest(
+            return GetTestnetSbchResponse(
         )
 
-    def testGetTestnetSbchRequest(self):
-        """Test GetTestnetSbchRequest"""
+    def testGetTestnetSbchResponse(self):
+        """Test GetTestnetSbchResponse"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mainnet-1.1.0/test/test_get_testnet_sbch_response.py` & `mainnet-1.1.1/test/test_get_testnet_sep20_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import mainnet
-from mainnet.models.get_testnet_sbch_response import GetTestnetSbchResponse  # noqa: E501
+from mainnet.models.get_testnet_sep20_response import GetTestnetSep20Response  # noqa: E501
 from mainnet.rest import ApiException
 
-class TestGetTestnetSbchResponse(unittest.TestCase):
-    """GetTestnetSbchResponse unit test stubs"""
+class TestGetTestnetSep20Response(unittest.TestCase):
+    """GetTestnetSep20Response unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test GetTestnetSbchResponse
+        """Test GetTestnetSep20Response
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = mainnet.models.get_testnet_sbch_response.GetTestnetSbchResponse()  # noqa: E501
+        # model = mainnet.models.get_testnet_sep20_response.GetTestnetSep20Response()  # noqa: E501
         if include_optional :
-            return GetTestnetSbchResponse(
+            return GetTestnetSep20Response(
                 success = True
             )
         else :
-            return GetTestnetSbchResponse(
+            return GetTestnetSep20Response(
         )
 
-    def testGetTestnetSbchResponse(self):
-        """Test GetTestnetSbchResponse"""
+    def testGetTestnetSep20Response(self):
+        """Test GetTestnetSep20Response"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mainnet-1.1.0/test/test_get_testnet_sep20_request.py` & `mainnet-1.1.1/test/test_get_testnet_sep20_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_get_testnet_sep20_response.py` & `mainnet-1.1.1/test/test_get_testnet_slp_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import mainnet
-from mainnet.models.get_testnet_sep20_response import GetTestnetSep20Response  # noqa: E501
+from mainnet.models.get_testnet_slp_response import GetTestnetSlpResponse  # noqa: E501
 from mainnet.rest import ApiException
 
-class TestGetTestnetSep20Response(unittest.TestCase):
-    """GetTestnetSep20Response unit test stubs"""
+class TestGetTestnetSlpResponse(unittest.TestCase):
+    """GetTestnetSlpResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test GetTestnetSep20Response
+        """Test GetTestnetSlpResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = mainnet.models.get_testnet_sep20_response.GetTestnetSep20Response()  # noqa: E501
+        # model = mainnet.models.get_testnet_slp_response.GetTestnetSlpResponse()  # noqa: E501
         if include_optional :
-            return GetTestnetSep20Response(
-                success = True
+            return GetTestnetSlpResponse(
+                tx_id = '0'
             )
         else :
-            return GetTestnetSep20Response(
+            return GetTestnetSlpResponse(
         )
 
-    def testGetTestnetSep20Response(self):
-        """Test GetTestnetSep20Response"""
+    def testGetTestnetSlpResponse(self):
+        """Test GetTestnetSlpResponse"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mainnet-1.1.0/test/test_get_testnet_slp_request.py` & `mainnet-1.1.1/test/test_get_testnet_slp_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_get_testnet_slp_response.py` & `mainnet-1.1.1/test/test_token_burn_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,61 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import mainnet
-from mainnet.models.get_testnet_slp_response import GetTestnetSlpResponse  # noqa: E501
+from mainnet.models.token_burn_request import TokenBurnRequest  # noqa: E501
 from mainnet.rest import ApiException
 
-class TestGetTestnetSlpResponse(unittest.TestCase):
-    """GetTestnetSlpResponse unit test stubs"""
+class TestTokenBurnRequest(unittest.TestCase):
+    """TokenBurnRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test GetTestnetSlpResponse
+        """Test TokenBurnRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = mainnet.models.get_testnet_slp_response.GetTestnetSlpResponse()  # noqa: E501
+        # model = mainnet.models.token_burn_request.TokenBurnRequest()  # noqa: E501
         if include_optional :
-            return GetTestnetSlpResponse(
-                tx_id = '0'
+            return TokenBurnRequest(
+                wallet_id = '0', 
+                token_id = '0', 
+                capability = 'none', 
+                commitment = '0', 
+                amount = 1.337, 
+                cashaddr = '0', 
+                message = '0'
             )
         else :
-            return GetTestnetSlpResponse(
+            return TokenBurnRequest(
+                wallet_id = '0',
+                token_id = '0',
         )
 
-    def testGetTestnetSlpResponse(self):
-        """Test GetTestnetSlpResponse"""
+    def testTokenBurnRequest(self):
+        """Test TokenBurnRequest"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mainnet-1.1.0/test/test_get_xpub_key_info_request.py` & `mainnet-1.1.1/test/test_get_xpub_key_info_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_get_xpub_key_info_response.py` & `mainnet-1.1.1/test/test_get_xpub_key_info_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_history_request.py` & `mainnet-1.1.1/test/test_history_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_history_response.py` & `mainnet-1.1.1/test/test_history_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_inline_object.py` & `mainnet-1.1.1/test/test_inline_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_inline_object1.py` & `mainnet-1.1.1/test/test_inline_object1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_inline_object2.py` & `mainnet-1.1.1/test/test_inline_object2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_inline_object3.py` & `mainnet-1.1.1/test/test_inline_object3.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_inline_object4.py` & `mainnet-1.1.1/test/test_inline_object4.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_max_amount_to_send_request.py` & `mainnet-1.1.1/test/test_max_amount_to_send_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_mine_api.py` & `mainnet-1.1.1/test/test_mine_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_mine_request.py` & `mainnet-1.1.1/test/test_get_testnet_bch_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import mainnet
-from mainnet.models.mine_request import MineRequest  # noqa: E501
+from mainnet.models.get_testnet_bch_request import GetTestnetBchRequest  # noqa: E501
 from mainnet.rest import ApiException
 
-class TestMineRequest(unittest.TestCase):
-    """MineRequest unit test stubs"""
+class TestGetTestnetBchRequest(unittest.TestCase):
+    """GetTestnetBchRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test MineRequest
+        """Test GetTestnetBchRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = mainnet.models.mine_request.MineRequest()  # noqa: E501
+        # model = mainnet.models.get_testnet_bch_request.GetTestnetBchRequest()  # noqa: E501
         if include_optional :
-            return MineRequest(
-                cashaddr = 'bchreg:qpttdv3qg2usm4nm7talhxhl05mlhms3ys43u76rn0', 
-                blocks = 105
+            return GetTestnetBchRequest(
+                cashaddr = '0'
             )
         else :
-            return MineRequest(
+            return GetTestnetBchRequest(
         )
 
-    def testMineRequest(self):
-        """Test MineRequest"""
+    def testGetTestnetBchRequest(self):
+        """Test GetTestnetBchRequest"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mainnet-1.1.0/test/test_network_enum.py` & `mainnet-1.1.1/test/test_network_enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_op_return_data.py` & `mainnet-1.1.1/test/test_op_return_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_scalable_vector_graphic.py` & `mainnet-1.1.1/test/test_scalable_vector_graphic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_send_max_request.py` & `mainnet-1.1.1/test/test_send_max_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_send_max_response.py` & `mainnet-1.1.1/test/test_send_max_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_send_request.py` & `mainnet-1.1.1/test/test_send_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_send_request_item.py` & `mainnet-1.1.1/test/test_send_request_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_send_request_item_any_of.py` & `mainnet-1.1.1/test/test_send_request_item_any_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_send_request_options.py` & `mainnet-1.1.1/test/test_send_request_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_send_response.py` & `mainnet-1.1.1/test/test_send_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_serialized_wallet.py` & `mainnet-1.1.1/test/test_serialized_wallet.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_signed_message_response.py` & `mainnet-1.1.1/test/test_signed_message_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_signed_message_response_details.py` & `mainnet-1.1.1/test/test_signed_message_response_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_signed_message_response_raw.py` & `mainnet-1.1.1/test/test_signed_message_response_raw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_slp_balance_request.py` & `mainnet-1.1.1/test/test_slp_balance_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_slp_balance_response.py` & `mainnet-1.1.1/test/test_slp_balance_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_slp_deposit_address_response.py` & `mainnet-1.1.1/test/test_slp_deposit_address_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_slp_genesis_request.py` & `mainnet-1.1.1/test/test_slp_genesis_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_slp_genesis_response.py` & `mainnet-1.1.1/test/test_slp_genesis_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_slp_mint_request.py` & `mainnet-1.1.1/test/test_slp_mint_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_slp_mint_response.py` & `mainnet-1.1.1/test/test_slp_mint_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_slp_outpoints_response.py` & `mainnet-1.1.1/test/test_slp_outpoints_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_slp_send_max_request.py` & `mainnet-1.1.1/test/test_slp_send_max_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_slp_send_request.py` & `mainnet-1.1.1/test/test_slp_send_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_slp_send_request_item.py` & `mainnet-1.1.1/test/test_slp_send_request_item.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_slp_send_request_options.py` & `mainnet-1.1.1/test/test_slp_send_request_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_slp_send_response.py` & `mainnet-1.1.1/test/test_slp_send_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_slp_token_info_request.py` & `mainnet-1.1.1/test/test_slp_token_info_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_slp_token_info_response.py` & `mainnet-1.1.1/test/test_slp_token_info_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_slp_utxo.py` & `mainnet-1.1.1/test/test_slp_utxo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_slp_utxo_response.py` & `mainnet-1.1.1/test/test_slp_utxo_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_contract_deploy_request.py` & `mainnet-1.1.1/test/test_smart_bch_contract_deploy_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_contract_deploy_response.py` & `mainnet-1.1.1/test/test_smart_bch_contract_deploy_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_contract_estimate_gas_request.py` & `mainnet-1.1.1/test/test_smart_bch_contract_estimate_gas_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_contract_estimate_gas_response.py` & `mainnet-1.1.1/test/test_smart_bch_contract_estimate_gas_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_contract_fn_call_request.py` & `mainnet-1.1.1/test/test_smart_bch_contract_fn_call_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_contract_fn_call_response.py` & `mainnet-1.1.1/test/test_smart_bch_contract_fn_call_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_contract_info_request.py` & `mainnet-1.1.1/test/test_smart_bch_contract_info_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_contract_info_response.py` & `mainnet-1.1.1/test/test_smart_bch_deposit_address_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,53 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import mainnet
-from mainnet.models.smart_bch_contract_info_response import SmartBchContractInfoResponse  # noqa: E501
+from mainnet.models.smart_bch_deposit_address_response import SmartBchDepositAddressResponse  # noqa: E501
 from mainnet.rest import ApiException
 
-class TestSmartBchContractInfoResponse(unittest.TestCase):
-    """SmartBchContractInfoResponse unit test stubs"""
+class TestSmartBchDepositAddressResponse(unittest.TestCase):
+    """SmartBchDepositAddressResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SmartBchContractInfoResponse
+        """Test SmartBchDepositAddressResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = mainnet.models.smart_bch_contract_info_response.SmartBchContractInfoResponse()  # noqa: E501
+        # model = mainnet.models.smart_bch_deposit_address_response.SmartBchDepositAddressResponse()  # noqa: E501
         if include_optional :
-            return SmartBchContractInfoResponse(
-                contract_id = '0', 
-                address = '0', 
-                abi = - ["function name() view returns (string)"]
-- ["function symbol() view returns (string)"]
-, 
-                script = '// SPDX-License-Identifier: MIT
-pragma solidity ^0.8.2;
-
-import "@openzeppelin/contracts/token/SEP20/SEP20.sol";
-
-contract MyToken is SEP20 {
-  constructor(string memory name, string memory symbol) SEP20(name, symbol) {}
-}
-', 
-                parameters = ["MyToken","MTK"]
+            return SmartBchDepositAddressResponse(
+                address = '0xE25ddbAF8DD61b627727e03e190E32feddBD1319'
             )
         else :
-            return SmartBchContractInfoResponse(
+            return SmartBchDepositAddressResponse(
         )
 
-    def testSmartBchContractInfoResponse(self):
-        """Test SmartBchContractInfoResponse"""
+    def testSmartBchDepositAddressResponse(self):
+        """Test SmartBchDepositAddressResponse"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_contract_request.py` & `mainnet-1.1.1/test/test_smart_bch_contract_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_contract_response.py` & `mainnet-1.1.1/test/test_smart_bch_contract_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_deposit_address_response.py` & `mainnet-1.1.1/test/test_watch_address_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import mainnet
-from mainnet.models.smart_bch_deposit_address_response import SmartBchDepositAddressResponse  # noqa: E501
+from mainnet.models.watch_address_response import WatchAddressResponse  # noqa: E501
 from mainnet.rest import ApiException
 
-class TestSmartBchDepositAddressResponse(unittest.TestCase):
-    """SmartBchDepositAddressResponse unit test stubs"""
+class TestWatchAddressResponse(unittest.TestCase):
+    """WatchAddressResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SmartBchDepositAddressResponse
+        """Test WatchAddressResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = mainnet.models.smart_bch_deposit_address_response.SmartBchDepositAddressResponse()  # noqa: E501
+        # model = mainnet.models.watch_address_response.WatchAddressResponse()  # noqa: E501
         if include_optional :
-            return SmartBchDepositAddressResponse(
-                address = '0xE25ddbAF8DD61b627727e03e190E32feddBD1319'
+            return WatchAddressResponse(
+                id = 1
             )
         else :
-            return SmartBchDepositAddressResponse(
+            return WatchAddressResponse(
         )
 
-    def testSmartBchDepositAddressResponse(self):
-        """Test SmartBchDepositAddressResponse"""
+    def testWatchAddressResponse(self):
+        """Test WatchAddressResponse"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_max_amount_to_send_request.py` & `mainnet-1.1.1/test/test_smart_bch_max_amount_to_send_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_overrides.py` & `mainnet-1.1.1/test/test_smart_bch_overrides.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_send_max_request.py` & `mainnet-1.1.1/test/test_smart_bch_send_max_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_send_request.py` & `mainnet-1.1.1/test/test_smart_bch_send_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_send_request_item.py` & `mainnet-1.1.1/test/test_smart_bch_send_request_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_send_request_item_any_of.py` & `mainnet-1.1.1/test/test_smart_bch_send_request_item_any_of.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_send_request_options.py` & `mainnet-1.1.1/test/test_smart_bch_send_request_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_send_response_item.py` & `mainnet-1.1.1/test/test_smart_bch_send_response_item.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_sep20_all_balances_request.py` & `mainnet-1.1.1/test/test_smart_bch_sep20_all_balances_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_sep20_balance_request.py` & `mainnet-1.1.1/test/test_smart_bch_sep20_balance_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_sep20_balance_response.py` & `mainnet-1.1.1/test/test_smart_bch_sep20_balance_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_sep20_genesis_request.py` & `mainnet-1.1.1/test/test_smart_bch_sep20_genesis_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_sep20_genesis_response.py` & `mainnet-1.1.1/test/test_smart_bch_sep20_genesis_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_sep20_mint_request.py` & `mainnet-1.1.1/test/test_smart_bch_sep20_mint_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_sep20_mint_response.py` & `mainnet-1.1.1/test/test_smart_bch_sep20_mint_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_sep20_send_max_request.py` & `mainnet-1.1.1/test/test_smart_bch_sep20_send_max_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_sep20_send_request.py` & `mainnet-1.1.1/test/test_smart_bch_sep20_send_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_sep20_send_request_item.py` & `mainnet-1.1.1/test/test_smart_bch_sep20_send_request_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_sep20_token_info_request.py` & `mainnet-1.1.1/test/test_smart_bch_sep20_token_info_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_sep20_token_info_response.py` & `mainnet-1.1.1/test/test_smart_bch_sep20_token_info_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smart_bch_transaction_receipt.py` & `mainnet-1.1.1/test/test_smart_bch_transaction_receipt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smartbch_contract_api.py` & `mainnet-1.1.1/test/test_smartbch_contract_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smartbch_sep20_api.py` & `mainnet-1.1.1/test/test_smartbch_sep20_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_smartbch_wallet_api.py` & `mainnet-1.1.1/test/test_smartbch_wallet_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_submit_transaction_request.py` & `mainnet-1.1.1/test/test_submit_transaction_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_submit_transaction_response.py` & `mainnet-1.1.1/test/test_submit_transaction_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_token_burn_request.py` & `mainnet-1.1.1/test/test_wif.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,53 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import mainnet
-from mainnet.models.token_burn_request import TokenBurnRequest  # noqa: E501
+from mainnet.models.wif import Wif  # noqa: E501
 from mainnet.rest import ApiException
 
-class TestTokenBurnRequest(unittest.TestCase):
-    """TokenBurnRequest unit test stubs"""
+class TestWif(unittest.TestCase):
+    """Wif unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test TokenBurnRequest
+        """Test Wif
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = mainnet.models.token_burn_request.TokenBurnRequest()  # noqa: E501
+        # model = mainnet.models.wif.Wif()  # noqa: E501
         if include_optional :
-            return TokenBurnRequest(
-                wallet_id = '0', 
-                token_id = '0', 
-                capability = 'none', 
-                commitment = '0', 
-                amount = 1.337, 
-                cashaddr = '0', 
-                message = '0'
+            return Wif(
+                wif = 'cNfsPtqN2bMRS7vH5qd8tR8GMvgXyL5BjnGAKgZ8DYEiCrCCQcP6'
             )
         else :
-            return TokenBurnRequest(
-                wallet_id = '0',
-                token_id = '0',
+            return Wif(
         )
 
-    def testTokenBurnRequest(self):
-        """Test TokenBurnRequest"""
+    def testWif(self):
+        """Test Wif"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mainnet-1.1.0/test/test_token_genesis_request.py` & `mainnet-1.1.1/test/test_token_genesis_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_token_mint_request.py` & `mainnet-1.1.1/test/test_token_mint_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_token_mint_request_requests.py` & `mainnet-1.1.1/test/test_token_mint_request_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_token_send_request.py` & `mainnet-1.1.1/test/test_token_send_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_transaction_history_item.py` & `mainnet-1.1.1/test/test_transaction_history_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_unit_type.py` & `mainnet-1.1.1/test/test_unit_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_util_api.py` & `mainnet-1.1.1/test/test_util_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_util_decode_transaction_request.py` & `mainnet-1.1.1/test/test_util_decode_transaction_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_utxo.py` & `mainnet-1.1.1/test/test_utxo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -33,24 +33,28 @@
         """Test Utxo
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = mainnet.models.utxo.Utxo()  # noqa: E501
         if include_optional :
             return Utxo(
-                index = 1.337, 
-                tx_id = '1e6442a0d3548bb4f917721184ac1cb163ddf324e2c09f55c46ff0ba521cb89f', 
-                value = 100, 
-                utxo_id = '1e6442a0d3548bb4f917721184ac1cb163ddf324e2c09f55c46ff0ba521cb89f:0:21005'
+                vout = 1.337, 
+                txid = '1e6442a0d3548bb4f917721184ac1cb163ddf324e2c09f55c46ff0ba521cb89f', 
+                satoshis = 100, 
+                token = mainnet.models.utxo_token.Utxo_token(
+                    amount = 1.337, 
+                    token_id = '0', 
+                    capability = 'none', 
+                    commitment = '0', )
             )
         else :
             return Utxo(
-                tx_id = '1e6442a0d3548bb4f917721184ac1cb163ddf324e2c09f55c46ff0ba521cb89f',
-                value = 100,
-                utxo_id = '1e6442a0d3548bb4f917721184ac1cb163ddf324e2c09f55c46ff0ba521cb89f:0:21005',
+                vout = 1.337,
+                txid = '1e6442a0d3548bb4f917721184ac1cb163ddf324e2c09f55c46ff0ba521cb89f',
+                satoshis = 100,
         )
 
     def testUtxo(self):
         """Test Utxo"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `mainnet-1.1.0/test/test_utxo_response.py` & `mainnet-1.1.1/test/test_utxo_token.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,56 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import mainnet
-from mainnet.models.utxo_response import UtxoResponse  # noqa: E501
+from mainnet.models.utxo_token import UtxoToken  # noqa: E501
 from mainnet.rest import ApiException
 
-class TestUtxoResponse(unittest.TestCase):
-    """UtxoResponse unit test stubs"""
+class TestUtxoToken(unittest.TestCase):
+    """UtxoToken unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test UtxoResponse
+        """Test UtxoToken
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = mainnet.models.utxo_response.UtxoResponse()  # noqa: E501
+        # model = mainnet.models.utxo_token.UtxoToken()  # noqa: E501
         if include_optional :
-            return UtxoResponse(
-                utxos = [
-                    mainnet.models.utxo.Utxo(
-                        index = 1.337, 
-                        tx_id = '1e6442a0d3548bb4f917721184ac1cb163ddf324e2c09f55c46ff0ba521cb89f', 
-                        value = 100, 
-                        utxo_id = '1e6442a0d3548bb4f917721184ac1cb163ddf324e2c09f55c46ff0ba521cb89f:0:21005', )
-                    ]
+            return UtxoToken(
+                amount = 1.337, 
+                token_id = '0', 
+                capability = 'none', 
+                commitment = '0'
             )
         else :
-            return UtxoResponse(
+            return UtxoToken(
         )
 
-    def testUtxoResponse(self):
-        """Test UtxoResponse"""
+    def testUtxoToken(self):
+        """Test UtxoToken"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mainnet-1.1.0/test/test_verify_signed_message_request.py` & `mainnet-1.1.1/test/test_verify_signed_message_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_verify_signed_message_response.py` & `mainnet-1.1.1/test/test_verify_signed_message_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_verify_signed_message_response_details.py` & `mainnet-1.1.1/test/test_verify_signed_message_response_details.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_wallet_api.py` & `mainnet-1.1.1/test/test_wallet_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_wallet_bcmr_api.py` & `mainnet-1.1.1/test/test_wallet_bcmr_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_wallet_info.py` & `mainnet-1.1.1/test/test_wallet_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_wallet_mnemonic.py` & `mainnet-1.1.1/test/test_wallet_mnemonic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_wallet_named_exists_request.py` & `mainnet-1.1.1/test/test_wallet_named_exists_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_wallet_replace_named_request.py` & `mainnet-1.1.1/test/test_wallet_replace_named_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_wallet_request.py` & `mainnet-1.1.1/test/test_wallet_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_wallet_response.py` & `mainnet-1.1.1/test/test_wallet_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_wallet_signed_api.py` & `mainnet-1.1.1/test/test_wallet_signed_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_wallet_slp_api.py` & `mainnet-1.1.1/test/test_wallet_slp_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_wallet_type.py` & `mainnet-1.1.1/test/test_wallet_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_wallet_util_api.py` & `mainnet-1.1.1/test/test_wallet_util_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_watch_address_request.py` & `mainnet-1.1.1/test/test_watch_address_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_webhook_api.py` & `mainnet-1.1.1/test/test_webhook_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_wif.py` & `mainnet-1.1.1/test/test_x_pub_key_request.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import mainnet
-from mainnet.models.wif import Wif  # noqa: E501
+from mainnet.models.x_pub_key_request import XPubKeyRequest  # noqa: E501
 from mainnet.rest import ApiException
 
-class TestWif(unittest.TestCase):
-    """Wif unit test stubs"""
+class TestXPubKeyRequest(unittest.TestCase):
+    """XPubKeyRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test Wif
+        """Test XPubKeyRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = mainnet.models.wif.Wif()  # noqa: E501
+        # model = mainnet.models.x_pub_key_request.XPubKeyRequest()  # noqa: E501
         if include_optional :
-            return Wif(
-                wif = 'cNfsPtqN2bMRS7vH5qd8tR8GMvgXyL5BjnGAKgZ8DYEiCrCCQcP6'
+            return XPubKeyRequest(
+                wallet_id = 'seed:testnet:anchor stone process they donkey foam danger boat palace kind west cute:m/44'/0'/0'/0/0', 
+                paths = [
+                    'm/44'/0'/0''
+                    ]
             )
         else :
-            return Wif(
+            return XPubKeyRequest(
+                wallet_id = 'seed:testnet:anchor stone process they donkey foam danger boat palace kind west cute:m/44'/0'/0'/0/0',
         )
 
-    def testWif(self):
-        """Test Wif"""
+    def testXPubKeyRequest(self):
+        """Test XPubKeyRequest"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mainnet-1.1.0/test/test_x_pub_key.py` & `mainnet-1.1.1/test/test_x_pub_key.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_x_pub_key_response.py` & `mainnet-1.1.1/test/test_x_pub_key_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `mainnet-1.1.0/test/test_zero_balance_response.py` & `mainnet-1.1.1/test/test_zero_balance_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mainnet Cash
 
     A developer friendly bitcoin cash wallet api  This API is currently in *active* development, breaking changes may be made prior to official release of version 1.0.0.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.18
+    The version of the OpenAPI document: 1.1.0
     Contact: hello@mainnet.cash
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

