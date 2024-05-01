# Comparing `tmp/flwr_nightly-1.9.0.dev20240429.tar.gz` & `tmp/flwr_nightly-1.9.0.dev20240430.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.9.0.dev20240429.tar", max compression
+gzip compressed data, was "flwr_nightly-1.9.0.dev20240430.tar", max compression
```

## Comparing `flwr_nightly-1.9.0.dev20240429.tar` & `flwr_nightly-1.9.0.dev20240430.tar`

### file list

```diff
@@ -1,216 +1,216 @@
--rw-r--r--   0        0        0    11358 2024-04-29 23:05:13.919324 flwr_nightly-1.9.0.dev20240429/LICENSE
--rw-r--r--   0        0        0    12916 2024-04-29 23:05:13.919324 flwr_nightly-1.9.0.dev20240429/README.md
--rw-r--r--   0        0        0     5776 2024-04-29 23:05:30.539412 flwr_nightly-1.9.0.dev20240429/pyproject.toml
--rw-r--r--   0        0        0      937 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/__init__.py
--rw-r--r--   0        0        0      720 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/__init__.py
--rw-r--r--   0        0        0     1095 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/app.py
--rw-r--r--   0        0        0     4899 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/config_utils.py
--rw-r--r--   0        0        0     2215 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/example.py
--rw-r--r--   0        0        0      789 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/__init__.py
--rw-r--r--   0        0        0     5989 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/new.py
--rw-r--r--   0        0        0      725 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/__init__.py
--rw-r--r--   0        0        0     3078 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/.gitignore.tpl
--rw-r--r--   0        0        0      667 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/README.md.tpl
--rw-r--r--   0        0        0      729 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/__init__.py
--rw-r--r--   0        0        0      736 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/__init__.py
--rw-r--r--   0        0        0       21 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
--rw-r--r--   0        0        0      521 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
--rw-r--r--   0        0        0     1172 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
--rw-r--r--   0        0        0     2801 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl
--rw-r--r--   0        0        0     1911 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
--rw-r--r--   0        0        0      248 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
--rw-r--r--   0        0        0      593 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
--rw-r--r--   0        0        0      341 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/server.sklearn.py.tpl
--rw-r--r--   0        0        0      371 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
--rw-r--r--   0        0        0     3684 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
--rw-r--r--   0        0        0      521 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
--rw-r--r--   0        0        0      590 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
--rw-r--r--   0        0        0      570 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl
--rw-r--r--   0        0        0      569 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
--rw-r--r--   0        0        0      789 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/run/__init__.py
--rw-r--r--   0        0        0     2334 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/run/run.py
--rw-r--r--   0        0        0     4119 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/utils.py
--rw-r--r--   0        0        0     1268 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    22313 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     8183 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     8636 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/client_app.py
--rw-r--r--   0        0        0     7435 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      735 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     8993 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      752 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     4761 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/grpc_rere_client/client_interceptor.py
--rw-r--r--   0        0        0     9597 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0     2404 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/heartbeat.py
--rw-r--r--   0        0        0      719 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     6553 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1824 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     1143 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/__init__.py
--rw-r--r--   0        0        0     5397 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/centraldp_mods.py
--rw-r--r--   0        0        0     2623 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/comms_mods.py
--rw-r--r--   0        0        0     4918 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/localdp_mod.py
--rw-r--r--   0        0        0      849 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     1095 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
--rw-r--r--   0        0        0    19699 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
--rw-r--r--   0        0        0     1226 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/utils.py
--rw-r--r--   0        0        0     1778 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/node_state.py
--rw-r--r--   0        0        0     2195 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/node_state_tests.py
--rw-r--r--   0        0        0    10283 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      735 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0    11520 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0      865 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/supernode/__init__.py
--rw-r--r--   0        0        0     9052 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/supernode/app.py
--rw-r--r--   0        0        0     1006 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/typing.py
--rw-r--r--   0        0        0     3721 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1882 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     2424 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0     1313 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/context.py
--rw-r--r--   0        0        0      891 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     6113 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/differential_privacy.py
--rw-r--r--   0        0        0     1074 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/differential_privacy_constants.py
--rw-r--r--   0        0        0     2004 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     2812 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/exit_handlers.py
--rw-r--r--   0        0        0     2460 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     6096 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0    12385 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/message.py
--rw-r--r--   0        0        0     4961 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/object_ref.py
--rw-r--r--   0        0        0     2095 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0     1385 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/pyproject.py
--rw-r--r--   0        0        0     1054 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/__init__.py
--rw-r--r--   0        0        0     4652 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/configsrecord.py
--rw-r--r--   0        0        0     1393 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/conversion_utils.py
--rw-r--r--   0        0        0     3923 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/metricsrecord.py
--rw-r--r--   0        0        0     4849 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/parametersrecord.py
--rw-r--r--   0        0        0     4553 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/recordset.py
--rw-r--r--   0        0        0     3879 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/typeddict.py
--rw-r--r--   0        0        0    13798 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/recordset_compat.py
--rw-r--r--   0        0        0    11707 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/retry_invoker.py
--rw-r--r--   0        0        0      731 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/__init__.py
--rw-r--r--   0        0        0      738 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/crypto/__init__.py
--rw-r--r--   0        0        0     2792 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/crypto/shamir.py
--rw-r--r--   0        0        0     4707 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
--rw-r--r--   0        0        0     3026 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
--rw-r--r--   0        0        0     2310 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/quantization.py
--rw-r--r--   0        0        0     2183 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
--rw-r--r--   0        0        0     3221 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
--rw-r--r--   0        0        0    22250 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7865 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     4382 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      666 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      683 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     3207 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     5016 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     7304 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     2022 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     1084 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/error_pb2.py
--rw-r--r--   0        0        0      734 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/error_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/error_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/error_pb2_grpc.pyi
--rw-r--r--   0        0        0     5018 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     9161 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0    10605 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     2811 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1081 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     6009 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/recordset_pb2.py
--rw-r--r--   0        0        0    14161 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/recordset_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/recordset_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/recordset_pb2_grpc.pyi
--rw-r--r--   0        0        0     2472 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     4320 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0     9781 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1785 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    28282 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6127 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2399 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0      892 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/compat/__init__.py
--rw-r--r--   0        0        0     5287 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/compat/app.py
--rw-r--r--   0        0        0     3468 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/compat/app_utils.py
--rw-r--r--   0        0        0     5444 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/compat/driver_client_proxy.py
--rw-r--r--   0        0        0     1766 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/compat/legacy_context.py
--rw-r--r--   0        0        0     1061 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      862 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     5090 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/driver/driver.py
--rw-r--r--   0        0        0    11832 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/driver/grpc_driver.py
--rw-r--r--   0        0        0     5121 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/history.py
--rw-r--r--   0        0        0     5972 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/run_serverapp.py
--rw-r--r--   0        0        0    17664 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/server.py
--rw-r--r--   0        0        0     4402 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/server_app.py
--rw-r--r--   0        0        0     1349 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/server_config.py
--rw-r--r--   0        0        0     2836 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0    13468 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     6532 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/bulyan.py
--rw-r--r--   0        0        0    17458 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/dp_adaptive_clipping.py
--rw-r--r--   0        0        0    12904 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/dp_fixed_clipping.py
--rw-r--r--   0        0        0     4877 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     7219 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5900 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6505 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     6763 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11799 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9784 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8132 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2704 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5242 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     6862 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     5890 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     6080 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedxgb_bagging.py
--rw-r--r--   0        0        0     5607 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedxgb_cyclic.py
--rw-r--r--   0        0        0     4047 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     6801 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6285 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10150 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7543 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      707 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/__init__.py
--rw-r--r--   0        0        0      712 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/driver/__init__.py
--rw-r--r--   0        0        0     1932 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/driver/driver_grpc.py
--rw-r--r--   0        0        0     4796 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/driver/driver_servicer.py
--rw-r--r--   0        0        0      711 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/__init__.py
--rw-r--r--   0        0        0      735 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     5993 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6458 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4887 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11932 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0      758 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     3387 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0     5799 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py
--rw-r--r--   0        0        0      731 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     3622 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      735 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     7621 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0      783 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/vce/__init__.py
--rw-r--r--   0        0        0     1466 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
--rw-r--r--   0        0        0     2260 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
--rw-r--r--   0        0        0     6375 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
--rw-r--r--   0        0        0    12454 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/vce/vce_api.py
--rw-r--r--   0        0        0     1003 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/__init__.py
--rw-r--r--   0        0        0    11651 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/in_memory_state.py
--rw-r--r--   0        0        0    27167 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/sqlite_state.py
--rw-r--r--   0        0        0     7709 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/state.py
--rw-r--r--   0        0        0     1654 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/state_factory.py
--rw-r--r--   0        0        0     2207 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/utils.py
--rw-r--r--   0        0        0      913 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/typing.py
--rw-r--r--   0        0        0      908 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5485 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     5301 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0      902 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/__init__.py
--rw-r--r--   0        0        0     1082 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/constant.py
--rw-r--r--   0        0        0    12547 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/default_workflows.py
--rw-r--r--   0        0        0      880 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     5838 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
--rw-r--r--   0        0        0    29038 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
--rw-r--r--   0        0        0     1400 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0    13904 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      734 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0    19367 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/ray_transport/ray_actor.py
--rw-r--r--   0        0        0     6738 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0     2392 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/ray_transport/utils.py
--rw-r--r--   0        0        0    15694 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/run_simulation.py
--rw-r--r--   0        0        0    15260 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240429/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-30 23:05:21.507832 flwr_nightly-1.9.0.dev20240430/LICENSE
+-rw-r--r--   0        0        0    12916 2024-04-30 23:05:21.507832 flwr_nightly-1.9.0.dev20240430/README.md
+-rw-r--r--   0        0        0     5776 2024-04-30 23:05:34.051937 flwr_nightly-1.9.0.dev20240430/pyproject.toml
+-rw-r--r--   0        0        0      937 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0      720 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/app.py
+-rw-r--r--   0        0        0     4899 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/config_utils.py
+-rw-r--r--   0        0        0     2215 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/example.py
+-rw-r--r--   0        0        0      789 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/__init__.py
+-rw-r--r--   0        0        0     5989 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/new.py
+-rw-r--r--   0        0        0      725 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/__init__.py
+-rw-r--r--   0        0        0     3078 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/.gitignore.tpl
+-rw-r--r--   0        0        0      667 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/README.md.tpl
+-rw-r--r--   0        0        0      729 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/__init__.py
+-rw-r--r--   0        0        0      736 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
+-rw-r--r--   0        0        0      521 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
+-rw-r--r--   0        0        0     1172 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
+-rw-r--r--   0        0        0     2801 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl
+-rw-r--r--   0        0        0     1911 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
+-rw-r--r--   0        0        0      248 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
+-rw-r--r--   0        0        0      593 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
+-rw-r--r--   0        0        0      341 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/server.sklearn.py.tpl
+-rw-r--r--   0        0        0      371 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
+-rw-r--r--   0        0        0     3684 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
+-rw-r--r--   0        0        0      521 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
+-rw-r--r--   0        0        0      590 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
+-rw-r--r--   0        0        0      570 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl
+-rw-r--r--   0        0        0      569 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
+-rw-r--r--   0        0        0      789 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/run/__init__.py
+-rw-r--r--   0        0        0     2334 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/run/run.py
+-rw-r--r--   0        0        0     4119 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/utils.py
+-rw-r--r--   0        0        0     1268 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    22313 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     8183 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     8636 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/client_app.py
+-rw-r--r--   0        0        0     7435 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      735 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     8993 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      752 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     4903 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/grpc_rere_client/client_interceptor.py
+-rw-r--r--   0        0        0     9597 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0     2404 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/heartbeat.py
+-rw-r--r--   0        0        0      719 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     6553 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1824 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     1143 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/__init__.py
+-rw-r--r--   0        0        0     5397 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/centraldp_mods.py
+-rw-r--r--   0        0        0     2623 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/comms_mods.py
+-rw-r--r--   0        0        0     4918 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/localdp_mod.py
+-rw-r--r--   0        0        0      849 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
+-rw-r--r--   0        0        0    19699 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
+-rw-r--r--   0        0        0     1226 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/utils.py
+-rw-r--r--   0        0        0     1778 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/node_state.py
+-rw-r--r--   0        0        0     2195 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/node_state_tests.py
+-rw-r--r--   0        0        0    10283 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      735 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0    11520 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0      865 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/supernode/__init__.py
+-rw-r--r--   0        0        0     9052 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/supernode/app.py
+-rw-r--r--   0        0        0     1006 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/typing.py
+-rw-r--r--   0        0        0     3721 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1882 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     2424 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0     1313 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/context.py
+-rw-r--r--   0        0        0      891 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     6113 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/differential_privacy.py
+-rw-r--r--   0        0        0     1074 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/differential_privacy_constants.py
+-rw-r--r--   0        0        0     2004 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     2812 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/exit_handlers.py
+-rw-r--r--   0        0        0     2460 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     6920 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0    12686 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/message.py
+-rw-r--r--   0        0        0     4961 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/object_ref.py
+-rw-r--r--   0        0        0     2095 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0     1385 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/pyproject.py
+-rw-r--r--   0        0        0     1054 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/__init__.py
+-rw-r--r--   0        0        0     4652 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/configsrecord.py
+-rw-r--r--   0        0        0     1393 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/conversion_utils.py
+-rw-r--r--   0        0        0     3923 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/metricsrecord.py
+-rw-r--r--   0        0        0     4849 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/parametersrecord.py
+-rw-r--r--   0        0        0     4533 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/recordset.py
+-rw-r--r--   0        0        0     3879 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/typeddict.py
+-rw-r--r--   0        0        0    13798 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/recordset_compat.py
+-rw-r--r--   0        0        0    11707 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/retry_invoker.py
+-rw-r--r--   0        0        0      731 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0      738 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/crypto/__init__.py
+-rw-r--r--   0        0        0     2792 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/crypto/shamir.py
+-rw-r--r--   0        0        0     4707 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
+-rw-r--r--   0        0        0     3026 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
+-rw-r--r--   0        0        0     2310 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/quantization.py
+-rw-r--r--   0        0        0     2183 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
+-rw-r--r--   0        0        0     3221 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
+-rw-r--r--   0        0        0    22250 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7865 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     4382 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      666 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      683 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     3207 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     5016 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     7304 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     2022 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1084 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/error_pb2.py
+-rw-r--r--   0        0        0      734 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/error_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/error_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/error_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5018 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     9161 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0    10605 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     2811 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1081 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6009 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/recordset_pb2.py
+-rw-r--r--   0        0        0    14161 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/recordset_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/recordset_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/recordset_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2472 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0     4320 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9781 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1785 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    28282 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6127 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2399 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0      892 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/compat/__init__.py
+-rw-r--r--   0        0        0     5287 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/compat/app.py
+-rw-r--r--   0        0        0     3468 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/compat/app_utils.py
+-rw-r--r--   0        0        0     5444 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/compat/driver_client_proxy.py
+-rw-r--r--   0        0        0     1766 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/compat/legacy_context.py
+-rw-r--r--   0        0        0     1061 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      862 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     5090 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/driver/driver.py
+-rw-r--r--   0        0        0    11832 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/driver/grpc_driver.py
+-rw-r--r--   0        0        0     5121 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0     5972 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/run_serverapp.py
+-rw-r--r--   0        0        0    17664 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0     4402 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/server_app.py
+-rw-r--r--   0        0        0     1349 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/server_config.py
+-rw-r--r--   0        0        0     2836 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0    13468 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     6532 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/bulyan.py
+-rw-r--r--   0        0        0    17458 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/dp_adaptive_clipping.py
+-rw-r--r--   0        0        0    12904 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/dp_fixed_clipping.py
+-rw-r--r--   0        0        0     4877 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     7219 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5900 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6505 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     6763 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11799 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9784 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8132 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2704 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5242 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     6862 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     5890 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     6080 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedxgb_bagging.py
+-rw-r--r--   0        0        0     5607 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedxgb_cyclic.py
+-rw-r--r--   0        0        0     4047 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     6801 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6285 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10150 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7543 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      707 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/driver/__init__.py
+-rw-r--r--   0        0        0     1932 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/driver/driver_grpc.py
+-rw-r--r--   0        0        0     4796 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/driver/driver_servicer.py
+-rw-r--r--   0        0        0      711 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/__init__.py
+-rw-r--r--   0        0        0      735 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     5993 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6458 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4887 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11932 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0      758 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     3387 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0     5902 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py
+-rw-r--r--   0        0        0      731 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     3622 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      735 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     7621 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0      783 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/vce/__init__.py
+-rw-r--r--   0        0        0     1466 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
+-rw-r--r--   0        0        0     2260 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
+-rw-r--r--   0        0        0     6375 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
+-rw-r--r--   0        0        0    12454 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/vce/vce_api.py
+-rw-r--r--   0        0        0     1003 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/__init__.py
+-rw-r--r--   0        0        0    11651 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/in_memory_state.py
+-rw-r--r--   0        0        0    27167 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/sqlite_state.py
+-rw-r--r--   0        0        0     7709 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/state.py
+-rw-r--r--   0        0        0     1654 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/state_factory.py
+-rw-r--r--   0        0        0     2207 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/utils.py
+-rw-r--r--   0        0        0      913 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/typing.py
+-rw-r--r--   0        0        0      908 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5485 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     5301 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0      902 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/__init__.py
+-rw-r--r--   0        0        0     1082 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/constant.py
+-rw-r--r--   0        0        0    12547 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/default_workflows.py
+-rw-r--r--   0        0        0      880 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     5838 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
+-rw-r--r--   0        0        0    29038 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
+-rw-r--r--   0        0        0     1400 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0    14380 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      734 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0    19367 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/ray_transport/ray_actor.py
+-rw-r--r--   0        0        0     6738 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0     2392 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/ray_transport/utils.py
+-rw-r--r--   0        0        0    15896 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/run_simulation.py
+-rw-r--r--   0        0        0    15260 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240430/PKG-INFO
```

### Comparing `flwr_nightly-1.9.0.dev20240429/LICENSE` & `flwr_nightly-1.9.0.dev20240430/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/README.md` & `flwr_nightly-1.9.0.dev20240430/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/pyproject.toml` & `flwr_nightly-1.9.0.dev20240430/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.9.0.dev20240429"
+version = "1.9.0.dev20240430"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.ai>"]
 readme = "README.md"
 homepage = "https://flower.ai"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.ai"
```

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/app.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/config_utils.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/config_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/example.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/example.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/new.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/new.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/.gitignore.tpl` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/.gitignore.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/README.md.tpl` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/README.md.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/run/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/run/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/run/run.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/run/run.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/utils.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/app.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/client.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/client_app.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/client_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/grpc_rere_client/client_interceptor.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/grpc_rere_client/client_interceptor.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,27 +28,29 @@
     generate_shared_key,
     public_key_to_bytes,
 )
 from flwr.proto.fleet_pb2 import (  # pylint: disable=E0611
     CreateNodeRequest,
     DeleteNodeRequest,
     GetRunRequest,
+    PingRequest,
     PullTaskInsRequest,
     PushTaskResRequest,
 )
 
 _PUBLIC_KEY_HEADER = "public-key"
 _AUTH_TOKEN_HEADER = "auth-token"
 
 Request = Union[
     CreateNodeRequest,
     DeleteNodeRequest,
     PullTaskInsRequest,
     PushTaskResRequest,
     GetRunRequest,
+    PingRequest,
 ]
 
 
 def _get_value_from_tuples(
     key_string: str, tuples: Sequence[Tuple[str, Union[str, bytes]]]
 ) -> bytes:
     value = next((value for key, value in tuples if key == key_string), "")
@@ -111,15 +113,21 @@
             )
         )
 
         if isinstance(request, CreateNodeRequest):
             postprocess = True
         elif isinstance(
             request,
-            (DeleteNodeRequest, PullTaskInsRequest, PushTaskResRequest, GetRunRequest),
+            (
+                DeleteNodeRequest,
+                PullTaskInsRequest,
+                PushTaskResRequest,
+                GetRunRequest,
+                PingRequest,
+            ),
         ):
             if self.shared_secret is None:
                 raise RuntimeError("Failure to compute hmac")
 
             metadata.append(
                 (
                     _AUTH_TOKEN_HEADER,
```

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/heartbeat.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/heartbeat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/centraldp_mods.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/centraldp_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/comms_mods.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/comms_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/localdp_mod.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/localdp_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/utils.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/node_state.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/node_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/node_state_tests.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/node_state_tests.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/rest_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/supernode/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/supernode/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/supernode/app.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/supernode/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/typing.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/address.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/constant.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/context.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/date.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/differential_privacy.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/differential_privacy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/differential_privacy_constants.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/differential_privacy_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/dp.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/exit_handlers.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/exit_handlers.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/grpc.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/logger.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -184,7 +184,33 @@
         """DEPRECATED FEATURE: %s
 
             This is a deprecated feature. It will be removed
             entirely in future versions of Flower.
         """,
         name,
     )
+
+
+def set_logger_propagation(
+    child_logger: logging.Logger, value: bool = True
+) -> logging.Logger:
+    """Set the logger propagation attribute.
+
+    Parameters
+    ----------
+    child_logger : logging.Logger
+        Child logger object
+    value : bool
+        Boolean setting for propagation. If True, both parent and child logger
+        display messages. Otherwise, only the child logger displays a message.
+        This False setting prevents duplicate logs in Colab notebooks.
+        Reference: https://stackoverflow.com/a/19561320
+
+    Returns
+    -------
+    logging.Logger
+        Child logger object with updated propagation setting
+    """
+    child_logger.propagate = value
+    if not child_logger.propagate:
+        child_logger.log(logging.DEBUG, "Logger propagate set to False")
+    return child_logger
```

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/message.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/message.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """Message."""
 
 from __future__ import annotations
 
 import time
 import warnings
 from dataclasses import dataclass
+from typing import Optional, cast
 
 from .record import RecordSet
 
 DEFAULT_TTL = 3600
 
 
 @dataclass
@@ -51,156 +52,148 @@
         the receiving end.
     partition_id : Optional[int]
         An identifier that can be used when loading a particular
         data partition for a ClientApp. Making use of this identifier
         is more relevant when conducting simulations.
     """
 
-    _run_id: int
-    _message_id: str
-    _src_node_id: int
-    _dst_node_id: int
-    _reply_to_message: str
-    _group_id: str
-    _ttl: float
-    _message_type: str
-    _partition_id: int | None
-    _created_at: float  # Unix timestamp (in seconds) to be set upon message creation
-
     def __init__(  # pylint: disable=too-many-arguments
         self,
         run_id: int,
         message_id: str,
         src_node_id: int,
         dst_node_id: int,
         reply_to_message: str,
         group_id: str,
         ttl: float,
         message_type: str,
         partition_id: int | None = None,
     ) -> None:
-        self._run_id = run_id
-        self._message_id = message_id
-        self._src_node_id = src_node_id
-        self._dst_node_id = dst_node_id
-        self._reply_to_message = reply_to_message
-        self._group_id = group_id
-        self._ttl = ttl
-        self._message_type = message_type
-        self._partition_id = partition_id
+        var_dict = {
+            "_run_id": run_id,
+            "_message_id": message_id,
+            "_src_node_id": src_node_id,
+            "_dst_node_id": dst_node_id,
+            "_reply_to_message": reply_to_message,
+            "_group_id": group_id,
+            "_ttl": ttl,
+            "_message_type": message_type,
+            "_partition_id": partition_id,
+        }
+        self.__dict__.update(var_dict)
 
     @property
     def run_id(self) -> int:
         """An identifier for the current run."""
-        return self._run_id
+        return cast(int, self.__dict__["_run_id"])
 
     @property
     def message_id(self) -> str:
         """An identifier for the current message."""
-        return self._message_id
+        return cast(str, self.__dict__["_message_id"])
 
     @property
     def src_node_id(self) -> int:
         """An identifier for the node sending this message."""
-        return self._src_node_id
+        return cast(int, self.__dict__["_src_node_id"])
 
     @property
     def reply_to_message(self) -> str:
         """An identifier for the message this message replies to."""
-        return self._reply_to_message
+        return cast(str, self.__dict__["_reply_to_message"])
 
     @property
     def dst_node_id(self) -> int:
         """An identifier for the node receiving this message."""
-        return self._dst_node_id
+        return cast(int, self.__dict__["_dst_node_id"])
 
     @dst_node_id.setter
     def dst_node_id(self, value: int) -> None:
         """Set dst_node_id."""
-        self._dst_node_id = value
+        self.__dict__["_dst_node_id"] = value
 
     @property
     def group_id(self) -> str:
         """An identifier for grouping messages."""
-        return self._group_id
+        return cast(str, self.__dict__["_group_id"])
 
     @group_id.setter
     def group_id(self, value: str) -> None:
         """Set group_id."""
-        self._group_id = value
+        self.__dict__["_group_id"] = value
 
     @property
     def created_at(self) -> float:
         """Unix timestamp when the message was created."""
-        return self._created_at
+        return cast(float, self.__dict__["_created_at"])
 
     @created_at.setter
     def created_at(self, value: float) -> None:
-        """Set creation timestamp for this messages."""
-        self._created_at = value
+        """Set creation timestamp for this message."""
+        self.__dict__["_created_at"] = value
 
     @property
     def ttl(self) -> float:
         """Time-to-live for this message."""
-        return self._ttl
+        return cast(float, self.__dict__["_ttl"])
 
     @ttl.setter
     def ttl(self, value: float) -> None:
         """Set ttl."""
-        self._ttl = value
+        self.__dict__["_ttl"] = value
 
     @property
     def message_type(self) -> str:
         """A string that encodes the action to be executed on the receiving end."""
-        return self._message_type
+        return cast(str, self.__dict__["_message_type"])
 
     @message_type.setter
     def message_type(self, value: str) -> None:
         """Set message_type."""
-        self._message_type = value
+        self.__dict__["_message_type"] = value
 
     @property
     def partition_id(self) -> int | None:
         """An identifier telling which data partition a ClientApp should use."""
-        return self._partition_id
+        return cast(int, self.__dict__["_partition_id"])
 
     @partition_id.setter
     def partition_id(self, value: int) -> None:
-        """Set patition_id."""
-        self._partition_id = value
+        """Set partition_id."""
+        self.__dict__["_partition_id"] = value
 
 
 @dataclass
 class Error:
     """A dataclass that stores information about an error that occurred.
 
     Parameters
     ----------
     code : int
         An identifier for the error.
     reason : Optional[str]
         A reason for why the error arose (e.g. an exception stack-trace)
     """
 
-    _code: int
-    _reason: str | None = None
-
     def __init__(self, code: int, reason: str | None = None) -> None:
-        self._code = code
-        self._reason = reason
+        var_dict = {
+            "_code": code,
+            "_reason": reason,
+        }
+        self.__dict__.update(var_dict)
 
     @property
     def code(self) -> int:
         """Error code."""
-        return self._code
+        return cast(int, self.__dict__["_code"])
 
     @property
     def reason(self) -> str | None:
         """Reason reported about the error."""
-        return self._reason
+        return cast(Optional[str], self.__dict__["_reason"])
 
 
 @dataclass
 class Message:
     """State of your application from the viewpoint of the entity using it.
 
     Parameters
@@ -211,96 +204,78 @@
         Holds records either sent by another entity (e.g. sent by the server-side
         logic to a client, or vice-versa) or that will be sent to it.
     error : Optional[Error]
         A dataclass that captures information about an error that took place
         when processing another message.
     """
 
-    _metadata: Metadata
-    _content: RecordSet | None = None
-    _error: Error | None = None
-
     def __init__(
         self,
         metadata: Metadata,
         content: RecordSet | None = None,
         error: Error | None = None,
     ) -> None:
-        self._metadata = metadata
-
-        # Set message creation timestamp
-        self._metadata.created_at = time.time()
-
         if not (content is None) ^ (error is None):
             raise ValueError("Either `content` or `error` must be set, but not both.")
 
-        self._content = content
-        self._error = error
+        metadata.created_at = time.time()  # Set the message creation timestamp
+        var_dict = {
+            "_metadata": metadata,
+            "_content": content,
+            "_error": error,
+        }
+        self.__dict__.update(var_dict)
 
     @property
     def metadata(self) -> Metadata:
         """A dataclass including information about the message to be executed."""
-        return self._metadata
+        return cast(Metadata, self.__dict__["_metadata"])
 
     @property
     def content(self) -> RecordSet:
         """The content of this message."""
-        if self._content is None:
+        if self.__dict__["_content"] is None:
             raise ValueError(
                 "Message content is None. Use <message>.has_content() "
                 "to check if a message has content."
             )
-        return self._content
+        return cast(RecordSet, self.__dict__["_content"])
 
     @content.setter
     def content(self, value: RecordSet) -> None:
         """Set content."""
-        if self._error is None:
-            self._content = value
+        if self.__dict__["_error"] is None:
+            self.__dict__["_content"] = value
         else:
             raise ValueError("A message with an error set cannot have content.")
 
     @property
     def error(self) -> Error:
         """Error captured by this message."""
-        if self._error is None:
+        if self.__dict__["_error"] is None:
             raise ValueError(
                 "Message error is None. Use <message>.has_error() "
                 "to check first if a message carries an error."
             )
-        return self._error
+        return cast(Error, self.__dict__["_error"])
 
     @error.setter
     def error(self, value: Error) -> None:
         """Set error."""
         if self.has_content():
             raise ValueError("A message with content set cannot carry an error.")
-        self._error = value
+        self.__dict__["_error"] = value
 
     def has_content(self) -> bool:
         """Return True if message has content, else False."""
-        return self._content is not None
+        return self.__dict__["_content"] is not None
 
     def has_error(self) -> bool:
         """Return True if message has an error, else False."""
-        return self._error is not None
-
-    def _create_reply_metadata(self, ttl: float) -> Metadata:
-        """Construct metadata for a reply message."""
-        return Metadata(
-            run_id=self.metadata.run_id,
-            message_id="",
-            src_node_id=self.metadata.dst_node_id,
-            dst_node_id=self.metadata.src_node_id,
-            reply_to_message=self.metadata.message_id,
-            group_id=self.metadata.group_id,
-            ttl=ttl,
-            message_type=self.metadata.message_type,
-            partition_id=self.metadata.partition_id,
-        )
+        return self.__dict__["_error"] is not None
 
     def create_error_reply(self, error: Error, ttl: float | None = None) -> Message:
         """Construct a reply message indicating an error happened.
 
         Parameters
         ----------
         error : Error
@@ -319,15 +294,15 @@
                 "version of Flower.",
                 stacklevel=2,
             )
         # If no TTL passed, use default for message creation (will update after
         # message creation)
         ttl_ = DEFAULT_TTL if ttl is None else ttl
         # Create reply with error
-        message = Message(metadata=self._create_reply_metadata(ttl_), error=error)
+        message = Message(metadata=_create_reply_metadata(self, ttl_), error=error)
 
         if ttl is None:
             # Set TTL equal to the remaining time for the received message to expire
             ttl = self.metadata.ttl - (
                 message.metadata.created_at - self.metadata.created_at
             )
             message.metadata.ttl = ttl
@@ -365,19 +340,34 @@
                 stacklevel=2,
             )
         # If no TTL passed, use default for message creation (will update after
         # message creation)
         ttl_ = DEFAULT_TTL if ttl is None else ttl
 
         message = Message(
-            metadata=self._create_reply_metadata(ttl_),
+            metadata=_create_reply_metadata(self, ttl_),
             content=content,
         )
 
         if ttl is None:
             # Set TTL equal to the remaining time for the received message to expire
             ttl = self.metadata.ttl - (
                 message.metadata.created_at - self.metadata.created_at
             )
             message.metadata.ttl = ttl
 
         return message
+
+
+def _create_reply_metadata(msg: Message, ttl: float) -> Metadata:
+    """Construct metadata for a reply message."""
+    return Metadata(
+        run_id=msg.metadata.run_id,
+        message_id="",
+        src_node_id=msg.metadata.dst_node_id,
+        dst_node_id=msg.metadata.src_node_id,
+        reply_to_message=msg.metadata.message_id,
+        group_id=msg.metadata.group_id,
+        ttl=ttl,
+        message_type=msg.metadata.message_type,
+        partition_id=msg.metadata.partition_id,
+    )
```

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/object_ref.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/object_ref.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/parameter.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/pyproject.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/pyproject.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/configsrecord.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/configsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/conversion_utils.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/metricsrecord.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/metricsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/parametersrecord.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/parametersrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/recordset.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/recordset.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 from .configsrecord import ConfigsRecord
 from .metricsrecord import MetricsRecord
 from .parametersrecord import ParametersRecord
 from .typeddict import TypedDict
 
 
+@dataclass
 class RecordSetData:
     """Inner data container for the RecordSet class."""
 
     parameters_records: TypedDict[str, ParametersRecord]
     metrics_records: TypedDict[str, MetricsRecord]
     configs_records: TypedDict[str, ConfigsRecord]
 
@@ -93,26 +94,26 @@
         configs_records: Optional[Dict[str, ConfigsRecord]] = None,
     ) -> None:
         data = RecordSetData(
             parameters_records=parameters_records,
             metrics_records=metrics_records,
             configs_records=configs_records,
         )
-        setattr(self, "_data", data)  # noqa
+        self.__dict__["_data"] = data
 
     @property
     def parameters_records(self) -> TypedDict[str, ParametersRecord]:
         """Dictionary holding ParametersRecord instances."""
-        data = cast(RecordSetData, getattr(self, "_data"))  # noqa
+        data = cast(RecordSetData, self.__dict__["_data"])
         return data.parameters_records
 
     @property
     def metrics_records(self) -> TypedDict[str, MetricsRecord]:
         """Dictionary holding MetricsRecord instances."""
-        data = cast(RecordSetData, getattr(self, "_data"))  # noqa
+        data = cast(RecordSetData, self.__dict__["_data"])
         return data.metrics_records
 
     @property
     def configs_records(self) -> TypedDict[str, ConfigsRecord]:
         """Dictionary holding ConfigsRecord instances."""
-        data = cast(RecordSetData, getattr(self, "_data"))  # noqa
+        data = cast(RecordSetData, self.__dict__["_data"])
         return data.configs_records
```

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/typeddict.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/typeddict.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/recordset_compat.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/recordset_compat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/retry_invoker.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/retry_invoker.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/crypto/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/crypto/shamir.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/crypto/shamir.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/quantization.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/quantization.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/secaggplus_constants.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/secaggplus_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/secaggplus_utils.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/secaggplus_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/serde.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/typing.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/version.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/error_pb2.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/error_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/error_pb2.pyi` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/error_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/recordset_pb2.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/recordset_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/recordset_pb2.pyi` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/recordset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/app.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/compat/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/compat/app.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/compat/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/compat/app_utils.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/compat/app_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/compat/driver_client_proxy.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/compat/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/compat/legacy_context.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/compat/legacy_context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/criterion.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/driver/driver.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/driver/grpc_driver.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/driver/grpc_driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/history.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/run_serverapp.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/run_serverapp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/server.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/server_app.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/server_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/server_config.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/server_config.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/bulyan.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/bulyan.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/dp_adaptive_clipping.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/dp_adaptive_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/dp_fixed_clipping.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/dp_fixed_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedxgb_bagging.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedxgb_bagging.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedxgb_cyclic.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedxgb_cyclic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/driver/driver_grpc.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/driver/driver_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/driver/driver_servicer.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 from flwr.proto.fleet_pb2 import (  # pylint: disable=E0611
     CreateNodeRequest,
     CreateNodeResponse,
     DeleteNodeRequest,
     DeleteNodeResponse,
     GetRunRequest,
     GetRunResponse,
+    PingRequest,
+    PingResponse,
     PullTaskInsRequest,
     PullTaskInsResponse,
     PushTaskResRequest,
     PushTaskResResponse,
 )
 
 _PUBLIC_KEY_HEADER = "public-key"
@@ -47,22 +49,24 @@
 
 Request = Union[
     CreateNodeRequest,
     DeleteNodeRequest,
     PullTaskInsRequest,
     PushTaskResRequest,
     GetRunRequest,
+    PingRequest,
 ]
 
 Response = Union[
     CreateNodeResponse,
     DeleteNodeResponse,
     PullTaskInsResponse,
     PushTaskResResponse,
     GetRunResponse,
+    PingResponse,
 ]
 
 
 def _get_value_from_tuples(
     key_string: str, tuples: Sequence[Tuple[str, Union[str, bytes]]]
 ) -> bytes:
     value = next((value for key, value in tuples if key == key_string), "")
@@ -136,14 +140,15 @@
             elif isinstance(
                 request,
                 (
                     DeleteNodeRequest,
                     PullTaskInsRequest,
                     PushTaskResRequest,
                     GetRunRequest,
+                    PingRequest,
                 ),
             ):
                 hmac_value = base64.urlsafe_b64decode(
                     _get_value_from_tuples(
                         _AUTH_TOKEN_HEADER, context.invocation_metadata()
                     )
                 )
```

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/vce/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/vce/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/vce/backend/backend.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/vce/backend/backend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/vce/vce_api.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/vce/vce_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/in_memory_state.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/sqlite_state.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/state.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/state_factory.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/utils.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/typing.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/constant.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/default_workflows.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/default_workflows.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/app.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower simulation app."""
 
 
+import asyncio
+import logging
 import sys
 import threading
 import traceback
 import warnings
 from logging import ERROR, INFO
 from typing import Any, Dict, List, Optional, Type, Union
 
 import ray
 from ray.util.scheduling_strategies import NodeAffinitySchedulingStrategy
 
 from flwr.client import ClientFn
 from flwr.common import EventType, event
-from flwr.common.logger import log
+from flwr.common.logger import log, set_logger_propagation
 from flwr.server.client_manager import ClientManager
 from flwr.server.history import History
 from flwr.server.server import Server, init_defaults, run_fl
 from flwr.server.server_config import ServerConfig
 from flwr.server.strategy import Strategy
 from flwr.simulation.ray_transport.ray_actor import (
     ClientAppActor,
@@ -152,25 +154,38 @@
         Optional string ("DEFAULT" or "SPREAD") for the VCE to choose in which
         node the actor is placed. If you are an advanced user needed more control
         you can use lower-level scheduling strategies to pin actors to specific
         compute nodes (e.g. via NodeAffinitySchedulingStrategy). Please note this
         is an advanced feature. For all details, please refer to the Ray documentation:
         https://docs.ray.io/en/latest/ray-core/scheduling/index.html
 
+
     Returns
     -------
     hist : flwr.server.history.History
         Object containing metrics from training.
     """  # noqa: E501
     # pylint: disable-msg=too-many-locals
     event(
         EventType.START_SIMULATION_ENTER,
         {"num_clients": len(clients_ids) if clients_ids is not None else num_clients},
     )
 
+    # Set logger propagation
+    loop: Optional[asyncio.AbstractEventLoop] = None
+    try:
+        loop = asyncio.get_running_loop()
+    except RuntimeError:
+        loop = None
+    finally:
+        if loop and loop.is_running():
+            # Set logger propagation to False to prevent duplicated log output in Colab.
+            logger = logging.getLogger("flwr")
+            _ = set_logger_propagation(logger, False)
+
     # Initialize server and server config
     initialized_server, initialized_config = init_defaults(
         server=server,
         config=config,
         strategy=strategy,
         client_manager=client_manager,
     )
```

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/ray_transport/ray_actor.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/ray_transport/ray_actor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/ray_transport/utils.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/ray_transport/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/run_simulation.py` & `flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/run_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from time import sleep
 from typing import Dict, Optional
 
 import grpc
 
 from flwr.client import ClientApp
 from flwr.common import EventType, event, log
+from flwr.common.logger import set_logger_propagation
 from flwr.common.typing import ConfigsRecordValues
 from flwr.server.driver import Driver, GrpcDriver
 from flwr.server.run_serverapp import run
 from flwr.server.server_app import ServerApp
 from flwr.server.superlink.driver.driver_grpc import run_driver_api_grpc
 from flwr.server.superlink.fleet import vce
 from flwr.server.superlink.state import StateFactory
@@ -360,14 +361,16 @@
         run_in_thread = True
 
     except RuntimeError:
         log(DEBUG, "No asyncio event loop runnig")
 
     finally:
         if run_in_thread:
+            # Set logger propagation to False to prevent duplicated log output in Colab.
+            logger = set_logger_propagation(logger, False)
             log(DEBUG, "Starting Simulation Engine on a new thread.")
             simulation_engine_th = threading.Thread(target=_main_loop, args=args)
             simulation_engine_th.start()
             simulation_engine_th.join()
         else:
             log(DEBUG, "Starting Simulation Engine on the main thread.")
             _main_loop(*args)
```

### Comparing `flwr_nightly-1.9.0.dev20240429/PKG-INFO` & `flwr_nightly-1.9.0.dev20240430/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.9.0.dev20240429
+Version: 1.9.0.dev20240430
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.ai
 License: Apache-2.0
 Keywords: flower,fl,federated learning,federated analytics,federated evaluation,machine learning
 Author: The Flower Authors
 Author-email: hello@flower.ai
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240429 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240430 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.ai
 License: Apache-2.0 Keywords: flower,fl,federated learning,federated
 analytics,federated evaluation,machine learning Author: The Flower Authors
 Author-email: hello@flower.ai Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
```

