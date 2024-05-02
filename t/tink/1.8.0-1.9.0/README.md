# Comparing `tmp/tink-1.8.0.tar.gz` & `tmp/tink-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tink-1.8.0.tar", last modified: Mon Aug 28 07:39:39 2023, max compression
+gzip compressed data, was "tink-1.9.0.tar", last modified: Mon Nov 27 08:36:14 2023, max compression
```

## Comparing `tink-1.8.0.tar` & `tink-1.9.0.tar`

### file list

```diff
@@ -1,342 +1,352 @@
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.579123 tink-1.8.0/
--rw-rw-r--   0 root         (0) root         (0)      259 2023-08-28 07:38:37.000000 tink-1.8.0/.bazelrc
--rw-rw-r--   0 root         (0) root         (0)        6 2023-08-28 07:38:37.000000 tink-1.8.0/.bazelversion
--rw-rw-r--   0 root         (0) root         (0)        0 2023-08-28 07:38:37.000000 tink-1.8.0/BUILD.bazel
--rw-rw-r--   0 root         (0) root         (0)    11358 2023-08-28 07:38:37.000000 tink-1.8.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      472 2023-08-28 07:38:37.000000 tink-1.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6337 2023-08-28 07:39:39.579123 tink-1.8.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     5659 2023-08-28 07:38:37.000000 tink-1.8.0/README.md
--rw-rw-r--   0 root         (0) root         (0)        6 2023-08-28 07:38:37.000000 tink-1.8.0/VERSION
--rw-rw-r--   0 root         (0) root         (0)      414 2023-08-28 07:38:37.000000 tink-1.8.0/WORKSPACE
--rw-rw-r--   0 root         (0) root         (0)      215 2023-08-28 07:38:37.000000 tink-1.8.0/requirements.in
--rw-rw-r--   0 root         (0) root         (0)    16812 2023-08-28 07:38:37.000000 tink-1.8.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-28 07:39:39.579123 tink-1.8.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     8673 2023-08-28 07:38:37.000000 tink-1.8.0/setup.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.499116 tink-1.8.0/tink/
--rw-rw-r--   0 root         (0) root         (0)     3847 2023-08-28 07:38:37.000000 tink-1.8.0/tink/BUILD.bazel
--rw-rw-r--   0 root         (0) root         (0)     1520 2023-08-28 07:38:37.000000 tink-1.8.0/tink/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11829 2023-08-28 07:38:37.000000 tink-1.8.0/tink/_keyset_handle.py
--rw-rw-r--   0 root         (0) root         (0)    12888 2023-08-28 07:38:37.000000 tink-1.8.0/tink/_keyset_handle_test.py
--rw-rw-r--   0 root         (0) root         (0)     2497 2023-08-28 07:38:37.000000 tink-1.8.0/tink/_keyset_reader.py
--rw-rw-r--   0 root         (0) root         (0)     6202 2023-08-28 07:38:37.000000 tink-1.8.0/tink/_keyset_reader_test.py
--rw-rw-r--   0 root         (0) root         (0)     2912 2023-08-28 07:38:37.000000 tink-1.8.0/tink/_keyset_writer.py
--rw-rw-r--   0 root         (0) root         (0)     4531 2023-08-28 07:38:37.000000 tink-1.8.0/tink/_keyset_writer_test.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.503116 tink-1.8.0/tink/aead/
--rw-rw-r--   0 root         (0) root         (0)     3796 2023-08-28 07:38:37.000000 tink-1.8.0/tink/aead/BUILD.bazel
--rw-rw-r--   0 root         (0) root         (0)      937 2023-08-28 07:38:37.000000 tink-1.8.0/tink/aead/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2133 2023-08-28 07:38:37.000000 tink-1.8.0/tink/aead/_aead.py
--rw-rw-r--   0 root         (0) root         (0)     2174 2023-08-28 07:38:37.000000 tink-1.8.0/tink/aead/_aead_key_manager.py
--rw-rw-r--   0 root         (0) root         (0)    11260 2023-08-28 07:38:37.000000 tink-1.8.0/tink/aead/_aead_key_manager_test.py
--rw-rw-r--   0 root         (0) root         (0)     9938 2023-08-28 07:38:37.000000 tink-1.8.0/tink/aead/_aead_key_templates.py
--rw-rw-r--   0 root         (0) root         (0)     5270 2023-08-28 07:38:37.000000 tink-1.8.0/tink/aead/_aead_key_templates_test.py
--rw-rw-r--   0 root         (0) root         (0)     2687 2023-08-28 07:38:37.000000 tink-1.8.0/tink/aead/_aead_wrapper.py
--rw-rw-r--   0 root         (0) root         (0)     4993 2023-08-28 07:38:37.000000 tink-1.8.0/tink/aead/_aead_wrapper_test.py
--rw-rw-r--   0 root         (0) root         (0)     4665 2023-08-28 07:38:37.000000 tink-1.8.0/tink/aead/_kms_aead_key_manager.py
--rw-rw-r--   0 root         (0) root         (0)     5069 2023-08-28 07:38:37.000000 tink-1.8.0/tink/aead/_kms_aead_key_manager_test.py
--rw-rw-r--   0 root         (0) root         (0)     4419 2023-08-28 07:38:37.000000 tink-1.8.0/tink/aead/_kms_envelope_aead.py
--rw-rw-r--   0 root         (0) root         (0)     6561 2023-08-28 07:38:37.000000 tink-1.8.0/tink/aead/_kms_envelope_aead_test.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.511117 tink-1.8.0/tink/cc/
--rw-rw-r--   0 root         (0) root         (0)     6544 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/BUILD.bazel
--rw-rw-r--   0 root         (0) root         (0)      912 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/cc_hpke_config.cc
--rw-rw-r--   0 root         (0) root         (0)      964 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/cc_hpke_config.h
--rw-rw-r--   0 root         (0) root         (0)     2107 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/cc_jwt_config.cc
--rw-rw-r--   0 root         (0) root         (0)     1001 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/cc_jwt_config.h
--rw-rw-r--   0 root         (0) root         (0)     4583 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/cc_key_manager.h
--rw-rw-r--   0 root         (0) root         (0)     2347 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/cc_streaming_aead_wrappers.cc
--rw-rw-r--   0 root         (0) root         (0)     2493 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/cc_streaming_aead_wrappers.h
--rw-rw-r--   0 root         (0) root         (0)     1729 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/cc_streaming_aead_wrappers_test.cc
--rw-rw-r--   0 root         (0) root         (0)     1083 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/cc_tink_config.cc
--rw-rw-r--   0 root         (0) root         (0)      983 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/cc_tink_config.h
--rw-rw-r--   0 root         (0) root         (0)     1464 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/input_stream_adapter.cc
--rw-rw-r--   0 root         (0) root         (0)     1558 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/input_stream_adapter.h
--rw-rw-r--   0 root         (0) root         (0)     4136 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/input_stream_adapter_test.cc
--rw-rw-r--   0 root         (0) root         (0)     1561 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/output_stream_adapter.cc
--rw-rw-r--   0 root         (0) root         (0)     1807 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/output_stream_adapter.h
--rw-rw-r--   0 root         (0) root         (0)     3492 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/output_stream_adapter_test.cc
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.523118 tink-1.8.0/tink/cc/pybind/
--rw-rw-r--   0 root         (0) root         (0)     6812 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/BUILD.bazel
--rw-rw-r--   0 root         (0) root         (0)     3178 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/aead.cc
--rw-rw-r--   0 root         (0) root         (0)      969 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/aead.h
--rw-rw-r--   0 root         (0) root         (0)     1264 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/cc_hpke_config.cc
--rw-rw-r--   0 root         (0) root         (0)     1003 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/cc_hpke_config.h
--rw-rw-r--   0 root         (0) root         (0)     1246 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/cc_jwt_config.cc
--rw-rw-r--   0 root         (0) root         (0)      997 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/cc_jwt_config.h
--rw-rw-r--   0 root         (0) root         (0)     3745 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/cc_key_manager.cc
--rw-rw-r--   0 root         (0) root         (0)     1002 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/cc_key_manager.h
--rw-rw-r--   0 root         (0) root         (0)    25593 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/cc_key_manager_test.py
--rw-rw-r--   0 root         (0) root         (0)     2800 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/cc_streaming_aead_wrappers.cc
--rw-rw-r--   0 root         (0) root         (0)     1048 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/cc_streaming_aead_wrappers.h
--rw-rw-r--   0 root         (0) root         (0)     1025 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/cc_tink_config.cc
--rw-rw-r--   0 root         (0) root         (0)     1001 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/cc_tink_config.h
--rw-rw-r--   0 root         (0) root         (0)      855 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/cc_tink_config_test.py
--rw-rw-r--   0 root         (0) root         (0)     3658 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/deterministic_aead.cc
--rw-rw-r--   0 root         (0) root         (0)     1019 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/deterministic_aead.h
--rw-rw-r--   0 root         (0) root         (0)     1821 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/hybrid_decrypt.cc
--rw-rw-r--   0 root         (0) root         (0)     1003 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/hybrid_decrypt.h
--rw-rw-r--   0 root         (0) root         (0)     1816 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/hybrid_encrypt.cc
--rw-rw-r--   0 root         (0) root         (0)     1003 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/hybrid_encrypt.h
--rw-rw-r--   0 root         (0) root         (0)     1141 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/import_helper.cc
--rw-rw-r--   0 root         (0) root         (0)     1205 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/import_helper.h
--rw-rw-r--   0 root         (0) root         (0)     2359 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/input_stream_adapter.cc
--rw-rw-r--   0 root         (0) root         (0)     1026 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/input_stream_adapter.h
--rw-rw-r--   0 root         (0) root         (0)     2515 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/mac.cc
--rw-rw-r--   0 root         (0) root         (0)      960 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/mac.h
--rw-rw-r--   0 root         (0) root         (0)     1829 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/output_stream_adapter.cc
--rw-rw-r--   0 root         (0) root         (0)     1030 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/output_stream_adapter.h
--rw-rw-r--   0 root         (0) root         (0)     1886 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/prf.cc
--rw-rw-r--   0 root         (0) root         (0)      965 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/prf.h
--rw-rw-r--   0 root         (0) root         (0)     2239 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/public_key_sign.cc
--rw-rw-r--   0 root         (0) root         (0)     1006 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/public_key_sign.h
--rw-rw-r--   0 root         (0) root         (0)     2329 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/public_key_verify.cc
--rw-rw-r--   0 root         (0) root         (0)     1013 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/public_key_verify.h
--rw-rw-r--   0 root         (0) root         (0)     4757 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/python_file_object_adapter.cc
--rw-rw-r--   0 root         (0) root         (0)     1049 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/python_file_object_adapter.h
--rw-rw-r--   0 root         (0) root         (0)     1882 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/streaming_aead.cc
--rw-rw-r--   0 root         (0) root         (0)     1008 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/streaming_aead.h
--rw-rw-r--   0 root         (0) root         (0)     2388 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/tink_bindings.cc
--rw-rw-r--   0 root         (0) root         (0)     1425 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/pybind/tink_exception.h
--rw-rw-r--   0 root         (0) root         (0)     1782 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/python_file_object_adapter.h
--rw-rw-r--   0 root         (0) root         (0)     3353 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/python_input_stream.cc
--rw-rw-r--   0 root         (0) root         (0)     2225 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/python_input_stream.h
--rw-rw-r--   0 root         (0) root         (0)     6559 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/python_input_stream_test.cc
--rw-rw-r--   0 root         (0) root         (0)     4123 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/python_output_stream.cc
--rw-rw-r--   0 root         (0) root         (0)     2256 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/python_output_stream.h
--rw-rw-r--   0 root         (0) root         (0)     7393 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/python_output_stream_test.cc
--rw-rw-r--   0 root         (0) root         (0)    11525 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cc/test_util.h
--rw-rw-r--   0 root         (0) root         (0)     1468 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cleartext_keyset_handle.py
--rw-rw-r--   0 root         (0) root         (0)     2013 2023-08-28 07:38:37.000000 tink-1.8.0/tink/cleartext_keyset_handle_test.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.527119 tink-1.8.0/tink/core/
--rw-rw-r--   0 root         (0) root         (0)     2575 2023-08-28 07:38:37.000000 tink-1.8.0/tink/core/BUILD.bazel
--rw-rw-r--   0 root         (0) root         (0)     1450 2023-08-28 07:38:37.000000 tink-1.8.0/tink/core/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1494 2023-08-28 07:38:37.000000 tink-1.8.0/tink/core/_crypto_format.py
--rw-rw-r--   0 root         (0) root         (0)     2729 2023-08-28 07:38:37.000000 tink-1.8.0/tink/core/_crypto_format_test.py
--rw-rw-r--   0 root         (0) root         (0)     5259 2023-08-28 07:38:37.000000 tink-1.8.0/tink/core/_key_manager.py
--rw-rw-r--   0 root         (0) root         (0)     3610 2023-08-28 07:38:37.000000 tink-1.8.0/tink/core/_primitive_set.py
--rw-rw-r--   0 root         (0) root         (0)     9880 2023-08-28 07:38:37.000000 tink-1.8.0/tink/core/_primitive_set_test.py
--rw-rw-r--   0 root         (0) root         (0)     1766 2023-08-28 07:38:37.000000 tink-1.8.0/tink/core/_primitive_wrapper.py
--rw-rw-r--   0 root         (0) root         (0)     9078 2023-08-28 07:38:37.000000 tink-1.8.0/tink/core/_registry.py
--rw-rw-r--   0 root         (0) root         (0)    14510 2023-08-28 07:38:37.000000 tink-1.8.0/tink/core/_registry_test.py
--rw-rw-r--   0 root         (0) root         (0)     1302 2023-08-28 07:38:37.000000 tink-1.8.0/tink/core/_tink_error.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.527119 tink-1.8.0/tink/daead/
--rw-rw-r--   0 root         (0) root         (0)     2343 2023-08-28 07:38:37.000000 tink-1.8.0/tink/daead/BUILD.bazel
--rw-rw-r--   0 root         (0) root         (0)      914 2023-08-28 07:38:37.000000 tink-1.8.0/tink/daead/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1956 2023-08-28 07:38:37.000000 tink-1.8.0/tink/daead/_deterministic_aead.py
--rw-rw-r--   0 root         (0) root         (0)     2129 2023-08-28 07:38:37.000000 tink-1.8.0/tink/daead/_deterministic_aead_key_manager.py
--rw-rw-r--   0 root         (0) root         (0)     2555 2023-08-28 07:38:37.000000 tink-1.8.0/tink/daead/_deterministic_aead_key_manager_test.py
--rw-rw-r--   0 root         (0) root         (0)     1788 2023-08-28 07:38:37.000000 tink-1.8.0/tink/daead/_deterministic_aead_key_templates.py
--rw-rw-r--   0 root         (0) root         (0)     1624 2023-08-28 07:38:37.000000 tink-1.8.0/tink/daead/_deterministic_aead_key_templates_test.py
--rw-rw-r--   0 root         (0) root         (0)     3400 2023-08-28 07:38:37.000000 tink-1.8.0/tink/daead/_deterministic_aead_wrapper.py
--rw-rw-r--   0 root         (0) root         (0)     5917 2023-08-28 07:38:37.000000 tink-1.8.0/tink/daead/_deterministic_aead_wrapper_test.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.531119 tink-1.8.0/tink/hybrid/
--rw-rw-r--   0 root         (0) root         (0)     2710 2023-08-28 07:38:37.000000 tink-1.8.0/tink/hybrid/BUILD.bazel
--rw-rw-r--   0 root         (0) root         (0)      927 2023-08-28 07:38:37.000000 tink-1.8.0/tink/hybrid/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2470 2023-08-28 07:38:37.000000 tink-1.8.0/tink/hybrid/_hybrid_decrypt.py
--rw-rw-r--   0 root         (0) root         (0)     2477 2023-08-28 07:38:37.000000 tink-1.8.0/tink/hybrid/_hybrid_encrypt.py
--rw-rw-r--   0 root         (0) root         (0)     3669 2023-08-28 07:38:37.000000 tink-1.8.0/tink/hybrid/_hybrid_key_manager.py
--rw-rw-r--   0 root         (0) root         (0)     8262 2023-08-28 07:38:37.000000 tink-1.8.0/tink/hybrid/_hybrid_key_manager_test.py
--rw-rw-r--   0 root         (0) root         (0)     5853 2023-08-28 07:38:37.000000 tink-1.8.0/tink/hybrid/_hybrid_key_templates.py
--rw-rw-r--   0 root         (0) root         (0)     3060 2023-08-28 07:38:37.000000 tink-1.8.0/tink/hybrid/_hybrid_key_templates_test.py
--rw-rw-r--   0 root         (0) root         (0)     4146 2023-08-28 07:38:37.000000 tink-1.8.0/tink/hybrid/_hybrid_wrapper.py
--rw-rw-r--   0 root         (0) root         (0)     9752 2023-08-28 07:38:37.000000 tink-1.8.0/tink/hybrid/_hybrid_wrapper_test.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.531119 tink-1.8.0/tink/integration/
--rw-rw-r--   0 root         (0) root         (0)      575 2023-08-28 07:38:37.000000 tink-1.8.0/tink/integration/__init__.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.531119 tink-1.8.0/tink/integration/awskms/
--rw-rw-r--   0 root         (0) root         (0)     1520 2023-08-28 07:38:37.000000 tink-1.8.0/tink/integration/awskms/BUILD.bazel
--rw-rw-r--   0 root         (0) root         (0)      709 2023-08-28 07:38:37.000000 tink-1.8.0/tink/integration/awskms/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6783 2023-08-28 07:38:37.000000 tink-1.8.0/tink/integration/awskms/_aws_kms_client.py
--rw-rw-r--   0 root         (0) root         (0)     4561 2023-08-28 07:38:37.000000 tink-1.8.0/tink/integration/awskms/_aws_kms_client_test.py
--rw-rw-r--   0 root         (0) root         (0)     8488 2023-08-28 07:38:37.000000 tink-1.8.0/tink/integration/awskms/_aws_kms_integration_test.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.535119 tink-1.8.0/tink/integration/gcpkms/
--rw-rw-r--   0 root         (0) root         (0)     1836 2023-08-28 07:38:37.000000 tink-1.8.0/tink/integration/gcpkms/BUILD.bazel
--rw-rw-r--   0 root         (0) root         (0)      697 2023-08-28 07:38:37.000000 tink-1.8.0/tink/integration/gcpkms/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5046 2023-08-28 07:38:37.000000 tink-1.8.0/tink/integration/gcpkms/_gcp_kms_client.py
--rw-rw-r--   0 root         (0) root         (0)     5805 2023-08-28 07:38:37.000000 tink-1.8.0/tink/integration/gcpkms/_gcp_kms_client_integration_test.py
--rw-rw-r--   0 root         (0) root         (0)     2345 2023-08-28 07:38:37.000000 tink-1.8.0/tink/integration/gcpkms/_gcp_kms_client_test.py
--rw-rw-r--   0 root         (0) root         (0)     9743 2023-08-28 07:38:37.000000 tink-1.8.0/tink/integration/gcpkms/_gcp_kms_integration_test.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.535119 tink-1.8.0/tink/internal/
--rw-rw-r--   0 root         (0) root         (0)      504 2023-08-28 07:38:37.000000 tink-1.8.0/tink/internal/BUILD.bazel
--rw-rw-r--   0 root         (0) root         (0)      575 2023-08-28 07:38:37.000000 tink-1.8.0/tink/internal/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      918 2023-08-28 07:38:37.000000 tink-1.8.0/tink/internal/big_integer_util.py
--rw-rw-r--   0 root         (0) root         (0)     1578 2023-08-28 07:38:37.000000 tink-1.8.0/tink/internal/big_integer_util_test.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.543120 tink-1.8.0/tink/jwt/
--rw-rw-r--   0 root         (0) root         (0)     7950 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/BUILD.bazel
--rw-rw-r--   0 root         (0) root         (0)     4228 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2124 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_json_util.py
--rw-rw-r--   0 root         (0) root         (0)     2001 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_json_util_test.py
--rw-rw-r--   0 root         (0) root         (0)    12814 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_jwk_set_converter.py
--rw-rw-r--   0 root         (0) root         (0)    37848 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_jwk_set_converter_test.py
--rw-rw-r--   0 root         (0) root         (0)      682 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_jwt_error.py
--rw-rw-r--   0 root         (0) root         (0)     7133 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_jwt_format.py
--rw-rw-r--   0 root         (0) root         (0)    17449 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_jwt_format_test.py
--rw-rw-r--   0 root         (0) root         (0)     5063 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_jwt_hmac_key_manager.py
--rw-rw-r--   0 root         (0) root         (0)    12970 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_jwt_hmac_key_manager_test.py
--rw-rw-r--   0 root         (0) root         (0)     7622 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_jwt_key_templates.py
--rw-rw-r--   0 root         (0) root         (0)     3975 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_jwt_key_templates_test.py
--rw-rw-r--   0 root         (0) root         (0)     3153 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_jwt_mac.py
--rw-rw-r--   0 root         (0) root         (0)     3344 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_jwt_mac_wrapper.py
--rw-rw-r--   0 root         (0) root         (0)    10572 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_jwt_mac_wrapper_test.py
--rw-rw-r--   0 root         (0) root         (0)     1674 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_jwt_public_key_sign.py
--rw-rw-r--   0 root         (0) root         (0)     2546 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_jwt_public_key_verify.py
--rw-rw-r--   0 root         (0) root         (0)    13099 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_jwt_signature_key_manager.py
--rw-rw-r--   0 root         (0) root         (0)    11632 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_jwt_signature_key_manager_test.py
--rw-rw-r--   0 root         (0) root         (0)     4077 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_jwt_signature_wrappers.py
--rw-rw-r--   0 root         (0) root         (0)    13424 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_jwt_signature_wrappers_test.py
--rw-rw-r--   0 root         (0) root         (0)     8268 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_jwt_validator.py
--rw-rw-r--   0 root         (0) root         (0)    14891 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_jwt_validator_test.py
--rw-rw-r--   0 root         (0) root         (0)     9502 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_raw_jwt.py
--rw-rw-r--   0 root         (0) root         (0)    16306 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_raw_jwt_test.py
--rw-rw-r--   0 root         (0) root         (0)     2910 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_verified_jwt.py
--rw-rw-r--   0 root         (0) root         (0)     4149 2023-08-28 07:38:37.000000 tink-1.8.0/tink/jwt/_verified_jwt_test.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.547120 tink-1.8.0/tink/mac/
--rw-rw-r--   0 root         (0) root         (0)     2216 2023-08-28 07:38:37.000000 tink-1.8.0/tink/mac/BUILD.bazel
--rw-rw-r--   0 root         (0) root         (0)      774 2023-08-28 07:38:37.000000 tink-1.8.0/tink/mac/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1698 2023-08-28 07:38:37.000000 tink-1.8.0/tink/mac/_mac.py
--rw-rw-r--   0 root         (0) root         (0)     1665 2023-08-28 07:38:37.000000 tink-1.8.0/tink/mac/_mac_key_manager.py
--rw-rw-r--   0 root         (0) root         (0)     2921 2023-08-28 07:38:37.000000 tink-1.8.0/tink/mac/_mac_key_manager_test.py
--rw-rw-r--   0 root         (0) root         (0)     3369 2023-08-28 07:38:37.000000 tink-1.8.0/tink/mac/_mac_key_templates.py
--rw-rw-r--   0 root         (0) root         (0)     2048 2023-08-28 07:38:37.000000 tink-1.8.0/tink/mac/_mac_key_templates_test.py
--rw-rw-r--   0 root         (0) root         (0)     3361 2023-08-28 07:38:37.000000 tink-1.8.0/tink/mac/_mac_wrapper.py
--rw-rw-r--   0 root         (0) root         (0)     5000 2023-08-28 07:38:37.000000 tink-1.8.0/tink/mac/_mac_wrapper_test.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.547120 tink-1.8.0/tink/prf/
--rw-rw-r--   0 root         (0) root         (0)     1961 2023-08-28 07:38:37.000000 tink-1.8.0/tink/prf/BUILD.bazel
--rw-rw-r--   0 root         (0) root         (0)      809 2023-08-28 07:38:37.000000 tink-1.8.0/tink/prf/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1720 2023-08-28 07:38:37.000000 tink-1.8.0/tink/prf/_prf_key_manager.py
--rw-rw-r--   0 root         (0) root         (0)     3336 2023-08-28 07:38:37.000000 tink-1.8.0/tink/prf/_prf_key_manager_test.py
--rw-rw-r--   0 root         (0) root         (0)     3087 2023-08-28 07:38:37.000000 tink-1.8.0/tink/prf/_prf_key_templates.py
--rw-rw-r--   0 root         (0) root         (0)     3127 2023-08-28 07:38:37.000000 tink-1.8.0/tink/prf/_prf_set.py
--rw-rw-r--   0 root         (0) root         (0)     1838 2023-08-28 07:38:37.000000 tink-1.8.0/tink/prf/_prf_set_wrapper.py
--rw-rw-r--   0 root         (0) root         (0)     2749 2023-08-28 07:38:37.000000 tink-1.8.0/tink/prf/_prf_set_wrapper_test.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.567122 tink-1.8.0/tink/proto/
--rw-rw-r--   0 root         (0) root         (0)     5468 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/BUILD.bazel
--rw-rw-r--   0 root         (0) root         (0)      575 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1176 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/aes_cmac.proto
--rw-r--r--   0 root         (0) root         (0)     1695 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/aes_cmac_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1104 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/aes_cmac_prf.proto
--rw-r--r--   0 root         (0) root         (0)     1486 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/aes_cmac_prf_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1168 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/aes_ctr.proto
--rw-rw-r--   0 root         (0) root         (0)     1254 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/aes_ctr_hmac_aead.proto
--rw-r--r--   0 root         (0) root         (0)     1972 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/aes_ctr_hmac_aead_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1697 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/aes_ctr_hmac_streaming.proto
--rw-r--r--   0 root         (0) root         (0)     2390 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/aes_ctr_hmac_streaming_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1692 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/aes_ctr_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1247 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/aes_eax.proto
--rw-r--r--   0 root         (0) root         (0)     1692 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/aes_eax_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     2589 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/aes_gcm.proto
--rw-rw-r--   0 root         (0) root         (0)     1599 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/aes_gcm_hkdf_streaming.proto
--rw-r--r--   0 root         (0) root         (0)     2215 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/aes_gcm_hkdf_streaming_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/aes_gcm_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1194 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/aes_gcm_siv.proto
--rw-r--r--   0 root         (0) root         (0)     1486 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/aes_gcm_siv_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1570 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/aes_siv.proto
--rw-r--r--   0 root         (0) root         (0)     1440 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/aes_siv_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1202 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/chacha20_poly1305.proto
--rw-r--r--   0 root         (0) root         (0)     1477 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/chacha20_poly1305_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1513 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/common.proto
--rw-r--r--   0 root         (0) root         (0)     1840 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/common_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1977 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/config.proto
--rw-r--r--   0 root         (0) root         (0)     1833 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/config_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     2554 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/ecdsa.proto
--rw-r--r--   0 root         (0) root         (0)     2538 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/ecdsa_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     3571 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/ecies_aead_hkdf.proto
--rw-r--r--   0 root         (0) root         (0)     3059 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/ecies_aead_hkdf_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1753 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/ed25519.proto
--rw-r--r--   0 root         (0) root         (0)     1747 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/ed25519_pb2.py
--rw-rw-r--   0 root         (0) root         (0)      900 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/empty.proto
--rw-r--r--   0 root         (0) root         (0)     1161 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/empty_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1390 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/hkdf_prf.proto
--rw-r--r--   0 root         (0) root         (0)     1888 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/hkdf_prf_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1257 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/hmac.proto
--rw-r--r--   0 root         (0) root         (0)     1843 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/hmac_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1255 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/hmac_prf.proto
--rw-r--r--   0 root         (0) root         (0)     1858 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/hmac_prf_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1894 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/hpke.proto
--rw-r--r--   0 root         (0) root         (0)     2825 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/hpke_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1997 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/jwt_ecdsa.proto
--rw-r--r--   0 root         (0) root         (0)     2374 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/jwt_ecdsa_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1576 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/jwt_hmac.proto
--rw-r--r--   0 root         (0) root         (0)     2049 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/jwt_hmac_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     2735 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/jwt_rsa_ssa_pkcs1.proto
--rw-r--r--   0 root         (0) root         (0)     2773 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/jwt_rsa_ssa_pkcs1_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     2768 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/jwt_rsa_ssa_pss.proto
--rw-r--r--   0 root         (0) root         (0)     2734 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/jwt_rsa_ssa_pss_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1388 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/kms_aead.proto
--rw-r--r--   0 root         (0) root         (0)     1442 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/kms_aead_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1587 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/kms_envelope.proto
--rw-r--r--   0 root         (0) root         (0)     1701 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/kms_envelope_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1295 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/prf_based_deriver.proto
--rw-r--r--   0 root         (0) root         (0)     2071 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/prf_based_deriver_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     2778 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/rsa_ssa_pkcs1.proto
--rw-r--r--   0 root         (0) root         (0)     2462 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/rsa_ssa_pkcs1_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     3092 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/rsa_ssa_pss.proto
--rw-r--r--   0 root         (0) root         (0)     2545 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/rsa_ssa_pss_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1068 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/test_proto.proto
--rw-r--r--   0 root         (0) root         (0)     1921 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/test_proto_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     7229 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/tink.proto
--rw-r--r--   0 root         (0) root         (0)     3912 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/tink_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1109 2023-08-28 07:38:37.000000 tink-1.8.0/tink/proto/xchacha20_poly1305.proto
--rw-r--r--   0 root         (0) root         (0)     1516 2023-08-28 07:39:39.000000 tink-1.8.0/tink/proto/xchacha20_poly1305_pb2.py
--rw-rw-r--   0 root         (0) root         (0)      882 2023-08-28 07:38:37.000000 tink-1.8.0/tink/secret_key_access.py
--rw-rw-r--   0 root         (0) root         (0)     1268 2023-08-28 07:38:37.000000 tink-1.8.0/tink/secret_key_access_test.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.571123 tink-1.8.0/tink/signature/
--rw-rw-r--   0 root         (0) root         (0)     2338 2023-08-28 07:38:37.000000 tink-1.8.0/tink/signature/BUILD.bazel
--rw-rw-r--   0 root         (0) root         (0)      966 2023-08-28 07:38:37.000000 tink-1.8.0/tink/signature/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1380 2023-08-28 07:38:37.000000 tink-1.8.0/tink/signature/_public_key_sign.py
--rw-rw-r--   0 root         (0) root         (0)     1507 2023-08-28 07:38:37.000000 tink-1.8.0/tink/signature/_public_key_verify.py
--rw-rw-r--   0 root         (0) root         (0)     2887 2023-08-28 07:38:37.000000 tink-1.8.0/tink/signature/_signature_key_manager.py
--rw-rw-r--   0 root         (0) root         (0)     4901 2023-08-28 07:38:37.000000 tink-1.8.0/tink/signature/_signature_key_manager_test.py
--rw-rw-r--   0 root         (0) root         (0)     7852 2023-08-28 07:38:37.000000 tink-1.8.0/tink/signature/_signature_key_templates.py
--rw-rw-r--   0 root         (0) root         (0)     5265 2023-08-28 07:38:37.000000 tink-1.8.0/tink/signature/_signature_wrapper.py
--rw-rw-r--   0 root         (0) root         (0)     5885 2023-08-28 07:38:37.000000 tink-1.8.0/tink/signature/_signature_wrapper_test.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.575123 tink-1.8.0/tink/streaming_aead/
--rw-rw-r--   0 root         (0) root         (0)     5481 2023-08-28 07:38:37.000000 tink-1.8.0/tink/streaming_aead/BUILD.bazel
--rw-rw-r--   0 root         (0) root         (0)      904 2023-08-28 07:38:37.000000 tink-1.8.0/tink/streaming_aead/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4767 2023-08-28 07:38:37.000000 tink-1.8.0/tink/streaming_aead/_decrypting_stream.py
--rw-rw-r--   0 root         (0) root         (0)     2896 2023-08-28 07:38:37.000000 tink-1.8.0/tink/streaming_aead/_decrypting_stream_test.py
--rw-rw-r--   0 root         (0) root         (0)     3874 2023-08-28 07:38:37.000000 tink-1.8.0/tink/streaming_aead/_encrypting_stream.py
--rw-rw-r--   0 root         (0) root         (0)     3778 2023-08-28 07:38:37.000000 tink-1.8.0/tink/streaming_aead/_encrypting_stream_test.py
--rw-rw-r--   0 root         (0) root         (0)     2165 2023-08-28 07:38:37.000000 tink-1.8.0/tink/streaming_aead/_file_object_adapter.py
--rw-rw-r--   0 root         (0) root         (0)     4079 2023-08-28 07:38:37.000000 tink-1.8.0/tink/streaming_aead/_file_object_adapter_test.py
--rw-rw-r--   0 root         (0) root         (0)     3176 2023-08-28 07:38:37.000000 tink-1.8.0/tink/streaming_aead/_pybind11_python_file_object_adapter_test.py
--rw-rw-r--   0 root         (0) root         (0)     4756 2023-08-28 07:38:37.000000 tink-1.8.0/tink/streaming_aead/_raw_streaming_aead.py
--rw-rw-r--   0 root         (0) root         (0)     3109 2023-08-28 07:38:37.000000 tink-1.8.0/tink/streaming_aead/_rewindable_input_stream.py
--rw-rw-r--   0 root         (0) root         (0)     6303 2023-08-28 07:38:37.000000 tink-1.8.0/tink/streaming_aead/_rewindable_input_stream_test.py
--rw-rw-r--   0 root         (0) root         (0)     4520 2023-08-28 07:38:37.000000 tink-1.8.0/tink/streaming_aead/_streaming_aead.py
--rw-rw-r--   0 root         (0) root         (0)     2894 2023-08-28 07:38:37.000000 tink-1.8.0/tink/streaming_aead/_streaming_aead_key_manager.py
--rw-rw-r--   0 root         (0) root         (0)    10488 2023-08-28 07:38:37.000000 tink-1.8.0/tink/streaming_aead/_streaming_aead_key_manager_test.py
--rw-rw-r--   0 root         (0) root         (0)     6540 2023-08-28 07:38:37.000000 tink-1.8.0/tink/streaming_aead/_streaming_aead_key_templates.py
--rw-rw-r--   0 root         (0) root         (0)     3569 2023-08-28 07:38:37.000000 tink-1.8.0/tink/streaming_aead/_streaming_aead_key_templates_test.py
--rw-rw-r--   0 root         (0) root         (0)     4470 2023-08-28 07:38:37.000000 tink-1.8.0/tink/streaming_aead/_streaming_aead_test.py
--rw-rw-r--   0 root         (0) root         (0)     6692 2023-08-28 07:38:37.000000 tink-1.8.0/tink/streaming_aead/_streaming_aead_wrapper.py
--rw-rw-r--   0 root         (0) root         (0)    12060 2023-08-28 07:38:37.000000 tink-1.8.0/tink/streaming_aead/_streaming_aead_wrapper_test.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.579123 tink-1.8.0/tink/testing/
--rw-rw-r--   0 root         (0) root         (0)     2181 2023-08-28 07:38:37.000000 tink-1.8.0/tink/testing/BUILD.bazel
--rw-rw-r--   0 root         (0) root         (0)      575 2023-08-28 07:38:37.000000 tink-1.8.0/tink/testing/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3518 2023-08-28 07:38:37.000000 tink-1.8.0/tink/testing/bytes_io.py
--rw-rw-r--   0 root         (0) root         (0)     5461 2023-08-28 07:38:37.000000 tink-1.8.0/tink/testing/bytes_io_test.py
--rw-rw-r--   0 root         (0) root         (0)     1914 2023-08-28 07:38:37.000000 tink-1.8.0/tink/testing/fake_kms.py
--rw-rw-r--   0 root         (0) root         (0)     2242 2023-08-28 07:38:37.000000 tink-1.8.0/tink/testing/fake_kms_test.py
--rw-rw-r--   0 root         (0) root         (0)     6601 2023-08-28 07:38:37.000000 tink-1.8.0/tink/testing/helper.py
--rw-rw-r--   0 root         (0) root         (0)     5409 2023-08-28 07:38:37.000000 tink-1.8.0/tink/testing/helper_test.py
--rw-rw-r--   0 root         (0) root         (0)     4487 2023-08-28 07:38:37.000000 tink-1.8.0/tink/testing/keyset_builder.py
--rw-rw-r--   0 root         (0) root         (0)     7016 2023-08-28 07:38:37.000000 tink-1.8.0/tink/testing/keyset_builder_test.py
--rw-rw-r--   0 root         (0) root         (0)      965 2023-08-28 07:38:37.000000 tink-1.8.0/tink/tink_config.py
--rw-rw-r--   0 root         (0) root         (0)     4207 2023-08-28 07:38:37.000000 tink-1.8.0/tink/tink_config_test.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.499116 tink-1.8.0/tink.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6337 2023-08-28 07:39:39.000000 tink-1.8.0/tink.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9983 2023-08-28 07:39:39.000000 tink-1.8.0/tink.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-28 07:39:39.000000 tink-1.8.0/tink.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-28 07:39:39.000000 tink-1.8.0/tink.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      173 2023-08-28 07:39:39.000000 tink-1.8.0/tink.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-08-28 07:39:39.000000 tink-1.8.0/tink.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)     2897 2023-08-28 07:38:37.000000 tink-1.8.0/tink_py_deps.bzl
--rw-rw-r--   0 root         (0) root         (0)      925 2023-08-28 07:38:37.000000 tink-1.8.0/tink_py_deps_init.bzl
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.579123 tink-1.8.0/tools/
--rw-rw-r--   0 root         (0) root         (0)       76 2023-08-28 07:38:37.000000 tink-1.8.0/tools/BUILD.bazel
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-08-28 07:39:39.579123 tink-1.8.0/tools/distribution/
--rwxrwxr-x   0 root         (0) root         (0)     3841 2023-08-28 07:38:37.000000 tink-1.8.0/tools/distribution/build_linux_binary_wheels.sh
--rwxrwxr-x   0 root         (0) root         (0)     8664 2023-08-28 07:38:37.000000 tink-1.8.0/tools/distribution/create_bdist.sh
--rwxrwxr-x   0 root         (0) root         (0)     2918 2023-08-28 07:38:37.000000 tink-1.8.0/tools/distribution/create_sdist.sh
--rw-rw-r--   0 root         (0) root         (0)       30 2023-08-28 07:38:37.000000 tink-1.8.0/tools/distribution/requirements.in
--rw-rw-r--   0 root         (0) root         (0)     1661 2023-08-28 07:38:37.000000 tink-1.8.0/tools/distribution/requirements.txt
--rwxrwxr-x   0 root         (0) root         (0)     4868 2023-08-28 07:38:37.000000 tink-1.8.0/tools/distribution/test_dist.sh
--rwxrwxr-x   0 root         (0) root         (0)     2825 2023-08-28 07:38:37.000000 tink-1.8.0/tools/distribution/test_linux_binary_wheel.sh
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.614238 tink-1.9.0/
+-rw-rw-r--   0 root         (0) root         (0)      259 2023-11-27 08:35:14.000000 tink-1.9.0/.bazelrc
+-rw-rw-r--   0 root         (0) root         (0)        6 2023-11-27 08:35:14.000000 tink-1.9.0/.bazelversion
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-11-27 08:35:14.000000 tink-1.9.0/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)    11358 2023-11-27 08:35:14.000000 tink-1.9.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      575 2023-11-27 08:35:14.000000 tink-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7065 2023-11-27 08:36:14.610237 tink-1.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     5659 2023-11-27 08:35:14.000000 tink-1.9.0/README.md
+-rw-rw-r--   0 root         (0) root         (0)        6 2023-11-27 08:35:14.000000 tink-1.9.0/VERSION
+-rw-rw-r--   0 root         (0) root         (0)      377 2023-11-27 08:35:14.000000 tink-1.9.0/WORKSPACE
+-rw-rw-r--   0 root         (0) root         (0)       89 2023-11-27 08:35:14.000000 tink-1.9.0/requirements.in
+-rw-rw-r--   0 root         (0) root         (0)    18623 2023-11-27 08:35:14.000000 tink-1.9.0/requirements_all.txt
+-rw-rw-r--   0 root         (0) root         (0)       15 2023-11-27 08:35:14.000000 tink-1.9.0/requirements_awskms.in
+-rw-rw-r--   0 root         (0) root         (0)       69 2023-11-27 08:35:14.000000 tink-1.9.0/requirements_gcpkms.in
+-rw-r--r--   0 root         (0) root         (0)       38 2023-11-27 08:36:14.614238 tink-1.9.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     8111 2023-11-27 08:35:14.000000 tink-1.9.0/setup.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.526230 tink-1.9.0/tink/
+-rw-rw-r--   0 root         (0) root         (0)     6217 2023-11-27 08:35:14.000000 tink-1.9.0/tink/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)     2142 2023-11-27 08:35:14.000000 tink-1.9.0/tink/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1362 2023-11-27 08:35:14.000000 tink-1.9.0/tink/_insecure_keyset_handle.py
+-rw-rw-r--   0 root         (0) root         (0)     2071 2023-11-27 08:35:14.000000 tink-1.9.0/tink/_insecure_keyset_handle_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2945 2023-11-27 08:35:14.000000 tink-1.9.0/tink/_json_proto_keyset_format.py
+-rw-rw-r--   0 root         (0) root         (0)     8769 2023-11-27 08:35:14.000000 tink-1.9.0/tink/_json_proto_keyset_format_test.py
+-rw-rw-r--   0 root         (0) root         (0)    11829 2023-11-27 08:35:14.000000 tink-1.9.0/tink/_keyset_handle.py
+-rw-rw-r--   0 root         (0) root         (0)    12888 2023-11-27 08:35:14.000000 tink-1.9.0/tink/_keyset_handle_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2497 2023-11-27 08:35:14.000000 tink-1.9.0/tink/_keyset_reader.py
+-rw-rw-r--   0 root         (0) root         (0)     6202 2023-11-27 08:35:14.000000 tink-1.9.0/tink/_keyset_reader_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2912 2023-11-27 08:35:14.000000 tink-1.9.0/tink/_keyset_writer.py
+-rw-rw-r--   0 root         (0) root         (0)     4531 2023-11-27 08:35:14.000000 tink-1.9.0/tink/_keyset_writer_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2115 2023-11-27 08:35:14.000000 tink-1.9.0/tink/_kms_clients.py
+-rw-rw-r--   0 root         (0) root         (0)     1838 2023-11-27 08:35:14.000000 tink-1.9.0/tink/_kms_clients_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2966 2023-11-27 08:35:14.000000 tink-1.9.0/tink/_proto_keyset_format.py
+-rw-rw-r--   0 root         (0) root         (0)     8618 2023-11-27 08:35:14.000000 tink-1.9.0/tink/_proto_keyset_format_test.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.534231 tink-1.9.0/tink/aead/
+-rw-rw-r--   0 root         (0) root         (0)     4131 2023-11-27 08:35:14.000000 tink-1.9.0/tink/aead/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      937 2023-11-27 08:35:14.000000 tink-1.9.0/tink/aead/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2133 2023-11-27 08:35:14.000000 tink-1.9.0/tink/aead/_aead.py
+-rw-rw-r--   0 root         (0) root         (0)     2174 2023-11-27 08:35:14.000000 tink-1.9.0/tink/aead/_aead_key_manager.py
+-rw-rw-r--   0 root         (0) root         (0)    11223 2023-11-27 08:35:14.000000 tink-1.9.0/tink/aead/_aead_key_manager_test.py
+-rw-rw-r--   0 root         (0) root         (0)     9938 2023-11-27 08:35:14.000000 tink-1.9.0/tink/aead/_aead_key_templates.py
+-rw-rw-r--   0 root         (0) root         (0)     5270 2023-11-27 08:35:14.000000 tink-1.9.0/tink/aead/_aead_key_templates_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2567 2023-11-27 08:35:14.000000 tink-1.9.0/tink/aead/_aead_wrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     4993 2023-11-27 08:35:14.000000 tink-1.9.0/tink/aead/_aead_wrapper_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3889 2023-11-27 08:35:14.000000 tink-1.9.0/tink/aead/_kms_aead_key_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     4183 2023-11-27 08:35:14.000000 tink-1.9.0/tink/aead/_kms_aead_key_manager_test.py
+-rw-rw-r--   0 root         (0) root         (0)     4419 2023-11-27 08:35:14.000000 tink-1.9.0/tink/aead/_kms_envelope_aead.py
+-rw-rw-r--   0 root         (0) root         (0)     6561 2023-11-27 08:35:14.000000 tink-1.9.0/tink/aead/_kms_envelope_aead_test.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.538231 tink-1.9.0/tink/cc/
+-rw-rw-r--   0 root         (0) root         (0)     6544 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      912 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/cc_hpke_config.cc
+-rw-rw-r--   0 root         (0) root         (0)      964 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/cc_hpke_config.h
+-rw-rw-r--   0 root         (0) root         (0)     2107 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/cc_jwt_config.cc
+-rw-rw-r--   0 root         (0) root         (0)     1001 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/cc_jwt_config.h
+-rw-rw-r--   0 root         (0) root         (0)     4583 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/cc_key_manager.h
+-rw-rw-r--   0 root         (0) root         (0)     2347 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/cc_streaming_aead_wrappers.cc
+-rw-rw-r--   0 root         (0) root         (0)     2493 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/cc_streaming_aead_wrappers.h
+-rw-rw-r--   0 root         (0) root         (0)     1729 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/cc_streaming_aead_wrappers_test.cc
+-rw-rw-r--   0 root         (0) root         (0)     1083 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/cc_tink_config.cc
+-rw-rw-r--   0 root         (0) root         (0)      983 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/cc_tink_config.h
+-rw-rw-r--   0 root         (0) root         (0)     1464 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/input_stream_adapter.cc
+-rw-rw-r--   0 root         (0) root         (0)     1558 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/input_stream_adapter.h
+-rw-rw-r--   0 root         (0) root         (0)     4136 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/input_stream_adapter_test.cc
+-rw-rw-r--   0 root         (0) root         (0)     1561 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/output_stream_adapter.cc
+-rw-rw-r--   0 root         (0) root         (0)     1807 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/output_stream_adapter.h
+-rw-rw-r--   0 root         (0) root         (0)     3492 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/output_stream_adapter_test.cc
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.550232 tink-1.9.0/tink/cc/pybind/
+-rw-rw-r--   0 root         (0) root         (0)     6812 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)     3178 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/aead.cc
+-rw-rw-r--   0 root         (0) root         (0)      969 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/aead.h
+-rw-rw-r--   0 root         (0) root         (0)     1264 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/cc_hpke_config.cc
+-rw-rw-r--   0 root         (0) root         (0)     1003 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/cc_hpke_config.h
+-rw-rw-r--   0 root         (0) root         (0)     1246 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/cc_jwt_config.cc
+-rw-rw-r--   0 root         (0) root         (0)      997 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/cc_jwt_config.h
+-rw-rw-r--   0 root         (0) root         (0)     3745 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/cc_key_manager.cc
+-rw-rw-r--   0 root         (0) root         (0)     1002 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/cc_key_manager.h
+-rw-rw-r--   0 root         (0) root         (0)    25593 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/cc_key_manager_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2800 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/cc_streaming_aead_wrappers.cc
+-rw-rw-r--   0 root         (0) root         (0)     1048 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/cc_streaming_aead_wrappers.h
+-rw-rw-r--   0 root         (0) root         (0)     1025 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/cc_tink_config.cc
+-rw-rw-r--   0 root         (0) root         (0)     1001 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/cc_tink_config.h
+-rw-rw-r--   0 root         (0) root         (0)      855 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/cc_tink_config_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3658 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/deterministic_aead.cc
+-rw-rw-r--   0 root         (0) root         (0)     1019 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/deterministic_aead.h
+-rw-rw-r--   0 root         (0) root         (0)     1821 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/hybrid_decrypt.cc
+-rw-rw-r--   0 root         (0) root         (0)     1003 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/hybrid_decrypt.h
+-rw-rw-r--   0 root         (0) root         (0)     1816 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/hybrid_encrypt.cc
+-rw-rw-r--   0 root         (0) root         (0)     1003 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/hybrid_encrypt.h
+-rw-rw-r--   0 root         (0) root         (0)     1141 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/import_helper.cc
+-rw-rw-r--   0 root         (0) root         (0)     1205 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/import_helper.h
+-rw-rw-r--   0 root         (0) root         (0)     2359 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/input_stream_adapter.cc
+-rw-rw-r--   0 root         (0) root         (0)     1026 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/input_stream_adapter.h
+-rw-rw-r--   0 root         (0) root         (0)     2515 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/mac.cc
+-rw-rw-r--   0 root         (0) root         (0)      960 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/mac.h
+-rw-rw-r--   0 root         (0) root         (0)     1829 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/output_stream_adapter.cc
+-rw-rw-r--   0 root         (0) root         (0)     1030 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/output_stream_adapter.h
+-rw-rw-r--   0 root         (0) root         (0)     1886 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/prf.cc
+-rw-rw-r--   0 root         (0) root         (0)      965 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/prf.h
+-rw-rw-r--   0 root         (0) root         (0)     2239 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/public_key_sign.cc
+-rw-rw-r--   0 root         (0) root         (0)     1006 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/public_key_sign.h
+-rw-rw-r--   0 root         (0) root         (0)     2329 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/public_key_verify.cc
+-rw-rw-r--   0 root         (0) root         (0)     1013 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/public_key_verify.h
+-rw-rw-r--   0 root         (0) root         (0)     4757 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/python_file_object_adapter.cc
+-rw-rw-r--   0 root         (0) root         (0)     1049 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/python_file_object_adapter.h
+-rw-rw-r--   0 root         (0) root         (0)     1882 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/streaming_aead.cc
+-rw-rw-r--   0 root         (0) root         (0)     1008 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/streaming_aead.h
+-rw-rw-r--   0 root         (0) root         (0)     2388 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/tink_bindings.cc
+-rw-rw-r--   0 root         (0) root         (0)     1425 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/pybind/tink_exception.h
+-rw-rw-r--   0 root         (0) root         (0)     1782 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/python_file_object_adapter.h
+-rw-rw-r--   0 root         (0) root         (0)     3353 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/python_input_stream.cc
+-rw-rw-r--   0 root         (0) root         (0)     2225 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/python_input_stream.h
+-rw-rw-r--   0 root         (0) root         (0)     6559 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/python_input_stream_test.cc
+-rw-rw-r--   0 root         (0) root         (0)     4123 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/python_output_stream.cc
+-rw-rw-r--   0 root         (0) root         (0)     2256 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/python_output_stream.h
+-rw-rw-r--   0 root         (0) root         (0)     7393 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/python_output_stream_test.cc
+-rw-rw-r--   0 root         (0) root         (0)    11525 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cc/test_util.h
+-rw-rw-r--   0 root         (0) root         (0)     1468 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cleartext_keyset_handle.py
+-rw-rw-r--   0 root         (0) root         (0)     2013 2023-11-27 08:35:14.000000 tink-1.9.0/tink/cleartext_keyset_handle_test.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.554233 tink-1.9.0/tink/core/
+-rw-rw-r--   0 root         (0) root         (0)     2575 2023-11-27 08:35:14.000000 tink-1.9.0/tink/core/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)     1450 2023-11-27 08:35:14.000000 tink-1.9.0/tink/core/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1494 2023-11-27 08:35:14.000000 tink-1.9.0/tink/core/_crypto_format.py
+-rw-rw-r--   0 root         (0) root         (0)     2729 2023-11-27 08:35:14.000000 tink-1.9.0/tink/core/_crypto_format_test.py
+-rw-rw-r--   0 root         (0) root         (0)     5259 2023-11-27 08:35:14.000000 tink-1.9.0/tink/core/_key_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     3734 2023-11-27 08:35:14.000000 tink-1.9.0/tink/core/_primitive_set.py
+-rw-rw-r--   0 root         (0) root         (0)     9916 2023-11-27 08:35:14.000000 tink-1.9.0/tink/core/_primitive_set_test.py
+-rw-rw-r--   0 root         (0) root         (0)     1766 2023-11-27 08:35:14.000000 tink-1.9.0/tink/core/_primitive_wrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     9078 2023-11-27 08:35:14.000000 tink-1.9.0/tink/core/_registry.py
+-rw-rw-r--   0 root         (0) root         (0)    14610 2023-11-27 08:35:14.000000 tink-1.9.0/tink/core/_registry_test.py
+-rw-rw-r--   0 root         (0) root         (0)     1302 2023-11-27 08:35:14.000000 tink-1.9.0/tink/core/_tink_error.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.558233 tink-1.9.0/tink/daead/
+-rw-rw-r--   0 root         (0) root         (0)     2311 2023-11-27 08:35:14.000000 tink-1.9.0/tink/daead/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      914 2023-11-27 08:35:14.000000 tink-1.9.0/tink/daead/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1956 2023-11-27 08:35:14.000000 tink-1.9.0/tink/daead/_deterministic_aead.py
+-rw-rw-r--   0 root         (0) root         (0)     2129 2023-11-27 08:35:14.000000 tink-1.9.0/tink/daead/_deterministic_aead_key_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     2555 2023-11-27 08:35:14.000000 tink-1.9.0/tink/daead/_deterministic_aead_key_manager_test.py
+-rw-rw-r--   0 root         (0) root         (0)     1788 2023-11-27 08:35:14.000000 tink-1.9.0/tink/daead/_deterministic_aead_key_templates.py
+-rw-rw-r--   0 root         (0) root         (0)     1624 2023-11-27 08:35:14.000000 tink-1.9.0/tink/daead/_deterministic_aead_key_templates_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3280 2023-11-27 08:35:14.000000 tink-1.9.0/tink/daead/_deterministic_aead_wrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     5917 2023-11-27 08:35:14.000000 tink-1.9.0/tink/daead/_deterministic_aead_wrapper_test.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.558233 tink-1.9.0/tink/hybrid/
+-rw-rw-r--   0 root         (0) root         (0)     2672 2023-11-27 08:35:14.000000 tink-1.9.0/tink/hybrid/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      927 2023-11-27 08:35:14.000000 tink-1.9.0/tink/hybrid/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2470 2023-11-27 08:35:14.000000 tink-1.9.0/tink/hybrid/_hybrid_decrypt.py
+-rw-rw-r--   0 root         (0) root         (0)     2477 2023-11-27 08:35:14.000000 tink-1.9.0/tink/hybrid/_hybrid_encrypt.py
+-rw-rw-r--   0 root         (0) root         (0)     3669 2023-11-27 08:35:14.000000 tink-1.9.0/tink/hybrid/_hybrid_key_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     8262 2023-11-27 08:35:14.000000 tink-1.9.0/tink/hybrid/_hybrid_key_manager_test.py
+-rw-rw-r--   0 root         (0) root         (0)     5853 2023-11-27 08:35:14.000000 tink-1.9.0/tink/hybrid/_hybrid_key_templates.py
+-rw-rw-r--   0 root         (0) root         (0)     3060 2023-11-27 08:35:14.000000 tink-1.9.0/tink/hybrid/_hybrid_key_templates_test.py
+-rw-rw-r--   0 root         (0) root         (0)     4026 2023-11-27 08:35:14.000000 tink-1.9.0/tink/hybrid/_hybrid_wrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     9832 2023-11-27 08:35:14.000000 tink-1.9.0/tink/hybrid/_hybrid_wrapper_test.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.562233 tink-1.9.0/tink/integration/
+-rw-rw-r--   0 root         (0) root         (0)      575 2023-11-27 08:35:14.000000 tink-1.9.0/tink/integration/__init__.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.562233 tink-1.9.0/tink/integration/awskms/
+-rw-rw-r--   0 root         (0) root         (0)     1490 2023-11-27 08:35:14.000000 tink-1.9.0/tink/integration/awskms/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      986 2023-11-27 08:35:14.000000 tink-1.9.0/tink/integration/awskms/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7871 2023-11-27 08:35:14.000000 tink-1.9.0/tink/integration/awskms/_aws_kms_client.py
+-rw-rw-r--   0 root         (0) root         (0)     8353 2023-11-27 08:35:14.000000 tink-1.9.0/tink/integration/awskms/_aws_kms_client_test.py
+-rw-rw-r--   0 root         (0) root         (0)    10117 2023-11-27 08:35:14.000000 tink-1.9.0/tink/integration/awskms/_aws_kms_integration_test.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.562233 tink-1.9.0/tink/integration/gcpkms/
+-rw-rw-r--   0 root         (0) root         (0)     1785 2023-11-27 08:35:14.000000 tink-1.9.0/tink/integration/gcpkms/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      943 2023-11-27 08:35:14.000000 tink-1.9.0/tink/integration/gcpkms/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4918 2023-11-27 08:35:14.000000 tink-1.9.0/tink/integration/gcpkms/_gcp_kms_client.py
+-rw-rw-r--   0 root         (0) root         (0)     5805 2023-11-27 08:35:14.000000 tink-1.9.0/tink/integration/gcpkms/_gcp_kms_client_integration_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2345 2023-11-27 08:35:14.000000 tink-1.9.0/tink/integration/gcpkms/_gcp_kms_client_test.py
+-rw-rw-r--   0 root         (0) root         (0)     9721 2023-11-27 08:35:14.000000 tink-1.9.0/tink/integration/gcpkms/_gcp_kms_integration_test.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.566234 tink-1.9.0/tink/internal/
+-rw-rw-r--   0 root         (0) root         (0)      504 2023-11-27 08:35:14.000000 tink-1.9.0/tink/internal/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      575 2023-11-27 08:35:14.000000 tink-1.9.0/tink/internal/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      918 2023-11-27 08:35:14.000000 tink-1.9.0/tink/internal/big_integer_util.py
+-rw-rw-r--   0 root         (0) root         (0)     1578 2023-11-27 08:35:14.000000 tink-1.9.0/tink/internal/big_integer_util_test.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.574234 tink-1.9.0/tink/jwt/
+-rw-rw-r--   0 root         (0) root         (0)     7932 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)     4228 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2124 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_json_util.py
+-rw-rw-r--   0 root         (0) root         (0)     2001 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_json_util_test.py
+-rw-rw-r--   0 root         (0) root         (0)    12921 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_jwk_set_converter.py
+-rw-rw-r--   0 root         (0) root         (0)    37806 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_jwk_set_converter_test.py
+-rw-rw-r--   0 root         (0) root         (0)      682 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_jwt_error.py
+-rw-rw-r--   0 root         (0) root         (0)     7133 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_jwt_format.py
+-rw-rw-r--   0 root         (0) root         (0)    17449 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_jwt_format_test.py
+-rw-rw-r--   0 root         (0) root         (0)     5063 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_jwt_hmac_key_manager.py
+-rw-rw-r--   0 root         (0) root         (0)    12970 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_jwt_hmac_key_manager_test.py
+-rw-rw-r--   0 root         (0) root         (0)     7622 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_jwt_key_templates.py
+-rw-rw-r--   0 root         (0) root         (0)     3975 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_jwt_key_templates_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3153 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_jwt_mac.py
+-rw-rw-r--   0 root         (0) root         (0)     3344 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_jwt_mac_wrapper.py
+-rw-rw-r--   0 root         (0) root         (0)    10684 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_jwt_mac_wrapper_test.py
+-rw-rw-r--   0 root         (0) root         (0)     1674 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_jwt_public_key_sign.py
+-rw-rw-r--   0 root         (0) root         (0)     2546 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_jwt_public_key_verify.py
+-rw-rw-r--   0 root         (0) root         (0)    13109 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_jwt_signature_key_manager.py
+-rw-rw-r--   0 root         (0) root         (0)    11632 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_jwt_signature_key_manager_test.py
+-rw-rw-r--   0 root         (0) root         (0)     4077 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_jwt_signature_wrappers.py
+-rw-rw-r--   0 root         (0) root         (0)    13519 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_jwt_signature_wrappers_test.py
+-rw-rw-r--   0 root         (0) root         (0)     8308 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_jwt_validator.py
+-rw-rw-r--   0 root         (0) root         (0)    14891 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_jwt_validator_test.py
+-rw-rw-r--   0 root         (0) root         (0)     9358 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_raw_jwt.py
+-rw-rw-r--   0 root         (0) root         (0)    16306 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_raw_jwt_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2910 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_verified_jwt.py
+-rw-rw-r--   0 root         (0) root         (0)     4149 2023-11-27 08:35:14.000000 tink-1.9.0/tink/jwt/_verified_jwt_test.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.574234 tink-1.9.0/tink/mac/
+-rw-rw-r--   0 root         (0) root         (0)     2184 2023-11-27 08:35:14.000000 tink-1.9.0/tink/mac/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      774 2023-11-27 08:35:14.000000 tink-1.9.0/tink/mac/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1698 2023-11-27 08:35:14.000000 tink-1.9.0/tink/mac/_mac.py
+-rw-rw-r--   0 root         (0) root         (0)     1665 2023-11-27 08:35:14.000000 tink-1.9.0/tink/mac/_mac_key_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     2921 2023-11-27 08:35:14.000000 tink-1.9.0/tink/mac/_mac_key_manager_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3369 2023-11-27 08:35:14.000000 tink-1.9.0/tink/mac/_mac_key_templates.py
+-rw-rw-r--   0 root         (0) root         (0)     2048 2023-11-27 08:35:14.000000 tink-1.9.0/tink/mac/_mac_key_templates_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3263 2023-11-27 08:35:14.000000 tink-1.9.0/tink/mac/_mac_wrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     5000 2023-11-27 08:35:14.000000 tink-1.9.0/tink/mac/_mac_wrapper_test.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.578235 tink-1.9.0/tink/prf/
+-rw-rw-r--   0 root         (0) root         (0)     1961 2023-11-27 08:35:14.000000 tink-1.9.0/tink/prf/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      809 2023-11-27 08:35:14.000000 tink-1.9.0/tink/prf/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1720 2023-11-27 08:35:14.000000 tink-1.9.0/tink/prf/_prf_key_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     3336 2023-11-27 08:35:14.000000 tink-1.9.0/tink/prf/_prf_key_manager_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3087 2023-11-27 08:35:14.000000 tink-1.9.0/tink/prf/_prf_key_templates.py
+-rw-rw-r--   0 root         (0) root         (0)     3127 2023-11-27 08:35:14.000000 tink-1.9.0/tink/prf/_prf_set.py
+-rw-rw-r--   0 root         (0) root         (0)     1838 2023-11-27 08:35:14.000000 tink-1.9.0/tink/prf/_prf_set_wrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     2749 2023-11-27 08:35:14.000000 tink-1.9.0/tink/prf/_prf_set_wrapper_test.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.598236 tink-1.9.0/tink/proto/
+-rw-rw-r--   0 root         (0) root         (0)     5468 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      575 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1176 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/aes_cmac.proto
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/aes_cmac_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1104 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/aes_cmac_prf.proto
+-rw-r--r--   0 root         (0) root         (0)     1610 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/aes_cmac_prf_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1168 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/aes_ctr.proto
+-rw-rw-r--   0 root         (0) root         (0)     1254 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/aes_ctr_hmac_aead.proto
+-rw-r--r--   0 root         (0) root         (0)     2096 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/aes_ctr_hmac_aead_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1697 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/aes_ctr_hmac_streaming.proto
+-rw-r--r--   0 root         (0) root         (0)     2538 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/aes_ctr_hmac_streaming_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/aes_ctr_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1247 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/aes_eax.proto
+-rw-r--r--   0 root         (0) root         (0)     1840 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/aes_eax_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     2589 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/aes_gcm.proto
+-rw-rw-r--   0 root         (0) root         (0)     1599 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/aes_gcm_hkdf_streaming.proto
+-rw-r--r--   0 root         (0) root         (0)     2363 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/aes_gcm_hkdf_streaming_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/aes_gcm_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1194 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/aes_gcm_siv.proto
+-rw-r--r--   0 root         (0) root         (0)     1610 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/aes_gcm_siv_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1570 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/aes_siv.proto
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/aes_siv_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1202 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/chacha20_poly1305.proto
+-rw-r--r--   0 root         (0) root         (0)     1601 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/chacha20_poly1305_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1513 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/common.proto
+-rw-r--r--   0 root         (0) root         (0)     1988 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/common_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1977 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/config.proto
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/config_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     2554 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/ecdsa.proto
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/ecdsa_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     3571 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/ecies_aead_hkdf.proto
+-rw-r--r--   0 root         (0) root         (0)     3279 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/ecies_aead_hkdf_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1753 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/ed25519.proto
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/ed25519_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)      900 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/empty.proto
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/empty_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1390 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/hkdf_prf.proto
+-rw-r--r--   0 root         (0) root         (0)     2036 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/hkdf_prf_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1257 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/hmac.proto
+-rw-r--r--   0 root         (0) root         (0)     1991 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/hmac_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1255 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/hmac_prf.proto
+-rw-r--r--   0 root         (0) root         (0)     2006 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/hmac_prf_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1894 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/hpke.proto
+-rw-r--r--   0 root         (0) root         (0)     3069 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/hpke_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1997 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/jwt_ecdsa.proto
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/jwt_ecdsa_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1576 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/jwt_hmac.proto
+-rw-r--r--   0 root         (0) root         (0)     2221 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/jwt_hmac_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     2735 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/jwt_rsa_ssa_pkcs1.proto
+-rw-r--r--   0 root         (0) root         (0)     2969 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/jwt_rsa_ssa_pkcs1_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     2768 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/jwt_rsa_ssa_pss.proto
+-rw-r--r--   0 root         (0) root         (0)     2930 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/jwt_rsa_ssa_pss_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1388 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/kms_aead.proto
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/kms_aead_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1587 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/kms_envelope.proto
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/kms_envelope_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1295 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/prf_based_deriver.proto
+-rw-r--r--   0 root         (0) root         (0)     2219 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/prf_based_deriver_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     2778 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/rsa_ssa_pkcs1.proto
+-rw-r--r--   0 root         (0) root         (0)     2634 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/rsa_ssa_pkcs1_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     3092 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/rsa_ssa_pss.proto
+-rw-r--r--   0 root         (0) root         (0)     2717 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/rsa_ssa_pss_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1068 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/test_proto.proto
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/test_proto_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     7229 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/tink.proto
+-rw-r--r--   0 root         (0) root         (0)     4252 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/tink_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1109 2023-11-27 08:35:14.000000 tink-1.9.0/tink/proto/xchacha20_poly1305.proto
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-11-27 08:36:14.000000 tink-1.9.0/tink/proto/xchacha20_poly1305_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)      882 2023-11-27 08:35:14.000000 tink-1.9.0/tink/secret_key_access.py
+-rw-rw-r--   0 root         (0) root         (0)     1268 2023-11-27 08:35:14.000000 tink-1.9.0/tink/secret_key_access_test.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.598236 tink-1.9.0/tink/signature/
+-rw-rw-r--   0 root         (0) root         (0)     2306 2023-11-27 08:35:14.000000 tink-1.9.0/tink/signature/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      966 2023-11-27 08:35:14.000000 tink-1.9.0/tink/signature/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1380 2023-11-27 08:35:14.000000 tink-1.9.0/tink/signature/_public_key_sign.py
+-rw-rw-r--   0 root         (0) root         (0)     1507 2023-11-27 08:35:14.000000 tink-1.9.0/tink/signature/_public_key_verify.py
+-rw-rw-r--   0 root         (0) root         (0)     2887 2023-11-27 08:35:14.000000 tink-1.9.0/tink/signature/_signature_key_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     4901 2023-11-27 08:35:14.000000 tink-1.9.0/tink/signature/_signature_key_manager_test.py
+-rw-rw-r--   0 root         (0) root         (0)     7852 2023-11-27 08:35:14.000000 tink-1.9.0/tink/signature/_signature_key_templates.py
+-rw-rw-r--   0 root         (0) root         (0)     5142 2023-11-27 08:35:14.000000 tink-1.9.0/tink/signature/_signature_wrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     5885 2023-11-27 08:35:14.000000 tink-1.9.0/tink/signature/_signature_wrapper_test.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.606237 tink-1.9.0/tink/streaming_aead/
+-rw-rw-r--   0 root         (0) root         (0)     5475 2023-11-27 08:35:14.000000 tink-1.9.0/tink/streaming_aead/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      904 2023-11-27 08:35:14.000000 tink-1.9.0/tink/streaming_aead/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4794 2023-11-27 08:35:14.000000 tink-1.9.0/tink/streaming_aead/_decrypting_stream.py
+-rw-rw-r--   0 root         (0) root         (0)     2896 2023-11-27 08:35:14.000000 tink-1.9.0/tink/streaming_aead/_decrypting_stream_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3874 2023-11-27 08:35:14.000000 tink-1.9.0/tink/streaming_aead/_encrypting_stream.py
+-rw-rw-r--   0 root         (0) root         (0)     3778 2023-11-27 08:35:14.000000 tink-1.9.0/tink/streaming_aead/_encrypting_stream_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2165 2023-11-27 08:35:14.000000 tink-1.9.0/tink/streaming_aead/_file_object_adapter.py
+-rw-rw-r--   0 root         (0) root         (0)     4079 2023-11-27 08:35:14.000000 tink-1.9.0/tink/streaming_aead/_file_object_adapter_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3176 2023-11-27 08:35:14.000000 tink-1.9.0/tink/streaming_aead/_pybind11_python_file_object_adapter_test.py
+-rw-rw-r--   0 root         (0) root         (0)     4756 2023-11-27 08:35:14.000000 tink-1.9.0/tink/streaming_aead/_raw_streaming_aead.py
+-rw-rw-r--   0 root         (0) root         (0)     3109 2023-11-27 08:35:14.000000 tink-1.9.0/tink/streaming_aead/_rewindable_input_stream.py
+-rw-rw-r--   0 root         (0) root         (0)     6303 2023-11-27 08:35:14.000000 tink-1.9.0/tink/streaming_aead/_rewindable_input_stream_test.py
+-rw-rw-r--   0 root         (0) root         (0)     4520 2023-11-27 08:35:14.000000 tink-1.9.0/tink/streaming_aead/_streaming_aead.py
+-rw-rw-r--   0 root         (0) root         (0)     2894 2023-11-27 08:35:14.000000 tink-1.9.0/tink/streaming_aead/_streaming_aead_key_manager.py
+-rw-rw-r--   0 root         (0) root         (0)    10488 2023-11-27 08:35:14.000000 tink-1.9.0/tink/streaming_aead/_streaming_aead_key_manager_test.py
+-rw-rw-r--   0 root         (0) root         (0)     6540 2023-11-27 08:35:14.000000 tink-1.9.0/tink/streaming_aead/_streaming_aead_key_templates.py
+-rw-rw-r--   0 root         (0) root         (0)     3569 2023-11-27 08:35:14.000000 tink-1.9.0/tink/streaming_aead/_streaming_aead_key_templates_test.py
+-rw-rw-r--   0 root         (0) root         (0)     4470 2023-11-27 08:35:14.000000 tink-1.9.0/tink/streaming_aead/_streaming_aead_test.py
+-rw-rw-r--   0 root         (0) root         (0)     6692 2023-11-27 08:35:14.000000 tink-1.9.0/tink/streaming_aead/_streaming_aead_wrapper.py
+-rw-rw-r--   0 root         (0) root         (0)    12108 2023-11-27 08:35:14.000000 tink-1.9.0/tink/streaming_aead/_streaming_aead_wrapper_test.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.606237 tink-1.9.0/tink/testing/
+-rw-rw-r--   0 root         (0) root         (0)     2130 2023-11-27 08:35:14.000000 tink-1.9.0/tink/testing/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      575 2023-11-27 08:35:14.000000 tink-1.9.0/tink/testing/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3537 2023-11-27 08:35:14.000000 tink-1.9.0/tink/testing/bytes_io.py
+-rw-rw-r--   0 root         (0) root         (0)     5461 2023-11-27 08:35:14.000000 tink-1.9.0/tink/testing/bytes_io_test.py
+-rw-rw-r--   0 root         (0) root         (0)     1831 2023-11-27 08:35:14.000000 tink-1.9.0/tink/testing/fake_kms.py
+-rw-rw-r--   0 root         (0) root         (0)     2242 2023-11-27 08:35:14.000000 tink-1.9.0/tink/testing/fake_kms_test.py
+-rw-rw-r--   0 root         (0) root         (0)     6601 2023-11-27 08:35:14.000000 tink-1.9.0/tink/testing/helper.py
+-rw-rw-r--   0 root         (0) root         (0)     5409 2023-11-27 08:35:14.000000 tink-1.9.0/tink/testing/helper_test.py
+-rw-rw-r--   0 root         (0) root         (0)     4324 2023-11-27 08:35:14.000000 tink-1.9.0/tink/testing/keyset_builder.py
+-rw-rw-r--   0 root         (0) root         (0)     7016 2023-11-27 08:35:14.000000 tink-1.9.0/tink/testing/keyset_builder_test.py
+-rw-rw-r--   0 root         (0) root         (0)      965 2023-11-27 08:35:14.000000 tink-1.9.0/tink/tink_config.py
+-rw-rw-r--   0 root         (0) root         (0)     4207 2023-11-27 08:35:14.000000 tink-1.9.0/tink/tink_config_test.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.530231 tink-1.9.0/tink.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7065 2023-11-27 08:36:14.000000 tink-1.9.0/tink.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10285 2023-11-27 08:36:14.000000 tink-1.9.0/tink.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-11-27 08:36:14.000000 tink-1.9.0/tink.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-11-27 08:36:14.000000 tink-1.9.0/tink.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      284 2023-11-27 08:36:14.000000 tink-1.9.0/tink.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-11-27 08:36:14.000000 tink-1.9.0/tink.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     2925 2023-11-27 08:35:14.000000 tink-1.9.0/tink_py_deps.bzl
+-rw-rw-r--   0 root         (0) root         (0)      969 2023-11-27 08:35:14.000000 tink-1.9.0/tink_py_deps_init.bzl
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.606237 tink-1.9.0/tools/
+-rw-rw-r--   0 root         (0) root         (0)       76 2023-11-27 08:35:14.000000 tink-1.9.0/tools/BUILD.bazel
+drwxr-sr-x   0 root         (0) root         (0)        0 2023-11-27 08:36:14.610237 tink-1.9.0/tools/distribution/
+-rwxrwxr-x   0 root         (0) root         (0)     3847 2023-11-27 08:35:14.000000 tink-1.9.0/tools/distribution/build_linux_binary_wheels.sh
+-rwxrwxr-x   0 root         (0) root         (0)     8658 2023-11-27 08:35:14.000000 tink-1.9.0/tools/distribution/create_bdist.sh
+-rwxrwxr-x   0 root         (0) root         (0)     2918 2023-11-27 08:35:14.000000 tink-1.9.0/tools/distribution/create_sdist.sh
+-rw-rw-r--   0 root         (0) root         (0)       30 2023-11-27 08:35:14.000000 tink-1.9.0/tools/distribution/requirements.in
+-rw-rw-r--   0 root         (0) root         (0)     1661 2023-11-27 08:35:14.000000 tink-1.9.0/tools/distribution/requirements.txt
+-rwxrwxr-x   0 root         (0) root         (0)     3339 2023-11-27 08:35:14.000000 tink-1.9.0/tools/distribution/test_dist.sh
+-rwxrwxr-x   0 root         (0) root         (0)     2825 2023-11-27 08:35:14.000000 tink-1.9.0/tools/distribution/test_linux_binary_wheel.sh
```

### Comparing `tink-1.8.0/LICENSE` & `tink-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/PKG-INFO` & `tink-1.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: tink
-Version: 1.8.0
-Summary: A multi-language, cross-platform library that provides cryptographic APIs that are secure, easy to use correctly, and hard(er) to misuse.
-Home-page: https://github.com/tink-crypto/tink-py
-Author: Tink Developers
-Author-email: tink-users@googlegroups.com
-License: Apache 2.0
-Keywords: tink cryptography
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Tink Python
 
 <!-- GCP Ubuntu --->
 
 [tink_py_bazel_badge_gcp_ubuntu]: https://storage.googleapis.com/tink-kokoro-build-badges/tink-py-bazel-gcp-ubuntu.svg
 [tink_py_bazel_kms_badge_gcp_ubuntu]: https://storage.googleapis.com/tink-kokoro-build-badges/tink-py-bazel-kms-gcp-ubuntu.svg
 [tink_py_pip_badge_gcp_ubuntu]: https://storage.googleapis.com/tink-kokoro-build-badges/tink-py-pip-gcp-ubuntu.svg
```

### Comparing `tink-1.8.0/requirements.txt` & `tink-1.9.0/requirements_all.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,193 +1,217 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --generate-hashes --output-file=requirements.txt requirements.in
+#    pip-compile --extra=all --generate-hashes --output-file=requirements_all.txt setup.py
 #
-absl-py==1.4.0 \
-    --hash=sha256:0d3fe606adfa4f7db64792dd4c7aee4ee0c38ab75dfd353b7a83ed3e957fcb47 \
-    --hash=sha256:d2c244d01048ba476e7c080bd2c6df5e141d211de80223460d5b3b8a2a58433d
-    # via -r requirements.in
-boto3==1.28.25 \
-    --hash=sha256:20feedb753e87d6dd55665e2e9dda08b031518291350c9c57b552c86a537fd4e \
-    --hash=sha256:f08f6c83608721c2142abd2ccc5f15bd5c98c282ad9e0d39f9efc59d98604658
-    # via -r requirements.in
-botocore==1.31.25 \
-    --hash=sha256:17cc6db84644251a5b519aeccd5eb1c313a18ef2e92616ec16182aa30c877152 \
-    --hash=sha256:b8a40b0ca1e3c8290a4c0d473c8e1575d2e8b2ddc3c61dd8814c3976357cac84
+absl-py==2.0.0 \
+    --hash=sha256:9a28abb62774ae4e8edbe2dd4c49ffcd45a6a848952a5eccc6a49f3f0fc1e2f3 \
+    --hash=sha256:d9690211c5fcfefcdd1a45470ac2b5c5acd45241c3af71eed96bc5441746c0d5
+    # via tink (setup.py)
+boto3==1.28.82 \
+    --hash=sha256:ae1352d0193aaf90c47d6e57ab054b0b1fabf0fbbe9f51eefec431bf2c3e18f4 \
+    --hash=sha256:bb8ecd6f86289ceaed566eefc0ce8ac66a85e5954aef115ed4ac602cbe61f101
+    # via tink (setup.py)
+botocore==1.31.82 \
+    --hash=sha256:5f213229348433d0b7b6aac2d9ae2fdd15c4ff9f38c30ea072f5b300bf6c1dcb \
+    --hash=sha256:9d7d8de1789b1ed37b86a2b0a4fcff9fac91deef0548461d411e1626f68ca70c
     # via
     #   boto3
     #   s3transfer
-cachetools==5.3.1 \
-    --hash=sha256:95ef631eeaea14ba2e36f06437f36463aac3a096799e876ee55e5cdccb102590 \
-    --hash=sha256:dce83f2d9b4e1f732a8cd44af8e8fab2dbe46201467fc98b3ef8f269092bf62b
+cachetools==5.3.2 \
+    --hash=sha256:086ee420196f7b2ab9ca2db2520aca326318b68fe5ba8bc4d49cca91add450f2 \
+    --hash=sha256:861f35a13a451f94e301ce2bec7cac63e881232ccce7ed67fab9b5df4d3beaa1
     # via google-auth
 certifi==2023.7.22 \
     --hash=sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082 \
     --hash=sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9
     # via requests
-charset-normalizer==3.2.0 \
-    --hash=sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96 \
-    --hash=sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c \
-    --hash=sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710 \
-    --hash=sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706 \
-    --hash=sha256:1249cbbf3d3b04902ff081ffbb33ce3377fa6e4c7356f759f3cd076cc138d020 \
-    --hash=sha256:1920d4ff15ce893210c1f0c0e9d19bfbecb7983c76b33f046c13a8ffbd570252 \
-    --hash=sha256:193cbc708ea3aca45e7221ae58f0fd63f933753a9bfb498a3b474878f12caaad \
-    --hash=sha256:1a100c6d595a7f316f1b6f01d20815d916e75ff98c27a01ae817439ea7726329 \
-    --hash=sha256:1f30b48dd7fa1474554b0b0f3fdfdd4c13b5c737a3c6284d3cdc424ec0ffff3a \
-    --hash=sha256:203f0c8871d5a7987be20c72442488a0b8cfd0f43b7973771640fc593f56321f \
-    --hash=sha256:246de67b99b6851627d945db38147d1b209a899311b1305dd84916f2b88526c6 \
-    --hash=sha256:2dee8e57f052ef5353cf608e0b4c871aee320dd1b87d351c28764fc0ca55f9f4 \
-    --hash=sha256:2efb1bd13885392adfda4614c33d3b68dee4921fd0ac1d3988f8cbb7d589e72a \
-    --hash=sha256:2f4ac36d8e2b4cc1aa71df3dd84ff8efbe3bfb97ac41242fbcfc053c67434f46 \
-    --hash=sha256:3170c9399da12c9dc66366e9d14da8bf7147e1e9d9ea566067bbce7bb74bd9c2 \
-    --hash=sha256:3b1613dd5aee995ec6d4c69f00378bbd07614702a315a2cf6c1d21461fe17c23 \
-    --hash=sha256:3bb3d25a8e6c0aedd251753a79ae98a093c7e7b471faa3aa9a93a81431987ace \
-    --hash=sha256:3bb7fda7260735efe66d5107fb7e6af6a7c04c7fce9b2514e04b7a74b06bf5dd \
-    --hash=sha256:41b25eaa7d15909cf3ac4c96088c1f266a9a93ec44f87f1d13d4a0e86c81b982 \
-    --hash=sha256:45de3f87179c1823e6d9e32156fb14c1927fcc9aba21433f088fdfb555b77c10 \
-    --hash=sha256:46fb8c61d794b78ec7134a715a3e564aafc8f6b5e338417cb19fe9f57a5a9bf2 \
-    --hash=sha256:48021783bdf96e3d6de03a6e39a1171ed5bd7e8bb93fc84cc649d11490f87cea \
-    --hash=sha256:4957669ef390f0e6719db3613ab3a7631e68424604a7b448f079bee145da6e09 \
-    --hash=sha256:5e86d77b090dbddbe78867a0275cb4df08ea195e660f1f7f13435a4649e954e5 \
-    --hash=sha256:6339d047dab2780cc6220f46306628e04d9750f02f983ddb37439ca47ced7149 \
-    --hash=sha256:681eb3d7e02e3c3655d1b16059fbfb605ac464c834a0c629048a30fad2b27489 \
-    --hash=sha256:6c409c0deba34f147f77efaa67b8e4bb83d2f11c8806405f76397ae5b8c0d1c9 \
-    --hash=sha256:7095f6fbfaa55defb6b733cfeb14efaae7a29f0b59d8cf213be4e7ca0b857b80 \
-    --hash=sha256:70c610f6cbe4b9fce272c407dd9d07e33e6bf7b4aa1b7ffb6f6ded8e634e3592 \
-    --hash=sha256:72814c01533f51d68702802d74f77ea026b5ec52793c791e2da806a3844a46c3 \
-    --hash=sha256:7a4826ad2bd6b07ca615c74ab91f32f6c96d08f6fcc3902ceeedaec8cdc3bcd6 \
-    --hash=sha256:7c70087bfee18a42b4040bb9ec1ca15a08242cf5867c58726530bdf3945672ed \
-    --hash=sha256:855eafa5d5a2034b4621c74925d89c5efef61418570e5ef9b37717d9c796419c \
-    --hash=sha256:8700f06d0ce6f128de3ccdbc1acaea1ee264d2caa9ca05daaf492fde7c2a7200 \
-    --hash=sha256:89f1b185a01fe560bc8ae5f619e924407efca2191b56ce749ec84982fc59a32a \
-    --hash=sha256:8b2c760cfc7042b27ebdb4a43a4453bd829a5742503599144d54a032c5dc7e9e \
-    --hash=sha256:8c2f5e83493748286002f9369f3e6607c565a6a90425a3a1fef5ae32a36d749d \
-    --hash=sha256:8e098148dd37b4ce3baca71fb394c81dc5d9c7728c95df695d2dca218edf40e6 \
-    --hash=sha256:94aea8eff76ee6d1cdacb07dd2123a68283cb5569e0250feab1240058f53b623 \
-    --hash=sha256:95eb302ff792e12aba9a8b8f8474ab229a83c103d74a750ec0bd1c1eea32e669 \
-    --hash=sha256:9bd9b3b31adcb054116447ea22caa61a285d92e94d710aa5ec97992ff5eb7cf3 \
-    --hash=sha256:9e608aafdb55eb9f255034709e20d5a83b6d60c054df0802fa9c9883d0a937aa \
-    --hash=sha256:a103b3a7069b62f5d4890ae1b8f0597618f628b286b03d4bc9195230b154bfa9 \
-    --hash=sha256:a386ebe437176aab38c041de1260cd3ea459c6ce5263594399880bbc398225b2 \
-    --hash=sha256:a38856a971c602f98472050165cea2cdc97709240373041b69030be15047691f \
-    --hash=sha256:a401b4598e5d3f4a9a811f3daf42ee2291790c7f9d74b18d75d6e21dda98a1a1 \
-    --hash=sha256:a7647ebdfb9682b7bb97e2a5e7cb6ae735b1c25008a70b906aecca294ee96cf4 \
-    --hash=sha256:aaf63899c94de41fe3cf934601b0f7ccb6b428c6e4eeb80da72c58eab077b19a \
-    --hash=sha256:b0dac0ff919ba34d4df1b6131f59ce95b08b9065233446be7e459f95554c0dc8 \
-    --hash=sha256:baacc6aee0b2ef6f3d308e197b5d7a81c0e70b06beae1f1fcacffdbd124fe0e3 \
-    --hash=sha256:bf420121d4c8dce6b889f0e8e4ec0ca34b7f40186203f06a946fa0276ba54029 \
-    --hash=sha256:c04a46716adde8d927adb9457bbe39cf473e1e2c2f5d0a16ceb837e5d841ad4f \
-    --hash=sha256:c0b21078a4b56965e2b12f247467b234734491897e99c1d51cee628da9786959 \
-    --hash=sha256:c1c76a1743432b4b60ab3358c937a3fe1341c828ae6194108a94c69028247f22 \
-    --hash=sha256:c4983bf937209c57240cff65906b18bb35e64ae872da6a0db937d7b4af845dd7 \
-    --hash=sha256:c4fb39a81950ec280984b3a44f5bd12819953dc5fa3a7e6fa7a80db5ee853952 \
-    --hash=sha256:c57921cda3a80d0f2b8aec7e25c8aa14479ea92b5b51b6876d975d925a2ea346 \
-    --hash=sha256:c8063cf17b19661471ecbdb3df1c84f24ad2e389e326ccaf89e3fb2484d8dd7e \
-    --hash=sha256:ccd16eb18a849fd8dcb23e23380e2f0a354e8daa0c984b8a732d9cfaba3a776d \
-    --hash=sha256:cd6dbe0238f7743d0efe563ab46294f54f9bc8f4b9bcf57c3c666cc5bc9d1299 \
-    --hash=sha256:d62e51710986674142526ab9f78663ca2b0726066ae26b78b22e0f5e571238dd \
-    --hash=sha256:db901e2ac34c931d73054d9797383d0f8009991e723dab15109740a63e7f902a \
-    --hash=sha256:e03b8895a6990c9ab2cdcd0f2fe44088ca1c65ae592b8f795c3294af00a461c3 \
-    --hash=sha256:e1c8a2f4c69e08e89632defbfabec2feb8a8d99edc9f89ce33c4b9e36ab63037 \
-    --hash=sha256:e4b749b9cc6ee664a3300bb3a273c1ca8068c46be705b6c31cf5d276f8628a94 \
-    --hash=sha256:e6a5bf2cba5ae1bb80b154ed68a3cfa2fa00fde979a7f50d6598d3e17d9ac20c \
-    --hash=sha256:e857a2232ba53ae940d3456f7533ce6ca98b81917d47adc3c7fd55dad8fab858 \
-    --hash=sha256:ee4006268ed33370957f55bf2e6f4d263eaf4dc3cfc473d1d90baff6ed36ce4a \
-    --hash=sha256:eef9df1eefada2c09a5e7a40991b9fc6ac6ef20b1372abd48d2794a316dc0449 \
-    --hash=sha256:f058f6963fd82eb143c692cecdc89e075fa0828db2e5b291070485390b2f1c9c \
-    --hash=sha256:f25c229a6ba38a35ae6e25ca1264621cc25d4d38dca2942a7fce0b67a4efe918 \
-    --hash=sha256:f2a1d0fd4242bd8643ce6f98927cf9c04540af6efa92323e9d3124f57727bfc1 \
-    --hash=sha256:f7560358a6811e52e9c4d142d497f1a6e10103d3a6881f18d04dbce3729c0e2c \
-    --hash=sha256:f779d3ad205f108d14e99bb3859aa7dd8e9c68874617c72354d7ecaec2a054ac \
-    --hash=sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa
+charset-normalizer==3.3.2 \
+    --hash=sha256:06435b539f889b1f6f4ac1758871aae42dc3a8c0e24ac9e60c2384973ad73027 \
+    --hash=sha256:06a81e93cd441c56a9b65d8e1d043daeb97a3d0856d177d5c90ba85acb3db087 \
+    --hash=sha256:0a55554a2fa0d408816b3b5cedf0045f4b8e1a6065aec45849de2d6f3f8e9786 \
+    --hash=sha256:0b2b64d2bb6d3fb9112bafa732def486049e63de9618b5843bcdd081d8144cd8 \
+    --hash=sha256:10955842570876604d404661fbccbc9c7e684caf432c09c715ec38fbae45ae09 \
+    --hash=sha256:122c7fa62b130ed55f8f285bfd56d5f4b4a5b503609d181f9ad85e55c89f4185 \
+    --hash=sha256:1ceae2f17a9c33cb48e3263960dc5fc8005351ee19db217e9b1bb15d28c02574 \
+    --hash=sha256:1d3193f4a680c64b4b6a9115943538edb896edc190f0b222e73761716519268e \
+    --hash=sha256:1f79682fbe303db92bc2b1136016a38a42e835d932bab5b3b1bfcfbf0640e519 \
+    --hash=sha256:2127566c664442652f024c837091890cb1942c30937add288223dc895793f898 \
+    --hash=sha256:22afcb9f253dac0696b5a4be4a1c0f8762f8239e21b99680099abd9b2b1b2269 \
+    --hash=sha256:25baf083bf6f6b341f4121c2f3c548875ee6f5339300e08be3f2b2ba1721cdd3 \
+    --hash=sha256:2e81c7b9c8979ce92ed306c249d46894776a909505d8f5a4ba55b14206e3222f \
+    --hash=sha256:3287761bc4ee9e33561a7e058c72ac0938c4f57fe49a09eae428fd88aafe7bb6 \
+    --hash=sha256:34d1c8da1e78d2e001f363791c98a272bb734000fcef47a491c1e3b0505657a8 \
+    --hash=sha256:37e55c8e51c236f95b033f6fb391d7d7970ba5fe7ff453dad675e88cf303377a \
+    --hash=sha256:3d47fa203a7bd9c5b6cee4736ee84ca03b8ef23193c0d1ca99b5089f72645c73 \
+    --hash=sha256:3e4d1f6587322d2788836a99c69062fbb091331ec940e02d12d179c1d53e25fc \
+    --hash=sha256:42cb296636fcc8b0644486d15c12376cb9fa75443e00fb25de0b8602e64c1714 \
+    --hash=sha256:45485e01ff4d3630ec0d9617310448a8702f70e9c01906b0d0118bdf9d124cf2 \
+    --hash=sha256:4a78b2b446bd7c934f5dcedc588903fb2f5eec172f3d29e52a9096a43722adfc \
+    --hash=sha256:4ab2fe47fae9e0f9dee8c04187ce5d09f48eabe611be8259444906793ab7cbce \
+    --hash=sha256:4d0d1650369165a14e14e1e47b372cfcb31d6ab44e6e33cb2d4e57265290044d \
+    --hash=sha256:549a3a73da901d5bc3ce8d24e0600d1fa85524c10287f6004fbab87672bf3e1e \
+    --hash=sha256:55086ee1064215781fff39a1af09518bc9255b50d6333f2e4c74ca09fac6a8f6 \
+    --hash=sha256:572c3763a264ba47b3cf708a44ce965d98555f618ca42c926a9c1616d8f34269 \
+    --hash=sha256:573f6eac48f4769d667c4442081b1794f52919e7edada77495aaed9236d13a96 \
+    --hash=sha256:5b4c145409bef602a690e7cfad0a15a55c13320ff7a3ad7ca59c13bb8ba4d45d \
+    --hash=sha256:6463effa3186ea09411d50efc7d85360b38d5f09b870c48e4600f63af490e56a \
+    --hash=sha256:65f6f63034100ead094b8744b3b97965785388f308a64cf8d7c34f2f2e5be0c4 \
+    --hash=sha256:663946639d296df6a2bb2aa51b60a2454ca1cb29835324c640dafb5ff2131a77 \
+    --hash=sha256:6897af51655e3691ff853668779c7bad41579facacf5fd7253b0133308cf000d \
+    --hash=sha256:68d1f8a9e9e37c1223b656399be5d6b448dea850bed7d0f87a8311f1ff3dabb0 \
+    --hash=sha256:6ac7ffc7ad6d040517be39eb591cac5ff87416c2537df6ba3cba3bae290c0fed \
+    --hash=sha256:6b3251890fff30ee142c44144871185dbe13b11bab478a88887a639655be1068 \
+    --hash=sha256:6c4caeef8fa63d06bd437cd4bdcf3ffefe6738fb1b25951440d80dc7df8c03ac \
+    --hash=sha256:6ef1d82a3af9d3eecdba2321dc1b3c238245d890843e040e41e470ffa64c3e25 \
+    --hash=sha256:753f10e867343b4511128c6ed8c82f7bec3bd026875576dfd88483c5c73b2fd8 \
+    --hash=sha256:7cd13a2e3ddeed6913a65e66e94b51d80a041145a026c27e6bb76c31a853c6ab \
+    --hash=sha256:7ed9e526742851e8d5cc9e6cf41427dfc6068d4f5a3bb03659444b4cabf6bc26 \
+    --hash=sha256:7f04c839ed0b6b98b1a7501a002144b76c18fb1c1850c8b98d458ac269e26ed2 \
+    --hash=sha256:802fe99cca7457642125a8a88a084cef28ff0cf9407060f7b93dca5aa25480db \
+    --hash=sha256:80402cd6ee291dcb72644d6eac93785fe2c8b9cb30893c1af5b8fdd753b9d40f \
+    --hash=sha256:8465322196c8b4d7ab6d1e049e4c5cb460d0394da4a27d23cc242fbf0034b6b5 \
+    --hash=sha256:86216b5cee4b06df986d214f664305142d9c76df9b6512be2738aa72a2048f99 \
+    --hash=sha256:87d1351268731db79e0f8e745d92493ee2841c974128ef629dc518b937d9194c \
+    --hash=sha256:8bdb58ff7ba23002a4c5808d608e4e6c687175724f54a5dade5fa8c67b604e4d \
+    --hash=sha256:8c622a5fe39a48f78944a87d4fb8a53ee07344641b0562c540d840748571b811 \
+    --hash=sha256:8d756e44e94489e49571086ef83b2bb8ce311e730092d2c34ca8f7d925cb20aa \
+    --hash=sha256:8f4a014bc36d3c57402e2977dada34f9c12300af536839dc38c0beab8878f38a \
+    --hash=sha256:9063e24fdb1e498ab71cb7419e24622516c4a04476b17a2dab57e8baa30d6e03 \
+    --hash=sha256:90d558489962fd4918143277a773316e56c72da56ec7aa3dc3dbbe20fdfed15b \
+    --hash=sha256:923c0c831b7cfcb071580d3f46c4baf50f174be571576556269530f4bbd79d04 \
+    --hash=sha256:95f2a5796329323b8f0512e09dbb7a1860c46a39da62ecb2324f116fa8fdc85c \
+    --hash=sha256:96b02a3dc4381e5494fad39be677abcb5e6634bf7b4fa83a6dd3112607547001 \
+    --hash=sha256:9f96df6923e21816da7e0ad3fd47dd8f94b2a5ce594e00677c0013018b813458 \
+    --hash=sha256:a10af20b82360ab00827f916a6058451b723b4e65030c5a18577c8b2de5b3389 \
+    --hash=sha256:a50aebfa173e157099939b17f18600f72f84eed3049e743b68ad15bd69b6bf99 \
+    --hash=sha256:a981a536974bbc7a512cf44ed14938cf01030a99e9b3a06dd59578882f06f985 \
+    --hash=sha256:a9a8e9031d613fd2009c182b69c7b2c1ef8239a0efb1df3f7c8da66d5dd3d537 \
+    --hash=sha256:ae5f4161f18c61806f411a13b0310bea87f987c7d2ecdbdaad0e94eb2e404238 \
+    --hash=sha256:aed38f6e4fb3f5d6bf81bfa990a07806be9d83cf7bacef998ab1a9bd660a581f \
+    --hash=sha256:b01b88d45a6fcb69667cd6d2f7a9aeb4bf53760d7fc536bf679ec94fe9f3ff3d \
+    --hash=sha256:b261ccdec7821281dade748d088bb6e9b69e6d15b30652b74cbbac25e280b796 \
+    --hash=sha256:b2b0a0c0517616b6869869f8c581d4eb2dd83a4d79e0ebcb7d373ef9956aeb0a \
+    --hash=sha256:b4a23f61ce87adf89be746c8a8974fe1c823c891d8f86eb218bb957c924bb143 \
+    --hash=sha256:bd8f7df7d12c2db9fab40bdd87a7c09b1530128315d047a086fa3ae3435cb3a8 \
+    --hash=sha256:beb58fe5cdb101e3a055192ac291b7a21e3b7ef4f67fa1d74e331a7f2124341c \
+    --hash=sha256:c002b4ffc0be611f0d9da932eb0f704fe2602a9a949d1f738e4c34c75b0863d5 \
+    --hash=sha256:c083af607d2515612056a31f0a8d9e0fcb5876b7bfc0abad3ecd275bc4ebc2d5 \
+    --hash=sha256:c180f51afb394e165eafe4ac2936a14bee3eb10debc9d9e4db8958fe36afe711 \
+    --hash=sha256:c235ebd9baae02f1b77bcea61bce332cb4331dc3617d254df3323aa01ab47bd4 \
+    --hash=sha256:cd70574b12bb8a4d2aaa0094515df2463cb429d8536cfb6c7ce983246983e5a6 \
+    --hash=sha256:d0eccceffcb53201b5bfebb52600a5fb483a20b61da9dbc885f8b103cbe7598c \
+    --hash=sha256:d965bba47ddeec8cd560687584e88cf699fd28f192ceb452d1d7ee807c5597b7 \
+    --hash=sha256:db364eca23f876da6f9e16c9da0df51aa4f104a972735574842618b8c6d999d4 \
+    --hash=sha256:ddbb2551d7e0102e7252db79ba445cdab71b26640817ab1e3e3648dad515003b \
+    --hash=sha256:deb6be0ac38ece9ba87dea880e438f25ca3eddfac8b002a2ec3d9183a454e8ae \
+    --hash=sha256:e06ed3eb3218bc64786f7db41917d4e686cc4856944f53d5bdf83a6884432e12 \
+    --hash=sha256:e27ad930a842b4c5eb8ac0016b0a54f5aebbe679340c26101df33424142c143c \
+    --hash=sha256:e537484df0d8f426ce2afb2d0f8e1c3d0b114b83f8850e5f2fbea0e797bd82ae \
+    --hash=sha256:eb00ed941194665c332bf8e078baf037d6c35d7c4f3102ea2d4f16ca94a26dc8 \
+    --hash=sha256:eb6904c354526e758fda7167b33005998fb68c46fbc10e013ca97f21ca5c8887 \
+    --hash=sha256:eb8821e09e916165e160797a6c17edda0679379a4be5c716c260e836e122f54b \
+    --hash=sha256:efcb3f6676480691518c177e3b465bcddf57cea040302f9f4e6e191af91174d4 \
+    --hash=sha256:f27273b60488abe721a075bcca6d7f3964f9f6f067c8c4c605743023d7d3944f \
+    --hash=sha256:f30c3cb33b24454a82faecaf01b19c18562b1e89558fb6c56de4d9118a032fd5 \
+    --hash=sha256:fb69256e180cb6c8a894fee62b3afebae785babc1ee98b81cdf68bbca1987f33 \
+    --hash=sha256:fd1abc0d89e30cc4e02e4064dc67fcc51bd941eb395c502aac3ec19fab46b519 \
+    --hash=sha256:ff8fa367d09b717b2a17a052544193ad76cd49979c805768879cb63d9ca50561
     # via requests
-google-api-core[grpc]==2.11.1 \
-    --hash=sha256:25d29e05a0058ed5f19c61c0a78b1b53adea4d9364b464d014fbda941f6d1c9a \
-    --hash=sha256:d92a5a92dc36dd4f4b9ee4e55528a90e432b059f93aee6ad857f9de8cc7ae94a
+google-api-core[grpc]==2.13.0 \
+    --hash=sha256:44ed591f6c3a0c1ac7a91867d2b3841f92839f860f3d3fe26c464dbd50f97094 \
+    --hash=sha256:abc1da067c9026c6cd15dfbd4f6ad07735a62eeadc541d1cc296314447fc3aad
     # via
-    #   -r requirements.in
     #   google-cloud-kms
-google-auth==2.22.0 \
-    --hash=sha256:164cba9af4e6e4e40c3a4f90a1a6c12ee56f14c0b4868d1ca91b32826ab334ce \
-    --hash=sha256:d61d1b40897407b574da67da1a833bdc10d5a11642566e506565d1b1a46ba873
+    #   tink (setup.py)
+google-auth==2.23.4 \
+    --hash=sha256:79905d6b1652187def79d491d6e23d0cbb3a21d3c7ba0dbaa9c8a01906b13ff3 \
+    --hash=sha256:d4bbc92fe4b8bfd2f3e8d88e5ba7085935da208ee38a134fc280e7ce682a05f2
     # via
-    #   -r requirements.in
     #   google-api-core
-google-cloud-kms==2.19.1 \
-    --hash=sha256:1275f2e7f08ee1106e094ec39f721af383814d94a8d123cf84bc0e9e0129562e \
-    --hash=sha256:89add70a92d45c9f7700610774368e89d4046a05243150276f65182be92dcca7
-    # via -r requirements.in
-googleapis-common-protos[grpc]==1.60.0 \
-    --hash=sha256:69f9bbcc6acde92cab2db95ce30a70bd2b81d20b12eff3f1aabaffcbe8a93918 \
-    --hash=sha256:e73ebb404098db405ba95d1e1ae0aa91c3e15a71da031a2eeb6b2e23e7bc3708
+    #   tink (setup.py)
+google-cloud-kms==2.19.2 \
+    --hash=sha256:0cc0b9d16338a46b7fc5beba7e96a88df0f836586eb8650e9acd36eb249b52d9 \
+    --hash=sha256:17a5034592e85ef0031d25bbe5894bdb2d719460855980bfeb68aa4e8ffc12bd
+    # via tink (setup.py)
+googleapis-common-protos[grpc]==1.61.0 \
+    --hash=sha256:22f1915393bb3245343f6efe87f6fe868532efc12aa26b391b15132e1279f1c0 \
+    --hash=sha256:8a64866a97f6304a7179873a465d6eee97b7a24ec6cfd78e0f575e96b821240b
     # via
     #   google-api-core
     #   grpc-google-iam-v1
     #   grpcio-status
 grpc-google-iam-v1==0.12.6 \
     --hash=sha256:2bc4b8fdf22115a65d751c9317329322602c39b7c86a289c9b72d228d960ef5f \
     --hash=sha256:5c10f3d8dc2d88678ab1a9b0cb5482735c5efee71e6c0cd59f872eef22913f5c
     # via google-cloud-kms
-grpcio==1.57.0 \
-    --hash=sha256:00258cbe3f5188629828363ae8ff78477ce976a6f63fb2bb5e90088396faa82e \
-    --hash=sha256:092fa155b945015754bdf988be47793c377b52b88d546e45c6a9f9579ac7f7b6 \
-    --hash=sha256:0f80bf37f09e1caba6a8063e56e2b87fa335add314cf2b78ebf7cb45aa7e3d06 \
-    --hash=sha256:20ec6fc4ad47d1b6e12deec5045ec3cd5402d9a1597f738263e98f490fe07056 \
-    --hash=sha256:2313b124e475aa9017a9844bdc5eafb2d5abdda9d456af16fc4535408c7d6da6 \
-    --hash=sha256:23e7d8849a0e58b806253fd206ac105b328171e01b8f18c7d5922274958cc87e \
-    --hash=sha256:2f708a6a17868ad8bf586598bee69abded4996b18adf26fd2d91191383b79019 \
-    --hash=sha256:2f7349786da979a94690cc5c2b804cab4e8774a3cf59be40d037c4342c906649 \
-    --hash=sha256:34950353539e7d93f61c6796a007c705d663f3be41166358e3d88c45760c7d98 \
-    --hash=sha256:40b72effd4c789de94ce1be2b5f88d7b9b5f7379fe9645f198854112a6567d9a \
-    --hash=sha256:4b089f7ad1eb00a104078bab8015b0ed0ebcb3b589e527ab009c53893fd4e613 \
-    --hash=sha256:4faea2cfdf762a664ab90589b66f416274887641ae17817de510b8178356bf73 \
-    --hash=sha256:5371bcd861e679d63b8274f73ac281751d34bd54eccdbfcd6aa00e692a82cd7b \
-    --hash=sha256:5613a2fecc82f95d6c51d15b9a72705553aa0d7c932fad7aed7afb51dc982ee5 \
-    --hash=sha256:57b183e8b252825c4dd29114d6c13559be95387aafc10a7be645462a0fc98bbb \
-    --hash=sha256:5b7a4ce8f862fe32b2a10b57752cf3169f5fe2915acfe7e6a1e155db3da99e79 \
-    --hash=sha256:5e5b58e32ae14658085c16986d11e99abd002ddbf51c8daae8a0671fffb3467f \
-    --hash=sha256:60fe15288a0a65d5c1cb5b4a62b1850d07336e3ba728257a810317be14f0c527 \
-    --hash=sha256:6907b1cf8bb29b058081d2aad677b15757a44ef2d4d8d9130271d2ad5e33efca \
-    --hash=sha256:76c44efa4ede1f42a9d5b2fed1fe9377e73a109bef8675fb0728eb80b0b8e8f2 \
-    --hash=sha256:7a635589201b18510ff988161b7b573f50c6a48fae9cb567657920ca82022b37 \
-    --hash=sha256:7b400807fa749a9eb286e2cd893e501b110b4d356a218426cb9c825a0474ca56 \
-    --hash=sha256:82640e57fb86ea1d71ea9ab54f7e942502cf98a429a200b2e743d8672171734f \
-    --hash=sha256:871f9999e0211f9551f368612460442a5436d9444606184652117d6a688c9f51 \
-    --hash=sha256:9338bacf172e942e62e5889b6364e56657fbf8ac68062e8b25c48843e7b202bb \
-    --hash=sha256:a8a8e560e8dbbdf29288872e91efd22af71e88b0e5736b0daf7773c1fecd99f0 \
-    --hash=sha256:aed90d93b731929e742967e236f842a4a2174dc5db077c8f9ad2c5996f89f63e \
-    --hash=sha256:b363bbb5253e5f9c23d8a0a034dfdf1b7c9e7f12e602fc788c435171e96daccc \
-    --hash=sha256:b4098b6b638d9e0ca839a81656a2fd4bc26c9486ea707e8b1437d6f9d61c3941 \
-    --hash=sha256:b53333627283e7241fcc217323f225c37783b5f0472316edcaa4479a213abfa6 \
-    --hash=sha256:b670c2faa92124b7397b42303e4d8eb64a4cd0b7a77e35a9e865a55d61c57ef9 \
-    --hash=sha256:bb396952cfa7ad2f01061fbc7dc1ad91dd9d69243bcb8110cf4e36924785a0fe \
-    --hash=sha256:c60b83c43faeb6d0a9831f0351d7787a0753f5087cc6fa218d78fdf38e5acef0 \
-    --hash=sha256:c6ebecfb7a31385393203eb04ed8b6a08f5002f53df3d59e5e795edb80999652 \
-    --hash=sha256:d78d8b86fcdfa1e4c21f8896614b6cc7ee01a2a758ec0c4382d662f2a62cf766 \
-    --hash=sha256:d7f8df114d6b4cf5a916b98389aeaf1e3132035420a88beea4e3d977e5f267a5 \
-    --hash=sha256:e1cb52fa2d67d7f7fab310b600f22ce1ff04d562d46e9e0ac3e3403c2bb4cc16 \
-    --hash=sha256:e3fdf04e402f12e1de8074458549337febb3b45f21076cc02ef4ff786aff687e \
-    --hash=sha256:e503cb45ed12b924b5b988ba9576dc9949b2f5283b8e33b21dcb6be74a7c58d0 \
-    --hash=sha256:f19ac6ac0a256cf77d3cc926ef0b4e64a9725cc612f97228cd5dc4bd9dbab03b \
-    --hash=sha256:f1fb0fd4a1e9b11ac21c30c169d169ef434c6e9344ee0ab27cfa6f605f6387b2 \
-    --hash=sha256:fada6b07ec4f0befe05218181f4b85176f11d531911b64c715d1875c4736d73a \
-    --hash=sha256:fd173b4cf02b20f60860dc2ffe30115c18972d7d6d2d69df97ac38dee03be5bf \
-    --hash=sha256:fe752639919aad9ffb0dee0d87f29a6467d1ef764f13c4644d212a9a853a078d \
-    --hash=sha256:fee387d2fab144e8a34e0e9c5ca0f45c9376b99de45628265cfa9886b1dbe62b
+grpcio==1.59.2 \
+    --hash=sha256:023088764012411affe7db183d1ada3ad9daf2e23ddc719ff46d7061de661340 \
+    --hash=sha256:08d77e682f2bf730a4961eea330e56d2f423c6a9b91ca222e5b1eb24a357b19f \
+    --hash=sha256:0a4a3833c0e067f3558538727235cd8a49709bff1003200bbdefa2f09334e4b1 \
+    --hash=sha256:0a754aff9e3af63bdc4c75c234b86b9d14e14a28a30c4e324aed1a9b873d755f \
+    --hash=sha256:11168ef43e4a43ff1b1a65859f3e0ef1a173e277349e7fb16923ff108160a8cd \
+    --hash=sha256:128e20f57c5f27cb0157e73756d1586b83c1b513ebecc83ea0ac37e4b0e4e758 \
+    --hash=sha256:1f9524d1d701e399462d2c90ba7c193e49d1711cf429c0d3d97c966856e03d00 \
+    --hash=sha256:1ff16d68bf453275466a9a46739061a63584d92f18a0f5b33d19fc97eb69867c \
+    --hash=sha256:2067274c88bc6de89c278a672a652b4247d088811ece781a4858b09bdf8448e3 \
+    --hash=sha256:2171c39f355ba5b551c5d5928d65aa6c69807fae195b86ef4a7d125bcdb860a9 \
+    --hash=sha256:242adc47725b9a499ee77c6a2e36688fa6c96484611f33b1be4c57ab075a92dd \
+    --hash=sha256:27f879ae604a7fcf371e59fba6f3ff4635a4c2a64768bd83ff0cac503142fef4 \
+    --hash=sha256:2b230028a008ae1d0f430acb227d323ff8a619017415cf334c38b457f814119f \
+    --hash=sha256:3059668df17627f0e0fa680e9ef8c995c946c792612e9518f5cc1503be14e90b \
+    --hash=sha256:31176aa88f36020055ace9adff2405a33c8bdbfa72a9c4980e25d91b2f196873 \
+    --hash=sha256:36f53c2b3449c015880e7d55a89c992c357f176327b0d2873cdaaf9628a37c69 \
+    --hash=sha256:3b4368b33908f683a363f376dfb747d40af3463a6e5044afee07cf9436addf96 \
+    --hash=sha256:3c61d641d4f409c5ae46bfdd89ea42ce5ea233dcf69e74ce9ba32b503c727e29 \
+    --hash=sha256:4abb717e320e74959517dc8e84a9f48fbe90e9abe19c248541e9418b1ce60acd \
+    --hash=sha256:4c93f4abbb54321ee6471e04a00139c80c754eda51064187963ddf98f5cf36a4 \
+    --hash=sha256:535561990e075fa6bd4b16c4c3c1096b9581b7bb35d96fac4650f1181e428268 \
+    --hash=sha256:53c9aa5ddd6857c0a1cd0287225a2a25873a8e09727c2e95c4aebb1be83a766a \
+    --hash=sha256:5d573e70a6fe77555fb6143c12d3a7d3fa306632a3034b4e7c59ca09721546f8 \
+    --hash=sha256:6009386a2df66159f64ac9f20425ae25229b29b9dd0e1d3dd60043f037e2ad7e \
+    --hash=sha256:686e975a5d16602dc0982c7c703948d17184bd1397e16c8ee03511ecb8c4cdda \
+    --hash=sha256:6959fb07e8351e20501ffb8cc4074c39a0b7ef123e1c850a7f8f3afdc3a3da01 \
+    --hash=sha256:6b25ed37c27e652db01be341af93fbcea03d296c024d8a0e680017a268eb85dd \
+    --hash=sha256:6da6dea3a1bacf99b3c2187e296db9a83029ed9c38fd4c52b7c9b7326d13c828 \
+    --hash=sha256:72ca2399097c0b758198f2ff30f7178d680de8a5cfcf3d9b73a63cf87455532e \
+    --hash=sha256:73abb8584b0cf74d37f5ef61c10722adc7275502ab71789a8fe3cb7ef04cf6e2 \
+    --hash=sha256:74100fecaec8a535e380cf5f2fb556ff84957d481c13e54051c52e5baac70541 \
+    --hash=sha256:75c6ecb70e809cf1504465174343113f51f24bc61e22a80ae1c859f3f7034c6d \
+    --hash=sha256:7cf05053242f61ba94014dd3a986e11a083400a32664058f80bf4cf817c0b3a1 \
+    --hash=sha256:9411e24328a2302e279e70cae6e479f1fddde79629fcb14e03e6d94b3956eabf \
+    --hash=sha256:a213acfbf186b9f35803b52e4ca9addb153fc0b67f82a48f961be7000ecf6721 \
+    --hash=sha256:bb7e0fe6ad73b7f06d7e2b689c19a71cf5cc48f0c2bf8608469e51ffe0bd2867 \
+    --hash=sha256:c2504eed520958a5b77cc99458297cb7906308cb92327f35fb7fbbad4e9b2188 \
+    --hash=sha256:c35aa9657f5d5116d23b934568e0956bd50c615127810fffe3ac356a914c176a \
+    --hash=sha256:c5f09cffa619adfb44799fa4a81c2a1ad77c887187613fb0a8f201ab38d89ba1 \
+    --hash=sha256:c978f864b35f2261e0819f5cd88b9830b04dc51bcf055aac3c601e525a10d2ba \
+    --hash=sha256:cbe946b3e6e60a7b4618f091e62a029cb082b109a9d6b53962dd305087c6e4fd \
+    --hash=sha256:cc3e4cd087f07758b16bef8f31d88dbb1b5da5671d2f03685ab52dece3d7a16e \
+    --hash=sha256:cf0dead5a2c5a3347af2cfec7131d4f2a2e03c934af28989c9078f8241a491fa \
+    --hash=sha256:d2794f0e68b3085d99b4f6ff9c089f6fdd02b32b9d3efdfbb55beac1bf22d516 \
+    --hash=sha256:d2fa68a96a30dd240be80bbad838a0ac81a61770611ff7952b889485970c4c71 \
+    --hash=sha256:d6f70406695e3220f09cd7a2f879333279d91aa4a8a1d34303b56d61a8180137 \
+    --hash=sha256:d8f9cd4ad1be90b0cf350a2f04a38a36e44a026cac1e036ac593dc48efe91d52 \
+    --hash=sha256:da2d94c15f88cd40d7e67f7919d4f60110d2b9d5b1e08cf354c2be773ab13479 \
+    --hash=sha256:e1727c1c0e394096bb9af185c6923e8ea55a5095b8af44f06903bcc0e06800a2 \
+    --hash=sha256:e420ced29b5904cdf9ee5545e23f9406189d8acb6750916c2db4793dada065c6 \
+    --hash=sha256:e82c5cf1495244adf5252f925ac5932e5fd288b3e5ab6b70bec5593074b7236c \
+    --hash=sha256:f1ef0d39bc1feb420caf549b3c657c871cad4ebbcf0580c4d03816b0590de0cf \
+    --hash=sha256:f8753a6c88d1d0ba64302309eecf20f70d2770f65ca02d83c2452279085bfcd3 \
+    --hash=sha256:f93dbf58f03146164048be5426ffde298b237a5e059144847e4940f5b80172c3
     # via
     #   google-api-core
     #   googleapis-common-protos
     #   grpc-google-iam-v1
     #   grpcio-status
-grpcio-status==1.57.0 \
-    --hash=sha256:15d6af055914ebbc4ed17e55ebfb8e6bb17a45a57fea32e6af19978fb7844690 \
-    --hash=sha256:b098da99df1eebe58337f8f78e50df990273ccacc1226fddeb47c590e3df9e02
+grpcio-status==1.59.2 \
+    --hash=sha256:24bdf3b3b83b9112f43bd0626f82510d12cc1d919a45028ac20eb6919218e508 \
+    --hash=sha256:a2c2b146e66b73ba80d021ab34fce5db4dd9be67ca4566cda40d36b185ce54f4
     # via google-api-core
 idna==3.4 \
     --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
     # via requests
 jmespath==1.0.1 \
     --hash=sha256:02e2e4cc71b5bcab88332eebf907519190dd9e6e82107fa7f83b1003a6252980 \
@@ -195,36 +219,34 @@
     # via
     #   boto3
     #   botocore
 proto-plus==1.22.3 \
     --hash=sha256:a49cd903bc0b6ab41f76bf65510439d56ca76f868adf0274e738bfdd096894df \
     --hash=sha256:fdcd09713cbd42480740d2fe29c990f7fbd885a67efc328aa8be6ee3e9f76a6b
     # via google-cloud-kms
-protobuf==4.24.0 \
-    --hash=sha256:44825e963008f8ea0d26c51911c30d3e82e122997c3c4568fd0385dd7bacaedf \
-    --hash=sha256:567fe6b0647494845d0849e3d5b260bfdd75692bf452cdc9cb660d12457c055d \
-    --hash=sha256:5ab19ee50037d4b663c02218a811a5e1e7bb30940c79aac385b96e7a4f9daa61 \
-    --hash=sha256:5d0ceb9de6e08311832169e601d1fc71bd8e8c779f3ee38a97a78554945ecb85 \
-    --hash=sha256:6c817cf4a26334625a1904b38523d1b343ff8b637d75d2c8790189a4064e51c3 \
-    --hash=sha256:81cb9c4621d2abfe181154354f63af1c41b00a4882fb230b4425cbaed65e8f52 \
-    --hash=sha256:82e6e9ebdd15b8200e8423676eab38b774624d6a1ad696a60d86a2ac93f18201 \
-    --hash=sha256:8bb52a2be32db82ddc623aefcedfe1e0eb51da60e18fcc908fb8885c81d72109 \
-    --hash=sha256:a38400a692fd0c6944c3c58837d112f135eb1ed6cdad5ca6c5763336e74f1a04 \
-    --hash=sha256:a6b1ca92ccabfd9903c0c7dde8876221dc7d8d87ad5c42e095cc11b15d3569c7 \
-    --hash=sha256:ae7a1835721086013de193311df858bc12cd247abe4ef9710b715d930b95b33e \
-    --hash=sha256:ae97b5de10f25b7a443b40427033e545a32b0e9dda17bcd8330d70033379b3e5 \
-    --hash=sha256:e8834ef0b4c88666ebb7c7ec18045aa0f4325481d724daa624a4cf9f28134653
+protobuf==4.25.0 \
+    --hash=sha256:1a3ba712877e6d37013cdc3476040ea1e313a6c2e1580836a94f76b3c176d575 \
+    --hash=sha256:1a53d6f64b00eecf53b65ff4a8c23dc95df1fa1e97bb06b8122e5a64f49fc90a \
+    --hash=sha256:32ac2100b0e23412413d948c03060184d34a7c50b3e5d7524ee96ac2b10acf51 \
+    --hash=sha256:5c1203ac9f50e4853b0a0bfffd32c67118ef552a33942982eeab543f5c634395 \
+    --hash=sha256:63714e79b761a37048c9701a37438aa29945cd2417a97076048232c1df07b701 \
+    --hash=sha256:683dc44c61f2620b32ce4927de2108f3ebe8ccf2fd716e1e684e5a50da154054 \
+    --hash=sha256:68f7caf0d4f012fd194a301420cf6aa258366144d814f358c5b32558228afa7c \
+    --hash=sha256:b2cf8b5d381f9378afe84618288b239e75665fe58d0f3fd5db400959274296e9 \
+    --hash=sha256:c40ff8f00aa737938c5378d461637d15c442a12275a81019cc2fef06d81c9419 \
+    --hash=sha256:cf21faba64cd2c9a3ed92b7a67f226296b10159dbb8fbc5e854fc90657d908e4 \
+    --hash=sha256:d94a33db8b7ddbd0af7c467475fb9fde0c705fb315a8433c0e2020942b863a1f
     # via
-    #   -r requirements.in
     #   google-api-core
     #   google-cloud-kms
     #   googleapis-common-protos
     #   grpc-google-iam-v1
     #   grpcio-status
     #   proto-plus
+    #   tink (setup.py)
 pyasn1==0.5.0 \
     --hash=sha256:87a2121042a1ac9358cabcaf1d07680ff97ee6404333bacca15f76aa8ad01a57 \
     --hash=sha256:97b7290ca68e62a832558ec3976f15cbf911bf5d7c7039d8b861c2a0ece69fde
     # via
     #   pyasn1-modules
     #   rsa
 pyasn1-modules==0.3.0 \
@@ -239,24 +261,21 @@
     --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
     --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
     # via google-api-core
 rsa==4.9 \
     --hash=sha256:90260d9058e514786967344d0ef75fa8727eed8a7d2e43ce9f4bcf1b536174f7 \
     --hash=sha256:e38464a49c6c85d7f1351b0126661487a7e0a14a50f1675ec50eb34d4f20ef21
     # via google-auth
-s3transfer==0.6.1 \
-    --hash=sha256:3c0da2d074bf35d6870ef157158641178a4204a6e689e82546083e31e0311346 \
-    --hash=sha256:640bb492711f4c0c0905e1f62b6aaeb771881935ad27884852411f8e9cacbca9
+s3transfer==0.7.0 \
+    --hash=sha256:10d6923c6359175f264811ef4bf6161a3156ce8e350e705396a7557d6293c33a \
+    --hash=sha256:fd3889a66f5fe17299fe75b82eae6cf722554edca744ca5d5fe308b104883d2e
     # via boto3
 six==1.16.0 \
     --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
-    # via
-    #   google-auth
-    #   python-dateutil
-urllib3==1.26.16 \
-    --hash=sha256:8d36afa7616d8ab714608411b4a3b13e58f463aee519024578e062e141dce20f \
-    --hash=sha256:8f135f6502756bde6b2a9b28989df5fbe87c9970cecaa69041edcce7f0589b14
+    # via python-dateutil
+urllib3==2.0.7 \
+    --hash=sha256:c97dfde1f7bd43a71c8d2a58e369e9b2bf692d1334ea9f9cae55add7d0dd0f84 \
+    --hash=sha256:fdb6d215c776278489906c2f8916e6e7d4f5a9b602ccbcfdf7f016fc8da0596e
     # via
     #   botocore
-    #   google-auth
     #   requests
```

### Comparing `tink-1.8.0/setup.py` & `tink-1.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 import glob
 import os
 import platform
 import posixpath
 import re
 import shutil
 import subprocess
-import textwrap
 from typing import List
 
 import setuptools
 from setuptools.command import build_ext
 
 _PROJECT_BASE_DIR = os.path.dirname(os.path.abspath(__file__))
 _TINK_CRYPTO_GITHUB_ORG_URL = 'https://github.com/tink-crypto'
@@ -54,38 +53,43 @@
 
 def _get_bazel_command() -> str:
   """Finds the bazel command."""
   if shutil.which('bazelisk'):
     return 'bazelisk'
   elif shutil.which('bazel'):
     return 'bazel'
-  raise FileNotFoundError('Could not find bazel executable. Please install '
-                          'bazel to compile the Tink Python package.')
+  raise FileNotFoundError(
+      'Could not find bazel executable. Please install '
+      'bazel to compile the Tink Python package.'
+  )
 
 
 def _get_protoc_command() -> str:
   """Finds the protoc command."""
   if 'PROTOC' in os.environ and os.path.exists(os.environ['PROTOC']):
     return os.environ['PROTOC']
   protoc_path = shutil.which('protoc')
   if protoc_path is None:
-    raise FileNotFoundError('Could not find protoc executable. Please install '
-                            'protoc to compile the Tink Python package.')
+    raise FileNotFoundError(
+        'Could not find protoc executable. Please install '
+        'protoc to compile the Tink Python package.'
+    )
   return protoc_path
 
 
 def _generate_proto(protoc: str, source: str) -> None:
   """Invokes protoc to generate a _pb2.py from .proto files."""
   if not os.path.exists(source):
     raise FileNotFoundError(f'Cannot find required file: {source}')
 
   output = source.replace('.proto', '_pb2.py')
 
-  if (os.path.exists(output) and
-      os.path.getmtime(source) < os.path.getmtime(output)):
+  if os.path.exists(output) and os.path.getmtime(source) < os.path.getmtime(
+      output
+  ):
     # No need to regenerate if output is newer than source.
     return
 
   print(f'Generating {output}...')
   protoc_args = [protoc, '-I.', '--python_out=.', source]
   subprocess.run(args=protoc_args, check=True)
 
@@ -96,56 +100,27 @@
     return [
         line.rstrip()
         for line in f
         if not (line.isspace() or line.startswith('#'))
     ]
 
 
-def _patch_workspace(workspace_file_path: str):
-  """Update WORKSPACE with local Bazel dependencies based on an env variable.
-
-  If TINK_PYTHON_SETUPTOOLS_LOCAL_TINK_CC_PATH is set, override the default
-  tink-cc dependency with a local_repository pointing to
-  TINK_PYTHON_SETUPTOOLS_LOCAL_TINK_CC_PATH.
-
-  NOTE: This is for testing only!
-
-  Args:
-    workspace_file_path: The WORKSPACE file path.
-  """
-  if 'TINK_PYTHON_SETUPTOOLS_LOCAL_TINK_CC_PATH' not in os.environ:
-    # Do nothing.
-    return
-
-  with open(workspace_file_path, 'r') as f:
-    workspace_content = f.read()
-  tink_cc_path = os.environ['TINK_PYTHON_SETUPTOOLS_LOCAL_TINK_CC_PATH']
-  before = '# Placeholder for tink-cc override.'
-  after = textwrap.dedent(f"""\
-      # Modified by setup.py
-      local_repository(
-          name = "tink_cc",
-          path = "{tink_cc_path}",
-      )""")
-  workspace_content = workspace_content.replace(before, after)
-  with open(workspace_file_path, 'w') as f:
-    f.write(workspace_content)
-
-
 class BazelExtension(setuptools.Extension):
   """A C/C++ extension that is defined as a Bazel BUILD target."""
 
   def __init__(self, bazel_target: str, target_name: str = '') -> None:
     self.bazel_target = bazel_target
-    self.relpath, self.target_name = (
-        posixpath.relpath(bazel_target, '//').split(':'))
+    self.relpath, self.target_name = posixpath.relpath(
+        bazel_target, '//'
+    ).split(':')
     if target_name:
       self.target_name = target_name
     ext_name = os.path.join(
-        self.relpath.replace(posixpath.sep, os.path.sep), self.target_name)
+        self.relpath.replace(posixpath.sep, os.path.sep), self.target_name
+    )
     setuptools.Extension.__init__(self, ext_name, sources=[])
 
 
 class BuildBazelExtension(build_ext.build_ext):
   """A command that runs Bazel to build a C/C++ extension."""
 
   def __init__(self, dist: str) -> None:
@@ -157,24 +132,24 @@
       self.bazel_build(ext)
     build_ext.build_ext.run(self)
 
   def bazel_build(self, ext: str) -> None:
     if not os.path.exists(self.build_temp):
       os.makedirs(self.build_temp)
 
-    _patch_workspace('WORKSPACE')
-
     # Ensure no artifacts from previous builds are reused (i.e. from builds
     # using a different Python version).
     bazel_clean_argv = [self.bazel_command, 'clean', '--expunge']
     self.spawn(bazel_clean_argv)
 
     bazel_argv = [
-        self.bazel_command, 'build', ext.bazel_target,
-        '--compilation_mode=' + ('dbg' if self.debug else 'opt')
+        self.bazel_command,
+        'build',
+        ext.bazel_target,
+        '--compilation_mode=' + ('dbg' if self.debug else 'opt'),
     ]
 
     if platform.system() == 'Darwin':
       # Set the minimum macOS version to support based on
       # MACOSX_DEPLOYMENT_TARGET. This mimics the CMake behavior: when
       # MACOSX_DEPLOYMENT_TARGET is set, use its value to determine the minimum
       # OS version.
@@ -189,56 +164,70 @@
 
       archflags = os.getenv('ARCHFLAGS', '')
       if platform.machine() == 'x86_64' and 'arm64' in archflags:
         # We are cross compiling for arm64; set the correct CPU params.
         bazel_argv += ['--cpu=darwin_arm64', '--macos_cpus=arm64']
 
     self.spawn(bazel_argv)
-    ext_bazel_bin_path = os.path.join('bazel-bin', ext.relpath,
-                                      ext.target_name + '.so')
+    ext_bazel_bin_path = os.path.join(
+        'bazel-bin', ext.relpath, ext.target_name + '.so'
+    )
     ext_dest_path = self.get_ext_fullpath(ext.name)
     ext_dest_dir = os.path.dirname(ext_dest_path)
     if not os.path.exists(ext_dest_dir):
       os.makedirs(ext_dest_dir)
     shutil.copyfile(ext_bazel_bin_path, ext_dest_path)
 
 
 def main() -> None:
   # Generate compiled protocol buffers.
   protoc_command = _get_protoc_command()
   for proto_file in glob.glob('tink/proto/*.proto'):
     _generate_proto(protoc_command, proto_file)
 
+  gcpkms_extra_requirements = _parse_requirements('requirements_gcpkms.in')
+  awskms_extra_requirements = _parse_requirements('requirements_awskms.in')
+
   setuptools.setup(
       name='tink',
       version=_get_tink_version(),
       url=f'{_TINK_CRYPTO_GITHUB_ORG_URL}/tink-py',
-      description='A multi-language, cross-platform library that provides '
-      'cryptographic APIs that are secure, easy to use correctly, and hard(er) '
-      'to misuse.',
+      description=(
+          'A multi-language, cross-platform library that provides cryptographic'
+          ' APIs that are secure, easy to use correctly, and hard(er) to'
+          ' misuse.'
+      ),
       author='Tink Developers',
       author_email='tink-users@googlegroups.com',
       long_description=open('README.md').read(),
       long_description_content_type='text/markdown',
       # Contained modules and scripts.
       packages=setuptools.find_packages(),
       install_requires=_parse_requirements('requirements.in'),
+      extras_require={
+          'gcpkms': gcpkms_extra_requirements,
+          'awskms': awskms_extra_requirements,
+          'all': gcpkms_extra_requirements + awskms_extra_requirements,
+      },
       cmdclass=dict(build_ext=BuildBazelExtension),
       ext_modules=[
           BazelExtension('//tink/cc/pybind:tink_bindings'),
       ],
       zip_safe=False,
       # PyPI package information.
       classifiers=[
-          'Programming Language :: Python :: 3.7',
+          'Programming Language :: Python',
+          'Programming Language :: Python :: 3',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11',
           'Topic :: Software Development :: Libraries',
       ],
       license='Apache 2.0',
       keywords='tink cryptography',
+      python_requires='>=3.8',
   )
 
 
 if __name__ == '__main__':
   main()
```

### Comparing `tink-1.8.0/tink/BUILD.bazel` & `tink-1.9.0/tink/BUILD.bazel`

 * *Files 22% similar despite different names*

```diff
@@ -15,17 +15,19 @@
     ],
 )
 
 py_library(
     name = "tink",
     srcs_version = "PY3",
     deps = [
+        ":_json_proto_keyset_format",
         ":_keyset_handle",
         ":_keyset_reader",
         ":_keyset_writer",
+        ":_proto_keyset_format",
         "//tink/core",
     ],
 )
 
 py_library(
     name = "_keyset_handle",
     srcs = ["_keyset_handle.py"],
@@ -137,14 +139,15 @@
     ],
 )
 
 py_library(
     name = "secret_key_access",
     srcs = ["secret_key_access.py"],
     srcs_version = "PY3",
+    visibility = ["//visibility:public"],
     deps = [
         "//tink/core",
     ],
 )
 
 py_test(
     name = "secret_key_access_test",
@@ -179,7 +182,113 @@
         ":tink_config",
         ":tink_python",
         requirement("absl-py"),
         "//tink/core",
         "//tink/mac",
     ],
 )
+
+py_library(
+    name = "_kms_clients",
+    srcs = ["_kms_clients.py"],
+    deps = [
+        "//tink/aead:_aead",
+        "//tink/core:_tink_error",
+    ],
+)
+
+py_test(
+    name = "_kms_clients_test",
+    srcs = ["_kms_clients_test.py"],
+    python_version = "PY3",
+    srcs_version = "PY3",
+    deps = [
+        ":_kms_clients",
+        ":tink_config",
+        ":tink_python",
+        requirement("absl-py"),
+        "//tink/aead",
+    ],
+)
+
+py_library(
+    name = "_insecure_keyset_handle",
+    srcs = ["_insecure_keyset_handle.py"],
+    deps = [
+        ":_keyset_handle",
+        ":secret_key_access",
+        "//tink/core",
+        "//tink/proto:tink_py_pb2",
+    ],
+)
+
+py_library(
+    name = "_insecure_keyset_handle_test",
+    srcs = ["_insecure_keyset_handle_test.py"],
+    deps = [
+        ":_insecure_keyset_handle",
+        ":secret_key_access",
+        ":tink_config",
+        ":tink_python",
+        requirement("absl-py"),
+        "//tink/aead",
+        "//tink/core",
+    ],
+)
+
+py_library(
+    name = "_proto_keyset_format",
+    srcs = ["_proto_keyset_format.py"],
+    srcs_version = "PY3",
+    deps = [
+        ":_insecure_keyset_handle",
+        ":_keyset_handle",
+        ":_keyset_reader",
+        ":_keyset_writer",
+        "//tink/aead",
+        "//tink/core",
+    ],
+)
+
+py_test(
+    name = "_proto_keyset_format_test",
+    srcs = ["_proto_keyset_format_test.py"],
+    srcs_version = "PY3",
+    deps = [
+        ":secret_key_access",
+        ":tink_config",
+        ":tink_python",
+        requirement("absl-py"),
+        "//tink/aead",
+        "//tink/core",
+        "//tink/hybrid",
+    ],
+)
+
+py_library(
+    name = "_json_proto_keyset_format",
+    srcs = ["_json_proto_keyset_format.py"],
+    srcs_version = "PY3",
+    deps = [
+        ":_insecure_keyset_handle",
+        ":_keyset_handle",
+        ":_keyset_reader",
+        ":_keyset_writer",
+        "//tink/aead",
+        "//tink/core",
+    ],
+)
+
+py_test(
+    name = "_json_proto_keyset_format_test",
+    srcs = ["_json_proto_keyset_format_test.py"],
+    srcs_version = "PY3",
+    deps = [
+        ":secret_key_access",
+        ":tink_config",
+        ":tink_python",
+        requirement("absl-py"),
+        "//tink/aead",
+        "//tink/core",
+        "//tink/hybrid",
+    ],
+)
```

### Comparing `tink-1.8.0/tink/_keyset_handle.py` & `tink-1.9.0/tink/_keyset_handle.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/_keyset_handle_test.py` & `tink-1.9.0/tink/_keyset_handle_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/_keyset_reader.py` & `tink-1.9.0/tink/_keyset_reader.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/_keyset_reader_test.py` & `tink-1.9.0/tink/_keyset_reader_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/_keyset_writer.py` & `tink-1.9.0/tink/_keyset_writer.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/_keyset_writer_test.py` & `tink-1.9.0/tink/_keyset_writer_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/aead/BUILD.bazel` & `tink-1.9.0/tink/aead/BUILD.bazel`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 py_test(
     name = "_aead_key_manager_test",
     srcs = ["_aead_key_manager_test.py"],
     srcs_version = "PY3",
     deps = [
         ":aead",
         requirement("absl-py"),
-        "//tink:cleartext_keyset_handle",
         "//tink:tink_python",
         "//tink/core",
         "//tink/mac",
         "//tink/proto:aes_ctr_hmac_aead_py_pb2",
         "//tink/proto:aes_eax_py_pb2",
         "//tink/proto:aes_gcm_py_pb2",
         "//tink/proto:aes_gcm_siv_py_pb2",
@@ -62,15 +61,14 @@
 
 py_library(
     name = "_aead_wrapper",
     srcs = ["_aead_wrapper.py"],
     srcs_version = "PY3",
     deps = [
         ":_aead",
-        requirement("absl-py"),
         "//tink/core",
     ],
 )
 
 py_test(
     name = "_aead_wrapper_test",
     srcs = ["_aead_wrapper_test.py"],
@@ -146,13 +144,29 @@
 
 py_library(
     name = "_kms_aead_key_manager",
     srcs = ["_kms_aead_key_manager.py"],
     deps = [
         ":_aead",
         ":_kms_envelope_aead",
+        "//tink:_kms_clients",
         "//tink/core",
         "//tink/proto:kms_aead_py_pb2",
         "//tink/proto:kms_envelope_py_pb2",
         "//tink/proto:tink_py_pb2",
     ],
 )
+
+py_test(
+    name = "_kms_aead_key_manager_test",
+    srcs = ["_kms_aead_key_manager_test.py"],
+    srcs_version = "PY3",
+    deps = [
+        ":_kms_aead_key_manager",
+        ":aead",
+        requirement("absl-py"),
+        "//tink:tink_python",
+        "//tink/proto:kms_aead_py_pb2",
+        "//tink/proto:kms_envelope_py_pb2",
+        "//tink/proto:tink_py_pb2",
+    ],
+)
```

### Comparing `tink-1.8.0/tink/aead/__init__.py` & `tink-1.9.0/tink/aead/__init__.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/aead/_aead.py` & `tink-1.9.0/tink/aead/_aead.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/aead/_aead_key_manager.py` & `tink-1.9.0/tink/aead/_aead_key_manager.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/aead/_aead_key_manager_test.py` & `tink-1.9.0/tink/aead/_aead_key_manager_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from tink.proto import aes_gcm_pb2
 from tink.proto import aes_gcm_siv_pb2
 from tink.proto import common_pb2
 from tink.proto import tink_pb2
 from tink.proto import xchacha20_poly1305_pb2
 import tink
 from tink import aead
-from tink import cleartext_keyset_handle
 from tink import core
 from tink import mac
 from tink.testing import fake_kms
 
 
 FAKE_KMS_URI = 'fake-kms://CM2b3_MDElQKSAowdHlwZS5nb29nbGVhcGlzLmNvbS9nb29nbGUuY3J5cHRvLnRpbmsuQWVzR2NtS2V5EhIaEIK75t5L-adlUwVhWvRuWUwYARABGM2b3_MDIAE'
 
@@ -230,16 +229,17 @@
           },
           "status": "ENABLED",
           "keyId": 371374440,
           "outputPrefixType": "RAW"
         }
       ]
     }'''
-    keyset_handle = cleartext_keyset_handle.read(
-        tink.JsonKeysetReader(json_keyset))
+    keyset_handle = tink.json_proto_keyset_format.parse_without_secret(
+        json_keyset
+    )
 
     ciphertext = bytes.fromhex(
         '00000033013e77cdcd39016d632a3bb83b694565d3d2d85329ccc3aff540'
         'ef00a7dcb95c157f0199fa7af825a2da2cf2ed0818e6eb0becb39d73d1b1'
         '26e60bdac2dbe7d742dabaedcc2b3809e429510d9a330dc9e2bb1dc9d5b59ecc'
     )
     primitive = keyset_handle.primitive(aead.Aead)
```

### Comparing `tink-1.8.0/tink/aead/_aead_key_templates.py` & `tink-1.9.0/tink/aead/_aead_key_templates.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/aead/_aead_key_templates_test.py` & `tink-1.9.0/tink/aead/_aead_key_templates_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/aead/_aead_wrapper.py` & `tink-1.9.0/tink/aead/_aead_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """AEAD wrapper."""
 
 from typing import Type
-from absl import logging
 
 from tink import core
 from tink.aead import _aead
 
 
 class _WrappedAead(_aead.Aead):
   """Implements Aead for a set of Aead primitives."""
@@ -36,22 +35,21 @@
     if len(ciphertext) > core.crypto_format.NON_RAW_PREFIX_SIZE:
       prefix = ciphertext[:core.crypto_format.NON_RAW_PREFIX_SIZE]
       ciphertext_no_prefix = ciphertext[core.crypto_format.NON_RAW_PREFIX_SIZE:]
       for entry in self._primitive_set.primitive_from_identifier(prefix):
         try:
           return entry.primitive.decrypt(ciphertext_no_prefix,
                                          associated_data)
-        except core.TinkError as e:
-          logging.info(
-              'ciphertext prefix matches a key, but cannot decrypt: %s', e)
+        except core.TinkError:
+          pass
     # Let's try all RAW keys.
     for entry in self._primitive_set.raw_primitives():
       try:
         return entry.primitive.decrypt(ciphertext, associated_data)
-      except core.TinkError as e:
+      except core.TinkError:
         pass
     # nothing works.
     raise core.TinkError('Decryption failed.')
 
 
 class AeadWrapper(core.PrimitiveWrapper[_aead.Aead, _aead.Aead]):
   """AeadWrapper is the implementation of PrimitiveWrapper for Aead.
```

### Comparing `tink-1.8.0/tink/aead/_aead_wrapper_test.py` & `tink-1.9.0/tink/aead/_aead_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/aead/_kms_aead_key_manager.py` & `tink-1.9.0/tink/aead/_kms_aead_key_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,58 +10,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Python KMS AEAD key manager."""
 
-import abc
 
-from typing import List, Type
+from typing import Type
 
 from tink.proto import kms_aead_pb2
 from tink.proto import kms_envelope_pb2
 from tink.proto import tink_pb2
+from tink import _kms_clients
 from tink import core
 from tink.aead import _aead
 from tink.aead import _kms_envelope_aead
 
 
-class KmsClient(metaclass=abc.ABCMeta):
-
-  @abc.abstractmethod
-  def does_support(self, key_uri: str) -> bool:
-    raise NotImplementedError()
-
-  @abc.abstractmethod
-  def get_aead(self, key_uri: str) -> _aead.Aead:
-    raise NotImplementedError()
-
-
-_kms_clients: List[KmsClient] = []
-
-
-def register_kms_client(client: KmsClient) -> None:
-  """Tink-internal function to register kms clients."""
-  _kms_clients.append(client)
-
-
-def reset_kms_clients() -> None:
-  """Removes all previously registered KMS clients. Used in tests."""
-  _kms_clients.clear()
-
-
-def _kms_client_from_uri(key_uri: str) -> KmsClient:
-  """Tink-internal function to get a KmsClient."""
-  for client in _kms_clients:
-    if client.does_support(key_uri):
-      return client
-  raise core.TinkError('No KMS client does support: ' + key_uri)
-
-
 _KMS_AEAD_KEY_TYPE_URL = 'type.googleapis.com/google.crypto.tink.KmsAeadKey'
 _KMS_ENVELOPE_AEAD_KEY_TYPE_URL = (
     'type.googleapis.com/google.crypto.tink.KmsEnvelopeAeadKey'
 )
 
 
 class KmsAeadKeyManager(core.KeyManager[_aead.Aead]):
@@ -70,15 +38,15 @@
   def primitive_class(self) -> Type[_aead.Aead]:
     return _aead.Aead
 
   def primitive(self, key_data: tink_pb2.KeyData) -> _aead.Aead:
     if key_data.type_url != _KMS_AEAD_KEY_TYPE_URL:
       raise core.TinkError('wrong key type: ' + key_data.type_url)
     kms_key = kms_aead_pb2.KmsAeadKey.FromString(key_data.value)
-    client = _kms_client_from_uri(kms_key.params.key_uri)
+    client = _kms_clients.kms_client_from_uri(kms_key.params.key_uri)
     return client.get_aead(key_uri=kms_key.params.key_uri)
 
   def key_type(self) -> str:
     return _KMS_AEAD_KEY_TYPE_URL
 
   def new_key_data(
       self, key_template: tink_pb2.KeyTemplate
@@ -105,15 +73,15 @@
   def primitive_class(self) -> Type[_aead.Aead]:
     return _aead.Aead
 
   def primitive(self, key_data: tink_pb2.KeyData) -> _aead.Aead:
     if key_data.type_url != _KMS_ENVELOPE_AEAD_KEY_TYPE_URL:
       raise core.TinkError('wrong key type: ' + key_data.type_url)
     env_key = kms_envelope_pb2.KmsEnvelopeAeadKey.FromString(key_data.value)
-    client = _kms_client_from_uri(env_key.params.kek_uri)
+    client = _kms_clients.kms_client_from_uri(env_key.params.kek_uri)
 
     return _kms_envelope_aead.KmsEnvelopeAead(
         env_key.params.dek_template,
         client.get_aead(key_uri=env_key.params.kek_uri),
     )
 
   def key_type(self) -> str:
```

### Comparing `tink-1.8.0/tink/aead/_kms_aead_key_manager_test.py` & `tink-1.9.0/tink/aead/_kms_aead_key_manager_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from tink.aead import _kms_aead_key_manager
 
 
 def setUpModule():
   aead.register()
 
 
-class FakeClient(_kms_aead_key_manager.KmsClient):
+class FakeClient(tink.KmsClient):
 
   def __init__(self, key_uri):
     self.key_uri = key_uri
 
   def does_support(self, key_uri: str) -> bool:
     return key_uri == self.key_uri
 
@@ -43,39 +43,17 @@
 KMS_ENVELOPE_AEAD_KEY_TYPE_URL = (
     'type.googleapis.com/google.crypto.tink.KmsEnvelopeAeadKey'
 )
 
 
 class KmsAeadKeyManagerTest(absltest.TestCase):
 
-  def test_register_get_and_reset_kms_clients(self):
-    client1 = FakeClient('key_uri1')
-    client2 = FakeClient('key_uri2')
-    client3 = FakeClient('key_uri3')
-    _kms_aead_key_manager.register_kms_client(client1)
-    _kms_aead_key_manager.register_kms_client(client2)
-    _kms_aead_key_manager.register_kms_client(client3)
-
-    # returns the first registered client that supports the uri.
-    self.assertEqual(
-        _kms_aead_key_manager._kms_client_from_uri('key_uri1'), client1
-    )
-    self.assertEqual(
-        _kms_aead_key_manager._kms_client_from_uri('key_uri2'), client2
-    )
-    with self.assertRaises(tink.TinkError):
-      _kms_aead_key_manager._kms_client_from_uri('unknown')
-
-    _kms_aead_key_manager.reset_kms_clients()
-    with self.assertRaises(tink.TinkError):
-      _kms_aead_key_manager._kms_client_from_uri('key_uri1')
-
   def test_kms_aead_new_key_data_success(self):
     client = FakeClient('key_uri')
-    _kms_aead_key_manager.register_kms_client(client)
+    tink.register_kms_client(client)
     template = aead.aead_key_templates.create_kms_aead_key_template(
         key_uri='key_uri'
     )
     key_data = _kms_aead_key_manager.KmsAeadKeyManager().new_key_data(template)
 
     self.assertEqual(key_data.type_url, KMS_AEAD_KEY_TYPE_URL)
     self.assertEqual(key_data.key_material_type, tink_pb2.KeyData.REMOTE)
```

### Comparing `tink-1.8.0/tink/aead/_kms_envelope_aead.py` & `tink-1.9.0/tink/aead/_kms_envelope_aead.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/aead/_kms_envelope_aead_test.py` & `tink-1.9.0/tink/aead/_kms_envelope_aead_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/BUILD.bazel` & `tink-1.9.0/tink/cc/BUILD.bazel`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/cc_hpke_config.cc` & `tink-1.9.0/tink/cc/cc_hpke_config.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/cc_hpke_config.h` & `tink-1.9.0/tink/cc/cc_hpke_config.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/cc_jwt_config.cc` & `tink-1.9.0/tink/cc/cc_jwt_config.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/cc_jwt_config.h` & `tink-1.9.0/tink/cc/cc_jwt_config.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/cc_key_manager.h` & `tink-1.9.0/tink/cc/cc_key_manager.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/cc_streaming_aead_wrappers.cc` & `tink-1.9.0/tink/cc/cc_streaming_aead_wrappers.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/cc_streaming_aead_wrappers.h` & `tink-1.9.0/tink/cc/cc_streaming_aead_wrappers.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/cc_streaming_aead_wrappers_test.cc` & `tink-1.9.0/tink/cc/cc_streaming_aead_wrappers_test.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/cc_tink_config.cc` & `tink-1.9.0/tink/cc/cc_tink_config.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/cc_tink_config.h` & `tink-1.9.0/tink/cc/cc_tink_config.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/input_stream_adapter.cc` & `tink-1.9.0/tink/cc/input_stream_adapter.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/input_stream_adapter.h` & `tink-1.9.0/tink/cc/input_stream_adapter.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/input_stream_adapter_test.cc` & `tink-1.9.0/tink/cc/input_stream_adapter_test.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/output_stream_adapter.cc` & `tink-1.9.0/tink/cc/output_stream_adapter.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/output_stream_adapter.h` & `tink-1.9.0/tink/cc/output_stream_adapter.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/output_stream_adapter_test.cc` & `tink-1.9.0/tink/cc/output_stream_adapter_test.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/BUILD.bazel` & `tink-1.9.0/tink/cc/pybind/BUILD.bazel`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/aead.cc` & `tink-1.9.0/tink/cc/pybind/aead.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/aead.h` & `tink-1.9.0/tink/cc/pybind/aead.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/cc_hpke_config.cc` & `tink-1.9.0/tink/cc/pybind/cc_hpke_config.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/cc_hpke_config.h` & `tink-1.9.0/tink/cc/pybind/cc_hpke_config.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/cc_jwt_config.cc` & `tink-1.9.0/tink/cc/pybind/cc_jwt_config.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/cc_jwt_config.h` & `tink-1.9.0/tink/cc/pybind/cc_jwt_config.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/cc_key_manager.cc` & `tink-1.9.0/tink/cc/pybind/cc_key_manager.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/cc_key_manager.h` & `tink-1.9.0/tink/cc/pybind/cc_key_manager.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/cc_key_manager_test.py` & `tink-1.9.0/tink/cc/pybind/cc_key_manager_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/cc_streaming_aead_wrappers.cc` & `tink-1.9.0/tink/cc/pybind/cc_streaming_aead_wrappers.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/cc_streaming_aead_wrappers.h` & `tink-1.9.0/tink/cc/pybind/cc_streaming_aead_wrappers.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/cc_tink_config.cc` & `tink-1.9.0/tink/cc/pybind/cc_tink_config.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/cc_tink_config.h` & `tink-1.9.0/tink/cc/pybind/cc_tink_config.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/cc_tink_config_test.py` & `tink-1.9.0/tink/cc/pybind/cc_tink_config_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/deterministic_aead.cc` & `tink-1.9.0/tink/cc/pybind/deterministic_aead.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/deterministic_aead.h` & `tink-1.9.0/tink/cc/pybind/deterministic_aead.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/hybrid_decrypt.cc` & `tink-1.9.0/tink/cc/pybind/hybrid_decrypt.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/hybrid_decrypt.h` & `tink-1.9.0/tink/cc/pybind/hybrid_decrypt.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/hybrid_encrypt.cc` & `tink-1.9.0/tink/cc/pybind/hybrid_encrypt.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/hybrid_encrypt.h` & `tink-1.9.0/tink/cc/pybind/hybrid_encrypt.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/import_helper.cc` & `tink-1.9.0/tink/cc/pybind/import_helper.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/import_helper.h` & `tink-1.9.0/tink/cc/pybind/import_helper.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/input_stream_adapter.cc` & `tink-1.9.0/tink/cc/pybind/input_stream_adapter.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/input_stream_adapter.h` & `tink-1.9.0/tink/cc/pybind/input_stream_adapter.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/mac.cc` & `tink-1.9.0/tink/cc/pybind/mac.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/mac.h` & `tink-1.9.0/tink/cc/pybind/mac.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/output_stream_adapter.cc` & `tink-1.9.0/tink/cc/pybind/output_stream_adapter.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/output_stream_adapter.h` & `tink-1.9.0/tink/cc/pybind/output_stream_adapter.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/prf.cc` & `tink-1.9.0/tink/cc/pybind/prf.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/prf.h` & `tink-1.9.0/tink/cc/pybind/prf.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/public_key_sign.cc` & `tink-1.9.0/tink/cc/pybind/public_key_sign.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/public_key_sign.h` & `tink-1.9.0/tink/cc/pybind/public_key_sign.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/public_key_verify.cc` & `tink-1.9.0/tink/cc/pybind/public_key_verify.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/public_key_verify.h` & `tink-1.9.0/tink/cc/pybind/public_key_verify.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/python_file_object_adapter.cc` & `tink-1.9.0/tink/cc/pybind/python_file_object_adapter.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/python_file_object_adapter.h` & `tink-1.9.0/tink/cc/pybind/python_file_object_adapter.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/streaming_aead.cc` & `tink-1.9.0/tink/cc/pybind/streaming_aead.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/streaming_aead.h` & `tink-1.9.0/tink/cc/pybind/streaming_aead.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/tink_bindings.cc` & `tink-1.9.0/tink/cc/pybind/tink_bindings.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/pybind/tink_exception.h` & `tink-1.9.0/tink/cc/pybind/tink_exception.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/python_file_object_adapter.h` & `tink-1.9.0/tink/cc/python_file_object_adapter.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/python_input_stream.cc` & `tink-1.9.0/tink/cc/python_input_stream.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/python_input_stream.h` & `tink-1.9.0/tink/cc/python_input_stream.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/python_input_stream_test.cc` & `tink-1.9.0/tink/cc/python_input_stream_test.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/python_output_stream.cc` & `tink-1.9.0/tink/cc/python_output_stream.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/python_output_stream.h` & `tink-1.9.0/tink/cc/python_output_stream.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/python_output_stream_test.cc` & `tink-1.9.0/tink/cc/python_output_stream_test.cc`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cc/test_util.h` & `tink-1.9.0/tink/cc/test_util.h`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cleartext_keyset_handle.py` & `tink-1.9.0/tink/cleartext_keyset_handle.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/cleartext_keyset_handle_test.py` & `tink-1.9.0/tink/cleartext_keyset_handle_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/core/BUILD.bazel` & `tink-1.9.0/tink/core/BUILD.bazel`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/core/__init__.py` & `tink-1.9.0/tink/core/__init__.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/core/_crypto_format.py` & `tink-1.9.0/tink/core/_crypto_format.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/core/_crypto_format_test.py` & `tink-1.9.0/tink/core/_crypto_format_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/core/_key_manager.py` & `tink-1.9.0/tink/core/_key_manager.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/core/_primitive_set.py` & `tink-1.9.0/tink/core/_primitive_set.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """A container class for a set of primitives."""
 
 import collections
-from typing import Generic, List, Type, TypeVar
+from typing import Generic, List, Type, TypeVar, Optional, Dict
 
 from tink.proto import tink_pb2
 from tink.core import _crypto_format
 from tink.core import _tink_error
 
 P = TypeVar('P')
 Entry = collections.namedtuple(
@@ -40,16 +40,16 @@
   Aead-primitives corresponding to the keys in the keyset, and uses the set
   members to do the actual crypto operations: to encrypt data the primary
   Aead-primitive from the set is used, and upon decryption the ciphertext's
   prefix determines the id of the primitive from the set.
   """
 
   def __init__(self, primitive_class: Type[P]):
-    self._primitives = {}  # Dict[bytes, List[Entry]]
-    self._primary = None
+    self._primitives: Dict[bytes, List[Entry]] = {}
+    self._primary: Optional[Entry] = None
     self._primitive_class = primitive_class
 
   def primitive_class(self) -> Type[P]:
     return self._primitive_class
 
   def primitive_from_identifier(self, identifier: bytes) -> List[Entry]:
     """Returns a copy of the list of entries for a given identifier."""
@@ -84,8 +84,10 @@
     entries.append(entry)
     return entry
 
   def set_primary(self, entry: Entry) -> None:
     self._primary = entry
 
   def primary(self) -> Entry:
+    if not self._primary:
+      raise _tink_error.TinkError('The primary entry is not set.')
     return self._primary
```

### Comparing `tink-1.8.0/tink/core/_primitive_set_test.py` & `tink-1.9.0/tink/core/_primitive_set_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,20 +95,21 @@
 
     entry = primitive_set.primary()
     self.assertEqual(primitive, entry.primitive)
     self.assertEqual(tink_pb2.ENABLED, entry.status)
     self.assertEqual(core.crypto_format.output_prefix(key), entry.identifier)
     self.assertEqual(1, entry.key_id)
 
-  def test_primary_returns_none(self):
+  def test_primary_not_set_primary_fails(self):
     primitive_set = core.new_primitive_set(mac.Mac)
     key = new_key(MAC_TEMPLATE, key_id=1)
     primitive = core.Registry.primitive(key.key_data, mac.Mac)
     primitive_set.add_primitive(primitive, key)
-    self.assertIsNone(primitive_set.primary())
+    with self.assertRaises(core.TinkError):
+      primitive_set.primary()
 
   def test_same_key_id_and_prefix_type(self):
     primitive_set = core.new_primitive_set(mac.Mac)
     key1 = new_key(MAC_TEMPLATE, key_id=1)
     primitive1 = core.Registry.primitive(key1.key_data, mac.Mac)
     primitive_set.add_primitive(primitive1, key1)
     key2 = new_key(MAC_TEMPLATE, key_id=1, status=tink_pb2.DISABLED)
```

### Comparing `tink-1.8.0/tink/core/_primitive_wrapper.py` & `tink-1.9.0/tink/core/_primitive_wrapper.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/core/_registry.py` & `tink-1.9.0/tink/core/_registry.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/core/_registry_test.py` & `tink-1.9.0/tink/core/_registry_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,18 +149,19 @@
     raise core.TinkError('Invalid Prf')
 
 
 class PrfToPrfWrapper(core.PrimitiveWrapper[prf.Prf, prf.Prf]):
   """A PrimitiveWrapper that wraps Prfs into a Prf."""
 
   def wrap(self, primitives_set: core.PrimitiveSet) -> prf.Prf:
-    if primitives_set.primary():
-      return primitives_set.primary().primitive
-    else:
+    # This is needed because register_primitive_wrapper calls wrap with
+    # an empty PrimitiveSet.
+    if not primitives_set.raw_primitives():
       return _InvalidPrf()
+    return primitives_set.primary().primitive
 
   def primitive_class(self) -> Type[prf.Prf]:
     return prf.Prf
 
   def input_primitive_class(self) -> Type[prf.Prf]:
     return prf.Prf
```

### Comparing `tink-1.8.0/tink/core/_tink_error.py` & `tink-1.9.0/tink/core/_tink_error.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/daead/BUILD.bazel` & `tink-1.9.0/tink/daead/BUILD.bazel`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,14 @@
 
 py_library(
     name = "_deterministic_aead_wrapper",
     srcs = ["_deterministic_aead_wrapper.py"],
     srcs_version = "PY3",
     deps = [
         ":_deterministic_aead",
-        requirement("absl-py"),
         "//tink/core",
     ],
 )
 
 py_test(
     name = "_deterministic_aead_wrapper_test",
     srcs = ["_deterministic_aead_wrapper_test.py"],
```

### Comparing `tink-1.8.0/tink/daead/__init__.py` & `tink-1.9.0/tink/daead/__init__.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/daead/_deterministic_aead.py` & `tink-1.9.0/tink/daead/_deterministic_aead.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/daead/_deterministic_aead_key_manager.py` & `tink-1.9.0/tink/daead/_deterministic_aead_key_manager.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/daead/_deterministic_aead_key_manager_test.py` & `tink-1.9.0/tink/daead/_deterministic_aead_key_manager_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/daead/_deterministic_aead_key_templates.py` & `tink-1.9.0/tink/daead/_deterministic_aead_key_templates.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/daead/_deterministic_aead_key_templates_test.py` & `tink-1.9.0/tink/daead/_deterministic_aead_key_templates_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/daead/_deterministic_aead_wrapper.py` & `tink-1.9.0/tink/daead/_deterministic_aead_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Deterministic AEAD wrapper."""
 
 from typing import Type
-from absl import logging
 
 from tink import core
 from tink.daead import _deterministic_aead
 
 
 class _WrappedDeterministicAead(_deterministic_aead.DeterministicAead):
   """Implements DeterministicAead for a set of DeterministicAead primitives."""
@@ -38,23 +37,22 @@
     if len(ciphertext) > core.crypto_format.NON_RAW_PREFIX_SIZE:
       prefix = ciphertext[:core.crypto_format.NON_RAW_PREFIX_SIZE]
       ciphertext_no_prefix = ciphertext[core.crypto_format.NON_RAW_PREFIX_SIZE:]
       for entry in self._primitive_set.primitive_from_identifier(prefix):
         try:
           return entry.primitive.decrypt_deterministically(ciphertext_no_prefix,
                                                            associated_data)
-        except core.TinkError as e:
-          logging.info(
-              'ciphertext prefix matches a key, but cannot decrypt: %s', e)
+        except core.TinkError:
+          pass
     # Let's try all RAW keys.
     for entry in self._primitive_set.raw_primitives():
       try:
         return entry.primitive.decrypt_deterministically(ciphertext,
                                                          associated_data)
-      except core.TinkError as e:
+      except core.TinkError:
         pass
     # nothing works.
     raise core.TinkError('Decryption failed.')
 
 
 class DeterministicAeadWrapper(
     core.PrimitiveWrapper[_deterministic_aead.DeterministicAead,
```

### Comparing `tink-1.8.0/tink/daead/_deterministic_aead_wrapper_test.py` & `tink-1.9.0/tink/daead/_deterministic_aead_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/hybrid/BUILD.bazel` & `tink-1.9.0/tink/hybrid/BUILD.bazel`

 * *Files 2% similar despite different names*

```diff
@@ -64,27 +64,26 @@
 py_library(
     name = "_hybrid_wrapper",
     srcs = ["_hybrid_wrapper.py"],
     srcs_version = "PY3",
     deps = [
         ":_hybrid_decrypt",
         ":_hybrid_encrypt",
-        requirement("absl-py"),
         "//tink/core",
     ],
 )
 
 py_test(
     name = "_hybrid_wrapper_test",
     srcs = ["_hybrid_wrapper_test.py"],
     srcs_version = "PY3",
     deps = [
         ":hybrid",
         requirement("absl-py"),
-        "//tink:cleartext_keyset_handle",
+        "//tink:secret_key_access",
         "//tink:tink_python",
         "//tink/proto:tink_py_pb2",
         "//tink/testing:keyset_builder",
     ],
 )
 
 py_library(
```

### Comparing `tink-1.8.0/tink/hybrid/__init__.py` & `tink-1.9.0/tink/hybrid/__init__.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/hybrid/_hybrid_decrypt.py` & `tink-1.9.0/tink/hybrid/_hybrid_decrypt.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/hybrid/_hybrid_encrypt.py` & `tink-1.9.0/tink/hybrid/_hybrid_encrypt.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/hybrid/_hybrid_key_manager.py` & `tink-1.9.0/tink/hybrid/_hybrid_key_manager.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/hybrid/_hybrid_key_manager_test.py` & `tink-1.9.0/tink/hybrid/_hybrid_key_manager_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/hybrid/_hybrid_key_templates.py` & `tink-1.9.0/tink/hybrid/_hybrid_key_templates.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/hybrid/_hybrid_key_templates_test.py` & `tink-1.9.0/tink/hybrid/_hybrid_key_templates_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/hybrid/_hybrid_wrapper.py` & `tink-1.9.0/tink/hybrid/_hybrid_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """HybridDecrypt wrapper."""
 
 from typing import Type
-from absl import logging
 
 from tink import core
 from tink.hybrid import _hybrid_decrypt
 from tink.hybrid import _hybrid_encrypt
 
 
 class _WrappedHybridDecrypt(_hybrid_decrypt.HybridDecrypt):
@@ -32,22 +31,21 @@
     if len(ciphertext) > core.crypto_format.NON_RAW_PREFIX_SIZE:
       prefix = ciphertext[:core.crypto_format.NON_RAW_PREFIX_SIZE]
       ciphertext_no_prefix = ciphertext[core.crypto_format.NON_RAW_PREFIX_SIZE:]
       for entry in self._primitive_set.primitive_from_identifier(prefix):
         try:
           return entry.primitive.decrypt(ciphertext_no_prefix,
                                          context_info)
-        except core.TinkError as e:
-          logging.info(
-              'ciphertext prefix matches a key, but cannot decrypt: %s', e)
+        except core.TinkError:
+          pass
     # Let's try all RAW keys.
     for entry in self._primitive_set.raw_primitives():
       try:
         return entry.primitive.decrypt(ciphertext, context_info)
-      except core.TinkError as e:
+      except core.TinkError:
         pass
     # nothing works.
     raise core.TinkError('Decryption failed.')
 
 
 class HybridDecryptWrapper(core.PrimitiveWrapper[_hybrid_decrypt.HybridDecrypt,
                                                  _hybrid_decrypt.HybridDecrypt]
```

### Comparing `tink-1.8.0/tink/hybrid/_hybrid_wrapper_test.py` & `tink-1.9.0/tink/hybrid/_hybrid_wrapper_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # limitations under the License.
 
 """Tests for tink.python.tink.aead_wrapper."""
 
 from absl.testing import absltest
 from absl.testing import parameterized
 import tink
-from tink import cleartext_keyset_handle
 from tink import core
 from tink import hybrid
+from tink import secret_key_access
 from tink.testing import keyset_builder
 
 
 TEMPLATE = hybrid.hybrid_key_templates.ECIES_P256_HKDF_HMAC_SHA256_AES128_GCM
 RAW_TEMPLATE = keyset_builder.raw_template(TEMPLATE)
 
 PRIVATE_KEYSET_WITH_PRIMARY = """
@@ -197,31 +197,39 @@
     with self.assertRaises(tink.TinkError):
       _ = dec1.decrypt(ciphertext4, b'context')
     self.assertEqual(dec2.decrypt(ciphertext4, b'context'), b'plaintext')
     self.assertEqual(dec3.decrypt(ciphertext4, b'context'), b'plaintext')
     self.assertEqual(dec4.decrypt(ciphertext4, b'context'), b'plaintext')
 
   def test_encrypt_decrypt_with_primary_key_succeeds(self):
-    private_handle_with_primary = cleartext_keyset_handle.read(
-        tink.JsonKeysetReader(PRIVATE_KEYSET_WITH_PRIMARY))
-    public_handle_with_primary = cleartext_keyset_handle.read(
-        tink.JsonKeysetReader(PUBLIC_KEYSET_WITH_PRIMARY))
+    private_handle_with_primary = tink.json_proto_keyset_format.parse(
+        PRIVATE_KEYSET_WITH_PRIMARY, secret_key_access.TOKEN
+    )
+    public_handle_with_primary = (
+        tink.json_proto_keyset_format.parse_without_secret(
+            PUBLIC_KEYSET_WITH_PRIMARY
+        )
+    )
     dec = private_handle_with_primary.primitive(hybrid.HybridDecrypt)
     enc = public_handle_with_primary.primitive(hybrid.HybridEncrypt)
     ciphertext = enc.encrypt(b'plaintext', b'context')
     self.assertEqual(dec.decrypt(ciphertext, b'context'), b'plaintext')
 
   def test_encrypt_decrypt_without_primary_key_fails(self):
     with self.assertRaises(tink.TinkError):
-      cleartext_keyset_handle.read(
-          tink.JsonKeysetReader(PRIVATE_KEYSET_WITHOUT_PRIMARY))
+      tink.json_proto_keyset_format.parse(
+          PRIVATE_KEYSET_WITHOUT_PRIMARY, secret_key_access.TOKEN
+      )
     # Currently, the public keyset only fails when 'encrypt' is called.
     # TODO(b/228140127): It would be preferable that it fails earlier.
-    public_handle_without_primary = cleartext_keyset_handle.read(
-        tink.JsonKeysetReader(PUBLIC_KEYSET_WITHOUT_PRIMARY))
+    public_handle_without_primary = (
+        tink.json_proto_keyset_format.parse_without_secret(
+            PUBLIC_KEYSET_WITHOUT_PRIMARY
+        )
+    )
     enc_without_primary = public_handle_without_primary.primitive(
         hybrid.HybridEncrypt)
     with self.assertRaises(tink.TinkError):
       enc_without_primary.encrypt(b'plaintext', b'context')
 
 
 if __name__ == '__main__':
```

### Comparing `tink-1.8.0/tink/integration/__init__.py` & `tink-1.9.0/tink/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/integration/awskms/BUILD.bazel` & `tink-1.9.0/tink/integration/awskms/BUILD.bazel`

 * *Files 6% similar despite different names*

```diff
@@ -16,34 +16,34 @@
 py_library(
     name = "_aws_kms_client",
     srcs = ["_aws_kms_client.py"],
     srcs_version = "PY3",
     deps = [
         "//tink:tink_python",
         "//tink/aead",
-        "//tink/aead:_kms_aead_key_manager",
         "//tink/core",
         requirement("boto3"),
     ],
 )
 
 py_test(
     name = "_aws_kms_client_test",
     srcs = ["_aws_kms_client_test.py"],
     data = [
         "//testdata/aws:bad_credentials",
         "//testdata/aws:credentials",
     ],
     srcs_version = "PY3",
     deps = [
-        ":awskms",
         ":_aws_kms_client",
+        ":awskms",
         "//tink:tink_python",
         "//tink/testing:helper",
         requirement("absl-py"),
+        requirement("boto3"),
     ],
 )
 
 py_test(
     name = "_aws_kms_integration_test",
     srcs = ["_aws_kms_integration_test.py"],
     data = [
@@ -53,12 +53,12 @@
     srcs_version = "PY3",
     # This test require valid AWS KMS credentials so we set it as `manual`.
     tags = ["manual"],
     deps = [
         ":awskms",
         "//tink:tink_python",
         "//tink/aead",
-        "//tink/aead:_kms_aead_key_manager",
         "//tink/testing:helper",
         requirement("absl-py"),
+        requirement("boto3"),
     ],
 )
```

### Comparing `tink-1.8.0/tink/integration/awskms/__init__.py` & `tink-1.9.0/tink/integration/awskms/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,13 +7,21 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 """AWS KMS integration package."""
 
-from tink.integration.awskms import _aws_kms_client
+try:
+  # pylint: disable=g-import-not-at-top
+  from tink.integration.awskms import _aws_kms_client
+except ImportError as import_error:
+  raise ImportError(
+      'Error importing the Tink AWS KMS module; did you forget to install the'
+      ' `tink[awskms]` extras?'
+  ) from import_error
 
 AwsKmsClient = _aws_kms_client.AwsKmsClient
+
+new_client = _aws_kms_client.new_client
```

### Comparing `tink-1.8.0/tink/integration/awskms/_aws_kms_client.py` & `tink-1.9.0/tink/integration/awskms/_aws_kms_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 import warnings
 
 import boto3
 from botocore import exceptions
 
 import tink
 from tink import aead
-from tink.aead import _kms_aead_key_manager
 
 
 AWS_KEYURI_PREFIX = 'aws-kms://'
 
 
 def _encryption_context(associated_data: bytes) -> Dict[str, str]:
   if associated_data:
@@ -64,20 +63,62 @@
           EncryptionContext=_encryption_context(associated_data),
       )
       return response['Plaintext']
     except exceptions.ClientError as e:
       raise tink.TinkError(e)
 
 
+def _has_aws_key_uri_format(key_uri: str) -> bool:
+  match = re.match('aws-kms://arn:aws:kms:([a-z0-9-]+):', key_uri)
+  return match is not None
+
+
 def _key_uri_to_key_arn(key_uri: str) -> str:
   if not key_uri.startswith(AWS_KEYURI_PREFIX):
     raise tink.TinkError('invalid key URI')
   return key_uri[len(AWS_KEYURI_PREFIX) :]
 
 
+class _KmsClient(tink.KmsClient):
+  """KMS client returned by new_client."""
+
+  def __init__(self, boto3_client: Any, key_uri: Optional[str]):
+    if not key_uri:
+      self._key_uri = None
+    else:
+      if not _has_aws_key_uri_format(key_uri):
+        raise tink.TinkError('invalid key URI')
+      self._key_uri = key_uri
+    self._boto3_client = boto3_client
+
+  def does_support(self, key_uri: str) -> bool:
+    if not _has_aws_key_uri_format(key_uri):
+      return False
+    if not self._key_uri:
+      return True
+    return key_uri == self._key_uri
+
+  def get_aead(self, key_uri: str) -> aead.Aead:
+    if not self.does_support(key_uri):
+      if self._key_uri:
+        raise tink.TinkError(
+            'This client is bound to %s and cannot use key %s' %
+            (self._key_uri, key_uri))
+      raise tink.TinkError(
+          'This client does not support key %s' % key_uri)
+    return _AwsKmsAead(self._boto3_client, _key_uri_to_key_arn(key_uri))
+
+
+def new_client(
+    *, boto3_client: Any, key_uri: Optional[str] = None
+) -> tink.KmsClient:
+  """Creates a new Tink KmsClient from a boto3 client."""
+  return _KmsClient(boto3_client, key_uri)
+
+
 def _parse_config(config_path: str) -> Tuple[str, str]:
   """Returns ('aws_access_key_id', 'aws_secret_access_key') from a config."""
   config = configparser.ConfigParser()
   config.read(config_path)
   if 'default' not in config:
     raise ValueError('invalid config: default not found')
   default = config['default']
@@ -95,15 +136,15 @@
   # arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab.
   key_arn_parts = key_arn.split(':')
   if len(key_arn_parts) < 6:
     raise tink.TinkError('invalid key id')
   return key_arn_parts[3]
 
 
-class AwsKmsClient(_kms_aead_key_manager.KmsClient):
+class AwsKmsClient(tink.KmsClient):
   """Basic AWS client for AEAD."""
 
   def __init__(self, key_uri: Optional[str], credentials_path: Optional[str]):
     """Creates a new AwsKmsClient that is bound to the key specified in 'key_uri'.
 
     For more information on credentials and in which order they are loaded see
     https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html.
@@ -115,20 +156,19 @@
           None or empty, then default credentials will be used.
 
     Raises:
       ValueError: If the path or filename of the credentials is invalid.
       TinkError: If the key uri is not valid.
     """
     if not key_uri:
-      self._key_arn = None
+      self._key_uri = None
     else:
-      match = re.match('aws-kms://arn:aws:kms:([a-z0-9-]+):', key_uri)
-      if not match:
+      if not _has_aws_key_uri_format(key_uri):
         raise tink.TinkError('invalid key URI')
-      self._key_arn = _key_uri_to_key_arn(key_uri)
+      self._key_uri = key_uri
     if not credentials_path:
       self._aws_access_key_id = None
       self._aws_secret_access_key = None
     else:
       aws_access_key_id, aws_secret_access_key = _parse_config(credentials_path)
       self._aws_access_key_id = aws_access_key_id
       self._aws_secret_access_key = aws_secret_access_key
@@ -138,37 +178,37 @@
 
     Args:
       key_uri: Text, URI of the key to be checked.
 
     Returns: A boolean value which is true if the key is supported and false
       otherwise.
     """
-    if not key_uri.startswith(AWS_KEYURI_PREFIX):
+    if not _has_aws_key_uri_format(key_uri):
       return False
-    if not self._key_arn:
+    if not self._key_uri:
       return True
-    return _key_uri_to_key_arn(key_uri) == self._key_arn
+    return key_uri == self._key_uri
 
   def get_aead(self, key_uri: str) -> aead.Aead:
     """Returns an Aead-primitive backed by KMS key specified by 'key_uri'.
 
     Args:
       key_uri: Text, URI of the key which should be used.
 
     Returns:
       An AEAD primitive which uses the specified key.
 
     Raises:
       TinkError: If the key_uri is not supported.
     """
     if not self.does_support(key_uri):
-      if self._key_arn:
+      if self._key_uri:
         raise tink.TinkError(
             'This client is bound to %s and cannot use key %s' %
-            (self._key_arn, key_uri))
+            (self._key_uri, key_uri))
       raise tink.TinkError(
           'This client does not support key %s' % key_uri)
     key_arn = _key_uri_to_key_arn(key_uri)
     session = boto3.session.Session(
         aws_access_key_id=self._aws_access_key_id,
         aws_secret_access_key=self._aws_secret_access_key,
         region_name=_get_region_from_key_arn(key_arn),
@@ -186,10 +226,8 @@
   ) -> None:
     """Registers the KMS client internally."""
     warnings.warn(
         'The "awskms.AwsKmsClient.register_client" function is deprecated.',
         DeprecationWarning,
         2,
     )
-    _kms_aead_key_manager.register_kms_client(  # pylint: disable=protected-access
-        AwsKmsClient(key_uri, credentials_path)
-    )
+    tink.register_kms_client(AwsKmsClient(key_uri, credentials_path))
```

### Comparing `tink-1.8.0/tink/integration/awskms/_aws_kms_integration_test.py` & `tink-1.9.0/tink/integration/awskms/_aws_kms_integration_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink.integration.aws_kms_aead."""
 
 import os
 
 from absl.testing import absltest
+import boto3
 import botocore
 
 import tink
+from tink import _kms_clients
 from tink import aead
-from tink.aead import _kms_aead_key_manager
 from tink.integration import awskms
 from tink.integration.awskms import _aws_kms_client
 from tink.testing import helper
 
 
 CREDENTIAL_PATH = os.path.join(helper.tink_py_testdata_path(),
                                'aws/credentials.ini')
@@ -50,15 +51,15 @@
   aead.register()
 
 
 class AwsKmsAeadTest(absltest.TestCase):
 
   def tearDown(self):
     super().tearDown()
-    _kms_aead_key_manager.reset_kms_clients()
+    _kms_clients.reset_kms_clients()
 
   def test_encrypt_decrypt(self):
     aws_client = awskms.AwsKmsClient(KEY_URI, CREDENTIAL_PATH)
     aws_aead = aws_client.get_aead(KEY_URI)
 
     plaintext = b'hello'
     associated_data = b'world'
@@ -109,14 +110,43 @@
     aws_aead = aws_client.get_aead(KEY_URI)
 
     plaintext = b'hello'
     associated_data = b'world'
     with self.assertRaises(tink.TinkError):
       aws_aead.encrypt(plaintext, associated_data)
 
+  def test_new_client_get_aead(self):
+    aws_access_key_id, aws_secret_access_key = _aws_kms_client._parse_config(
+        CREDENTIAL_PATH
+    )
+    boto3_client = boto3.client(
+        aws_access_key_id=aws_access_key_id,
+        aws_secret_access_key=aws_secret_access_key,
+        region_name='us-east-2',
+        service_name='kms',
+    )
+
+    aws_client = awskms.new_client(boto3_client=boto3_client)
+
+    aws_aead = aws_client.get_aead(KEY_URI)
+    ciphertext = aws_aead.encrypt(b'plaintext', b'associated_data')
+    self.assertEqual(
+        b'plaintext', aws_aead.decrypt(ciphertext, b'associated_data')
+    )
+
+    aws_aead_with_alias = aws_client.get_aead(KEY_ALIAS_URI)
+    ciphertext = aws_aead_with_alias.encrypt(b'plaintext', b'associated_data')
+    self.assertEqual(
+        b'plaintext',
+        aws_aead_with_alias.decrypt(ciphertext, b'associated_data'),
+    )
+
+    with self.assertRaises(tink.TinkError):
+      aws_client.get_aead(GCP_KEY_URI)
+
   def test_client_registration(self):
     # Register AWS KMS Client bound to KEY_URI.
     awskms.AwsKmsClient.register_client(KEY_URI, CREDENTIAL_PATH)
 
     # Create a keyset handle for KEY_URI and use it.
     handle = tink.new_keyset_handle(
         aead.aead_key_templates.create_kms_aead_key_template(KEY_URI)
@@ -161,14 +191,31 @@
     aws_aead = aws_client.get_aead(KEY_URI)
 
     ciphertext = aws_aead.encrypt(b'plaintext', b'associated_data')
     self.assertEqual(
         b'plaintext', aws_aead.decrypt(ciphertext, b'associated_data')
     )
 
+    # creates a boto3 client using default credentials
+    boto3_client = boto3.client(region_name='us-east-2', service_name='kms')
+    aws_client2 = awskms.new_client(boto3_client=boto3_client, key_uri=KEY_URI)
+    aws_aead2 = aws_client2.get_aead(KEY_URI)
+    ciphertext2 = aws_aead2.encrypt(b'plaintext', b'associated_data')
+    self.assertEqual(
+        b'plaintext', aws_aead2.decrypt(ciphertext2, b'associated_data')
+    )
+
+    # check that aws_aead and aws_aead2 are compatible
+    self.assertEqual(
+        b'plaintext', aws_aead2.decrypt(ciphertext, b'associated_data')
+    )
+    self.assertEqual(
+        b'plaintext', aws_aead.decrypt(ciphertext2, b'associated_data')
+    )
+
   def test_server_side_key_commitment(self):
     # TODO(b/242678738): Remove direct usage of KMS client and protected
     # functions in this test once client side key ID verifiaction is removed.
 
     plaintext = b'hello'
     associated_data = b'world'
     encryption_context = _aws_kms_client._encryption_context(associated_data)
@@ -210,15 +257,15 @@
           CiphertextBlob=ciphertext,
           EncryptionContext=encryption_context,
       )
       self.assertEqual(plaintext, response['Plaintext'])
 
       # Attempt to decrypt with KEY_URI_2.
       with self.assertRaises(botocore.exceptions.ClientError):
-        response = aws_aead.client.decrypt(
+        aws_aead.client.decrypt(
             KeyId=_aws_kms_client._key_uri_to_key_arn(KEY_URI_2),
             CiphertextBlob=ciphertext,
             EncryptionContext=encryption_context,
         )
 
 
 if __name__ == '__main__':
```

### Comparing `tink-1.8.0/tink/integration/gcpkms/BUILD.bazel` & `tink-1.9.0/tink/integration/gcpkms/BUILD.bazel`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 py_library(
     name = "_gcp_kms_client",
     srcs = ["_gcp_kms_client.py"],
     srcs_version = "PY3",
     deps = [
         "//tink:tink_python",
         "//tink/aead",
-        "//tink/aead:_kms_aead_key_manager",
         requirement("google-auth"),
         requirement("google-api-core"),
         requirement("google-cloud-kms"),
     ],
 )
 
 py_test(
@@ -64,15 +63,15 @@
         "//testdata/gcp:credentials",
         "@google_root_pem//file",
     ],
     srcs_version = "PY3",
     tags = ["manual"],
     deps = [
         ":gcpkms",
-        "//tink:cleartext_keyset_handle",
+        "//tink:secret_key_access",
         "//tink:tink_python",
         "//tink/aead",
         "//tink/aead:_kms_aead_key_manager",
         "//tink/testing:helper",
         requirement("absl-py"),
     ],
 )
```

### Comparing `tink-1.8.0/tink/integration/gcpkms/__init__.py` & `tink-1.9.0/tink/mac/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-# Copyright 2019 Google LLC
+# Copyright 2020 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""Mac package."""
 
-"""GCP KMS package."""
+from tink.mac import _mac
+from tink.mac import _mac_key_manager
+from tink.mac import _mac_key_templates as mac_key_templates
 
-from tink.integration.gcpkms import _gcp_kms_client
 
-GcpKmsClient = _gcp_kms_client.GcpKmsClient
+Mac = _mac.Mac
+register = _mac_key_manager.register
```

### Comparing `tink-1.8.0/tink/integration/gcpkms/_gcp_kms_client.py` & `tink-1.9.0/tink/integration/gcpkms/_gcp_kms_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 from google.api_core import exceptions as core_exceptions
 from google.cloud import kms_v1
 from google.oauth2 import service_account
 
 import tink
 from tink import aead
-from tink.aead import _kms_aead_key_manager
 
 GCP_KEYURI_PREFIX = 'gcp-kms://'
 
 
 class _GcpKmsAead(aead.Aead):
   """Implements the Aead interface for GCP KMS."""
 
@@ -59,15 +58,15 @@
          )
       )
       return response.plaintext
     except core_exceptions.GoogleAPIError as e:
       raise tink.TinkError(e)
 
 
-class GcpKmsClient(_kms_aead_key_manager.KmsClient):
+class GcpKmsClient(tink.KmsClient):
   """Basic GCP client for AEAD."""
 
   def __init__(
       self, key_uri: Optional[str], credentials_path: Optional[str]
   ) -> None:
     """Creates a new GcpKmsClient that is bound to the key specified in 'key_uri'.
 
@@ -143,10 +142,8 @@
   ) -> None:
     """Registers the KMS client internally."""
     warnings.warn(
         'The "gcpkms.GcpKmsClient.register_client" function is deprecated.',
         DeprecationWarning,
         2,
     )
-    _kms_aead_key_manager.register_kms_client(  # pylint: disable=protected-access
-        GcpKmsClient(key_uri, credentials_path)
-    )
+    tink.register_kms_client(GcpKmsClient(key_uri, credentials_path))
```

### Comparing `tink-1.8.0/tink/integration/gcpkms/_gcp_kms_client_integration_test.py` & `tink-1.9.0/tink/integration/gcpkms/_gcp_kms_client_integration_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/integration/gcpkms/_gcp_kms_client_test.py` & `tink-1.9.0/tink/integration/gcpkms/_gcp_kms_client_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/integration/gcpkms/_gcp_kms_integration_test.py` & `tink-1.9.0/tink/integration/gcpkms/_gcp_kms_integration_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 
 import base64
 import os
 
 from absl.testing import absltest
 
 import tink
+from tink import _kms_clients
 from tink import aead
-from tink import cleartext_keyset_handle
-from tink.aead import _kms_aead_key_manager
+from tink import secret_key_access
 from tink.integration import gcpkms
 from tink.testing import helper
 
 CREDENTIAL_PATH = os.path.join(
     helper.tink_py_testdata_path(), 'gcp/credential.json'
 )
 BAD_CREDENTIAL_PATH = os.path.join(
@@ -52,15 +52,15 @@
   def setUp(self):
     super().setUp()
     # Make sure default credentials are not set.
     os.environ['GOOGLE_APPLICATION_CREDENTIALS'] = ''
 
   def tearDown(self):
     super().tearDown()
-    _kms_aead_key_manager.reset_kms_clients()
+    _kms_clients.reset_kms_clients()
 
   def test_aead_from_keyset_handle_for_key_uri_works(self):
     # Register client not bound to a key URI.
     gcpkms.GcpKmsClient.register_client('', CREDENTIAL_PATH)
 
     handle = tink.new_keyset_handle(
         aead.aead_key_templates.create_kms_aead_key_template(KEY_URI)
@@ -190,16 +190,17 @@
         'AcpCNBevmQnr9momhlKKEyKDOCj5bMfizqC22N/hLZd58LFpC+r99C0='
     )
 
     key_uri = 'gcp-kms://projects/tink-test-infrastructure/locations/us/keyRings/big-query-test-key/cryptoKeys/aead-key'
     gcp_aead = gcpkms.GcpKmsClient('', CREDENTIAL_PATH).get_aead(key_uri)
 
     unwrapped_keyset = gcp_aead.decrypt(wrapped_keyset, b'')
-    keyset_handle = cleartext_keyset_handle.read(
-        tink.BinaryKeysetReader(unwrapped_keyset))
+    keyset_handle = tink.proto_keyset_format.parse(
+        unwrapped_keyset, secret_key_access.TOKEN
+    )
     primitive = keyset_handle.primitive(aead.Aead)
     decrypted = primitive.decrypt(ciphertext, b'animal')
     self.assertEqual(decrypted, b'elephant')
 
   def test_registration_client_bound_to_uri_works(self):
     # Register client bound to KEY_URI.
     gcpkms.GcpKmsClient.register_client(KEY_URI, CREDENTIAL_PATH)
```

### Comparing `tink-1.8.0/tink/internal/__init__.py` & `tink-1.9.0/tink/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/internal/big_integer_util.py` & `tink-1.9.0/tink/internal/big_integer_util.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/internal/big_integer_util_test.py` & `tink-1.9.0/tink/internal/big_integer_util_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/jwt/BUILD.bazel` & `tink-1.9.0/tink/jwt/BUILD.bazel`

 * *Files 2% similar despite different names*

```diff
@@ -252,15 +252,15 @@
     deps = [
         ":_json_util",
         ":_jwt_format",
         ":jwt",
         "//tink/proto:jwt_hmac_py_pb2",
         "//tink/proto:tink_py_pb2",
         requirement("absl-py"),
-        "//tink:cleartext_keyset_handle",
+        "//tink:secret_key_access",
         "//tink:tink_python",
         "//tink/testing:keyset_builder",
     ],
 )
 
 py_library(
     name = "_jwt_signature_key_manager",
@@ -324,15 +324,15 @@
         ":_jwt_format",
         ":jwt",
         "//tink/proto:jwt_ecdsa_py_pb2",
         "//tink/proto:jwt_rsa_ssa_pkcs1_py_pb2",
         "//tink/proto:jwt_rsa_ssa_pss_py_pb2",
         "//tink/proto:tink_py_pb2",
         requirement("absl-py"),
-        "//tink:cleartext_keyset_handle",
+        "//tink:secret_key_access",
         "//tink:tink_python",
         "//tink/testing:keyset_builder",
     ],
 )
 
 py_library(
     name = "_jwk_set_converter",
@@ -352,11 +352,11 @@
     name = "_jwk_set_converter_test",
     srcs = ["_jwk_set_converter_test.py"],
     python_version = "PY3",
     srcs_version = "PY3",
     deps = [
         ":jwt",
         requirement("absl-py"),
-        "//tink:cleartext_keyset_handle",
+        "//tink:secret_key_access",
         "//tink:tink_python",
     ],
 )
```

### Comparing `tink-1.8.0/tink/jwt/__init__.py` & `tink-1.9.0/tink/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/jwt/_json_util.py` & `tink-1.9.0/tink/jwt/_json_util.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/jwt/_json_util_test.py` & `tink-1.9.0/tink/jwt/_json_util_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/jwt/_jwk_set_converter.py` & `tink-1.9.0/tink/jwt/_jwk_set_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,26 +9,25 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Convert Tink Keyset with JWT keys from and to JWK sets."""
 
-import io
 import json
 import random
 
-from typing import Dict, List, Optional, Union
+from typing import cast, Dict, List, Optional, Union
 
 from tink.proto import jwt_ecdsa_pb2
 from tink.proto import jwt_rsa_ssa_pkcs1_pb2
 from tink.proto import jwt_rsa_ssa_pss_pb2
 from tink.proto import tink_pb2
 import tink
-from tink import cleartext_keyset_handle
+from tink import secret_key_access
 from tink.jwt import _jwt_format
 
 _JWT_ECDSA_PUBLIC_KEY_TYPE = (
     'type.googleapis.com/google.crypto.tink.JwtEcdsaPublicKey')
 _JWT_RSA_SSA_PKCS1_PUBLIC_KEY_TYPE = (
     'type.googleapis.com/google.crypto.tink.JwtRsaSsaPkcs1PublicKey')
 _JWT_RSA_SSA_PSS_PUBLIC_KEY_TYPE = (
@@ -94,19 +93,18 @@
   Returns:
     A JWK set, which is a JSON encoded string.
 
   Raises:
     TinkError if the keys are not of the expected type, or if they have a
     ouput prefix type that is not supported.
   """
-  output_stream = io.BytesIO()
-  writer = tink.BinaryKeysetWriter(output_stream)
-  keyset_handle.write_no_secret(writer)
-  keyset = tink_pb2.Keyset.FromString(output_stream.getvalue())
-
+  serialization = tink.proto_keyset_format.serialize_without_secret(
+      keyset_handle
+  )
+  keyset = tink_pb2.Keyset.FromString(serialization)
   keys = []
   for key in keyset.key:
     if key.status != tink_pb2.ENABLED:
       continue
     if key.key_data.key_material_type != tink_pb2.KeyData.ASYMMETRIC_PUBLIC:
       raise tink.TinkError('wrong key material type')
     if key.output_prefix_type not in [tink_pb2.RAW, tink_pb2.TINK]:
@@ -250,15 +248,16 @@
     new_id = _generate_unused_key_id(proto_keyset)
     proto_key.key_id = new_id
     proto_keyset.key.append(proto_key)
     # JWK sets do not really have a primary key (see RFC 7517, Section 5.1).
     # To verify signature, it also does not matter which key is primary. We
     # simply set it to the last key.
     proto_keyset.primary_key_id = new_id
-  return cleartext_keyset_handle.from_keyset(proto_keyset)
+  return tink.proto_keyset_format.parse(
+      proto_keyset.SerializeToString(), secret_key_access.TOKEN)
 
 
 # Deprecated. Use to_public_keyset_handle instead.
 def to_keyset_handle(
     jwk_set: str,
     key_access: Optional[tink.KeyAccess] = None) -> tink.KeysetHandle:
   _ = key_access
@@ -275,28 +274,28 @@
     raise tink.TinkError('invalid use')
 
 
 def _convert_to_ecdsa_key(
     key: Dict[str, Union[str, List[str]]]) -> tink_pb2.Keyset.Key:
   """Converts a EC Json Web Key (JWK) into a tink_pb2.Keyset.Key."""
   ecdsa_public_key = jwt_ecdsa_pb2.JwtEcdsaPublicKey()
-  algorithm = _ECDSA_NAME_TO_ALGORITHM.get(key['alg'], None)
+  algorithm = _ECDSA_NAME_TO_ALGORITHM.get(cast(str, key['alg']), None)
   if not algorithm:
     raise tink.TinkError('unknown ECDSA algorithm')
   if key.get('kty', None) != 'EC':
     raise tink.TinkError('invalid kty')
   _, crv = _ECDSA_PARAMS[algorithm]
   if key.get('crv', None) != crv:
     raise tink.TinkError('invalid crv')
   _validate_use_and_key_ops(key)
   if 'd' in key:
     raise tink.TinkError('cannot convert private ECDSA key')
   ecdsa_public_key.algorithm = algorithm
-  ecdsa_public_key.x = _base64_decode(key['x'])
-  ecdsa_public_key.y = _base64_decode(key['y'])
+  ecdsa_public_key.x = _base64_decode(cast(str, key['x']))
+  ecdsa_public_key.y = _base64_decode(cast(str, key['y']))
   if 'kid' in key:
     ecdsa_public_key.custom_kid.value = key['kid']
   proto_key = tink_pb2.Keyset.Key()
   proto_key.key_data.type_url = _JWT_ECDSA_PUBLIC_KEY_TYPE
   proto_key.key_data.value = ecdsa_public_key.SerializeToString()
   proto_key.key_data.key_material_type = tink_pb2.KeyData.ASYMMETRIC_PUBLIC
   proto_key.output_prefix_type = tink_pb2.RAW
@@ -304,26 +303,26 @@
   return proto_key
 
 
 def _convert_to_rsa_ssa_pkcs1_key(
     key: Dict[str, Union[str, List[str]]]) -> tink_pb2.Keyset.Key:
   """Converts a JWK into a JwtEcdsaPublicKey."""
   public_key = jwt_rsa_ssa_pkcs1_pb2.JwtRsaSsaPkcs1PublicKey()
-  algorithm = _RSA_SSA_PKCS1_NAME_TO_ALGORITHM.get(key['alg'], None)
+  algorithm = _RSA_SSA_PKCS1_NAME_TO_ALGORITHM.get(cast(str, key['alg']), None)
   if not algorithm:
     raise tink.TinkError('unknown RSA SSA PKCS1 algorithm')
   if key.get('kty', None) != 'RSA':
     raise tink.TinkError('invalid kty')
   _validate_use_and_key_ops(key)
   if ('p' in key or 'q' in key or 'dp' in key or 'dq' in key or 'd' in key or
       'qi' in key):
     raise tink.TinkError('importing RSA private keys is not implemented')
   public_key.algorithm = algorithm
-  public_key.n = _base64_decode(key['n'])
-  public_key.e = _base64_decode(key['e'])
+  public_key.n = _base64_decode(cast(str, key['n']))
+  public_key.e = _base64_decode(cast(str, key['e']))
   if 'kid' in key:
     public_key.custom_kid.value = key['kid']
   proto_key = tink_pb2.Keyset.Key()
   proto_key.key_data.type_url = _JWT_RSA_SSA_PKCS1_PUBLIC_KEY_TYPE
   proto_key.key_data.value = public_key.SerializeToString()
   proto_key.key_data.key_material_type = tink_pb2.KeyData.ASYMMETRIC_PUBLIC
   proto_key.output_prefix_type = tink_pb2.RAW
@@ -331,28 +330,28 @@
   return proto_key
 
 
 def _convert_to_rsa_ssa_pss_key(
     key: Dict[str, Union[str, List[str]]]) -> tink_pb2.Keyset.Key:
   """Converts a JWK into a JwtEcdsaPublicKey."""
   public_key = jwt_rsa_ssa_pss_pb2.JwtRsaSsaPssPublicKey()
-  algorithm = _RSA_SSA_PSS_NAME_TO_ALGORITHM.get(key['alg'], None)
+  algorithm = _RSA_SSA_PSS_NAME_TO_ALGORITHM.get(cast(str, key['alg']), None)
   if not algorithm:
     raise tink.TinkError('unknown RSA SSA PSS algorithm')
   if key.get('kty', None) != 'RSA':
     raise tink.TinkError('invalid kty')
   _validate_use_and_key_ops(key)
   if ('p' in key or 'q' in key or 'dp' in key or 'dq' in key or 'd' in key or
       'qi' in key):
     raise tink.TinkError('importing RSA private keys is not implemented')
   public_key.algorithm = algorithm
-  public_key.n = _base64_decode(key['n'])
-  public_key.e = _base64_decode(key['e'])
+  public_key.n = _base64_decode(cast(str, key['n']))
+  public_key.e = _base64_decode(cast(str, key['e']))
   if 'kid' in key:
-    public_key.custom_kid.value = key['kid']
+    public_key.custom_kid.value = cast(str, key['kid'])
   proto_key = tink_pb2.Keyset.Key()
   proto_key.key_data.type_url = _JWT_RSA_SSA_PSS_PUBLIC_KEY_TYPE
   proto_key.key_data.value = public_key.SerializeToString()
   proto_key.key_data.key_material_type = tink_pb2.KeyData.ASYMMETRIC_PUBLIC
   proto_key.output_prefix_type = tink_pb2.RAW
   proto_key.status = tink_pb2.ENABLED
   return proto_key
```

### Comparing `tink-1.8.0/tink/jwt/_jwk_set_converter_test.py` & `tink-1.9.0/tink/jwt/_jwk_set_converter_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 """Tests for tink.python.tink.jwt._jwk_set_converter."""
 
 from absl.testing import absltest
 from absl.testing import parameterized
 
 from tink.proto import tink_pb2
 import tink
-from tink import cleartext_keyset_handle
 from tink import jwt
+from tink import secret_key_access
 
 ES256_KEYSET = (
     '{"primaryKeyId":282600252,"key":[{"keyData":{'
     '"typeUrl":"type.googleapis.com/google.crypto.tink.JwtEcdsaPublicKey",'
     '"value":"EAEaIBDPI66hjLHvjxmUJ2nyHIBDmdOtQ4gPsvWgYYgZ0gygIiBTEK0rTACpAb97m'
     '+mvtJKAk0q3mHjPcUZm0C4EueDW4Q==",'
     '"keyMaterialType":"ASYMMETRIC_PUBLIC"'
@@ -385,16 +385,17 @@
       ('PS256_RAW', PS256_KEYSET, PS256_JWK_SET),
       ('PS384_RAW', PS384_KEYSET, PS384_JWK_SET),
       ('PS512_RAW', PS512_KEYSET, PS512_JWK_SET),
       ('PS256_TINK', PS256_KEYSET_TINK, PS256_JWK_SET_KID),
       ('TWO_KEYS', KEYSET_WITH_TWO_KEYS, JWK_SET_WITH_TWO_KEYS)
   ])
   def test_convert_from_jwt_key(self, tink_keyset, expected_jwk_set):
-    reader = tink.JsonKeysetReader(tink_keyset)
-    keyset_handle = cleartext_keyset_handle.read(reader)
+    keyset_handle = tink.json_proto_keyset_format.parse_without_secret(
+        tink_keyset
+    )
     jwk_set = jwt.jwk_set_from_public_keyset_handle(keyset_handle)
     self.assertEqual(jwk_set, expected_jwk_set)
 
   @parameterized.named_parameters([('ES256_RAW', ES256_JWK_SET),
                                    ('ES384_RAW', ES384_JWK_SET),
                                    ('ES512_RAW', ES512_JWK_SET),
                                    ('ES256_TINK', ES256_JWK_SET_KID),
@@ -423,52 +424,55 @@
     jwk_set_with_empty_kid = ES256_JWK_SET_KID.replace('"ENgjPA"', '""')
     keyset_handle = jwt.jwk_set_to_public_keyset_handle(jwk_set_with_empty_kid)
     output_jwk_set = jwt.jwk_set_from_public_keyset_handle(keyset_handle)
     self.assertEqual(output_jwk_set, jwk_set_with_empty_kid)
 
   def test_primary_key_id_missing_success(self):
     keyset = ES256_KEYSET.replace('"primaryKeyId":282600252,', '')
-    reader = tink.JsonKeysetReader(keyset)
-    keyset_handle = cleartext_keyset_handle.read(reader)
+    keyset_handle = tink.json_proto_keyset_format.parse_without_secret(keyset)
     jwk_set = jwt.jwk_set_from_public_keyset_handle(keyset_handle)
     self.assertEqual(jwk_set, ES256_JWK_SET)
 
   @parameterized.named_parameters([
       ('ES256_RAW', ES256_KEYSET),
       ('RS256_RAW', RS256_KEYSET),
       ('PS256_RAW', PS256_KEYSET)
   ])
   def test_from_legacy_ecdsa_keyset_fails(self, keyset):
     legacy_keyset = keyset.replace('RAW', 'LEGACY')
-    reader = tink.JsonKeysetReader(legacy_keyset)
-    keyset_handle = cleartext_keyset_handle.read(reader)
+    keyset_handle = tink.json_proto_keyset_format.parse_without_secret(
+        legacy_keyset
+    )
     with self.assertRaises(tink.TinkError):
       jwt.jwk_set_from_public_keyset_handle(keyset_handle)
 
   @parameterized.named_parameters([
       ('ES256_RAW', ES256_KEYSET),
       ('RS256_RAW', RS256_KEYSET),
       ('PS256_RAW', RS256_KEYSET)
   ])
   def test_from_crunchy_ecdsa_keyset_fails(self, keyset):
     crunchy_keyset = keyset.replace('RAW', 'CRUNCHY')
-    reader = tink.JsonKeysetReader(crunchy_keyset)
-    keyset_handle = cleartext_keyset_handle.read(reader)
+    keyset_handle = tink.json_proto_keyset_format.parse_without_secret(
+        crunchy_keyset
+    )
     with self.assertRaises(tink.TinkError):
       jwt.jwk_set_from_public_keyset_handle(keyset_handle)
 
   def test_from_hs256_keyset_fails(self):
-    reader = tink.JsonKeysetReader(HS256_KEYSET)
-    keyset_handle = cleartext_keyset_handle.read(reader)
+    keyset_handle = tink.json_proto_keyset_format.parse(
+        HS256_KEYSET, secret_key_access.TOKEN
+    )
     with self.assertRaises(tink.TinkError):
       jwt.jwk_set_from_public_keyset_handle(keyset_handle)
 
   def test_from_private_keyset_fails(self):
-    reader = tink.JsonKeysetReader(PRIVATEKEY_KEYSET)
-    keyset_handle = cleartext_keyset_handle.read(reader)
+    keyset_handle = tink.json_proto_keyset_format.parse(
+        PRIVATEKEY_KEYSET, secret_key_access.TOKEN
+    )
     with self.assertRaises(tink.TinkError):
       jwt.jwk_set_from_public_keyset_handle(keyset_handle)
 
   def test_ecdsa_without_use_or_key_ops_to_public_keyset_handle_success(self):
     jwk_set = """{"keys":[
         {
            "kty":"EC",
```

### Comparing `tink-1.8.0/tink/jwt/_jwt_error.py` & `tink-1.9.0/tink/jwt/_jwt_error.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/jwt/_jwt_format.py` & `tink-1.9.0/tink/jwt/_jwt_format.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/jwt/_jwt_format_test.py` & `tink-1.9.0/tink/jwt/_jwt_format_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/jwt/_jwt_hmac_key_manager.py` & `tink-1.9.0/tink/jwt/_jwt_hmac_key_manager.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/jwt/_jwt_hmac_key_manager_test.py` & `tink-1.9.0/tink/jwt/_jwt_hmac_key_manager_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/jwt/_jwt_key_templates.py` & `tink-1.9.0/tink/jwt/_jwt_key_templates.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/jwt/_jwt_key_templates_test.py` & `tink-1.9.0/tink/jwt/_jwt_key_templates_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/jwt/_jwt_mac.py` & `tink-1.9.0/tink/jwt/_jwt_mac.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/jwt/_jwt_mac_wrapper.py` & `tink-1.9.0/tink/jwt/_jwt_mac_wrapper.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/jwt/_jwt_mac_wrapper_test.py` & `tink-1.9.0/tink/jwt/_jwt_mac_wrapper_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,69 +9,72 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink.jwt._jwt_mac_wrapper."""
 
-import io
-
 from absl.testing import absltest
 from absl.testing import parameterized
 
-
 from tink.proto import jwt_hmac_pb2
 from tink.proto import tink_pb2
 import tink
-from tink import cleartext_keyset_handle
 from tink import jwt
+from tink import secret_key_access
 from tink.jwt import _json_util
 from tink.jwt import _jwt_format
 from tink.testing import keyset_builder
 
 
 def setUpModule():
   jwt.register_jwt_mac()
 
 
 def _set_custom_kid(keyset_handle: tink.KeysetHandle,
                     custom_kid: str) -> tink.KeysetHandle:
   """Set the custom_kid field of the first key."""
-  buffer = io.BytesIO()
-  cleartext_keyset_handle.write(
-      tink.BinaryKeysetWriter(buffer), keyset_handle)
-  keyset = tink_pb2.Keyset.FromString(buffer.getvalue())
+  serialized_keyset = tink.proto_keyset_format.serialize(
+      keyset_handle, secret_key_access.TOKEN
+  )
+  keyset = tink_pb2.Keyset.FromString(serialized_keyset)
   hmac_key = jwt_hmac_pb2.JwtHmacKey.FromString(keyset.key[0].key_data.value)
   hmac_key.custom_kid.value = custom_kid
   keyset.key[0].key_data.value = hmac_key.SerializeToString()
-  return cleartext_keyset_handle.from_keyset(keyset)
+  return tink.proto_keyset_format.parse(
+      keyset.SerializeToString(), secret_key_access.TOKEN
+  )
 
 
 def _change_key_id(keyset_handle: tink.KeysetHandle) -> tink.KeysetHandle:
   """Changes the key id of the first key and sets it primary."""
-  buffer = io.BytesIO()
-  cleartext_keyset_handle.write(
-      tink.BinaryKeysetWriter(buffer), keyset_handle)
-  keyset = tink_pb2.Keyset.FromString(buffer.getvalue())
+  serialized_keyset = tink.proto_keyset_format.serialize(
+      keyset_handle, secret_key_access.TOKEN
+  )
+  keyset = tink_pb2.Keyset.FromString(serialized_keyset)
   # XOR the key id with an arbitrary 32-bit string to get a new key id.
   new_key_id = keyset.key[0].key_id ^ 0xdeadbeef
   keyset.key[0].key_id = new_key_id
   keyset.primary_key_id = new_key_id
-  return cleartext_keyset_handle.from_keyset(keyset)
+  return tink.proto_keyset_format.parse(
+      keyset.SerializeToString(), secret_key_access.TOKEN
+  )
 
 
 def _change_output_prefix_to_tink(
     keyset_handle: tink.KeysetHandle) -> tink.KeysetHandle:
   """Changes the output prefix type of the first key to TINK."""
-  buffer = io.BytesIO()
-  cleartext_keyset_handle.write(
-      tink.BinaryKeysetWriter(buffer), keyset_handle)
-  keyset = tink_pb2.Keyset.FromString(buffer.getvalue())
+  serialization = tink.proto_keyset_format.serialize(
+      keyset_handle, secret_key_access.TOKEN
+  )
+  keyset = tink_pb2.Keyset.FromString(serialization)
   keyset.key[0].output_prefix_type = tink_pb2.TINK
-  return cleartext_keyset_handle.from_keyset(keyset)
+  return tink.proto_keyset_format.parse(
+      keyset.SerializeToString(), secret_key_access.TOKEN
+  )
 
 
 class JwtMacWrapperTest(parameterized.TestCase):
 
   @parameterized.parameters([
       (jwt.raw_jwt_hs256_template(), jwt.raw_jwt_hs256_template()),
       (jwt.raw_jwt_hs256_template(), jwt.jwt_hs256_template()),
```

### Comparing `tink-1.8.0/tink/jwt/_jwt_public_key_sign.py` & `tink-1.9.0/tink/jwt/_jwt_public_key_sign.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/jwt/_jwt_public_key_verify.py` & `tink-1.9.0/tink/jwt/_jwt_public_key_verify.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/jwt/_jwt_signature_key_manager.py` & `tink-1.9.0/tink/jwt/_jwt_signature_key_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 }
 
 
 class _JwtPublicKeySign(_jwt_public_key_sign.JwtPublicKeySignInternal):
   """Implementation of JwtPublicKeySignInternal using a PublicKeySign."""
 
   def __init__(self, cc_primitive: tink_bindings.PublicKeySign, algorithm: str,
-               custom_kid: str):
+               custom_kid: Optional[str]):
     self._public_key_sign = cc_primitive
     self._algorithm = algorithm
     self._custom_kid = custom_kid
 
   @core.use_tink_errors
   def _sign(self, data: bytes) -> bytes:
     return self._public_key_sign.sign(data)
```

### Comparing `tink-1.8.0/tink/jwt/_jwt_signature_key_manager_test.py` & `tink-1.9.0/tink/jwt/_jwt_signature_key_manager_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/jwt/_jwt_signature_wrappers.py` & `tink-1.9.0/tink/jwt/_jwt_signature_wrappers.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/jwt/_jwt_signature_wrappers_test.py` & `tink-1.9.0/tink/jwt/_jwt_signature_wrappers_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,71 +9,71 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink.jwt._jwt_signature_wrappers_test."""
 
-import io
-
-
 from absl.testing import absltest
 from absl.testing import parameterized
 
 from tink.proto import jwt_ecdsa_pb2
 from tink.proto import jwt_rsa_ssa_pkcs1_pb2
 from tink.proto import jwt_rsa_ssa_pss_pb2
 from tink.proto import tink_pb2
 import tink
-from tink import cleartext_keyset_handle
 from tink import jwt
+from tink import secret_key_access
 from tink.jwt import _json_util
 from tink.jwt import _jwt_format
-
 from tink.testing import keyset_builder
 
 
 LONG_CUSTOM_KID = 'Lorem ipsum dolor sit amet, consectetur adipiscing elit'
 
 
 def setUpModule():
   jwt.register_jwt_signature()
 
 
 def _change_key_id(keyset_handle: tink.KeysetHandle) -> tink.KeysetHandle:
   """Changes the key id of the first key and makes it primary."""
-  buffer = io.BytesIO()
-  cleartext_keyset_handle.write(
-      tink.BinaryKeysetWriter(buffer), keyset_handle)
-  keyset = tink_pb2.Keyset.FromString(buffer.getvalue())
+  serialization = tink.proto_keyset_format.serialize(
+      keyset_handle, secret_key_access.TOKEN
+  )
+  keyset = tink_pb2.Keyset.FromString(serialization)
   # XOR the key id with an arbitrary 32-bit string to get a new key id.
   new_key_id = keyset.key[0].key_id ^ 0xdeadbeef
   keyset.key[0].key_id = new_key_id
   keyset.primary_key_id = new_key_id
-  return cleartext_keyset_handle.from_keyset(keyset)
+  return tink.proto_keyset_format.parse(
+      keyset.SerializeToString(), secret_key_access.TOKEN
+  )
 
 
 def _change_output_prefix_to_tink(
     keyset_handle: tink.KeysetHandle) -> tink.KeysetHandle:
   """Changes the output prefix type of the first key to TINK."""
-  buffer = io.BytesIO()
-  cleartext_keyset_handle.write(
-      tink.BinaryKeysetWriter(buffer), keyset_handle)
-  keyset = tink_pb2.Keyset.FromString(buffer.getvalue())
+  serialization = tink.proto_keyset_format.serialize(
+      keyset_handle, secret_key_access.TOKEN
+  )
+  keyset = tink_pb2.Keyset.FromString(serialization)
   keyset.key[0].output_prefix_type = tink_pb2.TINK
-  return cleartext_keyset_handle.from_keyset(keyset)
+  return tink.proto_keyset_format.parse(
+      keyset.SerializeToString(), secret_key_access.TOKEN
+  )
 
 
 def _set_custom_kid(keyset_handle: tink.KeysetHandle,
                     custom_kid: str) -> tink.KeysetHandle:
   """Sets the custom_kid field of the first key."""
-  buffer = io.BytesIO()
-  cleartext_keyset_handle.write(
-      tink.BinaryKeysetWriter(buffer), keyset_handle)
-  keyset = tink_pb2.Keyset.FromString(buffer.getvalue())
+  serialization = tink.proto_keyset_format.serialize(
+      keyset_handle, secret_key_access.TOKEN
+  )
+  keyset = tink_pb2.Keyset.FromString(serialization)
   if keyset.key[0].key_data.type_url.endswith('JwtEcdsaPrivateKey'):
     jwt_ecdsa_key = jwt_ecdsa_pb2.JwtEcdsaPrivateKey.FromString(
         keyset.key[0].key_data.value)
     jwt_ecdsa_key.public_key.custom_kid.value = custom_kid
     keyset.key[0].key_data.value = jwt_ecdsa_key.SerializeToString()
   elif keyset.key[0].key_data.type_url.endswith('JwtRsaSsaPkcs1PrivateKey'):
     rsa_key = jwt_rsa_ssa_pkcs1_pb2.JwtRsaSsaPkcs1PrivateKey.FromString(
@@ -83,15 +83,17 @@
   elif keyset.key[0].key_data.type_url.endswith('JwtRsaSsaPssPrivateKey'):
     rsa_key = jwt_rsa_ssa_pss_pb2.JwtRsaSsaPssPrivateKey.FromString(
         keyset.key[0].key_data.value)
     rsa_key.public_key.custom_kid.value = custom_kid
     keyset.key[0].key_data.value = rsa_key.SerializeToString()
   else:
     raise tink.TinkError('unknown key type')
-  return cleartext_keyset_handle.from_keyset(keyset)
+  return tink.proto_keyset_format.parse(
+      keyset.SerializeToString(), secret_key_access.TOKEN
+  )
 
 
 class JwtSignatureWrapperTest(parameterized.TestCase):
 
   def test_interesting_error(self):
     private_handle = tink.new_keyset_handle(jwt.jwt_es256_template())
     sign = private_handle.primitive(jwt.JwtPublicKeySign)
```

### Comparing `tink-1.8.0/tink/jwt/_jwt_validator.py` & `tink-1.9.0/tink/jwt/_jwt_validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,27 +72,27 @@
     if fixed_now and not fixed_now.tzinfo:
       raise ValueError('fixed_now without tzinfo')
     self._fixed_now = fixed_now
 
   def has_expected_type_header(self) -> bool:
     return self._expected_type_header is not None
 
-  def expected_type_header(self) -> str:
+  def expected_type_header(self) -> Optional[str]:
     return self._expected_type_header
 
   def has_expected_issuer(self) -> bool:
     return self._expected_issuer is not None
 
-  def expected_issuer(self) -> str:
+  def expected_issuer(self) -> Optional[str]:
     return self._expected_issuer
 
   def has_expected_audience(self) -> bool:
     return self._expected_audience is not None
 
-  def expected_audience(self) -> str:
+  def expected_audience(self) -> Optional[str]:
     return self._expected_audience
 
   def ignore_type_header(self) -> bool:
     return self._ignore_type_header
 
   def ignore_issuer(self) -> bool:
     return self._ignore_issuer
@@ -108,15 +108,15 @@
 
   def clock_skew(self) -> datetime.timedelta:
     return self._clock_skew
 
   def has_fixed_now(self) -> bool:
     return self._fixed_now is not None
 
-  def fixed_now(self) -> datetime.datetime:
+  def fixed_now(self) -> Optional[datetime.datetime]:
     return self._fixed_now
 
 
 def new_validator(
     *,
     expected_type_header: Optional[str] = None,
     expected_issuer: Optional[str] = None,
```

### Comparing `tink-1.8.0/tink/jwt/_jwt_validator_test.py` & `tink-1.9.0/tink/jwt/_jwt_validator_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/jwt/_raw_jwt.py` & `tink-1.9.0/tink/jwt/_raw_jwt.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,16 +54,15 @@
   be chosen by the user. This ensures that the key can be changed without any
   changes to the user code.
   """
 
   def __new__(cls):
     raise core.TinkError('RawJwt cannot be instantiated directly.')
 
-  def __init__(self, type_header: Optional[str], payload: Dict[str,
-                                                               Any]) -> None:
+  def __init__(self, type_header: Optional[str], payload: Any) -> None:
     # No need to copy payload, because only create and from_json_payload
     # call this method.
     if not isinstance(payload, Dict):
       raise _jwt_error.JwtInvalidError('payload must be a dict')
     self._type_header = type_header
     self._payload = payload
     self._validate_string_claim('iss')
@@ -95,20 +94,19 @@
       if isinstance(audiences, str):
         return
       if not isinstance(audiences, list) or not audiences:
         raise _jwt_error.JwtInvalidError('audiences cannot be an empty list')
       if not all(isinstance(value, str) for value in audiences):
         raise _jwt_error.JwtInvalidError('audiences must only contain strings')
 
-  # TODO(juerg): Consider adding a raw_ prefix to all access methods
   def has_type_header(self) -> bool:
     return self._type_header is not None
 
   def type_header(self) -> str:
-    if not self.has_type_header():
+    if self._type_header is None:
       raise KeyError('type header is not set')
     return self._type_header
 
   def has_issuer(self) -> bool:
     return 'iss' in self._payload
 
   def issuer(self) -> str:
```

### Comparing `tink-1.8.0/tink/jwt/_raw_jwt_test.py` & `tink-1.9.0/tink/jwt/_raw_jwt_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/jwt/_verified_jwt.py` & `tink-1.9.0/tink/jwt/_verified_jwt.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/jwt/_verified_jwt_test.py` & `tink-1.9.0/tink/jwt/_verified_jwt_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/mac/BUILD.bazel` & `tink-1.9.0/tink/mac/BUILD.bazel`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 
 py_library(
     name = "_mac_wrapper",
     srcs = ["_mac_wrapper.py"],
     srcs_version = "PY3",
     deps = [
         ":_mac",
-        requirement("absl-py"),
         "//tink/core",
         "//tink/proto:tink_py_pb2",
     ],
 )
 
 py_test(
     name = "_mac_wrapper_test",
```

### Comparing `tink-1.8.0/tink/mac/__init__.py` & `tink-1.9.0/tink/prf/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Copyright 2020 Google LLC
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Mac package."""
+"""PrfSet package."""
 
-from tink.mac import _mac
-from tink.mac import _mac_key_manager
-from tink.mac import _mac_key_templates as mac_key_templates
+from tink.prf import _prf_key_manager
+from tink.prf import _prf_key_templates as prf_key_templates
+from tink.prf import _prf_set
 
-
-Mac = _mac.Mac
-register = _mac_key_manager.register
+Prf = _prf_set.Prf
+PrfSet = _prf_set.PrfSet
+register = _prf_key_manager.register
```

### Comparing `tink-1.8.0/tink/mac/_mac.py` & `tink-1.9.0/tink/mac/_mac.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/mac/_mac_key_manager.py` & `tink-1.9.0/tink/mac/_mac_key_manager.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/mac/_mac_key_manager_test.py` & `tink-1.9.0/tink/mac/_mac_key_manager_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/mac/_mac_key_templates.py` & `tink-1.9.0/tink/mac/_mac_key_templates.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/mac/_mac_key_templates_test.py` & `tink-1.9.0/tink/mac/_mac_key_templates_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/mac/_mac_wrapper.py` & `tink-1.9.0/tink/mac/_mac_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """MAC wrapper.
 """
 
 from typing import Type
-from absl import logging
-
 
 from tink.proto import tink_pb2
 from tink import core
 from tink.mac import _mac
 
 
 class _WrappedMac(_mac.Mac):
@@ -48,24 +46,24 @@
       try:
         if entry.output_prefix_type == tink_pb2.LEGACY:
           entry.primitive.verify_mac(mac_no_prefix, data + b'\x00')
         else:
           entry.primitive.verify_mac(mac_no_prefix, data)
         # If there is no exception, the MAC is valid and we can return.
         return
-      except core.TinkError as e:
-        logging.info('tag prefix matches a key, but cannot verify: %s', e)
+      except core.TinkError:
+        pass
 
     # No 'non-raw' key matched, so let's try the raw keys (if any exist).
     for entry in self._primitive_set.raw_primitives():
       try:
         entry.primitive.verify_mac(mac_value, data)
         # If there is no exception, the MAC is valid and we can return.
         return
-      except core.TinkError as e:
+      except core.TinkError:
         pass
     raise core.TinkError('invalid MAC')
 
 
 class MacWrapper(core.PrimitiveWrapper[_mac.Mac, _mac.Mac]):
   """MacWrapper is the implementation of PrimitiveWrapper for the Mac primitive.
```

### Comparing `tink-1.8.0/tink/mac/_mac_wrapper_test.py` & `tink-1.9.0/tink/mac/_mac_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/prf/BUILD.bazel` & `tink-1.9.0/tink/prf/BUILD.bazel`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/prf/_prf_key_manager.py` & `tink-1.9.0/tink/prf/_prf_key_manager.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/prf/_prf_key_manager_test.py` & `tink-1.9.0/tink/prf/_prf_key_manager_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/prf/_prf_key_templates.py` & `tink-1.9.0/tink/prf/_prf_key_templates.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/prf/_prf_set.py` & `tink-1.9.0/tink/prf/_prf_set.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/prf/_prf_set_wrapper.py` & `tink-1.9.0/tink/prf/_prf_set_wrapper.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/prf/_prf_set_wrapper_test.py` & `tink-1.9.0/tink/prf/_prf_set_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/BUILD.bazel` & `tink-1.9.0/tink/proto/BUILD.bazel`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/__init__.py` & `tink-1.9.0/tink/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/aes_cmac.proto` & `tink-1.9.0/tink/proto/aes_cmac.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/aes_cmac_pb2.py` & `tink-1.9.0/tink/proto/aes_cmac_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: tink/proto/aes_cmac.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19tink/proto/aes_cmac.proto\x12\x12google.crypto.tink\"!\n\rAesCmacParams\x12\x10\n\x08tag_size\x18\x01 \x01(\r\"c\n\nAesCmacKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x11\n\tkey_value\x18\x02 \x01(\x0c\x12\x31\n\x06params\x18\x03 \x01(\x0b\x32!.google.crypto.tink.AesCmacParams\"W\n\x10\x41\x65sCmacKeyFormat\x12\x10\n\x08key_size\x18\x01 \x01(\r\x12\x31\n\x06params\x18\x02 \x01(\x0b\x32!.google.crypto.tink.AesCmacParamsBS\n\x1c\x63om.google.crypto.tink.protoP\x01Z1github.com/google/tink/go/proto/aes_cmac_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.aes_cmac_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.aes_cmac_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z1github.com/google/tink/go/proto/aes_cmac_go_proto'
-  _AESCMACPARAMS._serialized_start=49
-  _AESCMACPARAMS._serialized_end=82
-  _AESCMACKEY._serialized_start=84
-  _AESCMACKEY._serialized_end=183
-  _AESCMACKEYFORMAT._serialized_start=185
-  _AESCMACKEYFORMAT._serialized_end=272
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z1github.com/google/tink/go/proto/aes_cmac_go_proto'
+  _globals['_AESCMACPARAMS']._serialized_start=49
+  _globals['_AESCMACPARAMS']._serialized_end=82
+  _globals['_AESCMACKEY']._serialized_start=84
+  _globals['_AESCMACKEY']._serialized_end=183
+  _globals['_AESCMACKEYFORMAT']._serialized_start=185
+  _globals['_AESCMACKEYFORMAT']._serialized_end=272
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/aes_cmac_prf.proto` & `tink-1.9.0/tink/proto/aes_cmac_prf.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/aes_cmac_prf_pb2.py` & `tink-1.9.0/tink/proto/hmac_prf_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tink/proto/aes_cmac_prf.proto
+# source: tink/proto/hmac_prf.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from tink.proto import common_pb2 as tink_dot_proto_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dtink/proto/aes_cmac_prf.proto\x12\x12google.crypto.tink\"3\n\rAesCmacPrfKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x11\n\tkey_value\x18\x02 \x01(\x0c\"8\n\x13\x41\x65sCmacPrfKeyFormat\x12\x0f\n\x07version\x18\x02 \x01(\r\x12\x10\n\x08key_size\x18\x01 \x01(\rBW\n\x1c\x63om.google.crypto.tink.protoP\x01Z5github.com/google/tink/go/proto/aes_cmac_prf_go_protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19tink/proto/hmac_prf.proto\x12\x12google.crypto.tink\x1a\x17tink/proto/common.proto\";\n\rHmacPrfParams\x12*\n\x04hash\x18\x01 \x01(\x0e\x32\x1c.google.crypto.tink.HashType\"c\n\nHmacPrfKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x31\n\x06params\x18\x02 \x01(\x0b\x32!.google.crypto.tink.HmacPrfParams\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\"h\n\x10HmacPrfKeyFormat\x12\x31\n\x06params\x18\x01 \x01(\x0b\x32!.google.crypto.tink.HmacPrfParams\x12\x10\n\x08key_size\x18\x02 \x01(\r\x12\x0f\n\x07version\x18\x03 \x01(\rBS\n\x1c\x63om.google.crypto.tink.protoP\x01Z1github.com/google/tink/go/proto/hmac_prf_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.aes_cmac_prf_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.hmac_prf_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z5github.com/google/tink/go/proto/aes_cmac_prf_go_proto'
-  _AESCMACPRFKEY._serialized_start=53
-  _AESCMACPRFKEY._serialized_end=104
-  _AESCMACPRFKEYFORMAT._serialized_start=106
-  _AESCMACPRFKEYFORMAT._serialized_end=162
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z1github.com/google/tink/go/proto/hmac_prf_go_proto'
+  _globals['_HMACPRFPARAMS']._serialized_start=74
+  _globals['_HMACPRFPARAMS']._serialized_end=133
+  _globals['_HMACPRFKEY']._serialized_start=135
+  _globals['_HMACPRFKEY']._serialized_end=234
+  _globals['_HMACPRFKEYFORMAT']._serialized_start=236
+  _globals['_HMACPRFKEYFORMAT']._serialized_end=340
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/aes_ctr.proto` & `tink-1.9.0/tink/proto/aes_ctr.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/aes_ctr_hmac_aead.proto` & `tink-1.9.0/tink/proto/aes_ctr_hmac_aead.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/aes_ctr_hmac_aead_pb2.py` & `tink-1.9.0/tink/proto/hmac_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tink/proto/aes_ctr_hmac_aead.proto
+# source: tink/proto/hmac.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from tink.proto import aes_ctr_pb2 as tink_dot_proto_dot_aes__ctr__pb2
-from tink.proto import hmac_pb2 as tink_dot_proto_dot_hmac__pb2
+from tink.proto import common_pb2 as tink_dot_proto_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"tink/proto/aes_ctr_hmac_aead.proto\x12\x12google.crypto.tink\x1a\x18tink/proto/aes_ctr.proto\x1a\x15tink/proto/hmac.proto\"\x96\x01\n\x17\x41\x65sCtrHmacAeadKeyFormat\x12?\n\x12\x61\x65s_ctr_key_format\x18\x01 \x01(\x0b\x32#.google.crypto.tink.AesCtrKeyFormat\x12:\n\x0fhmac_key_format\x18\x02 \x01(\x0b\x32!.google.crypto.tink.HmacKeyFormat\"\x87\x01\n\x11\x41\x65sCtrHmacAeadKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x32\n\x0b\x61\x65s_ctr_key\x18\x02 \x01(\x0b\x32\x1d.google.crypto.tink.AesCtrKey\x12-\n\x08hmac_key\x18\x03 \x01(\x0b\x32\x1b.google.crypto.tink.HmacKeyB\\\n\x1c\x63om.google.crypto.tink.protoP\x01Z:github.com/google/tink/go/proto/aes_ctr_hmac_aead_go_protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15tink/proto/hmac.proto\x12\x12google.crypto.tink\x1a\x17tink/proto/common.proto\"J\n\nHmacParams\x12*\n\x04hash\x18\x01 \x01(\x0e\x32\x1c.google.crypto.tink.HashType\x12\x10\n\x08tag_size\x18\x02 \x01(\r\"]\n\x07HmacKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12.\n\x06params\x18\x02 \x01(\x0b\x32\x1e.google.crypto.tink.HmacParams\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\"b\n\rHmacKeyFormat\x12.\n\x06params\x18\x01 \x01(\x0b\x32\x1e.google.crypto.tink.HmacParams\x12\x10\n\x08key_size\x18\x02 \x01(\r\x12\x0f\n\x07version\x18\x03 \x01(\rBO\n\x1c\x63om.google.crypto.tink.protoP\x01Z-github.com/google/tink/go/proto/hmac_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.aes_ctr_hmac_aead_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.hmac_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z:github.com/google/tink/go/proto/aes_ctr_hmac_aead_go_proto'
-  _AESCTRHMACAEADKEYFORMAT._serialized_start=108
-  _AESCTRHMACAEADKEYFORMAT._serialized_end=258
-  _AESCTRHMACAEADKEY._serialized_start=261
-  _AESCTRHMACAEADKEY._serialized_end=396
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z-github.com/google/tink/go/proto/hmac_go_proto'
+  _globals['_HMACPARAMS']._serialized_start=70
+  _globals['_HMACPARAMS']._serialized_end=144
+  _globals['_HMACKEY']._serialized_start=146
+  _globals['_HMACKEY']._serialized_end=239
+  _globals['_HMACKEYFORMAT']._serialized_start=241
+  _globals['_HMACKEYFORMAT']._serialized_end=339
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/aes_ctr_hmac_streaming.proto` & `tink-1.9.0/tink/proto/aes_ctr_hmac_streaming.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/aes_ctr_hmac_streaming_pb2.py` & `tink-1.9.0/tink/proto/aes_gcm_hkdf_streaming_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tink/proto/aes_ctr_hmac_streaming.proto
+# source: tink/proto/aes_gcm_hkdf_streaming.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from tink.proto import common_pb2 as tink_dot_proto_dot_common__pb2
-from tink.proto import hmac_pb2 as tink_dot_proto_dot_hmac__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'tink/proto/aes_ctr_hmac_streaming.proto\x12\x12google.crypto.tink\x1a\x17tink/proto/common.proto\x1a\x15tink/proto/hmac.proto\"\xc1\x01\n\x19\x41\x65sCtrHmacStreamingParams\x12\x1f\n\x17\x63iphertext_segment_size\x18\x01 \x01(\r\x12\x18\n\x10\x64\x65rived_key_size\x18\x02 \x01(\r\x12\x34\n\x0ehkdf_hash_type\x18\x03 \x01(\x0e\x32\x1c.google.crypto.tink.HashType\x12\x33\n\x0bhmac_params\x18\x04 \x01(\x0b\x32\x1e.google.crypto.tink.HmacParams\"\x80\x01\n\x1c\x41\x65sCtrHmacStreamingKeyFormat\x12\x0f\n\x07version\x18\x03 \x01(\r\x12=\n\x06params\x18\x01 \x01(\x0b\x32-.google.crypto.tink.AesCtrHmacStreamingParams\x12\x10\n\x08key_size\x18\x02 \x01(\r\"{\n\x16\x41\x65sCtrHmacStreamingKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12=\n\x06params\x18\x02 \x01(\x0b\x32-.google.crypto.tink.AesCtrHmacStreamingParams\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\x42\x61\n\x1c\x63om.google.crypto.tink.protoP\x01Z?github.com/google/tink/go/proto/aes_ctr_hmac_streaming_go_protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'tink/proto/aes_gcm_hkdf_streaming.proto\x12\x12google.crypto.tink\x1a\x17tink/proto/common.proto\"\x8c\x01\n\x19\x41\x65sGcmHkdfStreamingParams\x12\x1f\n\x17\x63iphertext_segment_size\x18\x01 \x01(\r\x12\x18\n\x10\x64\x65rived_key_size\x18\x02 \x01(\r\x12\x34\n\x0ehkdf_hash_type\x18\x03 \x01(\x0e\x32\x1c.google.crypto.tink.HashType\"\x80\x01\n\x1c\x41\x65sGcmHkdfStreamingKeyFormat\x12\x0f\n\x07version\x18\x03 \x01(\r\x12=\n\x06params\x18\x01 \x01(\x0b\x32-.google.crypto.tink.AesGcmHkdfStreamingParams\x12\x10\n\x08key_size\x18\x02 \x01(\r\"{\n\x16\x41\x65sGcmHkdfStreamingKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12=\n\x06params\x18\x02 \x01(\x0b\x32-.google.crypto.tink.AesGcmHkdfStreamingParams\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\x42\x61\n\x1c\x63om.google.crypto.tink.protoP\x01Z?github.com/google/tink/go/proto/aes_gcm_hkdf_streaming_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.aes_ctr_hmac_streaming_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.aes_gcm_hkdf_streaming_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z?github.com/google/tink/go/proto/aes_ctr_hmac_streaming_go_proto'
-  _AESCTRHMACSTREAMINGPARAMS._serialized_start=112
-  _AESCTRHMACSTREAMINGPARAMS._serialized_end=305
-  _AESCTRHMACSTREAMINGKEYFORMAT._serialized_start=308
-  _AESCTRHMACSTREAMINGKEYFORMAT._serialized_end=436
-  _AESCTRHMACSTREAMINGKEY._serialized_start=438
-  _AESCTRHMACSTREAMINGKEY._serialized_end=561
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z?github.com/google/tink/go/proto/aes_gcm_hkdf_streaming_go_proto'
+  _globals['_AESGCMHKDFSTREAMINGPARAMS']._serialized_start=89
+  _globals['_AESGCMHKDFSTREAMINGPARAMS']._serialized_end=229
+  _globals['_AESGCMHKDFSTREAMINGKEYFORMAT']._serialized_start=232
+  _globals['_AESGCMHKDFSTREAMINGKEYFORMAT']._serialized_end=360
+  _globals['_AESGCMHKDFSTREAMINGKEY']._serialized_start=362
+  _globals['_AESGCMHKDFSTREAMINGKEY']._serialized_end=485
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/aes_ctr_pb2.py` & `tink-1.9.0/tink/proto/aes_ctr_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: tink/proto/aes_ctr.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18tink/proto/aes_ctr.proto\x12\x12google.crypto.tink\"\x1f\n\x0c\x41\x65sCtrParams\x12\x0f\n\x07iv_size\x18\x01 \x01(\r\"U\n\x0f\x41\x65sCtrKeyFormat\x12\x30\n\x06params\x18\x01 \x01(\x0b\x32 .google.crypto.tink.AesCtrParams\x12\x10\n\x08key_size\x18\x02 \x01(\r\"a\n\tAesCtrKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x30\n\x06params\x18\x02 \x01(\x0b\x32 .google.crypto.tink.AesCtrParams\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\x42R\n\x1c\x63om.google.crypto.tink.protoP\x01Z0github.com/google/tink/go/proto/aes_ctr_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.aes_ctr_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.aes_ctr_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z0github.com/google/tink/go/proto/aes_ctr_go_proto'
-  _AESCTRPARAMS._serialized_start=48
-  _AESCTRPARAMS._serialized_end=79
-  _AESCTRKEYFORMAT._serialized_start=81
-  _AESCTRKEYFORMAT._serialized_end=166
-  _AESCTRKEY._serialized_start=168
-  _AESCTRKEY._serialized_end=265
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z0github.com/google/tink/go/proto/aes_ctr_go_proto'
+  _globals['_AESCTRPARAMS']._serialized_start=48
+  _globals['_AESCTRPARAMS']._serialized_end=79
+  _globals['_AESCTRKEYFORMAT']._serialized_start=81
+  _globals['_AESCTRKEYFORMAT']._serialized_end=166
+  _globals['_AESCTRKEY']._serialized_start=168
+  _globals['_AESCTRKEY']._serialized_end=265
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/aes_eax.proto` & `tink-1.9.0/tink/proto/aes_eax.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/aes_eax_pb2.py` & `tink-1.9.0/tink/proto/config_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tink/proto/aes_eax.proto
+# source: tink/proto/config.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18tink/proto/aes_eax.proto\x12\x12google.crypto.tink\"\x1f\n\x0c\x41\x65sEaxParams\x12\x0f\n\x07iv_size\x18\x01 \x01(\r\"U\n\x0f\x41\x65sEaxKeyFormat\x12\x30\n\x06params\x18\x01 \x01(\x0b\x32 .google.crypto.tink.AesEaxParams\x12\x10\n\x08key_size\x18\x02 \x01(\r\"a\n\tAesEaxKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x30\n\x06params\x18\x02 \x01(\x0b\x32 .google.crypto.tink.AesEaxParams\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\x42R\n\x1c\x63om.google.crypto.tink.protoP\x01Z0github.com/google/tink/go/proto/aes_eax_go_protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17tink/proto/config.proto\x12\x12google.crypto.tink\"\x8a\x01\n\x0cKeyTypeEntry\x12\x16\n\x0eprimitive_name\x18\x01 \x01(\t\x12\x10\n\x08type_url\x18\x02 \x01(\t\x12\x1b\n\x13key_manager_version\x18\x03 \x01(\r\x12\x17\n\x0fnew_key_allowed\x18\x04 \x01(\x08\x12\x16\n\x0e\x63\x61talogue_name\x18\x05 \x01(\t:\x02\x18\x01\"Z\n\x0eRegistryConfig\x12\x13\n\x0b\x63onfig_name\x18\x01 \x01(\t\x12/\n\x05\x65ntry\x18\x02 \x03(\x0b\x32 .google.crypto.tink.KeyTypeEntry:\x02\x18\x01\x42Q\n\x1c\x63om.google.crypto.tink.protoP\x01Z/github.com/google/tink/go/proto/config_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.aes_eax_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.config_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z0github.com/google/tink/go/proto/aes_eax_go_proto'
-  _AESEAXPARAMS._serialized_start=48
-  _AESEAXPARAMS._serialized_end=79
-  _AESEAXKEYFORMAT._serialized_start=81
-  _AESEAXKEYFORMAT._serialized_end=166
-  _AESEAXKEY._serialized_start=168
-  _AESEAXKEY._serialized_end=265
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z/github.com/google/tink/go/proto/config_go_proto'
+  _globals['_KEYTYPEENTRY']._options = None
+  _globals['_KEYTYPEENTRY']._serialized_options = b'\030\001'
+  _globals['_REGISTRYCONFIG']._options = None
+  _globals['_REGISTRYCONFIG']._serialized_options = b'\030\001'
+  _globals['_KEYTYPEENTRY']._serialized_start=48
+  _globals['_KEYTYPEENTRY']._serialized_end=186
+  _globals['_REGISTRYCONFIG']._serialized_start=188
+  _globals['_REGISTRYCONFIG']._serialized_end=278
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/aes_gcm.proto` & `tink-1.9.0/tink/proto/aes_gcm.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/aes_gcm_hkdf_streaming.proto` & `tink-1.9.0/tink/proto/aes_gcm_hkdf_streaming.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/aes_gcm_hkdf_streaming_pb2.py` & `tink-1.9.0/tink/proto/aes_eax_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tink/proto/aes_gcm_hkdf_streaming.proto
+# source: tink/proto/aes_eax.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from tink.proto import common_pb2 as tink_dot_proto_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'tink/proto/aes_gcm_hkdf_streaming.proto\x12\x12google.crypto.tink\x1a\x17tink/proto/common.proto\"\x8c\x01\n\x19\x41\x65sGcmHkdfStreamingParams\x12\x1f\n\x17\x63iphertext_segment_size\x18\x01 \x01(\r\x12\x18\n\x10\x64\x65rived_key_size\x18\x02 \x01(\r\x12\x34\n\x0ehkdf_hash_type\x18\x03 \x01(\x0e\x32\x1c.google.crypto.tink.HashType\"\x80\x01\n\x1c\x41\x65sGcmHkdfStreamingKeyFormat\x12\x0f\n\x07version\x18\x03 \x01(\r\x12=\n\x06params\x18\x01 \x01(\x0b\x32-.google.crypto.tink.AesGcmHkdfStreamingParams\x12\x10\n\x08key_size\x18\x02 \x01(\r\"{\n\x16\x41\x65sGcmHkdfStreamingKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12=\n\x06params\x18\x02 \x01(\x0b\x32-.google.crypto.tink.AesGcmHkdfStreamingParams\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\x42\x61\n\x1c\x63om.google.crypto.tink.protoP\x01Z?github.com/google/tink/go/proto/aes_gcm_hkdf_streaming_go_protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18tink/proto/aes_eax.proto\x12\x12google.crypto.tink\"\x1f\n\x0c\x41\x65sEaxParams\x12\x0f\n\x07iv_size\x18\x01 \x01(\r\"U\n\x0f\x41\x65sEaxKeyFormat\x12\x30\n\x06params\x18\x01 \x01(\x0b\x32 .google.crypto.tink.AesEaxParams\x12\x10\n\x08key_size\x18\x02 \x01(\r\"a\n\tAesEaxKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x30\n\x06params\x18\x02 \x01(\x0b\x32 .google.crypto.tink.AesEaxParams\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\x42R\n\x1c\x63om.google.crypto.tink.protoP\x01Z0github.com/google/tink/go/proto/aes_eax_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.aes_gcm_hkdf_streaming_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.aes_eax_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z?github.com/google/tink/go/proto/aes_gcm_hkdf_streaming_go_proto'
-  _AESGCMHKDFSTREAMINGPARAMS._serialized_start=89
-  _AESGCMHKDFSTREAMINGPARAMS._serialized_end=229
-  _AESGCMHKDFSTREAMINGKEYFORMAT._serialized_start=232
-  _AESGCMHKDFSTREAMINGKEYFORMAT._serialized_end=360
-  _AESGCMHKDFSTREAMINGKEY._serialized_start=362
-  _AESGCMHKDFSTREAMINGKEY._serialized_end=485
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z0github.com/google/tink/go/proto/aes_eax_go_proto'
+  _globals['_AESEAXPARAMS']._serialized_start=48
+  _globals['_AESEAXPARAMS']._serialized_end=79
+  _globals['_AESEAXKEYFORMAT']._serialized_start=81
+  _globals['_AESEAXKEYFORMAT']._serialized_end=166
+  _globals['_AESEAXKEY']._serialized_start=168
+  _globals['_AESEAXKEY']._serialized_end=265
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/aes_gcm_pb2.py` & `tink-1.9.0/tink/proto/aes_siv_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tink/proto/aes_gcm.proto
+# source: tink/proto/aes_siv.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18tink/proto/aes_gcm.proto\x12\x12google.crypto.tink\"4\n\x0f\x41\x65sGcmKeyFormat\x12\x10\n\x08key_size\x18\x02 \x01(\r\x12\x0f\n\x07version\x18\x03 \x01(\r\"/\n\tAesGcmKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\x42[\n\x1c\x63om.google.crypto.tink.protoP\x01Z0github.com/google/tink/go/proto/aes_gcm_go_proto\xa2\x02\x06TINKPBb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18tink/proto/aes_siv.proto\x12\x12google.crypto.tink\"4\n\x0f\x41\x65sSivKeyFormat\x12\x10\n\x08key_size\x18\x01 \x01(\r\x12\x0f\n\x07version\x18\x02 \x01(\r\"/\n\tAesSivKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x11\n\tkey_value\x18\x02 \x01(\x0c\x42R\n\x1c\x63om.google.crypto.tink.protoP\x01Z0github.com/google/tink/go/proto/aes_siv_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.aes_gcm_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.aes_siv_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z0github.com/google/tink/go/proto/aes_gcm_go_proto\242\002\006TINKPB'
-  _AESGCMKEYFORMAT._serialized_start=48
-  _AESGCMKEYFORMAT._serialized_end=100
-  _AESGCMKEY._serialized_start=102
-  _AESGCMKEY._serialized_end=149
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z0github.com/google/tink/go/proto/aes_siv_go_proto'
+  _globals['_AESSIVKEYFORMAT']._serialized_start=48
+  _globals['_AESSIVKEYFORMAT']._serialized_end=100
+  _globals['_AESSIVKEY']._serialized_start=102
+  _globals['_AESSIVKEY']._serialized_end=149
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/aes_gcm_siv.proto` & `tink-1.9.0/tink/proto/aes_gcm_siv.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/aes_gcm_siv_pb2.py` & `tink-1.9.0/tink/proto/aes_gcm_siv_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: tink/proto/aes_gcm_siv.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ctink/proto/aes_gcm_siv.proto\x12\x12google.crypto.tink\"7\n\x12\x41\x65sGcmSivKeyFormat\x12\x10\n\x08key_size\x18\x02 \x01(\r\x12\x0f\n\x07version\x18\x01 \x01(\r\"2\n\x0c\x41\x65sGcmSivKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\x42V\n\x1c\x63om.google.crypto.tink.protoP\x01Z4github.com/google/tink/go/proto/aes_gcm_siv_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.aes_gcm_siv_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.aes_gcm_siv_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z4github.com/google/tink/go/proto/aes_gcm_siv_go_proto'
-  _AESGCMSIVKEYFORMAT._serialized_start=52
-  _AESGCMSIVKEYFORMAT._serialized_end=107
-  _AESGCMSIVKEY._serialized_start=109
-  _AESGCMSIVKEY._serialized_end=159
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z4github.com/google/tink/go/proto/aes_gcm_siv_go_proto'
+  _globals['_AESGCMSIVKEYFORMAT']._serialized_start=52
+  _globals['_AESGCMSIVKEYFORMAT']._serialized_end=107
+  _globals['_AESGCMSIVKEY']._serialized_start=109
+  _globals['_AESGCMSIVKEY']._serialized_end=159
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/aes_siv.proto` & `tink-1.9.0/tink/proto/aes_siv.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/aes_siv_pb2.py` & `tink-1.9.0/tink/proto/empty_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tink/proto/aes_siv.proto
+# source: tink/proto/empty.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18tink/proto/aes_siv.proto\x12\x12google.crypto.tink\"4\n\x0f\x41\x65sSivKeyFormat\x12\x10\n\x08key_size\x18\x01 \x01(\r\x12\x0f\n\x07version\x18\x02 \x01(\r\"/\n\tAesSivKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x11\n\tkey_value\x18\x02 \x01(\x0c\x42R\n\x1c\x63om.google.crypto.tink.protoP\x01Z0github.com/google/tink/go/proto/aes_siv_go_protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16tink/proto/empty.proto\x12\x12google.crypto.tink\"\x07\n\x05\x45mptyBP\n\x1c\x63om.google.crypto.tink.protoP\x01Z.github.com/google/tink/go/proto/empty_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.aes_siv_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.empty_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z0github.com/google/tink/go/proto/aes_siv_go_proto'
-  _AESSIVKEYFORMAT._serialized_start=48
-  _AESSIVKEYFORMAT._serialized_end=100
-  _AESSIVKEY._serialized_start=102
-  _AESSIVKEY._serialized_end=149
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z.github.com/google/tink/go/proto/empty_go_proto'
+  _globals['_EMPTY']._serialized_start=46
+  _globals['_EMPTY']._serialized_end=53
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/chacha20_poly1305.proto` & `tink-1.9.0/tink/proto/chacha20_poly1305.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/chacha20_poly1305_pb2.py` & `tink-1.9.0/tink/proto/chacha20_poly1305_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: tink/proto/chacha20_poly1305.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"tink/proto/chacha20_poly1305.proto\x12\x12google.crypto.tink\"\x1b\n\x19\x43haCha20Poly1305KeyFormat\"9\n\x13\x43haCha20Poly1305Key\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x11\n\tkey_value\x18\x02 \x01(\x0c\x42\\\n\x1c\x63om.google.crypto.tink.protoP\x01Z:github.com/google/tink/go/proto/chacha20_poly1305_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.chacha20_poly1305_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.chacha20_poly1305_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z:github.com/google/tink/go/proto/chacha20_poly1305_go_proto'
-  _CHACHA20POLY1305KEYFORMAT._serialized_start=58
-  _CHACHA20POLY1305KEYFORMAT._serialized_end=85
-  _CHACHA20POLY1305KEY._serialized_start=87
-  _CHACHA20POLY1305KEY._serialized_end=144
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z:github.com/google/tink/go/proto/chacha20_poly1305_go_proto'
+  _globals['_CHACHA20POLY1305KEYFORMAT']._serialized_start=58
+  _globals['_CHACHA20POLY1305KEYFORMAT']._serialized_end=85
+  _globals['_CHACHA20POLY1305KEY']._serialized_start=87
+  _globals['_CHACHA20POLY1305KEY']._serialized_end=144
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/common.proto` & `tink-1.9.0/tink/proto/common.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/common_pb2.py` & `tink-1.9.0/tink/proto/common_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: tink/proto/common.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17tink/proto/common.proto\x12\x12google.crypto.tink*c\n\x11\x45llipticCurveType\x12\x11\n\rUNKNOWN_CURVE\x10\x00\x12\r\n\tNIST_P256\x10\x02\x12\r\n\tNIST_P384\x10\x03\x12\r\n\tNIST_P521\x10\x04\x12\x0e\n\nCURVE25519\x10\x05*j\n\rEcPointFormat\x12\x12\n\x0eUNKNOWN_FORMAT\x10\x00\x12\x10\n\x0cUNCOMPRESSED\x10\x01\x12\x0e\n\nCOMPRESSED\x10\x02\x12#\n\x1f\x44O_NOT_USE_CRUNCHY_UNCOMPRESSED\x10\x03*V\n\x08HashType\x12\x10\n\x0cUNKNOWN_HASH\x10\x00\x12\x08\n\x04SHA1\x10\x01\x12\n\n\x06SHA384\x10\x02\x12\n\n\x06SHA256\x10\x03\x12\n\n\x06SHA512\x10\x04\x12\n\n\x06SHA224\x10\x05\x42Q\n\x1c\x63om.google.crypto.tink.protoP\x01Z/github.com/google/tink/go/proto/common_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.common_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z/github.com/google/tink/go/proto/common_go_proto'
-  _ELLIPTICCURVETYPE._serialized_start=47
-  _ELLIPTICCURVETYPE._serialized_end=146
-  _ECPOINTFORMAT._serialized_start=148
-  _ECPOINTFORMAT._serialized_end=254
-  _HASHTYPE._serialized_start=256
-  _HASHTYPE._serialized_end=342
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z/github.com/google/tink/go/proto/common_go_proto'
+  _globals['_ELLIPTICCURVETYPE']._serialized_start=47
+  _globals['_ELLIPTICCURVETYPE']._serialized_end=146
+  _globals['_ECPOINTFORMAT']._serialized_start=148
+  _globals['_ECPOINTFORMAT']._serialized_end=254
+  _globals['_HASHTYPE']._serialized_start=256
+  _globals['_HASHTYPE']._serialized_end=342
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/config.proto` & `tink-1.9.0/tink/proto/config.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/config_pb2.py` & `tink-1.9.0/tink/proto/aes_gcm_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tink/proto/config.proto
+# source: tink/proto/aes_gcm.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17tink/proto/config.proto\x12\x12google.crypto.tink\"\x8a\x01\n\x0cKeyTypeEntry\x12\x16\n\x0eprimitive_name\x18\x01 \x01(\t\x12\x10\n\x08type_url\x18\x02 \x01(\t\x12\x1b\n\x13key_manager_version\x18\x03 \x01(\r\x12\x17\n\x0fnew_key_allowed\x18\x04 \x01(\x08\x12\x16\n\x0e\x63\x61talogue_name\x18\x05 \x01(\t:\x02\x18\x01\"Z\n\x0eRegistryConfig\x12\x13\n\x0b\x63onfig_name\x18\x01 \x01(\t\x12/\n\x05\x65ntry\x18\x02 \x03(\x0b\x32 .google.crypto.tink.KeyTypeEntry:\x02\x18\x01\x42Q\n\x1c\x63om.google.crypto.tink.protoP\x01Z/github.com/google/tink/go/proto/config_go_protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18tink/proto/aes_gcm.proto\x12\x12google.crypto.tink\"4\n\x0f\x41\x65sGcmKeyFormat\x12\x10\n\x08key_size\x18\x02 \x01(\r\x12\x0f\n\x07version\x18\x03 \x01(\r\"/\n\tAesGcmKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\x42[\n\x1c\x63om.google.crypto.tink.protoP\x01Z0github.com/google/tink/go/proto/aes_gcm_go_proto\xa2\x02\x06TINKPBb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.config_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.aes_gcm_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z/github.com/google/tink/go/proto/config_go_proto'
-  _KEYTYPEENTRY._options = None
-  _KEYTYPEENTRY._serialized_options = b'\030\001'
-  _REGISTRYCONFIG._options = None
-  _REGISTRYCONFIG._serialized_options = b'\030\001'
-  _KEYTYPEENTRY._serialized_start=48
-  _KEYTYPEENTRY._serialized_end=186
-  _REGISTRYCONFIG._serialized_start=188
-  _REGISTRYCONFIG._serialized_end=278
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z0github.com/google/tink/go/proto/aes_gcm_go_proto\242\002\006TINKPB'
+  _globals['_AESGCMKEYFORMAT']._serialized_start=48
+  _globals['_AESGCMKEYFORMAT']._serialized_end=100
+  _globals['_AESGCMKEY']._serialized_start=102
+  _globals['_AESGCMKEY']._serialized_end=149
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/ecdsa.proto` & `tink-1.9.0/tink/proto/ecdsa.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/ecdsa_pb2.py` & `tink-1.9.0/tink/proto/hkdf_prf_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tink/proto/ecdsa.proto
+# source: tink/proto/hkdf_prf.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from tink.proto import common_pb2 as tink_dot_proto_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16tink/proto/ecdsa.proto\x12\x12google.crypto.tink\x1a\x17tink/proto/common.proto\"\xb2\x01\n\x0b\x45\x63\x64saParams\x12/\n\thash_type\x18\x01 \x01(\x0e\x32\x1c.google.crypto.tink.HashType\x12\x34\n\x05\x63urve\x18\x02 \x01(\x0e\x32%.google.crypto.tink.EllipticCurveType\x12<\n\x08\x65ncoding\x18\x03 \x01(\x0e\x32*.google.crypto.tink.EcdsaSignatureEncoding\"h\n\x0e\x45\x63\x64saPublicKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12/\n\x06params\x18\x02 \x01(\x0b\x32\x1f.google.crypto.tink.EcdsaParams\x12\t\n\x01x\x18\x03 \x01(\x0c\x12\t\n\x01y\x18\x04 \x01(\x0c\"m\n\x0f\x45\x63\x64saPrivateKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x36\n\npublic_key\x18\x02 \x01(\x0b\x32\".google.crypto.tink.EcdsaPublicKey\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\"R\n\x0e\x45\x63\x64saKeyFormat\x12/\n\x06params\x18\x02 \x01(\x0b\x32\x1f.google.crypto.tink.EcdsaParams\x12\x0f\n\x07version\x18\x03 \x01(\r*G\n\x16\x45\x63\x64saSignatureEncoding\x12\x14\n\x10UNKNOWN_ENCODING\x10\x00\x12\x0e\n\nIEEE_P1363\x10\x01\x12\x07\n\x03\x44\x45R\x10\x02\x42P\n\x1c\x63om.google.crypto.tink.protoP\x01Z.github.com/google/tink/go/proto/ecdsa_go_protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19tink/proto/hkdf_prf.proto\x12\x12google.crypto.tink\x1a\x17tink/proto/common.proto\"I\n\rHkdfPrfParams\x12*\n\x04hash\x18\x01 \x01(\x0e\x32\x1c.google.crypto.tink.HashType\x12\x0c\n\x04salt\x18\x02 \x01(\x0c\"c\n\nHkdfPrfKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x31\n\x06params\x18\x02 \x01(\x0b\x32!.google.crypto.tink.HkdfPrfParams\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\"h\n\x10HkdfPrfKeyFormat\x12\x31\n\x06params\x18\x01 \x01(\x0b\x32!.google.crypto.tink.HkdfPrfParams\x12\x10\n\x08key_size\x18\x02 \x01(\r\x12\x0f\n\x07version\x18\x03 \x01(\rBP\n\x1c\x63om.google.crypto.tink.protoP\x01Z.github.com/google/tink/go/proto/hkdf_prf_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.ecdsa_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.hkdf_prf_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z.github.com/google/tink/go/proto/ecdsa_go_proto'
-  _ECDSASIGNATUREENCODING._serialized_start=553
-  _ECDSASIGNATUREENCODING._serialized_end=624
-  _ECDSAPARAMS._serialized_start=72
-  _ECDSAPARAMS._serialized_end=250
-  _ECDSAPUBLICKEY._serialized_start=252
-  _ECDSAPUBLICKEY._serialized_end=356
-  _ECDSAPRIVATEKEY._serialized_start=358
-  _ECDSAPRIVATEKEY._serialized_end=467
-  _ECDSAKEYFORMAT._serialized_start=469
-  _ECDSAKEYFORMAT._serialized_end=551
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z.github.com/google/tink/go/proto/hkdf_prf_proto'
+  _globals['_HKDFPRFPARAMS']._serialized_start=74
+  _globals['_HKDFPRFPARAMS']._serialized_end=147
+  _globals['_HKDFPRFKEY']._serialized_start=149
+  _globals['_HKDFPRFKEY']._serialized_end=248
+  _globals['_HKDFPRFKEYFORMAT']._serialized_start=250
+  _globals['_HKDFPRFKEYFORMAT']._serialized_end=354
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/ecies_aead_hkdf.proto` & `tink-1.9.0/tink/proto/ecies_aead_hkdf.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/ecies_aead_hkdf_pb2.py` & `tink-1.9.0/tink/proto/ecdsa_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tink/proto/ecies_aead_hkdf.proto
+# source: tink/proto/ecdsa.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from tink.proto import common_pb2 as tink_dot_proto_dot_common__pb2
-from tink.proto import tink_pb2 as tink_dot_proto_dot_tink__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n tink/proto/ecies_aead_hkdf.proto\x12\x12google.crypto.tink\x1a\x17tink/proto/common.proto\x1a\x15tink/proto/tink.proto\"\x98\x01\n\x12\x45\x63iesHkdfKemParams\x12\x39\n\ncurve_type\x18\x01 \x01(\x0e\x32%.google.crypto.tink.EllipticCurveType\x12\x34\n\x0ehkdf_hash_type\x18\x02 \x01(\x0e\x32\x1c.google.crypto.tink.HashType\x12\x11\n\thkdf_salt\x18\x0b \x01(\x0c\"G\n\x12\x45\x63iesAeadDemParams\x12\x31\n\x08\x61\x65\x61\x64_dem\x18\x02 \x01(\x0b\x32\x1f.google.crypto.tink.KeyTemplate\"\xc9\x01\n\x13\x45\x63iesAeadHkdfParams\x12:\n\nkem_params\x18\x01 \x01(\x0b\x32&.google.crypto.tink.EciesHkdfKemParams\x12:\n\ndem_params\x18\x02 \x01(\x0b\x32&.google.crypto.tink.EciesAeadDemParams\x12:\n\x0f\x65\x63_point_format\x18\x03 \x01(\x0e\x32!.google.crypto.tink.EcPointFormat\"x\n\x16\x45\x63iesAeadHkdfPublicKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x37\n\x06params\x18\x02 \x01(\x0b\x32\'.google.crypto.tink.EciesAeadHkdfParams\x12\t\n\x01x\x18\x03 \x01(\x0c\x12\t\n\x01y\x18\x04 \x01(\x0c\"}\n\x17\x45\x63iesAeadHkdfPrivateKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12>\n\npublic_key\x18\x02 \x01(\x0b\x32*.google.crypto.tink.EciesAeadHkdfPublicKey\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\"Q\n\x16\x45\x63iesAeadHkdfKeyFormat\x12\x37\n\x06params\x18\x01 \x01(\x0b\x32\'.google.crypto.tink.EciesAeadHkdfParamsBZ\n\x1c\x63om.google.crypto.tink.protoP\x01Z8github.com/google/tink/go/proto/ecies_aead_hkdf_go_protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16tink/proto/ecdsa.proto\x12\x12google.crypto.tink\x1a\x17tink/proto/common.proto\"\xb2\x01\n\x0b\x45\x63\x64saParams\x12/\n\thash_type\x18\x01 \x01(\x0e\x32\x1c.google.crypto.tink.HashType\x12\x34\n\x05\x63urve\x18\x02 \x01(\x0e\x32%.google.crypto.tink.EllipticCurveType\x12<\n\x08\x65ncoding\x18\x03 \x01(\x0e\x32*.google.crypto.tink.EcdsaSignatureEncoding\"h\n\x0e\x45\x63\x64saPublicKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12/\n\x06params\x18\x02 \x01(\x0b\x32\x1f.google.crypto.tink.EcdsaParams\x12\t\n\x01x\x18\x03 \x01(\x0c\x12\t\n\x01y\x18\x04 \x01(\x0c\"m\n\x0f\x45\x63\x64saPrivateKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x36\n\npublic_key\x18\x02 \x01(\x0b\x32\".google.crypto.tink.EcdsaPublicKey\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\"R\n\x0e\x45\x63\x64saKeyFormat\x12/\n\x06params\x18\x02 \x01(\x0b\x32\x1f.google.crypto.tink.EcdsaParams\x12\x0f\n\x07version\x18\x03 \x01(\r*G\n\x16\x45\x63\x64saSignatureEncoding\x12\x14\n\x10UNKNOWN_ENCODING\x10\x00\x12\x0e\n\nIEEE_P1363\x10\x01\x12\x07\n\x03\x44\x45R\x10\x02\x42P\n\x1c\x63om.google.crypto.tink.protoP\x01Z.github.com/google/tink/go/proto/ecdsa_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.ecies_aead_hkdf_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.ecdsa_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z8github.com/google/tink/go/proto/ecies_aead_hkdf_go_proto'
-  _ECIESHKDFKEMPARAMS._serialized_start=105
-  _ECIESHKDFKEMPARAMS._serialized_end=257
-  _ECIESAEADDEMPARAMS._serialized_start=259
-  _ECIESAEADDEMPARAMS._serialized_end=330
-  _ECIESAEADHKDFPARAMS._serialized_start=333
-  _ECIESAEADHKDFPARAMS._serialized_end=534
-  _ECIESAEADHKDFPUBLICKEY._serialized_start=536
-  _ECIESAEADHKDFPUBLICKEY._serialized_end=656
-  _ECIESAEADHKDFPRIVATEKEY._serialized_start=658
-  _ECIESAEADHKDFPRIVATEKEY._serialized_end=783
-  _ECIESAEADHKDFKEYFORMAT._serialized_start=785
-  _ECIESAEADHKDFKEYFORMAT._serialized_end=866
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z.github.com/google/tink/go/proto/ecdsa_go_proto'
+  _globals['_ECDSASIGNATUREENCODING']._serialized_start=553
+  _globals['_ECDSASIGNATUREENCODING']._serialized_end=624
+  _globals['_ECDSAPARAMS']._serialized_start=72
+  _globals['_ECDSAPARAMS']._serialized_end=250
+  _globals['_ECDSAPUBLICKEY']._serialized_start=252
+  _globals['_ECDSAPUBLICKEY']._serialized_end=356
+  _globals['_ECDSAPRIVATEKEY']._serialized_start=358
+  _globals['_ECDSAPRIVATEKEY']._serialized_end=467
+  _globals['_ECDSAKEYFORMAT']._serialized_start=469
+  _globals['_ECDSAKEYFORMAT']._serialized_end=551
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/ed25519.proto` & `tink-1.9.0/tink/proto/ed25519.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/ed25519_pb2.py` & `tink-1.9.0/tink/proto/prf_based_deriver_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tink/proto/ed25519.proto
+# source: tink/proto/prf_based_deriver.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from tink.proto import tink_pb2 as tink_dot_proto_dot_tink__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18tink/proto/ed25519.proto\x12\x12google.crypto.tink\"#\n\x10\x45\x64\x32\x35\x35\x31\x39KeyFormat\x12\x0f\n\x07version\x18\x01 \x01(\r\"6\n\x10\x45\x64\x32\x35\x35\x31\x39PublicKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x11\n\tkey_value\x18\x02 \x01(\x0c\"q\n\x11\x45\x64\x32\x35\x35\x31\x39PrivateKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x11\n\tkey_value\x18\x02 \x01(\x0c\x12\x38\n\npublic_key\x18\x03 \x01(\x0b\x32$.google.crypto.tink.Ed25519PublicKeyBR\n\x1c\x63om.google.crypto.tink.protoP\x01Z0github.com/google/tink/go/proto/ed25519_go_protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"tink/proto/prf_based_deriver.proto\x12\x12google.crypto.tink\x1a\x15tink/proto/tink.proto\"V\n\x15PrfBasedDeriverParams\x12=\n\x14\x64\x65rived_key_template\x18\x01 \x01(\x0b\x32\x1f.google.crypto.tink.KeyTemplate\"\x90\x01\n\x18PrfBasedDeriverKeyFormat\x12\x39\n\x10prf_key_template\x18\x01 \x01(\x0b\x32\x1f.google.crypto.tink.KeyTemplate\x12\x39\n\x06params\x18\x02 \x01(\x0b\x32).google.crypto.tink.PrfBasedDeriverParams\"\x8e\x01\n\x12PrfBasedDeriverKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12,\n\x07prf_key\x18\x02 \x01(\x0b\x32\x1b.google.crypto.tink.KeyData\x12\x39\n\x06params\x18\x03 \x01(\x0b\x32).google.crypto.tink.PrfBasedDeriverParamsB\\\n\x1c\x63om.google.crypto.tink.protoP\x01Z:github.com/google/tink/go/proto/prf_based_deriver_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.ed25519_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.prf_based_deriver_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z0github.com/google/tink/go/proto/ed25519_go_proto'
-  _ED25519KEYFORMAT._serialized_start=48
-  _ED25519KEYFORMAT._serialized_end=83
-  _ED25519PUBLICKEY._serialized_start=85
-  _ED25519PUBLICKEY._serialized_end=139
-  _ED25519PRIVATEKEY._serialized_start=141
-  _ED25519PRIVATEKEY._serialized_end=254
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z:github.com/google/tink/go/proto/prf_based_deriver_go_proto'
+  _globals['_PRFBASEDDERIVERPARAMS']._serialized_start=81
+  _globals['_PRFBASEDDERIVERPARAMS']._serialized_end=167
+  _globals['_PRFBASEDDERIVERKEYFORMAT']._serialized_start=170
+  _globals['_PRFBASEDDERIVERKEYFORMAT']._serialized_end=314
+  _globals['_PRFBASEDDERIVERKEY']._serialized_start=317
+  _globals['_PRFBASEDDERIVERKEY']._serialized_end=459
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/empty.proto` & `tink-1.9.0/tink/proto/empty.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/empty_pb2.py` & `tink-1.9.0/tink/proto/kms_aead_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tink/proto/empty.proto
+# source: tink/proto/kms_aead.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16tink/proto/empty.proto\x12\x12google.crypto.tink\"\x07\n\x05\x45mptyBP\n\x1c\x63om.google.crypto.tink.protoP\x01Z.github.com/google/tink/go/proto/empty_go_protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19tink/proto/kms_aead.proto\x12\x12google.crypto.tink\"#\n\x10KmsAeadKeyFormat\x12\x0f\n\x07key_uri\x18\x01 \x01(\t\"S\n\nKmsAeadKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x34\n\x06params\x18\x02 \x01(\x0b\x32$.google.crypto.tink.KmsAeadKeyFormatBS\n\x1c\x63om.google.crypto.tink.protoP\x01Z1github.com/google/tink/go/proto/kms_aead_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.empty_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.kms_aead_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z.github.com/google/tink/go/proto/empty_go_proto'
-  _EMPTY._serialized_start=46
-  _EMPTY._serialized_end=53
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z1github.com/google/tink/go/proto/kms_aead_go_proto'
+  _globals['_KMSAEADKEYFORMAT']._serialized_start=49
+  _globals['_KMSAEADKEYFORMAT']._serialized_end=84
+  _globals['_KMSAEADKEY']._serialized_start=86
+  _globals['_KMSAEADKEY']._serialized_end=169
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/hkdf_prf.proto` & `tink-1.9.0/tink/proto/hkdf_prf.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/hkdf_prf_pb2.py` & `tink-1.9.0/tink/proto/jwt_ecdsa_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tink/proto/hkdf_prf.proto
+# source: tink/proto/jwt_ecdsa.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from tink.proto import common_pb2 as tink_dot_proto_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19tink/proto/hkdf_prf.proto\x12\x12google.crypto.tink\x1a\x17tink/proto/common.proto\"I\n\rHkdfPrfParams\x12*\n\x04hash\x18\x01 \x01(\x0e\x32\x1c.google.crypto.tink.HashType\x12\x0c\n\x04salt\x18\x02 \x01(\x0c\"c\n\nHkdfPrfKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x31\n\x06params\x18\x02 \x01(\x0b\x32!.google.crypto.tink.HkdfPrfParams\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\"h\n\x10HkdfPrfKeyFormat\x12\x31\n\x06params\x18\x01 \x01(\x0b\x32!.google.crypto.tink.HkdfPrfParams\x12\x10\n\x08key_size\x18\x02 \x01(\r\x12\x0f\n\x07version\x18\x03 \x01(\rBP\n\x1c\x63om.google.crypto.tink.protoP\x01Z.github.com/google/tink/go/proto/hkdf_prf_protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1atink/proto/jwt_ecdsa.proto\x12\x12google.crypto.tink\"\xd5\x01\n\x11JwtEcdsaPublicKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x38\n\talgorithm\x18\x02 \x01(\x0e\x32%.google.crypto.tink.JwtEcdsaAlgorithm\x12\t\n\x01x\x18\x03 \x01(\x0c\x12\t\n\x01y\x18\x04 \x01(\x0c\x12\x43\n\ncustom_kid\x18\x05 \x01(\x0b\x32/.google.crypto.tink.JwtEcdsaPublicKey.CustomKid\x1a\x1a\n\tCustomKid\x12\r\n\x05value\x18\x01 \x01(\t\"s\n\x12JwtEcdsaPrivateKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x39\n\npublic_key\x18\x02 \x01(\x0b\x32%.google.crypto.tink.JwtEcdsaPublicKey\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\"^\n\x11JwtEcdsaKeyFormat\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x38\n\talgorithm\x18\x02 \x01(\x0e\x32%.google.crypto.tink.JwtEcdsaAlgorithm*D\n\x11JwtEcdsaAlgorithm\x12\x0e\n\nES_UNKNOWN\x10\x00\x12\t\n\x05\x45S256\x10\x01\x12\t\n\x05\x45S384\x10\x02\x12\t\n\x05\x45S512\x10\x03\x42T\n\x1c\x63om.google.crypto.tink.protoP\x01Z2github.com/google/tink/go/proto/jwt_ecdsa_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.hkdf_prf_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.jwt_ecdsa_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z.github.com/google/tink/go/proto/hkdf_prf_proto'
-  _HKDFPRFPARAMS._serialized_start=74
-  _HKDFPRFPARAMS._serialized_end=147
-  _HKDFPRFKEY._serialized_start=149
-  _HKDFPRFKEY._serialized_end=248
-  _HKDFPRFKEYFORMAT._serialized_start=250
-  _HKDFPRFKEYFORMAT._serialized_end=354
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z2github.com/google/tink/go/proto/jwt_ecdsa_go_proto'
+  _globals['_JWTECDSAALGORITHM']._serialized_start=479
+  _globals['_JWTECDSAALGORITHM']._serialized_end=547
+  _globals['_JWTECDSAPUBLICKEY']._serialized_start=51
+  _globals['_JWTECDSAPUBLICKEY']._serialized_end=264
+  _globals['_JWTECDSAPUBLICKEY_CUSTOMKID']._serialized_start=238
+  _globals['_JWTECDSAPUBLICKEY_CUSTOMKID']._serialized_end=264
+  _globals['_JWTECDSAPRIVATEKEY']._serialized_start=266
+  _globals['_JWTECDSAPRIVATEKEY']._serialized_end=381
+  _globals['_JWTECDSAKEYFORMAT']._serialized_start=383
+  _globals['_JWTECDSAKEYFORMAT']._serialized_end=477
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/hmac.proto` & `tink-1.9.0/tink/proto/hmac.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/hmac_pb2.py` & `tink-1.9.0/tink/proto/test_proto_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tink/proto/hmac.proto
+# source: tink/proto/test_proto.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from tink.proto import common_pb2 as tink_dot_proto_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15tink/proto/hmac.proto\x12\x12google.crypto.tink\x1a\x17tink/proto/common.proto\"J\n\nHmacParams\x12*\n\x04hash\x18\x01 \x01(\x0e\x32\x1c.google.crypto.tink.HashType\x12\x10\n\x08tag_size\x18\x02 \x01(\r\"]\n\x07HmacKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12.\n\x06params\x18\x02 \x01(\x0b\x32\x1e.google.crypto.tink.HmacParams\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\"b\n\rHmacKeyFormat\x12.\n\x06params\x18\x01 \x01(\x0b\x32\x1e.google.crypto.tink.HmacParams\x12\x10\n\x08key_size\x18\x02 \x01(\r\x12\x0f\n\x07version\x18\x03 \x01(\rBO\n\x1c\x63om.google.crypto.tink.protoP\x01Z-github.com/google/tink/go/proto/hmac_go_protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1btink/proto/test_proto.proto\x12\x12google.crypto.tink\")\n\tTestProto\x12\x0b\n\x03num\x18\x01 \x01(\x04\x12\x0f\n\x03str\x18\x02 \x01(\x0c\x42\x02\x08\x02\"\x83\x01\n\x0fNestedTestProto\x12(\n\x01\x61\x18\x01 \x01(\x0b\x32\x1d.google.crypto.tink.TestProto\x12(\n\x01\x62\x18\x02 \x01(\x0b\x32\x1d.google.crypto.tink.TestProto\x12\x0b\n\x03num\x18\x03 \x01(\x04\x12\x0f\n\x03str\x18\x04 \x01(\x0c\x42\x02\x08\x02\"$\n\x15TestProtoWithoutCtype\x12\x0b\n\x03str\x18\x01 \x01(\x0c\x42 \n\x1c\x63om.google.crypto.tink.protoP\x01\x62\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.hmac_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.test_proto_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z-github.com/google/tink/go/proto/hmac_go_proto'
-  _HMACPARAMS._serialized_start=70
-  _HMACPARAMS._serialized_end=144
-  _HMACKEY._serialized_start=146
-  _HMACKEY._serialized_end=239
-  _HMACKEYFORMAT._serialized_start=241
-  _HMACKEYFORMAT._serialized_end=339
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001'
+  _globals['_TESTPROTO'].fields_by_name['str']._options = None
+  _globals['_TESTPROTO'].fields_by_name['str']._serialized_options = b'\010\002'
+  _globals['_NESTEDTESTPROTO'].fields_by_name['str']._options = None
+  _globals['_NESTEDTESTPROTO'].fields_by_name['str']._serialized_options = b'\010\002'
+  _globals['_TESTPROTO']._serialized_start=51
+  _globals['_TESTPROTO']._serialized_end=92
+  _globals['_NESTEDTESTPROTO']._serialized_start=95
+  _globals['_NESTEDTESTPROTO']._serialized_end=226
+  _globals['_TESTPROTOWITHOUTCTYPE']._serialized_start=228
+  _globals['_TESTPROTOWITHOUTCTYPE']._serialized_end=264
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/hmac_prf.proto` & `tink-1.9.0/tink/proto/hmac_prf.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/hmac_prf_pb2.py` & `tink-1.9.0/tink/proto/aes_cmac_prf_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tink/proto/hmac_prf.proto
+# source: tink/proto/aes_cmac_prf.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from tink.proto import common_pb2 as tink_dot_proto_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19tink/proto/hmac_prf.proto\x12\x12google.crypto.tink\x1a\x17tink/proto/common.proto\";\n\rHmacPrfParams\x12*\n\x04hash\x18\x01 \x01(\x0e\x32\x1c.google.crypto.tink.HashType\"c\n\nHmacPrfKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x31\n\x06params\x18\x02 \x01(\x0b\x32!.google.crypto.tink.HmacPrfParams\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\"h\n\x10HmacPrfKeyFormat\x12\x31\n\x06params\x18\x01 \x01(\x0b\x32!.google.crypto.tink.HmacPrfParams\x12\x10\n\x08key_size\x18\x02 \x01(\r\x12\x0f\n\x07version\x18\x03 \x01(\rBS\n\x1c\x63om.google.crypto.tink.protoP\x01Z1github.com/google/tink/go/proto/hmac_prf_go_protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dtink/proto/aes_cmac_prf.proto\x12\x12google.crypto.tink\"3\n\rAesCmacPrfKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x11\n\tkey_value\x18\x02 \x01(\x0c\"8\n\x13\x41\x65sCmacPrfKeyFormat\x12\x0f\n\x07version\x18\x02 \x01(\r\x12\x10\n\x08key_size\x18\x01 \x01(\rBW\n\x1c\x63om.google.crypto.tink.protoP\x01Z5github.com/google/tink/go/proto/aes_cmac_prf_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.hmac_prf_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.aes_cmac_prf_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z1github.com/google/tink/go/proto/hmac_prf_go_proto'
-  _HMACPRFPARAMS._serialized_start=74
-  _HMACPRFPARAMS._serialized_end=133
-  _HMACPRFKEY._serialized_start=135
-  _HMACPRFKEY._serialized_end=234
-  _HMACPRFKEYFORMAT._serialized_start=236
-  _HMACPRFKEYFORMAT._serialized_end=340
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z5github.com/google/tink/go/proto/aes_cmac_prf_go_proto'
+  _globals['_AESCMACPRFKEY']._serialized_start=53
+  _globals['_AESCMACPRFKEY']._serialized_end=104
+  _globals['_AESCMACPRFKEYFORMAT']._serialized_start=106
+  _globals['_AESCMACPRFKEYFORMAT']._serialized_end=162
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/hpke.proto` & `tink-1.9.0/tink/proto/hpke.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/hpke_pb2.py` & `tink-1.9.0/tink/proto/ed25519_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tink/proto/hpke.proto
+# source: tink/proto/ed25519.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15tink/proto/hpke.proto\x12\x12google.crypto.tink\"\x8c\x01\n\nHpkeParams\x12(\n\x03kem\x18\x01 \x01(\x0e\x32\x1b.google.crypto.tink.HpkeKem\x12(\n\x03kdf\x18\x02 \x01(\x0e\x32\x1b.google.crypto.tink.HpkeKdf\x12*\n\x04\x61\x65\x61\x64\x18\x03 \x01(\x0e\x32\x1c.google.crypto.tink.HpkeAead\"d\n\rHpkePublicKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12.\n\x06params\x18\x02 \x01(\x0b\x32\x1e.google.crypto.tink.HpkeParams\x12\x12\n\npublic_key\x18\x03 \x01(\x0c\"m\n\x0eHpkePrivateKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x35\n\npublic_key\x18\x02 \x01(\x0b\x32!.google.crypto.tink.HpkePublicKey\x12\x13\n\x0bprivate_key\x18\x03 \x01(\x0c\"?\n\rHpkeKeyFormat\x12.\n\x06params\x18\x01 \x01(\x0b\x32\x1e.google.crypto.tink.HpkeParams*\x8c\x01\n\x07HpkeKem\x12\x0f\n\x0bKEM_UNKNOWN\x10\x00\x12\x1c\n\x18\x44HKEM_X25519_HKDF_SHA256\x10\x01\x12\x1a\n\x16\x44HKEM_P256_HKDF_SHA256\x10\x02\x12\x1a\n\x16\x44HKEM_P384_HKDF_SHA384\x10\x03\x12\x1a\n\x16\x44HKEM_P521_HKDF_SHA512\x10\x04*M\n\x07HpkeKdf\x12\x0f\n\x0bKDF_UNKNOWN\x10\x00\x12\x0f\n\x0bHKDF_SHA256\x10\x01\x12\x0f\n\x0bHKDF_SHA384\x10\x02\x12\x0f\n\x0bHKDF_SHA512\x10\x03*U\n\x08HpkeAead\x12\x10\n\x0c\x41\x45\x41\x44_UNKNOWN\x10\x00\x12\x0f\n\x0b\x41\x45S_128_GCM\x10\x01\x12\x0f\n\x0b\x41\x45S_256_GCM\x10\x02\x12\x15\n\x11\x43HACHA20_POLY1305\x10\x03\x42L\n\x1c\x63om.google.crypto.tink.protoP\x01Z*github.com/google/tink/go/proto/hpke_protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18tink/proto/ed25519.proto\x12\x12google.crypto.tink\"#\n\x10\x45\x64\x32\x35\x35\x31\x39KeyFormat\x12\x0f\n\x07version\x18\x01 \x01(\r\"6\n\x10\x45\x64\x32\x35\x35\x31\x39PublicKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x11\n\tkey_value\x18\x02 \x01(\x0c\"q\n\x11\x45\x64\x32\x35\x35\x31\x39PrivateKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x11\n\tkey_value\x18\x02 \x01(\x0c\x12\x38\n\npublic_key\x18\x03 \x01(\x0b\x32$.google.crypto.tink.Ed25519PublicKeyBR\n\x1c\x63om.google.crypto.tink.protoP\x01Z0github.com/google/tink/go/proto/ed25519_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.hpke_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.ed25519_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z*github.com/google/tink/go/proto/hpke_proto'
-  _HPKEKEM._serialized_start=467
-  _HPKEKEM._serialized_end=607
-  _HPKEKDF._serialized_start=609
-  _HPKEKDF._serialized_end=686
-  _HPKEAEAD._serialized_start=688
-  _HPKEAEAD._serialized_end=773
-  _HPKEPARAMS._serialized_start=46
-  _HPKEPARAMS._serialized_end=186
-  _HPKEPUBLICKEY._serialized_start=188
-  _HPKEPUBLICKEY._serialized_end=288
-  _HPKEPRIVATEKEY._serialized_start=290
-  _HPKEPRIVATEKEY._serialized_end=399
-  _HPKEKEYFORMAT._serialized_start=401
-  _HPKEKEYFORMAT._serialized_end=464
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z0github.com/google/tink/go/proto/ed25519_go_proto'
+  _globals['_ED25519KEYFORMAT']._serialized_start=48
+  _globals['_ED25519KEYFORMAT']._serialized_end=83
+  _globals['_ED25519PUBLICKEY']._serialized_start=85
+  _globals['_ED25519PUBLICKEY']._serialized_end=139
+  _globals['_ED25519PRIVATEKEY']._serialized_start=141
+  _globals['_ED25519PRIVATEKEY']._serialized_end=254
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/jwt_ecdsa.proto` & `tink-1.9.0/tink/proto/jwt_ecdsa.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/jwt_ecdsa_pb2.py` & `tink-1.9.0/tink/proto/kms_envelope_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tink/proto/jwt_ecdsa.proto
+# source: tink/proto/kms_envelope.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from tink.proto import tink_pb2 as tink_dot_proto_dot_tink__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1atink/proto/jwt_ecdsa.proto\x12\x12google.crypto.tink\"\xd5\x01\n\x11JwtEcdsaPublicKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x38\n\talgorithm\x18\x02 \x01(\x0e\x32%.google.crypto.tink.JwtEcdsaAlgorithm\x12\t\n\x01x\x18\x03 \x01(\x0c\x12\t\n\x01y\x18\x04 \x01(\x0c\x12\x43\n\ncustom_kid\x18\x05 \x01(\x0b\x32/.google.crypto.tink.JwtEcdsaPublicKey.CustomKid\x1a\x1a\n\tCustomKid\x12\r\n\x05value\x18\x01 \x01(\t\"s\n\x12JwtEcdsaPrivateKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x39\n\npublic_key\x18\x02 \x01(\x0b\x32%.google.crypto.tink.JwtEcdsaPublicKey\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\"^\n\x11JwtEcdsaKeyFormat\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x38\n\talgorithm\x18\x02 \x01(\x0e\x32%.google.crypto.tink.JwtEcdsaAlgorithm*D\n\x11JwtEcdsaAlgorithm\x12\x0e\n\nES_UNKNOWN\x10\x00\x12\t\n\x05\x45S256\x10\x01\x12\t\n\x05\x45S384\x10\x02\x12\t\n\x05\x45S512\x10\x03\x42T\n\x1c\x63om.google.crypto.tink.protoP\x01Z2github.com/google/tink/go/proto/jwt_ecdsa_go_protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dtink/proto/kms_envelope.proto\x12\x12google.crypto.tink\x1a\x15tink/proto/tink.proto\"b\n\x18KmsEnvelopeAeadKeyFormat\x12\x0f\n\x07kek_uri\x18\x01 \x01(\t\x12\x35\n\x0c\x64\x65k_template\x18\x02 \x01(\x0b\x32\x1f.google.crypto.tink.KeyTemplate\"c\n\x12KmsEnvelopeAeadKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12<\n\x06params\x18\x02 \x01(\x0b\x32,.google.crypto.tink.KmsEnvelopeAeadKeyFormatBW\n\x1c\x63om.google.crypto.tink.protoP\x01Z5github.com/google/tink/go/proto/kms_envelope_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.jwt_ecdsa_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.kms_envelope_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z2github.com/google/tink/go/proto/jwt_ecdsa_go_proto'
-  _JWTECDSAALGORITHM._serialized_start=479
-  _JWTECDSAALGORITHM._serialized_end=547
-  _JWTECDSAPUBLICKEY._serialized_start=51
-  _JWTECDSAPUBLICKEY._serialized_end=264
-  _JWTECDSAPUBLICKEY_CUSTOMKID._serialized_start=238
-  _JWTECDSAPUBLICKEY_CUSTOMKID._serialized_end=264
-  _JWTECDSAPRIVATEKEY._serialized_start=266
-  _JWTECDSAPRIVATEKEY._serialized_end=381
-  _JWTECDSAKEYFORMAT._serialized_start=383
-  _JWTECDSAKEYFORMAT._serialized_end=477
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z5github.com/google/tink/go/proto/kms_envelope_go_proto'
+  _globals['_KMSENVELOPEAEADKEYFORMAT']._serialized_start=76
+  _globals['_KMSENVELOPEAEADKEYFORMAT']._serialized_end=174
+  _globals['_KMSENVELOPEAEADKEY']._serialized_start=176
+  _globals['_KMSENVELOPEAEADKEY']._serialized_end=275
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/jwt_hmac.proto` & `tink-1.9.0/tink/proto/jwt_hmac.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/jwt_hmac_pb2.py` & `tink-1.9.0/tink/proto/jwt_hmac_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: tink/proto/jwt_hmac.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19tink/proto/jwt_hmac.proto\x12\x12google.crypto.tink\"\xc3\x01\n\nJwtHmacKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x37\n\talgorithm\x18\x02 \x01(\x0e\x32$.google.crypto.tink.JwtHmacAlgorithm\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\x12<\n\ncustom_kid\x18\x04 \x01(\x0b\x32(.google.crypto.tink.JwtHmacKey.CustomKid\x1a\x1a\n\tCustomKid\x12\r\n\x05value\x18\x01 \x01(\t\"n\n\x10JwtHmacKeyFormat\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x37\n\talgorithm\x18\x02 \x01(\x0e\x32$.google.crypto.tink.JwtHmacAlgorithm\x12\x10\n\x08key_size\x18\x03 \x01(\r*C\n\x10JwtHmacAlgorithm\x12\x0e\n\nHS_UNKNOWN\x10\x00\x12\t\n\x05HS256\x10\x01\x12\t\n\x05HS384\x10\x02\x12\t\n\x05HS512\x10\x03\x42S\n\x1c\x63om.google.crypto.tink.protoP\x01Z1github.com/google/tink/go/proto/jwt_hmac_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.jwt_hmac_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.jwt_hmac_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z1github.com/google/tink/go/proto/jwt_hmac_go_proto'
-  _JWTHMACALGORITHM._serialized_start=359
-  _JWTHMACALGORITHM._serialized_end=426
-  _JWTHMACKEY._serialized_start=50
-  _JWTHMACKEY._serialized_end=245
-  _JWTHMACKEY_CUSTOMKID._serialized_start=219
-  _JWTHMACKEY_CUSTOMKID._serialized_end=245
-  _JWTHMACKEYFORMAT._serialized_start=247
-  _JWTHMACKEYFORMAT._serialized_end=357
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z1github.com/google/tink/go/proto/jwt_hmac_go_proto'
+  _globals['_JWTHMACALGORITHM']._serialized_start=359
+  _globals['_JWTHMACALGORITHM']._serialized_end=426
+  _globals['_JWTHMACKEY']._serialized_start=50
+  _globals['_JWTHMACKEY']._serialized_end=245
+  _globals['_JWTHMACKEY_CUSTOMKID']._serialized_start=219
+  _globals['_JWTHMACKEY_CUSTOMKID']._serialized_end=245
+  _globals['_JWTHMACKEYFORMAT']._serialized_start=247
+  _globals['_JWTHMACKEYFORMAT']._serialized_end=357
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/jwt_rsa_ssa_pkcs1.proto` & `tink-1.9.0/tink/proto/jwt_rsa_ssa_pkcs1.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/jwt_rsa_ssa_pkcs1_pb2.py` & `tink-1.9.0/tink/proto/jwt_rsa_ssa_pkcs1_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: tink/proto/jwt_rsa_ssa_pkcs1.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"tink/proto/jwt_rsa_ssa_pkcs1.proto\x12\x12google.crypto.tink\"\xe7\x01\n\x17JwtRsaSsaPkcs1PublicKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12>\n\talgorithm\x18\x02 \x01(\x0e\x32+.google.crypto.tink.JwtRsaSsaPkcs1Algorithm\x12\t\n\x01n\x18\x03 \x01(\x0c\x12\t\n\x01\x65\x18\x04 \x01(\x0c\x12I\n\ncustom_kid\x18\x05 \x01(\x0b\x32\x35.google.crypto.tink.JwtRsaSsaPkcs1PublicKey.CustomKid\x1a\x1a\n\tCustomKid\x12\r\n\x05value\x18\x01 \x01(\t\"\xb2\x01\n\x18JwtRsaSsaPkcs1PrivateKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12?\n\npublic_key\x18\x02 \x01(\x0b\x32+.google.crypto.tink.JwtRsaSsaPkcs1PublicKey\x12\t\n\x01\x64\x18\x03 \x01(\x0c\x12\t\n\x01p\x18\x04 \x01(\x0c\x12\t\n\x01q\x18\x05 \x01(\x0c\x12\n\n\x02\x64p\x18\x06 \x01(\x0c\x12\n\n\x02\x64q\x18\x07 \x01(\x0c\x12\x0b\n\x03\x63rt\x18\x08 \x01(\x0c\"\xa1\x01\n\x17JwtRsaSsaPkcs1KeyFormat\x12\x0f\n\x07version\x18\x01 \x01(\r\x12>\n\talgorithm\x18\x02 \x01(\x0e\x32+.google.crypto.tink.JwtRsaSsaPkcs1Algorithm\x12\x1c\n\x14modulus_size_in_bits\x18\x03 \x01(\r\x12\x17\n\x0fpublic_exponent\x18\x04 \x01(\x0c*J\n\x17JwtRsaSsaPkcs1Algorithm\x12\x0e\n\nRS_UNKNOWN\x10\x00\x12\t\n\x05RS256\x10\x01\x12\t\n\x05RS384\x10\x02\x12\t\n\x05RS512\x10\x03\x42X\n\x1c\x63om.google.crypto.tink.protoP\x01Z6github.com/google/tink/go/proto/rsa_ssa_pkcs1_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.jwt_rsa_ssa_pkcs1_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.jwt_rsa_ssa_pkcs1_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z6github.com/google/tink/go/proto/rsa_ssa_pkcs1_go_proto'
-  _JWTRSASSAPKCS1ALGORITHM._serialized_start=637
-  _JWTRSASSAPKCS1ALGORITHM._serialized_end=711
-  _JWTRSASSAPKCS1PUBLICKEY._serialized_start=59
-  _JWTRSASSAPKCS1PUBLICKEY._serialized_end=290
-  _JWTRSASSAPKCS1PUBLICKEY_CUSTOMKID._serialized_start=264
-  _JWTRSASSAPKCS1PUBLICKEY_CUSTOMKID._serialized_end=290
-  _JWTRSASSAPKCS1PRIVATEKEY._serialized_start=293
-  _JWTRSASSAPKCS1PRIVATEKEY._serialized_end=471
-  _JWTRSASSAPKCS1KEYFORMAT._serialized_start=474
-  _JWTRSASSAPKCS1KEYFORMAT._serialized_end=635
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z6github.com/google/tink/go/proto/rsa_ssa_pkcs1_go_proto'
+  _globals['_JWTRSASSAPKCS1ALGORITHM']._serialized_start=637
+  _globals['_JWTRSASSAPKCS1ALGORITHM']._serialized_end=711
+  _globals['_JWTRSASSAPKCS1PUBLICKEY']._serialized_start=59
+  _globals['_JWTRSASSAPKCS1PUBLICKEY']._serialized_end=290
+  _globals['_JWTRSASSAPKCS1PUBLICKEY_CUSTOMKID']._serialized_start=264
+  _globals['_JWTRSASSAPKCS1PUBLICKEY_CUSTOMKID']._serialized_end=290
+  _globals['_JWTRSASSAPKCS1PRIVATEKEY']._serialized_start=293
+  _globals['_JWTRSASSAPKCS1PRIVATEKEY']._serialized_end=471
+  _globals['_JWTRSASSAPKCS1KEYFORMAT']._serialized_start=474
+  _globals['_JWTRSASSAPKCS1KEYFORMAT']._serialized_end=635
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/jwt_rsa_ssa_pss.proto` & `tink-1.9.0/tink/proto/jwt_rsa_ssa_pss.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/jwt_rsa_ssa_pss_pb2.py` & `tink-1.9.0/tink/proto/jwt_rsa_ssa_pss_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: tink/proto/jwt_rsa_ssa_pss.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n tink/proto/jwt_rsa_ssa_pss.proto\x12\x12google.crypto.tink\"\xe1\x01\n\x15JwtRsaSsaPssPublicKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12<\n\talgorithm\x18\x02 \x01(\x0e\x32).google.crypto.tink.JwtRsaSsaPssAlgorithm\x12\t\n\x01n\x18\x03 \x01(\x0c\x12\t\n\x01\x65\x18\x04 \x01(\x0c\x12G\n\ncustom_kid\x18\x05 \x01(\x0b\x32\x33.google.crypto.tink.JwtRsaSsaPssPublicKey.CustomKid\x1a\x1a\n\tCustomKid\x12\r\n\x05value\x18\x01 \x01(\t\"\xae\x01\n\x16JwtRsaSsaPssPrivateKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12=\n\npublic_key\x18\x02 \x01(\x0b\x32).google.crypto.tink.JwtRsaSsaPssPublicKey\x12\t\n\x01\x64\x18\x03 \x01(\x0c\x12\t\n\x01p\x18\x04 \x01(\x0c\x12\t\n\x01q\x18\x05 \x01(\x0c\x12\n\n\x02\x64p\x18\x06 \x01(\x0c\x12\n\n\x02\x64q\x18\x07 \x01(\x0c\x12\x0b\n\x03\x63rt\x18\x08 \x01(\x0c\"\x9d\x01\n\x15JwtRsaSsaPssKeyFormat\x12\x0f\n\x07version\x18\x01 \x01(\r\x12<\n\talgorithm\x18\x02 \x01(\x0e\x32).google.crypto.tink.JwtRsaSsaPssAlgorithm\x12\x1c\n\x14modulus_size_in_bits\x18\x03 \x01(\r\x12\x17\n\x0fpublic_exponent\x18\x04 \x01(\x0c*H\n\x15JwtRsaSsaPssAlgorithm\x12\x0e\n\nPS_UNKNOWN\x10\x00\x12\t\n\x05PS256\x10\x01\x12\t\n\x05PS384\x10\x02\x12\t\n\x05PS512\x10\x03\x42Z\n\x1c\x63om.google.crypto.tink.protoP\x01Z8github.com/google/tink/go/proto/jwt_rsa_ssa_pss_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.jwt_rsa_ssa_pss_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.jwt_rsa_ssa_pss_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z8github.com/google/tink/go/proto/jwt_rsa_ssa_pss_go_proto'
-  _JWTRSASSAPSSALGORITHM._serialized_start=621
-  _JWTRSASSAPSSALGORITHM._serialized_end=693
-  _JWTRSASSAPSSPUBLICKEY._serialized_start=57
-  _JWTRSASSAPSSPUBLICKEY._serialized_end=282
-  _JWTRSASSAPSSPUBLICKEY_CUSTOMKID._serialized_start=256
-  _JWTRSASSAPSSPUBLICKEY_CUSTOMKID._serialized_end=282
-  _JWTRSASSAPSSPRIVATEKEY._serialized_start=285
-  _JWTRSASSAPSSPRIVATEKEY._serialized_end=459
-  _JWTRSASSAPSSKEYFORMAT._serialized_start=462
-  _JWTRSASSAPSSKEYFORMAT._serialized_end=619
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z8github.com/google/tink/go/proto/jwt_rsa_ssa_pss_go_proto'
+  _globals['_JWTRSASSAPSSALGORITHM']._serialized_start=621
+  _globals['_JWTRSASSAPSSALGORITHM']._serialized_end=693
+  _globals['_JWTRSASSAPSSPUBLICKEY']._serialized_start=57
+  _globals['_JWTRSASSAPSSPUBLICKEY']._serialized_end=282
+  _globals['_JWTRSASSAPSSPUBLICKEY_CUSTOMKID']._serialized_start=256
+  _globals['_JWTRSASSAPSSPUBLICKEY_CUSTOMKID']._serialized_end=282
+  _globals['_JWTRSASSAPSSPRIVATEKEY']._serialized_start=285
+  _globals['_JWTRSASSAPSSPRIVATEKEY']._serialized_end=459
+  _globals['_JWTRSASSAPSSKEYFORMAT']._serialized_start=462
+  _globals['_JWTRSASSAPSSKEYFORMAT']._serialized_end=619
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/kms_aead.proto` & `tink-1.9.0/tink/proto/kms_aead.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/kms_envelope.proto` & `tink-1.9.0/tink/proto/kms_envelope.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/kms_envelope_pb2.py` & `tink-1.9.0/tink/proto/hpke_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tink/proto/kms_envelope.proto
+# source: tink/proto/hpke.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from tink.proto import tink_pb2 as tink_dot_proto_dot_tink__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dtink/proto/kms_envelope.proto\x12\x12google.crypto.tink\x1a\x15tink/proto/tink.proto\"b\n\x18KmsEnvelopeAeadKeyFormat\x12\x0f\n\x07kek_uri\x18\x01 \x01(\t\x12\x35\n\x0c\x64\x65k_template\x18\x02 \x01(\x0b\x32\x1f.google.crypto.tink.KeyTemplate\"c\n\x12KmsEnvelopeAeadKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12<\n\x06params\x18\x02 \x01(\x0b\x32,.google.crypto.tink.KmsEnvelopeAeadKeyFormatBW\n\x1c\x63om.google.crypto.tink.protoP\x01Z5github.com/google/tink/go/proto/kms_envelope_go_protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15tink/proto/hpke.proto\x12\x12google.crypto.tink\"\x8c\x01\n\nHpkeParams\x12(\n\x03kem\x18\x01 \x01(\x0e\x32\x1b.google.crypto.tink.HpkeKem\x12(\n\x03kdf\x18\x02 \x01(\x0e\x32\x1b.google.crypto.tink.HpkeKdf\x12*\n\x04\x61\x65\x61\x64\x18\x03 \x01(\x0e\x32\x1c.google.crypto.tink.HpkeAead\"d\n\rHpkePublicKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12.\n\x06params\x18\x02 \x01(\x0b\x32\x1e.google.crypto.tink.HpkeParams\x12\x12\n\npublic_key\x18\x03 \x01(\x0c\"m\n\x0eHpkePrivateKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x35\n\npublic_key\x18\x02 \x01(\x0b\x32!.google.crypto.tink.HpkePublicKey\x12\x13\n\x0bprivate_key\x18\x03 \x01(\x0c\"?\n\rHpkeKeyFormat\x12.\n\x06params\x18\x01 \x01(\x0b\x32\x1e.google.crypto.tink.HpkeParams*\x8c\x01\n\x07HpkeKem\x12\x0f\n\x0bKEM_UNKNOWN\x10\x00\x12\x1c\n\x18\x44HKEM_X25519_HKDF_SHA256\x10\x01\x12\x1a\n\x16\x44HKEM_P256_HKDF_SHA256\x10\x02\x12\x1a\n\x16\x44HKEM_P384_HKDF_SHA384\x10\x03\x12\x1a\n\x16\x44HKEM_P521_HKDF_SHA512\x10\x04*M\n\x07HpkeKdf\x12\x0f\n\x0bKDF_UNKNOWN\x10\x00\x12\x0f\n\x0bHKDF_SHA256\x10\x01\x12\x0f\n\x0bHKDF_SHA384\x10\x02\x12\x0f\n\x0bHKDF_SHA512\x10\x03*U\n\x08HpkeAead\x12\x10\n\x0c\x41\x45\x41\x44_UNKNOWN\x10\x00\x12\x0f\n\x0b\x41\x45S_128_GCM\x10\x01\x12\x0f\n\x0b\x41\x45S_256_GCM\x10\x02\x12\x15\n\x11\x43HACHA20_POLY1305\x10\x03\x42L\n\x1c\x63om.google.crypto.tink.protoP\x01Z*github.com/google/tink/go/proto/hpke_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.kms_envelope_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.hpke_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z5github.com/google/tink/go/proto/kms_envelope_go_proto'
-  _KMSENVELOPEAEADKEYFORMAT._serialized_start=76
-  _KMSENVELOPEAEADKEYFORMAT._serialized_end=174
-  _KMSENVELOPEAEADKEY._serialized_start=176
-  _KMSENVELOPEAEADKEY._serialized_end=275
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z*github.com/google/tink/go/proto/hpke_proto'
+  _globals['_HPKEKEM']._serialized_start=467
+  _globals['_HPKEKEM']._serialized_end=607
+  _globals['_HPKEKDF']._serialized_start=609
+  _globals['_HPKEKDF']._serialized_end=686
+  _globals['_HPKEAEAD']._serialized_start=688
+  _globals['_HPKEAEAD']._serialized_end=773
+  _globals['_HPKEPARAMS']._serialized_start=46
+  _globals['_HPKEPARAMS']._serialized_end=186
+  _globals['_HPKEPUBLICKEY']._serialized_start=188
+  _globals['_HPKEPUBLICKEY']._serialized_end=288
+  _globals['_HPKEPRIVATEKEY']._serialized_start=290
+  _globals['_HPKEPRIVATEKEY']._serialized_end=399
+  _globals['_HPKEKEYFORMAT']._serialized_start=401
+  _globals['_HPKEKEYFORMAT']._serialized_end=464
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/prf_based_deriver.proto` & `tink-1.9.0/tink/proto/prf_based_deriver.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/prf_based_deriver_pb2.py` & `tink-1.9.0/tink/proto/xchacha20_poly1305_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tink/proto/prf_based_deriver.proto
+# source: tink/proto/xchacha20_poly1305.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from tink.proto import tink_pb2 as tink_dot_proto_dot_tink__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"tink/proto/prf_based_deriver.proto\x12\x12google.crypto.tink\x1a\x15tink/proto/tink.proto\"V\n\x15PrfBasedDeriverParams\x12=\n\x14\x64\x65rived_key_template\x18\x01 \x01(\x0b\x32\x1f.google.crypto.tink.KeyTemplate\"\x90\x01\n\x18PrfBasedDeriverKeyFormat\x12\x39\n\x10prf_key_template\x18\x01 \x01(\x0b\x32\x1f.google.crypto.tink.KeyTemplate\x12\x39\n\x06params\x18\x02 \x01(\x0b\x32).google.crypto.tink.PrfBasedDeriverParams\"\x8e\x01\n\x12PrfBasedDeriverKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12,\n\x07prf_key\x18\x02 \x01(\x0b\x32\x1b.google.crypto.tink.KeyData\x12\x39\n\x06params\x18\x03 \x01(\x0b\x32).google.crypto.tink.PrfBasedDeriverParamsB\\\n\x1c\x63om.google.crypto.tink.protoP\x01Z:github.com/google/tink/go/proto/prf_based_deriver_go_protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#tink/proto/xchacha20_poly1305.proto\x12\x12google.crypto.tink\"-\n\x1aXChaCha20Poly1305KeyFormat\x12\x0f\n\x07version\x18\x01 \x01(\r\":\n\x14XChaCha20Poly1305Key\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x11\n\tkey_value\x18\x03 \x01(\x0c\x42]\n\x1c\x63om.google.crypto.tink.protoP\x01Z;github.com/google/tink/go/proto/xchacha20_poly1305_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.prf_based_deriver_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.xchacha20_poly1305_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z:github.com/google/tink/go/proto/prf_based_deriver_go_proto'
-  _PRFBASEDDERIVERPARAMS._serialized_start=81
-  _PRFBASEDDERIVERPARAMS._serialized_end=167
-  _PRFBASEDDERIVERKEYFORMAT._serialized_start=170
-  _PRFBASEDDERIVERKEYFORMAT._serialized_end=314
-  _PRFBASEDDERIVERKEY._serialized_start=317
-  _PRFBASEDDERIVERKEY._serialized_end=459
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z;github.com/google/tink/go/proto/xchacha20_poly1305_go_proto'
+  _globals['_XCHACHA20POLY1305KEYFORMAT']._serialized_start=59
+  _globals['_XCHACHA20POLY1305KEYFORMAT']._serialized_end=104
+  _globals['_XCHACHA20POLY1305KEY']._serialized_start=106
+  _globals['_XCHACHA20POLY1305KEY']._serialized_end=164
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/rsa_ssa_pkcs1.proto` & `tink-1.9.0/tink/proto/rsa_ssa_pkcs1.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/rsa_ssa_pkcs1_pb2.py` & `tink-1.9.0/tink/proto/rsa_ssa_pkcs1_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: tink/proto/rsa_ssa_pkcs1.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from tink.proto import common_pb2 as tink_dot_proto_dot_common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1etink/proto/rsa_ssa_pkcs1.proto\x12\x12google.crypto.tink\x1a\x17tink/proto/common.proto\"D\n\x11RsaSsaPkcs1Params\x12/\n\thash_type\x18\x01 \x01(\x0e\x32\x1c.google.crypto.tink.HashType\"t\n\x14RsaSsaPkcs1PublicKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x35\n\x06params\x18\x02 \x01(\x0b\x32%.google.crypto.tink.RsaSsaPkcs1Params\x12\t\n\x01n\x18\x03 \x01(\x0c\x12\t\n\x01\x65\x18\x04 \x01(\x0c\"\xac\x01\n\x15RsaSsaPkcs1PrivateKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12<\n\npublic_key\x18\x02 \x01(\x0b\x32(.google.crypto.tink.RsaSsaPkcs1PublicKey\x12\t\n\x01\x64\x18\x03 \x01(\x0c\x12\t\n\x01p\x18\x04 \x01(\x0c\x12\t\n\x01q\x18\x05 \x01(\x0c\x12\n\n\x02\x64p\x18\x06 \x01(\x0c\x12\n\n\x02\x64q\x18\x07 \x01(\x0c\x12\x0b\n\x03\x63rt\x18\x08 \x01(\x0c\"\x84\x01\n\x14RsaSsaPkcs1KeyFormat\x12\x35\n\x06params\x18\x01 \x01(\x0b\x32%.google.crypto.tink.RsaSsaPkcs1Params\x12\x1c\n\x14modulus_size_in_bits\x18\x02 \x01(\r\x12\x17\n\x0fpublic_exponent\x18\x03 \x01(\x0c\x42X\n\x1c\x63om.google.crypto.tink.protoP\x01Z6github.com/google/tink/go/proto/rsa_ssa_pkcs1_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.rsa_ssa_pkcs1_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.rsa_ssa_pkcs1_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z6github.com/google/tink/go/proto/rsa_ssa_pkcs1_go_proto'
-  _RSASSAPKCS1PARAMS._serialized_start=79
-  _RSASSAPKCS1PARAMS._serialized_end=147
-  _RSASSAPKCS1PUBLICKEY._serialized_start=149
-  _RSASSAPKCS1PUBLICKEY._serialized_end=265
-  _RSASSAPKCS1PRIVATEKEY._serialized_start=268
-  _RSASSAPKCS1PRIVATEKEY._serialized_end=440
-  _RSASSAPKCS1KEYFORMAT._serialized_start=443
-  _RSASSAPKCS1KEYFORMAT._serialized_end=575
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z6github.com/google/tink/go/proto/rsa_ssa_pkcs1_go_proto'
+  _globals['_RSASSAPKCS1PARAMS']._serialized_start=79
+  _globals['_RSASSAPKCS1PARAMS']._serialized_end=147
+  _globals['_RSASSAPKCS1PUBLICKEY']._serialized_start=149
+  _globals['_RSASSAPKCS1PUBLICKEY']._serialized_end=265
+  _globals['_RSASSAPKCS1PRIVATEKEY']._serialized_start=268
+  _globals['_RSASSAPKCS1PRIVATEKEY']._serialized_end=440
+  _globals['_RSASSAPKCS1KEYFORMAT']._serialized_start=443
+  _globals['_RSASSAPKCS1KEYFORMAT']._serialized_end=575
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/rsa_ssa_pss.proto` & `tink-1.9.0/tink/proto/rsa_ssa_pss.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/rsa_ssa_pss_pb2.py` & `tink-1.9.0/tink/proto/rsa_ssa_pss_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: tink/proto/rsa_ssa_pss.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from tink.proto import common_pb2 as tink_dot_proto_dot_common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ctink/proto/rsa_ssa_pss.proto\x12\x12google.crypto.tink\x1a\x17tink/proto/common.proto\"\x87\x01\n\x0fRsaSsaPssParams\x12.\n\x08sig_hash\x18\x01 \x01(\x0e\x32\x1c.google.crypto.tink.HashType\x12/\n\tmgf1_hash\x18\x02 \x01(\x0e\x32\x1c.google.crypto.tink.HashType\x12\x13\n\x0bsalt_length\x18\x03 \x01(\x05\"p\n\x12RsaSsaPssPublicKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x33\n\x06params\x18\x02 \x01(\x0b\x32#.google.crypto.tink.RsaSsaPssParams\x12\t\n\x01n\x18\x03 \x01(\x0c\x12\t\n\x01\x65\x18\x04 \x01(\x0c\"\xa8\x01\n\x13RsaSsaPssPrivateKey\x12\x0f\n\x07version\x18\x01 \x01(\r\x12:\n\npublic_key\x18\x02 \x01(\x0b\x32&.google.crypto.tink.RsaSsaPssPublicKey\x12\t\n\x01\x64\x18\x03 \x01(\x0c\x12\t\n\x01p\x18\x04 \x01(\x0c\x12\t\n\x01q\x18\x05 \x01(\x0c\x12\n\n\x02\x64p\x18\x06 \x01(\x0c\x12\n\n\x02\x64q\x18\x07 \x01(\x0c\x12\x0b\n\x03\x63rt\x18\x08 \x01(\x0c\"\x80\x01\n\x12RsaSsaPssKeyFormat\x12\x33\n\x06params\x18\x01 \x01(\x0b\x32#.google.crypto.tink.RsaSsaPssParams\x12\x1c\n\x14modulus_size_in_bits\x18\x02 \x01(\r\x12\x17\n\x0fpublic_exponent\x18\x03 \x01(\x0c\x42V\n\x1c\x63om.google.crypto.tink.protoP\x01Z4github.com/google/tink/go/proto/rsa_ssa_pss_go_protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.rsa_ssa_pss_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.rsa_ssa_pss_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z4github.com/google/tink/go/proto/rsa_ssa_pss_go_proto'
-  _RSASSAPSSPARAMS._serialized_start=78
-  _RSASSAPSSPARAMS._serialized_end=213
-  _RSASSAPSSPUBLICKEY._serialized_start=215
-  _RSASSAPSSPUBLICKEY._serialized_end=327
-  _RSASSAPSSPRIVATEKEY._serialized_start=330
-  _RSASSAPSSPRIVATEKEY._serialized_end=498
-  _RSASSAPSSKEYFORMAT._serialized_start=501
-  _RSASSAPSSKEYFORMAT._serialized_end=629
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z4github.com/google/tink/go/proto/rsa_ssa_pss_go_proto'
+  _globals['_RSASSAPSSPARAMS']._serialized_start=78
+  _globals['_RSASSAPSSPARAMS']._serialized_end=213
+  _globals['_RSASSAPSSPUBLICKEY']._serialized_start=215
+  _globals['_RSASSAPSSPUBLICKEY']._serialized_end=327
+  _globals['_RSASSAPSSPRIVATEKEY']._serialized_start=330
+  _globals['_RSASSAPSSPRIVATEKEY']._serialized_end=498
+  _globals['_RSASSAPSSKEYFORMAT']._serialized_start=501
+  _globals['_RSASSAPSSKEYFORMAT']._serialized_end=629
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/test_proto.proto` & `tink-1.9.0/tink/proto/test_proto.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/tink.proto` & `tink-1.9.0/tink/proto/tink.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/proto/tink_pb2.py` & `tink-1.9.0/tink/proto/tink_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: tink/proto/tink.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15tink/proto/tink.proto\x12\x12google.crypto.tink\"p\n\x0bKeyTemplate\x12\x10\n\x08type_url\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c\x12@\n\x12output_prefix_type\x18\x03 \x01(\x0e\x32$.google.crypto.tink.OutputPrefixType\"\xec\x01\n\x07KeyData\x12\x10\n\x08type_url\x18\x01 \x01(\t\x12\x11\n\x05value\x18\x02 \x01(\x0c\x42\x02\x08\x02\x12\x46\n\x11key_material_type\x18\x03 \x01(\x0e\x32+.google.crypto.tink.KeyData.KeyMaterialType\"t\n\x0fKeyMaterialType\x12\x17\n\x13UNKNOWN_KEYMATERIAL\x10\x00\x12\r\n\tSYMMETRIC\x10\x01\x12\x16\n\x12\x41SYMMETRIC_PRIVATE\x10\x02\x12\x15\n\x11\x41SYMMETRIC_PUBLIC\x10\x03\x12\n\n\x06REMOTE\x10\x04\"\x89\x02\n\x06Keyset\x12\x16\n\x0eprimary_key_id\x18\x01 \x01(\r\x12+\n\x03key\x18\x02 \x03(\x0b\x32\x1e.google.crypto.tink.Keyset.Key\x1a\xb9\x01\n\x03Key\x12-\n\x08key_data\x18\x01 \x01(\x0b\x32\x1b.google.crypto.tink.KeyData\x12\x31\n\x06status\x18\x02 \x01(\x0e\x32!.google.crypto.tink.KeyStatusType\x12\x0e\n\x06key_id\x18\x03 \x01(\r\x12@\n\x12output_prefix_type\x18\x04 \x01(\x0e\x32$.google.crypto.tink.OutputPrefixType\"\x81\x02\n\nKeysetInfo\x12\x16\n\x0eprimary_key_id\x18\x01 \x01(\r\x12\x38\n\x08key_info\x18\x02 \x03(\x0b\x32&.google.crypto.tink.KeysetInfo.KeyInfo\x1a\xa0\x01\n\x07KeyInfo\x12\x10\n\x08type_url\x18\x01 \x01(\t\x12\x31\n\x06status\x18\x02 \x01(\x0e\x32!.google.crypto.tink.KeyStatusType\x12\x0e\n\x06key_id\x18\x03 \x01(\r\x12@\n\x12output_prefix_type\x18\x04 \x01(\x0e\x32$.google.crypto.tink.OutputPrefixType\"`\n\x0f\x45ncryptedKeyset\x12\x18\n\x10\x65ncrypted_keyset\x18\x02 \x01(\x0c\x12\x33\n\x0bkeyset_info\x18\x03 \x01(\x0b\x32\x1e.google.crypto.tink.KeysetInfo*M\n\rKeyStatusType\x12\x12\n\x0eUNKNOWN_STATUS\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\r\n\tDESTROYED\x10\x03*R\n\x10OutputPrefixType\x12\x12\n\x0eUNKNOWN_PREFIX\x10\x00\x12\x08\n\x04TINK\x10\x01\x12\n\n\x06LEGACY\x10\x02\x12\x07\n\x03RAW\x10\x03\x12\x0b\n\x07\x43RUNCHY\x10\x04\x42X\n\x1c\x63om.google.crypto.tink.protoP\x01Z-github.com/google/tink/go/proto/tink_go_proto\xa2\x02\x06TINKPBb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.tink_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tink.proto.tink_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z-github.com/google/tink/go/proto/tink_go_proto\242\002\006TINKPB'
-  _KEYDATA.fields_by_name['value']._options = None
-  _KEYDATA.fields_by_name['value']._serialized_options = b'\010\002'
-  _KEYSTATUSTYPE._serialized_start=1024
-  _KEYSTATUSTYPE._serialized_end=1101
-  _OUTPUTPREFIXTYPE._serialized_start=1103
-  _OUTPUTPREFIXTYPE._serialized_end=1185
-  _KEYTEMPLATE._serialized_start=45
-  _KEYTEMPLATE._serialized_end=157
-  _KEYDATA._serialized_start=160
-  _KEYDATA._serialized_end=396
-  _KEYDATA_KEYMATERIALTYPE._serialized_start=280
-  _KEYDATA_KEYMATERIALTYPE._serialized_end=396
-  _KEYSET._serialized_start=399
-  _KEYSET._serialized_end=664
-  _KEYSET_KEY._serialized_start=479
-  _KEYSET_KEY._serialized_end=664
-  _KEYSETINFO._serialized_start=667
-  _KEYSETINFO._serialized_end=924
-  _KEYSETINFO_KEYINFO._serialized_start=764
-  _KEYSETINFO_KEYINFO._serialized_end=924
-  _ENCRYPTEDKEYSET._serialized_start=926
-  _ENCRYPTEDKEYSET._serialized_end=1022
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z-github.com/google/tink/go/proto/tink_go_proto\242\002\006TINKPB'
+  _globals['_KEYDATA'].fields_by_name['value']._options = None
+  _globals['_KEYDATA'].fields_by_name['value']._serialized_options = b'\010\002'
+  _globals['_KEYSTATUSTYPE']._serialized_start=1024
+  _globals['_KEYSTATUSTYPE']._serialized_end=1101
+  _globals['_OUTPUTPREFIXTYPE']._serialized_start=1103
+  _globals['_OUTPUTPREFIXTYPE']._serialized_end=1185
+  _globals['_KEYTEMPLATE']._serialized_start=45
+  _globals['_KEYTEMPLATE']._serialized_end=157
+  _globals['_KEYDATA']._serialized_start=160
+  _globals['_KEYDATA']._serialized_end=396
+  _globals['_KEYDATA_KEYMATERIALTYPE']._serialized_start=280
+  _globals['_KEYDATA_KEYMATERIALTYPE']._serialized_end=396
+  _globals['_KEYSET']._serialized_start=399
+  _globals['_KEYSET']._serialized_end=664
+  _globals['_KEYSET_KEY']._serialized_start=479
+  _globals['_KEYSET_KEY']._serialized_end=664
+  _globals['_KEYSETINFO']._serialized_start=667
+  _globals['_KEYSETINFO']._serialized_end=924
+  _globals['_KEYSETINFO_KEYINFO']._serialized_start=764
+  _globals['_KEYSETINFO_KEYINFO']._serialized_end=924
+  _globals['_ENCRYPTEDKEYSET']._serialized_start=926
+  _globals['_ENCRYPTEDKEYSET']._serialized_end=1022
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.8.0/tink/proto/xchacha20_poly1305.proto` & `tink-1.9.0/tink/proto/xchacha20_poly1305.proto`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/secret_key_access.py` & `tink-1.9.0/tink/secret_key_access.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/secret_key_access_test.py` & `tink-1.9.0/tink/secret_key_access_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/signature/BUILD.bazel` & `tink-1.9.0/tink/signature/BUILD.bazel`

 * *Files 5% similar despite different names*

```diff
@@ -62,15 +62,14 @@
 py_library(
     name = "_signature_wrapper",
     srcs = ["_signature_wrapper.py"],
     srcs_version = "PY3",
     deps = [
         ":_public_key_sign",
         ":_public_key_verify",
-        requirement("absl-py"),
         "//tink/core",
         "//tink/proto:tink_py_pb2",
     ],
 )
 
 py_test(
     name = "_signature_wrapper_test",
```

### Comparing `tink-1.8.0/tink/signature/__init__.py` & `tink-1.9.0/tink/signature/__init__.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/signature/_public_key_sign.py` & `tink-1.9.0/tink/signature/_public_key_sign.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/signature/_public_key_verify.py` & `tink-1.9.0/tink/signature/_public_key_verify.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/signature/_signature_key_manager.py` & `tink-1.9.0/tink/signature/_signature_key_manager.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/signature/_signature_key_manager_test.py` & `tink-1.9.0/tink/signature/_signature_key_manager_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/signature/_signature_key_templates.py` & `tink-1.9.0/tink/signature/_signature_key_templates.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/signature/_signature_wrapper.py` & `tink-1.9.0/tink/signature/_signature_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Public Key Sign wrapper."""
 
 from typing import Type
-from absl import logging
 
 from tink.proto import tink_pb2
 from tink import core
 from tink.signature import _public_key_sign
 from tink.signature import _public_key_verify
 
 
@@ -99,17 +98,16 @@
       try:
         if entry.output_prefix_type == tink_pb2.LEGACY:
           entry.primitive.verify(raw_sig, data + b'\x00')
         else:
           entry.primitive.verify(raw_sig, data)
         # Signature is valid, we can return
         return
-      except core.TinkError as err:
-        logging.info('signature prefix matches a key, but cannot verify: %s',
-                     err)
+      except core.TinkError:
+        pass
 
     # No matching key succeeded with verification, try all RAW keys
     for entry in self._primitive_set.raw_primitives():
       try:
         entry.primitive.verify(signature, data)
         # Signature is valid, we can return
         return
```

### Comparing `tink-1.8.0/tink/signature/_signature_wrapper_test.py` & `tink-1.9.0/tink/signature/_signature_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/streaming_aead/BUILD.bazel` & `tink-1.9.0/tink/streaming_aead/BUILD.bazel`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
     name = "_streaming_aead_wrapper_test",
     timeout = "short",
     srcs = ["_streaming_aead_wrapper_test.py"],
     srcs_version = "PY3",
     deps = [
         ":streaming_aead",
         requirement("absl-py"),
-        "//tink:cleartext_keyset_handle",
+        "//tink:secret_key_access",
         "//tink:tink_python",
         "//tink/proto:aes_gcm_hkdf_streaming_py_pb2",
         "//tink/proto:common_py_pb2",
         "//tink/proto:tink_py_pb2",
         "//tink/testing:bytes_io",
         "//tink/testing:keyset_builder",
     ],
```

### Comparing `tink-1.8.0/tink/streaming_aead/__init__.py` & `tink-1.9.0/tink/streaming_aead/__init__.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/streaming_aead/_decrypting_stream.py` & `tink-1.9.0/tink/streaming_aead/_decrypting_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 """A file-like object that decrypts the data it reads.
 
 It reads the ciphertext from a given other file-like object, and decrypts it.
 """
 
 import io
-from typing import BinaryIO
+from typing import BinaryIO, Optional
 
 from tink import core
 from tink.cc.pybind import tink_bindings
 from tink.streaming_aead import _file_object_adapter
 
 
 class RawDecryptingStream(io.RawIOBase):
@@ -62,15 +62,15 @@
         cc_primitive, aad, source)
 
   @core.use_tink_errors
   def _read_from_input_stream_adapter(self, size: int) -> bytes:
     """Implemented as a separate method to ensure correct error transform."""
     return self._input_stream_adapter.read(size)
 
-  def read(self, size=-1) -> bytes:
+  def read(self, size: Optional[int] = -1) -> bytes:
     """Read and return up to size bytes, where size is an int.
 
     It blocks until at least one byte can be returned.
 
     Args:
       size: Maximum number of bytes to read. As a convenience, if size is
       unspecified or -1, all bytes until EOF are returned.
```

### Comparing `tink-1.8.0/tink/streaming_aead/_decrypting_stream_test.py` & `tink-1.9.0/tink/streaming_aead/_decrypting_stream_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/streaming_aead/_encrypting_stream.py` & `tink-1.9.0/tink/streaming_aead/_encrypting_stream.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/streaming_aead/_encrypting_stream_test.py` & `tink-1.9.0/tink/streaming_aead/_encrypting_stream_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/streaming_aead/_file_object_adapter.py` & `tink-1.9.0/tink/streaming_aead/_file_object_adapter.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/streaming_aead/_file_object_adapter_test.py` & `tink-1.9.0/tink/streaming_aead/_file_object_adapter_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/streaming_aead/_pybind11_python_file_object_adapter_test.py` & `tink-1.9.0/tink/streaming_aead/_pybind11_python_file_object_adapter_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/streaming_aead/_raw_streaming_aead.py` & `tink-1.9.0/tink/streaming_aead/_raw_streaming_aead.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/streaming_aead/_rewindable_input_stream.py` & `tink-1.9.0/tink/streaming_aead/_rewindable_input_stream.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/streaming_aead/_rewindable_input_stream_test.py` & `tink-1.9.0/tink/streaming_aead/_rewindable_input_stream_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/streaming_aead/_streaming_aead.py` & `tink-1.9.0/tink/streaming_aead/_streaming_aead.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/streaming_aead/_streaming_aead_key_manager.py` & `tink-1.9.0/tink/streaming_aead/_streaming_aead_key_manager.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/streaming_aead/_streaming_aead_key_manager_test.py` & `tink-1.9.0/tink/streaming_aead/_streaming_aead_key_manager_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/streaming_aead/_streaming_aead_key_templates.py` & `tink-1.9.0/tink/streaming_aead/_streaming_aead_key_templates.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/streaming_aead/_streaming_aead_key_templates_test.py` & `tink-1.9.0/tink/streaming_aead/_streaming_aead_key_templates_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/streaming_aead/_streaming_aead_test.py` & `tink-1.9.0/tink/streaming_aead/_streaming_aead_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/streaming_aead/_streaming_aead_wrapper.py` & `tink-1.9.0/tink/streaming_aead/_streaming_aead_wrapper.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/streaming_aead/_streaming_aead_wrapper_test.py` & `tink-1.9.0/tink/streaming_aead/_streaming_aead_wrapper_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from tink.proto import aes_gcm_hkdf_streaming_pb2
 from tink.proto import common_pb2
 from tink.proto import tink_pb2
 import tink
-from tink import cleartext_keyset_handle
+from tink import secret_key_access
 from tink import streaming_aead
 from tink.testing import bytes_io
 from tink.testing import keyset_builder
 
 
 TEMPLATE = streaming_aead.streaming_aead_key_templates.AES128_GCM_HKDF_4KB
 TYPE_URL = 'type.googleapis.com/google.crypto.tink.AesGcmHkdfStreamingKey'
@@ -264,15 +264,17 @@
                 output_prefix_type=tink_pb2.OutputPrefixType.RAW,
                 status=tink_pb2.KeyStatusType.ENABLED,
                 key_id=2,
             ),
         ],
     )
 
-    keyset_handle = cleartext_keyset_handle.from_keyset(keyset)
+    keyset_handle = tink.proto_keyset_format.parse(
+        keyset.SerializeToString(), secret_key_access.TOKEN
+    )
     primitive = keyset_handle.primitive(streaming_aead.StreamingAead)
 
     plaintext = b'plaintext'
     associated_data = b'associated_data'
 
     ciphertext_dest = bytes_io.BytesIOWithValueAfterClose()
     with primitive.new_encrypting_stream(
```

### Comparing `tink-1.8.0/tink/testing/BUILD.bazel` & `tink-1.9.0/tink/testing/BUILD.bazel`

 * *Files 10% similar despite different names*

```diff
@@ -80,18 +80,17 @@
 
 py_library(
     name = "fake_kms",
     testonly = 1,
     srcs = ["fake_kms.py"],
     srcs_version = "PY3",
     deps = [
-        "//tink:cleartext_keyset_handle",
+        "//tink:secret_key_access",
         "//tink:tink_python",
         "//tink/aead",
-        "//tink/aead:_kms_aead_key_manager",
         "//tink/core",
     ],
 )
 
 py_test(
     name = "fake_kms_test",
     srcs = ["fake_kms_test.py"],
```

### Comparing `tink-1.8.0/tink/testing/__init__.py` & `tink-1.9.0/tink/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/testing/bytes_io.py` & `tink-1.9.0/tink/testing/bytes_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,16 @@
   """A readable BytesIO that raised BlockingIOError on some calls to read."""
 
   def __init__(self, data: bytes, seekable: bool = False):
     super().__init__(data)
     self._seekable = seekable
     self._state = -1
 
-  def read(self, size: int = -1) -> bytes:
-    if size > 0:
+  def read(self, size: Optional[int] = -1) -> bytes:
+    if size and size > 0:
       self._state += 1
       if self._state > 10000000:
         raise AssertionError('too many read. Is there an infinite loop?')
       if self._state % 3 == 0:   # block on every third call.
         raise io.BlockingIOError(
             errno.EAGAIN,
             'write could not complete without blocking', 0)
```

### Comparing `tink-1.8.0/tink/testing/bytes_io_test.py` & `tink-1.9.0/tink/testing/bytes_io_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/testing/fake_kms.py` & `tink-1.9.0/tink/testing/fake_kms.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,27 +10,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """A client for Fake KMS."""
 
 import base64
-
 from typing import Optional
 
 import tink
 from tink import aead
-from tink import cleartext_keyset_handle
-from tink.aead import _kms_aead_key_manager
+from tink import secret_key_access
 
 
 FAKE_KMS_PREFIX = 'fake-kms://'
 
 
-class FakeKmsClient(_kms_aead_key_manager.KmsClient):
+class FakeKmsClient(tink.KmsClient):
   """A fake KMS client."""
 
   def __init__(self, key_uri: Optional[str] = None):
     if not key_uri:
       self._key_uri = None
     elif key_uri.startswith(FAKE_KMS_PREFIX):
       self._key_uri = key_uri
@@ -45,17 +43,17 @@
     return key_uri == self._key_uri
 
   def get_aead(self, key_uri: str) -> aead.Aead:
     if not key_uri.startswith(FAKE_KMS_PREFIX):
       raise tink.TinkError('invalid key URI')
     key_id = key_uri[len(FAKE_KMS_PREFIX) :]
     serialized_key = base64.urlsafe_b64decode(key_id.encode('utf-8') + b'===')
-    handle = cleartext_keyset_handle.read(
-        tink.BinaryKeysetReader(serialized_key)
+    handle = tink.proto_keyset_format.parse(
+        serialized_key, secret_key_access.TOKEN
     )
     return handle.primitive(aead.Aead)
 
 
 def register_client(key_uri=None, credentials_path=None) -> None:
   """Registers a fake KMS client."""
   _ = credentials_path
-  _kms_aead_key_manager.register_kms_client(FakeKmsClient(key_uri))
+  tink.register_kms_client(FakeKmsClient(key_uri))
```

### Comparing `tink-1.8.0/tink/testing/fake_kms_test.py` & `tink-1.9.0/tink/testing/fake_kms_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/testing/helper.py` & `tink-1.9.0/tink/testing/helper.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/testing/helper_test.py` & `tink-1.9.0/tink/testing/helper_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/testing/keyset_builder.py` & `tink-1.9.0/tink/testing/keyset_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Python implementation of a KeysetBuilder."""
 
-import io
 import random
 from tink.proto import tink_pb2
 import tink
-from tink import cleartext_keyset_handle
+from tink import secret_key_access
 
 _MAX_INT32 = 4294967295  # 2^32-1
 
 
 def _new_key_data(key_template: tink_pb2.KeyTemplate) -> tink_pb2.KeyData:
   return tink.core.Registry.new_key_data(key_template)
 
@@ -54,27 +53,24 @@
   The validity of the keyset is checked when creating a keyset_handle.
   """
 
   def __init__(self, keyset_proto: tink_pb2.Keyset):
     self._keyset = keyset_proto
 
   def keyset_handle(self) -> tink.KeysetHandle:
-    keyset_copy = tink_pb2.Keyset()
-    keyset_copy.CopyFrom(self._keyset)
-    return cleartext_keyset_handle.from_keyset(keyset_copy)
+    return tink.proto_keyset_format.parse(
+        self._keyset.SerializeToString(), secret_key_access.TOKEN
+    )
 
   def keyset(self) -> bytes:
     return self._keyset.SerializeToString()
 
   def public_keyset(self) -> bytes:
     public_handle = self.keyset_handle().public_keyset_handle()
-    public_keyset = io.BytesIO()
-    writer = tink.BinaryKeysetWriter(public_keyset)
-    cleartext_keyset_handle.write(writer, public_handle)
-    return public_keyset.getvalue()
+    return tink.proto_keyset_format.serialize_without_secret(public_handle)
 
   def add_new_key(self, key_template: tink_pb2.KeyTemplate) -> int:
     """Generates a new key, adds it to the keyset, and returns its ID."""
     new_key = self._keyset.key.add()
     new_key.key_data.CopyFrom(_new_key_data(key_template))
     new_key.status = tink_pb2.ENABLED
     new_key_id = _generate_unused_key_id(self._keyset)
@@ -119,15 +115,15 @@
   """Return a KeysetBuilder for a Keyset copied from a KeysetHandle."""
   keyset_proto = tink_pb2.Keyset.FromString(keyset)
   return KeysetBuilder(keyset_proto)
 
 
 def from_keyset_handle(keyset_handle: tink.KeysetHandle) -> KeysetBuilder:
   """Return a KeysetBuilder for a Keyset copied from a KeysetHandle."""
-  keyset_buffer = io.BytesIO()
-  cleartext_keyset_handle.write(
-      tink.BinaryKeysetWriter(keyset_buffer), keyset_handle)
-  return from_keyset(keyset_buffer.getvalue())
+  serialized_keyset = tink.proto_keyset_format.serialize(
+      keyset_handle, secret_key_access.TOKEN
+  )
+  return from_keyset(serialized_keyset)
 
 
 def new_keyset_builder() -> KeysetBuilder:
   return KeysetBuilder(tink_pb2.Keyset())
```

### Comparing `tink-1.8.0/tink/testing/keyset_builder_test.py` & `tink-1.9.0/tink/testing/keyset_builder_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/tink_config.py` & `tink-1.9.0/tink/tink_config.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink/tink_config_test.py` & `tink-1.9.0/tink/tink_config_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tink.egg-info/PKG-INFO` & `tink-1.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,39 @@
 Metadata-Version: 2.1
 Name: tink
-Version: 1.8.0
+Version: 1.9.0
 Summary: A multi-language, cross-platform library that provides cryptographic APIs that are secure, easy to use correctly, and hard(er) to misuse.
 Home-page: https://github.com/tink-crypto/tink-py
 Author: Tink Developers
 Author-email: tink-users@googlegroups.com
 License: Apache 2.0
 Keywords: tink cryptography
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: absl-py>=1.3.0
+Requires-Dist: protobuf!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0.dev0,>=3.20.2
+Provides-Extra: gcpkms
+Requires-Dist: google-auth>=2.16.2; extra == "gcpkms"
+Requires-Dist: google-api-core>=2.11.0; extra == "gcpkms"
+Requires-Dist: google-cloud-kms>=2.16.1; extra == "gcpkms"
+Provides-Extra: awskms
+Requires-Dist: boto3>=1.26.89; extra == "awskms"
+Provides-Extra: all
+Requires-Dist: google-auth>=2.16.2; extra == "all"
+Requires-Dist: google-api-core>=2.11.0; extra == "all"
+Requires-Dist: google-cloud-kms>=2.16.1; extra == "all"
+Requires-Dist: boto3>=1.26.89; extra == "all"
 
 # Tink Python
 
 <!-- GCP Ubuntu --->
 
 [tink_py_bazel_badge_gcp_ubuntu]: https://storage.googleapis.com/tink-kokoro-build-badges/tink-py-bazel-gcp-ubuntu.svg
 [tink_py_bazel_kms_badge_gcp_ubuntu]: https://storage.googleapis.com/tink-kokoro-build-badges/tink-py-bazel-kms-gcp-ubuntu.svg
```

### Comparing `tink-1.8.0/tink.egg-info/SOURCES.txt` & `tink-1.9.0/tink.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,36 @@
 BUILD.bazel
 LICENSE
 MANIFEST.in
 README.md
 VERSION
 WORKSPACE
 requirements.in
-requirements.txt
+requirements_all.txt
+requirements_awskms.in
+requirements_gcpkms.in
 setup.py
 tink_py_deps.bzl
 tink_py_deps_init.bzl
 tink/BUILD.bazel
 tink/__init__.py
+tink/_insecure_keyset_handle.py
+tink/_insecure_keyset_handle_test.py
+tink/_json_proto_keyset_format.py
+tink/_json_proto_keyset_format_test.py
 tink/_keyset_handle.py
 tink/_keyset_handle_test.py
 tink/_keyset_reader.py
 tink/_keyset_reader_test.py
 tink/_keyset_writer.py
 tink/_keyset_writer_test.py
+tink/_kms_clients.py
+tink/_kms_clients_test.py
+tink/_proto_keyset_format.py
+tink/_proto_keyset_format_test.py
 tink/cleartext_keyset_handle.py
 tink/cleartext_keyset_handle_test.py
 tink/secret_key_access.py
 tink/secret_key_access_test.py
 tink/tink_config.py
 tink/tink_config_test.py
 tink.egg-info/PKG-INFO
```

### Comparing `tink-1.8.0/tink_py_deps.bzl` & `tink-1.9.0/tink_py_deps.bzl`

 * *Files 8% similar despite different names*

```diff
@@ -4,35 +4,35 @@
 
 def tink_py_deps():
     """Loads dependencies of tink-py."""
     if not native.existing_rule("google_root_pem"):
         http_file(
             name = "google_root_pem",
             executable = 0,
+            sha256 = "1acf0d4780541758be2c0f998e1e0275232626ed3f8793d8e2fe8e2753750613",
             urls = ["https://pki.goog/roots.pem"],
-            sha256 = "9c9b9685ad319b9747c3fe69b46a61c11a0efabdfa09ca6a8b0c3da421036d27",
         )
 
     if not native.existing_rule("bazel_skylib"):
         http_archive(
             name = "bazel_skylib",
-            sha256 = "66ffd9315665bfaafc96b52278f57c7e2dd09f5ede279ea6d39b2be471e7e3aa",
+            sha256 = "cd55a062e763b9349921f0f5db8c3933288dc8ba4f76dd9416aac68acee3cb94",
             urls = [
-                "https://mirror.bazel.build/github.com/bazelbuild/bazel-skylib/releases/download/1.4.2/bazel-skylib-1.4.2.tar.gz",
-                "https://github.com/bazelbuild/bazel-skylib/releases/download/1.4.2/bazel-skylib-1.4.2.tar.gz",
+                "https://mirror.bazel.build/github.com/bazelbuild/bazel-skylib/releases/download/1.5.0/bazel-skylib-1.5.0.tar.gz",
+                "https://github.com/bazelbuild/bazel-skylib/releases/download/1.5.0/bazel-skylib-1.5.0.tar.gz",
             ],
         )
 
     if not native.existing_rule("com_google_protobuf"):
-        # Release X.21.9 from 2022-10-26.
+        # Release X.25.1 from 2023-11-15.
         http_archive(
             name = "com_google_protobuf",
-            strip_prefix = "protobuf-21.9",
-            urls = ["https://github.com/protocolbuffers/protobuf/archive/refs/tags/v21.9.zip"],
-            sha256 = "5babb8571f1cceafe0c18e13ddb3be556e87e12ceea3463d6b0d0064e6cc1ac3",
+            sha256 = "5c86c077b0794c3e9bb30cac872cf883043febfb0f992137f0a8b1c3d534617c",
+            strip_prefix = "protobuf-25.1",
+            urls = ["https://github.com/protocolbuffers/protobuf/releases/download/v25.1/protobuf-25.1.zip"],
         )
 
     if not native.existing_rule("rules_python"):
         # Release from 2023-07-12
         http_archive(
             name = "rules_python",
             sha256 = "0a8003b044294d7840ac7d9d73eef05d6ceb682d7516781a4ec62eeb34702578",
@@ -58,11 +58,11 @@
             url = "https://github.com/pybind/pybind11_bazel/archive/refs/tags/v2.11.1.tar.gz",
             sha256 = "e8355ee56c2ff772334b4bfa22be17c709e5573f6d1d561c7176312156c27bd4",
         )
 
     if not native.existing_rule("tink_cc"):
         http_archive(
             name = "tink_cc",
-            urls = ["https://github.com/tink-crypto/tink-cc/archive/refs/tags/v2.0.0.zip"],
-            strip_prefix = "tink-cc-2.0.0",
-            sha256 = "103ddfce800e77f3b3b6b2c808a8611bc734b31ddb12fbcfd8bebc1b96a7e963",
+            urls = ["https://github.com/tink-crypto/tink-cc/releases/download/v2.1.0/tink-cc-2.1.0.zip"],
+            strip_prefix = "tink-cc-2.1.0",
+            sha256 = "3804afecbe7096d3786b660e9cd5f365f064743eec52d76984abb9da38dd0fb3",
         )
```

### Comparing `tink-1.8.0/tink_py_deps_init.bzl` & `tink-1.9.0/tink_py_deps_init.bzl`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Initialization of tink-py dependencies."""
 
+load("@pybind11_bazel//:python_configure.bzl", "python_configure")
+load("@rules_python//python:pip.bzl", "pip_parse")
 load("@tink_cc//:tink_cc_deps.bzl", "tink_cc_deps")
 load("@tink_cc//:tink_cc_deps_init.bzl", "tink_cc_deps_init")
-load("@rules_python//python:pip.bzl", "pip_parse")
-load("@pybind11_bazel//:python_configure.bzl", "python_configure")
 
 def tink_py_deps_init(workspace_name):
     tink_cc_deps()
 
     tink_cc_deps_init()
 
     pip_parse(
         name = "tink_py_pip_deps",
+        extra_pip_args = ["--no-deps"],
         quiet = False,
-        requirements_lock = "@" + workspace_name + "//:requirements.txt",
+        requirements_lock = "@" + workspace_name + "//:requirements_all.txt",
     )
 
     # Use `which python3` by default [1] unless PYTHON_BIN_PATH is specified [2].
     #
     # [1] https://github.com/pybind/pybind11_bazel/blob/fc56ce8a8b51e3dd941139d329b63ccfea1d304b/python_configure.bzl#L434
     # [2] https://github.com/pybind/pybind11_bazel/blob/fc56ce8a8b51e3dd941139d329b63ccfea1d304b/python_configure.bzl#L162
     python_configure(name = "local_config_python", python_version = "3")
```

### Comparing `tink-1.8.0/tools/distribution/build_linux_binary_wheels.sh` & `tink-1.9.0/tools/distribution/build_linux_binary_wheels.sh`

 * *Files 10% similar despite different names*

```diff
@@ -19,49 +19,50 @@
 # environment setup.
 
 set -euo pipefail
 
 # The following assoicative array contains:
 #   ["<Python version>"]="<python tag>-<abi tag>"
 # where:
-#   <Python version> = language version, e.g "3.7"
+#   <Python version> = language version, e.g "3.8"
 #   <python tag>, <abi tag> = as defined at
-#       https://packaging.python.org/en/latest/specifications/, e.g. "cp37-37m"
+#       https://packaging.python.org/en/latest/specifications/, e.g. "cp38-cp38"
 declare -A PYTHON_VERSIONS
-PYTHON_VERSIONS["3.7"]="cp37-cp37m"
 PYTHON_VERSIONS["3.8"]="cp38-cp38"
 PYTHON_VERSIONS["3.9"]="cp39-cp39"
 PYTHON_VERSIONS["3.10"]="cp310-cp310"
 PYTHON_VERSIONS["3.11"]="cp311-cp311"
 readonly -A PYTHON_VERSIONS
 
 export TINK_PYTHON_ROOT_PATH="${PWD}"
 export ARCH="$(uname -m)"
 
 # Install Bazelisk 1.17.0.
 readonly BAZELISK_VERSION="1.17.0"
-BAZELISK_URL="https://github.com/bazelbuild/bazelisk/releases/download/v${BAZELISK_VERSION}/bazelisk-linux-amd64"
+readonly BAZELISK_DOWNLOAD_URL="https://github.com/bazelbuild/bazelisk/releases/download"
+BAZELISK_URL="${BAZELISK_DOWNLOAD_URL}/v${BAZELISK_VERSION}/bazelisk-linux-amd64"
 BAZELISK_SHA256="61699e22abb2a26304edfa1376f65ad24191f94a4ffed68a58d42b6fee01e124"
 if [[ "${ARCH}" == "aarch64" || "${ARCH}" == "arm64" ]]; then
-  BAZELISK_URL="https://github.com/bazelbuild/bazelisk/releases/download/v${BAZELISK_VERSION}/bazelisk-linux-arm64"
+  BAZELISK_URL="${BAZELISK_DOWNLOAD_URL}/v${BAZELISK_VERSION}/bazelisk-linux-arm64"
   BAZELISK_SHA256="a836972b8a7c34970fb9ecc44768ece172f184c5f7e2972c80033fcdcf8c1870"
 fi
 readonly BAZELISK_URL
 readonly BAZELISK_SHA256
 curl -LsS "${BAZELISK_URL}" -o /usr/local/bin/bazelisk
 echo "${BAZELISK_SHA256} /usr/local/bin/bazelisk" | sha256sum -c
 chmod +x /usr/local/bin/bazelisk
 
 # Install protoc 21.12 (python version 4.21.12). Needed for protocol buffer
 # compilation.
+readonly PROTOC_DOWNLOAD_URL="https://github.com/protocolbuffers/protobuf/releases/download"
 readonly PROTOC_RELEASE_TAG="21.12"
-PROTOC_URL="https://github.com/protocolbuffers/protobuf/releases/download/v${PROTOC_RELEASE_TAG}/protoc-${PROTOC_RELEASE_TAG}-linux-x86_64.zip"
+PROTOC_URL="${PROTOC_DOWNLOAD_URL}/v${PROTOC_RELEASE_TAG}/protoc-${PROTOC_RELEASE_TAG}-linux-x86_64.zip"
 PROTOC_SHA256="3a4c1e5f2516c639d3079b1586e703fc7bcfa2136d58bda24d1d54f949c315e8"
 if [[ "${ARCH}" == "aarch64" || "${ARCH}" == "arm64" ]]; then
-  PROTOC_URL="https://github.com/protocolbuffers/protobuf/releases/download/v${PROTOC_RELEASE_TAG}/protoc-${PROTOC_RELEASE_TAG}-linux-aarch_64.zip"
+  PROTOC_URL="${PROTOC_DOWNLOAD_URL}/v${PROTOC_RELEASE_TAG}/protoc-${PROTOC_RELEASE_TAG}-linux-aarch_64.zip"
   PROTOC_SHA256="2dd17f75d66a682640b136e31848da9fb2eefe68d55303baf8b32617374f6711"
 fi
 readonly PROTOC_URL
 readonly PROTOC_SHA256
 curl -LsS "${PROTOC_URL}" -o protoc.zip
 echo "${PROTOC_SHA256} protoc.zip" | sha256sum -c
 unzip -o protoc.zip -d /usr/local bin/protoc
```

### Comparing `tink-1.8.0/tools/distribution/create_bdist.sh` & `tink-1.9.0/tools/distribution/create_bdist.sh`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # limitations under the License.
 ################################################################################
 
 # This script creates binary wheels for Tink Python for Linux and macOS.
 
 set -eEuox pipefail
 
-readonly PYTHON_VERSIONS=( "3.7" "3.8" "3.9" "3.10" "3.11" )
+readonly PYTHON_VERSIONS=( "3.8" "3.9" "3.10" "3.11" )
 
 readonly PLATFORM="$(uname | tr '[:upper:]' '[:lower:]')"
 
 export TINK_PYTHON_ROOT_PATH="${PWD}"
 
 readonly MANYLINUX_X86_64_IMAGE_NAME="quay.io/pypa/manylinux2014_x86_64"
 readonly MANYLINUX_X86_64_IMAGE_SHA256="sha256:2f9e5abda045d41f5418216fe7601cf12249989b9aba0a83d009b8cc434cb220"
```

### Comparing `tink-1.8.0/tools/distribution/create_sdist.sh` & `tink-1.9.0/tools/distribution/create_sdist.sh`

 * *Files identical despite different names*

### Comparing `tink-1.8.0/tools/distribution/test_linux_binary_wheel.sh` & `tink-1.9.0/tools/distribution/test_linux_binary_wheel.sh`

 * *Files 7% similar despite different names*

```diff
@@ -44,15 +44,14 @@
   exit 1
 }
 
 get_python_and_abi() {
   local -r wheel_file="$1"
   # The Python tag and ABI are defined here
   # https://packaging.python.org/en/latest/specifications/. Examples are:
-  #   - cp37-cp37m
   #   - cp38-cp38
   #   - cp39-cp39
   #   - cp310-cp310
   #   - cp311-cp311
   echo "${wheel_file}" | grep -oEi 'cp[0-9]{2,}-cp[0-9]{2,}m?'
 }
 
@@ -75,14 +74,14 @@
 
   local -r python_tag="$(get_python_and_abi "${BINARY_WHEEL_FILE}")"
   export PATH="${PATH}:/opt/python/${python_tag}/bin"
   export TINK_PYTHON_ROOT_PATH="${PWD}"
   # Required to fix https://github.com/pypa/manylinux/issues/357.
   export LD_LIBRARY_PATH="/usr/local/lib"
 
-  python3 -m pip install --require-hashes -r requirements.txt
-  python3 -m pip install --no-deps --no-index "${BINARY_WHEEL_FILE}"
+  python3 -m pip install --require-hashes --no-deps -r requirements_all.txt
+  python3 -m pip install --no-deps --no-index "${BINARY_WHEEL_FILE}[all]"
   find tink/ "${test_ignore_paths[@]}" -type f -name "*_test.py" -print0 \
     | xargs -0 -n1 python3
 }
 
 main "$@"
```

