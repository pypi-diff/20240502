# Comparing `tmp/securesystemslib-0.31.0.tar.gz` & `tmp/securesystemslib-1.0.0.tar.gz`

## Comparing `securesystemslib-0.31.0.tar` & `securesystemslib-1.0.0.tar`

### file list

```diff
@@ -1,142 +1,116 @@
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/.coveragerc
--rw-r--r--   0        0        0    17652 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/CHANGELOG.md
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/mypy.ini
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/pylintrc
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/requirements-build.txt
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/requirements-dev.txt
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/requirements-docs.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/requirements-kms.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/requirements-lint.txt
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/requirements-pinned.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/requirements-sigstore.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/requirements-test.txt
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/requirements.txt
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tox.ini
--rwxr-xr-x   0        0        0      824 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/__init__.py
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/dsse.py
--rwxr-xr-x   0        0        0    17697 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/ecdsa_keys.py
--rwxr-xr-x   0        0        0    13303 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/ed25519_keys.py
--rwxr-xr-x   0        0        0     3404 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/exceptions.py
--rwxr-xr-x   0        0        0    24735 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/formats.py
--rwxr-xr-x   0        0        0    13945 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/hash.py
--rw-r--r--   0        0        0    39124 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/interface.py
--rwxr-xr-x   0        0        0    67917 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/keys.py
--rwxr-xr-x   0        0        0    44340 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/rsa_keys.py
--rwxr-xr-x   0        0        0    32194 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/schema.py
--rwxr-xr-x   0        0        0     1317 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/settings.py
--rw-r--r--   0        0        0     9911 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/storage.py
--rwxr-xr-x   0        0        0     4182 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/unittest_toolbox.py
--rw-r--r--   0        0        0    14050 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/util.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/_internal/utils.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/_vendor/README.md
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/_vendor/__init__.py
--rwxr-xr-x   0        0        0     1026 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/_vendor/test-ed25519-upstream.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/_vendor/ed25519/.gitignore
--rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/_vendor/ed25519/LICENSE
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/_vendor/ed25519/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/_vendor/ed25519/__init__.py
--rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/_vendor/ed25519/ed25519.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/_vendor/ed25519/science.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/_vendor/ed25519/test_ed25519.py
--rw-r--r--   0        0        0  2427904 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/_vendor/ed25519/test_data/ed25519
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/gpg/__init__.py
--rw-r--r--   0        0        0    35971 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/gpg/common.py
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/gpg/constants.py
--rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/gpg/dsa.py
--rw-r--r--   0        0        0     7647 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/gpg/eddsa.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/gpg/exceptions.py
--rw-r--r--   0        0        0    11954 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/gpg/functions.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/gpg/handlers.py
--rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/gpg/rsa.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/gpg/util.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/signer/__init__.py
--rw-r--r--   0        0        0     8319 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/signer/_aws_signer.py
--rw-r--r--   0        0        0     9761 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/signer/_azure_signer.py
--rw-r--r--   0        0        0    10717 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/signer/_crypto_signer.py
--rw-r--r--   0        0        0     7474 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/signer/_gcp_signer.py
--rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/signer/_gpg_signer.py
--rw-r--r--   0        0        0    13352 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/signer/_hsm_signer.py
--rw-r--r--   0        0        0    14970 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/signer/_key.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/signer/_signature.py
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/signer/_signer.py
--rw-r--r--   0        0        0     9410 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/signer/_sigstore_signer.py
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/signer/_spx_signer.py
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/signer/_sslib_signer.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/securesystemslib/signer/_utils.py
--rwxr-xr-x   0        0        0      333 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/__init__.py
--rwxr-xr-x   0        0        0      706 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/aggregate_tests.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/check_aws_signer.py
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/check_azure_signer.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/check_gpg_available.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/check_kms_signers.py
--rw-r--r--   0        0        0    17578 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/check_public_interfaces.py
--rw-r--r--   0        0        0     8395 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/check_public_interfaces_gpg.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/check_sigstore_signer.py
--rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/test_dsse.py
--rwxr-xr-x   0        0        0     7324 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/test_ecdsa_keys.py
--rwxr-xr-x   0        0        0     5758 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/test_ed25519_keys.py
--rwxr-xr-x   0        0        0     1291 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/test_exceptions.py
--rwxr-xr-x   0        0        0    14102 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/test_formats.py
--rw-r--r--   0        0        0    36690 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/test_gpg.py
--rwxr-xr-x   0        0        0    11694 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/test_hash.py
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/test_hsm_signer.py
--rwxr-xr-x   0        0        0    39239 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/test_interface.py
--rwxr-xr-x   0        0        0    32332 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/test_keys.py
--rw-r--r--   0        0        0     5077 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/test_migrate_key.py
--rwxr-xr-x   0        0        0    14742 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/test_rsa_keys.py
--rwxr-xr-x   0        0        0    17816 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/test_schema.py
--rw-r--r--   0        0        0    37865 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/test_signer.py
--rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/test_storage.py
--rw-r--r--   0        0        0    14260 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/test_util.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/keystore/ecdsa_key
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/keystore/ecdsa_key.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/keystore/ed25519_key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/keystore/ed25519_key.pub
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/keystore/no_key
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/keystore/rsa_key
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/keystore/rsa_key.pub
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/legacy/ecdsa_private_encrypted
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/legacy/ecdsa_private_unencrypted
--rwxr-xr-x   0        0        0      307 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/legacy/ecdsa_public
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/legacy/ed25519_private_encrypted
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/legacy/ed25519_private_unencrypted
--rwxr-xr-x   0        0        0      181 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/legacy/ed25519_public
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/legacy/rsa_private_encrypted
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/legacy/rsa_private_unencrypted
--rwxr-xr-x   0        0        0      625 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/legacy/rsa_public
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/pems/ecdsa_private.pem
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/pems/ecdsa_private_encrypted.pem
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/pems/ecdsa_public.pem
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/pems/ed25519_private.pem
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/pems/ed25519_private_encrypted.pem
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/pems/ed25519_public.pem
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/pems/rsa_private.pem
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/pems/rsa_private_encrypted.pem
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/data/pems/rsa_public.pem
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.pem
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/dsa/pubring.gpg
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/dsa/random_seed
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/dsa/secring.gpg
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/dsa/trustdb.gpg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/eddsa/pubring.gpg
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/eddsa/pubring.kbx
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/eddsa/pubring.kbx~
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/eddsa/short.sig
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/eddsa/trustdb.gpg
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/eddsa/openpgp-revocs.d/4E630F84838BF6F7447B830B22692F5FEA9E2DD2.rev
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/eddsa/private-keys-v1.d/672E9A973B33784B4579F316820434E5631C086A.key
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/rsa/7B3ABB26B97B655AB9296BD15B0BD02E1C768C43.ssh
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/rsa/8288EF560ED3795F9DF2C0DB56193089B285DA58.ssh
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/rsa/8465A1E2E0FB2B40ADB2478E18FB3F537E0C8A17.ssh
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/rsa/E8AC80C924116DABB51D4B987CB07D6D2C199C7C.raw
--rw-r--r--   0        0        0     6792 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/rsa/F557D0FF451DEF45372591429EA70BD13D883381.raw
--rw-r--r--   0        0        0    17740 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/rsa/pubring.gpg
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/rsa/random_seed
--rw-r--r--   0        0        0    27893 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/rsa/secring.gpg
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/tests/gpg_keyrings/rsa/trustdb.gpg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/LICENSE
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/README.md
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/pyproject.toml
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 securesystemslib-0.31.0/PKG-INFO
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/.coveragerc
+-rw-r--r--   0        0        0    19409 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/mypy.ini
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/pylintrc
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/requirements-aws.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/requirements-build.txt
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/requirements-dev.txt
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/requirements-docs.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/requirements-kms.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/requirements-lint.txt
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/requirements-pinned.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/requirements-sigstore.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/requirements-test.txt
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/requirements-vault.txt
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/requirements.txt
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tox.ini
+-rwxr-xr-x   0        0        0      654 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/__init__.py
+-rw-r--r--   0        0        0     5386 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/dsse.py
+-rwxr-xr-x   0        0        0     1179 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/exceptions.py
+-rwxr-xr-x   0        0        0     5050 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/formats.py
+-rwxr-xr-x   0        0        0    11612 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/hash.py
+-rw-r--r--   0        0        0     9911 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/storage.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_gpg/__init__.py
+-rw-r--r--   0        0        0    35488 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_gpg/common.py
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_gpg/constants.py
+-rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_gpg/dsa.py
+-rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_gpg/eddsa.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_gpg/exceptions.py
+-rw-r--r--   0        0        0    10791 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_gpg/functions.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_gpg/handlers.py
+-rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_gpg/rsa.py
+-rw-r--r--   0        0        0    10505 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_gpg/util.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_internal/utils.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_vendor/README.md
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_vendor/__init__.py
+-rwxr-xr-x   0        0        0     1026 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_vendor/test-ed25519-upstream.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_vendor/ed25519/.gitignore
+-rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_vendor/ed25519/LICENSE
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_vendor/ed25519/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_vendor/ed25519/__init__.py
+-rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_vendor/ed25519/ed25519.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_vendor/ed25519/science.py
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_vendor/ed25519/test_ed25519.py
+-rw-r--r--   0        0        0  2427904 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/_vendor/ed25519/test_data/ed25519
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/signer/__init__.py
+-rw-r--r--   0        0        0     7911 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/signer/_aws_signer.py
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/signer/_azure_signer.py
+-rw-r--r--   0        0        0    11153 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/signer/_crypto_signer.py
+-rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/signer/_gcp_signer.py
+-rw-r--r--   0        0        0     7832 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/signer/_gpg_signer.py
+-rw-r--r--   0        0        0    13451 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/signer/_hsm_signer.py
+-rw-r--r--   0        0        0    15031 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/signer/_key.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/signer/_signature.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/signer/_signer.py
+-rw-r--r--   0        0        0    10005 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/signer/_sigstore_signer.py
+-rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/signer/_spx_signer.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/signer/_utils.py
+-rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/securesystemslib/signer/_vault_signer.py
+-rwxr-xr-x   0        0        0      370 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/__init__.py
+-rwxr-xr-x   0        0        0      706 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/aggregate_tests.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/check_aws_signer.py
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/check_azure_signer.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/check_gpg_available.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/check_kms_signers.py
+-rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/check_public_interfaces.py
+-rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/check_public_interfaces_gpg.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/check_sigstore_signer.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/check_vault_signer.py
+-rw-r--r--   0        0        0     5981 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/test_dsse.py
+-rwxr-xr-x   0        0        0     2297 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/test_formats.py
+-rw-r--r--   0        0        0    36506 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/test_gpg.py
+-rwxr-xr-x   0        0        0    10713 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/test_hash.py
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/test_hsm_signer.py
+-rw-r--r--   0        0        0    38073 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/test_signer.py
+-rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/test_storage.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/data/pems/ecdsa_private.pem
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/data/pems/ecdsa_private_encrypted.pem
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/data/pems/ecdsa_public.pem
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/data/pems/ecdsa_secp384r1_private.pem
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/data/pems/ecdsa_secp384r1_public.pem
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/data/pems/ed25519_private.pem
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/data/pems/ed25519_private_encrypted.pem
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/data/pems/ed25519_public.pem
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/data/pems/rsa_private.pem
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/data/pems/rsa_private_encrypted.pem
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/data/pems/rsa_public.pem
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.pem
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/dsa/pubring.gpg
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/dsa/random_seed
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/dsa/secring.gpg
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/dsa/trustdb.gpg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/eddsa/pubring.gpg
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/eddsa/pubring.kbx
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/eddsa/pubring.kbx~
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/eddsa/short.sig
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/eddsa/trustdb.gpg
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/eddsa/openpgp-revocs.d/4E630F84838BF6F7447B830B22692F5FEA9E2DD2.rev
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/eddsa/private-keys-v1.d/672E9A973B33784B4579F316820434E5631C086A.key
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/rsa/7B3ABB26B97B655AB9296BD15B0BD02E1C768C43.ssh
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/rsa/8288EF560ED3795F9DF2C0DB56193089B285DA58.ssh
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/rsa/8465A1E2E0FB2B40ADB2478E18FB3F537E0C8A17.ssh
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/rsa/E8AC80C924116DABB51D4B987CB07D6D2C199C7C.raw
+-rw-r--r--   0        0        0     6792 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/rsa/F557D0FF451DEF45372591429EA70BD13D883381.raw
+-rw-r--r--   0        0        0    17740 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/rsa/pubring.gpg
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/rsa/random_seed
+-rw-r--r--   0        0        0    27893 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/rsa/secring.gpg
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/gpg_keyrings/rsa/trustdb.gpg
+-rwxr-xr-x   0        0        0      799 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/scripts/init-aws-kms.sh
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/scripts/init-vault.sh
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/tests/scripts/stop-vault.sh
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/README.md
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 securesystemslib-1.0.0/PKG-INFO
```

### Comparing `securesystemslib-0.31.0/CHANGELOG.md` & `securesystemslib-1.0.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,49 @@
 # Changelog
 
+## securesystemslib v1.0.0
+
+Securesystemslib API is now considered stable. The core functionality is
+provided in the _Signer_ interface and the half a dozen integrated _Signer_
+implementations that can be found in the `signer` module. Smaller helper
+modules `dsse`, `formats`, `hash` and `storage` are also part of the API.
+Several legacy modules have been removed.
+
+### Added
+* Signer: add public_key attribute to interface (#756)
+* VaultSigner: Signer implementation for HashiCorp Vault (#800)
+* CryptoSigner: support ecdsa keytype that is no longer in spec (#711)
+* CryptoSigner: add private_bytes property (#799)
+* CryptoSigner: add `"file2"` signer uri (#759)
+* test: use localstack to test AWSSigner (#777)
+
+### Removed
+* CryptoSigner: remove `"file"` signer uri (#759)
+* migration script for legacy keys  (#770)
+* `SSlibSigner` class and `*_securesystemslib_key` methods (#771)
+* legacy key `key*`, `interface`, `util` and `schema` modules (#772, #773, #776)
+* unused functions in `hash`, and `formats` module (#774, #776)
+* unused global key constants (#806)
+
+### Changed
+* SSlibKey: strengthen input validation (#780, #795)
+* AWSSigner: support default scheme and add stronger input validation (#724, #778)
+* dsse: change Envelope.signatures type to dict (#743)
+* vendor: update ed25519 copy (#793)
+* docs: improve user and contributor docs (#744, #745, #746, #749, #759, #796)
+* test: improve and temporarily disable SigstoreSigner test (#779, #785)
+* ci: use dependabot groups, update weekly (#735)
+* ci: test macOS and Windows on latest Python only (#797)
+* Make securessystemslib.gpg internal (#792)
+
+### Fixed
+* Fix check-upstream-ed25519 workflow permission (#706)
+* SSlibKey: fix default scheme and test for ecdsa nistp384 key (#763 #794)
+
+
 ## securesystemslib v0.31.0
 
 ### Added
 * CryptoSigner: create from `cryptography` private key with new constructor (#675)
 * SSlibKey: create from `cryptography` public key with new `from_crypto` method (#678)
 * Release: auto-release with PyPI Trusted Publishing (#683)
 * Docs to migrate legacy key files (#658)
```

### Comparing `securesystemslib-0.31.0/mypy.ini` & `securesystemslib-1.0.0/mypy.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [mypy]
 warn_unused_configs = True
 files =
-    securesystemslib/util.py,
     securesystemslib/signer/*.py,
     securesystemslib/storage.py,
-    securesystemslib/gpg/constants.py
+    securesystemslib/_gpg/constants.py
 
 # Supress error messages until enough modules
 # are type annotated
 follow_imports = silent
 
 # let's not install typeshed annotations for GCPSigner
 [mypy-google.*]
@@ -34,7 +33,10 @@
 ignore_missing_imports = True
 
 [mypy-boto3.*]
 ignore_missing_imports = True
 
 [mypy-botocore.*]
 ignore_missing_imports = True
+
+[mypy-hvac.*]
+ignore_missing_imports = True
```

### Comparing `securesystemslib-0.31.0/pylintrc` & `securesystemslib-1.0.0/pylintrc`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/tox.ini` & `securesystemslib-1.0.0/tox.ini`

 * *Files 23% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 deps =
     -r{toxinidir}/requirements-pinned.txt
     -r{toxinidir}/requirements-test.txt
 
 commands =
     python -m tests.check_gpg_available
     coverage run tests/aggregate_tests.py
-    coverage report -m --fail-under 83
+    coverage report -m --fail-under 70
 
 [testenv:purepy311]
 deps =
 
 commands =
     python -m tests.check_gpg_available
     python -m tests.check_public_interfaces
@@ -45,36 +45,87 @@
 commands =
     python -m tests.check_kms_signers
 
 [testenv:sigstore]
 deps =
     -r{toxinidir}/requirements-pinned.txt
     -r{toxinidir}/requirements-sigstore.txt
-passenv =
-    # These are required to detect ambient credentials on GitHub
-    GITHUB_ACTIONS
-    ACTIONS_ID_TOKEN_REQUEST_TOKEN
-    ACTIONS_ID_TOKEN_REQUEST_URL
-    CERT_ID
-    CERT_ISSUER
 commands =
     python -m tests.check_sigstore_signer
 
-# This checks that importing securesystemslib.gpg.constants doesn't shell out on
-# import.
+# Check that importing securesystemslib._gpg.constants doesn't shell out.
 [testenv:py311-test-gpg-fails]
 setenv =
     GNUPG = false
 commands =
-    python -c "import securesystemslib.gpg.constants"
+    python -c "import securesystemslib._gpg.constants"
 
 [testenv:lint]
 deps =
     -r{toxinidir}/requirements-pinned.txt
     -r{toxinidir}/requirements-lint.txt
 commands =
     black --check --diff  .
     isort --check --diff  .
 
     pylint -j 0 --rcfile=pylintrc securesystemslib tests
     bandit --recursive securesystemslib --exclude _vendor
     mypy
+
+# Requires docker running
+[testenv:local-aws-kms]
+deps =
+    -r{toxinidir}/requirements-pinned.txt
+    -r{toxinidir}/requirements-aws.txt
+    localstack
+    awscli
+    awscli-local
+
+allowlist_externals =
+    localstack
+    bash
+
+setenv =
+    AWS_ACCESS_KEY_ID = test
+    AWS_SECRET_ACCESS_KEY = test
+    AWS_ENDPOINT_URL = http://localhost:4566/
+    AWS_DEFAULT_REGION = us-east-1
+
+commands_pre =
+    # Start virtual AWS KMS
+    localstack start --detached
+    localstack wait
+
+    # Create test keys
+    bash {toxinidir}/tests/scripts/init-aws-kms.sh
+
+commands =
+    # Run tests
+    python -m tests.check_aws_signer
+
+commands_post =
+    # Stop virtual AWS KMS
+    localstack stop
+
+
+# Requires `vault`
+# https://developer.hashicorp.com/vault/tutorials/getting-started/getting-started-install
+[testenv:local-vault]
+deps =
+    -r{toxinidir}/requirements-pinned.txt
+    -r{toxinidir}/requirements-vault.txt
+
+allowlist_externals =
+    bash
+
+setenv =
+    VAULT_ADDR = http://localhost:8200
+    VAULT_TOKEN = test-root-token
+
+commands_pre =
+    bash {toxinidir}/tests/scripts/init-vault.sh
+
+commands =
+     python -m tests.check_vault_signer
+
+commands_post =
+    bash {toxinidir}/tests/scripts/stop-vault.sh
```

### Comparing `securesystemslib-0.31.0/securesystemslib/dsse.py` & `securesystemslib-1.0.0/securesystemslib/dsse.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,20 +13,23 @@
 
 class Envelope:
     """DSSE Envelope to provide interface for signing arbitrary data.
 
     Attributes:
         payload: Arbitrary byte sequence of serialized body.
         payload_type: string that identifies how to interpret payload.
-        signatures: list of Signature.
+        signatures: dict of Signature key id and Signatures.
 
     """
 
     def __init__(
-        self, payload: bytes, payload_type: str, signatures: List[Signature]
+        self,
+        payload: bytes,
+        payload_type: str,
+        signatures: Dict[str, Signature],
     ):
         self.payload = payload
         self.payload_type = payload_type
         self.signatures = signatures
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, Envelope):
@@ -54,26 +57,31 @@
         Returns:
             A "Envelope" instance.
         """
 
         payload = b64dec(data["payload"])
         payload_type = data["payloadType"]
 
-        signatures = []
+        signatures = {}
         for signature in data["signatures"]:
             signature["sig"] = b64dec(signature["sig"]).hex()
-            signatures.append(Signature.from_dict(signature))
+            signature = Signature.from_dict(signature)
+            if signature.keyid in signatures:
+                raise ValueError(
+                    f"Multiple signatures found for keyid {signature.keyid}"
+                )
+            signatures[signature.keyid] = signature
 
         return cls(payload, payload_type, signatures)
 
     def to_dict(self) -> dict:
         """Returns the JSON-serializable dictionary representation of self."""
 
         signatures = []
-        for signature in self.signatures:
+        for signature in self.signatures.values():
             sig_dict = signature.to_dict()
             sig_dict["sig"] = b64enc(bytes.fromhex(sig_dict["sig"]))
             signatures.append(sig_dict)
 
         return {
             "payload": b64enc(self.payload),
             "payloadType": self.payload_type,
@@ -97,24 +105,21 @@
             signer: A "Signer" class instance.
 
         Returns:
             A "Signature" instance.
         """
 
         signature = signer.sign(self.pae())
-        self.signatures.append(signature)
+        self.signatures[signature.keyid] = signature
 
         return signature
 
     def verify(self, keys: List[Key], threshold: int) -> Dict[str, Key]:
         """Verify the payload with the provided Keys.
 
-        NOTE: This API is experimental and might change (see
-        secure-systems-lab/dsse#55)
-
         Arguments:
             keys: A list of public keys to verify the signatures.
             threshold: Number of signatures needed to pass the verification.
 
         Raises:
             ValueError: If "threshold" is not valid.
             VerificationError: If the enclosed signatures do not pass the
@@ -136,15 +141,15 @@
         # checks for threshold value.
         if threshold <= 0:
             raise ValueError("Threshold must be greater than 0")
 
         if len(keys) < threshold:
             raise ValueError("Number of keys can't be less than threshold")
 
-        for signature in self.signatures:
+        for signature in self.signatures.values():
             for key in keys:
                 # If Signature keyid doesn't match with Key, skip.
                 if not key.keyid == signature.keyid:
                     continue
 
                 # If a key verifies the signature, we exit and use the result.
                 try:
```

### Comparing `securesystemslib-0.31.0/securesystemslib/hash.py` & `securesystemslib-1.0.0/securesystemslib/hash.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   include functions to create digest objects given a filename or file object.
   Only the standard hashlib library is currently supported, but
   pyca/cryptography support will be added in the future.
 """
 
 import hashlib
 
-from securesystemslib import exceptions, formats
+from securesystemslib import exceptions
 from securesystemslib.storage import FilesystemBackend
 
 DEFAULT_CHUNK_SIZE = 4096
 DEFAULT_HASH_ALGORITHM = "sha256"
 DEFAULT_HASH_LIBRARY = "hashlib"
 SUPPORTED_LIBRARIES = ["hashlib"]
 
@@ -60,16 +60,15 @@
             digest_object.digest_size
             digest_object.hexdigest()
             digest_object.update('data')
             digest_object.digest()
 
         <Properties>
           algorithm:
-            Specific for `cryptography.hazmat.primitives.hashes.Hash` object, but
-            needed for `rsa_keys.py`
+            Specific for `cryptography.hazmat.primitives.hashes.Hash` object.
 
           digest_size:
             Returns original's object digest size.
 
         <Methods>
           digest(self) -> bytes:
             Calls original's object `finalize` method and returns digest as bytes.
@@ -142,17 +141,14 @@
       algorithm:
         The hash algorithm (e.g., 'sha256', 'sha512').
 
       hash_library:
         The crypto library to use for the given hash algorithm (e.g., 'hashlib').
 
     <Exceptions>
-      securesystemslib.exceptions.FormatError, if the arguments are
-      improperly formatted.
-
       securesystemslib.exceptions.UnsupportedAlgorithmError, if an unsupported
       hashing algorithm is specified, or digest could not be generated with given
       the algorithm.
 
       securesystemslib.exceptions.UnsupportedLibraryError, if an unsupported
       library was requested via 'hash_library'.
 
@@ -163,19 +159,14 @@
       Digest object
 
       e.g.
         hashlib.new(algorithm) or
         PycaDiggestWrapper object
     """
 
-    # Are the arguments properly formatted?  If not, raise
-    # 'securesystemslib.exceptions.FormatError'.
-    formats.NAME_SCHEMA.check_match(algorithm)
-    formats.NAME_SCHEMA.check_match(hash_library)
-
     # Was a hashlib digest object requested and is it supported?
     # If so, return the digest object.
     if hash_library == "hashlib" and hash_library in SUPPORTED_LIBRARIES:
         try:
             if algorithm == "blake2b-256":  # pylint: disable=no-else-return
                 return hashlib.new("blake2b", digest_size=32)
             else:
@@ -257,20 +248,14 @@
     <Returns>
       Digest object
 
       e.g.
         hashlib.new(algorithm) or
         PycaDiggestWrapper object
     """
-
-    # Are the arguments properly formatted?  If not, raise
-    # 'securesystemslib.exceptions.FormatError'.
-    formats.NAME_SCHEMA.check_match(algorithm)
-    formats.NAME_SCHEMA.check_match(hash_library)
-
     # Digest object returned whose hash will be updated using 'file_object'.
     # digest() raises:
     # securesystemslib.exceptions.UnsupportedAlgorithmError
     # securesystemslib.exceptions.UnsupportedLibraryError
     digest_object = digest(algorithm, hash_library)
 
     # Defensively seek to beginning, as there's no case where we don't
@@ -337,17 +322,14 @@
 
       storage_backend:
         An object which implements
         securesystemslib.storage.StorageBackendInterface. When no object is
         passed a FilesystemBackend will be instantiated and used.
 
     <Exceptions>
-      securesystemslib.exceptions.FormatError, if the arguments are
-      improperly formatted.
-
       securesystemslib.exceptions.UnsupportedAlgorithmError, if the given
       'algorithm' is unsupported.
 
       securesystemslib.exceptions.UnsupportedLibraryError, if the given
       'hash_library' is unsupported.
 
       securesystemslib.exceptions.StorageError, if the file cannot be opened.
@@ -358,20 +340,14 @@
     <Returns>
       Digest object
 
       e.g.
         hashlib.new(algorithm) or
         PycaDiggestWrapper object
     """
-    # Are the arguments properly formatted?  If not, raise
-    # 'securesystemslib.exceptions.FormatError'.
-    formats.PATH_SCHEMA.check_match(filename)
-    formats.NAME_SCHEMA.check_match(algorithm)
-    formats.NAME_SCHEMA.check_match(hash_library)
-
     digest_object = None
 
     if storage_backend is None:
         storage_backend = FilesystemBackend()
 
     # Open 'filename' in read+binary mode.
     with storage_backend.get(filename) as file_object:
@@ -380,52 +356,7 @@
         # securesystemslib.exceptions.UnsupportedAlgorithmError
         # securesystemslib.exceptions.UnsupportedLibraryError
         digest_object = digest_fileobject(
             file_object, algorithm, hash_library, normalize_line_endings
         )
 
     return digest_object
-
-
-def digest_from_rsa_scheme(scheme, hash_library=DEFAULT_HASH_LIBRARY):
-    """
-    <Purpose>
-      Get digest object from RSA scheme.
-
-    <Arguments>
-      scheme:
-        A string that indicates the signature scheme used to generate
-        'signature'. Currently supported RSA schemes are defined in
-        `securesystemslib.keys.RSA_SIGNATURE_SCHEMES`
-
-      hash_library:
-        The crypto library to use for the given hash algorithm (e.g., 'hashlib').
-
-    <Exceptions>
-      securesystemslib.exceptions.FormatError, if the arguments are
-      improperly formatted.
-
-      securesystemslib.exceptions.UnsupportedAlgorithmError, if an unsupported
-      hashing algorithm is specified, or digest could not be generated with given
-      the algorithm.
-
-      securesystemslib.exceptions.UnsupportedLibraryError, if an unsupported
-      library was requested via 'hash_library'.
-
-    <Side Effects>
-      None.
-
-    <Returns>
-      Digest object
-
-      e.g.
-        hashlib.new(algorithm) or
-        PycaDiggestWrapper object
-    """
-    # Are the arguments properly formatted?  If not, raise
-    # 'securesystemslib.exceptions.FormatError'.
-    formats.RSA_SCHEME_SCHEMA.check_match(scheme)
-
-    # Get hash algorithm from rsa scheme (hash algorithm id is specified after
-    # the last dash; e.g. rsassa-pss-sha256 -> sha256)
-    hash_algorithm = scheme.split("-")[-1]
-    return digest(hash_algorithm, hash_library)
```

### Comparing `securesystemslib-0.31.0/securesystemslib/storage.py` & `securesystemslib-1.0.0/securesystemslib/storage.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/securesystemslib/_internal/utils.py` & `securesystemslib-1.0.0/securesystemslib/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/securesystemslib/_vendor/README.md` & `securesystemslib-1.0.0/securesystemslib/_vendor/README.md`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/securesystemslib/_vendor/test-ed25519-upstream.sh` & `securesystemslib-1.0.0/securesystemslib/_vendor/test-ed25519-upstream.sh`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # This is used in CI workflow to open an issue if new commits are found
 
 set -eu
 
 # This commit matches our securesystemslib/_vendor/ed25519/ content.
 # If upstream changes, we should review the changes, vendor them,
 # and update the hash here
-pyca_ed25519_expected="f98354b09ffde8444a04c71f8e3ac7b948c89a02"
+pyca_ed25519_expected="08a7962a8059e4546a21b97f4a847f75cd1a1bbb"
 pyca_ed25519_git_url="https://github.com/pyca/ed25519.git"
 
 pyca_ed25519_main_head=$(git ls-remote "$pyca_ed25519_git_url" main | cut -f1)
 if [ "$pyca_ed25519_main_head" != "$pyca_ed25519_expected" ]; then
     echo "Expected [main](https://github.com/pyca/ed25519/commits/main)" \
 	 "to be commit ${pyca_ed25519_expected:0:7}, found" \
 	 "${pyca_ed25519_main_head:0:7} instead" \
```

### Comparing `securesystemslib-0.31.0/securesystemslib/_vendor/ed25519/LICENSE` & `securesystemslib-1.0.0/securesystemslib/_vendor/ed25519/LICENSE`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/securesystemslib/_vendor/ed25519/README.rst` & `securesystemslib-1.0.0/securesystemslib/_vendor/ed25519/README.rst`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/securesystemslib/_vendor/ed25519/ed25519.py` & `securesystemslib-1.0.0/securesystemslib/_vendor/ed25519/ed25519.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,39 +27,19 @@
 inputs, and its memory access patterns may also depend on the inputs.
 This opens it to timing and cache side-channel attacks which can
 disclose data to an attacker.  We rely on Python's long-integer
 arithmetic, so we cannot handle secrets without risking their disclosure.
 """
 
 import hashlib
-import operator
-import sys
 
 
 __version__ = "1.0.dev0"
 
 
-# Useful for very coarse version differentiation.
-PY3 = sys.version_info[0] == 3
-
-if PY3:
-    indexbytes = operator.getitem
-    intlist2bytes = bytes
-    int2byte = operator.methodcaller("to_bytes", 1, "big")
-else:
-    int2byte = chr
-    range = xrange  # noqa: F821
-
-    def indexbytes(buf, i):
-        return ord(buf[i])
-
-    def intlist2bytes(l):
-        return b"".join(chr(c) for c in l)
-
-
 b = 256
 q = 2**255 - 19
 l = 2**252 + 27742317777372353535851937790883648493
 
 
 def H(m):
     return hashlib.sha512(m).digest()
@@ -193,38 +173,32 @@
         e = e // 2
     assert e == 0, e
     return P
 
 
 def encodeint(y):
     bits = [(y >> i) & 1 for i in range(b)]
-    return b"".join(
-        [
-            int2byte(sum([bits[i * 8 + j] << j for j in range(8)]))
-            for i in range(b // 8)
-        ]
+    return bytes(
+        [sum([bits[i * 8 + j] << j for j in range(8)]) for i in range(b // 8)]
     )
 
 
 def encodepoint(P):
     (x, y, z, t) = P
     zi = inv(z)
     x = (x * zi) % q
     y = (y * zi) % q
     bits = [(y >> i) & 1 for i in range(b - 1)] + [x & 1]
-    return b"".join(
-        [
-            int2byte(sum([bits[i * 8 + j] << j for j in range(8)]))
-            for i in range(b // 8)
-        ]
+    return bytes(
+        [sum([bits[i * 8 + j] << j for j in range(8)]) for i in range(b // 8)]
     )
 
 
 def bit(h, i):
-    return (indexbytes(h, i // 8) >> (i % 8)) & 1
+    return (h[i // 8] >> (i % 8)) & 1
 
 
 def publickey_unsafe(sk):
     """
     Not safe to use with secret keys or secret data.
 
     See module docstring.  This function should be used for testing only.
@@ -244,17 +218,15 @@
     """
     Not safe to use with secret keys or secret data.
 
     See module docstring.  This function should be used for testing only.
     """
     h = H(sk)
     a = 2 ** (b - 2) + sum(2**i * bit(h, i) for i in range(3, b - 2))
-    r = Hint(
-        intlist2bytes([indexbytes(h, j) for j in range(b // 8, b // 4)]) + m
-    )
+    r = Hint(bytes([h[j] for j in range(b // 8, b // 4)]) + m)
     R = scalarmult_B(r)
     S = (r + Hint(encodepoint(R) + pk + m) * a) % l
     return encodepoint(R) + encodeint(S)
 
 
 def isoncurve(P):
     (x, y, z, t) = P
```

### Comparing `securesystemslib-0.31.0/securesystemslib/_vendor/ed25519/science.py` & `securesystemslib-1.0.0/securesystemslib/_vendor/ed25519/science.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/securesystemslib/_vendor/ed25519/test_ed25519.py` & `securesystemslib-1.0.0/securesystemslib/_vendor/ed25519/test_ed25519.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,20 +71,15 @@
     ed25519.checkvalid(sig, m, pk)
 
     # Assert that we cannot forge a message
     try:
         if len(m) == 0:
             forgedm = b"x"
         else:
-            forgedm = ed25519.intlist2bytes(
-                [
-                    ed25519.indexbytes(m, i) + (i == len(m) - 1)
-                    for i in range(len(m))
-                ]
-            )
+            forgedm = bytes([m[i] + (i == len(m) - 1) for i in range(len(m))])
     except ValueError:
         # TODO: Yes this means that we "pass" a test if we can't generate a
         # forged message. This matches the original test suite, it's
         # unclear if it was intentional there or not.
         pass
     else:
         with pytest.raises(ed25519.SignatureMismatch):
```

### Comparing `securesystemslib-0.31.0/securesystemslib/_vendor/ed25519/test_data/ed25519` & `securesystemslib-1.0.0/securesystemslib/_vendor/ed25519/test_data/ed25519`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/securesystemslib/gpg/__init__.py` & `securesystemslib-1.0.0/securesystemslib/_gpg/__init__.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/securesystemslib/gpg/common.py` & `securesystemslib-1.0.0/securesystemslib/_gpg/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 
 <Purpose>
   Provides algorithm-agnostic gpg public key and signature parsing functions.
   The functions select the appropriate functions for each algorithm and
   call them.
 
 """
+
 import binascii
 import collections
 import logging
 import struct
 
-from securesystemslib import formats
-from securesystemslib.gpg import util as gpg_util
-from securesystemslib.gpg.constants import (
+from securesystemslib._gpg import util as gpg_util
+from securesystemslib._gpg.constants import (
     FULL_KEYID_SUBPACKET,
+    GPG_HASH_ALGORITHM_STRING,
     KEY_EXPIRATION_SUBPACKET,
     PACKET_TYPE_PRIMARY_KEY,
     PACKET_TYPE_SIGNATURE,
     PACKET_TYPE_SUB_KEY,
     PACKET_TYPE_USER_ATTR,
     PACKET_TYPE_USER_ID,
     PARTIAL_KEYID_SUBPACKET,
@@ -40,21 +41,21 @@
     SIG_CREATION_SUBPACKET,
     SIGNATURE_TYPE_BINARY,
     SIGNATURE_TYPE_CERTIFICATES,
     SIGNATURE_TYPE_SUB_KEY_BINDING,
     SUPPORTED_PUBKEY_PACKET_VERSIONS,
     SUPPORTED_SIGNATURE_PACKET_VERSIONS,
 )
-from securesystemslib.gpg.exceptions import (
+from securesystemslib._gpg.exceptions import (
     KeyNotFoundError,
     PacketParsingError,
     PacketVersionNotSupportedError,
     SignatureAlgorithmNotSupportedError,
 )
-from securesystemslib.gpg.handlers import (
+from securesystemslib._gpg.handlers import (
     SIGNATURE_HANDLERS,
     SUPPORTED_SIGNATURE_ALGORITHMS,
 )
 
 log = logging.getLogger(__name__)
 
 
@@ -66,37 +67,37 @@
 
     <Arguments>
       data:
             An RFC4880 public key packet payload as described in section 5.5.2.
             (version 4) of the RFC.
 
             NOTE: The payload can be parsed from a full key packet (header +
-            payload) by using securesystemslib.gpg.util.parse_packet_header.
+            payload) by using securesystemslib._gpg.util.parse_packet_header.
 
             WARNING: this doesn't support armored pubkey packets, so use with
             care. pubkey packets are a little bit more complicated than the
             signature ones
 
     <Exceptions>
       ValueError
             If the passed public key data is empty.
 
-      securesystemslib.gpg.exceptions.PacketVersionNotSupportedError
+      securesystemslib._gpg.exceptions.PacketVersionNotSupportedError
             If the packet version does not match
-            securesystemslib.gpg.constants.SUPPORTED_PUBKEY_PACKET_VERSIONS
+            securesystemslib._gpg.constants.SUPPORTED_PUBKEY_PACKET_VERSIONS
 
-      securesystemslib.gpg.exceptions.SignatureAlgorithmNotSupportedError
+      securesystemslib._gpg.exceptions.SignatureAlgorithmNotSupportedError
             If the signature algorithm does not match one of
-            securesystemslib.gpg.constants.SUPPORTED_SIGNATURE_ALGORITHMS
+            securesystemslib._gpg.constants.SUPPORTED_SIGNATURE_ALGORITHMS
 
     <Side Effects>
       None.
 
     <Returns>
-      A public key in the format securesystemslib.formats.GPG_PUBKEY_SCHEMA
+      A public key dict.
 
     """
     if not data:
         raise ValueError("Could not parse empty pubkey payload.")
 
     ptr = 0
     keyinfo = {}
@@ -140,15 +141,15 @@
     handler = SIGNATURE_HANDLERS[keyinfo["type"]]
     keyinfo["keyid"] = gpg_util.compute_keyid(data)
     key_params = handler.get_pubkey_params(data[ptr:])
 
     return {
         "method": keyinfo["method"],
         "type": keyinfo["type"],
-        "hashes": [formats.GPG_HASH_ALGORITHM_STRING],
+        "hashes": [GPG_HASH_ALGORITHM_STRING],
         "creation_time": time_of_creation[0],
         "keyid": keyinfo["keyid"],
         "keyval": {"private": "", "public": key_params},
     }
 
 
 def parse_pubkey_bundle(data):
@@ -164,15 +165,15 @@
       primary key via signatures.
 
     <Arguments>
       data:
             Public key data as written to stdout by gpg_export_pubkey_command.
 
     <Exceptions>
-      securesystemslib.gpg.exceptions.PacketParsingError
+      securesystemslib._gpg.exceptions.PacketParsingError
             If data is empty.
             If data cannot be parsed.
 
     <Side Effects>
       None.
 
     <Returns>
@@ -328,15 +329,15 @@
     <Exceptions>
       None.
 
     <Side Effects>
       None.
 
     <Returns>
-      A public key in the format securesystemslib.formats.GPG_PUBKEY_SCHEMA.
+      A public key dict.
 
     """
     # Create handler shortcut
     handler = SIGNATURE_HANDLERS[bundle[PACKET_TYPE_PRIMARY_KEY]["key"]["type"]]
 
     is_primary_user = False
     validity_period = None
@@ -471,16 +472,15 @@
     <Exceptions>
       None.
 
     <Side Effects>
       None.
 
     <Returns>
-      A dictionary of public keys in the format
-      securesystemslib.formats.GPG_PUBKEY_SCHEMA, with keyids as dict keys.
+      A dict of public keys dicts with keyids as dict keys.
 
     """
     # Create handler shortcut
     handler = SIGNATURE_HANDLERS[bundle[PACKET_TYPE_PRIMARY_KEY]["key"]["type"]]
 
     # Verify subkey binding signatures and only keep verified keys
     # See notes about subkey binding signature in RFC4880 5.2.3.3
@@ -581,42 +581,37 @@
       - If the keyid matches one of the subkeys, a warning is issued to notify
         the user about potential privilege escalation
       - Subkeys with invalid key binding signatures are discarded
 
     <Arguments>
       data:
             Public key data as written to stdout by
-            securesystemslib.gpg.constants.gpg_export_pubkey_command.
+            securesystemslib._gpg.constants.gpg_export_pubkey_command.
 
       keyid:
             The keyid of the master key or one of its subkeys expected to be
             contained in the passed gpg data.
 
     <Exceptions>
-      securesystemslib.gpg.exceptions.PacketParsingError
+      securesystemslib._gpg.exceptions.PacketParsingError
             If the key data could not be parsed
 
-      securesystemslib.gpg.exceptions.KeyNotFoundError
+      securesystemslib._gpg.exceptions.KeyNotFoundError
             If the passed data is empty.
             If no master key or subkeys could be found that matches the passed
             keyid.
 
-      securesystemslib.exceptions.FormatError
-            If the passed keyid does not match
-            securesystemslib.formats.KEYID_SCHEMA
 
     <Side Effects>
       None.
 
     <Returns>
-      A public key in the format securesystemslib.formats.GPG_PUBKEY_SCHEMA with
-      optional subkeys.
+      A public key dict with optional subkeys.
 
     """
-    formats.KEYID_SCHEMA.check_match(keyid)
     if not data:
         raise KeyNotFoundError(
             "Could not find gpg key '{}' in empty exported key "  # pylint: disable=consider-using-f-string
             "data.".format(keyid)
         )
 
     # Parse out master key and subkeys (enriched and verified via certificates
@@ -677,20 +672,20 @@
 
     <Arguments>
       data:
              the RFC4880-encoded binary signature data buffer as described in
              section 5.2 (and 5.2.3.1).
       supported_signature_types: (optional)
             a set of supported signature_types, the signature packet may be
-            (see securesystemslib.gpg.constants for available types). If None is
+            (see securesystemslib._gpg.constants for available types). If None is
             specified the signature packet must be of type SIGNATURE_TYPE_BINARY.
       supported_hash_algorithms: (optional)
             a set of supported hash algorithm ids, the signature packet
             may use. Available ids are SHA1, SHA256, SHA512 (see
-            securesystemslib.gpg.constants). If None is specified, the signature
+            securesystemslib._gpg.constants). If None is specified, the signature
             packet must use SHA256.
       include_info: (optional)
             a boolean that indicates whether an opaque dictionary should be
             added to the returned signature under the key "info". Default is
             False.
 
     <Exceptions>
@@ -698,17 +693,15 @@
         malformed
       IndexError: if the signature packet is incomplete
 
     <Side Effects>
       None.
 
     <Returns>
-      A signature dictionary matching
-      securesystemslib.formats.GPG_SIGNATURE_SCHEMA with the following special
-      characteristics:
+      A signature dict with the following special characteristics:
        - The "keyid" field is an empty string if it cannot be determined
        - The "short_keyid" is not added if it cannot be determined
        - At least one of non-empty "keyid" or "short_keyid" are part of the
          signature
 
     """
     if not supported_signature_types:
```

### Comparing `securesystemslib-0.31.0/securesystemslib/gpg/constants.py` & `securesystemslib-1.0.0/securesystemslib/_gpg/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 <Copyright>
   See LICENSE for licensing information.
 
 <Purpose>
   aggregates all the constant definitions and lookup structures for signature
   handling
 """
+
 import functools
 import logging
 import os
 import shlex
 import subprocess  # nosec
 from typing import List, Optional
 
@@ -126,7 +127,9 @@
 PARTIAL_KEYID_SUBPACKET = 0x10
 # See section 5.2.3.6 (Key Expiration Time) of RFC4880
 KEY_EXPIRATION_SUBPACKET = 0x09
 # See section 5.2.3.19 (Primary User ID) of RFC4880
 PRIMARY_USERID_SUBPACKET = 0x19
 # See section 5.2.3.28. (Issuer Fingerprint) of rfc4880bis-06
 FULL_KEYID_SUBPACKET = 0x21
+
+GPG_HASH_ALGORITHM_STRING = "pgp+SHA2"
```

### Comparing `securesystemslib-0.31.0/securesystemslib/gpg/dsa.py` & `securesystemslib-1.0.0/securesystemslib/_gpg/dsa.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,62 +10,57 @@
 
 <Copyright>
   See LICENSE for licensing information.
 
 <Purpose>
   DSA-specific handling routines for signature verification and key parsing
 """
+
 import binascii
 
 CRYPTO = True
 NO_CRYPTO_MSG = "DSA key support for GPG requires the cryptography library"
 try:
     from cryptography.exceptions import InvalidSignature
     from cryptography.hazmat import backends
     from cryptography.hazmat.primitives.asymmetric import dsa
     from cryptography.hazmat.primitives.asymmetric import utils as dsautils
 except ImportError:
     CRYPTO = False
 
 # pylint: disable=wrong-import-position
-from securesystemslib import exceptions, formats
-from securesystemslib.gpg import util as gpg_util
-from securesystemslib.gpg.exceptions import PacketParsingError
+from securesystemslib import exceptions
+from securesystemslib._gpg import util as gpg_util
+from securesystemslib._gpg.exceptions import PacketParsingError
 
 # pylint: enable=wrong-import-position
 
 
 def create_pubkey(pubkey_info):
     """
     <Purpose>
       Create and return a DSAPublicKey object from the passed pubkey_info
       using pyca/cryptography.
 
     <Arguments>
       pubkey_info:
-              The DSA pubkey info dictionary as specified by
-              securesystemslib.formats.GPG_DSA_PUBKEY_SCHEMA
+              The DSA pubkey dict.
 
     <Exceptions>
-      securesystemslib.exceptions.FormatError if
-        pubkey_info does not match securesystemslib.formats.GPG_DSA_PUBKEY_SCHEMA
-
       securesystemslib.exceptions.UnsupportedLibraryError if
         the cryptography module is not available
 
     <Returns>
       A cryptography.hazmat.primitives.asymmetric.dsa.DSAPublicKey based on the
       passed pubkey_info.
 
     """
     if not CRYPTO:  # pragma: no cover
         raise exceptions.UnsupportedLibraryError(NO_CRYPTO_MSG)
 
-    formats.GPG_DSA_PUBKEY_SCHEMA.check_match(pubkey_info)
-
     y = int(pubkey_info["keyval"]["public"]["y"], 16)
     g = int(pubkey_info["keyval"]["public"]["g"], 16)
     p = int(pubkey_info["keyval"]["public"]["p"], 16)
     q = int(pubkey_info["keyval"]["public"]["q"], 16)
     parameter_numbers = dsa.DSAParameterNumbers(p, q, g)
     pubkey = dsa.DSAPublicNumbers(y, parameter_numbers).public_key(
         backends.default_backend()
@@ -81,23 +76,22 @@
 
     <Arguments>
       data:
              the RFC4880-encoded public key parameters data buffer as described
              in the fifth paragraph of section 5.5.2.
 
     <Exceptions>
-      securesystemslib.gpg.exceptions.PacketParsingError:
+      securesystemslib._gpg.exceptions.PacketParsingError:
              if the public key parameters are malformed
 
     <Side Effects>
       None.
 
     <Returns>
-      The parsed DSA public key in the format
-      securesystemslib.formats.GPG_DSA_PUBKEY_SCHEMA.
+      A DSA public key dict.
 
     """
     ptr = 0
 
     prime_p_length = gpg_util.get_mpi_length(data[ptr : ptr + 2])
     ptr += 2
     prime_p = data[ptr : ptr + prime_p_length]
@@ -140,15 +134,15 @@
 
     <Arguments>
       data:
              the RFC4880-encoded signature data buffer as described
              in the fourth paragraph of section 5.2.2
 
     <Exceptions>
-      securesystemslib.gpg.exceptions.PacketParsingError:
+      securesystemslib._gpg.exceptions.PacketParsingError:
              if the public key parameters are malformed
 
       securesystemslib.exceptions.UnsupportedLibraryError:
              if the cryptography module is not available
 
     <Side Effects>
       None.
@@ -185,52 +179,43 @@
     """
     <Purpose>
       Verify the passed signature against the passed content with the passed
       DSA public key using pyca/cryptography.
 
     <Arguments>
       signature_object:
-              A signature dictionary as specified by
-              securesystemslib.formats.GPG_SIGNATURE_SCHEMA
+              A signature dict.
 
       pubkey_info:
-              The DSA public key info dictionary as specified by
-              securesystemslib.formats.GPG_DSA_PUBKEY_SCHEMA
+              The DSA public key dict.
 
       hash_algorithm_id:
-              one of SHA1, SHA256, SHA512 (see securesystemslib.gpg.constants)
+              one of SHA1, SHA256, SHA512 (see securesystemslib._gpg.constants)
               used to verify the signature
               NOTE: Overrides any hash algorithm specification in "pubkey_info"'s
               "hashes" or "method" fields.
 
       content:
               The signed bytes against which the signature is verified
 
     <Exceptions>
-      securesystemslib.exceptions.FormatError if:
-        signature_object does not match securesystemslib.formats.GPG_SIGNATURE_SCHEMA
-        pubkey_info does not match securesystemslib.formats.GPG_DSA_PUBKEY_SCHEMA
-
       securesystemslib.exceptions.UnsupportedLibraryError if:
         the cryptography module is not available
 
       ValueError:
         if the passed hash_algorithm_id is not supported (see
-        securesystemslib.gpg.util.get_hashing_class)
+        securesystemslib._gpg.util.get_hashing_class)
 
     <Returns>
       True if signature verification passes and False otherwise
 
     """
     if not CRYPTO:  # pragma: no cover
         raise exceptions.UnsupportedLibraryError(NO_CRYPTO_MSG)
 
-    formats.GPG_SIGNATURE_SCHEMA.check_match(signature_object)
-    formats.GPG_DSA_PUBKEY_SCHEMA.check_match(pubkey_info)
-
     hasher = gpg_util.get_hashing_class(hash_algorithm_id)
 
     pubkey_object = create_pubkey(pubkey_info)
 
     digest = gpg_util.hash_object(
         binascii.unhexlify(signature_object["other_headers"]), hasher(), content
     )
```

### Comparing `securesystemslib-0.31.0/securesystemslib/gpg/eddsa.py` & `securesystemslib-1.0.0/securesystemslib/_gpg/eddsa.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,19 +12,20 @@
   See LICENSE for licensing information.
 
 <Purpose>
   EdDSA/ed25519 algorithm-specific handling routines for pubkey and signature
   parsing and verification.
 
 """
+
 import binascii
 
-from securesystemslib import exceptions, formats
-from securesystemslib.gpg import util as gpg_util
-from securesystemslib.gpg.exceptions import PacketParsingError
+from securesystemslib import exceptions
+from securesystemslib._gpg import util as gpg_util
+from securesystemslib._gpg.exceptions import PacketParsingError
 
 CRYPTO = True
 NO_CRYPTO_MSG = "EdDSA key support for GPG requires the cryptography library"
 try:
     from cryptography.exceptions import InvalidSignature
     from cryptography.hazmat.primitives.asymmetric import (
         ed25519 as pyca_ed25519,
@@ -52,24 +53,23 @@
 
     <Arguments>
       data:
             The EdDSA public key data AFTER the one-octet number denoting the
             public-key algorithm of this key.
 
     <Exceptions>
-      securesystemslib.gpg.exceptions.PacketParsingError or IndexError:
+      securesystemslib._gpg.exceptions.PacketParsingError or IndexError:
             if the public key data is malformed.
 
     <Side Effects>
       None.
 
     <Returns>
       A dictionary with an element "q" that holds the ascii hex representation
-      of the MPI of an EC point representing an EdDSA public key that conforms
-      with securesystemslib.formats.GPG_ED25519_PUBKEY_SCHEMA.
+      of the MPI of an EC point representing an EdDSA public key.
 
     """
     ptr = 0
 
     curve_oid_len = data[ptr]
     ptr += 1
 
@@ -158,86 +158,72 @@
     """
     <Purpose>
       Create and return an Ed25519PublicKey object from the passed pubkey_info
       using pyca/cryptography.
 
     <Arguments>
       pubkey_info:
-            The ED25519 public key dictionary as specified by
-            securesystemslib.formats.GPG_ED25519_PUBKEY_SCHEMA
+            The ED25519 public key dict.
 
     <Exceptions>
-      securesystemslib.exceptions.FormatError if
-        pubkey_info does not match securesystemslib.formats.GPG_DSA_PUBKEY_SCHEMA
 
       securesystemslib.exceptions.UnsupportedLibraryError if
         the cryptography module is unavailable
 
     <Returns>
       A cryptography.hazmat.primitives.asymmetric.ed25519.Ed25519PublicKey based
       on the passed pubkey_info.
 
     """
     if not CRYPTO:  # pragma: no cover
         raise exceptions.UnsupportedLibraryError(NO_CRYPTO_MSG)
 
-    formats.GPG_ED25519_PUBKEY_SCHEMA.check_match(pubkey_info)
-
     public_bytes = binascii.unhexlify(pubkey_info["keyval"]["public"]["q"])
     public_key = pyca_ed25519.Ed25519PublicKey.from_public_bytes(public_bytes)
 
     return public_key
 
 
 def verify_signature(signature_object, pubkey_info, content, hash_algorithm_id):
     """
     <Purpose>
       Verify the passed signature against the passed content with the passed
       ED25519 public key using pyca/cryptography.
 
     <Arguments>
       signature_object:
-              A signature dictionary as specified by
-              securesystemslib.formats.GPG_SIGNATURE_SCHEMA
+              A signature dict.
 
       pubkey_info:
-              The DSA public key info dictionary as specified by
-              securesystemslib.formats.GPG_ED25519_PUBKEY_SCHEMA
+              A DSA public key dict.
 
       hash_algorithm_id:
-              one of SHA1, SHA256, SHA512 (see securesystemslib.gpg.constants)
+              one of SHA1, SHA256, SHA512 (see securesystemslib._gpg.constants)
               used to verify the signature
               NOTE: Overrides any hash algorithm specification in "pubkey_info"'s
               "hashes" or "method" fields.
 
       content:
               The signed bytes against which the signature is verified
 
     <Exceptions>
-      securesystemslib.exceptions.FormatError if:
-        signature_object does not match securesystemslib.formats.GPG_SIGNATURE_SCHEMA
-        pubkey_info does not match securesystemslib.formats.GPG_ED25519_PUBKEY_SCHEMA
-
       securesystemslib.exceptions.UnsupportedLibraryError if:
         the cryptography module is unavailable
 
       ValueError:
         if the passed hash_algorithm_id is not supported (see
-        securesystemslib.gpg.util.get_hashing_class)
+        securesystemslib._gpg.util.get_hashing_class)
 
     <Returns>
       True if signature verification passes and False otherwise.
 
     """
     if not CRYPTO:  # pragma: no cover
         raise exceptions.UnsupportedLibraryError(NO_CRYPTO_MSG)
 
-    formats.GPG_SIGNATURE_SCHEMA.check_match(signature_object)
-    formats.GPG_ED25519_PUBKEY_SCHEMA.check_match(pubkey_info)
-
     hasher = gpg_util.get_hashing_class(hash_algorithm_id)
 
     pubkey_object = create_pubkey(pubkey_info)
 
     # See RFC4880-bis8 14.8. EdDSA and 5.2.4 "Computing Signatures"
     digest = gpg_util.hash_object(
         binascii.unhexlify(signature_object["other_headers"]), hasher(), content
```

### Comparing `securesystemslib-0.31.0/securesystemslib/gpg/exceptions.py` & `securesystemslib-1.0.0/securesystemslib/_gpg/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 <Purpose>
   Define Exceptions used in the gpg package. Following the practice from
   securesystemslib the names chosen for exception classes should end in
   'Error' (except where there is a good reason not to).
 
 """
+
 import datetime
 
 
 class PacketParsingError(Exception):
     pass
 
 
@@ -33,18 +34,14 @@
     pass
 
 
 class SignatureAlgorithmNotSupportedError(Exception):
     pass
 
 
-class CommandError(Exception):
-    pass
-
-
 class KeyExpirationError(Exception):  # pylint: disable=missing-class-docstring
     def __init__(self, key):
         super(  # pylint: disable=super-with-arguments
             KeyExpirationError, self
         ).__init__()
         self.key = key
```

### Comparing `securesystemslib-0.31.0/securesystemslib/gpg/functions.py` & `securesystemslib-1.0.0/securesystemslib/_gpg/functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,52 +11,53 @@
 <Copyright>
   See LICENSE for licensing information.
 
 <Purpose>
   publicly-usable functions for exporting public-keys, signing data and
   verifying signatures.
 """
+
 import logging
 import subprocess  # nosec
 import time
 
-from securesystemslib import exceptions, formats
-from securesystemslib.gpg.common import (
+from securesystemslib import exceptions
+from securesystemslib._gpg.common import (
     get_pubkey_bundle,
     parse_signature_packet,
 )
-from securesystemslib.gpg.constants import (
+from securesystemslib._gpg.constants import (
     FULLY_SUPPORTED_MIN_VERSION,
     GPG_TIMEOUT,
     NO_GPG_MSG,
     SHA256,
     gpg_export_pubkey_command,
     gpg_sign_command,
     have_gpg,
 )
-from securesystemslib.gpg.exceptions import CommandError, KeyExpirationError
-from securesystemslib.gpg.handlers import SIGNATURE_HANDLERS
-from securesystemslib.gpg.rsa import CRYPTO
+from securesystemslib._gpg.exceptions import KeyExpirationError
+from securesystemslib._gpg.handlers import SIGNATURE_HANDLERS
+from securesystemslib._gpg.rsa import CRYPTO
 
 log = logging.getLogger(__name__)
 
 NO_CRYPTO_MSG = "GPG support requires the cryptography library"
 
 
 def create_signature(content, keyid=None, homedir=None, timeout=GPG_TIMEOUT):
     """
     <Purpose>
       Calls the gpg command line utility to sign the passed content with the key
       identified by the passed keyid from the gpg keyring at the passed homedir.
 
       The executed base command is defined in
-      securesystemslib.gpg.constants.gpg_sign_command.
+      securesystemslib._gpg.constants.gpg_sign_command.
 
       NOTE: On not fully supported versions of GPG, i.e. versions below
-      securesystemslib.gpg.constants.FULLY_SUPPORTED_MIN_VERSION the returned
+      securesystemslib._gpg.constants.FULLY_SUPPORTED_MIN_VERSION the returned
       signature does not contain the full keyid. As a work around, we export the
       public key bundle identified by the short keyid to compute the full keyid
       and add it to the returned signature.
 
     <Arguments>
       content:
               The content to be signed. (bytes)
@@ -68,52 +69,45 @@
       homedir: (optional)
               Path to the gpg keyring. If not passed the default keyring is used.
 
       timeout (optional):
               gpg command timeout in seconds. Default is 10.
 
     <Exceptions>
-      securesystemslib.exceptions.FormatError:
-              If the keyid was passed and does not match
-              securesystemslib.formats.KEYID_SCHEMA
 
       ValueError:
               If the gpg command failed to create a valid signature.
 
       OSError:
-              If the gpg command is not present or non-executable.
+              If the gpg command is not present, or non-executable,
+              or returned a non-zero exit code
 
       securesystemslib.exceptions.UnsupportedLibraryError:
               If the gpg command is not available, or
               the cryptography library is not installed.
 
-      securesystemslib.gpg.exceptions.CommandError:
-              If the gpg command returned a non-zero exit code
-
-      securesystemslib.gpg.exceptions.KeyNotFoundError:
+      securesystemslib._gpg.exceptions.KeyNotFoundError:
               If the used gpg version is not fully supported
               and no public key can be found for short keyid.
 
     <Side Effects>
       None.
 
     <Returns>
-      The created signature in the format:
-      securesystemslib.formats.GPG_SIGNATURE_SCHEMA.
+      A signature dict.
 
     """
     if not have_gpg():  # pragma: no cover
         raise exceptions.UnsupportedLibraryError(NO_GPG_MSG)
 
     if not CRYPTO:  # pragma: no cover
         raise exceptions.UnsupportedLibraryError(NO_CRYPTO_MSG)
 
     keyarg = ""
     if keyid:
-        formats.KEYID_SCHEMA.check_match(keyid)
         keyarg = (
             "--local-user {}".format(  # pylint: disable=consider-using-f-string
                 keyid
             )
         )
 
     homearg = ""
@@ -134,15 +128,15 @@
         timeout=timeout,
     )
 
     # TODO: It's suggested to take a look at `--status-fd` for proper error
     # reporting, as there is no clear distinction between the return codes
     # https://lists.gnupg.org/pipermail/gnupg-devel/2005-December/022559.html
     if gpg_process.returncode != 0:
-        raise CommandError(
+        raise OSError(
             "Command '{}' returned "  # pylint: disable=consider-using-f-string
             "non-zero exit status '{}', stderr was:\n{}.".format(
                 gpg_process.args,
                 gpg_process.returncode,
                 gpg_process.stderr.decode(),
             )
         )
@@ -206,26 +200,24 @@
       keyid.
 
       The function selects the appropriate verification algorithm (rsa or dsa)
       based on the "type" field in the passed public key object.
 
     <Arguments>
       signature_object:
-              A signature object in the format:
-              securesystemslib.formats.GPG_SIGNATURE_SCHEMA
+              A signature dict.
 
       pubkey_info:
-              A public key object in the format:
-              securesystemslib.formats.GPG_PUBKEY_SCHEMA
+              A public key dict.
 
       content:
               The content to be verified. (bytes)
 
     <Exceptions>
-      securesystemslib.gpg.exceptions.KeyExpirationError:
+      securesystemslib._gpg.exceptions.KeyExpirationError:
               if the passed public key has expired
 
       securesystemslib.exceptions.UnsupportedLibraryError:
               if the cryptography module is unavailable
 
     <Side Effects>
       None.
@@ -233,17 +225,14 @@
     <Returns>
       True if signature verification passes, False otherwise.
 
     """
     if not CRYPTO:  # pragma: no cover
         raise exceptions.UnsupportedLibraryError(NO_CRYPTO_MSG)
 
-    formats.GPG_PUBKEY_SCHEMA.check_match(pubkey_info)
-    formats.GPG_SIGNATURE_SCHEMA.check_match(signature_object)
-
     handler = SIGNATURE_HANDLERS[pubkey_info["type"]]
     sig_keyid = signature_object["keyid"]
 
     verification_key = pubkey_info
 
     # If the keyid on the signature matches a subkey of the passed key,
     # we use that subkey for verification instead of the master key.
@@ -265,46 +254,37 @@
     )
 
 
 def export_pubkey(keyid, homedir=None, timeout=GPG_TIMEOUT):
     """Exports a public key from a GnuPG keyring.
 
     Arguments:
-      keyid: An OpenPGP keyid in KEYID_SCHEMA format.
+      keyid: An OpenPGP keyid..
       homedir (optional): A path to the GnuPG home directory. If not set the
           default GnuPG home directory is used.
       timeout (optional): gpg command timeout in seconds. Default is 10.
 
     Raises:
-      ValueError: Keyid is not a string.
       UnsupportedLibraryError: The gpg command or pyca/cryptography are not
           available.
       KeyNotFoundError: No key or subkey was found for that keyid.
 
     Side Effects:
       Calls system gpg command in a subprocess.
 
     Returns:
-      An OpenPGP public key object in GPG_PUBKEY_SCHEMA format.
+      An OpenPGP public key dict.
 
     """
     if not have_gpg():  # pragma: no cover
         raise exceptions.UnsupportedLibraryError(NO_GPG_MSG)
 
     if not CRYPTO:  # pragma: no cover
         raise exceptions.UnsupportedLibraryError(NO_CRYPTO_MSG)
 
-    if not formats.KEYID_SCHEMA.matches(keyid):
-        # FIXME: probably needs smarter parsing of what a valid keyid is so as to
-        # not export more than one pubkey packet.
-        raise ValueError(
-            "we need to export an individual key. Please provide a "  # pylint: disable=consider-using-f-string
-            " valid keyid! Keyid was '{}'.".format(keyid)
-        )
-
     homearg = ""
     if homedir:
         homearg = (
             "--homedir {}".format(  # pylint: disable=consider-using-f-string
                 homedir
             ).replace("\\", "/")
         )
@@ -325,15 +305,15 @@
     return key_bundle
 
 
 def export_pubkeys(keyids, homedir=None, timeout=GPG_TIMEOUT):
     """Exports multiple public keys from a GnuPG keyring.
 
     Arguments:
-      keyids: A list of OpenPGP keyids in KEYID_SCHEMA format.
+      keyids: A list of OpenPGP keyids.
       homedir (optional): A path to the GnuPG home directory. If not set the
           default GnuPG home directory is used.
       timeout (optional): gpg command timeout in seconds. Default is 10.
 
     Raises:
       TypeError: Keyids is not iterable.
       ValueError: A Keyid is not a string.
@@ -341,15 +321,15 @@
           available.
       KeyNotFoundError: No key or subkey was found for that keyid.
 
     Side Effects:
       Calls system gpg command in a subprocess.
 
     Returns:
-      A dict of OpenPGP public key objects in GPG_PUBKEY_SCHEMA format as values,
+      A dict of OpenPGP public key dicts as values,
       and their keyids as dict keys.
 
 
     """
     public_key_dict = {}
     for gpg_keyid in keyids:
         public_key = export_pubkey(gpg_keyid, homedir=homedir, timeout=timeout)
```

### Comparing `securesystemslib-0.31.0/securesystemslib/gpg/handlers.py` & `securesystemslib-1.0.0/securesystemslib/_gpg/handlers.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   See LICENSE for licensing information.
 
 <Purpose>
   Provides links from signatures/algorithms to modules implementing
   the signature verification and key parsing.
 """
 
-from securesystemslib.gpg import dsa, eddsa, rsa
+from securesystemslib._gpg import dsa, eddsa, rsa
 
 # See section 9.1. (public-key algorithms) of RFC4880 (-bis8)
 SUPPORTED_SIGNATURE_ALGORITHMS = {
     0x01: {"type": "rsa", "method": "pgp+rsa-pkcsv1.5", "handler": rsa},
     0x11: {"type": "dsa", "method": "pgp+dsa-fips-180-2", "handler": dsa},
     0x16: {"type": "eddsa", "method": "pgp+eddsa-ed25519", "handler": eddsa},
 }
```

### Comparing `securesystemslib-0.31.0/securesystemslib/gpg/rsa.py` & `securesystemslib-1.0.0/securesystemslib/_gpg/rsa.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,61 +10,56 @@
 
 <Copyright>
   See LICENSE for licensing information.
 
 <Purpose>
   RSA-specific handling routines for signature verification and key parsing
 """
+
 import binascii
 
 CRYPTO = True
 NO_CRYPTO_MSG = "RSA key support for GPG requires the cryptography library"
 try:
     from cryptography.exceptions import InvalidSignature
     from cryptography.hazmat import backends
     from cryptography.hazmat.primitives.asymmetric import padding, rsa, utils
 except ImportError:
     CRYPTO = False
 
 # pylint: disable=wrong-import-position
-from securesystemslib import exceptions, formats
-from securesystemslib.gpg import util as gpg_util
-from securesystemslib.gpg.exceptions import PacketParsingError
+from securesystemslib import exceptions
+from securesystemslib._gpg import util as gpg_util
+from securesystemslib._gpg.exceptions import PacketParsingError
 
 # pylint: enable=wrong-import-position
 
 
 def create_pubkey(pubkey_info):
     """
     <Purpose>
       Create and return an RSAPublicKey object from the passed pubkey_info
       using pyca/cryptography.
 
     <Arguments>
       pubkey_info:
-              The RSA pubkey info dictionary as specified by
-              securesystemslib.formats.GPG_RSA_PUBKEY_SCHEMA
+              An RSA pubkey dict.
 
     <Exceptions>
-      securesystemslib.exceptions.FormatError if
-        pubkey_info does not match securesystemslib.formats.GPG_RSA_PUBKEY_SCHEMA
-
       securesystemslib.exceptions.UnsupportedLibraryError if
         the cryptography module is unavailable
 
     <Returns>
       A cryptography.hazmat.primitives.asymmetric.rsa.RSAPublicKey based on the
       passed pubkey_info.
 
     """
     if not CRYPTO:  # pragma: no cover
         raise exceptions.UnsupportedLibraryError(NO_CRYPTO_MSG)
 
-    formats.GPG_RSA_PUBKEY_SCHEMA.check_match(pubkey_info)
-
     e = int(pubkey_info["keyval"]["public"]["e"], 16)
     n = int(pubkey_info["keyval"]["public"]["n"], 16)
     pubkey = rsa.RSAPublicNumbers(e, n).public_key(backends.default_backend())
 
     return pubkey
 
 
@@ -75,24 +70,22 @@
 
     <Arguments>
       data:
              the RFC4880-encoded public key parameters data buffer as described
              in the fifth paragraph of section 5.5.2.
 
     <Exceptions>
-      securesystemslib.gpg.exceptions.PacketParsingError:
+      securesystemslib._gpg.exceptions.PacketParsingError:
              if the public key parameters are malformed
 
     <Side Effects>
       None.
 
     <Returns>
-      The parsed RSA public key in the format
-      securesystemslib.formats.GPG_RSA_PUBKEY_SCHEMA.
-
+      An RSA public key dict.
     """
     ptr = 0
 
     modulus_length = gpg_util.get_mpi_length(data[ptr : ptr + 2])
     ptr += 2
     modulus = data[ptr : ptr + modulus_length]
     if len(modulus) != modulus_length:  # pragma: no cover
@@ -118,15 +111,15 @@
 
     <Arguments>
       data:
              the RFC4880-encoded signature data buffer as described
              in the third paragraph of section 5.2.2.
 
     <Exceptions>
-      securesystemslib.gpg.exceptions.PacketParsingError:
+      securesystemslib._gpg.exceptions.PacketParsingError:
              if the public key parameters are malformed
 
     <Side Effects>
       None.
 
     <Returns>
       The decoded signature buffer
@@ -146,70 +139,60 @@
     """
     <Purpose>
       Verify the passed signature against the passed content with the passed
       RSA public key using pyca/cryptography.
 
     <Arguments>
       signature_object:
-              A signature dictionary as specified by
-              securesystemslib.formats.GPG_SIGNATURE_SCHEMA
+              A signature dict.
 
       pubkey_info:
-              The RSA public key info dictionary as specified by
-              securesystemslib.formats.GPG_RSA_PUBKEY_SCHEMA
+              The RSA public key dict.
 
       content:
               The signed bytes against which the signature is verified
 
       hash_algorithm_id:
-              one of SHA1, SHA256, SHA512 (see securesystemslib.gpg.constants)
+              one of SHA1, SHA256, SHA512 (see securesystemslib._gpg.constants)
               used to verify the signature
               NOTE: Overrides any hash algorithm specification in "pubkey_info"'s
               "hashes" or "method" fields.
 
     <Exceptions>
-      securesystemslib.exceptions.FormatError if:
-        signature_object does not match
-        securesystemslib.formats.GPG_SIGNATURE_SCHEMA,
-        pubkey_info does not match securesystemslib.formats.GPG_RSA_PUBKEY_SCHEMA
-
       securesystemslib.exceptions.UnsupportedLibraryError if:
         the cryptography module is unavailable
 
       ValueError:
         if the passed hash_algorithm_id is not supported (see
-        securesystemslib.gpg.util.get_hashing_class)
+        securesystemslib._gpg.util.get_hashing_class)
 
     <Returns>
       True if signature verification passes and False otherwise
 
     """
     if not CRYPTO:  # pragma: no cover
         raise exceptions.UnsupportedLibraryError(NO_CRYPTO_MSG)
 
-    formats.GPG_SIGNATURE_SCHEMA.check_match(signature_object)
-    formats.GPG_RSA_PUBKEY_SCHEMA.check_match(pubkey_info)
-
     hasher = gpg_util.get_hashing_class(hash_algorithm_id)
 
     pubkey_object = create_pubkey(pubkey_info)
 
     # zero-pad the signature due to a discrepancy between the openssl backend
     # and the gnupg interpretation of PKCSv1.5. Read more at:
     # https://github.com/in-toto/in-toto/issues/171#issuecomment-440039256
     # we are skipping this if on the tests because well, how would one test this
     # deterministically.
     pubkey_length = len(pubkey_info["keyval"]["public"]["n"])
     signature_length = len(signature_object["signature"])
     if pubkey_length != signature_length:  # pragma: no cover
         zero_pad = "0" * (pubkey_length - signature_length)
-        signature_object[
-            "signature"
-        ] = "{}{}".format(  # pylint: disable=consider-using-f-string
-            zero_pad, signature_object["signature"]
+        signature_object["signature"] = (
+            "{}{}".format(  # pylint: disable=consider-using-f-string
+                zero_pad, signature_object["signature"]
+            )
         )
 
     digest = gpg_util.hash_object(
         binascii.unhexlify(signature_object["other_headers"]), hasher(), content
     )
 
     try:
```

### Comparing `securesystemslib-0.31.0/securesystemslib/gpg/util.py` & `securesystemslib-1.0.0/securesystemslib/_gpg/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,31 @@
 
 <Copyright>
   See LICENSE for licensing information.
 
 <Purpose>
   general-purpose utilities for binary data handling and pgp data parsing
 """
+
 import binascii
 import logging
 import struct
 
 CRYPTO = True
 NO_CRYPTO_MSG = "gpg.utils requires the cryptography library"
 try:
     from cryptography.hazmat import backends
     from cryptography.hazmat.primitives import hashes as hashing
 except ImportError:
     CRYPTO = False
 
 # pylint: disable=wrong-import-position
 from securesystemslib import exceptions
-from securesystemslib.gpg import constants
-from securesystemslib.gpg.exceptions import PacketParsingError
+from securesystemslib._gpg import constants
+from securesystemslib._gpg.exceptions import PacketParsingError
 
 log = logging.getLogger(__name__)
 
 
 def get_mpi_length(data):
     """
     <Purpose>
@@ -108,19 +109,19 @@
 
     <Arguments>
       data:
               An RFC4880 packet as described in section 4.2 of the rfc.
 
       expected_type: (optional)
               Used to error out if the packet does not have the expected
-              type. See securesystemslib.gpg.constants.PACKET_TYPE_* for
+              type. See securesystemslib._gpg.constants.PACKET_TYPE_* for
               available types.
 
     <Exceptions>
-      securesystemslib.gpg.exceptions.PacketParsingError
+      securesystemslib._gpg.exceptions.PacketParsingError
               If the new format packet length encodes a partial body length
               If the old format packet length encodes an indeterminate length
               If header or body length could not be determined
               If the expected_type was passed and does not match the packet type
 
       IndexError
               If the passed data is incomplete
@@ -310,15 +311,15 @@
     """
     <Purpose>
       Return a pyca/cryptography hashing class reference for the passed RFC4880
       hash algorithm ID.
 
     <Arguments>
       hash_algorithm_id:
-              one of SHA1, SHA256, SHA512 (see securesystemslib.gpg.constants)
+              one of SHA1, SHA256, SHA512 (see securesystemslib._gpg.constants)
 
     <Exceptions>
       ValueError
               if the passed hash_algorithm_id is not supported.
 
     <Returns>
       A pyca/cryptography hashing class
```

### Comparing `securesystemslib-0.31.0/securesystemslib/signer/__init__.py` & `securesystemslib-1.0.0/securesystemslib/signer/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 The Signer API
 
 This module provides extensible interfaces for public keys and signers:
 Some implementations are provided by default but more can be added by users.
 """
+
 from securesystemslib.signer._aws_signer import AWSSigner
 from securesystemslib.signer._azure_signer import AzureSigner
 from securesystemslib.signer._crypto_signer import CryptoSigner
 from securesystemslib.signer._gcp_signer import GCPSigner
 from securesystemslib.signer._gpg_signer import GPGKey, GPGSigner
 from securesystemslib.signer._hsm_signer import HSMSigner
 from securesystemslib.signer._key import KEY_FOR_TYPE_AND_SCHEME, Key, SSlibKey
@@ -19,26 +20,26 @@
 )
 from securesystemslib.signer._sigstore_signer import SigstoreKey, SigstoreSigner
 from securesystemslib.signer._spx_signer import (
     SpxKey,
     SpxSigner,
     generate_spx_key_pair,
 )
-from securesystemslib.signer._sslib_signer import SSlibSigner
+from securesystemslib.signer._vault_signer import VaultSigner
 
 # Register supported private key uri schemes and the Signers implementing them
 SIGNER_FOR_URI_SCHEME.update(
     {
-        SSlibSigner.ENVVAR_URI_SCHEME: SSlibSigner,
-        SSlibSigner.FILE_URI_SCHEME: SSlibSigner,
+        CryptoSigner.SCHEME: CryptoSigner,
         GCPSigner.SCHEME: GCPSigner,
         HSMSigner.SCHEME: HSMSigner,
         GPGSigner.SCHEME: GPGSigner,
         AzureSigner.SCHEME: AzureSigner,
         AWSSigner.SCHEME: AWSSigner,
+        VaultSigner.SCHEME: VaultSigner,
     }
 )
 
 # Signers with currently unstable metadata formats, not supported by default:
 #   SigstoreSigner,
 #   SpxSigner (also does not yet support private key uri scheme)
```

### Comparing `securesystemslib-0.31.0/securesystemslib/signer/_aws_signer.py` & `securesystemslib-1.0.0/securesystemslib/signer/_aws_signer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Signer implementation for AWS Key Management Service"""
 
 import logging
-from typing import Optional, Tuple
+from typing import List, Optional, Tuple
 from urllib import parse
 
-import securesystemslib.hash as sslib_hash
-from securesystemslib import exceptions
-from securesystemslib.exceptions import UnsupportedLibraryError
+from securesystemslib.exceptions import (
+    UnsupportedAlgorithmError,
+    UnsupportedLibraryError,
+)
 from securesystemslib.signer._key import Key, SSlibKey
 from securesystemslib.signer._signer import SecretsHandler, Signature, Signer
 from securesystemslib.signer._utils import compute_default_keyid
 
 logger = logging.getLogger(__name__)
 
 AWS_IMPORT_ERROR = None
@@ -54,23 +55,40 @@
         BotoCoreError: Errors from the botocore.exceptions library.
         ClientError: Errors related to AWS KMS client.
         UnsupportedLibraryError: If necessary libraries for AWS KMS are not available.
     """
 
     SCHEME = "awskms"
 
+    # Ordered dict of securesystemslib schemes to aws signing algorithms
+    # NOTE: the order matters when choosing a default (see _get_default_scheme)
+    aws_algos = {
+        "ecdsa-sha2-nistp256": "ECDSA_SHA_256",
+        "ecdsa-sha2-nistp384": "ECDSA_SHA_384",
+        # "ecdsa-sha2-nistp521": "ECDSA_SHA_512", # FIXME: needs SSlibKey support
+        "rsassa-pss-sha256": "RSASSA_PSS_SHA_256",
+        "rsassa-pss-sha384": "RSASSA_PSS_SHA_384",
+        "rsassa-pss-sha512": "RSASSA_PSS_SHA_512",
+        "rsa-pkcs1v15-sha256": "RSASSA_PKCS1_V1_5_SHA_256",
+        "rsa-pkcs1v15-sha384": "RSASSA_PKCS1_V1_5_SHA_384",
+        "rsa-pkcs1v15-sha512": "RSASSA_PKCS1_V1_5_SHA_512",
+    }
+
     def __init__(self, aws_key_id: str, public_key: Key):
         if AWS_IMPORT_ERROR:
             raise UnsupportedLibraryError(AWS_IMPORT_ERROR)
 
-        self.hash_algorithm = self._get_hash_algorithm(public_key)
         self.aws_key_id = aws_key_id
-        self.public_key = public_key
+        self._public_key = public_key
         self.client = boto3.client("kms")
-        self.aws_algo = self._get_aws_signing_algo(self.public_key.scheme)
+        self.aws_algo = self.aws_algos[self.public_key.scheme]
+
+    @property
+    def public_key(self) -> Key:
+        return self._public_key
 
     @classmethod
     def from_priv_key_uri(
         cls,
         priv_key_uri: str,
         public_key: Key,
         secrets_handler: Optional[SecretsHandler] = None,
@@ -79,158 +97,121 @@
 
         if uri.scheme != cls.SCHEME:
             raise ValueError(f"AWSSigner does not support {priv_key_uri}")
 
         return cls(uri.path, public_key)
 
     @classmethod
-    def import_(cls, aws_key_id: str, local_scheme: str) -> Tuple[str, Key]:
+    def _get_default_scheme(cls, supported_by_key: List[str]) -> Optional[str]:
+        # Iterate over supported AWS algorithms, pick the **first** that is also
+        # supported by the key, and return the related securesystemslib scheme.
+        for scheme, algo in cls.aws_algos.items():
+            if algo in supported_by_key:
+                return scheme
+        return None
+
+    @staticmethod
+    def _get_keytype_for_scheme(scheme: str) -> str:
+        if scheme.startswith("ecdsa"):
+            return "ecdsa"
+        if scheme.startswith("rsa"):
+            return "rsa"
+        raise RuntimeError
+
+    @classmethod
+    def import_(
+        cls, aws_key_id: str, local_scheme: Optional[str] = None
+    ) -> Tuple[str, Key]:
         """Loads a key and signer details from AWS KMS.
 
         Returns the private key uri and the public key. This method should only
         be called once per key: the uri and Key should be stored for later use.
 
         Arguments:
             aws_key_id (str): AWS KMS key ID.
-            local_scheme (str): Local scheme to use.
+            local_scheme (Optional[str]): The Secure Systems Library RSA or ECDSA scheme.
+            Defaults to 'rsassa-pss-sha256' if not provided and RSA.
 
         Returns:
             Tuple[str, Key]: A tuple where the first element is a string
             representing the private key URI, and the second element is an
             instance of the public key.
 
         Raises:
             UnsupportedAlgorithmError: If the AWS KMS signing algorithm is
             unsupported.
-            BotoCoreError: Errors from the botocore.exceptions library.
+            BotoCoreError: Errors from the botocore library.
             ClientError: Errors related to AWS KMS client.
         """
         if AWS_IMPORT_ERROR:
             raise UnsupportedLibraryError(AWS_IMPORT_ERROR)
 
+        if local_scheme:
+            if local_scheme not in cls.aws_algos:
+                raise ValueError(f"Unsupported scheme '{local_scheme}'")
+
         client = boto3.client("kms")
         request = client.get_public_key(KeyId=aws_key_id)
+        key_algos = request["SigningAlgorithms"]
+
+        if local_scheme:
+            if cls.aws_algos[local_scheme] not in key_algos:
+                raise UnsupportedAlgorithmError(
+                    f"Unsupported scheme '{local_scheme}' for AWS key"
+                )
+
+        else:
+            local_scheme = cls._get_default_scheme(key_algos)
+            if not local_scheme:
+                raise UnsupportedAlgorithmError(
+                    f"Unsupported AWS key algorithms: {key_algos}"
+                )
+
+        keytype = cls._get_keytype_for_scheme(local_scheme)
+
         kms_pubkey = serialization.load_der_public_key(request["PublicKey"])
 
         public_key_pem = kms_pubkey.public_bytes(
             encoding=serialization.Encoding.PEM,
             format=serialization.PublicFormat.SubjectPublicKeyInfo,
         ).decode("utf-8")
-        try:
-            keytype = cls._get_keytype_for_scheme(local_scheme)
-        except KeyError as e:
-            raise exceptions.UnsupportedAlgorithmError(
-                f"{local_scheme} is not a supported signing algorithm"
-            ) from e
 
         keyval = {"public": public_key_pem}
         keyid = compute_default_keyid(keytype, local_scheme, keyval)
         public_key = SSlibKey(keyid, keytype, local_scheme, keyval)
         return f"{cls.SCHEME}:{aws_key_id}", public_key
 
-    @staticmethod
-    def _get_keytype_for_scheme(
-        scheme: str,
-    ) -> str:
-        """Returns the Secure Systems Library key type.
-
-        Arguments:
-            (str): The Secure Systems Library scheme.
-
-        Returns:
-            str: The Secure Systems Library key type.
-        """
-        keytype_for_scheme = {
-            "ecdsa-sha2-nistp256": "ecdsa",
-            "ecdsa-sha2-nistp384": "ecdsa",
-            "ecdsa-sha2-nistp512": "ecdsa",
-            "rsassa-pss-sha256": "rsa",
-            "rsassa-pss-sha384": "rsa",
-            "rsassa-pss-sha512": "rsa",
-            "rsa-pkcs1v15-sha256": "rsa",
-            "rsa-pkcs1v15-sha384": "rsa",
-            "rsa-pkcs1v15-sha512": "rsa",
-        }
-        return keytype_for_scheme[scheme]
-
-    @staticmethod
-    def _get_aws_signing_algo(
-        scheme: str,
-    ) -> str:
-        """Returns AWS signing algorithm
-
-        Arguments:
-            scheme (str): The Secure Systems Library signing scheme.
-
-        Returns:
-            str: AWS signing scheme.
-        """
-        aws_signing_algorithms = {
-            "ecdsa-sha2-nistp256": "ECDSA_SHA_256",
-            "ecdsa-sha2-nistp384": "ECDSA_SHA_384",
-            "ecdsa-sha2-nistp512": "ECDSA_SHA_512",
-            "rsassa-pss-sha256": "RSASSA_PSS_SHA_256",
-            "rsassa-pss-sha384": "RSASSA_PSS_SHA_384",
-            "rsassa-pss-sha512": "RSASSA_PSS_SHA_512",
-            "rsa-pkcs1v15-sha256": "RSASSA_PKCS1_V1_5_SHA_256",
-            "rsa-pkcs1v15-sha384": "RSASSA_PKCS1_V1_5_SHA_384",
-            "rsa-pkcs1v15-sha512": "RSASSA_PKCS1_V1_5_SHA_512",
-        }
-        return aws_signing_algorithms[scheme]
-
-    @staticmethod
-    def _get_hash_algorithm(public_key: Key) -> str:
-        """Helper function to return payload hash algorithm used for this key
-
-        Arguments:
-            public_key (Key): Public key object
-
-        Returns:
-            str: Hash algorithm
-        """
-        if public_key.keytype == "rsa":
-            # hash algorithm is encoded as last scheme portion
-            algo = public_key.scheme.split("-")[-1]
-        if public_key.keytype in [
-            "ecdsa",
-            "ecdsa-sha2-nistp256",
-            "ecdsa-sha2-nistp384",
-        ]:
-            # nistp256 uses sha-256, nistp384 uses sha-384
-            bits = public_key.scheme.split("-nistp")[-1]
-            algo = f"sha{bits}"
-
-        # trigger UnsupportedAlgorithm if appropriate
-        _ = sslib_hash.digest(algo)
-        return algo
-
     def sign(self, payload: bytes) -> Signature:
         """Sign the payload with the AWS KMS key
 
+        This method sends the payload to AWS KMS, where it is signed using the specified
+        key and algorithm using the raw message type.
+
         Arguments:
-            payload: bytes to be signed.
+            payload (bytes): The payload to be signed.
 
         Raises:
-            BotoCoreError: Errors from the botocore.exceptions library.
-            ClientError: Errors related to AWS KMS client.
+            BotoCoreError, ClientError: If an error occurs during the signing process.
 
         Returns:
-            Signature.
+            Signature: A signature object containing the key ID and the signature.
         """
         try:
-            request = self.client.sign(
+            sign_request = self.client.sign(
                 KeyId=self.aws_key_id,
                 Message=payload,
                 MessageType="RAW",
                 SigningAlgorithm=self.aws_algo,
             )
 
-            hasher = sslib_hash.digest(self.hash_algorithm)
-            hasher.update(payload)
-            logger.debug("signing response %s", request)
-            response = request["Signature"]
-            logger.debug("signing response %s", response)
+            logger.debug("Signing response: %s", sign_request)
+            response = sign_request["Signature"]
+            logger.debug("Signature response: %s", response)
 
             return Signature(self.public_key.keyid, response.hex())
         except (BotoCoreError, ClientError) as e:
-            logger.error("Failed to sign with AWS KMS: %s", str(e))
+            logger.error(
+                "Failed to sign using AWS KMS key ID %s: %s",
+                self.aws_key_id,
+                str(e),
+            )
             raise e
```

### Comparing `securesystemslib-0.31.0/securesystemslib/signer/_azure_signer.py` & `securesystemslib-1.0.0/securesystemslib/signer/_azure_signer.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,19 @@
             )
             self.hash_algorithm = self._get_hash_algorithm(public_key)
         except UnsupportedKeyType as e:
             logger.info(
                 "Key %s has unsupported key type or unsupported elliptic curve"
             )
             raise e
-        self.public_key = public_key
+        self._public_key = public_key
+
+    @property
+    def public_key(self) -> Key:
+        return self._public_key
 
     @staticmethod
     def _get_key_vault_key(
         cred: "DefaultAzureCredential",
         vault_name: str,
         key_name: str,
     ) -> "KeyVaultKey":
```

### Comparing `securesystemslib-0.31.0/securesystemslib/signer/_crypto_signer.py` & `securesystemslib-1.0.0/securesystemslib/signer/_crypto_signer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Signer implementation for pyca/cryptography signing. """
 
 import logging
+import os
 from dataclasses import astuple, dataclass
-from typing import Any, Dict, Optional, Union
+from typing import Optional, Union
 from urllib import parse
 
 from securesystemslib.exceptions import UnsupportedLibraryError
 from securesystemslib.signer._key import Key, SSlibKey
 from securesystemslib.signer._signature import Signature
 from securesystemslib.signer._signer import SecretsHandler, Signer
 
@@ -22,15 +23,14 @@
     )
     from cryptography.hazmat.primitives.asymmetric.ed25519 import (
         Ed25519PrivateKey,
     )
     from cryptography.hazmat.primitives.asymmetric.padding import (
         MGF1,
         PSS,
-        AsymmetricPadding,
         PKCS1v15,
     )
     from cryptography.hazmat.primitives.asymmetric.rsa import (
         AsymmetricPadding,
         RSAPrivateKey,
     )
     from cryptography.hazmat.primitives.asymmetric.rsa import (
@@ -41,14 +41,17 @@
         SHA224,
         SHA256,
         SHA384,
         SHA512,
         HashAlgorithm,
     )
     from cryptography.hazmat.primitives.serialization import (
+        Encoding,
+        NoEncryption,
+        PrivateFormat,
         load_pem_private_key,
     )
 except ImportError:
     CRYPTO_IMPORT_ERROR = "'pyca/cryptography' library required"
 
 logger = logging.getLogger(__name__)
 
@@ -65,14 +68,19 @@
 
 
 @dataclass
 class _NoSignArgs:
     pass
 
 
+# for backwards compat: use when spec-deprecated keytype ecdsa-sha2-nistp256
+# should be accepted in addition to "ecdsa"
+_ECDSA_KEYTYPES = ["ecdsa", "ecdsa-sha2-nistp256"]
+
+
 def _get_hash_algorithm(name: str) -> "HashAlgorithm":
     """Helper to return hash algorithm for name."""
     algorithm: HashAlgorithm
     if name == "sha224":
         algorithm = SHA224()
     if name == "sha256":
         algorithm = SHA256()
@@ -99,32 +107,32 @@
 
 
 class CryptoSigner(Signer):
     """PYCA/cryptography Signer implementations.
 
     A CryptoSigner can be created from:
 
-        a. private key file -- ``Signer.from_priv_key_uri()``
-
-          URI has the format "file:<PATH>?encrypted=[true|false]", where
-          PATH is the path to a file with private key data in a standard
-          PEM/PKCS8 format.
+        a. private key file -- see ``Signer.from_priv_key_uri()``
 
-          A related public key must be passed.
+          This is the generic (not CryptoSigner specific) way to
+          create a signer: use this when you already have a private
+          key  (and a private key URI) you can use.
 
-          If  ``encrypted=true``, the optional secrets handler is expected to
-          return a decryption password.
+        b. newly generated key pair -- see ``CryptoSigner.generate_*()``
 
-        b. newly generated key pair -- ``CryptoSigner.generate_*()``
+          Use this when you need a brand new private key pair.
 
         c. existing pyca/cryptography private key object -- ``CryptoSigner()``
 
+          Use this if you need a brand new private key pair and option
+          b is not flexible enough for your case.
     """
 
-    FILE_URI_SCHEME = "file"
+    SCHEME = "file2"
+    PREFIX_ENV_VAR = "CRYPTO_SIGNER_PATH_PREFIX"
 
     def __init__(
         self,
         private_key: "PrivateKeyTypes",
         public_key: Optional[SSlibKey] = None,
     ):
         if CRYPTO_IMPORT_ERROR:
@@ -152,15 +160,15 @@
             padding_name, hash_name = public_key.scheme.split("-")[1:]
             hash_algo = _get_hash_algorithm(hash_name)
             padding = _get_rsa_padding(padding_name, hash_algo)
             self._sign_args = _RSASignArgs(padding, hash_algo)
             self._private_key = private_key
 
         elif (
-            public_key.keytype == "ecdsa"
+            public_key.keytype in _ECDSA_KEYTYPES
             and public_key.scheme == "ecdsa-sha2-nistp256"
         ):
             if not isinstance(private_key, EllipticCurvePrivateKey):
                 raise ValueError(f"invalid ecdsa key: {type(private_key)}")
 
             signature_algorithm = ECDSA(SHA256())
             self._sign_args = _ECDSASignArgs(signature_algorithm)
@@ -174,37 +182,31 @@
             self._private_key = private_key
 
         else:
             raise ValueError(
                 f"unsupported public key {public_key.keytype}/{public_key.scheme}"
             )
 
-        self.public_key = public_key
-
-    @classmethod
-    def from_securesystemslib_key(
-        cls, key_dict: Dict[str, Any]
-    ) -> "CryptoSigner":
-        """Factory to create CryptoSigner from securesystemslib private key dict."""
-        private = key_dict["keyval"]["private"]
-        public_key = SSlibKey.from_securesystemslib_key(key_dict)
-
-        private_key: PrivateKeyTypes
-        if public_key.keytype in ["rsa", "ecdsa"]:
-            private_key = load_pem_private_key(private.encode(), password=None)
-
-        elif public_key.keytype == "ed25519":
-            private_key = Ed25519PrivateKey.from_private_bytes(
-                bytes.fromhex(private)
-            )
-
-        else:
-            raise ValueError(f"unsupported keytype: {public_key.keytype}")
+        self._public_key = public_key
 
-        return CryptoSigner(private_key, public_key)
+    @property
+    def public_key(self) -> Key:
+        return self._public_key
+
+    @property
+    def private_bytes(self) -> bytes:
+        """Return the PEM encoded PKCS8 format private key as bytes
+
+        The return value can be used as file content when a Signer is loaded with
+        `Signer.from_priv_key_uri('file2:<FILEPATH>')`."""
+        return self._private_key.private_bytes(
+            encoding=Encoding.PEM,
+            format=PrivateFormat.PKCS8,
+            encryption_algorithm=NoEncryption(),
+        )
 
     @classmethod
     def from_priv_key_uri(
         cls,
         priv_key_uri: str,
         public_key: Key,
         secrets_handler: Optional[SecretsHandler] = None,
@@ -213,14 +215,21 @@
 
         Please refer to Signer.from_priv_key_uri() documentation.
 
         NOTE: pyca/cryptography is used to deserialize the key data. The
         expected (and tested) encoding/format is PEM/PKCS8. Other formats may
         but are not guaranteed to work.
 
+        URI has the format "file2:<PATH>", where PATH is a filesystem path to the
+        private key file. If CRYPTO_SIGNER_PATH_PREFIX environment variable
+        is set, the private key will be read from
+        ``CRYPTO_SIGNER_PATH_PREFIX + <SEPARATOR> + PATH``. The purpose of this
+        is to allow PATH to only encode an identifier (e.g. filename) while allowing
+        the signing system to store the private keys whereever it wants at runtime.
+
         Additionally raises:
             UnsupportedLibraryError: pyca/cryptography not installed
             OSError: file cannot be read
             ValueError: various errors passed arguments
             ValueError, TypeError, \
                     cryptography.exceptions.UnsupportedAlgorithm:
                 pyca/cryptography deserialization failed
@@ -230,33 +239,29 @@
             raise UnsupportedLibraryError(CRYPTO_IMPORT_ERROR)
 
         if not isinstance(public_key, SSlibKey):
             raise ValueError(f"Expected SSlibKey for {priv_key_uri}")
 
         uri = parse.urlparse(priv_key_uri)
 
-        if uri.scheme != cls.FILE_URI_SCHEME:
+        if uri.scheme != cls.SCHEME:
             raise ValueError(f"CryptoSigner does not support {priv_key_uri}")
 
-        params = dict(parse.parse_qsl(uri.query))
-
-        if "encrypted" not in params:
-            raise ValueError(f"{uri.scheme} requires 'encrypted' parameter")
-
-        secret = None
-        if params["encrypted"] != "false":
-            if not secrets_handler:
-                raise ValueError("encrypted key requires a secrets handler")
-
-            secret = secrets_handler("passphrase").encode()
-
-        with open(uri.path, "rb") as f:
-            private_pem = f.read()
+        prefix = os.environ.get(cls.PREFIX_ENV_VAR)
+        path = os.path.join(prefix, uri.path) if prefix else uri.path
+        try:
+            with open(path, "rb") as f:
+                private_pem = f.read()
+        except FileNotFoundError as e:
+            raise FileNotFoundError(
+                f"Private key not found in '{path}' (with ",
+                f"{cls.PREFIX_ENV_VAR}: {prefix}, path: {uri.path})",
+            ) from e
 
-        private_key = load_pem_private_key(private_pem, secret)
+        private_key = load_pem_private_key(private_pem, None)
         return CryptoSigner(private_key, public_key)
 
     @staticmethod
     def generate_ed25519(
         keyid: Optional[str] = None,
     ) -> "CryptoSigner":
         """Generate new key pair as "ed25519" signer.
```

### Comparing `securesystemslib-0.31.0/securesystemslib/signer/_gcp_signer.py` & `securesystemslib-1.0.0/securesystemslib/signer/_gcp_signer.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,17 +57,21 @@
 
     def __init__(self, gcp_keyid: str, public_key: Key):
         if GCP_IMPORT_ERROR:
             raise exceptions.UnsupportedLibraryError(GCP_IMPORT_ERROR)
 
         self.hash_algorithm = self._get_hash_algorithm(public_key)
         self.gcp_keyid = gcp_keyid
-        self.public_key = public_key
+        self._public_key = public_key
         self.client = kms.KeyManagementServiceClient()
 
+    @property
+    def public_key(self) -> Key:
+        return self._public_key
+
     @classmethod
     def from_priv_key_uri(
         cls,
         priv_key_uri: str,
         public_key: Key,
         secrets_handler: Optional[SecretsHandler] = None,
     ) -> "GCPSigner":
```

### Comparing `securesystemslib-0.31.0/securesystemslib/signer/_gpg_signer.py` & `securesystemslib-1.0.0/securesystemslib/signer/_gpg_signer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Signer implementation for OpenPGP """
 
 import logging
 from typing import Any, Dict, Optional, Tuple
 from urllib import parse
 
-from securesystemslib import exceptions, formats
-from securesystemslib.gpg import exceptions as gpg_exceptions
-from securesystemslib.gpg import functions as gpg
+from securesystemslib import exceptions
+from securesystemslib._gpg import constants as gpg_constants
+from securesystemslib._gpg import exceptions as gpg_exceptions
+from securesystemslib._gpg import functions as gpg
 from securesystemslib.signer._key import Key
 from securesystemslib.signer._signer import SecretsHandler, Signature, Signer
 
 logger = logging.getLogger(__name__)
 
 
 class GPGKey(Key):
@@ -48,18 +49,15 @@
                     self
                 ),
                 data,
             ):
                 raise exceptions.UnverifiedSignatureError(
                     f"Failed to verify signature by {self.keyid}"
                 )
-        except (
-            exceptions.FormatError,
-            exceptions.UnsupportedLibraryError,
-        ) as e:
+        except (exceptions.UnsupportedLibraryError,) as e:
             logger.info("Key %s failed to verify sig: %s", self.keyid, str(e))
             raise exceptions.VerificationError(
                 f"Unknown failure to verify signature by {self.keyid}"
             ) from e
 
 
 class GPGSigner(Signer):
@@ -89,15 +87,19 @@
 
     def __init__(
         self,
         public_key: Key,
         homedir: Optional[str] = None,
     ):
         self.homedir = homedir
-        self.public_key = public_key
+        self._public_key = public_key
+
+    @property
+    def public_key(self) -> Key:
+        return self._public_key
 
     @classmethod
     def from_priv_key_uri(
         cls,
         priv_key_uri: str,
         public_key: Key,
         secrets_handler: Optional[SecretsHandler] = None,
@@ -130,15 +132,15 @@
     @staticmethod
     def _key_to_legacy_dict(key: GPGKey) -> Dict[str, Any]:
         """Returns legacy dictionary representation of self."""
         return {
             "keyid": key.keyid,
             "type": key.keytype,
             "method": key.scheme,
-            "hashes": [formats.GPG_HASH_ALGORITHM_STRING],
+            "hashes": [gpg_constants.GPG_HASH_ALGORITHM_STRING],
             "keyval": key.keyval,
         }
 
     @staticmethod
     def _key_from_legacy_dict(key_dict: Dict[str, Any]) -> GPGKey:
         """Create GPGKey from legacy dictionary representation."""
         keyid = key_dict["keyid"]
@@ -161,64 +163,71 @@
             keyid: GnuPG local user signing key id.
             homedir: GnuPG home directory path. If not passed, the default homedir is
                     used.
 
         Raises:
             UnsupportedLibraryError: The gpg command or pyca/cryptography are
                 not available.
-            KeyNotFoundError: No key was found for the passed keyid.
+            ValueError: No key was found for the passed keyid.
 
         Returns:
             Tuple of private key uri and the public key.
 
         """
         uri = f"{cls.SCHEME}:{homedir or ''}"
 
-        raw_key = gpg.export_pubkey(keyid, homedir)
+        try:
+            raw_key = gpg.export_pubkey(keyid, homedir)
+
+        except gpg_exceptions.KeyNotFoundError as e:
+            raise ValueError(e) from e
+
         raw_keys = [raw_key] + list(raw_key.pop("subkeys", {}).values())
         keyids = []
 
         for key in raw_keys:
             if key["keyid"] == keyid:
                 # TODO: Raise here if key is expired, revoked, incapable, ...
                 public_key = cls._key_from_legacy_dict(key)
                 break
             keyids.append(key["keyid"])
 
         else:
-            raise gpg_exceptions.KeyNotFoundError(
+            raise ValueError(
                 f"No exact match found for passed keyid"
                 f" {keyid}, found: {keyids}."
             )
 
         return (uri, public_key)
 
     def sign(self, payload: bytes) -> Signature:
         """Signs payload with GnuPG.
 
         Arguments:
             payload: bytes to be signed.
 
         Raises:
-            ValueError: gpg command failed to create a valid signature.
-            OSError: gpg command is not present or non-executable.
+            ValueError: gpg command failed to create a valid signature, e.g.
+                because its keyid does not match the public key keyid.
+            OSError: gpg command is not present, or non-executable, or returned
+                a non-zero exit code.
             securesystemslib.exceptions.UnsupportedLibraryError: gpg command is not
                 available, or the cryptography library is not installed.
-            securesystemslib.gpg.exceptions.CommandError: gpg command returned a
-                non-zero exit code.
-            securesystemslib.gpg.exceptions.KeyNotFoundError: gpg version is not fully
-                supported.
 
         Returns:
             Signature.
 
         """
-        raw_sig = gpg.create_signature(
-            payload, self.public_key.keyid, self.homedir
-        )
+        try:
+            raw_sig = gpg.create_signature(
+                payload, self.public_key.keyid, self.homedir
+            )
+        except gpg_exceptions.KeyNotFoundError as e:
+            raise ValueError(e) from e
+
         if raw_sig["keyid"] != self.public_key.keyid:
             raise ValueError(
                 f"The signing key {raw_sig['keyid']} does not"
                 f" match the attached public key {self.public_key.keyid}."
             )
 
         return self._sig_from_legacy_dict(raw_sig)
```

### Comparing `securesystemslib-0.31.0/securesystemslib/signer/_hsm_signer.py` & `securesystemslib-1.0.0/securesystemslib/signer/_hsm_signer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """Hardware Security Module (HSM) Signer
 
 Uses PKCS#11/Cryptoki API to create signatures with HSMs (e.g. YubiKey) and to export
 the related public keys.
 
 """
+
 import binascii
 from contextlib import contextmanager
 from typing import Dict, Iterator, List, Optional, Tuple
 from urllib import parse
 
-from securesystemslib import KEY_TYPE_ECDSA
 from securesystemslib.exceptions import UnsupportedLibraryError
 from securesystemslib.hash import digest
 from securesystemslib.signer._key import Key, SSlibKey
 from securesystemslib.signer._signature import Signature
 from securesystemslib.signer._signer import SecretsHandler, Signer
 from securesystemslib.signer._utils import compute_default_keyid
 
+_KEY_TYPE_ECDSA = "ecdsa"
+
 # pylint: disable=wrong-import-position
 CRYPTO_IMPORT_ERROR = None
 try:
     from cryptography.hazmat.primitives import serialization
     from cryptography.hazmat.primitives.asymmetric.ec import (
         SECP256R1,
         SECP384R1,
@@ -139,17 +141,21 @@
             "ecdsa-sha2-nistp256",
             "ecdsa-sha2-nistp384",
         ]:
             raise ValueError(f"unsupported scheme {public_key.scheme}")
 
         self.hsm_keyid = hsm_keyid
         self.token_filter = token_filter
-        self.public_key = public_key
+        self._public_key = public_key
         self.pin_handler = pin_handler
 
+    @property
+    def public_key(self) -> Key:
+        return self._public_key
+
     @staticmethod
     def _find_pkcs_slot(filters: Dict[str, str]) -> int:
         """Return the PKCS slot with initialized token that matches filter
 
         Raises ValueError if more or less than 1 PKCS slot is found.
         """
         lib = PYKCS11LIB()
@@ -208,19 +214,21 @@
             [
                 (PyKCS11.CKA_CLASS, key_type),
                 (PyKCS11.CKA_KEY_TYPE, PyKCS11.CKK_ECDSA),
                 (PyKCS11.CKA_ID, (keyid,)),
             ]
         )
         if not keys:
-            raise ValueError(f"could not find {KEY_TYPE_ECDSA} key for {keyid}")
+            raise ValueError(
+                f"could not find {_KEY_TYPE_ECDSA} key for {keyid}"
+            )
 
         if len(keys) > 1:
             raise ValueError(
-                f"found more than one {KEY_TYPE_ECDSA} key for {keyid}"
+                f"found more than one {_KEY_TYPE_ECDSA} key for {keyid}"
             )
 
         return keys[0]
 
     @classmethod
     def _find_key_values(
         cls, session: "PyKCS11.Session", keyid: int
@@ -318,16 +326,16 @@
                 serialization.PublicFormat.SubjectPublicKeyInfo,
             )
             .decode()
         )
 
         keyval = {"public": public_pem}
         scheme = _SCHEME_FOR_CURVE[curve]
-        keyid = compute_default_keyid(KEY_TYPE_ECDSA, scheme, keyval)
-        key = SSlibKey(keyid, KEY_TYPE_ECDSA, scheme, keyval)
+        keyid = compute_default_keyid(_KEY_TYPE_ECDSA, scheme, keyval)
+        key = SSlibKey(keyid, _KEY_TYPE_ECDSA, scheme, keyval)
 
         return uri, key
 
     @classmethod
     def from_priv_key_uri(
         cls,
         priv_key_uri: str,
```

### Comparing `securesystemslib-0.31.0/securesystemslib/signer/_key.py` & `securesystemslib-1.0.0/securesystemslib/signer/_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Key interface and the default implementations"""
+
 import logging
 from abc import ABCMeta, abstractmethod
 from typing import Any, Dict, Optional, Tuple, Type, cast
 
 from securesystemslib._vendor.ed25519.ed25519 import (
     SignatureMismatch,
     checkvalid,
@@ -16,14 +17,16 @@
 from securesystemslib.signer._utils import compute_default_keyid
 
 CRYPTO_IMPORT_ERROR = None
 try:
     from cryptography.exceptions import InvalidSignature
     from cryptography.hazmat.primitives.asymmetric.ec import (
         ECDSA,
+        SECP256R1,
+        SECP384R1,
         EllipticCurvePublicKey,
     )
     from cryptography.hazmat.primitives.asymmetric.ed25519 import (
         Ed25519PublicKey,
     )
     from cryptography.hazmat.primitives.asymmetric.padding import (
         MGF1,
@@ -193,133 +196,107 @@
         """
         raise NotImplementedError
 
 
 class SSlibKey(Key):
     """Key implementation for RSA, Ed25519, ECDSA keys"""
 
-    def to_securesystemslib_key(self) -> Dict[str, Any]:
-        """Internal helper, returns a classic securesystemslib keydict.
-
-        .. deprecated:: 0.28.0
-            Please use ``CryptoSigner`` instead of securesystemslib keydicts.
-        """
-        return {
-            "keyid": self.keyid,
-            "keytype": self.keytype,
-            "scheme": self.scheme,
-            "keyval": self.keyval,
-        }
-
-    @classmethod
-    def from_securesystemslib_key(cls, key_dict: Dict[str, Any]) -> "SSlibKey":
-        """Constructor from classic securesystemslib keydict
-
-        .. deprecated:: 0.28.0
-            Please use ``CryptoSigner`` instead of securesystemslib keydicts.
-        """
-        # ensure possible private keys are not included in keyval
-        return SSlibKey(
-            key_dict["keyid"],
-            key_dict["keytype"],
-            key_dict["scheme"],
-            {"public": key_dict["keyval"]["public"]},
-        )
+    def __init__(
+        self,
+        keyid: str,
+        keytype: str,
+        scheme: str,
+        keyval: Dict[str, Any],
+        unrecognized_fields: Optional[Dict[str, Any]] = None,
+    ):
+        if "public" not in keyval or not isinstance(keyval["public"], str):
+            raise ValueError(f"public key string required for scheme {scheme}")
+        super().__init__(keyid, keytype, scheme, keyval, unrecognized_fields)
 
     @classmethod
     def from_dict(cls, keyid: str, key_dict: Dict[str, Any]) -> "SSlibKey":
         keytype, scheme, keyval = cls._from_dict(key_dict)
 
-        if "public" not in keyval or not isinstance(keyval["public"], str):
-            raise ValueError(f"public key string required for scheme {scheme}")
-
         # All fields left in the key_dict are unrecognized.
         return cls(keyid, keytype, scheme, keyval, key_dict)
 
     def to_dict(self) -> Dict[str, Any]:
         return self._to_dict()
 
-    def _from_pem(self) -> "PublicKeyTypes":
-        """Helper to load public key instance from PEM-formatted keyval.
-
-        # FIXME: Sounds like it's an SSlibKey factory, but isn't. Should think
-        of a better name or refactor _verify!
-        """
+    def _crypto_key(self) -> "PublicKeyTypes":
+        """Helper to get a `cryptography` public key for this SSlibKey."""
         public_bytes = self.keyval["public"].encode("utf-8")
         return load_pem_public_key(public_bytes)
 
     @staticmethod
-    def _get_keytype_for_crypto_key(public_key: "PublicKeyTypes") -> str:
-        """Helper to return keytype for pyca/cryptography public key."""
-        if isinstance(public_key, RSAPublicKey):
-            return "rsa"
+    def _from_crypto(public_key: "PublicKeyTypes") -> Tuple[str, str, str]:
+        """Return tuple of keytype, default scheme and serialized public key
+        value for the passed public key.
 
-        if isinstance(public_key, EllipticCurvePublicKey):
-            return "ecdsa"
+        Raise ValueError if public key is not supported.
+        """
 
-        if isinstance(public_key, Ed25519PublicKey):
-            return "ed25519"
+        def _raw() -> str:
+            return public_key.public_bytes(
+                encoding=Encoding.Raw, format=PublicFormat.Raw
+            ).hex()
+
+        def _pem() -> str:
+            return public_key.public_bytes(
+                encoding=Encoding.PEM, format=PublicFormat.SubjectPublicKeyInfo
+            ).decode()
 
-        raise ValueError(f"unsupported 'public_key' type {type(public_key)}")
+        if isinstance(public_key, RSAPublicKey):
+            return "rsa", "rsassa-pss-sha256", _pem()
 
-    @staticmethod
-    def _get_default_scheme(keytype: str) -> str:
-        """Helper to return default scheme for keytype."""
-        if keytype == "rsa":
-            return "rsassa-pss-sha256"
+        if isinstance(public_key, EllipticCurvePublicKey):
+            if isinstance(public_key.curve, SECP256R1):
+                return "ecdsa", "ecdsa-sha2-nistp256", _pem()
+
+            if isinstance(public_key.curve, SECP384R1):
+                return "ecdsa", "ecdsa-sha2-nistp384", _pem()
 
-        if keytype == "ecdsa":
-            return "ecdsa-sha2-nistp256"
+            raise ValueError(f"unsupported curve '{public_key.curve.name}'")
 
-        if keytype == "ed25519":
-            return "ed25519"
+        if isinstance(public_key, Ed25519PublicKey):
+            return "ed25519", "ed25519", _raw()
 
-        raise ValueError(f"unsupported 'keytype' {keytype}")
+        raise ValueError(f"unsupported key '{type(public_key)}'")
 
     @classmethod
     def from_crypto(
         cls,
         public_key: "PublicKeyTypes",
         keyid: Optional[str] = None,
         scheme: Optional[str] = None,
     ) -> "SSlibKey":
         """Create SSlibKey from pyca/cryptography public key.
 
         Args:
             public_key: pyca/cryptography public key object.
             keyid: Key identifier. If not passed, a default keyid is computed.
             scheme: SSlibKey signing scheme. Defaults are "rsassa-pss-sha256",
-                "ecdsa-sha2-nistp256", and "ed25519" according to the keytype
+                "ecdsa-sha2-nistp256", "ecdsa-sha2-nistp384" and "ed25519"
+                according to the keytype.
 
         Raises:
             UnsupportedLibraryError: pyca/cryptography not installed
             ValueError: Key type not supported
 
         Returns:
             SSlibKey
 
         """
         if CRYPTO_IMPORT_ERROR:
             raise UnsupportedLibraryError(CRYPTO_IMPORT_ERROR)
 
-        keytype = cls._get_keytype_for_crypto_key(public_key)
-        if not scheme:
-            scheme = cls._get_default_scheme(keytype)
-
-        if keytype in ["rsa", "ecdsa"]:
-            pem: bytes = public_key.public_bytes(
-                encoding=Encoding.PEM, format=PublicFormat.SubjectPublicKeyInfo
-            )
-            public_key_value = pem.decode()
+        keytype, default_scheme, public_key_value = cls._from_crypto(public_key)
 
-        else:  # ed25519
-            raw: bytes = public_key.public_bytes(
-                encoding=Encoding.Raw, format=PublicFormat.Raw
-            )
-            public_key_value = raw.hex()
+        if not scheme:
+            scheme = default_scheme
 
         keyval = {"public": public_key_value}
 
         if not keyid:
             keyid = compute_default_keyid(keytype, scheme, keyval)
 
         return SSlibKey(keyid, keytype, scheme, keyval)
@@ -360,49 +337,69 @@
             checkvalid(signature, data, public_bytes)
 
         except SignatureMismatch as e:
             raise UnverifiedSignatureError from e
 
     def _verify(self, signature: bytes, data: bytes) -> None:
         """Helper to verify signature using pyca/cryptography (default)."""
+
+        def _validate_type(key, type_):
+            if not isinstance(key, type_):
+                raise ValueError(f"bad key {key} for {self.scheme}")
+
+        def _validate_curve(key, curve):
+            if not isinstance(key.curve, curve):
+                raise ValueError(f"bad curve {key.curve} for {self.scheme}")
+
         try:
             key: PublicKeyTypes
-            if self.scheme in [
+            if self.keytype == "rsa" and self.scheme in [
                 "rsassa-pss-sha224",
                 "rsassa-pss-sha256",
                 "rsassa-pss-sha384",
                 "rsassa-pss-sha512",
                 "rsa-pkcs1v15-sha224",
                 "rsa-pkcs1v15-sha256",
                 "rsa-pkcs1v15-sha384",
                 "rsa-pkcs1v15-sha512",
             ]:
-                key = cast(RSAPublicKey, self._from_pem())
+                key = cast(RSAPublicKey, self._crypto_key())
+                _validate_type(key, RSAPublicKey)
                 padding_name, hash_name = self.scheme.split("-")[1:]
                 hash_algorithm = self._get_hash_algorithm(hash_name)
                 padding = self._get_rsa_padding(padding_name, hash_algorithm)
                 key.verify(signature, data, padding, hash_algorithm)
 
-            elif self.scheme in [
-                "ecdsa-sha2-nistp256",
-                "ecdsa-sha2-nistp384",
-            ]:
-                key = cast(EllipticCurvePublicKey, self._from_pem())
-                hash_name = f"sha{self.scheme[-3:]}"
-                hash_algorithm = self._get_hash_algorithm(hash_name)
-                signature_algorithm = ECDSA(hash_algorithm)
-                key.verify(signature, data, signature_algorithm)
+            elif (
+                self.keytype in ["ecdsa", "ecdsa-sha2-nistp256"]
+                and self.scheme == "ecdsa-sha2-nistp256"
+            ):
+                key = cast(EllipticCurvePublicKey, self._crypto_key())
+                _validate_type(key, EllipticCurvePublicKey)
+                _validate_curve(key, SECP256R1)
+                key.verify(signature, data, ECDSA(SHA256()))
+
+            elif (
+                self.keytype in ["ecdsa", "ecdsa-sha2-nistp384"]
+                and self.scheme == "ecdsa-sha2-nistp384"
+            ):
+                key = cast(EllipticCurvePublicKey, self._crypto_key())
+                _validate_type(key, EllipticCurvePublicKey)
+                _validate_curve(key, SECP384R1)
+                key.verify(signature, data, ECDSA(SHA384()))
 
-            elif self.scheme in ["ed25519"]:
+            elif self.keytype == "ed25519" and self.scheme == "ed25519":
                 public_bytes = bytes.fromhex(self.keyval["public"])
                 key = Ed25519PublicKey.from_public_bytes(public_bytes)
                 key.verify(signature, data)
 
             else:
-                raise ValueError(f"unknown scheme '{self.scheme}'")
+                raise ValueError(
+                    f"Unsupported public key {self.keytype}/{self.scheme}"
+                )
 
         except InvalidSignature as e:
             raise UnverifiedSignatureError from e
 
     def verify_signature(self, signature: Signature, data: bytes) -> None:
         try:
             if signature.keyid != self.keyid:
```

### Comparing `securesystemslib-0.31.0/securesystemslib/signer/_signature.py` & `securesystemslib-1.0.0/securesystemslib/signer/_signature.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/securesystemslib/signer/_signer.py` & `securesystemslib-1.0.0/securesystemslib/signer/_signer.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,45 +26,35 @@
 
 
 class Signer(metaclass=ABCMeta):
     """Signer interface that supports multiple signing implementations.
 
     Usage example::
 
-        signer = Signer.from_priv_key_uri("envvar:MYPRIVKEY", pub_key)
+        signer = Signer.from_priv_key_uri(uri, pub_key)
         sig = signer.sign(b"data")
 
     Note that signer implementations may raise errors (during both
     ``Signer.from_priv_key_uri()`` and ``Signer.sign()``) that are not
     documented here: examples could include network errors or file read errors.
     Applications should use generic try-except here if unexpected raises are
     not an option.
 
-    See ``SIGNER_FOR_URI_SCHEME`` for supported private key URI schemes. The
-    currently supported default schemes are:
-
-    * envvar: see ``SSlibSigner`` for details
-    * file: see ``SSlibSigner`` for details
+    See ``SIGNER_FOR_URI_SCHEME`` for supported private key URI schemes.
 
     Interactive applications may also define a secrets handler that allows
     asking for user secrets if they are needed::
 
         from getpass import getpass
 
         def sec_handler(secret_name:str) -> str:
             return getpass(f"Enter {secret_name}: ")
 
-        # user will not be asked for a passphrase for unencrypted key
-        uri = "file:keys/mykey?encrypted=false"
         signer = Signer.from_priv_key_uri(uri, pub_key, sec_handler)
 
-        # user will be asked for a passphrase for encrypted key
-        uri2 = "file:keys/myenckey?encrypted=true"
-        signer2 = Signer.from_priv_key_uri(uri2, pub_key2, sec_handler)
-
     Applications can provide their own Signer and Key implementations::
 
         from securesystemslib.signer import Signer, SIGNER_FOR_URI_SCHEME
         from mylib import MySigner
 
         SIGNER_FOR_URI_SCHEME[MySigner.MY_SCHEME] = MySigner
 
@@ -115,7 +105,16 @@
         if scheme not in SIGNER_FOR_URI_SCHEME:
             raise ValueError(f"Unsupported private key scheme {scheme}")
 
         signer = SIGNER_FOR_URI_SCHEME[scheme]
         return signer.from_priv_key_uri(
             priv_key_uri, public_key, secrets_handler
         )
+
+    @property
+    @abstractmethod
+    def public_key(self) -> Key:
+        """
+        Returns:
+            Public key the signer is based off.
+        """
+        raise NotImplementedError
```

### Comparing `securesystemslib-0.31.0/securesystemslib/signer/_sigstore_signer.py` & `securesystemslib-1.0.0/securesystemslib/signer/_sigstore_signer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 """Signer implementation for project sigstore.
 
+NOTE: SigstoreSigner and -Key are disabled temporarily around
+the Securesystemslib 1.0 release as the cyclic dependency
+(securesystemslib -> sigstore-python -> tuf -> securesystemslib)
+is problematic during API deprecations.
+See issue #781.
 """
 
 import io
 import logging
 from typing import Any, Dict, Optional, Tuple
 from urllib import parse
 
@@ -32,24 +37,32 @@
     considered stable in securesystemslib. They may change in future releases
     and may not be supported by other implementations.
     """
 
     DEFAULT_KEY_TYPE = "sigstore-oidc"
     DEFAULT_SCHEME = "Fulcio"
 
-    @classmethod
-    def from_dict(cls, keyid: str, key_dict: Dict[str, Any]) -> "SigstoreKey":
-        keytype, scheme, keyval = cls._from_dict(key_dict)
-
+    def __init__(
+        self,
+        keyid: str,
+        keytype: str,
+        scheme: str,
+        keyval: Dict[str, Any],
+        unrecognized_fields: Optional[Dict[str, Any]] = None,
+    ):
         for content in ["identity", "issuer"]:
             if content not in keyval or not isinstance(keyval[content], str):
                 raise ValueError(
                     f"{content} string required for scheme {scheme}"
                 )
+        super().__init__(keyid, keytype, scheme, keyval, unrecognized_fields)
 
+    @classmethod
+    def from_dict(cls, keyid: str, key_dict: Dict[str, Any]) -> "SigstoreKey":
+        keytype, scheme, keyval = cls._from_dict(key_dict)
         return cls(keyid, keytype, scheme, keyval, key_dict)
 
     def to_dict(self) -> Dict:
         return self._to_dict()
 
     def verify_signature(self, signature: Signature, data: bytes) -> None:
         # pylint: disable=import-outside-toplevel,import-error
@@ -127,19 +140,23 @@
     Raises:
         UnsupportedLibraryError: sigstore library not found.
     """
 
     SCHEME = "sigstore"
 
     def __init__(self, token: Any, public_key: Key):
-        self.public_key = public_key
+        self._public_key = public_key
         # token is of type sigstore.oidc.IdentityToken but the module should be usable
         # without sigstore so it's not annotated
         self._token = token
 
+    @property
+    def public_key(self) -> Key:
+        return self._public_key
+
     @classmethod
     def from_priv_key_uri(
         cls,
         priv_key_uri: str,
         public_key: Key,
         secrets_handler: Optional[SecretsHandler] = None,
     ) -> "SigstoreSigner":
```

### Comparing `securesystemslib-0.31.0/securesystemslib/signer/_spx_signer.py` & `securesystemslib-1.0.0/securesystemslib/signer/_spx_signer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Signer implementation for project SPHINCS+ post-quantum signature support.
 
 """
+
 import logging
 import os
 from typing import Any, Dict, Optional, Tuple
 
 from securesystemslib.exceptions import (
     UnsupportedLibraryError,
     UnverifiedSignatureError,
@@ -109,15 +110,19 @@
         public_key = signer.public_key
         public_key.verify_signature(signature, b"payload")
 
     """
 
     def __init__(self, private: bytes, public: SpxKey):
         self.private_key = private
-        self.public_key = public
+        self._public_key = public
+
+    @property
+    def public_key(self) -> Key:
+        return self._public_key
 
     @classmethod
     def from_priv_key_uri(
         cls,
         priv_key_uri: str,
         public_key: Key,
         secrets_handler: Optional[SecretsHandler] = None,
```

### Comparing `securesystemslib-0.31.0/securesystemslib/signer/_sslib_signer.py` & `securesystemslib-1.0.0/securesystemslib/signer/_vault_signer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,113 +1,135 @@
-"""Legacy signer default implementations"""
+"""Signer implementation for HashiCorp Vault (Transit secrets engine)"""
 
-import logging
-import os
-from typing import Dict, Optional
+from base64 import b64decode, b64encode
+from typing import Optional, Tuple
 from urllib import parse
 
-from securesystemslib import keys as sslib_keys
-from securesystemslib.signer._crypto_signer import CryptoSigner
+from securesystemslib.exceptions import UnsupportedLibraryError
 from securesystemslib.signer._key import Key, SSlibKey
-from securesystemslib.signer._signature import Signature
-from securesystemslib.signer._signer import SecretsHandler, Signer
+from securesystemslib.signer._signer import SecretsHandler, Signature, Signer
 
-logger = logging.getLogger(__name__)
+VAULT_IMPORT_ERROR = None
+try:
+    import hvac
+    from cryptography.hazmat.primitives.asymmetric.ed25519 import (
+        Ed25519PublicKey,
+    )
 
+except ImportError:
+    VAULT_IMPORT_ERROR = (
+        "Signing with HashiCorp Vault requires hvac and cryptography."
+    )
 
-class SSlibSigner(Signer):
-    """A securesystemslib signer implementation.
 
-    Provides a sign method to generate a cryptographic signature with a
-    securesystemslib-style rsa, ed25519 or ecdsa key. See keys module
-    for the supported types, schemes and hash algorithms.
-
-    SSlibSigners should be instantiated with Signer.from_priv_key_uri().
-    These private key URI schemes are supported:
-    * "envvar:<VAR>":
-        VAR is an environment variable with unencrypted private key content.
-           envvar:MYPRIVKEY
-    * "file:<PATH>?encrypted=[true|false]":
-        PATH is a file path to a file with private key content. If
-        encrypted=true, the file is expected to have been created with
-        securesystemslib.keys.encrypt_key().
-           file:path/to/file?encrypted=true
-           file:/abs/path/to/file?encrypted=false
-
-    Attributes:
-        key_dict:
-            A securesystemslib-style key dictionary. This is an implementation
-            detail, not part of public API
+class VaultSigner(Signer):
+    """Signer for HashiCorp Vault Transit secrets engine
 
-    .. deprecated:: 0.28.0
-        Please use ``CryptoSigner`` instead.
+    The signer uses "ambient" credentials to connect to vault, most notably
+    the environment variables ``VAULT_ADDR`` and ``VAULT_TOKEN`` must be set:
+    https://developer.hashicorp.com/vault/docs/commands#environment-variables
+
+    Priv key uri format is: ``hv:<KEY NAME>/<KEY VERSION>``.
+
+    Arguments:
+        hv_key_name: Name of vault key used for signing.
+        public_key: Related public key instance.
+        hv_key_version: Version of vault key used for signing.
+
+    Raises:
+        UnsupportedLibraryError: hvac or cryptography are not installed.
     """
 
-    ENVVAR_URI_SCHEME = "envvar"
-    FILE_URI_SCHEME = "file"
+    SCHEME = "hv"
+
+    def __init__(self, hv_key_name: str, public_key: Key, hv_key_version: int):
+        if VAULT_IMPORT_ERROR:
+            raise UnsupportedLibraryError(VAULT_IMPORT_ERROR)
+
+        self.hv_key_name = hv_key_name
+        self._public_key = public_key
+        self.hv_key_version = hv_key_version
+
+        # Client caches ambient settings in __init__. This means settings are
+        # stable for subsequent calls to sign, also if the environment changes.
+        self._client = hvac.Client()
+
+    def sign(self, payload: bytes) -> Signature:
+        """Signs payload with HashiCorp Vault Transit secrets engine.
+
+        Arguments:
+            payload: bytes to be signed.
 
-    def __init__(self, key_dict: Dict):
-        self.key_dict = key_dict
-        self._crypto_signer = CryptoSigner.from_securesystemslib_key(key_dict)
+        Raises:
+            Various errors from hvac.
+
+        Returns:
+            Signature.
+        """
+        resp = self._client.secrets.transit.sign_data(
+            self.hv_key_name,
+            hash_input=b64encode(payload).decode(),
+            key_version=self.hv_key_version,
+        )
+
+        sig_b64 = resp["data"]["signature"].split(":")[2]
+        sig = b64decode(sig_b64).hex()
+
+        return Signature(self.public_key.keyid, sig)
+
+    @property
+    def public_key(self) -> Key:
+        return self._public_key
 
     @classmethod
     def from_priv_key_uri(
         cls,
         priv_key_uri: str,
         public_key: Key,
         secrets_handler: Optional[SecretsHandler] = None,
-    ) -> "SSlibSigner":
-        """Constructor for Signer to call
+    ) -> "VaultSigner":
+        uri = parse.urlparse(priv_key_uri)
 
-        Please refer to Signer.from_priv_key_uri() documentation.
+        if uri.scheme != cls.SCHEME:
+            raise ValueError(f"VaultSigner does not support {priv_key_uri}")
 
-        Additionally raises:
-            OSError: Reading the file failed with "file:" URI
-        """
-        if not isinstance(public_key, SSlibKey):
-            raise ValueError(f"Expected SSlibKey for {priv_key_uri}")
+        name, version = uri.path.split("/")
 
-        uri = parse.urlparse(priv_key_uri)
+        return cls(name, public_key, int(version))
 
-        if uri.scheme == cls.ENVVAR_URI_SCHEME:
-            # read private key from environment variable
-            private = os.getenv(uri.path)
-            if private is None:
-                raise ValueError(f"Unset env var for {priv_key_uri}")
-
-        elif uri.scheme == cls.FILE_URI_SCHEME:
-            params = dict(parse.parse_qsl(uri.query))
-            if "encrypted" not in params:
-                raise ValueError(f"{uri.scheme} requires 'encrypted' parameter")
-
-            # read private key (may be encrypted or not) from file
-            with open(uri.path, "rb") as f:
-                private = f.read().decode()
-
-            if params["encrypted"] != "false":
-                if not secrets_handler:
-                    raise ValueError("encrypted key requires a secrets handler")
-
-                secret = secrets_handler("passphrase")
-                decrypted = sslib_keys.decrypt_key(private, secret)
-                private = decrypted["keyval"]["private"]
+    @classmethod
+    def import_(cls, hv_key_name: str) -> Tuple[str, Key]:
+        """Load key and signer details from HashiCorp Vault.
 
-        else:
-            raise ValueError(f"SSlibSigner does not support {priv_key_uri}")
+        If multiple keys exist in the vault under the passed name, only the
+        newest key is returned. Supported key type is: ed25519
 
-        keydict = public_key.to_securesystemslib_key()
-        keydict["keyval"]["private"] = private
+        See class documentation for details about settings and uri format.
 
-        return cls(keydict)
+        Arguments:
+            hv_key_name: Name of vault key to import.
 
-    def sign(self, payload: bytes) -> Signature:
-        """Signs a given payload by the key assigned to the SSlibSigner instance.
+        Raises:
+            UnsupportedLibraryError: hvac or cryptography are not installed.
+            Various errors from hvac.
 
-        Please see Signer.sign() documentation.
+        Returns:
+            Private key uri and public key.
 
-        Additionally raises:
-            securesystemslib.exceptions.FormatError: Key argument is malformed.
-            securesystemslib.exceptions.CryptoError, \
-                securesystemslib.exceptions.UnsupportedAlgorithmError:
-                Signing errors.
         """
-        return self._crypto_signer.sign(payload)
+        if VAULT_IMPORT_ERROR:
+            raise UnsupportedLibraryError(VAULT_IMPORT_ERROR)
+
+        client = hvac.Client()
+        resp = client.secrets.transit.read_key(hv_key_name)
+
+        # Pick key with highest version number
+        version, key_info = sorted(resp["data"]["keys"].items())[-1]
+
+        crypto_key = Ed25519PublicKey.from_public_bytes(
+            b64decode(key_info["public_key"])
+        )
+
+        key = SSlibKey.from_crypto(crypto_key)
+        uri = f"{VaultSigner.SCHEME}:{hv_key_name}/{version}"
+
+        return uri, key
```

### Comparing `securesystemslib-0.31.0/securesystemslib/signer/_utils.py` & `securesystemslib-1.0.0/securesystemslib/signer/_utils.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/tests/aggregate_tests.py` & `securesystemslib-1.0.0/tests/aggregate_tests.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/tests/check_aws_signer.py` & `securesystemslib-1.0.0/tests/check_azure_signer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,66 @@
-"""This module confirms that signing using AWS KMS keys works.
+"""
+This module confirms that signing using Azure KMS keys works.
+
+The purpose is to do a smoke test, not to exhaustively test every possible
+key and environment combination.
 
-The purpose is to do a smoke test, not to exhaustively test every possible key
-and environment combination.
+For Azure, the requirements to successfully test are:
+* Azure authentication details have to be available in the environment
+* The key defined in the test has to be available to the authenticated user
 
-For AWS, the requirements to successfully test are:
-* AWS authentication details
-have to be available in the environment
-* The key defined in the test has to be
-available to the authenticated user
-
-Remember to replace the REDACTED fields to include the necessary values:
-* keyid: Hash of the public key
-* public: The public key, refer to other KMS tests to see the format
-* aws_id: AWS KMS ID or alias
+NOTE: the filename is purposefully check_ rather than test_ so that tests are
+only run when explicitly invoked.
 """
 
 import unittest
 
 from securesystemslib.exceptions import UnverifiedSignatureError
-from securesystemslib.signer import AWSSigner, Key, Signer
+from securesystemslib.signer import AzureSigner, Key, Signer
 
 
-class TestAWSKMSKeys(unittest.TestCase):
-    """Test that AWS KMS keys can be used to sign."""
+class TestAzureKeys(unittest.TestCase):
+    """Test that KMS keys can be used to sign."""
 
-    pubkey = Key.from_dict(
-        "REDACTED",
+    azure_pubkey = Key.from_dict(
+        "8b4af6aec66518bc66718474aa15c8becd3286e8e2b958c497a60a828d591d04",
         {
-            "keytype": "rsa",
-            "scheme": "rsassa-pss-sha256",
+            "keytype": "ecdsa",
+            "scheme": "ecdsa-sha2-nistp256",
             "keyval": {
-                "public": "-----BEGIN PUBLIC KEY-----\nREDACTED\n-----END PUBLIC KEY-----\n"
+                "public": "-----BEGIN PUBLIC KEY-----\nMFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAE95qxD+/kX6oCace7hrfChtz2IYGK\nHNBmUwtf3wXH0VEdLPWVoFgGITonvA7vxqYrF8ZzAeeZYNyEBbod7SEeaw==\n-----END PUBLIC KEY-----\n"
             },
         },
     )
-    aws_key_id = "REDACTED"
+    azure_id = "azurekms://fsn-vault-1.vault.azure.net/keys/ec-key-1/b1089bbf068742d483970282f02090de"
+
+    def test_azure_sign(self):
+        """Test that Azure KMS key works for signing
 
-    def test_aws_sign(self):
-        """Test that AWS KMS key works for signing"""
+        Note that this test requires valid credentials available.
+        """
 
         data = "data".encode("utf-8")
 
-        signer = Signer.from_priv_key_uri(
-            f"awskms:{self.aws_key_id}", self.pubkey
-        )
+        signer = Signer.from_priv_key_uri(self.azure_id, self.azure_pubkey)
         sig = signer.sign(data)
 
-        self.pubkey.verify_signature(sig, data)
+        print(sig.signature)
+
+        self.azure_pubkey.verify_signature(sig, data)
         with self.assertRaises(UnverifiedSignatureError):
-            self.pubkey.verify_signature(sig, b"NOT DATA")
+            self.azure_pubkey.verify_signature(sig, b"NOT DATA")
+
+    def test_azure_import(self):
+        """Test that Azure KMS key works for signing
+
+        Note that this test requires valid credentials available.
+        """
 
-    def test_aws_import(self):
-        """Test that AWS KMS key can be imported"""
+        uri, pubkey = AzureSigner.import_("fsn-vault-1", "ec-key-1")
 
-        uri, key = AWSSigner.import_(self.aws_key_id, self.pubkey.scheme)
-        self.assertEqual(key.keytype, self.pubkey.keytype)
-        self.assertEqual(uri, f"awskms:{self.aws_key_id}")
+        self.assertEqual(pubkey, self.azure_pubkey)
+        self.assertEqual(uri, self.azure_id)
 
 
 if __name__ == "__main__":
-    unittest.main(verbosity=1)
+    unittest.main(verbosity=1, buffer=True)
```

### Comparing `securesystemslib-0.31.0/tests/check_azure_signer.py` & `securesystemslib-1.0.0/tests/check_kms_signers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,72 @@
 """
-This module confirms that signing using Azure KMS keys works.
+This module confirms that signing using KMS keys works.
 
 The purpose is to do a smoke test, not to exhaustively test every possible
 key and environment combination.
 
-For Azure, the requirements to successfully test are:
-* Azure authentication details have to be available in the environment
+For Google Cloud (GCP), the requirements to successfully test are:
+* Google Cloud authentication details have to be available in the environment
 * The key defined in the test has to be available to the authenticated user
 
 NOTE: the filename is purposefully check_ rather than test_ so that tests are
-only run when explicitly invoked.
+only run when explicitly invoked: The tests can only pass on Securesystemslib
+GitHub Action environment because of the above requirements.
 """
 
 import unittest
 
 from securesystemslib.exceptions import UnverifiedSignatureError
-from securesystemslib.signer import AzureSigner, Key, Signer
+from securesystemslib.signer import GCPSigner, Key, Signer
 
 
-class TestAzureKeys(unittest.TestCase):
+class TestKMSKeys(unittest.TestCase):
     """Test that KMS keys can be used to sign."""
 
-    azure_pubkey = Key.from_dict(
-        "8b4af6aec66518bc66718474aa15c8becd3286e8e2b958c497a60a828d591d04",
+    pubkey = Key.from_dict(
+        "ab45d8d98992a4128efaea284c7ef0459557db199aeadf237ae41b915b9b5a1c",
         {
             "keytype": "ecdsa",
             "scheme": "ecdsa-sha2-nistp256",
             "keyval": {
-                "public": "-----BEGIN PUBLIC KEY-----\nMFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAE95qxD+/kX6oCace7hrfChtz2IYGK\nHNBmUwtf3wXH0VEdLPWVoFgGITonvA7vxqYrF8ZzAeeZYNyEBbod7SEeaw==\n-----END PUBLIC KEY-----\n"
+                "public": "-----BEGIN PUBLIC KEY-----\nMFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAE/ptvrXYuUc2ZaKssHhtg/IKNbO1X\ncDWlbKqLNpaK62MKdOwDz1qlp5AGHZkTY9tO09iq1F16SvVot1BQ9FJ2dw==\n-----END PUBLIC KEY-----\n"
             },
         },
     )
-    azure_id = "azurekms://fsn-vault-1.vault.azure.net/keys/ec-key-1/b1089bbf068742d483970282f02090de"
+    gcp_id = "projects/python-tuf-kms/locations/global/keyRings/securesystemslib-tests/cryptoKeys/ecdsa-sha2-nistp256/cryptoKeyVersions/1"
 
-    def test_azure_sign(self):
-        """Test that Azure KMS key works for signing
+    def test_gcp_sign(self):
+        """Test that GCP KMS key works for signing
 
-        Note that this test requires valid credentials available.
+        NOTE: The KMS account is setup to only accept requests from the
+        Securesystemslib GitHub Action environment: test cannot pass elsewhere.
+
+        In case of problems with KMS account, please file an issue and
+        assign @jku.
         """
 
         data = "data".encode("utf-8")
 
-        signer = Signer.from_priv_key_uri(self.azure_id, self.azure_pubkey)
+        signer = Signer.from_priv_key_uri(f"gcpkms:{self.gcp_id}", self.pubkey)
         sig = signer.sign(data)
 
-        print(sig.signature)
-
-        self.azure_pubkey.verify_signature(sig, data)
+        self.pubkey.verify_signature(sig, data)
         with self.assertRaises(UnverifiedSignatureError):
-            self.azure_pubkey.verify_signature(sig, b"NOT DATA")
+            self.pubkey.verify_signature(sig, b"NOT DATA")
 
-    def test_azure_import(self):
-        """Test that Azure KMS key works for signing
+    def test_gcp_import(self):
+        """Test that GCP KMS key can be imported
 
-        Note that this test requires valid credentials available.
-        """
+        NOTE: The KMS account is setup to only accept requests from the
+        Securesystemslib GitHub Action environment: test cannot pass elsewhere.
 
-        uri, pubkey = AzureSigner.import_("fsn-vault-1", "ec-key-1")
+        In case of problems with KMS account, please file an issue and
+        assign @jku.
+        """
 
-        self.assertEqual(pubkey, self.azure_pubkey)
-        self.assertEqual(uri, self.azure_id)
+        uri, key = GCPSigner.import_(self.gcp_id)
+        self.assertEqual(key, self.pubkey)
+        self.assertEqual(uri, f"gcpkms:{self.gcp_id}")
 
 
 if __name__ == "__main__":
     unittest.main(verbosity=1, buffer=True)
```

### Comparing `securesystemslib-0.31.0/tests/check_gpg_available.py` & `securesystemslib-1.0.0/tests/check_gpg_available.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,20 +22,22 @@
   NOTE: the filename is purposefully check_ rather than test_ so that test
   discovery doesn't find this unittest and the tests within are only run
   when explicitly invoked.
 """
 
 import unittest
 
-import securesystemslib.gpg.constants
+import securesystemslib._gpg.constants
 
 
 class TestGpgAvailable(unittest.TestCase):
     """Test that securesystemslib finds some GPG executable in the environment."""
 
     def test_gpg_available(self):
         """Test that GPG is available."""
-        self.assertTrue(securesystemslib.gpg.constants.have_gpg())
+        self.assertTrue(
+            securesystemslib._gpg.constants.have_gpg()  # pylint: disable=protected-access
+        )
 
 
 if __name__ == "__main__":
     unittest.main(verbosity=1, buffer=True)
```

### Comparing `securesystemslib-0.31.0/tests/check_public_interfaces_gpg.py` & `securesystemslib-1.0.0/tests/check_public_interfaces_gpg.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 <Started>
   Feb 26, 2020.
 
 <Copyright>
   See LICENSE for licensing information.
 
 <Purpose>
-  Check that the public facing 'gpg.functions' module remains importable if
+  Check that the public facing '_gpg.functions' module remains importable if
   gnupg is not installed, and that each function presents meaningful
   user-feedback.
   Further check that gpg signature verification works even without gpg.
 
   NOTE: the filename is purposefully check_ rather than test_ so that test
   discovery doesn't find this test module and the test cases within are only
   run when explicitly invoked.
 
 """
 
 import unittest
 
-from securesystemslib.exceptions import UnsupportedLibraryError
-from securesystemslib.gpg.constants import NO_GPG_MSG, have_gpg
-from securesystemslib.gpg.functions import (
+from securesystemslib._gpg.constants import NO_GPG_MSG, have_gpg
+from securesystemslib._gpg.functions import (
     create_signature,
     export_pubkey,
     export_pubkeys,
     verify_signature,
 )
+from securesystemslib.exceptions import UnsupportedLibraryError
 from securesystemslib.signer import GPGKey, GPGSigner, Signer
 
 
 class TestPublicInterfacesGPG(
     unittest.TestCase
 ):  # pylint: disable=missing-class-docstring
     @classmethod
```

### Comparing `securesystemslib-0.31.0/tests/test_gpg.py` & `securesystemslib-1.0.0/tests/test_gpg.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,51 +27,49 @@
 from copy import deepcopy
 from unittest.mock import patch
 
 import cryptography.hazmat.primitives.hashes as hashing
 from cryptography.hazmat import backends
 from cryptography.hazmat.primitives import serialization
 
-from securesystemslib.formats import ANY_PUBKEY_DICT_SCHEMA, GPG_PUBKEY_SCHEMA
-from securesystemslib.gpg.common import (
+from securesystemslib._gpg.common import (
     _assign_certified_key_info,
     _get_verified_subkeys,
     get_pubkey_bundle,
     parse_pubkey_bundle,
     parse_pubkey_payload,
     parse_signature_packet,
 )
-from securesystemslib.gpg.constants import (
+from securesystemslib._gpg.constants import (
     PACKET_TYPE_PRIMARY_KEY,
     PACKET_TYPE_SUB_KEY,
     PACKET_TYPE_USER_ATTR,
     PACKET_TYPE_USER_ID,
     SHA1,
     SHA256,
     SHA512,
     have_gpg,
 )
-from securesystemslib.gpg.dsa import create_pubkey as dsa_create_pubkey
-from securesystemslib.gpg.eddsa import ED25519_SIG_LENGTH
-from securesystemslib.gpg.exceptions import (
-    CommandError,
+from securesystemslib._gpg.dsa import create_pubkey as dsa_create_pubkey
+from securesystemslib._gpg.eddsa import ED25519_SIG_LENGTH
+from securesystemslib._gpg.exceptions import (
     KeyExpirationError,
     KeyNotFoundError,
     PacketParsingError,
     PacketVersionNotSupportedError,
     SignatureAlgorithmNotSupportedError,
 )
-from securesystemslib.gpg.functions import (
+from securesystemslib._gpg.functions import (
     create_signature,
     export_pubkey,
     export_pubkeys,
     verify_signature,
 )
-from securesystemslib.gpg.rsa import create_pubkey as rsa_create_pubkey
-from securesystemslib.gpg.util import (
+from securesystemslib._gpg.rsa import create_pubkey as rsa_create_pubkey
+from securesystemslib._gpg.util import (
     get_hashing_class,
     parse_packet_header,
     parse_subpacket_header,
 )
 
 # pylint: enable=wrong-import-position
 
@@ -193,15 +191,15 @@
         for idx, data in enumerate(data_list):
             result = parse_subpacket_header(bytearray(data))
             self.assertEqual(result, expected[idx])
 
 
 @unittest.skipIf(not have_gpg(), "gpg not found")
 class TestCommon(unittest.TestCase):
-    """Test common functions of the securesystemslib.gpg module."""
+    """Test common functions of the securesystemslib._gpg module."""
 
     @classmethod
     def setUpClass(self):  # pylint: disable=bad-classmethod-argument
         gpg_keyring_path = os.path.join(
             os.path.dirname(os.path.realpath(__file__)), "gpg_keyrings", "rsa"
         )
 
@@ -268,33 +266,32 @@
             with self.assertRaises(PacketParsingError) as ctx:
                 parse_pubkey_bundle(data)
             self.assertTrue(error_str in str(ctx.exception))
 
         # Create empty packet of unsupported type 66 (bit 0-5) and length 0 and
         # pass as second packet to provoke skipping of unsupported packet
         unsupported_packet = bytearray([0b01111111, 0])
-        with patch("securesystemslib.gpg.common.log") as mock_log:
+        with patch("securesystemslib._gpg.common.log") as mock_log:
             parse_pubkey_bundle(primary_key_packet + unsupported_packet)
             self.assertTrue(
                 "Ignoring gpg key packet '63'" in mock_log.info.call_args[0][0]
             )
 
     def test_parse_pubkey_bundle(self):
         """Assert presence of packets expected returned from `parse_pubkey_bundle`
     for specific test key). See
     ```
     gpg --homedir tests/gpg_keyrings/rsa/ --export 9EA70BD13D883381 | \
         gpg --list-packets
     ```
     """
-        # Expect parsed primary key matching GPG_PUBKEY_SCHEMA
-        self.assertTrue(
-            GPG_PUBKEY_SCHEMA.matches(
-                self.raw_key_bundle[PACKET_TYPE_PRIMARY_KEY]["key"]
-            )
+        # Expect parsed primary key
+        self.assertEqual(
+            self.raw_key_bundle[PACKET_TYPE_PRIMARY_KEY]["key"]["method"],
+            "pgp+rsa-pkcsv1.5",
         )
 
         # Parse corresponding raw packet for comparison
         _, header_len, _, _ = parse_packet_header(
             self.raw_key_bundle[PACKET_TYPE_PRIMARY_KEY]["packet"]
         )
 
@@ -368,15 +365,15 @@
             # Skip and log signature packet that doesn't match primary key id
             (wrong_keyid_bundle, "Ignoring User ID certificate issued by"),
             # Skip and log invalid signature
             (invalid_cert_bundle, "Ignoring invalid User ID self-certificate"),
         ]
 
         for bundle, expected_msg in test_data:
-            with patch("securesystemslib.gpg.common.log") as mock_log:
+            with patch("securesystemslib._gpg.common.log") as mock_log:
                 _assign_certified_key_info(bundle)
                 msg = str(mock_log.info.call_args[0][0])
                 self.assertTrue(
                     expected_msg in msg,
                     "'{}' not in '{}'".format(  # pylint: disable=consider-using-f-string
                         expected_msg, msg
                     ),
@@ -462,17 +459,17 @@
             PACKET_TYPE_SUB_KEY
         ].popitem()
         packet_data["signatures"] = packet_data["signatures"] * 2
         too_many_sigs_bundle[PACKET_TYPE_SUB_KEY][packet] = packet_data
 
         # Tamper with primary key to trigger signature verification error
         invalid_sig_bundle = deepcopy(self.raw_key_bundle)
-        invalid_sig_bundle[PACKET_TYPE_PRIMARY_KEY][
-            "packet"
-        ] = invalid_sig_bundle[PACKET_TYPE_PRIMARY_KEY]["packet"][:-1]
+        invalid_sig_bundle[PACKET_TYPE_PRIMARY_KEY]["packet"] = (
+            invalid_sig_bundle[PACKET_TYPE_PRIMARY_KEY]["packet"][:-1]
+        )
 
         test_data = [
             (bad_subkey_bundle, "Pubkey packet version '3' not supported"),
             (wrong_sig_bundle, "Expected packet 2, but got 63 instead"),
             (
                 not_enough_sigs_bundle,
                 "wrong amount of key binding signatures (0)",
@@ -481,15 +478,15 @@
                 too_many_sigs_bundle,
                 "wrong amount of key binding signatures (2)",
             ),
             (invalid_sig_bundle, "invalid key binding signature"),
         ]
 
         for bundle, expected_msg in test_data:
-            with patch("securesystemslib.gpg.common.log") as mock_log:
+            with patch("securesystemslib._gpg.common.log") as mock_log:
                 _get_verified_subkeys(bundle)
                 msg = str(mock_log.info.call_args[0][0])
                 self.assertTrue(
                     expected_msg in msg,
                     "'{}' not in '{}'".format(  # pylint: disable=consider-using-f-string
                         expected_msg, msg
                     ),
@@ -595,15 +592,15 @@
         os.chdir(self.working_dir)
         shutil.rmtree(
             self.test_dir, onerror=GPGTestUtils.ignore_not_found_error
         )
 
     def test_export_pubkey_error(self):
         """Test correct error is raised if function called incorrectly."""
-        with self.assertRaises(ValueError):
+        with self.assertRaises(KeyNotFoundError):
             export_pubkey("not-a-key-id")
 
     def test_export_pubkey(self):
         """export a public key and make sure the parameters are the right ones:
 
         since there's very little we can do to check rsa key parameters are right
         we pre-exported the public key to an ssh key, which we can load with
@@ -651,15 +648,14 @@
 
     def test_export_pubkeys(self):
         """Test export multiple pubkeys at once."""
         key_dict = export_pubkeys(
             [self.default_keyid, self.keyid_768C43], homedir=self.gnupg_home
         )
 
-        ANY_PUBKEY_DICT_SCHEMA.check_match(key_dict)
         self.assertListEqual(
             sorted([self.default_keyid.lower(), self.keyid_768C43.lower()]),
             sorted(key_dict.keys()),
         )
 
     def test_gpg_sign_and_verify_object_with_default_key(self):
         """Create a signature using the default key on the keyring"""
@@ -701,16 +697,16 @@
         # Reset GNUPGHOME
         if gnupg_home_backup:
             os.environ["GNUPGHOME"] = gnupg_home_backup
         else:
             del os.environ["GNUPGHOME"]
 
     def test_create_signature_with_expired_key(self):
-        """Test signing with expired key raises gpg CommandError."""
-        with self.assertRaises(CommandError) as ctx:
+        """Test signing with expired key raises OSError."""
+        with self.assertRaises(OSError) as ctx:
             create_signature(
                 b"livestock",
                 keyid=self.expired_key_keyid,
                 homedir=self.gnupg_home,
             )
 
         expected = "returned non-zero exit status '2'"
```

### Comparing `securesystemslib-0.31.0/tests/test_hash.py` & `securesystemslib-1.0.0/tests/test_hash.py`

 * *Files 5% similar despite different names*

```diff
@@ -252,43 +252,14 @@
             file_obj, algorithm, library
         )
 
         # Note: we don't seek because the update_file_obj call is supposed
         # to always seek to the beginning.
         self.assertEqual(digest_object_truth.digest(), digest_object.digest())
 
-    def test_digest_from_rsa_scheme(self):
-        self._run_with_all_hash_libraries(
-            self._do_get_digest_from_rsa_valid_schemes, "sha256"
-        )
-        self._run_with_all_hash_libraries(
-            self._do_get_digest_from_rsa_non_valid_schemes, "sha256"
-        )
-
-    def _do_get_digest_from_rsa_valid_schemes(self, library, algorithm):
-        scheme = "rsassa-pss-sha256"
-        expected_digest_cls = type(
-            securesystemslib.hash.digest(algorithm, library)
-        )
-
-        self.assertIsInstance(
-            securesystemslib.hash.digest_from_rsa_scheme(scheme, library),
-            expected_digest_cls,
-        )
-
-    def _do_get_digest_from_rsa_non_valid_schemes(
-        self, library, algorithm
-    ):  # pylint: disable=unused-argument
-        self.assertRaises(
-            securesystemslib.exceptions.FormatError,
-            securesystemslib.hash.digest_from_rsa_scheme,
-            "rsassa-pss-sha123",
-            library,
-        )
-
     def test_unsupported_digest_algorithm_and_library(self):
         self.assertRaises(
             securesystemslib.exceptions.UnsupportedAlgorithmError,
             securesystemslib.hash.digest,
             "sha123",
             "hashlib",
         )
```

### Comparing `securesystemslib-0.31.0/tests/test_hsm_signer.py` & `securesystemslib-1.0.0/tests/test_hsm_signer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Test HSMSigner
 """
+
 import os
 import shutil
 import tempfile
 import unittest
 
 from asn1crypto.keys import (  # pylint: disable=import-error
     ECDomainParameters,
```

### Comparing `securesystemslib-0.31.0/tests/test_signer.py` & `securesystemslib-1.0.0/tests/test_signer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,39 @@
 """Test cases for "signer.py". """
 
 import copy
 import os
 import shutil
 import tempfile
 import unittest
+from contextlib import suppress
 from pathlib import Path
 from typing import Any, Dict, Optional
 
+from cryptography.hazmat.primitives.asymmetric.types import PrivateKeyTypes
 from cryptography.hazmat.primitives.serialization import (
     load_pem_private_key,
     load_pem_public_key,
 )
 
-import securesystemslib.keys as KEYS
-from securesystemslib.exceptions import (
-    CryptoError,
-    FormatError,
-    UnverifiedSignatureError,
-    VerificationError,
-)
-from securesystemslib.gpg.constants import have_gpg
-from securesystemslib.gpg.exceptions import CommandError, KeyNotFoundError
+from securesystemslib._gpg.constants import have_gpg
+from securesystemslib.exceptions import FormatError, UnverifiedSignatureError
 from securesystemslib.signer import (
     KEY_FOR_TYPE_AND_SCHEME,
     SIGNER_FOR_URI_SCHEME,
     CryptoSigner,
     GPGKey,
     GPGSigner,
     Key,
     SecretsHandler,
     Signature,
     Signer,
     SpxKey,
     SpxSigner,
     SSlibKey,
-    SSlibSigner,
     generate_spx_key_pair,
 )
 from securesystemslib.signer._utils import compute_default_keyid
 
 PEMS_DIR = Path(__file__).parent / "data" / "pems"
 
 
@@ -78,28 +72,33 @@
             },
         ]
         for keydict in invalid_dicts:
             with self.assertRaises((KeyError, ValueError)):
                 Key.from_dict("aa", keydict)
 
     def test_key_verify_signature(self):
+        # pylint: disable=too-many-locals
         ed25519_keyid = (
             "fc3920f44a1deec695ed9327f70513909a36f51ad19774167ddf28a12f8bbbed"
         )
         ed25519_pub = (
             "50a5768a7a577483c28e57a6742b4d2170b9be628a961355ef127c45f2aefdc5"
         )
         rsa_keyid = (
             "b7c94258646e970d336b779eea6b90ef931ea56e2d356ce487201f6bb776e94b"
         )
         rsa_pub = "-----BEGIN PUBLIC KEY-----\nMIIBojANBgkqhkiG9w0BAQEFAAOCAY8AMIIBigKCAYEAsDqUoiFJZX+5gm5pyI1l\nVc/N3yjJVOIl9GyiK0mRyzV3IzUQzhjq8nhk0eLfzXw2XwIAYOJC6dR/tGRG4JDx\nJkez5FFH4zLosr/XzT7CG5zxJ3kKICLD1v9rZQr5ZgARQDOpkxzPz46rGnE0sHd7\nMpnpPMScA1pMIzwM1RoPS4ntZipI1cl9M7HMQ6mkBp8/DNKCqaDWixJqaGgWrhhK\nhI/1mzBliMKriNxPKSCGVlOk/QpZft+y1fs42s0DMd5BOFBo+ZcoXLYRncg9S3A2\nxx/jT69Bt3ceiAZqnp7f6M+ZzoUifSelaoL7QIYg/GkEl+0oxTD0yRphGiCKwn9c\npSbn7NgnbjqSgIMeEtlf/5Coyrs26pyFf/9GbusddPSxxxwIJ/7IJuF7P1Yy0WpZ\nkMeY83h9n2IdnEYi+rpdbLJPQd7Fpu2xrdA3Fokj8AvCpcmxn8NIXZuK++r8/xsE\nAUL30HH7dgVn50AvdPaJnqAORT3OlabW0DK9prcwKnyzAgMBAAE=\n-----END PUBLIC KEY-----"
         ecdsa_keyid = (
             "985171ff9ee901fbab17aa6f57347933aeae9d194f0f93e83e5c3dbc1755e754"
         )
         ecdsa_pub = "-----BEGIN PUBLIC KEY-----\nMFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAEsYJfSlYU3UlYbGOZfE/yOHkayWWq\nLPR/NeCa83szZmnJGc9wwCRPvJS87K+eDGIhhhKueTyrLqXQqmyHioQbOQ==\n-----END PUBLIC KEY-----\n"
+        ecdsa_nistp384_keyid = (
+            "0155661bdf705f621a74f55eef36c9ae041e456141eced7a45d4a1f75ded9ac0"
+        )
+        ecdsa_nistp384_pub = "-----BEGIN PUBLIC KEY-----\nMHYwEAYHKoZIzj0CAQYFK4EEACIDYgAEksAG80nLUksODTEUBTPJJPYN0bfxhkrr\n2hlyokfRG4kDYsRRN86vWwxDTW7qhWNZPFhJMJxHmvHsCbLz/IF7hdo8Xv/vRO4M\nVHbwq0fiWznUvkZowHC5fH2EEvNF1R5t\n-----END PUBLIC KEY-----\n"
 
         key_sig_data = [
             (
                 ed25519_keyid,
                 "ed25519",
                 "ed25519",
                 ed25519_pub,
@@ -173,33 +172,33 @@
                 ecdsa_keyid,
                 "ecdsa",
                 "ecdsa-sha2-nistp256",
                 ecdsa_pub,
                 "3045022100b3db1e5ca53226ee27f93a3b2f5e1534f4a4c51f872aa1b6efd0b37be27f483602204f793f7ad7c25188ad55eb6a8a8d142f89b0b0090815de47d9a24389872b02e3",
             ),
             (
-                ecdsa_keyid,
+                ecdsa_nistp384_keyid,
                 "ecdsa",
                 "ecdsa-sha2-nistp384",
-                ecdsa_pub,
-                "3045022100fc41dad2236dc479454cfeab69a8d77b67e38ef3290ddef3f240406db63c407c0220402ef9c132ec6682f70143079c6e0c11ce4904be03354bd1b0bc7553125e013e",
+                ecdsa_nistp384_pub,
+                "30650230747ffab40d894dcacfa2da613a312b2423aa744c7b2365345467819c2af210983c5a7ce6810db995f2e6c90f90f9ad1c023100fdde5013796916af1989b757b64f2fad8496fa7b2b19e9568260868d4a670e6feb123b3337179a4d06b5fbe42b6937fb",
             ),
             (
                 ecdsa_keyid,
                 "ecdsa-sha2-nistp256",
                 "ecdsa-sha2-nistp256",
                 ecdsa_pub,
                 "304502207d0058b745b2259501204c2ba287ba3769ec2420e12463a325c59670c24df9b6022100836ca63a1b870f755c1596711a003a505e72e25cb0970e823a331e044adc63ec",
             ),
             (
-                ecdsa_keyid,
+                ecdsa_nistp384_keyid,
                 "ecdsa-sha2-nistp384",
                 "ecdsa-sha2-nistp384",
-                ecdsa_pub,
-                "304502200cf6f9794205d4694438cc4f394fe385c85d2ee6938f079c7e1bd896dcd8c635022100a2ba46172be199955be7317c9335ae7f073328d26a5f561968024ff46e430c21",
+                ecdsa_nistp384_pub,
+                "30650230747ffab40d894dcacfa2da613a312b2423aa744c7b2365345467819c2af210983c5a7ce6810db995f2e6c90f90f9ad1c023100fdde5013796916af1989b757b64f2fad8496fa7b2b19e9568260868d4a670e6feb123b3337179a4d06b5fbe42b6937fb",
             ),
         ]
         for keyid, keytype, scheme, pub, sig in key_sig_data:
             key = Key.from_dict(
                 keyid,
                 {
                     "keytype": keytype,
@@ -295,36 +294,45 @@
     def test_from_crypto(self):
         """Test load pyca/cryptography public key for each SSlibKey keytype"""
         test_data = [
             (
                 "rsa",
                 "rsassa-pss-sha256",
                 "2f685fa7546f1856b123223ab086b3def14c89d24eef18f49c32508c2f60e241",
+                "rsa_public.pem",
             ),
             (
                 "ecdsa",
                 "ecdsa-sha2-nistp256",
                 "50d7e110ad65f3b2dba5c3cfc8c5ca259be9774cc26be3410044ffd4be3aa5f3",
+                "ecdsa_public.pem",
+            ),
+            (
+                "ecdsa",
+                "ecdsa-sha2-nistp384",
+                "0155661bdf705f621a74f55eef36c9ae041e456141eced7a45d4a1f75ded9ac0",
+                "ecdsa_secp384r1_public.pem",
             ),
             (
                 "ed25519",
                 "ed25519",
                 "c6d8bf2e4f48b41ac2ce8eca21415ca8ef68c133b47fc33df03d4070a7e1e9cc",
+                "ed25519_public.pem",
             ),
         ]
 
         def _from_file(path):
             with open(path, "rb") as f:
                 pem = f.read()
 
             crypto_key = load_pem_public_key(pem)
             return crypto_key
 
-        for keytype, default_scheme, default_keyid in test_data:
-            crypto_key = _from_file(PEMS_DIR / f"{keytype}_public.pem")
+        for keytype, default_scheme, default_keyid, fname in test_data:
+            crypto_key = _from_file(PEMS_DIR / fname)
             key = SSlibKey.from_crypto(crypto_key)
             self.assertEqual(key.keytype, keytype)
             self.assertEqual(key.scheme, default_scheme)
             self.assertEqual(key.keyid, default_keyid)
 
         # Test with non-default scheme/keyid
         crypto_key = _from_file(PEMS_DIR / "rsa_public.pem")
@@ -332,198 +340,56 @@
             crypto_key,
             scheme="rsa-pkcs1v15-sha224",
             keyid="abcdef",
         )
         self.assertEqual(key.scheme, "rsa-pkcs1v15-sha224")
         self.assertEqual(key.keyid, "abcdef")
 
+    def test_verify_invalid_keytype_scheme(self):
 
-class TestSigner(unittest.TestCase):
-    """Test Signer and SSlibSigner functionality"""
+        rsa = "-----BEGIN PUBLIC KEY-----\nMIIBojANBgkqhkiG9w0BAQEFAAOCAY8AMIIBigKCAYEAsDqUoiFJZX+5gm5pyI1l\nVc/N3yjJVOIl9GyiK0mRyzV3IzUQzhjq8nhk0eLfzXw2XwIAYOJC6dR/tGRG4JDx\nJkez5FFH4zLosr/XzT7CG5zxJ3kKICLD1v9rZQr5ZgARQDOpkxzPz46rGnE0sHd7\nMpnpPMScA1pMIzwM1RoPS4ntZipI1cl9M7HMQ6mkBp8/DNKCqaDWixJqaGgWrhhK\nhI/1mzBliMKriNxPKSCGVlOk/QpZft+y1fs42s0DMd5BOFBo+ZcoXLYRncg9S3A2\nxx/jT69Bt3ceiAZqnp7f6M+ZzoUifSelaoL7QIYg/GkEl+0oxTD0yRphGiCKwn9c\npSbn7NgnbjqSgIMeEtlf/5Coyrs26pyFf/9GbusddPSxxxwIJ/7IJuF7P1Yy0WpZ\nkMeY83h9n2IdnEYi+rpdbLJPQd7Fpu2xrdA3Fokj8AvCpcmxn8NIXZuK++r8/xsE\nAUL30HH7dgVn50AvdPaJnqAORT3OlabW0DK9prcwKnyzAgMBAAE=\n-----END PUBLIC KEY-----"
+        ed25519 = (
+            "50a5768a7a577483c28e57a6742b4d2170b9be628a961355ef127c45f2aefdc5"
+        )
+        ecdsa_nistp256 = "-----BEGIN PUBLIC KEY-----\nMFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAEsYJfSlYU3UlYbGOZfE/yOHkayWWq\nLPR/NeCa83szZmnJGc9wwCRPvJS87K+eDGIhhhKueTyrLqXQqmyHioQbOQ==\n-----END PUBLIC KEY-----\n"
+        ecdsa_nistp384 = "-----BEGIN PUBLIC KEY-----\nMHYwEAYHKoZIzj0CAQYFK4EEACIDYgAEksAG80nLUksODTEUBTPJJPYN0bfxhkrr\n2hlyokfRG4kDYsRRN86vWwxDTW7qhWNZPFhJMJxHmvHsCbLz/IF7hdo8Xv/vRO4M\nVHbwq0fiWznUvkZowHC5fH2EEvNF1R5t\n-----END PUBLIC KEY-----\n"
 
-    @classmethod
-    def setUpClass(cls):
-        cls.keys = [
-            KEYS.generate_rsa_key(),
-            KEYS.generate_ed25519_key(),
-            KEYS.generate_ecdsa_key(),
+        test_data = [
+            # bad keytype / scheme
+            ("ed25519", "rsassa-pss-sha256", rsa),
+            ("ecdsa-sha2-nistp384", "ecdsa-sha2-nistp256", ecdsa_nistp256),
+            ("ecdsa-sha2-nistp256", "ecdsa-sha2-nistp384", ecdsa_nistp384),
+            ("rsa", "ed25519", ed25519),
+            # bad key type (pem formatted keys only)
+            ("rsa", "rsassa-pss-sha256", ecdsa_nistp256),
+            ("ecdsa", "ecdsa-sha2-nistp256", rsa),
+            # bad curve (ecdsa keys only)
+            ("ecdsa", "ecdsa-sha2-nistp256", ecdsa_nistp384),
+            ("ecdsa", "ecdsa-sha2-nistp384", ecdsa_nistp256),
         ]
 
-        cls.DATA = b"DATA"
+        for keytype, scheme, val in test_data:
+            key = SSlibKey("fake", keytype, scheme, {"public": val})
+            with self.assertRaises(ValueError):
+                key._verify(  # pylint: disable=protected-access
+                    b"fakesig", b"fakedata"
+                )
 
-        # pylint: disable=consider-using-with
-        cls.testdir = tempfile.TemporaryDirectory()
 
-    @classmethod
-    def tearDownClass(cls):
-        cls.testdir.cleanup()
+class TestSigner(unittest.TestCase):
+    """Test Signer and SSlibSigner functionality"""
 
     def test_signer_sign_with_incorrect_uri(self):
-        pubkey = SSlibKey.from_securesystemslib_key(self.keys[0])
-        with self.assertRaises(ValueError):
-            # unknown uri
+        pubkey = "fake key"
+        with self.assertRaises(ValueError) as ctx:
             Signer.from_priv_key_uri("unknownscheme:x", pubkey)
 
-        with self.assertRaises(ValueError):
-            # env variable not defined
-            Signer.from_priv_key_uri("envvar:NONEXISTENTVAR", pubkey)
-
-        with self.assertRaises(ValueError):
-            # no "encrypted" param
-            Signer.from_priv_key_uri("file:path/to/privkey", pubkey)
-
-        with self.assertRaises(OSError):
-            # file not found
-            uri = "file:nonexistentfile?encrypted=false"
-            Signer.from_priv_key_uri(uri, pubkey)
-
-    def test_signer_sign_with_envvar_uri(self):
-        for key in self.keys:
-            # setup
-            pubkey = SSlibKey.from_securesystemslib_key(key)
-            os.environ["PRIVKEY"] = key["keyval"]["private"]
-
-            # test signing
-            signer = Signer.from_priv_key_uri("envvar:PRIVKEY", pubkey)
-            sig = signer.sign(self.DATA)
-
-            pubkey.verify_signature(sig, self.DATA)
-            with self.assertRaises(UnverifiedSignatureError):
-                pubkey.verify_signature(sig, b"NOT DATA")
-
-    def test_signer_sign_with_file_uri(self):
-        for key in self.keys:
-            # setup
-            pubkey = SSlibKey.from_securesystemslib_key(key)
-            # let teardownclass handle the file removal
-            with tempfile.NamedTemporaryFile(
-                dir=self.testdir.name, delete=False
-            ) as f:
-                f.write(key["keyval"]["private"].encode())
-
-            # test signing with unencrypted key
-            uri = f"file:{f.name}?encrypted=false"
-            signer = Signer.from_priv_key_uri(uri, pubkey)
-            sig = signer.sign(self.DATA)
-
-            pubkey.verify_signature(sig, self.DATA)
-            with self.assertRaises(UnverifiedSignatureError):
-                pubkey.verify_signature(sig, b"NOT DATA")
-
-    def test_signer_sign_with_enc_file_uri(self):
-        for key in self.keys:
-            # setup
-            pubkey = SSlibKey.from_securesystemslib_key(key)
-            privkey = KEYS.encrypt_key(key, "hunter2")
-            # let teardownclass handle the file removal
-            with tempfile.NamedTemporaryFile(
-                dir=self.testdir.name, delete=False
-            ) as f:
-                f.write(privkey.encode())
-
-            # test signing with encrypted key
-            def secrets_handler(secret: str) -> str:
-                if secret != "passphrase":
-                    raise ValueError("Only prepared to return a passphrase")
-                return "hunter2"
-
-            uri = f"file:{f.name}?encrypted=true"
-
-            signer = Signer.from_priv_key_uri(uri, pubkey, secrets_handler)
-            sig = signer.sign(self.DATA)
-
-            pubkey.verify_signature(sig, self.DATA)
-            with self.assertRaises(UnverifiedSignatureError):
-                pubkey.verify_signature(sig, b"NOT DATA")
-
-            # test wrong passphrase
-            def fake_handler(_) -> str:
-                return "12345"
-
-            with self.assertRaises(CryptoError):
-                signer = Signer.from_priv_key_uri(uri, pubkey, fake_handler)
-
-    def test_sslib_signer_sign_all_schemes(self):
-        rsa_key, ed25519_key, ecdsa_key = self.keys
-        keys = []
-        for scheme in [
-            "rsassa-pss-sha224",
-            "rsassa-pss-sha256",
-            "rsassa-pss-sha384",
-            "rsassa-pss-sha512",
-            "rsa-pkcs1v15-sha224",
-            "rsa-pkcs1v15-sha256",
-            "rsa-pkcs1v15-sha384",
-            "rsa-pkcs1v15-sha512",
-        ]:
-            key = copy.deepcopy(rsa_key)
-            key["scheme"] = scheme
-            keys.append(key)
-
-        self.assertEqual(ecdsa_key["scheme"], "ecdsa-sha2-nistp256")
-        self.assertEqual(ed25519_key["scheme"], "ed25519")
-        keys += [ecdsa_key, ed25519_key]
-
-        # Test sign/verify for each supported scheme
-        for scheme_dict in keys:
-            # Test generation of signatures.
-            sslib_signer = SSlibSigner(scheme_dict)
-            sig_obj = sslib_signer.sign(self.DATA)
-
-            # Verify signature
-            verified = KEYS.verify_signature(
-                scheme_dict, sig_obj.to_dict(), self.DATA
-            )
-            self.assertTrue(verified, "Incorrect signature.")
-
-    def test_sslib_signer_errors(self):
-        # Test basic initialization errors for each keytype
-        for scheme_dict in self.keys:
-            # Assert error for invalid private key data
-            bad_private = copy.deepcopy(scheme_dict)
-            bad_private["keyval"]["private"] = ""
-            with self.assertRaises(ValueError):
-                SSlibSigner(bad_private)
-
-            # Assert error for invalid scheme
-            invalid_scheme = copy.deepcopy(scheme_dict)
-            invalid_scheme["scheme"] = "invalid_scheme"
-            with self.assertRaises(ValueError):
-                SSlibSigner(invalid_scheme)
-
-    def test_custom_signer(self):
-        # setup
-        key = self.keys[0]
-        pubkey = SSlibKey.from_securesystemslib_key(key)
-
-        class CustomSigner(SSlibSigner):
-            """Custom signer with a hard coded key"""
-
-            CUSTOM_SCHEME = "custom"
-
-            @classmethod
-            def from_priv_key_uri(
-                cls,
-                priv_key_uri: str,
-                public_key: Key,
-                secrets_handler: Optional[SecretsHandler] = None,
-            ) -> "CustomSigner":
-                return cls(key)
-
-        # register custom signer
-        SIGNER_FOR_URI_SCHEME[CustomSigner.CUSTOM_SCHEME] = CustomSigner
-
-        # test signing
-        signer = Signer.from_priv_key_uri("custom:foo", pubkey)
-        self.assertIsInstance(signer, CustomSigner)
-        sig = signer.sign(self.DATA)
-
-        pubkey.verify_signature(sig, self.DATA)
-        with self.assertRaises(UnverifiedSignatureError):
-            pubkey.verify_signature(sig, b"NOT DATA")
+        self.assertEqual(
+            "Unsupported private key scheme unknownscheme", str(ctx.exception)
+        )
 
     def test_signature_from_to_dict(self):
         signature_dict = {
             "sig": "30460221009342e4566528fcecf6a7a5d53ebacdb1df151e242f55f8775883469cb01dbc6602210086b426cc826709acfa2c3f9214610cb0a832db94bbd266fd7c5939a48064a851",
             "keyid": "11fa391a0ed7a447cbfeb4b2667e286fc248f64d5e6d0eeed2e5e23f97f9f714",
             "foo": "bar",  # unrecognized_field
         }
@@ -602,42 +468,38 @@
         sig = signer.sign(self.test_data)
 
         public_key.verify_signature(sig, self.test_data)
 
         with self.assertRaises(UnverifiedSignatureError):
             public_key.verify_signature(sig, self.wrong_data)
 
-        sig.keyid = 123456
-        with self.assertRaises(VerificationError):
-            public_key.verify_signature(sig, self.test_data)
-
     def test_gpg_fail_sign_keyid_match(self):
         """Fail signing because signature keyid does not match public key."""
         uri, public_key = GPGSigner.import_(self.default_keyid, self.gnupg_home)
         signer = Signer.from_priv_key_uri(uri, public_key)
 
         # Fail because we imported main key, but gpg favors signing subkey
         with self.assertRaises(ValueError):
             signer.sign(self.test_data)
 
     def test_gpg_fail_import_keyid_match(self):
         """Fail key import because passed keyid does not match returned key."""
 
         # gpg exports the right key, but we require an exact keyid match
         non_matching_keyid = self.default_keyid.upper()
-        with self.assertRaises(KeyNotFoundError):
+        with self.assertRaises(ValueError):
             GPGSigner.import_(non_matching_keyid, self.gnupg_home)
 
     def test_gpg_fail_sign_expired_key(self):
         """Signing fails with non-zero exit code if key is expired."""
         expired_key = "e8ac80c924116dabb51d4b987cb07d6d2c199c7c"
 
         uri, public_key = GPGSigner.import_(expired_key, self.gnupg_home)
         signer = Signer.from_priv_key_uri(uri, public_key)
-        with self.assertRaises(CommandError):
+        with self.assertRaises(OSError):
             signer.sign(self.test_data)
 
     def test_gpg_signer_load_with_bad_scheme(self):
         """Load from priv key uri with wrong uri scheme."""
         key = GPGKey("aa", "rsa", "pgp+rsa-pkcsv1.5", {"public": "val"})
         with self.assertRaises(ValueError):
             GPGSigner.from_priv_key_uri("wrong:", key)
@@ -745,84 +607,123 @@
             ),
         )
 
 
 class TestCryptoSigner(unittest.TestCase):
     """CryptoSigner tests"""
 
-    def test_init(self):
-        """Test CryptoSigner constructor."""
+    @classmethod
+    def setUpClass(cls):
+        cls.keys: list[PrivateKeyTypes] = []
         for keytype in ["rsa", "ecdsa", "ed25519"]:
             path = PEMS_DIR / f"{keytype}_private.pem"
 
             with open(path, "rb") as f:
                 data = f.read()
 
             private_key = load_pem_private_key(data, None)
 
+            cls.keys.append(private_key)
+
+    def test_init(self):
+        """Test CryptoSigner constructor."""
+        for keytype, private_key in zip(["rsa", "ecdsa", "ed25519"], self.keys):
+
             # Init w/o public key (public key is created from private key)
             signer = CryptoSigner(private_key)
             self.assertEqual(keytype, signer.public_key.keytype)
 
             # Re-init with passed public key
             signer2 = CryptoSigner(private_key, signer.public_key)
             self.assertEqual(keytype, signer2.public_key.keytype)
 
+    def test_sign(self):
+        rsa_schemes = [
+            "rsassa-pss-sha224",
+            "rsassa-pss-sha256",
+            "rsassa-pss-sha384",
+            "rsassa-pss-sha512",
+            "rsa-pkcs1v15-sha224",
+            "rsa-pkcs1v15-sha256",
+            "rsa-pkcs1v15-sha384",
+            "rsa-pkcs1v15-sha512",
+        ]
+        ecdsa_schemes = ["ecdsa-sha2-nistp256"]
+        ed25519_schemes = ["ed25519"]
+        schemes = [rsa_schemes, ecdsa_schemes, ed25519_schemes]
+
+        for private_key, key_schemes in zip(self.keys, schemes):
+            public_key = SSlibKey.from_crypto(private_key.public_key())
+            for scheme in key_schemes:
+                public_key.scheme = scheme
+                signer = CryptoSigner(private_key, public_key)
+                sig = signer.sign(b"DATA")
+                self.assertIsNone(
+                    signer.public_key.verify_signature(sig, b"DATA")
+                )
+                with self.assertRaises(UnverifiedSignatureError):
+                    signer.public_key.verify_signature(sig, b"NOT DATA")
+
     def test_from_priv_key_uri(self):
         """Test load and use PEM/PKCS#8 files for each sslib keytype"""
         test_data = [
             (
                 "rsa",
                 "rsassa-pss-sha256",
                 "-----BEGIN PUBLIC KEY-----\nMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAwhX6rioiL/cX5Ys32InF\nU52H8tL14QeX0tacZdb+AwcH6nIh97h3RSHvGD7Xy6uaMRmGldAnSVYwJHqoJ5j2\nynVzU/RFpr+6n8Ps0QFg5GmlEqZboFjLbS0bsRQcXXnqJNsVLEPT3ULvu1rFRbWz\nAMFjNtNNk5W/u0GEzXn3D03jIdhD8IKAdrTRf0VMD9TRCXLdMmEU2vkf1NVUnOTb\n/dRX5QA8TtBylVnouZknbavQ0J/pPlHLfxUgsKzodwDlJmbPG9BWwXqQCmP0DgOG\nNIZ1X281MOBaGbkNVEuntNjCSaQxQjfALVVU5NAfal2cwMINtqaoc7Wa+TWvpFEI\nWwIDAQAB\n-----END PUBLIC KEY-----\n",
+                "rsa_private.pem",
             ),
             (
                 "ecdsa",
                 "ecdsa-sha2-nistp256",
                 "-----BEGIN PUBLIC KEY-----\nMFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAEcLYSZyFGeKdWNt5dWFbnv6N9NyHC\noUNLcG6GZIxLwN8Q8MUdHdOOxGkDnyBRSJpIZ/r/oDECSTwfCYhdogweLA==\n-----END PUBLIC KEY-----\n",
+                "ecdsa_private.pem",
+            ),
+            (
+                "ecdsa-sha2-nistp256",  # keytype deprecated in TUF spec, tested for backwards compat with older metadata
+                "ecdsa-sha2-nistp256",
+                "-----BEGIN PUBLIC KEY-----\nMFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAEcLYSZyFGeKdWNt5dWFbnv6N9NyHC\noUNLcG6GZIxLwN8Q8MUdHdOOxGkDnyBRSJpIZ/r/oDECSTwfCYhdogweLA==\n-----END PUBLIC KEY-----\n",
+                "ecdsa_private.pem",
             ),
             (
                 "ed25519",
                 "ed25519",
                 "4f66dabebcf30628963786001984c0b75c175cdcf3bc4855933a2628f0cd0a0f",
+                "ed25519_private.pem",
             ),
         ]
 
-        signer_backup = SIGNER_FOR_URI_SCHEME[CryptoSigner.FILE_URI_SCHEME]
-        SIGNER_FOR_URI_SCHEME[CryptoSigner.FILE_URI_SCHEME] = CryptoSigner
-
-        for keytype, scheme, public_key_value in test_data:
-            for encrypted in [True, False]:
-                if encrypted:
-                    file_name = f"{keytype}_private_encrypted.pem"
-                    parameter = "true"
-
-                    def handler(_):
-                        return "hunter2"
-
+        for keytype, scheme, public_key_value, fname in test_data:
+            for use_prefix in [True, False]:
+                if use_prefix:
+                    # uri path is relative from CRYPTO_SIGNER_PATH_PREFIX
+                    os.environ["CRYPTO_SIGNER_PATH_PREFIX"] = str(PEMS_DIR)
+                    uri = f"file2:{fname}"
                 else:
-                    file_name = f"{keytype}_private.pem"
-                    parameter = "false"
-                    handler = None
+                    with suppress(KeyError):
+                        del os.environ["CRYPTO_SIGNER_PATH_PREFIX"]
+                    uri = f"file2:{PEMS_DIR / fname}"
 
-                uri = f"file:{PEMS_DIR / file_name}?encrypted={parameter}"
                 public_key = SSlibKey(
                     "abcdefg", keytype, scheme, {"public": public_key_value}
                 )
-                signer = Signer.from_priv_key_uri(uri, public_key, handler)
+                signer = Signer.from_priv_key_uri(uri, public_key)
                 self.assertIsInstance(signer, CryptoSigner)
 
                 sig = signer.sign(b"DATA")
                 self.assertIsNone(
                     signer.public_key.verify_signature(sig, b"DATA")
                 )
                 with self.assertRaises(UnverifiedSignatureError):
                     signer.public_key.verify_signature(sig, b"NOT DATA")
 
-        SIGNER_FOR_URI_SCHEME[CryptoSigner.FILE_URI_SCHEME] = signer_backup
+        with self.assertRaises(OSError):
+            # file not found
+            uri = "file2:nonexistentfile"
+            Signer.from_priv_key_uri(uri, public_key)
 
     def test_generate(self):
         """Test generate and use signer (key pair) for each sslib keytype"""
         test_data = [
             (CryptoSigner.generate_rsa, "rsa", "rsassa-pss-sha256"),
             (CryptoSigner.generate_ecdsa, "ecdsa", "ecdsa-sha2-nistp256"),
             (CryptoSigner.generate_ed25519, "ed25519", "ed25519"),
@@ -833,11 +734,59 @@
             self.assertEqual(signer.public_key.scheme, default_scheme)
 
             sig = signer.sign(b"DATA")
             self.assertIsNone(signer.public_key.verify_signature(sig, b"DATA"))
             with self.assertRaises(UnverifiedSignatureError):
                 signer.public_key.verify_signature(sig, b"NOT DATA")
 
+    def test_private_bytes(self):
+        """Test private_bytes -> from_priv_key_uri"""
+        with tempfile.TemporaryDirectory() as tempdir:
+            priv_key_path = os.path.join(tempdir, "privkey.pem")
+            for pem in ["rsa", "ecdsa", "ed25519"]:
+                with open(PEMS_DIR / f"{pem}_private.pem", "rb") as f:
+                    privkey = load_pem_private_key(f.read(), None)
+                    signer = CryptoSigner(privkey)
+
+                with open(priv_key_path, "wb") as f:
+                    f.write(signer.private_bytes)
+
+                signer2 = Signer.from_priv_key_uri(
+                    f"file2:{priv_key_path}", signer.public_key
+                )
+                self.assertEqual(signer.private_bytes, signer2.private_bytes)
+
+    def test_custom_crypto_signer(self):
+        # setup
+        key = self.keys[0]
+        pubkey = SSlibKey.from_crypto(key.public_key())
+
+        class CustomSigner(CryptoSigner):
+            """Custom signer with a hard coded key"""
+
+            CUSTOM_SCHEME = "custom"
+
+            @classmethod
+            def from_priv_key_uri(
+                cls,
+                priv_key_uri: str,
+                public_key: Key,
+                secrets_handler: Optional[SecretsHandler] = None,
+            ) -> "CustomSigner":
+                return cls(key)
+
+        # register custom signer
+        SIGNER_FOR_URI_SCHEME[CustomSigner.CUSTOM_SCHEME] = CustomSigner
+
+        # test signing
+        signer = Signer.from_priv_key_uri("custom:foo", pubkey)
+        self.assertIsInstance(signer, CustomSigner)
+        sig = signer.sign(b"DATA")
+
+        pubkey.verify_signature(sig, b"DATA")
+        with self.assertRaises(UnverifiedSignatureError):
+            pubkey.verify_signature(sig, b"NOT DATA")
+
 
 # Run the unit tests.
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `securesystemslib-0.31.0/tests/test_storage.py` & `securesystemslib-1.0.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/tests/data/pems/rsa_private.pem` & `securesystemslib-1.0.0/tests/data/pems/rsa_private.pem`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/tests/data/pems/rsa_private_encrypted.pem` & `securesystemslib-1.0.0/tests/data/pems/rsa_private_encrypted.pem`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.pem` & `securesystemslib-1.0.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.pem`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh` & `securesystemslib-1.0.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/tests/gpg_keyrings/dsa/pubring.gpg` & `securesystemslib-1.0.0/tests/gpg_keyrings/dsa/pubring.gpg`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/tests/gpg_keyrings/dsa/random_seed` & `securesystemslib-1.0.0/tests/gpg_keyrings/dsa/random_seed`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/tests/gpg_keyrings/dsa/secring.gpg` & `securesystemslib-1.0.0/tests/gpg_keyrings/dsa/secring.gpg`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/tests/gpg_keyrings/dsa/trustdb.gpg` & `securesystemslib-1.0.0/tests/gpg_keyrings/dsa/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/tests/gpg_keyrings/eddsa/trustdb.gpg` & `securesystemslib-1.0.0/tests/gpg_keyrings/eddsa/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/tests/gpg_keyrings/eddsa/openpgp-revocs.d/4E630F84838BF6F7447B830B22692F5FEA9E2DD2.rev` & `securesystemslib-1.0.0/tests/gpg_keyrings/eddsa/openpgp-revocs.d/4E630F84838BF6F7447B830B22692F5FEA9E2DD2.rev`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/tests/gpg_keyrings/rsa/E8AC80C924116DABB51D4B987CB07D6D2C199C7C.raw` & `securesystemslib-1.0.0/tests/gpg_keyrings/rsa/E8AC80C924116DABB51D4B987CB07D6D2C199C7C.raw`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/tests/gpg_keyrings/rsa/F557D0FF451DEF45372591429EA70BD13D883381.raw` & `securesystemslib-1.0.0/tests/gpg_keyrings/rsa/F557D0FF451DEF45372591429EA70BD13D883381.raw`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/tests/gpg_keyrings/rsa/pubring.gpg` & `securesystemslib-1.0.0/tests/gpg_keyrings/rsa/pubring.gpg`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/tests/gpg_keyrings/rsa/random_seed` & `securesystemslib-1.0.0/tests/gpg_keyrings/rsa/random_seed`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/tests/gpg_keyrings/rsa/secring.gpg` & `securesystemslib-1.0.0/tests/gpg_keyrings/rsa/secring.gpg`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/tests/gpg_keyrings/rsa/trustdb.gpg` & `securesystemslib-1.0.0/tests/gpg_keyrings/rsa/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/LICENSE` & `securesystemslib-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `securesystemslib-0.31.0/README.md` & `securesystemslib-1.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -32,25 +32,22 @@
 ## Usage
 [python-securesystemslib.readthedocs.io](https://python-securesystemslib.readthedocs.io)
 
 ## Contact
 - Questions and discussions:
   [`#securesystemslib-python`](https://cloud-native.slack.com/archives/C05PF3GA7AL)
   on [CNCF Slack](https://communityinviter.com/apps/cloud-native/cncf)
-- Security issues: [*Report a vulnerability*](https://github.com/secure-systems-lab/securesystemslib/security/advisories/new)
+- Security issues: see [Security policy](docs/SECURITY.md)
 - Other issues and requests: [*Open a new
   issue*](https://github.com/secure-systems-lab/securesystemslib/issues/new)
 
-## Testing
-`tox` is used for testing. It can be installed via
-[pip](https://tox.wiki/en/4.9.0/installation.html#via-pip) and executed from the
-command line in the root of the repository.
-
-```bash
-tox
-```
+## Contribute
+See [Instructions for contributors](docs/CONTRIBUTING.md).
 
 ## Legacy key migration
 
-Use [`migrate_keys`](docs/migrate_key.py) script to convert key pairs generated
-with legacy `keys` or `interface` modules to a consistent standard format, which
-is compatible with [`CryptoSigner`](docs/CRYPTO_SIGNER.md).
+Use
+[`migrate_keys`](https://github.com/secure-systems-lab/securesystemslib/blob/v0.31.0/docs/migrate_key.py)
+script to convert key pairs generated with legacy `keys` or `interface` modules
+to a consistent standard format, which is compatible with
+[`CryptoSigner`](docs/CRYPTO_SIGNER.md). The script requires
+`securesystemslib~=0.31.0`.
```

### Comparing `securesystemslib-0.31.0/pyproject.toml` & `securesystemslib-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 [build-system]
-# Version needs manual updates (dependabot/dependabot-core#8465)
-requires = ["hatchling==1.18.0"]
+# Dependabot cannot do `build-system.requires` (dependabot/dependabot-core#8465)
+# workaround to get reproducibility and auto-updates:
+#   PIP_CONSTRAINT=requirements/build.txt python3 -m build ...
+requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "securesystemslib"
 authors = [{name = "https://www.updateframework.com", email = "theupdateframework@googlegroups.com"}]
 license = {text = "MIT"}
 description = "A library that provides cryptographic and general-purpose routines for Secure Systems Lab projects at NYU"
@@ -45,17 +47,17 @@
 
 [project.optional-dependencies]
 crypto = ["cryptography>=40.0.0"]
 gcpkms = ["google-cloud-kms", "cryptography>=40.0.0"]
 azurekms = ["azure-identity", "azure-keyvault-keys", "cryptography>=40.0.0"]
 awskms = ["boto3", "botocore", "cryptography>=40.0.0"]
 hsm = ["asn1crypto", "cryptography>=40.0.0", "PyKCS11"]
-pynacl = ["pynacl>1.2.0"]
 PySPX = ["PySPX>=0.5.0"]
 sigstore = ["sigstore~=2.0"]
+vault = ["hvac", "cryptography>=40.0.0"]
 
 [tool.hatch.version]
 path = "securesystemslib/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
   "/tests",
```

### Comparing `securesystemslib-0.31.0/PKG-INFO` & `securesystemslib-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: securesystemslib
-Version: 0.31.0
+Version: 1.0.0
 Summary: A library that provides cryptographic and general-purpose routines for Secure Systems Lab projects at NYU
 Project-URL: Homepage, https://github.com/secure-systems-lab/securesystemslib
 Project-URL: Source, https://github.com/secure-systems-lab/securesystemslib
 Project-URL: Issues, https://github.com/secure-systems-lab/securesystemslib/issues
 Author-email: "https://www.updateframework.com" <theupdateframework@googlegroups.com>
 License: MIT
 License-File: LICENSE
@@ -39,20 +39,21 @@
 Provides-Extra: gcpkms
 Requires-Dist: cryptography>=40.0.0; extra == 'gcpkms'
 Requires-Dist: google-cloud-kms; extra == 'gcpkms'
 Provides-Extra: hsm
 Requires-Dist: asn1crypto; extra == 'hsm'
 Requires-Dist: cryptography>=40.0.0; extra == 'hsm'
 Requires-Dist: pykcs11; extra == 'hsm'
-Provides-Extra: pynacl
-Requires-Dist: pynacl>1.2.0; extra == 'pynacl'
 Provides-Extra: pyspx
 Requires-Dist: pyspx>=0.5.0; extra == 'pyspx'
 Provides-Extra: sigstore
 Requires-Dist: sigstore~=2.0; extra == 'sigstore'
+Provides-Extra: vault
+Requires-Dist: cryptography>=40.0.0; extra == 'vault'
+Requires-Dist: hvac; extra == 'vault'
 Description-Content-Type: text/markdown
 
 # securesystemslib
 
 [![CI](https://github.com/secure-systems-lab/securesystemslib/workflows/Run%20Securesystemslib%20tests/badge.svg)](https://github.com/secure-systems-lab/securesystemslib/actions?query=workflow%3A%22Run+Securesystemslib+tests%22+branch%3Amain)
 [![Documentation Status](https://readthedocs.org/projects/python-securesystemslib/badge/?version=latest)](https://python-securesystemslib.readthedocs.io/en/latest/?badge=latest)
 
@@ -85,25 +86,22 @@
 ## Usage
 [python-securesystemslib.readthedocs.io](https://python-securesystemslib.readthedocs.io)
 
 ## Contact
 - Questions and discussions:
   [`#securesystemslib-python`](https://cloud-native.slack.com/archives/C05PF3GA7AL)
   on [CNCF Slack](https://communityinviter.com/apps/cloud-native/cncf)
-- Security issues: [*Report a vulnerability*](https://github.com/secure-systems-lab/securesystemslib/security/advisories/new)
+- Security issues: see [Security policy](docs/SECURITY.md)
 - Other issues and requests: [*Open a new
   issue*](https://github.com/secure-systems-lab/securesystemslib/issues/new)
 
-## Testing
-`tox` is used for testing. It can be installed via
-[pip](https://tox.wiki/en/4.9.0/installation.html#via-pip) and executed from the
-command line in the root of the repository.
-
-```bash
-tox
-```
+## Contribute
+See [Instructions for contributors](docs/CONTRIBUTING.md).
 
 ## Legacy key migration
 
-Use [`migrate_keys`](docs/migrate_key.py) script to convert key pairs generated
-with legacy `keys` or `interface` modules to a consistent standard format, which
-is compatible with [`CryptoSigner`](docs/CRYPTO_SIGNER.md).
+Use
+[`migrate_keys`](https://github.com/secure-systems-lab/securesystemslib/blob/v0.31.0/docs/migrate_key.py)
+script to convert key pairs generated with legacy `keys` or `interface` modules
+to a consistent standard format, which is compatible with
+[`CryptoSigner`](docs/CRYPTO_SIGNER.md). The script requires
+`securesystemslib~=0.31.0`.
```

