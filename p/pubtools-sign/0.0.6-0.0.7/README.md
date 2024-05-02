# Comparing `tmp/pubtools_sign-0.0.6.tar.gz` & `tmp/pubtools_sign-0.0.7.tar.gz`

## Comparing `pubtools_sign-0.0.6.tar` & `pubtools_sign-0.0.7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/.coveragerc
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/AppImageBuilder.yml
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/MANIFEST.in
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/mypy.ini
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/requirements-test.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/requirements.txt
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tox.ini
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/.github/renovate.json
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/.github/workflows/docs.yml
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/.github/workflows/owasp.yml
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/.github/workflows/release.yml
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/.github/workflows/tox-tests.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/docs/make.bat
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/docs/source/CHANGELOG.rst
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/docs/source/conf.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/docs/source/index.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/__init__.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/bundle.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/exceptions.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/ansible/__init__.py
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/ansible/msg_clear_sign.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/clients/__init__.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/clients/msg.py
--rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/clients/msg_recv_client.py
--rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/clients/msg_send_client.py
--rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/clients/registry.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/conf/conf.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/models/msg.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/operations/__init__.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/operations/base.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/operations/clearsign.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/operations/containersign.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/results/__init__.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/results/clearsign.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/results/containersign.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/results/operation_result.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/results/signing_results.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/signers/__init__.py
--rw-r--r--   0        0        0    14528 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/signers/cosignsigner.py
--rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/signers/msgsigner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0    16932 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/conftest.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/conftest_cosignsig.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/conftest_msgsig.py
--rw-r--r--   0        0        0     5293 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_ansible_clearsign.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_bundle.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_config.py
--rw-r--r--   0        0        0    25384 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_cosign_signer.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_msg_handle.py
--rw-r--r--   0        0        0    12970 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_msg_recv_client.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_msg_send_client.py
--rw-r--r--   0        0        0    42730 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_msg_signer.py
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_registry_client.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_results.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_sign_operations.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_utils.py
--rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/utils/pre-commit
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/.gitignore
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/LICENSE
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/README.rst
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/.coveragerc
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/AppImageBuilder.yml
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/MANIFEST.in
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/mypy.ini
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/requirements-test.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/requirements.txt
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/tox.ini
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/.github/renovate.json
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/.github/workflows/owasp.yml
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/.github/workflows/tox-tests.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/docs/make.bat
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/docs/source/CHANGELOG.rst
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/docs/source/conf.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/__init__.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/bundle.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/exceptions.py
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/ansible/__init__.py
+-rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/ansible/msg_clear_sign.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/clients/__init__.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/clients/msg.py
+-rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/clients/msg_recv_client.py
+-rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/clients/msg_send_client.py
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/clients/registry.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/conf/conf.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/models/msg.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/operations/__init__.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/operations/base.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/operations/clearsign.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/operations/containersign.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/results/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/results/clearsign.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/results/containersign.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/results/operation_result.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/results/signing_results.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/signers/__init__.py
+-rw-r--r--   0        0        0    14317 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/signers/cosignsigner.py
+-rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/src/pubtools/sign/signers/msgsigner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0    16932 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/tests/conftest.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/tests/conftest_cosignsig.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/tests/conftest_msgsig.py
+-rw-r--r--   0        0        0     5293 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/tests/test_ansible_clearsign.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/tests/test_bundle.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/tests/test_config.py
+-rw-r--r--   0        0        0    25384 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/tests/test_cosign_signer.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/tests/test_msg_handle.py
+-rw-r--r--   0        0        0    12970 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/tests/test_msg_recv_client.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/tests/test_msg_send_client.py
+-rw-r--r--   0        0        0    42730 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/tests/test_msg_signer.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/tests/test_registry_client.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/tests/test_results.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/tests/test_sign_operations.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/tests/test_utils.py
+-rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/utils/pre-commit
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/.gitignore
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/LICENSE
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/README.rst
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pubtools_sign-0.0.7/PKG-INFO
```

### Comparing `pubtools_sign-0.0.6/AppImageBuilder.yml` & `pubtools_sign-0.0.7/AppImageBuilder.yml`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/tox.ini` & `pubtools_sign-0.0.7/tox.ini`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/.github/workflows/docs.yml` & `pubtools_sign-0.0.7/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/.github/workflows/owasp.yml` & `pubtools_sign-0.0.7/.github/workflows/owasp.yml`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/.github/workflows/release.yml` & `pubtools_sign-0.0.7/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/.github/workflows/tox-tests.yml` & `pubtools_sign-0.0.7/.github/workflows/tox-tests.yml`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/docs/Makefile` & `pubtools_sign-0.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/docs/make.bat` & `pubtools_sign-0.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/docs/source/CHANGELOG.rst` & `pubtools_sign-0.0.7/docs/source/CHANGELOG.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 ChangeLog
 =========
 
+0.0.7 (02-05-2024)
+-------------------
+Fixed cosign OOM
+
 0.0.6 (25-04-2024)
 -------------------
 Add OTEL trace instrument for signing
 Added send+recv retry cycles
 
 0.0.5 (19-02-2024)
 -------------------
```

### Comparing `pubtools_sign-0.0.6/docs/source/conf.py` & `pubtools_sign-0.0.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/src/pubtools/sign/utils.py` & `pubtools_sign-0.0.7/src/pubtools/sign/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from concurrent import futures
 from concurrent.futures.thread import ThreadPoolExecutor
 from dataclasses import dataclass, field
 import datetime
 import subprocess
 import os
 import logging
-from typing import Any, Dict, List, Union, Callable, cast, Iterable
+import time
+from typing import Any, Dict, List, Union, Callable, cast, Iterable, Tuple
 
 from .conf.conf import CONFIG_PATHS
 
 from pubtools.tracing import get_trace_wrapper
 
 tw = get_trace_wrapper()
+LOG = logging.getLogger("pubtools.sign.utils")
 
 
 def set_log_level(logger: logging.Logger, level: str) -> None:
     """Set log level for provided logger.
 
     :param logger: logger
     :type logger: logging.Logger
@@ -46,20 +48,41 @@
 
     :return: str
     """
     return datetime.datetime.utcnow().isoformat() + "Z"
 
 
 @tw.instrument_func(args_to_attr=True)
-def run_command(cmd: List[str], env: Union[Dict[str, Any], None] = None) -> Any:
-    """Run external command and return Process instance."""
-    process = subprocess.Popen(
-        cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True, env=env
-    )
-    return process
+def run_command(
+    cmd: List[str], env: Union[Dict[str, Any], None] = None, tries: int = 3
+) -> Tuple[str, str, int]:
+    """Run external command and return stdout, stderr and returncode."""
+
+    def _run_command(
+        cmd: List[str], env: Union[Dict[str, Any], None] = None
+    ) -> Tuple[str, str, int]:
+        process = subprocess.Popen(
+            cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True, env=env
+        )
+        stdout, stderr = process.communicate()
+        return (stdout, stderr, process.returncode)
+
+    for i in range(tries):
+        stdout, stderr, returncode = _run_command(cmd, env)
+        if returncode != 0:
+            wait_time = i * 10
+            LOG.warning(
+                "Run command failed. Will retry in %d seconds [try %s/%s]: %s"
+                % (wait_time, i + 1, tries, stderr)
+            )
+            time.sleep(wait_time)
+            stdout, stderr, returncode = _run_command(cmd, env)
+        else:
+            break
+    return (stdout, stderr, returncode)
 
 
 def _get_config_file(config_candidate: str) -> str:
     if not os.path.exists(config_candidate):
         for config_candidate in CONFIG_PATHS:
             if os.path.exists(os.path.expanduser(config_candidate)):
                 break
```

### Comparing `pubtools_sign-0.0.6/src/pubtools/sign/ansible/msg_clear_sign.py` & `pubtools_sign-0.0.7/src/pubtools/sign/ansible/msg_clear_sign.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/src/pubtools/sign/clients/msg.py` & `pubtools_sign-0.0.7/src/pubtools/sign/clients/msg.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/src/pubtools/sign/clients/msg_recv_client.py` & `pubtools_sign-0.0.7/src/pubtools/sign/clients/msg_recv_client.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/src/pubtools/sign/clients/msg_send_client.py` & `pubtools_sign-0.0.7/src/pubtools/sign/clients/msg_send_client.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/src/pubtools/sign/clients/registry.py` & `pubtools_sign-0.0.7/src/pubtools/sign/clients/registry.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/src/pubtools/sign/conf/conf.py` & `pubtools_sign-0.0.7/src/pubtools/sign/conf/conf.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/src/pubtools/sign/operations/base.py` & `pubtools_sign-0.0.7/src/pubtools/sign/operations/base.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/src/pubtools/sign/operations/clearsign.py` & `pubtools_sign-0.0.7/src/pubtools/sign/operations/clearsign.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/src/pubtools/sign/operations/containersign.py` & `pubtools_sign-0.0.7/src/pubtools/sign/operations/containersign.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/src/pubtools/sign/results/__init__.py` & `pubtools_sign-0.0.7/src/pubtools/sign/results/__init__.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/src/pubtools/sign/results/clearsign.py` & `pubtools_sign-0.0.7/src/pubtools/sign/results/clearsign.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/src/pubtools/sign/results/containersign.py` & `pubtools_sign-0.0.7/src/pubtools/sign/results/containersign.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/src/pubtools/sign/results/signing_results.py` & `pubtools_sign-0.0.7/src/pubtools/sign/results/signing_results.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/src/pubtools/sign/signers/__init__.py` & `pubtools_sign-0.0.7/src/pubtools/sign/signers/__init__.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/src/pubtools/sign/signers/cosignsigner.py` & `pubtools_sign-0.0.7/src/pubtools/sign/signers/cosignsigner.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,15 +228,15 @@
             signer=self,
             operation=operation,
             signer_results=signer_results,
             operation_result=operation_result,
         )
 
         outputs = {}
-        processes = {}
+        ref_args = {}
         common_args = [
             self.cosign_bin,
             "-t",
             self.timeout,
             "sign",
             "-y",
             "--key",
@@ -252,24 +252,20 @@
         if self.registry_password:
             common_args += ["--registry-password", self.registry_password]
         env_vars = os.environ.copy()
         env_vars.update(self.env_variables)
         if operation.references:
             for ref, digest in zip(operation.references, operation.digests):
                 repo, tag = ref.rsplit(":", 1)
-                processes[f"{repo}:{digest}"] = run_command(
-                    common_args + ["-a", f"tag={tag}", f"{repo}@{digest}"],
-                    env=env_vars,
-                )
+                ref_args[f"{repo}@{digest}"] = ["-a", f"tag={tag}", f"{repo}@{digest}"]
         else:
             for ref_digest in operation.digests:
-                processes[f"{ref_digest}"] = run_command(common_args + [ref_digest], env=env_vars)
-        for ref, process in processes.items():
-            stdout, stderr = process.communicate()
-            outputs[ref] = (stdout, stderr, process.returncode)
+                ref_args[ref_digest] = [ref_digest]
+        for ref, args in ref_args.items():
+            outputs[ref] = run_command(common_args + args, env=env_vars, tries=self.retries)
 
         for ref, (stdout, stderr, returncode) in outputs.items():
             if returncode != 0:
                 operation_result.results.append(stderr)
                 operation_result.failed = True
                 signing_results.signer_results.status = "failed"
                 signing_results.signer_results.error_message += stderr
@@ -296,20 +292,19 @@
         ]
         if self.registry_user:
             common_args += ["--registry-username", self.registry_user]
         if self.registry_password:
             common_args += ["--registry-password", self.registry_password]
         env_vars = os.environ.copy()
         env_vars.update(self.env_variables)
-        process = run_command(
+        stdout, stderr, returncode = run_command(
             common_args + [reference],
             env=env_vars,
         )
-        stdout, stderr = process.communicate()
-        if process.returncode != 0:
+        if returncode != 0:
             return False, stderr
         else:
             ret, err_msg = self.container_registry_client.check_container_image_exists(
                 stdout.strip("\n"), auth_token=self.auth_token
             )
             if ret:
                 return True, stdout.split("\n")
```

### Comparing `pubtools_sign-0.0.6/src/pubtools/sign/signers/msgsigner.py` & `pubtools_sign-0.0.7/src/pubtools/sign/signers/msgsigner.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/tests/conftest.py` & `pubtools_sign-0.0.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/tests/conftest_cosignsig.py` & `pubtools_sign-0.0.7/tests/conftest_cosignsig.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         tmpf.write(
             """
 cosign_signer:
   timeout: 30s
   rekor_url: https://rekor.sigstore.dev
   registry_user: some-user
   registry_password: some-password
+  retries: 1
   log_level: debug
         """.encode(
                 "utf-8"
             )
         )
         tmpf.flush()
         yield tmpf.name
```

### Comparing `pubtools_sign-0.0.6/tests/conftest_msgsig.py` & `pubtools_sign-0.0.7/tests/conftest_msgsig.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/tests/test_ansible_clearsign.py` & `pubtools_sign-0.0.7/tests/test_ansible_clearsign.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/tests/test_bundle.py` & `pubtools_sign-0.0.7/tests/test_bundle.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/tests/test_config.py` & `pubtools_sign-0.0.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/tests/test_cosign_signer.py` & `pubtools_sign-0.0.7/tests/test_cosign_signer.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/tests/test_msg_handle.py` & `pubtools_sign-0.0.7/tests/test_msg_handle.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/tests/test_msg_recv_client.py` & `pubtools_sign-0.0.7/tests/test_msg_recv_client.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/tests/test_msg_send_client.py` & `pubtools_sign-0.0.7/tests/test_msg_send_client.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/tests/test_msg_signer.py` & `pubtools_sign-0.0.7/tests/test_msg_signer.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/tests/test_registry_client.py` & `pubtools_sign-0.0.7/tests/test_registry_client.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/tests/test_results.py` & `pubtools_sign-0.0.7/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/tests/test_sign_operations.py` & `pubtools_sign-0.0.7/tests/test_sign_operations.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/tests/test_utils.py` & `pubtools_sign-0.0.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/.gitignore` & `pubtools_sign-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/LICENSE` & `pubtools_sign-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.6/pyproject.toml` & `pubtools_sign-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "pubtools-sign"
 description = "Collection of tools producing signed artifacts"
 readme = "README.rst"
 requires-python = ">=3.7"
-version = "0.0.6"
+version = "0.0.7"
 
 classifiers = [  # Optional
   # How mature is this project? Common values are
   #   3 - Alpha
   #   4 - Beta
   #   5 - Production/Stable
   "Development Status :: 3 - Alpha",
```

### Comparing `pubtools_sign-0.0.6/PKG-INFO` & `pubtools_sign-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pubtools-sign
-Version: 0.0.6
+Version: 0.0.7
 Summary: Collection of tools producing signed artifacts
 Author-email: Jindrich Luza <jluza@redhat.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

