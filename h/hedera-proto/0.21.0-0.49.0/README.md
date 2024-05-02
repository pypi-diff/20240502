# Comparing `tmp/hedera-proto-0.21.0.tar.gz` & `tmp/hedera_proto-0.49.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hedera-proto-0.21.0.tar", last modified: Sat Dec 11 21:54:14 2021, max compression
+gzip compressed data, was "hedera_proto-0.49.0.tar", last modified: Thu May  2 06:57:57 2024, max compression
```

## Comparing `hedera-proto-0.21.0.tar` & `hedera_proto-0.49.0.tar`

### file list

```diff
@@ -1,120 +1,139 @@
-drwxrwxr-x   0 wensheng  (1000) wensheng  (1000)        0 2021-12-11 21:54:14.286856 hedera-proto-0.21.0/
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    11357 2021-10-29 23:12:03.000000 hedera-proto-0.21.0/LICENSE
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)       33 2021-10-29 23:12:15.000000 hedera-proto-0.21.0/MANIFEST.in
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1334 2021-12-11 21:54:14.286856 hedera-proto-0.21.0/PKG-INFO
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)      767 2021-10-30 00:37:02.000000 hedera-proto-0.21.0/README.md
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)      104 2021-10-29 23:12:15.000000 hedera-proto-0.21.0/pyproject.toml
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)       38 2021-12-11 21:54:14.286856 hedera-proto-0.21.0/setup.cfg
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1206 2021-12-11 21:53:59.000000 hedera-proto-0.21.0/setup.py
-drwxrwxr-x   0 wensheng  (1000) wensheng  (1000)        0 2021-12-11 21:54:14.270856 hedera-proto-0.21.0/src/
-drwxrwxr-x   0 wensheng  (1000) wensheng  (1000)        0 2021-12-11 21:54:14.286856 hedera-proto-0.21.0/src/hedera_proto/
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     7319 2021-12-11 21:47:30.000000 hedera-proto-0.21.0/src/hedera_proto/__init__.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     7616 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/account_balance_file_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)   118558 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/basic_types_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     5134 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/consensus_create_topic_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2711 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/consensus_delete_topic_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     6347 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/consensus_get_topic_info_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3856 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/consensus_service_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    18461 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/consensus_service_pb2_grpc.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     6333 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/consensus_submit_message_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     6404 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/consensus_topic_info_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     6761 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/consensus_update_topic_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    14288 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/contract_call_local_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3991 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/contract_call_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     8191 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/contract_create_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     4720 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/contract_delete_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     5407 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/contract_get_bytecode_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    12755 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/contract_get_info_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     6359 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/contract_get_records_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     8056 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/contract_update_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     5549 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/crypto_add_live_hash_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     8809 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/crypto_create_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3263 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/crypto_delete_live_hash_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3238 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/crypto_delete_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     8259 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/crypto_get_account_balance_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     6403 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/crypto_get_account_records_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    16628 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/crypto_get_info_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     6049 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/crypto_get_live_hash_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     9142 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/crypto_get_stakers_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     7463 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/crypto_service_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    23108 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/crypto_service_pb2_grpc.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3255 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/crypto_transfer_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    14218 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/crypto_update_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    14534 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/custom_fees_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2085 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/duration_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     5244 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/exchange_rate_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3005 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/file_append_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     5912 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/file_create_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2538 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/file_delete_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     7490 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/file_get_contents_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     9405 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/file_get_info_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     4985 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/file_service_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    13343 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/file_service_pb2_grpc.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     5037 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/file_update_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     6551 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/freeze_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1978 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/freeze_service_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2602 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/freeze_service_pb2_grpc.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2903 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/freeze_type_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     9131 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/get_by_key_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     6435 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/get_by_solidity_id_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     5581 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/network_get_execution_time_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     5709 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/network_get_version_info_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2945 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/network_service_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     6278 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/network_service_pb2_grpc.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    11982 2021-12-11 21:47:30.000000 hedera-proto-0.21.0/src/hedera_proto/pom.xml
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     4449 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/query_header_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    24650 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/query_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    69350 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/response_code_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     4217 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/response_header_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    25536 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/response_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    38184 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/schedulable_transaction_body_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     4564 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/schedule_create_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2618 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/schedule_delete_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    13379 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/schedule_get_info_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3439 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/schedule_service_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    12177 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/schedule_service_pb2_grpc.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2584 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/schedule_sign_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     6508 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/smart_contract_service_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    18531 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/smart_contract_service_pb2_grpc.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     4605 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/system_delete_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3945 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/system_undelete_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     6672 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/throttle_definitions_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3798 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/timestamp_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3194 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/token_associate_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3440 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/token_burn_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    13755 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/token_create_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2546 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/token_delete_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3213 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/token_dissociate_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3467 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/token_fee_schedule_update_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3269 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/token_freeze_account_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     6689 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/token_get_account_nft_infos_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    19505 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/token_get_info_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    10003 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/token_get_nft_info_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     6996 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/token_get_nft_infos_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3177 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/token_grant_kyc_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3428 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/token_mint_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2529 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/token_pause_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3196 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/token_revoke_kyc_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     9862 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/token_service_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    31143 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/token_service_pb2_grpc.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3307 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/token_unfreeze_account_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2563 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/token_unpause_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    10875 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/token_update_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     4183 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/token_wipe_account_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    44323 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/transaction_body_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2926 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/transaction_contents_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     5895 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/transaction_get_fast_record_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     8150 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/transaction_get_receipt_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     8128 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/transaction_get_record_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2457 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/transaction_list_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     4913 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/transaction_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     9747 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/transaction_receipt_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    11833 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/transaction_record_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3033 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/transaction_response_pb2.py
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2270 2021-12-11 21:46:10.000000 hedera-proto-0.21.0/src/hedera_proto/unchecked_submit_pb2.py
-drwxrwxr-x   0 wensheng  (1000) wensheng  (1000)        0 2021-12-11 21:54:14.286856 hedera-proto-0.21.0/src/hedera_proto.egg-info/
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1334 2021-12-11 21:54:14.000000 hedera-proto-0.21.0/src/hedera_proto.egg-info/PKG-INFO
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     4556 2021-12-11 21:54:14.000000 hedera-proto-0.21.0/src/hedera_proto.egg-info/SOURCES.txt
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)        1 2021-12-11 21:54:14.000000 hedera-proto-0.21.0/src/hedera_proto.egg-info/dependency_links.txt
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)       32 2021-12-11 21:54:14.000000 hedera-proto-0.21.0/src/hedera_proto.egg-info/requires.txt
--rw-rw-r--   0 wensheng  (1000) wensheng  (1000)       13 2021-12-11 21:54:14.000000 hedera-proto-0.21.0/src/hedera_proto.egg-info/top_level.txt
+drwxrwxr-x   0 wensheng  (1000) wensheng  (1000)        0 2024-05-02 06:57:57.594838 hedera_proto-0.49.0/
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    11357 2024-05-02 04:34:39.000000 hedera_proto-0.49.0/LICENSE
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)       33 2024-05-02 04:34:39.000000 hedera_proto-0.49.0/MANIFEST.in
+-rw-r--r--   0 wensheng  (1000) wensheng  (1000)     1311 2024-05-02 06:57:57.594838 hedera_proto-0.49.0/PKG-INFO
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)      767 2024-05-02 04:34:39.000000 hedera_proto-0.49.0/README.md
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)       87 2024-05-02 06:56:00.000000 hedera_proto-0.49.0/pyproject.toml
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)       38 2024-05-02 06:57:57.594838 hedera_proto-0.49.0/setup.cfg
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1151 2024-05-02 06:55:52.000000 hedera_proto-0.49.0/setup.py
+drwxrwxr-x   0 wensheng  (1000) wensheng  (1000)        0 2024-05-02 06:57:57.586838 hedera_proto-0.49.0/src/
+drwxrwxr-x   0 wensheng  (1000) wensheng  (1000)        0 2024-05-02 06:57:57.594838 hedera_proto-0.49.0/src/hedera_proto/
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1059 2024-05-02 05:20:17.000000 hedera_proto-0.49.0/src/hedera_proto/__init__.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2080 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/account_balance_file_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    18664 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/basic_types_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1702 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/consensus_create_topic_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1401 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/consensus_delete_topic_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2076 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/consensus_get_topic_info_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1875 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/consensus_service_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    20281 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/consensus_service_pb2_grpc.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1849 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/consensus_submit_message_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1912 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/consensus_topic_info_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2049 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/consensus_update_topic_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3021 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/contract_action_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1427 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/contract_bytecode_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     4013 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/contract_call_local_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1489 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/contract_call_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2621 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/contract_create_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1598 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/contract_delete_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1865 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/contract_get_bytecode_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3290 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/contract_get_info_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2342 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/contract_get_records_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2057 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/contract_state_change_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1494 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/contract_types_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3130 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/contract_update_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1771 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/crypto_add_live_hash_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2867 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/crypto_approve_allowance_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2959 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/crypto_create_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1728 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/crypto_delete_allowance_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1473 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/crypto_delete_live_hash_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1439 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/crypto_delete_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2365 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/crypto_get_account_balance_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2075 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/crypto_get_account_records_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     4405 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/crypto_get_info_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1999 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/crypto_get_live_hash_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2331 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/crypto_get_stakers_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2755 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/crypto_service_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    30099 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/crypto_service_pb2_grpc.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1448 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/crypto_transfer_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     4536 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/crypto_update_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2882 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/custom_fees_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1192 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/duration_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1454 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/ethereum_transaction_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1657 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/exchange_rate_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1389 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/file_append_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1740 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/file_create_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1343 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/file_delete_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2160 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/file_get_contents_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2401 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/file_get_info_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2062 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/file_service_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    15665 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/file_service_pb2_grpc.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1772 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/file_update_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2587 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/freeze_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1415 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/freeze_service_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3743 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/freeze_service_pb2_grpc.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1396 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/freeze_type_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     4637 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/get_account_details_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2266 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/get_by_key_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1941 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/get_by_solidity_id_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1483 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/hash_object_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1704 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/mirror_network_service_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     4063 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/mirror_network_service_pb2_grpc.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1909 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/network_get_execution_time_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1937 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/network_get_version_info_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1758 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/network_service_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     9521 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/network_service_pb2_grpc.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2849 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/node_stake_update_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    12147 2024-05-02 05:20:17.000000 hedera_proto-0.49.0/src/hedera_proto/pom.xml
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1645 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/query_header_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     5884 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/query_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2775 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/record_stream_file_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    17654 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/response_code_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1572 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/response_header_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     6002 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/response_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     8171 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/schedulable_transaction_body_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1866 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/schedule_create_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1363 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/schedule_delete_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3001 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/schedule_get_info_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1794 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/schedule_service_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    18132 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/schedule_service_pb2_grpc.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1351 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/schedule_sign_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2199 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/sidecar_file_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2053 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/signature_file_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2729 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/smart_contract_service_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    23111 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/smart_contract_service_pb2_grpc.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1581 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/system_delete_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1450 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/system_undelete_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1869 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/throttle_definitions_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1391 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/timestamp_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1430 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_associate_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1417 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_burn_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2720 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_create_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1342 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_delete_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1436 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_dissociate_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1550 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_fee_schedule_update_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1453 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_freeze_account_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2079 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_get_account_nft_infos_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3706 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_get_info_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2344 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_get_nft_info_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2078 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_get_nft_infos_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1426 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_grant_kyc_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1414 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_mint_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1336 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_pause_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1432 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_revoke_kyc_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3543 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_service_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)    37074 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_service_pb2_grpc.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1465 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_unfreeze_account_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1348 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_unpause_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1739 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_update_nfts_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2528 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_update_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1538 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/token_wipe_account_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     9978 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/transaction_body_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1381 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/transaction_contents_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2029 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/transaction_get_fast_record_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2297 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/transaction_get_receipt_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2292 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/transaction_get_record_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1326 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/transaction_list_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2309 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/transaction_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     2269 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/transaction_receipt_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3025 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/transaction_record_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1415 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/transaction_response_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1249 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/unchecked_submit_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1227 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/util_prng_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     1397 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/util_service_pb2.py
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     3680 2024-05-02 05:19:37.000000 hedera_proto-0.49.0/src/hedera_proto/util_service_pb2_grpc.py
+drwxrwxr-x   0 wensheng  (1000) wensheng  (1000)        0 2024-05-02 06:57:57.594838 hedera_proto-0.49.0/src/hedera_proto.egg-info/
+-rw-r--r--   0 wensheng  (1000) wensheng  (1000)     1311 2024-05-02 06:57:57.000000 hedera_proto-0.49.0/src/hedera_proto.egg-info/PKG-INFO
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)     5360 2024-05-02 06:57:57.000000 hedera_proto-0.49.0/src/hedera_proto.egg-info/SOURCES.txt
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)        1 2024-05-02 06:57:57.000000 hedera_proto-0.49.0/src/hedera_proto.egg-info/dependency_links.txt
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)       15 2024-05-02 06:57:57.000000 hedera_proto-0.49.0/src/hedera_proto.egg-info/requires.txt
+-rw-rw-r--   0 wensheng  (1000) wensheng  (1000)       13 2024-05-02 06:57:57.000000 hedera_proto-0.49.0/src/hedera_proto.egg-info/top_level.txt
```

### Comparing `hedera-proto-0.21.0/LICENSE` & `hedera_proto-0.49.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hedera-proto-0.21.0/PKG-INFO` & `hedera_proto-0.49.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: hedera-proto
-Version: 0.21.0
+Version: 0.49.0
 Summary: Hedera Protobufs
-Home-page: https://github.com/carady/hedera-protobufs-python
+Home-page: https://github.com/carady/hedera-proto-py
 Author: Wensheng Wang
 Author-email: wenshengwang@gmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/carady/hedera-protobufs-python/issues
-Platform: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/carady/hedera-proto-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: grpcio>=1.34.1
 
 # hedera-protobufs-python
 
 Hedera API Definitions in Protocol Buffer compiled to Python
 
 They are compiled from .proto files in [Java Protobufs](https://github.com/hashgraph/hedera-protobufs-java).
 
@@ -38,9 +37,7 @@
     accountId = proto.AccountID()
 
 ## Note
 
 This is used by pure Python Hedera SDK, which, as of now (2021/11), has not been released yet.
 
 You are encouraged to use the fully functional Python SDK [github.com/wensheng/hedera-sdk-py](https://github.com/wensheng/hedera-sdk-py), which is a Python wrapper around Java SDK, while waiting for pure Python SDK.
-
-
```

### Comparing `hedera-proto-0.21.0/README.md` & `hedera_proto-0.49.0/README.md`

 * *Files identical despite different names*

### Comparing `hedera-proto-0.21.0/setup.py` & `hedera_proto-0.49.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import os
 import setuptools
 import xml.etree.ElementTree as ET
 
 pom = ET.parse("./src/hedera_proto/pom.xml")
-version = [a.text for a in pom.getroot().getchildren() if a.tag == '{http://maven.apache.org/POM/4.0.0}version'][0]
-version = version.split("-")[0]
+version_element = pom.getroot().find('{http://maven.apache.org/POM/4.0.0}version')
+version = version_element.text.split('-')[0]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hedera-proto",
     version=version,
     author="Wensheng Wang",
     author_email="wenshengwang@gmail.com",
     description="Hedera Protobufs",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/carady/hedera-protobufs-python",
+    url="https://github.com/carady/hedera-proto-py",
     project_urls={
-        "Bug Tracker": "https://github.com/carady/hedera-protobufs-python/issues",
+        "Bug Tracker": "https://github.com/carady/hedera-proto-py/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    install_requires=['grpcio>=1.41.1','protobuf>=3.19.1'],
-    python_requires=">=3.7",
+    install_requires=['grpcio>=1.34.1'],
+    python_requires=">=3.6",
     include_package_data=True,
     package_data={ "hedera_proto": ["*.xml"]},
 )
```

### Comparing `hedera-proto-0.21.0/src/hedera_proto/consensus_service_pb2_grpc.py` & `hedera_proto-0.49.0/src/hedera_proto/consensus_service_pb2_grpc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,41 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
+import warnings
 
 import query_pb2 as query__pb2
 import response_pb2 as response__pb2
 import transaction_pb2 as transaction__pb2
 import transaction_response_pb2 as transaction__response__pb2
 
+GRPC_GENERATED_VERSION = '1.63.0'
+GRPC_VERSION = grpc.__version__
+EXPECTED_ERROR_RELEASE = '1.65.0'
+SCHEDULED_RELEASE_DATE = 'June 25, 2024'
+_version_not_supported = False
+
+try:
+    from grpc._utilities import first_version_is_lower
+    _version_not_supported = first_version_is_lower(GRPC_VERSION, GRPC_GENERATED_VERSION)
+except ImportError:
+    _version_not_supported = True
+
+if _version_not_supported:
+    warnings.warn(
+        f'The grpc package installed is at version {GRPC_VERSION},'
+        + f' but the generated code in consensus_service_pb2_grpc.py depends on'
+        + f' grpcio>={GRPC_GENERATED_VERSION}.'
+        + f' Please upgrade your grpc module to grpcio>={GRPC_GENERATED_VERSION}'
+        + f' or downgrade your generated code using grpcio-tools<={GRPC_VERSION}.'
+        + f' This warning will become an error in {EXPECTED_ERROR_RELEASE},'
+        + f' scheduled for release on {SCHEDULED_RELEASE_DATE}.',
+        RuntimeWarning
+    )
+
 
 class ConsensusServiceStub(object):
     """*
     The Consensus Service provides the ability for Hedera Hashgraph to provide aBFT consensus as to
     the order and validity of messages submitted to a *topic*, as well as a *consensus timestamp* for
     those messages.
 
@@ -60,35 +85,35 @@
         Args:
             channel: A grpc.Channel.
         """
         self.createTopic = channel.unary_unary(
                 '/proto.ConsensusService/createTopic',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.updateTopic = channel.unary_unary(
                 '/proto.ConsensusService/updateTopic',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.deleteTopic = channel.unary_unary(
                 '/proto.ConsensusService/deleteTopic',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.getTopicInfo = channel.unary_unary(
                 '/proto.ConsensusService/getTopicInfo',
                 request_serializer=query__pb2.Query.SerializeToString,
                 response_deserializer=response__pb2.Response.FromString,
-                )
+                _registered_method=True)
         self.submitMessage = channel.unary_unary(
                 '/proto.ConsensusService/submitMessage',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
 
 
 class ConsensusServiceServicer(object):
     """*
     The Consensus Service provides the ability for Hedera Hashgraph to provide aBFT consensus as to
     the order and validity of messages submitted to a *topic*, as well as a *consensus timestamp* for
     those messages.
@@ -282,80 +307,130 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.ConsensusService/createTopic',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.ConsensusService/createTopic',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def updateTopic(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.ConsensusService/updateTopic',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.ConsensusService/updateTopic',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def deleteTopic(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.ConsensusService/deleteTopic',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.ConsensusService/deleteTopic',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def getTopicInfo(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.ConsensusService/getTopicInfo',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.ConsensusService/getTopicInfo',
             query__pb2.Query.SerializeToString,
             response__pb2.Response.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def submitMessage(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.ConsensusService/submitMessage',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.ConsensusService/submitMessage',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
```

### Comparing `hedera-proto-0.21.0/src/hedera_proto/crypto_service_pb2_grpc.py` & `hedera_proto-0.49.0/src/hedera_proto/smart_contract_service_pb2_grpc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,536 +1,608 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
+import warnings
 
 import query_pb2 as query__pb2
 import response_pb2 as response__pb2
 import transaction_pb2 as transaction__pb2
 import transaction_response_pb2 as transaction__response__pb2
 
+GRPC_GENERATED_VERSION = '1.63.0'
+GRPC_VERSION = grpc.__version__
+EXPECTED_ERROR_RELEASE = '1.65.0'
+SCHEDULED_RELEASE_DATE = 'June 25, 2024'
+_version_not_supported = False
+
+try:
+    from grpc._utilities import first_version_is_lower
+    _version_not_supported = first_version_is_lower(GRPC_VERSION, GRPC_GENERATED_VERSION)
+except ImportError:
+    _version_not_supported = True
+
+if _version_not_supported:
+    warnings.warn(
+        f'The grpc package installed is at version {GRPC_VERSION},'
+        + f' but the generated code in smart_contract_service_pb2_grpc.py depends on'
+        + f' grpcio>={GRPC_GENERATED_VERSION}.'
+        + f' Please upgrade your grpc module to grpcio>={GRPC_GENERATED_VERSION}'
+        + f' or downgrade your generated code using grpcio-tools<={GRPC_VERSION}.'
+        + f' This warning will become an error in {EXPECTED_ERROR_RELEASE},'
+        + f' scheduled for release on {SCHEDULED_RELEASE_DATE}.',
+        RuntimeWarning
+    )
 
-class CryptoServiceStub(object):
+
+class SmartContractServiceStub(object):
     """*
-    Transactions and queries for the Crypto Service
+    Transactions and queries for the file service. 
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.createAccount = channel.unary_unary(
-                '/proto.CryptoService/createAccount',
-                request_serializer=transaction__pb2.Transaction.SerializeToString,
-                response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
-        self.updateAccount = channel.unary_unary(
-                '/proto.CryptoService/updateAccount',
-                request_serializer=transaction__pb2.Transaction.SerializeToString,
-                response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
-        self.cryptoTransfer = channel.unary_unary(
-                '/proto.CryptoService/cryptoTransfer',
-                request_serializer=transaction__pb2.Transaction.SerializeToString,
-                response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
-        self.cryptoDelete = channel.unary_unary(
-                '/proto.CryptoService/cryptoDelete',
+        self.createContract = channel.unary_unary(
+                '/proto.SmartContractService/createContract',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
-        self.addLiveHash = channel.unary_unary(
-                '/proto.CryptoService/addLiveHash',
+                _registered_method=True)
+        self.updateContract = channel.unary_unary(
+                '/proto.SmartContractService/updateContract',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
-        self.deleteLiveHash = channel.unary_unary(
-                '/proto.CryptoService/deleteLiveHash',
+                _registered_method=True)
+        self.contractCallMethod = channel.unary_unary(
+                '/proto.SmartContractService/contractCallMethod',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
-        self.getLiveHash = channel.unary_unary(
-                '/proto.CryptoService/getLiveHash',
+                _registered_method=True)
+        self.getContractInfo = channel.unary_unary(
+                '/proto.SmartContractService/getContractInfo',
                 request_serializer=query__pb2.Query.SerializeToString,
                 response_deserializer=response__pb2.Response.FromString,
-                )
-        self.getAccountRecords = channel.unary_unary(
-                '/proto.CryptoService/getAccountRecords',
+                _registered_method=True)
+        self.contractCallLocalMethod = channel.unary_unary(
+                '/proto.SmartContractService/contractCallLocalMethod',
                 request_serializer=query__pb2.Query.SerializeToString,
                 response_deserializer=response__pb2.Response.FromString,
-                )
-        self.cryptoGetBalance = channel.unary_unary(
-                '/proto.CryptoService/cryptoGetBalance',
+                _registered_method=True)
+        self.ContractGetBytecode = channel.unary_unary(
+                '/proto.SmartContractService/ContractGetBytecode',
                 request_serializer=query__pb2.Query.SerializeToString,
                 response_deserializer=response__pb2.Response.FromString,
-                )
-        self.getAccountInfo = channel.unary_unary(
-                '/proto.CryptoService/getAccountInfo',
+                _registered_method=True)
+        self.getBySolidityID = channel.unary_unary(
+                '/proto.SmartContractService/getBySolidityID',
                 request_serializer=query__pb2.Query.SerializeToString,
                 response_deserializer=response__pb2.Response.FromString,
-                )
-        self.getTransactionReceipts = channel.unary_unary(
-                '/proto.CryptoService/getTransactionReceipts',
+                _registered_method=True)
+        self.getTxRecordByContractID = channel.unary_unary(
+                '/proto.SmartContractService/getTxRecordByContractID',
                 request_serializer=query__pb2.Query.SerializeToString,
                 response_deserializer=response__pb2.Response.FromString,
-                )
-        self.getFastTransactionRecord = channel.unary_unary(
-                '/proto.CryptoService/getFastTransactionRecord',
-                request_serializer=query__pb2.Query.SerializeToString,
-                response_deserializer=response__pb2.Response.FromString,
-                )
-        self.getTxRecordByTxID = channel.unary_unary(
-                '/proto.CryptoService/getTxRecordByTxID',
-                request_serializer=query__pb2.Query.SerializeToString,
-                response_deserializer=response__pb2.Response.FromString,
-                )
-        self.getStakersByAccountID = channel.unary_unary(
-                '/proto.CryptoService/getStakersByAccountID',
-                request_serializer=query__pb2.Query.SerializeToString,
-                response_deserializer=response__pb2.Response.FromString,
-                )
+                _registered_method=True)
+        self.deleteContract = channel.unary_unary(
+                '/proto.SmartContractService/deleteContract',
+                request_serializer=transaction__pb2.Transaction.SerializeToString,
+                response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
+                _registered_method=True)
+        self.systemDelete = channel.unary_unary(
+                '/proto.SmartContractService/systemDelete',
+                request_serializer=transaction__pb2.Transaction.SerializeToString,
+                response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
+                _registered_method=True)
+        self.systemUndelete = channel.unary_unary(
+                '/proto.SmartContractService/systemUndelete',
+                request_serializer=transaction__pb2.Transaction.SerializeToString,
+                response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
+                _registered_method=True)
+        self.callEthereum = channel.unary_unary(
+                '/proto.SmartContractService/callEthereum',
+                request_serializer=transaction__pb2.Transaction.SerializeToString,
+                response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
+                _registered_method=True)
 
 
-class CryptoServiceServicer(object):
+class SmartContractServiceServicer(object):
     """*
-    Transactions and queries for the Crypto Service
+    Transactions and queries for the file service. 
     """
 
-    def createAccount(self, request, context):
-        """*
-        Creates a new account by submitting the transaction
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def updateAccount(self, request, context):
-        """*
-        Updates an account by submitting the transaction
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def cryptoTransfer(self, request, context):
+    def createContract(self, request, context):
         """*
-        Initiates a transfer by submitting the transaction
+        Creates a contract
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def cryptoDelete(self, request, context):
+    def updateContract(self, request, context):
         """*
-        Deletes and account by submitting the transaction
+        Updates a contract with the content
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def addLiveHash(self, request, context):
+    def contractCallMethod(self, request, context):
         """*
-        (NOT CURRENTLY SUPPORTED) Adds a livehash
+        Calls a contract
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def deleteLiveHash(self, request, context):
+    def getContractInfo(self, request, context):
         """*
-        (NOT CURRENTLY SUPPORTED) Deletes a livehash
+        Retrieves the contract information
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def getLiveHash(self, request, context):
+    def contractCallLocalMethod(self, request, context):
         """*
-        (NOT CURRENTLY SUPPORTED) Retrieves a livehash for an account
+        Calls a smart contract to be run on a single node
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def getAccountRecords(self, request, context):
+    def ContractGetBytecode(self, request, context):
         """*
-        Returns all transactions in the last 180s of consensus time for which the given account was
-        the effective payer <b>and</b> network property <tt>ledger.keepRecordsInState</tt> was
-        <tt>true</tt>.
+        Retrieves the runtime code of a contract
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def cryptoGetBalance(self, request, context):
+    def getBySolidityID(self, request, context):
         """*
-        Retrieves the balance of an account
+        Retrieves a contract by its Solidity address
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def getAccountInfo(self, request, context):
+    def getTxRecordByContractID(self, request, context):
         """*
-        Retrieves the metadata of an account
+        Always returns an empty record list, as contract accounts are never effective payers for
+        transactions
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def getTransactionReceipts(self, request, context):
+    def deleteContract(self, request, context):
         """*
-        Retrieves the latest receipt for a transaction that is either awaiting consensus, or reached
-        consensus in the last 180 seconds
+        Deletes a contract instance and transfers any remaining hbars to a specified receiver
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def getFastTransactionRecord(self, request, context):
+    def systemDelete(self, request, context):
         """*
-        (NOT CURRENTLY SUPPORTED) Returns the records of transactions recently funded by an account
+        Deletes a contract if the submitting account has network admin privileges
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def getTxRecordByTxID(self, request, context):
+    def systemUndelete(self, request, context):
         """*
-        Retrieves the record of a transaction that is either awaiting consensus, or reached consensus
-        in the last 180 seconds
+        Undeletes a contract if the submitting account has network admin privileges
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def getStakersByAccountID(self, request, context):
+    def callEthereum(self, request, context):
         """*
-        (NOT CURRENTLY SUPPORTED) Retrieves the stakers for a node by account id
+        Ethereum transaction
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_CryptoServiceServicer_to_server(servicer, server):
+def add_SmartContractServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'createAccount': grpc.unary_unary_rpc_method_handler(
-                    servicer.createAccount,
-                    request_deserializer=transaction__pb2.Transaction.FromString,
-                    response_serializer=transaction__response__pb2.TransactionResponse.SerializeToString,
-            ),
-            'updateAccount': grpc.unary_unary_rpc_method_handler(
-                    servicer.updateAccount,
-                    request_deserializer=transaction__pb2.Transaction.FromString,
-                    response_serializer=transaction__response__pb2.TransactionResponse.SerializeToString,
-            ),
-            'cryptoTransfer': grpc.unary_unary_rpc_method_handler(
-                    servicer.cryptoTransfer,
-                    request_deserializer=transaction__pb2.Transaction.FromString,
-                    response_serializer=transaction__response__pb2.TransactionResponse.SerializeToString,
-            ),
-            'cryptoDelete': grpc.unary_unary_rpc_method_handler(
-                    servicer.cryptoDelete,
+            'createContract': grpc.unary_unary_rpc_method_handler(
+                    servicer.createContract,
                     request_deserializer=transaction__pb2.Transaction.FromString,
                     response_serializer=transaction__response__pb2.TransactionResponse.SerializeToString,
             ),
-            'addLiveHash': grpc.unary_unary_rpc_method_handler(
-                    servicer.addLiveHash,
+            'updateContract': grpc.unary_unary_rpc_method_handler(
+                    servicer.updateContract,
                     request_deserializer=transaction__pb2.Transaction.FromString,
                     response_serializer=transaction__response__pb2.TransactionResponse.SerializeToString,
             ),
-            'deleteLiveHash': grpc.unary_unary_rpc_method_handler(
-                    servicer.deleteLiveHash,
+            'contractCallMethod': grpc.unary_unary_rpc_method_handler(
+                    servicer.contractCallMethod,
                     request_deserializer=transaction__pb2.Transaction.FromString,
                     response_serializer=transaction__response__pb2.TransactionResponse.SerializeToString,
             ),
-            'getLiveHash': grpc.unary_unary_rpc_method_handler(
-                    servicer.getLiveHash,
+            'getContractInfo': grpc.unary_unary_rpc_method_handler(
+                    servicer.getContractInfo,
                     request_deserializer=query__pb2.Query.FromString,
                     response_serializer=response__pb2.Response.SerializeToString,
             ),
-            'getAccountRecords': grpc.unary_unary_rpc_method_handler(
-                    servicer.getAccountRecords,
+            'contractCallLocalMethod': grpc.unary_unary_rpc_method_handler(
+                    servicer.contractCallLocalMethod,
                     request_deserializer=query__pb2.Query.FromString,
                     response_serializer=response__pb2.Response.SerializeToString,
             ),
-            'cryptoGetBalance': grpc.unary_unary_rpc_method_handler(
-                    servicer.cryptoGetBalance,
+            'ContractGetBytecode': grpc.unary_unary_rpc_method_handler(
+                    servicer.ContractGetBytecode,
                     request_deserializer=query__pb2.Query.FromString,
                     response_serializer=response__pb2.Response.SerializeToString,
             ),
-            'getAccountInfo': grpc.unary_unary_rpc_method_handler(
-                    servicer.getAccountInfo,
+            'getBySolidityID': grpc.unary_unary_rpc_method_handler(
+                    servicer.getBySolidityID,
                     request_deserializer=query__pb2.Query.FromString,
                     response_serializer=response__pb2.Response.SerializeToString,
             ),
-            'getTransactionReceipts': grpc.unary_unary_rpc_method_handler(
-                    servicer.getTransactionReceipts,
+            'getTxRecordByContractID': grpc.unary_unary_rpc_method_handler(
+                    servicer.getTxRecordByContractID,
                     request_deserializer=query__pb2.Query.FromString,
                     response_serializer=response__pb2.Response.SerializeToString,
             ),
-            'getFastTransactionRecord': grpc.unary_unary_rpc_method_handler(
-                    servicer.getFastTransactionRecord,
-                    request_deserializer=query__pb2.Query.FromString,
-                    response_serializer=response__pb2.Response.SerializeToString,
+            'deleteContract': grpc.unary_unary_rpc_method_handler(
+                    servicer.deleteContract,
+                    request_deserializer=transaction__pb2.Transaction.FromString,
+                    response_serializer=transaction__response__pb2.TransactionResponse.SerializeToString,
             ),
-            'getTxRecordByTxID': grpc.unary_unary_rpc_method_handler(
-                    servicer.getTxRecordByTxID,
-                    request_deserializer=query__pb2.Query.FromString,
-                    response_serializer=response__pb2.Response.SerializeToString,
+            'systemDelete': grpc.unary_unary_rpc_method_handler(
+                    servicer.systemDelete,
+                    request_deserializer=transaction__pb2.Transaction.FromString,
+                    response_serializer=transaction__response__pb2.TransactionResponse.SerializeToString,
             ),
-            'getStakersByAccountID': grpc.unary_unary_rpc_method_handler(
-                    servicer.getStakersByAccountID,
-                    request_deserializer=query__pb2.Query.FromString,
-                    response_serializer=response__pb2.Response.SerializeToString,
+            'systemUndelete': grpc.unary_unary_rpc_method_handler(
+                    servicer.systemUndelete,
+                    request_deserializer=transaction__pb2.Transaction.FromString,
+                    response_serializer=transaction__response__pb2.TransactionResponse.SerializeToString,
+            ),
+            'callEthereum': grpc.unary_unary_rpc_method_handler(
+                    servicer.callEthereum,
+                    request_deserializer=transaction__pb2.Transaction.FromString,
+                    response_serializer=transaction__response__pb2.TransactionResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'proto.CryptoService', rpc_method_handlers)
+            'proto.SmartContractService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class CryptoService(object):
+class SmartContractService(object):
     """*
-    Transactions and queries for the Crypto Service
+    Transactions and queries for the file service. 
     """
 
     @staticmethod
-    def createAccount(request,
+    def createContract(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.CryptoService/createAccount',
-            transaction__pb2.Transaction.SerializeToString,
-            transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def updateAccount(request,
+        return grpc.experimental.unary_unary(
+            request,
             target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.CryptoService/updateAccount',
+            '/proto.SmartContractService/createContract',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
-    def cryptoTransfer(request,
+    def updateContract(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.CryptoService/cryptoTransfer',
-            transaction__pb2.Transaction.SerializeToString,
-            transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def cryptoDelete(request,
+        return grpc.experimental.unary_unary(
+            request,
             target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.CryptoService/cryptoDelete',
+            '/proto.SmartContractService/updateContract',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
-    def addLiveHash(request,
+    def contractCallMethod(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.CryptoService/addLiveHash',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.SmartContractService/contractCallMethod',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
-    def deleteLiveHash(request,
+    def getContractInfo(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.CryptoService/deleteLiveHash',
-            transaction__pb2.Transaction.SerializeToString,
-            transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.SmartContractService/getContractInfo',
+            query__pb2.Query.SerializeToString,
+            response__pb2.Response.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
-    def getLiveHash(request,
+    def contractCallLocalMethod(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.CryptoService/getLiveHash',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.SmartContractService/contractCallLocalMethod',
             query__pb2.Query.SerializeToString,
             response__pb2.Response.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
-    def getAccountRecords(request,
+    def ContractGetBytecode(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.CryptoService/getAccountRecords',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.SmartContractService/ContractGetBytecode',
             query__pb2.Query.SerializeToString,
             response__pb2.Response.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
-    def cryptoGetBalance(request,
+    def getBySolidityID(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.CryptoService/cryptoGetBalance',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.SmartContractService/getBySolidityID',
             query__pb2.Query.SerializeToString,
             response__pb2.Response.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
-    def getAccountInfo(request,
+    def getTxRecordByContractID(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.CryptoService/getAccountInfo',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.SmartContractService/getTxRecordByContractID',
             query__pb2.Query.SerializeToString,
             response__pb2.Response.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
-    def getTransactionReceipts(request,
+    def deleteContract(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.CryptoService/getTransactionReceipts',
-            query__pb2.Query.SerializeToString,
-            response__pb2.Response.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.SmartContractService/deleteContract',
+            transaction__pb2.Transaction.SerializeToString,
+            transaction__response__pb2.TransactionResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
-    def getFastTransactionRecord(request,
+    def systemDelete(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.CryptoService/getFastTransactionRecord',
-            query__pb2.Query.SerializeToString,
-            response__pb2.Response.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.SmartContractService/systemDelete',
+            transaction__pb2.Transaction.SerializeToString,
+            transaction__response__pb2.TransactionResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
-    def getTxRecordByTxID(request,
+    def systemUndelete(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.CryptoService/getTxRecordByTxID',
-            query__pb2.Query.SerializeToString,
-            response__pb2.Response.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.SmartContractService/systemUndelete',
+            transaction__pb2.Transaction.SerializeToString,
+            transaction__response__pb2.TransactionResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
-    def getStakersByAccountID(request,
+    def callEthereum(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.CryptoService/getStakersByAccountID',
-            query__pb2.Query.SerializeToString,
-            response__pb2.Response.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.SmartContractService/callEthereum',
+            transaction__pb2.Transaction.SerializeToString,
+            transaction__response__pb2.TransactionResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
```

### Comparing `hedera-proto-0.21.0/src/hedera_proto/duration_pb2.py` & `hedera_proto-0.49.0/src/hedera_proto/consensus_create_topic_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,71 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: duration.proto
+# source: consensus_create_topic.proto
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
+from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+import basic_types_pb2 as basic__types__pb2
+import duration_pb2 as duration__pb2
 
 
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='duration.proto',
-  package='proto',
-  syntax='proto3',
-  serialized_options=b'\n\"com.hederahashgraph.api.proto.javaP\001',
-  create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x0e\x64uration.proto\x12\x05proto\"\x1b\n\x08\x44uration\x12\x0f\n\x07seconds\x18\x01 \x01(\x03\x42&\n\"com.hederahashgraph.api.proto.javaP\x01\x62\x06proto3'
-)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x63onsensus_create_topic.proto\x12\x05proto\x1a\x11\x62\x61sic_types.proto\x1a\x0e\x64uration.proto\"\xc6\x01\n#ConsensusCreateTopicTransactionBody\x12\x0c\n\x04memo\x18\x01 \x01(\t\x12\x1c\n\x08\x61\x64minKey\x18\x02 \x01(\x0b\x32\n.proto.Key\x12\x1d\n\tsubmitKey\x18\x03 \x01(\x0b\x32\n.proto.Key\x12(\n\x0f\x61utoRenewPeriod\x18\x06 \x01(\x0b\x32\x0f.proto.Duration\x12*\n\x10\x61utoRenewAccount\x18\x07 \x01(\x0b\x32\x10.proto.AccountIDB&\n\"com.hederahashgraph.api.proto.javaP\x01\x62\x06proto3')
 
-
-
-
-_DURATION = _descriptor.Descriptor(
-  name='Duration',
-  full_name='proto.Duration',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='seconds', full_name='proto.Duration.seconds', index=0,
-      number=1, type=3, cpp_type=2, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=25,
-  serialized_end=52,
-)
-
-DESCRIPTOR.message_types_by_name['Duration'] = _DURATION
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
-
-Duration = _reflection.GeneratedProtocolMessageType('Duration', (_message.Message,), {
-  'DESCRIPTOR' : _DURATION,
-  '__module__' : 'duration_pb2'
-  # @@protoc_insertion_point(class_scope:proto.Duration)
-  })
-_sym_db.RegisterMessage(Duration)
-
-
-DESCRIPTOR._options = None
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'consensus_create_topic_pb2', _globals)
+if not _descriptor._USE_C_DESCRIPTORS:
+  _globals['DESCRIPTOR']._loaded_options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\"com.hederahashgraph.api.proto.javaP\001'
+  _globals['_CONSENSUSCREATETOPICTRANSACTIONBODY']._serialized_start=75
+  _globals['_CONSENSUSCREATETOPICTRANSACTIONBODY']._serialized_end=273
 # @@protoc_insertion_point(module_scope)
```

### Comparing `hedera-proto-0.21.0/src/hedera_proto/file_service_pb2_grpc.py` & `hedera_proto-0.49.0/src/hedera_proto/file_service_pb2_grpc.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,41 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
+import warnings
 
 import query_pb2 as query__pb2
 import response_pb2 as response__pb2
 import transaction_pb2 as transaction__pb2
 import transaction_response_pb2 as transaction__response__pb2
 
+GRPC_GENERATED_VERSION = '1.63.0'
+GRPC_VERSION = grpc.__version__
+EXPECTED_ERROR_RELEASE = '1.65.0'
+SCHEDULED_RELEASE_DATE = 'June 25, 2024'
+_version_not_supported = False
+
+try:
+    from grpc._utilities import first_version_is_lower
+    _version_not_supported = first_version_is_lower(GRPC_VERSION, GRPC_GENERATED_VERSION)
+except ImportError:
+    _version_not_supported = True
+
+if _version_not_supported:
+    warnings.warn(
+        f'The grpc package installed is at version {GRPC_VERSION},'
+        + f' but the generated code in file_service_pb2_grpc.py depends on'
+        + f' grpcio>={GRPC_GENERATED_VERSION}.'
+        + f' Please upgrade your grpc module to grpcio>={GRPC_GENERATED_VERSION}'
+        + f' or downgrade your generated code using grpcio-tools<={GRPC_VERSION}.'
+        + f' This warning will become an error in {EXPECTED_ERROR_RELEASE},'
+        + f' scheduled for release on {SCHEDULED_RELEASE_DATE}.',
+        RuntimeWarning
+    )
+
 
 class FileServiceStub(object):
     """*
     Transactions and queries for the file service. 
     """
 
     def __init__(self, channel):
@@ -19,50 +44,50 @@
         Args:
             channel: A grpc.Channel.
         """
         self.createFile = channel.unary_unary(
                 '/proto.FileService/createFile',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.updateFile = channel.unary_unary(
                 '/proto.FileService/updateFile',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.deleteFile = channel.unary_unary(
                 '/proto.FileService/deleteFile',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.appendContent = channel.unary_unary(
                 '/proto.FileService/appendContent',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.getFileContent = channel.unary_unary(
                 '/proto.FileService/getFileContent',
                 request_serializer=query__pb2.Query.SerializeToString,
                 response_deserializer=response__pb2.Response.FromString,
-                )
+                _registered_method=True)
         self.getFileInfo = channel.unary_unary(
                 '/proto.FileService/getFileInfo',
                 request_serializer=query__pb2.Query.SerializeToString,
                 response_deserializer=response__pb2.Response.FromString,
-                )
+                _registered_method=True)
         self.systemDelete = channel.unary_unary(
                 '/proto.FileService/systemDelete',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.systemUndelete = channel.unary_unary(
                 '/proto.FileService/systemUndelete',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
 
 
 class FileServiceServicer(object):
     """*
     Transactions and queries for the file service. 
     """
 
@@ -192,131 +217,211 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.FileService/createFile',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.FileService/createFile',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def updateFile(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.FileService/updateFile',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.FileService/updateFile',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def deleteFile(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.FileService/deleteFile',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.FileService/deleteFile',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def appendContent(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.FileService/appendContent',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.FileService/appendContent',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def getFileContent(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.FileService/getFileContent',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.FileService/getFileContent',
             query__pb2.Query.SerializeToString,
             response__pb2.Response.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def getFileInfo(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.FileService/getFileInfo',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.FileService/getFileInfo',
             query__pb2.Query.SerializeToString,
             response__pb2.Response.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def systemDelete(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.FileService/systemDelete',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.FileService/systemDelete',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def systemUndelete(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.FileService/systemUndelete',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.FileService/systemUndelete',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
```

### Comparing `hedera-proto-0.21.0/src/hedera_proto/freeze_service_pb2.py` & `hedera_proto-0.49.0/src/hedera_proto/file_service_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: freeze_service.proto
+# source: file_service.proto
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
+from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+import query_pb2 as query__pb2
+import response_pb2 as response__pb2
 import transaction_response_pb2 as transaction__response__pb2
 import transaction_pb2 as transaction__pb2
 
 
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='freeze_service.proto',
-  package='proto',
-  syntax='proto3',
-  serialized_options=b'\n&com.hederahashgraph.service.proto.java',
-  create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x14\x66reeze_service.proto\x12\x05proto\x1a\x1atransaction_response.proto\x1a\x11transaction.proto2I\n\rFreezeService\x12\x38\n\x06\x66reeze\x12\x12.proto.Transaction\x1a\x1a.proto.TransactionResponseB(\n&com.hederahashgraph.service.proto.javab\x06proto3'
-  ,
-  dependencies=[transaction__response__pb2.DESCRIPTOR,transaction__pb2.DESCRIPTOR,])
-
-
-
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
-
-
-DESCRIPTOR._options = None
-
-_FREEZESERVICE = _descriptor.ServiceDescriptor(
-  name='FreezeService',
-  full_name='proto.FreezeService',
-  file=DESCRIPTOR,
-  index=0,
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_start=78,
-  serialized_end=151,
-  methods=[
-  _descriptor.MethodDescriptor(
-    name='freeze',
-    full_name='proto.FreezeService.freeze',
-    index=0,
-    containing_service=None,
-    input_type=transaction__pb2._TRANSACTION,
-    output_type=transaction__response__pb2._TRANSACTIONRESPONSE,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-])
-_sym_db.RegisterServiceDescriptor(_FREEZESERVICE)
-
-DESCRIPTOR.services_by_name['FreezeService'] = _FREEZESERVICE
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x66ile_service.proto\x12\x05proto\x1a\x0bquery.proto\x1a\x0eresponse.proto\x1a\x1atransaction_response.proto\x1a\x11transaction.proto2\xe9\x03\n\x0b\x46ileService\x12<\n\ncreateFile\x12\x12.proto.Transaction\x1a\x1a.proto.TransactionResponse\x12<\n\nupdateFile\x12\x12.proto.Transaction\x1a\x1a.proto.TransactionResponse\x12<\n\ndeleteFile\x12\x12.proto.Transaction\x1a\x1a.proto.TransactionResponse\x12?\n\rappendContent\x12\x12.proto.Transaction\x1a\x1a.proto.TransactionResponse\x12/\n\x0egetFileContent\x12\x0c.proto.Query\x1a\x0f.proto.Response\x12,\n\x0bgetFileInfo\x12\x0c.proto.Query\x1a\x0f.proto.Response\x12>\n\x0csystemDelete\x12\x12.proto.Transaction\x1a\x1a.proto.TransactionResponse\x12@\n\x0esystemUndelete\x12\x12.proto.Transaction\x1a\x1a.proto.TransactionResponseB(\n&com.hederahashgraph.service.proto.javab\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'file_service_pb2', _globals)
+if not _descriptor._USE_C_DESCRIPTORS:
+  _globals['DESCRIPTOR']._loaded_options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n&com.hederahashgraph.service.proto.java'
+  _globals['_FILESERVICE']._serialized_start=106
+  _globals['_FILESERVICE']._serialized_end=595
 # @@protoc_insertion_point(module_scope)
```

### Comparing `hedera-proto-0.21.0/src/hedera_proto/pom.xml` & `hedera_proto-0.49.0/src/hedera_proto/pom.xml`

 * *Files 2% similar despite different names*

#### Comparing `hedera-proto-0.21.0/src/hedera_proto/pom.xml` & `hedera_proto-0.49.0/src/hedera_proto/pom.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <groupId>com.hedera.hashgraph</groupId>
   <artifactId>hedera-protobuf-java-api</artifactId>
   <packaging>jar</packaging>
-  <version>0.21.0</version>
+  <version>0.49.0</version>
   <name>hedera-protobuf-java-api</name>
   <description>Hedera Protobuf Java API</description>
   <url>https://github.com/hashgraph/hedera-protobuf</url>
   <licenses>
     <license>
       <name>Apache License, Version 2.0</name>
       <url>http://www.apache.org/licenses/LICENSE-2.0.txt</url>
@@ -21,15 +21,15 @@
       <organizationUrl>http://www.hedera.com</organizationUrl>
     </developer>
   </developers>
   <scm>
     <connection>scm:git:git@github.com:hashgraph/hedera-protobuf.git</connection>
     <developerConnection>scm:git:git@github.com:hashgraph/hedera-protobuf.git</developerConnection>
     <url>https://github.com/hashgraph/hedera-protobuf</url>
-    <tag>v0.21.0</tag>
+    <tag>v0.49.0</tag>
   </scm>
   <distributionManagement>
     <snapshotRepository>
       <id>ossrh</id>
       <url>https://oss.sonatype.org/content/repositories/snapshots</url>
     </snapshotRepository>
     <repository>
@@ -38,34 +38,34 @@
     </repository>
   </distributionManagement>
   <properties>
     <maven.compiler.source>8</maven.compiler.source>
     <maven.compiler.target>8</maven.compiler.target>
     <app.name>hedera-protobuf-java-api</app.name>
     <eddsa.version>0.3.0</eddsa.version>
-    <protobuf-java.version>3.8.0</protobuf-java.version>
+    <protobuf-java.version>3.16.1</protobuf-java.version>
     <javax.annotation-api.version>1.3.2</javax.annotation-api.version>
-    <grpc.version>1.39.0</grpc.version>
+    <grpc.version>1.45.1</grpc.version>
     <netty.version>4.1.66.Final</netty.version>
     <maven-jar.version>3.2.0</maven-jar.version>
     <maven-source.version>3.2.0</maven-source.version>
     <maven-license.version>2.0.0</maven-license.version>
     <maven-compiler.version>3.8.1</maven-compiler.version>
     <maven-jar.version>3.2.0</maven-jar.version>
     <maven-javadoc.version>3.2.0</maven-javadoc.version>
     <maven-release.version>3.0.0-M1</maven-release.version>
     <maven-surefire.version>2.22.2</maven-surefire.version>
     <maven-gpg.version>1.6</maven-gpg.version>
     <maven-dependency.version>3.1.1</maven-dependency.version>
     <maven-versions.version>2.8.1</maven-versions.version>
     <maven-project-info.version>2.8</maven-project-info.version>
-    <nexus-staging.version>1.6.8</nexus-staging.version>
+    <nexus-staging.version>1.6.13</nexus-staging.version>
     <os.plugin.version>1.6.0</os.plugin.version>
     <protobuf.plugin.version>0.6.1</protobuf.plugin.version>
-    <protoc.version>3.8.0</protoc.version>
+    <protoc.version>3.17.3</protoc.version>
   </properties>
   <dependencies>
     <dependency>
       <groupId>io.grpc</groupId>
       <artifactId>grpc-netty</artifactId>
       <version>${grpc.version}</version>
     </dependency>
@@ -180,14 +180,17 @@
         <artifactId>maven-jar-plugin</artifactId>
         <configuration>
           <archive>
             <manifest>
               <addClasspath>true</addClasspath>
               <classpathPrefix>lib/</classpathPrefix>
             </manifest>
+            <manifestEntries>
+              <Automatic-Module-Name>com.hedera.hashgraph.protobuf.java.api</Automatic-Module-Name>
+            </manifestEntries>
           </archive>
         </configuration>
       </plugin>
       <plugin>
         <groupId>org.apache.maven.plugins</groupId>
         <artifactId>maven-source-plugin</artifactId>
         <executions>
```

### Comparing `hedera-proto-0.21.0/src/hedera_proto/schedule_service_pb2_grpc.py` & `hedera_proto-0.49.0/src/hedera_proto/schedule_service_pb2_grpc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,184 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
+import warnings
 
 import query_pb2 as query__pb2
 import response_pb2 as response__pb2
 import transaction_pb2 as transaction__pb2
 import transaction_response_pb2 as transaction__response__pb2
 
+GRPC_GENERATED_VERSION = '1.63.0'
+GRPC_VERSION = grpc.__version__
+EXPECTED_ERROR_RELEASE = '1.65.0'
+SCHEDULED_RELEASE_DATE = 'June 25, 2024'
+_version_not_supported = False
+
+try:
+    from grpc._utilities import first_version_is_lower
+    _version_not_supported = first_version_is_lower(GRPC_VERSION, GRPC_GENERATED_VERSION)
+except ImportError:
+    _version_not_supported = True
+
+if _version_not_supported:
+    warnings.warn(
+        f'The grpc package installed is at version {GRPC_VERSION},'
+        + f' but the generated code in schedule_service_pb2_grpc.py depends on'
+        + f' grpcio>={GRPC_GENERATED_VERSION}.'
+        + f' Please upgrade your grpc module to grpcio>={GRPC_GENERATED_VERSION}'
+        + f' or downgrade your generated code using grpcio-tools<={GRPC_VERSION}.'
+        + f' This warning will become an error in {EXPECTED_ERROR_RELEASE},'
+        + f' scheduled for release on {SCHEDULED_RELEASE_DATE}.',
+        RuntimeWarning
+    )
+
 
 class ScheduleServiceStub(object):
     """*
     Transactions and queries for the Schedule Service
+
     The Schedule Service allows transactions to be submitted without all the required signatures and
     allows anyone to provide the required signatures independently after a transaction has already
-    been created.
+    been created. The transactions can be executed immediately when all required signatures are received
+    or at a future date if Long Term Scheduled Transactions are enabled.
+
     Execution:
-    Scheduled Transactions are executed once all required signatures are collected and witnessed.
+
+    Scheduled Transactions are executed in two different modes.
+
+    1. If Long Term Scheduled Transactions are enabled and <tt>wait_for_expiry</tt> was set to <tt>true</tt> on the
+    <tt>ScheduleCreate</tt>, then the transaction will be executed at the <tt>expiration_time</tt> specified on the
+    <tt>ScheduleCreate</tt>.
+
+    2. Otherwise Scheduled Transactions are executed once all required signatures are collected and witnessed.
     Every time new signature is provided, a check is performed on the "readiness" of the execution.
-    The Scheduled Transaction will be executed immediately after the transaction that triggered it
-    and will be externalised in a separate Transaction Record.
+    The Scheduled Transaction will be executed immediately after the transaction that triggered it.
+
+    NOTICE:
+    A Scheduled Transaction being ready to execute, or even not ready to execute, at the time a <tt>ScheduleCreate</tt> or
+    <tt>ScheduleSign</tt> comes in does not guarantee it will stay that way. Any number of things can happen over time that
+    impact the transaction.
+
+    For example, account keys can change, accounts can be deleted, and account balances can change.
+
+    A particularly noteworthy case is if Long Term Scheduled Transactions are enabled and signature requirements for a Scheduled
+    Transaction change such that existing signatures become sufficient to allow the transaction to go through. In this case the transaction
+    will execute at expiration_time unless a ScheduleSign comes in to push it through.
+
     Transaction Record:
-    The timestamp of the Scheduled Transaction will be equal to consensusTimestamp + 1 nano, where
+
+    If a Scheduled Transaction is executed immediately following the transaction that provided all required signatures,
+    the timestamp of the Scheduled Transaction will be equal to consensusTimestamp + 1 nano, where
     consensusTimestamp is the timestamp of the transaction that triggered the execution.
+
     The Transaction ID of the Scheduled Transaction will have the scheduled property set to true and
-    inherit the transactionValidStart and accountID from the ScheduleCreate transaction.
-    The scheduleRef property of the transaction record will be populated with the ScheduleID of the
+    inherit the <tt>transactionValidStart</tt> and <tt>accountID</tt> from the <tt>ScheduleCreate</tt> transaction.
+
+    The <tt>scheduleRef</tt> property of the transaction record will be populated with the <tt>ScheduleID</tt> of the
     Scheduled Transaction.
+
     Post execution:
-    Once a given Scheduled Transaction executes, it will be removed from the ledger and any upcoming
-    operation referring the ScheduleID will resolve to INVALID_SCHEDULE_ID.
+
+    After execution, a Scheduled Transaction will remain in state and can be queried using <tt>GetScheduleInfo</tt> until expiration.
+
     Expiry:
-    Scheduled Transactions have a global expiry time txExpiryTimeSecs (Currently set to 30 minutes).
-    If txExpiryTimeSecs pass and the Scheduled Transaction haven't yet executed, it will be removed
-    from the ledger as if ScheduleDelete operation is executed.
+
+    The expiration time of a schedule is controlled by it's <tt>expiration_time</tt>. If Long Term Scheduled Transactions are disabled,
+    the <tt>expiration_time</tt> is always 30 minutes in the future.
+
+    Once a given Scheduled Transaction expires, it will be removed from the ledger and any upcoming
+    operation referring the ScheduleID will resolve to INVALID_SCHEDULE_ID.
+
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.createSchedule = channel.unary_unary(
                 '/proto.ScheduleService/createSchedule',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.signSchedule = channel.unary_unary(
                 '/proto.ScheduleService/signSchedule',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.deleteSchedule = channel.unary_unary(
                 '/proto.ScheduleService/deleteSchedule',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.getScheduleInfo = channel.unary_unary(
                 '/proto.ScheduleService/getScheduleInfo',
                 request_serializer=query__pb2.Query.SerializeToString,
                 response_deserializer=response__pb2.Response.FromString,
-                )
+                _registered_method=True)
 
 
 class ScheduleServiceServicer(object):
     """*
     Transactions and queries for the Schedule Service
+
     The Schedule Service allows transactions to be submitted without all the required signatures and
     allows anyone to provide the required signatures independently after a transaction has already
-    been created.
+    been created. The transactions can be executed immediately when all required signatures are received
+    or at a future date if Long Term Scheduled Transactions are enabled.
+
     Execution:
-    Scheduled Transactions are executed once all required signatures are collected and witnessed.
+
+    Scheduled Transactions are executed in two different modes.
+
+    1. If Long Term Scheduled Transactions are enabled and <tt>wait_for_expiry</tt> was set to <tt>true</tt> on the
+    <tt>ScheduleCreate</tt>, then the transaction will be executed at the <tt>expiration_time</tt> specified on the
+    <tt>ScheduleCreate</tt>.
+
+    2. Otherwise Scheduled Transactions are executed once all required signatures are collected and witnessed.
     Every time new signature is provided, a check is performed on the "readiness" of the execution.
-    The Scheduled Transaction will be executed immediately after the transaction that triggered it
-    and will be externalised in a separate Transaction Record.
+    The Scheduled Transaction will be executed immediately after the transaction that triggered it.
+
+    NOTICE:
+    A Scheduled Transaction being ready to execute, or even not ready to execute, at the time a <tt>ScheduleCreate</tt> or
+    <tt>ScheduleSign</tt> comes in does not guarantee it will stay that way. Any number of things can happen over time that
+    impact the transaction.
+
+    For example, account keys can change, accounts can be deleted, and account balances can change.
+
+    A particularly noteworthy case is if Long Term Scheduled Transactions are enabled and signature requirements for a Scheduled
+    Transaction change such that existing signatures become sufficient to allow the transaction to go through. In this case the transaction
+    will execute at expiration_time unless a ScheduleSign comes in to push it through.
+
     Transaction Record:
-    The timestamp of the Scheduled Transaction will be equal to consensusTimestamp + 1 nano, where
+
+    If a Scheduled Transaction is executed immediately following the transaction that provided all required signatures,
+    the timestamp of the Scheduled Transaction will be equal to consensusTimestamp + 1 nano, where
     consensusTimestamp is the timestamp of the transaction that triggered the execution.
+
     The Transaction ID of the Scheduled Transaction will have the scheduled property set to true and
-    inherit the transactionValidStart and accountID from the ScheduleCreate transaction.
-    The scheduleRef property of the transaction record will be populated with the ScheduleID of the
+    inherit the <tt>transactionValidStart</tt> and <tt>accountID</tt> from the <tt>ScheduleCreate</tt> transaction.
+
+    The <tt>scheduleRef</tt> property of the transaction record will be populated with the <tt>ScheduleID</tt> of the
     Scheduled Transaction.
+
     Post execution:
-    Once a given Scheduled Transaction executes, it will be removed from the ledger and any upcoming
-    operation referring the ScheduleID will resolve to INVALID_SCHEDULE_ID.
+
+    After execution, a Scheduled Transaction will remain in state and can be queried using <tt>GetScheduleInfo</tt> until expiration.
+
     Expiry:
-    Scheduled Transactions have a global expiry time txExpiryTimeSecs (Currently set to 30 minutes).
-    If txExpiryTimeSecs pass and the Scheduled Transaction haven't yet executed, it will be removed
-    from the ledger as if ScheduleDelete operation is executed.
+
+    The expiration time of a schedule is controlled by it's <tt>expiration_time</tt>. If Long Term Scheduled Transactions are disabled,
+    the <tt>expiration_time</tt> is always 30 minutes in the future.
+
+    Once a given Scheduled Transaction expires, it will be removed from the ledger and any upcoming
+    operation referring the ScheduleID will resolve to INVALID_SCHEDULE_ID.
+
     """
 
     def createSchedule(self, request, context):
         """*
         Creates a new Schedule by submitting the transaction
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
@@ -151,98 +238,169 @@
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class ScheduleService(object):
     """*
     Transactions and queries for the Schedule Service
+
     The Schedule Service allows transactions to be submitted without all the required signatures and
     allows anyone to provide the required signatures independently after a transaction has already
-    been created.
+    been created. The transactions can be executed immediately when all required signatures are received
+    or at a future date if Long Term Scheduled Transactions are enabled.
+
     Execution:
-    Scheduled Transactions are executed once all required signatures are collected and witnessed.
+
+    Scheduled Transactions are executed in two different modes.
+
+    1. If Long Term Scheduled Transactions are enabled and <tt>wait_for_expiry</tt> was set to <tt>true</tt> on the
+    <tt>ScheduleCreate</tt>, then the transaction will be executed at the <tt>expiration_time</tt> specified on the
+    <tt>ScheduleCreate</tt>.
+
+    2. Otherwise Scheduled Transactions are executed once all required signatures are collected and witnessed.
     Every time new signature is provided, a check is performed on the "readiness" of the execution.
-    The Scheduled Transaction will be executed immediately after the transaction that triggered it
-    and will be externalised in a separate Transaction Record.
+    The Scheduled Transaction will be executed immediately after the transaction that triggered it.
+
+    NOTICE:
+    A Scheduled Transaction being ready to execute, or even not ready to execute, at the time a <tt>ScheduleCreate</tt> or
+    <tt>ScheduleSign</tt> comes in does not guarantee it will stay that way. Any number of things can happen over time that
+    impact the transaction.
+
+    For example, account keys can change, accounts can be deleted, and account balances can change.
+
+    A particularly noteworthy case is if Long Term Scheduled Transactions are enabled and signature requirements for a Scheduled
+    Transaction change such that existing signatures become sufficient to allow the transaction to go through. In this case the transaction
+    will execute at expiration_time unless a ScheduleSign comes in to push it through.
+
     Transaction Record:
-    The timestamp of the Scheduled Transaction will be equal to consensusTimestamp + 1 nano, where
+
+    If a Scheduled Transaction is executed immediately following the transaction that provided all required signatures,
+    the timestamp of the Scheduled Transaction will be equal to consensusTimestamp + 1 nano, where
     consensusTimestamp is the timestamp of the transaction that triggered the execution.
+
     The Transaction ID of the Scheduled Transaction will have the scheduled property set to true and
-    inherit the transactionValidStart and accountID from the ScheduleCreate transaction.
-    The scheduleRef property of the transaction record will be populated with the ScheduleID of the
+    inherit the <tt>transactionValidStart</tt> and <tt>accountID</tt> from the <tt>ScheduleCreate</tt> transaction.
+
+    The <tt>scheduleRef</tt> property of the transaction record will be populated with the <tt>ScheduleID</tt> of the
     Scheduled Transaction.
+
     Post execution:
-    Once a given Scheduled Transaction executes, it will be removed from the ledger and any upcoming
-    operation referring the ScheduleID will resolve to INVALID_SCHEDULE_ID.
+
+    After execution, a Scheduled Transaction will remain in state and can be queried using <tt>GetScheduleInfo</tt> until expiration.
+
     Expiry:
-    Scheduled Transactions have a global expiry time txExpiryTimeSecs (Currently set to 30 minutes).
-    If txExpiryTimeSecs pass and the Scheduled Transaction haven't yet executed, it will be removed
-    from the ledger as if ScheduleDelete operation is executed.
+
+    The expiration time of a schedule is controlled by it's <tt>expiration_time</tt>. If Long Term Scheduled Transactions are disabled,
+    the <tt>expiration_time</tt> is always 30 minutes in the future.
+
+    Once a given Scheduled Transaction expires, it will be removed from the ledger and any upcoming
+    operation referring the ScheduleID will resolve to INVALID_SCHEDULE_ID.
+
     """
 
     @staticmethod
     def createSchedule(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.ScheduleService/createSchedule',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.ScheduleService/createSchedule',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def signSchedule(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.ScheduleService/signSchedule',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.ScheduleService/signSchedule',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def deleteSchedule(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.ScheduleService/deleteSchedule',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.ScheduleService/deleteSchedule',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def getScheduleInfo(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.ScheduleService/getScheduleInfo',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.ScheduleService/getScheduleInfo',
             query__pb2.Query.SerializeToString,
             response__pb2.Response.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
```

### Comparing `hedera-proto-0.21.0/src/hedera_proto/token_service_pb2_grpc.py` & `hedera_proto-0.49.0/src/hedera_proto/token_service_pb2_grpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,41 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
+import warnings
 
 import query_pb2 as query__pb2
 import response_pb2 as response__pb2
 import transaction_pb2 as transaction__pb2
 import transaction_response_pb2 as transaction__response__pb2
 
+GRPC_GENERATED_VERSION = '1.63.0'
+GRPC_VERSION = grpc.__version__
+EXPECTED_ERROR_RELEASE = '1.65.0'
+SCHEDULED_RELEASE_DATE = 'June 25, 2024'
+_version_not_supported = False
+
+try:
+    from grpc._utilities import first_version_is_lower
+    _version_not_supported = first_version_is_lower(GRPC_VERSION, GRPC_GENERATED_VERSION)
+except ImportError:
+    _version_not_supported = True
+
+if _version_not_supported:
+    warnings.warn(
+        f'The grpc package installed is at version {GRPC_VERSION},'
+        + f' but the generated code in token_service_pb2_grpc.py depends on'
+        + f' grpcio>={GRPC_GENERATED_VERSION}.'
+        + f' Please upgrade your grpc module to grpcio>={GRPC_GENERATED_VERSION}'
+        + f' or downgrade your generated code using grpcio-tools<={GRPC_VERSION}.'
+        + f' This warning will become an error in {EXPECTED_ERROR_RELEASE},'
+        + f' scheduled for release on {SCHEDULED_RELEASE_DATE}.',
+        RuntimeWarning
+    )
+
 
 class TokenServiceStub(object):
     """*
     Transactions and queries for the Token Service
     """
 
     def __init__(self, channel):
@@ -19,105 +44,110 @@
         Args:
             channel: A grpc.Channel.
         """
         self.createToken = channel.unary_unary(
                 '/proto.TokenService/createToken',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.updateToken = channel.unary_unary(
                 '/proto.TokenService/updateToken',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.mintToken = channel.unary_unary(
                 '/proto.TokenService/mintToken',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.burnToken = channel.unary_unary(
                 '/proto.TokenService/burnToken',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.deleteToken = channel.unary_unary(
                 '/proto.TokenService/deleteToken',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.wipeTokenAccount = channel.unary_unary(
                 '/proto.TokenService/wipeTokenAccount',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.freezeTokenAccount = channel.unary_unary(
                 '/proto.TokenService/freezeTokenAccount',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.unfreezeTokenAccount = channel.unary_unary(
                 '/proto.TokenService/unfreezeTokenAccount',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.grantKycToTokenAccount = channel.unary_unary(
                 '/proto.TokenService/grantKycToTokenAccount',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.revokeKycFromTokenAccount = channel.unary_unary(
                 '/proto.TokenService/revokeKycFromTokenAccount',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.associateTokens = channel.unary_unary(
                 '/proto.TokenService/associateTokens',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.dissociateTokens = channel.unary_unary(
                 '/proto.TokenService/dissociateTokens',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.updateTokenFeeSchedule = channel.unary_unary(
                 '/proto.TokenService/updateTokenFeeSchedule',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.getTokenInfo = channel.unary_unary(
                 '/proto.TokenService/getTokenInfo',
                 request_serializer=query__pb2.Query.SerializeToString,
                 response_deserializer=response__pb2.Response.FromString,
-                )
+                _registered_method=True)
         self.getAccountNftInfos = channel.unary_unary(
                 '/proto.TokenService/getAccountNftInfos',
                 request_serializer=query__pb2.Query.SerializeToString,
                 response_deserializer=response__pb2.Response.FromString,
-                )
+                _registered_method=True)
         self.getTokenNftInfo = channel.unary_unary(
                 '/proto.TokenService/getTokenNftInfo',
                 request_serializer=query__pb2.Query.SerializeToString,
                 response_deserializer=response__pb2.Response.FromString,
-                )
+                _registered_method=True)
         self.getTokenNftInfos = channel.unary_unary(
                 '/proto.TokenService/getTokenNftInfos',
                 request_serializer=query__pb2.Query.SerializeToString,
                 response_deserializer=response__pb2.Response.FromString,
-                )
+                _registered_method=True)
         self.pauseToken = channel.unary_unary(
                 '/proto.TokenService/pauseToken',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
         self.unpauseToken = channel.unary_unary(
                 '/proto.TokenService/unpauseToken',
                 request_serializer=transaction__pb2.Transaction.SerializeToString,
                 response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
-                )
+                _registered_method=True)
+        self.updateNfts = channel.unary_unary(
+                '/proto.TokenService/updateNfts',
+                request_serializer=transaction__pb2.Transaction.SerializeToString,
+                response_deserializer=transaction__response__pb2.TransactionResponse.FromString,
+                _registered_method=True)
 
 
 class TokenServiceServicer(object):
     """*
     Transactions and queries for the Token Service
     """
 
@@ -267,14 +297,22 @@
     def unpauseToken(self, request, context):
         """Unpause the token
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def updateNfts(self, request, context):
+        """*
+        Updates the NFTs in a collection by TokenID and serial number
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_TokenServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'createToken': grpc.unary_unary_rpc_method_handler(
                     servicer.createToken,
                     request_deserializer=transaction__pb2.Transaction.FromString,
                     response_serializer=transaction__response__pb2.TransactionResponse.SerializeToString,
@@ -365,14 +403,19 @@
                     response_serializer=transaction__response__pb2.TransactionResponse.SerializeToString,
             ),
             'unpauseToken': grpc.unary_unary_rpc_method_handler(
                     servicer.unpauseToken,
                     request_deserializer=transaction__pb2.Transaction.FromString,
                     response_serializer=transaction__response__pb2.TransactionResponse.SerializeToString,
             ),
+            'updateNfts': grpc.unary_unary_rpc_method_handler(
+                    servicer.updateNfts,
+                    request_deserializer=transaction__pb2.Transaction.FromString,
+                    response_serializer=transaction__response__pb2.TransactionResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'proto.TokenService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -388,318 +431,535 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.TokenService/createToken',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.TokenService/createToken',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def updateToken(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.TokenService/updateToken',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.TokenService/updateToken',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def mintToken(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.TokenService/mintToken',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.TokenService/mintToken',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def burnToken(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.TokenService/burnToken',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.TokenService/burnToken',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def deleteToken(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.TokenService/deleteToken',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.TokenService/deleteToken',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def wipeTokenAccount(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.TokenService/wipeTokenAccount',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.TokenService/wipeTokenAccount',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def freezeTokenAccount(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.TokenService/freezeTokenAccount',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.TokenService/freezeTokenAccount',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def unfreezeTokenAccount(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.TokenService/unfreezeTokenAccount',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.TokenService/unfreezeTokenAccount',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def grantKycToTokenAccount(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.TokenService/grantKycToTokenAccount',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.TokenService/grantKycToTokenAccount',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def revokeKycFromTokenAccount(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.TokenService/revokeKycFromTokenAccount',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.TokenService/revokeKycFromTokenAccount',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def associateTokens(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.TokenService/associateTokens',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.TokenService/associateTokens',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def dissociateTokens(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.TokenService/dissociateTokens',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.TokenService/dissociateTokens',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def updateTokenFeeSchedule(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.TokenService/updateTokenFeeSchedule',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.TokenService/updateTokenFeeSchedule',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def getTokenInfo(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.TokenService/getTokenInfo',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.TokenService/getTokenInfo',
             query__pb2.Query.SerializeToString,
             response__pb2.Response.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def getAccountNftInfos(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.TokenService/getAccountNftInfos',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.TokenService/getAccountNftInfos',
             query__pb2.Query.SerializeToString,
             response__pb2.Response.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def getTokenNftInfo(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.TokenService/getTokenNftInfo',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.TokenService/getTokenNftInfo',
             query__pb2.Query.SerializeToString,
             response__pb2.Response.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def getTokenNftInfos(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.TokenService/getTokenNftInfos',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.TokenService/getTokenNftInfos',
             query__pb2.Query.SerializeToString,
             response__pb2.Response.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def pauseToken(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.TokenService/pauseToken',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.TokenService/pauseToken',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def unpauseToken(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/proto.TokenService/unpauseToken',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.TokenService/unpauseToken',
+            transaction__pb2.Transaction.SerializeToString,
+            transaction__response__pb2.TransactionResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
+
+    @staticmethod
+    def updateNfts(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/proto.TokenService/updateNfts',
             transaction__pb2.Transaction.SerializeToString,
             transaction__response__pb2.TransactionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
```

### Comparing `hedera-proto-0.21.0/src/hedera_proto.egg-info/PKG-INFO` & `hedera_proto-0.49.0/src/hedera_proto.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: hedera-proto
-Version: 0.21.0
+Version: 0.49.0
 Summary: Hedera Protobufs
-Home-page: https://github.com/carady/hedera-protobufs-python
+Home-page: https://github.com/carady/hedera-proto-py
 Author: Wensheng Wang
 Author-email: wenshengwang@gmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/carady/hedera-protobufs-python/issues
-Platform: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/carady/hedera-proto-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: grpcio>=1.34.1
 
 # hedera-protobufs-python
 
 Hedera API Definitions in Protocol Buffer compiled to Python
 
 They are compiled from .proto files in [Java Protobufs](https://github.com/hashgraph/hedera-protobufs-java).
 
@@ -38,9 +37,7 @@
     accountId = proto.AccountID()
 
 ## Note
 
 This is used by pure Python Hedera SDK, which, as of now (2021/11), has not been released yet.
 
 You are encouraged to use the fully functional Python SDK [github.com/wensheng/hedera-sdk-py](https://github.com/wensheng/hedera-sdk-py), which is a Python wrapper around Java SDK, while waiting for pure Python SDK.
-
-
```

### Comparing `hedera-proto-0.21.0/src/hedera_proto.egg-info/SOURCES.txt` & `hedera_proto-0.49.0/src/hedera_proto.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -10,69 +10,84 @@
 src/hedera_proto/consensus_delete_topic_pb2.py
 src/hedera_proto/consensus_get_topic_info_pb2.py
 src/hedera_proto/consensus_service_pb2.py
 src/hedera_proto/consensus_service_pb2_grpc.py
 src/hedera_proto/consensus_submit_message_pb2.py
 src/hedera_proto/consensus_topic_info_pb2.py
 src/hedera_proto/consensus_update_topic_pb2.py
+src/hedera_proto/contract_action_pb2.py
+src/hedera_proto/contract_bytecode_pb2.py
 src/hedera_proto/contract_call_local_pb2.py
 src/hedera_proto/contract_call_pb2.py
 src/hedera_proto/contract_create_pb2.py
 src/hedera_proto/contract_delete_pb2.py
 src/hedera_proto/contract_get_bytecode_pb2.py
 src/hedera_proto/contract_get_info_pb2.py
 src/hedera_proto/contract_get_records_pb2.py
+src/hedera_proto/contract_state_change_pb2.py
+src/hedera_proto/contract_types_pb2.py
 src/hedera_proto/contract_update_pb2.py
 src/hedera_proto/crypto_add_live_hash_pb2.py
+src/hedera_proto/crypto_approve_allowance_pb2.py
 src/hedera_proto/crypto_create_pb2.py
+src/hedera_proto/crypto_delete_allowance_pb2.py
 src/hedera_proto/crypto_delete_live_hash_pb2.py
 src/hedera_proto/crypto_delete_pb2.py
 src/hedera_proto/crypto_get_account_balance_pb2.py
 src/hedera_proto/crypto_get_account_records_pb2.py
 src/hedera_proto/crypto_get_info_pb2.py
 src/hedera_proto/crypto_get_live_hash_pb2.py
 src/hedera_proto/crypto_get_stakers_pb2.py
 src/hedera_proto/crypto_service_pb2.py
 src/hedera_proto/crypto_service_pb2_grpc.py
 src/hedera_proto/crypto_transfer_pb2.py
 src/hedera_proto/crypto_update_pb2.py
 src/hedera_proto/custom_fees_pb2.py
 src/hedera_proto/duration_pb2.py
+src/hedera_proto/ethereum_transaction_pb2.py
 src/hedera_proto/exchange_rate_pb2.py
 src/hedera_proto/file_append_pb2.py
 src/hedera_proto/file_create_pb2.py
 src/hedera_proto/file_delete_pb2.py
 src/hedera_proto/file_get_contents_pb2.py
 src/hedera_proto/file_get_info_pb2.py
 src/hedera_proto/file_service_pb2.py
 src/hedera_proto/file_service_pb2_grpc.py
 src/hedera_proto/file_update_pb2.py
 src/hedera_proto/freeze_pb2.py
 src/hedera_proto/freeze_service_pb2.py
 src/hedera_proto/freeze_service_pb2_grpc.py
 src/hedera_proto/freeze_type_pb2.py
+src/hedera_proto/get_account_details_pb2.py
 src/hedera_proto/get_by_key_pb2.py
 src/hedera_proto/get_by_solidity_id_pb2.py
+src/hedera_proto/hash_object_pb2.py
+src/hedera_proto/mirror_network_service_pb2.py
+src/hedera_proto/mirror_network_service_pb2_grpc.py
 src/hedera_proto/network_get_execution_time_pb2.py
 src/hedera_proto/network_get_version_info_pb2.py
 src/hedera_proto/network_service_pb2.py
 src/hedera_proto/network_service_pb2_grpc.py
+src/hedera_proto/node_stake_update_pb2.py
 src/hedera_proto/pom.xml
 src/hedera_proto/query_header_pb2.py
 src/hedera_proto/query_pb2.py
+src/hedera_proto/record_stream_file_pb2.py
 src/hedera_proto/response_code_pb2.py
 src/hedera_proto/response_header_pb2.py
 src/hedera_proto/response_pb2.py
 src/hedera_proto/schedulable_transaction_body_pb2.py
 src/hedera_proto/schedule_create_pb2.py
 src/hedera_proto/schedule_delete_pb2.py
 src/hedera_proto/schedule_get_info_pb2.py
 src/hedera_proto/schedule_service_pb2.py
 src/hedera_proto/schedule_service_pb2_grpc.py
 src/hedera_proto/schedule_sign_pb2.py
+src/hedera_proto/sidecar_file_pb2.py
+src/hedera_proto/signature_file_pb2.py
 src/hedera_proto/smart_contract_service_pb2.py
 src/hedera_proto/smart_contract_service_pb2_grpc.py
 src/hedera_proto/system_delete_pb2.py
 src/hedera_proto/system_undelete_pb2.py
 src/hedera_proto/throttle_definitions_pb2.py
 src/hedera_proto/timestamp_pb2.py
 src/hedera_proto/token_associate_pb2.py
@@ -90,25 +105,29 @@
 src/hedera_proto/token_mint_pb2.py
 src/hedera_proto/token_pause_pb2.py
 src/hedera_proto/token_revoke_kyc_pb2.py
 src/hedera_proto/token_service_pb2.py
 src/hedera_proto/token_service_pb2_grpc.py
 src/hedera_proto/token_unfreeze_account_pb2.py
 src/hedera_proto/token_unpause_pb2.py
+src/hedera_proto/token_update_nfts_pb2.py
 src/hedera_proto/token_update_pb2.py
 src/hedera_proto/token_wipe_account_pb2.py
 src/hedera_proto/transaction_body_pb2.py
 src/hedera_proto/transaction_contents_pb2.py
 src/hedera_proto/transaction_get_fast_record_pb2.py
 src/hedera_proto/transaction_get_receipt_pb2.py
 src/hedera_proto/transaction_get_record_pb2.py
 src/hedera_proto/transaction_list_pb2.py
 src/hedera_proto/transaction_pb2.py
 src/hedera_proto/transaction_receipt_pb2.py
 src/hedera_proto/transaction_record_pb2.py
 src/hedera_proto/transaction_response_pb2.py
 src/hedera_proto/unchecked_submit_pb2.py
+src/hedera_proto/util_prng_pb2.py
+src/hedera_proto/util_service_pb2.py
+src/hedera_proto/util_service_pb2_grpc.py
 src/hedera_proto.egg-info/PKG-INFO
 src/hedera_proto.egg-info/SOURCES.txt
 src/hedera_proto.egg-info/dependency_links.txt
 src/hedera_proto.egg-info/requires.txt
 src/hedera_proto.egg-info/top_level.txt
```

