# Comparing `tmp/glitter_sdk-1.0.3.tar.gz` & `tmp/glitter_sdk-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glitter_sdk-1.0.3.tar", max compression
+gzip compressed data, was "glitter_sdk-1.0.4.tar", max compression
```

## Comparing `glitter_sdk-1.0.3.tar` & `glitter_sdk-1.0.4.tar`

### file list

```diff
@@ -1,159 +1,159 @@
--rw-r--r--   0        0        0     1073 2023-09-03 07:54:13.137170 glitter_sdk-1.0.3/LICENSE
--rw-r--r--   0        0        0       95 2023-09-03 07:54:13.138300 glitter_sdk-1.0.3/README.md
--rw-r--r--   0        0        0       13 2023-09-03 07:54:13.380840 glitter_sdk-1.0.3/glitter_sdk/.gitignore
--rw-r--r--   0        0        0      163 2023-09-03 07:54:13.368337 glitter_sdk-1.0.3/glitter_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-09-03 07:54:13.383129 glitter_sdk-1.0.3/glitter_sdk/client/__init__.py
--rw-r--r--   0        0        0      196 2023-09-03 07:54:13.387634 glitter_sdk-1.0.3/glitter_sdk/client/lcd/__init__.py
--rw-r--r--   0        0        0        0 2023-09-03 07:54:13.398728 glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/__init__.py
--rw-r--r--   0        0        0      812 2023-09-03 07:54:13.397064 glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/_base.py
--rw-r--r--   0        0        0     1491 2023-09-03 07:54:13.396619 glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/auth.py
--rw-r--r--   0        0        0     3436 2023-09-03 07:54:13.426154 glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/authz.py
--rw-r--r--   0        0        0     2471 2023-09-03 07:54:13.399962 glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/bank.py
--rw-r--r--   0        0        0     4394 2023-09-03 07:54:13.423967 glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/distribution.py
--rw-r--r--   0        0        0     3632 2023-09-03 07:54:13.399297 glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/feegrant.py
--rw-r--r--   0        0        0    10274 2023-09-03 07:54:13.426902 glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/gov.py
--rw-r--r--   0        0        0      587 2023-09-03 07:54:13.400568 glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/ibc.py
--rw-r--r--   0        0        0      762 2023-09-03 07:54:13.425645 glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/ibc_transfer.py
--rw-r--r--   0        0        0     2330 2023-09-03 07:54:13.425202 glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/mint.py
--rw-r--r--   0        0        0     3776 2023-09-03 07:54:13.424822 glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/slashing.py
--rw-r--r--   0        0        0    13196 2023-09-03 07:54:13.397808 glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/staking.py
--rw-r--r--   0        0        0     3065 2023-09-03 07:54:13.398507 glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/tendermint.py
--rw-r--r--   0        0        0    14761 2023-09-03 07:54:13.426493 glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/tx.py
--rw-r--r--   0        0        0     5011 2023-09-03 07:54:13.424466 glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/wasm.py
--rw-r--r--   0        0        0      878 2023-09-03 07:54:13.387230 glitter_sdk-1.0.3/glitter_sdk/client/lcd/constants/CLIENT.py
--rw-r--r--   0        0        0        0 2023-09-03 07:54:13.387350 glitter_sdk-1.0.3/glitter_sdk/client/lcd/constants/__init__.py
--rw-r--r--   0        0        0    19291 2023-09-03 07:54:13.385851 glitter_sdk-1.0.3/glitter_sdk/client/lcd/db.py
--rw-r--r--   0        0        0    11250 2023-09-03 07:54:13.385407 glitter_sdk-1.0.3/glitter_sdk/client/lcd/lcdclient.py
--rw-r--r--   0        0        0     1803 2023-09-03 07:54:13.386589 glitter_sdk-1.0.3/glitter_sdk/client/lcd/lcdutils.py
--rw-r--r--   0        0        0     2394 2023-09-03 07:54:13.386324 glitter_sdk-1.0.3/glitter_sdk/client/lcd/params.py
--rw-r--r--   0        0        0     4901 2023-09-03 07:54:13.380244 glitter_sdk-1.0.3/glitter_sdk/connection.py
--rw-r--r--   0        0        0      949 2023-09-03 07:54:13.213135 glitter_sdk-1.0.3/glitter_sdk/core/__init__.py
--rw-r--r--   0        0        0      661 2023-09-03 07:54:13.166849 glitter_sdk-1.0.3/glitter_sdk/core/auth/__init__.py
--rw-r--r--   0        0        0      656 2023-09-03 07:54:13.179549 glitter_sdk-1.0.3/glitter_sdk/core/auth/data/__init__.py
--rw-r--r--   0        0        0     1835 2023-09-03 07:54:13.193756 glitter_sdk-1.0.3/glitter_sdk/core/auth/data/account.py
--rw-r--r--   0        0        0     2953 2023-09-03 07:54:13.180040 glitter_sdk-1.0.3/glitter_sdk/core/auth/data/base_account.py
--rw-r--r--   0        0        0     3965 2023-09-03 07:54:13.180496 glitter_sdk-1.0.3/glitter_sdk/core/auth/data/base_vesting_account.py
--rw-r--r--   0        0        0     2731 2023-09-03 07:54:13.193175 glitter_sdk-1.0.3/glitter_sdk/core/auth/data/continuous_vesting_account.py
--rw-r--r--   0        0        0     2498 2023-09-03 07:54:13.192420 glitter_sdk-1.0.3/glitter_sdk/core/auth/data/delayed_vesting_account.py
--rw-r--r--   0        0        0     2340 2023-09-03 07:54:13.178489 glitter_sdk-1.0.3/glitter_sdk/core/auth/data/eth_account.py
--rw-r--r--   0        0        0     4441 2023-09-03 07:54:13.179015 glitter_sdk-1.0.3/glitter_sdk/core/auth/data/periodic_vesting_account.py
--rw-r--r--   0        0        0      331 2023-09-03 07:54:13.169621 glitter_sdk-1.0.3/glitter_sdk/core/auth/msgs/__init__.py
--rw-r--r--   0        0        0     2921 2023-09-03 07:54:13.176777 glitter_sdk-1.0.3/glitter_sdk/core/auth/msgs/msg_create_periodic_vesting_account.py
--rw-r--r--   0        0        0     2838 2023-09-03 07:54:13.177286 glitter_sdk-1.0.3/glitter_sdk/core/auth/msgs/msg_create_vesting_account.py
--rw-r--r--   0        0        0     1620 2023-09-03 07:54:13.177856 glitter_sdk-1.0.3/glitter_sdk/core/auth/msgs/msg_donate_all_vesting_tokens.py
--rw-r--r--   0        0        0      446 2023-09-03 07:54:13.294076 glitter_sdk-1.0.3/glitter_sdk/core/authz/__init__.py
--rw-r--r--   0        0        0     9613 2023-09-03 07:54:13.302174 glitter_sdk-1.0.3/glitter_sdk/core/authz/data.py
--rw-r--r--   0        0        0     6109 2023-09-03 07:54:13.301531 glitter_sdk-1.0.3/glitter_sdk/core/authz/msgs.py
--rw-r--r--   0        0        0      149 2023-09-03 07:54:13.195011 glitter_sdk-1.0.3/glitter_sdk/core/bank/__init__.py
--rw-r--r--   0        0        0     7099 2023-09-03 07:54:13.196914 glitter_sdk-1.0.3/glitter_sdk/core/bank/msgs.py
--rw-r--r--   0        0        0     5009 2023-09-03 07:54:13.159260 glitter_sdk-1.0.3/glitter_sdk/core/bech32.py
--rw-r--r--   0        0        0     1616 2023-09-03 07:54:13.302812 glitter_sdk-1.0.3/glitter_sdk/core/block.py
--rw-r--r--   0        0        0     2724 2023-09-03 07:54:13.304464 glitter_sdk-1.0.3/glitter_sdk/core/broadcast.py
--rw-r--r--   0        0        0     7746 2023-09-03 07:54:13.307900 glitter_sdk-1.0.3/glitter_sdk/core/coin.py
--rw-r--r--   0        0        0     8360 2023-09-03 07:54:13.293168 glitter_sdk-1.0.3/glitter_sdk/core/coins.py
--rw-r--r--   0        0        0     2707 2023-09-03 07:54:13.291864 glitter_sdk-1.0.3/glitter_sdk/core/compact_bit_array.py
--rw-r--r--   0        0        0       71 2023-09-03 07:54:13.238361 glitter_sdk-1.0.3/glitter_sdk/core/crisis/__init__.py
--rw-r--r--   0        0        0     2069 2023-09-03 07:54:13.238872 glitter_sdk-1.0.3/glitter_sdk/core/crisis/msgs.py
--rw-r--r--   0        0        0     1085 2023-09-03 07:54:13.166080 glitter_sdk-1.0.3/glitter_sdk/core/deposit.py
--rw-r--r--   0        0        0      371 2023-09-03 07:54:13.207165 glitter_sdk-1.0.3/glitter_sdk/core/distribution/__init__.py
--rw-r--r--   0        0        0     6940 2023-09-03 07:54:13.212207 glitter_sdk-1.0.3/glitter_sdk/core/distribution/msgs.py
--rw-r--r--   0        0        0     2692 2023-09-03 07:54:13.212710 glitter_sdk-1.0.3/glitter_sdk/core/distribution/proposals.py
--rw-r--r--   0        0        0     2008 2023-09-03 07:54:13.239461 glitter_sdk-1.0.3/glitter_sdk/core/fee.py
--rw-r--r--   0        0        0      297 2023-09-03 07:54:13.159943 glitter_sdk-1.0.3/glitter_sdk/core/feegrant/__init__.py
--rw-r--r--   0        0        0     9141 2023-09-03 07:54:13.165604 glitter_sdk-1.0.3/glitter_sdk/core/feegrant/data.py
--rw-r--r--   0        0        0     3178 2023-09-03 07:54:13.165112 glitter_sdk-1.0.3/glitter_sdk/core/feegrant/msgs.py
--rw-r--r--   0        0        0      412 2023-09-03 07:54:13.309717 glitter_sdk-1.0.3/glitter_sdk/core/gov/__init__.py
--rw-r--r--   0        0        0     6154 2023-09-03 07:54:13.319571 glitter_sdk-1.0.3/glitter_sdk/core/gov/data.py
--rw-r--r--   0        0        0     6516 2023-09-03 07:54:13.318341 glitter_sdk-1.0.3/glitter_sdk/core/gov/msgs.py
--rw-r--r--   0        0        0     1695 2023-09-03 07:54:13.318999 glitter_sdk-1.0.3/glitter_sdk/core/gov/proposals.py
--rw-r--r--   0        0        0       47 2023-09-03 07:54:13.240105 glitter_sdk-1.0.3/glitter_sdk/core/ibc/__init__.py
--rw-r--r--   0        0        0      492 2023-09-03 07:54:13.248049 glitter_sdk-1.0.3/glitter_sdk/core/ibc/data/__init__.py
--rw-r--r--   0        0        0     4811 2023-09-03 07:54:13.246755 glitter_sdk-1.0.3/glitter_sdk/core/ibc/data/channel.py
--rw-r--r--   0        0        0     5323 2023-09-03 07:54:13.246122 glitter_sdk-1.0.3/glitter_sdk/core/ibc/data/client.py
--rw-r--r--   0        0        0     1407 2023-09-03 07:54:13.247476 glitter_sdk-1.0.3/glitter_sdk/core/ibc/data/commitment.py
--rw-r--r--   0        0        0     1947 2023-09-03 07:54:13.257072 glitter_sdk-1.0.3/glitter_sdk/core/ibc/data/connection.py
--rw-r--r--   0        0        0      944 2023-09-03 07:54:13.244510 glitter_sdk-1.0.3/glitter_sdk/core/ibc/msgs/__init__.py
--rw-r--r--   0        0        0    14728 2023-09-03 07:54:13.243958 glitter_sdk-1.0.3/glitter_sdk/core/ibc/msgs/channel.py
--rw-r--r--   0        0        0     5942 2023-09-03 07:54:13.243364 glitter_sdk-1.0.3/glitter_sdk/core/ibc/msgs/client.py
--rw-r--r--   0        0        0     9941 2023-09-03 07:54:13.245135 glitter_sdk-1.0.3/glitter_sdk/core/ibc/msgs/connection.py
--rw-r--r--   0        0        0       80 2023-09-03 07:54:13.258189 glitter_sdk-1.0.3/glitter_sdk/core/ibc/proposals/__init__.py
--rw-r--r--   0        0        0     2205 2023-09-03 07:54:13.263097 glitter_sdk-1.0.3/glitter_sdk/core/ibc/proposals/proposals.py
--rw-r--r--   0        0        0      100 2023-09-03 07:54:13.197656 glitter_sdk-1.0.3/glitter_sdk/core/ibc_transfer/__init__.py
--rw-r--r--   0        0        0      703 2023-09-03 07:54:13.198623 glitter_sdk-1.0.3/glitter_sdk/core/ibc_transfer/data.py
--rw-r--r--   0        0        0     3369 2023-09-03 07:54:13.198226 glitter_sdk-1.0.3/glitter_sdk/core/ibc_transfer/msgs.py
--rw-r--r--   0        0        0     3334 2023-09-03 07:54:13.292510 glitter_sdk-1.0.3/glitter_sdk/core/mode_info.py
--rw-r--r--   0        0        0      805 2023-09-03 07:54:13.306638 glitter_sdk-1.0.3/glitter_sdk/core/msg.py
--rw-r--r--   0        0        0      188 2023-09-03 07:54:13.265527 glitter_sdk-1.0.3/glitter_sdk/core/msgs/__init__.py
--rw-r--r--   0        0        0      813 2023-09-03 07:54:13.264216 glitter_sdk-1.0.3/glitter_sdk/core/msgs/argument.py
--rw-r--r--   0        0        0     1927 2023-09-03 07:54:13.264850 glitter_sdk-1.0.3/glitter_sdk/core/msgs/arguments.py
--rw-r--r--   0        0        0     2983 2023-09-03 07:54:13.274427 glitter_sdk-1.0.3/glitter_sdk/core/msgs/msgs.py
--rw-r--r--   0        0        0     2394 2023-09-03 07:54:13.194332 glitter_sdk-1.0.3/glitter_sdk/core/multisig.py
--rw-r--r--   0        0        0    11366 2023-09-03 07:54:13.291161 glitter_sdk-1.0.3/glitter_sdk/core/numeric.py
--rw-r--r--   0        0        0      114 2023-09-03 07:54:13.286028 glitter_sdk-1.0.3/glitter_sdk/core/params/__init__.py
--rw-r--r--   0        0        0     3325 2023-09-03 07:54:13.289824 glitter_sdk-1.0.3/glitter_sdk/core/params/proposals.py
--rw-r--r--   0        0        0    12728 2023-09-03 07:54:13.303735 glitter_sdk-1.0.3/glitter_sdk/core/public_key.py
--rw-r--r--   0        0        0     2621 2023-09-03 07:54:13.308657 glitter_sdk-1.0.3/glitter_sdk/core/sign_doc.py
--rw-r--r--   0        0        0     3550 2023-09-03 07:54:13.290523 glitter_sdk-1.0.3/glitter_sdk/core/signature_v2.py
--rw-r--r--   0        0        0       53 2023-09-03 07:54:13.305439 glitter_sdk-1.0.3/glitter_sdk/core/slashing/__init__.py
--rw-r--r--   0        0        0     1103 2023-09-03 07:54:13.306083 glitter_sdk-1.0.3/glitter_sdk/core/slashing/msgs.py
--rw-r--r--   0        0        0      661 2023-09-03 07:54:13.275069 glitter_sdk-1.0.3/glitter_sdk/core/staking/__init__.py
--rw-r--r--   0        0        0      429 2023-09-03 07:54:13.279862 glitter_sdk-1.0.3/glitter_sdk/core/staking/data/__init__.py
--rw-r--r--   0        0        0    11301 2023-09-03 07:54:13.285309 glitter_sdk-1.0.3/glitter_sdk/core/staking/data/delegation.py
--rw-r--r--   0        0        0     9625 2023-09-03 07:54:13.279283 glitter_sdk-1.0.3/glitter_sdk/core/staking/data/validator.py
--rw-r--r--   0        0        0    11092 2023-09-03 07:54:13.278610 glitter_sdk-1.0.3/glitter_sdk/core/staking/msgs.py
--rw-r--r--   0        0        0    15136 2023-09-03 07:54:13.307205 glitter_sdk-1.0.3/glitter_sdk/core/tx.py
--rw-r--r--   0        0        0      176 2023-09-03 07:54:13.151360 glitter_sdk-1.0.3/glitter_sdk/core/upgrade/__init__.py
--rw-r--r--   0        0        0      149 2023-09-03 07:54:13.155547 glitter_sdk-1.0.3/glitter_sdk/core/upgrade/data/__init__.py
--rw-r--r--   0        0        0     3330 2023-09-03 07:54:13.158732 glitter_sdk-1.0.3/glitter_sdk/core/upgrade/data/proposal.py
--rw-r--r--   0        0        0     2191 2023-09-03 07:54:13.150673 glitter_sdk-1.0.3/glitter_sdk/core/upgrade/plan.py
--rw-r--r--   0        0        0      315 2023-09-03 07:54:13.199336 glitter_sdk-1.0.3/glitter_sdk/core/wasm/__init__.py
--rw-r--r--   0        0        0     9320 2023-09-03 07:54:13.206497 glitter_sdk-1.0.3/glitter_sdk/core/wasm/data.py
--rw-r--r--   0        0        0    11303 2023-09-03 07:54:13.205440 glitter_sdk-1.0.3/glitter_sdk/core/wasm/msgs.py
--rw-r--r--   0        0        0    24195 2023-09-03 07:54:13.205957 glitter_sdk-1.0.3/glitter_sdk/core/wasm/proposals.py
--rw-r--r--   0        0        0    16112 2023-09-03 07:54:13.382295 glitter_sdk-1.0.3/glitter_sdk/driver.py
--rw-r--r--   0        0        0      968 2023-09-03 07:54:13.381896 glitter_sdk-1.0.3/glitter_sdk/exceptions.py
--rw-r--r--   0        0        0        0 2023-09-03 07:54:13.370079 glitter_sdk-1.0.3/glitter_sdk/key/__init__.py
--rw-r--r--   0        0        0     8381 2023-12-10 10:23:55.800668 glitter_sdk-1.0.3/glitter_sdk/key/key.py
--rw-r--r--   0        0        0     2371 2023-09-03 07:54:13.376633 glitter_sdk-1.0.3/glitter_sdk/key/mnemonic.py
--rw-r--r--   0        0        0     1846 2023-09-03 07:54:13.369060 glitter_sdk-1.0.3/glitter_sdk/key/raw.py
--rw-r--r--   0        0        0     3623 2023-09-03 07:54:13.369952 glitter_sdk-1.0.3/glitter_sdk/key/topub.py
--rw-r--r--   0        0        0     2406 2023-09-03 07:54:13.382768 glitter_sdk-1.0.3/glitter_sdk/pool.py
--rw-r--r--   0        0        0     3219 2023-09-03 07:54:13.367875 glitter_sdk-1.0.3/glitter_sdk/transport.py
--rw-r--r--   0        0        0        0 2023-09-03 07:54:13.331216 glitter_sdk-1.0.3/glitter_sdk/util/__init__.py
--rw-r--r--   0        0        0     1678 2023-09-03 07:54:13.367452 glitter_sdk-1.0.3/glitter_sdk/util/base.py
--rw-r--r--   0        0        0      878 2023-09-03 07:54:13.323603 glitter_sdk-1.0.3/glitter_sdk/util/constants/CLIENT.py
--rw-r--r--   0        0        0      679 2023-09-03 07:54:13.323026 glitter_sdk-1.0.3/glitter_sdk/util/constants/COMMAND.py
--rw-r--r--   0        0        0     1927 2023-09-03 07:54:13.329424 glitter_sdk-1.0.3/glitter_sdk/util/constants/CR.py
--rw-r--r--   0        0        0    12296 2023-09-03 07:54:13.328682 glitter_sdk-1.0.3/glitter_sdk/util/constants/ER.py
--rw-r--r--   0        0        0      370 2023-09-03 07:54:13.330491 glitter_sdk-1.0.3/glitter_sdk/util/constants/FIELD_TYPE.py
--rw-r--r--   0        0        0      214 2023-09-03 07:54:13.322530 glitter_sdk-1.0.3/glitter_sdk/util/constants/FLAG.py
--rw-r--r--   0        0        0      333 2023-09-03 07:54:13.330083 glitter_sdk-1.0.3/glitter_sdk/util/constants/SERVER_STATUS.py
--rw-r--r--   0        0        0        0 2023-09-03 07:54:13.323809 glitter_sdk-1.0.3/glitter_sdk/util/constants/__init__.py
--rw-r--r--   0        0        0     3253 2023-09-03 07:54:13.353785 glitter_sdk-1.0.3/glitter_sdk/util/contract.py
--rw-r--r--   0        0        0      199 2023-09-03 07:54:13.330984 glitter_sdk-1.0.3/glitter_sdk/util/converter.py
--rw-r--r--   0        0        0     1325 2023-09-03 07:54:13.362858 glitter_sdk-1.0.3/glitter_sdk/util/encrypt/__init__.py
--rw-r--r--   0        0        0     1386 2023-09-03 07:54:13.361222 glitter_sdk-1.0.3/glitter_sdk/util/encrypt/converter/__init__.py
--rw-r--r--   0        0        0     5017 2023-09-03 07:54:13.361009 glitter_sdk-1.0.3/glitter_sdk/util/encrypt/converter/bech32.py
--rw-r--r--   0        0        0      230 2023-09-03 07:54:13.356383 glitter_sdk-1.0.3/glitter_sdk/util/encrypt/crypto/__init__.py
--rw-r--r--   0        0        0      270 2023-09-03 07:54:13.360027 glitter_sdk-1.0.3/glitter_sdk/util/encrypt/crypto/ecdsa.py
--rw-r--r--   0        0        0     6072 2023-09-03 07:54:13.360522 glitter_sdk-1.0.3/glitter_sdk/util/encrypt/crypto/ecdsa_base.py
--rw-r--r--   0        0        0    14377 2023-09-03 07:54:13.355356 glitter_sdk-1.0.3/glitter_sdk/util/encrypt/crypto/ecdsa_openssl.py
--rw-r--r--   0        0        0    24914 2023-09-03 07:54:13.355925 glitter_sdk-1.0.3/glitter_sdk/util/encrypt/crypto/ecdsa_python.py
--rw-r--r--   0        0        0    17376 2023-09-03 07:54:13.354862 glitter_sdk-1.0.3/glitter_sdk/util/encrypt/crypto/openssl.py
--rw-r--r--   0        0        0     8962 2023-09-03 07:54:13.359592 glitter_sdk-1.0.3/glitter_sdk/util/encrypt/crypto/utils.py
--rw-r--r--   0        0        0        0 2023-09-03 07:54:13.363790 glitter_sdk-1.0.3/glitter_sdk/util/encrypt/eth/__init__.py
--rw-r--r--   0        0        0    55432 2023-12-12 12:39:21.810674 glitter_sdk-1.0.3/glitter_sdk/util/encrypt/eth/ethereum.py
--rw-r--r--   0        0        0      211 2023-09-03 07:54:13.350571 glitter_sdk-1.0.3/glitter_sdk/util/hash.py
--rw-r--r--   0        0        0      401 2024-03-22 13:35:11.141546 glitter_sdk-1.0.3/glitter_sdk/util/highlight.py
--rw-r--r--   0        0        0     1696 2023-09-03 07:54:13.366672 glitter_sdk-1.0.3/glitter_sdk/util/json.py
--rw-r--r--   0        0        0     1045 2023-09-03 07:54:13.367158 glitter_sdk-1.0.3/glitter_sdk/util/parse_authorization.py
--rw-r--r--   0        0        0     2550 2023-09-03 07:54:13.351695 glitter_sdk-1.0.3/glitter_sdk/util/parse_content.py
--rw-r--r--   0        0        0     3887 2023-09-03 07:54:13.352692 glitter_sdk-1.0.3/glitter_sdk/util/parse_msg.py
--rw-r--r--   0        0        0      732 2023-09-03 07:54:13.320976 glitter_sdk-1.0.3/glitter_sdk/util/parse_proto.py
--rw-r--r--   0        0        0     2950 2023-09-03 07:54:13.350164 glitter_sdk-1.0.3/glitter_sdk/util/parse_query_str.py
--rw-r--r--   0        0        0    14729 2023-12-12 12:45:01.366871 glitter_sdk-1.0.3/glitter_sdk/util/parse_sql.py
--rw-r--r--   0        0        0      294 2023-09-03 07:54:13.321619 glitter_sdk-1.0.3/glitter_sdk/util/remove_none.py
--rw-r--r--   0        0        0      133 2023-09-03 07:54:13.351084 glitter_sdk-1.0.3/glitter_sdk/util/url.py
--rw-r--r--   0        0        0     3404 2023-09-03 07:54:13.381386 glitter_sdk-1.0.3/glitter_sdk/utils.py
--rw-r--r--   0        0        0      765 2024-03-22 13:35:11.138774 glitter_sdk-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 glitter_sdk-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-09-03 07:54:13.137170 glitter_sdk-1.0.4/LICENSE
+-rw-r--r--   0        0        0       95 2023-09-03 07:54:13.138300 glitter_sdk-1.0.4/README.md
+-rw-r--r--   0        0        0       13 2023-09-03 07:54:13.380840 glitter_sdk-1.0.4/glitter_sdk/.gitignore
+-rw-r--r--   0        0        0      163 2023-09-03 07:54:13.368337 glitter_sdk-1.0.4/glitter_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-03 07:54:13.383129 glitter_sdk-1.0.4/glitter_sdk/client/__init__.py
+-rw-r--r--   0        0        0      196 2023-09-03 07:54:13.387634 glitter_sdk-1.0.4/glitter_sdk/client/lcd/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-03 07:54:13.398728 glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/__init__.py
+-rw-r--r--   0        0        0      812 2023-09-03 07:54:13.397064 glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/_base.py
+-rw-r--r--   0        0        0     1491 2024-04-06 11:02:33.246689 glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/auth.py
+-rw-r--r--   0        0        0     3436 2023-09-03 07:54:13.426154 glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/authz.py
+-rw-r--r--   0        0        0     2471 2023-09-03 07:54:13.399962 glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/bank.py
+-rw-r--r--   0        0        0     4394 2023-09-03 07:54:13.423967 glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/distribution.py
+-rw-r--r--   0        0        0     3632 2023-09-03 07:54:13.399297 glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/feegrant.py
+-rw-r--r--   0        0        0    10274 2023-09-03 07:54:13.426902 glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/gov.py
+-rw-r--r--   0        0        0      587 2023-09-03 07:54:13.400568 glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/ibc.py
+-rw-r--r--   0        0        0      762 2023-09-03 07:54:13.425645 glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/ibc_transfer.py
+-rw-r--r--   0        0        0     2330 2023-09-03 07:54:13.425202 glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/mint.py
+-rw-r--r--   0        0        0     3776 2023-09-03 07:54:13.424822 glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/slashing.py
+-rw-r--r--   0        0        0    13196 2023-09-03 07:54:13.397808 glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/staking.py
+-rw-r--r--   0        0        0     3065 2023-09-03 07:54:13.398507 glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/tendermint.py
+-rw-r--r--   0        0        0    14761 2023-09-03 07:54:13.426493 glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/tx.py
+-rw-r--r--   0        0        0     5011 2023-09-03 07:54:13.424466 glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/wasm.py
+-rw-r--r--   0        0        0      878 2023-09-03 07:54:13.387230 glitter_sdk-1.0.4/glitter_sdk/client/lcd/constants/CLIENT.py
+-rw-r--r--   0        0        0        0 2023-09-03 07:54:13.387350 glitter_sdk-1.0.4/glitter_sdk/client/lcd/constants/__init__.py
+-rw-r--r--   0        0        0    19291 2024-04-14 06:06:14.087021 glitter_sdk-1.0.4/glitter_sdk/client/lcd/db.py
+-rw-r--r--   0        0        0    11250 2023-09-03 07:54:13.385407 glitter_sdk-1.0.4/glitter_sdk/client/lcd/lcdclient.py
+-rw-r--r--   0        0        0     1803 2023-09-03 07:54:13.386589 glitter_sdk-1.0.4/glitter_sdk/client/lcd/lcdutils.py
+-rw-r--r--   0        0        0     2394 2023-09-03 07:54:13.386324 glitter_sdk-1.0.4/glitter_sdk/client/lcd/params.py
+-rw-r--r--   0        0        0     4901 2023-09-03 07:54:13.380244 glitter_sdk-1.0.4/glitter_sdk/connection.py
+-rw-r--r--   0        0        0      949 2024-04-06 11:02:33.248530 glitter_sdk-1.0.4/glitter_sdk/core/__init__.py
+-rw-r--r--   0        0        0      661 2024-04-06 11:02:33.249622 glitter_sdk-1.0.4/glitter_sdk/core/auth/__init__.py
+-rw-r--r--   0        0        0      656 2024-04-06 11:02:33.251581 glitter_sdk-1.0.4/glitter_sdk/core/auth/data/__init__.py
+-rw-r--r--   0        0        0     1835 2024-04-06 11:02:33.252163 glitter_sdk-1.0.4/glitter_sdk/core/auth/data/account.py
+-rw-r--r--   0        0        0     2953 2023-09-03 07:54:13.180040 glitter_sdk-1.0.4/glitter_sdk/core/auth/data/base_account.py
+-rw-r--r--   0        0        0     3965 2023-09-03 07:54:13.180496 glitter_sdk-1.0.4/glitter_sdk/core/auth/data/base_vesting_account.py
+-rw-r--r--   0        0        0     2731 2023-09-03 07:54:13.193175 glitter_sdk-1.0.4/glitter_sdk/core/auth/data/continuous_vesting_account.py
+-rw-r--r--   0        0        0     2498 2023-09-03 07:54:13.192420 glitter_sdk-1.0.4/glitter_sdk/core/auth/data/delayed_vesting_account.py
+-rw-r--r--   0        0        0     2340 2024-04-06 11:03:21.168125 glitter_sdk-1.0.4/glitter_sdk/core/auth/data/eth_account.py
+-rw-r--r--   0        0        0     4441 2023-09-03 07:54:13.179015 glitter_sdk-1.0.4/glitter_sdk/core/auth/data/periodic_vesting_account.py
+-rw-r--r--   0        0        0      331 2023-09-03 07:54:13.169621 glitter_sdk-1.0.4/glitter_sdk/core/auth/msgs/__init__.py
+-rw-r--r--   0        0        0     2921 2023-09-03 07:54:13.176777 glitter_sdk-1.0.4/glitter_sdk/core/auth/msgs/msg_create_periodic_vesting_account.py
+-rw-r--r--   0        0        0     2838 2023-09-03 07:54:13.177286 glitter_sdk-1.0.4/glitter_sdk/core/auth/msgs/msg_create_vesting_account.py
+-rw-r--r--   0        0        0     1620 2023-09-03 07:54:13.177856 glitter_sdk-1.0.4/glitter_sdk/core/auth/msgs/msg_donate_all_vesting_tokens.py
+-rw-r--r--   0        0        0      446 2023-09-03 07:54:13.294076 glitter_sdk-1.0.4/glitter_sdk/core/authz/__init__.py
+-rw-r--r--   0        0        0     9613 2023-09-03 07:54:13.302174 glitter_sdk-1.0.4/glitter_sdk/core/authz/data.py
+-rw-r--r--   0        0        0     6109 2023-09-03 07:54:13.301531 glitter_sdk-1.0.4/glitter_sdk/core/authz/msgs.py
+-rw-r--r--   0        0        0      149 2023-09-03 07:54:13.195011 glitter_sdk-1.0.4/glitter_sdk/core/bank/__init__.py
+-rw-r--r--   0        0        0     7099 2023-09-03 07:54:13.196914 glitter_sdk-1.0.4/glitter_sdk/core/bank/msgs.py
+-rw-r--r--   0        0        0     5009 2023-09-03 07:54:13.159260 glitter_sdk-1.0.4/glitter_sdk/core/bech32.py
+-rw-r--r--   0        0        0     1616 2023-09-03 07:54:13.302812 glitter_sdk-1.0.4/glitter_sdk/core/block.py
+-rw-r--r--   0        0        0     2724 2023-09-03 07:54:13.304464 glitter_sdk-1.0.4/glitter_sdk/core/broadcast.py
+-rw-r--r--   0        0        0     7746 2023-09-03 07:54:13.307900 glitter_sdk-1.0.4/glitter_sdk/core/coin.py
+-rw-r--r--   0        0        0     8360 2023-09-03 07:54:13.293168 glitter_sdk-1.0.4/glitter_sdk/core/coins.py
+-rw-r--r--   0        0        0     2707 2023-09-03 07:54:13.291864 glitter_sdk-1.0.4/glitter_sdk/core/compact_bit_array.py
+-rw-r--r--   0        0        0       71 2023-09-03 07:54:13.238361 glitter_sdk-1.0.4/glitter_sdk/core/crisis/__init__.py
+-rw-r--r--   0        0        0     2069 2023-09-03 07:54:13.238872 glitter_sdk-1.0.4/glitter_sdk/core/crisis/msgs.py
+-rw-r--r--   0        0        0     1085 2023-09-03 07:54:13.166080 glitter_sdk-1.0.4/glitter_sdk/core/deposit.py
+-rw-r--r--   0        0        0      371 2023-09-03 07:54:13.207165 glitter_sdk-1.0.4/glitter_sdk/core/distribution/__init__.py
+-rw-r--r--   0        0        0     6940 2023-09-03 07:54:13.212207 glitter_sdk-1.0.4/glitter_sdk/core/distribution/msgs.py
+-rw-r--r--   0        0        0     2692 2023-09-03 07:54:13.212710 glitter_sdk-1.0.4/glitter_sdk/core/distribution/proposals.py
+-rw-r--r--   0        0        0     2008 2023-09-03 07:54:13.239461 glitter_sdk-1.0.4/glitter_sdk/core/fee.py
+-rw-r--r--   0        0        0      297 2023-09-03 07:54:13.159943 glitter_sdk-1.0.4/glitter_sdk/core/feegrant/__init__.py
+-rw-r--r--   0        0        0     9141 2023-09-03 07:54:13.165604 glitter_sdk-1.0.4/glitter_sdk/core/feegrant/data.py
+-rw-r--r--   0        0        0     3178 2023-09-03 07:54:13.165112 glitter_sdk-1.0.4/glitter_sdk/core/feegrant/msgs.py
+-rw-r--r--   0        0        0      412 2023-09-03 07:54:13.309717 glitter_sdk-1.0.4/glitter_sdk/core/gov/__init__.py
+-rw-r--r--   0        0        0     6154 2023-09-03 07:54:13.319571 glitter_sdk-1.0.4/glitter_sdk/core/gov/data.py
+-rw-r--r--   0        0        0     6516 2023-09-03 07:54:13.318341 glitter_sdk-1.0.4/glitter_sdk/core/gov/msgs.py
+-rw-r--r--   0        0        0     1695 2023-09-03 07:54:13.318999 glitter_sdk-1.0.4/glitter_sdk/core/gov/proposals.py
+-rw-r--r--   0        0        0       47 2023-09-03 07:54:13.240105 glitter_sdk-1.0.4/glitter_sdk/core/ibc/__init__.py
+-rw-r--r--   0        0        0      492 2023-09-03 07:54:13.248049 glitter_sdk-1.0.4/glitter_sdk/core/ibc/data/__init__.py
+-rw-r--r--   0        0        0     4811 2023-09-03 07:54:13.246755 glitter_sdk-1.0.4/glitter_sdk/core/ibc/data/channel.py
+-rw-r--r--   0        0        0     5323 2023-09-03 07:54:13.246122 glitter_sdk-1.0.4/glitter_sdk/core/ibc/data/client.py
+-rw-r--r--   0        0        0     1407 2023-09-03 07:54:13.247476 glitter_sdk-1.0.4/glitter_sdk/core/ibc/data/commitment.py
+-rw-r--r--   0        0        0     1947 2023-09-03 07:54:13.257072 glitter_sdk-1.0.4/glitter_sdk/core/ibc/data/connection.py
+-rw-r--r--   0        0        0      944 2023-09-03 07:54:13.244510 glitter_sdk-1.0.4/glitter_sdk/core/ibc/msgs/__init__.py
+-rw-r--r--   0        0        0    14728 2023-09-03 07:54:13.243958 glitter_sdk-1.0.4/glitter_sdk/core/ibc/msgs/channel.py
+-rw-r--r--   0        0        0     5942 2023-09-03 07:54:13.243364 glitter_sdk-1.0.4/glitter_sdk/core/ibc/msgs/client.py
+-rw-r--r--   0        0        0     9941 2023-09-03 07:54:13.245135 glitter_sdk-1.0.4/glitter_sdk/core/ibc/msgs/connection.py
+-rw-r--r--   0        0        0       80 2023-09-03 07:54:13.258189 glitter_sdk-1.0.4/glitter_sdk/core/ibc/proposals/__init__.py
+-rw-r--r--   0        0        0     2205 2023-09-03 07:54:13.263097 glitter_sdk-1.0.4/glitter_sdk/core/ibc/proposals/proposals.py
+-rw-r--r--   0        0        0      100 2023-09-03 07:54:13.197656 glitter_sdk-1.0.4/glitter_sdk/core/ibc_transfer/__init__.py
+-rw-r--r--   0        0        0      703 2023-09-03 07:54:13.198623 glitter_sdk-1.0.4/glitter_sdk/core/ibc_transfer/data.py
+-rw-r--r--   0        0        0     3369 2023-09-03 07:54:13.198226 glitter_sdk-1.0.4/glitter_sdk/core/ibc_transfer/msgs.py
+-rw-r--r--   0        0        0     3334 2023-09-03 07:54:13.292510 glitter_sdk-1.0.4/glitter_sdk/core/mode_info.py
+-rw-r--r--   0        0        0      805 2023-09-03 07:54:13.306638 glitter_sdk-1.0.4/glitter_sdk/core/msg.py
+-rw-r--r--   0        0        0      188 2023-09-03 07:54:13.265527 glitter_sdk-1.0.4/glitter_sdk/core/msgs/__init__.py
+-rw-r--r--   0        0        0      813 2023-09-03 07:54:13.264216 glitter_sdk-1.0.4/glitter_sdk/core/msgs/argument.py
+-rw-r--r--   0        0        0     1927 2023-09-03 07:54:13.264850 glitter_sdk-1.0.4/glitter_sdk/core/msgs/arguments.py
+-rw-r--r--   0        0        0     2983 2023-09-03 07:54:13.274427 glitter_sdk-1.0.4/glitter_sdk/core/msgs/msgs.py
+-rw-r--r--   0        0        0     2394 2023-09-03 07:54:13.194332 glitter_sdk-1.0.4/glitter_sdk/core/multisig.py
+-rw-r--r--   0        0        0    11366 2023-09-03 07:54:13.291161 glitter_sdk-1.0.4/glitter_sdk/core/numeric.py
+-rw-r--r--   0        0        0      114 2023-09-03 07:54:13.286028 glitter_sdk-1.0.4/glitter_sdk/core/params/__init__.py
+-rw-r--r--   0        0        0     3325 2023-09-03 07:54:13.289824 glitter_sdk-1.0.4/glitter_sdk/core/params/proposals.py
+-rw-r--r--   0        0        0    12728 2024-04-06 11:02:33.255276 glitter_sdk-1.0.4/glitter_sdk/core/public_key.py
+-rw-r--r--   0        0        0     2621 2023-09-03 07:54:13.308657 glitter_sdk-1.0.4/glitter_sdk/core/sign_doc.py
+-rw-r--r--   0        0        0     3550 2023-09-03 07:54:13.290523 glitter_sdk-1.0.4/glitter_sdk/core/signature_v2.py
+-rw-r--r--   0        0        0       53 2023-09-03 07:54:13.305439 glitter_sdk-1.0.4/glitter_sdk/core/slashing/__init__.py
+-rw-r--r--   0        0        0     1103 2023-09-03 07:54:13.306083 glitter_sdk-1.0.4/glitter_sdk/core/slashing/msgs.py
+-rw-r--r--   0        0        0      661 2023-09-03 07:54:13.275069 glitter_sdk-1.0.4/glitter_sdk/core/staking/__init__.py
+-rw-r--r--   0        0        0      429 2023-09-03 07:54:13.279862 glitter_sdk-1.0.4/glitter_sdk/core/staking/data/__init__.py
+-rw-r--r--   0        0        0    11301 2023-09-03 07:54:13.285309 glitter_sdk-1.0.4/glitter_sdk/core/staking/data/delegation.py
+-rw-r--r--   0        0        0     9625 2023-09-03 07:54:13.279283 glitter_sdk-1.0.4/glitter_sdk/core/staking/data/validator.py
+-rw-r--r--   0        0        0    11092 2023-09-03 07:54:13.278610 glitter_sdk-1.0.4/glitter_sdk/core/staking/msgs.py
+-rw-r--r--   0        0        0    15136 2023-09-03 07:54:13.307205 glitter_sdk-1.0.4/glitter_sdk/core/tx.py
+-rw-r--r--   0        0        0      176 2023-09-03 07:54:13.151360 glitter_sdk-1.0.4/glitter_sdk/core/upgrade/__init__.py
+-rw-r--r--   0        0        0      149 2023-09-03 07:54:13.155547 glitter_sdk-1.0.4/glitter_sdk/core/upgrade/data/__init__.py
+-rw-r--r--   0        0        0     3330 2023-09-03 07:54:13.158732 glitter_sdk-1.0.4/glitter_sdk/core/upgrade/data/proposal.py
+-rw-r--r--   0        0        0     2191 2023-09-03 07:54:13.150673 glitter_sdk-1.0.4/glitter_sdk/core/upgrade/plan.py
+-rw-r--r--   0        0        0      315 2023-09-03 07:54:13.199336 glitter_sdk-1.0.4/glitter_sdk/core/wasm/__init__.py
+-rw-r--r--   0        0        0     9320 2023-09-03 07:54:13.206497 glitter_sdk-1.0.4/glitter_sdk/core/wasm/data.py
+-rw-r--r--   0        0        0    11303 2023-09-03 07:54:13.205440 glitter_sdk-1.0.4/glitter_sdk/core/wasm/msgs.py
+-rw-r--r--   0        0        0    24195 2023-09-03 07:54:13.205957 glitter_sdk-1.0.4/glitter_sdk/core/wasm/proposals.py
+-rw-r--r--   0        0        0    16112 2023-09-03 07:54:13.382295 glitter_sdk-1.0.4/glitter_sdk/driver.py
+-rw-r--r--   0        0        0      968 2023-09-03 07:54:13.381896 glitter_sdk-1.0.4/glitter_sdk/exceptions.py
+-rw-r--r--   0        0        0        0 2023-09-03 07:54:13.370079 glitter_sdk-1.0.4/glitter_sdk/key/__init__.py
+-rw-r--r--   0        0        0     8381 2023-12-10 10:23:55.800668 glitter_sdk-1.0.4/glitter_sdk/key/key.py
+-rw-r--r--   0        0        0     2371 2023-09-03 07:54:13.376633 glitter_sdk-1.0.4/glitter_sdk/key/mnemonic.py
+-rw-r--r--   0        0        0     1846 2024-04-06 11:02:33.256157 glitter_sdk-1.0.4/glitter_sdk/key/raw.py
+-rw-r--r--   0        0        0     3623 2023-09-03 07:54:13.369952 glitter_sdk-1.0.4/glitter_sdk/key/topub.py
+-rw-r--r--   0        0        0     2406 2023-09-03 07:54:13.382768 glitter_sdk-1.0.4/glitter_sdk/pool.py
+-rw-r--r--   0        0        0     3219 2023-09-03 07:54:13.367875 glitter_sdk-1.0.4/glitter_sdk/transport.py
+-rw-r--r--   0        0        0        0 2023-09-03 07:54:13.331216 glitter_sdk-1.0.4/glitter_sdk/util/__init__.py
+-rw-r--r--   0        0        0     1678 2023-09-03 07:54:13.367452 glitter_sdk-1.0.4/glitter_sdk/util/base.py
+-rw-r--r--   0        0        0      878 2023-09-03 07:54:13.323603 glitter_sdk-1.0.4/glitter_sdk/util/constants/CLIENT.py
+-rw-r--r--   0        0        0      679 2023-09-03 07:54:13.323026 glitter_sdk-1.0.4/glitter_sdk/util/constants/COMMAND.py
+-rw-r--r--   0        0        0     1927 2023-09-03 07:54:13.329424 glitter_sdk-1.0.4/glitter_sdk/util/constants/CR.py
+-rw-r--r--   0        0        0    12296 2023-09-03 07:54:13.328682 glitter_sdk-1.0.4/glitter_sdk/util/constants/ER.py
+-rw-r--r--   0        0        0      370 2023-09-03 07:54:13.330491 glitter_sdk-1.0.4/glitter_sdk/util/constants/FIELD_TYPE.py
+-rw-r--r--   0        0        0      214 2023-09-03 07:54:13.322530 glitter_sdk-1.0.4/glitter_sdk/util/constants/FLAG.py
+-rw-r--r--   0        0        0      333 2023-09-03 07:54:13.330083 glitter_sdk-1.0.4/glitter_sdk/util/constants/SERVER_STATUS.py
+-rw-r--r--   0        0        0        0 2023-09-03 07:54:13.323809 glitter_sdk-1.0.4/glitter_sdk/util/constants/__init__.py
+-rw-r--r--   0        0        0     3253 2023-09-03 07:54:13.353785 glitter_sdk-1.0.4/glitter_sdk/util/contract.py
+-rw-r--r--   0        0        0      199 2023-09-03 07:54:13.330984 glitter_sdk-1.0.4/glitter_sdk/util/converter.py
+-rw-r--r--   0        0        0     1325 2023-09-03 07:54:13.362858 glitter_sdk-1.0.4/glitter_sdk/util/encrypt/__init__.py
+-rw-r--r--   0        0        0     1386 2023-09-03 07:54:13.361222 glitter_sdk-1.0.4/glitter_sdk/util/encrypt/converter/__init__.py
+-rw-r--r--   0        0        0     5017 2023-09-03 07:54:13.361009 glitter_sdk-1.0.4/glitter_sdk/util/encrypt/converter/bech32.py
+-rw-r--r--   0        0        0      230 2023-09-03 07:54:13.356383 glitter_sdk-1.0.4/glitter_sdk/util/encrypt/crypto/__init__.py
+-rw-r--r--   0        0        0      270 2023-09-03 07:54:13.360027 glitter_sdk-1.0.4/glitter_sdk/util/encrypt/crypto/ecdsa.py
+-rw-r--r--   0        0        0     6072 2023-09-03 07:54:13.360522 glitter_sdk-1.0.4/glitter_sdk/util/encrypt/crypto/ecdsa_base.py
+-rw-r--r--   0        0        0    14377 2023-09-03 07:54:13.355356 glitter_sdk-1.0.4/glitter_sdk/util/encrypt/crypto/ecdsa_openssl.py
+-rw-r--r--   0        0        0    24914 2023-09-03 07:54:13.355925 glitter_sdk-1.0.4/glitter_sdk/util/encrypt/crypto/ecdsa_python.py
+-rw-r--r--   0        0        0    17376 2023-09-03 07:54:13.354862 glitter_sdk-1.0.4/glitter_sdk/util/encrypt/crypto/openssl.py
+-rw-r--r--   0        0        0     8962 2023-09-03 07:54:13.359592 glitter_sdk-1.0.4/glitter_sdk/util/encrypt/crypto/utils.py
+-rw-r--r--   0        0        0        0 2023-09-03 07:54:13.363790 glitter_sdk-1.0.4/glitter_sdk/util/encrypt/eth/__init__.py
+-rw-r--r--   0        0        0    55432 2023-12-12 12:39:21.810674 glitter_sdk-1.0.4/glitter_sdk/util/encrypt/eth/ethereum.py
+-rw-r--r--   0        0        0      211 2023-09-03 07:54:13.350571 glitter_sdk-1.0.4/glitter_sdk/util/hash.py
+-rw-r--r--   0        0        0      401 2024-03-22 13:35:11.141546 glitter_sdk-1.0.4/glitter_sdk/util/highlight.py
+-rw-r--r--   0        0        0     1696 2023-09-03 07:54:13.366672 glitter_sdk-1.0.4/glitter_sdk/util/json.py
+-rw-r--r--   0        0        0     1045 2023-09-03 07:54:13.367158 glitter_sdk-1.0.4/glitter_sdk/util/parse_authorization.py
+-rw-r--r--   0        0        0     2550 2023-09-03 07:54:13.351695 glitter_sdk-1.0.4/glitter_sdk/util/parse_content.py
+-rw-r--r--   0        0        0     3887 2023-09-03 07:54:13.352692 glitter_sdk-1.0.4/glitter_sdk/util/parse_msg.py
+-rw-r--r--   0        0        0      732 2023-09-03 07:54:13.320976 glitter_sdk-1.0.4/glitter_sdk/util/parse_proto.py
+-rw-r--r--   0        0        0     2950 2023-09-03 07:54:13.350164 glitter_sdk-1.0.4/glitter_sdk/util/parse_query_str.py
+-rw-r--r--   0        0        0    14729 2023-12-12 12:45:01.366871 glitter_sdk-1.0.4/glitter_sdk/util/parse_sql.py
+-rw-r--r--   0        0        0      294 2023-09-03 07:54:13.321619 glitter_sdk-1.0.4/glitter_sdk/util/remove_none.py
+-rw-r--r--   0        0        0      133 2023-09-03 07:54:13.351084 glitter_sdk-1.0.4/glitter_sdk/util/url.py
+-rw-r--r--   0        0        0     3404 2023-09-03 07:54:13.381386 glitter_sdk-1.0.4/glitter_sdk/utils.py
+-rw-r--r--   0        0        0      764 2024-04-30 09:01:35.420243 glitter_sdk-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 glitter_sdk-1.0.4/PKG-INFO
```

### Comparing `glitter_sdk-1.0.3/LICENSE` & `glitter_sdk-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/_base.py` & `glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/_base.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/auth.py` & `glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/auth.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/authz.py` & `glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/authz.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/bank.py` & `glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/bank.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/distribution.py` & `glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/distribution.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/feegrant.py` & `glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/feegrant.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/gov.py` & `glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/gov.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/ibc.py` & `glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/ibc.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/ibc_transfer.py` & `glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/ibc_transfer.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/mint.py` & `glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/mint.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/slashing.py` & `glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/slashing.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/staking.py` & `glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/staking.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/tendermint.py` & `glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/tendermint.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/tx.py` & `glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/tx.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/client/lcd/api/wasm.py` & `glitter_sdk-1.0.4/glitter_sdk/client/lcd/api/wasm.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/client/lcd/constants/CLIENT.py` & `glitter_sdk-1.0.4/glitter_sdk/client/lcd/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/client/lcd/db.py` & `glitter_sdk-1.0.4/glitter_sdk/client/lcd/db.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/client/lcd/lcdclient.py` & `glitter_sdk-1.0.4/glitter_sdk/client/lcd/lcdclient.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/client/lcd/lcdutils.py` & `glitter_sdk-1.0.4/glitter_sdk/client/lcd/lcdutils.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/client/lcd/params.py` & `glitter_sdk-1.0.4/glitter_sdk/client/lcd/params.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/connection.py` & `glitter_sdk-1.0.4/glitter_sdk/connection.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/__init__.py` & `glitter_sdk-1.0.4/glitter_sdk/core/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/auth/__init__.py` & `glitter_sdk-1.0.4/glitter_sdk/core/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/auth/data/__init__.py` & `glitter_sdk-1.0.4/glitter_sdk/core/auth/data/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/auth/data/account.py` & `glitter_sdk-1.0.4/glitter_sdk/core/auth/data/account.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/auth/data/base_account.py` & `glitter_sdk-1.0.4/glitter_sdk/core/auth/data/base_account.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/auth/data/base_vesting_account.py` & `glitter_sdk-1.0.4/glitter_sdk/core/auth/data/base_vesting_account.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/auth/data/continuous_vesting_account.py` & `glitter_sdk-1.0.4/glitter_sdk/core/auth/data/continuous_vesting_account.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/auth/data/delayed_vesting_account.py` & `glitter_sdk-1.0.4/glitter_sdk/core/auth/data/delayed_vesting_account.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/auth/data/eth_account.py` & `glitter_sdk-1.0.4/glitter_sdk/core/auth/data/eth_account.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/auth/data/periodic_vesting_account.py` & `glitter_sdk-1.0.4/glitter_sdk/core/auth/data/periodic_vesting_account.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/auth/msgs/msg_create_periodic_vesting_account.py` & `glitter_sdk-1.0.4/glitter_sdk/core/auth/msgs/msg_create_periodic_vesting_account.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/auth/msgs/msg_create_vesting_account.py` & `glitter_sdk-1.0.4/glitter_sdk/core/auth/msgs/msg_create_vesting_account.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/auth/msgs/msg_donate_all_vesting_tokens.py` & `glitter_sdk-1.0.4/glitter_sdk/core/auth/msgs/msg_donate_all_vesting_tokens.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/authz/data.py` & `glitter_sdk-1.0.4/glitter_sdk/core/authz/data.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/authz/msgs.py` & `glitter_sdk-1.0.4/glitter_sdk/core/authz/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/bank/msgs.py` & `glitter_sdk-1.0.4/glitter_sdk/core/bank/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/bech32.py` & `glitter_sdk-1.0.4/glitter_sdk/core/bech32.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/block.py` & `glitter_sdk-1.0.4/glitter_sdk/core/block.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/broadcast.py` & `glitter_sdk-1.0.4/glitter_sdk/core/broadcast.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/coin.py` & `glitter_sdk-1.0.4/glitter_sdk/core/coin.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/coins.py` & `glitter_sdk-1.0.4/glitter_sdk/core/coins.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/compact_bit_array.py` & `glitter_sdk-1.0.4/glitter_sdk/core/compact_bit_array.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/crisis/msgs.py` & `glitter_sdk-1.0.4/glitter_sdk/core/crisis/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/deposit.py` & `glitter_sdk-1.0.4/glitter_sdk/core/deposit.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/distribution/msgs.py` & `glitter_sdk-1.0.4/glitter_sdk/core/distribution/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/distribution/proposals.py` & `glitter_sdk-1.0.4/glitter_sdk/core/distribution/proposals.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/fee.py` & `glitter_sdk-1.0.4/glitter_sdk/core/fee.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/feegrant/data.py` & `glitter_sdk-1.0.4/glitter_sdk/core/feegrant/data.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/feegrant/msgs.py` & `glitter_sdk-1.0.4/glitter_sdk/core/feegrant/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/gov/data.py` & `glitter_sdk-1.0.4/glitter_sdk/core/gov/data.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/gov/msgs.py` & `glitter_sdk-1.0.4/glitter_sdk/core/gov/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/gov/proposals.py` & `glitter_sdk-1.0.4/glitter_sdk/core/gov/proposals.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/ibc/data/channel.py` & `glitter_sdk-1.0.4/glitter_sdk/core/ibc/data/channel.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/ibc/data/client.py` & `glitter_sdk-1.0.4/glitter_sdk/core/ibc/data/client.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/ibc/data/commitment.py` & `glitter_sdk-1.0.4/glitter_sdk/core/ibc/data/commitment.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/ibc/data/connection.py` & `glitter_sdk-1.0.4/glitter_sdk/core/ibc/data/connection.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/ibc/msgs/__init__.py` & `glitter_sdk-1.0.4/glitter_sdk/core/ibc/msgs/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/ibc/msgs/channel.py` & `glitter_sdk-1.0.4/glitter_sdk/core/ibc/msgs/channel.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/ibc/msgs/client.py` & `glitter_sdk-1.0.4/glitter_sdk/core/ibc/msgs/client.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/ibc/msgs/connection.py` & `glitter_sdk-1.0.4/glitter_sdk/core/ibc/msgs/connection.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/ibc/proposals/proposals.py` & `glitter_sdk-1.0.4/glitter_sdk/core/ibc/proposals/proposals.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/ibc_transfer/data.py` & `glitter_sdk-1.0.4/glitter_sdk/core/ibc_transfer/data.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/ibc_transfer/msgs.py` & `glitter_sdk-1.0.4/glitter_sdk/core/ibc_transfer/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/mode_info.py` & `glitter_sdk-1.0.4/glitter_sdk/core/mode_info.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/msg.py` & `glitter_sdk-1.0.4/glitter_sdk/core/msg.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/msgs/argument.py` & `glitter_sdk-1.0.4/glitter_sdk/core/msgs/argument.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/msgs/arguments.py` & `glitter_sdk-1.0.4/glitter_sdk/core/msgs/arguments.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/msgs/msgs.py` & `glitter_sdk-1.0.4/glitter_sdk/core/msgs/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/multisig.py` & `glitter_sdk-1.0.4/glitter_sdk/core/multisig.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/numeric.py` & `glitter_sdk-1.0.4/glitter_sdk/core/numeric.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/params/proposals.py` & `glitter_sdk-1.0.4/glitter_sdk/core/params/proposals.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/public_key.py` & `glitter_sdk-1.0.4/glitter_sdk/core/public_key.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/sign_doc.py` & `glitter_sdk-1.0.4/glitter_sdk/core/sign_doc.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/signature_v2.py` & `glitter_sdk-1.0.4/glitter_sdk/core/signature_v2.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/slashing/msgs.py` & `glitter_sdk-1.0.4/glitter_sdk/core/slashing/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/staking/__init__.py` & `glitter_sdk-1.0.4/glitter_sdk/core/staking/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/staking/data/delegation.py` & `glitter_sdk-1.0.4/glitter_sdk/core/staking/data/delegation.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/staking/data/validator.py` & `glitter_sdk-1.0.4/glitter_sdk/core/staking/data/validator.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/staking/msgs.py` & `glitter_sdk-1.0.4/glitter_sdk/core/staking/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/tx.py` & `glitter_sdk-1.0.4/glitter_sdk/core/tx.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/upgrade/data/proposal.py` & `glitter_sdk-1.0.4/glitter_sdk/core/upgrade/data/proposal.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/upgrade/plan.py` & `glitter_sdk-1.0.4/glitter_sdk/core/upgrade/plan.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/wasm/data.py` & `glitter_sdk-1.0.4/glitter_sdk/core/wasm/data.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/wasm/msgs.py` & `glitter_sdk-1.0.4/glitter_sdk/core/wasm/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/core/wasm/proposals.py` & `glitter_sdk-1.0.4/glitter_sdk/core/wasm/proposals.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/driver.py` & `glitter_sdk-1.0.4/glitter_sdk/driver.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/exceptions.py` & `glitter_sdk-1.0.4/glitter_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/key/key.py` & `glitter_sdk-1.0.4/glitter_sdk/key/key.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/key/mnemonic.py` & `glitter_sdk-1.0.4/glitter_sdk/key/mnemonic.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/key/raw.py` & `glitter_sdk-1.0.4/glitter_sdk/key/raw.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/key/topub.py` & `glitter_sdk-1.0.4/glitter_sdk/key/topub.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/pool.py` & `glitter_sdk-1.0.4/glitter_sdk/pool.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/transport.py` & `glitter_sdk-1.0.4/glitter_sdk/transport.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/base.py` & `glitter_sdk-1.0.4/glitter_sdk/util/base.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/constants/CLIENT.py` & `glitter_sdk-1.0.4/glitter_sdk/util/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/constants/COMMAND.py` & `glitter_sdk-1.0.4/glitter_sdk/util/constants/COMMAND.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/constants/CR.py` & `glitter_sdk-1.0.4/glitter_sdk/util/constants/CR.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/constants/ER.py` & `glitter_sdk-1.0.4/glitter_sdk/util/constants/ER.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/contract.py` & `glitter_sdk-1.0.4/glitter_sdk/util/contract.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/encrypt/__init__.py` & `glitter_sdk-1.0.4/glitter_sdk/util/encrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/encrypt/converter/__init__.py` & `glitter_sdk-1.0.4/glitter_sdk/util/encrypt/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/encrypt/converter/bech32.py` & `glitter_sdk-1.0.4/glitter_sdk/util/encrypt/converter/bech32.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/encrypt/crypto/ecdsa_base.py` & `glitter_sdk-1.0.4/glitter_sdk/util/encrypt/crypto/ecdsa_base.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/encrypt/crypto/ecdsa_openssl.py` & `glitter_sdk-1.0.4/glitter_sdk/util/encrypt/crypto/ecdsa_openssl.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/encrypt/crypto/ecdsa_python.py` & `glitter_sdk-1.0.4/glitter_sdk/util/encrypt/crypto/ecdsa_python.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/encrypt/crypto/openssl.py` & `glitter_sdk-1.0.4/glitter_sdk/util/encrypt/crypto/openssl.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/encrypt/crypto/utils.py` & `glitter_sdk-1.0.4/glitter_sdk/util/encrypt/crypto/utils.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/encrypt/eth/ethereum.py` & `glitter_sdk-1.0.4/glitter_sdk/util/encrypt/eth/ethereum.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/json.py` & `glitter_sdk-1.0.4/glitter_sdk/util/json.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/parse_authorization.py` & `glitter_sdk-1.0.4/glitter_sdk/util/parse_authorization.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/parse_content.py` & `glitter_sdk-1.0.4/glitter_sdk/util/parse_content.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/parse_msg.py` & `glitter_sdk-1.0.4/glitter_sdk/util/parse_msg.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/parse_proto.py` & `glitter_sdk-1.0.4/glitter_sdk/util/parse_proto.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/parse_query_str.py` & `glitter_sdk-1.0.4/glitter_sdk/util/parse_query_str.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/util/parse_sql.py` & `glitter_sdk-1.0.4/glitter_sdk/util/parse_sql.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/glitter_sdk/utils.py` & `glitter_sdk-1.0.4/glitter_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-1.0.3/pyproject.toml` & `glitter_sdk-1.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glitter-sdk"
-version = "1.0.3"
+version = "1.0.4"
 description='Glitter Protocol is a blockchain based database and index engine for developing and hosting web3 applications in decentralized storage networks.'
 authors = ["Glitter Protocol <ted@glitterprotocol.io>"]
 readme = "README.md"
 packages = [{include = "glitter_sdk"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -15,16 +15,16 @@
 furl = "^2.1.3"
 wrapt = "^1.15.0"
 bip32utils = "^0.3.post4"
 mnemonic = "^0.20"
 attrs = "^22.2.0"
 attr = "^0.3.2"
 betterproto = "2.0.0b4"
-coincurve = "^18.0.0"
 base58 = "^2.1.1"
 pycryptodomex = "^3.17"
 glitter-proto = "^0.4.0"
+coincurve = "19.0.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `glitter_sdk-1.0.3/PKG-INFO` & `glitter_sdk-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glitter-sdk
-Version: 1.0.3
+Version: 1.0.4
 Summary: Glitter Protocol is a blockchain based database and index engine for developing and hosting web3 applications in decentralized storage networks.
 Author: Glitter Protocol
 Author-email: ted@glitterprotocol.io
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,15 +15,15 @@
 Requires-Dist: attr (>=0.3.2,<0.4.0)
 Requires-Dist: attrs (>=22.2.0,<23.0.0)
 Requires-Dist: base58 (>=2.1.1,<3.0.0)
 Requires-Dist: bech32 (>=1.2.0,<2.0.0)
 Requires-Dist: betterproto (==2.0.0b4)
 Requires-Dist: bip32utils (>=0.3.post4,<0.4)
 Requires-Dist: boltons (>=23.0.0,<24.0.0)
-Requires-Dist: coincurve (>=18.0.0,<19.0.0)
+Requires-Dist: coincurve (==19.0.1)
 Requires-Dist: furl (>=2.1.3,<3.0.0)
 Requires-Dist: glitter-proto (>=0.4.0,<0.5.0)
 Requires-Dist: mnemonic (>=0.20,<0.21)
 Requires-Dist: nest-asyncio (>=1.5.6,<2.0.0)
 Requires-Dist: pycryptodomex (>=3.17,<4.0)
 Requires-Dist: wrapt (>=1.15.0,<2.0.0)
 Description-Content-Type: text/markdown
```

