# Comparing `tmp/edgepi-python-sdk-1.2.6.tar.gz` & `tmp/edgepi-python-sdk-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgepi-python-sdk-1.2.6.tar", last modified: Wed Aug  2 23:31:42 2023, max compression
+gzip compressed data, was "edgepi-python-sdk-1.2.8.tar", last modified: Thu Sep  7 18:52:20 2023, max compression
```

## Comparing `edgepi-python-sdk-1.2.6.tar` & `edgepi-python-sdk-1.2.8.tar`

### file list

```diff
@@ -1,209 +1,209 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.050837 edgepi-python-sdk-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-08-02 23:31:42.046836 edgepi-python-sdk-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 23:31:42.050837 edgepi-python-sdk-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.022836 edgepi-python-sdk-1.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.026836 edgepi-python-sdk-1.2.6/src/edgepi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.026836 edgepi-python-sdk-1.2.6/src/edgepi/adc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_conv_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_multiplexers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_query_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_voltage.py
--rw-r--r--   0 runner    (1001) docker     (123)    38761 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/edgepi_adc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.030836 edgepi-python-sdk-1.2.6/src/edgepi/calibration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/calibration/calibration_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/calibration/edgepi_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.030836 edgepi-python-sdk-1.2.6/src/edgepi/dac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/dac/dac_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/dac/dac_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13470 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/dac/edgepi_dac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.030836 edgepi-python-sdk-1.2.6/src/edgepi/digital_input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/digital_input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/digital_input/digital_input_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/digital_input/edgepi_digital_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.030836 edgepi-python-sdk-1.2.6/src/edgepi/digital_output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/digital_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/digital_output/digital_output_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/digital_output/edgepi_digital_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.030836 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/edgepi_eeprom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/edgepi_eeprom_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/eeprom_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.030836 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.030836 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_adc_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_dac_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_key_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_rtd_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_tc_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.034836 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/adc_module_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/calibration_parameters_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/dac_module_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/edgepi_module_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/keys_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/rtd_module_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/tc_module_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.034836 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/proto_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/proto_files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.034836 edgepi-python-sdk-1.2.6/src/edgepi/gpio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/gpio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/gpio/edgepi_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/gpio/edgepi_gpio_chip.py
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/gpio/edgepi_gpio_expander.py
--rw-r--r--   0 runner    (1001) docker     (123)    16842 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/gpio/gpio_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/gpio/gpio_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.034836 edgepi-python-sdk-1.2.6/src/edgepi/led/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/led/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/led/edgepi_leds.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/led/led_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.034836 edgepi-python-sdk-1.2.6/src/edgepi/peripherals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/peripherals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/peripherals/gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/peripherals/i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/peripherals/pwm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/peripherals/spi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.034836 edgepi-python-sdk-1.2.6/src/edgepi/pwm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/pwm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/pwm/edgepi_pwm.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/pwm/pwm_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.034836 edgepi-python-sdk-1.2.6/src/edgepi/reg_helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/reg_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/reg_helper/reg_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.034836 edgepi-python-sdk-1.2.6/src/edgepi/relay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/relay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/relay/edgepi_relay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/edgepi/tc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/tc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21394 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/tc/edgepi_tc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/tc/tc_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/tc/tc_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/tc/tc_conv_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/tc/tc_faults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/edgepi/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/utilities/crc_8_atm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/utilities/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/edgepi_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-08-02 23:31:42.000000 edgepi-python-sdk-1.2.6/src/edgepi_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-08-02 23:31:42.000000 edgepi-python-sdk-1.2.6/src/edgepi_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:31:42.000000 edgepi-python-sdk-1.2.6/src/edgepi_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-02 23:31:42.000000 edgepi-python-sdk-1.2.6/src/edgepi_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 23:31:42.000000 edgepi-python-sdk-1.2.6/src/edgepi_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.022836 edgepi-python-sdk-1.2.6/src/test_edgepi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_adc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_adc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_adc/test_adc.py
--rw-r--r--   0 runner    (1001) docker     (123)    55717 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_adc/test_adc_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_dac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_dac/test_dac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_digital_in/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_digital_in/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_digital_in/test_digital_in.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_digital_out/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_digital_out/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_digital_out/test_digital_out.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_eeprom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_eeprom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_eeprom/test_eeprom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_gpio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_gpio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_gpio/test_gpio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_led/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_led/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_led/test_led.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.042837 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_peripherals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_peripherals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_peripherals/test_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_peripherals/test_i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_peripherals/test_spi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.042837 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_pwm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_pwm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_pwm/test_edgepi_pwm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.042837 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_relay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_relay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_relay/test_relay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.042837 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_tc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_tc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_tc/test_tc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.042837 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.042837 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    24417 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_conv_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_multiplexers.py
--rw-r--r--   0 runner    (1001) docker     (123)    29323 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_voltage.py
--rw-r--r--   0 runner    (1001) docker     (123)    45764 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_edgepi_adc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.042837 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_calibration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_calibration/test_edgepi_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_calibration/test_protobuf_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.042837 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_dac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_dac/test_dac_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    19916 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_dac/test_edgepi_dac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.042837 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_din/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_din/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_din/test_edgepi_din.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.042837 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_dout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_dout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_dout/test_edgepi_dout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.046836 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_eeprom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_eeprom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_eeprom/read_serialized.py
--rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_eeprom/test_access_eeprom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_eeprom/test_edgepi_eeprom_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.046836 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio_expander.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/test_edgpepi_gpio_chip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/test_gpio_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/test_gpio_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.046836 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_peripherals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_peripherals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_peripherals/test_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_peripherals/test_i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_peripherals/test_pwm.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_peripherals/test_spi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.046836 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_pwm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_pwm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17768 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_pwm/test_edgepi_pwm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.046836 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_reg_helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_reg_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15302 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_reg_helper/test_reg_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.046836 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_relay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_relay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_relay/test_relay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.046836 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_tc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_tc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24741 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_tc/test_edgepi_tc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21079 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_tc/test_tc_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    39495 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_tc/test_tc_conv_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_tc/test_tc_faults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.046836 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_utilities/test_crc_8_atm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_utilities/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.079639 edgepi-python-sdk-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6298 2023-09-07 18:52:20.079639 edgepi-python-sdk-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-07 18:52:20.079639 edgepi-python-sdk-1.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.035639 edgepi-python-sdk-1.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.039639 edgepi-python-sdk-1.2.8/src/edgepi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.043639 edgepi-python-sdk-1.2.8/src/edgepi/adc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/adc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/adc/adc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14779 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/adc/adc_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8273 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/adc/adc_conv_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/adc/adc_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/adc/adc_multiplexers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15154 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/adc/adc_query_lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/adc/adc_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/adc/adc_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/adc/adc_voltage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39031 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/adc/edgepi_adc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.043639 edgepi-python-sdk-1.2.8/src/edgepi/calibration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/calibration/calibration_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/calibration/edgepi_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.043639 edgepi-python-sdk-1.2.8/src/edgepi/dac/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/dac/dac_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/dac/dac_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/dac/edgepi_dac.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.043639 edgepi-python-sdk-1.2.8/src/edgepi/digital_input/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/digital_input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/digital_input/digital_input_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/digital_input/edgepi_digital_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.047639 edgepi-python-sdk-1.2.8/src/edgepi/digital_output/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/digital_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/digital_output/digital_output_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/digital_output/edgepi_digital_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.047639 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16841 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/edgepi_eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/edgepi_eeprom_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/eeprom_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.047639 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.047639 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_adc_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_dac_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_key_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_rtd_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_tc_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.051639 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/generated_pb2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/generated_pb2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/generated_pb2/adc_module_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/generated_pb2/calibration_parameters_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/generated_pb2/dac_module_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/generated_pb2/edgepi_module_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/generated_pb2/keys_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/generated_pb2/rtd_module_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/generated_pb2/tc_module_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.051639 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/proto_files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/proto_files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.051639 edgepi-python-sdk-1.2.8/src/edgepi/gpio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/gpio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/gpio/edgepi_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/gpio/edgepi_gpio_chip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9510 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/gpio/edgepi_gpio_expander.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16842 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/gpio/gpio_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9348 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/gpio/gpio_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.051639 edgepi-python-sdk-1.2.8/src/edgepi/led/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/led/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/led/edgepi_leds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/led/led_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.051639 edgepi-python-sdk-1.2.8/src/edgepi/peripherals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/peripherals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/peripherals/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/peripherals/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/peripherals/pwm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/peripherals/spi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.055639 edgepi-python-sdk-1.2.8/src/edgepi/pwm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/pwm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/pwm/edgepi_pwm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/pwm/pwm_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.055639 edgepi-python-sdk-1.2.8/src/edgepi/reg_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/reg_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/reg_helper/reg_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.055639 edgepi-python-sdk-1.2.8/src/edgepi/relay/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/relay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/relay/edgepi_relay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.055639 edgepi-python-sdk-1.2.8/src/edgepi/tc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/tc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21496 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/tc/edgepi_tc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11643 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/tc/tc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12909 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/tc/tc_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/tc/tc_conv_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/tc/tc_faults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.055639 edgepi-python-sdk-1.2.8/src/edgepi/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/utilities/crc_8_atm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/edgepi/utilities/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.059639 edgepi-python-sdk-1.2.8/src/edgepi_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6298 2023-09-07 18:52:20.000000 edgepi-python-sdk-1.2.8/src/edgepi_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2023-09-07 18:52:20.000000 edgepi-python-sdk-1.2.8/src/edgepi_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-07 18:52:20.000000 edgepi-python-sdk-1.2.8/src/edgepi_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-09-07 18:52:20.000000 edgepi-python-sdk-1.2.8/src/edgepi_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-09-07 18:52:20.000000 edgepi-python-sdk-1.2.8/src/edgepi_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.035639 edgepi-python-sdk-1.2.8/src/test_edgepi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.059639 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.059639 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_adc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_adc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21046 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_adc/test_adc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55717 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_adc/test_adc_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.059639 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_dac/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_dac/test_dac.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.059639 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_digital_in/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_digital_in/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_digital_in/test_digital_in.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.059639 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_digital_out/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_digital_out/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_digital_out/test_digital_out.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.063639 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_eeprom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_eeprom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_eeprom/test_eeprom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.063639 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_gpio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_gpio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_gpio/test_gpio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.063639 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_led/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_led/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_led/test_led.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.063639 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_peripherals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_peripherals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_peripherals/test_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_peripherals/test_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_peripherals/test_spi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.063639 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_pwm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_pwm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_pwm/test_edgepi_pwm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.063639 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_relay/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_relay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_relay/test_relay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.067639 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_tc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_tc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11253 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_tc/test_tc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.067639 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.067639 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_adc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_adc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_adc/test_adc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24417 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_adc/test_adc_conv_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_adc/test_adc_multiplexers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29323 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_adc/test_adc_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_adc/test_adc_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_adc/test_adc_voltage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45764 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_adc/test_edgepi_adc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.067639 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_calibration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_calibration/test_edgepi_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_calibration/test_protobuf_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.071639 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_dac/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_dac/test_dac_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19916 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_dac/test_edgepi_dac.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.071639 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_din/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_din/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_din/test_edgepi_din.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.071639 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_dout/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_dout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5439 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_dout/test_edgepi_dout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.071639 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_eeprom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_eeprom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_eeprom/read_serialized.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14738 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_eeprom/test_access_eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_eeprom/test_edgepi_eeprom_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.075639 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_gpio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_gpio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7406 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10422 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio_expander.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_gpio/test_edgpepi_gpio_chip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7758 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_gpio/test_gpio_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_gpio/test_gpio_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.075639 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_peripherals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_peripherals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_peripherals/test_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_peripherals/test_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_peripherals/test_pwm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_peripherals/test_spi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.075639 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_pwm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_pwm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17806 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_pwm/test_edgepi_pwm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.075639 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_reg_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_reg_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15302 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_reg_helper/test_reg_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.075639 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_relay/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_relay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_relay/test_relay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.079639 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_tc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_tc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24741 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_tc/test_edgepi_tc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21079 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_tc/test_tc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39495 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_tc/test_tc_conv_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6345 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_tc/test_tc_faults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:52:20.079639 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_utilities/test_crc_8_atm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2023-09-07 18:51:45.000000 edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_utilities/test_utilities.py
```

### Comparing `edgepi-python-sdk-1.2.6/LICENSE` & `edgepi-python-sdk-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/PKG-INFO` & `edgepi-python-sdk-1.2.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: edgepi-python-sdk
-Version: 1.2.6
-Summary: EdgePi Python SDK package
-Home-page: https://github.com/EdgePi-Cloud/edgepi-python-sdk
-Author: S.Park
-Author-email: spark@osensa.com
-Project-URL: Bug Tracker, https://github.com/EdgePi-Cloud/edgepi-python-sdk/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![Image](https://user-images.githubusercontent.com/3793563/207438826-bb656ca5-f19d-4699-8cb4-35acccb2ce58.svg)
 
 EdgePi is a DIN rail-mounted, Raspberry Pi 4 industrial PC with the features of a Programmable Logic Controller (PLC), and Internet of Things (IoT) cloud edge device. Visit [edgepi.com](https://www.edgepi.com) for more information.
 
 ![](https://github.com/EdgePi-Cloud/edgepi-python-sdk/actions/workflows/python-unit-test.yml/badge.svg)
 ![](https://github.com/EdgePi-Cloud/edgepi-python-sdk/actions/workflows/python-lint.yml/badge.svg)
 [![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/EdgePi-Cloud/edgepi-python-sdk/blob/main/LICENSE)
```

### Comparing `edgepi-python-sdk-1.2.6/README.md` & `edgepi-python-sdk-1.2.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: edgepi-python-sdk
+Version: 1.2.8
+Summary: EdgePi Python SDK package
+Home-page: https://github.com/EdgePi-Cloud/edgepi-python-sdk
+Author: S.Park
+Author-email: spark@osensa.com
+Project-URL: Bug Tracker, https://github.com/EdgePi-Cloud/edgepi-python-sdk/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: python-periphery>=2.3.0
+Requires-Dist: bitstring>=3.1.9
+Requires-Dist: protobuf>=3.20
+
 ![Image](https://user-images.githubusercontent.com/3793563/207438826-bb656ca5-f19d-4699-8cb4-35acccb2ce58.svg)
 
 EdgePi is a DIN rail-mounted, Raspberry Pi 4 industrial PC with the features of a Programmable Logic Controller (PLC), and Internet of Things (IoT) cloud edge device. Visit [edgepi.com](https://www.edgepi.com) for more information.
 
 ![](https://github.com/EdgePi-Cloud/edgepi-python-sdk/actions/workflows/python-unit-test.yml/badge.svg)
 ![](https://github.com/EdgePi-Cloud/edgepi-python-sdk/actions/workflows/python-lint.yml/badge.svg)
 [![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/EdgePi-Cloud/edgepi-python-sdk/blob/main/LICENSE)
```

### Comparing `edgepi-python-sdk-1.2.6/setup.py` & `edgepi-python-sdk-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as file:
     long_description = file.read()
 
 setuptools.setup(
     name="edgepi-python-sdk",
-    version="1.2.6",
+    version="1.2.8",
     author="S.Park",
     author_email="spark@osensa.com",
     description="EdgePi Python SDK package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EdgePi-Cloud/edgepi-python-sdk",
     project_urls={
```

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_commands.py` & `edgepi-python-sdk-1.2.8/src/edgepi/adc/adc_commands.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_constants.py` & `edgepi-python-sdk-1.2.8/src/edgepi/adc/adc_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_conv_time.py` & `edgepi-python-sdk-1.2.8/src/edgepi/adc/adc_conv_time.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_exceptions.py` & `edgepi-python-sdk-1.2.8/src/edgepi/adc/adc_exceptions.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_multiplexers.py` & `edgepi-python-sdk-1.2.8/src/edgepi/adc/adc_multiplexers.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_query_lang.py` & `edgepi-python-sdk-1.2.8/src/edgepi/adc/adc_query_lang.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_state.py` & `edgepi-python-sdk-1.2.8/src/edgepi/adc/adc_state.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_status.py` & `edgepi-python-sdk-1.2.8/src/edgepi/adc/adc_status.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_voltage.py` & `edgepi-python-sdk-1.2.8/src/edgepi/adc/adc_voltage.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/adc/edgepi_adc.py` & `edgepi-python-sdk-1.2.8/src/edgepi/adc/edgepi_adc.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,18 +208,19 @@
         Returns:
             `list`: a list of ints representing bytes formatted as [reg_1_data, reg_2_data,...]
                 where reg_1_data is the data of the register at start_addx.
         """
         if num_regs < 1:
             raise ValueError("Number of registers to read must be at least 1")
         code = self.adc_ops.read_register_command(start_addx.value, num_regs)
-        out = self.transfer(code)
-        _logger.debug(f"__read_register: received {out}")
-        # first 2 entries are null bytes
-        return out[2:]
+        with self.spi_open():
+            out = self.transfer(code)
+            _logger.debug(f"__read_register: received {out}")
+            # first 2 entries are null bytes
+            return out[2:]
 
     def __write_register(self, start_addx: ADCReg, data: list[int]):
         """
         Write data to ADC registers, either individually or as a block.
 
         Args:
             `start_addx` (ADCReg): address of register to start writing data from.
@@ -227,15 +228,16 @@
             `data` (list): list of int values, where each value represents a byte of data
                 to write to a register.
         """
         if len(data) < 1:
             raise ValueError("Number of registers to write to must be at least 1")
         code = self.adc_ops.write_register_command(start_addx.value, data)
         _logger.debug(f"__write_register: sending {code}")
-        out = self.transfer(code)
+        with self.spi_open():
+            out = self.transfer(code)
         return out
 
     def __set_rtd_pin(self, enable: bool = False):
         """
         Set or clear RTD_EN pin
         Args:
             enable (bool): RTD enable flag
@@ -269,20 +271,22 @@
             self.gpio.clear_pin_state(ADCPins.GNDSW_IN2.value)
 
     def stop_conversions(self, adc_num: ADCNum):
         """
         Halt voltage read conversions when ADC is set to perform continuous conversions
         """
         stop_cmd = self.adc_ops.stop_adc(adc_num=adc_num.value)
-        self.transfer(stop_cmd)
+        with self.spi_open():
+            self.transfer(stop_cmd)
 
     def __send_start_command(self, adc_num: ADCNum):
         """Triggers ADC conversion(s)"""
         start_cmd = self.adc_ops.start_adc(adc_num=adc_num.value)
-        self.transfer(start_cmd)
+        with self.spi_open():
+            self.transfer(start_cmd)
 
     def start_conversions(self, adc_num: ADCNum):
         """
         Start ADC voltage read conversions. If ADC is continuous conversion mode,
         this method must be called before performing reads. If ADC is in
         pulse conversion mode, this method does not need to be called before
         performing reads.
@@ -317,15 +321,16 @@
         Clearing this bit allows subsequent non-standard resets to be detected (by reading the
         STATUS byte of a voltage read).
         """
         self.__config(reset_clear=ADCPower.RESET_CLEAR)
 
     def __read_data(self, adc: ADCNum, data_size: int):
         """Sends command to ADC to get new voltage conversion data"""
-        return self.transfer([adc.value.read_cmd] + [255] * data_size)
+        with self.spi_open():
+            return self.transfer([adc.value.read_cmd] + [255] * data_size)
 
     def __voltage_read(self, adc_num: ADCNum):
         """
         Performs ADC voltage read and formats output into status, voltage,
         and check bytes
 
         Returns:
@@ -550,27 +555,29 @@
 
     def reset(self):
         """
         Reset ADC register values to EdgePi ADC power-on state.
         Note this state differs from ADS1263 default power-on, due to
         application of custom power-on configurations required by EdgePi.
         """
-        self.transfer(self.adc_ops.reset_adc())
+        with self.spi_open():
+            self.transfer(self.adc_ops.reset_adc())
         self.__reapply_config()
 
     def __is_data_ready(self, adc_num: ADCNum):
         # pylint: disable=unused-private-member
         # required for integration testing in test_conversion_times.py
         """Utility for testing conversion times, returns True if ADC indicates new voltage data"""
-        read_data = self.transfer([adc_num.value.read_cmd] + [255] * 6)
-        if adc_num is ADCNum.ADC_1:
-            ready = (read_data[1] & 0b01000000) == 0b01000000
-        if adc_num is ADCNum.ADC_2:
-            ready = (read_data[1] & 0b10000000) == 0b10000000
-        return ready
+        with self.spi_open():
+            read_data = self.transfer([adc_num.value.read_cmd] + [255] * 6)
+            if adc_num is ADCNum.ADC_1:
+                ready = (read_data[1] & 0b01000000) == 0b01000000
+            if adc_num is ADCNum.ADC_2:
+                ready = (read_data[1] & 0b10000000) == 0b10000000
+            return ready
 
     def __read_registers_to_map(self):
         """
         Reads value of all ADC registers to a dictionary
 
         Returns:
             `dict`: contains {register addx (int): register_value (int)} pairs
```

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/calibration/calibration_constants.py` & `edgepi-python-sdk-1.2.8/src/edgepi/calibration/calibration_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/calibration/edgepi_calibration.py` & `edgepi-python-sdk-1.2.8/src/edgepi/calibration/edgepi_calibration.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/dac/dac_commands.py` & `edgepi-python-sdk-1.2.8/src/edgepi/dac/dac_commands.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/dac/dac_constants.py` & `edgepi-python-sdk-1.2.8/src/edgepi/dac/dac_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/dac/edgepi_dac.py` & `edgepi-python-sdk-1.2.8/src/edgepi/dac/edgepi_dac.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,15 +120,16 @@
         dac_gain = CalibConst.DAC_GAIN_FACTOR.value if self.__get_gain_state() else 1
         self.dac_ops.check_range(analog_out.value, 0, NUM_PINS-1)
         self.dac_ops.check_range(voltage, 0, (UPPER_LIMIT*dac_gain))
         code = self.dac_ops.voltage_to_code(analog_out.value, voltage, dac_gain)
         self.log.debug(f'Code: {code}')
 
         # update DAC register
-        self.transfer(self.dac_ops.generate_write_and_update_command(analog_out.value, code))
+        with self.spi_open():
+            self.transfer(self.dac_ops.generate_write_and_update_command(analog_out.value, code))
         # send voltage to analog out pin
         self.__send_to_gpio_pins(analog_out.value, voltage)
         return code
 
     def set_power_mode(self, analog_out: DACChannel, power_mode: PowerMode):
         """
         Set power mode for individual DAC channels to either normal power consumption,
@@ -141,23 +142,25 @@
 
             `power_mode` (PowerMode): a valid hex code for setting DAC channel power mode
         """
         self.dac_ops.check_range(analog_out.value, 0, NUM_PINS-1)
         self.__dac_power_state[analog_out.value] = power_mode.value
         power_code = self.dac_ops.generate_power_code(self.__dac_power_state.values())
         cmd = self.dac_ops.combine_command(COM.COM_POWER_DOWN_OP.value, NULL_BITS, power_code)
-        self.transfer(cmd)
+        with self.spi_open():
+            self.transfer(cmd)
 
     def reset(self):
         """
         Performs a software reset of the EdgePi DAC to power-on default values,
         and stops all voltage transmissions through pins.
         """
         cmd = self.dac_ops.combine_command(COM.COM_SW_RESET.value, NULL_BITS, SW_RESET)
-        self.transfer(cmd)
+        with self.spi_open():
+            self.transfer(cmd)
 
     def channel_readback(self, analog_out: DACChannel) -> int:
         """
         Readback the input register of DAC.
 
         Args:
             `analog_out` (DACChannel): the analog out pin to read voltage from
@@ -166,18 +169,19 @@
             voltage
         """
         self.dac_ops.check_range(analog_out.value, 0, NUM_PINS-1)
         # first transfer triggers read mode, second is needed to fetch data
         cmd = self.dac_ops.combine_command(
                 COM.COM_READBACK.value, DACChannel(analog_out.value).value, NULL_BITS
             )
-        self.transfer(cmd)
-        # all zero dummy command to trigger second transfer which
-        # contains the DAC register contents.
-        read_data = self.transfer([NULL_BITS, NULL_BITS, NULL_BITS])
+        with self.spi_open():
+            self.transfer(cmd)
+            # all zero dummy command to trigger second transfer which
+            # contains the DAC register contents.
+            read_data = self.transfer([NULL_BITS, NULL_BITS, NULL_BITS])
         self.log.debug(f"reading code {read_data}")
         return self.dac_ops.extract_read_data(read_data)
 
 
     def compute_expected_voltage(self, analog_out: DACChannel) -> float:
         """
         Computes expected voltage from the DAC channel corresponding to analog out pin.
@@ -243,26 +247,27 @@
         self.log.debug(f'Code: {codes}')
 
         # When the DAC_GAIN is enabled/disabled, the output voltage is doubled/halved instantly.
         # This may damage the circuit that the output is connected to. Therefore, enabling/disabling
         # gain have different steps of sending code value and toggling the GPIO pin.
 
         # gain being enabled, change code first than enable gain
-        if set_gain:
-            for ch, code in enumerate(codes):
-                # update DAC register
-                self.transfer(self.dac_ops.generate_write_and_update_command(ch, code))
-            self.gpio.set_pin_state(GainPin.DAC_GAIN.value)
-
-        # Disabling gain, change gain first than change codes
-        else:
-            self.gpio.clear_pin_state(GainPin.DAC_GAIN.value)
-            for ch, code in enumerate(codes):
-                # update DAC register
-                self.transfer(self.dac_ops.generate_write_and_update_command(ch, code))
+        with self.spi_open():
+            if set_gain:
+                for ch, code in enumerate(codes):
+                    # update DAC register
+                    self.transfer(self.dac_ops.generate_write_and_update_command(ch, code))
+                self.gpio.set_pin_state(GainPin.DAC_GAIN.value)
+
+            # Disabling gain, change gain first than change codes
+            else:
+                self.gpio.clear_pin_state(GainPin.DAC_GAIN.value)
+                for ch, code in enumerate(codes):
+                    # update DAC register
+                    self.transfer(self.dac_ops.generate_write_and_update_command(ch, code))
 
     def set_dac_gain(self, set_gain: bool, auto_code_change: bool = False):
         """
         Enable/Disable internal DAC gain.
         Args:
             set_gain (bool): True enable DAC gain, False disable DAC gain
             auto_code_change (bool): flag to re-write code value of each channel to keep the same
```

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/digital_input/edgepi_digital_input.py` & `edgepi-python-sdk-1.2.8/src/edgepi/digital_input/edgepi_digital_input.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/digital_output/edgepi_digital_output.py` & `edgepi-python-sdk-1.2.8/src/edgepi/digital_output/edgepi_digital_output.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/edgepi_eeprom.py` & `edgepi-python-sdk-1.2.8/src/edgepi/eeprom/edgepi_eeprom.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,16 @@
         Args:
             offset: memory offset,
                     - reserved offset = EdgePiMemoryInfo.USED_SPACE.value
                     - userspace offset = EdgePiMemoryInfo.USER_SPACE_START_BYTE.value
         Return:
             length (int): size of memory to read
         '''
-        read_data = self.__sequential_read(offset, EEPROMInfo.PAGE_SIZE.value)
+        with self.i2c_open():
+            read_data = self.__sequential_read(offset, EEPROMInfo.PAGE_SIZE.value)
         check_crc(read_data[:-1], read_data[-1])
         return (read_data[0]<<8)| read_data[1]
 
     def __generate_data_list(self, data_b: bytes):
         """
         Transform data bytes to list with 255 filling the remainder of the last page. The remainder
         is calculated with the page size of PAGE_SIZE-CRC_BYTE_SIZE because we want to insert CRC
@@ -120,18 +121,19 @@
         data = self.__generate_data_list(pb_serial_list)
         # length of data + # of CRC to be added, # of CRC = # of pages
         expected_data_size = len(data) + len(data)/(EEPROMInfo.PAGE_SIZE.value-CRC_BYTE_SIZE)
         self.__parameter_sanity_check(start_mem, expected_data_size, False)
         pages = self.__generate_list_of_pages_crc(data)
 
         mem_offset = start_mem
-        for page in pages:
-            self.__page_write_register(mem_offset, page)
-            mem_offset = mem_offset+len(page)
-            time.sleep(PAGE_WRITE_CYCLE_TIME)
+        with self.i2c_open():
+            for page in pages:
+                self.__page_write_register(mem_offset, page)
+                mem_offset = mem_offset+len(page)
+                time.sleep(PAGE_WRITE_CYCLE_TIME)
 
     def __read_edgepi_reserved_memory(self):
         '''
         Read Edgepi reserved memory space to retreive parameters. This function will return byte
         strings, that can be converted into protocol buffer message format
         Args:
             N/A
@@ -145,19 +147,20 @@
 
         # Calculated number of pages being used
         num_pages = (buff_and_len)/(page_size-CRC_BYTE_SIZE) \
                     if buff_and_len%(page_size-CRC_BYTE_SIZE) == 0 else\
                     int((buff_and_len)/(page_size-CRC_BYTE_SIZE))+1
 
         mem_offset = EdgePiMemoryInfo.PRIVATE_SPACE_START_BYTE.value
-        for page in range(num_pages):
-            buff_list = self.__sequential_read(mem_offset+(page*page_size), page_size)
-            check_crc(buff_list[:-1], buff_list[-1])
-            buff+=buff_list[:-1]
-            time.sleep(0.01)
+        with self.i2c_open():
+            for page in range(num_pages):
+                buff_list = self.__sequential_read(mem_offset+(page*page_size), page_size)
+                check_crc(buff_list[:-1], buff_list[-1])
+                buff+=buff_list[:-1]
+                time.sleep(0.01)
         return bytes(buff[2:buff_and_len])
 
     def read_edgepi_data(self):
         """
         Read Edgepi reserved memory space and populate dataclass
         Args:
             N/A
@@ -286,18 +289,19 @@
         # Calculated number of pages being used
         if buff_and_len%(page_size-CRC_BYTE_SIZE) == 0:
             num_pages = (buff_and_len)/(page_size-CRC_BYTE_SIZE)
         else:
             num_pages = int((buff_and_len)/(page_size-CRC_BYTE_SIZE))+1
 
         mem_offset = EdgePiMemoryInfo.USER_SPACE_START_BYTE.value
-        for page in range(num_pages):
-            buff_list = self.__sequential_read(mem_offset+(page*page_size), page_size)
-            check_crc(buff_list[:-1], buff_list[-1])
-            buff+=buff_list[:-1]
+        with self.i2c_open():
+            for page in range(num_pages):
+                buff_list = self.__sequential_read(mem_offset+(page*page_size), page_size)
+                check_crc(buff_list[:-1], buff_list[-1])
+                buff+=buff_list[:-1]
         return buff[2:buff_and_len]
 
     def write_user_space(self, data: bytes):
         """
         Writes data to the eeprom
         Args:
             data (bytes): serialized json data
@@ -310,18 +314,19 @@
         data = self.__generate_data_list(data)
         # length of data + # of CRC to be added, # of CRC = # of pages
         expected_data_size = len(data) + len(data)/(EEPROMInfo.PAGE_SIZE.value-CRC_BYTE_SIZE)
         self.__parameter_sanity_check(start_mem, expected_data_size, True)
         pages = self.__generate_list_of_pages_crc(data)
 
         mem_offset = start_mem
-        for page in pages:
-            self.__page_write_register(mem_offset, page)
-            mem_offset = mem_offset+len(page)
-            time.sleep(PAGE_WRITE_CYCLE_TIME)
+        with self.i2c_open():
+            for page in pages:
+                self.__page_write_register(mem_offset, page)
+                mem_offset = mem_offset+len(page)
+                time.sleep(PAGE_WRITE_CYCLE_TIME)
 
 # TODO why not separate it into a class
     def init_memory(self):
         """
         Initial Memory Reading
         Args:
             N/A
@@ -377,18 +382,19 @@
         start_address_page = EdgePiMemoryInfo.USER_SPACE_START_BYTE.value
         page_size = EEPROMInfo.PAGE_SIZE.value
         tatal_page = EdgePiMemoryInfo.USER_SPACE_END_PAGE.value - \
                      EdgePiMemoryInfo.USER_SPACE_START_PAGE.value + 1
         reset_vals = [255] * page_size
 
         mem_offset = start_address_page
-        for _ in range(tatal_page):
-            self.__page_write_register(mem_offset, reset_vals)
-            mem_offset = mem_offset+page_size
-            time.sleep(PAGE_WRITE_CYCLE_TIME)
+        with self.i2c_open():
+            for _ in range(tatal_page):
+                self.__page_write_register(mem_offset, reset_vals)
+                mem_offset = mem_offset+page_size
+                time.sleep(PAGE_WRITE_CYCLE_TIME)
 
     def reset_edgepi_memory(self, bin_hash: str = None, bin_bytes: bytes = None):
         """
         reset edgepi reserved memory by reading default binary files. In order to trigger this
         method, correct md5sum hash must be passed.
         Args:
             bin_hash (str): md5sum hash string to compare with default eeprom hash
```

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/edgepi_eeprom_data.py` & `edgepi-python-sdk-1.2.8/src/edgepi/eeprom/edgepi_eeprom_data.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/eeprom_constants.py` & `edgepi-python-sdk-1.2.8/src/edgepi/eeprom/eeprom_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_adc_module.py` & `edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_adc_module.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_dac_module.py` & `edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_dac_module.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_key_module.py` & `edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_key_module.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_rtd_module.py` & `edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_rtd_module.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_tc_module.py` & `edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_tc_module.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/adc_module_pb2.py` & `edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/generated_pb2/adc_module_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/calibration_parameters_pb2.py` & `edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/generated_pb2/calibration_parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/dac_module_pb2.py` & `edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/generated_pb2/dac_module_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/edgepi_module_pb2.py` & `edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/generated_pb2/edgepi_module_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/keys_pb2.py` & `edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/generated_pb2/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/rtd_module_pb2.py` & `edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/generated_pb2/rtd_module_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/tc_module_pb2.py` & `edgepi-python-sdk-1.2.8/src/edgepi/eeprom/protobuf_assets/generated_pb2/tc_module_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/gpio/edgepi_gpio.py` & `edgepi-python-sdk-1.2.8/src/edgepi/gpio/edgepi_gpio.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/gpio/edgepi_gpio_chip.py` & `edgepi-python-sdk-1.2.8/src/edgepi/gpio/edgepi_gpio_chip.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,60 +35,55 @@
         object until close() method is called. So every time the state is read, it will instantiate
         before read and cloase() after read.
         Args:
             pin_name (str): name of the pin
         Returns:
             `bool`: True if state is high, False if state is low
         """
-        self.open_gpio(pin_num=self.__pin_name_dict[pin_name],
+        with self.open_gpio(pin_num=self.__pin_name_dict[pin_name],
                        pin_dir=self.gpiochip_pins_dict[pin_name].dir,
-                       pin_bias=self.gpiochip_pins_dict[pin_name].bias)
-        state = self.read_state()
-        self.close_gpio()
+                       pin_bias=self.gpiochip_pins_dict[pin_name].bias):
+            state = self.read_state()
         return state
 
     def write_gpio_pin_state(self, pin_name: str = None, state: bool = None):
         """
         write pin state
         Args:
             pin_name (str): name of the pin to write state to
             state (bool): state to write, True = High, False = Low
         Return:
             N/A
         """
-        self.open_gpio(pin_num=self.__pin_name_dict[pin_name],
+        with self.open_gpio(pin_num=self.__pin_name_dict[pin_name],
                        pin_dir=self.gpiochip_pins_dict[pin_name].dir,
-                       pin_bias=self.gpiochip_pins_dict[pin_name].bias)
-        self.write_state(state)
-        read_back = self.read_state()
-        self.close_gpio()
+                       pin_bias=self.gpiochip_pins_dict[pin_name].bias):
+            self.write_state(state)
+            read_back = self.read_state()
         return read_back
 
     def set_gpio_pin_dir(self, pin_name: str = None, direction: bool = None):
         """
         Set gpio pin direction
         Args:
             pin_name (str): name of the pin
             direction (bool): direction to write, True = Input, False = Output
         """
-        self.open_gpio(pin_num=self.__pin_name_dict[pin_name],
+        with self.open_gpio(pin_num=self.__pin_name_dict[pin_name],
                        pin_dir="in" if direction else "out",
-                       pin_bias=self.gpiochip_pins_dict[pin_name].bias)
-        self.close_gpio()
+                       pin_bias=self.gpiochip_pins_dict[pin_name].bias):
+            return self.gpio.direction
 
     def toggle_gpio_pin_state(self, pin_name: str = None):
         """
         Toggle pin state
         Args:
             pin_name (str): name of the pin to write state to
         Return:
             N/A
         """
-        self.open_gpio(pin_num=self.__pin_name_dict[pin_name],
+        with self.open_gpio(pin_num=self.__pin_name_dict[pin_name],
                        pin_dir=self.gpiochip_pins_dict[pin_name].dir,
-                       pin_bias=self.gpiochip_pins_dict[pin_name].bias)
-        state = self.read_state()
-        if state:
-            self.write_state(False)
-        else:
-            self.write_state(True)
-        self.close_gpio()
+                       pin_bias=self.gpiochip_pins_dict[pin_name].bias):
+            state = self.read_state()
+            self.write_state(not state)
+
```

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/gpio/edgepi_gpio_expander.py` & `edgepi-python-sdk-1.2.8/src/edgepi/gpio/edgepi_gpio_expander.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,37 +28,39 @@
         function to read one register value from an I2C device
         Args:
             `reg_address`: register/port address to read data from
             `dev_address`: expander address to read
         Returns:
             `int`: 8-bit uint value of port/register
         '''
-        msg_read = self.set_read_msg(reg_address, [0xFF])
-        _logger.debug(f"Read Message: Register Address {msg_read[0].data}"
-                      f", Msg Place Holder {msg_read[1].data}")
-        self.transfer(dev_address, msg_read)
-        _logger.debug(f"Message Read: Register Address {msg_read[0].data},"
-                      f"Msg Place Holder {msg_read[1].data}")
+        with self.i2c_open():
+            msg_read = self.set_read_msg(reg_address, [0xFF])
+            _logger.debug(f"Read Message: Register Address {msg_read[0].data}"
+                          f", Msg Place Holder {msg_read[1].data}")
+            self.transfer(dev_address, msg_read)
+            _logger.debug(f"Message Read: Register Address {msg_read[0].data},"
+                          f"Msg Place Holder {msg_read[1].data}")
         return msg_read[1].data[0]
 
     def __write_changed_values(self, reg_dict: dict, dev_address: int):
         '''
         Function to write changed values to the specified register
         In:
             reg_dict (dict): register address to value and is_changed flag
                              {register_address : {'value' : value(int), is_changed : bool}}
             dev_address: device address, 32 or 33
         Returns:
             void
         '''
-        for reg_addx, entry in reg_dict.items():
-            if entry['is_changed']:
-                msg_write = self.set_write_msg(reg_addx, [entry['value']])
-                _logger.debug(f'Write Message Content {msg_write[0]}')
-                self.transfer(dev_address, msg_write)
+        with self.i2c_open():
+            for reg_addx, entry in reg_dict.items():
+                if entry['is_changed']:
+                    msg_write = self.set_write_msg(reg_addx, [entry['value']])
+                    _logger.debug(f'Write Message Content {msg_write[0]}')
+                    self.transfer(dev_address, msg_write)
 
     def read_expander_pin(self, pin_name: str) -> bool:
         '''
         Get the current state of a GPIO expander pin (low or high).
 
         Args:
             `pin_name` (str): name of the pin whose state to read
```

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/gpio/gpio_configs.py` & `edgepi-python-sdk-1.2.8/src/edgepi/gpio/gpio_configs.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/gpio/gpio_constants.py` & `edgepi-python-sdk-1.2.8/src/edgepi/gpio/gpio_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/led/edgepi_leds.py` & `edgepi-python-sdk-1.2.8/src/edgepi/led/edgepi_leds.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/peripherals/i2c.py` & `edgepi-python-sdk-1.2.8/src/edgepi/peripherals/i2c.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,26 +3,43 @@
 
 Classes:
     I2CDevice
 """
 import logging
 
 from typing import Union
+from contextlib import contextmanager
 from periphery import I2C
 
 _logger = logging.getLogger(__name__)
 
 class I2CDevice():
     '''
     I2C Device class
     '''
     def __init__(self, fd: str = None):
-        self.fd = fd
-        _logger.debug(f"Initialized I2C device with path '{self.fd}'")
-        self.i2cdev = I2C(devpath=fd)
+        self.i2c_fd = fd
+        self.i2cdev = None
+
+    @contextmanager
+    def i2c_open(self):
+        """
+        Open I2C device
+        Attributes:
+            N/A
+        Return:
+            N/A
+        """
+        try:
+            self.i2cdev = I2C(devpath=self.i2c_fd)
+            _logger.debug(f"Open I2C device with path '{self.i2c_fd}'")
+            yield self.i2cdev
+        finally:
+            self.i2cdev.close()
+
 
     def set_read_msg(self, addr:Union[int,list] = None, msg:list = None):
         '''
         set Read message to be sent through I2C.
         Attributes:
             addr(int or list): Register address to read from
             Msg: list of place holder bytes
@@ -58,13 +75,7 @@
         Return:
             MsgList: list of message bytes if reading flag was set
         '''
         self.i2cdev.transfer(dev_addr, msg)
         if len(msg)>1:
             return msg[1].data
         return None
-
-    def close(self):
-        '''
-        Close I2C device
-        '''
-        self.i2cdev.close()
```

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/peripherals/pwm.py` & `edgepi-python-sdk-1.2.8/src/edgepi/peripherals/pwm.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/peripherals/spi.py` & `edgepi-python-sdk-1.2.8/src/edgepi/peripherals/spi.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 
 Classes:
     SpiDevice
 """
 
 
 import logging
-
+from contextlib import contextmanager
 from periphery import SPI
 
 
 _logger = logging.getLogger(__name__)
 
-# TODO: This class needs to be changed as the SPI library changes
 class SpiDevice:
     """Class representing an I2C device"""
 
     _devPath = "/dev/spidev"
 
     def __init__(
         self,
@@ -26,25 +25,38 @@
         mode: int = 1,
         max_speed: int = 1000000,
         bit_order: str = "msb",
         bits_per_word: int = 8,
         extra_flags: int = 0,
     ):
         self.devpath = f"/dev/spidev{bus_num}.{dev_id}"
-        _logger.debug(f"Initialized SPI device with path '{self.devpath}'")
-        self.spi = SPI(
-            self.devpath,
-            mode,
-            max_speed,
-            bit_order,
-            bits_per_word,
-            extra_flags,
-        )
+        self.mode = mode
+        self.max_speed = max_speed
+        self.bit_order = bit_order
+        self.bits_per_word = bits_per_word
+        self.extra_flags = extra_flags
+        self.spi = None
+
+    @contextmanager
+    def spi_open(self):
+        """
+        Open SPI device file
+        """
+        try:
+            self.spi = SPI(
+                self.devpath,
+                self.mode,
+                self.max_speed,
+                self.bit_order,
+                self.bits_per_word,
+                self.extra_flags,
+            )
+            _logger.debug(f"Open SPI device with path '{self.devpath}'")
+            yield self.spi
+        finally:
+            self.spi.close()
+
 
     def transfer(self, data: list) -> list:
         """Conduct an SPI data transfer"""
         out = self.spi.transfer(data)
         return out
-
-    def close(self):
-        """Close SPI connection"""
-        self.spi.close()
```

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/pwm/edgepi_pwm.py` & `edgepi-python-sdk-1.2.8/src/edgepi/pwm/edgepi_pwm.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,16 @@
         Args:
             pwm_num (PWMPins): target pwm device
         Returns:
             N/A
         """
         if pwm_num is None or pwm_num not in self.__pwm_devs:
             raise ValueError(f"get_enabled: PWM number is missing {pwm_num}")
-        return self.__pwm_devs[pwm_num].close_pwm()
+        self.__pwm_devs[pwm_num].close_pwm()
+        self.__pwm_devs[pwm_num] = None
 
     def __init_pwm_dev(self, pwm_num: PWMPins):
         self.__pwm_devs[pwm_num]=PwmDevice(channel=self.__pwm_pin_to_channel[pwm_num].value.channel,
                                            chip=self.__pwm_pin_to_channel[pwm_num].value.chip)
         self.__pwm_devs[pwm_num].open_pwm()
         self.log.debug(f"init_pwm: Instantiating PWM Device for the first time "
                        f"{self.__pwm_devs[pwm_num].chip}"
```

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/pwm/pwm_constants.py` & `edgepi-python-sdk-1.2.8/src/edgepi/pwm/pwm_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/reg_helper/reg_helper.py` & `edgepi-python-sdk-1.2.8/src/edgepi/reg_helper/reg_helper.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/relay/edgepi_relay.py` & `edgepi-python-sdk-1.2.8/src/edgepi/relay/edgepi_relay.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/tc/edgepi_tc.py` & `edgepi-python-sdk-1.2.8/src/edgepi/tc/edgepi_tc.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,16 @@
             reg_addx (TCAddress.Enum.value): the register's address
 
         Returns:
             a list containing two entries:
             new_data[0] = register address, new_data[1] = register value
         """
         data = [reg_addx] + [0xFF]
-        new_data = self.transfer(data)
+        with self.spi_open():
+            new_data = self.transfer(data)
         _logger.debug(f"__read_register: addx = {reg_addx} => data after xfer = {new_data}")
         return new_data
 
     def __read_registers(self, start_addx: int = 0, regs_to_read: int = 16):
         """read a variable number of registers sequentially
 
         Args:
@@ -266,29 +267,31 @@
             regs_to_read (int): number of registers to read, including starting register.
 
         Returns:
             a list containing register values starting from start_addx. Note, first entry
             is the start address: register values begin from the second entry.
         """
         data = [start_addx] + [0xFF] * regs_to_read
-        new_data = self.transfer(data)
+        with self.spi_open():
+            new_data = self.transfer(data)
         _logger.debug(f"__read_registers: shifted out data => {new_data}")
         return new_data
 
     def __write_to_register(self, reg_addx: int, value: int):
         """write a value to a register.
 
         Args:
             reg_addx (TCAddress.Enum.value): address of the register to write the value to.
 
             value (int): a values to be written to the register.
         """
         data = [reg_addx] + [value]
         _logger.debug(f"__write_to_registers: shifting in data => {data}")
-        self.transfer(data)
+        with self.spi_open():
+            self.transfer(data)
 
     def __read_registers_to_map(self):
         """
         Builds a map of write register address to corresponding read register value.
         Note, each register has a read and write address, but only the read address
         contains the register's value. Write addresses are only for writing.
```

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/tc/tc_commands.py` & `edgepi-python-sdk-1.2.8/src/edgepi/tc/tc_commands.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/tc/tc_constants.py` & `edgepi-python-sdk-1.2.8/src/edgepi/tc/tc_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/tc/tc_conv_time.py` & `edgepi-python-sdk-1.2.8/src/edgepi/tc/tc_conv_time.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/tc/tc_faults.py` & `edgepi-python-sdk-1.2.8/src/edgepi/tc/tc_faults.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/utilities/crc_8_atm.py` & `edgepi-python-sdk-1.2.8/src/edgepi/utilities/crc_8_atm.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi/utilities/utilities.py` & `edgepi-python-sdk-1.2.8/src/edgepi/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi_python_sdk.egg-info/PKG-INFO` & `edgepi-python-sdk-1.2.8/src/edgepi_python_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: edgepi-python-sdk
-Version: 1.2.6
+Version: 1.2.8
 Summary: EdgePi Python SDK package
 Home-page: https://github.com/EdgePi-Cloud/edgepi-python-sdk
 Author: S.Park
 Author-email: spark@osensa.com
 Project-URL: Bug Tracker, https://github.com/EdgePi-Cloud/edgepi-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-periphery>=2.3.0
+Requires-Dist: bitstring>=3.1.9
+Requires-Dist: protobuf>=3.20
 
 ![Image](https://user-images.githubusercontent.com/3793563/207438826-bb656ca5-f19d-4699-8cb4-35acccb2ce58.svg)
 
 EdgePi is a DIN rail-mounted, Raspberry Pi 4 industrial PC with the features of a Programmable Logic Controller (PLC), and Internet of Things (IoT) cloud edge device. Visit [edgepi.com](https://www.edgepi.com) for more information.
 
 ![](https://github.com/EdgePi-Cloud/edgepi-python-sdk/actions/workflows/python-unit-test.yml/badge.svg)
 ![](https://github.com/EdgePi-Cloud/edgepi-python-sdk/actions/workflows/python-lint.yml/badge.svg)
```

### Comparing `edgepi-python-sdk-1.2.6/src/edgepi_python_sdk.egg-info/SOURCES.txt` & `edgepi-python-sdk-1.2.8/src/edgepi_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_adc/test_adc.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_adc/test_adc.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_adc/test_adc_state.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_adc/test_adc_state.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_dac/test_dac.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_dac/test_dac.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_digital_in/test_digital_in.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_digital_in/test_digital_in.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_digital_out/test_digital_out.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_digital_out/test_digital_out.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_eeprom/test_eeprom.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_eeprom/test_eeprom.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,23 +30,24 @@
                         [
                          (list(range(0,64)),0),
                          (list(range(64,128)),64),
                         ])
 # pylint: disable=protected-access
 def test__page_write_register(data, address, eeprom):
     addrx = EdgePiMemoryInfo.USER_SPACE_START_BYTE.value + address
-    initial_data = eeprom._EdgePiEEPROM__sequential_read(addrx,len(data))
-    eeprom._EdgePiEEPROM__page_write_register(addrx, data)
-    time.sleep(0.5)
-    new_data = eeprom._EdgePiEEPROM__sequential_read(addrx,len(data))
-    time.sleep(0.5)
-    eeprom._EdgePiEEPROM__page_write_register(addrx, [255]*len(data))
-    _logger.info(f"data to write = {data}")
-    _logger.info(f"initial data  = {initial_data}")
-    _logger.info(f"new data      = {new_data}")
+    with eeprom.i2c_open():
+        initial_data = eeprom._EdgePiEEPROM__sequential_read(addrx,len(data))
+        eeprom._EdgePiEEPROM__page_write_register(addrx, data)
+        time.sleep(0.5)
+        new_data = eeprom._EdgePiEEPROM__sequential_read(addrx,len(data))
+        time.sleep(0.5)
+        eeprom._EdgePiEEPROM__page_write_register(addrx, [255]*len(data))
+        _logger.info(f"data to write = {data}")
+        _logger.info(f"initial data  = {initial_data}")
+        _logger.info(f"new data      = {new_data}")
     for indx, init_data in enumerate(initial_data):
         assert init_data != new_data[indx]
         assert new_data[indx] == data[indx]
 
 DUMMY_KEY = '-----BEGIN RSA PRIVATE KEY-----\nMIIEpQIBAAKCAQEAnwu+S/OI3Hl0BCNQASv0HU5Jc4KUT2X4/tLyk\
 Qcd6pE\nv7fji6ZoW/dl8dKwwdi/cfSS/J5Iv+5FwQU4KGNBbhVAnmJeLd+PMUT4bQTf9rVF\nHsDoIPoQLDH7jmBu8ai7jQ0hY\
 5SqPbynPGELFrk/vEpHwg/8fO4lbw1YxwgGc0SR\n8k1tFdi4On7NymBiv88HOsrrziAPGCd7Hc07s+SdFQF+nDPidyM1pMqvUC\
```

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_gpio/test_gpio.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_gpio/test_gpio.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_led/test_led.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_led/test_led.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_peripherals/test_i2c.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_peripherals/test_i2c.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ integration tests for peripherals/i2c.py """
 
-
+from contextlib import nullcontext as does_not_raise
 import pytest
 from edgepi.peripherals.i2c import I2CDevice
 
 
 @pytest.mark.parametrize(
     "fd",
     [
@@ -14,25 +14,34 @@
         ("/dev/i2c-20"),
         ("/dev/i2c-21"),
         ("/dev/i2c-22"),
     ],
 )
 def test_i2c_init_param(fd):
     i2c_device = I2CDevice(fd)
-    assert i2c_device.fd == fd
+    assert i2c_device.i2c_fd == fd
 
 
 @pytest.mark.parametrize(
     "addrx, data",
     [
         (32, [46]),
         ([32,24], [46]),
         ([64, 2], [2,3,4,5,6,7,8,9,10])
     ]
 )
 def test_i2c_set_write_msg(addrx, data):
     i2c_device = I2CDevice("/dev/i2c-0")
-    msg = i2c_device.set_write_msg(addrx, data)
-    if isinstance(addrx, int):
-        assert msg[0].data == [addrx]+data
-    else:
-        assert msg[0].data == addrx+data
+    with i2c_device.i2c_open():
+        msg = i2c_device.set_write_msg(addrx, data)
+        if isinstance(addrx, int):
+            assert msg[0].data == [addrx]+data
+        else:
+            assert msg[0].data == addrx+data
+
+def test_file_descriptor_open():
+    with does_not_raise():
+        i2c_devices = [0]*2048
+        for i2cdev in i2c_devices:
+            i2cdev = I2CDevice("/dev/i2c-10")
+            with i2cdev.i2c_open():
+                pass
```

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_pwm/test_edgepi_pwm.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_pwm/test_edgepi_pwm.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_relay/test_relay.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_relay/test_relay.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_tc/test_tc.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/integration_tests/test_tc/test_tc.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     VoltageMode,
 )
 from edgepi.tc.tc_faults import FaultType
 
 
 def test_tc_init():
     tc = EdgePiTC()
-    assert tc.spi.devpath == f"/dev/spidev{6}.{2}"
+    assert tc.devpath == f"/dev/spidev{6}.{2}"
 
 
 @pytest.fixture(name="tc")
 def fixture_test_edgepi_tc():
     return EdgePiTC()
```

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_commands.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_adc/test_adc_commands.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_conv_time.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_adc/test_adc_conv_time.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_multiplexers.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_adc/test_adc_multiplexers.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_state.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_adc/test_adc_state.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_status.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_adc/test_adc_status.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_voltage.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_adc/test_adc_voltage.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_edgepi_adc.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_adc/test_edgepi_adc.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_calibration/test_edgepi_calibration.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_calibration/test_edgepi_calibration.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_calibration/test_protobuf_mapping.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_calibration/test_protobuf_mapping.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_dac/test_dac_commands.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_dac/test_dac_commands.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_dac/test_edgepi_dac.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_dac/test_edgepi_dac.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_din/test_edgepi_din.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_din/test_edgepi_din.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_dout/test_edgepi_dout.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_dout/test_edgepi_dout.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_eeprom/test_access_eeprom.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_eeprom/test_access_eeprom.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,16 +77,18 @@
 
 @pytest.mark.parametrize("reg_addr, length, mock_val, result", [(1, 5,
                                                                 [23, 34, 56, 7, 8],
                                                                 [23, 34, 56, 7, 8])])
 def test_sequential_read(mocker, eeprom, reg_addr, length, mock_val, result):
     mocker.patch("edgepi.peripherals.i2c.I2CDevice.transfer",return_value = mock_val)
     # pylint: disable=protected-access
-    read_result = eeprom._EdgePiEEPROM__sequential_read( reg_addr, length)
+    with eeprom.i2c_open():
+        read_result = eeprom._EdgePiEEPROM__sequential_read( reg_addr, length)
     assert read_result == result
+    assert eeprom.i2cdev.close.called_once()
 
 @pytest.mark.parametrize("mock_value,result",
                         [([0,123], 123),
                          ([1,1], 257),
                          ([63,255], 16383),
                          ([63, 0], 16128)
                         ])
@@ -95,14 +97,16 @@
     data = get_crc(data)
     # pylint: disable=protected-access
     mocker.patch("edgepi.eeprom.edgepi_eeprom.EdgePiEEPROM._EdgePiEEPROM__sequential_read",
                 return_value =data)
     # pylint: disable=protected-access
     length = eeprom._EdgePiEEPROM__allocated_memory(EdgePiMemoryInfo.USED_SPACE.value)
     assert length == result
+    assert eeprom.i2cdev.close.called_once()
+
 
 def test__read_edgepi_reserved_memory(mocker, eeprom):
     data_b = read_binfile()
     # pylint: disable=protected-access
     data_l = eeprom._EdgePiEEPROM__generate_data_list(data_b)
     # pylint: disable=protected-access
     pages = eeprom._EdgePiEEPROM__generate_list_of_pages_crc(data_l)
@@ -111,14 +115,17 @@
     mocker.patch("edgepi.eeprom.edgepi_eeprom.EdgePiEEPROM._EdgePiEEPROM__allocated_memory",
                  return_value = (data_l[0]<<8) + data_l[1])
     mocker.patch("edgepi.eeprom.edgepi_eeprom.EdgePiEEPROM._EdgePiEEPROM__sequential_read",
                 side_effect = list(pages))
     # pylint: disable=protected-access
     byte_string = eeprom._EdgePiEEPROM__read_edgepi_reserved_memory()
     assert byte_string == data_b
+    # expected call count of close is one due to the mocked __allocated_memory
+    assert eeprom.i2cdev.close.called_once()
+
 
 dac_dict_calib = {0:CalibParam(gain = 1.0229951270016944, offset= -0.01787674545454656),
                   1:CalibParam(gain = 1.0233775195153139, offset= -0.019239763636362414),
                   2:CalibParam(gain = 1.0238480841375301, offset= -0.014646763636360628),
                   3:CalibParam(gain = 1.021600135, offset= -0.0190202),
                   4:CalibParam(gain = 1.022255745463092, offset= -0.0165660727272739),
                   5:CalibParam(gain = 1.0229838854579036, offset= -0.017047454545456923),
@@ -255,14 +262,15 @@
     pages = eeprom._EdgePiEEPROM__generate_list_of_pages_crc(dummy_data_l)
     mocker.patch(
         "edgepi.eeprom.edgepi_eeprom.EdgePiEEPROM._EdgePiEEPROM__sequential_read",
         side_effect = pages)
     data_size = (dummy_data_l[0]<<8) + dummy_data_l[1]
     result = eeprom.read_user_space(data_size)
     assert result == list(dummy_data_b)
+    assert eeprom.i2cdev.close.called_once()
 
 @pytest.mark.parametrize("mem_size, dummy_size, result, error",
                         [(3, 3,[False, False], does_not_raise()),
                          (512, 512, [False, False], does_not_raise()),
                          (0x3FFF, 0, [True, False], pytest.raises(ValueError)),
                          (0x3FFC, 5460, [True, False], does_not_raise()),
                          (0xFFFF, 0, [False, True], does_not_raise()),
```

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_eeprom/test_edgepi_eeprom_data.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_eeprom/test_edgepi_eeprom_data.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio_expander.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio_expander.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,25 +33,51 @@
                         [(32, 255),
                          (33, 255),
                          (33, 255),
                          (32, 255),
                         ])
 @patch('edgepi.gpio.edgepi_gpio.EdgePiGPIOExpander.set_read_msg')
 @patch('edgepi.gpio.edgepi_gpio.EdgePiGPIOExpander.transfer')
+# pylint: disable=no-member
+# pylint: disable=unused-argument
 def test_edgepi_expander_read_register(mock_data, mock_msg, dev_address, out, mock_i2c):
-    mock_i2c.return_value = None
     mock_msg.data = [255]
     mock_msg.return_value = (mock_msg ,mock_msg)
     mock_data.return_value = out
     gpio_ctrl = EdgePiGPIOExpander()
     out_data = gpio_ctrl._EdgePiGPIOExpander__read_register(7,
                                                             dev_address)
     assert out_data == out
+    mock_msg.assert_called_once()
+    mock_data.assert_called_once()
+    gpio_ctrl.i2cdev.close.assert_called_once()
+
+@pytest.mark.parametrize("dev_address, reg_dict",
+                        [(32, {7:{"value":255, "is_changed":True}}),
+                         (33, {7:{"value":255, "is_changed":False}}),
+                         (33, {6:{"value":255, "is_changed":True}}),
+                         (32, {6:{"value":255, "is_changed":False}}),
+                        ])
+@patch('edgepi.gpio.edgepi_gpio.EdgePiGPIOExpander.set_write_msg')
+@patch('edgepi.gpio.edgepi_gpio.EdgePiGPIOExpander.transfer')
+# pylint: disable=no-member
+# pylint: disable=unused-argument
+def test_edgepi_expander__write_changed_values(mock_data, mock_msg, dev_address, reg_dict,mock_i2c):
+    gpio_ctrl = EdgePiGPIOExpander()
+    gpio_ctrl._EdgePiGPIOExpander__write_changed_values(reg_dict,
+                                                            dev_address)
+    for reg_addx, entry in reg_dict.items():
+        if entry["is_changed"]:
+            mock_msg.assert_called_once_with(reg_addx, [entry["value"]])
+            mock_data.assert_called_once()
+        else:
+            assert mock_msg.call_count == 0
+            assert mock_data.call_count == 0
+    gpio_ctrl.i2cdev.close.assert_called_once()
 
-# TODO: these need to be refactored to work with new methods
 @pytest.mark.parametrize("pin_name, mock_value, result",
                          [(DACPins.AO_EN1.value, 170, True),
                           (DACPins.AO_EN2.value, 170, False),
                           (DACPins.AO_EN3.value, 170, True),
                           (DACPins.AO_EN4.value, 170, False),
                           (DACPins.AO_EN5.value, 170, True),
                           (DACPins.AO_EN6.value, 170, False),
```

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/test_gpio_config.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_gpio/test_gpio_config.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/test_gpio_constants.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_gpio/test_gpio_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_peripherals/test_gpio.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_peripherals/test_gpio.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,17 +13,25 @@
     [
         ("/dev/gpiochip0", 27, "in", "pull_down"),
     ],
 )
 def test_gpio_init_param(mocker, fd):
     mocker.patch("edgepi.peripherals.gpio.GPIO")
     gpio = GpioDevice(fd)
-    assert gpio.fd == fd
+    assert gpio.gpio_fd == fd
     assert gpio.gpio is None
 
+# pylint: disable=no-member
+def test_gpio_open(mocker):
+    periph_gpio = mocker.patch("edgepi.peripherals.gpio.GPIO")
+    gpiodev = GpioDevice("/dev/gpiochip0")
+    with gpiodev.open_gpio("DIN1","IN","Pull-down"):
+        assert periph_gpio.called_once()
+    gpiodev.gpio.close.assert_called_once()
+
 @pytest.mark.parametrize(
     "fd, result",
     [
         ("/dev/gpiochip0", True),
         ("/dev/gpiochip0", False),
         ("/dev/gpiochip0",True),
         ("/dev/gpiochip0", False),
```

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_peripherals/test_pwm.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_peripherals/test_pwm.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_pwm/test_edgepi_pwm.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_pwm/test_edgepi_pwm.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,16 @@
                           (None, pytest.raises(ValueError)),
                           ])
 def test_pwm_close(mocker, pwm_num, error, pwm_dev):
     mock_pwmdevice= mocker.patch("edgepi.peripherals.pwm.PwmDevice")
     pwm_dev._EdgePiPWM__pwm_devs[pwm_num] = mock_pwmdevice
     with error:
         pwm_dev.close(pwm_num)
-        pwm_dev._EdgePiPWM__pwm_devs[pwm_num].close_pwm.assert_called_once()
+        mock_pwmdevice.close_pwm.assert_called_once()
+        assert pwm_dev._EdgePiPWM__pwm_devs[pwm_num] is None
 
 
 @pytest.mark.parametrize("pwm_num ,expected, error",
                          [(PWMPins.PWM1, 1000.0, does_not_raise()),
                           (PWMPins.PWM1, 5000.0, does_not_raise()),
                           (PWMPins.PWM1, 10000.0, does_not_raise()),
                           (PWMPins.PWM2, 1000.0, does_not_raise()),
```

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_reg_helper/test_reg_helper.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_reg_helper/test_reg_helper.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_relay/test_relay.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_relay/test_relay.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_tc/test_edgepi_tc.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_tc/test_edgepi_tc.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_tc/test_tc_commands.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_tc/test_tc_commands.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_tc/test_tc_conv_time.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_tc/test_tc_conv_time.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_tc/test_tc_faults.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_tc/test_tc_faults.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_utilities/test_crc_8_atm.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_utilities/test_crc_8_atm.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_utilities/test_utilities.py` & `edgepi-python-sdk-1.2.8/src/test_edgepi/unit_tests/test_utilities/test_utilities.py`

 * *Files identical despite different names*

