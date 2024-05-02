# Comparing `tmp/ironic-python-agent-9.8.0.tar.gz` & `tmp/ironic-python-agent-9.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ironic-python-agent-9.8.0.tar", last modified: Thu Nov 30 09:34:23 2023, max compression
+gzip compressed data, was "ironic-python-agent-9.9.0.tar", last modified: Thu Feb  1 10:59:12 2024, max compression
```

## Comparing `ironic-python-agent-9.8.0.tar` & `ironic-python-agent-9.9.0.tar`

### file list

```diff
@@ -1,480 +1,488 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.173299 ironic-python-agent-9.8.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8107 2023-11-30 09:34:22.000000 ironic-python-agent-9.8.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    68666 2023-11-30 09:34:22.000000 ironic-python-agent-9.8.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      561 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3438 2023-11-30 09:34:23.173299 ironic-python-agent-9.8.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      835 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.097299 ironic-python-agent-9.8.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.097299 ironic-python-agent-9.8.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.097299 ironic-python-agent-9.8.0/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10195 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/doc/source/admin/hardware_managers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10359 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/doc/source/admin/how_it_works.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/doc/source/admin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1757 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/doc/source/admin/rescue.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10282 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/doc/source/admin/troubleshooting.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2394 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.101299 ironic-python-agent-9.8.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13834 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/doc/source/contributor/hardware_managers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2177 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/doc/source/contributor/metrics.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1582 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/doc/source/contributor/rescue.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.101299 ironic-python-agent-9.8.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6877 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.101299 ironic-python-agent-9.8.0/examples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1711 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/examples/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.101299 ironic-python-agent-9.8.0/examples/business-logic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8581 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/examples/business-logic/example_business_logic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/examples/business-logic/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/examples/business-logic/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.101299 ironic-python-agent-9.8.0/examples/custom-disk-erase/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2348 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/examples/custom-disk-erase/example_disk_eraser.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      562 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/examples/custom-disk-erase/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/examples/custom-disk-erase/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.101299 ironic-python-agent-9.8.0/examples/vendor-device/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6669 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/examples/vendor-device/example_device.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/examples/vendor-device/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/examples/vendor-device/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.101299 ironic-python-agent-9.8.0/imagebuild/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/imagebuild/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.105299 ironic-python-agent-9.8.0/ironic_python_agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1218 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20336 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/agent.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.105299 ironic-python-agent-9.8.0/ironic_python_agent/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8659 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/api/app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16063 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/burnin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.109299 ironic-python-agent-9.8.0/ironic_python_agent/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2397 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/cmd/agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      914 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/cmd/inspect.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20654 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4090 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/dmi_inspector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15965 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/efi_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2692 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/encoding.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12142 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/errors.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.109299 ironic-python-agent-9.8.0/ironic_python_agent/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/extensions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13990 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/extensions/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4243 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/extensions/clean.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4307 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/extensions/deploy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1828 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/extensions/flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33196 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/extensions/image.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/extensions/log.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1700 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/extensions/poll.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2610 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/extensions/rescue.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4253 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/extensions/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    46572 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/extensions/standby.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   146554 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/hardware.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.109299 ironic-python-agent-9.8.0/ironic_python_agent/hardware_managers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/hardware_managers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3333 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/hardware_managers/cna.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6885 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/hardware_managers/mlnx.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.109299 ironic-python-agent-9.8.0/ironic_python_agent/hardware_managers/nvidia/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35365 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/hardware_managers/nvidia/nvidia_fw_update.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9476 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/inject_files.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5148 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/inspect.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14493 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/inspector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12795 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/ironic_api_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14227 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/netutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10331 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/numa_inspector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31964 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/partition_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18235 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/raid_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.109299 ironic-python-agent-9.8.0/ironic_python_agent/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.109299 ironic-python-agent-9.8.0/ironic_python_agent/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3838 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/functional/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3656 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/functional/test_commands.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.117299 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3270 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22841 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/dmi_inspector_data.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.117299 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10145 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11831 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/test_clean.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11843 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/test_deploy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4358 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/test_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   110879 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/test_image.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1398 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/test_log.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2776 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/test_poll.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4188 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/test_rescue.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12105 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    99432 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/test_standby.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.117299 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/hardware_managers/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/hardware_managers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.117299 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/hardware_managers/nvidia/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/hardware_managers/nvidia/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    53130 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/hardware_managers/nvidia/test_nvidia_fw_update.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7103 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/hardware_managers/test_cna.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7847 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/hardware_managers/test_mlnx.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.121299 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    53498 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/samples/hardware_samples.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    51216 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13193 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2815 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21146 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_burnin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4833 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_dmi_inspector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29022 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_efi_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2763 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_encoding.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6022 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_errors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   285271 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_hardware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17824 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_inject_files.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24075 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_inspector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24336 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_ironic_api_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7947 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_multi_hardware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4665 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_multi_hardware_clean_steps.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13272 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_netutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18131 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_numa_inspector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    77377 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_partition_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18467 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_raid_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3340 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_tls_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49689 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4771 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/tls_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33708 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      754 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/ironic_python_agent/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.105299 ironic-python-agent-9.8.0/ironic_python_agent.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3438 2023-11-30 09:34:22.000000 ironic-python-agent-9.8.0/ironic_python_agent.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24366 2023-11-30 09:34:23.000000 ironic-python-agent-9.8.0/ironic_python_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-11-30 09:34:22.000000 ironic-python-agent-9.8.0/ironic_python_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1548 2023-11-30 09:34:22.000000 ironic-python-agent-9.8.0/ironic_python_agent.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-11-30 09:34:22.000000 ironic-python-agent-9.8.0/ironic_python_agent.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-11-30 09:34:22.000000 ironic-python-agent-9.8.0/ironic_python_agent.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2023-11-30 09:34:22.000000 ironic-python-agent-9.8.0/ironic_python_agent.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2023-11-30 09:34:22.000000 ironic-python-agent-9.8.0/ironic_python_agent.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/plugin-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.121299 ironic-python-agent-9.8.0/releasenotes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/config.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.169299 ironic-python-agent-9.8.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/4k-block-size-config-drives-4470828dd06d2600.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/Collect_NIC_name_given_by_BIOS-657c68c0ae16365b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/LLDP-ignore-NICs-that-are-not-plugged-in-29213f0a701a72e4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/ability-to-disable-secure-erase-c3223262726d5aff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add-block-device-uuid-c8b38264e1688110.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add-coreos-dhcp-rescue-support-1dd8e9d5ac9c7594.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add-disk-wait-config-opts-fe805292baca8029.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add-erase-devices-express-1df107c75f2b3627.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add-hostname-8bbf24712b6a4919.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add-inspection-retry-1d385f69607c1452.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add-log-extension-35ca22cc0709af4c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add-more-lan-channels-8f5197ed5f057c25.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add-named-logfiles-to-burnin-4388309bf7442d53.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add-numa-topology-info-8c253fd9e56169f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add-optional-tls-support-3ab6a834154fedec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add-pci-devices-info-3f86934a505d1b31.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add-portal-port-arg-6d4faec2f709c8e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add-secondary-sorting-by-name-for-root-disks-4de2c0358b9a1e2c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add-service-steps-support-655cc02d112ed0a8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add-smart-test-to-disk-burnin-d02d31e23e5efa9a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add-unit-test-cc4a1a05859ad17d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add-vendor-info-56be9a8605d80bf0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add-vlan-interfaces-cdfeb39d0f3d444d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add_burnin_cpu-9acbb36048246a6b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add_burnin_disk-12adb5735a41af47.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      981 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add_burnin_dynamic_network_pairing-33e398255050eb98.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add_burnin_memory-4099ca42bd3b99db.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add_burnin_network-4856153d21c25f4a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add_erase_pstore-b109c58ed8f5d351.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add_interface_vendor_and_product-74e9815f20ee0cac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/add_mellanox_hardware_manager-edfae87964737df1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/additional-wwn-hints-ffd02ceafcb3dc70.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/adds-nvme-secure-erase-0ecfd624e5f50581.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      528 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/adds-smartctl-ata-check-to-secure-erase-caebba4f25821575.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/advertise-address-c3b152fe475fb539.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/advertise-protocol-110ae1587f727e62.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/agent-fully-retries-image-downloads-67409a493c6d08ae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/agent-token-support-1086218cf2a0c917.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/agent_partition_image-91941adc6683c673.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/allows-bootloader-install-failure-to-be-ignored-b99667b13afa9759.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/append-efi-partition-to-fstab-e9f945a4dd19bd7a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/apply-raid-aeca7848c6320d6b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      769 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/ataraid_does_not_appear_as_disk-8a260e66b3496bf6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/attempts-ata-disk-unlock-897d76c494ec2976.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/auto-tls-b52b873663f35618.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/avoid-grub2-using-efibootmgr-bd27c0978d1cf71b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/bandit-fixes-a971142075b29ca9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1766 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/basic-auth-for-user-image-server-150835e7567444da.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/bindmount-run-4c6a31d3ee4e0ed6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/block-device-hctl-e81573812be3d469.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/bmc-mac-introspection-e4c2e203d8529710.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/bmo-extra-147559c8d1776e8c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/boot-info-f18336ada089f6dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/bootloader-ignored-uefi-mode-8578a009d5b5be62.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/bug-2010123-d4c38d8f6606d0e0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/build-tinyipa-with-python3-d4a64aa18f970968.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/build-tinyipa-with-tinycore8-b39d0415b1c25f6b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/bumpsipalookupattempts-29de7c949aaf6556.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/cache-image-removal-3b5a80a6038a320b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/capture-early-logging-0f3fa58d75656117.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/change-heartbeat-method-d0119406137022e3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/check-if-ESP-is-mounted-f9e0eff3609c2668.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/check-partition-table-after-writing-34efbd557d8de7cb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1478 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/check-virtual-media-devices-a9b1f54c3fe7884d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/checksum-before-considering-download-completed-91cca9fef34d8cf5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      481 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/clarify-heartbeat-connection-errors-2af152bf2d7928e2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/clock-skew-1fbf542b193cec17.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/coalesce_heartbeats-fb8899a5f9fe4709.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/collect-dmi-output-f2e9feabef16bacf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/collect-manager-a80bcf370048eeec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/collect-more-8bc9ad4c63e873e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/collect-udev-f6ada5163cf4a26c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/command_params-869fa547b5be2236.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/configdrive-dup-3fc46a878fe82485.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/configdrive-partuuid-3259cfb7428c1483.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/configdrive-ssl-02b069948dfef814.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/container-poweroff-d9ffb637cf1cee6c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/coreos-uses-chroot-8a01ba0b38a4a4f4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/coreos_ipa_image_poweroff_reboot_in_chroot_by_sysrq-42447fc4cdd7dafe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/correct-uefi-regex-112211c2427cd4d9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/correction-failure-output-when-downloading-image-39f93838d1ed2928.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/cpu-flags-e3cec7e5cba069ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/create_raids_with_volume_name-93e0bb59ef210fe4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/de-duplicate-by-label-baa090c5b1bff992.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1703 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/deprecate-coreos-8b01bcf796c0dc54.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/detect-endianness-f53a6c4571aba3fe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/device-hints-from-node-object-9a689f5a4175a1a6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      461 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/disable-md5-image-checksum-7def176928d36e75.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/discover-ipv6-bmc-address-b3b357ff6c5d822c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/disk-label-fix-536897e41a4d817f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/disk-wait-2e0e85e0947f80e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/drop-python2-2006fd8a4a6de56d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/efi-partuuid-5fe933a462eeede1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      643 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/enable-cleaning-fallback-57e8c9aa2f24e63d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/enable-skipping-disks-0c4c8b72231715a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/enable-skipping-raids-40263cc3a19cfd27.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/enhance-checksum-2256ffdcce13836e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/erase-deploy-step-3e952fa863bca908.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/erase-device-metadata-clean-step-31b4a615c0ff7f18.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/erase_metadata_from_partitions-4f1902533d530b8f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/executes-gpt-partition-fix-b6156cc16da00dfc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      421 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/extend-ipa-lookup-timeout-05ee5b1372792dbe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/extend-pci-metric-5482284d6a9fe765.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/extend-retry-timeout-30c930a33d97c193.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fail_ipa_start_if_ironic_api_invalid-7b78fcaba2141cc5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fallback-to-findfs-59abde55221e1e84.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fasttrack-stale-cache-fd93b56a955c7ab1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/feature-2010228-cf3a59b88f07c3a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fetc-checksum-support-additional-format-4b29c5cdaa6b8d16.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/findbonds-733c7c91a5665b05.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-agent-determination-of-partition-table-type-3c78bf78266e8cef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-agent-unable-to-stop-py3-6c210793476968d1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-auxillarly-node-lookup-argument-83d3f717c039e454.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-bmc-ip-detection-for-coreos-483be0286593e393.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-boot-mode-for-partition-images-f96cf2b3c27b6533.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-bootloader-install-with-mdraid-0a254035df9d0bed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-bytes-json-serializable-collected-logs-ad61022b287dc3e2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-clean-config-for-full-device-28ee09b58d97d122.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-cleaning-read-only-device-c8a0f4cc2f434d99.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-coreos-modprobe-75bda45c7bbeb469.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-hardcoded-path-to-grub-7006f29a9ef72e75.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-high-cpu-usage-eventlet-1dccf3b81dd42c47.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-iscsi-teardown-handling-0df2345318d3c843.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-local-boot-for-partition-images-755f570dc0982868.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-mlnx-hardware-mgr-never-run-72072580be4d6e7a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-multipath-parent-device-e85afad63159250c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-nic-without-numa-node-b401f97c46afa4a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-nvidia-hw-mgr-https-38825a4161a8561b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-nvme-partition-image-handling-b8487133a188fd32.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-nvme-software-raid-race-2e0e104de9611228.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-physical-memory-arm64-957755f6cd91ad85.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-rescan-device-7b00c6836b687ce8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-rescan-device-raid-29aa1558b036b496.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-softraid-name-poisoning-4e934dd4e60830b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-to-pass-root-uuid-for-whole-disk-image-1c13b70f6b74bce0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-uefi-boot-entry-creation-for-aarch64-2b143c5bf189c2f6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix-vfd-mount-for-capitalized-device-name-db7f519e900f4e22.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix_chronyd_time_sync-626a14b66ca37677.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix_efi_uuid_fstab-f2edbee9bfbac64a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fix_partition_cleanup-46491861c930db12.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fixes-agent-lookup-retries-1b4bb90b8e783aca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fixes-centos-fedora-grub2-mkconfig-hang-fe22cde231994044.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fixes-efibootmgr-character-encoding-19e531ba694824c1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/fixes-error-handling-of-efibootmgr-not-present-in-ramdisk-f11b4241edcf0e81.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/get-holder-disks-with-nvme-7d5fa75df2fd5904.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/get-physical-memory-535a32362bcdf83a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/get_md_components_by_uuid-7f08d423ea9e7c94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/get_numa_node-eeab34a92739b6f6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/handle-configdrive-large-disks-3517e9fcf16c7f39.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/handle-fd0-devices-3d1f31c3b34819e8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/handle-partuuid-for-fstab-e0aadea20a056982.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/handle-ssl-063a91fb7bdcf9b9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      532 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/ignore-grub-efi-fail-dcf7eb07f61f4388.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/image-checksum-39b2ceef40933c28.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/image-download-retries-65ac31fe4328e438.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/improve-tgtd-status-d17173dc8f67959f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/inject-files-b411369ce6856dac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/inspect-to-clean-b3616d843775c187.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/inspection-to-report-disk-by-path-e3fd4c331d200903.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/inspection-wait-for-ips-223e39b65fef31bd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/inspection-wait-for-ips-v2-146016f758d7010c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/inspector-logs-9b7c010c219691d2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/instance-info-root-device-02fed0966bb00fb3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/inventory-conf-29b59ebe97aefbde.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/ip6-addresses-1c2b9bcd9a124de7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/ipa-debug-68c86101b1fdc3d9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/ipmi-address-channel-b6b8010c41d05c1b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/ipmi-cleanup-a4454f6851d81c4d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/ipv6-listen-85d40e58156e398f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/ipv6-provision-42e9000f6f6a7a3a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/ironic-error-97e76d9ddacff039.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/iscsi-detection-on-diskless-hw-f27dcce3aaa35ac2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/jitter-for-inspection-command-5a226927757a0308.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/let_crypt_generate_the_salt-99876591325275a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/lib-exc-41ee122eb4a04bc4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/limit-qemu-img-malloc-arena-025ed84115481eae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/limit-qemu-img-ram-usage-d7b7a16ac5e9c917.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/lldp-error-handling-5b6576b378ef9c3a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/lldp-loop-fdfa584caf33d847.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/lldp-raw-a09174cb930bca97.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/log-download-size-57982fa8df336520.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/log-file-7aaaf31693ddc617.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/logs-collector-non-ascii-010339bf256443c8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/lsblk-all-956c1df808a169bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/lshw-cb89894be057bdc9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/lshw-for-memory-and-system-info-35c69da067c72b36.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/lshw-no-memory-bank-size-05ea71987362986e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/manual-introspection-b04b5c25f5e004ac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/manually-configure-ironic-api-version-517afd0a423036ad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/md-restart-9e0d47863a086792.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/mdadm-d5b8c186182620b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/mdns-e020484e64d76edb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/min-ironic-ocata-dff80e567783e87c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/mlnx-steps-now-available-for-deploy-4a4226ffaae888f3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/move_swraid_to_efibootmgr-d87c1bfde1661fb5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/multipath-handling-00a5b412d2cf2e4e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/multipath-serial-615fc925984abbf7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1243 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/multipath_error_handling_improvement-1669d0de4bfdbe95.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/multiple-lan-channels-ee32d80150f990bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/name-root-device-hints-0cfc8c90d03c8bf0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/net-speed-8854901e2051bb79.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/new-agent-api-afbe7391493749be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/new-sync-command-6f5fa55df2fd5903.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/no-bash-for-grub-c38369af8cc7cf26.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/no-coreos-3345cc69009dead9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/no-iscsi-fd21808edbea5ac2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/no-link-local-2e861978c5c7bf30.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/no-mac-54616606ee6b844d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/no-netboot-d034bb1d1d9166c5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/no-sample-ac11bd0fa27af62a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/no-standalone-bb34eae2cc468837.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/no-zram-78cc6583f4f90a9c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/old-inspector-data-5e63c9bce72b4fb5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/oslo-config-generator-b0f70b9fb7e23997.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/parallel-erase-disk-devices-09ea33d5443aead0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/partition_check_read_only_base_device-5bc15ac2f034aca9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/permit-pre-hashed-rescue-passwords-4275f6e697533cec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/pint-0.5-816aaf3a4f6d4a6e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/poll-mode-063bd36b2b18bffb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/prefix-lldp-timeout-50acc656313d8dd2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/prepare-image-49744276cef719d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/preserve-efi-folder-contents-ea1e278b3093ec55.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1151 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/prevent-deletion-of-shared-disk-filesystems-4c17c7666d2fe3bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/prevent-needless-iscsi-cleanup-f8d602c0abc7e8ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/prioritize-lsblk-device-serials-8cae406ca5164a01.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/qemu-img-ooo-write-721b8a0057ab7b8a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/qemu-write-zeros-2edbf3152c57e2b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/raid-esp-size-2c322adb2d3b9ce7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/raid-hints-604f9ffdd86432eb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/raid5-6-support-0807597c3633a26c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/readd_missing_devs-2ed85805388b6e42.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/rebuild_on_esp_raid-33f359bdf5ccaa09.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/relax-checksum-feeding-11044ae02b411a07.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/remove-lldp-timeout-ea481dbb01a39522.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/remove-switch_port_descr-switch_chassis_descr-40f2bb37b5f1fdd1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/remove-sysrq-2c2804930180f408.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/remove-vendor-passthru-eda3519c322eb4e2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/rescan-before-checking-uefi-64597c937880134d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/rescan-device-after-mkfs-3f9d52a2e3b6fff3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/rescue-dhcp_network-for-tinyipa-a14de5fae38a5dce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/respect-listen-directives-94fb863c5b692c07.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      473 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/rework-ata-secure-erase-c6684962ef078281.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/root-device-hints-rotational-67e6e61074c26561.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/set-clock-prior-to-poweroff-af6ec210aad8b45a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/skip-lookup-and-heartbeat-if-apiurl-not-configured-5ae8b04ae1e74673.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/skips-bootloader-install-35c463195aa61800.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/sleep-ebe58fbe07d30219.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/softraid-bootable-with-uefi-aa22e6cbaf1ea747.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/softraid-creation-on-nvme-a2fd4c531d200904.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/softraid-partitioning-refactor-104b817c3bdc73e3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/softraid-zap-superblocks-anywhere.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/software-raid-4a88e6c5af9ea742.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/software-raid-raid-ESPs-25a2aa117b99620a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/software-raid-use-label-as-rootfs-uuid-d9a3827180f1a238.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/software_raid_use_rootfs_uuid-9149cc0c8638d5d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/start_passing_agent_version_to_ironic-6fa8670ae0e7eb38.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      567 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/stream-raw-images-d2e245aaed991d86.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/streaming-partition-images-cdeb260ef8f90012.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/streaming-uuid-fdf136a7745fbb3d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1083 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/support-bootloader-csv-file-use-c815b520c600cd98.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/support-collecting-ipv6-address-dd819d543f851a63.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/support-image-proxy-e2987a6589375451.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/support-linux-io-6bbd7ff1f0d70a0e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/support-lldp-in-inventory-4ab6e45ccd35dace.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/support-prep-partitions-5e273572ab7ce018.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/suse-tinyipa-support-20acecd6d7b20952.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/sw-raid-assemble-9c20fe967f73d1dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/timeout_on_file_download-ed77918318316075.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/tinycore-ipv6-1b620c61402b5720.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/tinyipa-python3-default-b8434793e17465db.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/tinyipa-rescue-dhcp-multi-tenant-b32bda7bf2b12679.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/tinyipa-ssh-e8a3a01a3f3ff5f4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/udev-settle-f75db34db990ad68.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/udevadm-settle-9d3e5f1f20211857.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/uefi-esp-660fc2c650e6af92.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/uefi-fallback-266c647f6aff58fd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/uefi-images-38c8536db189ffc1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      698 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/understand-node-conflict-is-locked-2ea21dd45abfe4f7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/up-qemuimg-mem-1536183a02b3a235.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/use-latest-coreos-87f826d26b46548d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/use-system-random-00b0721c8ebd0c5a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/vmedia-copy-6a58f3183b166c42.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/wait-for-interfaces-before-lookup-9bf38852b2f176a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/wait-root-device-504b517c3aec73e2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/whole-disk-grub-0b1b8b9c44e31d28.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/notes/zero-size-78d3be2ac8fd59c2.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.169299 ironic-python-agent-9.8.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.169299 ironic-python-agent-9.8.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.169299 ironic-python-agent-9.8.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9279 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/liberty.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2608 2023-11-30 09:34:23.173299 ironic-python-agent-9.8.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      716 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.173299 ironic-python-agent-9.8.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8385 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/tools/bandit.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.173299 ironic-python-agent-9.8.0/tools/config/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1015 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/tools/config/check_uptodate.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/tools/config/ipa-config-generator.conf
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1233 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/tools/run_bashate.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/tools/with_venv.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4385 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-30 09:34:23.173299 ironic-python-agent-9.8.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5210 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/zuul.d/ironic-python-agent-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1527 2023-11-30 09:33:54.000000 ironic-python-agent-9.8.0/zuul.d/project.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.581787 ironic-python-agent-9.9.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/.git-blame-ignore-revs
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8270 2024-02-01 10:59:12.000000 ironic-python-agent-9.9.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    69662 2024-02-01 10:59:12.000000 ironic-python-agent-9.9.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      561 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3489 2024-02-01 10:59:12.581787 ironic-python-agent-9.9.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      835 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.541787 ironic-python-agent-9.9.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.541787 ironic-python-agent-9.9.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.541787 ironic-python-agent-9.9.0/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10196 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/doc/source/admin/hardware_managers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10377 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/doc/source/admin/how_it_works.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1757 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/doc/source/admin/rescue.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10786 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/doc/source/admin/troubleshooting.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2394 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.541787 ironic-python-agent-9.9.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13834 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/doc/source/contributor/hardware_managers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2177 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/doc/source/contributor/metrics.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1584 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/doc/source/contributor/rescue.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.541787 ironic-python-agent-9.9.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6877 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.541787 ironic-python-agent-9.9.0/examples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1711 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/examples/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.541787 ironic-python-agent-9.9.0/examples/business-logic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8581 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/examples/business-logic/example_business_logic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/examples/business-logic/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/examples/business-logic/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.541787 ironic-python-agent-9.9.0/examples/custom-disk-erase/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2348 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/examples/custom-disk-erase/example_disk_eraser.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      562 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/examples/custom-disk-erase/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/examples/custom-disk-erase/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.541787 ironic-python-agent-9.9.0/examples/vendor-device/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6671 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/examples/vendor-device/example_device.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/examples/vendor-device/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/examples/vendor-device/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.541787 ironic-python-agent-9.9.0/imagebuild/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/imagebuild/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.545787 ironic-python-agent-9.9.0/ironic_python_agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1218 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22743 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/agent.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.545787 ironic-python-agent-9.9.0/ironic_python_agent/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8659 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/api/app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16063 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/burnin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.545787 ironic-python-agent-9.9.0/ironic_python_agent/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1685 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/cmd/agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      914 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/cmd/inspect.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20777 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4090 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/dmi_inspector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16128 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/efi_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2692 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/encoding.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12143 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/errors.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.545787 ironic-python-agent-9.9.0/ironic_python_agent/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/extensions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13990 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/extensions/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4243 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/extensions/clean.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4307 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/extensions/deploy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1828 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/extensions/flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33174 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/extensions/image.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/extensions/log.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1700 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/extensions/poll.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2610 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/extensions/rescue.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4253 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/extensions/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    46585 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/extensions/standby.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   146682 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/hardware.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.545787 ironic-python-agent-9.9.0/ironic_python_agent/hardware_managers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/hardware_managers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3333 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/hardware_managers/cna.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6885 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/hardware_managers/mlnx.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.545787 ironic-python-agent-9.9.0/ironic_python_agent/hardware_managers/nvidia/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35365 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/hardware_managers/nvidia/nvidia_fw_update.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9476 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/inject_files.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5149 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/inspect.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15546 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/inspector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13762 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/ironic_api_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14227 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/netutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10331 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/numa_inspector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31965 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/partition_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18237 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/raid_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.545787 ironic-python-agent-9.9.0/ironic_python_agent/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.545787 ironic-python-agent-9.9.0/ironic_python_agent/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3838 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/functional/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3656 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/functional/test_commands.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.549787 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3270 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22841 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/dmi_inspector_data.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.549787 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10145 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11831 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/test_clean.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11843 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/test_deploy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4358 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/test_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   110878 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/test_image.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1398 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/test_log.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2776 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/test_poll.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4188 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/test_rescue.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12105 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    99434 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/test_standby.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.549787 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/hardware_managers/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/hardware_managers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.549787 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/hardware_managers/nvidia/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/hardware_managers/nvidia/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    53130 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/hardware_managers/nvidia/test_nvidia_fw_update.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7103 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/hardware_managers/test_cna.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7847 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/hardware_managers/test_mlnx.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.553787 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    53498 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/samples/hardware_samples.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    54555 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13193 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2815 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21145 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_burnin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4833 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_dmi_inspector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30279 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_efi_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2763 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_encoding.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6022 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_errors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   285366 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_hardware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17825 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_inject_files.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26959 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_inspector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24787 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_ironic_api_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7947 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_multi_hardware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4665 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_multi_hardware_clean_steps.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13272 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_netutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18131 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_numa_inspector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    77378 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_partition_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18467 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_raid_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3340 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_tls_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    49689 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4771 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/tls_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33701 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      754 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/ironic_python_agent/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.545787 ironic-python-agent-9.9.0/ironic_python_agent.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3489 2024-02-01 10:59:12.000000 ironic-python-agent-9.9.0/ironic_python_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24798 2024-02-01 10:59:12.000000 ironic-python-agent-9.9.0/ironic_python_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-01 10:59:12.000000 ironic-python-agent-9.9.0/ironic_python_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1548 2024-02-01 10:59:12.000000 ironic-python-agent-9.9.0/ironic_python_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-01 10:59:12.000000 ironic-python-agent-9.9.0/ironic_python_agent.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-02-01 10:59:12.000000 ironic-python-agent-9.9.0/ironic_python_agent.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2024-02-01 10:59:12.000000 ironic-python-agent-9.9.0/ironic_python_agent.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2024-02-01 10:59:12.000000 ironic-python-agent-9.9.0/ironic_python_agent.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/plugin-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.553787 ironic-python-agent-9.9.0/releasenotes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/config.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.577787 ironic-python-agent-9.9.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/4k-block-size-config-drives-4470828dd06d2600.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/Collect_NIC_name_given_by_BIOS-657c68c0ae16365b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/LLDP-ignore-NICs-that-are-not-plugged-in-29213f0a701a72e4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/ability-to-disable-secure-erase-c3223262726d5aff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add-block-device-uuid-c8b38264e1688110.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add-coreos-dhcp-rescue-support-1dd8e9d5ac9c7594.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add-disk-wait-config-opts-fe805292baca8029.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add-erase-devices-express-1df107c75f2b3627.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add-hostname-8bbf24712b6a4919.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add-inspection-retry-1d385f69607c1452.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add-log-extension-35ca22cc0709af4c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add-more-lan-channels-8f5197ed5f057c25.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add-named-logfiles-to-burnin-4388309bf7442d53.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add-numa-topology-info-8c253fd9e56169f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add-optional-tls-support-3ab6a834154fedec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add-pci-devices-info-3f86934a505d1b31.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add-portal-port-arg-6d4faec2f709c8e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add-secondary-sorting-by-name-for-root-disks-4de2c0358b9a1e2c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add-service-steps-support-655cc02d112ed0a8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add-smart-test-to-disk-burnin-d02d31e23e5efa9a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add-unit-test-cc4a1a05859ad17d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add-vendor-info-56be9a8605d80bf0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add-vlan-interfaces-cdfeb39d0f3d444d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add_burnin_cpu-9acbb36048246a6b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add_burnin_disk-12adb5735a41af47.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      981 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add_burnin_dynamic_network_pairing-33e398255050eb98.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add_burnin_memory-4099ca42bd3b99db.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add_burnin_network-4856153d21c25f4a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add_erase_pstore-b109c58ed8f5d351.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add_interface_vendor_and_product-74e9815f20ee0cac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/add_mellanox_hardware_manager-edfae87964737df1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/additional-wwn-hints-ffd02ceafcb3dc70.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/adds-nvme-secure-erase-0ecfd624e5f50581.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      531 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/adds-smartctl-ata-check-to-secure-erase-caebba4f25821575.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/advertise-address-c3b152fe475fb539.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/advertise-protocol-110ae1587f727e62.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/agent-fully-retries-image-downloads-67409a493c6d08ae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/agent-token-support-1086218cf2a0c917.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/agent_partition_image-91941adc6683c673.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      843 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/allows-bootloader-install-failure-to-be-ignored-b99667b13afa9759.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/append-efi-partition-to-fstab-e9f945a4dd19bd7a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/apply-raid-aeca7848c6320d6b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      769 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/ataraid_does_not_appear_as_disk-8a260e66b3496bf6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/attempts-ata-disk-unlock-897d76c494ec2976.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/auto-tls-b52b873663f35618.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/avoid-grub2-using-efibootmgr-bd27c0978d1cf71b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/bandit-fixes-a971142075b29ca9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1766 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/basic-auth-for-user-image-server-150835e7567444da.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/bindmount-run-4c6a31d3ee4e0ed6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/block-device-hctl-e81573812be3d469.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/bmc-mac-introspection-e4c2e203d8529710.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/bmo-extra-147559c8d1776e8c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/boot-info-f18336ada089f6dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/bootloader-ignored-uefi-mode-8578a009d5b5be62.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/bug-2010123-d4c38d8f6606d0e0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/build-tinyipa-with-python3-d4a64aa18f970968.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/build-tinyipa-with-tinycore8-b39d0415b1c25f6b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/bumpsipalookupattempts-29de7c949aaf6556.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/cache-image-removal-3b5a80a6038a320b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/capture-early-logging-0f3fa58d75656117.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/change-heartbeat-method-d0119406137022e3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/check-if-ESP-is-mounted-f9e0eff3609c2668.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/check-partition-table-after-writing-34efbd557d8de7cb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1478 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/check-virtual-media-devices-a9b1f54c3fe7884d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/checksum-before-considering-download-completed-91cca9fef34d8cf5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/clarify-heartbeat-connection-errors-2af152bf2d7928e2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/clock-skew-1fbf542b193cec17.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/coalesce_heartbeats-fb8899a5f9fe4709.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/collect-cpu-sockets-0dbc09a1ebccfe77.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/collect-dmi-output-f2e9feabef16bacf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/collect-manager-a80bcf370048eeec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/collect-more-8bc9ad4c63e873e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/collect-udev-f6ada5163cf4a26c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/command_params-869fa547b5be2236.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/configdrive-dup-3fc46a878fe82485.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/configdrive-partuuid-3259cfb7428c1483.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/configdrive-ssl-02b069948dfef814.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/container-poweroff-d9ffb637cf1cee6c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/content-type-f4d5ab15adf37252.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/coreos-uses-chroot-8a01ba0b38a4a4f4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/coreos_ipa_image_poweroff_reboot_in_chroot_by_sysrq-42447fc4cdd7dafe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/correct-uefi-regex-112211c2427cd4d9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/correction-failure-output-when-downloading-image-39f93838d1ed2928.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/cpu-flags-e3cec7e5cba069ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/create_raids_with_volume_name-93e0bb59ef210fe4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/de-duplicate-by-label-baa090c5b1bff992.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1703 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/deprecate-coreos-8b01bcf796c0dc54.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/detect-endianness-f53a6c4571aba3fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/device-hints-from-node-object-9a689f5a4175a1a6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      461 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/disable-md5-image-checksum-7def176928d36e75.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/discover-ipv6-bmc-address-b3b357ff6c5d822c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/disk-label-fix-536897e41a4d817f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/disk-wait-2e0e85e0947f80e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/drop-python2-2006fd8a4a6de56d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/efi-partuuid-5fe933a462eeede1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      643 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/enable-cleaning-fallback-57e8c9aa2f24e63d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/enable-skipping-disks-0c4c8b72231715a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/enable-skipping-raids-40263cc3a19cfd27.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/enhance-checksum-2256ffdcce13836e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/erase-deploy-step-3e952fa863bca908.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/erase-device-metadata-clean-step-31b4a615c0ff7f18.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/erase_metadata_from_partitions-4f1902533d530b8f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/executes-gpt-partition-fix-b6156cc16da00dfc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      421 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/extend-ipa-lookup-timeout-05ee5b1372792dbe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/extend-pci-metric-5482284d6a9fe765.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/extend-retry-timeout-30c930a33d97c193.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fail_ipa_start_if_ironic_api_invalid-7b78fcaba2141cc5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      408 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fallback-to-findfs-59abde55221e1e84.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fasttrack-stale-cache-fd93b56a955c7ab1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/feature-2010228-cf3a59b88f07c3a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fetc-checksum-support-additional-format-4b29c5cdaa6b8d16.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/findbonds-733c7c91a5665b05.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-agent-determination-of-partition-table-type-3c78bf78266e8cef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-agent-unable-to-stop-py3-6c210793476968d1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-auxillarly-node-lookup-argument-83d3f717c039e454.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-bmc-ip-detection-for-coreos-483be0286593e393.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-boot-mode-for-partition-images-f96cf2b3c27b6533.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-bootloader-install-with-mdraid-0a254035df9d0bed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-bytes-json-serializable-collected-logs-ad61022b287dc3e2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-clean-config-for-full-device-28ee09b58d97d122.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-cleaning-read-only-device-c8a0f4cc2f434d99.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-coreos-modprobe-75bda45c7bbeb469.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-hardcoded-path-to-grub-7006f29a9ef72e75.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-high-cpu-usage-eventlet-1dccf3b81dd42c47.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-iscsi-teardown-handling-0df2345318d3c843.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-local-boot-for-partition-images-755f570dc0982868.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-mlnx-hardware-mgr-never-run-72072580be4d6e7a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-multipath-parent-device-e85afad63159250c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-nic-without-numa-node-b401f97c46afa4a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-nvidia-hw-mgr-https-38825a4161a8561b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-nvme-partition-image-handling-b8487133a188fd32.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-nvme-software-raid-race-2e0e104de9611228.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-physical-memory-arm64-957755f6cd91ad85.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-raid_device-not-set-8b03688ce83ce22e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-rescan-device-7b00c6836b687ce8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-rescan-device-raid-29aa1558b036b496.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-softraid-name-poisoning-4e934dd4e60830b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-to-pass-root-uuid-for-whole-disk-image-1c13b70f6b74bce0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-uefi-boot-entry-creation-for-aarch64-2b143c5bf189c2f6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix-vfd-mount-for-capitalized-device-name-db7f519e900f4e22.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix_chronyd_time_sync-626a14b66ca37677.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix_efi_uuid_fstab-f2edbee9bfbac64a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fix_partition_cleanup-46491861c930db12.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fixes-agent-lookup-retries-1b4bb90b8e783aca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fixes-centos-fedora-grub2-mkconfig-hang-fe22cde231994044.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fixes-efibootmgr-character-encoding-19e531ba694824c1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/fixes-error-handling-of-efibootmgr-not-present-in-ramdisk-f11b4241edcf0e81.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/get-holder-disks-with-nvme-7d5fa75df2fd5904.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/get-physical-memory-535a32362bcdf83a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/get_md_components_by_uuid-7f08d423ea9e7c94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/get_numa_node-eeab34a92739b6f6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/handle-configdrive-large-disks-3517e9fcf16c7f39.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/handle-fd0-devices-3d1f31c3b34819e8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/handle-partuuid-for-fstab-e0aadea20a056982.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/handle-ssl-063a91fb7bdcf9b9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/heartbeat-jitter-620bbcba591d2894.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      532 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/ignore-grub-efi-fail-dcf7eb07f61f4388.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/image-checksum-39b2ceef40933c28.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/image-download-retries-65ac31fe4328e438.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/improve-tgtd-status-d17173dc8f67959f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/inject-files-b411369ce6856dac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/inspect-to-clean-b3616d843775c187.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/inspection-409-69d5bd6c2a49d2ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/inspection-to-report-disk-by-path-e3fd4c331d200903.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/inspection-wait-for-ips-223e39b65fef31bd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/inspection-wait-for-ips-v2-146016f758d7010c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/inspector-logs-9b7c010c219691d2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/inspector-retry-502-2b286e2ccc64c195.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/instance-info-root-device-02fed0966bb00fb3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/inventory-conf-29b59ebe97aefbde.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/ip6-addresses-1c2b9bcd9a124de7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/ipa-debug-68c86101b1fdc3d9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/ipmi-address-channel-b6b8010c41d05c1b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/ipmi-cleanup-a4454f6851d81c4d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/ipv6-listen-85d40e58156e398f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/ipv6-provision-42e9000f6f6a7a3a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/ironic-error-97e76d9ddacff039.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/iscsi-detection-on-diskless-hw-f27dcce3aaa35ac2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/jitter-for-inspection-command-5a226927757a0308.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/let_crypt_generate_the_salt-99876591325275a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/lib-exc-41ee122eb4a04bc4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/limit-qemu-img-malloc-arena-025ed84115481eae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/limit-qemu-img-ram-usage-d7b7a16ac5e9c917.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/lldp-error-handling-5b6576b378ef9c3a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/lldp-loop-fdfa584caf33d847.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/lldp-raw-a09174cb930bca97.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/log-download-size-57982fa8df336520.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/log-file-7aaaf31693ddc617.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/logs-collector-non-ascii-010339bf256443c8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/lsblk-all-956c1df808a169bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/lshw-cb89894be057bdc9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/lshw-for-memory-and-system-info-35c69da067c72b36.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/lshw-no-memory-bank-size-05ea71987362986e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/manual-introspection-b04b5c25f5e004ac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/manually-configure-ironic-api-version-517afd0a423036ad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/md-restart-9e0d47863a086792.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/mdadm-d5b8c186182620b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/mdns-e020484e64d76edb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/min-ironic-ocata-dff80e567783e87c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/mlnx-steps-now-available-for-deploy-4a4226ffaae888f3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/move_swraid_to_efibootmgr-d87c1bfde1661fb5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/multipath-handling-00a5b412d2cf2e4e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/multipath-serial-615fc925984abbf7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1243 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/multipath_error_handling_improvement-1669d0de4bfdbe95.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/multiple-lan-channels-ee32d80150f990bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/name-root-device-hints-0cfc8c90d03c8bf0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/net-speed-8854901e2051bb79.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/new-agent-api-afbe7391493749be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/new-sync-command-6f5fa55df2fd5903.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/no-bash-for-grub-c38369af8cc7cf26.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/no-coreos-3345cc69009dead9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/no-iscsi-fd21808edbea5ac2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/no-link-local-2e861978c5c7bf30.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/no-mac-54616606ee6b844d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/no-netboot-d034bb1d1d9166c5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/no-sample-ac11bd0fa27af62a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/no-standalone-bb34eae2cc468837.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/no-zram-78cc6583f4f90a9c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/old-inspector-data-5e63c9bce72b4fb5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/oslo-config-generator-b0f70b9fb7e23997.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/parallel-erase-disk-devices-09ea33d5443aead0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/partition_check_read_only_base_device-5bc15ac2f034aca9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/permit-pre-hashed-rescue-passwords-4275f6e697533cec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/pint-0.5-816aaf3a4f6d4a6e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/poll-mode-063bd36b2b18bffb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/prefix-lldp-timeout-50acc656313d8dd2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/prepare-image-49744276cef719d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/preserve-efi-folder-contents-ea1e278b3093ec55.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1151 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/prevent-deletion-of-shared-disk-filesystems-4c17c7666d2fe3bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/prevent-needless-iscsi-cleanup-f8d602c0abc7e8ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/prioritize-lsblk-device-serials-8cae406ca5164a01.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/qemu-img-ooo-write-721b8a0057ab7b8a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/qemu-write-zeros-2edbf3152c57e2b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/raid-esp-size-2c322adb2d3b9ce7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/raid-hints-604f9ffdd86432eb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/raid5-6-support-0807597c3633a26c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/readd_missing_devs-2ed85805388b6e42.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/rebuild_on_esp_raid-33f359bdf5ccaa09.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/relax-checksum-feeding-11044ae02b411a07.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/remove-lldp-timeout-ea481dbb01a39522.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/remove-switch_port_descr-switch_chassis_descr-40f2bb37b5f1fdd1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/remove-sysrq-2c2804930180f408.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/remove-vendor-passthru-eda3519c322eb4e2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/rescan-before-checking-uefi-64597c937880134d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/rescan-device-after-mkfs-3f9d52a2e3b6fff3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/rescue-dhcp_network-for-tinyipa-a14de5fae38a5dce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/respect-listen-directives-94fb863c5b692c07.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      473 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/rework-ata-secure-erase-c6684962ef078281.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/root-device-hints-rotational-67e6e61074c26561.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/set-clock-prior-to-poweroff-af6ec210aad8b45a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/several-urls-9c3b8c14338b06ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/skip-lookup-and-heartbeat-if-apiurl-not-configured-5ae8b04ae1e74673.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/skips-bootloader-install-35c463195aa61800.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/sleep-ebe58fbe07d30219.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/softraid-bootable-with-uefi-aa22e6cbaf1ea747.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/softraid-creation-on-nvme-a2fd4c531d200904.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/softraid-partitioning-refactor-104b817c3bdc73e3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/softraid-zap-superblocks-anywhere.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/software-raid-4a88e6c5af9ea742.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/software-raid-raid-ESPs-25a2aa117b99620a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/software-raid-use-label-as-rootfs-uuid-d9a3827180f1a238.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/software_raid_use_rootfs_uuid-9149cc0c8638d5d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/start_passing_agent_version_to_ironic-6fa8670ae0e7eb38.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      567 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/stream-raw-images-d2e245aaed991d86.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/streaming-partition-images-cdeb260ef8f90012.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/streaming-uuid-fdf136a7745fbb3d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1083 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/support-bootloader-csv-file-use-c815b520c600cd98.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/support-collecting-ipv6-address-dd819d543f851a63.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/support-image-proxy-e2987a6589375451.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/support-linux-io-6bbd7ff1f0d70a0e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/support-lldp-in-inventory-4ab6e45ccd35dace.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/support-prep-partitions-5e273572ab7ce018.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/suse-tinyipa-support-20acecd6d7b20952.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/sw-raid-assemble-9c20fe967f73d1dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/timeout_on_file_download-ed77918318316075.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/tinycore-ipv6-1b620c61402b5720.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/tinyipa-python3-default-b8434793e17465db.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/tinyipa-rescue-dhcp-multi-tenant-b32bda7bf2b12679.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/tinyipa-ssh-e8a3a01a3f3ff5f4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/udev-settle-f75db34db990ad68.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/udevadm-settle-9d3e5f1f20211857.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/uefi-esp-660fc2c650e6af92.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/uefi-fallback-266c647f6aff58fd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/uefi-images-38c8536db189ffc1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/understand-node-conflict-is-locked-2ea21dd45abfe4f7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/up-qemuimg-mem-1536183a02b3a235.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/use-latest-coreos-87f826d26b46548d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/use-system-random-00b0721c8ebd0c5a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/vmedia-copy-6a58f3183b166c42.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/wait-for-interfaces-before-lookup-9bf38852b2f176a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/wait-root-device-504b517c3aec73e2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/whole-disk-grub-0b1b8b9c44e31d28.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/notes/zero-size-78d3be2ac8fd59c2.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.577787 ironic-python-agent-9.9.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/2023.2.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.577787 ironic-python-agent-9.9.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.577787 ironic-python-agent-9.9.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9279 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/liberty.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2614 2024-02-01 10:59:12.581787 ironic-python-agent-9.9.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      716 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.577787 ironic-python-agent-9.9.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8385 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/tools/bandit.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.577787 ironic-python-agent-9.9.0/tools/config/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1015 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/tools/config/check_uptodate.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/tools/config/ipa-config-generator.conf
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1233 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/tools/run_bashate.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/tools/with_venv.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4649 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-01 10:59:12.581787 ironic-python-agent-9.9.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5328 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/zuul.d/ironic-python-agent-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1582 2024-02-01 10:58:20.000000 ironic-python-agent-9.9.0/zuul.d/project.yaml
```

### Comparing `ironic-python-agent-9.8.0/AUTHORS` & `ironic-python-agent-9.9.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -99,18 +99,20 @@
 Luong Anh Tuan <tuanla@vn.fujitsu.com>
 Madhuri Kumari <madhuri.kumari@intel.com>
 Madhuri Kumari <madhuri.rai07@gmail.com>
 Mario Villaplana <mario.villaplana@gmail.com>
 Mark Goddard <mark@stackhpc.com>
 Markos Chandras <mchandras@suse.de>
 Martin André <m.andre@redhat.com>
+Maryna Savchenko <maryna.savchenko@cern.ch>
 Mateusz Kowalski <mateusz.kowalski@cern.ch>
 Mathieu Mitchell <mmitchell@iweb.com>
 Matthew Thode <mthode@mthode.org>
 Michael Turek <mjturek@linux.vnet.ibm.com>
+Michal Nasiadka <mnasiadka@gmail.com>
 Mike Heald <mike.heald@hp.com>
 Mike Turek <mjturek@linux.vnet.ibm.com>
 Miles Gould <mgould@redhat.com>
 Mohammed Naser <mnaser@vexxhost.com>
 Moshe Levi <moshele@mellanox.com>
 Nam Nguyen Hoai <namnh@vn.fujitsu.com>
 Naohiro Tamura <naohirot@jp.fujitsu.com>
@@ -142,20 +144,22 @@
 Ruby Loo <ruby.loo@intel.com>
 Russell Haering <russell.haering@rackspace.com>
 Russell Haering <russellhaering@gmail.com>
 Sam Betts <sam@code-smash.net>
 Sean McGinnis <sean.mcginnis@gmail.com>
 Sergey Vilgelm <sergey@vilgelm.info>
 ShangXiao <shangxiaobj@inspur.com>
+Sharpz7 <adam.mcarthur62@gmail.com>
 Shivanand Tendulker <stendulker@gmail.com>
 Shuquan Huang <huang.shuquan@99cloud.net>
 Steve Baker <sbaker@redhat.com>
 Swapnil Kulkarni (coolsvap) <me@coolsvap.net>
 Szymon Borkowski <szymon.borkowski@intel.com>
 Szymon Wroblewski <szymon.wroblewski@intel.com>
+Takashi Kajinami <kajinamit@oss.nttdata.com>
 Tao Li <litao3721@126.com>
 Tom Cocozzello <tjcocozz@us.ibm.com>
 Tony Breeds <tony@bakeyournoodle.com>
 Uros Orozel <uros.orozel@gmail.com>
 Vanou Ishii <ishii.vanou@fujitsu.com>
 Vasyl Saienko <vsaienko@mirantis.com>
 Vladimir Kozhukalov <vkozhukalov@mirantis.com>
```

### Comparing `ironic-python-agent-9.8.0/CONTRIBUTING.rst` & `ironic-python-agent-9.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ChangeLog` & `ironic-python-agent-9.9.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,40 @@
 CHANGES
 =======
 
+9.9.0
+-----
+
+* Also retry inspection on HTTP CONFLICT
+* [codespell] Adding git-blame-ignore-revs to clear codespell changes
+* Add support for reporting CPU socket number
+* [Codespell] Adding tox target to CI (Non-Voting)
+* Update python classifier in setup.cfg
+* Support several API and Inspector URLs
+* Add missing headers to the inspection callback
+* Update to latest pep8/code style versions
+* Add tox target and configuration for codespell
+* [codespell] Fix spelling issues in IPA
+* Remove deprecated pbr options
+* Remove unnecessary egg\_info options
+* Fix inspector retries to not take a long time
+* Reformat and update the section on injecting root credentials
+* Add a jitter to heartbeat retries
+* Retry in ProxyError during post inspector data
+* Revert "Fix vmedia network config drive handling"
+* Fix referencing to the raid\_device var which is not set
+* Parse efibootmgr type and details
+
 9.8.0
 -----
 
 * Handle different device outputs for multipath
+* docs: improve rootpwd password generation command
 * fix multipathd error handling release notes
+* Fix vmedia network config drive handling
 * Test coverage for efi\_utils.get\_boot\_record
 * Remove standby.cache\_image support
 * Get numa\_node info when collecting pci devices info
 * improve multipathd error handling
 * Replace shlex module with helper function
 * Retry on checksum failures
 * implement basic-auth support for user-image download process
```

### Comparing `ironic-python-agent-9.8.0/LICENSE` & `ironic-python-agent-9.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/PKG-INFO` & `ironic-python-agent-9.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ironic-python-agent
-Version: 9.8.0
+Version: 9.9.0
 Summary: Ironic Python Agent Ramdisk
 Home-page: https://docs.openstack.org/ironic-python-agent/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache-2
 Description: ===================
         Ironic Python Agent
@@ -79,10 +79,11 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Provides-Extra: burnin_network_kazoo
 Provides-Extra: test
```

### Comparing `ironic-python-agent-9.8.0/README.rst` & `ironic-python-agent-9.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/bindep.txt` & `ironic-python-agent-9.9.0/bindep.txt`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/doc/source/admin/hardware_managers.rst` & `ironic-python-agent-9.9.0/doc/source/admin/hardware_managers.rst`

 * *Files 0% similar despite different names*

```diff
@@ -143,28 +143,28 @@
     way of writing an image.
 ``deploy.inject_files(node, ports, files, verify_ca=True)``
     A step to inject files into a system. Specifically this step is documented
     earlier in this documentation.
 
 .. NOTE::
    The Ironic Developers chose to limit the items available for service steps
-   such that the risk of data distruction is generally minimized.
+   such that the risk of data destruction is generally minimized.
    That being said, it could be reasonable to reconfigure RAID devices through
    local hardware managers *or* to write the base OS image as part of a
    service operation. As such, caution should be taken, and if additional data
    erasure steps are needed you may want to consider moving a node through
    cleaning to remove the workload. Otherwise, if you have a use case, please
    feel free to reach out to the Ironic Developers so we can understand and
    enable your use case.
 
 Cleaning safeguards
 -------------------
 
 The stock hardware manager contains a number of safeguards to prevent
-unsafe conditions from occuring.
+unsafe conditions from occurring.
 
 Devices Skip List
 ~~~~~~~~~~~~~~~~~
 
 A list of devices that Ironic does not touch during the cleaning and deployment
 process can be specified in the node properties field under
 ``skip_block_devices``. This should be a list of dictionaries
```

### Comparing `ironic-python-agent-9.8.0/doc/source/admin/how_it_works.rst` & `ironic-python-agent-9.9.0/doc/source/admin/how_it_works.rst`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 The exact format of the inventory depends on the hardware manager used.
 Here is the basic format expected to be provided by all hardware managers.
 The inventory is a dictionary (JSON object), containing at least the following
 fields:
 
 ``cpu``
     CPU information: ``model_name``, ``frequency``, ``count``,
-    ``architecture`` and ``flags``.
+    ``architecture``, ``flags`` and ``socket_count``.
 
 ``memory``
     RAM information: ``total`` (total size in bytes), ``physical_mb``
     (physically installed memory size in MiB, optional).
 
     .. note::
         The difference is that the latter includes the memory region reserved
@@ -241,15 +241,15 @@
 For the purposes of Ironic, we continue to support the pass-through checksum
 field as we support the checksum being retrieved via a URL.
 
 We also support determining the checksum by length.
 
 The field can be utilized to designate:
 
-* A URL to retreive a checksum from.
+* A URL to retrieve a checksum from.
 * MD5 (Disabled by default, see ``[DEFAULT]md5_enabled`` in the agent
   configuration file.)
 * SHA-2 based SHA256
 * SHA-2 based SHA512
 
 SHA-3 based checksums are not supported for auto-determination as they can
 have a variable length checksum result. At of when this documentation was
```

### Comparing `ironic-python-agent-9.8.0/doc/source/admin/rescue.rst` & `ironic-python-agent-9.9.0/doc/source/admin/rescue.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/doc/source/admin/troubleshooting.rst` & `ironic-python-agent-9.9.0/doc/source/admin/troubleshooting.rst`

 * *Files 2% similar despite different names*

```diff
@@ -60,34 +60,57 @@
 Installed SSH server is configured to disable Password authentication.
 
 Access via console
 ------------------
 If you need to use console access, passwords must be enabled there are a
 couple ways to enable this depending on how the IPA image was created:
 
-ironic-python-agent-builder
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
+ironic-python-agent-builder: dynamic-login
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Users wishing to use password access can be add the dynamic-login [0]_ or the
 devuser element [1]_
 
 The dynamic-login element allows the operator to change the root password
 dynamically when the image boots. Kernel command line parameters
 are used to do this.
 
-dynamic-login element example::
+Generate a password hash with following command:
 
-  Generate a ENCRYPTED_PASSWORD with the openssl passwd -1 command
-  Add rootpwd="$ENCRYPTED_PASSWORD" value on the kernel_append_params setting in /etc/ironic/ironic.conf
-  Restart the ironic-conductor with the command service ironic-conductor restart
+.. code-block:: console
 
-Users can also be added to DIB built IPA images with the devuser element [1]_
+    $ openssl passwd -1 -stdin | sed 's/\$/\$\$/g'
 
-Install ``ironic-python-agent-builder`` following the guide [2]_
+Add ``rootpwd="<openssl output>"`` value on the ``kernel_append_params``
+setting in the Ironic configuration file (``/etc/ironic/ironic.conf``).
+Restart the ironic-conductor e.g. with
 
-Example::
+.. code-block:: console
+
+   $ sudo systemctl restart ironic-conductor
+
+Alternatively, you can use the contents of the SSH public key.
+
+.. warning::
+
+   * The ``sed`` command is used to escape the ``$`` symbols in the
+     configuration file.
+
+   * The quotation marks around the value are mandatory.
+
+   * Only 1 password or 1 SSH key is supported.
+
+ironic-python-agent-builder: devuser
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Users can also be added to DIB built IPA images with the devuser element [1]_.
+Install ``ironic-python-agent-builder`` following the guide [2]_.
+
+Example:
+
+.. code-block:: bash
 
   export DIB_DEV_USER_USERNAME=username
   export DIB_DEV_USER_PWDLESS_SUDO=yes
   export DIB_DEV_USER_PASSWORD=PASSWORD
   ironic-python-agent-builder -o /path/to/custom-ipa -e devuser debian
 
 tinyipa
@@ -162,15 +185,16 @@
   sudo systemctl restart ironic-python-agent.service
 
 Cleaning halted with ProtectedDeviceError
 =========================================
 
 The IPA service has halted cleaning as one of the block devices within or
 attached to the bare metal node contains a class of filesystem which **MAY**
-cause irreparable harm to a potentially running cluster if accidently removed.
+cause irreparable harm to a potentially running cluster if accidentally
+removed.
 
 These filesystems *may* be used for only local storage and as a result be
 safe to erase. However if a shared block device is in use, such as a device
 supplied via a Storage Area Network utilizing protocols such as iSCSI or
 FibreChannel. Ultimately the Host Bus Adapter (HBA) may not be an entirely
 "detectable" entity given the hardware market place and aspects such as
 "SmartNICs" and Converged Network Adapters with specific offload functions
```

### Comparing `ironic-python-agent-9.8.0/doc/source/conf.py` & `ironic-python-agent-9.9.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/doc/source/contributor/hardware_managers.rst` & `ironic-python-agent-9.9.0/doc/source/contributor/hardware_managers.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/doc/source/contributor/index.rst` & `ironic-python-agent-9.9.0/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/doc/source/contributor/metrics.rst` & `ironic-python-agent-9.9.0/doc/source/contributor/metrics.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/doc/source/contributor/rescue.rst` & `ironic-python-agent-9.9.0/doc/source/contributor/rescue.rst`

 * *Files 0% similar despite different names*

```diff
@@ -35,13 +35,13 @@
      "command_status": "SUCCEEDED"
      "command_result": null
      "command_error": null
     }
 
 If successful, this synchronous command will:
 
-1. Write the salted and crypted ``rescue_password`` to
+1. Write the salted and encrypted ``rescue_password`` to
    ``/etc/ipa-rescue-config/ipa-rescue-password`` in the chroot or filesystem
    that ironic-python-agent is running in.
 
 2. Stop the ironic-python-agent process after completing these actions and
    returning the response to the API request.
```

### Comparing `ironic-python-agent-9.8.0/doc/source/index.rst` & `ironic-python-agent-9.9.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/doc/source/install/index.rst` & `ironic-python-agent-9.9.0/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/examples/README.rst` & `ironic-python-agent-9.9.0/examples/README.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/examples/business-logic/example_business_logic.py` & `ironic-python-agent-9.9.0/examples/business-logic/example_business_logic.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/examples/business-logic/setup.cfg` & `ironic-python-agent-9.9.0/examples/business-logic/setup.cfg`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/examples/custom-disk-erase/example_disk_eraser.py` & `ironic-python-agent-9.9.0/examples/custom-disk-erase/example_disk_eraser.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/examples/custom-disk-erase/setup.cfg` & `ironic-python-agent-9.9.0/examples/custom-disk-erase/setup.cfg`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/examples/vendor-device/example_device.py` & `ironic-python-agent-9.9.0/examples/vendor-device/example_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 LOG = log.getLogger()
 
 
 # All the helper methods should be kept outside of the HardwareManager
 # so they'll never get accidentally called by dispatch_to_managers()
 def _initialize_hardware():
-    """Example method for initalizing hardware."""
+    """Example method for initializing hardware."""
     # Perform any operations here that are required to initialize your
     # hardware.
     LOG.debug('Loading drivers, settling udevs, and generally initalizing')
     pass
 
 
 def _detect_hardware():
@@ -60,15 +60,15 @@
     HARDWARE_MANAGER_NAME = 'ExampleDeviceHardwareManager'
     HARDWARE_MANAGER_VERSION = '1'
 
     def evaluate_hardware_support(self):
         """Declare level of hardware support provided.
 
         Since this example covers a case of supporting a specific device,
-        this method is where you would do anything needed to initalize that
+        this method is where you would do anything needed to initialize that
         device, including loading drivers, and then detect if one exists.
 
         In some cases, if you expect the hardware to be available on any node
         running this hardware manager, or it's undetectable, you may want to
         return a static value here.
 
         Be aware all managers' loaded in IPA will run this method before IPA
```

### Comparing `ironic-python-agent-9.8.0/examples/vendor-device/setup.cfg` & `ironic-python-agent-9.9.0/examples/vendor-device/setup.cfg`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/__init__.py` & `ironic-python-agent-9.9.0/ironic_python_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/agent.py` & `ironic-python-agent-9.9.0/ironic_python_agent/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,22 +64,32 @@
     serializable_fields = ('started_at', 'version')
 
     def __init__(self, started_at, version):
         self.started_at = started_at
         self.version = version
 
 
+def _with_jitter(value, min_multiplier, max_multiplier):
+    interval_multiplier = random.uniform(min_multiplier, max_multiplier)
+    return value * interval_multiplier
+
+
 class IronicPythonAgentHeartbeater(threading.Thread):
     """Thread that periodically heartbeats to Ironic."""
 
-    # If we could wait at most N seconds between heartbeats (or in case of an
-    # error) we will instead wait r x N seconds, where r is a random value
-    # between these multipliers.
+    # If we could wait at most N seconds between heartbeats, we will instead
+    # wait r x N seconds, where r is a random value between these multipliers.
     min_jitter_multiplier = 0.3
     max_jitter_multiplier = 0.6
+    # Error retry between 5 and 10 seconds, at least 12 retries with
+    # the default ramdisk_heartbeat_timeout of 300 and the worst case interval
+    # jitter of 0.6.
+    min_heartbeat_interval = 5
+    min_error_jitter_multiplier = 1.0
+    max_error_jitter_multiplier = 2.0
 
     def __init__(self, agent):
         """Initialize the heartbeat thread.
 
         :param agent: an :class:`ironic_python_agent.agent.IronicPythonAgent`
                       instance.
         """
@@ -93,93 +103,136 @@
 
     def run(self):
         """Start the heartbeat thread."""
         # The first heartbeat happens immediately
         LOG.info('Starting heartbeater')
         self.agent.set_agent_advertise_addr()
 
-        while not self.stop_event.wait(min(self.interval, 5)):
-            if self._heartbeat_expected():
-                self.do_heartbeat()
+        while self._run_next():
             eventlet.sleep(0)
 
+    def _run_next(self):
+        # The logic here makes sure we don't wait exactly 5 seconds more or
+        # less regardless of the current interval since it may cause a
+        # thundering herd problem when a lot of agents are heartbeating.
+        # Essentially, if the next heartbeat is due in 2 seconds, don't wait 5.
+        # But if the next one is scheduled in 2 minutes, do wait 5 to account
+        # for forced heartbeats.
+        wait = min(
+            self.min_heartbeat_interval,
+            # This operation checks how much of the initially planned interval
+            # we have still left. Compare with 0 in case we overshoot the goal.
+            max(0, self.interval - (_time() - self.previous_heartbeat)),
+        )
+        if self.stop_event.wait(wait):
+            return False  # done
+
+        if self._heartbeat_expected():
+            self.do_heartbeat()
+
+        return True
+
     def _heartbeat_expected(self):
+        elapsed = _time() - self.previous_heartbeat
+
         # Normal heartbeating
-        if _time() > self.previous_heartbeat + self.interval:
+        if elapsed >= self.interval:
             return True
 
         # Forced heartbeating, but once in 5 seconds
-        if (self.heartbeat_forced
-                and _time() > self.previous_heartbeat + 5):
+        if self.heartbeat_forced and elapsed > self.min_heartbeat_interval:
             return True
 
     def do_heartbeat(self):
         """Send a heartbeat to Ironic."""
         try:
             self.api.heartbeat(
                 uuid=self.agent.get_node_uuid(),
                 advertise_address=self.agent.advertise_address,
                 advertise_protocol=self.agent.advertise_protocol,
                 generated_cert=self.agent.generated_cert,
             )
-            LOG.info('heartbeat successful')
+        except Exception as exc:
+            if isinstance(exc, errors.HeartbeatConflictError):
+                LOG.warning('conflict error sending heartbeat to %s',
+                            self.agent.api_urls)
+            else:
+                LOG.exception('error sending heartbeat to %s',
+                              self.agent.api_urls)
+            self.interval = _with_jitter(self.min_heartbeat_interval,
+                                         self.min_error_jitter_multiplier,
+                                         self.max_error_jitter_multiplier)
+        else:
+            LOG.debug('heartbeat successful')
             self.heartbeat_forced = False
-            self.previous_heartbeat = _time()
-        except errors.HeartbeatConflictError:
-            LOG.warning('conflict error sending heartbeat to %s',
-                        self.agent.api_url)
-        except Exception:
-            LOG.exception('error sending heartbeat to %s', self.agent.api_url)
-        finally:
-            interval_multiplier = random.uniform(self.min_jitter_multiplier,
-                                                 self.max_jitter_multiplier)
-            self.interval = self.agent.heartbeat_timeout * interval_multiplier
-            LOG.info('sleeping before next heartbeat, interval: %s',
-                     self.interval)
+            self.interval = _with_jitter(self.agent.heartbeat_timeout,
+                                         self.min_jitter_multiplier,
+                                         self.max_jitter_multiplier)
+        self.previous_heartbeat = _time()
+        LOG.info('sleeping before next heartbeat, interval: %s', self.interval)
 
     def force_heartbeat(self):
         self.heartbeat_forced = True
 
     def stop(self):
         """Stop the heartbeat thread."""
         LOG.info('stopping heartbeater')
         self.stop_event.set()
         return self.join()
 
 
 class IronicPythonAgent(base.ExecuteCommandMixin):
     """Class for base agent functionality."""
 
+    @classmethod
+    def from_config(cls, conf):
+        return cls(conf.api_url,
+                   Host(hostname=conf.advertise_host,
+                        port=conf.advertise_port),
+                   Host(hostname=conf.listen_host,
+                        port=conf.listen_port),
+                   conf.ip_lookup_attempts,
+                   conf.ip_lookup_sleep,
+                   conf.network_interface,
+                   conf.lookup_timeout,
+                   conf.lookup_interval,
+                   False,
+                   conf.agent_token,
+                   conf.hardware_initialization_delay,
+                   conf.advertise_protocol)
+
     def __init__(self, api_url, advertise_address, listen_address,
                  ip_lookup_attempts, ip_lookup_sleep, network_interface,
                  lookup_timeout, lookup_interval, standalone, agent_token,
                  hardware_initialization_delay=0, advertise_protocol='http'):
         super(IronicPythonAgent, self).__init__()
         if bool(cfg.CONF.keyfile) != bool(cfg.CONF.certfile):
             LOG.warning("Only one of 'keyfile' and 'certfile' options is "
                         "defined in config file. Its value will be ignored.")
         self.ext_mgr = base.init_ext_manager(self)
-        self.api_url = api_url
-        if (not self.api_url or self.api_url == 'mdns') and not standalone:
+        if (not api_url or api_url == 'mdns') and not standalone:
             try:
-                self.api_url, params = mdns.get_endpoint('baremetal')
+                api_url, params = mdns.get_endpoint('baremetal')
             except lib_exc.ServiceLookupFailure:
-                if self.api_url:
+                if api_url:
                     # mDNS explicitly requested, report failure.
                     raise
                 else:
                     # implicit fallback to mDNS, do not fail (maybe we're only
                     # running inspection).
                     LOG.warning('Could not get baremetal endpoint from mDNS, '
                                 'will not heartbeat')
             else:
                 config.override(params)
-
-        if self.api_url:
-            self.api_client = ironic_api_client.APIClient(self.api_url)
+        if api_url:
+            self.api_urls = list(filter(None, api_url.split(',')))
+        else:
+            self.api_urls = None
+        if self.api_urls:
+            self.api_client = ironic_api_client.APIClient(self.api_urls)
             self.heartbeater = IronicPythonAgentHeartbeater(self)
         self.listen_address = listen_address
         self.advertise_address = advertise_address
         self.advertise_protocol = advertise_protocol
         self.version = pkg_resources.get_distribution('ironic-python-agent')\
             .version
         self.api = app.Application(self, cfg.CONF)
@@ -255,14 +308,33 @@
         except ValueError as exc:
             LOG.warning('Invalid IP address %(addr)s returned as a route '
                         'to host %(dest)s: %(err)s',
                         {'dest': dest, 'addr': source, 'err': exc})
 
         return source
 
+    def _find_routable_addr(self):
+        ips = []
+        for api_url in self.api_urls:
+            ironic_host = urlparse.urlparse(api_url).hostname
+            # Try resolving it in case it's not an IP address
+            try:
+                ironic_host = socket.gethostbyname(ironic_host)
+            except socket.gaierror:
+                LOG.debug('Could not resolve %s, maybe no DNS', ironic_host)
+            ips.append(ironic_host)
+
+        for attempt in range(self.ip_lookup_attempts):
+            for ironic_host in ips:
+                found_ip = self._get_route_source(ironic_host)
+                if found_ip:
+                    return found_ip
+
+            time.sleep(self.ip_lookup_sleep)
+
     def set_agent_advertise_addr(self):
         """Set advertised IP address for the agent, if not already set.
 
         If agent's advertised IP address is still default (None), try to
         find a better one.  If the agent's network interface is None, replace
         that as well.
 
@@ -273,28 +345,15 @@
 
         found_ip = None
         if self.network_interface is not None:
             # TODO(dtantsur): deprecate this
             found_ip = hardware.dispatch_to_managers('get_ipv4_addr',
                                                      self.network_interface)
         else:
-            url = urlparse.urlparse(self.api_url)
-            ironic_host = url.hostname
-            # Try resolving it in case it's not an IP address
-            try:
-                ironic_host = socket.gethostbyname(ironic_host)
-            except socket.gaierror:
-                LOG.debug('Count not resolve %s, maybe no DNS', ironic_host)
-
-            for attempt in range(self.ip_lookup_attempts):
-                found_ip = self._get_route_source(ironic_host)
-                if found_ip:
-                    break
-
-                time.sleep(self.ip_lookup_sleep)
+            found_ip = self._find_routable_addr()
 
         if found_ip:
             self.advertise_address = Host(hostname=found_ip,
                                           port=self.advertise_address.port)
         else:
             raise errors.LookupAgentIPError('Agent could not find a valid IP '
                                             'address.')
@@ -359,15 +418,15 @@
     def _start_auto_tls(self):
         # NOTE(dtantsur): if listen_tls is True, assume static TLS
         # configuration and don't auto-generate anything.
         if cfg.CONF.listen_tls or not cfg.CONF.enable_auto_tls:
             LOG.debug('Automated TLS is disabled')
             return None, None
 
-        if not self.api_url or not self.api_client.supports_auto_tls():
+        if not self.api_urls or not self.api_client.supports_auto_tls():
             LOG.warning('Ironic does not support automated TLS')
             return None, None
 
         self.set_agent_advertise_addr()
 
         LOG.info('Generating TLS parameters automatically for IP %s',
                  self.advertise_address.hostname)
@@ -377,15 +436,15 @@
         self.advertise_protocol = 'https'
         return tls_info.path, tls_info.private_key_path
 
     def serve_ipa_api(self):
         """Serve the API until an extension terminates it."""
         cert_file, key_file = self._start_auto_tls()
         self.api.start(cert_file, key_file)
-        if not self.standalone and self.api_url:
+        if not self.standalone and self.api_urls:
             # Don't start heartbeating until the server is listening
             self.heartbeater.start()
         try:
             while self.serve_api:
                 eventlet.sleep(0.1)
         except KeyboardInterrupt:
             LOG.info('Caught keyboard interrupt, exiting')
@@ -471,15 +530,15 @@
                 try:
                     # Attempt inspection. This may fail, and previously
                     # an error would be logged.
                     uuid = inspector.inspect()
                 except errors.InspectionError as e:
                     LOG.error('Failed to perform inspection: %s', e)
 
-            if self.api_url:
+            if self.api_urls:
                 content = self.api_client.lookup_node(
                     hardware_info=hardware.list_hardware_info(use_cache=True),
                     timeout=self.lookup_timeout,
                     starting_interval=self.lookup_interval,
                     node_uuid=uuid)
                 LOG.debug('Received lookup results: %s', content)
                 self.process_lookup_data(content)
@@ -496,9 +555,9 @@
                 # able to be driven solely from the conductor, this is no
                 # longer a major issue.
                 LOG.error('Neither ipa-api-url nor inspection_callback_url'
                           'found, please check your pxe append parameters.')
 
         self.serve_ipa_api()
 
-        if not self.standalone and self.api_url:
+        if not self.standalone and self.api_urls:
             self.heartbeater.stop()
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/api/app.py` & `ironic-python-agent-9.9.0/ironic_python_agent/api/app.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/burnin.py` & `ironic-python-agent-9.9.0/ironic_python_agent/burnin.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/cmd/agent.py` & `ironic-python-agent-9.9.0/ironic_python_agent/cmd/agent.py`

 * *Files 23% similar despite different names*

```diff
@@ -43,21 +43,8 @@
     # Used for TLS configuration
     sslutils.register_opts(CONF)
 
     logger = log.getLogger(__name__)
     logger.debug("Configuration:")
     CONF.log_opt_values(logger, log.DEBUG)
     utils.log_early_log_to_logger()
-    agent.IronicPythonAgent(CONF.api_url,
-                            agent.Host(hostname=CONF.advertise_host,
-                                       port=CONF.advertise_port),
-                            agent.Host(hostname=CONF.listen_host,
-                                       port=CONF.listen_port),
-                            CONF.ip_lookup_attempts,
-                            CONF.ip_lookup_sleep,
-                            CONF.network_interface,
-                            CONF.lookup_timeout,
-                            CONF.lookup_interval,
-                            False,
-                            CONF.agent_token,
-                            CONF.hardware_initialization_delay,
-                            CONF.advertise_protocol).run()
+    agent.IronicPythonAgent.from_config(CONF).run()
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/cmd/inspect.py` & `ironic-python-agent-9.9.0/ironic_python_agent/cmd/inspect.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/config.py` & `ironic-python-agent-9.9.0/ironic_python_agent/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,19 +26,21 @@
 INSPECTION_DEFAULT_COLLECTOR = 'default,logs'
 INSPECTION_DEFAULT_DHCP_WAIT_TIMEOUT = 60
 
 cli_opts = [
     cfg.StrOpt('api_url',
                default=APARAMS.get('ipa-api-url'),
                regex='^(mdns|http(s?):\\/\\/.+)',
-               help='URL of the Ironic API. '
+               help='URL(s) of the Ironic API. '
                     'Can be supplied as "ipa-api-url" kernel parameter.'
-                    'The value must start with either http:// or https://. '
+                    'The value(s) must start with either http:// or https://. '
                     'A special value "mdns" can be specified to fetch the '
-                    'URL using multicast DNS service discovery.'),
+                    'URL using multicast DNS service discovery. If several '
+                    'URLs are provided, all of them are tried until one '
+                    'does not return a connection error.'),
 
     cfg.StrOpt('global_request_id',
                default=APARAMS.get('ipa-global-request-id'),
                help='Global request ID header to provide to Ironic API. '
                     'Can be supplied as "ipa-global-request-id" kernel '
                     'parameter. The value must be in form "req-<UUID>".'),
 
@@ -151,17 +153,16 @@
                      'Can be supplied as "ipa-collect-lldp" '
                      'kernel parameter.',
                 deprecated_for_removal=True,
                 deprecated_reason="Use the lldp collector instead"),
 
     cfg.StrOpt('inspection_callback_url',
                default=APARAMS.get('ipa-inspection-callback-url'),
-               help='Endpoint of ironic-inspector. If set, hardware inventory '
-                    'will be collected and sent to ironic-inspector '
-                    'on start up. '
+               help='Endpoint(s) to send inspection data to. If set, hardware '
+                    'inventory will be collected and sent there on start up. '
                     'A special value "mdns" can be specified to fetch the '
                     'URL using multicast DNS service discovery. '
                     'Can be supplied as "ipa-inspection-callback-url" '
                     'kernel parameter.'),
 
     cfg.StrOpt('inspection_collectors',
                default=APARAMS.get('ipa-inspection-collectors',
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/dmi_inspector.py` & `ironic-python-agent-9.9.0/ironic_python_agent/dmi_inspector.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/efi_utils.py` & `ironic-python-agent-9.9.0/ironic_python_agent/efi_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,34 +263,37 @@
                 # question is which is right/first/preferred.
                 return [v_bl]
     return valid_bootloaders
 
 
 # NOTE(TheJulia): regex used to identify entries in the efibootmgr
 # output on stdout.
-_ENTRY_LABEL = re.compile(r'Boot([0-9a-f-A-F]+)\*?\s(.*).*$')
+_ENTRY_LABEL = re.compile(
+    r'Boot([0-9a-f-A-F]+)\*?\s+(.*?)\s+'
+    r'((BBS|HD|FvFile|FvVol|PciRoot|VenMsg|VenHw|UsbClass)\(.*)$')
 
 
 def get_boot_records():
     """Executes efibootmgr and returns boot records.
 
-    :return: an iterator yielding pairs (boot number, boot record).
+    :return: An iterator yielding tuples
+             (boot number, boot record, root device type, device path).
     """
     # Invokes binary=True so we get a bytestream back.
     efi_output = utils.execute('efibootmgr', '-v', binary=True)
     # Bytes must be decoded before regex can be run and
     # matching to work as intended.
     # Also ignore errors on decoding, as we can basically get
     # garbage out of the nvram record, this way we don't fail
     # hard on unrelated records.
     cmd_output = efi_output[0].decode('utf-16', errors='ignore')
     for line in cmd_output.split('\n'):
         match = _ENTRY_LABEL.match(line)
         if match is not None:
-            yield (match[1], match[2])
+            yield (match[1], match[2], match[4], match[3])
 
 
 def add_boot_record(device, efi_partition, loader, label):
     """Add an EFI boot record with efibootmgr.
 
     :param device: the device to be used
     :param efi_partition: the number of the EFI partition on the device
@@ -354,19 +357,19 @@
         else:
             v_efi_bl_path = '\\' + v_bl.replace('/', '\\')
             label = 'ironic' + str(label_id)
             if label_suffix:
                 label = label + " " + str(label_suffix)
 
         # Iterate through standard out, and look for duplicates
-        for boot_num, boot_rec in boot_records:
+        for boot_num, boot_rec, boot_type, boot_details in boot_records:
             # Look for the base label in the string if a line match
             # occurs, so we can identify if we need to eliminate the
             # entry.
-            if label in boot_rec:
+            if label == boot_rec:
                 LOG.debug("Found bootnum %s matching label", boot_num)
                 remove_boot_record(boot_num)
 
         LOG.info("Adding loader %(path)s on partition %(part)s of device "
                  " %(dev)s with label %(label)s",
                  {'path': v_efi_bl_path, 'part': efi_partition,
                   'dev': device, 'label': label})
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/encoding.py` & `ironic-python-agent-9.9.0/ironic_python_agent/encoding.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/errors.py` & `ironic-python-agent-9.9.0/ironic_python_agent/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
 class ClockSyncError(RESTError):
     """Error raised when attempting to sync the system clock."""
 
     message = 'Error syncing system clock'
 
 
 class HeartbeatConnectionError(IronicAPIError):
-    """Transitory connection failure occured attempting to contact the API."""
+    """Transitory connection failure occurred attempting to contact the API."""
 
     message = ("Error attempting to heartbeat - Possible transitory network "
                "failure or blocking port may be present.")
 
     def __init__(self, details):
         super(HeartbeatConnectionError, self).__init__(details)
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/extensions/base.py` & `ironic-python-agent-9.9.0/ironic_python_agent/extensions/base.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/extensions/clean.py` & `ironic-python-agent-9.9.0/ironic_python_agent/extensions/clean.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/extensions/deploy.py` & `ironic-python-agent-9.9.0/ironic_python_agent/extensions/deploy.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/extensions/flow.py` & `ironic-python-agent-9.9.0/ironic_python_agent/extensions/flow.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/extensions/image.py` & `ironic-python-agent-9.9.0/ironic_python_agent/extensions/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
                    'path': path})
         try:
             utils.execute('mount', partition, path)
         except processutils.ProcessExecutionError as e:
             # NOTE(TheJulia): It seems in some cases,
             # the python os.path.ismount can return False
             # even *if* it is actually mounted. This appears
-            # to be becasue it tries to rely on inode on device
+            # to be because it tries to rely on inode on device
             # logic, yet the rules are sometimes different inside
             # ramdisks. So lets check the error first.
             if 'already mounted' not in e:
                 # Raise the error, since this is not a known
                 # failure case
                 raise
             else:
@@ -432,38 +432,37 @@
 
 def _try_preserve_efi_assets(device, path,
                              efi_system_part_uuid,
                              efi_partition,
                              efi_partition_mount_point):
     """Attempt to preserve UEFI boot assets.
 
-    :param device: The device upon which wich to try to preserve
-                   assets.
+    :param device: The device upon which to try to preserve assets.
     :param path: The path in which the filesystem is already mounted
                  which we should examine to preserve assets from.
     :param efi_system_part_uuid: The partition ID representing the
                                  created EFI system partition.
-    :param efi_partition: The partitions upon wich to write the preserved
+    :param efi_partition: The partitions upon which to write the preserved
                           assets to.
     :param efi_partition_mount_point: The folder at which to mount
                                       the assets for the process of
                                       preservation.
 
     :returns: True if assets have been preserved, otherwise False.
               None is the result of this method if a failure has
-              occured.
+              occurred.
     """
     efi_assets_folder = efi_partition_mount_point + '/EFI'
     if os.path.exists(efi_assets_folder):
         # We appear to have EFI Assets, that need to be preserved
         # and as such if we succeed preserving them, we will be returned
         # True from _preserve_efi_assets to correspond with success or
         # failure in this action.
         # NOTE(TheJulia): Still makes sense to invoke grub-install as
-        # fragmentation of grub has occured.
+        # fragmentation of grub has occurred.
         if (os.path.exists(os.path.join(path, 'usr/sbin/grub2-install'))
             or os.path.exists(os.path.join(path, 'usr/sbin/grub-install'))):
             _configure_grub(device, path)
         # But first, if we have grub, we should try to build a grub config!
         LOG.debug('EFI asset folder detected, attempting to preserve assets.')
         if _preserve_efi_assets(path, efi_assets_folder,
                                 efi_partition,
@@ -588,15 +587,15 @@
                          efi_partition_mount_point):
     """Preserve the EFI assets in a partition image.
 
     :param path: The path used for the mounted image filesystem.
     :param efi_assets_folder: The folder where we can find the
                               UEFI assets required for booting.
     :param efi_partition: The partition upon which to write the
-                          perserved assets to.
+                          preserved assets to.
     :param efi_partition_mount_point: The folder at which to mount
                                       the assets for the process of
                                       preservation.
     :returns: True if EFI assets were able to be located and preserved
               to their appropriate locations based upon the supplied
               efi_partition.
               False if any error is encountered in this process.
@@ -625,15 +624,15 @@
                     except (IOError, OSError, shutil.SameFileError) as e:
                         LOG.warning('Failed to copy grub.cfg file for '
                                     'EFI boot operation. Error %s', e)
         grub2_env_file = os.path.join(path, 'boot/grub2/grubenv')
         # NOTE(TheJulia): By saving the default, this file should be created.
         # this appears to what diskimage-builder does.
         # if the file is just a file, then we'll need to copy it. If it is
-        # anything else like a link, we're good. This behaivor is inconsistent
+        # anything else like a link, we're good. This behavior is inconsistent
         # depending on packager install scripts for grub.
         if os.path.isfile(grub2_env_file):
             LOG.debug('Detected grub environment file %s, will attempt '
                       'to copy this file to align with apparent bootloaders',
                       grub2_env_file)
             for dest in destlist:
                 grub2env_dest = os.path.join(save_efi, dest, 'grubenv')
@@ -681,15 +680,15 @@
         :param efi_system_part_uuid: The UUID of the efi system partition.
             To be used only for uefi boot mode.  For uefi boot mode, the
             boot loader will be installed here.
         :param prep_boot_part_uuid: The UUID of the PReP Boot partition.
             Used only for booting ppc64* partition images locally. In this
             scenario the bootloader will be installed here.
         :param target_boot_mode: bios, uefi. Only taken into account
-            for softraid, when no efi partition is explicitely provided
+            for softraid, when no efi partition is explicitly provided
             (happens for whole disk images)
         :raises: CommandExecutionError if the installation of the
                  bootloader fails.
         :raises: DeviceNotFound if the root partition is not found.
 
         """
         device = hardware.dispatch_to_managers('get_os_install_device')
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/extensions/log.py` & `ironic-python-agent-9.9.0/ironic_python_agent/extensions/log.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/extensions/poll.py` & `ironic-python-agent-9.9.0/ironic_python_agent/extensions/poll.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/extensions/rescue.py` & `ironic-python-agent-9.9.0/ironic_python_agent/extensions/rescue.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/extensions/service.py` & `ironic-python-agent-9.9.0/ironic_python_agent/extensions/service.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/extensions/standby.py` & `ironic-python-agent-9.9.0/ironic_python_agent/extensions/standby.py`

 * *Files 0% similar despite different names*

```diff
@@ -411,15 +411,15 @@
 
 
 def _get_algorithm_by_length(checksum):
     """Determine the SHA-2 algorithm by checksum length.
 
     :param checksum: The requested checksum.
     :returns: A hashlib object based upon the checksum
-              or ValueError if the algorthm could not be
+              or ValueError if the algorithm could not be
               identified.
     """
     # NOTE(TheJulia): This is all based on SHA-2 lengths.
     # SHA-3 would require a hint, thus ValueError because
     # it may not be a fixed length. That said, SHA-2 is not
     # as of this not being added, being withdrawn standards wise.
     checksum_len = len(checksum)
@@ -458,15 +458,15 @@
     and create an iterator so the image can be downloaded in chunks. The
     MD5 hash of the image being downloaded is calculated on-the-fly.
     """
 
     def __init__(self, image_info, time_obj=None):
         """Initialize an instance of the ImageDownload class.
 
-        Trys each URL in image_info successively until a URL returns a
+        Tries each URL in image_info successively until a URL returns a
         successful request code. Once the object is initialized, the user may
         retrieve chunks of the image through the standard python iterator
         interface until either the image is fully downloaded, or an error is
         encountered.
 
         :param image_info: Image information dictionary.
         :param time_obj: Optional time object to indicate when the image
@@ -496,25 +496,25 @@
             # Treat checksum urls as first class request citizens, else
             # fallback to legacy handling.
             self._expected_hash_value = _fetch_checksum(
                 checksum,
                 image_info)
             retrieved_checksum = True
             if not algo:
-                # Override algorithm not suppied as os_hash_algo
+                # Override algorithm not supplied as os_hash_algo
                 self._hash_algo = _get_algorithm_by_length(
                     self._expected_hash_value)
         elif checksum:
             # Fallback to md5 path.
             try:
                 new_algo = _get_algorithm_by_length(checksum)
 
                 if not new_algo:
                     # Realistically, this should never happen, but for
-                    # compatability...
+                    # compatibility...
                     # TODO(TheJulia): Remove for a 2024 release.
                     self._hash_algo = hashlib.new('md5')  # nosec
                 else:
                     self._hash_algo = new_algo
             except ValueError as e:
                 message = ('Unable to proceed with image {} as the '
                            'checksum indicator has been used but the '
@@ -672,15 +672,15 @@
                 time.sleep(CONF.image_download_connection_retry_interval)
         else:
             break
 
     totaltime = time.time() - starttime
     LOG.info("Image downloaded from %(image_location)s "
              "in %(totaltime)s seconds. Transferred %(size)s bytes. "
-             "Server originaly reported: %(reported)s.",
+             "Server originally reported: %(reported)s.",
              {'image_location': image_location,
               'totaltime': totaltime,
               'size': image_download.bytes_transferred,
               'reported': image_download.content_length})
 
 
 def _validate_image_info(ext, image_info=None, **kwargs):
@@ -702,15 +702,15 @@
     os_hash_checksum_avail = False
 
     for field in ['id', 'urls']:
         if field not in image_info:
             msg = 'Image is missing \'{}\' field.'.format(field)
             raise errors.InvalidCommandParamsError(msg)
 
-    if type(image_info['urls']) != list or not image_info['urls']:
+    if not isinstance(image_info['urls'], list) or not image_info['urls']:
         raise errors.InvalidCommandParamsError(
             'Image \'urls\' must be a list with at least one element.')
 
     checksum = image_info.get('checksum')
     if checksum is not None:
         if (not isinstance(image_info['checksum'], str)
                 or not image_info['checksum']):
@@ -850,15 +850,15 @@
                                  'error': e})
                     time.sleep(CONF.image_download_connection_retry_interval)
             else:
                 break
 
         totaltime = time.time() - starttime
         LOG.info("Image streamed onto device %(device)s in %(totaltime)s "
-                 "seconds for %(size)s bytes. Server originaly reported "
+                 "seconds for %(size)s bytes. Server originally reported "
                  "%(reported)s.",
                  {'device': device, 'totaltime': totaltime,
                   'size': image_download.bytes_transferred,
                   'reported': image_download.content_length})
         # Fix any gpt partition
         try:
             disk_utils.fix_gpt_partition(device, node_uuid=None)
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/hardware.py` & `ironic-python-agent-9.9.0/ironic_python_agent/hardware.py`

 * *Files 1% similar despite different names*

```diff
@@ -699,25 +699,25 @@
                                    uuid=device_raw['uuid'],
                                    partuuid=device_raw['partuuid'],
                                    **extra))
     return devices
 
 
 def save_api_client(client=None, timeout=None, interval=None):
-    """Preserves access to the API client for potential later re-use."""
+    """Preserves access to the API client for potential later reuse."""
     global API_CLIENT, API_LOOKUP_TIMEOUT, API_LOOKUP_INTERVAL
 
     if client and timeout and interval and not API_CLIENT:
         API_CLIENT = client
         API_LOOKUP_TIMEOUT = timeout
         API_LOOKUP_INTERVAL = interval
 
 
 def update_cached_node():
-    """Attmepts to update the node cache via the API"""
+    """Attempts to update the node cache via the API"""
     cached_node = get_cached_node()
     if API_CLIENT:
         LOG.info('Agent is requesting to perform an explicit node cache '
                  'update. This is to pickup any changes in the cache '
                  'before deployment.')
         try:
             if cached_node is None:
@@ -804,21 +804,22 @@
         # client identifier Option to allow DHCP to work over InfiniBand.
         # see https://tools.ietf.org/html/rfc4390
         self.client_id = client_id
 
 
 class CPU(encoding.SerializableComparable):
     serializable_fields = ('model_name', 'frequency', 'count', 'architecture',
-                           'flags')
+                           'flags', 'socket_count')
 
     def __init__(self, model_name, frequency, count, architecture,
-                 flags=None):
+                 flags=None, socket_count=None):
         self.model_name = model_name
         self.frequency = frequency
         self.count = count
+        self.socket_count = socket_count
         self.architecture = architecture
         self.flags = flags or []
 
 
 class Memory(encoding.SerializableComparable):
     serializable_fields = ('total', 'physical_mb')
     # physical = total + kernel binary + reserved space
@@ -1161,15 +1162,15 @@
 
         Returns a list of steps. Each step is represented by a dict::
 
           {
            'interface': the name of the driver interface that should execute
                         the step.
            'step': the HardwareManager function to call.
-           'priority': the order steps will be run in if excuted upon
+           'priority': the order steps will be run in if executed upon
                        similar to automated cleaning or deployment.
                        In service steps, the order comes from the user request,
                        but this similarity is kept for consistency should we
                        further extend the capability at some point in the
                        future.
            'reboot_requested': Whether the agent should request Ironic reboots
                                the node via the power driver after the
@@ -1492,15 +1493,16 @@
             LOG.warning('Failed to get CPU flags')
 
         return CPU(model_name=cpu_info.get('model name'),
                    frequency=freq,
                    # this includes hyperthreading cores
                    count=int(cpu_info.get('cpu(s)')),
                    architecture=cpu_info.get('architecture'),
-                   flags=flags)
+                   flags=flags,
+                   socket_count=int(cpu_info.get('socket(s)', 0)))
 
     def get_memory(self):
         # psutil returns a long, so we force it to an int
         try:
             total = int(psutil.virtual_memory().total)
         except Exception:
             # This is explicitly catching all exceptions. We want to catch any
@@ -2292,15 +2294,15 @@
         raise errors.IncompatibleHardwareMethodError()
 
     def get_bmc_v6address(self):
         """Attempt to detect BMC v6 address
 
         :return: IPv6 address of lan channel or ::/0 in case none of them is
                  configured properly. May return None value if it cannot
-                 interract with system tools or critical error occurs.
+                 interact with system tools or critical error occurs.
         """
         null_address_re = re.compile(r'^::(/\d{1,3})*$')
 
         def get_addr(channel, dynamic=False):
             cmd = "ipmitool lan6 print {} {}_addr".format(
                 channel, 'dynamic' if dynamic else 'static')
             try:
@@ -2309,17 +2311,17 @@
                 return
 
             # NOTE: More likely ipmitool was not intended to return
             #       stdout in yaml format. Fortunately, output of
             #       dynamic_addr and static_addr commands is a valid yaml.
             try:
                 out = yaml.safe_load(out.strip())
-            except yaml.YAMLError as excpt:
+            except yaml.YAMLError as ex:
                 LOG.warning('Cannot process output of "%(cmd)s" '
-                            'command: %(e)s', {'cmd': cmd, 'e': excpt})
+                            'command: %(e)s', {'cmd': cmd, 'e': ex})
                 return
 
             for addr_dict in out.values():
                 address = addr_dict['Address']
                 if dynamic:
                     enabled = addr_dict['Source/Type'] in ['DHCPv6', 'SLAAC']
                 else:
@@ -2494,16 +2496,16 @@
             {
                 'step': 'burnin_cpu',
                 'priority': 0,
                 'interface': 'deploy',
                 'reboot_requested': False,
                 'abortable': True
             },
-            # NOTE(TheJulia): Burnin disk is explicilty not carried in this
-            # list because it would be distructive to data on a disk.
+            # NOTE(TheJulia): Burnin disk is explicitly not carried in this
+            # list because it would be destructive to data on a disk.
             # If someone needs to do that, the machine should be
             # unprovisioned.
             {
                 'step': 'burnin_memory',
                 'priority': 0,
                 'interface': 'deploy',
                 'reboot_requested': False,
@@ -2922,15 +2924,15 @@
                                 {'name': blk.name, 'err': e})
                     continue
             try:
                 il_utils.execute('mdadm', '--zero-superblock', blk.name)
             except processutils.ProcessExecutionError as e:
                 LOG.warning('Failed to remove superblock from'
                             '%(device)s: %(err)s',
-                            {'device': raid_device.name, 'err': e})
+                            {'device': blk.name, 'err': e})
 
         # Erase all partition tables we created
         all_holder_disks_uniq = list(
             collections.OrderedDict.fromkeys(all_holder_disks))
         for holder_disk in all_holder_disks_uniq:
             if holder_disk in do_not_delete_disks:
                 # Remove just partitions not listed in keep_partitions
@@ -3416,24 +3418,24 @@
     # tests endlessly.
     return MULTIPATH_ENABLED
 
 
 def safety_check_block_device(node, device):
     """Performs safety checking of a block device before destroying.
 
-    In order to guard against distruction of file systems such as
+    In order to guard against destruction of file systems such as
     shared-disk file systems
     (https://en.wikipedia.org/wiki/Clustered_file_system#SHARED-DISK)
     or similar filesystems where multiple distinct computers may have
     unlocked concurrent IO access to the entire block device or
     SAN Logical Unit Number, we need to evaluate, and block cleaning
-    from occuring on these filesystems *unless* we have been explicitly
+    from occurring on these filesystems *unless* we have been explicitly
     configured to do so.
 
-    This is because cleaning is an intentionally distructive operation,
+    This is because cleaning is an intentionally destructive operation,
     and once started against such a device, given the complexities of
     shared disk clustered filesystems where concurrent access is a design
     element, in all likelihood the entire cluster can be negatively
     impacted, and an operator will be forced to recover from snapshot and
     or backups of the volume's contents.
 
     :param node: A node, or cached node object.
@@ -3483,15 +3485,15 @@
         identified_ids,
         identified_fs_types)
 
 
 def _check_for_special_partitions_filesystems(device, ids, fs_types):
     """Compare supplied IDs, Types to known items, and raise if found.
 
-    :param device: The block device in use, specificially for logging.
+    :param device: The block device in use, specifically for logging.
     :param ids: A list above IDs found to check.
     :param fs_types: A list of FS types found to check.
     :raises: ProtectedDeviceError should a partition label or metadata
              be discovered which suggests a shared disk clustered filesystem
              has been discovered.
     """
     guarded_ids = {
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/hardware_managers/cna.py` & `ironic-python-agent-9.9.0/ironic_python_agent/hardware_managers/cna.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/hardware_managers/mlnx.py` & `ironic-python-agent-9.9.0/ironic_python_agent/hardware_managers/mlnx.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/hardware_managers/nvidia/nvidia_fw_update.py` & `ironic-python-agent-9.9.0/ironic_python_agent/hardware_managers/nvidia/nvidia_fw_update.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/inject_files.py` & `ironic-python-agent-9.9.0/ironic_python_agent/inject_files.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/inspect.py` & `ironic-python-agent-9.9.0/ironic_python_agent/inspect.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                                   'endpoint: %(err)s',
                                   {'err': e})
                         exception_encountered = True
                         interval = min(interval * self.backoff_factor,
                                        self.max_delay)
                     except Exception as e:
                         # General failure such as requests ConnectionError
-                        LOG.error('Error occured attempting to connect to '
+                        LOG.error('Error occurred attempting to connect to '
                                   'connect to the introspection service. '
                                   'Error: %(err)s',
                                   {'err': e})
                         exception_encountered = True
                         interval = min(interval * self.backoff_factor,
                                        self.max_delay)
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/inspector.py` & `ironic-python-agent-9.9.0/ironic_python_agent/inspector.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
 # implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from http import client as http_client
 import json
 import os
 import time
 
 from ironic_lib import mdns
 from oslo_concurrency import processutils
 from oslo_config import cfg
@@ -113,40 +114,67 @@
                                      'returned an error')
 
     LOG.info('inspection finished successfully')
     return resp.get('uuid')
 
 
 _RETRY_WAIT = 5
+_RETRY_WAIT_MAX = 30
 _RETRY_ATTEMPTS = 5
 
 
 def call_inspector(data, failures):
     """Post data to inspector."""
     data['error'] = failures.get_error()
 
-    LOG.info('posting collected data to %s', CONF.inspection_callback_url)
     LOG.debug('collected data: %s',
               {k: v for k, v in data.items() if k not in _NO_LOGGING_FIELDS})
 
     encoder = encoding.RESTJSONEncoder()
     data = encoder.encode(data)
     verify, cert = utils.get_ssl_client_options(CONF)
 
+    headers = {
+        'Content-Type': 'application/json',
+        'Accept': 'application/json',
+    }
+    if CONF.global_request_id:
+        headers["X-OpenStack-Request-ID"] = CONF.global_request_id
+
+    urls = list(filter(None, CONF.inspection_callback_url.split(',')))
+
     @tenacity.retry(
         retry=tenacity.retry_if_exception_type(
-            requests.exceptions.ConnectionError),
+            (requests.exceptions.ConnectionError,
+             requests.exceptions.HTTPError)),
         stop=tenacity.stop_after_attempt(_RETRY_ATTEMPTS),
-        wait=tenacity.wait_fixed(_RETRY_WAIT),
+        wait=tenacity.wait_exponential(multiplier=1.5,
+                                       min=_RETRY_WAIT, max=_RETRY_WAIT_MAX),
         reraise=True)
     def _post_to_inspector():
-        return requests.post(
-            CONF.inspection_callback_url, data=data,
-            verify=verify, cert=cert,
-            timeout=CONF.http_request_timeout)
+        for url in urls:
+            LOG.info('Posting collected data to %s', url)
+            try:
+                inspector_resp = requests.post(
+                    url, data=data, headers=headers,
+                    verify=verify, cert=cert,
+                    timeout=CONF.http_request_timeout)
+            except requests.exceptions.ConnectionError as exc:
+                if url == urls[-1]:
+                    raise
+                LOG.warning("Connection error when accessing %s, trying the "
+                            "next URL. Error: %s", url, exc)
+            else:
+                break
+
+        if (inspector_resp.status_code >= 500
+                or inspector_resp.status_code == http_client.CONFLICT):
+            raise requests.exceptions.HTTPError(response=inspector_resp)
+
+        return inspector_resp
 
     resp = _post_to_inspector()
     if resp.status_code >= 400:
         LOG.error('inspector %s error %d: %s, proceeding with lookup',
                   CONF.inspection_callback_url,
                   resp.status_code, resp.content.decode('utf-8'))
         return
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/ironic_api_client.py` & `ironic-python-agent-9.9.0/ironic_python_agent/ironic_api_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,59 +35,80 @@
 AGENT_VERSION_IRONIC_VERSION = (1, 36)
 AGENT_TOKEN_IRONIC_VERSION = (1, 62)
 AGENT_VERIFY_CA_IRONIC_VERSION = (1, 68)
 # NOTE(dtantsur): change this constant every time you add support for more
 # versions to ensure that we send the highest version we know about.
 MAX_KNOWN_VERSION = AGENT_VERIFY_CA_IRONIC_VERSION
 
+CONNECT_EXCEPTIONS = (requests.exceptions.Timeout,
+                      requests.exceptions.ConnectTimeout,
+                      requests.exceptions.ConnectionError,
+                      requests.exceptions.ReadTimeout,
+                      requests.exceptions.HTTPError)
+
 
 class APIClient(object):
     api_version = 'v1'
     lookup_api = '/%s/lookup' % api_version
     heartbeat_api = '/%s/heartbeat/{uuid}' % api_version
     _ironic_api_version = None
     agent_token = None
     lookup_lock_pause = 0
 
-    def __init__(self, api_url):
-        self.api_url = api_url.rstrip('/')
+    def __init__(self, api_urls):
+        if isinstance(api_urls, str):
+            api_urls = [api_urls]
+        self.api_urls = [url.rstrip('/') for url in api_urls]
 
         # Only keep alive a maximum of 2 connections to the API. More will be
         # opened if they are needed, but they will be closed immediately after
         # use.
         adapter = requests.adapters.HTTPAdapter(pool_connections=2,
                                                 pool_maxsize=2)
         self.session = requests.Session()
-        self.session.mount(self.api_url, adapter)
+        self.session.mount('https://', adapter)
+        self.session.mount('http://', adapter)
 
         self.encoder = encoding.RESTJSONEncoder()
 
     def _request(self, method, path, data=None, headers=None, **kwargs):
-        request_url = '{api_url}{path}'.format(api_url=self.api_url, path=path)
 
         if data is not None:
             data = self.encoder.encode(data)
 
         headers = headers or {}
         headers.update({
             'Content-Type': 'application/json',
             'Accept': 'application/json',
         })
         if CONF.global_request_id:
             headers["X-OpenStack-Request-ID"] = CONF.global_request_id
 
         verify, cert = utils.get_ssl_client_options(CONF)
-        return self.session.request(method,
-                                    request_url,
-                                    headers=headers,
-                                    data=data,
-                                    verify=verify,
-                                    cert=cert,
-                                    timeout=CONF.http_request_timeout,
-                                    **kwargs)
+        for idx, api_url in enumerate(self.api_urls):
+            request_url = f'{api_url}{path}'
+            try:
+                resp = self.session.request(method,
+                                            request_url,
+                                            headers=headers,
+                                            data=data,
+                                            verify=verify,
+                                            cert=cert,
+                                            timeout=CONF.http_request_timeout,
+                                            **kwargs)
+                # Make sure the working URL is on the top, so that the next
+                # time we start from it. Also allows us to log self.api_urls[0]
+                # as the currently used URL.
+                self.api_urls = self.api_urls[idx:] + self.api_urls[:idx]
+                return resp
+            except CONNECT_EXCEPTIONS as exc:
+                if idx == len(self.api_urls) - 1:
+                    raise
+                LOG.warning("Connection error when accessing %s, trying the "
+                            "next URL. Error: %s", request_url, exc)
 
     def _get_ironic_api_version_header(self, version=None):
         if version is None:
             ironic_version = self._get_ironic_api_version()
             version = min(ironic_version, AGENT_TOKEN_IRONIC_VERSION)
         return {'X-OpenStack-Ironic-API-Version': '%d.%d' % version}
 
@@ -200,53 +221,50 @@
                                   for iface in hardware_info['interfaces']
                                   if iface.mac_address)
         }
         if node_uuid:
             params['node_uuid'] = node_uuid
 
         LOG.debug('Looking up node with addresses %r and UUID %s at %s',
-                  params['addresses'], node_uuid, self.api_url)
+                  params['addresses'], node_uuid, self.api_urls)
 
         try:
             response = self._request(
                 'GET', self.lookup_api,
                 headers=self._get_ironic_api_version_header(),
                 params=params)
-        except (requests.exceptions.Timeout,
-                requests.exceptions.ConnectTimeout,
-                requests.exceptions.ConnectionError,
-                requests.exceptions.ReadTimeout,
-                requests.exceptions.HTTPError) as err:
+        except CONNECT_EXCEPTIONS as err:
+            # Report the last URL, there are warnings for the rest already
             LOG.warning(
                 'Error detected while attempting to perform lookup '
-                'with %s, retrying. Error: %s', self.api_url, err
+                'with %s, retrying. Error: %s', self.api_urls[-1], err
             )
             return False
         except Exception as err:
             # NOTE(TheJulia): If you're looking here, and you're wondering
             # why the retry logic is not working or your investigating a weird
             # error or even IPA just exiting,
             # See https://storyboard.openstack.org/#!/story/2007968
             # To be clear, we're going to try to provide as much detail as
             # possible in the exit handling
             msg = ('Unhandled error looking up node with addresses {} at '
-                   '{}: {}'.format(params['addresses'], self.api_url, err))
+                   '{}: {}'.format(params['addresses'], self.api_urls, err))
             # No matter what we do at this point, IPA is going to exit.
-            # This is because we don't know why the exception occured and
+            # This is because we don't know why the exception occurred and
             # we likely should not try to retry as such.
             # We will attempt to provide as much detail to the logs as
-            # possible as to what occured, although depending on the logging
+            # possible as to what occurred, although depending on the logging
             # subsystem, additional errors can occur, thus the additional
             # handling below.
             try:
                 LOG.exception(msg)
                 return False
             except Exception as exc_err:
                 LOG.error(msg)
-                exc_msg = ('Unexpected exception occured while trying to '
+                exc_msg = ('Unexpected exception occurred while trying to '
                            'log additional detail. Error: {}'.format(exc_err))
                 LOG.error(exc_msg)
                 raise errors.LookupNodeError(msg)
 
         if response.status_code == requests.codes.CONFLICT:
             if self.lookup_lock_pause == 0:
                 self.lookup_lock_pause = 5
@@ -268,15 +286,15 @@
             time.sleep(self.lookup_lock_pause)
             return False
 
         if response.status_code != requests.codes.OK:
             LOG.warning(
                 'Failed looking up node with addresses %r at %s. '
                 'Check if inspection has completed? %s',
-                params['addresses'], self.api_url,
+                params['addresses'], self.api_urls[0],
                 self._error_from_response(response)
             )
             return False
 
         try:
             content = json.loads(response.content)
         except json.decoder.JSONDecodeError as e:
@@ -284,15 +302,15 @@
             return False
 
         # Check for valid response data
         if 'node' not in content or 'uuid' not in content['node']:
             LOG.warning(
                 'Got invalid node data in response to query for node '
                 'with addresses %r from %s: %s',
-                params['addresses'], self.api_url, content,
+                params['addresses'], self.api_urls[0], content,
             )
             return False
 
         if 'config' not in content:
             # Old API
             try:
                 content['config'] = {'heartbeat_timeout':
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/netutils.py` & `ironic-python-agent-9.9.0/ironic_python_agent/netutils.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/numa_inspector.py` & `ironic-python-agent-9.9.0/ironic_python_agent/numa_inspector.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/partition_utils.py` & `ironic-python-agent-9.9.0/ironic_python_agent/partition_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -558,15 +558,15 @@
         shutil.copytree(conf_drive_temp, new_drive_temp, dirs_exist_ok=True)
     except (processutils.ProcessExecutionError, OSError) as e:
         # We failed to make the filesystem :(
         # This is a fairly hard error as we could not use the
         # config drive, nor could we recover the state.
         LOG.error('We were unable to make a new filesystem for the '
                   'configuration drive. Error: %s', e)
-        msg = ('A failure occured while attempting to format, copy, and '
+        msg = ('A failure occurred while attempting to format, copy, and '
                're-create the configuration drive in a structure which '
                'is compatible with the underlying hardware and Operating '
                'System. Due to the nature of configuration drive, it could '
                'have been incorrectly formatted. Operator investigation is '
                'required. Error: {}'.format(str(e)))
         raise exception.InstanceDeployFailure(msg)
     finally:
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/raid_utils.py` & `ironic-python-agent-9.9.0/ironic_python_agent/raid_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
 
 def calc_raid_partition_sectors(psize, start):
     """Calculates end sector and converts start and end sectors including
 
     the unit of measure, compatible with parted.
     :param psize: size of the raid partition
-    :param start: start sector of the raid partion in integer format
+    :param start: start sector of the raid partition in integer format
     :return: start and end sector in parted compatible format, end sector
         as integer
     """
 
     if isinstance(start, int):
         start_str = '%dGiB' % start
     else:
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/functional/base.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/functional/test_commands.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/functional/test_commands.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/base.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/base.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/dmi_inspector_data.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/dmi_inspector_data.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/test_base.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/test_base.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/test_clean.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/test_clean.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/test_deploy.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/test_deploy.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/test_flow.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/test_flow.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/test_image.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/test_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -385,15 +385,15 @@
             self.fake_dev, hardware.BootInfo(current_boot_mode='uefi')
         ]
         mock_get_part_path.return_value = self.fake_efi_system_part
         mock_utils_efi_part.return_value = {'number': '1'}
         mock_efi_bl.return_value = ['EFI/BOOT/BOOTX64.EFI']
         # NOTE(TheJulia): This test string was derived from a lenovo SR650
         # which does do some weird things with additional entries.
-        # most notabley
+        # most notably
         stdout_msg = """
 BootCurrent: 0000
 Timeout: 1 seconds
 BootOrder: 0000,0003,0002,0001
 Boot0000* ironic1       HD(1,GPT,55db8d03-c8f6-4a5b-9155-790dddc348fa,0x800,0x64000)/File(\EFI\boot\shimx64.efi)
 Boot0001* CD/DVD Rom    VenHw(1fad3248-0000-7950-2166-a1e506fdb83a,02000000)..GO
 Boot0002* Hard Disk     VenHw(1fad3248-0000-7950-2166-a1e506fdb83a,01000000)..GO..NO..........V.U.E.F.I.:. . . .S.C.S.I. .H.a.r.d. .D.r.i.v.e........A....................................*..............@.........U..[J.Uy...H.......BO
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/test_log.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/test_log.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/test_poll.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/test_poll.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/test_rescue.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/test_rescue.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/test_service.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/test_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,12 +289,12 @@
             {'GenericHardwareManager': 1}, {'GenericHardwareManager': 2})
 
         async_result = self.agent_extension.execute_service_step(
             step=self.step['GenericHardwareManager'][0], node=self.node,
             ports=self.ports, service_version=self.version)
         async_result.join()
         # NOTE(TheJulia): This remains CLEAN_VERSION_MISMATCH for backwards
-        # compatability with base.py and API consumers.
+        # compatibility with base.py and API consumers.
         self.assertEqual('CLEAN_VERSION_MISMATCH',
                          async_result.command_status)
 
         mock_version.assert_called_once_with(self.version)
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/extensions/test_standby.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/extensions/test_standby.py`

 * *Files 0% similar despite different names*

```diff
@@ -519,15 +519,15 @@
             mock.call.debug('Verifying image at %(image_location)s against '
                             '%(algo_name)s checksum %(checksum)s',
                             {'image_location': mock.ANY,
                              'algo_name': mock.ANY,
                              'checksum': 'fake-checksum'}),
             mock.call.info('Image downloaded from %(image_location)s in '
                            '%(totaltime)s seconds. Transferred %(size)s '
-                           'bytes. Server originaly reported: %(reported)s.',
+                           'bytes. Server originally reported: %(reported)s.',
                            {'image_location': mock.ANY,
                             'totaltime': mock.ANY,
                             'size': 11,
                             'reported': None}),
         ]
         log_mock.assert_has_calls(log_mock_calls)
 
@@ -1397,15 +1397,15 @@
             mock.call.debug('Verifying image at %(image_location)s '
                             'against %(algo_name)s checksum %(checksum)s',
                             {'image_location': '/dev/foo',
                              'algo_name': mock.ANY,
                              'checksum': 'fake-checksum'}),
             mock.call.info('Image streamed onto device %(device)s in '
                            '%(totaltime)s seconds for %(size)s bytes. '
-                           'Server originaly reported %(reported)s.',
+                           'Server originally reported %(reported)s.',
                            {'device': '/dev/foo',
                             'totaltime': mock.ANY,
                             'size': 11,
                             'reported': 11}),
             mock.call.info('%(device)s UUID is now %(root_uuid)s',
                            {'device': '/dev/foo', 'root_uuid': 'aaaabbbb'})
         ]
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/hardware_managers/nvidia/test_nvidia_fw_update.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/hardware_managers/nvidia/test_nvidia_fw_update.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/hardware_managers/test_cna.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/hardware_managers/test_cna.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/hardware_managers/test_mlnx.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/hardware_managers/test_mlnx.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/samples/hardware_samples.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/samples/hardware_samples.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 """
 
 # NOTE(TheJulia): This list intentionally contains duplicates
 # as the code filters them out by kernel device name.
 # NOTE(dszumski): We include some partitions here to verify that
 # they are filtered out when not requested. It is assumed that
 # ROTA has been set to 0 on some software RAID devices for testing
-# purposes. In practice is appears to inherit from the underyling
+# purposes. In practice is appears to inherit from the underlying
 # devices, so in this example it would normally be 1.
 RAID_BLK_DEVICE_TEMPLATE = ("""
 {
     "blockdevices": [
       {"kname":"sda", "model":"DRIVE 0", "size":1765517033472, "rota":true,
       "type":"disk", "serial":"sda123", "uuid":null, "partuuid":null},
       {"kname":"sda1", "model":"DRIVE 0", "size":107373133824, "rota":true,
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_agent.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,97 +46,125 @@
         return 'command execution succeeded'
 
 
 class FakeExtension(base.BaseAgentExtension):
     pass
 
 
+class FakeClock:
+    current = 0
+    last_wait = None
+    wait_result = False
+
+    def get(self):
+        return self.current
+
+    def wait(self, interval):
+        self.last_wait = interval
+        self.current += interval
+        return self.wait_result
+
+
 class TestHeartbeater(ironic_agent_base.IronicAgentTest):
     def setUp(self):
         super(TestHeartbeater, self).setUp()
         self.mock_agent = mock.Mock()
         self.mock_agent.api_url = 'https://fake_api.example.org:8081/'
         self.heartbeater = agent.IronicPythonAgentHeartbeater(self.mock_agent)
         self.heartbeater.api = mock.Mock()
         self.heartbeater.hardware = mock.create_autospec(
             hardware.HardwareManager)
         self.heartbeater.stop_event = mock.Mock()
 
     @mock.patch('ironic_python_agent.agent._time', autospec=True)
     @mock.patch('random.uniform', autospec=True)
     def test_heartbeat(self, mock_uniform, mock_time):
-        time_responses = []
-        uniform_responses = []
-        heartbeat_responses = []
-        wait_responses = []
-        expected_stop_calls = []
-
-        # FIRST RUN:
-        # initial delay is 0
-        expected_stop_calls.append(mock.call(0))
-        wait_responses.append(False)
-        # next heartbeat due at t=100
-        heartbeat_responses.append(100)
-        # random interval multiplier is 0.5
-        uniform_responses.append(0.5)
-        # time is now 50
-        time_responses.append(50)
-
-        # SECOND RUN:
-        expected_stop_calls.append(mock.call(5))
-        wait_responses.append(False)
-        # next heartbeat due at t=180
-        heartbeat_responses.append(180)
-        # random interval multiplier is 0.4
-        uniform_responses.append(0.4)
-        # time is now 80
-        time_responses.append(80)
-        # add one response for _time in _heartbeat_expected
-        time_responses.append(80)
-
-        # THIRD RUN:
-        expected_stop_calls.append(mock.call(5))
-        wait_responses.append(False)
-        # this heartbeat attempt fails
-        heartbeat_responses.append(Exception('uh oh!'))
-        # random interval multiplier is 0.5
-        uniform_responses.append(0.5)
-        # we check the time to generate a fake deadline, now t=125
-        time_responses.append(125)
-        # time is now 125.5
-        time_responses.append(125.5)
-
-        # FOURTH RUN:
-        expected_stop_calls.append(mock.call(5))
-        # Stop now
-        wait_responses.append(True)
-
-        # Hook it up and run it
-        mock_time.side_effect = time_responses
-        mock_uniform.side_effect = uniform_responses
-        self.mock_agent.heartbeat_timeout = 50
-        self.heartbeater.api.heartbeat.side_effect = heartbeat_responses
-        self.heartbeater.stop_event.wait.side_effect = wait_responses
-        self.heartbeater.run()
-
-        # Validate expectations
-        self.assertEqual(expected_stop_calls,
-                         self.heartbeater.stop_event.wait.call_args_list)
-        self.assertEqual(self.heartbeater.api.heartbeat.call_count, 2)
-        self.assertEqual(mock_time.call_count, 5)
+        clock = FakeClock()
+        mock_time.side_effect = clock.get
+        self.heartbeater.stop_event.wait.side_effect = clock.wait
+
+        heartbeat_mock = self.heartbeater.api.heartbeat
+        self.mock_agent.heartbeat_timeout = 20
+
+        # First run right after start
+        mock_uniform.return_value = 0.6
+        self.assertTrue(self.heartbeater._run_next())
+        self.assertEqual(0, clock.last_wait)
+        heartbeat_mock.assert_called_once_with(
+            uuid=self.mock_agent.get_node_uuid.return_value,
+            advertise_address=self.mock_agent.advertise_address,
+            advertise_protocol=self.mock_agent.advertise_protocol,
+            generated_cert=self.mock_agent.generated_cert)
+        heartbeat_mock.reset_mock()
+        self.assertEqual(12, self.heartbeater.interval)  # 20*0.6
+        self.assertEqual(0, self.heartbeater.previous_heartbeat)
+
+        # A few empty runs before reaching the next heartbeat
+        for ts in [5, 10]:
+            self.assertTrue(self.heartbeater._run_next())
+            self.assertEqual(5, clock.last_wait)
+            self.assertEqual(ts, clock.current)
+            heartbeat_mock.assert_not_called()
+            self.assertEqual(0, self.heartbeater.previous_heartbeat)
+
+        # Second run when the heartbeat is due
+        mock_uniform.return_value = 0.4
+        self.assertTrue(self.heartbeater._run_next())
+        self.assertEqual(2, clock.last_wait)  # 12-2*5
+        self.assertTrue(heartbeat_mock.called)
+        heartbeat_mock.reset_mock()
+        self.assertEqual(8, self.heartbeater.interval)  # 20*0.4
+        self.assertEqual(12, self.heartbeater.previous_heartbeat)
+
+        # One empty run before reaching the next heartbeat
+        self.assertTrue(self.heartbeater._run_next())
+        self.assertEqual(5, clock.last_wait)
+        heartbeat_mock.assert_not_called()
+        self.assertEqual(12, self.heartbeater.previous_heartbeat)
+
+        # Failed run resulting in a fast retry
+        mock_uniform.return_value = 1.2
+        heartbeat_mock.side_effect = Exception('uh oh!')
+        self.assertTrue(self.heartbeater._run_next())
+        self.assertEqual(3, clock.last_wait)  # 8-5
+        self.assertTrue(heartbeat_mock.called)
+        heartbeat_mock.reset_mock(side_effect=True)
+        self.assertEqual(6, self.heartbeater.interval)  # 5*1.2
+        self.assertEqual(20, self.heartbeater.previous_heartbeat)
+
+        # One empty run because 6>5
+        self.assertTrue(self.heartbeater._run_next())
+        self.assertEqual(5, clock.last_wait)
+        heartbeat_mock.assert_not_called()
+        self.assertEqual(20, self.heartbeater.previous_heartbeat)
+
+        # Retry after the remaining 1 second
+        mock_uniform.return_value = 0.5
+        self.assertTrue(self.heartbeater._run_next())
+        self.assertEqual(1, clock.last_wait)
+        self.assertTrue(heartbeat_mock.called)
+        heartbeat_mock.reset_mock()
+        self.assertEqual(10, self.heartbeater.interval)  # 20*0.5
+        self.assertEqual(26, self.heartbeater.previous_heartbeat)
+
+        # Stop on the next empty run
+        clock.wait_result = True
+        self.assertFalse(self.heartbeater._run_next())
+        heartbeat_mock.assert_not_called()
+        self.assertEqual(26, self.heartbeater.previous_heartbeat)
 
     @mock.patch('ironic_python_agent.agent._time', autospec=True)
     def test__heartbeat_expected(self, mock_time):
 
         # initial setting
         self.heartbeater.previous_heartbeat = 0
         self.heartbeater.interval = 0
         self.heartbeater.heartbeat_forced = False
         mock_time.return_value = 0
-        self.assertFalse(self.heartbeater._heartbeat_expected())
+        self.assertTrue(self.heartbeater._heartbeat_expected())
 
         # 1st cadence
         self.heartbeater.previous_heartbeat = 0
         self.heartbeater.interval = 100
         self.heartbeater.heartbeat_forced = False
         mock_time.return_value = 5
         self.assertFalse(self.heartbeater._heartbeat_expected())
@@ -1033,15 +1061,15 @@
                           self.agent.set_agent_advertise_addr)
 
         mock_get_ipv4.assert_called_once_with('em1')
         self.assertFalse(mock_exec.called)
         self.assertFalse(mock_gethostbyname.called)
 
     def test_route_with_ip(self, mock_exec, mock_gethostbyname):
-        self.agent.api_url = 'http://1.2.1.2:8081/v1'
+        self.agent.api_urls = ['http://1.2.1.2:8081/v1']
         mock_gethostbyname.side_effect = socket.gaierror()
         mock_exec.return_value = (
             """1.2.1.2 via 192.168.122.1 dev eth0  src 192.168.122.56
                 cache """,
             ""
         )
 
@@ -1049,15 +1077,15 @@
 
         self.assertEqual(('192.168.122.56', 9990),
                          self.agent.advertise_address)
         mock_exec.assert_called_once_with('ip', 'route', 'get', '1.2.1.2')
         mock_gethostbyname.assert_called_once_with('1.2.1.2')
 
     def test_route_with_ipv6(self, mock_exec, mock_gethostbyname):
-        self.agent.api_url = 'http://[fc00:1111::1]:8081/v1'
+        self.agent.api_urls = ['http://[fc00:1111::1]:8081/v1']
         mock_gethostbyname.side_effect = socket.gaierror()
         mock_exec.return_value = (
             """fc00:101::1 dev br-ctlplane  src fc00:101::4  metric 0
                 cache """,
             ""
         )
 
@@ -1106,14 +1134,54 @@
         mock_exec.assert_called_with('ip', 'route', 'get', '1.2.1.2')
         mock_gethostbyname.assert_called_once_with('fake_api.example.org')
         mock_sleep.assert_called_with(10)
         self.assertEqual(3, mock_exec.call_count)
         self.assertEqual(2, mock_sleep.call_count)
 
     @mock.patch.object(time, 'sleep', autospec=True)
+    def test_route_several_urls_and_retries(self, mock_sleep, mock_exec,
+                                            mock_gethostbyname):
+        mock_gethostbyname.side_effect = lambda x: x
+        self.agent.api_urls = ['http://[fc00:1111::1]:8081/v1',
+                               'http://1.2.1.2:8081/v1']
+        mock_exec.side_effect = [
+            processutils.ProcessExecutionError('boom'),
+            (
+                "Error: some error text",
+                ""
+            ),
+            processutils.ProcessExecutionError('boom'),
+            (
+                """1.2.1.2 via 192.168.122.1 dev eth0  src 192.168.122.56
+                    cache """,
+                ""
+            )
+        ]
+
+        self.agent.set_agent_advertise_addr()
+
+        self.assertEqual(('192.168.122.56', 9990),
+                         self.agent.advertise_address)
+        mock_exec.assert_has_calls([
+            mock.call('ip', 'route', 'get', 'fc00:1111::1'),
+            mock.call('ip', 'route', 'get', '1.2.1.2'),
+            mock.call('ip', 'route', 'get', 'fc00:1111::1'),
+            mock.call('ip', 'route', 'get', '1.2.1.2'),
+        ])
+        mock_gethostbyname.assert_has_calls([
+            mock.call('fc00:1111::1'),
+            mock.call('1.2.1.2'),
+        ])
+        mock_sleep.assert_called_with(10)
+        self.assertEqual(4, mock_exec.call_count)
+        # Both URLs are handled in a single attempt, so only one sleep here
+        self.assertEqual(1, mock_sleep.call_count)
+        self.assertEqual(2, mock_gethostbyname.call_count)
+
+    @mock.patch.object(time, 'sleep', autospec=True)
     def test_route_failed(self, mock_sleep, mock_exec, mock_gethostbyname):
         mock_gethostbyname.return_value = '1.2.1.2'
         mock_exec.side_effect = processutils.ProcessExecutionError('boom')
 
         self.assertRaises(errors.LookupAgentIPError,
                           self.agent.set_agent_advertise_addr)
 
@@ -1193,7 +1261,16 @@
         mock_wait.assert_called_once_with(mock.ANY)
         self.assertEqual([mock.call('list_hardware_info'),
                           mock.call('wait_for_disks')],
                          mock_dispatch.call_args_list)
         self.agent.heartbeater.start.assert_called_once_with()
         self.assertEqual('1' * 128, self.agent.agent_token)
         self.assertEqual('1' * 128, self.agent.api_client.agent_token)
+
+
+class TestFromConfig(ironic_agent_base.IronicAgentTest):
+
+    def test_override_urls(self):
+        urls = ['http://[fc00:1111::1]:8081/v1', 'http://1.2.1.2:8081/v1']
+        CONF.set_override('api_url', ','.join(urls))
+        ag = agent.IronicPythonAgent.from_config(CONF)
+        self.assertEqual(urls, ag.api_urls)
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_api.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_base.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_burnin.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_burnin.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,15 +460,15 @@
                 self.members = members
 
             def get(self):
                 return self.members
 
         # we are the first node to enter, so no other host
         # initially until the second one appears after some
-        # interations
+        # iterations
         mock_coordinator.get_members.side_effect = \
             [Members(), Members([b'host1']), Members([b'host1']),
              Members([b'host1']), Members([b'host1', b'host2'])]
 
         (partner, role) = \
             burnin._find_network_burnin_partner_and_role("zk://xyz",
                                                          "group", 10)
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_dmi_inspector.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_dmi_inspector.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_efi_utils.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_efi_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -207,17 +207,17 @@
                              mock_get_part_path,
                              mock_get_part_uuid, mock_execute,
                              mock_rescan):
         efibootmgr_resp = """
 BootCurrent: 0001
 Timeout: 0 seconds
 BootOrder: 0001,0000,001B,001C,001D,001E,001F,0020,0021,0022,0012,0011,0023,0024,0002
-Boot0000* Red Hat Enterprise Linux	HD(1,GPT,34178504-2340-4fe0-8001-264372cf9b2d,0x800,0x64000)/File(\EFI\redhat\shimx64.efi)
-Boot0001* Fedora	HD(1,GPT,da6b4491-61f2-42b0-8ab1-7c4a87317c4e,0x800,0x64000)/File(\EFI\fedora\shimx64.efi)
-Boot0002* Linux-Firmware-Updater	HD(1,GPT,da6b4491-61f2-42b0-8ab1-7c4a87317c4e,0x800,0x64000)/File(\EFI\fedora\fwupdx64.efi)
+Boot0000* Red Hat Enterprise Linux	HD(1,GPT,34178504-2340-4fe0-8001-264372cf9b2d,0x800,0x64000)/File(\\EFI\\redhat\\shimx64.efi)
+Boot0001* Fedora	HD(1,GPT,da6b4491-61f2-42b0-8ab1-7c4a87317c4e,0x800,0x64000)/File(\\EFI\\fedora\\shimx64.efi)
+Boot0002* Linux-Firmware-Updater	HD(1,GPT,da6b4491-61f2-42b0-8ab1-7c4a87317c4e,0x800,0x64000)/File(\\EFI\\fedora\\fwupdx64.efi)
 Boot0003  ThinkShield secure wipe	FvFile(3593a0d5-bd52-43a0-808e-cbff5ece2477)
 Boot0004  LENOVO CLOUD	VenMsg(bc7838d2-0f82-4d60-8316-c068ee79d25b,ad38ccbbf7edf04d959cf42aa74d3650)/Uri(https://download.lenovo.com/pccbbs/cdeploy/efi/boot.efi)
 Boot0005  IDER BOOT CDROM	PciRoot(0x0)/Pci(0x14,0x0)/USB(11,1)
 Boot0006 ATA HDD	VenMsg(bc7838d2-0f82-4d60-8316-c068ee79d25b,91af625956449f41a7b91f4f892ab0f6)
 Boot0007* Hard drive C: VenHw(d6c0639f-c705-4eb9-aa4f-5802d8823de6)......................................................................................A.....................P.E.R.C. .H.7.3.0.P. .M.i.n.i.(.b.u.s. .1.8. .d.e.v. .0.0.)...
 BootAAA8* IBA GE Slot 0100 v1588        BBS(128,IBA GE Slot 0100 v1588,0x0)........................B.............................................................A.....................I.B.A. .G.E. .S.l.o.t. .0.1.0.0. .v.1.5.8.8...
 Boot0FF9* Virtual CD/DVD        PciRoot(0x0)/Pci(0x14,0x0)/USB(13,0)/USB(3,0)/USB(1,0)
@@ -225,61 +225,79 @@
 Boot000B* UEFI: PXE IPv4 Realtek PCIe 2.5GBE Family Controller	PciRoot(0x0)/Pci(0x1c,0x0)/Pci(0x0,0x0)/MAC([REDACTED],0)/IPv4(0.0.0.00.0.0.0,0,0)..BO
 Boot0008* Generic USB Boot UsbClass(ffff,ffff,255,255)
 Boot0009* Internal CD/DVD ROM Drive (UEFI)      PciRoot(0x0)/Pci(0x11,0x0)/Sata(1,65535,0)/CDROM(1,0x265,0x2000)
 """.encode('utf-16') # noqa This is a giant literal string for testing.
         mock_execute.return_value = (efibootmgr_resp, '')
         result = list(efi_utils.get_boot_records())
 
-        def assertEntry(expected, actual):
-            self.assertEqual(2, len(actual))
-            self.assertEqual(expected[0], actual[0])
-            self.assertIn(expected[1], actual[1])
-
-        assertEntry(
-            ('0000', 'Red Hat Enterprise Linux'),
+        self.assertEqual(
+            ('0000', 'Red Hat Enterprise Linux', 'HD',
+             'HD(1,GPT,34178504-2340-4fe0-8001-264372cf9b2d,0x800,0x64000)/'
+             'File(\\EFI\\redhat\\shimx64.efi)'),
             result[0])
-        assertEntry(
-            ('0001', 'Fedora'),
+        self.assertEqual(
+            ('0001', 'Fedora', 'HD',
+             'HD(1,GPT,da6b4491-61f2-42b0-8ab1-7c4a87317c4e,0x800,0x64000)/'
+             'File(\\EFI\\fedora\\shimx64.efi)'),
             result[1])
-        assertEntry(
-            ('0002', 'Linux-Firmware-Updater'),
+        self.assertEqual(
+            ('0002', 'Linux-Firmware-Updater', 'HD',
+             'HD(1,GPT,da6b4491-61f2-42b0-8ab1-7c4a87317c4e,0x800,0x64000)/'
+             'File(\\EFI\\fedora\\fwupdx64.efi)'),
             result[2])
-        assertEntry(
-            ('0003', 'ThinkShield secure wipe'),
+        self.assertEqual(
+            ('0003', 'ThinkShield secure wipe', 'FvFile',
+             'FvFile(3593a0d5-bd52-43a0-808e-cbff5ece2477)'),
             result[3])
-        assertEntry(
-            ('0004', 'LENOVO CLOUD'),
+        self.assertEqual(
+            ('0004', 'LENOVO CLOUD', 'VenMsg',
+             'VenMsg(bc7838d2-0f82-4d60-8316-c068ee79d25b,'
+             'ad38ccbbf7edf04d959cf42aa74d3650)/'
+             'Uri(https://download.lenovo.com/pccbbs/cdeploy/efi/boot.efi)'),
             result[4])
-        assertEntry(
-            ('0005', 'IDER BOOT CDROM'),
+        self.assertEqual(
+            ('0005', 'IDER BOOT CDROM', 'PciRoot',
+             'PciRoot(0x0)/Pci(0x14,0x0)/USB(11,1)'),
             result[5])
-        assertEntry(
-            ('0006', 'ATA HDD'),
+        self.assertEqual(
+            ('0006', 'ATA HDD', 'VenMsg',
+             'VenMsg(bc7838d2-0f82-4d60-8316-c068ee79d25b,'
+             '91af625956449f41a7b91f4f892ab0f6)'),
             result[6])
-        assertEntry(
-            ('0007', 'Hard drive C:'),
+        self.assertEqual(
+            ('0007', 'Hard drive C:', 'VenHw',
+             mock.ANY),
             result[7])
-        assertEntry(
-            ('AAA8', 'IBA GE Slot 0100 v1588'),
+        self.assertEqual(
+            ('AAA8', 'IBA GE Slot 0100 v1588', 'BBS',
+             mock.ANY),
             result[8])
-        assertEntry(
-            ('0FF9', 'Virtual CD/DVD'),
+        self.assertEqual(
+            ('0FF9', 'Virtual CD/DVD', 'PciRoot',
+             'PciRoot(0x0)/Pci(0x14,0x0)/USB(13,0)/USB(3,0)/USB(1,0)'),
             result[9])
-        assertEntry(
-            ('123A', 'Integrated NIC 1 Port 1 Partition 1'),
+        self.assertEqual(
+            ('123A', 'Integrated NIC 1 Port 1 Partition 1', 'VenHw',
+             'VenHw(33391845-5f86-4e78-8fce-c4cff59f9bbb)'),
             result[10])
-        assertEntry(
+        self.assertEqual(
             ('000B',
-             'UEFI: PXE IPv4 Realtek PCIe 2.5GBE Family Controller'),
+             'UEFI: PXE IPv4 Realtek PCIe 2.5GBE Family Controller',
+             'PciRoot',
+             'PciRoot(0x0)/Pci(0x1c,0x0)/Pci(0x0,0x0)/MAC([REDACTED],0)/'
+             'IPv4(0.0.0.00.0.0.0,0,0)..BO'),
             result[11])
-        assertEntry(
-            ('0008', 'Generic USB Boot'),
+        self.assertEqual(
+            ('0008', 'Generic USB Boot', 'UsbClass',
+             'UsbClass(ffff,ffff,255,255)'),
             result[12])
-        assertEntry(
-            ('0009', 'Internal CD/DVD ROM Drive (UEFI'),
+        self.assertEqual(
+            ('0009', 'Internal CD/DVD ROM Drive (UEFI)', 'PciRoot',
+             'PciRoot(0x0)/Pci(0x11,0x0)/Sata(1,65535,0)/'
+             'CDROM(1,0x265,0x2000)'),
             result[13])
 
     @mock.patch.object(os.path, 'exists', lambda *_: False)
     @mock.patch.object(hardware, 'is_md_device', autospec=True)
     @mock.patch.object(efi_utils, '_get_efi_bootloaders', autospec=True)
     @mock.patch.object(os, 'makedirs', autospec=True)
     def test_found_csv(self, mkdir_mock, mock_efi_bl, mock_is_md_device,
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_encoding.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_encoding.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_errors.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_hardware.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_hardware.py`

 * *Files 0% similar despite different names*

```diff
@@ -867,27 +867,29 @@
                                       (hws.CPUINFO_FLAGS_OUTPUT, '')]
 
         cpus = self.hardware.get_cpus()
         self.assertEqual('Intel(R) Xeon(R) CPU E5-2609 0 @ 2.40GHz',
                          cpus.model_name)
         self.assertEqual('2400.0000', cpus.frequency)
         self.assertEqual(4, cpus.count)
+        self.assertEqual(1, cpus.socket_count)
         self.assertEqual('x86_64', cpus.architecture)
         self.assertEqual(['fpu', 'vme', 'de', 'pse'], cpus.flags)
 
     @mock.patch.object(il_utils, 'execute', autospec=True)
     def test_get_cpus2(self, mocked_execute):
         mocked_execute.side_effect = [(hws.LSCPU_OUTPUT_NO_MAX_MHZ, ''),
                                       (hws.CPUINFO_FLAGS_OUTPUT, '')]
 
         cpus = self.hardware.get_cpus()
         self.assertEqual('Intel(R) Xeon(R) CPU E5-1650 v3 @ 3.50GHz',
                          cpus.model_name)
         self.assertEqual('1794.433', cpus.frequency)
         self.assertEqual(12, cpus.count)
+        self.assertEqual(1, cpus.socket_count)
         self.assertEqual('x86_64', cpus.architecture)
         self.assertEqual(['fpu', 'vme', 'de', 'pse'], cpus.flags)
 
     @mock.patch.object(il_utils, 'execute', autospec=True)
     def test_get_cpus_no_flags(self, mocked_execute):
         mocked_execute.side_effect = [(hws.LSCPU_OUTPUT, ''),
                                       processutils.ProcessExecutionError()]
@@ -3947,15 +3949,15 @@
         device2 = hardware.BlockDevice('/dev/sdb', 'sdb', 107374182400, True)
         device3 = hardware.BlockDevice('/dev/sdc', 'sdc', 107374182400, True)
         self.hardware.list_block_devices = mock.Mock()
         self.hardware.list_block_devices.side_effect = [
             [device1, device2, device3],
             [device1, device2, device3]]
 
-        # pre-creation validation fails as insufficent number of devices found
+        # pre-creation validation fails as insufficient number of devices found
         error_regex = ("Software RAID configuration is not possible for "
                        "RAID level 6 with only 3 block devices found.")
 
         # Execute is actually called for listing_block_devices
         self.assertFalse(mocked_execute.called)
         self.assertRaisesRegex(errors.SoftwareRAIDError, error_regex,
                                self.hardware.create_configuration,
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_inject_files.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_inject_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
 
         inject_files._inject_one(self.node, self.ports, fl,
                                  '/dev/root', self.http_get)
 
         with open(self.path, 'rb') as fp:
             self.assertEqual(b'content', fp.read())
         self.assertEqual(0o602, stat.S_IMODE(os.stat(self.path).st_mode))
-        # Exising directories do not change their permissions
+        # Existing directories do not change their permissions
         self.assertNotEqual(0o703, stat.S_IMODE(os.stat(self.dirpath).st_mode))
 
         mock_find_and_mount.assert_called_once_with(fl['path'], None,
                                                     '/dev/root')
         self.http_get.assert_not_called()
 
     @mock.patch.object(os, 'chown', autospec=True)
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_inspector.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_inspector.py`

 * *Files 4% similar despite different names*

```diff
@@ -157,57 +157,116 @@
     def test_ok(self, mock_post):
         failures = utils.AccumulatedFailures()
         data = collections.OrderedDict(data=42)
         mock_post.return_value.status_code = 200
 
         res = inspector.call_inspector(data, failures)
 
-        mock_post.assert_called_once_with('url',
-                                          cert=None, verify=True,
-                                          data='{"data": 42, "error": null}',
-                                          timeout=30)
+        mock_post.assert_called_once_with(
+            'url', data='{"data": 42, "error": null}',
+            cert=None, verify=True,
+            headers={'Content-Type': 'application/json',
+                     'Accept': 'application/json'},
+            timeout=30)
         self.assertEqual(mock_post.return_value.json.return_value, res)
 
     def test_send_failure(self, mock_post):
         failures = mock.Mock(spec=utils.AccumulatedFailures)
         failures.get_error.return_value = "boom"
         data = collections.OrderedDict(data=42)
         mock_post.return_value.status_code = 200
 
         res = inspector.call_inspector(data, failures)
 
         mock_post.assert_called_once_with('url',
                                           cert=None, verify=True,
                                           data='{"data": 42, "error": "boom"}',
+                                          headers=mock.ANY,
                                           timeout=30)
         self.assertEqual(mock_post.return_value.json.return_value, res)
 
     def test_inspector_error(self, mock_post):
         failures = utils.AccumulatedFailures()
         data = collections.OrderedDict(data=42)
         mock_post.return_value.status_code = 400
 
         res = inspector.call_inspector(data, failures)
 
         mock_post.assert_called_once_with('url',
                                           cert=None, verify=True,
                                           data='{"data": 42, "error": null}',
+                                          headers=mock.ANY,
                                           timeout=30)
         self.assertIsNone(res)
 
     @mock.patch.object(inspector, '_RETRY_WAIT', 0.01)
+    @mock.patch.object(inspector, '_RETRY_WAIT_MAX', 1)
     def test_inspector_retries(self, mock_post):
         mock_post.side_effect = requests.exceptions.ConnectionError
         failures = utils.AccumulatedFailures()
         data = collections.OrderedDict(data=42)
         self.assertRaises(requests.exceptions.ConnectionError,
                           inspector.call_inspector,
                           data, failures)
         self.assertEqual(5, mock_post.call_count)
 
+    @mock.patch.object(inspector, '_RETRY_WAIT', 0.01)
+    @mock.patch.object(inspector, '_RETRY_WAIT_MAX', 1)
+    def test_inspector_several_urls(self, mock_post):
+        CONF.set_override('inspection_callback_url', 'url1,url2')
+        mock_post.side_effect = [
+            requests.exceptions.ConnectionError,
+            requests.exceptions.ConnectionError,
+            mock.Mock(status_code=200),
+        ]
+        failures = utils.AccumulatedFailures()
+        data = collections.OrderedDict(data=42)
+        inspector.call_inspector(data, failures)
+        self.assertEqual(3, mock_post.call_count)
+        mock_post.assert_has_calls([
+            mock.call('url1', cert=None, verify=True, headers=mock.ANY,
+                      data='{"data": 42, "error": null}', timeout=30),
+            mock.call('url2', cert=None, verify=True, headers=mock.ANY,
+                      data='{"data": 42, "error": null}', timeout=30),
+            mock.call('url1', cert=None, verify=True, headers=mock.ANY,
+                      data='{"data": 42, "error": null}', timeout=30),
+        ])
+
+    @mock.patch.object(inspector, '_RETRY_WAIT', 0.01)
+    @mock.patch.object(inspector, '_RETRY_WAIT_MAX', 1)
+    @mock.patch.object(inspector, '_RETRY_ATTEMPTS', 3)
+    def test_inspector_retries_on_50X_error(self, mock_post):
+        mock_post.side_effect = [mock.Mock(status_code=500),
+                                 mock.Mock(status_code=409),
+                                 mock.Mock(status_code=502)]
+        failures = utils.AccumulatedFailures()
+        data = collections.OrderedDict(data=42)
+        self.assertRaises(requests.exceptions.HTTPError,
+                          inspector.call_inspector,
+                          data, failures)
+        self.assertEqual(3, mock_post.call_count)
+
+    @mock.patch.object(inspector, '_RETRY_WAIT', 0.01)
+    @mock.patch.object(inspector, '_RETRY_WAIT_MAX', 1)
+    @mock.patch.object(inspector, '_RETRY_ATTEMPTS', 3)
+    def test_inspector_retry_on_50X_and_succeed(self, mock_post):
+        mock_post.side_effect = [mock.Mock(status_code=503),
+                                 mock.Mock(status_code=409),
+                                 mock.Mock(status_code=200)]
+
+        failures = utils.AccumulatedFailures()
+        data = collections.OrderedDict(data=42)
+        inspector.call_inspector(data, failures)
+        self.assertEqual(3, mock_post.call_count)
+        mock_post.assert_called_with('url',
+                                     cert=None, verify=True,
+                                     data='{"data": 42, "error": null}',
+                                     headers=mock.ANY,
+                                     timeout=30)
+
 
 class BaseDiscoverTest(base.IronicAgentTest):
     def setUp(self):
         super(BaseDiscoverTest, self).setUp()
         self.inventory = {
             'interfaces': [
                 hardware.NetworkInterface(name='em1',
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_ironic_api_client.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_ironic_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,14 +336,24 @@
             requests.exceptions.ConnectionError
         self.assertRaisesRegex(errors.HeartbeatConnectionError,
                                'transitory network failure or blocking port',
                                self.api_client.heartbeat,
                                uuid='meow',
                                advertise_address=('192.0.2.1', '9999'))
 
+    def test_heartbeat_requests_several_urls(self):
+        self.api_client.api_urls = ['2001:db8::1', '192.0.2.1']
+        self.api_client.session.request = mock.Mock()
+        self.api_client.session.request.side_effect = [
+            requests.exceptions.ConnectionError,
+            FakeResponse(status_code=202),
+        ]
+        self.api_client.heartbeat(uuid='meow',
+                                  advertise_address=('192.0.2.1', '9999'))
+
     @mock.patch('time.sleep', autospec=True)
     @mock.patch('ironic_python_agent.ironic_api_client.APIClient._do_lookup',
                 autospec=True)
     def test_lookup_node(self, lookup_mock, sleep_mock):
         content = {
             'node': {
                 'uuid': 'deadbeef-dabb-ad00-b105-f00d00bab10c'
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_multi_hardware.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_multi_hardware.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_multi_hardware_clean_steps.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_multi_hardware_clean_steps.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_netutils.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_netutils.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_numa_inspector.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_numa_inspector.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_partition_utils.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_partition_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1497,15 +1497,15 @@
             self,
             mock_mkfs,
             mock_copy,
             mock_execute):
         mock_mkfs.side_effect = processutils.ProcessExecutionError('boom')
         self.assertRaisesRegex(
             exception.InstanceDeployFailure,
-            'A failure occured while attempting to format.*',
+            'A failure occurred while attempting to format.*',
             partition_utils._try_build_fat32_config_drive,
             self.fake_dev,
             self.configdrive_file)
         mock_execute.assert_has_calls([
             mock.call('mount', '-o', 'loop,ro', '-t', 'auto',
                       self.configdrive_file, mock.ANY),
             mock.call('umount', mock.ANY),
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_raid_utils.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_raid_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_tls_utils.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_tls_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tests/unit/test_utils.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/tls_utils.py` & `ironic-python-agent-9.9.0/ironic_python_agent/tls_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/utils.py` & `ironic-python-agent-9.9.0/ironic_python_agent/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
     else:
         return path.strip()
 
 
 def _check_vmedia_device(vmedia_device_file):
     """Check if a virtual media device appears valid.
 
-    Explicitly ignores partitions, actual disks, and other itmes that
+    Explicitly ignores partitions, actual disks, and other items that
     seem unlikely to be virtual media based items being provided
     into the running operating system via a BMC.
 
     :param vmedia_device_file: Path to the device to examine.
     :returns: False by default, True if the device appears to be
               valid.
     """
@@ -618,15 +618,15 @@
 
 
 # See ironic.drivers.utils.get_node_capability
 def _parse_capabilities_str(cap_str):
     """Extract capabilities from string.
 
     :param cap_str: string meant to meet key1:value1,key2:value2 format
-    :return: a dictionnary
+    :return: a dictionary
     """
     LOG.debug("Parsing capability string %s", cap_str)
     capabilities = {}
 
     for node_capability in cap_str.split(','):
         parts = node_capability.split(':')
         if len(parts) == 2 and parts[0] and parts[1]:
@@ -685,23 +685,23 @@
 def get_node_boot_mode(node):
     """Returns the node boot mode.
 
     It returns 'uefi' if 'secure_boot' is set to 'true' in
     'instance_info/capabilities' of node. Otherwise it directly look for boot
     mode hints into
 
-    :param node: dictionnary.
+    :param node: dictionary.
     :returns: 'bios' or 'uefi'
     """
     instance_info = node.get('instance_info', {})
     instance_info_caps = parse_capabilities(instance_info)
     node_caps = parse_capabilities(node.get('properties', {}))
 
     if _is_secure_boot(instance_info_caps, node_caps):
-        LOG.debug('Deploy boot mode is implicitely uefi for because secure '
+        LOG.debug('Deploy boot mode is implicitly uefi because secure '
                   'boot is activated.')
         return 'uefi'
 
     ramdisk_boot_mode = 'uefi' if os.path.isdir('/sys/firmware/efi') \
         else 'bios'
 
     # Priority order implemented in ironic
@@ -766,15 +766,15 @@
 
 
 def determine_time_method():
     """Helper method to determine what time utility is present.
 
     :returns: "ntpdate" if ntpdate has been found, "chrony" if chrony
               was located, and None if neither are located. If both tools
-              are present, "chrony" will supercede "ntpdate".
+              are present, "chrony" will supersede "ntpdate".
     """
     try:
         execute('chronyd', '-h')
         return 'chronyd'
     except OSError:
         LOG.debug('Command \'chronyd\' not found for time sync.')
     try:
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent/version.py` & `ironic-python-agent-9.9.0/ironic_python_agent/version.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent.egg-info/PKG-INFO` & `ironic-python-agent-9.9.0/ironic_python_agent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ironic-python-agent
-Version: 9.8.0
+Version: 9.9.0
 Summary: Ironic Python Agent Ramdisk
 Home-page: https://docs.openstack.org/ironic-python-agent/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache-2
 Description: ===================
         Ironic Python Agent
@@ -79,10 +79,11 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Provides-Extra: burnin_network_kazoo
 Provides-Extra: test
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent.egg-info/SOURCES.txt` & `ironic-python-agent-9.9.0/ironic_python_agent.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.git-blame-ignore-revs
 .stestr.conf
 AUTHORS
 CONTRIBUTING.rst
 ChangeLog
 LICENSE
 README.rst
 bindep.txt
@@ -193,23 +194,25 @@
 releasenotes/notes/check-if-ESP-is-mounted-f9e0eff3609c2668.yaml
 releasenotes/notes/check-partition-table-after-writing-34efbd557d8de7cb.yaml
 releasenotes/notes/check-virtual-media-devices-a9b1f54c3fe7884d.yaml
 releasenotes/notes/checksum-before-considering-download-completed-91cca9fef34d8cf5.yaml
 releasenotes/notes/clarify-heartbeat-connection-errors-2af152bf2d7928e2.yaml
 releasenotes/notes/clock-skew-1fbf542b193cec17.yaml
 releasenotes/notes/coalesce_heartbeats-fb8899a5f9fe4709.yaml
+releasenotes/notes/collect-cpu-sockets-0dbc09a1ebccfe77.yaml
 releasenotes/notes/collect-dmi-output-f2e9feabef16bacf.yaml
 releasenotes/notes/collect-manager-a80bcf370048eeec.yaml
 releasenotes/notes/collect-more-8bc9ad4c63e873e1.yaml
 releasenotes/notes/collect-udev-f6ada5163cf4a26c.yaml
 releasenotes/notes/command_params-869fa547b5be2236.yaml
 releasenotes/notes/configdrive-dup-3fc46a878fe82485.yaml
 releasenotes/notes/configdrive-partuuid-3259cfb7428c1483.yaml
 releasenotes/notes/configdrive-ssl-02b069948dfef814.yaml
 releasenotes/notes/container-poweroff-d9ffb637cf1cee6c.yaml
+releasenotes/notes/content-type-f4d5ab15adf37252.yaml
 releasenotes/notes/coreos-uses-chroot-8a01ba0b38a4a4f4.yaml
 releasenotes/notes/coreos_ipa_image_poweroff_reboot_in_chroot_by_sysrq-42447fc4cdd7dafe.yaml
 releasenotes/notes/correct-uefi-regex-112211c2427cd4d9.yaml
 releasenotes/notes/correction-failure-output-when-downloading-image-39f93838d1ed2928.yaml
 releasenotes/notes/cpu-flags-e3cec7e5cba069ef.yaml
 releasenotes/notes/create_raids_with_volume_name-93e0bb59ef210fe4.yaml
 releasenotes/notes/de-duplicate-by-label-baa090c5b1bff992.yaml
@@ -256,14 +259,15 @@
 releasenotes/notes/fix-mlnx-hardware-mgr-never-run-72072580be4d6e7a.yaml
 releasenotes/notes/fix-multipath-parent-device-e85afad63159250c.yaml
 releasenotes/notes/fix-nic-without-numa-node-b401f97c46afa4a1.yaml
 releasenotes/notes/fix-nvidia-hw-mgr-https-38825a4161a8561b.yaml
 releasenotes/notes/fix-nvme-partition-image-handling-b8487133a188fd32.yaml
 releasenotes/notes/fix-nvme-software-raid-race-2e0e104de9611228.yaml
 releasenotes/notes/fix-physical-memory-arm64-957755f6cd91ad85.yaml
+releasenotes/notes/fix-raid_device-not-set-8b03688ce83ce22e.yaml
 releasenotes/notes/fix-rescan-device-7b00c6836b687ce8.yaml
 releasenotes/notes/fix-rescan-device-raid-29aa1558b036b496.yaml
 releasenotes/notes/fix-softraid-name-poisoning-4e934dd4e60830b1.yaml
 releasenotes/notes/fix-to-pass-root-uuid-for-whole-disk-image-1c13b70f6b74bce0.yaml
 releasenotes/notes/fix-uefi-boot-entry-creation-for-aarch64-2b143c5bf189c2f6.yaml
 releasenotes/notes/fix-vfd-mount-for-capitalized-device-name-db7f519e900f4e22.yaml
 releasenotes/notes/fix_chronyd_time_sync-626a14b66ca37677.yaml
@@ -277,24 +281,27 @@
 releasenotes/notes/get-physical-memory-535a32362bcdf83a.yaml
 releasenotes/notes/get_md_components_by_uuid-7f08d423ea9e7c94.yaml
 releasenotes/notes/get_numa_node-eeab34a92739b6f6.yaml
 releasenotes/notes/handle-configdrive-large-disks-3517e9fcf16c7f39.yaml
 releasenotes/notes/handle-fd0-devices-3d1f31c3b34819e8.yaml
 releasenotes/notes/handle-partuuid-for-fstab-e0aadea20a056982.yaml
 releasenotes/notes/handle-ssl-063a91fb7bdcf9b9.yaml
+releasenotes/notes/heartbeat-jitter-620bbcba591d2894.yaml
 releasenotes/notes/ignore-grub-efi-fail-dcf7eb07f61f4388.yaml
 releasenotes/notes/image-checksum-39b2ceef40933c28.yaml
 releasenotes/notes/image-download-retries-65ac31fe4328e438.yaml
 releasenotes/notes/improve-tgtd-status-d17173dc8f67959f.yaml
 releasenotes/notes/inject-files-b411369ce6856dac.yaml
 releasenotes/notes/inspect-to-clean-b3616d843775c187.yaml
+releasenotes/notes/inspection-409-69d5bd6c2a49d2ec.yaml
 releasenotes/notes/inspection-to-report-disk-by-path-e3fd4c331d200903.yaml
 releasenotes/notes/inspection-wait-for-ips-223e39b65fef31bd.yaml
 releasenotes/notes/inspection-wait-for-ips-v2-146016f758d7010c.yaml
 releasenotes/notes/inspector-logs-9b7c010c219691d2.yaml
+releasenotes/notes/inspector-retry-502-2b286e2ccc64c195.yaml
 releasenotes/notes/instance-info-root-device-02fed0966bb00fb3.yaml
 releasenotes/notes/inventory-conf-29b59ebe97aefbde.yaml
 releasenotes/notes/ip6-addresses-1c2b9bcd9a124de7.yaml
 releasenotes/notes/ipa-debug-68c86101b1fdc3d9.yaml
 releasenotes/notes/ipmi-address-channel-b6b8010c41d05c1b.yaml
 releasenotes/notes/ipmi-cleanup-a4454f6851d81c4d.yaml
 releasenotes/notes/ipv6-listen-85d40e58156e398f.yaml
@@ -369,14 +376,15 @@
 releasenotes/notes/rescan-before-checking-uefi-64597c937880134d.yaml
 releasenotes/notes/rescan-device-after-mkfs-3f9d52a2e3b6fff3.yaml
 releasenotes/notes/rescue-dhcp_network-for-tinyipa-a14de5fae38a5dce.yaml
 releasenotes/notes/respect-listen-directives-94fb863c5b692c07.yaml
 releasenotes/notes/rework-ata-secure-erase-c6684962ef078281.yaml
 releasenotes/notes/root-device-hints-rotational-67e6e61074c26561.yaml
 releasenotes/notes/set-clock-prior-to-poweroff-af6ec210aad8b45a.yaml
+releasenotes/notes/several-urls-9c3b8c14338b06ba.yaml
 releasenotes/notes/skip-lookup-and-heartbeat-if-apiurl-not-configured-5ae8b04ae1e74673.yaml
 releasenotes/notes/skips-bootloader-install-35c463195aa61800.yaml
 releasenotes/notes/sleep-ebe58fbe07d30219.yaml
 releasenotes/notes/softraid-bootable-with-uefi-aa22e6cbaf1ea747.yaml
 releasenotes/notes/softraid-creation-on-nvme-a2fd4c531d200904.yaml
 releasenotes/notes/softraid-partitioning-refactor-104b817c3bdc73e3.yaml
 releasenotes/notes/softraid-zap-superblocks-anywhere.yaml
```

### Comparing `ironic-python-agent-9.8.0/ironic_python_agent.egg-info/entry_points.txt` & `ironic-python-agent-9.9.0/ironic_python_agent.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/4k-block-size-config-drives-4470828dd06d2600.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/4k-block-size-config-drives-4470828dd06d2600.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/Collect_NIC_name_given_by_BIOS-657c68c0ae16365b.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/Collect_NIC_name_given_by_BIOS-657c68c0ae16365b.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/add-service-steps-support-655cc02d112ed0a8.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/add-service-steps-support-655cc02d112ed0a8.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/add-vlan-interfaces-cdfeb39d0f3d444d.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/add-vlan-interfaces-cdfeb39d0f3d444d.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/add_burnin_dynamic_network_pairing-33e398255050eb98.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/add_burnin_dynamic_network_pairing-33e398255050eb98.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/adds-smartctl-ata-check-to-secure-erase-caebba4f25821575.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/adds-smartctl-ata-check-to-secure-erase-caebba4f25821575.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ---
 fixes:
   - |
     Adds an additional check if the ``smartctl`` utility is present from the
     ``smartmontools`` package, which performs an ATA disk specific check that
-    should prevent ATA Secure Erase from being performed if a pass-thru
+    should prevent ATA Secure Erase from being performed if a pass-through
     device is detected that requires a non-ATA command signling sequence.
     Devices such as these can be `smart` disk interfaces such as
     RAID controllers and USB disk adapters, which can cause failures
     when attempting to Secure Erase, which may render the disk unreachable.
```

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/allows-bootloader-install-failure-to-be-ignored-b99667b13afa9759.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/allows-bootloader-install-failure-to-be-ignored-b99667b13afa9759.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -3,13 +3,13 @@
   - |
     Adds an configuration option which can be encoded into the ramdisk itself
     or the PXE parameters being provided to instruct the agent to ignore
     bootloader installation or configuration failures. This functionality is
     useful to work around well-intentioned hardware which is auto-populating
     all possible device into the UEFI nvram firmware in order to try and help
     ensure the machine boots. Except, this can also mean any
-    explict configuration attempt will fail. Operators needing this bypass
+    explicit configuration attempt will fail. Operators needing this bypass
     can use the ``ipa-ignore-bootloader-failure`` configuration option on the
     PXE command line or utilize the ``ignore_bootloader_failure`` option
     for the Ramdisk configuration.
-    In a future version of ironic, this setting may be able to be overriden
+    In a future version of ironic, this setting may be able to be overridden
     by ironic node level configuration.
```

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/ataraid_does_not_appear_as_disk-8a260e66b3496bf6.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/ataraid_does_not_appear_as_disk-8a260e66b3496bf6.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/attempts-ata-disk-unlock-897d76c494ec2976.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/attempts-ata-disk-unlock-897d76c494ec2976.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/bandit-fixes-a971142075b29ca9.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/bandit-fixes-a971142075b29ca9.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/basic-auth-for-user-image-server-150835e7567444da.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/basic-auth-for-user-image-server-150835e7567444da.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/check-virtual-media-devices-a9b1f54c3fe7884d.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/check-virtual-media-devices-a9b1f54c3fe7884d.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/configdrive-partuuid-3259cfb7428c1483.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/configdrive-partuuid-3259cfb7428c1483.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/deprecate-coreos-8b01bcf796c0dc54.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/deprecate-coreos-8b01bcf796c0dc54.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     This decision is not taken lightly, and is due to multiple constraints
     combined with technical changes over time as CoreOS has evolved.
 
     Per the `CoreOS limitations <https://coreos.com/os/docs/latest/booting-with-iso.html#known-limitations>`_,
     as of January 2019, CoreOS:
 
     1) Current CoreOS images require 2GB of RAM to operate.
-    As a result of the RAM requirement, it is problematic for continious
+    As a result of the RAM requirement, it is problematic for continuous
     integration testing to occur with the CoreOS based Ironic-Python-Agent
     image in OpenStack testing infrastructure.
 
     2) UEFI is not a supported configuration. CoreOS details the required
     use of BIOS compatibility mode. Intel is anticipated to remove
     BIOS compatibility by `2020 <https://arstechnica.com/gadgets/2017/11/intel-to-kill-off-the-last-vestiges-of-the-ancient-pc-bios-by-2020/>`_.
```

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/enable-cleaning-fallback-57e8c9aa2f24e63d.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/enable-cleaning-fallback-57e8c9aa2f24e63d.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/fix-iscsi-teardown-handling-0df2345318d3c843.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/fix-iscsi-teardown-handling-0df2345318d3c843.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/fixes-centos-fedora-grub2-mkconfig-hang-fe22cde231994044.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/fixes-centos-fedora-grub2-mkconfig-hang-fe22cde231994044.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/handle-partuuid-for-fstab-e0aadea20a056982.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/handle-partuuid-for-fstab-e0aadea20a056982.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/handle-ssl-063a91fb7bdcf9b9.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/handle-ssl-063a91fb7bdcf9b9.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/ignore-grub-efi-fail-dcf7eb07f61f4388.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/ignore-grub-efi-fail-dcf7eb07f61f4388.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/jitter-for-inspection-command-5a226927757a0308.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/jitter-for-inspection-command-5a226927757a0308.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/lshw-for-memory-and-system-info-35c69da067c72b36.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/lshw-for-memory-and-system-info-35c69da067c72b36.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/manual-introspection-b04b5c25f5e004ac.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/manual-introspection-b04b5c25f5e004ac.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/multipath-handling-00a5b412d2cf2e4e.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/multipath-handling-00a5b412d2cf2e4e.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   - |
     Fixes failures with handling of Multipath IO devices where Active/Passive
     storage arrays are in use. Previously, "standby" paths could result in
     IO errors causing cleaning to terminate. The agent now explicitly attempts
     to handle and account for multipaths based upon the MPIO data available.
     This requires the ``multipath`` and ``multipathd`` utility to be present
     in the ramdisk. These are supplied by the ``device-mapper-multipath`` or
-    ``multipath-tools`` packages, and are not requried for the agent's use.
+    ``multipath-tools`` packages, and are not required for the agent's use.
   - |
     Fixes non-ideal behavior when performing cleaning where Active/Active
     MPIO devices would ultimately be cleaned once per IO path, instead of
     once per backend device.
 other:
   - |
     The agent will now attempt to collect any multipath path information
```

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/multipath_error_handling_improvement-1669d0de4bfdbe95.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/multipath_error_handling_improvement-1669d0de4bfdbe95.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/prevent-deletion-of-shared-disk-filesystems-4c17c7666d2fe3bc.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/prevent-deletion-of-shared-disk-filesystems-4c17c7666d2fe3bc.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/softraid-bootable-with-uefi-aa22e6cbaf1ea747.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/softraid-bootable-with-uefi-aa22e6cbaf1ea747.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/softraid-partitioning-refactor-104b817c3bdc73e3.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/softraid-partitioning-refactor-104b817c3bdc73e3.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/stream-raw-images-d2e245aaed991d86.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/stream-raw-images-d2e245aaed991d86.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/support-bootloader-csv-file-use-c815b520c600cd98.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/support-bootloader-csv-file-use-c815b520c600cd98.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/support-lldp-in-inventory-4ab6e45ccd35dace.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/support-lldp-in-inventory-4ab6e45ccd35dace.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/releasenotes/notes/understand-node-conflict-is-locked-2ea21dd45abfe4f7.yaml` & `ironic-python-agent-9.9.0/releasenotes/notes/understand-node-conflict-is-locked-2ea21dd45abfe4f7.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ---
 fixes:
   - |
     Fixes, or at least lessens the case where a running Ironic agent can stack
     up numerous lookup requests against an Ironic deployment when a node is
-    locked. In particular, this is beause the lookup also drives generation of
+    locked. In particular, this is because the lookup also drives generation of
     the agent token, which requires the conductor to allocate a worker, and
     generate the token, and return the result to the API client.
     Ironic's retry logic will now wait up to ``60`` seconds, and if an HTTP
     Conflict (409) message is received, the agent will automatically pause
     lookup operations for thirty seconds as opposed continue to attempt
     lookups which could create more work for the Ironic deployment
     needlessly.
```

### Comparing `ironic-python-agent-9.8.0/releasenotes/source/conf.py` & `ironic-python-agent-9.9.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/requirements.txt` & `ironic-python-agent-9.9.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/setup.cfg` & `ironic-python-agent-9.9.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 	Programming Language :: Python
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [files]
 packages = 
 	ironic_python_agent
 
 [entry_points]
 oslo.config.opts = 
@@ -51,20 +52,19 @@
 	logs = ironic_python_agent.inspector:collect_logs
 	extra-hardware = ironic_python_agent.inspector:collect_extra_hardware
 	pci-devices = ironic_python_agent.inspector:collect_pci_devices_info
 	numa-topology = ironic_python_agent.numa_inspector:collect_numa_topology_info
 	dmi-decode = ironic_python_agent.dmi_inspector:collect_dmidecode_info
 	lldp = ironic_python_agent.inspector:collect_lldp
 
-[pbr]
-autodoc_index_modules = True
-api_doc_dir = contributor/api
+[extras]
+burnin-network-kazoo = 
+	kazoo>=2.8.0 # Apache-2.0
+
+[codespell]
+quiet-level = 4
+ignore-words-list = cna
 
 [egg_info]
 tag_build = 
 tag_date = 0
-tag_svn_revision = 0
-
-[extras]
-burnin-network-kazoo = 
-	kazoo>=2.8.0 # Apache-2.0
```

### Comparing `ironic-python-agent-9.8.0/setup.py` & `ironic-python-agent-9.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/tools/bandit.yml` & `ironic-python-agent-9.9.0/tools/bandit.yml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/tools/config/check_uptodate.sh` & `ironic-python-agent-9.9.0/tools/config/check_uptodate.sh`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/tools/run_bashate.sh` & `ironic-python-agent-9.9.0/tools/run_bashate.sh`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.8.0/tox.ini` & `ironic-python-agent-9.9.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -20,32 +20,41 @@
     http_proxy
     HTTP_PROXY
     https_proxy
     HTTPS_PROXY
     no_proxy
     NO_PROXY
 
+[testenv:codespell]
+description =
+  Run codespell to check spelling
+deps = codespell
+# note(JayF): {posargs} lets us run `tox -ecodespell -- -w` to get codespell
+#             to correct spelling issues in our code it's aware of.
+commands =
+  codespell {posargs}
+
 [testenv:functional]
 # Define virtualenv directory, port to use for functional testing, and number
 # of seconds to wait for the agent to come alive during functional testing.
 setenv =
   VIRTUAL_ENV={envdir}
   PYTHONDONTWRITEBYTECODE = 1
   OS_TEST_PATH=./ironic_python_agent/tests/functional
   TEST_PORT=9999
   IPA_WAIT_TRIES=100
 commands = stestr run {posargs}
 
 [testenv:pep8]
 deps =
-    hacking~=6.0.0 # Apache-2.0
-    bashate>=0.5.1 # Apache-2.0
-    flake8-import-order>=0.17.1 # LGPLv3
+    hacking~=6.1.0 # Apache-2.0
+    bashate~=2.1.0 # Apache-2.0
+    flake8-import-order~=0.18.0 # LGPLv3
     pycodestyle>=2.0.0,<3.0.0 # MIT
-    doc8>=0.8.1 # Apache-2.0
+    doc8~=1.1.0 # Apache-2.0
 allowlist_externals = bash
                       {toxinidir}/tools/run_bashate.sh
 commands =
   flake8 {posargs:ironic_python_agent examples}
   # Run bashate during pep8 runs to ensure violations are caught by
   # the check and gate queues.
   {toxinidir}/tools/run_bashate.sh {toxinidir}
```

### Comparing `ironic-python-agent-9.8.0/zuul.d/ironic-python-agent-jobs.yaml` & `ironic-python-agent-9.9.0/zuul.d/ironic-python-agent-jobs.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -165,7 +165,14 @@
 - job:
     name: ipa-tempest-bios-ipmi-direct-tinyipa-src
     parent: ipa-tempest-bios-ipmi-direct-src
     vars:
       devstack_localrc:
         IRONIC_RAMDISK_TYPE: tinyipa
         IRONIC_VM_SPECS_RAM: 1024
+
+- job:
+    name: ipa-tox-codespell
+    parent: openstack-tox
+    timeout: 7200
+    vars:
+      tox_envlist: codespell
```

### Comparing `ironic-python-agent-9.8.0/zuul.d/project.yaml` & `ironic-python-agent-9.9.0/zuul.d/project.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
         - ironic-python-agent-check-image-tinyipa:
             voting: false
         - ironic-python-agent-check-image-dib-centos9:
             voting: false
         # Non-voting jobs
         - ipa-tempest-ironic-inspector-src:
             voting: false
+        - ipa-tox-codespell:
+            voting: false
     gate:
       jobs:
         - openstack-tox-functional
         - ipa-tox-bandit
         - ipa-tox-examples
         - ipa-tempest-bios-ipmi-direct-src
         - ipa-tempest-uefi-redfish-vmedia-src
```

