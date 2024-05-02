# Comparing `tmp/shepherd_core-2024.4.2.tar.gz` & `tmp/shepherd_core-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shepherd_core-2024.4.2.tar", last modified: Wed Apr 24 19:38:56 2024, max compression
+gzip compressed data, was "shepherd_core-2024.5.1.tar", last modified: Thu May  2 10:00:36 2024, max compression
```

## Comparing `shepherd_core-2024.4.2.tar` & `shepherd_core-2024.5.1.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.229001 shepherd_core-2024.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-04-24 19:38:56.229001 shepherd_core-2024.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.205001 shepherd_core-2024.4.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/experiment_from_yaml.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/experiment_generic_var1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/experiment_generic_var2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/experiment_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/firmware_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/firmware_modification.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/uart_decode_waveform.py
--rw-r--r--   0 runner    (1001) docker     (127)   229877 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/uart_raw2.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/vharvester_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/vsource_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:38:56.229001 shepherd_core-2024.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.205001 shepherd_core-2024.4.2/shepherd_core/
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/calibration_hw_def.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.209001 shepherd_core-2024.4.2/shepherd_core/data_models/
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.209001 shepherd_core-2024.4.2/shepherd_core/data_models/base/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/base/cal_measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)    10320 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/base/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/base/content.py
--rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/base/shepherd.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/base/timezone.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/base/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.209001 shepherd_core-2024.4.2/shepherd_core/data_models/content/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12259 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/content/_external_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/content/energy_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/content/energy_environment_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/content/firmware.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/content/firmware_datatype.py
--rw-r--r--   0 runner    (1001) docker     (127)     9448 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/content/virtual_harvester.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/content/virtual_harvester_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14142 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/content/virtual_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/content/virtual_source_fixture.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.209001 shepherd_core-2024.4.2/shepherd_core/data_models/experiment/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/experiment/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/experiment/observer_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/experiment/target_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.213001 shepherd_core-2024.4.2/shepherd_core/data_models/task/
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/task/emulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/task/firmware_mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/task/harvest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/task/observer_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/task/programming.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/task/testbed_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.213001 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/cape.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/cape_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/gpio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/gpio_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/mcu.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/mcu_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/observer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/observer_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/target.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/target_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/testbed.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/testbed_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/virtual_source_doc.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.213001 shepherd_core-2024.4.2/shepherd_core/decoder_waveform/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/decoder_waveform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/decoder_waveform/uart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.217001 shepherd_core-2024.4.2/shepherd_core/fw_tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/fw_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/fw_tools/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/fw_tools/converter_elf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/fw_tools/patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/fw_tools/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.217001 shepherd_core-2024.4.2/shepherd_core/inventory/
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/inventory/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/inventory/system.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/inventory/target.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    26245 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.217001 shepherd_core-2024.4.2/shepherd_core/testbed_client/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/testbed_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/testbed_client/cache_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/testbed_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/testbed_client/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/testbed_client/user_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.217001 shepherd_core-2024.4.2/shepherd_core/vsource/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/vsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/vsource/virtual_converter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/vsource/virtual_harvester_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/vsource/virtual_source_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14482 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.229001 shepherd_core-2024.4.2/shepherd_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-04-24 19:38:56.000000 shepherd_core-2024.4.2/shepherd_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-24 19:38:56.000000 shepherd_core-2024.4.2/shepherd_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:38:56.000000 shepherd_core-2024.4.2/shepherd_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-24 19:38:56.000000 shepherd_core-2024.4.2/shepherd_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 19:38:56.000000 shepherd_core-2024.4.2/shepherd_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:38:55.000000 shepherd_core-2024.4.2/shepherd_core.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.217001 shepherd_core-2024.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.221001 shepherd_core-2024.4.2/tests/data_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_cal_data.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_cal_data_faulty.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_cal_meas.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_cal_meas_faulty1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_cal_meas_faulty2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_config_emulator.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_config_experiment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_config_experiment_alternative.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_config_harvester.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_config_testbed.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_config_virtsource.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/test_base_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/test_content_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/test_content_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/test_experiment_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/test_task_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/test_task_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/test_testbed_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/test_testbed_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.225001 shepherd_core-2024.4.2/tests/decoder_waveform/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/decoder_waveform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/decoder_waveform/test_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.225001 shepherd_core-2024.4.2/tests/fw_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/fw_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   345592 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/fw_tools/build_msp.elf
--rw-r--r--   0 runner    (1001) docker     (127)   887576 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/fw_tools/build_nrf.elf
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/fw_tools/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/fw_tools/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/fw_tools/test_patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/fw_tools/test_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.225001 shepherd_core-2024.4.2/tests/inventory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/inventory/test_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/test_cal_hw.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9560 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.225001 shepherd_core-2024.4.2/tests/testbed_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/testbed_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.229001 shepherd_core-2024.4.2/tests/vsource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/vsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/vsource/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/vsource/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/vsource/test_harvester.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/vsource/test_z.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.330633 shepherd_core-2024.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-02 10:00:36.330633 shepherd_core-2024.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.306633 shepherd_core-2024.5.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/examples/experiment_from_yaml.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/examples/experiment_generic_var1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/examples/experiment_generic_var2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/examples/experiment_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/examples/firmware_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/examples/firmware_modification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/examples/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/examples/uart_decode_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (127)   229877 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/examples/uart_raw2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/examples/vharvester_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/examples/vsource_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 10:00:36.330633 shepherd_core-2024.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.306633 shepherd_core-2024.5.1/shepherd_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/calibration_hw_def.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.310633 shepherd_core-2024.5.1/shepherd_core/data_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.310633 shepherd_core-2024.5.1/shepherd_core/data_models/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/base/cal_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/base/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/base/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/base/shepherd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/base/timezone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/base/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.310633 shepherd_core-2024.5.1/shepherd_core/data_models/content/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12259 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/content/_external_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/content/energy_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/content/energy_environment_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/content/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/content/firmware_datatype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9448 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/content/virtual_harvester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/content/virtual_harvester_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14142 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/content/virtual_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/content/virtual_source_fixture.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.314633 shepherd_core-2024.5.1/shepherd_core/data_models/experiment/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/experiment/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/experiment/observer_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/experiment/target_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.314633 shepherd_core-2024.5.1/shepherd_core/data_models/task/
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/task/emulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/task/firmware_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/task/harvest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/task/observer_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/task/programming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/task/testbed_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.318633 shepherd_core-2024.5.1/shepherd_core/data_models/testbed/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/testbed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/testbed/cape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/testbed/cape_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/testbed/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/testbed/gpio_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/testbed/mcu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/testbed/mcu_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/testbed/observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/testbed/observer_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/testbed/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/testbed/target_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/testbed/testbed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/testbed/testbed_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/data_models/virtual_source_doc.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.318633 shepherd_core-2024.5.1/shepherd_core/decoder_waveform/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/decoder_waveform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/decoder_waveform/uart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.318633 shepherd_core-2024.5.1/shepherd_core/fw_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/fw_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/fw_tools/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/fw_tools/converter_elf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/fw_tools/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/fw_tools/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.318633 shepherd_core-2024.5.1/shepherd_core/inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/inventory/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/inventory/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/inventory/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26245 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.318633 shepherd_core-2024.5.1/shepherd_core/testbed_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/testbed_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/testbed_client/cache_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/testbed_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/testbed_client/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/testbed_client/user_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.318633 shepherd_core-2024.5.1/shepherd_core/vsource/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/vsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/vsource/virtual_converter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/vsource/virtual_harvester_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/vsource/virtual_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14475 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/shepherd_core/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.330633 shepherd_core-2024.5.1/shepherd_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-02 10:00:36.000000 shepherd_core-2024.5.1/shepherd_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-05-02 10:00:36.000000 shepherd_core-2024.5.1/shepherd_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:00:36.000000 shepherd_core-2024.5.1/shepherd_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-02 10:00:36.000000 shepherd_core-2024.5.1/shepherd_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-02 10:00:36.000000 shepherd_core-2024.5.1/shepherd_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:00:36.000000 shepherd_core-2024.5.1/shepherd_core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.322633 shepherd_core-2024.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.326633 shepherd_core-2024.5.1/tests/data_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/example_cal_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/example_cal_data_faulty.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/example_cal_meas.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/example_cal_meas_faulty1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/example_cal_meas_faulty2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/example_config_emulator.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/example_config_experiment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/example_config_experiment_alternative.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/example_config_harvester.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/example_config_testbed.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/example_config_virtsource.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/test_base_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/test_content_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/test_content_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/test_experiment_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/test_task_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/test_task_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/test_testbed_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/data_models/test_testbed_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.326633 shepherd_core-2024.5.1/tests/decoder_waveform/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/decoder_waveform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/decoder_waveform/test_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.326633 shepherd_core-2024.5.1/tests/fw_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/fw_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   345592 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/fw_tools/build_msp.elf
+-rw-r--r--   0 runner    (1001) docker     (127)   887576 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/fw_tools/build_nrf.elf
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/fw_tools/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/fw_tools/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/fw_tools/test_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/fw_tools/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.326633 shepherd_core-2024.5.1/tests/inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/inventory/test_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/test_cal_hw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9560 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.326633 shepherd_core-2024.5.1/tests/testbed_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/testbed_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:36.330633 shepherd_core-2024.5.1/tests/vsource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/vsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/vsource/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/vsource/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/vsource/test_harvester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-02 10:00:29.000000 shepherd_core-2024.5.1/tests/vsource/test_z.py
```

### Comparing `shepherd_core-2024.4.2/PKG-INFO` & `shepherd_core-2024.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd_core
-Version: 2024.4.2
+Version: 2024.5.1
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Author-email: Ingmar Splitt <ingmar.splitt@tu-dresden.de>
 Maintainer-email: Ingmar Splitt <ingmar.splitt@tu-dresden.de>
 Project-URL: Documentation, https://github.com/orgua/shepherd-datalib/blob/main/README.md
 Project-URL: Issues, https://github.com/orgua/shepherd-datalib/issues
 Project-URL: Source, https://pypi.org/project/shepherd-core/
 Keywords: testbed,beaglebone,pru,batteryless,energyharvesting,solar
```

### Comparing `shepherd_core-2024.4.2/README.md` & `shepherd_core-2024.5.1/README.md`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/examples/experiment_from_yaml.yaml` & `shepherd_core-2024.5.1/examples/experiment_from_yaml.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/examples/experiment_generic_var1.py` & `shepherd_core-2024.5.1/examples/experiment_generic_var1.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/examples/experiment_generic_var2.py` & `shepherd_core-2024.5.1/examples/experiment_generic_var2.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/examples/experiment_models.py` & `shepherd_core-2024.5.1/examples/experiment_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/examples/firmware_model.py` & `shepherd_core-2024.5.1/examples/firmware_model.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/examples/firmware_modification.py` & `shepherd_core-2024.5.1/examples/firmware_modification.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/examples/inventory.py` & `shepherd_core-2024.5.1/examples/inventory.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/examples/uart_decode_waveform.py` & `shepherd_core-2024.5.1/examples/uart_decode_waveform.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/examples/uart_raw2.csv` & `shepherd_core-2024.5.1/examples/uart_raw2.csv`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/examples/vharvester_simulation.py` & `shepherd_core-2024.5.1/examples/vharvester_simulation.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/examples/vsource_simulation.py` & `shepherd_core-2024.5.1/examples/vsource_simulation.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/pyproject.toml` & `shepherd_core-2024.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/__init__.py` & `shepherd_core-2024.5.1/shepherd_core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from .logger import increase_verbose_level
 from .logger import logger
 from .reader import Reader
 from .testbed_client.client import TestbedClient
 from .testbed_client.client import tb_client
 from .writer import Writer
 
-__version__ = "2024.4.2"
+__version__ = "2024.5.1"
 
 __all__ = [
     "Reader",
     "Writer",
     "get_verbose_level",
     "increase_verbose_level",
     "logger",
```

### Comparing `shepherd_core-2024.4.2/shepherd_core/calibration_hw_def.py` & `shepherd_core-2024.5.1/shepherd_core/calibration_hw_def.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/__init__.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/base/cal_measurement.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/base/cal_measurement.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/base/calibration.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/base/calibration.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 
     def si_to_raw(self, values_si: Calc_t) -> Calc_t:
         """Convert between physical units and raw unsigned integers."""
         values_raw = (values_si - self.offset) / self.gain
         if isinstance(values_raw, np.ndarray):
             values_raw[values_raw < 0.0] = 0.0
             values_raw = np.around(values_raw)
+            # TODO: overflow should also be prevented (add bit-width) -> fail or warn at both?
         else:
             values_raw = round(max(values_raw, 0.0))
         return values_raw
 
     @classmethod
     def from_fn(cls, fn: Callable) -> Self:
         """Probe linear function to determine scaling values."""
```

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/base/content.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/base/content.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/base/shepherd.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/base/shepherd.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/base/timezone.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/base/timezone.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/base/wrapper.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/base/wrapper.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/content/__init__.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/content/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/content/_external_fixtures.yaml` & `shepherd_core-2024.5.1/shepherd_core/data_models/content/_external_fixtures.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/content/energy_environment.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/content/energy_environment.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/content/energy_environment_fixture.yaml` & `shepherd_core-2024.5.1/shepherd_core/data_models/content/energy_environment_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/content/firmware.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/content/firmware.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/content/virtual_harvester.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/content/virtual_harvester.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/content/virtual_harvester_fixture.yaml` & `shepherd_core-2024.5.1/shepherd_core/data_models/content/virtual_harvester_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/content/virtual_source.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/content/virtual_source.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/content/virtual_source_fixture.yaml` & `shepherd_core-2024.5.1/shepherd_core/data_models/content/virtual_source_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/experiment/__init__.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/experiment/experiment.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/experiment/observer_features.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/experiment/observer_features.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/experiment/target_config.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/experiment/target_config.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/readme.md` & `shepherd_core-2024.5.1/shepherd_core/data_models/readme.md`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/task/__init__.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/task/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/task/emulation.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/task/emulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     # ⤷ Overwrite existing file
     output_compression: Optional[Compression] = Compression.default
     # ⤷ should be lzf, 1 (gzip level 1) or None (order of recommendation)
     time_start: Optional[datetime] = None
     # timestamp or unix epoch time, None = ASAP
     duration: Optional[timedelta] = None
     # ⤷ Duration of recording in seconds, None = till EOF
-    abort_on_error: bool = False
+    abort_on_error: bool = False  # TODO: remove, should not exist
 
     # emulation-specific
     use_cal_default: bool = False
     # ⤷ Use default calibration values, skip loading from EEPROM
 
     enable_io: bool = False
     # TODO: add direction of pins! also it seems error-prone when only setting _tracing
```

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/task/firmware_mod.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/task/firmware_mod.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/task/harvest.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/task/harvest.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/task/observer_tasks.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/task/observer_tasks.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/task/programming.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/task/programming.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/task/testbed_tasks.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/task/testbed_tasks.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/testbed/__init__.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/testbed/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/testbed/cape.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/testbed/cape.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/testbed/cape_fixture.yaml` & `shepherd_core-2024.5.1/shepherd_core/data_models/testbed/cape_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/testbed/gpio.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/testbed/gpio.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/testbed/gpio_fixture.yaml` & `shepherd_core-2024.5.1/shepherd_core/data_models/testbed/gpio_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/testbed/mcu.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/testbed/mcu.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/testbed/mcu_fixture.yaml` & `shepherd_core-2024.5.1/shepherd_core/data_models/testbed/mcu_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/testbed/observer.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/testbed/observer.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/testbed/observer_fixture.yaml` & `shepherd_core-2024.5.1/shepherd_core/data_models/testbed/observer_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/testbed/target.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/testbed/target.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/testbed/target_fixture.yaml` & `shepherd_core-2024.5.1/shepherd_core/data_models/testbed/target_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/testbed/testbed.py` & `shepherd_core-2024.5.1/shepherd_core/data_models/testbed/testbed.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/testbed/testbed_fixture.yaml` & `shepherd_core-2024.5.1/shepherd_core/data_models/testbed/testbed_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/data_models/virtual_source_doc.txt` & `shepherd_core-2024.5.1/shepherd_core/data_models/virtual_source_doc.txt`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/decoder_waveform/uart.py` & `shepherd_core-2024.5.1/shepherd_core/decoder_waveform/uart.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/fw_tools/__init__.py` & `shepherd_core-2024.5.1/shepherd_core/fw_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/fw_tools/converter.py` & `shepherd_core-2024.5.1/shepherd_core/fw_tools/converter.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/fw_tools/converter_elf.py` & `shepherd_core-2024.5.1/shepherd_core/fw_tools/converter_elf.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/fw_tools/patcher.py` & `shepherd_core-2024.5.1/shepherd_core/fw_tools/patcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .validation import is_elf
 
 try:
     from pwnlib.elf import ELF
 except ImportError as e:
     ELF = None
     elf_error_text = (
-        "Please install functionality with 'pip install shepherd_core[elf] -U' first, "
+        "Please install functionality with 'pip install shepherd-core[elf] -U' first, "
         f"underlying exception: {e.msg}"
     )
 
 
 @validate_call
 def find_symbol(file_elf: Path, symbol: str) -> bool:
     """Find a symbol in the ELF file."""
```

### Comparing `shepherd_core-2024.4.2/shepherd_core/fw_tools/validation.py` & `shepherd_core-2024.5.1/shepherd_core/fw_tools/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 try:
     from elftools.common.exceptions import ELFError
     from pwnlib.elf import ELF
 except ImportError as e:
     ELF = None
     ELFError = None
     elf_error_text = (
-        "Please install functionality with 'pip install shepherd_core[elf] -U' first, "
+        "Please install functionality with 'pip install shepherd-core[elf] -U' first, "
         f"underlying exception: {e.msg}"
     )
 
 
 @validate_call
 def is_hex(file: Path) -> bool:
     """Check if file is containing intel-hex data."""
```

### Comparing `shepherd_core-2024.4.2/shepherd_core/inventory/__init__.py` & `shepherd_core-2024.5.1/shepherd_core/inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/inventory/python.py` & `shepherd_core-2024.5.1/shepherd_core/inventory/python.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/inventory/system.py` & `shepherd_core-2024.5.1/shepherd_core/inventory/system.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/logger.py` & `shepherd_core-2024.5.1/shepherd_core/logger.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/reader.py` & `shepherd_core-2024.5.1/shepherd_core/reader.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/testbed_client/client.py` & `shepherd_core-2024.5.1/shepherd_core/testbed_client/client.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/testbed_client/fixtures.py` & `shepherd_core-2024.5.1/shepherd_core/testbed_client/fixtures.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/testbed_client/user_model.py` & `shepherd_core-2024.5.1/shepherd_core/testbed_client/user_model.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/vsource/virtual_converter_model.py` & `shepherd_core-2024.5.1/shepherd_core/vsource/virtual_converter_model.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/vsource/virtual_harvester_model.py` & `shepherd_core-2024.5.1/shepherd_core/vsource/virtual_harvester_model.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/vsource/virtual_source_model.py` & `shepherd_core-2024.5.1/shepherd_core/vsource/virtual_source_model.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/shepherd_core/writer.py` & `shepherd_core-2024.5.1/shepherd_core/writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,15 @@
         self.is_valid()
         self.h5file.close()
 
     def _create_skeleton(self) -> None:
         """Initialize the structure of the HDF5 file.
 
         HDF5 is hierarchically structured and before writing data, we have to
-        setup this structure, i.e. creating the right groups with corresponding
+        set up this structure, i.e. creating the right groups with corresponding
         data types. We will store 3 types of data in a database: The
         actual IV samples recorded either from the harvester (during recording)
         or the target (during emulation). Any log messages, that can be used to
         store relevant events or tag some parts of the recorded data.
 
         """
         # Store voltage and current samples in the data group,
@@ -363,15 +363,15 @@
 
     def store_config(self, data: dict) -> None:
         """Get a better self-describing Output-File.
 
         TODO: use data-model?
         :param data: from virtual harvester or converter / source.
         """
-        self.h5file["data"].attrs["config"] = yaml.safe_dump(
+        self.h5file.attrs["config"] = yaml.safe_dump(
             data, default_flow_style=False, sort_keys=False
         )
 
     def store_hostname(self, name: str) -> None:
         """Option to distinguish the host, target or data-source -> perfect for plotting later.
 
         :param name: something unique, or "artificial" in case of generated content
```

### Comparing `shepherd_core-2024.4.2/shepherd_core.egg-info/PKG-INFO` & `shepherd_core-2024.5.1/shepherd_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd_core
-Version: 2024.4.2
+Version: 2024.5.1
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Author-email: Ingmar Splitt <ingmar.splitt@tu-dresden.de>
 Maintainer-email: Ingmar Splitt <ingmar.splitt@tu-dresden.de>
 Project-URL: Documentation, https://github.com/orgua/shepherd-datalib/blob/main/README.md
 Project-URL: Issues, https://github.com/orgua/shepherd-datalib/issues
 Project-URL: Source, https://pypi.org/project/shepherd-core/
 Keywords: testbed,beaglebone,pru,batteryless,energyharvesting,solar
```

### Comparing `shepherd_core-2024.4.2/shepherd_core.egg-info/SOURCES.txt` & `shepherd_core-2024.5.1/shepherd_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/conftest.py` & `shepherd_core-2024.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/data_models/example_cal_data.yaml` & `shepherd_core-2024.5.1/tests/data_models/example_cal_data.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/data_models/example_cal_data_faulty.yaml` & `shepherd_core-2024.5.1/tests/data_models/example_cal_data_faulty.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/data_models/example_cal_meas.yaml` & `shepherd_core-2024.5.1/tests/data_models/example_cal_meas.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/data_models/example_cal_meas_faulty1.yaml` & `shepherd_core-2024.5.1/tests/data_models/example_cal_meas_faulty1.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/data_models/example_cal_meas_faulty2.yaml` & `shepherd_core-2024.5.1/tests/data_models/example_cal_meas_faulty2.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/data_models/example_config_emulator.yaml` & `shepherd_core-2024.5.1/tests/data_models/example_config_emulator.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/data_models/example_config_harvester.yaml` & `shepherd_core-2024.5.1/tests/data_models/example_config_harvester.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/data_models/example_config_virtsource.yaml` & `shepherd_core-2024.5.1/tests/data_models/example_config_virtsource.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/data_models/test_base_models.py` & `shepherd_core-2024.5.1/tests/data_models/test_base_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/data_models/test_content_fixtures.py` & `shepherd_core-2024.5.1/tests/data_models/test_content_fixtures.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/data_models/test_content_models.py` & `shepherd_core-2024.5.1/tests/data_models/test_content_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/data_models/test_examples.py` & `shepherd_core-2024.5.1/tests/data_models/test_examples.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/data_models/test_experiment_models.py` & `shepherd_core-2024.5.1/tests/data_models/test_experiment_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/data_models/test_task_generation.py` & `shepherd_core-2024.5.1/tests/data_models/test_task_generation.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/data_models/test_task_models.py` & `shepherd_core-2024.5.1/tests/data_models/test_task_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/data_models/test_testbed_fixtures.py` & `shepherd_core-2024.5.1/tests/data_models/test_testbed_fixtures.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/data_models/test_testbed_models.py` & `shepherd_core-2024.5.1/tests/data_models/test_testbed_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/decoder_waveform/test_decoder.py` & `shepherd_core-2024.5.1/tests/decoder_waveform/test_decoder.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/fw_tools/build_msp.elf` & `shepherd_core-2024.5.1/tests/fw_tools/build_msp.elf`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/fw_tools/build_nrf.elf` & `shepherd_core-2024.5.1/tests/fw_tools/build_nrf.elf`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/fw_tools/test_converter.py` & `shepherd_core-2024.5.1/tests/fw_tools/test_converter.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/fw_tools/test_patcher.py` & `shepherd_core-2024.5.1/tests/fw_tools/test_patcher.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/fw_tools/test_validation.py` & `shepherd_core-2024.5.1/tests/fw_tools/test_validation.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/inventory/test_inventory.py` & `shepherd_core-2024.5.1/tests/inventory/test_inventory.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/test_cal_hw.py` & `shepherd_core-2024.5.1/tests/test_cal_hw.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/test_examples.py` & `shepherd_core-2024.5.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/test_reader.py` & `shepherd_core-2024.5.1/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/test_writer.py` & `shepherd_core-2024.5.1/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/vsource/conftest.py` & `shepherd_core-2024.5.1/tests/vsource/conftest.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/vsource/test_converter.py` & `shepherd_core-2024.5.1/tests/vsource/test_converter.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.2/tests/vsource/test_harvester.py` & `shepherd_core-2024.5.1/tests/vsource/test_harvester.py`

 * *Files identical despite different names*

