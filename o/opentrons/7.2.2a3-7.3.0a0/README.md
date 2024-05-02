# Comparing `tmp/opentrons-7.2.2a3.tar.gz` & `tmp/opentrons-7.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentrons-7.2.2a3.tar", last modified: Mon Apr  8 17:03:53 2024, max compression
+gzip compressed data, was "opentrons-7.3.0a0.tar", last modified: Thu May  2 12:13:44 2024, max compression
```

## Comparing `opentrons-7.2.2a3.tar` & `opentrons-7.3.0a0.tar`

### file list

```diff
@@ -1,542 +1,554 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.061577 opentrons-7.2.2a3/
--rwxr-xr-x   0 runner    (1001) docker     (127)       80 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-08 17:03:53.061577 opentrons-7.2.2a3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     7455 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)      158 2024-04-08 17:03:53.061577 opentrons-7.2.2a3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3631 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:52.973579 opentrons-7.2.2a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:52.981578 opentrons-7.2.2a3/src/opentrons/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4551 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:52.985578 opentrons-7.2.2a3/src/opentrons/calibration_storage/
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/deck_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/file_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:52.985578 opentrons-7.2.2a3/src/opentrons/calibration_storage/ot2/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/ot2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/ot2/deck_attitude.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/ot2/mark_bad_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:52.985578 opentrons-7.2.2a3/src/opentrons/calibration_storage/ot2/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/ot2/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/ot2/models/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/ot2/models/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/ot2/pipette_offset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9715 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/ot2/tip_length.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:52.985578 opentrons-7.2.2a3/src/opentrons/calibration_storage/ot3/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/ot3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/ot3/deck_attitude.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/ot3/gripper_offset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:52.985578 opentrons-7.2.2a3/src/opentrons/calibration_storage/ot3/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/ot3/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/ot3/models/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/ot3/models/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/ot3/module_offset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/ot3/pipette_offset.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/calibration_storage/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:52.985578 opentrons-7.2.2a3/src/opentrons/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/cli/analyze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:52.989578 opentrons-7.2.2a3/src/opentrons/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/commands/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9005 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/commands/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/commands/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/commands/module_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/commands/protocol_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/commands/publisher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23582 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/commands/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:52.989578 opentrons-7.2.2a3/src/opentrons/config/
--rw-r--r--   0 runner    (1001) docker     (127)    20571 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24616 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/config/advanced_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/config/defaults_ot2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14026 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/config/defaults_ot3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/config/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/config/gripper_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/config/reset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6094 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/config/robot_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/config/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:52.989578 opentrons-7.2.2a3/src/opentrons/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:52.989578 opentrons-7.2.2a3/src/opentrons/drivers/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/asyncio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:52.989578 opentrons-7.2.2a3/src/opentrons/drivers/asyncio/communication/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/asyncio/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/asyncio/communication/async_serial.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/asyncio/communication/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    15405 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/asyncio/communication/serial_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/command_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:52.993578 opentrons-7.2.2a3/src/opentrons/drivers/heater_shaker/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/heater_shaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/heater_shaker/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/heater_shaker/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/heater_shaker/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:52.993578 opentrons-7.2.2a3/src/opentrons/drivers/mag_deck/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/mag_deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/mag_deck/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     6440 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/mag_deck/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/mag_deck/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:52.993578 opentrons-7.2.2a3/src/opentrons/drivers/rpi_drivers/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1078 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/rpi_drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/rpi_drivers/dev_types.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9573 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/rpi_drivers/gpio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/rpi_drivers/gpio_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/rpi_drivers/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/rpi_drivers/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/rpi_drivers/usb.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/rpi_drivers/usb_simulator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4592 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/serial_communication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:52.993578 opentrons-7.2.2a3/src/opentrons/drivers/smoothie_drivers/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/smoothie_drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/smoothie_drivers/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/smoothie_drivers/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    76707 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/smoothie_drivers/driver_3_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/smoothie_drivers/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/smoothie_drivers/parse_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/smoothie_drivers/simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/smoothie_drivers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:52.993578 opentrons-7.2.2a3/src/opentrons/drivers/temp_deck/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/temp_deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/temp_deck/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/temp_deck/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/temp_deck/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:52.997578 opentrons-7.2.2a3/src/opentrons/drivers/thermocycler/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/thermocycler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/thermocycler/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    13100 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/thermocycler/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/thermocycler/simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/drivers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    28659 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/execute.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.001578 opentrons-7.2.2a3/src/opentrons/hardware_control/
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)    48650 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.001578 opentrons-7.2.2a3/src/opentrons/hardware_control/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/backends/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/backends/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/backends/estop_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/backends/flex_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    57013 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/backends/ot3controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    27159 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/backends/ot3simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21150 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/backends/ot3utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/backends/simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/backends/status_bar_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    16484 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/backends/subsystem_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/backends/tip_presence_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/backends/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/dev_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.005578 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/abstract_emulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/connection_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/heater_shaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/magdeck.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.005578 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/module_server/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/module_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/module_server/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/module_server/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/module_server/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/module_server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/run_emulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.005578 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/scripts/run_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/scripts/run_module_emulator.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/scripts/run_smoothie.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/simulations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/smoothie.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/tempdeck.py
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/thermocycler.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/execution_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.005578 opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/instrument_abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/instrument_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.005578 opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/ot2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/ot2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/ot2/instrument_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)    26329 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/ot2/pipette.py
--rw-r--r--   0 runner    (1001) docker     (127)    38839 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/ot2/pipette_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.009578 opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/ot3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/ot3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13566 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/ot3/gripper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/ot3/gripper_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/ot3/instrument_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)    29115 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/ot3/pipette.py
--rw-r--r--   0 runner    (1001) docker     (127)    35820 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/ot3/pipette_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/module_control.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.009578 opentrons-7.2.2a3/src/opentrons/hardware_control/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/modules/heater_shaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/modules/lid_temp_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/modules/magdeck.py
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/modules/mod_abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/modules/module_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/modules/plate_temp_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/modules/tempdeck.py
--rw-r--r--   0 runner    (1001) docker     (127)    22324 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/modules/thermocycler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/modules/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/modules/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/modules/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/motion_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    15337 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/nozzle_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    44753 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/ot3_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)   105753 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/ot3api.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/pause_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/poller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.013578 opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/asyncio_configurable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/calibratable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/chassis_accessory_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/configurable.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/event_sourcer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/execution_controllable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/flex_calibratable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/flex_instrument_configurer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/gripper_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/hardware_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/identifiable.py
--rw-r--r--   0 runner    (1001) docker     (127)     7232 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/instrument_configurer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/liquid_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/module_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     9415 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/motion_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/simulatable.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/stoppable.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/robot_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.013578 opentrons-7.2.2a3/src/opentrons/hardware_control/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/scripts/gripper_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/scripts/repl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/simulator_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    15528 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/thread_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/threaded_async_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    20754 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/hardware_control/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/legacy_broker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.013578 opentrons-7.2.2a3/src/opentrons/motion_planning/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/motion_planning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/motion_planning/adjacent_slots_getters.py
--rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/motion_planning/deck_conflict.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/motion_planning/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/motion_planning/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/motion_planning/waypoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/ordered_set.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.017578 opentrons-7.2.2a3/src/opentrons/protocol_api/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/_liquid.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/_nozzle_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/_trash_bin.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/_waste_chute.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.017578 opentrons-7.2.2a3/src/opentrons/protocol_api/core/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/core_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.021578 opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24501 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/deck_conflict.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    29514 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/labware.py
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/load_labware_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    18722 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/module_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/point_calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)    29187 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/stringify.py
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/well.py
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/labware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.021578 opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/deck.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/labware_offset_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    20470 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/legacy_instrument_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/legacy_labware_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    23111 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/legacy_module_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    21097 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/legacy_protocol_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/legacy_well_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/load_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    20890 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/module_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/well_geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.021578 opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy_simulator/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy_simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17143 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy_simulator/legacy_instrument_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy_simulator/legacy_protocol_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/well.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/core/well_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/create_protocol_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/deck.py
--rw-r--r--   0 runner    (1001) docker     (127)    79370 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/instrument_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    44613 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/labware.py
--rw-r--r--   0 runner    (1001) docker     (127)    35944 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/module_contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/module_validation_and_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    49985 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/protocol_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    18022 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_api/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.025578 opentrons-7.2.2a3/src/opentrons/protocol_engine/
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.025578 opentrons-7.2.2a3/src/opentrons/protocol_engine/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/actions/action_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/actions/action_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/actions/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.025578 opentrons-7.2.2a3/src/opentrons/protocol_engine/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33525 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/clients/sync_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/clients/transports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.033578 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/
--rw-r--r--   0 runner    (1001) docker     (127)    13122 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/aspirate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/aspirate_in_place.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/blow_out.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/blow_out_in_place.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.033578 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/calibration/
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/calibration/calibrate_gripper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/calibration/calibrate_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/calibration/calibrate_pipette.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/calibration/move_to_maintenance_position.py
--rw-r--r--   0 runner    (1001) docker     (127)     7865 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (127)    16112 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/command_unions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/configure_for_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/configure_nozzle_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/configuring_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/dispense.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/dispense_in_place.py
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/drop_tip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/drop_tip_in_place.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/generate_command_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/get_tip_presence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/hash_command_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.033578 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/heater_shaker/
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/heater_shaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/heater_shaker/close_labware_latch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/heater_shaker/deactivate_heater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/heater_shaker/deactivate_shaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/heater_shaker/open_labware_latch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/heater_shaker/set_and_wait_for_shake_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/heater_shaker/set_target_temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/heater_shaker/wait_for_temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/home.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/load_labware.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/load_liquid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/load_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/load_pipette.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.033578 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/magnetic_module/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/magnetic_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/magnetic_module/disengage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/magnetic_module/engage.py
--rw-r--r--   0 runner    (1001) docker     (127)     9850 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/move_labware.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/move_relative.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/move_to_addressable_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/move_to_addressable_area_for_drop_tip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/move_to_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/move_to_well.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/pick_up_tip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/pipetting_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/prepare_to_aspirate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/retract_axis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/save_position.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/set_rail_lights.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/set_status_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.033578 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/temperature_module/
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/temperature_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/temperature_module/deactivate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/temperature_module/set_target_temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/temperature_module/wait_for_temperature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.037578 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/thermocycler/
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/thermocycler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/thermocycler/close_lid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/thermocycler/deactivate_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/thermocycler/deactivate_lid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/thermocycler/open_lid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/thermocycler/run_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/thermocycler/set_target_block_temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/thermocycler/set_target_lid_temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/thermocycler/wait_for_block_temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/thermocycler/wait_for_lid_temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/touch_tip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/verify_tip_presence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/wait_for_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/wait_for_resume.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/create_protocol_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.037578 opentrons-7.2.2a3/src/opentrons/protocol_engine/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/errors/error_occurrence.py
--rw-r--r--   0 runner    (1001) docker     (127)    34377 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/errors/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.041578 opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/command_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/create_queue_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/door_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    21357 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/equipment.py
--rw-r--r--   0 runner    (1001) docker     (127)    11585 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/gantry_mover.py
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/hardware_stopper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9287 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/heater_shaker_movement_flagger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9832 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/labware_movement.py
--rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/movement.py
--rw-r--r--   0 runner    (1001) docker     (127)    11663 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/pipetting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/queue_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/rail_lights.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/run_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/status_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/thermocycler_movement_flagger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/thermocycler_plate_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12497 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/tip_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    23623 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/protocol_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.041578 opentrons-7.2.2a3/src/opentrons/protocol_engine/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/resources/deck_configuration_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/resources/deck_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/resources/fixture_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/resources/labware_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/resources/labware_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/resources/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/resources/module_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/resources/ot3_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10078 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/resources/pipette_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/slot_standardization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.045578 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/abstract_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    24674 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/addressable_areas.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/change_notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    27929 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    47318 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    36822 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/labware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/liquids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.045578 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/module_substates/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/module_substates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/module_substates/heater_shaker_module_substate.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/module_substates/magnetic_block_substate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/module_substates/magnetic_module_substate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/module_substates/temperature_module_substate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/module_substates/thermocycler_module_substate.py
--rw-r--r--   0 runner    (1001) docker     (127)    42533 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    13955 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/motion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/move_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    29494 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/pipettes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11505 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/state.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/state_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/state/tips.py
--rw-r--r--   0 runner    (1001) docker     (127)    26461 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_engine/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.049578 opentrons-7.2.2a3/src/opentrons/protocol_reader/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_reader/extract_labware_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_reader/file_format_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_reader/file_hasher.py
--rw-r--r--   0 runner    (1001) docker     (127)     9465 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_reader/file_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_reader/file_reader_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_reader/input_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_reader/protocol_files_invalid_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_reader/protocol_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_reader/protocol_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_reader/role_analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.049578 opentrons-7.2.2a3/src/opentrons/protocol_runner/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_runner/create_simulating_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_runner/json_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10178 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_runner/json_translator.py
--rw-r--r--   0 runner    (1001) docker     (127)    27719 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_runner/legacy_command_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_runner/legacy_context_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_runner/legacy_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16089 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_runner/protocol_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_runner/task_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocol_runner/thread_async_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.049578 opentrons-7.2.2a3/src/opentrons/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.049578 opentrons-7.2.2a3/src/opentrons/protocols/advanced_control/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/advanced_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/advanced_control/mix.py
--rw-r--r--   0 runner    (1001) docker     (127)    36651 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/advanced_control/transfers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.053578 opentrons-7.2.2a3/src/opentrons/protocols/api_support/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/api_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/api_support/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/api_support/deck_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/api_support/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/api_support/instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/api_support/labware_like.py
--rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/api_support/tip_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/api_support/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/api_support/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/bundle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.053578 opentrons-7.2.2a3/src/opentrons/protocols/duration/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/duration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/duration/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    23295 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/duration/estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.053578 opentrons-7.2.2a3/src/opentrons/protocols/execution/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/execution/dev_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/execution/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/execution/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/execution/execute_json_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/execution/execute_json_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/execution/execute_json_v5.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/execution/execute_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/execution/json_dispatchers.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/execution/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.053578 opentrons-7.2.2a3/src/opentrons/protocols/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/geometry/labware_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10925 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/geometry/planning.py
--rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/labware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.053578 opentrons-7.2.2a3/src/opentrons/protocols/models/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20240 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/models/json_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/protocols/types.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.053578 opentrons-7.2.2a3/src/opentrons/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.057577 opentrons-7.2.2a3/src/opentrons/resources/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)   329864 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/resources/scripts/lpc21isp
--rw-r--r--   0 runner    (1001) docker     (127)  1035222 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/resources/smoothie-edge-8414642.hex
--rw-r--r--   0 runner    (1001) docker     (127)    40057 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/simulate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.057577 opentrons-7.2.2a3/src/opentrons/system/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/system/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/system/log_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    30317 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/system/nmcli.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/system/resin.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/system/smoothie_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/system/wifi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.057577 opentrons-7.2.2a3/src/opentrons/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/tools/args_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/tools/write_pipette_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    12280 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.061577 opentrons-7.2.2a3/src/opentrons/util/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/util/async_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/util/broker.py
--rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/util/entrypoint_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/util/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/util/linal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-08 17:02:37.000000 opentrons-7.2.2a3/src/opentrons/util/logging_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:53.061577 opentrons-7.2.2a3/src/opentrons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-08 17:03:52.000000 opentrons-7.2.2a3/src/opentrons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24605 2024-04-08 17:03:52.000000 opentrons-7.2.2a3/src/opentrons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:03:52.000000 opentrons-7.2.2a3/src/opentrons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-08 17:03:52.000000 opentrons-7.2.2a3/src/opentrons.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:03:19.000000 opentrons-7.2.2a3/src/opentrons.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-08 17:03:52.000000 opentrons-7.2.2a3/src/opentrons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 17:03:52.000000 opentrons-7.2.2a3/src/opentrons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.224283 opentrons-7.3.0a0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       80 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-02 12:13:44.224283 opentrons-7.3.0a0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7455 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      158 2024-05-02 12:13:44.224283 opentrons-7.3.0a0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3542 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.124284 opentrons-7.3.0a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.132284 opentrons-7.3.0a0/src/opentrons/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4551 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.136284 opentrons-7.3.0a0/src/opentrons/calibration_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/deck_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/file_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.136284 opentrons-7.3.0a0/src/opentrons/calibration_storage/ot2/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/ot2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/ot2/deck_attitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/ot2/mark_bad_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.136284 opentrons-7.3.0a0/src/opentrons/calibration_storage/ot2/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/ot2/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/ot2/models/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/ot2/models/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/ot2/pipette_offset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9715 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/ot2/tip_length.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.140284 opentrons-7.3.0a0/src/opentrons/calibration_storage/ot3/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/ot3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/ot3/deck_attitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/ot3/gripper_offset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.140284 opentrons-7.3.0a0/src/opentrons/calibration_storage/ot3/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/ot3/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/ot3/models/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/ot3/models/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/ot3/module_offset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/ot3/pipette_offset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/calibration_storage/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.140284 opentrons-7.3.0a0/src/opentrons/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/cli/analyze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.140284 opentrons-7.3.0a0/src/opentrons/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    20909 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26456 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/config/advanced_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/config/defaults_ot2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15904 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/config/defaults_ot3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/config/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/config/gripper_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/config/reset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6094 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/config/robot_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/config/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.144284 opentrons-7.3.0a0/src/opentrons/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.144284 opentrons-7.3.0a0/src/opentrons/drivers/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/asyncio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.144284 opentrons-7.3.0a0/src/opentrons/drivers/asyncio/communication/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/asyncio/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/asyncio/communication/async_serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/asyncio/communication/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15405 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/asyncio/communication/serial_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/command_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.144284 opentrons-7.3.0a0/src/opentrons/drivers/heater_shaker/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/heater_shaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/heater_shaker/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/heater_shaker/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/heater_shaker/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.144284 opentrons-7.3.0a0/src/opentrons/drivers/mag_deck/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/mag_deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/mag_deck/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6440 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/mag_deck/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/mag_deck/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.148284 opentrons-7.3.0a0/src/opentrons/drivers/rpi_drivers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1078 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/rpi_drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/rpi_drivers/dev_types.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9573 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/rpi_drivers/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/rpi_drivers/gpio_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/rpi_drivers/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/rpi_drivers/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/rpi_drivers/usb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/rpi_drivers/usb_simulator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4592 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/serial_communication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.148284 opentrons-7.3.0a0/src/opentrons/drivers/smoothie_drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/smoothie_drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/smoothie_drivers/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/smoothie_drivers/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    76707 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/smoothie_drivers/driver_3_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/smoothie_drivers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/smoothie_drivers/parse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/smoothie_drivers/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/smoothie_drivers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.148284 opentrons-7.3.0a0/src/opentrons/drivers/temp_deck/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/temp_deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/temp_deck/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/temp_deck/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/temp_deck/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.148284 opentrons-7.3.0a0/src/opentrons/drivers/thermocycler/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/thermocycler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/thermocycler/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13100 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/thermocycler/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/thermocycler/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/drivers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28835 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/execute.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.152284 opentrons-7.3.0a0/src/opentrons/hardware_control/
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48713 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.156283 opentrons-7.3.0a0/src/opentrons/hardware_control/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/backends/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/backends/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/backends/estop_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11754 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/backends/flex_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60763 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/backends/ot3controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29210 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/backends/ot3simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21195 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/backends/ot3utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17305 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/backends/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/backends/status_bar_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16484 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/backends/subsystem_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5973 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/backends/tip_presence_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/backends/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/dev_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.160283 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/abstract_emulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/connection_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/heater_shaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/magdeck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.160283 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/module_server/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/module_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/module_server/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/module_server/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/module_server/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/module_server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/run_emulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.160283 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/scripts/run_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/scripts/run_module_emulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/scripts/run_smoothie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/simulations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/smoothie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/tempdeck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/thermocycler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/execution_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.160283 opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/instrument_abc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.160283 opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/ot2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/ot2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/ot2/instrument_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26349 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/ot2/pipette.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38795 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/ot2/pipette_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.164283 opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/ot3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/ot3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13706 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/ot3/gripper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/ot3/gripper_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/ot3/instrument_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29487 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/ot3/pipette.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35928 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/ot3/pipette_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/module_control.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.164283 opentrons-7.3.0a0/src/opentrons/hardware_control/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14704 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/modules/heater_shaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/modules/lid_temp_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/modules/magdeck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/modules/mod_abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/modules/module_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/modules/plate_temp_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/modules/tempdeck.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22406 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/modules/thermocycler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/modules/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/modules/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/modules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/motion_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15837 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/nozzle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44753 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/ot3_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108638 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/ot3api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/pause_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/poller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.168283 opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/asyncio_configurable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/calibratable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/chassis_accessory_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/configurable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/event_sourcer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/execution_controllable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/flex_calibratable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/flex_instrument_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/gripper_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/hardware_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/identifiable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/instrument_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/liquid_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/module_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9415 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/motion_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/simulatable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/stoppable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/robot_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.168283 opentrons-7.3.0a0/src/opentrons/hardware_control/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/scripts/gripper_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/scripts/repl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8690 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/simulator_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15528 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/thread_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/threaded_async_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20947 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/hardware_control/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/legacy_broker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.168283 opentrons-7.3.0a0/src/opentrons/legacy_commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/legacy_commands/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8966 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/legacy_commands/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/legacy_commands/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/legacy_commands/module_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/legacy_commands/protocol_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/legacy_commands/publisher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23539 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/legacy_commands/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.172283 opentrons-7.3.0a0/src/opentrons/motion_planning/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/motion_planning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/motion_planning/adjacent_slots_getters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/motion_planning/deck_conflict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/motion_planning/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/motion_planning/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/motion_planning/waypoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/ordered_set.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.176283 opentrons-7.3.0a0/src/opentrons/protocol_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/_liquid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/_nozzle_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9043 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/_parameter_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.176283 opentrons-7.3.0a0/src/opentrons/protocol_api/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/core_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.180283 opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24548 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/deck_conflict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30138 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/labware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/load_labware_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18722 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/module_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/point_calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29557 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/stringify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/well.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8407 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/labware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.180283 opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13963 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/deck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/labware_offset_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20960 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/legacy_instrument_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/legacy_labware_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23111 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/legacy_module_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21432 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/legacy_protocol_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/legacy_well_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/load_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20890 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/module_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/well_geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.180283 opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy_simulator/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy_simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17633 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy_simulator/legacy_instrument_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy_simulator/legacy_protocol_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/well.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/core/well_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/create_protocol_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/deck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/disposal_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82740 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/instrument_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46155 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/labware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36014 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/module_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/module_validation_and_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49434 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/protocol_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18136 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_api/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.184283 opentrons-7.3.0a0/src/opentrons/protocol_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.184283 opentrons-7.3.0a0/src/opentrons/protocol_engine/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/actions/action_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/actions/action_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/actions/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.184283 opentrons-7.3.0a0/src/opentrons/protocol_engine/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34969 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/clients/sync_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/clients/transports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.192283 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/aspirate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/aspirate_in_place.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/blow_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/blow_out_in_place.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.192283 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/calibration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/calibration/calibrate_gripper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/calibration/calibrate_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/calibration/calibrate_pipette.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/calibration/move_to_maintenance_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16401 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/command_unions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/configure_for_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/configure_nozzle_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/configuring_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/dispense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/dispense_in_place.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/drop_tip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/drop_tip_in_place.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/generate_command_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/get_tip_presence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/hash_command_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.196283 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/heater_shaker/
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/heater_shaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/heater_shaker/close_labware_latch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/heater_shaker/deactivate_heater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/heater_shaker/deactivate_shaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/heater_shaker/open_labware_latch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/heater_shaker/set_and_wait_for_shake_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/heater_shaker/set_target_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/heater_shaker/wait_for_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/home.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/load_labware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/load_liquid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/load_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/load_pipette.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.196283 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/magnetic_module/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/magnetic_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/magnetic_module/disengage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/magnetic_module/engage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9850 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/move_labware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/move_relative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/move_to_addressable_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/move_to_addressable_area_for_drop_tip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/move_to_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/move_to_well.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/pick_up_tip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/pipetting_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/prepare_to_aspirate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/reload_labware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/retract_axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/save_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/set_rail_lights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/set_status_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.196283 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/temperature_module/
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/temperature_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/temperature_module/deactivate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/temperature_module/set_target_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/temperature_module/wait_for_temperature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.196283 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/thermocycler/
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/thermocycler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/thermocycler/close_lid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/thermocycler/deactivate_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/thermocycler/deactivate_lid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/thermocycler/open_lid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/thermocycler/run_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/thermocycler/set_target_block_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/thermocycler/set_target_lid_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/thermocycler/wait_for_block_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/thermocycler/wait_for_lid_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/touch_tip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/verify_tip_presence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/wait_for_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/wait_for_resume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/create_protocol_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/error_recovery_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.196283 opentrons-7.3.0a0/src/opentrons/protocol_engine/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/errors/error_occurrence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35716 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/errors/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.200283 opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/command_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/create_queue_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/door_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22443 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/equipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11585 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/gantry_mover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/hardware_stopper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9287 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/heater_shaker_movement_flagger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9832 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/labware_movement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/movement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12702 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/pipetting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/queue_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/rail_lights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/run_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/status_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/thermocycler_movement_flagger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/thermocycler_plate_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12833 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/tip_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.200283 opentrons-7.3.0a0/src/opentrons/protocol_engine/notes/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/notes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/notes/notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26087 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/protocol_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.204283 opentrons-7.3.0a0/src/opentrons/protocol_engine/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/resources/deck_configuration_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/resources/deck_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/resources/fixture_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/resources/labware_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/resources/labware_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/resources/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/resources/module_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/resources/ot3_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9622 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/resources/pipette_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/slot_standardization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.208283 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/abstract_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26571 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/addressable_areas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/change_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/command_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36269 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49607 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37293 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/labware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/liquids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.208283 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/module_substates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/module_substates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/module_substates/heater_shaker_module_substate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/module_substates/magnetic_block_substate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/module_substates/magnetic_module_substate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/module_substates/temperature_module_substate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/module_substates/thermocycler_module_substate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47626 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13955 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/move_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29910 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/pipettes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12930 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/state_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22053 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/state/tips.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30665 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_engine/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.208283 opentrons-7.3.0a0/src/opentrons/protocol_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_reader/extract_labware_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_reader/file_format_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_reader/file_hasher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9465 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_reader/file_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_reader/file_reader_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_reader/input_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_reader/protocol_files_invalid_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7712 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_reader/protocol_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_reader/protocol_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_reader/role_analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.212283 opentrons-7.3.0a0/src/opentrons/protocol_runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_runner/create_simulating_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_runner/json_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10178 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_runner/json_translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33603 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_runner/legacy_command_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_runner/legacy_context_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_runner/legacy_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18304 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_runner/protocol_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_runner/task_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocol_runner/thread_async_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.212283 opentrons-7.3.0a0/src/opentrons/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.212283 opentrons-7.3.0a0/src/opentrons/protocols/advanced_control/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/advanced_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/advanced_control/mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36651 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/advanced_control/transfers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.216283 opentrons-7.3.0a0/src/opentrons/protocols/api_support/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/api_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/api_support/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/api_support/deck_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/api_support/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/api_support/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/api_support/labware_like.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/api_support/tip_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/api_support/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/api_support/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.216283 opentrons-7.3.0a0/src/opentrons/protocols/duration/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/duration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/duration/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23302 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/duration/estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.216283 opentrons-7.3.0a0/src/opentrons/protocols/execution/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/execution/dev_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/execution/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/execution/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/execution/execute_json_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/execution/execute_json_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/execution/execute_json_v5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/execution/execute_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/execution/json_dispatchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/execution/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.220283 opentrons-7.3.0a0/src/opentrons/protocols/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/geometry/labware_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10925 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/geometry/planning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/labware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.220283 opentrons-7.3.0a0/src/opentrons/protocols/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20240 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/models/json_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.220283 opentrons-7.3.0a0/src/opentrons/protocols/parameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8824 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/parameters/parameter_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/parameters/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/parameters/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/protocols/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.220283 opentrons-7.3.0a0/src/opentrons/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.220283 opentrons-7.3.0a0/src/opentrons/resources/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   329864 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/resources/scripts/lpc21isp
+-rw-r--r--   0 runner    (1001) docker     (127)  1035222 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/resources/smoothie-edge-8414642.hex
+-rw-r--r--   0 runner    (1001) docker     (127)    40613 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/simulate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.224283 opentrons-7.3.0a0/src/opentrons/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/system/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/system/log_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30317 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/system/nmcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/system/resin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/system/smoothie_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/system/wifi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.224283 opentrons-7.3.0a0/src/opentrons/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/tools/args_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/tools/write_pipette_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12280 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.224283 opentrons-7.3.0a0/src/opentrons/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/util/async_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/util/broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/util/entrypoint_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/util/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/util/linal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/util/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-02 12:12:45.000000 opentrons-7.3.0a0/src/opentrons/util/performance_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:44.224283 opentrons-7.3.0a0/src/opentrons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-02 12:13:44.000000 opentrons-7.3.0a0/src/opentrons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25146 2024-05-02 12:13:44.000000 opentrons-7.3.0a0/src/opentrons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:13:44.000000 opentrons-7.3.0a0/src/opentrons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 12:13:44.000000 opentrons-7.3.0a0/src/opentrons.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:13:13.000000 opentrons-7.3.0a0/src/opentrons.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-02 12:13:44.000000 opentrons-7.3.0a0/src/opentrons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 12:13:44.000000 opentrons-7.3.0a0/src/opentrons.egg-info/top_level.txt
```

### Comparing `opentrons-7.2.2a3/PKG-INFO` & `opentrons-7.3.0a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentrons
-Version: 7.2.2a3
+Version: 7.3.0a0
 Summary: The Opentrons API is a simple framework designed to make writing automated biology lab protocols easy.
 Author: Opentrons
 Author-email: engineering@opentrons.com
 Maintainer: Opentrons
 Maintainer-email: engineering@opentrons.com
 License: Apache 2.0
 Project-URL: opentrons.com, https://www.opentrons.com
@@ -13,34 +13,32 @@
 Keywords: robots,protocols,synbio,pcr,automation,lab
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 License-File: ../LICENSE
-Requires-Dist: opentrons-shared-data==7.2.2a3
+Requires-Dist: opentrons-shared-data==7.3.0a0
 Requires-Dist: aionotify==0.2.0
 Requires-Dist: anyio<4.0.0,>=3.6.1
 Requires-Dist: jsonschema<4.18.0,>=3.0.1
 Requires-Dist: numpy<2,>=1.20.0
 Requires-Dist: pydantic<2.0.0,>=1.10.9
 Requires-Dist: pyserial>=3.5
 Requires-Dist: typing-extensions<5,>=4.0.0
 Requires-Dist: click<9,>=8.0.0
 Requires-Dist: importlib-metadata>=1.0; python_version < "3.8"
 Provides-Extra: ot2-hardware
-Requires-Dist: opentrons-hardware==7.2.2a3; extra == "ot2-hardware"
+Requires-Dist: opentrons-hardware==7.3.0a0; extra == "ot2-hardware"
 Provides-Extra: flex-hardware
-Requires-Dist: opentrons-hardware[FLEX]==7.2.2a3; extra == "flex-hardware"
+Requires-Dist: opentrons-hardware[FLEX]==7.3.0a0; extra == "flex-hardware"
 
 .. _Full API Documentation: http://docs.opentrons.com
 
 The Opentrons API is a simple framework designed to make it easy to write automated biology lab protocols for Opentrons robots.
 
 This package can be used to simulate protocols on your computer without connecting to a robot. Please refer to our `Full API Documentation`_ for detailed instructions on how to write and simulate your first protocol.
```

### Comparing `opentrons-7.2.2a3/README.rst` & `opentrons-7.3.0a0/README.rst`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/setup.py` & `opentrons-7.3.0a0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,16 +42,14 @@
 CLASSIFIERS = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering",
 ]
 KEYWORDS = ["robots", "protocols", "synbio", "pcr", "automation", "lab"]
 DESCRIPTION = (
     "The Opentrons API is a simple framework designed to make "
     "writing automated biology lab protocols easy."
@@ -83,15 +81,15 @@
     """
     with codecs.open(os.path.join(HERE, *parts), "rb", "utf-8") as f:
         return f.read()
 
 
 if __name__ == "__main__":
     setup(
-        python_requires=">=3.8",
+        python_requires=">=3.10",
         name=DISTNAME,
         description=DESCRIPTION,
         license=LICENSE,
         version=VERSION,
         author=AUTHOR,
         author_email=EMAIL,
         maintainer=AUTHOR,
```

### Comparing `opentrons-7.2.2a3/src/opentrons/__init__.py` & `opentrons-7.3.0a0/src/opentrons/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/calibration_storage/__init__.py` & `opentrons-7.3.0a0/src/opentrons/calibration_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/calibration_storage/deck_configuration.py` & `opentrons-7.3.0a0/src/opentrons/calibration_storage/deck_configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .types import CutoutFixturePlacement
 from . import file_operators as io
 
 
 class _CutoutFixturePlacementModel(pydantic.BaseModel):
     cutoutId: str
     cutoutFixtureId: str
+    opentronsModuleSerialNumber: Optional[str]
 
 
 class _DeckConfigurationModel(pydantic.BaseModel):
     """The on-filesystem representation of a deck configuration."""
 
     cutoutFixtures: List[_CutoutFixturePlacementModel]
     lastModified: datetime
@@ -22,15 +23,17 @@
 def serialize_deck_configuration(
     cutout_fixture_placements: List[CutoutFixturePlacement], last_modified: datetime
 ) -> bytes:
     """Serialize a deck configuration for storing on the filesystem."""
     data = _DeckConfigurationModel.construct(
         cutoutFixtures=[
             _CutoutFixturePlacementModel.construct(
-                cutoutId=e.cutout_id, cutoutFixtureId=e.cutout_fixture_id
+                cutoutId=e.cutout_id,
+                cutoutFixtureId=e.cutout_fixture_id,
+                opentronsModuleSerialNumber=e.opentrons_module_serial_number,
             )
             for e in cutout_fixture_placements
         ],
         lastModified=last_modified,
     )
     return io.serialize_pydantic_model(data)
 
@@ -46,12 +49,14 @@
     """
     parsed = io.deserialize_pydantic_model(serialized, _DeckConfigurationModel)
     if parsed is None:
         return None
     else:
         cutout_fixture_placements = [
             CutoutFixturePlacement(
-                cutout_id=e.cutoutId, cutout_fixture_id=e.cutoutFixtureId
+                cutout_id=e.cutoutId,
+                cutout_fixture_id=e.cutoutFixtureId,
+                opentrons_module_serial_number=e.opentronsModuleSerialNumber,
             )
             for e in parsed.cutoutFixtures
         ]
         return cutout_fixture_placements, parsed.lastModified
```

### Comparing `opentrons-7.2.2a3/src/opentrons/calibration_storage/encoder_decoder.py` & `opentrons-7.3.0a0/src/opentrons/calibration_storage/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/calibration_storage/file_operators.py` & `opentrons-7.3.0a0/src/opentrons/calibration_storage/file_operators.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/calibration_storage/helpers.py` & `opentrons-7.3.0a0/src/opentrons/calibration_storage/helpers.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/calibration_storage/ot2/__init__.py` & `opentrons-7.3.0a0/src/opentrons/calibration_storage/ot2/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/calibration_storage/ot2/deck_attitude.py` & `opentrons-7.3.0a0/src/opentrons/calibration_storage/ot2/deck_attitude.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/calibration_storage/ot2/mark_bad_calibration.py` & `opentrons-7.3.0a0/src/opentrons/calibration_storage/ot2/mark_bad_calibration.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/calibration_storage/ot2/models/v1.py` & `opentrons-7.3.0a0/src/opentrons/calibration_storage/ot2/models/v1.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/calibration_storage/ot2/pipette_offset.py` & `opentrons-7.3.0a0/src/opentrons/calibration_storage/ot2/pipette_offset.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/calibration_storage/ot2/tip_length.py` & `opentrons-7.3.0a0/src/opentrons/calibration_storage/ot2/tip_length.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/calibration_storage/ot3/__init__.py` & `opentrons-7.3.0a0/src/opentrons/calibration_storage/ot3/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/calibration_storage/ot3/deck_attitude.py` & `opentrons-7.3.0a0/src/opentrons/calibration_storage/ot3/deck_attitude.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/calibration_storage/ot3/gripper_offset.py` & `opentrons-7.3.0a0/src/opentrons/calibration_storage/ot3/gripper_offset.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/calibration_storage/ot3/models/v1.py` & `opentrons-7.3.0a0/src/opentrons/calibration_storage/ot3/models/v1.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/calibration_storage/ot3/module_offset.py` & `opentrons-7.3.0a0/src/opentrons/calibration_storage/ot3/module_offset.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/calibration_storage/ot3/pipette_offset.py` & `opentrons-7.3.0a0/src/opentrons/calibration_storage/ot3/pipette_offset.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/calibration_storage/types.py` & `opentrons-7.3.0a0/src/opentrons/calibration_storage/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -38,7 +38,8 @@
 
 # TODO(mm, 2023-11-20): Deduplicate this with similar types in robot_server
 # and opentrons.protocol_engine.
 @dataclass
 class CutoutFixturePlacement:
     cutout_fixture_id: str
     cutout_id: str
+    opentrons_module_serial_number: typing.Optional[str]
```

### Comparing `opentrons-7.2.2a3/src/opentrons/commands/commands.py` & `opentrons-7.3.0a0/src/opentrons/legacy_commands/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from typing import TYPE_CHECKING, List, Union, overload
 
 
 from .helpers import stringify_location, stringify_disposal_location, listify
 from . import types as command_types
 
 from opentrons.types import Location
-from opentrons.protocol_api._trash_bin import TrashBin
-from opentrons.protocol_api._waste_chute import WasteChute
+from opentrons.protocol_api.disposal_locations import TrashBin, WasteChute
 
 if TYPE_CHECKING:
     from opentrons.protocol_api import InstrumentContext
     from opentrons.protocol_api.labware import Well
 
 
 def home(mount: str) -> command_types.HomeCommand:
```

### Comparing `opentrons-7.2.2a3/src/opentrons/commands/helpers.py` & `opentrons-7.3.0a0/src/opentrons/legacy_commands/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import List, Union
 
 from opentrons.protocol_api.labware import Well, Labware
 from opentrons.protocol_api.module_contexts import ModuleContext
-from opentrons.protocol_api._trash_bin import TrashBin
-from opentrons.protocol_api._waste_chute import WasteChute
+from opentrons.protocol_api.disposal_locations import TrashBin, WasteChute
 from opentrons.protocol_api._types import OffDeckType
 from opentrons.types import Location, DeckLocation
 
 
 CommandLocation = Union[Location, Well]
```

### Comparing `opentrons-7.2.2a3/src/opentrons/commands/module_commands.py` & `opentrons-7.3.0a0/src/opentrons/legacy_commands/module_commands.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/commands/protocol_commands.py` & `opentrons-7.3.0a0/src/opentrons/legacy_commands/protocol_commands.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/commands/publisher.py` & `opentrons-7.3.0a0/src/opentrons/legacy_commands/publisher.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/commands/types.py` & `opentrons-7.3.0a0/src/opentrons/legacy_commands/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from typing_extensions import Literal, Final, TypedDict
 from typing import Optional, List, Sequence, TYPE_CHECKING, Union
 from opentrons.hardware_control.modules import ThermocyclerStep
 
 if TYPE_CHECKING:
     from opentrons.protocol_api import InstrumentContext
     from opentrons.protocol_api.labware import Well
-    from opentrons.protocol_api._trash_bin import TrashBin
-    from opentrons.protocol_api._waste_chute import WasteChute
+    from opentrons.protocol_api.disposal_locations import TrashBin, WasteChute
 
 from opentrons.types import Location
 
 
 # type for subscriptions
 COMMAND: Final = "command"
```

### Comparing `opentrons-7.2.2a3/src/opentrons/config/__init__.py` & `opentrons-7.3.0a0/src/opentrons/config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,14 +280,21 @@
     ConfigElement(
         "module_calibration_dir",
         "Module Calibration Directory",
         Path("robot") / "modules",
         ConfigElementType.DIR,
         "The dir where module calibration is stored",
     ),
+    ConfigElement(
+        "performance_metrics_dir",
+        "Performance Metrics Directory",
+        Path("performance_metrics_data"),
+        ConfigElementType.DIR,
+        "The dir where performance metrics are stored",
+    ),
 )
 #: The available configuration file elements to modify. All of these can be
 #: changed by editing opentrons.json, where the keys are the name elements,
 #: or by specifying as environment variables, where the keys are uppercase
 #: versions of the name elements.
 #: In addition to these flags, the OT_API_CONFIG_DIR env var (if present)
 #: will change where the API looks for these settings by prepending it to the
@@ -598,7 +605,11 @@
 
 def get_tip_length_cal_path() -> Path:
     return get_opentrons_path("tip_length_calibration_dir")
 
 
 def get_custom_tiprack_def_path() -> Path:
     return get_opentrons_path("custom_tiprack_dir")
+
+
+def get_performance_metrics_data_dir() -> Path:
+    return get_opentrons_path("performance_metrics_dir")
```

### Comparing `opentrons-7.2.2a3/src/opentrons/config/advanced_settings.py` & `opentrons-7.3.0a0/src/opentrons/config/advanced_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -156,27 +156,14 @@
         "Opening the robot door during a run will "
         "pause your robot only after it has completed its "
         "current motion.",
         robot_type=[RobotTypeEnum.OT2],
         default_true_on_robot_types=[RobotTypeEnum.FLEX],
     ),
     SettingDefinition(
-        _id="disableFastProtocolUpload",
-        title="Use older protocol analysis method",
-        description=(
-            "Use an older, slower method of analyzing uploaded protocols. "
-            "This changes how the OT-2 validates your protocol during the upload "
-            "step, but does not affect how your protocol actually runs. "
-            "Opentrons Support might ask you to change this setting if you encounter "
-            "problems with the newer, faster protocol analysis method."
-        ),
-        restart_required=False,
-        robot_type=[RobotTypeEnum.OT2, RobotTypeEnum.FLEX],
-    ),
-    SettingDefinition(
         _id="enableOT3HardwareController",
         title="Enable experimental OT-3 hardware controller",
         description=(
             "Do not enable. This is an Opentrons-internal setting to test "
             "new hardware."
         ),
         restart_required=True,
@@ -215,14 +202,45 @@
     ),
     SettingDefinition(
         _id="disableOverpressureDetection",
         title="Disable Flex pipette pressure sensing.",
         description="When this setting is on, Flex will continue its activities regardless of pressure changes inside the pipette. Do not turn this setting on unless you are intentionally causing pressures over 8 kPa inside the pipette air channel.",
         robot_type=[RobotTypeEnum.FLEX],
     ),
+    SettingDefinition(
+        _id="enableErrorRecoveryExperiments",
+        title="Enable error recovery experiments",
+        description=(
+            "Do not enable."
+            " This is an Opentrons internal setting to experiment with"
+            " in-development error recovery features."
+            " This will interfere with your protocol runs,"
+            " corrupt your robot's storage,"
+            " bring misfortune and pestilence upon you and your livestock, etc."
+        ),
+        robot_type=[RobotTypeEnum.FLEX],
+        internal_only=True,
+    ),
+    SettingDefinition(
+        _id="enableOEMMode",
+        title="Enable OEM Mode",
+        description="This setting anonymizes Opentrons branding in the ODD app.",
+        robot_type=[RobotTypeEnum.FLEX],
+    ),
+    SettingDefinition(
+        _id="enablePerformanceMetrics",
+        title="Enable performance metrics",
+        description=(
+            "Do not enable."
+            " This is an Opentrons internal setting to collect performance metrics."
+            " Do not turn this on unless you are playing with the performance metrics system."
+        ),
+        robot_type=[RobotTypeEnum.OT2, RobotTypeEnum.FLEX],
+        internal_only=True,
+    ),
 ]
 
 if (
     ARCHITECTURE == SystemArchitecture.BUILDROOT
     or ARCHITECTURE == SystemArchitecture.YOCTO
 ):
     settings.append(DisableLogIntegrationSettingDefinition())
@@ -664,14 +682,54 @@
     """Migrate to version 30 of the feature flags file.
 
     - Removes the disableTipPresenceDetection flag.
     """
     return {k: v for k, v in previous.items() if "disableTipPresenceDetection" != k}
 
 
+def _migrate30to31(previous: SettingsMap) -> SettingsMap:
+    """Migrate to version 31 of the feature flags file.
+
+    - Adds the enableErrorRecoveryExperiments config element.
+    """
+    newmap = {k: v for k, v in previous.items()}
+    newmap["enableErrorRecoveryExperiments"] = None
+    return newmap
+
+
+def _migrate31to32(previous: SettingsMap) -> SettingsMap:
+    """Migrate to version 32 of the feature flags file.
+
+    - Adds the enableOEMMode config element.
+    """
+    newmap = {k: v for k, v in previous.items()}
+    newmap["enableOEMMode"] = None
+    return newmap
+
+
+def _migrate32to33(previous: SettingsMap) -> SettingsMap:
+    """Migrate to version 33 of the feature flags file.
+
+    - Adds the enablePerformanceMetrics config element.
+    """
+    newmap = {k: v for k, v in previous.items()}
+    newmap["enablePerformanceMetrics"] = None
+    return newmap
+
+
+def _migrate33to34(previous: SettingsMap) -> SettingsMap:
+    """Migrate to version 34 of the feature flags file.
+
+    - Removes disableFastProtocolUpload
+    """
+    removals = ["disableFastProtocolUpload"]
+    newmap = {k: v for k, v in previous.items() if k not in removals}
+    return newmap
+
+
 _MIGRATIONS = [
     _migrate0to1,
     _migrate1to2,
     _migrate2to3,
     _migrate3to4,
     _migrate4to5,
     _migrate5to6,
@@ -695,14 +753,18 @@
     _migrate23to24,
     _migrate24to25,
     _migrate25to26,
     _migrate26to27,
     _migrate27to28,
     _migrate28to29,
     _migrate29to30,
+    _migrate30to31,
+    _migrate31to32,
+    _migrate32to33,
+    _migrate33to34,
 ]
 """
 List of all migrations to apply, indexed by (version - 1). See _migrate below
 for how the migration functions are applied. Each migration function should
 return a new dictionary (rather than modify their input)
 """
```

### Comparing `opentrons-7.2.2a3/src/opentrons/config/defaults_ot2.py` & `opentrons-7.3.0a0/src/opentrons/config/defaults_ot2.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/config/defaults_ot3.py` & `opentrons-7.3.0a0/src/opentrons/config/defaults_ot3.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,44 @@
-from typing import Any, Dict, cast, List, Iterable, Tuple
+from typing import Any, Dict, cast, List, Iterable, Tuple, Optional
 from typing_extensions import Final
 from dataclasses import asdict
 
-from opentrons.hardware_control.types import OT3AxisKind
+from opentrons.hardware_control.types import OT3AxisKind, InstrumentProbeType
 from .types import (
     OT3Config,
     ByGantryLoad,
     OT3CurrentSettings,
     OT3MotionSettings,
     OT3Transform,
     Offset,
     OT3CalibrationSettings,
     CapacitivePassSettings,
     LiquidProbeSettings,
     ZSenseSettings,
     EdgeSenseSettings,
+    OutputOptions,
 )
 
+
 DEFAULT_PIPETTE_OFFSET = [0.0, 0.0, 0.0]
 DEFAULT_MODULE_OFFSET = [0.0, 0.0, 0.0]
 
 DEFAULT_LIQUID_PROBE_SETTINGS: Final[LiquidProbeSettings] = LiquidProbeSettings(
     starting_mount_height=100,
     max_z_distance=40,
     min_z_distance=5,
     mount_speed=10,
     plunger_speed=5,
     sensor_threshold_pascals=40,
     expected_liquid_height=110,
-    log_pressure=True,
+    output_option=OutputOptions.stream_to_csv,
     aspirate_while_sensing=False,
     auto_zero_sensor=True,
     num_baseline_reads=10,
-    data_file="/var/pressure_sensor_data.csv",
+    data_files={InstrumentProbeType.PRIMARY: "/data/pressure_sensor_data.csv"},
 )
 
 DEFAULT_CALIBRATION_SETTINGS: Final[OT3CalibrationSettings] = OT3CalibrationSettings(
     z_offset=ZSenseSettings(
         pass_settings=CapacitivePassSettings(
             prep_distance_mm=4.0,
             max_overrun_distance_mm=5.0,
@@ -188,14 +190,57 @@
         # TODO: verify this value
         OT3AxisKind.P: 1.0,
         OT3AxisKind.Z_G: 0.67,
     },
 )
 
 
+def _build_output_option_with_default(
+    from_conf: Any, default: OutputOptions
+) -> OutputOptions:
+    if from_conf is None:
+        return default
+    else:
+        if isinstance(from_conf, OutputOptions):
+            return from_conf
+        else:
+            try:
+                enumval = OutputOptions[from_conf]
+            except KeyError:  # not an enum entry
+                return default
+            else:
+                return enumval
+
+
+def _build_log_files_with_default(
+    from_conf: Any,
+    default: Optional[Dict[InstrumentProbeType, str]],
+) -> Optional[Dict[InstrumentProbeType, str]]:
+    print(f"from_conf {from_conf} default {default}")
+    if not isinstance(from_conf, dict):
+        if default is None:
+            return None
+        else:
+            return {k: v for k, v in default.items()}
+    else:
+        validated: Dict[InstrumentProbeType, str] = {}
+        for k, v in from_conf.items():
+            if isinstance(k, InstrumentProbeType):
+                validated[k] = v
+            else:
+                try:
+                    enumval = InstrumentProbeType[k]
+                except KeyError:  # not an enum entry
+                    pass
+                else:
+                    validated[enumval] = v
+        print(f"result {validated}")
+        return validated
+
+
 def _build_dict_with_default(
     from_conf: Any,
     default: Dict[OT3AxisKind, float],
 ) -> Dict[OT3AxisKind, float]:
     if not isinstance(from_conf, dict):
         return {k: v for k, v in default.items()}
     else:
@@ -272,39 +317,50 @@
         ),
     )
 
 
 def _build_default_liquid_probe(
     from_conf: Any, default: LiquidProbeSettings
 ) -> LiquidProbeSettings:
+    output_option = _build_output_option_with_default(
+        from_conf.get("output_option", None), default.output_option
+    )
+    data_files: Optional[Dict[InstrumentProbeType, str]] = None
+    if (
+        output_option is OutputOptions.sync_buffer_to_csv
+        or output_option is OutputOptions.stream_to_csv
+    ):
+        data_files = _build_log_files_with_default(
+            from_conf.get("data_files", {}), default.data_files
+        )
     return LiquidProbeSettings(
         starting_mount_height=from_conf.get(
             "starting_mount_height", default.starting_mount_height
         ),
         max_z_distance=from_conf.get("max_z_distance", default.max_z_distance),
         min_z_distance=from_conf.get("min_z_distance", default.min_z_distance),
         mount_speed=from_conf.get("mount_speed", default.mount_speed),
         plunger_speed=from_conf.get("plunger_speed", default.plunger_speed),
         sensor_threshold_pascals=from_conf.get(
             "sensor_threshold_pascals", default.sensor_threshold_pascals
         ),
         expected_liquid_height=from_conf.get(
             "expected_liquid_height", default.expected_liquid_height
         ),
-        log_pressure=from_conf.get("log_pressure", default.log_pressure),
+        output_option=from_conf.get("output_option", default.output_option),
         aspirate_while_sensing=from_conf.get(
             "aspirate_while_sensing", default.aspirate_while_sensing
         ),
         auto_zero_sensor=from_conf.get(
             "get_pressure_baseline", default.auto_zero_sensor
         ),
         num_baseline_reads=from_conf.get(
             "num_baseline_reads", default.num_baseline_reads
         ),
-        data_file=from_conf.get("data_file", default.data_file),
+        data_files=data_files,
     )
 
 
 def _build_default_z_pass(from_conf: Any, default: ZSenseSettings) -> ZSenseSettings:
     return ZSenseSettings(
         pass_settings=_build_default_cap_pass(
             from_conf.get("pass_settings", {}), default.pass_settings
@@ -406,15 +462,15 @@
         ),
     )
 
 
 def serialize(config: OT3Config) -> Dict[str, Any]:
     def _build_dict(pairs: Iterable[Tuple[Any, Any]]) -> Dict[str, Any]:
         def _normalize_key(key: Any) -> Any:
-            if isinstance(key, OT3AxisKind):
+            if isinstance(key, OT3AxisKind) or isinstance(key, InstrumentProbeType):
                 return key.name
             return key
 
         def _normalize_value(value: Any) -> Any:
             if isinstance(value, dict):
                 return {
                     _normalize_key(k): _normalize_value(v) for k, v in value.items()
```

### Comparing `opentrons-7.2.2a3/src/opentrons/config/feature_flags.py` & `opentrons-7.3.0a0/src/opentrons/config/feature_flags.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,20 +20,14 @@
     )
 
 
 def enable_door_safety_switch(robot_type: RobotTypeEnum) -> bool:
     return advs.get_setting_with_env_overload("enableDoorSafetySwitch", robot_type)
 
 
-def disable_fast_protocol_upload() -> bool:
-    return advs.get_setting_with_env_overload(
-        "disableFastProtocolUpload", RobotTypeEnum.FLEX
-    )
-
-
 def enable_ot3_hardware_controller() -> bool:
     """Get whether to use the OT-3 hardware controller."""
 
     return advs.get_setting_with_env_overload(
         "enableOT3HardwareController", RobotTypeEnum.FLEX
     )
 
@@ -66,7 +60,21 @@
 
 
 def require_estop() -> bool:
     """Whether the OT3 should allow gantry movements with no Estop plugged in."""
     return not advs.get_setting_with_env_overload(
         "estopNotRequired", RobotTypeEnum.FLEX
     )
+
+
+def enable_error_recovery_experiments() -> bool:
+    return advs.get_setting_with_env_overload(
+        "enableErrorRecoveryExperiments", RobotTypeEnum.FLEX
+    )
+
+
+def enable_performance_metrics(robot_type: RobotTypeEnum) -> bool:
+    return advs.get_setting_with_env_overload("enablePerformanceMetrics", robot_type)
+
+
+def oem_mode_enabled() -> bool:
+    return advs.get_setting_with_env_overload("enableOEMMode", RobotTypeEnum.FLEX)
```

### Comparing `opentrons-7.2.2a3/src/opentrons/config/gripper_config.py` & `opentrons-7.3.0a0/src/opentrons/config/gripper_config.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/config/reset.py` & `opentrons-7.3.0a0/src/opentrons/config/reset.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/config/robot_configs.py` & `opentrons-7.3.0a0/src/opentrons/config/robot_configs.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/config/types.py` & `opentrons-7.3.0a0/src/opentrons/config/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 from dataclasses import dataclass, asdict, fields
-from typing import Dict, Tuple, TypeVar, Generic, List, cast
+from typing import Dict, Tuple, TypeVar, Generic, List, cast, Optional
 from typing_extensions import TypedDict, Literal
-from opentrons.hardware_control.types import OT3AxisKind
+from opentrons.hardware_control.types import OT3AxisKind, InstrumentProbeType
 
 
 class AxisDict(TypedDict):
     X: float
     Y: float
     Z: float
     A: float
@@ -112,28 +112,38 @@
 
 
 @dataclass(frozen=True)
 class ZSenseSettings:
     pass_settings: CapacitivePassSettings
 
 
+# str enum so it can be json serializable
+class OutputOptions(int, Enum):
+    """Specifies where we should report sensor data to during a sensor pass."""
+
+    stream_to_csv = 0x1
+    sync_buffer_to_csv = 0x2
+    can_bus_only = 0x4
+    sync_only = 0x8
+
+
 @dataclass
 class LiquidProbeSettings:
     starting_mount_height: float
     max_z_distance: float
     min_z_distance: float
     mount_speed: float
     plunger_speed: float
     sensor_threshold_pascals: float
     expected_liquid_height: float
-    log_pressure: bool
+    output_option: OutputOptions
     aspirate_while_sensing: bool
     auto_zero_sensor: bool
     num_baseline_reads: int
-    data_file: str
+    data_files: Optional[Dict[InstrumentProbeType, str]]
 
 
 @dataclass(frozen=True)
 class EdgeSenseSettings:
     overrun_tolerance_mm: float
     early_sense_tolerance_mm: float
     pass_settings: CapacitivePassSettings
```

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/asyncio/communication/async_serial.py` & `opentrons-7.3.0a0/src/opentrons/drivers/asyncio/communication/async_serial.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/asyncio/communication/errors.py` & `opentrons-7.3.0a0/src/opentrons/drivers/asyncio/communication/errors.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/asyncio/communication/serial_connection.py` & `opentrons-7.3.0a0/src/opentrons/drivers/asyncio/communication/serial_connection.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/command_builder.py` & `opentrons-7.3.0a0/src/opentrons/drivers/command_builder.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/heater_shaker/abstract.py` & `opentrons-7.3.0a0/src/opentrons/drivers/heater_shaker/abstract.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/heater_shaker/driver.py` & `opentrons-7.3.0a0/src/opentrons/drivers/heater_shaker/driver.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/heater_shaker/simulator.py` & `opentrons-7.3.0a0/src/opentrons/drivers/heater_shaker/simulator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from typing import Dict
+from typing import Dict, Optional
 from opentrons.util.async_helpers import ensure_yield
 from opentrons.drivers.heater_shaker.abstract import AbstractHeaterShakerDriver
 from opentrons.drivers.types import Temperature, RPM, HeaterShakerLabwareLatchStatus
 
 
 class SimulatingDriver(AbstractHeaterShakerDriver):
     DEFAULT_TEMP = 23
 
-    def __init__(self) -> None:
+    def __init__(self, serial_number: Optional[str] = None) -> None:
         self._labware_latch_state = HeaterShakerLabwareLatchStatus.IDLE_UNKNOWN
         self._current_temperature = self.DEFAULT_TEMP
         self._temperature = Temperature(current=self.DEFAULT_TEMP, target=None)
         self._rpm = RPM(current=0, target=None)
         self._homing_status = True
+        self._serial_number = serial_number
 
     @ensure_yield
     async def connect(self) -> None:
         pass
 
     @ensure_yield
     async def disconnect(self) -> None:
@@ -79,15 +80,15 @@
         self._temperature.current = 23
         self._rpm.target = 0
         self._rpm.current = 0
 
     @ensure_yield
     async def get_device_info(self) -> Dict[str, str]:
         return {
-            "serial": "dummySerialHS",
+            "serial": self._serial_number if self._serial_number else "dummySerialHS",
             "model": "dummyModelHS",
             "version": "dummyVersionHS",
         }
 
     @ensure_yield
     async def enter_programming_mode(self) -> None:
         pass
```

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/mag_deck/abstract.py` & `opentrons-7.3.0a0/src/opentrons/drivers/mag_deck/abstract.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/mag_deck/driver.py` & `opentrons-7.3.0a0/src/opentrons/drivers/mag_deck/driver.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/mag_deck/simulator.py` & `opentrons-7.3.0a0/src/opentrons/drivers/mag_deck/simulator.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 MAG_DECK_MODELS = {
     "magneticModuleV1": "mag_deck_v1.1",
     "magneticModuleV2": "mag_deck_v20",
 }
 
 
 class SimulatingDriver(AbstractMagDeckDriver):
-    def __init__(self, sim_model: Optional[str] = None) -> None:
+    def __init__(
+        self, sim_model: Optional[str] = None, serial_number: Optional[str] = None
+    ) -> None:
         self._height = 0.0
         self._model = MAG_DECK_MODELS[sim_model] if sim_model else "mag_deck_v1.1"
+        self._serial_number = serial_number
 
     @ensure_yield
     async def probe_plate(self) -> None:
         pass
 
     @ensure_yield
     async def home(self) -> None:
@@ -26,15 +29,15 @@
     @ensure_yield
     async def move(self, location: float) -> None:
         self._height = location
 
     @ensure_yield
     async def get_device_info(self) -> Dict[str, str]:
         return {
-            "serial": "dummySerialMD",
+            "serial": self._serial_number if self._serial_number else "dummySerialMD",
             "model": self._model,
             "version": "dummyVersionMD",
         }
 
     @ensure_yield
     async def connect(self) -> None:
         pass
```

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/rpi_drivers/__init__.py` & `opentrons-7.3.0a0/src/opentrons/drivers/rpi_drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/rpi_drivers/dev_types.py` & `opentrons-7.3.0a0/src/opentrons/drivers/rpi_drivers/dev_types.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/rpi_drivers/gpio.py` & `opentrons-7.3.0a0/src/opentrons/drivers/rpi_drivers/gpio.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/rpi_drivers/gpio_simulator.py` & `opentrons-7.3.0a0/src/opentrons/drivers/rpi_drivers/gpio_simulator.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/rpi_drivers/types.py` & `opentrons-7.3.0a0/src/opentrons/drivers/rpi_drivers/types.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/rpi_drivers/usb.py` & `opentrons-7.3.0a0/src/opentrons/drivers/rpi_drivers/usb.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 A class to convert info from the usb bus into a
 more readable format.
 """
 
 import subprocess
 import re
 import os
-from typing import List
+from typing import List, Union
 
-from opentrons.hardware_control.modules.types import ModuleAtPort
+from opentrons.hardware_control.modules.types import (
+    ModuleAtPort,
+    SimulatingModuleAtPort,
+)
 from opentrons.hardware_control.types import BoardRevision
 
 from .interfaces import USBDriverInterface
 from .types import USBPort
 
 
 # Example usb path might look like:
@@ -75,25 +78,25 @@
                 port_matches.append(
                     USBPort.build(match.group(0).strip("/"), self._board_revision)
                 )
         return port_matches
 
     def match_virtual_ports(
         self,
-        virtual_ports: List[ModuleAtPort],
-    ) -> List[ModuleAtPort]:
+        virtual_ports: Union[List[ModuleAtPort], List[SimulatingModuleAtPort]],
+    ) -> Union[List[ModuleAtPort], List[SimulatingModuleAtPort]]:
         """
         Match Virtual Ports
 
         Given a list of virtual module ports, look up the
         symlink to find the device path and link that to
         the physical usb port information.
         The virtual port path looks something like:
         dev/ot_module_[MODULE NAME]
-        :param virtual_ports: A list of ModuleAtPort objects
+        :param virtual_ports: A list of ModuleAtPort or SimulatingModuleAtPort objects
         that hold the name and virtual port of each module
         connected to the robot.
 
         :returns: The updated list of ModuleAtPort
         dataclasses with the physical usb port
         information updated.
         """
```

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/serial_communication.py` & `opentrons-7.3.0a0/src/opentrons/drivers/serial_communication.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/smoothie_drivers/connection.py` & `opentrons-7.3.0a0/src/opentrons/drivers/smoothie_drivers/connection.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/smoothie_drivers/constants.py` & `opentrons-7.3.0a0/src/opentrons/drivers/smoothie_drivers/constants.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/smoothie_drivers/driver_3_0.py` & `opentrons-7.3.0a0/src/opentrons/drivers/smoothie_drivers/driver_3_0.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/smoothie_drivers/errors.py` & `opentrons-7.3.0a0/src/opentrons/drivers/smoothie_drivers/errors.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/smoothie_drivers/parse_utils.py` & `opentrons-7.3.0a0/src/opentrons/drivers/smoothie_drivers/parse_utils.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/smoothie_drivers/simulator.py` & `opentrons-7.3.0a0/src/opentrons/drivers/smoothie_drivers/simulator.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/temp_deck/abstract.py` & `opentrons-7.3.0a0/src/opentrons/drivers/temp_deck/abstract.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/temp_deck/driver.py` & `opentrons-7.3.0a0/src/opentrons/drivers/temp_deck/driver.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/temp_deck/simulator.py` & `opentrons-7.3.0a0/src/opentrons/drivers/temp_deck/simulator.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,18 +7,21 @@
 TEMP_DECK_MODELS = {
     "temperatureModuleV1": "temp_deck_v1.1",
     "temperatureModuleV2": "temp_deck_v20",
 }
 
 
 class SimulatingDriver(AbstractTempDeckDriver):
-    def __init__(self, sim_model: Optional[str] = None):
+    def __init__(
+        self, sim_model: Optional[str] = None, serial_number: Optional[str] = None
+    ):
         self._temp = Temperature(target=None, current=0)
         self._port: Optional[str] = None
         self._model = TEMP_DECK_MODELS[sim_model] if sim_model else "temp_deck_v1.1"
+        self._serial_number = serial_number
 
     @ensure_yield
     async def set_temperature(self, celsius: float) -> None:
         self._temp.target = celsius
         self._temp.current = self._temp.target
 
     @ensure_yield
@@ -44,11 +47,11 @@
     @ensure_yield
     async def enter_programming_mode(self) -> None:
         pass
 
     @ensure_yield
     async def get_device_info(self) -> Dict[str, str]:
         return {
-            "serial": "dummySerialTD",
+            "serial": self._serial_number if self._serial_number else "dummySerialTD",
             "model": self._model,
             "version": "dummyVersionTD",
         }
```

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/thermocycler/abstract.py` & `opentrons-7.3.0a0/src/opentrons/drivers/thermocycler/abstract.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/thermocycler/driver.py` & `opentrons-7.3.0a0/src/opentrons/drivers/thermocycler/driver.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/thermocycler/simulator.py` & `opentrons-7.3.0a0/src/opentrons/drivers/thermocycler/simulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,25 @@
 from opentrons.hardware_control.modules.types import ThermocyclerModuleModel
 from opentrons.drivers.asyncio.communication.errors import ErrorResponse
 
 
 class SimulatingDriver(AbstractThermocyclerDriver):
     DEFAULT_TEMP = 23
 
-    def __init__(self, model: Optional[str] = None) -> None:
+    def __init__(
+        self, model: Optional[str] = None, serial_number: Optional[str] = None
+    ) -> None:
         self._ramp_rate: Optional[float] = None
         self._lid_status = ThermocyclerLidStatus.OPEN
         self._lid_temperature = Temperature(current=self.DEFAULT_TEMP, target=None)
         self._plate_temperature = PlateTemperature(
             current=self.DEFAULT_TEMP, target=None, hold=None
         )
         self._model = model if model else "thermocyclerModuleV1"
+        self._serial_number = serial_number
 
     def model(self) -> str:
         return self._model
 
     @ensure_yield
     async def connect(self) -> None:
         pass
@@ -99,15 +102,15 @@
     async def deactivate_all(self) -> None:
         await self.deactivate_lid()
         await self.deactivate_block()
 
     @ensure_yield
     async def get_device_info(self) -> Dict[str, str]:
         return {
-            "serial": "dummySerialTC",
+            "serial": self._serial_number if self._serial_number else "dummySerialTC",
             "model": "dummyModelTC",
             "version": "dummyVersionTC",
         }
 
     @ensure_yield
     async def enter_programming_mode(self) -> None:
         pass
```

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/types.py` & `opentrons-7.3.0a0/src/opentrons/drivers/types.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/drivers/utils.py` & `opentrons-7.3.0a0/src/opentrons/drivers/utils.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/execute.py` & `opentrons-7.3.0a0/src/opentrons/execute.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 )
 
 from opentrons_shared_data.labware.labware_definition import LabwareDefinition
 from opentrons_shared_data.robot.dev_types import RobotType
 
 from opentrons import protocol_api, __version__, should_use_ot3
 
-from opentrons.commands import types as command_types
+from opentrons.legacy_commands import types as command_types
 
 from opentrons.hardware_control import (
     API as OT2API,
     ThreadManagedHardware,
     ThreadManager,
 )
 from opentrons.hardware_control.types import HardwareFeatureFlags
@@ -329,15 +329,15 @@
 
           {
             'name': command_name,
             'payload': {
               'text': string_command_text,
               # The rest of this struct is
               # command-dependent; see
-              # opentrons.commands.commands.
+              # opentrons.legacy_commands.commands.
              }
           }
 
         .. note::
           In older software versions, ``payload["text"]`` was a
           `format string <https://docs.python.org/3/library/string.html#formatstrings>`_.
           To get human-readable text, you had to do ``payload["text"].format(**payload)``.
@@ -596,15 +596,17 @@
     )
 
     if emit_runlog:
         context.broker.subscribe(command_types.COMMAND, emit_runlog)
 
     context.home()
     try:
-        execute_apiv2.run_protocol(protocol, context)
+        # TODO (spp, 2024-03-18): use true run-time param overrides once enabled
+        #  for cli protocol simulation/ execution
+        execute_apiv2.run_protocol(protocol, context, run_time_param_overrides=None)
     finally:
         context.cleanup()
 
 
 def _run_file_pe(
     protocol: Protocol,
     hardware_api: ThreadManagedHardware,
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/__init__.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/__main__.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/__main__.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/adapters.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/adapters.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/api.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,15 @@
 
     @classmethod
     async def build_hardware_simulator(
         cls,
         attached_instruments: Optional[
             Dict[top_types.Mount, Dict[str, Optional[str]]]
         ] = None,
-        attached_modules: Optional[List[str]] = None,
+        attached_modules: Optional[Dict[str, List[str]]] = None,
         config: Optional[Union[RobotConfig, OT3Config]] = None,
         loop: Optional[asyncio.AbstractEventLoop] = None,
         strict_attached_instruments: bool = True,
         feature_flags: Optional[HardwareFeatureFlags] = None,
     ) -> "API":
         """Build a simulating hardware controller.
 
@@ -267,15 +267,15 @@
         Multiple simulating hardware controllers may be active at one time.
         """
 
         if None is attached_instruments:
             attached_instruments = {}
 
         if None is attached_modules:
-            attached_modules = []
+            attached_modules = {}
 
         checked_loop = use_or_initialize_loop(loop)
         if isinstance(config, RobotConfig):
             checked_config = config
         else:
             checked_config = robot_configs.load_ot2()
         backend = await Simulator.build(
@@ -427,15 +427,17 @@
             firmware_file, checked_loop, explicit_modeset
         )
 
     def has_gripper(self) -> bool:
         return False
 
     async def cache_instruments(
-        self, require: Optional[Dict[top_types.Mount, PipetteName]] = None
+        self,
+        require: Optional[Dict[top_types.Mount, PipetteName]] = None,
+        skip_if_would_block: bool = False,
     ) -> None:
         """
         Scan the attached instruments, take necessary configuration actions,
         and set up hardware controller internal state if necessary.
         """
         self._log.info("Updating instrument model cache")
         checked_require = require or {}
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/backends/controller.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/backends/controller.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/backends/estop_state.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/backends/estop_state.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/backends/flex_protocol.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/backends/flex_protocol.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Tuple,
     Set,
     TypeVar,
 )
 from opentrons_shared_data.pipette.dev_types import (
     PipetteName,
 )
-from opentrons.config.types import GantryLoad
+from opentrons.config.types import GantryLoad, OutputOptions
 from opentrons.hardware_control.types import (
     BoardRevision,
     Axis,
     OT3Mount,
     OT3AxisMap,
     InstrumentProbeType,
     MotorStatus,
@@ -29,18 +29,20 @@
     TipStateType,
     GripperJawState,
     HardwareFeatureFlags,
     EstopOverallStatus,
     EstopState,
     HardwareEventHandler,
     HardwareEventUnsubscriber,
+    HepaFanState,
+    HepaUVState,
+    StatusBarState,
 )
 from opentrons.hardware_control.module_control import AttachedModulesControl
 from ..dev_types import OT3AttachedInstruments
-from ..types import StatusBarState
 from .types import HWStopCondition
 
 Cls = TypeVar("Cls")
 
 
 class FlexBackend(Protocol):
     """Flex backend mypy protocol."""
@@ -140,15 +142,16 @@
     async def liquid_probe(
         self,
         mount: OT3Mount,
         max_z_distance: float,
         mount_speed: float,
         plunger_speed: float,
         threshold_pascals: float,
-        log_pressure: bool = True,
+        output_format: OutputOptions = OutputOptions.can_bus_only,
+        data_files: Optional[Dict[InstrumentProbeType, str]] = None,
         auto_zero_sensor: bool = True,
         num_baseline_reads: int = 10,
         probe: InstrumentProbeType = InstrumentProbeType.PRIMARY,
     ) -> float:
         ...
 
     async def move(
@@ -303,14 +306,22 @@
         """Updates the firmware on the OT3."""
         ...
 
     def engaged_axes(self) -> OT3AxisMap[bool]:
         """Get engaged axes."""
         ...
 
+    async def update_engaged_axes(self) -> None:
+        """Update engaged axes."""
+        ...
+
+    async def is_motor_engaged(self, axis: Axis) -> bool:
+        """Check if axis is enabled."""
+        ...
+
     async def disengage_axes(self, axes: List[Axis]) -> None:
         """Disengage axes."""
         ...
 
     async def engage_axes(self, axes: List[Axis]) -> None:
         """Engage axes."""
         ...
@@ -368,15 +379,17 @@
     ) -> List[float]:
         ...
 
     @property
     def subsystems(self) -> Dict[SubSystem, SubSystemState]:
         ...
 
-    async def get_tip_status(self, mount: OT3Mount) -> TipStateType:
+    async def get_tip_status(
+        self, mount: OT3Mount, ht_operation_sensor: Optional[InstrumentProbeType] = None
+    ) -> TipStateType:
         ...
 
     def current_tip_state(self, mount: OT3Mount) -> Optional[bool]:
         ...
 
     async def update_tip_detector(self, mount: OT3Mount, sensor_count: int) -> None:
         ...
@@ -413,7 +426,21 @@
         grip_width_uncertainty_narrower: float,
         jaw_width: float,
         max_allowed_grip_error: float,
         hard_limit_lower: float,
         hard_limit_upper: float,
     ) -> None:
         ...
+
+    async def set_hepa_fan_state(self, fan_on: bool, duty_cycle: int) -> bool:
+        """Sets the state and duty cycle of the Hepa/UV module."""
+        ...
+
+    async def get_hepa_fan_state(self) -> Optional[HepaFanState]:
+        ...
+
+    async def set_hepa_uv_state(self, light_on: bool, uv_duration_s: int) -> bool:
+        """Sets the state and duration (seconds) of the UV light for the Hepa/UV module."""
+        ...
+
+    async def get_hepa_uv_state(self) -> Optional[HepaUVState]:
+        ...
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/backends/ot3controller.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/backends/ot3controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Set,
     TypeVar,
     Iterator,
     KeysView,
     Union,
     Mapping,
 )
-from opentrons.config.types import OT3Config, GantryLoad
+from opentrons.config.types import OT3Config, GantryLoad, OutputOptions
 from opentrons.config import gripper_config
 from .ot3utils import (
     axis_convert,
     create_move_group,
     axis_to_node,
     get_current_settings,
     create_home_groups,
@@ -82,14 +82,15 @@
 from opentrons.hardware_control.backends.estop_state import EstopStateMachine
 
 from opentrons_hardware.hardware_control.motor_enable_disable import (
     set_enable_motor,
     set_disable_motor,
     set_enable_tip_motor,
     set_disable_tip_motor,
+    get_motor_enabled,
 )
 from opentrons_hardware.hardware_control.motor_position_status import (
     get_motor_position,
     update_motor_position_estimation,
 )
 from opentrons_hardware.hardware_control.limit_switches import get_limit_switches
 from opentrons_hardware.hardware_control.current_settings import (
@@ -165,14 +166,20 @@
     get_door_state,
     set_deck_light,
     get_deck_light_state,
 )
 from opentrons_hardware.hardware_control.gripper_settings import (
     get_gripper_jaw_state,
 )
+from opentrons_hardware.hardware_control.hepa_uv_settings import (
+    set_hepa_fan_state as set_hepa_fan_state_fw,
+    get_hepa_fan_state as get_hepa_fan_state_fw,
+    set_hepa_uv_state as set_hepa_uv_state_fw,
+    get_hepa_uv_state as get_hepa_uv_state_fw,
+)
 
 from opentrons_hardware.drivers.gpio import OT3GPIO, RemoteOT3GPIO
 from opentrons_shared_data.pipette.dev_types import PipetteName
 from opentrons_shared_data.pipette import (
     pipette_load_name_conversions as pipette_load_name,
     load_data as load_pipette_data,
 )
@@ -189,15 +196,15 @@
 from .subsystem_manager import SubsystemManager
 
 from ..dev_types import (
     AttachedPipette,
     AttachedGripper,
     OT3AttachedInstruments,
 )
-from ..types import StatusBarState
+from ..types import HepaFanState, HepaUVState, StatusBarState
 
 from .types import HWStopCondition
 from .flex_protocol import FlexBackend
 from .status_bar_state import StatusBarStateController
 
 log = logging.getLogger(__name__)
 
@@ -249,14 +256,15 @@
     _initialized: bool
     _messenger: CanMessenger
     _usb_messenger: Optional[BinaryMessenger]
     _position: Dict[NodeId, float]
     _encoder_position: Dict[NodeId, float]
     _motor_status: Dict[NodeId, MotorStatus]
     _subsystem_manager: SubsystemManager
+    _engaged_axes: OT3AxisMap[bool]
 
     @classmethod
     async def build(
         cls,
         config: OT3Config,
         use_usb_bus: bool = False,
         check_updates: bool = True,
@@ -324,14 +332,15 @@
         )
         self._estop_detector: Optional[EstopDetector] = None
         self._estop_state_machine = EstopStateMachine(detector=None)
         self._position = self._get_home_position()
         self._gear_motor_position: Dict[NodeId, float] = {}
         self._encoder_position = self._get_home_position()
         self._motor_status = {}
+        self._engaged_axes = {}
         self._check_updates = check_updates
         self._initialized = False
         self._status_bar = status_bar.StatusBar(messenger=self._usb_messenger)
         self._status_bar_controller = StatusBarStateController(self._status_bar)
 
         try:
             self._event_watcher = self._build_event_watcher()
@@ -1147,45 +1156,66 @@
         while can_watch and (not self._event_watcher.closed):
             await self._handle_watch_event()
 
     @property
     def axis_bounds(self) -> OT3AxisMap[Tuple[float, float]]:
         """Get the axis bounds."""
         # TODO (AL, 2021-11-18): The bounds need to be defined
-        phony_bounds = (0, 500)
         return {
-            Axis.Z_L: phony_bounds,
-            Axis.Z_R: phony_bounds,
-            Axis.P_L: phony_bounds,
-            Axis.P_R: phony_bounds,
-            Axis.X: phony_bounds,
-            Axis.Y: phony_bounds,
-            Axis.Z_G: phony_bounds,
-            Axis.Q: phony_bounds,
+            Axis.Z_L: (0, 300),
+            Axis.Z_R: (0, 300),
+            Axis.P_L: (0, 200),
+            Axis.P_R: (0, 200),
+            Axis.X: (0, 550),
+            Axis.Y: (0, 550),
+            Axis.Z_G: (0, 300),
+            Axis.Q: (0, 200),
         }
 
     def engaged_axes(self) -> OT3AxisMap[bool]:
         """Get engaged axes."""
-        return {}
+        return self._engaged_axes
+
+    async def update_engaged_axes(self) -> None:
+        """Update engaged axes."""
+        motor_nodes = self._motor_nodes()
+        results = await get_motor_enabled(self._messenger, motor_nodes)
+        for node, status in results.items():
+            self._engaged_axes[node_to_axis(node)] = status
+
+    async def is_motor_engaged(self, axis: Axis) -> bool:
+        node = axis_to_node(axis)
+        result = await get_motor_enabled(self._messenger, {node})
+        engaged = result[node]
+        self._engaged_axes.update({axis: engaged})
+        return engaged
 
     async def disengage_axes(self, axes: List[Axis]) -> None:
         """Disengage axes."""
         if Axis.Q in axes:
             await set_disable_tip_motor(self._messenger, {axis_to_node(Axis.Q)})
-        nodes = {axis_to_node(ax) for ax in axes if ax is not Axis.Q}
-        if len(nodes) > 0:
-            await set_disable_motor(self._messenger, nodes)
+            self._engaged_axes[Axis.Q] = False
+            axes = [ax for ax in axes if ax is not Axis.Q]
+
+        if len(axes) > 0:
+            await set_disable_motor(self._messenger, {axis_to_node(ax) for ax in axes})
+        for ax in axes:
+            self._engaged_axes[ax] = False
 
     async def engage_axes(self, axes: List[Axis]) -> None:
         """Engage axes."""
         if Axis.Q in axes:
             await set_enable_tip_motor(self._messenger, {axis_to_node(Axis.Q)})
-        nodes = {axis_to_node(ax) for ax in axes if ax is not Axis.Q}
-        if len(nodes) > 0:
-            await set_enable_motor(self._messenger, nodes)
+            self._engaged_axes[Axis.Q] = True
+            axes = [ax for ax in axes if ax is not Axis.Q]
+
+        if len(axes) > 0:
+            await set_enable_motor(self._messenger, {axis_to_node(ax) for ax in axes})
+        for ax in axes:
+            self._engaged_axes[ax] = True
 
     @requires_update
     async def set_lights(self, button: Optional[bool], rails: Optional[bool]) -> None:
         """Set the light states."""
         if rails is not None:
             await set_deck_light(1 if rails else 0, self._usb_messenger)
 
@@ -1316,33 +1346,59 @@
     async def liquid_probe(
         self,
         mount: OT3Mount,
         max_z_distance: float,
         mount_speed: float,
         plunger_speed: float,
         threshold_pascals: float,
-        log_pressure: bool = True,
+        output_option: OutputOptions = OutputOptions.can_bus_only,
+        data_files: Optional[Dict[InstrumentProbeType, str]] = None,
         auto_zero_sensor: bool = True,
         num_baseline_reads: int = 10,
         probe: InstrumentProbeType = InstrumentProbeType.PRIMARY,
     ) -> float:
+        if output_option == OutputOptions.sync_buffer_to_csv:
+            assert (
+                self._subsystem_manager.device_info[
+                    SubSystem.of_mount(mount)
+                ].revision.tertiary
+                == "1"
+            )
         head_node = axis_to_node(Axis.by_mount(mount))
         tool = sensor_node_for_pipette(OT3Mount(mount.value))
+        csv_output = bool(output_option.value & OutputOptions.stream_to_csv.value)
+        sync_buffer_output = bool(
+            output_option.value & OutputOptions.sync_buffer_to_csv.value
+        )
+        can_bus_only_output = bool(
+            output_option.value & OutputOptions.can_bus_only.value
+        )
+        data_files_transposed = (
+            None
+            if data_files is None
+            else {
+                sensor_id_for_instrument(probe): data_files[probe]
+                for probe in data_files.keys()
+            }
+        )
         positions = await liquid_probe(
-            self._messenger,
-            tool,
-            head_node,
-            max_z_distance,
-            plunger_speed,
-            mount_speed,
-            threshold_pascals,
-            log_pressure,
-            auto_zero_sensor,
-            num_baseline_reads,
-            sensor_id_for_instrument(probe),
+            messenger=self._messenger,
+            tool=tool,
+            head_node=head_node,
+            max_z_distance=max_z_distance,
+            plunger_speed=plunger_speed,
+            mount_speed=mount_speed,
+            threshold_pascals=threshold_pascals,
+            csv_output=csv_output,
+            sync_buffer_output=sync_buffer_output,
+            can_bus_only_output=can_bus_only_output,
+            data_files=data_files_transposed,
+            auto_zero_sensor=auto_zero_sensor,
+            num_baseline_reads=num_baseline_reads,
+            sensor_id=sensor_id_for_instrument(probe),
         )
         for node, point in positions.items():
             self._position.update({node: point.motor_position})
             self._encoder_position.update({node: point.encoder_position})
         return self._position[axis_to_node(Axis.by_mount(mount))]
 
     async def capacitive_probe(
@@ -1461,16 +1517,22 @@
         """Build indiviudal tip detector for a mount."""
         await self.teardown_tip_detector(mount)
         await self._tip_presence_manager.build_detector(mount, sensor_count)
 
     async def teardown_tip_detector(self, mount: OT3Mount) -> None:
         await self._tip_presence_manager.clear_detector(mount)
 
-    async def get_tip_status(self, mount: OT3Mount) -> TipStateType:
-        return await self.tip_presence_manager.get_tip_status(mount)
+    async def get_tip_status(
+        self,
+        mount: OT3Mount,
+        follow_singular_sensor: Optional[InstrumentProbeType] = None,
+    ) -> TipStateType:
+        return await self.tip_presence_manager.get_tip_status(
+            mount, follow_singular_sensor
+        )
 
     def current_tip_state(self, mount: OT3Mount) -> Optional[bool]:
         return self.tip_presence_manager.current_tip_state(mount)
 
     async def set_status_bar_state(self, state: StatusBarState) -> None:
         await self._status_bar_controller.set_status_bar_state(state)
 
@@ -1566,7 +1628,41 @@
                 details={
                     "failure-type": "jaws-more-open-than-expected",
                     "upper-bound-labware-width": expected_grip_width
                     - grip_width_uncertainty_narrower,
                     "actual-jaw-width": current_gripper_position,
                 },
             )
+
+    async def set_hepa_fan_state(self, fan_on: bool, duty_cycle: int) -> bool:
+        return await set_hepa_fan_state_fw(self._messenger, fan_on, duty_cycle)
+
+    async def get_hepa_fan_state(self) -> Optional[HepaFanState]:
+        res = await get_hepa_fan_state_fw(self._messenger)
+        return (
+            HepaFanState(
+                fan_on=res.fan_on,
+                duty_cycle=res.duty_cycle,
+            )
+            if res
+            else None
+        )
+
+    async def set_hepa_uv_state(self, light_on: bool, uv_duration_s: int) -> bool:
+        return await set_hepa_uv_state_fw(self._messenger, light_on, uv_duration_s)
+
+    async def get_hepa_uv_state(self) -> Optional[HepaUVState]:
+        res = await get_hepa_uv_state_fw(self._messenger)
+        return (
+            HepaUVState(
+                light_on=res.uv_light_on,
+                uv_duration_s=res.uv_duration_s,
+                remaining_time_s=res.remaining_time_s,
+            )
+            if res
+            else None
+        )
+
+    def _update_tip_state(self, mount: OT3Mount, status: bool) -> None:
+        """This is something we only use in the simulator.
+        It is required so that PE simulations using ot3api don't break."""
+        pass
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/backends/ot3simulator.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/backends/ot3simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,24 @@
     AsyncIterator,
     cast,
     Set,
     Union,
     Mapping,
 )
 
-from opentrons.config.types import OT3Config, GantryLoad
+from opentrons.config.types import OT3Config, GantryLoad, OutputOptions
 from opentrons.config import gripper_config
 
 from opentrons.hardware_control.module_control import AttachedModulesControl
 from opentrons.hardware_control import modules
 from opentrons.hardware_control.types import (
     BoardRevision,
     Axis,
+    HepaFanState,
+    HepaUVState,
     OT3Mount,
     OT3AxisMap,
     CurrentConfig,
     InstrumentProbeType,
     MotorStatus,
     UpdateStatus,
     UpdateState,
@@ -58,14 +60,15 @@
     AttachedGripper,
     OT3AttachedInstruments,
 )
 from opentrons.util.async_helpers import ensure_yield
 from .types import HWStopCondition
 from .flex_protocol import FlexBackend
 
+
 log = logging.getLogger(__name__)
 
 AXIS_TO_SUBSYSTEM = {
     Axis.X: SubSystem.gantry_x,
     Axis.Y: SubSystem.gantry_y,
     Axis.Z_L: SubSystem.head,
     Axis.Z_R: SubSystem.head,
@@ -91,20 +94,21 @@
 
 class OT3Simulator(FlexBackend):
     """OT3 Hardware Controller Backend."""
 
     _position: Dict[Axis, float]
     _encoder_position: Dict[Axis, float]
     _motor_status: Dict[Axis, MotorStatus]
+    _engaged_axes: Dict[Axis, bool]
 
     @classmethod
     async def build(
         cls,
         attached_instruments: Dict[OT3Mount, Dict[str, Optional[str]]],
-        attached_modules: List[str],
+        attached_modules: Dict[str, List[str]],
         config: OT3Config,
         loop: asyncio.AbstractEventLoop,
         strict_attached_instruments: bool = True,
         feature_flags: Optional[HardwareFeatureFlags] = None,
     ) -> OT3Simulator:
         """Create the OT3Simulator instance.
 
@@ -122,15 +126,15 @@
             strict_attached_instruments,
             feature_flags,
         )
 
     def __init__(
         self,
         attached_instruments: Dict[OT3Mount, Dict[str, Optional[str]]],
-        attached_modules: List[str],
+        attached_modules: Dict[str, List[str]],
         config: OT3Config,
         loop: asyncio.AbstractEventLoop,
         strict_attached_instruments: bool = True,
         feature_flags: Optional[HardwareFeatureFlags] = None,
     ) -> None:
         """Construct.
 
@@ -142,14 +146,15 @@
         self._loop = loop
         self._strict_attached = bool(strict_attached_instruments)
         self._stubbed_attached_modules = attached_modules
         self._update_required = False
         self._initialized = False
         self._lights = {"button": False, "rails": False}
         self._gear_motor_position: Dict[Axis, float] = {}
+        self._engaged_axes: Dict[Axis, bool] = {}
         self._feature_flags = feature_flags or HardwareFeatureFlags()
 
         def _sanitize_attached_instrument(
             mount: OT3Mount, passed_ai: Optional[Dict[str, Optional[str]]] = None
         ) -> Union[PipetteSpec, GripperSpec]:
             if mount is OT3Mount.GRIPPER:
                 gripper_spec: GripperSpec = {"model": None, "id": None}
@@ -336,15 +341,16 @@
     async def liquid_probe(
         self,
         mount: OT3Mount,
         max_z_distance: float,
         mount_speed: float,
         plunger_speed: float,
         threshold_pascals: float,
-        log_pressure: bool = True,
+        output_format: OutputOptions = OutputOptions.can_bus_only,
+        data_files: Optional[Dict[InstrumentProbeType, str]] = None,
         auto_zero_sensor: bool = True,
         num_baseline_reads: int = 10,
         probe: InstrumentProbeType = InstrumentProbeType.PRIMARY,
     ) -> float:
         z_axis = Axis.by_mount(mount)
         pos = self._position
         pos[z_axis] += max_z_distance
@@ -368,14 +374,16 @@
             home_flagged_axes: Whether to home afterwords.
             speed: Optional speed
             axis_max_speeds: Optional map of axis to speed.
 
         Returns:
             None
         """
+        for ax in origin:
+            self._engaged_axes[ax] = True
         self._position.update(target)
         self._encoder_position.update(target)
 
     @ensure_yield
     async def home(
         self, axes: Sequence[Axis], gantry_load: GantryLoad
     ) -> OT3AxisMap[float]:
@@ -390,14 +398,15 @@
         if axes:
             homed = axes
         else:
             homed = list(iter(self._position.keys()))
         for h in homed:
             self._position[h] = self._get_home_position()[h]
             self._motor_status[h] = MotorStatus(True, True)
+            self._engaged_axes[h] = True
         return axis_pad(self._position, 0.0)
 
     @ensure_yield
     async def gripper_grip_jaw(
         self,
         duty_cycle: float,
         expected_displacement: float,
@@ -493,21 +502,28 @@
                     "config": load_pipette_data.load_definition(
                         converted_name.pipette_type,
                         converted_name.pipette_channels,
                         converted_name.pipette_version,
                     ),
                     "id": None,
                 }
-        if found_model and expected_instr or found_model:
+        if found_model and init_instr["id"] is not None:
             # Instrument detected matches instrument expected (note:
             # "instrument detected" means passed as an argument to the
             # constructor of this class)
 
             # OR Instrument detected and no expected instrument specified
-            converted_name = pipette_load_name.convert_pipette_model(found_model)
+
+            found_model_version = ""
+            if found_model.find("flex") > -1:
+                found_model = found_model.replace("_flex", "")  # type: ignore
+                found_model_version = f"{init_instr['id'][4]}.{init_instr['id'][5]}"
+            converted_name = pipette_load_name.convert_pipette_model(
+                found_model, found_model_version
+            )
             return {
                 "config": load_pipette_data.load_definition(
                     converted_name.pipette_type,
                     converted_name.pipette_channels,
                     converted_name.pipette_version,
                 ),
                 "id": init_instr["id"],
@@ -584,18 +600,24 @@
         Temporarily increase the hold current when engaging the Z_L axis
         while the 96-channel is attached
         """
         yield
 
     @ensure_yield
     async def watch(self, loop: asyncio.AbstractEventLoop) -> None:
-        new_mods_at_ports = [
-            modules.ModuleAtPort(port=f"/dev/ot_module_sim_{mod}{str(idx)}", name=mod)
-            for idx, mod in enumerate(self._stubbed_attached_modules)
-        ]
+        new_mods_at_ports = []
+        for mod, serials in self._stubbed_attached_modules.items():
+            for serial in serials:
+                new_mods_at_ports.append(
+                    modules.SimulatingModuleAtPort(
+                        port=f"/dev/ot_module_sim_{mod}{str(serial)}",
+                        name=mod,
+                        serial_number=serial,
+                    )
+                )
         await self.module_controls.register_modules(new_mods_at_ports=new_mods_at_ports)
 
     @property
     def axis_bounds(self) -> OT3AxisMap[Tuple[float, float]]:
         """Get the axis bounds."""
         # TODO (AL, 2021-11-18): The bounds need to be defined
         phony_bounds = (0, 10000)
@@ -637,24 +659,37 @@
         for subsystem in subsystems:
             yield UpdateStatus(
                 subsystem=subsystem, state=UpdateState.done, progress=100
             )
 
     def engaged_axes(self) -> OT3AxisMap[bool]:
         """Get engaged axes."""
-        return {}
+        return self._engaged_axes
+
+    async def update_engaged_axes(self) -> None:
+        """Update engaged axes."""
+        return None
+
+    async def is_motor_engaged(self, axis: Axis) -> bool:
+        if axis not in self._engaged_axes.keys():
+            return False
+        return self._engaged_axes[axis]
 
     @ensure_yield
     async def disengage_axes(self, axes: List[Axis]) -> None:
         """Disengage axes."""
+        for ax in axes:
+            self._engaged_axes.update({ax: False})
         return None
 
     @ensure_yield
     async def engage_axes(self, axes: List[Axis]) -> None:
         """Engage axes."""
+        for ax in axes:
+            self._engaged_axes.update({ax: True})
         return None
 
     @ensure_yield
     async def set_lights(self, button: Optional[bool], rails: Optional[bool]) -> None:
         """Set the light states."""
         # Simulate how the real driver does this - there's no button so it's always false
         if rails is not None:
@@ -741,15 +776,19 @@
                 current_fw_sha="simulated",
                 pcba_revision="A1",
                 update_state=None,
             )
             for axis in self._present_axes
         }
 
-    async def get_tip_status(self, mount: OT3Mount) -> TipStateType:
+    async def get_tip_status(
+        self,
+        mount: OT3Mount,
+        follow_singular_sensor: Optional[InstrumentProbeType] = None,
+    ) -> TipStateType:
         return TipStateType(self._sim_tip_state[mount])
 
     def current_tip_state(self, mount: OT3Mount) -> Optional[bool]:
         return self._sim_tip_state[mount]
 
     async def update_tip_detector(self, mount: OT3Mount, sensor_count: int) -> None:
         pass
@@ -799,7 +838,24 @@
         max_allowed_grip_error: float,
         hard_limit_lower: float,
         hard_limit_upper: float,
     ) -> None:
         # This is a (pretty bad) simulation of the gripper actually gripping something,
         # but it should work.
         self._encoder_position[Axis.G] = (hard_limit_upper - jaw_width) / 2
+
+    async def set_hepa_fan_state(self, fan_on: bool, duty_cycle: int) -> bool:
+        return False
+
+    async def get_hepa_fan_state(self) -> Optional[HepaFanState]:
+        return None
+
+    async def set_hepa_uv_state(self, light_on: bool, timeout_s: int) -> bool:
+        return False
+
+    async def get_hepa_uv_state(self) -> Optional[HepaUVState]:
+        return None
+
+    def _update_tip_state(self, mount: OT3Mount, status: bool) -> None:
+        """This is something we only use in the simulator.
+        It is required so that PE simulations using ot3api don't break."""
+        self._sim_tip_state[mount] = status
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/backends/ot3utils.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/backends/ot3utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -540,14 +540,15 @@
 def sensor_node_for_pipette(mount: OT3Mount) -> PipetteProbeTarget:
     return _sensor_node_lookup_pipettes_only[mount]
 
 
 _instr_sensor_id_lookup: Dict[InstrumentProbeType, SensorId] = {
     InstrumentProbeType.PRIMARY: SensorId.S0,
     InstrumentProbeType.SECONDARY: SensorId.S1,
+    InstrumentProbeType.BOTH: SensorId.BOTH,
 }
 
 
 def sensor_id_for_instrument(probe: InstrumentProbeType) -> SensorId:
     return _instr_sensor_id_lookup[probe]
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/backends/simulator.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/backends/simulator.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     a robot with no smoothie connected.
     """
 
     @classmethod
     async def build(
         cls,
         attached_instruments: Dict[types.Mount, Dict[str, Optional[str]]],
-        attached_modules: List[str],
+        attached_modules: Dict[str, List[str]],
         config: RobotConfig,
         loop: asyncio.AbstractEventLoop,
         strict_attached_instruments: bool = True,
     ) -> Simulator:
         """Build the simulator.
 
         Use this factory method rather than the initializer to handle proper GPIO
@@ -101,15 +101,15 @@
             gpio,
             strict_attached_instruments,
         )
 
     def __init__(
         self,
         attached_instruments: Dict[types.Mount, Dict[str, Optional[str]]],
-        attached_modules: List[str],
+        attached_modules: Dict[str, List[str]],
         config: RobotConfig,
         loop: asyncio.AbstractEventLoop,
         gpio_chardev: GPIODriverLike,
         strict_attached_instruments: bool = True,
     ) -> None:
         """Initialize the simulator.
 
@@ -328,18 +328,24 @@
         }
 
     def set_active_current(self, axis_currents: Dict[Axis, float]) -> None:
         pass
 
     @ensure_yield
     async def watch(self) -> None:
-        new_mods_at_ports = [
-            modules.ModuleAtPort(port=f"/dev/ot_module_sim_{mod}{str(idx)}", name=mod)
-            for idx, mod in enumerate(self._stubbed_attached_modules)
-        ]
+        new_mods_at_ports = []
+        for mod, serials in self._stubbed_attached_modules.items():
+            for serial in serials:
+                new_mods_at_ports.append(
+                    modules.SimulatingModuleAtPort(
+                        port=f"/dev/ot_module_sim_{mod}{str(serial)}",
+                        name=mod,
+                        serial_number=serial,
+                    )
+                )
         await self.module_controls.register_modules(new_mods_at_ports=new_mods_at_ports)
 
     @contextmanager
     def save_current(self) -> Iterator[None]:
         yield
 
     @property
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/backends/status_bar_state.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/backends/status_bar_state.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/backends/subsystem_manager.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/backends/subsystem_manager.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/backends/tip_presence_manager.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/backends/tip_presence_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import logging
 from functools import partial
 from typing import cast, Callable, Optional, List, Set
 from typing_extensions import TypedDict, Literal
 
-from opentrons.hardware_control.types import TipStateType, OT3Mount
+from opentrons.hardware_control.types import TipStateType, OT3Mount, InstrumentProbeType
 
 from opentrons_hardware.drivers.can_bus import CanMessenger
 from opentrons_hardware.firmware_bindings.constants import NodeId
 from opentrons_hardware.hardware_control.tip_presence import (
     TipDetector,
     types as tip_types,
 )
 from opentrons_shared_data.errors.exceptions import (
     TipDetectorNotFound,
     UnmatchedTipPresenceStates,
+    GeneralError,
 )
 
+from .ot3utils import sensor_id_for_instrument
+
 log = logging.getLogger(__name__)
 
 TipListener = Callable[[OT3Mount, bool], None]
 PipetteMountKeys = Literal["left", "right"]
 
 
 class TipDetectorByMount(TypedDict):
@@ -107,25 +110,48 @@
             listener(mount, update.presence)
 
     def current_tip_state(self, mount: OT3Mount) -> Optional[bool]:
         state = self._last_state[self._get_key(mount)]
         return state
 
     @staticmethod
-    def _get_tip_presence(results: List[tip_types.TipNotification]) -> TipStateType:
+    def _get_tip_presence(
+        results: List[tip_types.TipNotification],
+        follow_singular_sensor: Optional[InstrumentProbeType] = None,
+    ) -> TipStateType:
+        """
+        We can use follow_singular_sensor used to specify that we only care
+        about the status of one tip presence sensor on a high throughput
+        pipette, and the other is allowed to be different.
+        """
+        if follow_singular_sensor:
+            target_sensor_id = sensor_id_for_instrument(follow_singular_sensor)
+            for r in results:
+                if r.sensor == target_sensor_id:
+                    return TipStateType(r.presence)
+            # raise an error if requested sensor response isn't found
+            raise GeneralError(
+                message=f"Requested status for sensor {follow_singular_sensor} not found."
+            )
         # more than one sensor reported, we have to check if their states match
         if len(set(r.presence for r in results)) > 1:
             raise UnmatchedTipPresenceStates(
                 {int(r.sensor): int(r.presence) for r in results}
             )
         return TipStateType(results[0].presence)
 
-    async def get_tip_status(self, mount: OT3Mount) -> TipStateType:
+    async def get_tip_status(
+        self,
+        mount: OT3Mount,
+        follow_singular_sensor: Optional[InstrumentProbeType] = None,
+    ) -> TipStateType:
         detector = self.get_detector(mount)
-        return self._get_tip_presence(await detector.request_tip_status())
+        return self._get_tip_presence(
+            await detector.request_tip_status(), follow_singular_sensor
+        )
 
     def get_detector(self, mount: OT3Mount) -> TipDetector:
         detector = self._detectors[self._get_key(mount)]
         if not detector:
             raise TipDetectorNotFound(
                 message=f"Tip detector not set up for {mount} mount",
                 detail={"mount": str(mount)},
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/dev_types.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/dev_types.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/abstract_emulator.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/abstract_emulator.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/app.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/app.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/connection_handler.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/connection_handler.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/heater_shaker.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/heater_shaker.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/magdeck.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/magdeck.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/module_server/client.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/module_server/client.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/module_server/helpers.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/module_server/helpers.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/module_server/models.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/module_server/models.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/module_server/server.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/module_server/server.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/parser.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/parser.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/proxy.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/proxy.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/run_emulator.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/run_emulator.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/scripts/run_app.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/scripts/run_app.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/scripts/run_module_emulator.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/scripts/run_module_emulator.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/scripts/run_smoothie.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/scripts/run_smoothie.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/settings.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/settings.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/simulations.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/simulations.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/smoothie.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/smoothie.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/tempdeck.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/tempdeck.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/thermocycler.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/thermocycler.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/emulation/util.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/emulation/util.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/errors.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/errors.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/execution_manager.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/execution_manager.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/instrument_abc.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/instrument_abc.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/ot2/instrument_calibration.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/ot2/instrument_calibration.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/ot2/pipette.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/ot2/pipette.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,26 +22,27 @@
     load_data as load_pipette_data,
     types as pip_types,
 )
 from opentrons_shared_data.errors.exceptions import (
     InvalidLiquidClassName,
     CommandPreconditionViolated,
 )
+from opentrons_shared_data.pipette.ul_per_mm import (
+    piecewise_volume_conversion,
+    PIPETTING_FUNCTION_FALLBACK_VERSION,
+    PIPETTING_FUNCTION_LATEST_VERSION,
+)
 
 
 from opentrons.types import Point, Mount
 from opentrons.config import robot_configs
 from opentrons.config.types import RobotConfig
 from opentrons.drivers.types import MoveSplit
 from ..instrument_abc import AbstractInstrument
-from ..instrument_helpers import (
-    piecewise_volume_conversion,
-    PIPETTING_FUNCTION_FALLBACK_VERSION,
-    PIPETTING_FUNCTION_LATEST_VERSION,
-)
+
 from .instrument_calibration import (
     PipetteOffsetByPipetteMount,
     load_pipette_offset,
 )
 from opentrons.hardware_control.types import (
     CriticalPoint,
     BoardRevision,
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/ot2/pipette_handler.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/ot2/pipette_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -768,36 +768,39 @@
         increment,
     ):
         # Prechecks: ready for pickup tip and press/increment are valid
         instrument = self.get_pipette(mount)
         if instrument.has_tip:
             raise UnexpectedTipAttachError("pick_up_tip", instrument.name, mount.name)
         self._ihp_log.debug(f"Picking up tip on {mount.name}")
-
+        tip_count = instrument.nozzle_manager.current_configuration.tip_count
         if presses is None or presses < 0:
             checked_presses = instrument.pick_up_configurations.press_fit.presses
         else:
             checked_presses = presses
 
         if not increment or increment < 0:
             check_incr = instrument.pick_up_configurations.press_fit.increment
         else:
             check_incr = increment
 
-        pick_up_speed = instrument.pick_up_configurations.press_fit.speed
+        pick_up_speed = instrument.pick_up_configurations.press_fit.speed_by_tip_count[
+            tip_count
+        ]
+        pick_up_distance = (
+            instrument.pick_up_configurations.press_fit.distance_by_tip_count[tip_count]
+        )
 
         def build_presses() -> Iterator[Tuple[float, float]]:
             # Press the nozzle into the tip <presses> number of times,
             # moving further by <increment> mm after each press
             for i in range(checked_presses):
                 # move nozzle down into the tip
-                press_dist = (
-                    -1.0 * instrument.pick_up_configurations.press_fit.distance
-                    + -1.0 * check_incr * i
-                )
+
+                press_dist = -1.0 * pick_up_distance + -1.0 * check_incr * i
                 # move nozzle back up
                 backup_dist = -press_dist
                 yield (press_dist, backup_dist)
 
         def add_tip_to_instr() -> None:
             instrument.add_tip(tip_length=tip_length)
             instrument.set_current_volume(0)
@@ -811,27 +814,25 @@
                     },
                     presses=[
                         PickUpTipPressSpec(
                             current={
                                 Axis.by_mount(
                                     mount
                                 ): instrument.pick_up_configurations.press_fit.current_by_tip_count[
-                                    instrument.nozzle_manager.current_configuration.tip_count
+                                    tip_count
                                 ]
                             },
                             speed=pick_up_speed,
                             relative_down=top_types.Point(0, 0, press_dist),
                             relative_up=top_types.Point(0, 0, backup_dist),
                         )
                         for press_dist, backup_dist in build_presses()
                     ],
                     shake_off_list=self._build_pickup_shakes(instrument),
-                    retract_target=instrument.pick_up_configurations.press_fit.distance
-                    + check_incr * checked_presses
-                    + 2,
+                    retract_target=pick_up_distance + check_incr * checked_presses + 2,
                 ),
                 add_tip_to_instr,
             )
         else:
             return (
                 PickUpTipSpec(
                     plunger_prep_pos=instrument.plunger_positions.bottom,
@@ -852,17 +853,15 @@
                             speed=pick_up_speed,
                             relative_down=top_types.Point(0, 0, press_dist),
                             relative_up=top_types.Point(0, 0, backup_dist),
                         )
                         for press_dist, backup_dist in build_presses()
                     ],
                     shake_off_list=self._build_pickup_shakes(instrument),
-                    retract_target=instrument.pick_up_configurations.press_fit.distance
-                    + check_incr * checked_presses
-                    + 2,
+                    retract_target=pick_up_distance + check_incr * checked_presses + 2,
                 ),
                 add_tip_to_instr,
             )
 
     @staticmethod
     def _shake_off_tips_drop(
         tiprack_diameter: float,
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/ot3/gripper.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/ot3/gripper.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 from opentrons_shared_data.gripper import (
     GripperDefinition,
     GripForceProfile,
     Geometry,
 )
 
-RECONFIG_KEYS = {"quirks"}
+RECONFIG_KEYS = {"quirks", "grip_force_profile"}
 
 MAX_ACCEPTABLE_JAW_DISPLACEMENT: Final = 20
 
 mod_log = logging.getLogger(__name__)
 
 
 class Gripper(AbstractInstrument[GripperDefinition]):
@@ -48,14 +48,15 @@
     """
 
     def __init__(
         self,
         config: GripperDefinition,
         gripper_cal_offset: GripperCalibrationOffset,
         gripper_id: str,
+        jaw_max_offset: Optional[float] = None,
     ) -> None:
         self._config = config
         self._model = config.model
 
         self._geometry = self._config.geometry
         base_offset = Point(*self._geometry.base_offset_from_mount)
         self._jaw_center_offset = (
@@ -79,15 +80,15 @@
         self._state = GripperJawState.UNHOMED
         self._current_jaw_displacement = 0.0
         self._attached_probe: Optional[GripperProbe] = None
         self._log = mod_log.getChild(self._gripper_id)
         self._log.info(
             f"loaded: {self._model}, gripper offset: {self._calibration_offset}"
         )
-        self._jaw_max_offset: Optional[float] = None
+        self._jaw_max_offset = jaw_max_offset
 
     @property
     def grip_force_profile(self) -> GripForceProfile:
         return self._config.grip_force_profile
 
     @property
     def geometry(self) -> Geometry:
@@ -321,19 +322,21 @@
         olddict = attached_instr.config.dict()
         changed: Set[str] = set()
         for k in newdict.keys():
             if newdict[k] != olddict[k]:
                 changed.add(k)
         if changed.intersection(RECONFIG_KEYS):
             # Something has changed that requires reconfig
+            # we shoud recalibrate the jaw as well
             return (
                 Gripper(
                     new_config,
                     cal_offset,
                     attached_instr._gripper_id,
+                    None,
                 ),
                 False,
             )
         else:
             # update just the cal offset and update info
             attached_instr._calibration_offset = cal_offset
             return attached_instr, True
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/ot3/gripper_handler.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/ot3/gripper_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         og_gripper = self._gripper
         if not og_gripper:
             return
         new_gripper = Gripper(
             og_gripper.config,
             load_gripper_calibration_offset(og_gripper.gripper_id),
             og_gripper.gripper_id,
+            og_gripper._jaw_max_offset,
         )
         self._gripper = new_gripper
 
     async def reset(self) -> None:
         self._gripper = None
 
     @property
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/ot3/instrument_calibration.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/ot3/instrument_calibration.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 )
 from opentrons.calibration_storage import (
     types as cal_top_types,
     gripper_offset,
 )
 from opentrons.hardware_control.types import OT3Mount
 
-PIPETTE_OFFSET_CONSISTENCY_LIMIT: Final = 1.5
+PIPETTE_OFFSET_CONSISTENCY_LIMIT: Final = 4.0
 
 # These type aliases aid typechecking in tests that work the same on this and
 # the hardware_control.instruments.ot2 variant
 SourceType = cal_top_types.SourceType
 CalibrationStatus = cal_top_types.CalibrationStatus
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/ot3/pipette.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/ot3/pipette.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,20 +21,20 @@
     default_tip_for_liquid_class,
 )
 from opentrons_shared_data.errors.exceptions import (
     InvalidLiquidClassName,
     CommandPreconditionViolated,
     PythonException,
 )
-from ..instrument_abc import AbstractInstrument
-from ..instrument_helpers import (
+from opentrons_shared_data.pipette.ul_per_mm import (
     piecewise_volume_conversion,
     PIPETTING_FUNCTION_FALLBACK_VERSION,
     PIPETTING_FUNCTION_LATEST_VERSION,
 )
+from ..instrument_abc import AbstractInstrument
 from .instrument_calibration import (
     save_pipette_offset_calibration,
     load_pipette_offset,
     PipetteOffsetByPipetteMount,
 )
 from opentrons_shared_data.pipette.dev_types import (
     UlPerMmAction,
@@ -663,16 +663,26 @@
     ) -> Union[CamActionPickUpTipConfiguration, PressFitPickUpTipConfiguration]:
         for config in (
             self._config.pick_up_tip_configurations.press_fit,
             self._config.pick_up_tip_configurations.cam_action,
         ):
             if not config:
                 continue
-            if count in config.current_by_tip_count:
+
+            if isinstance(config, PressFitPickUpTipConfiguration) and all(
+                [
+                    config.speed_by_tip_count.get(count),
+                    config.distance_by_tip_count.get(count),
+                    config.current_by_tip_count.get(count),
+                ]
+            ):
                 return config
+            elif config.current_by_tip_count.get(count) is not None:
+                return config
+
         raise CommandPreconditionViolated(
             message=f"No pick up tip configuration for {count} tips",
         )
 
 
 def _reload_and_check_skip(
     new_config: PipetteConfigurations,
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/instruments/ot3/pipette_handler.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/instruments/ot3/pipette_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -793,23 +793,26 @@
             checked_presses = presses
 
         if not increment or increment < 0:
             check_incr = pick_up_config.increment
         else:
             check_incr = increment
 
-        pick_up_speed = pick_up_config.speed
+        pick_up_speed = pick_up_config.speed_by_tip_count[tip_count]
 
         def build_presses() -> List[TipActionMoveSpec]:
             # Press the nozzle into the tip <presses> number of times,
             # moving further by <increment> mm after each press
             press_moves = []
             for i in range(checked_presses):
                 # move nozzle down into the tip
-                press_dist = -1.0 * pick_up_config.distance + -1.0 * check_incr * i
+                press_dist = (
+                    -1.0 * pick_up_config.distance_by_tip_count[tip_count]
+                    + -1.0 * check_incr * i
+                )
                 press_moves.append(
                     TipActionMoveSpec(
                         distance=press_dist,
                         speed=pick_up_speed,
                         currents={
                             Axis.by_mount(mount): pick_up_config.current_by_tip_count[
                                 tip_count
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/module_control.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/module_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 )
 from opentrons.hardware_control.modules.module_calibration import (
     ModuleCalibrationOffset,
     load_module_calibration_offset,
     save_module_calibration_offset,
 )
 from opentrons.hardware_control.modules.types import ModuleType
+from opentrons.hardware_control.modules import SimulatingModuleAtPort
+
 from opentrons.types import Point
 from .types import AionotifyEvent, BoardRevision, OT3Mount
 from . import modules
 
 if TYPE_CHECKING:
     from .api import API
     from .ot3api import OT3API
@@ -80,27 +82,32 @@
 
     async def build_module(
         self,
         port: str,
         usb_port: types.USBPort,
         type: modules.ModuleType,
         sim_model: Optional[str] = None,
+        sim_serial_number: Optional[str] = None,
     ) -> modules.AbstractModule:
         return await modules.build(
             port=port,
             usb_port=usb_port,
             type=type,
             simulating=self._api.is_simulator,
             hw_control_loop=self._api.loop,
             execution_manager=self._api._execution_manager,
             sim_model=sim_model,
+            sim_serial_number=sim_serial_number,
         )
 
     async def unregister_modules(
-        self, mods_at_ports: List[modules.ModuleAtPort]
+        self,
+        mods_at_ports: Union[
+            List[modules.ModuleAtPort], List[modules.SimulatingModuleAtPort]
+        ],
     ) -> None:
         """
         De-register Modules.
 
         Remove any modules that are no longer found by aionotify.
         """
         removed_modules = []
@@ -122,15 +129,17 @@
             await removed_mod.cleanup()
         self._available_modules = sorted(
             self._available_modules, key=modules.AbstractModule.sort_key
         )
 
     async def register_modules(
         self,
-        new_mods_at_ports: Optional[List[modules.ModuleAtPort]] = None,
+        new_mods_at_ports: Optional[
+            Union[List[modules.ModuleAtPort], List[modules.SimulatingModuleAtPort]]
+        ] = None,
         removed_mods_at_ports: Optional[List[modules.ModuleAtPort]] = None,
     ) -> None:
         """
         Register Modules.
 
         Upon system recognition of a module being plugged in, we should
         register that module and de-register any modules that are
@@ -148,14 +157,17 @@
 
         # build new mods
         for mod in unsorted_mods_at_port:
             new_instance = await self.build_module(
                 port=mod.port,
                 usb_port=mod.usb_port,
                 type=modules.MODULE_TYPE_BY_NAME[mod.name],
+                sim_serial_number=mod.serial_number
+                if isinstance(mod, SimulatingModuleAtPort)
+                else None,
             )
             self._available_modules.append(new_instance)
             log.info(
                 f"Module {mod.name} discovered and attached"
                 f" at port {mod.port}, new_instance: {new_instance}"
             )
         self._available_modules = sorted(
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/modules/__init__.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/modules/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .utils import MODULE_TYPE_BY_NAME, build
 from .types import (
     ThermocyclerStep,
     UploadFunction,
     BundledFirmware,
     UpdateError,
     ModuleAtPort,
+    SimulatingModuleAtPort,
     ModuleType,
     ModuleModel,
     TemperatureStatus,
     MagneticStatus,
     HeaterShakerStatus,
     SpeedStatus,
     LiveData,
@@ -29,14 +30,15 @@
     "TempDeck",
     "MagDeck",
     "Thermocycler",
     "UploadFunction",
     "BundledFirmware",
     "UpdateError",
     "ModuleAtPort",
+    "SimulatingModuleAtPort",
     "HeaterShaker",
     "ModuleType",
     "ModuleModel",
     "TemperatureStatus",
     "MagneticStatus",
     "HeaterShakerStatus",
     "SpeedStatus",
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/modules/heater_shaker.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/modules/heater_shaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         port: str,
         usb_port: USBPort,
         execution_manager: ExecutionManager,
         hw_control_loop: asyncio.AbstractEventLoop,
         poll_interval_seconds: Optional[float] = None,
         simulating: bool = False,
         sim_model: Optional[str] = None,
+        sim_serial_number: Optional[str] = None,
     ) -> "HeaterShaker":
         """
         Build a HeaterShaker
 
         Args:
             port: The port to connect to
             usb_port: USB Port
@@ -67,15 +68,15 @@
             HeaterShaker instance
         """
         driver: AbstractHeaterShakerDriver
         if not simulating:
             driver = await HeaterShakerDriver.create(port=port, loop=hw_control_loop)
             poll_interval_seconds = poll_interval_seconds or POLL_PERIOD
         else:
-            driver = SimulatingDriver()
+            driver = SimulatingDriver(serial_number=sim_serial_number)
             poll_interval_seconds = poll_interval_seconds or SIMULATING_POLL_PERIOD
 
         reader = HeaterShakerReader(driver=driver)
         poller = Poller(reader=reader, interval=poll_interval_seconds)
         module = cls(
             port=port,
             usb_port=usb_port,
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/modules/lid_temp_status.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/modules/lid_temp_status.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/modules/magdeck.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/modules/magdeck.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,21 +49,24 @@
         port: str,
         usb_port: USBPort,
         execution_manager: ExecutionManager,
         hw_control_loop: asyncio.AbstractEventLoop,
         poll_interval_seconds: Optional[float] = None,
         simulating: bool = False,
         sim_model: Optional[str] = None,
+        sim_serial_number: Optional[str] = None,
     ) -> "MagDeck":
         """Factory function."""
         driver: AbstractMagDeckDriver
         if not simulating:
             driver = await MagDeckDriver.create(port=port, loop=hw_control_loop)
         else:
-            driver = SimulatingDriver(sim_model=sim_model)
+            driver = SimulatingDriver(
+                sim_model=sim_model, serial_number=sim_serial_number
+            )
 
         mod = cls(
             port=port,
             usb_port=usb_port,
             execution_manager=execution_manager,
             hw_control_loop=hw_control_loop,
             device_info=await driver.get_device_info(),
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/modules/mod_abc.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/modules/mod_abc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 import abc
 import asyncio
 import logging
 import re
-from pkg_resources import parse_version
-from typing import ClassVar, Mapping, Optional, cast, TypeVar
-
+from typing import ClassVar, Mapping, Optional, TypeVar
+from packaging.version import InvalidVersion, parse, Version
 from opentrons.config import IS_ROBOT, ROBOT_FIRMWARE_DIR
 from opentrons.drivers.rpi_drivers.types import USBPort
 
 from ..execution_manager import ExecutionManager
 from .types import BundledFirmware, UploadFunction, LiveData, ModuleType
 
 mod_log = logging.getLogger(__name__)
 
 TaskPayload = TypeVar("TaskPayload")
 
 
+def parse_fw_version(version: str) -> Version:
+    try:
+        device_version = parse(version)
+    except InvalidVersion:
+        device_version = parse("v0.0.0")
+    return device_version
+
+
 class AbstractModule(abc.ABC):
     """Defines the common methods of a module."""
 
     MODULE_TYPE: ClassVar[ModuleType]
 
     @classmethod
     @abc.abstractmethod
@@ -28,14 +35,15 @@
         port: str,
         usb_port: USBPort,
         execution_manager: ExecutionManager,
         hw_control_loop: asyncio.AbstractEventLoop,
         poll_interval_seconds: Optional[float] = None,
         simulating: bool = False,
         sim_model: Optional[str] = None,
+        sim_serial_number: Optional[str] = None,
     ) -> "AbstractModule":
         """Modules should always be created using this factory.
 
         This lets the (perhaps blocking) work of connecting to and initializing
         a module be in a place that can be async.
         """
 
@@ -83,17 +91,17 @@
 
         mod_log.info(f"no available fw file found for: {file_prefix}")
         return None
 
     def has_available_update(self) -> bool:
         """Return whether a newer firmware file is available"""
         if self.device_info and self._bundled_fw:
-            device_version = parse_version(self.device_info["version"])
-            available_version = parse_version(self._bundled_fw.version)
-            return cast(bool, available_version > device_version)
+            device_version = parse_fw_version(self.device_info["version"])
+            available_version = parse_fw_version(self._bundled_fw.version)
+            return available_version > device_version
         return False
 
     async def wait_for_is_running(self) -> None:
         if not self.is_simulated:
             await self._execution_manager.wait_for_is_running()
 
     def make_cancellable(self, task: "asyncio.Task[TaskPayload]") -> None:
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/modules/module_calibration.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/modules/module_calibration.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/modules/plate_temp_status.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/modules/plate_temp_status.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/modules/tempdeck.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/modules/tempdeck.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         port: str,
         usb_port: USBPort,
         execution_manager: ExecutionManager,
         hw_control_loop: asyncio.AbstractEventLoop,
         poll_interval_seconds: Optional[float] = None,
         simulating: bool = False,
         sim_model: Optional[str] = None,
+        sim_serial_number: Optional[str] = None,
     ) -> "TempDeck":
         """
         Build a TempDeck
 
         Args:
             port: The port to connect to
             usb_port: USB Port
@@ -56,15 +57,17 @@
             Tempdeck instance
         """
         driver: AbstractTempDeckDriver
         if not simulating:
             driver = await TempDeckDriver.create(port=port, loop=hw_control_loop)
             poll_interval_seconds = poll_interval_seconds or TEMP_POLL_INTERVAL_SECS
         else:
-            driver = SimulatingDriver(sim_model=sim_model)
+            driver = SimulatingDriver(
+                sim_model=sim_model, serial_number=sim_serial_number
+            )
             poll_interval_seconds = poll_interval_seconds or SIM_TEMP_POLL_INTERVAL_SECS
 
         reader = TempDeckReader(driver=driver)
         poller = Poller(reader=reader, interval=poll_interval_seconds)
         module = cls(
             port=port,
             usb_port=usb_port,
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/modules/thermocycler.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/modules/thermocycler.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         port: str,
         usb_port: USBPort,
         execution_manager: ExecutionManager,
         hw_control_loop: asyncio.AbstractEventLoop,
         poll_interval_seconds: Optional[float] = None,
         simulating: bool = False,
         sim_model: Optional[str] = None,
+        sim_serial_number: Optional[str] = None,
     ) -> "Thermocycler":
         """
         Build and connect to a Thermocycler
 
         Args:
             port: The port to connect to
             usb_port: USB Port
@@ -83,15 +84,15 @@
         driver: AbstractThermocyclerDriver
         if not simulating:
             driver = await ThermocyclerDriverFactory.create(
                 port=port, loop=hw_control_loop
             )
             poll_interval_seconds = poll_interval_seconds or POLLING_FREQUENCY_SEC
         else:
-            driver = SimulatingDriver(model=sim_model)
+            driver = SimulatingDriver(model=sim_model, serial_number=sim_serial_number)
             poll_interval_seconds = poll_interval_seconds or SIM_POLLING_FREQUENCY_SEC
 
         reader = ThermocyclerReader(driver=driver)
         poller = Poller(reader=reader, interval=poll_interval_seconds)
         module = cls(
             port=port,
             usb_port=usb_port,
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/modules/types.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/modules/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,14 +60,30 @@
         if isinstance(model, ThermocyclerModuleModel):
             return cls.THERMOCYCLER
         if isinstance(model, HeaterShakerModuleModel):
             return cls.HEATER_SHAKER
         if isinstance(model, MagneticBlockModel):
             return cls.MAGNETIC_BLOCK
 
+    @classmethod
+    def to_module_fixture_id(cls, module_type: ModuleType) -> str:
+        if module_type == ModuleType.THERMOCYCLER:
+            # Thermocyclers are "loaded" in B1 only
+            return "thermocyclerModuleV2Front"
+        if module_type == ModuleType.TEMPERATURE:
+            return "temperatureModuleV2"
+        if module_type == ModuleType.HEATER_SHAKER:
+            return "heaterShakerModuleV1"
+        if module_type == ModuleType.MAGNETIC_BLOCK:
+            return "magneticBlockV1"
+        else:
+            raise ValueError(
+                f"Module Type {module_type} does not have a related fixture ID."
+            )
+
 
 class MagneticModuleModel(str, Enum):
     MAGNETIC_V1: str = "magneticModuleV1"
     MAGNETIC_V2: str = "magneticModuleV2"
 
 
 class TemperatureModuleModel(str, Enum):
@@ -99,21 +115,26 @@
         try:
             return cast(ModuleModel, model_enum(model_string))
         except ValueError:
             pass
     raise ValueError(f"No such module model {model_string}")
 
 
-@dataclass
+@dataclass(kw_only=True)
 class ModuleAtPort:
     port: str
     name: str
     usb_port: USBPort = USBPort(name="", port_number=0)
 
 
+@dataclass(kw_only=True)
+class SimulatingModuleAtPort(ModuleAtPort):
+    serial_number: str
+
+
 class BundledFirmware(NamedTuple):
     """Represents a versioned firmware file, generally bundled into the fs"""
 
     version: str
     path: Path
 
     def __repr__(self) -> str:
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/modules/update.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/modules/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import logging
 import os
 from pathlib import Path
 from glob import glob
-from typing import Any, AsyncGenerator, Dict, Tuple, Optional, Union
+from typing import Any, AsyncGenerator, Dict, Tuple, Union
 from .types import UpdateError
 from .mod_abc import AbstractModule
 from opentrons.hardware_control.threaded_async_lock import ThreadedAsyncLock
 from contextlib import asynccontextmanager
 
 log = logging.getLogger(__name__)
 
@@ -19,15 +19,14 @@
     async with _update_transition_lock.lock():
         yield
 
 
 async def update_firmware(
     module: AbstractModule,
     firmware_file: Union[str, Path],
-    loop: Optional[asyncio.AbstractEventLoop],
 ) -> None:
     """Apply update of given firmware file to given module.
 
     raises an UpdateError with the reason for the failure.
     """
     async with protect_update_transition():
         flash_port_or_dfu_serial = await module.prep_for_update()
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/modules/utils.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/modules/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,22 +38,24 @@
     port: str,
     type: ModuleType,
     simulating: bool,
     usb_port: USBPort,
     hw_control_loop: asyncio.AbstractEventLoop,
     execution_manager: ExecutionManager,
     sim_model: Optional[str] = None,
+    sim_serial_number: Optional[str] = None,
 ) -> AbstractModule:
     return await _MODULE_CLS_BY_TYPE[type].build(
         port=port,
         usb_port=usb_port,
         simulating=simulating,
         hw_control_loop=hw_control_loop,
         execution_manager=execution_manager,
         sim_model=sim_model,
+        sim_serial_number=sim_serial_number,
     )
 
 
 async def disable_module(module: AbstractModule) -> None:
     """Async function to deactivate a module immediately, for error recovery."""
     if isinstance(module, HeaterShaker):
         await module.deactivate_heater(must_be_running=False)
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/motion_utilities.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/motion_utilities.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/nozzle_manager.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/nozzle_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from opentrons.types import Point
 from opentrons_shared_data.pipette.pipette_definition import (
     PipetteGeometryDefinition,
     PipetteRowDefinition,
 )
 from opentrons_shared_data.errors import ErrorCodes, GeneralError, PythonException
 
+MAXIMUM_NOZZLE_COUNT = 24
+
 
 def _nozzle_names_by_row(rows: List[PipetteRowDefinition]) -> Iterator[str]:
     for row in rows:
         for nozzle in row.ordered_nozzles:
             yield nozzle
 
 
@@ -263,14 +265,25 @@
         ]
         columns = OrderedDict(correct_columns)
 
         map_store = OrderedDict(
             (nozzle, physical_nozzles[nozzle]) for nozzle in chain(*rows.values())
         )
 
+        if (
+            NozzleConfigurationType.determine_nozzle_configuration(
+                physical_rows, rows, physical_columns, columns
+            )
+            != NozzleConfigurationType.FULL
+        ):
+            if len(rows) * len(columns) > MAXIMUM_NOZZLE_COUNT:
+                raise IncompatibleNozzleConfiguration(
+                    f"Partial Nozzle Layouts may not be configured to contain more than {MAXIMUM_NOZZLE_COUNT} channels."
+                )
+
         return cls(
             starting_nozzle=starting_nozzle,
             map_store=map_store,
             rows=rows,
             full_instrument_map_store=physical_nozzles,
             full_instrument_rows=physical_rows,
             columns=columns,
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/ot3_calibration.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/ot3_calibration.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/ot3api.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/ot3api.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,16 @@
     CriticalPoint,
     DoorState,
     DoorStateNotification,
     ErrorMessageNotification,
     HardwareEvent,
     HardwareEventHandler,
     HardwareAction,
+    HepaFanState,
+    HepaUVState,
     MotionChecks,
     SubSystem,
     PauseType,
     Axis,
     OT3AxisKind,
     OT3Mount,
     OT3AxisMap,
@@ -250,21 +252,23 @@
         (disengaged).
 
         If gripper mount is NOT the last moved mount, it's idle.
         If a 96-channel pipette is attached, the mount is idle if it's not
         the last moved mount.
         """
         realmount = OT3Mount.from_mount(mount)
-        if not self._last_moved_mount or realmount == self._last_moved_mount:
-            return False
-
-        return (
+        if realmount == OT3Mount.GRIPPER or (
             realmount == OT3Mount.LEFT
             and self._gantry_load == GantryLoad.HIGH_THROUGHPUT
-        ) or (realmount == OT3Mount.GRIPPER)
+        ):
+            ax = Axis.by_mount(realmount)
+            if ax in self.engaged_axes.keys():
+                return not self.engaged_axes[ax]
+
+        return False
 
     @property
     def door_state(self) -> DoorState:
         return self._door_state
 
     @door_state.setter
     def door_state(self, door_state: DoorState) -> None:
@@ -405,29 +409,29 @@
     async def build_hardware_simulator(
         cls,
         attached_instruments: Union[
             None,
             Dict[OT3Mount, Dict[str, Optional[str]]],
             Dict[top_types.Mount, Dict[str, Optional[str]]],
         ] = None,
-        attached_modules: Optional[List[str]] = None,
+        attached_modules: Optional[Dict[str, List[str]]] = None,
         config: Union[RobotConfig, OT3Config, None] = None,
         loop: Optional[asyncio.AbstractEventLoop] = None,
         strict_attached_instruments: bool = True,
         feature_flags: Optional[HardwareFeatureFlags] = None,
     ) -> "OT3API":
         """Build a simulating hardware controller.
 
         This method may be used both on a real robot and on dev machines.
         Multiple simulating hardware controllers may be active at one time.
         """
         if feature_flags is None:
             feature_flags = HardwareFeatureFlags()
 
-        checked_modules = attached_modules or []
+        checked_modules = attached_modules or {}
 
         checked_loop = use_or_initialize_loop(loop)
         if not isinstance(config, OT3Config):
             checked_config = robot_configs.load_ot3()
         else:
             checked_config = config
 
@@ -644,20 +648,24 @@
             OT3Mount.LEFT: self.attached_pipettes[top_types.Mount.LEFT],
             OT3Mount.RIGHT: self.attached_pipettes[top_types.Mount.RIGHT],
             OT3Mount.GRIPPER: self.attached_gripper,
         }
 
     # TODO (spp, 2023-01-31): add unit tests
     async def cache_instruments(
-        self, require: Optional[Dict[top_types.Mount, PipetteName]] = None
+        self,
+        require: Optional[Dict[top_types.Mount, PipetteName]] = None,
+        skip_if_would_block: bool = False,
     ) -> None:
         """
         Scan the attached instruments, take necessary configuration actions,
         and set up hardware controller internal state if necessary.
         """
+        if skip_if_would_block and self._motion_lock.locked():
+            return
         async with self._motion_lock:
             skip_configure = await self._cache_instruments(require)
             if not skip_configure or not self._configured_since_update:
                 self._log.info("Reconfiguring instrument cache")
                 await self._configure_instruments()
 
     async def _cache_instruments(  # noqa: C901
@@ -1307,37 +1315,41 @@
         in :py:attr:`_last_moved_mount`. Also unconditionally update
         :py:attr:`_last_moved_mount` to contain `mount`.
 
         Disengage the 96-channel and gripper mount if retracted. Re-engage
         the 96-channel or gripper mount if it is about to move.
         """
         last_moved = self._last_moved_mount
-        if self.is_idle_mount(mount):
-            # home the left/gripper mount if it is current disengaged
-            await self.home_z(mount)
-
-        if mount != last_moved and last_moved:
-            await self.retract(last_moved, 10)
-
-            # disengage Axis.Z_L motor and engage the brake to lower power
-            # consumption and reduce the chance of the 96-channel pipette dropping
-            if (
-                self.gantry_load == GantryLoad.HIGH_THROUGHPUT
-                and last_moved == OT3Mount.LEFT
-            ):
-                await self.disengage_axes([Axis.Z_L])
+        # if gripper exists and it's not the moving mount, it should retract
+        if (
+            self.has_gripper()
+            and mount != OT3Mount.GRIPPER
+            and not self.is_idle_mount(OT3Mount.GRIPPER)
+        ):
+            await self.retract(OT3Mount.GRIPPER, 10)
+            await self.disengage_axes([Axis.Z_G])
+            await self.idle_gripper()
 
-            # disegnage Axis.Z_G when we can to reduce the chance of
-            # the gripper dropping
-            if last_moved == OT3Mount.GRIPPER:
-                await self.disengage_axes([Axis.Z_G])
+        # if 96-channel pipette is attached and not being moved, it should retract
+        if (
+            mount != OT3Mount.LEFT
+            and self._gantry_load == GantryLoad.HIGH_THROUGHPUT
+            and not self.is_idle_mount(OT3Mount.LEFT)
+        ):
+            await self.retract(OT3Mount.LEFT, 10)
+            await self.disengage_axes([Axis.Z_L])
 
-        if mount != OT3Mount.GRIPPER:
-            await self.idle_gripper()
+        # if the last moved mount is not covered in neither of the above scenario,
+        # simply retract the last moved mount
+        if last_moved and not self.is_idle_mount(last_moved) and mount != last_moved:
+            await self.retract(last_moved, 10)
 
+        # finally, home the current left/gripper mount to prepare for movement
+        if self.is_idle_mount(mount):
+            await self.home_z(mount)
         self._last_moved_mount = mount
 
     async def prepare_for_mount_movement(
         self, mount: Union[top_types.Mount, OT3Mount]
     ) -> None:
         """Retract the idle mount if necessary."""
         realmount = OT3Mount.from_mount(mount)
@@ -1469,14 +1481,30 @@
         self, axis: Axis
     ) -> Tuple[OT3AxisMap[float], OT3AxisMap[float]]:
         origin = await self._backend.update_position()
         origin_pos = {axis: origin[axis]}
         target_pos = {axis: self._backend.home_position()[axis]}
         return origin_pos, target_pos
 
+    async def _enable_before_update_estimation(self, axis: Axis) -> None:
+        enabled = await self._backend.is_motor_engaged(axis)
+
+        if not enabled:
+            if axis == Axis.Z_L and self.gantry_load == GantryLoad.HIGH_THROUGHPUT:
+                # we're here if the left mount has been idle and the brake is engaged
+                # we want to temporarily increase its hold current to prevent the z
+                # stage from dropping when switching off the ebrake
+                async with self._backend.increase_z_l_hold_current():
+                    await self.engage_axes([axis])
+            else:
+                await self.engage_axes([axis])
+
+        # now that motor is enabled, we can update position estimation
+        await self._update_position_estimation([axis])
+
     @_adjust_high_throughput_z_current
     async def _home_axis(self, axis: Axis) -> None:
         """
         Perform home; base on axis motor/encoder statuses, shorten homing time
         if possible.
 
         1. If stepper position status is valid, move directly to the home position.
@@ -1490,35 +1518,31 @@
         switch will not be triggered.
         """
 
         # G, Q should be handled in the backend through `self._home()`
         assert axis not in [Axis.G, Axis.Q]
 
         encoder_ok = self._backend.check_encoder_status([axis])
-        motor_ok = self._backend.check_motor_status([axis])
-
         if encoder_ok:
-            # ensure stepper position can be updated after boot
-            if axis == Axis.Z_L and self.gantry_load == GantryLoad.HIGH_THROUGHPUT:
-                # we're here if the left mount has been idle and the brake is engaged
-                # we want to temporarily increase its hold current to prevent the z
-                # stage from dropping when switching off the ebrake
-                async with self._backend.increase_z_l_hold_current():
-                    await self.engage_axes([axis])
-            else:
-                await self.engage_axes([axis])
-            await self._update_position_estimation([axis])
-            # refresh motor and encoder statuses after position estimation update
-            motor_ok = self._backend.check_motor_status([axis])
-            encoder_ok = self._backend.check_encoder_status([axis])
+            # enable motor (if needed) and update estimation
+            await self._enable_before_update_estimation(axis)
+
+        # refresh motor status after position estimation update
+        motor_ok = self._backend.check_motor_status([axis])
 
         if Axis.to_kind(axis) == OT3AxisKind.P:
             await self._set_plunger_current_and_home(axis, motor_ok, encoder_ok)
             return
 
+        # TODO: (ba, 2024-04-19): We need to explictly engage the axis and enable
+        # the motor when we are attempting to move. This should be already
+        # happening but something on the firmware is either not enabling the motor or
+        # disabling the motor.
+        await self.engage_axes([axis])
+
         # we can move to safe home distance!
         if encoder_ok and motor_ok:
             origin, target_pos = await self._retrieve_home_position(axis)
             if Axis.to_kind(axis) == OT3AxisKind.Z:
                 axis_home_dist = self._config.safe_home_distance
             else:
                 # FIXME: (AA 2/15/23) This is a temporary workaround because of
@@ -1537,30 +1561,29 @@
             await self._backend.home([axis], self.gantry_load)
         else:
             # both stepper and encoder positions are invalid, must home
             await self._backend.home([axis], self.gantry_load)
 
     async def _home(self, axes: Sequence[Axis]) -> None:
         """Home one axis at a time."""
-        async with self._motion_lock:
-            for axis in axes:
-                try:
-                    if axis == Axis.G:
-                        await self.home_gripper_jaw()
-                    elif axis == Axis.Q:
-                        await self._backend.home([axis], self.gantry_load)
-                    else:
-                        await self._home_axis(axis)
-                except BaseException as e:
-                    self._log.exception(f"Homing failed: {e}")
-                    self._current_position.clear()
-                    raise
+        for axis in axes:
+            try:
+                if axis == Axis.G:
+                    await self.home_gripper_jaw()
+                elif axis == Axis.Q:
+                    await self._backend.home([axis], self.gantry_load)
                 else:
-                    await self._cache_current_position()
-                    await self._cache_encoder_position()
+                    await self._home_axis(axis)
+            except BaseException as e:
+                self._log.exception(f"Homing failed: {e}")
+                self._current_position.clear()
+                raise
+            else:
+                await self._cache_current_position()
+                await self._cache_encoder_position()
 
     @ExecutionManagerProvider.wait_for_running
     async def home(
         self,
         axes: Optional[List[Axis]] = None,
         skip: Optional[List[Axis]] = None,
     ) -> None:
@@ -1583,15 +1606,16 @@
 
         home_seq = [
             ax
             for ax in AXES_IN_HOMING_ORDER
             if (ax in checked_axes and self._backend.axis_is_present(ax))
         ]
         self._log.info(f"home was called with {axes} generating sequence {home_seq}")
-        await self._home(home_seq)
+        async with self._motion_lock:
+            await self._home(home_seq)
 
     def get_engaged_axes(self) -> Dict[Axis, bool]:
         """Which axes are engaged and holding."""
         return self._backend.engaged_axes()
 
     @property
     def engaged_axes(self) -> Dict[Axis, bool]:
@@ -1627,24 +1651,32 @@
         OT-2 uses this function to recover from a stall. In order to keep
         the behaviors between the two robots similar, retract_axis on the FLEX
         will call home if the stepper position is inaccurate.
         """
         motor_ok = self._backend.check_motor_status([axis])
         encoder_ok = self._backend.check_encoder_status([axis])
 
-        if motor_ok and encoder_ok:
-            # we can move to the home position without checking the limit switch
-            origin = await self._backend.update_position()
-            target_pos = {axis: self._backend.home_position()[axis]}
-            await self._backend.move(origin, target_pos, 400, HWStopCondition.none)
-        else:
-            # home the axis
-            await self._home_axis(axis)
-        await self._cache_current_position()
-        await self._cache_encoder_position()
+        async with self._motion_lock:
+            if motor_ok and encoder_ok:
+                # TODO: (ba, 2024-04-19): We need to explictly engage the axis and enable
+                # the motor when we are attempting to move. This should be already
+                # happening but something on the firmware is either not enabling the motor or
+                # disabling the motor.
+                await self.engage_axes([axis])
+
+                # we can move to the home position without checking the limit switch
+                origin = await self._backend.update_position()
+                target_pos = {axis: self._backend.home_position()[axis]}
+                await self._backend.move(origin, target_pos, 400, HWStopCondition.none)
+            else:
+                # home the axis
+                await self._home_axis(axis)
+
+            await self._cache_current_position()
+            await self._cache_encoder_position()
 
     # Gantry/frame (i.e. not pipette) config API
     @property
     def config(self) -> OT3Config:
         """Get the robot's configuration object.
 
         :returns .RobotConfig: The object.
@@ -2036,51 +2068,60 @@
             yield
         finally:
             await self.home_gear_motors()
 
     async def get_tip_presence_status(
         self,
         mount: Union[top_types.Mount, OT3Mount],
+        follow_singular_sensor: Optional[InstrumentProbeType] = None,
     ) -> TipStateType:
         """
         Check tip presence status. If a high throughput pipette is present,
         move the tip motors down before checking the sensor status.
         """
         async with self._motion_lock:
             real_mount = OT3Mount.from_mount(mount)
             async with contextlib.AsyncExitStack() as stack:
                 if (
                     real_mount == OT3Mount.LEFT
                     and self._gantry_load == GantryLoad.HIGH_THROUGHPUT
                 ):
                     await stack.enter_async_context(self._high_throughput_check_tip())
-                result = await self._backend.get_tip_status(real_mount)
+                result = await self._backend.get_tip_status(
+                    real_mount, follow_singular_sensor
+                )
             return result
 
     async def verify_tip_presence(
-        self, mount: Union[top_types.Mount, OT3Mount], expected: TipStateType
+        self,
+        mount: Union[top_types.Mount, OT3Mount],
+        expected: TipStateType,
+        follow_singular_sensor: Optional[InstrumentProbeType] = None,
     ) -> None:
         real_mount = OT3Mount.from_mount(mount)
-        status = await self.get_tip_presence_status(real_mount)
+        status = await self.get_tip_presence_status(real_mount, follow_singular_sensor)
         if status != expected:
             raise FailedTipStateCheck(expected, status.value)
 
     async def _force_pick_up_tip(
         self, mount: OT3Mount, pipette_spec: TipActionSpec
     ) -> None:
         for press in pipette_spec.tip_action_moves:
             async with self._backend.motor_current(run_currents=press.currents):
-                target_down = target_position_from_relative(
+                target = target_position_from_relative(
                     mount, top_types.Point(z=press.distance), self._current_position
                 )
-                await self._move(target_down, speed=press.speed, expect_stalls=True)
-            if press.distance < 0:
-                # we expect a stall has happened during a downward movement into the tiprack, so
-                # we want to update the motor estimation
-                await self._update_position_estimation([Axis.by_mount(mount)])
+                if press.distance < 0:
+                    # we expect a stall has happened during a downward movement into the tiprack, so
+                    # we want to update the motor estimation
+                    await self._move(target, speed=press.speed, expect_stalls=True)
+                    await self._update_position_estimation([Axis.by_mount(mount)])
+                else:
+                    # we should not ignore stalls that happen during the retract part of the routine
+                    await self._move(target, speed=press.speed, expect_stalls=False)
 
     async def _tip_motor_action(
         self, mount: OT3Mount, pipette_spec: List[TipActionMoveSpec]
     ) -> None:
         # currents should be the same for each move in tip motor pickup
         assert [move.currents == pipette_spec[0].currents for move in pipette_spec]
         currents = pipette_spec[0].currents
@@ -2111,14 +2152,16 @@
         """Pick up tip from current location."""
         realmount = OT3Mount.from_mount(mount)
         instrument = self._pipette_handler.get_pipette(realmount)
 
         def add_tip_to_instr() -> None:
             instrument.add_tip(tip_length=tip_length)
             instrument.set_current_volume(0)
+            if isinstance(self._backend, OT3Simulator):
+                self._backend._update_tip_state(realmount, True)
 
         await self._move_to_plunger_bottom(realmount, rate=1.0)
         if (
             self.gantry_load == GantryLoad.HIGH_THROUGHPUT
             and instrument.nozzle_manager.current_configuration.configuration
             == NozzleConfigurationType.FULL
         ):
@@ -2211,14 +2254,17 @@
             await self.move_rel(mount, shake[0], speed=shake[1])
 
         # home mount axis
         if home_after:
             await self._home([Axis.by_mount(mount)])
 
         _remove_tips()
+        # call this in case we're simulating
+        if isinstance(self._backend, OT3Simulator):
+            self._backend._update_tip_state(realmount, False)
 
     async def clean_up(self) -> None:
         """Get the API ready to stop cleanly."""
         await self._backend.clean_up()
 
     def critical_point_for(
         self,
@@ -2550,15 +2596,16 @@
         plunger_direction = -1 if probe_settings.aspirate_while_sensing else 1
         await self._backend.liquid_probe(
             mount,
             probe_settings.max_z_distance,
             probe_settings.mount_speed,
             (probe_settings.plunger_speed * plunger_direction),
             probe_settings.sensor_threshold_pascals,
-            probe_settings.log_pressure,
+            probe_settings.output_option,
+            probe_settings.data_files,
             probe_settings.auto_zero_sensor,
             probe_settings.num_baseline_reads,
             probe=probe if probe else InstrumentProbeType.PRIMARY,
         )
         end_pos = await self.gantry_position(mount, refresh=True)
         await self.move_to(mount, probe_start_pos)
         return end_pos.z
@@ -2683,7 +2730,25 @@
 
         Returns the estop status after clearing the status."""
         self._backend.estop_acknowledge_and_clear()
         return self.estop_status
 
     def get_estop_state(self) -> EstopState:
         return self._backend.get_estop_state()
+
+    async def set_hepa_fan_state(
+        self, turn_on: bool = False, duty_cycle: int = 75
+    ) -> bool:
+        """Sets the state and duty cycle of the Hepa/UV module."""
+        return await self._backend.set_hepa_fan_state(turn_on, duty_cycle)
+
+    async def get_hepa_fan_state(self) -> Optional[HepaFanState]:
+        return await self._backend.get_hepa_fan_state()
+
+    async def set_hepa_uv_state(
+        self, turn_on: bool = False, uv_duration_s: int = 900
+    ) -> bool:
+        """Sets the state and duration (seconds) of the UV light for the Hepa/UV module."""
+        return await self._backend.set_hepa_uv_state(turn_on, uv_duration_s)
+
+    async def get_hepa_uv_state(self) -> Optional[HepaUVState]:
+        return await self._backend.get_hepa_uv_state()
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/pause_manager.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/pause_manager.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/poller.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/poller.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/__init__.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/calibratable.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/calibratable.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/chassis_accessory_manager.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/chassis_accessory_manager.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/configurable.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/configurable.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/event_sourcer.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/event_sourcer.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/execution_controllable.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/execution_controllable.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/flex_calibratable.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/flex_calibratable.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/flex_instrument_configurer.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/flex_instrument_configurer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Flex-specific extensions to instrument configuration."""
-from typing import Union
+from typing import Union, Optional
 from typing_extensions import Protocol
 
 from .types import MountArgType
 
 from opentrons.hardware_control.dev_types import (
     PipetteStateDict,
 )
 from opentrons.hardware_control.types import (
     TipStateType,
+    InstrumentProbeType,
 )
 from opentrons.hardware_control.instruments.ot3.instrument_calibration import (
     PipetteOffsetSummary,
     GripperCalibrationOffset,
 )
 
 
@@ -38,11 +39,14 @@
 
         If a high throughput pipette is present,
         move the tip motors down before checking the sensor status.
         """
         ...
 
     async def verify_tip_presence(
-        self, mount: MountArgType, expected: TipStateType
+        self,
+        mount: MountArgType,
+        expected: TipStateType,
+        follow_singular_sensor: Optional[InstrumentProbeType] = None,
     ) -> None:
         """Check tip presence status and raise if it does not match `expected`."""
         ...
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/gripper_controller.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/gripper_controller.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/hardware_manager.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/hardware_manager.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/identifiable.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/identifiable.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/instrument_configurer.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/instrument_configurer.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         mount: If specified, reset that mount. If not specified, reset both
         """
         ...
 
     async def cache_instruments(
         self,
         require: Optional[Dict[Mount, PipetteName]] = None,
+        skip_if_would_block: bool = False,
     ) -> None:
         """
         Scan the attached instruments, take necessary configuration actions,
         and set up hardware controller internal state if necessary.
 
         require: If specified, the require should be a dict of mounts to
                  instrument names describing the instruments expected to be
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/liquid_handler.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/liquid_handler.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/motion_controller.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/motion_controller.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/protocols/types.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/protocols/types.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/robot_calibration.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/robot_calibration.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/scripts/gripper_control.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/scripts/gripper_control.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/scripts/repl.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/scripts/repl.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/simulator_setup.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/simulator_setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,73 +18,87 @@
 class ModuleCall:
     function_name: str
     args: List[Any] = field(default_factory=list)
     kwargs: Dict[str, Any] = field(default_factory=dict)
 
 
 @dataclass(frozen=True)
+class ModuleItem:
+    serial_number: str
+    calls: List[ModuleCall] = field(default_factory=list)
+
+
+@dataclass(frozen=True)
 class OT2SimulatorSetup:
     machine: Literal["OT-2 Standard"] = "OT-2 Standard"
     attached_instruments: Dict[Mount, Dict[str, Optional[str]]] = field(
         default_factory=dict
     )
-    attached_modules: Dict[str, List[ModuleCall]] = field(default_factory=dict)
+    attached_modules: Dict[str, List[ModuleItem]] = field(default_factory=dict)
     config: Optional[RobotConfig] = None
     strict_attached_instruments: bool = True
 
 
 @dataclass(frozen=True)
 class OT3SimulatorSetup:
     machine: Literal["OT-3 Standard"] = "OT-3 Standard"
     attached_instruments: Dict[OT3Mount, Dict[str, Optional[str]]] = field(
         default_factory=dict
     )
-    attached_modules: Dict[str, List[ModuleCall]] = field(default_factory=dict)
+    attached_modules: Dict[str, List[ModuleItem]] = field(default_factory=dict)
     config: Optional[OT3Config] = None
     strict_attached_instruments: bool = True
 
 
 SimulatorSetup = Union[OT2SimulatorSetup, OT3SimulatorSetup]
 
 
 async def _simulator_for_setup(
     setup: SimulatorSetup, loop: Optional[asyncio.AbstractEventLoop]
 ) -> HardwareControlAPI:
     if setup.machine == "OT-2 Standard":
         return await API.build_hardware_simulator(
             attached_instruments=setup.attached_instruments,
-            attached_modules=list(setup.attached_modules.keys()),
+            attached_modules={
+                k: [m.serial_number for m in v]
+                for k, v in setup.attached_modules.items()
+            },
             config=setup.config,
             strict_attached_instruments=setup.strict_attached_instruments,
             loop=loop,
             feature_flags=HardwareFeatureFlags.build_from_ff(),
         )
     else:
         from opentrons.hardware_control.ot3api import OT3API
 
         return await OT3API.build_hardware_simulator(
             attached_instruments=setup.attached_instruments,
-            attached_modules=list(setup.attached_modules.keys()),
+            attached_modules={
+                k: [m.serial_number for m in v]
+                for k, v in setup.attached_modules.items()
+            },
             config=setup.config,
             strict_attached_instruments=setup.strict_attached_instruments,
             loop=loop,
             feature_flags=HardwareFeatureFlags.build_from_ff(),
         )
 
 
 async def create_simulator(
     setup: SimulatorSetup, loop: Optional[asyncio.AbstractEventLoop] = None
 ) -> HardwareControlAPI:
     """Create a simulator"""
     simulator = await _simulator_for_setup(setup, loop)
     for attached_module in simulator.attached_modules:
-        calls = setup.attached_modules[attached_module.name()]
-        for call in calls:
-            f = getattr(attached_module, call.function_name)
-            await f(*call.args, **call.kwargs)
+        modules = setup.attached_modules[attached_module.name()]
+        for module in modules:
+            if module.serial_number == attached_module.device_info.get("serial"):
+                for call in module.calls:
+                    f = getattr(attached_module, call.function_name)
+                    await f(*call.args, **call.kwargs)
 
     return simulator
 
 
 async def load_simulator(
     path: Path, loop: Optional[asyncio.AbstractEventLoop] = None
 ) -> HardwareControlAPI:
@@ -95,44 +109,51 @@
 def _thread_manager_for_setup(
     setup: SimulatorSetup,
 ) -> ThreadManager[HardwareControlAPI]:
     if setup.machine == "OT-2 Standard":
         return ThreadManager(
             API.build_hardware_simulator,
             attached_instruments=setup.attached_instruments,
-            attached_modules=list(setup.attached_modules.keys()),
+            attached_modules={
+                k: [m.serial_number for m in v]
+                for k, v in setup.attached_modules.items()
+            },
             config=setup.config,
             strict_attached_instruments=setup.strict_attached_instruments,
             feature_flags=HardwareFeatureFlags.build_from_ff(),
         )
     else:
         from opentrons.hardware_control.ot3api import OT3API
 
         return ThreadManager(
             OT3API.build_hardware_simulator,
             attached_instruments=setup.attached_instruments,
-            attached_modules=list(setup.attached_modules.keys()),
+            attached_modules={
+                k: [m.serial_number for m in v]
+                for k, v in setup.attached_modules.items()
+            },
             config=setup.config,
             strict_attached_instruments=setup.strict_attached_instruments,
             feature_flags=HardwareFeatureFlags.build_from_ff(),
         )
 
 
 async def create_simulator_thread_manager(
     setup: SimulatorSetup,
 ) -> ThreadManager[HardwareControlAPI]:
     """Create a simulator thread manager from a loaded config."""
     thread_manager = _thread_manager_for_setup(setup)
     await thread_manager.managed_thread_ready_async()
 
     for attached_module in thread_manager.wrapped().attached_modules:
-        calls = setup.attached_modules[attached_module.name()]
-        for call in calls:
-            f = getattr(attached_module, call.function_name)
-            await f(*call.args, **call.kwargs)
+        modules = setup.attached_modules[attached_module.name()]
+        for module in modules:
+            for call in module.calls:
+                f = getattr(attached_module, call.function_name)
+                await f(*call.args, **call.kwargs)
 
     return thread_manager
 
 
 async def load_simulator_thread_manager(
     path: Path,
 ) -> ThreadManager[HardwareControlAPI]:
@@ -184,19 +205,40 @@
 def _prepare_for_simulator_setup(key: str, value: Dict[str, Any]) -> Any:
     """Convert value to a SimulatorSetup"""
     if key == "attached_instruments" and value:
         return {Mount[mount.upper()]: data for (mount, data) in value.items()}
     if key == "config" and value:
         return robot_configs.build_config_ot2(value)
     if key == "attached_modules" and value:
-        return {k: [ModuleCall(**data) for data in v] for (k, v) in value.items()}
+        attached_modules: Dict[str, List[ModuleItem]] = {}
+        for key, item in value.items():
+            for obj in item:
+                attached_modules.setdefault(key, []).append(
+                    ModuleItem(
+                        serial_number=obj["serial_number"],
+                        calls=[ModuleCall(**data) for data in obj["calls"]],
+                    )
+                )
+
+        return attached_modules
+
     return value
 
 
 def _prepare_for_ot3_simulator_setup(key: str, value: Dict[str, Any]) -> Any:
     if key == "attached_instruments" and value:
         return {OT3Mount[mount.upper()]: data for (mount, data) in value.items()}
     if key == "config" and value:
         return robot_configs.build_config_ot3(value)
     if key == "attached_modules" and value:
-        return {k: [ModuleCall(**data) for data in v] for (k, v) in value.items()}
+        attached_modules: Dict[str, List[ModuleItem]] = {}
+        for key, item in value.items():
+            for obj in item:
+                attached_modules.setdefault(key, []).append(
+                    ModuleItem(
+                        serial_number=obj["serial_number"],
+                        calls=[ModuleCall(**data) for data in obj["calls"]],
+                    )
+                )
+
+        return attached_modules
     return value
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/thread_manager.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/thread_manager.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/threaded_async_lock.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/threaded_async_lock.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/types.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,14 +388,27 @@
 @dataclass
 class EstopOverallStatus:
     state: EstopState
     left_physical_state: EstopPhysicalStatus
     right_physical_state: EstopPhysicalStatus
 
 
+@dataclass
+class HepaFanState:
+    fan_on: bool
+    duty_cycle: int
+
+
+@dataclass
+class HepaUVState:
+    light_on: bool
+    uv_duration_s: int
+    remaining_time_s: int
+
+
 @dataclass(frozen=True)
 class DoorStateNotification:
     event: Literal[
         HardwareEventType.DOOR_SWITCH_CHANGE
     ] = HardwareEventType.DOOR_SWITCH_CHANGE
     new_state: DoorState = DoorState.CLOSED
 
@@ -607,14 +620,15 @@
     HOLDING = enum.auto()
     #: the gripper is in position-control mode
 
 
 class InstrumentProbeType(enum.Enum):
     PRIMARY = enum.auto()
     SECONDARY = enum.auto()
+    BOTH = enum.auto()
 
 
 class GripperProbe(enum.Enum):
     FRONT = enum.auto()
     REAR = enum.auto()
 
     @classmethod
```

### Comparing `opentrons-7.2.2a3/src/opentrons/hardware_control/util.py` & `opentrons-7.3.0a0/src/opentrons/hardware_control/util.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/legacy_broker.py` & `opentrons-7.3.0a0/src/opentrons/legacy_broker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # noqa: D100
 
 from __future__ import annotations
 import logging
 from typing import Callable, Dict, List
 from typing_extensions import Literal
 
-from opentrons.commands import types
+from opentrons.legacy_commands import types
 
 
 MODULE_LOG = logging.getLogger(__name__)
 
 
 class LegacyBroker:
     """A pub/sub message broker.
 
     Deprecated:
         Use the newer, more generic `opentrons.utils.Broker` class instead.
-        This class is coupled to old types from `opentrons.commands`.
+        This class is coupled to old types from `opentrons.legacy_commands`.
         https://opentrons.atlassian.net/browse/RSS-270
     """
 
     def __init__(self) -> None:
         self.subscriptions: Dict[
             Literal["command"],
             List[Callable[[types.CommandMessage], None]],
```

### Comparing `opentrons-7.2.2a3/src/opentrons/motion_planning/__init__.py` & `opentrons-7.3.0a0/src/opentrons/motion_planning/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/motion_planning/adjacent_slots_getters.py` & `opentrons-7.3.0a0/src/opentrons/motion_planning/adjacent_slots_getters.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/motion_planning/deck_conflict.py` & `opentrons-7.3.0a0/src/opentrons/motion_planning/deck_conflict.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 
 
 @dataclass
 class TrashBin:
     """A non-labware trash bin (loaded via api level 2.16 and above)."""
 
     name_for_errors: str
+    highest_z: float
 
 
 @dataclass
 class _Module:
     name_for_errors: str
     highest_z_including_labware: float
 
@@ -134,17 +135,15 @@
             if item.uri in self.allowed_labware:
                 return True
             else:
                 return item.highest_z < self.max_height
         elif isinstance(item, _Module):
             return item.highest_z_including_labware < self.max_height
         elif isinstance(item, TrashBin):
-            # Since this is a restriction for OT-2 only and OT-2 trashes exceeded the height limit, always return False
-            # TODO(jbl 2024-01-16) Include trash height and use that for check for more robustness
-            return False
+            return item.highest_z < self.max_height
 
 
 class _NoModule(NamedTuple):
     """No module of any kind is allowed in this slot."""
 
     location: DeckSlotName
     source_item: DeckItem
```

### Comparing `opentrons-7.2.2a3/src/opentrons/motion_planning/errors.py` & `opentrons-7.3.0a0/src/opentrons/motion_planning/errors.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/motion_planning/types.py` & `opentrons-7.3.0a0/src/opentrons/motion_planning/types.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/motion_planning/waypoints.py` & `opentrons-7.3.0a0/src/opentrons/motion_planning/waypoints.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/ordered_set.py` & `opentrons-7.3.0a0/src/opentrons/ordered_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,32 +77,32 @@
         self, default_value: _DefaultValueT
     ) -> Union[_SetElementT, _DefaultValueT]:
         ...
 
     def head(
         self, default_value: Union[_DefaultValueT, _NOT_SPECIFIED] = _NOT_SPECIFIED()
     ) -> Union[_SetElementT, _DefaultValueT]:
-        """Get the head of the set.
+        """Get the head (oldest-added element) of the set.
 
         Args:
             default_value: A value to return if set is empty.
 
         Returns:
             The head of the set, or the default value, if specified.
 
         Raises:
             IndexError: set is empty and default was not specified.
         """
         try:
-            return next(iter(self))
-        except StopIteration as e:
+            return next(iter(self._elements))
+        except StopIteration:
             if isinstance(default_value, _NOT_SPECIFIED):
-                raise IndexError("Set is empty") from e
-
-        return default_value
+                raise IndexError("Set is empty") from None
+            else:
+                return default_value
 
     def __iter__(self) -> Iterator[_SetElementT]:
         """Enable iteration over all elements in the set.
 
         Elements are returned in the order they were added, oldest first.
         """
         return iter(self._elements)
@@ -126,7 +126,13 @@
         self, other: Union[OrderedSet[_SetElementT], Set[_SetElementT]]
     ) -> OrderedSet[_SetElementT]:
         """Return this set, without any elements that appear in `other`.
 
         The elements that aren't removed retain their original relative order.
         """
         return OrderedSet(e for e in self if e not in other)
+
+    def __repr__(self) -> str:  # noqa: D105
+        # Use repr() on the keys view in case it's super long and Python is smart
+        # enough to abbreviate it.
+        elements_str = repr(self._elements.keys())
+        return f"OrderedSet({elements_str})"
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/__init__.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,22 +18,23 @@
     ModuleContext,
     ThermocyclerContext,
     MagneticModuleContext,
     TemperatureModuleContext,
     HeaterShakerContext,
     MagneticBlockContext,
 )
+from .disposal_locations import TrashBin, WasteChute
 from ._liquid import Liquid
 from ._types import OFF_DECK
-from ._trash_bin import TrashBin
-from ._waste_chute import WasteChute
 from ._nozzle_layout import (
     COLUMN,
     ALL,
 )
+from ._parameters import Parameters
+from ._parameter_context import ParameterContext
 
 from .create_protocol_context import (
     create_protocol_context,
     ProtocolEngineCoreRequiredError,
 )
 
 __all__ = [
@@ -45,19 +46,21 @@
     "ModuleContext",
     "InstrumentContext",
     "TemperatureModuleContext",
     "MagneticModuleContext",
     "ThermocyclerContext",
     "HeaterShakerContext",
     "MagneticBlockContext",
+    "ParameterContext",
     "Labware",
     "TrashBin",
     "WasteChute",
     "Well",
     "Liquid",
+    "Parameters",
     "COLUMN",
     "ALL",
     "OFF_DECK",
     # For internal Opentrons use only:
     "create_protocol_context",
     "ProtocolEngineCoreRequiredError",
 ]
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/_nozzle_layout.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/_nozzle_layout.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/_types.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/_types.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/config.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/config.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/__init__.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/common.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/common.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/core_map.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/core_map.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/__init__.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .protocol import ProtocolCore
 from .instrument import InstrumentCore
 from .labware import LabwareCore
 from .module_core import ModuleCore
 from .well import WellCore
 
 ENGINE_CORE_API_VERSION: Final = APIVersion(2, 14)
+SET_OFFSET_RESTORED_API_VERSION: Final = APIVersion(2, 18)
 
 __all__ = [
     "ENGINE_CORE_API_VERSION",
     "ProtocolCore",
     "InstrumentCore",
     "LabwareCore",
     "WellCore",
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/deck_conflict.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/deck_conflict.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,16 @@
     DropTipWellLocation,
 )
 from opentrons.protocol_engine.errors.exceptions import LabwareNotLoadedOnModuleError
 from opentrons.protocol_engine.types import (
     StagingSlotLocation,
 )
 from opentrons.types import DeckSlotName, StagingSlotName, Point
+from ...disposal_locations import TrashBin, WasteChute
 from . import point_calculations
-from ..._trash_bin import TrashBin
-from ..._waste_chute import WasteChute
 
 if TYPE_CHECKING:
     from ...labware import Labware
 
 
 class PartialTipMovementNotAllowedError(MotionPlanningFailureError):
     """Error raised when trying to perform a partial tip movement to an illegal location."""
@@ -586,15 +585,17 @@
 
 def _map_disposal_location(
     disposal_location: Union[Labware, WasteChute, TrashBin],
 ) -> Optional[Tuple[DeckSlotName, wrapped_deck_conflict.DeckItem]]:
     if isinstance(disposal_location, TrashBin):
         return (
             disposal_location.location,
-            wrapped_deck_conflict.TrashBin(name_for_errors="trash bin"),
+            wrapped_deck_conflict.TrashBin(
+                name_for_errors="trash bin", highest_z=disposal_location.height
+            ),
         )
     else:
         return None
 
 
 def _deck_slot_to_int(deck_slot_location: DeckSlotLocation) -> int:
     return deck_slot_location.slotName.as_int()
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/exceptions.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/exceptions.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/instrument.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/instrument.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,21 @@
 from opentrons.protocol_engine.errors.exceptions import TipNotAttachedError
 from opentrons.protocol_engine.clients import SyncClient as EngineClient
 from opentrons.protocols.api_support.definitions import MAX_SUPPORTED_VERSION
 
 from opentrons_shared_data.pipette.dev_types import PipetteNameType
 from opentrons.protocol_api._nozzle_layout import NozzleLayout
 from opentrons.hardware_control.nozzle_manager import NozzleConfigurationType
+from opentrons.hardware_control.nozzle_manager import NozzleMap
 from . import deck_conflict
 
 from ..instrument import AbstractInstrument
 from .well import WellCore
 
-from ..._trash_bin import TrashBin
-from ..._waste_chute import WasteChute
+from ...disposal_locations import TrashBin, WasteChute
 
 if TYPE_CHECKING:
     from .protocol import ProtocolCore
 
 
 _DISPENSE_VOLUME_VALIDATION_ADDED_IN = APIVersion(2, 17)
 
@@ -404,21 +404,26 @@
         deck_conflict.check_safe_for_pipette_movement(
             engine_state=self._engine_client.state,
             pipette_id=self._pipette_id,
             labware_id=labware_id,
             well_name=well_name,
             well_location=well_location,
         )
-        self._engine_client.pick_up_tip(
+
+        self._engine_client.pick_up_tip_wait_for_recovery(
             pipette_id=self._pipette_id,
             labware_id=labware_id,
             well_name=well_name,
             well_location=well_location,
         )
 
+        # Set the "last location" unconditionally, even if the command failed
+        # and was recovered from and we don't know if the pipette is physically here.
+        # This isn't used for path planning, but rather for implicit destination
+        # selection like in `pipette.aspirate(location=None)`.
         self._protocol_core.set_last_location(location=location, mount=self.get_mount())
 
     def drop_tip(
         self,
         location: Optional[Location],
         well_core: WellCore,
         home_after: Optional[bool],
@@ -474,38 +479,45 @@
             home_after=home_after,
             alternateDropLocation=alternate_drop_location,
         )
 
         self._protocol_core.set_last_location(location=location, mount=self.get_mount())
 
     def drop_tip_in_disposal_location(
-        self, disposal_location: Union[TrashBin, WasteChute], home_after: Optional[bool]
+        self,
+        disposal_location: Union[TrashBin, WasteChute],
+        home_after: Optional[bool],
+        alternate_tip_drop: bool = False,
     ) -> None:
         self._move_to_disposal_location(
             disposal_location,
             force_direct=False,
             speed=None,
-            alternate_tip_drop=True,
+            alternate_tip_drop=alternate_tip_drop,
         )
         self._drop_tip_in_place(home_after=home_after)
         self._protocol_core.set_last_location(location=None, mount=self.get_mount())
 
     def _move_to_disposal_location(
         self,
         disposal_location: Union[TrashBin, WasteChute],
         force_direct: bool,
         speed: Optional[float],
         alternate_tip_drop: bool = False,
     ) -> None:
         # TODO (nd, 2023-11-30): give appropriate offset when finalized
         # https://opentrons.atlassian.net/browse/RSS-391
-        offset = AddressableOffsetVector(x=0, y=0, z=0)
+
+        disposal_offset = disposal_location.offset
+        offset = AddressableOffsetVector(
+            x=disposal_offset.x, y=disposal_offset.y, z=disposal_offset.z
+        )
 
         if isinstance(disposal_location, TrashBin):
-            addressable_area_name = disposal_location._addressable_area_name
+            addressable_area_name = disposal_location.area_name
             self._engine_client.move_to_addressable_area_for_drop_tip(
                 pipette_id=self._pipette_id,
                 addressable_area_name=addressable_area_name,
                 offset=offset,
                 force_direct=force_direct,
                 speed=speed,
                 minimum_z_height=None,
@@ -665,14 +677,17 @@
         return self._engine_client.state.tips.get_pipette_channels(self._pipette_id)
 
     def get_active_channels(self) -> int:
         return self._engine_client.state.tips.get_pipette_active_channels(
             self._pipette_id
         )
 
+    def get_nozzle_map(self) -> NozzleMap:
+        return self._engine_client.state.tips.get_pipette_nozzle_map(self._pipette_id)
+
     def has_tip(self) -> bool:
         return (
             self._engine_client.state.pipettes.get_attached_tip(self._pipette_id)
             is not None
         )
 
     def get_return_height(self) -> float:
@@ -699,22 +714,17 @@
         primary_nozzle = self._engine_client.state.pipettes.get_primary_nozzle(
             self._pipette_id
         )
         if self.get_nozzle_configuration() == NozzleConfigurationType.FULL:
             return True
         else:
             if self.get_channels() == 96:
-                # SINGLE configuration with H12 nozzle is technically supported by the
-                # current tip tracking implementation but we don't do any deck conflict
-                # checks for it, so we won't provide full support for it yet.
-                return (
-                    self.get_nozzle_configuration() == NozzleConfigurationType.COLUMN
-                    and primary_nozzle == "A12"
-                )
+                return True
             if self.get_channels() == 8:
+                # TODO: (cb, 03/06/24): Enable automatic tip tracking on the 8 channel pipettes once PAPI support exists
                 return (
                     self.get_nozzle_configuration() == NozzleConfigurationType.SINGLE
                     and primary_nozzle == "H1"
                 )
         return False
 
     def set_flow_rate(
@@ -768,7 +778,12 @@
                 primaryNozzle=cast(PRIMARY_NOZZLE_LITERAL, primary_nozzle)
             )
         else:
             configuration_model = AllNozzleLayoutConfiguration()
         self._engine_client.configure_nozzle_layout(
             pipette_id=self._pipette_id, configuration_params=configuration_model
         )
+
+    def retract(self) -> None:
+        """Retract this instrument to the top of the gantry."""
+        z_axis = self._engine_client.state.pipettes.get_z_axis(self._pipette_id)
+        self._engine_client.home([z_axis])
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/labware.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/labware.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,21 @@
     LabwareDefinition as LabwareDefinitionDict,
 )
 
 from opentrons_shared_data.labware.labware_definition import LabwareRole
 
 from opentrons.protocol_engine.errors import LabwareNotOnDeckError, ModuleNotOnDeckError
 from opentrons.protocol_engine.clients import SyncClient as ProtocolEngineClient
+from opentrons.protocol_engine.types import (
+    LabwareOffsetCreate,
+    LabwareOffsetVector,
+)
 from opentrons.types import DeckSlotName, Point
+from opentrons.hardware_control.nozzle_manager import NozzleMap
+
 
 from ..labware import AbstractLabware, LabwareLoadParams
 from .well import WellCore
 
 
 class LabwareCore(AbstractLabware[WellCore]):
     """Labware API core using a ProtocolEngine.
@@ -87,16 +93,36 @@
             self._definition.parameters.dict(exclude_none=True),
         )
 
     def get_quirks(self) -> List[str]:
         return self._definition.parameters.quirks or []
 
     def set_calibration(self, delta: Point) -> None:
-        raise NotImplementedError(
-            "Setting a labware's calibration after it's been loaded is not supported."
+        """Add a labware offset for this labware at its current location.
+
+        This will override any previous labware offsets for this definition URI and location,
+        even if the other labware offset was for a different specific labware instance.
+        """
+        offset_location = self._engine_client.state.geometry.get_offset_location(
+            self._labware_id
+        )
+        if not offset_location:
+            raise LabwareNotOnDeckError(
+                message=f"Cannot set offset for {self.get_name()} as it is not currently in a deck slot.",
+                details={"kind": "labware-not-in-slot"},
+            )
+
+        request = LabwareOffsetCreate.construct(
+            definitionUri=self.get_uri(),
+            location=offset_location,
+            vector=LabwareOffsetVector(x=delta.x, y=delta.y, z=delta.z),
+        )
+        self._engine_client.add_labware_offset(request)
+        self._engine_client.reload_labware(
+            labware_id=self._labware_id,
         )
 
     def get_calibrated_offset(self) -> Point:
         return self._engine_client.state.geometry.get_labware_position(self._labware_id)
 
     def is_tip_rack(self) -> bool:
         """Whether the labware is a tip rack."""
@@ -118,24 +144,28 @@
     def reset_tips(self) -> None:
         if self.is_tip_rack():
             self._engine_client.reset_tips(labware_id=self.labware_id)
         else:
             raise TypeError(f"{self.get_display_name()} is not a tip rack.")
 
     def get_next_tip(
-        self, num_tips: int, starting_tip: Optional[WellCore]
+        self,
+        num_tips: int,
+        starting_tip: Optional[WellCore],
+        nozzle_map: Optional[NozzleMap],
     ) -> Optional[str]:
         return self._engine_client.state.tips.get_next_tip(
             labware_id=self._labware_id,
             num_tips=num_tips,
             starting_tip_name=(
                 starting_tip.get_name()
                 if starting_tip and starting_tip.labware_id == self._labware_id
                 else None
             ),
+            nozzle_map=nozzle_map,
         )
 
     def get_well_columns(self) -> List[List[str]]:
         """Get the all well names, organized by column, from the labware's definition."""
         return self._definition.ordering
 
     def get_well_core(self, well_name: str) -> WellCore:
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/load_labware_params.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/load_labware_params.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/module_core.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/module_core.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/point_calculations.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/point_calculations.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/protocol.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/protocol.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ProtocolEngine-based Protocol API core implementation."""
 from __future__ import annotations
 from typing import Dict, Optional, Type, Union, List, Tuple, TYPE_CHECKING
 
 from opentrons.protocol_engine.commands import LoadModuleResult
-from opentrons_shared_data.deck.dev_types import DeckDefinitionV4, SlotDefV3
+from opentrons_shared_data.deck.dev_types import DeckDefinitionV5, SlotDefV3
 from opentrons_shared_data.labware.labware_definition import LabwareDefinition
 from opentrons_shared_data.labware.dev_types import LabwareDefinition as LabwareDefDict
 from opentrons_shared_data.pipette.dev_types import PipetteNameType
 from opentrons_shared_data.robot.dev_types import RobotType
 
 from opentrons.types import (
     DeckSlotName,
@@ -47,16 +47,15 @@
     LabwareNotLoadedOnModuleError,
     LabwareNotLoadedOnLabwareError,
 )
 
 from ... import validation
 from ..._types import OffDeckType
 from ..._liquid import Liquid
-from ..._trash_bin import TrashBin
-from ..._waste_chute import WasteChute
+from ...disposal_locations import TrashBin, WasteChute
 from ..protocol import AbstractProtocol
 from ..labware import LabwareLoadParams
 from .labware import LabwareCore
 from .instrument import InstrumentCore
 from .module_core import (
     ModuleCore,
     TemperatureModuleCore,
@@ -134,47 +133,34 @@
     def append_disposal_location(
         self,
         disposal_location: Union[Labware, TrashBin, WasteChute],
     ) -> None:
         """Append a disposal location object to the core."""
         self._disposal_locations.append(disposal_location)
 
-    def add_disposal_location_to_engine(
+    def _add_disposal_location_to_engine(
         self, disposal_location: Union[TrashBin, WasteChute]
     ) -> None:
         """Verify and add disposal location to engine store and append it to the core."""
+        self._engine_client.state.addressable_areas.raise_if_area_not_in_deck_configuration(
+            disposal_location.area_name
+        )
         if isinstance(disposal_location, TrashBin):
-            self._engine_client.state.addressable_areas.raise_if_area_not_in_deck_configuration(
-                disposal_location.area_name
-            )
             deck_conflict.check(
                 engine_state=self._engine_client.state,
                 new_trash_bin=disposal_location,
                 existing_disposal_locations=self._disposal_locations,
                 # TODO: We can now fetch these IDs from engine too.
                 #  See comment in self.load_labware().
                 #
                 # Wrapping .keys() in list() is just to make Decoy verification easier.
                 existing_labware_ids=list(self._labware_cores_by_id.keys()),
                 existing_module_ids=list(self._module_cores_by_id.keys()),
             )
-            self._engine_client.add_addressable_area(disposal_location.area_name)
-        elif isinstance(disposal_location, WasteChute):
-            # TODO(jbl 2024-01-25) hardcoding this specific addressable area should be refactored
-            #   when analysis is fixed up
-            #
-            # We want to tell Protocol Engine that there's a waste chute in the waste chute location when it's loaded,
-            # so analysis can prevent the user from doing anything that would collide with it. At the same time, we
-            # do not want to create a false negative when it comes to addressable area conflict. We therefore use the
-            # addressable area `1ChannelWasteChute` because every waste chute cutout fixture provides it and it will
-            # provide the engine with the information it needs.
-            self._engine_client.state.addressable_areas.raise_if_area_not_in_deck_configuration(
-                "1ChannelWasteChute"
-            )
-            self._engine_client.add_addressable_area("1ChannelWasteChute")
+        self._engine_client.add_addressable_area(disposal_location.area_name)
         self.append_disposal_location(disposal_location)
 
     def get_disposal_locations(self) -> List[Union[Labware, TrashBin, WasteChute]]:
         """Get disposal locations."""
         return self._disposal_locations
 
     def get_max_speeds(self) -> AxisMaxSpeeds:
@@ -419,15 +405,14 @@
             if module_type == ModuleType.THERMOCYCLER:
                 deck_slot = DeckSlotName.SLOT_7
             else:
                 raise InvalidModuleLocationError(deck_slot, model.name)
 
         robot_type = self._engine_client.state.config.robot_type
         normalized_deck_slot = deck_slot.to_equivalent_for_robot_type(robot_type)
-        self._ensure_module_location(normalized_deck_slot, module_type)
 
         result = self._engine_client.load_module(
             model=EngineModuleModel(model),
             location=DeckSlotLocation(slotName=normalized_deck_slot),
         )
 
         module_core = self._get_module_core(load_module_result=result, model=model)
@@ -520,14 +505,59 @@
             engine_client=self._engine_client,
             sync_hardware_api=self._sync_hardware,
             protocol_core=self,
             # TODO(mm, 2022-11-10): Deduplicate "400" with legacy core.
             default_movement_speed=400,
         )
 
+    def load_trash_bin(self, slot_name: DeckSlotName, area_name: str) -> TrashBin:
+        """Load a deck configuration based trash bin.
+
+        Args:
+            slot_name: the slot the trash is being loaded into.
+            area_name: the addressable area name of the trash.
+
+        Returns:
+            A trash bin object.
+        """
+        trash_bin = TrashBin(
+            location=slot_name,
+            addressable_area_name=area_name,
+            api_version=self._api_version,
+            engine_client=self._engine_client,
+        )
+        self._add_disposal_location_to_engine(trash_bin)
+        return trash_bin
+
+    def load_ot2_fixed_trash_bin(self) -> None:
+        """Load a deck configured OT-2 fixed trash in Slot 12."""
+        _fixed_trash_trash_bin = TrashBin(
+            location=DeckSlotName.FIXED_TRASH,
+            addressable_area_name="fixedTrash",
+            api_version=self._api_version,
+            engine_client=self._engine_client,
+        )
+        # We are just appending the fixed trash to the core's internal list here, not adding it to the engine via
+        # the core, since that method works through the SyncClient and if called from here, will cause protocols
+        # to deadlock. Instead, that method is called in protocol engine directly in create_protocol_context after
+        # ProtocolContext is initialized.
+        self.append_disposal_location(_fixed_trash_trash_bin)
+
+    def load_waste_chute(self) -> WasteChute:
+        """Load a deck configured waste chute into Slot D3.
+
+        Returns:
+            A waste chute object.
+        """
+        waste_chute = WasteChute(
+            engine_client=self._engine_client, api_version=self._api_version
+        )
+        self._add_disposal_location_to_engine(waste_chute)
+        return waste_chute
+
     def pause(self, msg: Optional[str]) -> None:
         """Pause the protocol."""
         self._engine_client.wait_for_resume(message=msg)
 
     def comment(self, msg: str) -> None:
         """Create a comment in the protocol to be shown in the log."""
         self._engine_client.comment(message=msg)
@@ -567,15 +597,15 @@
         location: Optional[Location],
         mount: Optional[Mount] = None,
     ) -> None:
         """Set the last accessed location."""
         self._last_location = location
         self._last_mount = mount
 
-    def get_deck_definition(self) -> DeckDefinitionV4:
+    def get_deck_definition(self) -> DeckDefinitionV5:
         """Get the geometry definition of the robot's deck."""
         return self._engine_client.state.labware.get_deck_definition()
 
     def get_slot_definition(
         self, slot: Union[DeckSlotName, StagingSlotName]
     ) -> SlotDefV3:
         """Get the slot definition from the robot's deck."""
@@ -587,22 +617,14 @@
 
     def get_staging_slot_definitions(self) -> Dict[str, SlotDefV3]:
         """Get all staging slot definitions available in the deck definition."""
         return (
             self._engine_client.state.addressable_areas.get_staging_slot_definitions()
         )
 
-    def _ensure_module_location(
-        self, slot: DeckSlotName, module_type: ModuleType
-    ) -> None:
-        slot_def = self.get_slot_definition(slot)
-        compatible_modules = slot_def["compatibleModuleTypes"]
-        if module_type.value not in compatible_modules:
-            raise ValueError(f"A {module_type.value} cannot be loaded into slot {slot}")
-
     def get_slot_item(
         self, slot_name: Union[DeckSlotName, StagingSlotName]
     ) -> Union[LabwareCore, ModuleCore, NonConnectedModuleCore, None]:
         """Get the contents of a given slot, if any."""
         loaded_item = self._engine_client.state.geometry.get_slot_item(
             slot_name=slot_name
         )
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/stringify.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/stringify.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/engine/well.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/engine/well.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/instrument.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/instrument.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from abc import abstractmethod, ABC
 from typing import Any, Generic, Optional, TypeVar, Union
 
 from opentrons import types
 from opentrons.hardware_control.dev_types import PipetteDict
 from opentrons.protocols.api_support.util import FlowRates
 from opentrons.protocol_api._nozzle_layout import NozzleLayout
+from opentrons.hardware_control.nozzle_manager import NozzleMap
 
-from .._trash_bin import TrashBin
-from .._waste_chute import WasteChute
+from ..disposal_locations import TrashBin, WasteChute
 from .well import WellCoreType
 
 
 class AbstractInstrument(ABC, Generic[WellCoreType]):
     @abstractmethod
     def get_default_speed(self) -> float:
         ...
@@ -133,21 +133,25 @@
             alternate_drop_location: Whether to randomize the exact location to drop tip
                 within the specified well.
         """
         ...
 
     @abstractmethod
     def drop_tip_in_disposal_location(
-        self, disposal_location: Union[TrashBin, WasteChute], home_after: Optional[bool]
+        self,
+        disposal_location: Union[TrashBin, WasteChute],
+        home_after: Optional[bool],
+        alternate_tip_drop: bool = False,
     ) -> None:
         """Move to and drop tip into a TrashBin or WasteChute.
 
         Args:
             disposal_location: The disposal location object we're dropping to.
             home_after: Whether to home the pipette after the tip is dropped.
+            alternate_tip_drop: Whether to alternate tip drop location in a trash bin.
         """
         ...
 
     @abstractmethod
     def home(self) -> None:
         ...
 
@@ -212,14 +216,18 @@
         ...
 
     @abstractmethod
     def get_active_channels(self) -> int:
         ...
 
     @abstractmethod
+    def get_nozzle_map(self) -> NozzleMap:
+        ...
+
+    @abstractmethod
     def has_tip(self) -> bool:
         ...
 
     @abstractmethod
     def get_return_height(self) -> float:
         ...
 
@@ -277,11 +285,14 @@
             front_right_nozzle: The front right most nozzle in the requested layout.
         """
         ...
 
     @abstractmethod
     def is_tip_tracking_available(self) -> bool:
         """Return whether auto tip tracking is available for the pipette's current nozzle configuration."""
+
+    def retract(self) -> None:
+        """Retract this instrument to the top of the gantry."""
         ...
 
 
 InstrumentCoreType = TypeVar("InstrumentCoreType", bound=AbstractInstrument[Any])
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/labware.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/labware.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from opentrons_shared_data.labware.dev_types import (
     LabwareUri,
     LabwareParameters as LabwareParametersDict,
     LabwareDefinition as LabwareDefinitionDict,
 )
 
 from opentrons.types import DeckSlotName, Point
+from opentrons.hardware_control.nozzle_manager import NozzleMap
 
 from .well import WellCoreType
 
 
 class LabwareLoadParams(NamedTuple):
     """Unique load parameters of a labware."""
 
@@ -106,15 +107,18 @@
 
     @abstractmethod
     def reset_tips(self) -> None:
         ...
 
     @abstractmethod
     def get_next_tip(
-        self, num_tips: int, starting_tip: Optional[WellCoreType]
+        self,
+        num_tips: int,
+        starting_tip: Optional[WellCoreType],
+        nozzle_map: Optional[NozzleMap],
     ) -> Optional[str]:
         """Get the name of the next available tip(s) in the rack, if available."""
 
     @abstractmethod
     def get_well_columns(self) -> List[List[str]]:
         """Get the all well names, organized by column, from the labware's definition."""
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/deck.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/deck.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,14 +276,19 @@
             ModuleType.HEATER_SHAKER: "Heater-Shaker",
         }
         if isinstance(location, str) or isinstance(location, int):
             slot_def = self.get_slot_definition(str(location))
             compatible_modules = slot_def["compatibleModuleTypes"]
             if module_type.value in compatible_modules:
                 return location
+            elif (
+                self._definition["robot"]["model"] == "OT-3 Standard"
+                and ModuleType.to_module_fixture_id(module_type) == slot_def["id"]
+            ):
+                return location
             else:
                 raise ValueError(
                     f"A {dn_from_type[module_type]} cannot be loaded"
                     f" into slot {location}"
                 )
         else:
             valid_slots = [
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/labware_offset_provider.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/labware_offset_provider.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/legacy_instrument_core.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/legacy_instrument_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     build_edges,
     FlowRates,
     PlungerSpeeds,
     APIVersionError,
 )
 from opentrons.protocols.geometry import planning
 from opentrons.protocol_api._nozzle_layout import NozzleLayout
+from opentrons.hardware_control.nozzle_manager import NozzleMap
 
-from ..._trash_bin import TrashBin
-from ..._waste_chute import WasteChute
+from ...disposal_locations import TrashBin, WasteChute
 from ..instrument import AbstractInstrument
 from .legacy_well_core import LegacyWellCore
 from .legacy_module_core import LegacyThermocyclerCore, LegacyHeaterShakerCore
 
 if TYPE_CHECKING:
     from .legacy_protocol_core import LegacyProtocolCore
 
@@ -291,15 +291,18 @@
                 # just means the tip can't be reused, so don't actually stop
                 # the protocol
                 _log.warning(
                     f"Could not return tip to {labware_core.get_display_name()}"
                 )
 
     def drop_tip_in_disposal_location(
-        self, disposal_location: Union[TrashBin, WasteChute], home_after: Optional[bool]
+        self,
+        disposal_location: Union[TrashBin, WasteChute],
+        home_after: Optional[bool],
+        alternate_tip_drop: bool = False,
     ) -> None:
         raise APIVersionError(
             "Dropping tips in a trash bin or waste chute is not supported in this API Version."
         )
 
     def home(self) -> None:
         """Home the mount"""
@@ -544,10 +547,18 @@
         """This will never be called because it was added in API 2.16."""
         pass
 
     def get_active_channels(self) -> int:
         """This will never be called because it was added in API 2.16."""
         assert False, "get_active_channels only supported in API 2.16 & later"
 
+    def get_nozzle_map(self) -> NozzleMap:
+        """This will never be called because it was added in API 2.18."""
+        assert False, "get_nozzle_map only supported in API 2.18 & later"
+
     def is_tip_tracking_available(self) -> bool:
         # Tip tracking is always available in legacy context
         return True
+
+    def retract(self) -> None:
+        """Retract this instrument to the top of the gantry."""
+        self._protocol_interface.get_hardware.retract(self._mount)  # type: ignore [attr-defined]
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/legacy_labware_core.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/legacy_labware_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import List, Optional
 
 from opentrons.calibration_storage import helpers
 from opentrons.protocols.geometry.labware_geometry import LabwareGeometry
 from opentrons.protocols.api_support.tip_tracker import TipTracker
 
 from opentrons.types import DeckSlotName, Location, Point
+from opentrons.hardware_control.nozzle_manager import NozzleMap
 from opentrons_shared_data.labware.dev_types import LabwareParameters, LabwareDefinition
 
 from ..labware import AbstractLabware, LabwareLoadParams
 from .legacy_well_core import LegacyWellCore
 from .well_geometry import WellGeometry
 
 
@@ -149,16 +150,23 @@
 
     def reset_tips(self) -> None:
         if self.is_tip_rack():
             for well in self._wells_by_name.values():
                 well.set_has_tip(True)
 
     def get_next_tip(
-        self, num_tips: int, starting_tip: Optional[LegacyWellCore]
+        self,
+        num_tips: int,
+        starting_tip: Optional[LegacyWellCore],
+        nozzle_map: Optional[NozzleMap],
     ) -> Optional[str]:
+        if nozzle_map is not None:
+            raise ValueError(
+                "Nozzle Map cannot be provided to calls for next tip in legacy protocols."
+            )
         next_well = self._tip_tracker.next_tip(num_tips, starting_tip)
         return next_well.get_name() if next_well else None
 
     def get_tip_tracker(self) -> TipTracker:
         return self._tip_tracker
 
     def get_well_columns(self) -> List[List[str]]:
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/legacy_module_core.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/legacy_module_core.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/legacy_protocol_core.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/legacy_protocol_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import logging
 from typing import Dict, List, Optional, Set, Union, cast, Tuple
 
-from opentrons_shared_data.deck.dev_types import DeckDefinitionV4, SlotDefV3
+from opentrons_shared_data.deck.dev_types import DeckDefinitionV5, SlotDefV3
 from opentrons_shared_data.labware.dev_types import LabwareDefinition
 from opentrons_shared_data.pipette.dev_types import PipetteNameType
 from opentrons_shared_data.robot.dev_types import RobotType
 
 from opentrons.types import DeckSlotName, StagingSlotName, Location, Mount, Point
 from opentrons.util.broker import Broker
 from opentrons.hardware_control import SyncHardwareAPI
 from opentrons.hardware_control.modules import AbstractModule, ModuleModel, ModuleType
 from opentrons.hardware_control.types import DoorState, PauseType
 from opentrons.protocols.api_support.types import APIVersion
 from opentrons.protocols.api_support.util import AxisMaxSpeeds, APIVersionError
 from opentrons.protocols import labware as labware_definition
 
 from ...labware import Labware
+from ...disposal_locations import TrashBin, WasteChute
 from ..._liquid import Liquid
 from ..._types import OffDeckType
-from ..._trash_bin import TrashBin
-from ..._waste_chute import WasteChute
 from ..protocol import AbstractProtocol
 from ..labware import LabwareLoadParams
 
 from . import legacy_module_core, module_geometry
 from .deck import Deck
 from .legacy_instrument_core import LegacyInstrumentCore
 from .labware_offset_provider import AbstractLabwareOffsetProvider
@@ -139,19 +138,14 @@
     ) -> None:
         if isinstance(disposal_location, (TrashBin, WasteChute)):
             raise APIVersionError(
                 "Trash Bin and Waste Chute Disposal locations are not supported in this API Version."
             )
         self._disposal_locations.append(disposal_location)
 
-    def add_disposal_location_to_engine(
-        self, disposal_location: Union[TrashBin, WasteChute]
-    ) -> None:
-        assert False, "add_disposal_location_to_engine only supported on engine core"
-
     def add_labware_definition(
         self,
         definition: LabwareDefinition,
     ) -> LabwareLoadParams:
         """Add a labware definition to the set of loadable definitions."""
         load_params = LabwareLoadParams(
             namespace=definition["namespace"],
@@ -380,14 +374,29 @@
                 mount=mount,
                 pipette_dict=pipette_dict,
             )
         )
 
         return new_instr
 
+    def load_trash_bin(self, slot_name: DeckSlotName, area_name: str) -> TrashBin:
+        raise APIVersionError(
+            "Loading deck configured trash bin is not supported in this API version."
+        )
+
+    def load_ot2_fixed_trash_bin(self) -> None:
+        raise APIVersionError(
+            "Loading deck configured OT-2 fixed trash bin is not supported in this API version."
+        )
+
+    def load_waste_chute(self) -> WasteChute:
+        raise APIVersionError(
+            "Loading waste chute is not supported in this API version."
+        )
+
     def get_loaded_instruments(
         self,
     ) -> Dict[Mount, Optional[LegacyInstrumentCore]]:
         """Get a mapping of mount to instrument."""
         return self._instruments
 
     def get_disposal_locations(self) -> List[Union[Labware, TrashBin, WasteChute]]:
@@ -478,15 +487,15 @@
         return cast(LegacyLabwareCore, labware._core) if labware is not None else None
 
     def get_labware_on_labware(
         self, labware_core: LegacyLabwareCore
     ) -> Optional[LegacyLabwareCore]:
         assert False, "get_labware_on_labware only supported on engine core"
 
-    def get_deck_definition(self) -> DeckDefinitionV4:
+    def get_deck_definition(self) -> DeckDefinitionV5:
         """Get the geometry definition of the robot's deck."""
         assert False, "get_deck_definition only supported on engine core"
 
     def get_slot_definition(
         self, slot: Union[DeckSlotName, StagingSlotName]
     ) -> SlotDefV3:
         """Get the slot definition from the robot's deck."""
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/legacy_well_core.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/legacy_well_core.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/load_info.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/load_info.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/module_geometry.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/module_geometry.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy/well_geometry.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy/well_geometry.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy_simulator/__init__.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy_simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy_simulator/legacy_instrument_core.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy_simulator/legacy_instrument_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 )
 from opentrons.protocols.geometry import planning
 from opentrons_shared_data.errors.exceptions import (
     UnexpectedTipRemovalError,
     UnexpectedTipAttachError,
 )
 
-from ..._trash_bin import TrashBin
-from ..._waste_chute import WasteChute
+from ...disposal_locations import TrashBin, WasteChute
 from opentrons.protocol_api._nozzle_layout import NozzleLayout
+from opentrons.hardware_control.nozzle_manager import NozzleMap
 
 from ..instrument import AbstractInstrument
 
 from ..legacy.legacy_well_core import LegacyWellCore
 from ..legacy.legacy_module_core import LegacyThermocyclerCore, LegacyHeaterShakerCore
 
 if TYPE_CHECKING:
@@ -259,15 +259,18 @@
                 # just means the tip can't be reused, so don't actually stop
                 # the protocol
                 _log.warning(
                     f"Could not return tip to {labware_core.get_display_name()}"
                 )
 
     def drop_tip_in_disposal_location(
-        self, disposal_location: Union[TrashBin, WasteChute], home_after: Optional[bool]
+        self,
+        disposal_location: Union[TrashBin, WasteChute],
+        home_after: Optional[bool],
+        alternate_tip_drop: bool = False,
     ) -> None:
         raise APIVersionError(
             "Dropping tips in a trash bin or waste chute is not supported in this API Version."
         )
 
     def home(self) -> None:
         self._protocol_interface.set_last_location(None)
@@ -462,10 +465,18 @@
         """This will never be called because it was added in API 2.15."""
         pass
 
     def get_active_channels(self) -> int:
         """This will never be called because it was added in API 2.16."""
         assert False, "get_active_channels only supported in API 2.16 & later"
 
+    def get_nozzle_map(self) -> NozzleMap:
+        """This will never be called because it was added in API 2.18."""
+        assert False, "get_nozzle_map only supported in API 2.18 & later"
+
     def is_tip_tracking_available(self) -> bool:
         # Tip tracking is always available in legacy context
         return True
+
+    def retract(self) -> None:
+        """Retract this instrument to the top of the gantry."""
+        self._protocol_interface.get_hardware.retract(self._mount)  # type: ignore [attr-defined]
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/legacy_simulator/legacy_protocol_core.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/legacy_simulator/legacy_protocol_core.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/module.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/module.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/protocol.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 """The interface that implements ProtocolContext."""
 
 from __future__ import annotations
 
 from abc import abstractmethod, ABC
 from typing import Generic, List, Optional, Union, Tuple, Dict, TYPE_CHECKING
 
-from opentrons_shared_data.deck.dev_types import DeckDefinitionV4, SlotDefV3
+from opentrons_shared_data.deck.dev_types import DeckDefinitionV5, SlotDefV3
 from opentrons_shared_data.pipette.dev_types import PipetteNameType
 from opentrons_shared_data.labware.dev_types import LabwareDefinition
 from opentrons_shared_data.robot.dev_types import RobotType
 
 from opentrons.types import DeckSlotName, StagingSlotName, Location, Mount, Point
 from opentrons.hardware_control import SyncHardwareAPI
 from opentrons.hardware_control.modules.types import ModuleModel
 from opentrons.protocols.api_support.util import AxisMaxSpeeds
 
 from .instrument import InstrumentCoreType
 from .labware import LabwareCoreType, LabwareLoadParams
 from .module import ModuleCoreType
 from .._liquid import Liquid
-from .._trash_bin import TrashBin
-from .._waste_chute import WasteChute
 from .._types import OffDeckType
+from ..disposal_locations import TrashBin, WasteChute
 
 if TYPE_CHECKING:
     from ..labware import Labware
 
 
 class AbstractProtocol(
     ABC, Generic[InstrumentCoreType, LabwareCoreType, ModuleCoreType]
@@ -66,21 +65,14 @@
         self,
         disposal_location: Union[Labware, TrashBin, WasteChute],
     ) -> None:
         """Append a disposal location object to the core"""
         ...
 
     @abstractmethod
-    def add_disposal_location_to_engine(
-        self, disposal_location: Union[TrashBin, WasteChute]
-    ) -> None:
-        """Verify and add disposal location to engine store and append it to the core."""
-        ...
-
-    @abstractmethod
     def load_labware(
         self,
         load_name: str,
         location: Union[
             DeckSlotName, StagingSlotName, LabwareCoreType, ModuleCoreType, OffDeckType
         ],
         label: Optional[str],
@@ -133,14 +125,26 @@
     @abstractmethod
     def load_instrument(
         self, instrument_name: PipetteNameType, mount: Mount
     ) -> InstrumentCoreType:
         ...
 
     @abstractmethod
+    def load_trash_bin(self, slot_name: DeckSlotName, area_name: str) -> TrashBin:
+        ...
+
+    @abstractmethod
+    def load_ot2_fixed_trash_bin(self) -> None:
+        ...
+
+    @abstractmethod
+    def load_waste_chute(self) -> WasteChute:
+        ...
+
+    @abstractmethod
     def pause(self, msg: Optional[str]) -> None:
         ...
 
     @abstractmethod
     def comment(self, msg: str) -> None:
         ...
 
@@ -180,15 +184,15 @@
         self,
         location: Optional[Location],
         mount: Optional[Mount] = None,
     ) -> None:
         ...
 
     @abstractmethod
-    def get_deck_definition(self) -> DeckDefinitionV4:
+    def get_deck_definition(self) -> DeckDefinitionV5:
         """Get the geometry definition of the robot's deck."""
 
     @abstractmethod
     def get_slot_definition(
         self, slot: Union[DeckSlotName, StagingSlotName]
     ) -> SlotDefV3:
         """Get the slot definition from the robot's deck."""
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/well.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/well.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/core/well_grid.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/core/well_grid.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/create_protocol_context.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/create_protocol_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """ProtocolContext factory."""
 import asyncio
 from typing import Any, Dict, Optional, Union, cast
 
 from opentrons_shared_data.labware.dev_types import LabwareDefinition
 
-from opentrons.config import feature_flags
 from opentrons.hardware_control import (
     HardwareControlAPI,
     ThreadManager,
     SynchronousAdapter,
 )
 from opentrons.legacy_broker import LegacyBroker
 from opentrons.util.broker import Broker
@@ -18,15 +17,15 @@
 from opentrons.protocols.api_support.deck_type import (
     should_load_fixed_trash_area_for_python_protocol,
 )
 from opentrons.protocols.api_support.definitions import MAX_SUPPORTED_VERSION
 
 from .protocol_context import ProtocolContext
 from .deck import Deck
-from ._trash_bin import TrashBin
+from .disposal_locations import TrashBin
 
 from .core.common import ProtocolCore as AbstractProtocolCore
 from .core.legacy.deck import Deck as LegacyDeck
 from .core.legacy.legacy_protocol_core import LegacyProtocolCore
 from .core.legacy.labware_offset_provider import (
     AbstractLabwareOffsetProvider,
     LabwareOffsetProvider,
@@ -119,16 +118,15 @@
         engine_client = SyncClient(transport=engine_client_transport)
         core = ProtocolCore(
             engine_client=engine_client,
             api_version=api_version,
             sync_hardware=sync_hardware,
         )
 
-    # TODO(mc, 2022-8-22): remove `disable_fast_protocol_upload`
-    elif use_simulating_core and not feature_flags.disable_fast_protocol_upload():
+    elif use_simulating_core:
         legacy_deck = LegacyDeck(deck_type=deck_type)
         core = LegacyProtocolCoreSimulator(
             sync_hardware=sync_hardware,
             labware_offset_provider=labware_offset_provider,
             deck_layout=legacy_deck,
             equipment_broker=equipment_broker,
             api_version=api_version,
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/deck.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/deck.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/instrument_context.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/instrument_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,37 +7,37 @@
     CommandPreconditionViolated,
     CommandParameterLimitViolated,
     UnexpectedTipRemovalError,
 )
 from opentrons.legacy_broker import LegacyBroker
 from opentrons.hardware_control.dev_types import PipetteDict
 from opentrons import types
-from opentrons.commands import commands as cmds
+from opentrons.legacy_commands import commands as cmds
 
-from opentrons.commands import publisher
+from opentrons.legacy_commands import publisher
 from opentrons.protocols.advanced_control.mix import mix_from_kwargs
 from opentrons.protocols.advanced_control import transfers
 
 from opentrons.protocols.api_support.deck_type import NoTrashDefinedError
 from opentrons.protocols.api_support.types import APIVersion
 from opentrons.protocols.api_support import instrument
 from opentrons.protocols.api_support.util import (
     FlowRates,
     PlungerSpeeds,
     clamp_value,
     requires_version,
     APIVersionError,
 )
+from opentrons.hardware_control.nozzle_manager import NozzleConfigurationType
 
 from .core.common import InstrumentCore, ProtocolCore
 from .core.engine import ENGINE_CORE_API_VERSION
 from .core.legacy.legacy_instrument_core import LegacyInstrumentCore
 from .config import Clearances
-from ._trash_bin import TrashBin
-from ._waste_chute import WasteChute
+from .disposal_locations import TrashBin, WasteChute
 from ._nozzle_layout import NozzleLayout
 from . import labware, validation
 
 
 AdvancedLiquidHandling = Union[
     labware.Well,
     types.Location,
@@ -53,14 +53,19 @@
 _PREP_AFTER_ADDED_IN = APIVersion(2, 13)
 """The version after which the pick-up tip procedure should also prepare the plunger."""
 _PRESSES_INCREMENT_REMOVED_IN = APIVersion(2, 14)
 """The version after which the pick-up tip procedure deprecates presses and increment arguments."""
 _DROP_TIP_LOCATION_ALTERNATING_ADDED_IN = APIVersion(2, 15)
 """The version after which a drop-tip-into-trash procedure drops tips in different alternating locations within the trash well."""
 _PARTIAL_NOZZLE_CONFIGURATION_ADDED_IN = APIVersion(2, 16)
+"""The version after which a partial nozzle configuration became available for the 96 Channel Pipette."""
+_PARTIAL_NOZZLE_CONFIGURATION_AUTOMATIC_TIP_TRACKING_IN = APIVersion(2, 18)
+"""The version after which automatic tip tracking supported partially configured nozzle layouts."""
+_DISPOSAL_LOCATION_OFFSET_ADDED_IN = APIVersion(2, 18)
+"""The version after which offsets for deck configured trash containers and changes to alternating tip drop behavior were introduced."""
 
 
 class InstrumentContext(publisher.CommandPublisher):
     """
     A context for a specific pipette or instrument.
 
     The InstrumentContext class provides the objects, attributes, and methods that allow
@@ -286,23 +291,28 @@
         push_out: Optional[float] = None,
     ) -> InstrumentContext:
         """
         Dispense liquid from a pipette tip.
 
         See :ref:`new-dispense` for more details and examples.
 
-        :param volume: The volume to dispense, measured in µL. If unspecified,
-                       defaults to :py:attr:`current_volume`. If only a volume is
-                       passed, the pipette will dispense from its current position.
+        :param volume: The volume to dispense, measured in µL.
+
+                         - If unspecified or ``None``, dispense the :py:attr:`current_volume`.
+
+                         - If 0, the behavior of ``dispense()`` depends on the API level
+                           of the protocol. In API version 2.16 and earlier, dispense all
+                           liquid in the pipette (same as unspecified or ``None``). In API
+                           version 2.17 and later, dispense no liquid.
+
+                         - If greater than :py:obj:`.current_volume`, the behavior of
+                           ``dispense()`` depends on the API level of the protocol. In API
+                           version 2.16 and earlier, dispense all liquid in the pipette.
+                           In API version 2.17 and later, raise an error.
 
-                       If ``dispense`` is called with a volume of precisely 0, its behavior
-                       depends on the API level of the protocol. On API levels below 2.16,
-                       it will behave the same as a volume of ``None``/unspecified: dispense
-                       all liquid in the pipette. On API levels at or above 2.16, no liquid
-                       will be dispensed.
         :type volume: int or float
 
         :param location: Tells the robot where to dispense liquid held in the pipette.
                          The location can be a :py:class:`.Well` or a
                          :py:class:`.Location`.
 
                             - If the location is a ``Well``, the pipette will dispense
@@ -341,14 +351,17 @@
             If ``dispense`` is called with a single, unnamed argument, it will treat
             that argument as ``volume``. If you want to call ``dispense`` with only
             ``location``, specify it as a keyword argument:
             ``pipette.dispense(location=plate['A1'])``.
 
         .. versionchanged:: 2.15
             Added the ``push_out`` parameter.
+
+        .. versionchanged:: 2.17
+            Behavior of the ``volume`` parameter.
         """
         if self.api_version < APIVersion(2, 15) and push_out:
             raise APIVersionError(
                 "Unsupported parameter push_out. Change your API version to 2.15 or above to use this parameter."
             )
         _log.debug(
             "dispense {} from {} at {}".format(
@@ -866,39 +879,63 @@
         tip_rack: labware.Labware
         move_to_location: Optional[types.Location] = None
         active_channels = (
             self.active_channels
             if self._api_version >= _PARTIAL_NOZZLE_CONFIGURATION_ADDED_IN
             else self.channels
         )
+        nozzle_map = (
+            self._core.get_nozzle_map()
+            if self._api_version
+            >= _PARTIAL_NOZZLE_CONFIGURATION_AUTOMATIC_TIP_TRACKING_IN
+            else None
+        )
 
         if location is None:
+            if (
+                nozzle_map is not None
+                and nozzle_map.configuration != NozzleConfigurationType.FULL
+                and self.starting_tip is not None
+            ):
+                # Disallowing this avoids concerning the system with the direction
+                # in which self.starting_tip consumes tips. It would currently vary
+                # depending on the configuration layout of a pipette at a given
+                # time, which means that some combination of starting tip and partial
+                # configuraiton are incompatible under the current understanding of
+                # starting tip behavior. Replacing starting_tip with an undeprecated
+                # Labware.has_tip may solve this.
+                raise CommandPreconditionViolated(
+                    "Automatic tip tracking is not available when using a partial pipette"
+                    " nozzle configuration and InstrumentContext.starting_tip."
+                    " Switch to a full configuration or set starting_tip to None."
+                )
             if not self._core.is_tip_tracking_available():
                 raise CommandPreconditionViolated(
                     "Automatic tip tracking is not available for the current pipette"
                     " nozzle configuration. We suggest switching to a configuration"
                     " that supports automatic tip tracking or specifying the exact tip"
                     " to pick up."
                 )
-
             tip_rack, well = labware.next_available_tip(
                 starting_tip=self.starting_tip,
                 tip_racks=self.tip_racks,
                 channels=active_channels,
+                nozzle_map=nozzle_map,
             )
 
         elif isinstance(location, labware.Well):
             well = location
             tip_rack = well.parent
 
         elif isinstance(location, labware.Labware):
             tip_rack, well = labware.next_available_tip(
                 starting_tip=None,
                 tip_racks=[location],
                 channels=active_channels,
+                nozzle_map=nozzle_map,
             )
 
         elif isinstance(location, types.Location):
             maybe_tip_rack, maybe_well = location.labware.get_parent_labware_and_well()
 
             if maybe_well is not None:
                 well = maybe_well
@@ -906,14 +943,15 @@
                 move_to_location = location
 
             elif maybe_tip_rack is not None:
                 tip_rack, well = labware.next_available_tip(
                     starting_tip=None,
                     tip_racks=[maybe_tip_rack],
                     channels=active_channels,
+                    nozzle_map=nozzle_map,
                 )
             else:
                 raise TypeError(
                     "If specified as a `types.Location`,"
                     " `location` should refer to a ``Labware` or `Well` location."
                     f" However, it refers to {location.labware}"
                 )
@@ -1022,14 +1060,15 @@
                     command=cmds.drop_tip_in_disposal_location(
                         instrument=self, location=trash_container
                     ),
                 ):
                     self._core.drop_tip_in_disposal_location(
                         trash_container,
                         home_after=home_after,
+                        alternate_tip_drop=True,
                     )
                 self._last_tip_picked_up_from = None
                 return self
 
         elif isinstance(location, labware.Well):
             well = location
             location = None
@@ -1045,22 +1084,30 @@
                     " since that is where a tip is dropped."
                     f" However, the given location refers to {location.labware}"
                 )
 
             well = maybe_well
 
         elif isinstance(location, (TrashBin, WasteChute)):
+            # In 2.16 and 2.17, we would always automatically use automatic alternate tip drop locations regardless
+            # of whether you explicitly passed the disposal location as a location or if none was provided. Now, in
+            # 2.18 and moving forward, passing it in will bypass the automatic behavior and instead go to the set
+            # offset or the XY center if none is provided.
+            if self.api_version < _DISPOSAL_LOCATION_OFFSET_ADDED_IN:
+                alternate_drop_location = True
             with publisher.publish_context(
                 broker=self.broker,
                 command=cmds.drop_tip_in_disposal_location(
                     instrument=self, location=location
                 ),
             ):
                 self._core.drop_tip_in_disposal_location(
-                    location, home_after=home_after
+                    location,
+                    home_after=home_after,
+                    alternate_tip_drop=alternate_drop_location,
                 )
             self._last_tip_picked_up_from = None
             return self
 
         else:
             raise TypeError(
                 "If specified, location should be an instance of"
@@ -1311,14 +1358,20 @@
         blow_out = kwargs.get("blow_out")
         blow_out_strategy = None
         active_channels = (
             self.active_channels
             if self._api_version >= _PARTIAL_NOZZLE_CONFIGURATION_ADDED_IN
             else self.channels
         )
+        nozzle_map = (
+            self._core.get_nozzle_map()
+            if self._api_version
+            >= _PARTIAL_NOZZLE_CONFIGURATION_AUTOMATIC_TIP_TRACKING_IN
+            else None
+        )
 
         if blow_out and not blowout_location:
             if self.current_volume:
                 blow_out_strategy = transfers.BlowOutStrategy.SOURCE
             else:
                 blow_out_strategy = transfers.BlowOutStrategy.TRASH
         elif blow_out and blowout_location:
@@ -1327,15 +1380,18 @@
             elif blowout_location == "destination well":
                 blow_out_strategy = transfers.BlowOutStrategy.DEST
             elif blowout_location == "trash":
                 blow_out_strategy = transfers.BlowOutStrategy.TRASH
 
         if new_tip != types.TransferTipPolicy.NEVER:
             tr, next_tip = labware.next_available_tip(
-                self.starting_tip, self.tip_racks, active_channels
+                self.starting_tip,
+                self.tip_racks,
+                active_channels,
+                nozzle_map=nozzle_map,
             )
             max_volume = min(next_tip.max_volume, self.max_volume)
         else:
             max_volume = self._core.get_working_volume()
 
         touch_tip = None
         if kwargs.get("touch_tip"):
@@ -1480,14 +1536,20 @@
                     force_direct=force_direct,
                     minimum_z_height=minimum_z_height,
                     speed=speed,
                 )
 
         return self
 
+    @requires_version(2, 18)
+    def _retract(
+        self,
+    ) -> None:
+        self._core.retract()
+
     @property
     @requires_version(2, 0)
     def mount(self) -> str:
         """
         Return the name of the mount the pipette is attached to.
 
         The possible names are ``"left"`` and ``"right"``.
@@ -1870,33 +1932,40 @@
 
         :type style: ``NozzleLayout`` or ``None``
         :param start: The nozzle at the back left of the layout, which the robot uses
             to determine how it will move to different locations on the deck. The string
             should be of the same format used when identifying wells by name.
             Required unless setting ``style=ALL``.
 
-            .. note::
-                When using the ``COLUMN`` layout, the only fully supported value is
-                ``start="A12"``. You can use ``start="A1"``, but this will disable tip
-                tracking and you will have to specify the ``location`` every time you
-                call :py:meth:`.pick_up_tip`, such that the pipette picks up columns of
-                tips *from right to left* on the tip rack.
-
         :type start: str or ``None``
         :param tip_racks: Behaves the same as setting the ``tip_racks`` parameter of
             :py:meth:`.load_instrument`. If not specified, the new configuration resets
             :py:obj:`.InstrumentContext.tip_racks` and you must specify the location
             every time you call :py:meth:`~.InstrumentContext.pick_up_tip`.
         :type tip_racks: List[:py:class:`.Labware`]
         """
         #       TODO: add the following back into the docstring when QUADRANT is supported
         #
         #       :param front_right: The nozzle at the front left of the layout. Only used for
         #           NozzleLayout.QUADRANT configurations.
         #       :type front_right: str or ``None``
+        #
+        #       NOTE: Disabled layouts error case can be removed once desired map configurations
+        #       have appropriate data regarding tip-type to map current values added to the
+        #       pipette definitions.
+        disabled_layouts = [
+            NozzleLayout.ROW,
+            NozzleLayout.SINGLE,
+            NozzleLayout.QUADRANT,
+        ]
+        if style in disabled_layouts:
+            raise ValueError(
+                f"Nozzle layout configuration of style {style.value} is currently unsupported."
+            )
+
         if style != NozzleLayout.ALL:
             if start is None:
                 raise ValueError(
                     f"Cannot configure a nozzle layout of style {style.value} without a starting nozzle."
                 )
             if start not in types.ALLOWED_PRIMARY_NOZZLES:
                 raise ValueError(
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/labware.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/labware.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,41 +3,43 @@
 This module provides things like :py:class:`Labware`, and :py:class:`Well`
 to encapsulate labware instances used in protocols
 and their wells. It also provides helper functions to load and save labware
 and labware calibration offsets. It contains all the code necessary to
 transform from labware symbolic points (such as "well a1 of an opentrons
 tiprack") to points in deck coordinates.
 """
+
 from __future__ import annotations
 
 import logging
 
 from itertools import dropwhile
 from typing import TYPE_CHECKING, Any, List, Dict, Optional, Union, Tuple, cast
 
 from opentrons_shared_data.labware.dev_types import LabwareDefinition, LabwareParameters
 
 from opentrons.types import Location, Point
 from opentrons.protocols.api_support.types import APIVersion
 from opentrons.protocols.api_support.util import requires_version, APIVersionError
+from opentrons.hardware_control.nozzle_manager import NozzleMap
 
 # TODO(mc, 2022-09-02): re-exports provided for backwards compatibility
 # remove when their usage is no longer needed
 from opentrons.protocols.labware import (  # noqa: F401
     get_labware_definition as get_labware_definition,
     get_all_labware_definitions as get_all_labware_definitions,
     verify_definition as verify_definition,
     save_definition as save_definition,
 )
 
 from . import validation
 from ._liquid import Liquid
 from ._types import OffDeckType
 from .core import well_grid
-from .core.engine import ENGINE_CORE_API_VERSION
+from .core.engine import ENGINE_CORE_API_VERSION, SET_OFFSET_RESTORED_API_VERSION
 from .core.labware import AbstractLabware
 from .core.module import AbstractModuleCore
 from .core.core_map import LoadedCoreMap
 from .core.legacy.legacy_labware_core import LegacyLabwareCore
 from .core.legacy.legacy_well_core import LegacyWellCore
 from .core.legacy.well_geometry import WellGeometry
 
@@ -292,37 +294,30 @@
 
     def __hash__(self) -> int:
         return hash(self.top().point)
 
 
 class Labware:
     """
-    This class represents a labware, such as a PCR plate, a tube rack,
-    reservoir, tip rack, etc. It defines the physical geometry of the labware,
-    and provides methods for accessing wells within the labware.
-
-    It is commonly created by calling ``ProtocolContext.load_labware()``.
-
-    To access a labware's wells, you can use its well accessor methods:
-    :py:meth:`wells_by_name`, :py:meth:`wells`, :py:meth:`columns`,
-    :py:meth:`rows`, :py:meth:`rows_by_name`, and :py:meth:`columns_by_name`.
-    You can also use an instance of a labware as a Python dictionary, accessing
-    wells by their names. The following example shows how to use all of these
-    methods to access well A1:
-
-    .. code-block :: python
-
-       labware = context.load_labware('corning_96_wellplate_360ul_flat', 1)
-       labware['A1']
-       labware.wells_by_name()['A1']
-       labware.wells()[0]
-       labware.rows()[0][0]
-       labware.columns()[0][0]
-       labware.rows_by_name()['A'][0]
-       labware.columns_by_name()[0][0]
+    This class represents a piece of labware.
+
+    Labware available in the API generally fall under two categories.
+
+      - Consumable labware: well plates, tubes in racks, reservoirs, tip racks, etc.
+      - Adapters: durable items that hold other labware, either on modules or directly
+        on the deck.
+
+    The ``Labware`` class defines the physical geometry of the labware
+    and provides methods for :ref:`accessing wells <new-well-access>` within the labware.
+
+    Create ``Labware`` objects by calling the appropriate ``load_labware()`` method,
+    depending on where you are loading the labware. For example, to load labware on a
+    Thermocycler Module, use :py:meth:`.ThermocyclerContext.load_labware`. To load
+    labware directly on the deck, use :py:meth:`.ProtocolContext.load_labware`. See
+    :ref:`loading-labware`.
 
     """
 
     def __init__(
         self,
         core: AbstractLabware[Any],
         api_version: APIVersion,
@@ -366,49 +361,53 @@
             " It no longer has meaning, but will always return `False`"
         )
         return False
 
     @property
     @requires_version(2, 0)
     def api_version(self) -> APIVersion:
+        """See :py:obj:`.ProtocolContext.api_version`."""
         return self._api_version
 
     def __getitem__(self, key: str) -> Well:
         return self.wells_by_name()[key]
 
     @property
     @requires_version(2, 0)
     def uri(self) -> str:
         """A string fully identifying the labware.
 
-        :returns: The URI, ``"namespace/loadname/version"``
+        The URI has three parts and follows the pattern ``"namespace/load_name/version"``.
+        For example, ``opentrons/corning_96_wellplate_360ul_flat/2``.
         """
         return self._core.get_uri()
 
     @property
     @requires_version(2, 0)
     def parent(self) -> Union[str, Labware, ModuleTypes, OffDeckType]:
-        """The parent of this labware---where this labware is loaded.
+        """Where the labware is loaded.
+
+        This corresponds to the physical object that the labware *directly* rests upon.
 
         Returns:
             If the labware is directly on the robot's deck, the ``str`` name of the deck slot,
             like ``"D1"`` (Flex) or ``"1"`` (OT-2). See :ref:`deck-slots`.
 
             If the labware is on a module, a module context.
 
             If the labware is on a labware or adapter, a :py:class:`Labware`.
 
             If the labware is off-deck, :py:obj:`OFF_DECK`.
 
         .. versionchanged:: 2.14
             Return type for module parent changed.
-            Prior to this version, an internal geometry interface was returned.
+            Formerly, the API returned an internal geometry interface.
         .. versionchanged:: 2.15
-            Will return a :py:class:`Labware` if the labware is loaded onto a labware/adapter.
-            Will now return :py:obj:`OFF_DECK` if the labware is off-deck.
+            Returns a :py:class:`Labware` if the labware is loaded onto a labware/adapter.
+            Returns :py:obj:`OFF_DECK` if the labware is off-deck.
             Formerly, if the labware was removed by using ``del`` on :py:obj:`.deck`,
             this would return where it was before its removal.
         """
         if isinstance(self._core, LegacyLabwareCore):
             # Type ignoring to preserve backwards compatibility
             return self._core.get_geometry().parent.labware.object  # type: ignore
 
@@ -420,16 +419,21 @@
             return self._core_map.get(labware_location)
 
         return labware_location
 
     @property
     @requires_version(2, 0)
     def name(self) -> str:
-        """Can either be the canonical name of the labware, which is used to
-        load it, or the label of the labware specified by a user."""
+        """The display name of the labware.
+
+        If you specified a value for ``label`` when loading the labware, ``name`` is
+        that value.
+
+        Otherwise, it is the :py:obj:`~.Labware.load_name` of the labware.
+        """
         return self._core.get_name()
 
     @name.setter
     def name(self, new_name: str) -> None:
         """Set the labware name.
 
         .. deprecated: 2.14
@@ -532,35 +536,35 @@
 
         return labware
 
     @requires_version(2, 15)
     def load_labware_from_definition(
         self, definition: LabwareDefinition, label: Optional[str] = None
     ) -> Labware:
-        """Load a labware onto the module using an inline definition.
+        """Load a compatible labware onto the labware using an inline definition.
 
         :param definition: The labware definition.
-        :param str label: An optional special name to give the labware. If
-                          specified, this is the name the labware will appear
-                          as in the run log and the calibration view in the
-                          Opentrons App.
+        :param str label: An optional special name to give the labware. If specified,
+            this is how the labware will appear in the run log, Labware Position
+            Check, and elsewhere in the Opentrons App and on the touchscreen.
+
         :returns: The initialized and loaded labware object.
         """
         load_params = self._protocol_core.add_labware_definition(definition)
 
         return self.load_labware(
             name=load_params.load_name,
             namespace=load_params.namespace,
             version=load_params.version,
             label=label,
         )
 
     def set_calibration(self, delta: Point) -> None:
         """
-        An internal, deprecated method used for updating the offset on the object.
+        An internal, deprecated method used for updating the labware offset.
 
         .. deprecated:: 2.14
         """
         if self._api_version >= ENGINE_CORE_API_VERSION:
             raise APIVersionError(
                 "Labware.set_calibration() is not supported when apiLevel is 2.14 or higher."
                 " Use a lower apiLevel"
@@ -572,48 +576,48 @@
     def set_offset(self, x: float, y: float, z: float) -> None:
         """Set the labware's position offset.
 
         The offset is an x, y, z vector in deck coordinates
         (see :ref:`protocol-api-deck-coords`) that the motion system
         will add to any movement targeting this labware instance.
 
-        The offset *will not* apply to any other labware instances,
+        The offset *will not apply* to any other labware instances,
         even if those labware are of the same type.
 
-        .. caution::
-            This method is *only* for use with mechanisms like
-            :obj:`opentrons.execute.get_protocol_api`, which lack an interactive way
-            to adjust labware offsets. (See :ref:`advanced-control`.)
+        This method is *only* for use with mechanisms like
+        :obj:`opentrons.execute.get_protocol_api`, which lack an interactive way
+        to adjust labware offsets. (See :ref:`advanced-control`.)
+
+        .. warning::
 
             If you're uploading a protocol via the Opentrons App, don't use this method,
             because it will produce undefined behavior.
-            Instead, use Labware Position Check in the app.
+            Instead, use Labware Position Check in the app or on the touchscreen.
 
-            Because protocols using :ref:`API version <v2-versioning>` 2.14 or higher
-            can currently *only* be uploaded via the Opentrons App, it doesn't make
-            sense to use this method with them. Trying to do so will raise an exception.
         """
-        if self._api_version >= ENGINE_CORE_API_VERSION:
-            # TODO(mm, 2023-02-13): See Jira RCORE-535.
-            #
-            # Until that issue is resolved, the only way to simulate or run a
-            # >=ENGINE_CORE_API_VERSION protocol is through the Opentrons App.
-            # Therefore, in >=ENGINE_CORE_API_VERSION protocols,
-            # there's no legitimate way to use this method.
+        if (
+            self._api_version >= ENGINE_CORE_API_VERSION
+            and self._api_version < SET_OFFSET_RESTORED_API_VERSION
+        ):
             raise APIVersionError(
-                "Labware.set_offset() is not supported when apiLevel is 2.14 or higher."
-                " Use a lower apiLevel"
+                "Labware.set_offset() is not supported when apiLevel is 2.14, 2.15, 2.16, or 2.17."
+                " Use apilevel 2.13 or below, or 2.18 or above to set offset,"
                 " or use the Opentrons App's Labware Position Check."
             )
         else:
             self._core.set_calibration(Point(x=x, y=y, z=z))
 
     @property
     @requires_version(2, 0)
     def calibrated_offset(self) -> Point:
+        """The front-left-bottom corner of the labware, including its labware offset.
+
+        When running a protocol in the Opentrons App or on the touchscreen, Labware
+        Position Check sets the labware offset.
+        """
         return self._core.get_calibrated_offset()
 
     @requires_version(2, 0)
     def well(self, idx: Union[int, str]) -> Well:
         """Deprecated. Use result of :py:meth:`wells` or :py:meth:`wells_by_name`."""
         if isinstance(idx, int):
             return self.wells()[idx]
@@ -623,22 +627,27 @@
             raise TypeError(
                 f"`Labware.well` must be called with an `int` or `str`, but got {idx}"
             )
 
     @requires_version(2, 0)
     def wells(self, *args: Union[str, int]) -> List[Well]:
         """
-        Accessor function that generates a list of wells in a top down,
-        left to right order. This is representative of moving down rows and
-        across columns (i.e., A1, B1, C1…A2, B2, C2…).
+        Accessor function to navigate a labware top to bottom, left to right.
+
+        i.e., this method returns a list ordered A1, B1, C1…A2, B2, C2….
 
-        With indexing one can treat it as a typical python
-        list. For example, access well A1 with ``labware.wells()[0]``.
+        Use indexing to access individual wells contained in the list.
+        For example, access well A1 with ``labware.wells()[0]``.
 
-        Note that this method takes args for backward-compatibility. But using args is deprecated and will be removed in future versions. Args can be either strings or integers, but must all be the same type. For example, ``self.columns(1, 4, 8)`` or ``self.columns('1', '2')`` are valid, but ``self.columns('1', 4)`` is not.
+        .. note::
+            Using args with this method is deprecated. Use indexing instead.
+
+            If your code uses args, they can be either strings or integers, but not a
+            mix of the two. For example, ``.wells(1, 4)`` or ``.wells("1", "4")`` is
+            valid, but ``.wells("1", 4)`` is not.
 
         :return: Ordered list of all wells in a labware.
         """
         if not args:
             return list(self._wells_by_name.values())
 
         elif validation.is_all_integers(args):
@@ -654,19 +663,18 @@
                 "`Labware.wells` must be called with all `int`'s or all `str`'s,"
                 f" but was called with {args}"
             )
 
     @requires_version(2, 0)
     def wells_by_name(self) -> Dict[str, Well]:
         """
-        Accessor function used to create a look-up table of wells by name.
+        Accessor function used to navigate through a labware by well name.
 
-        With indexing one can treat it as a typical Python
-        dictionary whose keys are well names. For example, access well A1
-        with ``labware.wells_by_name()['A1']``.
+        Use indexing to access individual wells contained in the dictionary.
+        For example, access well A1 with ``labware.wells_by_name()["A1"]``.
 
         :return: Dictionary of :py:class:`.Well` objects keyed by well name.
         """
         return dict(self._wells_by_name)
 
     @requires_version(2, 0)
     def wells_by_index(self) -> Dict[str, Well]:
@@ -678,21 +686,26 @@
             "wells_by_index is deprecated. Use wells_by_name or dict access instead."
         )
         return self.wells_by_name()
 
     @requires_version(2, 0)
     def rows(self, *args: Union[int, str]) -> List[List[Well]]:
         """
-        Accessor function used to navigate through a labware by row.
-
-        With indexing one can treat it as a typical python nested list.
-        For example, access row A with ``labware.rows()[0]``. This
-        will output ``['A1', 'A2', 'A3', 'A4'...]``.
+        Accessor function to navigate through a labware by row.
 
-        Note that this method takes args for backward-compatibility. But using args is deprecated and will be removed in future versions. Args can be either strings or integers, but must all be the same type. For example, ``self.columns(1, 4, 8)`` or ``self.columns('1', '2')`` are valid, but ``self.columns('1', 4)`` is not.
+        Use indexing to access individual rows or wells contained in the nested list.
+        On a standard 96-well plate, this will output a list of :py:class:`.Well`
+        objects containing A1 through A12.
+
+        .. note::
+            Using args with this method is deprecated. Use indexing instead.
+
+            If your code uses args, they can be either strings or integers, but not a
+            mix of the two. For example, ``.rows(1, 4)`` or ``.rows("1", "4")`` is
+            valid, but ``.rows("1", 4)`` is not.
 
         :return: A list of row lists.
         """
         if not args:
             return [
                 [self._wells_by_name[well_name] for well_name in row]
                 for row in self._well_grid.rows_by_name.values()
@@ -711,19 +724,20 @@
                 "`Labware.rows` must be called with all `int`'s or all `str`'s,"
                 f" but was called with {args}"
             )
 
     @requires_version(2, 0)
     def rows_by_name(self) -> Dict[str, List[Well]]:
         """
-        Accessor function used to navigate through a labware by row name.
+        Accessor function to navigate through a labware by row name.
 
-        With indexing one can treat it as a typical python dictionary.
-        For example, access row A with ``labware.rows_by_name()['A']``.
-        This will output ``['A1', 'A2', 'A3', 'A4'...]``.
+        Use indexing to access individual rows or wells contained in the dictionary.
+        For example, access row A with ``labware.rows_by_name()["A"]``.
+        On a standard 96-well plate, this will output a list of :py:class:`.Well`
+        objects containing A1 through A12.
 
         :return: Dictionary of :py:class:`.Well` lists keyed by row name.
         """
         return {
             row_name: [self._wells_by_name[well_name] for well_name in row]
             for row_name, row in self._well_grid.rows_by_name.items()
         }
@@ -736,24 +750,27 @@
         """
         _log.warning("rows_by_index is deprecated. Use rows_by_name instead.")
         return self.rows_by_name()
 
     @requires_version(2, 0)
     def columns(self, *args: Union[int, str]) -> List[List[Well]]:
         """
-        Accessor function used to navigate through a labware by column.
+        Accessor function to navigate through a labware by column.
 
-        With indexing one can treat it as a typical python nested list.
-        For example, access row A with ``labware.columns()[0]``.
-        This will output ``['A1', 'B1', 'C1', 'D1'...]``.
-
-        Note that this method takes args for backward-compatibility. But using args is deprecated and will be removed in future versions. Args
-        can be either strings or integers, but must all be the same type. For example,
-        ``self.columns(1, 4, 8)`` or ``self.columns('1', '2')`` are valid, but
-        ``self.columns('1', 4)`` is not.
+        Use indexing to access individual columns or wells contained in the nested list.
+        For example, access column 1 with ``labware.columns()[0]``.
+        On a standard 96-well plate, this will output a list of :py:class:`.Well`
+        objects containing A1 through H1.
+
+        .. note::
+            Using args with this method is deprecated. Use indexing instead.
+
+            If your code uses args, they can be either strings or integers, but not a
+            mix of the two. For example, ``.columns(1, 4)`` or ``.columns("1", "4")`` is
+            valid, but ``.columns("1", 4)`` is not.
 
         :return: A list of column lists.
         """
         if not args:
             return [
                 [self._wells_by_name[well_name] for well_name in column]
                 for column in self._well_grid.columns_by_name.values()
@@ -772,19 +789,20 @@
                 "`Labware.columns` must be called with all `int`'s or all `str`'s,"
                 f" but was called with {args}"
             )
 
     @requires_version(2, 0)
     def columns_by_name(self) -> Dict[str, List[Well]]:
         """
-        Accessor function used to navigate through a labware by column name.
+        Accessor function to navigate through a labware by column name.
 
-        With indexing one can treat it as a typical python dictionary.
-        For example, access row A with ``labware.columns_by_name()['1']``.
-        This will output ``['A1', 'B1', 'C1', 'D1'...]``.
+        Use indexing to access individual columns or wells contained in the dictionary.
+        For example, access column 1 with ``labware.columns_by_name()["1"]``.
+        On a standard 96-well plate, this will output a list of :py:class:`.Well`
+        objects containing A1 through H1.
 
         :return: Dictionary of :py:class:`.Well` lists keyed by column name.
         """
         return {
             column_name: [self._wells_by_name[well_name] for well_name in column]
             for column_name, column in self._well_grid.columns_by_name.items()
         }
@@ -801,36 +819,51 @@
     @property
     @requires_version(2, 0)
     def highest_z(self) -> float:
         """
         The z-coordinate of the highest single point anywhere on the labware.
 
         This is taken from the ``zDimension`` property of the ``dimensions`` object in the
-        labware definition and takes into account the calibration offset.
+        labware definition and takes into account the labware offset.
         """
         return self._core.highest_z
 
     @property
     def _is_tiprack(self) -> bool:
         """as is_tiprack but not subject to version checking for speed"""
         return self._core.is_tip_rack()
 
     @property
     @requires_version(2, 0)
     def is_tiprack(self) -> bool:
+        """Whether the labware behaves as a tip rack.
+
+        Returns ``True`` if the labware definition specifies ``isTiprack`` as ``True``.
+        """
         return self._is_tiprack
 
     @property
     @requires_version(2, 15)
     def is_adapter(self) -> bool:
+        """Whether the labware behaves as an adapter.
+
+        Returns ``True`` if the labware definition specifies ``adapter`` as one of the
+        labware's ``allowedRoles``.
+        """
         return self._core.is_adapter()
 
     @property
     @requires_version(2, 0)
     def tip_length(self) -> float:
+        """For a tip rack labware, the length of the tips it holds, in mm.
+
+        This is taken from the ``tipLength`` property of the ``parameters`` object in the labware definition.
+
+        This method will raise an exception if you call it on a labware that isn’t a tip rack.
+        """
         return self._core.get_tip_length()
 
     @tip_length.setter
     def tip_length(self, length: float) -> None:
         """
         Set the tip rack's tip length.
 
@@ -844,15 +877,19 @@
         # TODO(mc, 2023-02-06): this assert should be enough for mypy
         # investigate if upgrading mypy allows the `cast` to be removed
         assert isinstance(self._core, LegacyLabwareCore)
         cast(LegacyLabwareCore, self._core).set_tip_length(length)
 
     # TODO(mc, 2022-11-09): implementation detail; deprecate public method
     def next_tip(
-        self, num_tips: int = 1, starting_tip: Optional[Well] = None
+        self,
+        num_tips: int = 1,
+        starting_tip: Optional[Well] = None,
+        *,
+        nozzle_map: Optional[NozzleMap] = None,
     ) -> Optional[Well]:
         """
         Find the next valid well for pick-up.
 
         Determines the next valid start tip from which to retrieve the
         specified number of tips. There must be at least `num_tips` sequential
         wells for which all wells have tips, in the same column.
@@ -865,14 +902,15 @@
         :return: the :py:class:`.Well` meeting the target criteria, or None
         """
         assert num_tips > 0, f"num_tips must be positive integer, but got {num_tips}"
 
         well_name = self._core.get_next_tip(
             num_tips=num_tips,
             starting_tip=starting_tip._core if starting_tip else None,
+            nozzle_map=nozzle_map,
         )
 
         return self._wells_by_name[well_name] if well_name is not None else None
 
     def use_tips(self, start_well: Well, num_channels: int = 1) -> None:
         """
         Removes tips from the tip tracker.
@@ -996,15 +1034,21 @@
         assert isinstance(self._core, LegacyLabwareCore)
         cast(LegacyLabwareCore, self._core).get_tip_tracker().return_tips(
             start_well=start_well._core, num_channels=num_channels
         )
 
     @requires_version(2, 0)
     def reset(self) -> None:
-        """Reset all tips in a tip rack.
+        """Reset tip tracking for a tip rack.
+
+        After resetting, the API treats all wells on the rack as if they contain unused tips.
+        This is useful if you want to reuse tips after calling :py:meth:`.return_tip()`.
+
+        If you need to physically replace an empty tip rack in the middle of your protocol,
+        use :py:meth:`.move_labware()` instead. See :ref:`off-deck-location` for an example.
 
         .. versionchanged:: 2.14
             This method will raise an exception if you call it on a labware that isn't
             a tip rack. Formerly, it would do nothing.
         """
         self._core.reset_tips()
 
@@ -1016,54 +1060,69 @@
     except IndexError:
         rest = []
     return tip_racks[0], rest
 
 
 # TODO(mc, 2022-11-09): implementation detail, move to core
 def select_tiprack_from_list(
-    tip_racks: List[Labware], num_channels: int, starting_point: Optional[Well] = None
+    tip_racks: List[Labware],
+    num_channels: int,
+    starting_point: Optional[Well] = None,
+    *,
+    nozzle_map: Optional[NozzleMap] = None,
 ) -> Tuple[Labware, Well]:
     try:
         first, rest = split_tipracks(tip_racks)
     except IndexError:
         raise OutOfTipsError
 
     if starting_point and starting_point.parent != first:
         raise TipSelectionError(
             f"The starting tip you selected does not exist in {first}"
         )
     elif starting_point:
         first_well = starting_point
+    elif nozzle_map:
+        first_well = None
     else:
         first_well = first.wells()[0]
 
-    next_tip = first.next_tip(num_channels, first_well)
+    next_tip = first.next_tip(num_channels, first_well, nozzle_map=nozzle_map)
     if next_tip:
         return first, next_tip
     else:
-        return select_tiprack_from_list(rest, num_channels)
+        return select_tiprack_from_list(rest, num_channels, None, nozzle_map=nozzle_map)
 
 
 # TODO(mc, 2022-11-09): implementation detail, move to core
 def filter_tipracks_to_start(
     starting_point: Well, tipracks: List[Labware]
 ) -> List[Labware]:
     return list(dropwhile(lambda tr: starting_point.parent != tr, tipracks))
 
 
 # TODO(mc, 2022-11-09): implementation detail, move to core
 def next_available_tip(
-    starting_tip: Optional[Well], tip_racks: List[Labware], channels: int
+    starting_tip: Optional[Well],
+    tip_racks: List[Labware],
+    channels: int,
+    *,
+    nozzle_map: Optional[NozzleMap] = None,
 ) -> Tuple[Labware, Well]:
     start = starting_tip
     if start is None:
-        return select_tiprack_from_list(tip_racks, channels)
+        return select_tiprack_from_list(
+            tip_racks, channels, None, nozzle_map=nozzle_map
+        )
     else:
         return select_tiprack_from_list(
-            filter_tipracks_to_start(start, tip_racks), channels, start
+            filter_tipracks_to_start(start, tip_racks),
+            channels,
+            start,
+            nozzle_map=nozzle_map,
         )
 
 
 # TODO(mc, 2022-11-09): implementation detail, move somewhere else
 # only used in old calibration flows by robot-server
 def load_from_definition(
     definition: "LabwareDefinition",
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/module_contexts.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/module_contexts.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from typing import List, Optional, Union, cast
 
 from opentrons_shared_data.labware.dev_types import LabwareDefinition
 from opentrons_shared_data.module.dev_types import ModuleModel, ModuleType
 
 from opentrons.legacy_broker import LegacyBroker
 from opentrons.hardware_control.modules import ThermocyclerStep
-from opentrons.commands import module_commands as cmds
-from opentrons.commands.publisher import CommandPublisher, publish
+from opentrons.legacy_commands import module_commands as cmds
+from opentrons.legacy_commands.publisher import CommandPublisher, publish
 from opentrons.protocols.api_support.types import APIVersion
 from opentrons.protocols.api_support.util import APIVersionError, requires_version
 
 from .core.common import (
     ProtocolCore,
     LabwareCore,
     ModuleCore,
@@ -147,15 +147,15 @@
             loaded_adapter = self.load_adapter(
                 name=adapter,
                 namespace=namespace,
             )
             load_location = loaded_adapter._core
         else:
             load_location = self._core
-
+        name = validation.ensure_lowercase_name(name)
         labware_core = self._protocol_core.load_labware(
             load_name=name,
             label=label,
             namespace=namespace,
             version=version,
             location=load_location,
         )
@@ -463,17 +463,17 @@
 
         You shouldn't specify more than one of these parameters. However, if you do,
         their order of precedence is ``height``, then ``height_from_base``, then ``offset``.
         """
         if height is not None:
             if self._api_version >= _MAGNETIC_MODULE_HEIGHT_PARAM_REMOVED_IN:
                 raise APIVersionError(
-                    "The height parameter of MagneticModuleContext.engage() was removed"
-                    " in {_MAGNETIC_MODULE_HEIGHT_PARAM_REMOVED_IN}."
-                    " Use offset or height_from_base instead."
+                    f"The height parameter of MagneticModuleContext.engage() was removed"
+                    f" in {_MAGNETIC_MODULE_HEIGHT_PARAM_REMOVED_IN}."
+                    f" Use offset or height_from_base instead."
                 )
             self._core.engage(height_from_home=height)
 
         # This version check has a bug:
         # if the caller sets height_from_base in an API version that's too low,
         # we will silently ignore it instead of raising APIVersionError.
         # Leaving this unfixed because we haven't thought through
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/module_validation_and_errors.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/module_validation_and_errors.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/protocol_context.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/protocol_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,21 @@
 from opentrons_shared_data.labware.dev_types import LabwareDefinition
 from opentrons_shared_data.pipette.dev_types import PipetteNameType
 
 from opentrons.types import Mount, Location, DeckLocation, DeckSlotName, StagingSlotName
 from opentrons.legacy_broker import LegacyBroker
 from opentrons.hardware_control import SyncHardwareAPI
 from opentrons.hardware_control.modules.types import MagneticBlockModel
-from opentrons.commands import protocol_commands as cmds, types as cmd_types
-from opentrons.commands.helpers import stringify_labware_movement_command
-from opentrons.commands.publisher import CommandPublisher, publish, publish_context
+from opentrons.legacy_commands import protocol_commands as cmds, types as cmd_types
+from opentrons.legacy_commands.helpers import stringify_labware_movement_command
+from opentrons.legacy_commands.publisher import (
+    CommandPublisher,
+    publish,
+    publish_context,
+)
 from opentrons.protocols.api_support import instrument as instrument_support
 from opentrons.protocols.api_support.deck_type import (
     NoTrashDefinedError,
     should_load_fixed_trash_labware_for_python_protocol,
     should_load_fixed_trash_area_for_python_protocol,
 )
 from opentrons.protocols.api_support.types import APIVersion
@@ -48,27 +52,27 @@
     AbstractMagneticBlockCore,
 )
 from .core.engine import ENGINE_CORE_API_VERSION
 from .core.legacy.legacy_protocol_core import LegacyProtocolCore
 
 from . import validation
 from ._liquid import Liquid
-from ._trash_bin import TrashBin
-from ._waste_chute import WasteChute
+from .disposal_locations import TrashBin, WasteChute
 from .deck import Deck
 from .instrument_context import InstrumentContext
 from .labware import Labware
 from .module_contexts import (
     MagneticModuleContext,
     TemperatureModuleContext,
     ThermocyclerContext,
     HeaterShakerContext,
     MagneticBlockContext,
     ModuleContext,
 )
+from ._parameters import Parameters
 
 
 logger = logging.getLogger(__name__)
 
 
 ModuleTypes = Union[
     TemperatureModuleContext,
@@ -161,24 +165,18 @@
 
         self._load_fixed_trash()
         if should_load_fixed_trash_labware_for_python_protocol(self._api_version):
             self._core.append_disposal_location(self.fixed_trash)
         elif should_load_fixed_trash_area_for_python_protocol(
             self._api_version, self._core.robot_type
         ):
-            _fixed_trash_trashbin = TrashBin(
-                location=DeckSlotName.FIXED_TRASH, addressable_area_name="fixedTrash"
-            )
-            # We are just appending the fixed trash to the core's internal list here, not adding it to the engine via
-            # the core, since that method works through the SyncClient and if called from here, will cause protocols
-            # to deadlock. Instead, that method is called in protocol engine directly in create_protocol_context after
-            # ProtocolContext is initialized.
-            self._core.append_disposal_location(_fixed_trash_trashbin)
+            self._core.load_ot2_fixed_trash_bin()
 
         self._commands: List[str] = []
+        self._params: Parameters = Parameters()
         self._unsubscribe_commands: Optional[Callable[[], None]] = None
         self.clear_commands()
 
     @property
     @requires_version(2, 0)
     def api_version(self) -> APIVersion:
         """Return the API version specified for this protocol context.
@@ -219,14 +217,19 @@
         contents. The filename keys are formatted with extensions but without paths. For
         example, a file stored in the bundle as ``data/mydata/aspirations.csv`` will
         have the key ``"aspirations.csv"``. The values are :py:class:`bytes` objects
         representing the contents of the files.
         """
         return self._bundled_data
 
+    @property
+    @requires_version(2, 18)
+    def params(self) -> Parameters:
+        return self._params
+
     def cleanup(self) -> None:
         """Finalize and clean up the protocol context."""
         if self._unsubscribe_commands:
             self._unsubscribe_commands()
             self._unsubscribe_commands = None
 
     def __del__(self) -> None:
@@ -508,18 +511,15 @@
         if not isinstance(slot_name, DeckSlotName):
             raise ValueError("Staging areas not permitted for trash bin.")
         addressable_area_name = validation.ensure_and_convert_trash_bin_location(
             location,
             api_version=self._api_version,
             robot_type=self._core.robot_type,
         )
-        trash_bin = TrashBin(
-            location=slot_name, addressable_area_name=addressable_area_name
-        )
-        self._core.add_disposal_location_to_engine(trash_bin)
+        trash_bin = self._core.load_trash_bin(slot_name, addressable_area_name)
         return trash_bin
 
     @requires_version(2, 16)
     def load_waste_chute(
         self,
     ) -> WasteChute:
         """Load the waste chute on the deck of a Flex.
@@ -527,17 +527,15 @@
         See :ref:`configure-waste-chute` for details, including the deck configuration
         variants of the waste chute.
 
         The deck plate adapter for the waste chute can only go in slot D3. If you try to
         load another item in slot D3 after loading the waste chute, or vice versa, the
         API will raise an error.
         """
-        waste_chute = WasteChute()
-        self._core.add_disposal_location_to_engine(waste_chute)
-        return waste_chute
+        return self._core.load_waste_chute()
 
     @requires_version(2, 15)
     def load_adapter(
         self,
         load_name: str,
         location: Union[DeckLocation, OffDeckType],
         namespace: Optional[str] = None,
@@ -975,17 +973,17 @@
     @publish(command=cmds.pause)
     @requires_version(2, 0)
     def pause(self, msg: Optional[str] = None) -> None:
         """Pause execution of the protocol until it's resumed.
 
         A human can resume the protocol in the Opentrons App or on the touchscreen.
 
-        This function returns immediately, but the next function call that
-        is blocked by a paused robot (anything that involves moving) will
-        not return until the protocol is resumed.
+        .. note::
+            In Python Protocol API version 2.13 and earlier, the pause will only
+            take effect on the next function call that involves moving the robot.
 
         :param str msg: An optional message to show in the run log entry for the pause step.
         """
         self._core.pause(msg=msg)
 
     @publish(command=cmds.resume)
     @requires_version(2, 0)
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_api/validation.py` & `opentrons-7.3.0a0/src/opentrons/protocol_api/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,15 @@
     TemperatureModuleModel,
     ThermocyclerModuleModel,
     HeaterShakerModuleModel,
     MagneticBlockModel,
     ThermocyclerStep,
 )
 
-from ._trash_bin import TrashBin
-from ._waste_chute import WasteChute
+from .disposal_locations import TrashBin, WasteChute
 
 if TYPE_CHECKING:
     from .labware import Well
 
 
 # The first APIVersion where Python protocols can specify deck labels like "D1" instead of "1".
 _COORDINATE_DECK_LABEL_VERSION_GATE = APIVersion(2, 15)
@@ -84,14 +83,18 @@
     """An error raised when a labware is not loaded using `load_labware`."""
 
 
 class InvalidTrashBinLocationError(ValueError):
     """An error raised when attempting to load trash bins in invalid slots."""
 
 
+class InvalidFixtureLocationError(ValueError):
+    """An error raised when attempting to load a fixture in an invalid cutout."""
+
+
 def ensure_mount_for_pipette(
     mount: Union[str, Mount, None], pipette: PipetteNameType
 ) -> Mount:
     """Ensure that an input value represents a valid mount, and is valid for the given pipette."""
     if pipette == PipetteNameType.P1000_96:
         # Always validate the raw mount input, even if the pipette is a 96-channel and we're not going
         # to use the mount value.
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/__init__.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from .create_protocol_engine import (
     create_protocol_engine,
     create_protocol_engine_in_thread,
 )
 from .protocol_engine import ProtocolEngine
 from .errors import ProtocolEngineError, ErrorOccurrence
+from .notes import CommandNote
 from .commands import (
     Command,
     CommandParams,
     CommandCreate,
     CommandStatus,
     CommandType,
     CommandIntent,
@@ -75,14 +76,15 @@
     # top level command unions and values
     "Command",
     "CommandParams",
     "CommandCreate",
     "CommandStatus",
     "CommandType",
     "CommandIntent",
+    "CommandNote",
     # state interfaces and models
     "State",
     "StateView",
     "CommandSlice",
     "CurrentCommand",
     # public value interfaces and models
     "LabwareOffset",
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/actions/__init__.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/actions/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 from .action_handler import ActionHandler
 from .actions import (
     Action,
     PlayAction,
     PauseAction,
     PauseSource,
     StopAction,
+    ResumeFromRecoveryAction,
     FinishAction,
     HardwareStoppedAction,
     QueueCommandAction,
-    UpdateCommandAction,
+    RunCommandAction,
+    SucceedCommandAction,
     FailCommandAction,
     AddLabwareOffsetAction,
     AddLabwareDefinitionAction,
     AddLiquidAction,
     AddAddressableAreaAction,
     AddModuleAction,
     FinishErrorDetails,
@@ -33,18 +35,20 @@
     # action reaction interface
     "ActionHandler",
     # action values
     "Action",
     "PlayAction",
     "PauseAction",
     "StopAction",
+    "ResumeFromRecoveryAction",
     "FinishAction",
     "HardwareStoppedAction",
     "QueueCommandAction",
-    "UpdateCommandAction",
+    "RunCommandAction",
+    "SucceedCommandAction",
     "FailCommandAction",
     "AddLabwareOffsetAction",
     "AddLabwareDefinitionAction",
     "AddLiquidAction",
     "AddAddressableAreaAction",
     "AddModuleAction",
     "DoorChangeAction",
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/actions/action_dispatcher.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/actions/action_dispatcher.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/actions/actions.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/actions/actions.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 
 Actions can be passed to the ActionDispatcher, where they will trigger
 reactions in objects that subscribe to the pipeline, like the StateStore.
 """
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
-from typing import Optional, Union
+from typing import List, Optional, Union
 
 from opentrons.protocols.models import LabwareDefinition
 from opentrons.hardware_control.types import DoorState
 from opentrons.hardware_control.modules import LiveData
 
 from opentrons_shared_data.errors import EnumeratedError
 
 from ..commands import Command, CommandCreate, CommandPrivateResult
+from ..error_recovery_policy import ErrorRecoveryType
+from ..notes.notes import CommandNote
 from ..types import (
     LabwareOffsetCreate,
     ModuleDefinition,
     Liquid,
     DeckConfigurationType,
     AddressableAreaLocation,
 )
@@ -49,23 +51,27 @@
     """Pause processing commands in the engine."""
 
     source: PauseSource
 
 
 @dataclass(frozen=True)
 class StopAction:
-    """Stop the current engine execution.
-
-    After a StopAction, the engine status will be marked as stopped.
-    """
+    """Request engine execution to stop soon."""
 
     from_estop: bool = False
 
 
 @dataclass(frozen=True)
+class ResumeFromRecoveryAction:
+    """See `ProtocolEngine.resume_from_recovery()`."""
+
+    pass
+
+
+@dataclass(frozen=True)
 class FinishErrorDetails:
     """Error details for the payload of a FinishAction or HardwareStoppedAction."""
 
     error: Exception
     error_id: str
     created_at: datetime
 
@@ -106,38 +112,76 @@
 class QueueCommandAction:
     """Add a command request to the queue."""
 
     command_id: str
     created_at: datetime
     request: CommandCreate
     request_hash: Optional[str]
+    failed_command_id: Optional[str] = None
+
+
+@dataclass(frozen=True)
+class RunCommandAction:
+    """Mark a given command as running.
+
+    At the time of dispatching this action, the command must be queued,
+    and no other command may be running.
+    """
+
+    command_id: str
+    started_at: datetime
 
 
 @dataclass(frozen=True)
-class UpdateCommandAction:
-    """Update a given command."""
+class SucceedCommandAction:
+    """Mark a given command as succeeded.
+
+    At the time of dispatching this action, the command must be running.
+    """
 
     command: Command
+    """The command in its new succeeded state."""
+
     private_result: CommandPrivateResult
 
 
 @dataclass(frozen=True)
 class FailCommandAction:
     """Mark a given command as failed.
 
-    The given command and all currently queued commands will be marked
-    as failed due to the given error.
+    At the time of dispatching this action, the command must be running.
     """
 
-    # TODO(mc, 2021-11-12): we'll likely need to add the command params
-    # to this payload for state reaction purposes
     command_id: str
+    """The command to fail."""
+
     error_id: str
+    """An ID to assign to the command's error.
+
+    Must be unique to this occurrence of the error.
+    """
+
     failed_at: datetime
+    """When the command failed."""
+
     error: EnumeratedError
+    """The underlying exception that caused this command to fail."""
+
+    notes: List[CommandNote]
+    """Overwrite the command's `.notes` with these."""
+
+    type: ErrorRecoveryType
+    """How this error should be handled in the context of the overall run."""
+
+    # This is a quick hack so FailCommandAction handlers can get the params of the
+    # command that failed. We probably want this to be a new "failure details"
+    # object instead, similar to how succeeded commands can send a "private result"
+    # to Protocol Engine internals.
+    running_command: Command
+    """The command to fail, in its prior `running` state."""
 
 
 @dataclass(frozen=True)
 class AddLabwareOffsetAction:
     """Add a labware offset, to apply to subsequent `LoadLabwareCommand`s."""
 
     labware_offset_id: str
@@ -199,19 +243,21 @@
     speed: Optional[float]
 
 
 Action = Union[
     PlayAction,
     PauseAction,
     StopAction,
+    ResumeFromRecoveryAction,
     FinishAction,
     HardwareStoppedAction,
     DoorChangeAction,
     QueueCommandAction,
-    UpdateCommandAction,
+    RunCommandAction,
+    SucceedCommandAction,
     FailCommandAction,
     AddLabwareOffsetAction,
     AddLabwareDefinitionAction,
     AddModuleAction,
     AddAddressableAreaAction,
     AddLiquidAction,
     ResetTipsAction,
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/clients/sync_client.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/clients/sync_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 from typing import cast, List, Optional, Dict
 
 from opentrons_shared_data.pipette.dev_types import PipetteNameType
 from opentrons_shared_data.labware.dev_types import LabwareUri
 from opentrons_shared_data.labware.labware_definition import LabwareDefinition
 
-from opentrons.commands.protocol_commands import comment as make_legacy_comment_command
+from opentrons.legacy_commands.protocol_commands import (
+    comment as make_legacy_comment_command,
+)
 from opentrons.types import MountType
 from opentrons.hardware_control.modules.types import ThermocyclerStep
 
 from .. import commands
 from ..state import StateView
 from ..types import (
     DeckPoint,
@@ -21,14 +23,15 @@
     WellLocation,
     DropTipWellLocation,
     LabwareOffsetVector,
     MotorAxis,
     Liquid,
     NozzleLayoutConfigurationType,
     AddressableOffsetVector,
+    LabwareOffsetCreate,
 )
 from .transports import ChildThreadTransport
 
 
 class SyncClient:
     """Control a `ProtocolEngine` without async/await.
 
@@ -86,14 +89,18 @@
     def reset_tips(self, labware_id: str) -> None:
         """Reset a labware's tip tracking state.."""
         self._transport.call_method(
             "reset_tips",
             labware_id=labware_id,
         )
 
+    def add_labware_offset(self, request: LabwareOffsetCreate) -> None:
+        """Add a labware offset."""
+        self._transport.call_method("add_labware_offset", request=request)
+
     def set_pipette_movement_speed(
         self, pipette_id: str, speed: Optional[float]
     ) -> None:
         """Set the speed of a pipette's X/Y/Z movements. Does not affect plunger speed.
 
         None will use the hardware API's default.
         """
@@ -121,14 +128,27 @@
                 displayName=display_name,
             )
         )
         result = self._transport.execute_command(request=request)
 
         return cast(commands.LoadLabwareResult, result)
 
+    def reload_labware(
+        self,
+        labware_id: str,
+    ) -> commands.ReloadLabwareResult:
+        """Execute a ReloadLabware command and return the result."""
+        request = commands.ReloadLabwareCreate(
+            params=commands.ReloadLabwareParams(
+                labwareId=labware_id,
+            )
+        )
+        result = self._transport.execute_command(request=request)
+        return cast(commands.ReloadLabwareResult, result)
+
     # TODO (spp, 2022-12-14): https://opentrons.atlassian.net/browse/RLAB-237
     def move_labware(
         self,
         labware_id: str,
         new_location: LabwareLocation,
         strategy: LabwareMovementStrategy,
         pick_up_offset: Optional[LabwareOffsetVector],
@@ -290,14 +310,37 @@
                 wellLocation=well_location,
             )
         )
         result = self._transport.execute_command(request=request)
 
         return cast(commands.PickUpTipResult, result)
 
+    def pick_up_tip_wait_for_recovery(
+        self,
+        pipette_id: str,
+        labware_id: str,
+        well_name: str,
+        well_location: WellLocation,
+    ) -> commands.PickUpTip:
+        """Execute a PickUpTip, wait for any error recovery, and return it.
+
+        Note that the returned command will not necessarily have a `result`.
+        """
+        request = commands.PickUpTipCreate(
+            params=commands.PickUpTipParams(
+                pipetteId=pipette_id,
+                labwareId=labware_id,
+                wellName=well_name,
+                wellLocation=well_location,
+            )
+        )
+        command = self._transport.execute_command_wait_for_recovery(request=request)
+
+        return cast(commands.PickUpTip, command)
+
     def drop_tip(
         self,
         pipette_id: str,
         labware_id: str,
         well_name: str,
         well_location: DropTipWellLocation,
         home_after: Optional[bool],
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/__init__.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from . import heater_shaker
 from . import magnetic_module
 from . import temperature_module
 from . import thermocycler
 from . import calibration
 
-from .hash_command_params import hash_command_params
+from .hash_command_params import hash_protocol_command_params
 from .generate_command_schema import generate_command_schema
 
 from .command import (
     AbstractCommandImpl,
     BaseCommand,
     BaseCommandCreate,
     CommandStatus,
@@ -116,14 +116,22 @@
     LoadLabware,
     LoadLabwareParams,
     LoadLabwareCreate,
     LoadLabwareResult,
     LoadLabwareCommandType,
 )
 
+from .reload_labware import (
+    ReloadLabware,
+    ReloadLabwareParams,
+    ReloadLabwareCreate,
+    ReloadLabwareResult,
+    ReloadLabwareCommandType,
+)
+
 from .load_liquid import (
     LoadLiquid,
     LoadLiquidParams,
     LoadLiquidResult,
     LoadLiquidCreate,
     LoadLiquidCommandType,
     LoadLiquidImplementation,
@@ -329,15 +337,15 @@
     "AbstractCommandImpl",
     "AbstractCommandWithPrivateResultImpl",
     "BaseCommand",
     "BaseCommandCreate",
     "CommandStatus",
     "CommandIntent",
     # command parameter hashing
-    "hash_command_params",
+    "hash_protocol_command_params",
     # command schema generation
     "generate_command_schema",
     # aspirate command models
     "Aspirate",
     "AspirateCreate",
     "AspirateParams",
     "AspirateResult",
@@ -398,14 +406,20 @@
     "RetractAxisCommandType",
     # load labware command models
     "LoadLabware",
     "LoadLabwareCreate",
     "LoadLabwareParams",
     "LoadLabwareResult",
     "LoadLabwareCommandType",
+    # reload labware command models
+    "ReloadLabware",
+    "ReloadLabwareCreate",
+    "ReloadLabwareParams",
+    "ReloadLabwareResult",
+    "ReloadLabwareCommandType",
     # load module command models
     "LoadModule",
     "LoadModuleCreate",
     "LoadModuleParams",
     "LoadModuleResult",
     "LoadModuleCommandType",
     # load pipette command models
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/aspirate.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/aspirate.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from opentrons.hardware_control import HardwareControlAPI
 
 from ..types import WellLocation, WellOrigin, CurrentWell, DeckPoint
 
 if TYPE_CHECKING:
     from ..execution import MovementHandler, PipettingHandler
     from ..state import StateView
+    from ..notes import CommandNoteAdder
 
 
 AspirateCommandType = Literal["aspirate"]
 
 
 class AspirateParams(
     PipetteIdMixin, AspirateVolumeMixin, FlowRateMixin, WellLocationMixin
@@ -44,20 +45,22 @@
 
     def __init__(
         self,
         pipetting: PipettingHandler,
         state_view: StateView,
         hardware_api: HardwareControlAPI,
         movement: MovementHandler,
+        command_note_adder: CommandNoteAdder,
         **kwargs: object,
     ) -> None:
         self._pipetting = pipetting
         self._state_view = state_view
         self._hardware_api = hardware_api
         self._movement = movement
+        self._command_note_adder = command_note_adder
 
     async def execute(self, params: AspirateParams) -> AspirateResult:
         """Move to and aspirate from the requested well.
 
         Raises:
             TipNotAttachedError: if no tip is attached to the pipette.
         """
@@ -94,15 +97,18 @@
             labware_id=labware_id,
             well_name=well_name,
             well_location=params.wellLocation,
             current_well=current_well,
         )
 
         volume = await self._pipetting.aspirate_in_place(
-            pipette_id=pipette_id, volume=params.volume, flow_rate=params.flowRate
+            pipette_id=pipette_id,
+            volume=params.volume,
+            flow_rate=params.flowRate,
+            command_note_adder=self._command_note_adder,
         )
 
         return AspirateResult(
             volume=volume, position=DeckPoint(x=position.x, y=position.y, z=position.z)
         )
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/aspirate_in_place.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/aspirate_in_place.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 )
 from .command import AbstractCommandImpl, BaseCommand, BaseCommandCreate
 from ..errors.exceptions import PipetteNotReadyToAspirateError
 
 if TYPE_CHECKING:
     from ..execution import PipettingHandler
     from ..state import StateView
-
+    from ..notes import CommandNoteAdder
 
 AspirateInPlaceCommandType = Literal["aspirateInPlace"]
 
 
 class AspirateInPlaceParams(PipetteIdMixin, AspirateVolumeMixin, FlowRateMixin):
     """Payload required to aspirate in place."""
 
@@ -41,19 +41,21 @@
     """AspirateInPlace command implementation."""
 
     def __init__(
         self,
         pipetting: PipettingHandler,
         hardware_api: HardwareControlAPI,
         state_view: StateView,
+        command_note_adder: CommandNoteAdder,
         **kwargs: object,
     ) -> None:
         self._pipetting = pipetting
         self._state_view = state_view
         self._hardware_api = hardware_api
+        self._command_note_adder = command_note_adder
 
     async def execute(self, params: AspirateInPlaceParams) -> AspirateInPlaceResult:
         """Aspirate without moving the pipette.
 
         Raises:
             TipNotAttachedError: if no tip is attached to the pipette.
             PipetteNotReadyToAspirateError: pipette plunger is not ready.
@@ -65,15 +67,18 @@
         if not ready_to_aspirate:
             raise PipetteNotReadyToAspirateError(
                 "Pipette cannot aspirate in place because of a previous blow out."
                 " The first aspirate following a blow-out must be from a specific well"
                 " so the plunger can be reset in a known safe position."
             )
         volume = await self._pipetting.aspirate_in_place(
-            pipette_id=params.pipetteId, volume=params.volume, flow_rate=params.flowRate
+            pipette_id=params.pipetteId,
+            volume=params.volume,
+            flow_rate=params.flowRate,
+            command_note_adder=self._command_note_adder,
         )
 
         return AspirateInPlaceResult(volume=volume)
 
 
 class AspirateInPlace(BaseCommand[AspirateInPlaceParams, AspirateInPlaceResult]):
     """AspirateInPlace command model."""
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/blow_out.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/blow_out.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/blow_out_in_place.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/blow_out_in_place.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/calibration/__init__.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/calibration/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/calibration/calibrate_gripper.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/calibration/calibrate_gripper.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/calibration/calibrate_module.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/calibration/calibrate_module.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/calibration/calibrate_pipette.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/calibration/calibrate_pipette.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/command.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/command.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,34 +2,44 @@
 
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from datetime import datetime
 from enum import Enum
-from typing import TYPE_CHECKING, Generic, Optional, TypeVar, Tuple
+from typing import (
+    TYPE_CHECKING,
+    Generic,
+    Optional,
+    TypeVar,
+    Tuple,
+    List,
+    Type,
+    Union,
+)
 
 from pydantic import BaseModel, Field
 from pydantic.generics import GenericModel
 
 from opentrons.hardware_control import HardwareControlAPI
 
 from ..errors import ErrorOccurrence
+from ..notes import CommandNote, CommandNoteAdder
 
 # Work around type-only circular dependencies.
 if TYPE_CHECKING:
     from .. import execution
     from ..state import StateView
 
 
-CommandParamsT = TypeVar("CommandParamsT", bound=BaseModel)
-
-CommandResultT = TypeVar("CommandResultT", bound=BaseModel)
-
-CommandPrivateResultT = TypeVar("CommandPrivateResultT")
+_ParamsT = TypeVar("_ParamsT", bound=BaseModel)
+_ParamsT_contra = TypeVar("_ParamsT_contra", bound=BaseModel, contravariant=True)
+_ResultT = TypeVar("_ResultT", bound=BaseModel)
+_ResultT_co = TypeVar("_ResultT_co", bound=BaseModel, covariant=True)
+_PrivateResultT_co = TypeVar("_PrivateResultT_co", covariant=True)
 
 
 class CommandStatus(str, Enum):
     """Command execution status."""
 
     QUEUED = "queued"
     RUNNING = "running"
@@ -43,31 +53,32 @@
     Props:
         PROTOCOL: the command is part of the protocol run itself.
         SETUP: the command is part of the setup phase of a run.
     """
 
     PROTOCOL = "protocol"
     SETUP = "setup"
+    FIXIT = "fixit"
 
 
-class BaseCommandCreate(GenericModel, Generic[CommandParamsT]):
+class BaseCommandCreate(GenericModel, Generic[_ParamsT]):
     """Base class for command creation requests.
 
     You shouldn't use this class directly; instead, use or define
     your own subclass per specific command type.
     """
 
     commandType: str = Field(
         ...,
         description=(
             "Specific command type that determines data requirements and "
             "execution behavior"
         ),
     )
-    params: CommandParamsT = Field(..., description="Command execution data payload")
+    params: _ParamsT = Field(..., description="Command execution data payload")
     intent: Optional[CommandIntent] = Field(
         None,
         description=(
             "The reason the command was added. If not specified or `protocol`,"
             " the command will be treated as part of the protocol run itself,"
             " and added to the end of the existing command queue."
             "\n\n"
@@ -84,15 +95,15 @@
             "A key value, unique in this run, that can be used to track"
             " the same logical command across multiple runs of the same protocol."
             " If a value is not provided, one will be generated."
         ),
     )
 
 
-class BaseCommand(GenericModel, Generic[CommandParamsT, CommandResultT]):
+class BaseCommand(GenericModel, Generic[_ParamsT, _ResultT]):
     """Base command model.
 
     You shouldn't use this class directly; instead, use or define
     your own subclass per specific command type.
     """
 
     id: str = Field(
@@ -114,16 +125,16 @@
             " A command's `key` will be unique within a given run, but stable"
             " across all runs that perform the same exact procedure. Thus,"
             " `key` be used to compare/match commands across multiple runs"
             " of the same protocol."
         ),
     )
     status: CommandStatus = Field(..., description="Command execution status")
-    params: CommandParamsT = Field(..., description="Command execution data payload")
-    result: Optional[CommandResultT] = Field(
+    params: _ParamsT = Field(..., description="Command execution data payload")
+    result: Optional[_ResultT] = Field(
         None,
         description="Command execution result data, if succeeded",
     )
     error: Optional[ErrorOccurrence] = Field(
         None,
         description="Reference to error occurrence, if execution failed",
     )
@@ -140,19 +151,37 @@
         description=(
             "The reason the command was added to the run."
             " If not specified or `protocol`, it is part of the protocol itself."
             " If `setup`, it was added as part of setup; for example,"
             " a command that is part of a calibration procedure."
         ),
     )
+    notes: Optional[List[CommandNote]] = Field(
+        None,
+        description=(
+            "Information not critical to the execution of the command derived from either"
+            " the command's execution or the command's generation."
+        ),
+    )
+    failedCommandId: Optional[str] = Field(
+        None,
+        description=(
+            "FIXIT command use only. Reference of the failed command id we are trying to fix."
+        ),
+    )
+
+    _ImplementationCls: Union[
+        Type[AbstractCommandImpl[_ParamsT, _ResultT]],
+        Type[AbstractCommandWithPrivateResultImpl[_ParamsT, _ResultT, object]],
+    ]
 
 
 class AbstractCommandImpl(
     ABC,
-    Generic[CommandParamsT, CommandResultT],
+    Generic[_ParamsT_contra, _ResultT_co],
 ):
     """Abstract command creation and execution implementation.
 
     A given command request should map to a specific command implementation,
     which defines how to:
 
     - Create a command resource from the request model
@@ -172,27 +201,28 @@
         gantry_mover: execution.GantryMover,
         labware_movement: execution.LabwareMovementHandler,
         pipetting: execution.PipettingHandler,
         tip_handler: execution.TipHandler,
         run_control: execution.RunControlHandler,
         rail_lights: execution.RailLightsHandler,
         status_bar: execution.StatusBarHandler,
+        command_note_adder: CommandNoteAdder,
     ) -> None:
         """Initialize the command implementation with execution handlers."""
         pass
 
     @abstractmethod
-    async def execute(self, params: CommandParamsT) -> CommandResultT:
+    async def execute(self, params: _ParamsT_contra) -> _ResultT_co:
         """Execute the command, mapping data from execution into a response model."""
         ...
 
 
 class AbstractCommandWithPrivateResultImpl(
     ABC,
-    Generic[CommandParamsT, CommandResultT, CommandPrivateResultT],
+    Generic[_ParamsT_contra, _ResultT_co, _PrivateResultT_co],
 ):
     """Abstract command creation and execution implementation if the command has private results.
 
     A given command request should map to a specific command implementation,
     which defines how to:
 
     - Create a command resource from the request model
@@ -213,17 +243,18 @@
         gantry_mover: execution.GantryMover,
         labware_movement: execution.LabwareMovementHandler,
         pipetting: execution.PipettingHandler,
         tip_handler: execution.TipHandler,
         run_control: execution.RunControlHandler,
         rail_lights: execution.RailLightsHandler,
         status_bar: execution.StatusBarHandler,
+        command_note_adder: CommandNoteAdder,
     ) -> None:
         """Initialize the command implementation with execution handlers."""
         pass
 
     @abstractmethod
     async def execute(
-        self, params: CommandParamsT
-    ) -> Tuple[CommandResultT, CommandPrivateResultT]:
+        self, params: _ParamsT_contra
+    ) -> Tuple[_ResultT_co, _PrivateResultT_co]:
         """Execute the command, mapping data from execution into a response model."""
         ...
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/command_unions.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/command_unions.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,22 @@
     LoadLabware,
     LoadLabwareParams,
     LoadLabwareCreate,
     LoadLabwareResult,
     LoadLabwareCommandType,
 )
 
+from .reload_labware import (
+    ReloadLabware,
+    ReloadLabwareParams,
+    ReloadLabwareCreate,
+    ReloadLabwareResult,
+    ReloadLabwareCommandType,
+)
+
 from .load_liquid import (
     LoadLiquid,
     LoadLiquidParams,
     LoadLiquidCreate,
     LoadLiquidResult,
     LoadLiquidCommandType,
 )
@@ -300,14 +308,15 @@
         ConfigureForVolume,
         ConfigureNozzleLayout,
         DropTip,
         DropTipInPlace,
         Home,
         RetractAxis,
         LoadLabware,
+        ReloadLabware,
         LoadLiquid,
         LoadModule,
         LoadPipette,
         MoveLabware,
         MoveRelative,
         MoveToCoordinates,
         MoveToWell,
@@ -364,14 +373,15 @@
     BlowOutParams,
     BlowOutInPlaceParams,
     DropTipParams,
     DropTipInPlaceParams,
     HomeParams,
     RetractAxisParams,
     LoadLabwareParams,
+    ReloadLabwareParams,
     LoadLiquidParams,
     LoadModuleParams,
     LoadPipetteParams,
     MoveLabwareParams,
     MoveRelativeParams,
     MoveToCoordinatesParams,
     MoveToWellParams,
@@ -427,14 +437,15 @@
     BlowOutCommandType,
     BlowOutInPlaceCommandType,
     DropTipCommandType,
     DropTipInPlaceCommandType,
     HomeCommandType,
     RetractAxisCommandType,
     LoadLabwareCommandType,
+    ReloadLabwareCommandType,
     LoadLiquidCommandType,
     LoadModuleCommandType,
     LoadPipetteCommandType,
     MoveLabwareCommandType,
     MoveRelativeCommandType,
     MoveToCoordinatesCommandType,
     MoveToWellCommandType,
@@ -490,14 +501,15 @@
         BlowOutCreate,
         BlowOutInPlaceCreate,
         DropTipCreate,
         DropTipInPlaceCreate,
         HomeCreate,
         RetractAxisCreate,
         LoadLabwareCreate,
+        ReloadLabwareCreate,
         LoadLiquidCreate,
         LoadModuleCreate,
         LoadPipetteCreate,
         MoveLabwareCreate,
         MoveRelativeCreate,
         MoveToCoordinatesCreate,
         MoveToWellCreate,
@@ -554,14 +566,15 @@
     BlowOutResult,
     BlowOutInPlaceResult,
     DropTipResult,
     DropTipInPlaceResult,
     HomeResult,
     RetractAxisResult,
     LoadLabwareResult,
+    ReloadLabwareResult,
     LoadLiquidResult,
     LoadModuleResult,
     LoadPipetteResult,
     MoveLabwareResult,
     MoveRelativeResult,
     MoveToCoordinatesResult,
     MoveToWellResult,
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/comment.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/comment.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/configure_for_volume.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/configure_for_volume.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/configure_nozzle_layout.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/configure_nozzle_layout.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/custom.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/custom.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/dispense.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/dispense.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/dispense_in_place.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/dispense_in_place.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/drop_tip.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/drop_tip.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/drop_tip_in_place.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/drop_tip_in_place.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/generate_command_schema.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/generate_command_schema.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/get_tip_presence.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/get_tip_presence.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/hash_command_params.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/hash_command_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .command import CommandIntent
 from .command_unions import CommandCreate
 
 
 # TODO(mm, 2023-04-28):
 # This implementation will not notice that commands are different if they have different params
 # but share the same commandType. We should also hash command params. (Jira RCORE-326.)
-def hash_command_params(
+def hash_protocol_command_params(
     create: CommandCreate, last_hash: Optional[str]
 ) -> Optional[str]:
     """Given a command create object, return a hash.
 
     The hash is based on three things:
     - The command parameters
     - The latest hash (yo dawg I heard you like blockchains)
@@ -24,16 +24,15 @@
         create: The command create request.
         last_hash: The last command hash, if it exists.
 
     Returns:
         The command hash, if the command is a protocol command.
         `None` if the command is a setup command.
     """
-    if create.intent == CommandIntent.SETUP:
+    if create.intent in [CommandIntent.SETUP, CommandIntent.FIXIT]:
         return None
-    else:
-        # We avoid Python's built-in hash() function because it's not stable across
-        # runs of the Python interpreter. (Jira RSS-215.)
-        last_contribution = b"" if last_hash is None else last_hash.encode("ascii")
-        this_contribution = md5(create.commandType.encode("ascii")).digest()
-        to_hash = last_contribution + this_contribution
-        return md5(to_hash).hexdigest()
+    # We avoid Python's built-in hash() function because it's not stable across
+    # runs of the Python interpreter. (Jira RSS-215.)
+    last_contribution = b"" if last_hash is None else last_hash.encode("ascii")
+    this_contribution = md5(create.commandType.encode("ascii")).digest()
+    to_hash = last_contribution + this_contribution
+    return md5(to_hash).hexdigest()
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/heater_shaker/__init__.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/heater_shaker/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/heater_shaker/close_labware_latch.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/heater_shaker/close_labware_latch.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/heater_shaker/deactivate_heater.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/heater_shaker/deactivate_heater.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/heater_shaker/deactivate_shaker.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/heater_shaker/deactivate_shaker.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/heater_shaker/open_labware_latch.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/heater_shaker/open_labware_latch.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/heater_shaker/set_and_wait_for_shake_speed.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/heater_shaker/set_and_wait_for_shake_speed.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/heater_shaker/set_target_temperature.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/heater_shaker/set_target_temperature.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/heater_shaker/wait_for_temperature.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/heater_shaker/wait_for_temperature.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/home.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/home.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/load_labware.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/load_labware.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/load_liquid.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/load_liquid.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/load_module.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/load_module.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 """Implementation, request models, and response models for the load module command."""
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional, Type
 from typing_extensions import Literal
 from pydantic import BaseModel, Field
 
 from .command import AbstractCommandImpl, BaseCommand, BaseCommandCreate
-from ..types import DeckSlotLocation, ModuleModel, ModuleDefinition
+from ..types import (
+    DeckSlotLocation,
+    ModuleType,
+    ModuleModel,
+    ModuleDefinition,
+)
+from opentrons.types import DeckSlotName
+
+from opentrons.protocol_engine.resources import deck_configuration_provider
 
 if TYPE_CHECKING:
     from ..state import StateView
     from ..execution import EquipmentHandler
 
 
 LoadModuleCommandType = Literal["loadModule"]
@@ -100,17 +108,30 @@
         self, equipment: EquipmentHandler, state_view: StateView, **kwargs: object
     ) -> None:
         self._equipment = equipment
         self._state_view = state_view
 
     async def execute(self, params: LoadModuleParams) -> LoadModuleResult:
         """Check that the requested module is attached and assign its identifier."""
-        self._state_view.addressable_areas.raise_if_area_not_in_deck_configuration(
-            params.location.slotName.id
-        )
+        module_type = params.model.as_type()
+        self._ensure_module_location(params.location.slotName, module_type)
+
+        if self._state_view.config.robot_type == "OT-2 Standard":
+            self._state_view.addressable_areas.raise_if_area_not_in_deck_configuration(
+                params.location.slotName.id
+            )
+        else:
+            addressable_area = self._state_view.geometry._modules.ensure_and_convert_module_fixture_location(
+                deck_slot=params.location.slotName,
+                deck_type=self._state_view.config.deck_type,
+                model=params.model,
+            )
+            self._state_view.addressable_areas.raise_if_area_not_in_deck_configuration(
+                addressable_area
+            )
 
         verified_location = self._state_view.geometry.ensure_location_not_occupied(
             params.location
         )
 
         if params.model == ModuleModel.MAGNETIC_BLOCK_V1:
             loaded_module = await self._equipment.load_magnetic_block(
@@ -128,14 +149,38 @@
         return LoadModuleResult(
             moduleId=loaded_module.module_id,
             serialNumber=loaded_module.serial_number,
             model=loaded_module.definition.model,
             definition=loaded_module.definition,
         )
 
+    def _ensure_module_location(
+        self, slot: DeckSlotName, module_type: ModuleType
+    ) -> None:
+        if self._state_view.config.robot_type == "OT-2 Standard":
+            slot_def = self._state_view.addressable_areas.get_slot_definition(slot.id)
+            compatible_modules = slot_def["compatibleModuleTypes"]
+            if module_type.value not in compatible_modules:
+                raise ValueError(
+                    f"A {module_type.value} cannot be loaded into slot {slot}"
+                )
+        else:
+            cutout_fixture_id = ModuleType.to_module_fixture_id(module_type)
+            module_fixture = deck_configuration_provider.get_cutout_fixture(
+                cutout_fixture_id,
+                self._state_view.addressable_areas.state.deck_definition,
+            )
+            cutout_id = (
+                self._state_view.addressable_areas.get_cutout_id_by_deck_slot_name(slot)
+            )
+            if cutout_id not in module_fixture["mayMountTo"]:
+                raise ValueError(
+                    f"A {module_type.value} cannot be loaded into slot {slot}"
+                )
+
 
 class LoadModule(BaseCommand[LoadModuleParams, LoadModuleResult]):
     """The model for a load module command."""
 
     commandType: LoadModuleCommandType = "loadModule"
     params: LoadModuleParams
     result: Optional[LoadModuleResult]
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/load_pipette.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/load_pipette.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/magnetic_module/__init__.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/magnetic_module/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/magnetic_module/disengage.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/magnetic_module/disengage.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/magnetic_module/engage.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/magnetic_module/engage.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/move_labware.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/move_labware.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/move_relative.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/move_relative.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/move_to_addressable_area.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/move_to_addressable_area.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/move_to_addressable_area_for_drop_tip.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/move_to_addressable_area_for_drop_tip.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/move_to_coordinates.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/move_to_coordinates.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/move_to_well.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/move_to_well.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/pick_up_tip.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/pick_up_tip.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/pipetting_common.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/pipetting_common.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/prepare_to_aspirate.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/prepare_to_aspirate.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/retract_axis.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/retract_axis.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/save_position.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/save_position.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/set_rail_lights.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/set_rail_lights.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/set_status_bar.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/set_status_bar.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/temperature_module/__init__.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/temperature_module/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/temperature_module/deactivate.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/temperature_module/deactivate.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/temperature_module/set_target_temperature.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/temperature_module/set_target_temperature.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/temperature_module/wait_for_temperature.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/temperature_module/wait_for_temperature.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/thermocycler/__init__.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/thermocycler/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/thermocycler/close_lid.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/thermocycler/close_lid.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/thermocycler/deactivate_block.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/thermocycler/deactivate_block.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/thermocycler/deactivate_lid.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/thermocycler/deactivate_lid.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/thermocycler/open_lid.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/thermocycler/open_lid.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/thermocycler/run_profile.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/thermocycler/run_profile.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/thermocycler/set_target_block_temperature.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/thermocycler/set_target_block_temperature.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/thermocycler/set_target_lid_temperature.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/thermocycler/set_target_lid_temperature.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/thermocycler/wait_for_block_temperature.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/thermocycler/wait_for_block_temperature.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/thermocycler/wait_for_lid_temperature.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/thermocycler/wait_for_lid_temperature.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/touch_tip.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/touch_tip.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/verify_tip_presence.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/verify_tip_presence.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,29 +4,32 @@
 from pydantic import Field, BaseModel
 from typing import TYPE_CHECKING, Optional, Type
 from typing_extensions import Literal
 
 from .pipetting_common import PipetteIdMixin
 from .command import AbstractCommandImpl, BaseCommand, BaseCommandCreate
 
-from ..types import TipPresenceStatus
+from ..types import TipPresenceStatus, InstrumentSensorId
 
 if TYPE_CHECKING:
     from ..execution import TipHandler
 
 
 VerifyTipPresenceCommandType = Literal["verifyTipPresence"]
 
 
 class VerifyTipPresenceParams(PipetteIdMixin):
     """Payload required for a VerifyTipPresence command."""
 
     expectedState: TipPresenceStatus = Field(
         ..., description="The expected tip presence status on the pipette."
     )
+    followSingularSensor: Optional[InstrumentSensorId] = Field(
+        default=None, description="The sensor id to follow if the other can be ignored."
+    )
 
 
 class VerifyTipPresenceResult(BaseModel):
     """Result data from the execution of a VerifyTipPresence command."""
 
     pass
 
@@ -43,18 +46,24 @@
     ) -> None:
         self._tip_handler = tip_handler
 
     async def execute(self, params: VerifyTipPresenceParams) -> VerifyTipPresenceResult:
         """Verify if tip presence is as expected for the requested pipette."""
         pipette_id = params.pipetteId
         expected_state = params.expectedState
+        follow_singular_sensor = (
+            InstrumentSensorId.to_instrument_probe_type(params.followSingularSensor)
+            if params.followSingularSensor
+            else None
+        )
 
         await self._tip_handler.verify_tip_presence(
             pipette_id=pipette_id,
             expected=expected_state,
+            follow_singular_sensor=follow_singular_sensor,
         )
 
         return VerifyTipPresenceResult()
 
 
 class VerifyTipPresence(BaseCommand[VerifyTipPresenceParams, VerifyTipPresenceResult]):
     """VerifyTipPresence command model."""
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/wait_for_duration.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/wait_for_duration.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/commands/wait_for_resume.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/commands/wait_for_resume.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/create_protocol_engine.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/create_protocol_engine.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,22 +16,24 @@
 # TODO(mm, 2023-06-16): Arguably, this not being a context manager makes us prone to forgetting to
 # clean it up properly, especially in tests. See e.g. https://opentrons.atlassian.net/browse/RSS-222
 async def create_protocol_engine(
     hardware_api: HardwareControlAPI,
     config: Config,
     load_fixed_trash: bool = False,
     deck_configuration: typing.Optional[DeckConfigurationType] = None,
+    notify_publishers: typing.Optional[typing.Callable[[], None]] = None,
 ) -> ProtocolEngine:
     """Create a ProtocolEngine instance.
 
     Arguments:
         hardware_api: Hardware control API to pass down to dependencies.
         config: ProtocolEngine configuration.
         load_fixed_trash: Automatically load fixed trash labware in engine.
         deck_configuration: The initial deck configuration the engine will be instantiated with.
+        notify_publishers: Notifies robot server publishers of internal state change.
     """
     deck_data = DeckDataProvider(config.deck_type)
     deck_definition = await deck_data.get_deck_definition()
     deck_fixed_labware = (
         await deck_data.get_deck_fixed_labware(deck_definition)
         if load_fixed_trash
         else []
@@ -41,14 +43,15 @@
     state_store = StateStore(
         config=config,
         deck_definition=deck_definition,
         deck_fixed_labware=deck_fixed_labware,
         is_door_open=hardware_api.door_state is DoorState.OPEN,
         module_calibration_offsets=module_calibration_offsets,
         deck_configuration=deck_configuration,
+        notify_publishers=notify_publishers,
     )
 
     return ProtocolEngine(state_store=state_store, hardware_api=hardware_api)
 
 
 @contextlib.contextmanager
 def create_protocol_engine_in_thread(
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/errors/__init__.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/errors/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     FixtureDoesNotProvideAreasError,
     AreaNotInDeckConfigurationError,
     IncompatibleAddressableAreaError,
     FailedToPlanMoveError,
     MustHomeError,
     RunStoppedError,
     SetupCommandNotAllowedError,
+    FixitCommandNotAllowedError,
     ModuleNotAttachedError,
     ModuleAlreadyPresentError,
     WrongModuleTypeError,
     ThermocyclerNotOpenError,
     RobotDoorOpenError,
     PipetteMovementRestrictedByHeaterShakerError,
     HeaterShakerLabwareLatchNotOpenError,
@@ -51,24 +52,26 @@
     NoTargetTemperatureSetError,
     InvalidTargetSpeedError,
     InvalidTargetTemperatureError,
     InvalidBlockVolumeError,
     InvalidHoldTimeError,
     CannotPerformModuleAction,
     PauseNotAllowedError,
+    ResumeFromRecoveryNotAllowedError,
     GripperNotAttachedError,
     CannotPerformGripperAction,
     HardwareNotSupportedError,
     LabwareMovementNotAllowedError,
     LabwareIsNotAllowedInLocationError,
     LocationIsOccupiedError,
     LocationNotAccessibleByPipetteError,
     LocationIsStagingSlotError,
     InvalidAxisForRobotType,
     NotSupportedOnRobotType,
+    CommandNotAllowedError,
 )
 
 from .error_occurrence import ErrorOccurrence, ProtocolCommandFailedError
 
 __all__ = [
     # exceptions
     "ProtocolEngineError",
@@ -105,14 +108,15 @@
     "FixtureDoesNotProvideAreasError",
     "AreaNotInDeckConfigurationError",
     "IncompatibleAddressableAreaError",
     "FailedToPlanMoveError",
     "MustHomeError",
     "RunStoppedError",
     "SetupCommandNotAllowedError",
+    "FixitCommandNotAllowedError",
     "ModuleNotAttachedError",
     "ModuleAlreadyPresentError",
     "WrongModuleTypeError",
     "ThermocyclerNotOpenError",
     "RobotDoorOpenError",
     "PipetteMovementRestrictedByHeaterShakerError",
     "HeaterShakerLabwareLatchNotOpenError",
@@ -120,23 +124,24 @@
     "EngageHeightOutOfRangeError",
     "NoTargetTemperatureSetError",
     "InvalidTargetTemperatureError",
     "InvalidTargetSpeedError",
     "InvalidBlockVolumeError",
     "InvalidHoldTimeError",
     "CannotPerformModuleAction",
+    "ResumeFromRecoveryNotAllowedError",
     "PauseNotAllowedError",
     "ProtocolCommandFailedError",
     "GripperNotAttachedError",
     "CannotPerformGripperAction",
     "HardwareNotSupportedError",
     "LabwareMovementNotAllowedError",
     "LabwareIsNotAllowedInLocationError",
     "LocationIsOccupiedError",
     "LocationNotAccessibleByPipetteError",
     "LocationIsStagingSlotError",
     "InvalidAxisForRobotType",
     "NotSupportedOnRobotType",
     # error occurrence models
     "ErrorOccurrence",
-    "FailedGripperPickupError",
+    "CommandNotAllowedError",
 ]
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/errors/error_occurrence.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/errors/error_occurrence.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/errors/exceptions.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/errors/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -501,27 +501,66 @@
         details: Optional[Dict[str, Any]] = None,
         wrapping: Optional[Sequence[EnumeratedError]] = None,
     ) -> None:
         """Build a MustHomeError."""
         super().__init__(ErrorCodes.POSITION_UNKNOWN, message, details, wrapping)
 
 
+class CommandNotAllowedError(ProtocolEngineError):
+    """Raised when adding a command with bad data."""
+
+    def __init__(
+        self,
+        message: Optional[str] = None,
+        details: Optional[Dict[str, Any]] = None,
+        wrapping: Optional[Sequence[EnumeratedError]] = None,
+    ) -> None:
+        """Build a CommandNotAllowedError."""
+        super().__init__(ErrorCodes.GENERAL_ERROR, message, details, wrapping)
+
+
+class FixitCommandNotAllowedError(ProtocolEngineError):
+    """Raised when adding a fixit command to a non-recoverable engine."""
+
+    def __init__(
+        self,
+        message: Optional[str] = None,
+        details: Optional[Dict[str, Any]] = None,
+        wrapping: Optional[Sequence[EnumeratedError]] = None,
+    ) -> None:
+        """Build a SetupCommandNotAllowedError."""
+        super().__init__(ErrorCodes.GENERAL_ERROR, message, details, wrapping)
+
+
 class SetupCommandNotAllowedError(ProtocolEngineError):
     """Raised when adding a setup command to a non-idle/non-paused engine."""
 
     def __init__(
         self,
         message: Optional[str] = None,
         details: Optional[Dict[str, Any]] = None,
         wrapping: Optional[Sequence[EnumeratedError]] = None,
     ) -> None:
         """Build a SetupCommandNotAllowedError."""
         super().__init__(ErrorCodes.GENERAL_ERROR, message, details, wrapping)
 
 
+class ResumeFromRecoveryNotAllowedError(ProtocolEngineError):
+    """Raised when attempting to resume a run from recovery that has a fixit command in the queue."""
+
+    def __init__(
+        self,
+        message: Optional[str] = None,
+        details: Optional[Dict[str, Any]] = None,
+        wrapping: Optional[Sequence[EnumeratedError]] = None,
+    ) -> None:
+        """Build a ResumeFromRecoveryNotAllowedError."""
+        super().__init__(ErrorCodes.GENERAL_ERROR, message, details, wrapping)
+
+
 class PauseNotAllowedError(ProtocolEngineError):
     """Raised when attempting to pause a run that is not running."""
 
     def __init__(
         self,
         message: Optional[str] = None,
         details: Optional[Dict[str, Any]] = None,
@@ -947,24 +986,26 @@
         wrapping: Optional[Sequence[EnumeratedError]] = None,
     ) -> None:
         """Build a InvalidAxisForRobotType."""
         super().__init__(ErrorCodes.GENERAL_ERROR, message, details, wrapping)
 
 
 class EStopActivatedError(ProtocolEngineError):
-    """Raised when an operation's required pipette tip is not attached."""
+    """Represents an E-stop event."""
 
     def __init__(
         self,
-        message: Optional[str] = None,
-        details: Optional[Dict[str, Any]] = None,
         wrapping: Optional[Sequence[EnumeratedError]] = None,
     ) -> None:
         """Build an EStopActivatedError."""
-        super().__init__(ErrorCodes.E_STOP_ACTIVATED, message, details, wrapping)
+        super().__init__(
+            code=ErrorCodes.E_STOP_ACTIVATED,
+            message="E-stop activated.",
+            wrapping=wrapping,
+        )
 
 
 class NotSupportedOnRobotType(ProtocolEngineError):
     """Raised when attempting to perform an action that is not supported for the given robot type."""
 
     def __init__(
         self,
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/__init__.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .create_queue_worker import create_queue_worker
 from .equipment import (
     EquipmentHandler,
     LoadedLabwareData,
     LoadedPipetteData,
     LoadedModuleData,
     LoadedConfigureForVolumeData,
+    ReloadedLabwareData,
 )
 from .movement import MovementHandler
 from .gantry_mover import GantryMover
 from .labware_movement import LabwareMovementHandler
 from .pipetting import PipettingHandler
 from .tip_handler import TipHandler
 from .queue_worker import QueueWorker
@@ -25,14 +26,15 @@
 
 
 __all__ = [
     "CommandExecutor",
     "create_queue_worker",
     "EquipmentHandler",
     "LoadedLabwareData",
+    "ReloadedLabwareData",
     "LoadedPipetteData",
     "LoadedModuleData",
     "LoadedConfigureForVolumeData",
     "MovementHandler",
     "GantryMover",
     "PipettingHandler",
     "TipHandler",
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/create_queue_worker.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/create_queue_worker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """QueueWorker and dependency factory."""
 from opentrons.hardware_control import HardwareControlAPI
+from opentrons.protocol_engine.error_recovery_policy import ErrorRecoveryPolicy
 from opentrons.protocol_engine.execution.rail_lights import RailLightsHandler
 
 from ..state import StateStore
 from ..actions import ActionDispatcher
 from .equipment import EquipmentHandler
 from .movement import MovementHandler
 from .gantry_mover import create_gantry_mover
@@ -16,31 +17,32 @@
 from .status_bar import StatusBarHandler
 
 
 def create_queue_worker(
     hardware_api: HardwareControlAPI,
     state_store: StateStore,
     action_dispatcher: ActionDispatcher,
+    error_recovery_policy: ErrorRecoveryPolicy,
 ) -> QueueWorker:
     """Create a ready-to-use QueueWorker instance.
 
     Arguments:
         hardware_api: Hardware control API to pass down to dependencies.
         state_store: StateStore to pass down to dependencies.
         action_dispatcher: ActionDispatcher to pass down to dependencies.
+        error_recovery_policy: ErrorRecoveryPolicy to pass down to dependencies.
     """
     gantry_mover = create_gantry_mover(
         hardware_api=hardware_api,
         state_view=state_store,
     )
 
     equipment_handler = EquipmentHandler(
         hardware_api=hardware_api,
         state_store=state_store,
-        action_dispatcher=action_dispatcher,
     )
 
     movement_handler = MovementHandler(
         hardware_api=hardware_api,
         state_store=state_store,
         gantry_mover=gantry_mover,
     )
@@ -81,13 +83,14 @@
         gantry_mover=gantry_mover,
         labware_movement=labware_movement_handler,
         pipetting=pipetting_handler,
         tip_handler=tip_handler,
         run_control=run_control_handler,
         rail_lights=rail_lights_handler,
         status_bar=status_bar_handler,
+        error_recovery_policy=error_recovery_policy,
     )
 
     return QueueWorker(
         state_store=state_store,
         command_executor=command_executor,
     )
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/door_watcher.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/door_watcher.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/equipment.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/equipment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Equipment command side-effect logic."""
 from dataclasses import dataclass
-from typing import Optional, overload
+from typing import Optional, overload, Union
 
 from opentrons_shared_data.pipette.dev_types import PipetteNameType
 
 from opentrons.calibration_storage.helpers import uri_from_details
 from opentrons.protocols.models import LabwareDefinition
 from opentrons.types import MountType
 from opentrons.hardware_control import HardwareControlAPI
@@ -18,15 +18,14 @@
 from opentrons.hardware_control.nozzle_manager import NozzleMap
 from opentrons.protocol_engine.state.module_substates import (
     MagneticModuleId,
     HeaterShakerModuleId,
     TemperatureModuleId,
     ThermocyclerModuleId,
 )
-from ..actions import ActionDispatcher
 from ..errors import (
     FailedToLoadPipetteError,
     LabwareDefinitionDoesNotExistError,
     ModuleNotAttachedError,
 )
 from ..resources import (
     LabwareDataProvider,
@@ -40,27 +39,36 @@
     DeckSlotLocation,
     ModuleLocation,
     OnLabwareLocation,
     LabwareOffset,
     LabwareOffsetLocation,
     ModuleModel,
     ModuleDefinition,
+    AddressableAreaLocation,
 )
 
 
 @dataclass(frozen=True)
 class LoadedLabwareData:
     """The result of a load labware procedure."""
 
     labware_id: str
     definition: LabwareDefinition
     offsetId: Optional[str]
 
 
 @dataclass(frozen=True)
+class ReloadedLabwareData:
+    """The result of a reload labware procedure."""
+
+    location: LabwareLocation
+    offsetId: Optional[str]
+
+
+@dataclass(frozen=True)
 class LoadedPipetteData:
     """The result of a load pipette procedure."""
 
     pipette_id: str
     serial_number: str
     static_config: pipette_data_provider.LoadedStaticPipetteData
 
@@ -94,26 +102,24 @@
     _model_utils: ModelUtils
     _virtual_pipette_data_provider: pipette_data_provider.VirtualPipetteDataProvider
 
     def __init__(
         self,
         hardware_api: HardwareControlAPI,
         state_store: StateStore,
-        action_dispatcher: ActionDispatcher,
         labware_data_provider: Optional[LabwareDataProvider] = None,
         module_data_provider: Optional[ModuleDataProvider] = None,
         model_utils: Optional[ModelUtils] = None,
         virtual_pipette_data_provider: Optional[
             pipette_data_provider.VirtualPipetteDataProvider
         ] = None,
     ) -> None:
         """Initialize an EquipmentHandler instance."""
         self._hardware_api = hardware_api
         self._state_store = state_store
-        self._action_dispatcher = action_dispatcher
         self._labware_data_provider = labware_data_provider or LabwareDataProvider()
         self._module_data_provider = module_data_provider or ModuleDataProvider()
         self._model_utils = model_utils or ModelUtils()
         self._virtual_pipette_data_provider = (
             virtual_pipette_data_provider
             or pipette_data_provider.VirtualPipetteDataProvider()
         )
@@ -169,14 +175,33 @@
             labware_location=location,
         )
 
         return LoadedLabwareData(
             labware_id=labware_id, definition=definition, offsetId=offset_id
         )
 
+    async def reload_labware(self, labware_id: str) -> ReloadedLabwareData:
+        """Reload an already-loaded labware. This cannot change the labware location.
+
+        Args:
+            labware_id: The ID of the already-loaded labware.
+
+        Raises:
+            LabwareNotLoadedError: If `labware_id` does not reference a loaded labware.
+
+        """
+        location = self._state_store.labware.get_location(labware_id)
+        definition_uri = self._state_store.labware.get_definition_uri(labware_id)
+        offset_id = self.find_applicable_labware_offset_id(
+            labware_definition_uri=definition_uri,
+            labware_location=location,
+        )
+
+        return ReloadedLabwareData(location=location, offsetId=offset_id)
+
     async def load_pipette(
         self,
         pipette_name: PipetteNameType,
         mount: MountType,
         pipette_id: Optional[str],
     ) -> LoadedPipetteData:
         """Ensure the requested pipette is attached.
@@ -198,15 +223,14 @@
         pipette_name_value = (
             pipette_name.value
             if isinstance(pipette_name, PipetteNameType)
             else pipette_name
         )
 
         pipette_id = pipette_id or self._model_utils.generate_id()
-
         if not use_virtual_pipettes:
             cache_request = {mount.to_hw_mount(): pipette_name_value}
 
             # TODO(mc, 2022-12-09): putting the other pipette in the cache request
             # is only to support protocol analysis, since the hardware simulator
             # does not cache requested virtual instruments. Remove per
             # https://opentrons.atlassian.net/browse/RLIQ-258
@@ -240,25 +264,24 @@
             serial_number = self._model_utils.generate_id(prefix="fake-serial-number-")
             static_pipette_config = (
                 self._virtual_pipette_data_provider.get_virtual_pipette_static_config(
                     pipette_name_value, pipette_id
                 )
             )
         serial = serial_number or ""
-
         return LoadedPipetteData(
             pipette_id=pipette_id,
             serial_number=serial,
             static_config=static_pipette_config,
         )
 
     async def load_magnetic_block(
         self,
         model: ModuleModel,
-        location: DeckSlotLocation,
+        location: Union[DeckSlotLocation, AddressableAreaLocation],
         module_id: Optional[str],
     ) -> LoadedModuleData:
         """Ensure the required magnetic block is attached.
 
         Args:
             model: The model name of the module.
             location: The deck location of the module
@@ -315,18 +338,22 @@
                     definition=self._module_data_provider.get_definition(
                         ModuleModel(hw_mod.model())
                     ),
                 )
                 for hw_mod in self._hardware_api.attached_modules
             ]
 
+            serial_number_at_locaiton = self._state_store.geometry._addressable_areas.get_fixture_serial_from_deck_configuration_by_deck_slot(
+                location.slotName
+            )
             attached_module = self._state_store.modules.select_hardware_module_to_load(
                 model=model,
                 location=location,
                 attached_modules=attached_modules,
+                expected_serial_number=serial_number_at_locaiton,
             )
 
         else:
             attached_module = HardwareModule(
                 serial_number=self._model_utils.generate_id(
                     prefix="fake-serial-number-"
                 ),
@@ -386,15 +413,15 @@
 
     async def configure_nozzle_layout(
         self,
         pipette_id: str,
         primary_nozzle: Optional[str] = None,
         front_right_nozzle: Optional[str] = None,
         back_left_nozzle: Optional[str] = None,
-    ) -> Optional[NozzleMap]:
+    ) -> NozzleMap:
         """Ensure the requested nozzle layout is compatible with the current pipette.
 
         Args:
             pipette_id: The identifier for the pipette.
             primary_nozzle: The nozzle which will be used as the
             front_right_nozzle
             back_left_nozzle
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/gantry_mover.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/gantry_mover.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/hardware_stopper.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/hardware_stopper.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/heater_shaker_movement_flagger.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/heater_shaker_movement_flagger.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/labware_movement.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/labware_movement.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/movement.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/movement.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/pipetting.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/pipetting.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Optional, Iterator
 from typing_extensions import Protocol as TypingProtocol
 from contextlib import contextmanager
 
 from opentrons.hardware_control import HardwareControlAPI
 
 from ..state import StateView, HardwarePipette
+from ..notes import CommandNoteAdder, CommandNote
 from ..errors.exceptions import (
     TipNotAttachedError,
     InvalidAspirateVolumeError,
     InvalidPushOutVolumeError,
     InvalidDispenseVolumeError,
 )
 
@@ -35,14 +36,15 @@
         """Prepare for pipette aspiration."""
 
     async def aspirate_in_place(
         self,
         pipette_id: str,
         volume: float,
         flow_rate: float,
+        command_note_adder: CommandNoteAdder,
     ) -> float:
         """Set flow-rate and aspirate."""
 
     async def dispense_in_place(
         self,
         pipette_id: str,
         volume: float,
@@ -84,19 +86,23 @@
         await self._hardware_api.prepare_for_aspirate(mount=hw_mount)
 
     async def aspirate_in_place(
         self,
         pipette_id: str,
         volume: float,
         flow_rate: float,
+        command_note_adder: CommandNoteAdder,
     ) -> float:
         """Set flow-rate and aspirate."""
         # get mount and config data from state and hardware controller
         adjusted_volume = _validate_aspirate_volume(
-            state_view=self._state_view, pipette_id=pipette_id, aspirate_volume=volume
+            state_view=self._state_view,
+            pipette_id=pipette_id,
+            aspirate_volume=volume,
+            command_note_adder=command_note_adder,
         )
         hw_pipette = self._state_view.pipettes.get_hardware_pipette(
             pipette_id=pipette_id,
             attached_pipettes=self._hardware_api.attached_instruments,
         )
         with self._set_flow_rate(pipette=hw_pipette, aspirate_flow_rate=flow_rate):
             await self._hardware_api.aspirate(
@@ -195,19 +201,23 @@
         """Virtually prepare to aspirate (no-op)."""
 
     async def aspirate_in_place(
         self,
         pipette_id: str,
         volume: float,
         flow_rate: float,
+        command_note_adder: CommandNoteAdder,
     ) -> float:
         """Virtually aspirate (no-op)."""
         self._validate_tip_attached(pipette_id=pipette_id, command_name="aspirate")
         return _validate_aspirate_volume(
-            state_view=self._state_view, pipette_id=pipette_id, aspirate_volume=volume
+            state_view=self._state_view,
+            pipette_id=pipette_id,
+            aspirate_volume=volume,
+            command_note_adder=command_note_adder,
         )
 
     async def dispense_in_place(
         self,
         pipette_id: str,
         volume: float,
         flow_rate: float,
@@ -248,15 +258,18 @@
         HardwarePipettingHandler(state_view=state_view, hardware_api=hardware_api)
         if state_view.config.use_virtual_pipettes is False
         else VirtualPipettingHandler(state_view=state_view)
     )
 
 
 def _validate_aspirate_volume(
-    state_view: StateView, pipette_id: str, aspirate_volume: float
+    state_view: StateView,
+    pipette_id: str,
+    aspirate_volume: float,
+    command_note_adder: CommandNoteAdder,
 ) -> float:
     """Get whether the given volume is valid to aspirate right now.
 
     Return the volume to aspirate, possibly clamped, or raise an
     InvalidAspirateVolumeError.
     """
     working_volume = state_view.pipettes.get_working_volume(pipette_id=pipette_id)
@@ -281,15 +294,29 @@
                 pipette_id=pipette_id
             ),
             max_tip_volume=_get_max_tip_volume(
                 state_view=state_view, pipette_id=pipette_id
             ),
         )
     else:
-        return min(aspirate_volume, available_volume)
+        volume_to_aspirate = min(aspirate_volume, available_volume)
+        if volume_to_aspirate < aspirate_volume:
+            command_note_adder(
+                CommandNote(
+                    noteKind="warning",
+                    shortMessage=f"Aspirate clamped to {available_volume} µL",
+                    longMessage=(
+                        f"Command requested to aspirate {aspirate_volume} µL but only"
+                        f" {available_volume} µL were available in the pipette. This is"
+                        " probably a floating point artifact."
+                    ),
+                    source="execution",
+                )
+            )
+        return volume_to_aspirate
 
 
 def _validate_dispense_volume(
     state_view: StateView, pipette_id: str, dispense_volume: float
 ) -> float:
     """Get whether the given volume is valid to dispense right now.
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/queue_worker.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/queue_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,17 @@
 
     async def _run_commands(self) -> None:
         while True:
             try:
                 command_id = await self._state_store.wait_for(
                     condition=self._state_store.commands.get_next_to_execute
                 )
+                # Assert for type hinting. This is valid because the wait_for() above
+                # only returns when the value is truthy.
+                assert command_id is not None
             except RunStoppedError:
                 # There are no more commands that we should execute, either because the run has
                 # completed on its own, or because a client requested it to stop.
                 break
             else:
                 await self._command_executor.execute(command_id=command_id)
                 # Yield to the event loop in case we're executing a long sequence of commands
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/rail_lights.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/rail_lights.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/run_control.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/run_control.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/status_bar.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/status_bar.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/thermocycler_movement_flagger.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/thermocycler_movement_flagger.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/thermocycler_plate_lifter.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/thermocycler_plate_lifter.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/execution/tip_handler.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/execution/tip_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Tip pickup and drop procedures."""
 from typing import Optional, Dict
 from typing_extensions import Protocol as TypingProtocol
 
 from opentrons.hardware_control import HardwareControlAPI
-from opentrons.hardware_control.types import FailedTipStateCheck
+from opentrons.hardware_control.types import FailedTipStateCheck, InstrumentProbeType
 from opentrons_shared_data.errors.exceptions import (
     CommandPreconditionViolated,
     CommandParameterLimitViolated,
     PythonException,
 )
 
 from ..resources import LabwareDataProvider, ensure_ot3_hardware
@@ -70,15 +70,18 @@
     async def add_tip(self, pipette_id: str, tip: TipGeometry) -> None:
         """Tell the Hardware API that a tip is attached."""
 
     async def get_tip_presence(self, pipette_id: str) -> TipPresenceStatus:
         """Get tip presence status on the pipette."""
 
     async def verify_tip_presence(
-        self, pipette_id: str, expected: TipPresenceStatus
+        self,
+        pipette_id: str,
+        expected: TipPresenceStatus,
+        follow_singular_sensor: Optional[InstrumentProbeType] = None,
     ) -> None:
         """Verify the expected tip presence status."""
 
 
 async def _available_for_nozzle_layout(
     channels: int,
     style: str,
@@ -233,25 +236,30 @@
             status = await ot3api.get_tip_presence_status(hw_mount)
             return TipPresenceStatus.from_hw_state(status)
         except HardwareNotSupportedError:
             # Tip presence sensing is not supported on the OT2
             return TipPresenceStatus.UNKNOWN
 
     async def verify_tip_presence(
-        self, pipette_id: str, expected: TipPresenceStatus
+        self,
+        pipette_id: str,
+        expected: TipPresenceStatus,
+        follow_singular_sensor: Optional[InstrumentProbeType] = None,
     ) -> None:
         """Verify the expecterd tip presence status of the pipette.
 
         This function will raise an exception if the specified tip presence status
         isn't matched.
         """
         try:
             ot3api = ensure_ot3_hardware(hardware_api=self._hardware_api)
             hw_mount = self._state_view.pipettes.get_mount(pipette_id).to_hw_mount()
-            await ot3api.verify_tip_presence(hw_mount, expected.to_hw_state())
+            await ot3api.verify_tip_presence(
+                hw_mount, expected.to_hw_state(), follow_singular_sensor
+            )
         except HardwareNotSupportedError:
             # Tip presence sensing is not supported on the OT2
             pass
         except FailedTipStateCheck as e:
             if expected == TipPresenceStatus.ABSENT:
                 raise TipAttachedError(wrapping=[PythonException(e)])
             elif expected == TipPresenceStatus.PRESENT:
@@ -328,15 +336,18 @@
         """Add a tip using a virtual pipette.
 
         This should not be called when using virtual pipettes.
         """
         assert False, "TipHandler.add_tip should not be used with virtual pipettes"
 
     async def verify_tip_presence(
-        self, pipette_id: str, expected: TipPresenceStatus
+        self,
+        pipette_id: str,
+        expected: TipPresenceStatus,
+        follow_singular_sensor: Optional[InstrumentProbeType] = None,
     ) -> None:
         """Verify tip presence.
 
         This should not be called when using virtual pipettes.
         """
 
     async def get_tip_presence(self, pipette_id: str) -> TipPresenceStatus:
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/plugins.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/plugins.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/protocol_engine.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/protocol_engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 """ProtocolEngine class definition."""
 from contextlib import AsyncExitStack
 from logging import getLogger
 from typing import Dict, Optional, Union
+from opentrons.protocol_engine.actions.actions import ResumeFromRecoveryAction
+from opentrons.protocol_engine.error_recovery_policy import (
+    ErrorRecoveryPolicy,
+    error_recovery_by_ff,
+)
 
 from opentrons.protocols.models import LabwareDefinition
 from opentrons.hardware_control import HardwareControlAPI
 from opentrons.hardware_control.modules import AbstractModule as HardwareModuleAPI
 from opentrons.hardware_control.types import PauseType as HardwarePauseType
 from opentrons_shared_data.errors import (
     ErrorCodes,
     EnumeratedError,
 )
 
-from .errors import ProtocolCommandFailedError, ErrorOccurrence
+from .errors import ProtocolCommandFailedError, ErrorOccurrence, CommandNotAllowedError
 from .errors.exceptions import EStopActivatedError
 from . import commands, slot_standardization
 from .resources import ModelUtils, ModuleDataProvider
 from .types import (
     LabwareOffset,
     LabwareOffsetCreate,
     LabwareUri,
@@ -48,15 +53,14 @@
     AddLabwareDefinitionAction,
     AddLiquidAction,
     AddAddressableAreaAction,
     AddModuleAction,
     HardwareStoppedAction,
     ResetTipsAction,
     SetPipetteMovementSpeedAction,
-    FailCommandAction,
 )
 
 
 _log = getLogger(__name__)
 
 
 class ProtocolEngine:
@@ -85,14 +89,15 @@
         action_dispatcher: Optional[ActionDispatcher] = None,
         plugin_starter: Optional[PluginStarter] = None,
         queue_worker: Optional[QueueWorker] = None,
         model_utils: Optional[ModelUtils] = None,
         hardware_stopper: Optional[HardwareStopper] = None,
         door_watcher: Optional[DoorWatcher] = None,
         module_data_provider: Optional[ModuleDataProvider] = None,
+        error_recovery_policy: ErrorRecoveryPolicy = error_recovery_by_ff,
     ) -> None:
         """Initialize a ProtocolEngine instance.
 
         Must be called while an event loop is active.
 
         This constructor does not inject provider implementations.
         Prefer the `create_protocol_engine()` factory function.
@@ -108,14 +113,15 @@
             state=self._state_store,
             action_dispatcher=self._action_dispatcher,
         )
         self._queue_worker = queue_worker or create_queue_worker(
             hardware_api=hardware_api,
             state_store=self._state_store,
             action_dispatcher=self._action_dispatcher,
+            error_recovery_policy=error_recovery_policy,
         )
         self._hardware_stopper = hardware_stopper or HardwareStopper(
             hardware_api=hardware_api,
             state_store=state_store,
         )
         self._door_watcher = door_watcher or DoorWatcher(
             state_store=state_store,
@@ -147,54 +153,81 @@
         self._action_dispatcher.dispatch(action)
 
         if self._state_store.commands.get_is_door_blocking():
             self._hardware_api.pause(HardwarePauseType.PAUSE)
         else:
             self._hardware_api.resume(HardwarePauseType.PAUSE)
 
-    def pause(self) -> None:
-        """Pause executing commands in the queue."""
+    def request_pause(self) -> None:
+        """Make command execution pause soon.
+
+        This will try to pause in the middle of the ongoing command, if there is one.
+        Otherwise, whenever the next command begins, the pause will happen then.
+        """
         action = self._state_store.commands.validate_action_allowed(
             PauseAction(source=PauseSource.CLIENT)
         )
         self._action_dispatcher.dispatch(action)
         self._hardware_api.pause(HardwarePauseType.PAUSE)
 
-    def add_command(self, request: commands.CommandCreate) -> commands.Command:
+    def resume_from_recovery(self) -> None:
+        """Resume normal protocol execution after the engine was `AWAITING_RECOVERY`."""
+        action = self._state_store.commands.validate_action_allowed(
+            ResumeFromRecoveryAction()
+        )
+        self._action_dispatcher.dispatch(action)
+
+    def add_command(
+        self, request: commands.CommandCreate, failed_command_id: Optional[str] = None
+    ) -> commands.Command:
         """Add a command to the `ProtocolEngine`'s queue.
 
         Arguments:
             request: The command type and payload data used to construct
                 the command in state.
 
         Returns:
             The full, newly queued command.
 
         Raises:
             SetupCommandNotAllowed: the request specified a setup command,
                 but the engine was not idle or paused.
             RunStoppedError: the run has been stopped, so no new commands
                 may be added.
+            CommandNotAllowedError: the request specified a failed command id
+                with a non fixit command.
         """
         request = slot_standardization.standardize_command(
             request, self.state_view.config.robot_type
         )
 
+        if failed_command_id and request.intent != commands.CommandIntent.FIXIT:
+            raise CommandNotAllowedError(
+                "failed command id should be supplied with a FIXIT command."
+            )
+
         command_id = self._model_utils.generate_id()
-        request_hash = commands.hash_command_params(
-            create=request,
-            last_hash=self._state_store.commands.get_latest_command_hash(),
-        )
+        if request.intent in (
+            commands.CommandIntent.SETUP,
+            commands.CommandIntent.FIXIT,
+        ):
+            request_hash = None
+        else:
+            request_hash = commands.hash_protocol_command_params(
+                create=request,
+                last_hash=self._state_store.commands.get_latest_protocol_command_hash(),
+            )
 
         action = self.state_view.commands.validate_action_allowed(
             QueueCommandAction(
                 request=request,
                 request_hash=request_hash,
                 command_id=command_id,
                 created_at=self._model_utils.get_timestamp(),
+                failed_command_id=failed_command_id,
             )
         )
         self._action_dispatcher.dispatch(action)
         return self._state_store.commands.get(command_id)
 
     async def wait_for_command(self, command_id: str) -> None:
         """Wait for a command to be completed.
@@ -215,85 +248,104 @@
         execute. You only need to call `play` once.
 
         Arguments:
             request: The command type and payload data used to construct
                 the command in state.
 
         Returns:
-            The command. If the command completed, it will be succeeded or failed.
+            The command.
+
+            If the command completed, it will be succeeded or failed.
+
             If the engine was stopped before it reached the command,
             the command will be queued.
         """
         command = self.add_command(request)
         await self.wait_for_command(command.id)
         return self._state_store.commands.get(command.id)
 
-    def estop(self, maintenance_run: bool) -> None:
-        """Signal to the engine that an estop event occurred.
+    async def add_and_execute_command_wait_for_recovery(
+        self, request: commands.CommandCreate
+    ) -> commands.Command:
+        """Like `add_and_execute_command()`, except wait for error recovery.
 
-        If there are any queued commands for the engine, they will be marked
-        as failed due to the estop event. If there aren't any queued commands
-        *and* this is a maintenance run (which has commands queued one-by-one),
-        a series of actions will mark the engine as Stopped. In either case the
-        queue worker will be deactivated; the primary difference is that the former
-        case will expect the protocol runner to `finish()` the engine, whereas the
-        maintenance run will be put into a state wherein the engine can be discarded.
-        """
-        if self._state_store.commands.get_is_stopped():
-            return
-        current_id = (
-            self._state_store.commands.state.running_command_id
-            or self._state_store.commands.state.queued_command_ids.head(None)
-        )
+        Unlike `add_and_execute_command()`, if the command fails, this will not
+        immediately return the failed command. Instead, if the error is recoverable,
+        it will wait until error recovery has completed (e.g. when some other task
+        calls `self.resume_from_recovery()`).
 
-        if current_id is not None:
-            fail_action = FailCommandAction(
-                command_id=current_id,
-                error_id=self._model_utils.generate_id(),
-                failed_at=self._model_utils.get_timestamp(),
-                error=EStopActivatedError(message="Estop Activated"),
-            )
-            self._action_dispatcher.dispatch(fail_action)
+        Returns:
+            The command.
+
+            If the command completed, it will be succeeded or failed. If it failed
+            and then its failure was recovered from, it will still be failed.
+
+            If the engine was stopped before it reached the command,
+            the command will be queued.
+        """
+        queued_command = self.add_command(request)
+        await self.wait_for_command(command_id=queued_command.id)
+        completed_command = self._state_store.commands.get(queued_command.id)
+        await self._state_store.wait_for_not(
+            self.state_view.commands.get_recovery_in_progress_for_command,
+            queued_command.id,
+        )
+        return completed_command
+
+    def estop(self) -> None:
+        """Signal to the engine that an E-stop event occurred.
+
+        If an estop happens while the robot is moving, lower layers physically stop
+        motion and raise the event as an exception, which fails the Protocol Engine
+        command. No action from the `ProtocolEngine` caller is needed to handle that.
+
+        However, if an estop happens in between commands, or in the middle of
+        a command like `comment` or `waitForDuration` that doesn't access the hardware,
+        `ProtocolEngine` needs to be told about it so it can interrupt the command
+        and stop executing any more. This method is how to do that.
 
-            # In the case where the running command was a setup command - check if there
-            # are any pending *run* commands and, if so, clear them all
-            current_id = self._state_store.commands.state.queued_command_ids.head(None)
-            if current_id is not None:
-                fail_action = FailCommandAction(
-                    command_id=current_id,
-                    error_id=self._model_utils.generate_id(),
-                    failed_at=self._model_utils.get_timestamp(),
-                    error=EStopActivatedError(message="Estop Activated"),
-                )
-                self._action_dispatcher.dispatch(fail_action)
-            self._queue_worker.cancel()
-        elif maintenance_run:
-            stop_action = self._state_store.commands.validate_action_allowed(
+        This acts roughly like `request_stop()`. After calling this, you should call
+        `finish()` with an EStopActivatedError.
+        """
+        try:
+            action = self._state_store.commands.validate_action_allowed(
                 StopAction(from_estop=True)
             )
-            self._action_dispatcher.dispatch(stop_action)
-            hardware_stop_action = HardwareStoppedAction(
-                completed_at=self._model_utils.get_timestamp(),
-                finish_error_details=FinishErrorDetails(
-                    error=EStopActivatedError(message="Estop Activated"),
-                    error_id=self._model_utils.generate_id(),
-                    created_at=self._model_utils.get_timestamp(),
-                ),
+        except Exception:  # todo(mm, 2024-04-16): Catch a more specific type.
+            # This is likely called from some hardware API callback that doesn't care
+            # about ProtocolEngine lifecycle or what methods are valid to call at what
+            # times. So it makes more sense for us to no-op here than to propagate this
+            # as an error.
+            _log.info(
+                "ProtocolEngine cannot handle E-stop event right now. Ignoring it.",
+                exc_info=True,
             )
-            self._action_dispatcher.dispatch(hardware_stop_action)
-            self._queue_worker.cancel()
-        else:
-            _log.info("estop pressed before protocol was started, taking no action.")
+            return
+        self._action_dispatcher.dispatch(action)
+        # self._queue_worker.cancel() will try to interrupt any ongoing command.
+        # Unfortunately, if it's a hardware command, this interruption will race
+        # against the E-stop exception propagating up from lower layers. But we need to
+        # do this because we want to make sure non-hardware commands, like
+        # `waitForDuration`, are also interrupted.
+        self._queue_worker.cancel()
+        # Unlike self.request_stop(), we don't need to do
+        # self._hardware_api.cancel_execution_and_running_tasks(). Since this was an
+        # E-stop event, the hardware API already knows.
 
-    async def stop(self) -> None:
-        """Stop execution immediately, halting all motion and cancelling future commands.
+    async def request_stop(self) -> None:
+        """Make command execution stop soon.
 
-        After an engine has been `stop`'ed, it cannot be restarted.
+        This will try to interrupt the ongoing command, if there is one. Future commands
+        are canceled. However, by the time this method returns, things may not have
+        settled by the time this method returns; the last command may still be
+        running.
 
-        After a `stop`, you must still call `finish` to give the engine a chance
+        After a stop has been requested, the engine cannot be restarted.
+
+        After a stop request, you must still call `finish` to give the engine a chance
         to clean up resources and propagate errors.
         """
         action = self._state_store.commands.validate_action_allowed(StopAction())
         self._action_dispatcher.dispatch(action)
         self._queue_worker.cancel()
         if self._hardware_api.is_movement_execution_taskified():
             # We 'taskify' hardware controller movement functions when running protocols
@@ -304,55 +356,60 @@
             # run function execution, just like `_queue_worker.cancel()` does for
             # engine-backed runs.
             await self._hardware_api.cancel_execution_and_running_tasks()
 
     async def wait_until_complete(self) -> None:
         """Wait until there are no more commands to execute.
 
-        Raises:
-            CommandExecutionFailedError: if any protocol command failed.
+        If a command encountered a fatal error, it's raised as an exception.
         """
         await self._state_store.wait_for(
             condition=self._state_store.commands.get_all_commands_final
         )
+        self._state_store.commands.raise_fatal_command_error()
 
     async def finish(
         self,
         error: Optional[Exception] = None,
         drop_tips_after_run: bool = True,
         set_run_status: bool = True,
         post_run_hardware_state: PostRunHardwareState = PostRunHardwareState.HOME_AND_STAY_ENGAGED,
     ) -> None:
-        """Gracefully finish using the ProtocolEngine, waiting for it to become idle.
+        """Finish using the `ProtocolEngine`.
+
+        This does a few things:
+
+        1. It may do post-run actions like homing and dropping tips. This depends on the
+           arguments passed as well as heuristics based on the history of the engine.
+        2. It waits for the engine to be done controlling the robot's hardware.
+        3. It releases internal resources, like background tasks.
 
-        The engine will finish executing its current command (if any),
-        and then shut down. After an engine has been `finished`'ed, it cannot
-        be restarted.
+        It's safe to call `finish()` multiple times. After you call `finish()`,
+        the engine can't be restarted.
 
         This method should not raise. If any exceptions happened during execution that were not
-        properly caught by the CommandExecutor, or if any exceptions happen during this
+        properly caught by `ProtocolEngine` internals, or if any exceptions happen during this
         `finish()` call, they should be saved as `.state_view.get_summary().errors`.
 
         Arguments:
             error: An error that caused the stop, if applicable.
             drop_tips_after_run: Whether to drop tips as part of cleanup.
             set_run_status: Whether to calculate a `success` or `failure` run status.
                 If `False`, will set status to `stopped`.
             post_run_hardware_state: The state in which to leave the gantry and motors in
                 after the run is over.
         """
         if self._state_store.commands.state.stopped_by_estop:
             # This handles the case where the E-stop was pressed while we were *not* in the middle
             # of some hardware interaction that would raise it as an exception. For example, imagine
-            # we were paused between two commands, or imagine we were executing a very long run of
-            # comment commands.
+            # we were paused between two commands, or imagine we were executing a waitForDuration.
             drop_tips_after_run = False
             post_run_hardware_state = PostRunHardwareState.DISENGAGE_IN_PLACE
             if error is None:
-                error = EStopActivatedError(message="Estop was activated during a run")
+                error = EStopActivatedError()
 
         if error:
             # If the run had an error, check if that error indicates an E-stop.
             # This handles the case where the run was in the middle of some hardware control
             # method and the hardware controller raised an E-stop error from it.
             #
             # To do this, we need to scan all the way through the error tree.
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/resources/__init__.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/resources/deck_configuration_provider.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/resources/deck_configuration_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Deck configuration resource provider."""
 from typing import List, Set, Tuple
 
-from opentrons_shared_data.deck.dev_types import DeckDefinitionV4, CutoutFixture
+from opentrons_shared_data.deck.dev_types import DeckDefinitionV5, CutoutFixture
 
 from opentrons.types import DeckSlotName
 
 from ..types import (
     AddressableArea,
     AreaType,
     PotentialCutoutFixture,
@@ -13,67 +13,64 @@
     Dimensions,
     AddressableOffsetVector,
 )
 from ..errors import (
     CutoutDoesNotExistError,
     FixtureDoesNotExistError,
     AddressableAreaDoesNotExistError,
-    FixtureDoesNotProvideAreasError,
 )
 
 
-def get_cutout_position(cutout_id: str, deck_definition: DeckDefinitionV4) -> DeckPoint:
+def get_cutout_position(cutout_id: str, deck_definition: DeckDefinitionV5) -> DeckPoint:
     """Get the base position of a cutout on the deck."""
     for cutout in deck_definition["locations"]["cutouts"]:
         if cutout_id == cutout["id"]:
             position = cutout["position"]
             return DeckPoint(x=position[0], y=position[1], z=position[2])
     else:
         raise CutoutDoesNotExistError(f"Could not find cutout with name {cutout_id}")
 
 
 def get_cutout_fixture(
-    cutout_fixture_id: str, deck_definition: DeckDefinitionV4
+    cutout_fixture_id: str, deck_definition: DeckDefinitionV5
 ) -> CutoutFixture:
     """Gets cutout fixture from deck that matches the cutout fixture ID provided."""
     for cutout_fixture in deck_definition["cutoutFixtures"]:
         if cutout_fixture["id"] == cutout_fixture_id:
             return cutout_fixture
     raise FixtureDoesNotExistError(
         f"Could not find cutout fixture with name {cutout_fixture_id}"
     )
 
 
 def get_provided_addressable_area_names(
-    cutout_fixture_id: str, cutout_id: str, deck_definition: DeckDefinitionV4
+    cutout_fixture_id: str, cutout_id: str, deck_definition: DeckDefinitionV5
 ) -> List[str]:
     """Gets a list of the addressable areas provided by the cutout fixture on the cutout."""
     cutout_fixture = get_cutout_fixture(cutout_fixture_id, deck_definition)
     try:
         return cutout_fixture["providesAddressableAreas"][cutout_id]
-    except KeyError as exception:
-        raise FixtureDoesNotProvideAreasError(
-            f"Cutout fixture {cutout_fixture['id']} does not provide addressable areas for {cutout_id}"
-        ) from exception
+    except KeyError:
+        return []
 
 
 def get_addressable_area_display_name(
-    addressable_area_name: str, deck_definition: DeckDefinitionV4
+    addressable_area_name: str, deck_definition: DeckDefinitionV5
 ) -> str:
     """Get the display name for an addressable area name."""
     for addressable_area in deck_definition["locations"]["addressableAreas"]:
         if addressable_area["id"] == addressable_area_name:
             return addressable_area["displayName"]
     raise AddressableAreaDoesNotExistError(
         f"Could not find addressable area with name {addressable_area_name}"
     )
 
 
 def get_potential_cutout_fixtures(
-    addressable_area_name: str, deck_definition: DeckDefinitionV4
+    addressable_area_name: str, deck_definition: DeckDefinitionV5
 ) -> Tuple[str, Set[PotentialCutoutFixture]]:
     """Given an addressable area name, gets the cutout ID associated with it and a set of potential fixtures."""
     potential_fixtures = []
     for cutout_fixture in deck_definition["cutoutFixtures"]:
         for cutout_id, provided_areas in cutout_fixture[
             "providesAddressableAreas"
         ].items():
@@ -98,15 +95,15 @@
     return cutout_id, set(potential_fixtures)
 
 
 def get_addressable_area_from_name(
     addressable_area_name: str,
     cutout_position: DeckPoint,
     base_slot: DeckSlotName,
-    deck_definition: DeckDefinitionV4,
+    deck_definition: DeckDefinitionV5,
 ) -> AddressableArea:
     """Given a name and a cutout position, get an addressable area on the deck."""
     for addressable_area in deck_definition["locations"]["addressableAreas"]:
         if addressable_area["id"] == addressable_area_name:
             area_offset = addressable_area["offsetFromCutoutFixture"]
             position = AddressableOffsetVector(
                 x=area_offset[0] + cutout_position.x,
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/resources/deck_data_provider.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/resources/deck_data_provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import anyio
 
 from opentrons_shared_data.deck import (
     load as load_deck,
     DEFAULT_DECK_DEFINITION_VERSION,
 )
-from opentrons_shared_data.deck.dev_types import DeckDefinitionV4
+from opentrons_shared_data.deck.dev_types import DeckDefinitionV5
 from opentrons.protocols.models import LabwareDefinition
 from opentrons.types import DeckSlotName
 
 from ..types import DeckSlotLocation, DeckType
 from .labware_data_provider import LabwareDataProvider
 
 
@@ -35,27 +35,27 @@
     def __init__(
         self, deck_type: DeckType, labware_data: Optional[LabwareDataProvider] = None
     ) -> None:
         """Initialize a DeckDataProvider."""
         self._deck_type = deck_type
         self._labware_data = labware_data or LabwareDataProvider()
 
-    async def get_deck_definition(self) -> DeckDefinitionV4:
+    async def get_deck_definition(self) -> DeckDefinitionV5:
         """Get a labware definition given the labware's identification."""
 
-        def sync() -> DeckDefinitionV4:
+        def sync() -> DeckDefinitionV5:
             return load_deck(
                 name=self._deck_type.value, version=DEFAULT_DECK_DEFINITION_VERSION
             )
 
         return await anyio.to_thread.run_sync(sync)
 
     async def get_deck_fixed_labware(
         self,
-        deck_definition: DeckDefinitionV4,
+        deck_definition: DeckDefinitionV5,
     ) -> List[DeckFixedLabware]:
         """Get a list of all labware fixtures from a given deck definition."""
         labware: List[DeckFixedLabware] = []
 
         for fixture in deck_definition["locations"]["legacyFixtures"]:
             labware_id = fixture["id"]
             load_name = cast(Optional[str], fixture.get("labware"))
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/resources/fixture_validation.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/resources/fixture_validation.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/resources/labware_data_provider.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/resources/labware_data_provider.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/resources/labware_validation.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/resources/labware_validation.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/resources/model_utils.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/resources/model_utils.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/resources/module_data_provider.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/resources/module_data_provider.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/resources/ot3_validation.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/resources/ot3_validation.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/resources/pipette_data_provider.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/resources/pipette_data_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,18 +33,17 @@
     home_position: float
     nozzle_offset_z: float
     flow_rates: FlowRates
     tip_configuration_lookup_table: Dict[
         float, pipette_definition.SupportedTipsDefinition
     ]
     nominal_tip_overlap: Dict[str, float]
+    nozzle_map: NozzleMap
     back_left_corner_offset: Point
     front_right_corner_offset: Point
-    back_left_nozzle_offset: Point
-    front_right_nozzle_offset: Point
 
 
 class VirtualPipetteDataProvider:
     """Provide pipette data without requiring hardware control."""
 
     def __init__(self) -> None:
         """Build a VirtualPipetteDataProvider."""
@@ -173,22 +172,21 @@
                 default_blow_out=tip_configuration.default_blowout_flowrate.values_by_api_level,
                 default_aspirate=tip_configuration.default_aspirate_flowrate.values_by_api_level,
                 default_dispense=tip_configuration.default_dispense_flowrate.values_by_api_level,
             ),
             nominal_tip_overlap=config.liquid_properties[
                 liquid_class
             ].tip_overlap_dictionary,
+            nozzle_map=nozzle_manager.current_configuration,
             back_left_corner_offset=Point(
                 pip_back_left[0], pip_back_left[1], pip_back_left[2]
             ),
             front_right_corner_offset=Point(
                 pip_front_right[0], pip_front_right[1], pip_front_right[2]
             ),
-            back_left_nozzle_offset=nozzle_manager.current_configuration.back_left_nozzle_offset,
-            front_right_nozzle_offset=nozzle_manager.current_configuration.front_right_nozzle_offset,
         )
 
     def get_virtual_pipette_static_config(
         self, pipette_name: PipetteName, pipette_id: str
     ) -> LoadedStaticPipetteData:
         """Get the config for a virtual pipette, given only the pipette name."""
         pipette_model = pipette_load_name.convert_pipette_name(pipette_name)
@@ -216,21 +214,15 @@
             k.value: v for k, v in pipette_dict["supported_tips"].items()
         },
         nominal_tip_overlap=pipette_dict["tip_overlap"],
         # TODO(mc, 2023-02-28): these two values are not present in PipetteDict
         # https://opentrons.atlassian.net/browse/RCORE-655
         home_position=0,
         nozzle_offset_z=0,
-        # TODO (spp): Confirm that the nozzle map is populated by the hardware api by default
-        back_left_nozzle_offset=pipette_dict[
-            "current_nozzle_map"
-        ].back_left_nozzle_offset,
-        front_right_nozzle_offset=pipette_dict[
-            "current_nozzle_map"
-        ].front_right_nozzle_offset,
+        nozzle_map=pipette_dict["current_nozzle_map"],
         back_left_corner_offset=Point(
             back_left_offset[0], back_left_offset[1], back_left_offset[2]
         ),
         front_right_corner_offset=Point(
             front_right_offset[0], front_right_offset[1], front_right_offset[2]
         ),
     )
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/slot_standardization.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/slot_standardization.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/state/__init__.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/state/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 """Protocol engine state module."""
 
 from .state import State, StateStore, StateView
 from .state_summary import StateSummary
 from .config import Config
-from .commands import CommandState, CommandView, CommandSlice, CurrentCommand
+from .commands import (
+    CommandState,
+    CommandView,
+    CommandSlice,
+    CurrentCommand,
+)
+from .command_history import CommandEntry
 from .labware import LabwareState, LabwareView
 from .pipettes import PipetteState, PipetteView, HardwarePipette
 from .modules import ModuleState, ModuleView, HardwareModule
 from .module_substates import (
     MagneticModuleId,
     MagneticModuleSubState,
     HeaterShakerModuleId,
@@ -30,14 +36,15 @@
     # static engine configuration
     "Config",
     # command state and values
     "CommandState",
     "CommandView",
     "CommandSlice",
     "CurrentCommand",
+    "CommandEntry",
     # labware state and values
     "LabwareState",
     "LabwareView",
     # pipette state and values
     "PipetteState",
     "PipetteView",
     "HardwarePipette",
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/state/abstract_store.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/state/abstract_store.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/state/addressable_areas.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/state/addressable_areas.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Basic addressable area data state and store."""
 from dataclasses import dataclass
 from typing import Dict, List, Optional, Set, Union
 
 from opentrons_shared_data.robot.dev_types import RobotType
 from opentrons_shared_data.deck.dev_types import (
-    DeckDefinitionV4,
+    DeckDefinitionV5,
     SlotDefV3,
     CutoutFixture,
 )
 
 from opentrons.types import Point, DeckSlotName
 
 from ..commands import (
@@ -31,15 +31,15 @@
     DeckSlotLocation,
     AddressableAreaLocation,
     AddressableArea,
     PotentialCutoutFixture,
     DeckConfigurationType,
     Dimensions,
 )
-from ..actions import Action, UpdateCommandAction, PlayAction, AddAddressableAreaAction
+from ..actions import Action, SucceedCommandAction, PlayAction, AddAddressableAreaAction
 from .config import Config
 from .abstract_store import HasState, HandlesActions
 
 
 @dataclass
 class AddressableAreaState:
     """State of all loaded addressable area resources."""
@@ -52,15 +52,15 @@
 
     When `use_simulated_deck_config` is `True`, these are the addressable areas that have been
     referenced by the protocol so far.
     """
 
     potential_cutout_fixtures_by_cutout_id: Dict[str, Set[PotentialCutoutFixture]]
 
-    deck_definition: DeckDefinitionV4
+    deck_definition: DeckDefinitionV5
 
     deck_configuration: Optional[DeckConfigurationType]
     """The host robot's full deck configuration.
 
     If `use_simulated_deck_config` is `True`, this is meaningless and this value is undefined.
     In practice it will probably be `None` or `[]`.
 
@@ -90,15 +90,15 @@
 ]
 _FLEX_ORDERED_STAGING_SLOTS = ["D4", "C4", "B4", "A4"]
 
 
 def _get_conflicting_addressable_areas_error_string(
     potential_cutout_fixtures: Set[PotentialCutoutFixture],
     loaded_addressable_areas: Dict[str, AddressableArea],
-    deck_definition: DeckDefinitionV4,
+    deck_definition: DeckDefinitionV5,
 ) -> str:
     loaded_areas_on_cutout = set()
     for fixture in potential_cutout_fixtures:
         loaded_areas_on_cutout.update(
             deck_configuration_provider.get_provided_addressable_area_names(
                 fixture.cutout_fixture_id,
                 fixture.cutout_id,
@@ -154,15 +154,15 @@
 
     _state: AddressableAreaState
 
     def __init__(
         self,
         deck_configuration: DeckConfigurationType,
         config: Config,
-        deck_definition: DeckDefinitionV4,
+        deck_definition: DeckDefinitionV5,
     ) -> None:
         """Initialize an addressable area store and its state."""
         if config.use_simulated_deck_config:
             loaded_addressable_areas_by_name = {}
         else:
             loaded_addressable_areas_by_name = (
                 self._get_addressable_areas_from_deck_configuration(
@@ -178,15 +178,15 @@
             deck_definition=deck_definition,
             robot_type=config.robot_type,
             use_simulated_deck_config=config.use_simulated_deck_config,
         )
 
     def handle_action(self, action: Action) -> None:
         """Modify state in reaction to an action."""
-        if isinstance(action, UpdateCommandAction):
+        if isinstance(action, SucceedCommandAction):
             self._handle_command(action.command)
         elif isinstance(action, AddAddressableAreaAction):
             self._check_location_is_addressable_area(action.addressable_area)
         elif isinstance(action, PlayAction):
             current_state = self._state
             if (
                 action.deck_configuration is not None
@@ -220,19 +220,19 @@
             (MoveToAddressableAreaResult, MoveToAddressableAreaForDropTipResult),
         ):
             addressable_area_name = command.params.addressableAreaName
             self._check_location_is_addressable_area(addressable_area_name)
 
     @staticmethod
     def _get_addressable_areas_from_deck_configuration(
-        deck_config: DeckConfigurationType, deck_definition: DeckDefinitionV4
+        deck_config: DeckConfigurationType, deck_definition: DeckDefinitionV5
     ) -> Dict[str, AddressableArea]:
         """Return all addressable areas provided by the given deck configuration."""
         addressable_areas = []
-        for cutout_id, cutout_fixture_id in deck_config:
+        for cutout_id, cutout_fixture_id, opentrons_module_serial_number in deck_config:
             provided_addressable_areas = (
                 deck_configuration_provider.get_provided_addressable_area_names(
                     cutout_fixture_id, cutout_id, deck_definition
                 )
             )
             cutout_position = deck_configuration_provider.get_cutout_position(
                 cutout_id, deck_definition
@@ -347,15 +347,15 @@
         """
         if self._state.use_simulated_deck_config:
             return None
         else:
             assert self._state.deck_configuration is not None
             return [
                 cutout_fixture_id
-                for _, cutout_fixture_id in self._state.deck_configuration
+                for _, cutout_fixture_id, _serial in self._state.deck_configuration
             ]
 
     def _get_loaded_addressable_area(
         self, addressable_area_name: str
     ) -> AddressableArea:
         """Get an addressable area that has been loaded into state. Will raise error if it does not exist."""
         try:
@@ -449,19 +449,39 @@
         trashBinAdapter cutout fixture.
 
         Besides that instance, for movement purposes, this should only be called for
         areas that have been pre-validated, otherwise there could be the risk of collision.
         """
         addressable_area = self._get_addressable_area_from_deck_data(
             addressable_area_name=addressable_area_name,
-            do_compatibility_check=do_compatibility_check,
+            do_compatibility_check=False,  # This should probably not default to false
         )
         position = addressable_area.position
         return Point(x=position.x, y=position.y, z=position.z)
 
+    def get_addressable_area_offsets_from_cutout(
+        self,
+        addressable_area_name: str,
+    ) -> Point:
+        """Get the offset form cutout fixture of an addressable area."""
+        for addressable_area in self.state.deck_definition["locations"][
+            "addressableAreas"
+        ]:
+            if addressable_area["id"] == addressable_area_name:
+                area_offset = addressable_area["offsetFromCutoutFixture"]
+                position = Point(
+                    x=area_offset[0],
+                    y=area_offset[1],
+                    z=area_offset[2],
+                )
+                return Point(x=position.x, y=position.y, z=position.z)
+        raise ValueError(
+            f"No matching addressable area named {addressable_area_name} identified."
+        )
+
     def get_addressable_area_bounding_box(
         self,
         addressable_area_name: str,
         do_compatibility_check: bool = True,
     ) -> Dimensions:
         """Get the bounding box of an addressable area.
 
@@ -495,24 +515,32 @@
         bounding_box = addressable_area.bounding_box
         return Point(
             x=position.x + bounding_box.x / 2,
             y=position.y + bounding_box.y / 2,
             z=position.z,
         )
 
+    def get_cutout_id_by_deck_slot_name(self, slot_name: DeckSlotName) -> str:
+        """Get the Cutout ID of a given Deck Slot by Deck Slot Name."""
+        return DECK_SLOT_TO_CUTOUT_MAP[slot_name]
+
     def get_fixture_by_deck_slot_name(
         self, slot_name: DeckSlotName
     ) -> Optional[CutoutFixture]:
         """Get the Cutout Fixture currently loaded where a specific Deck Slot would be."""
         deck_config = self.state.deck_configuration
         if deck_config:
             slot_cutout_id = DECK_SLOT_TO_CUTOUT_MAP[slot_name]
             slot_cutout_fixture = None
             # This will only ever be one under current assumptions
-            for cutout_id, cutout_fixture_id in deck_config:
+            for (
+                cutout_id,
+                cutout_fixture_id,
+                opentrons_module_serial_number,
+            ) in deck_config:
                 if cutout_id == slot_cutout_id:
                     slot_cutout_fixture = (
                         deck_configuration_provider.get_cutout_fixture(
                             cutout_fixture_id, self.state.deck_definition
                         )
                     )
                     return slot_cutout_fixture
@@ -528,14 +556,31 @@
     def get_fixture_height(self, cutout_fixture_name: str) -> float:
         """Get the z height of a cutout fixture."""
         cutout_fixture = deck_configuration_provider.get_cutout_fixture(
             cutout_fixture_name, self._state.deck_definition
         )
         return cutout_fixture["height"]
 
+    def get_fixture_serial_from_deck_configuration_by_deck_slot(
+        self, slot_name: DeckSlotName
+    ) -> Optional[str]:
+        """Get the serial number provided by the deck configuration for a Fixture at a given location."""
+        deck_config = self.state.deck_configuration
+        if deck_config:
+            slot_cutout_id = DECK_SLOT_TO_CUTOUT_MAP[slot_name]
+            # This will only ever be one under current assumptions
+            for (
+                cutout_id,
+                cutout_fixture_id,
+                opentrons_module_serial_number,
+            ) in deck_config:
+                if cutout_id == slot_cutout_id:
+                    return opentrons_module_serial_number
+        return None
+
     def get_slot_definition(self, slot_id: str) -> SlotDefV3:
         """Get the definition of a slot in the deck.
 
         This does not require that the slot exist in deck configuration.
         """
         try:
             addressable_area = self._get_addressable_area_from_deck_data(
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/state/change_notifier.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/state/change_notifier.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/state/commands.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/state/commands.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,99 @@
 """Protocol engine commands sub-state."""
 from __future__ import annotations
-from collections import OrderedDict
-from enum import Enum
+
+import enum
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Dict, List, Optional, Union
+from typing_extensions import assert_never
 
 from opentrons_shared_data.errors import EnumeratedError, ErrorCodes, PythonException
 
 from opentrons.ordered_set import OrderedSet
 
 from opentrons.hardware_control.types import DoorState
+from opentrons.protocol_engine.actions.actions import (
+    ResumeFromRecoveryAction,
+    RunCommandAction,
+)
+from opentrons.protocol_engine.error_recovery_policy import ErrorRecoveryType
+from opentrons.protocol_engine.notes.notes import CommandNote
 
 from ..actions import (
     Action,
     QueueCommandAction,
-    UpdateCommandAction,
+    SucceedCommandAction,
     FailCommandAction,
     PlayAction,
     PauseAction,
     StopAction,
     FinishAction,
     HardwareStoppedAction,
     DoorChangeAction,
 )
 
 from ..commands import Command, CommandStatus, CommandIntent
 from ..errors import (
-    CommandDoesNotExistError,
     RunStoppedError,
     ErrorOccurrence,
     RobotDoorOpenError,
     SetupCommandNotAllowedError,
+    FixitCommandNotAllowedError,
+    ResumeFromRecoveryNotAllowedError,
     PauseNotAllowedError,
     UnexpectedProtocolError,
     ProtocolCommandFailedError,
 )
 from ..types import EngineStatus
 from .abstract_store import HasState, HandlesActions
+from .command_history import (
+    CommandEntry,
+    CommandHistory,
+)
 from .config import Config
 
 
-class QueueStatus(str, Enum):
-    """Execution status of the command queue.
+class QueueStatus(enum.Enum):
+    """Execution status of the command queue."""
+
+    SETUP = enum.auto()
+    """The engine has been created, but the run has not yet started.
 
-    Properties:
-        SETUP: The engine has been created, but the run has not yet started.
-            New protocol commands may be enqueued but will wait to execute.
-            New setup commands may be enqueued and will execute immediately.
-        RUNNING: The queue is running though protocol commands.
-            New protocol commands may be enqueued and will execute immediately.
-            New setup commands may not be enqueued.
-        PAUSED: Execution of protocol commands has been paused.
-            New protocol commands may be enqueued but wait to execute.
-            New setup commands may not be enqueued.
-    """
-
-    SETUP = "setup"
-    RUNNING = "running"
-    PAUSED = "paused"
+    New protocol commands may be enqueued, but will wait to execute.
+    New setup commands may be enqueued and will execute immediately.
+    New fixup commands may not be enqueued.
+    """
+
+    RUNNING = enum.auto()
+    """The queue is running through protocol commands.
+
+    New protocol commands may be enqueued and will execute immediately.
+    New setup commands may not be enqueued.
+    New fixup commands may not be enqueued.
+    """
 
+    PAUSED = enum.auto()
+    """Execution of protocol commands has been paused.
 
-class RunResult(str, Enum):
+    New protocol commands may be enqueued, but will wait to execute.
+    New setup commands may not be enqueued.
+    New fixup commands may not be enqueued.
+    """
+
+    AWAITING_RECOVERY = enum.auto()
+    """A protocol command has encountered a recoverable error.
+
+    New protocol commands may be enqueued, but will wait to execute.
+    New setup commands may not be enqueued.
+    New fixup commands may be enqueued and will execute immediately.
+    """
+
+
+class RunResult(str, enum.Enum):
     """Result of the run."""
 
     SUCCEEDED = "succeeded"
     FAILED = "failed"
     STOPPED = "stopped"
 
 
@@ -84,46 +112,25 @@
 
     command_id: str
     command_key: str
     created_at: datetime
     index: int
 
 
-@dataclass(frozen=True)
-class CommandEntry:
-    """An command entry in state, including its index in the list."""
-
-    command: Command
-    index: int
-
-
 @dataclass
 class CommandState:
     """State of all protocol engine command resources."""
 
-    all_command_ids: List[str]
-    """All command IDs, in insertion order."""
-
-    queued_command_ids: OrderedSet[str]
-    """The IDs of queued commands, in FIFO order"""
-
-    queued_setup_command_ids: OrderedSet[str]
-    """The IDs of queued setup commands, in FIFO order"""
-
-    running_command_id: Optional[str]
-    """The ID of the currently running command, if any"""
-
-    commands_by_id: Dict[str, CommandEntry]
-    """All command resources, in insertion order, mapped by their unique IDs."""
+    command_history: CommandHistory
 
     queue_status: QueueStatus
     """Whether the engine is currently pulling new commands off the queue to execute.
 
     A command may still be executing, and the robot may still be in motion,
-    even if INACTIVE.
+    even if PAUSED.
     """
 
     run_started_at: Optional[datetime]
     """The time the run was started.
 
     Set when the first `PlayAction` is dispatched.
     """
@@ -149,65 +156,82 @@
     """The run's fatal error occurrence, if there was one.
 
     Individual command errors, which may or may not be fatal,
     are stored on the individual commands themselves.
     """
 
     failed_command: Optional[CommandEntry]
-    """The command, if any, that made the run fail and the index in the command list."""
+    """The most recent command failure, if any."""
+    # TODO(mm, 2024-03-19): This attribute is currently only used to help robot-server
+    # with pagination, but "the failed command" is an increasingly nuanced idea, now
+    # that we're doing error recovery. See if we can implement robot-server pagination
+    # atop simpler concepts, like "the last command that ran" or "the next command that
+    # would run."
+    #
+    # TODO(mm, 2024-04-03): Can this be replaced by
+    # CommandHistory.get_terminal_command() now?
+
+    command_error_recovery_types: Dict[str, ErrorRecoveryType]
+    """For each command that failed (indexed by ID), what its recovery type was.
+
+    This only includes commands that actually failed, not the ones that we mark as
+    failed but that are effectively "cancelled" because a command before them failed.
+
+    This separate attribute is a stopgap until error recovery concepts are a bit more
+    stable. Eventually, we might want this info to be stored directly on each command.
+    """
+
+    recovery_target_command_id: Optional[str]
+    """If we're currently recovering from a command failure, which command it was."""
 
     finish_error: Optional[ErrorOccurrence]
     """The error that happened during the post-run finish steps (homing & dropping tips), if any."""
 
-    latest_command_hash: Optional[str]
-    """The latest hash value received in a QueueCommandAction.
+    latest_protocol_command_hash: Optional[str]
+    """The latest PROTOCOL command hash value received in a QueueCommandAction.
 
     This value can be used to generate future hashes.
     """
 
     stopped_by_estop: bool
     """If this is set to True, the engine was stopped by an estop event."""
 
 
 class CommandStore(HasState[CommandState], HandlesActions):
-    """Command state container."""
+    """Command state container for run-level command concerns."""
 
     _state: CommandState
 
     def __init__(
         self,
         *,
         config: Config,
         is_door_open: bool,
     ) -> None:
         """Initialize a CommandStore and its state."""
         self._config = config
         self._state = CommandState(
+            command_history=CommandHistory(),
             queue_status=QueueStatus.SETUP,
             is_door_blocking=is_door_open and config.block_on_door_open,
             run_result=None,
-            running_command_id=None,
-            all_command_ids=[],
-            queued_command_ids=OrderedSet(),
-            queued_setup_command_ids=OrderedSet(),
-            commands_by_id=OrderedDict(),
             run_error=None,
             finish_error=None,
             failed_command=None,
+            command_error_recovery_types={},
+            recovery_target_command_id=None,
             run_completed_at=None,
             run_started_at=None,
-            latest_command_hash=None,
+            latest_protocol_command_hash=None,
             stopped_by_estop=False,
         )
 
     def handle_action(self, action: Action) -> None:  # noqa: C901
         """Modify state in reaction to an action."""
         if isinstance(action, QueueCommandAction):
-            assert action.command_id not in self._state.commands_by_id
-
             # TODO(mc, 2021-06-22): mypy has trouble with this automatic
             # request > command mapping, figure out how to type precisely
             # (or wait for a future mypy version that can figure it out).
             # For now, unit tests cover mapping every request type
             queued_command = action.request._CommandCls.construct(
                 id=action.command_id,
                 key=(
@@ -215,107 +239,111 @@
                     if action.request.key is not None
                     else (action.request_hash or action.command_id)
                 ),
                 createdAt=action.created_at,
                 params=action.request.params,  # type: ignore[arg-type]
                 intent=action.request.intent,
                 status=CommandStatus.QUEUED,
+                failedCommandId=action.failed_command_id,
             )
 
-            next_index = len(self._state.all_command_ids)
-            self._state.all_command_ids.append(action.command_id)
-            self._state.commands_by_id[queued_command.id] = CommandEntry(
-                index=next_index,
-                command=queued_command,
-            )
-
-            if action.request.intent == CommandIntent.SETUP:
-                self._state.queued_setup_command_ids.add(queued_command.id)
-            else:
-                self._state.queued_command_ids.add(queued_command.id)
+            self._state.command_history.set_command_queued(queued_command)
 
             if action.request_hash is not None:
-                self._state.latest_command_hash = action.request_hash
+                self._state.latest_protocol_command_hash = action.request_hash
 
-        # TODO(mc, 2021-12-28): replace "UpdateCommandAction" with explicit
-        # state change actions (e.g. RunCommandAction, SucceedCommandAction)
-        # to make a command's queue transition logic easier to follow
-        elif isinstance(action, UpdateCommandAction):
-            command = action.command
-            prev_entry = self._state.commands_by_id.get(command.id)
-
-            if prev_entry is None:
-                index = len(self._state.all_command_ids)
-                self._state.all_command_ids.append(command.id)
-                self._state.commands_by_id[command.id] = CommandEntry(
-                    index=index,
-                    command=command,
-                )
-            else:
-                self._state.commands_by_id[command.id] = CommandEntry(
-                    index=prev_entry.index,
-                    command=command,
-                )
+        elif isinstance(action, RunCommandAction):
+            prev_entry = self._state.command_history.get(action.command_id)
+
+            running_command = prev_entry.command.copy(
+                update={
+                    "status": CommandStatus.RUNNING,
+                    "startedAt": action.started_at,
+                }
+            )
+
+            self._state.command_history.set_command_running(running_command)
 
-            self._state.queued_command_ids.discard(command.id)
-            self._state.queued_setup_command_ids.discard(command.id)
-
-            if command.status == CommandStatus.RUNNING:
-                self._state.running_command_id = command.id
-            elif self._state.running_command_id == command.id:
-                self._state.running_command_id = None
+        elif isinstance(action, SucceedCommandAction):
+            succeeded_command = action.command
+            self._state.command_history.set_command_succeeded(succeeded_command)
 
         elif isinstance(action, FailCommandAction):
             error_occurrence = ErrorOccurrence.from_failed(
                 id=action.error_id,
                 createdAt=action.failed_at,
                 error=action.error,
             )
-            prev_entry = self._state.commands_by_id[action.command_id]
-            self._state.commands_by_id[action.command_id] = CommandEntry(
-                index=prev_entry.index,
-                # TODO(mc, 2022-06-06): add new "cancelled" status or similar
-                # and don't set `completedAt` in commands other than the
-                # specific one that failed
-                command=prev_entry.command.copy(
-                    update={
-                        "error": error_occurrence,
-                        "completedAt": action.failed_at,
-                        "status": CommandStatus.FAILED,
-                    }
-                ),
+
+            self._update_to_failed(
+                command_id=action.command_id,
+                failed_at=action.failed_at,
+                error_occurrence=error_occurrence,
+                error_recovery_type=action.type,
+                notes=action.notes,
             )
 
-            self._state.failed_command = self._state.commands_by_id[action.command_id]
+            self._state.failed_command = self._state.command_history.get(
+                action.command_id
+            )
+
+            prev_entry = self.state.command_history.get(action.command_id)
             if prev_entry.command.intent == CommandIntent.SETUP:
-                other_command_ids_to_fail = [
-                    *[i for i in self._state.queued_setup_command_ids],
-                ]
-                self._state.queued_setup_command_ids.clear()
-            else:
-                other_command_ids_to_fail = [
-                    *[i for i in self._state.queued_command_ids],
-                ]
-                self._state.queued_command_ids.clear()
-
-            for command_id in other_command_ids_to_fail:
-                prev_entry = self._state.commands_by_id[command_id]
-
-                self._state.commands_by_id[command_id] = CommandEntry(
-                    index=prev_entry.index,
-                    command=prev_entry.command.copy(
-                        update={
-                            "completedAt": action.failed_at,
-                            "status": CommandStatus.FAILED,
-                        }
-                    ),
+                other_command_ids_to_fail = (
+                    self._state.command_history.get_setup_queue_ids()
                 )
-
-            if self._state.running_command_id == action.command_id:
-                self._state.running_command_id = None
+                for command_id in other_command_ids_to_fail:
+                    # TODO(mc, 2022-06-06): add new "cancelled" status or similar
+                    self._update_to_failed(
+                        command_id=command_id,
+                        failed_at=action.failed_at,
+                        error_occurrence=None,
+                        error_recovery_type=None,
+                        notes=None,
+                    )
+                self._state.command_history.clear_setup_queue()
+            elif (
+                prev_entry.command.intent == CommandIntent.PROTOCOL
+                or prev_entry.command.intent is None
+            ):
+                if action.type == ErrorRecoveryType.WAIT_FOR_RECOVERY:
+                    self._state.queue_status = QueueStatus.AWAITING_RECOVERY
+                    self._state.recovery_target_command_id = action.command_id
+                elif action.type == ErrorRecoveryType.FAIL_RUN:
+                    other_command_ids_to_fail = (
+                        self._state.command_history.get_queue_ids()
+                    )
+                    for command_id in other_command_ids_to_fail:
+                        # TODO(mc, 2022-06-06): add new "cancelled" status or similar
+                        self._update_to_failed(
+                            command_id=command_id,
+                            failed_at=action.failed_at,
+                            error_occurrence=None,
+                            error_recovery_type=None,
+                            notes=None,
+                        )
+                    self._state.command_history.clear_queue()
+                else:
+                    assert_never(action.type)
+            elif prev_entry.command.intent == CommandIntent.FIXIT:
+                other_command_ids_to_fail = (
+                    self._state.command_history.get_fixit_queue_ids()
+                )
+                for command_id in other_command_ids_to_fail:
+                    # TODO(mc, 2022-06-06): add new "cancelled" status or similar
+                    self._update_to_failed(
+                        command_id=command_id,
+                        failed_at=action.failed_at,
+                        error_occurrence=None,
+                        error_recovery_type=None,
+                        notes=None,
+                    )
+                self._state.command_history.clear_fixit_queue()
+            else:
+                assert_never(prev_entry.command.intent)
 
         elif isinstance(action, PlayAction):
             if not self._state.run_result:
                 self._state.run_started_at = (
                     self._state.run_started_at or action.requested_at
                 )
                 if self._state.is_door_blocking:
@@ -323,39 +351,49 @@
                     self._state.queue_status = QueueStatus.PAUSED
                 else:
                     self._state.queue_status = QueueStatus.RUNNING
 
         elif isinstance(action, PauseAction):
             self._state.queue_status = QueueStatus.PAUSED
 
+        elif isinstance(action, ResumeFromRecoveryAction):
+            self._state.command_history.clear_fixit_queue()
+            self._state.queue_status = QueueStatus.RUNNING
+            self._state.recovery_target_command_id = None
+
         elif isinstance(action, StopAction):
             if not self._state.run_result:
+                if self._state.queue_status == QueueStatus.AWAITING_RECOVERY:
+                    self._state.recovery_target_command_id = None
+
                 self._state.queue_status = QueueStatus.PAUSED
-                self._state.run_result = RunResult.STOPPED
                 if action.from_estop:
                     self._state.stopped_by_estop = True
+                    self._state.run_result = RunResult.FAILED
+                else:
+                    self._state.run_result = RunResult.STOPPED
 
         elif isinstance(action, FinishAction):
             if not self._state.run_result:
                 self._state.queue_status = QueueStatus.PAUSED
                 if action.set_run_status:
                     self._state.run_result = (
                         RunResult.SUCCEEDED
                         if not action.error_details
                         else RunResult.FAILED
                     )
                 else:
                     self._state.run_result = RunResult.STOPPED
 
-                if action.error_details:
-                    self._state.run_error = self._map_run_exception_to_error_occurrence(
-                        action.error_details.error_id,
-                        action.error_details.created_at,
-                        action.error_details.error,
-                    )
+            if not self._state.run_error and action.error_details:
+                self._state.run_error = self._map_run_exception_to_error_occurrence(
+                    action.error_details.error_id,
+                    action.error_details.created_at,
+                    action.error_details.error,
+                )
 
         elif isinstance(action, HardwareStoppedAction):
             self._state.queue_status = QueueStatus.PAUSED
             self._state.run_result = self._state.run_result or RunResult.STOPPED
             self._state.run_completed_at = (
                 self._state.run_completed_at or action.completed_at
             )
@@ -369,19 +407,45 @@
                     )
                 )
 
         elif isinstance(action, DoorChangeAction):
             if self._config.block_on_door_open:
                 if action.door_state == DoorState.OPEN:
                     self._state.is_door_blocking = True
+                    # todo(mm, 2024-03-19): It's unclear how the door should interact
+                    # with error recovery (QueueStatus.AWAITING_RECOVERY).
                     if self._state.queue_status != QueueStatus.SETUP:
                         self._state.queue_status = QueueStatus.PAUSED
                 elif action.door_state == DoorState.CLOSED:
                     self._state.is_door_blocking = False
 
+    def _update_to_failed(
+        self,
+        command_id: str,
+        failed_at: datetime,
+        error_occurrence: Optional[ErrorOccurrence],
+        error_recovery_type: Optional[ErrorRecoveryType],
+        notes: Optional[List[CommandNote]],
+    ) -> None:
+        prev_entry = self._state.command_history.get(command_id)
+        failed_command = prev_entry.command.copy(
+            update={
+                "completedAt": failed_at,
+                "status": CommandStatus.FAILED,
+                **({"error": error_occurrence} if error_occurrence is not None else {}),
+                # Assume we're not overwriting any existing notes because they can
+                # only be added when a command completes, and if we're failing this
+                # command, it wouldn't have completed before now.
+                **({"notes": notes} if notes is not None else {}),
+            }
+        )
+        self._state.command_history.set_command_failed(failed_command)
+        if error_recovery_type is not None:
+            self._state.command_error_recovery_types[command_id] = error_recovery_type
+
     @staticmethod
     def _map_run_exception_to_error_occurrence(
         error_id: str, created_at: datetime, exception: Exception
     ) -> ErrorOccurrence:
         """Map a fatal exception from the main part of the run to an ErrorOccurrence."""
         if (
             isinstance(exception, ProtocolCommandFailedError)
@@ -424,69 +488,65 @@
 
     def __init__(self, state: CommandState) -> None:
         """Initialize the view of command state with its underlying data."""
         self._state = state
 
     def get(self, command_id: str) -> Command:
         """Get a command by its unique identifier."""
-        try:
-            return self._state.commands_by_id[command_id].command
-        except KeyError:
-            raise CommandDoesNotExistError(f"Command {command_id} does not exist")
+        return self._state.command_history.get(command_id).command
 
     def get_all(self) -> List[Command]:
         """Get a list of all commands in state.
 
         Entries are returned in the order of first-added command to last-added command.
         Replacing a command (to change its status, for example) keeps its place in the
         ordering.
         """
-        return [
-            self._state.commands_by_id[cid].command
-            for cid in self._state.all_command_ids
-        ]
+        return self._state.command_history.get_all_commands()
 
     def get_slice(
         self,
         cursor: Optional[int],
         length: int,
     ) -> CommandSlice:
         """Get a subset of commands around a given cursor.
 
         If the cursor is omitted, a cursor will be selected automatically
-        based on the currently running or most recently executed command."
+        based on the currently running or most recently executed command.
         """
-        # TODO(mc, 2022-01-31): this is not the most performant way to implement
-        # this; if this becomes a problem, change or the underlying data structure
-        # to something that isn't just an OrderedDict
-        all_command_ids = self._state.all_command_ids
-        commands_by_id = self._state.commands_by_id
-        running_command_id = self._state.running_command_id
-        queued_command_ids = self._state.queued_command_ids
-        total_length = len(all_command_ids)
+        running_command = self._state.command_history.get_running_command()
+        queued_command_ids = self._state.command_history.get_queue_ids()
+        total_length = self._state.command_history.length()
 
         if cursor is None:
-            if running_command_id is not None:
-                cursor = commands_by_id[running_command_id].index
+            if running_command is not None:
+                cursor = running_command.index
             elif len(queued_command_ids) > 0:
-                cursor = commands_by_id[queued_command_ids.head()].index - 1
+                # Get the most recently executed command,
+                # which we can find just before the first queued command.
+                cursor = (
+                    self._state.command_history.get(queued_command_ids.head()).index - 1
+                )
             elif (
                 self._state.run_result
                 and self._state.run_result == RunResult.FAILED
                 and self._state.failed_command
             ):
+                # Currently, if the run fails, we mark all the commands we didn't
+                # reach as failed. This makes command status alone insufficient to
+                # find the most recent command that actually executed, so we need to
+                # store that separately.
                 cursor = self._state.failed_command.index
             else:
                 cursor = total_length - length
 
         # start is inclusive, stop is exclusive
         actual_cursor = max(0, min(cursor, total_length - 1))
         stop = min(total_length, actual_cursor + length)
-        command_ids = all_command_ids[actual_cursor:stop]
-        commands = [commands_by_id[cid].command for cid in command_ids]
+        commands = self._state.command_history.get_slice(start=actual_cursor, stop=stop)
 
         return CommandSlice(
             commands=commands,
             cursor=actual_cursor,
             total_length=total_length,
         )
 
@@ -512,40 +572,49 @@
                     finish_error,
                 ],
             )
             return combined_error
         else:
             return run_error or finish_error
 
+    def get_running_command_id(self) -> Optional[str]:
+        """Return the ID of the command that's currently running, if there is one."""
+        running_command = self._state.command_history.get_running_command()
+        if running_command is not None:
+            return running_command.command.id
+        else:
+            return None
+
+    def get_queue_ids(self) -> OrderedSet[str]:
+        """Get the IDs of all queued protocol commands, in FIFO order."""
+        return self._state.command_history.get_queue_ids()
+
     def get_current(self) -> Optional[CurrentCommand]:
         """Return the "current" command, if any.
 
         The "current" command is the command that is currently executing,
         or the most recent command to have completed.
         """
-        if self._state.running_command_id:
-            entry = self._state.commands_by_id[self._state.running_command_id]
+        running_command = self._state.command_history.get_running_command()
+        if running_command:
             return CurrentCommand(
-                command_id=entry.command.id,
-                command_key=entry.command.key,
-                created_at=entry.command.createdAt,
-                index=entry.index,
-            )
-
-        # TODO(mc, 2022-02-07): this is O(n) in the worst case for no good reason.
-        # Resolve prior to JSONv6 support, where this will matter.
-        for reverse_index, cid in enumerate(reversed(self._state.all_command_ids)):
-            if self.get_command_is_final(cid):
-                entry = self._state.commands_by_id[cid]
-                return CurrentCommand(
-                    command_id=entry.command.id,
-                    command_key=entry.command.key,
-                    created_at=entry.command.createdAt,
-                    index=len(self._state.all_command_ids) - reverse_index - 1,
-                )
+                command_id=running_command.command.id,
+                command_key=running_command.command.key,
+                created_at=running_command.command.createdAt,
+                index=running_command.index,
+            )
+
+        final_command = self.get_final_command()
+        if final_command:
+            return CurrentCommand(
+                command_id=final_command.command.id,
+                command_key=final_command.command.key,
+                created_at=final_command.command.createdAt,
+                index=final_command.index,
+            )
 
         return None
 
     def get_next_to_execute(self) -> Optional[str]:
         """Return the next command in line to be executed.
 
         Returns:
@@ -554,34 +623,43 @@
         Raises:
             RunStoppedError: The engine is currently stopped or stopping,
                 so it will never run any more commands.
         """
         if self._state.run_result:
             raise RunStoppedError("Engine was stopped")
 
+        # if queue is in recovery mode, return the next fixit command
+        next_fixit_cmd = self._state.command_history.get_fixit_queue_ids().head(None)
+        if next_fixit_cmd and self._state.queue_status == QueueStatus.AWAITING_RECOVERY:
+            return next_fixit_cmd
+
         # if there is a setup command queued, prioritize it
-        next_setup_cmd = self._state.queued_setup_command_ids.head(None)
-        if self._state.queue_status != QueueStatus.PAUSED and next_setup_cmd:
+        next_setup_cmd = self._state.command_history.get_setup_queue_ids().head(None)
+        if (
+            self._state.queue_status
+            not in [QueueStatus.PAUSED, QueueStatus.AWAITING_RECOVERY]
+            and next_setup_cmd
+        ):
             return next_setup_cmd
 
         # if the queue is running, return the next protocol command
         if self._state.queue_status == QueueStatus.RUNNING:
-            return self._state.queued_command_ids.head(None)
+            return self._state.command_history.get_queue_ids().head(None)
 
         # otherwise we've got nothing to do
         return None
 
     def get_is_okay_to_clear(self) -> bool:
         """Get whether the engine is stopped or sitting idly so it could be removed."""
         if self.get_is_stopped():
             return True
         elif (
             self.get_status() == EngineStatus.IDLE
-            and self._state.running_command_id is None
-            and len(self._state.queued_setup_command_ids) == 0
+            and self._state.command_history.get_running_command() is None
+            and len(self._state.command_history.get_setup_queue_ids()) == 0
         ):
             return True
         else:
             return False
 
     def get_is_door_blocking(self) -> bool:
         """Get whether the robot door is open when 'pause on door open' ff is True."""
@@ -591,14 +669,44 @@
         """Get whether the queue is implicitly active, i.e., never 'played'."""
         return self._state.queue_status == QueueStatus.SETUP
 
     def get_is_running(self) -> bool:
         """Get whether the protocol is running & queued commands should be executed."""
         return self._state.queue_status == QueueStatus.RUNNING
 
+    def get_final_command(self) -> Optional[CommandEntry]:
+        """Get the most recent command that has reached its final `status`. See get_command_is_final."""
+        run_requested_to_stop = self._state.run_result is not None
+
+        if run_requested_to_stop:
+            tail_command = self._state.command_history.get_tail_command()
+            if not tail_command:
+                return None
+            if tail_command.command.status != CommandStatus.RUNNING:
+                return tail_command
+            else:
+                return self._state.command_history.get_prev(tail_command.command.id)
+        else:
+            final_command = self._state.command_history.get_terminal_command()
+            # This iteration is effectively O(1) as we'll only ever have to iterate one or two times at most.
+            while final_command is not None:
+                next_command = self._state.command_history.get_next(
+                    final_command.command.id
+                )
+                if (
+                    next_command is not None
+                    and next_command.command.status != CommandStatus.QUEUED
+                    and next_command.command.status != CommandStatus.RUNNING
+                ):
+                    final_command = next_command
+                else:
+                    break
+
+        return final_command
+
     def get_command_is_final(self, command_id: str) -> bool:
         """Get whether a given command has reached its final `status`.
 
         This happens when one of the following is true:
 
         - Its status is `CommandStatus.SUCCEEDED`.
         - Its status is `CommandStatus.FAILED`.
@@ -606,63 +714,103 @@
           so the run will never reach it.
 
         Arguments:
             command_id: Command to check.
         """
         status = self.get(command_id).status
 
+        run_requested_to_stop = self._state.run_result is not None
+
         return (
             status == CommandStatus.SUCCEEDED
             or status == CommandStatus.FAILED
-            or (status == CommandStatus.QUEUED and self._state.run_result is not None)
+            or (status == CommandStatus.QUEUED and run_requested_to_stop)
         )
 
     def get_all_commands_final(self) -> bool:
         """Get whether all commands added so far have reached their final `status`.
 
         See `get_command_is_final()`.
 
         Raises:
             CommandExecutionFailedError: if any added command failed, and its `intent` wasn't
             `setup`.
         """
-        no_command_running = self._state.running_command_id is None
+        no_command_running = self._state.command_history.get_running_command() is None
+        run_requested_to_stop = self._state.run_result is not None
         no_command_to_execute = (
-            self._state.run_result is not None
-            or len(self._state.queued_command_ids) == 0
+            run_requested_to_stop
+            # TODO(mm, 2024-03-15): This ignores queued setup commands,
+            # which seems questionable?
+            or len(self._state.command_history.get_queue_ids()) == 0
         )
 
-        if no_command_running and no_command_to_execute:
-            for command_id in self._state.all_command_ids:
-                command = self._state.commands_by_id[command_id].command
-                if command.error and command.intent != CommandIntent.SETUP:
-                    # TODO(tz, 7-11-23): avoid raising an error and return the status instead
-                    raise ProtocolCommandFailedError(
-                        original_error=command.error, message=command.error.detail
-                    )
-            return True
-        else:
-            return False
+        return no_command_running and no_command_to_execute
+
+    def get_recovery_in_progress_for_command(self, command_id: str) -> bool:
+        """Return whether the given command failed and its error recovery is in progress."""
+        return self._state.recovery_target_command_id == command_id
+
+    def raise_fatal_command_error(self) -> None:
+        """Raise the run's fatal command error, if there was one, as an exception.
+
+        The "fatal command error" is the error from any non-setup command.
+        It's intended to be used as the fatal error of the overall run
+        (see `ProtocolEngine.finish()`) for JSON and live HTTP protocols.
+
+        This isn't useful for Python protocols, which have to account for the
+        fatal error of the overall coming from anywhere in the Python script,
+        including in between commands.
+        """
+        failed_command = self.state.failed_command
+        if (
+            failed_command
+            and failed_command.command.error
+            and failed_command.command.intent != CommandIntent.SETUP
+        ):
+            raise ProtocolCommandFailedError(
+                original_error=failed_command.command.error,
+                message=failed_command.command.error.detail,
+            )
+
+    def get_error_recovery_type(self, command_id: str) -> ErrorRecoveryType:
+        """Return the error recovery type with which the given command failed.
+
+        The command ID is assumed to point to a failed command.
+        """
+        return self.state.command_error_recovery_types[command_id]
 
     def get_is_stopped(self) -> bool:
         """Get whether an engine stop has completed."""
         return self._state.run_completed_at is not None
 
     def has_been_played(self) -> bool:
         """Get whether engine has started."""
         return self._state.run_started_at is not None
 
     def get_is_terminal(self) -> bool:
         """Get whether engine is in a terminal state."""
         return self._state.run_result is not None
 
-    def validate_action_allowed(
+    def validate_action_allowed(  # noqa: C901
         self,
-        action: Union[PlayAction, PauseAction, StopAction, QueueCommandAction],
-    ) -> Union[PlayAction, PauseAction, StopAction, QueueCommandAction]:
+        action: Union[
+            PlayAction,
+            PauseAction,
+            StopAction,
+            ResumeFromRecoveryAction,
+            QueueCommandAction,
+        ],
+    ) -> Union[
+        PlayAction,
+        PauseAction,
+        StopAction,
+        ResumeFromRecoveryAction,
+        QueueCommandAction,
+    ]:
         """Validate whether a given control action is allowed.
 
         Returns:
             The action, if valid.
 
         Raises:
             RunStoppedError: The engine has been stopped.
@@ -673,29 +821,65 @@
         """
         if self._state.run_result is not None:
             raise RunStoppedError("The run has already stopped.")
 
         elif isinstance(action, PlayAction):
             if self.get_status() == EngineStatus.BLOCKED_BY_OPEN_DOOR:
                 raise RobotDoorOpenError("Front door or top window is currently open.")
+            elif self.get_status() == EngineStatus.AWAITING_RECOVERY:
+                raise NotImplementedError()
+            else:
+                return action
 
         elif isinstance(action, PauseAction):
             if not self.get_is_running():
                 raise PauseNotAllowedError("Cannot pause a run that is not running.")
+            elif self.get_status() == EngineStatus.AWAITING_RECOVERY:
+                raise NotImplementedError()
+            else:
+                return action
 
-        elif (
-            isinstance(action, QueueCommandAction)
-            and action.request.intent == CommandIntent.SETUP
-        ):
-            if self._state.queue_status != QueueStatus.SETUP:
+        elif isinstance(action, QueueCommandAction):
+            if (
+                action.request.intent == CommandIntent.SETUP
+                and self._state.queue_status != QueueStatus.SETUP
+            ):
                 raise SetupCommandNotAllowedError(
                     "Setup commands are not allowed after run has started."
                 )
+            elif action.request.intent == CommandIntent.FIXIT:
+                if self._state.queue_status != QueueStatus.AWAITING_RECOVERY:
+                    raise FixitCommandNotAllowedError(
+                        "Fixit commands are not allowed when the run is not in a recoverable state."
+                    )
+                else:
+                    return action
+            else:
+                return action
+
+        elif isinstance(action, ResumeFromRecoveryAction):
+            if self.get_status() != EngineStatus.AWAITING_RECOVERY:
+                raise ResumeFromRecoveryNotAllowedError(
+                    "Cannot resume from recovery if the run is not in recovery mode."
+                )
+            elif (
+                self.get_status() == EngineStatus.AWAITING_RECOVERY
+                and len(self._state.command_history.get_fixit_queue_ids()) > 0
+            ):
+                raise ResumeFromRecoveryNotAllowedError(
+                    "Cannot resume from recovery while there are fixit commands in the queue."
+                )
+            else:
+                return action
 
-        return action
+        elif isinstance(action, StopAction):
+            return action
+
+        else:
+            assert_never(action)
 
     def get_status(self) -> EngineStatus:
         """Get the current execution status of the engine."""
         if self._state.run_result:
             # The main part of the run is over, or will be over soon.
             # Have we also completed the post-run finish steps (homing and dropping tips)?
             if self.get_is_stopped():
@@ -724,12 +908,17 @@
 
         elif self._state.queue_status == QueueStatus.PAUSED:
             if self._state.is_door_blocking:
                 return EngineStatus.BLOCKED_BY_OPEN_DOOR
             else:
                 return EngineStatus.PAUSED
 
+        elif self._state.queue_status == QueueStatus.AWAITING_RECOVERY:
+            return EngineStatus.AWAITING_RECOVERY
+
+        # todo(mm, 2024-03-19): Does this intentionally return idle if QueueStatus is
+        # SETUP and we're currently a setup command?
         return EngineStatus.IDLE
 
-    def get_latest_command_hash(self) -> Optional[str]:
+    def get_latest_protocol_command_hash(self) -> Optional[str]:
         """Get the command hash of the last queued command, if any."""
-        return self._state.latest_command_hash
+        return self._state.latest_protocol_command_hash
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/state/config.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/state/config.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/state/geometry.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/state/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     CurrentPipetteLocation,
     TipGeometry,
     LabwareMovementOffsetData,
     OnDeckLabwareLocation,
     AddressableAreaLocation,
     AddressableOffsetVector,
     StagingSlotLocation,
+    LabwareOffsetLocation,
 )
 from .config import Config
 from .labware import LabwareView
 from .modules import ModuleView
 from .pipettes import PipetteView
 from .addressable_areas import AddressableAreaView
 
@@ -162,14 +163,15 @@
             # get height of module + all labware on it
             module_id = slot_item.id
             try:
                 labware_id = self._labware.get_id_by_module(module_id=module_id)
             except LabwareNotLoadedOnModuleError:
                 return self._modules.get_module_highest_z(
                     module_id=module_id,
+                    addressable_areas=self._addressable_areas,
                 )
             else:
                 return self.get_highest_z_of_labware_stack(labware_id)
         elif isinstance(slot_item, LoadedLabware):
             # get stacked heights of all labware in the slot
             return self.get_highest_z_of_labware_stack(slot_item.id)
         elif type(slot_item) is dict:
@@ -242,15 +244,17 @@
           on modules as well as stacking overlaps.
           Does not include module calibration offset or LPC offset.
         """
         if isinstance(labware_location, (AddressableAreaLocation, DeckSlotLocation)):
             return LabwareOffsetVector(x=0, y=0, z=0)
         elif isinstance(labware_location, ModuleLocation):
             module_id = labware_location.moduleId
-            module_offset = self._modules.get_nominal_module_offset(module_id=module_id)
+            module_offset = self._modules.get_nominal_module_offset(
+                module_id=module_id, addressable_areas=self._addressable_areas
+            )
             module_model = self._modules.get_connected_model(module_id)
             stacking_overlap = self._labware.get_module_overlap_offsets(
                 labware_id, module_model
             )
             return LabwareOffsetVector(
                 x=module_offset.x - stacking_overlap.x,
                 y=module_offset.y - stacking_overlap.y,
@@ -1083,7 +1087,52 @@
         slot_based_offset = self._labware.get_labware_gripper_offsets(
             labware_id=labware_id, slot_name=slot_name.to_ot3_equivalent()
         )
 
         return slot_based_offset or self._labware.get_labware_gripper_offsets(
             labware_id=labware_id, slot_name=None
         )
+
+    def get_offset_location(self, labware_id: str) -> Optional[LabwareOffsetLocation]:
+        """Provide the LabwareOffsetLocation specifying the current position of the labware.
+
+        If the labware is in a location that cannot be specified by a LabwareOffsetLocation
+        (for instance, OFF_DECK) then return None.
+        """
+        parent_location = self._labware.get_location(labware_id)
+
+        if isinstance(parent_location, DeckSlotLocation):
+            return LabwareOffsetLocation(
+                slotName=parent_location.slotName, moduleModel=None, definitionUri=None
+            )
+        elif isinstance(parent_location, ModuleLocation):
+            module_model = self._modules.get_requested_model(parent_location.moduleId)
+            module_location = self._modules.get_location(parent_location.moduleId)
+            return LabwareOffsetLocation(
+                slotName=module_location.slotName,
+                moduleModel=module_model,
+                definitionUri=None,
+            )
+        elif isinstance(parent_location, OnLabwareLocation):
+            non_labware_parent_location = self._labware.get_parent_location(labware_id)
+
+            parent_uri = self._labware.get_definition_uri(parent_location.labwareId)
+            if isinstance(non_labware_parent_location, DeckSlotLocation):
+                return LabwareOffsetLocation(
+                    slotName=non_labware_parent_location.slotName,
+                    moduleModel=None,
+                    definitionUri=parent_uri,
+                )
+            elif isinstance(non_labware_parent_location, ModuleLocation):
+                module_model = self._modules.get_requested_model(
+                    non_labware_parent_location.moduleId
+                )
+                module_location = self._modules.get_location(
+                    non_labware_parent_location.moduleId
+                )
+                return LabwareOffsetLocation(
+                    slotName=module_location.slotName,
+                    moduleModel=module_model,
+                    definitionUri=parent_uri,
+                )
+
+        return None
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/state/labware.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/state/labware.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Sequence,
     Tuple,
     NamedTuple,
     cast,
     Union,
 )
 
-from opentrons_shared_data.deck.dev_types import DeckDefinitionV4
+from opentrons_shared_data.deck.dev_types import DeckDefinitionV5
 from opentrons_shared_data.gripper.constants import LABWARE_GRIP_FORCE
 from opentrons_shared_data.labware.labware_definition import LabwareRole
 from opentrons_shared_data.pipette.dev_types import LabwareUri
 
 from opentrons.types import DeckSlotName, StagingSlotName, MountType
 from opentrons.protocols.api_support.constants import OPENTRONS_NAMESPACE
 from opentrons.protocols.models import LabwareDefinition, WellDefinition
@@ -27,14 +27,15 @@
 
 from .. import errors
 from ..resources import DeckFixedLabware, labware_validation, fixture_validation
 from ..commands import (
     Command,
     LoadLabwareResult,
     MoveLabwareResult,
+    ReloadLabwareResult,
 )
 from ..types import (
     DeckSlotLocation,
     OnLabwareLocation,
     AddressableAreaLocation,
     NonStackedLocation,
     Dimensions,
@@ -48,15 +49,15 @@
     OverlapOffset,
     LabwareMovementOffsetData,
     OnDeckLabwareLocation,
     OFF_DECK_LOCATION,
 )
 from ..actions import (
     Action,
-    UpdateCommandAction,
+    SucceedCommandAction,
     AddLabwareOffsetAction,
     AddLabwareDefinitionAction,
 )
 from .abstract_store import HasState, HandlesActions
 from .move_types import EdgePathType
 
 
@@ -102,25 +103,25 @@
     labware_by_id: Dict[str, LoadedLabware]
 
     # Indexed by LabwareOffset.id.
     # We rely on Python 3.7+ preservation of dict insertion order.
     labware_offsets_by_id: Dict[str, LabwareOffset]
 
     definitions_by_uri: Dict[str, LabwareDefinition]
-    deck_definition: DeckDefinitionV4
+    deck_definition: DeckDefinitionV5
 
 
 class LabwareStore(HasState[LabwareState], HandlesActions):
     """Labware state container."""
 
     _state: LabwareState
 
     def __init__(
         self,
-        deck_definition: DeckDefinitionV4,
+        deck_definition: DeckDefinitionV5,
         deck_fixed_labware: Sequence[DeckFixedLabware],
     ) -> None:
         """Initialize a labware store and its state."""
         definitions_by_uri: Dict[str, LabwareDefinition] = {
             uri_from_details(
                 load_name=fixed_labware.definition.parameters.loadName,
                 namespace=fixed_labware.definition.namespace,
@@ -148,15 +149,15 @@
             labware_offsets_by_id={},
             labware_by_id=labware_by_id,
             deck_definition=deck_definition,
         )
 
     def handle_action(self, action: Action) -> None:
         """Modify state in reaction to an action."""
-        if isinstance(action, UpdateCommandAction):
+        if isinstance(action, SucceedCommandAction):
             self._handle_command(action.command)
 
         elif isinstance(action, AddLabwareOffsetAction):
             labware_offset = LabwareOffset.construct(
                 id=action.labware_offset_id,
                 createdAt=action.created_at,
                 definitionUri=action.request.definitionUri,
@@ -183,26 +184,35 @@
             definition_uri = uri_from_details(
                 namespace=command.result.definition.namespace,
                 load_name=command.result.definition.parameters.loadName,
                 version=command.result.definition.version,
             )
 
             self._state.definitions_by_uri[definition_uri] = command.result.definition
+            if isinstance(command.result, LoadLabwareResult):
+                location = command.params.location
+            else:
+                location = self._state.labware_by_id[command.result.labwareId].location
 
             self._state.labware_by_id[
                 command.result.labwareId
             ] = LoadedLabware.construct(
                 id=command.result.labwareId,
-                location=command.params.location,
+                location=location,
                 loadName=command.result.definition.parameters.loadName,
                 definitionUri=definition_uri,
                 offsetId=command.result.offsetId,
                 displayName=command.params.displayName,
             )
 
+        elif isinstance(command.result, ReloadLabwareResult):
+            labware_id = command.params.labwareId
+            new_offset_id = command.result.offsetId
+            self._state.labware_by_id[labware_id].offsetId = new_offset_id
+
         elif isinstance(command.result, MoveLabwareResult):
             labware_id = command.params.labwareId
             new_location = command.params.newLocation
             new_offset_id = command.result.offsetId
 
             self._state.labware_by_id[labware_id].offsetId = new_offset_id
             if isinstance(
@@ -320,15 +330,15 @@
         display name from the definition.
         """
         return (
             self.get_user_specified_display_name(labware_id)
             or self.get_definition(labware_id).metadata.displayName
         )
 
-    def get_deck_definition(self) -> DeckDefinitionV4:
+    def get_deck_definition(self) -> DeckDefinitionV5:
         """Get the current deck definition."""
         return self._state.deck_definition
 
     def get_definition_by_uri(self, uri: LabwareUri) -> LabwareDefinition:
         """Get the labware definition matching loadName namespace and version."""
         try:
             return self._state.definitions_by_uri[uri]
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/state/liquids.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/state/liquids.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/state/module_substates/__init__.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/state/module_substates/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/state/module_substates/heater_shaker_module_substate.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/state/module_substates/heater_shaker_module_substate.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/state/module_substates/magnetic_module_substate.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/state/module_substates/magnetic_module_substate.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/state/module_substates/temperature_module_substate.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/state/module_substates/temperature_module_substate.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/state/module_substates/thermocycler_module_substate.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/state/module_substates/thermocycler_module_substate.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/state/modules.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/state/modules.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,23 +42,24 @@
     ModuleDimensions,
     LabwareOffsetVector,
     HeaterShakerLatchStatus,
     HeaterShakerMovementRestrictors,
     DeckType,
     LabwareMovementOffsetData,
 )
+from .addressable_areas import AddressableAreaView
 from .. import errors
 from ..commands import (
     Command,
     LoadModuleResult,
     heater_shaker,
     temperature_module,
     thermocycler,
 )
-from ..actions import Action, UpdateCommandAction, AddModuleAction
+from ..actions import Action, SucceedCommandAction, AddModuleAction
 from .abstract_store import HasState, HandlesActions
 from .module_substates import (
     MagneticModuleSubState,
     HeaterShakerModuleSubState,
     TemperatureModuleSubState,
     ThermocyclerModuleSubState,
     MagneticModuleId,
@@ -191,34 +192,35 @@
             module_offset_by_serial=module_calibration_offsets or {},
             deck_type=config.deck_type,
         )
         self._robot_type = config.robot_type
 
     def handle_action(self, action: Action) -> None:
         """Modify state in reaction to an action."""
-        if isinstance(action, UpdateCommandAction):
+        if isinstance(action, SucceedCommandAction):
             self._handle_command(action.command)
 
         elif isinstance(action, AddModuleAction):
             self._add_module_substate(
                 module_id=action.module_id,
                 serial_number=action.serial_number,
                 definition=action.definition,
                 slot_name=None,
                 requested_model=None,
                 module_live_data=action.module_live_data,
             )
 
     def _handle_command(self, command: Command) -> None:
         if isinstance(command.result, LoadModuleResult):
+            slot_name = command.params.location.slotName
             self._add_module_substate(
                 module_id=command.result.moduleId,
                 serial_number=command.result.serialNumber,
                 definition=command.result.definition,
-                slot_name=command.params.location.slotName,
+                slot_name=slot_name,
                 requested_model=command.params.model,
                 module_live_data=None,
             )
 
         if isinstance(command.result, CalibrateModuleResult):
             self._update_module_calibration(
                 module_id=command.params.moduleId,
@@ -703,43 +705,78 @@
     def get_dimensions(self, module_id: str) -> ModuleDimensions:
         """Get the specified module's dimensions."""
         return self.get_definition(module_id).dimensions
 
     def get_nominal_module_offset(
         self,
         module_id: str,
+        addressable_areas: AddressableAreaView,
     ) -> LabwareOffsetVector:
         """Get the module's nominal offset vector computed with slot transform."""
-        definition = self.get_definition(module_id)
-        slot = self.get_location(module_id).slotName.id
+        if (
+            self.state.deck_type == DeckType.OT2_STANDARD
+            or self.state.deck_type == DeckType.OT2_SHORT_TRASH
+        ):
+            definition = self.get_definition(module_id)
+            slot = self.get_location(module_id).slotName.id
 
-        pre_transform: NDArray[npdouble] = array(
-            (
-                definition.labwareOffset.x,
-                definition.labwareOffset.y,
-                definition.labwareOffset.z,
-                1,
+            pre_transform: NDArray[npdouble] = array(
+                (
+                    definition.labwareOffset.x,
+                    definition.labwareOffset.y,
+                    definition.labwareOffset.z,
+                    1,
+                )
+            )
+            xforms_ser = definition.slotTransforms.get(
+                str(self._state.deck_type.value), {}
+            ).get(
+                slot,
+                {
+                    "labwareOffset": [
+                        [1, 0, 0, 0],
+                        [0, 1, 0, 0],
+                        [0, 0, 1, 0],
+                        [0, 0, 0, 1],
+                    ]
+                },
+            )
+            xforms_ser_offset = xforms_ser["labwareOffset"]
+
+            # Apply the slot transform, if any
+            xform: NDArray[npdouble] = array(xforms_ser_offset)
+            xformed = dot(xform, pre_transform)
+            return LabwareOffsetVector(
+                x=xformed[0],
+                y=xformed[1],
+                z=xformed[2],
+            )
+        else:
+            module = self.get(module_id)
+            if isinstance(module.location, DeckSlotLocation):
+                location = module.location.slotName
+            elif module.model == ModuleModel.THERMOCYCLER_MODULE_V2:
+                location = DeckSlotName.SLOT_B1
+            else:
+                raise ValueError(
+                    "Module location invalid for nominal module offset calculation."
+                )
+            module_addressable_area = self.ensure_and_convert_module_fixture_location(
+                location, self.state.deck_type, module.model
+            )
+            module_addressable_area_position = (
+                addressable_areas.get_addressable_area_offsets_from_cutout(
+                    module_addressable_area
+                )
+            )
+            return LabwareOffsetVector(
+                x=module_addressable_area_position.x,
+                y=module_addressable_area_position.y,
+                z=module_addressable_area_position.z,
             )
-        )
-        xforms_ser = definition.slotTransforms.get(
-            str(self._state.deck_type.value), {}
-        ).get(
-            slot,
-            {"labwareOffset": [[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]},
-        )
-        xforms_ser_offset = xforms_ser["labwareOffset"]
-
-        # Apply the slot transform, if any
-        xform: NDArray[npdouble] = array(xforms_ser_offset)
-        xformed = dot(xform, pre_transform)
-        return LabwareOffsetVector(
-            x=xformed[0],
-            y=xformed[1],
-            z=xformed[2],
-        )
 
     def get_module_calibration_offset(
         self, module_id: str
     ) -> Optional[ModuleOffsetData]:
         """Get the calibration module offset."""
         module_serial = self.get(module_id).serialNumber
         if module_serial:
@@ -751,15 +788,17 @@
         return self.get_dimensions(module_id).bareOverallHeight
 
     # TODO(mc, 2022-01-19): this method is missing unit test coverage
     def get_height_over_labware(self, module_id: str) -> float:
         """Get the height of module parts above module labware base."""
         return self.get_dimensions(module_id).overLabwareHeight
 
-    def get_module_highest_z(self, module_id: str) -> float:
+    def get_module_highest_z(
+        self, module_id: str, addressable_areas: AddressableAreaView
+    ) -> float:
         """Get the highest z point of the module, as placed on the robot.
 
         The highest Z of a module, unlike the bare overall height, depends on
         the robot it is on. We will calculate this value using the info we already have
         about the transformation of the module's placement, based on the deck it is on.
 
         This value is calculated as:
@@ -777,15 +816,15 @@
         Note: For thermocycler, the lid height is not taken into account.
         """
         module_height = self.get_overall_height(module_id)
         default_lw_offset_point = self.get_definition(module_id).labwareOffset.z
         z_difference = module_height - default_lw_offset_point
 
         nominal_transformed_lw_offset_z = self.get_nominal_module_offset(
-            module_id=module_id
+            module_id=module_id, addressable_areas=addressable_areas
         ).z
         calibration_offset = self.get_module_calibration_offset(module_id)
         return (
             nominal_transformed_lw_offset_z
             + z_difference
             + (calibration_offset.moduleOffsetVector.z if calibration_offset else 0)
         )
@@ -939,19 +978,20 @@
             if neighbor_int is None:
                 return False
             else:
                 neighbor_slot = DeckSlotName.from_primitive(neighbor_int)
 
         return neighbor_slot in self._state.slot_by_module_id.values()
 
-    def select_hardware_module_to_load(
+    def select_hardware_module_to_load(  # noqa: C901
         self,
         model: ModuleModel,
         location: DeckSlotLocation,
         attached_modules: Sequence[HardwareModule],
+        expected_serial_number: Optional[str] = None,
     ) -> HardwareModule:
         """Get the next matching hardware module for the given model and location.
 
         If a "matching" model is found already loaded in state at the requested
         location, that hardware module will be "reused" and selected. This behavior
         allows multiple load module commands to be issued while always preserving
         module hardware instance to deck slot mapping, which is required for
@@ -959,28 +999,29 @@
 
         Args:
             model: The requested module model. The selected module may have a
                 different model if the definition lists the model as compatible.
             location: The location the module will be assigned to.
             attached_modules: All attached modules as reported by the HardwareAPI,
                 in the order in which they should be used.
+            expected_serial_number: An optional variable containing the serial number
+                expected of the module identified.
 
         Raises:
             ModuleNotAttachedError: A not-yet-assigned module matching the requested
                 parameters could not be found in the attached modules list.
             ModuleAlreadyPresentError: A module of a different type is already
                 assigned to the requested location.
         """
         existing_mod_in_slot = None
 
         for mod_id, slot in self._state.slot_by_module_id.items():
             if slot == location.slotName:
                 existing_mod_in_slot = self._state.hardware_by_module_id.get(mod_id)
                 break
-
         if existing_mod_in_slot:
             existing_def = existing_mod_in_slot.definition
 
             if existing_def.model == model or model in existing_def.compatibleWith:
                 return existing_mod_in_slot
 
             else:
@@ -988,15 +1029,19 @@
                     f"A {existing_def.model.value} is already"
                     f" present in {location.slotName.value}"
                 )
 
         for m in attached_modules:
             if m not in self._state.hardware_by_module_id.values():
                 if model == m.definition.model or model in m.definition.compatibleWith:
-                    return m
+                    if expected_serial_number is not None:
+                        if m.serial_number == expected_serial_number:
+                            return m
+                    else:
+                        return m
 
         raise errors.ModuleNotAttachedError(f"No available {model.value} found.")
 
     def get_heater_shaker_movement_restrictors(
         self,
     ) -> List[HeaterShakerMovementRestrictors]:
         """Get shaking status, latch status, and location for every heater-shaker on deck."""
@@ -1059,7 +1104,96 @@
             self._state.deck_type == DeckType.OT3_STANDARD
             and maybe_module
             and maybe_module.model == ModuleModel.THERMOCYCLER_MODULE_V2
         ):
             return True
         else:
             return False
+
+    def ensure_and_convert_module_fixture_location(
+        self,
+        deck_slot: DeckSlotName,
+        deck_type: DeckType,
+        model: ModuleModel,
+    ) -> str:
+        """Ensure module fixture load location is valid.
+
+        Also, convert the deck slot to a valid module fixture addressable area.
+        """
+        if deck_type == DeckType.OT2_STANDARD or deck_type == DeckType.OT2_SHORT_TRASH:
+            raise ValueError(
+                f"Invalid Deck Type: {deck_type.name} - Does not support modules as fixtures."
+            )
+
+        if model == ModuleModel.MAGNETIC_BLOCK_V1:
+            valid_slots = [
+                slot
+                for slot in [
+                    "A1",
+                    "B1",
+                    "C1",
+                    "D1",
+                    "A2",
+                    "B2",
+                    "C2",
+                    "D2",
+                    "A3",
+                    "B3",
+                    "C3",
+                    "D3",
+                ]
+            ]
+            addressable_areas = [
+                "magneticBlockV1A1",
+                "magneticBlockV1B1",
+                "magneticBlockV1C1",
+                "magneticBlockV1D1",
+                "magneticBlockV1A2",
+                "magneticBlockV1B2",
+                "magneticBlockV1C2",
+                "magneticBlockV1D2",
+                "magneticBlockV1A3",
+                "magneticBlockV1B3",
+                "magneticBlockV1C3",
+                "magneticBlockV1D3",
+            ]
+
+        elif model == ModuleModel.HEATER_SHAKER_MODULE_V1:
+            valid_slots = [
+                slot for slot in ["A1", "B1", "C1", "D1", "A3", "B3", "C3", "D3"]
+            ]
+            addressable_areas = [
+                "heaterShakerV1A1",
+                "heaterShakerV1B1",
+                "heaterShakerV1C1",
+                "heaterShakerV1D1",
+                "heaterShakerV1A3",
+                "heaterShakerV1B3",
+                "heaterShakerV1C3",
+                "heaterShakerV1D3",
+            ]
+        elif model == ModuleModel.TEMPERATURE_MODULE_V2:
+            valid_slots = [
+                slot for slot in ["A1", "B1", "C1", "D1", "A3", "B3", "C3", "D3"]
+            ]
+            addressable_areas = [
+                "temperatureModuleV2A1",
+                "temperatureModuleV2B1",
+                "temperatureModuleV2C1",
+                "temperatureModuleV2D1",
+                "temperatureModuleV2A3",
+                "temperatureModuleV2B3",
+                "temperatureModuleV2C3",
+                "temperatureModuleV2D3",
+            ]
+        elif model == ModuleModel.THERMOCYCLER_MODULE_V2:
+            return "thermocyclerModuleV2"
+        else:
+            raise ValueError(
+                f"Unknown module {model.name} has no addressable areas to provide."
+            )
+
+        map_addressable_area = {
+            slot: addressable_area
+            for slot, addressable_area in zip(valid_slots, addressable_areas)
+        }
+        return map_addressable_area[deck_slot.value]
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/state/motion.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/state/motion.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/state/move_types.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/state/move_types.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/state/pipettes.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/state/pipettes.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 from ..commands.configuring_common import (
     PipetteConfigUpdateResultMixin,
     PipetteNozzleLayoutResultMixin,
 )
 from ..actions import (
     Action,
     SetPipetteMovementSpeedAction,
-    UpdateCommandAction,
+    SucceedCommandAction,
 )
 from .abstract_store import HasState, HandlesActions
 
 
 @dataclass(frozen=True)
 class HardwarePipette:
     """Hardware pipette data."""
@@ -107,14 +107,15 @@
         float, pipette_definition.SupportedTipsDefinition
     ]
     nominal_tip_overlap: Dict[str, float]
     home_position: float
     nozzle_offset_z: float
     pipette_bounding_box_offsets: PipetteBoundingBoxOffsets
     bounding_nozzle_offsets: BoundingNozzlesOffsets
+    default_nozzle_map: NozzleMap
 
 
 @dataclass
 class PipetteState:
     """Basic pipette data state and getter methods."""
 
     pipettes_by_id: Dict[str, LoadedPipette]
@@ -145,15 +146,15 @@
             static_config_by_id={},
             flow_rates_by_id={},
             nozzle_configuration_by_id={},
         )
 
     def handle_action(self, action: Action) -> None:
         """Modify state in reaction to an action."""
-        if isinstance(action, UpdateCommandAction):
+        if isinstance(action, SucceedCommandAction):
             self._handle_command(action.command, action.private_result)
         elif isinstance(action, SetPipetteMovementSpeedAction):
             self._state.movement_speed_by_id[action.pipette_id] = action.speed
 
     def _handle_command(  # noqa: C901
         self, command: Command, private_result: CommandPrivateResult
     ) -> None:
@@ -176,19 +177,23 @@
                 home_position=config.home_position,
                 nozzle_offset_z=config.nozzle_offset_z,
                 pipette_bounding_box_offsets=PipetteBoundingBoxOffsets(
                     back_left_corner=config.back_left_corner_offset,
                     front_right_corner=config.front_right_corner_offset,
                 ),
                 bounding_nozzle_offsets=BoundingNozzlesOffsets(
-                    back_left_offset=config.back_left_nozzle_offset,
-                    front_right_offset=config.front_right_nozzle_offset,
+                    back_left_offset=config.nozzle_map.back_left_nozzle_offset,
+                    front_right_offset=config.nozzle_map.front_right_nozzle_offset,
                 ),
+                default_nozzle_map=config.nozzle_map,
             )
             self._state.flow_rates_by_id[private_result.pipette_id] = config.flow_rates
+            self._state.nozzle_configuration_by_id[
+                private_result.pipette_id
+            ] = config.nozzle_map
         elif isinstance(private_result, PipetteNozzleLayoutResultMixin):
             self._state.nozzle_configuration_by_id[
                 private_result.pipette_id
             ] = private_result.nozzle_map
 
         if isinstance(command.result, LoadPipetteResult):
             pipette_id = command.result.pipetteId
@@ -197,15 +202,19 @@
                 id=pipette_id,
                 pipetteName=command.params.pipetteName,
                 mount=command.params.mount,
             )
             self._state.aspirated_volume_by_id[pipette_id] = None
             self._state.movement_speed_by_id[pipette_id] = None
             self._state.attached_tip_by_id[pipette_id] = None
-            self._state.nozzle_configuration_by_id[pipette_id] = None
+            static_config = self._state.static_config_by_id.get(pipette_id)
+            if static_config:
+                self._state.nozzle_configuration_by_id[
+                    pipette_id
+                ] = static_config.default_nozzle_map
 
         elif isinstance(command.result, (AspirateResult, AspirateInPlaceResult)):
             pipette_id = command.params.pipetteId
             previous_volume = self._state.aspirated_volume_by_id[pipette_id] or 0
             # PipetteHandler will have clamped command.result.volume for us, so
             # next_volume should always be in bounds.
             next_volume = previous_volume + command.result.volume
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/state/state.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/state/state.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Protocol engine state management."""
 from __future__ import annotations
 
 from dataclasses import dataclass
-from functools import partial
-from typing import Any, Callable, Dict, List, Optional, Sequence, TypeVar
+from typing import Callable, Dict, List, Optional, Sequence, TypeVar
+from typing_extensions import ParamSpec
 
-from opentrons_shared_data.deck.dev_types import DeckDefinitionV4
+from opentrons_shared_data.deck.dev_types import DeckDefinitionV5
 
 from opentrons.protocol_engine.types import ModuleOffsetData
 
 from ..resources import DeckFixedLabware
 from ..actions import Action, ActionHandler
 from .abstract_store import HasState, HandlesActions
 from .change_notifier import ChangeNotifier
@@ -26,15 +26,17 @@
 from .tips import TipState, TipView, TipStore
 from .geometry import GeometryView
 from .motion import MotionView
 from .config import Config
 from .state_summary import StateSummary
 from ..types import DeckConfigurationType
 
-ReturnT = TypeVar("ReturnT")
+
+_ParamsT = ParamSpec("_ParamsT")
+_ReturnT = TypeVar("_ReturnT")
 
 
 @dataclass(frozen=True)
 class State:
     """Underlying engine state."""
 
     commands: CommandState
@@ -136,33 +138,35 @@
     stores should be treated as immutable.
     """
 
     def __init__(
         self,
         *,
         config: Config,
-        deck_definition: DeckDefinitionV4,
+        deck_definition: DeckDefinitionV5,
         deck_fixed_labware: Sequence[DeckFixedLabware],
         is_door_open: bool,
         change_notifier: Optional[ChangeNotifier] = None,
         module_calibration_offsets: Optional[Dict[str, ModuleOffsetData]] = None,
         deck_configuration: Optional[DeckConfigurationType] = None,
+        notify_publishers: Optional[Callable[[], None]] = None,
     ) -> None:
         """Initialize a StateStore and its substores.
 
         Arguments:
             config: Top-level configuration.
             deck_definition: The deck definition to preload into
                 labware state.
             deck_fixed_labware: Labware definitions from the deck
                 definition to preload into labware state.
             is_door_open: Whether the robot's door is currently open.
             change_notifier: Internal state change notifier.
             module_calibration_offsets: Module offsets to preload.
             deck_configuration: The initial deck configuration the addressable area store will be instantiated with.
+            notify_publishers: Notifies robot server publishers of internal state change.
         """
         self._command_store = CommandStore(config=config, is_door_open=is_door_open)
         self._pipette_store = PipetteStore()
         if deck_configuration is None:
             deck_configuration = []
         self._addressable_area_store = AddressableAreaStore(
             deck_configuration=deck_configuration,
@@ -187,14 +191,15 @@
             self._labware_store,
             self._module_store,
             self._liquid_store,
             self._tip_store,
         ]
         self._config = config
         self._change_notifier = change_notifier or ChangeNotifier()
+        self._notify_robot_server = notify_publishers
         self._initialize_state()
 
     def handle_action(self, action: Action) -> None:
         """Modify State in reaction to an action.
 
         Arguments:
             action: An action object representing a state change. Will be
@@ -203,18 +208,18 @@
         for substore in self._substores:
             substore.handle_action(action)
 
         self._update_state_views()
 
     async def wait_for(
         self,
-        condition: Callable[..., Optional[ReturnT]],
-        *args: Any,
-        **kwargs: Any,
-    ) -> ReturnT:
+        condition: Callable[_ParamsT, _ReturnT],
+        *args: _ParamsT.args,
+        **kwargs: _ParamsT.kwargs,
+    ) -> _ReturnT:
         """Wait for a condition to become true, checking whenever state changes.
 
         If the condition is already true, return immediately.
 
         !!! Warning:
             This will only return when `condition` is true right now.
             If you're not careful, this can cause you to miss updates,
@@ -251,22 +256,51 @@
 
         Returns:
             The truthy value returned by the `condition` function.
 
         Raises:
             The exception raised by the `condition` function, if any.
         """
-        predicate = partial(condition, *args, **kwargs)
-        is_done = predicate()
 
-        while not is_done:
+        def predicate() -> _ReturnT:
+            return condition(*args, **kwargs)
+
+        return await self._wait_for(condition=predicate, truthiness_to_wait_for=True)
+
+    async def wait_for_not(
+        self,
+        condition: Callable[_ParamsT, _ReturnT],
+        *args: _ParamsT.args,
+        **kwargs: _ParamsT.kwargs,
+    ) -> _ReturnT:
+        """Like `wait_for()`, except wait for the condition to become false.
+
+        See the documentation in `wait_for()`, especially the warning about condition
+        design.
+
+        The advantage of having this separate method over just passing a wrapper lambda
+        as the condition to `wait_for()` yourself is that wrapper lambdas are hard to
+        test in the mock-heavy Decoy + Protocol Engine style.
+        """
+
+        def predicate() -> _ReturnT:
+            return condition(*args, **kwargs)
+
+        return await self._wait_for(condition=predicate, truthiness_to_wait_for=False)
+
+    async def _wait_for(
+        self, condition: Callable[[], _ReturnT], truthiness_to_wait_for: bool
+    ) -> _ReturnT:
+        current_value = condition()
+
+        while bool(current_value) != truthiness_to_wait_for:
             await self._change_notifier.wait()
-            is_done = predicate()
+            current_value = condition()
 
-        return is_done
+        return current_value
 
     def _get_next_state(self) -> State:
         """Get a new instance of the state value object."""
         return State(
             commands=self._command_store.state,
             addressable_areas=self._addressable_area_store.state,
             labware=self._labware_store.state,
@@ -315,7 +349,9 @@
         self._addressable_areas._state = next_state.addressable_areas
         self._labware._state = next_state.labware
         self._pipettes._state = next_state.pipettes
         self._modules._state = next_state.modules
         self._liquid._state = next_state.liquids
         self._tips._state = next_state.tips
         self._change_notifier.notify()
+        if self._notify_robot_server is not None:
+            self._notify_robot_server()
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/state/state_summary.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/state/state_summary.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_engine/types.py` & `opentrons-7.3.0a0/src/opentrons/protocol_engine/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 from dataclasses import dataclass
 from pydantic import BaseModel, Field, validator
 from typing import Optional, Union, List, Dict, Any, NamedTuple, Tuple, FrozenSet
 from typing_extensions import Literal, TypeGuard
 
 from opentrons_shared_data.pipette.dev_types import PipetteNameType
 from opentrons.types import MountType, DeckSlotName, StagingSlotName
-from opentrons.hardware_control.types import TipStateType as HwTipStateType
+from opentrons.hardware_control.types import (
+    TipStateType as HwTipStateType,
+    InstrumentProbeType,
+)
 from opentrons.hardware_control.modules import (
     ModuleType as ModuleType,
 )
 
 from opentrons_shared_data.pipette.dev_types import (  # noqa: F401
     # convenience re-export of LabwareUri type
     LabwareUri as LabwareUri,
@@ -31,14 +34,22 @@
     BLOCKED_BY_OPEN_DOOR = "blocked-by-open-door"
     STOP_REQUESTED = "stop-requested"
     STOPPED = "stopped"
     FINISHING = "finishing"
     FAILED = "failed"
     SUCCEEDED = "succeeded"
 
+    AWAITING_RECOVERY = "awaiting-recovery"
+    """The engine is waiting for external input to recover from a nonfatal error.
+
+    New fixup commands may be enqueued, which will run immediately.
+    The run can't be paused in this state, but it can be canceled, or resumed from the
+    next protocol command if recovery is complete.
+    """
+
 
 class DeckSlotLocation(BaseModel):
     """The location of something placed in a single deck slot."""
 
     slotName: DeckSlotName = Field(
         ...,
         description=(
@@ -702,14 +713,18 @@
     """The type of addressable area."""
 
     SLOT = "slot"
     STAGING_SLOT = "stagingSlot"
     MOVABLE_TRASH = "movableTrash"
     FIXED_TRASH = "fixedTrash"
     WASTE_CHUTE = "wasteChute"
+    THERMOCYCLER = "thermocycler"
+    HEATER_SHAKER = "heaterShaker"
+    TEMPERATURE = "temperatureModule"
+    MAGNETICBLOCK = "magneticBlock"
 
 
 @dataclass(frozen=True)
 class AddressableArea:
     """Addressable area that has been loaded."""
 
     area_name: str
@@ -744,15 +759,15 @@
 
     HOME_AND_STAY_ENGAGED = "homeAndStayEngaged"
     HOME_THEN_DISENGAGE = "homeThenDisengage"
     STAY_ENGAGED_IN_PLACE = "stayEngagedInPlace"
     DISENGAGE_IN_PLACE = "disengageInPlace"
 
 
-NOZZLE_NAME_REGEX = "[A-Z][0-100]"
+NOZZLE_NAME_REGEX = r"[A-Z]\d{1,2}"
 PRIMARY_NOZZLE_LITERAL = Literal["A1", "H1", "A12", "H12"]
 
 
 class AllNozzleLayoutConfiguration(BaseModel):
     """All basemodel to represent a reset to the nozzle configuration. Sending no parameters resets to default."""
 
     style: Literal["ALL"] = "ALL"
@@ -808,15 +823,34 @@
     SingleNozzleLayoutConfiguration,
     ColumnNozzleLayoutConfiguration,
     RowNozzleLayoutConfiguration,
     QuadrantNozzleLayoutConfiguration,
 ]
 
 # TODO make the below some sort of better type
-DeckConfigurationType = List[Tuple[str, str]]  # cutout_id, cutout_fixture_id
+# TODO This should instead contain a proper cutout fixture type
+DeckConfigurationType = List[
+    Tuple[str, str, Optional[str]]
+]  # cutout_id, cutout_fixture_id, opentrons_module_serial_number
+
+
+class InstrumentSensorId(str, Enum):
+    """Primary and secondary sensor ids."""
+
+    PRIMARY = "primary"
+    SECONDARY = "secondary"
+    BOTH = "both"
+
+    def to_instrument_probe_type(self) -> InstrumentProbeType:
+        """Convert to InstrumentProbeType."""
+        return {
+            InstrumentSensorId.PRIMARY: InstrumentProbeType.PRIMARY,
+            InstrumentSensorId.SECONDARY: InstrumentProbeType.SECONDARY,
+            InstrumentSensorId.BOTH: InstrumentProbeType.BOTH,
+        }[self]
 
 
 class TipPresenceStatus(str, Enum):
     """Tip presence status reported by a pipette."""
 
     PRESENT = "present"
     ABSENT = "absent"
@@ -833,7 +867,96 @@
     @classmethod
     def from_hw_state(cls, state: HwTipStateType) -> "TipPresenceStatus":
         """Convert from hardware tip state."""
         return {
             HwTipStateType.PRESENT: TipPresenceStatus.PRESENT,
             HwTipStateType.ABSENT: TipPresenceStatus.ABSENT,
         }[state]
+
+
+# TODO (spp, 2024-04-02): move all RTP types to runner
+class RTPBase(BaseModel):
+    """Parameters defined in a protocol."""
+
+    displayName: str = Field(..., description="Display string for the parameter.")
+    variableName: str = Field(..., description="Python variable name of the parameter.")
+    description: Optional[str] = Field(
+        None, description="Detailed description of the parameter."
+    )
+    suffix: Optional[str] = Field(
+        None,
+        description="Units (like mL, mm/sec, etc) or a custom suffix for the parameter.",
+    )
+
+
+class NumberParameter(RTPBase):
+    """An integer parameter defined in a protocol."""
+
+    type: Literal["int", "float"] = Field(
+        ..., description="String specifying whether the number is an int or float type."
+    )
+    min: float = Field(
+        ..., description="Minimum value that the number param is allowed to have."
+    )
+    max: float = Field(
+        ..., description="Maximum value that the number param is allowed to have."
+    )
+    value: float = Field(
+        ...,
+        description="The value assigned to the parameter; if not supplied by the client, will be assigned the default value.",
+    )
+    default: float = Field(
+        ...,
+        description="Default value of the parameter, to be used when there is no client-specified value.",
+    )
+
+
+class BooleanParameter(RTPBase):
+    """A boolean parameter defined in a protocol."""
+
+    type: Literal["bool"] = Field(
+        default="bool", description="String specifying the type of this parameter"
+    )
+    value: bool = Field(
+        ...,
+        description="The value assigned to the parameter; if not supplied by the client, will be assigned the default value.",
+    )
+    default: bool = Field(
+        ...,
+        description="Default value of the parameter, to be used when there is no client-specified value.",
+    )
+
+
+class EnumChoice(BaseModel):
+    """Components of choices used in RTP Enum Parameters."""
+
+    displayName: str = Field(..., description="Display string for the param's choice.")
+    value: Union[float, str] = Field(
+        ..., description="Enum value of the param's choice."
+    )
+
+
+class EnumParameter(RTPBase):
+    """A string enum defined in a protocol."""
+
+    type: Literal["int", "float", "str"] = Field(
+        ...,
+        description="String specifying whether the parameter is an int or float or string type.",
+    )
+    choices: List[EnumChoice] = Field(
+        ..., description="List of valid choices for this parameter."
+    )
+    value: Union[float, str] = Field(
+        ...,
+        description="The value assigned to the parameter; if not supplied by the client, will be assigned the default value.",
+    )
+    default: Union[float, str] = Field(
+        ...,
+        description="Default value of the parameter, to be used when there is no client-specified value.",
+    )
+
+
+RunTimeParameter = Union[NumberParameter, EnumParameter, BooleanParameter]
+
+RunTimeParamValuesType = Dict[
+    str, Union[float, bool, str]
+]  # update value types as more RTP types are added
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_reader/__init__.py` & `opentrons-7.3.0a0/src/opentrons/protocol_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_reader/extract_labware_definitions.py` & `opentrons-7.3.0a0/src/opentrons/protocol_reader/extract_labware_definitions.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_reader/file_format_validator.py` & `opentrons-7.3.0a0/src/opentrons/protocol_reader/file_format_validator.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_reader/file_hasher.py` & `opentrons-7.3.0a0/src/opentrons/protocol_reader/file_hasher.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_reader/file_identifier.py` & `opentrons-7.3.0a0/src/opentrons/protocol_reader/file_identifier.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_reader/file_reader_writer.py` & `opentrons-7.3.0a0/src/opentrons/protocol_reader/file_reader_writer.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_reader/protocol_reader.py` & `opentrons-7.3.0a0/src/opentrons/protocol_reader/protocol_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,18 @@
         self._file_reader_writer = file_reader_writer or FileReaderWriter()
         self._file_identifier = file_identifier or FileIdentifier()
         self._role_analyzer = role_analyzer or RoleAnalyzer()
         self._file_format_validator = file_format_validator or FileFormatValidator()
         self._file_hasher = file_hasher or FileHasher()
 
     async def save(
-        self, files: Sequence[BufferedFile], directory: Path, content_hash: str
+        self,
+        files: Sequence[BufferedFile],
+        directory: Path,
+        content_hash: str,
     ) -> ProtocolSource:
         """Compute a `ProtocolSource` from buffered files and save them as files.
 
         The input is parsed and statically analyzed to ensure it's basically
         well-formed. For example, labware definition files must conform to the labware
         definition schema.
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_reader/protocol_source.py` & `opentrons-7.3.0a0/src/opentrons/protocol_reader/protocol_source.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_reader/role_analyzer.py` & `opentrons-7.3.0a0/src/opentrons/protocol_reader/role_analyzer.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_runner/__init__.py` & `opentrons-7.3.0a0/src/opentrons/protocol_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_runner/create_simulating_runner.py` & `opentrons-7.3.0a0/src/opentrons/protocol_runner/create_simulating_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Simulating AbstractRunner factory."""
 
-from opentrons.config import feature_flags
 from opentrons.hardware_control import API as OT2API, HardwareControlAPI
 from opentrons.protocols.api_support import deck_type
 from opentrons.protocols.api_support.deck_type import should_load_fixed_trash
 from opentrons.protocol_engine import (
     Config as ProtocolEngineConfig,
     DeckType,
     create_protocol_engine,
@@ -54,15 +53,15 @@
         config=ProtocolEngineConfig(
             robot_type=robot_type,
             deck_type=DeckType(deck_type.for_simulation(robot_type)),
             ignore_pause=True,
             use_virtual_modules=True,
             use_virtual_gripper=True,
             use_simulated_deck_config=True,
-            use_virtual_pipettes=(not feature_flags.disable_fast_protocol_upload()),
+            use_virtual_pipettes=True,
         ),
         load_fixed_trash=should_load_fixed_trash(protocol_config),
     )
 
     simulating_legacy_context_creator = LegacySimulatingContextCreator(
         hardware_api=simulating_hardware_api,
         protocol_engine=protocol_engine,
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_runner/json_file_reader.py` & `opentrons-7.3.0a0/src/opentrons/protocol_runner/json_file_reader.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_runner/json_translator.py` & `opentrons-7.3.0a0/src/opentrons/protocol_runner/json_translator.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_runner/legacy_command_mapper.py` & `opentrons-7.3.0a0/src/opentrons/protocol_runner/legacy_command_mapper.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 
 from collections import defaultdict
 from datetime import datetime
 from typing import Dict, List, Optional, Tuple, Union
 
 from opentrons_shared_data.pipette.dev_types import PipetteNameType
 from opentrons.types import MountType, DeckSlotName, Location
-from opentrons.commands import types as legacy_command_types
+from opentrons.legacy_commands import types as legacy_command_types
 from opentrons.protocol_engine import (
     ProtocolEngineError,
     actions as pe_actions,
     commands as pe_commands,
     types as pe_types,
 )
+from opentrons.protocol_engine.error_recovery_policy import ErrorRecoveryType
 from opentrons.protocol_engine.resources import (
     ModelUtils,
     ModuleDataProvider,
     pipette_data_provider,
 )
 from opentrons_shared_data.labware.labware_definition import LabwareDefinition
 from opentrons_shared_data.errors import ErrorCodes, EnumeratedError, PythonException
@@ -43,15 +44,14 @@
     legacyCommandText: str
 
 
 class LegacyContextCommandError(ProtocolEngineError):
     """An error returned when a PAPIv2 ProtocolContext command fails."""
 
     def __init__(self, wrapping_exc: BaseException) -> None:
-
         if isinstance(wrapping_exc, EnumeratedError):
             super().__init__(
                 wrapping_exc.code,
                 wrapping_exc.message,
                 wrapping_exc.detail,
                 wrapping_exc.wrapping,
             )
@@ -75,14 +75,15 @@
 
 _HIGHER_ORDER_COMMAND_TYPES = {
     legacy_command_types.MIX,
     legacy_command_types.CONSOLIDATE,
     legacy_command_types.DISTRIBUTE,
     legacy_command_types.TRANSFER,
     legacy_command_types.RETURN_TIP,
+    legacy_command_types.AIR_GAP,
 }
 
 
 class LegacyCommandMapper:
     """Map broker commands to protocol engine commands.
 
     Each protocol should use its own instance of this class.
@@ -140,21 +141,34 @@
         now = ModelUtils.get_timestamp()
 
         results: List[pe_actions.Action] = []
 
         if stage == "before":
             count = self._command_count[command_type]
             command_id = f"{command_type}-{count}"
-            engine_command = self._build_initial_command(command, command_id, now)
+            command_create, running_command = self._build_initial_command(
+                command, command_id, now
+            )
 
             self._command_count[command_type] = count + 1
-            self._commands_by_broker_id[broker_id] = engine_command
+            self._commands_by_broker_id[broker_id] = running_command
 
             results.append(
-                pe_actions.UpdateCommandAction(engine_command, private_result=None)
+                pe_actions.QueueCommandAction(
+                    command_id=command_id,
+                    created_at=running_command.createdAt,
+                    request=command_create,
+                    request_hash=None,
+                )
+            )
+            assert running_command.startedAt is not None
+            results.append(
+                pe_actions.RunCommandAction(
+                    running_command.id, started_at=running_command.startedAt
+                )
             )
 
         elif stage == "after":
             running_command = self._commands_by_broker_id[broker_id]
             completed_command: pe_commands.Command
             if command_error is None:
                 if isinstance(running_command, pe_commands.PickUpTip):
@@ -163,228 +177,255 @@
                             "result": pe_commands.PickUpTipResult.construct(
                                 tipVolume=command["payload"]["location"].max_volume,  # type: ignore[typeddict-item]
                                 tipLength=command["payload"]["instrument"].hw_pipette["tip_length"],  # type: ignore[typeddict-item]
                                 position=pe_types.DeckPoint(x=0, y=0, z=0),
                             ),
                             "status": pe_commands.CommandStatus.SUCCEEDED,
                             "completedAt": now,
+                            "notes": [],
                         }
                     )
                 elif isinstance(running_command, pe_commands.DropTip):
                     completed_command = running_command.copy(
                         update={
                             "result": pe_commands.DropTipResult.construct(
                                 position=pe_types.DeckPoint(x=0, y=0, z=0)
                             ),
                             "status": pe_commands.CommandStatus.SUCCEEDED,
                             "completedAt": now,
+                            "notes": [],
                         }
                     )
                 elif isinstance(running_command, pe_commands.Aspirate):
                     completed_command = running_command.copy(
                         update={
                             # Don't .construct() result, because we want to validate
                             # volume.
                             "result": pe_commands.AspirateResult(
                                 volume=running_command.params.volume,
                                 position=pe_types.DeckPoint(x=0, y=0, z=0),
                             ),
                             "status": pe_commands.CommandStatus.SUCCEEDED,
                             "completedAt": now,
+                            "notes": [],
                         }
                     )
                 elif isinstance(running_command, pe_commands.Dispense):
                     completed_command = running_command.copy(
                         update={
                             # Don't .construct() result, because we want to validate
                             # volume.
                             "result": pe_commands.DispenseResult(
                                 volume=running_command.params.volume,
                                 position=pe_types.DeckPoint(x=0, y=0, z=0),
                             ),
                             "status": pe_commands.CommandStatus.SUCCEEDED,
                             "completedAt": now,
+                            "notes": [],
                         }
                     )
                 elif isinstance(running_command, pe_commands.BlowOut):
                     completed_command = running_command.copy(
                         update={
                             "result": pe_commands.BlowOutResult.construct(
                                 position=pe_types.DeckPoint(x=0, y=0, z=0)
                             ),
                             "status": pe_commands.CommandStatus.SUCCEEDED,
                             "completedAt": now,
+                            "notes": [],
                         }
                     )
                 elif isinstance(running_command, pe_commands.Custom):
                     completed_command = running_command.copy(
                         update={
                             "result": pe_commands.CustomResult.construct(),
                             "status": pe_commands.CommandStatus.SUCCEEDED,
                             "completedAt": now,
+                            "notes": [],
                         }
                     )
                 else:
                     completed_command = running_command.copy(
                         update={
                             "status": pe_commands.CommandStatus.SUCCEEDED,
                             "completedAt": now,
+                            "notes": [],
                         }
                     )
                 results.append(
-                    pe_actions.UpdateCommandAction(
+                    pe_actions.SucceedCommandAction(
                         completed_command, private_result=None
                     )
                 )
 
                 if isinstance(completed_command, pe_commands.WaitForResume):
                     results.append(
                         pe_actions.PauseAction(source=pe_actions.PauseSource.PROTOCOL)
                     )
 
             else:
                 results.append(
                     pe_actions.FailCommandAction(
                         command_id=running_command.id,
+                        running_command=running_command,
                         error_id=ModelUtils.generate_id(),
                         failed_at=now,
                         error=LegacyContextCommandError(command_error),
+                        notes=[],
+                        # For legacy protocols, we don't attempt to support any kind
+                        # of error recovery at the Protocol Engine level.
+                        # These protocols only run on the OT-2, which doesn't have
+                        # any recoverable errors, anyway.
+                        type=ErrorRecoveryType.FAIL_RUN,
                     )
                 )
 
         return results
 
-    def map_equipment_load(
-        self, load_info: LegacyLoadInfo
-    ) -> Tuple[pe_commands.Command, pe_commands.CommandPrivateResult]:
+    def map_equipment_load(self, load_info: LegacyLoadInfo) -> List[pe_actions.Action]:
         """Map a labware, instrument (pipette), or module load to a PE command."""
         if isinstance(load_info, LegacyLabwareLoadInfo):
-            return (self._map_labware_load(load_info), None)
+            return self._map_labware_load(load_info)
         elif isinstance(load_info, LegacyInstrumentLoadInfo):
             return self._map_instrument_load(load_info)
         elif isinstance(load_info, LegacyModuleLoadInfo):
-            return (self._map_module_load(load_info), None)
+            return self._map_module_load(load_info)
 
     def _build_initial_command(
         self,
         command: legacy_command_types.CommandMessage,
         command_id: str,
         now: datetime,
-    ) -> pe_commands.Command:
-        engine_command: pe_commands.Command
+    ) -> Tuple[pe_commands.CommandCreate, pe_commands.Command]:
         if command["name"] == legacy_command_types.PICK_UP_TIP:
-            engine_command = self._build_pick_up_tip_command(
+            return self._build_pick_up_tip(
                 command=command, command_id=command_id, now=now
             )
         elif command["name"] == legacy_command_types.DROP_TIP:
-            engine_command = self._build_drop_tip_command(
-                command=command, command_id=command_id, now=now
-            )
+            return self._build_drop_tip(command=command, command_id=command_id, now=now)
 
         elif (
             command["name"] == legacy_command_types.ASPIRATE
             or command["name"] == legacy_command_types.DISPENSE
         ):
-            engine_command = self._build_liquid_handling_command(
+            return self._build_liquid_handling(
                 command=command, command_id=command_id, now=now
             )
         elif command["name"] == legacy_command_types.BLOW_OUT:
-            engine_command = self._build_blow_out_command(
-                command=command, command_id=command_id, now=now
-            )
+            return self._build_blow_out(command=command, command_id=command_id, now=now)
         elif command["name"] == legacy_command_types.PAUSE:
-            engine_command = pe_commands.WaitForResume.construct(
+            wait_for_resume_running = pe_commands.WaitForResume.construct(
                 id=command_id,
                 key=command_id,
                 status=pe_commands.CommandStatus.RUNNING,
                 createdAt=now,
                 startedAt=now,
                 params=pe_commands.WaitForResumeParams.construct(
                     message=command["payload"]["userMessage"],
                 ),
             )
+            wait_for_resume_create: pe_commands.CommandCreate = (
+                pe_commands.WaitForResumeCreate.construct(
+                    key=wait_for_resume_running.key,
+                    params=wait_for_resume_running.params,
+                )
+            )
+            return wait_for_resume_create, wait_for_resume_running
         else:
-            engine_command = pe_commands.Custom.construct(
+            custom_running = pe_commands.Custom.construct(
                 id=command_id,
                 key=command_id,
                 status=pe_commands.CommandStatus.RUNNING,
                 createdAt=now,
                 startedAt=now,
                 params=LegacyCommandParams.construct(
                     legacyCommandType=command["name"],
                     legacyCommandText=command["payload"]["text"],
                 ),
             )
+            custom_create = pe_commands.CustomCreate.construct(
+                key=custom_running.key,
+                params=custom_running.params,
+            )
+            return custom_create, custom_running
 
-        return engine_command
-
-    def _build_drop_tip_command(
+    def _build_drop_tip(
         self,
         command: legacy_command_types.DropTipMessage,
         command_id: str,
         now: datetime,
-    ) -> pe_commands.Command:
+    ) -> Tuple[pe_commands.CommandCreate, pe_commands.Command]:
         pipette: LegacyPipetteContext = command["payload"]["instrument"]
         well = command["payload"]["location"]
         mount = MountType(pipette.mount)
         #   the following type checking suppression assumes the tiprack is not loaded on top of a module
         slot = DeckSlotName.from_primitive(well.parent.parent)  # type: ignore[arg-type]
         well_name = well.well_name
         labware_id = self._labware_id_by_slot[slot]
         pipette_id = self._pipette_id_by_mount[mount]
-        return pe_commands.DropTip.construct(
+
+        running = pe_commands.DropTip.construct(
             id=command_id,
             key=command_id,
             status=pe_commands.CommandStatus.RUNNING,
             createdAt=now,
             startedAt=now,
             params=pe_commands.DropTipParams.construct(
                 pipetteId=pipette_id,
                 labwareId=labware_id,
                 wellName=well_name,
             ),
         )
+        create = pe_commands.DropTipCreate.construct(
+            key=running.key,
+            params=running.params,
+        )
+        return create, running
 
-    def _build_pick_up_tip_command(
+    def _build_pick_up_tip(
         self,
         command: legacy_command_types.PickUpTipMessage,
         command_id: str,
         now: datetime,
-    ) -> pe_commands.Command:
+    ) -> Tuple[pe_commands.CommandCreate, pe_commands.Command]:
         pipette: LegacyPipetteContext = command["payload"]["instrument"]
         location = command["payload"]["location"]
         well = location
         mount = MountType(pipette.mount)
         #   the following type checking suppression assumes the tiprack is not loaded on top of a module
         slot = DeckSlotName.from_primitive(well.parent.parent)  # type: ignore[arg-type]
         well_name = well.well_name
         labware_id = self._labware_id_by_slot[slot]
         pipette_id = self._pipette_id_by_mount[mount]
 
-        return pe_commands.PickUpTip.construct(
+        running = pe_commands.PickUpTip.construct(
             id=command_id,
             key=command_id,
             status=pe_commands.CommandStatus.RUNNING,
             createdAt=now,
             startedAt=now,
             params=pe_commands.PickUpTipParams.construct(
                 pipetteId=pipette_id,
                 labwareId=labware_id,
                 wellName=well_name,
             ),
         )
+        create = pe_commands.PickUpTipCreate.construct(
+            key=running.key, params=running.params
+        )
+        return create, running
 
-    def _build_liquid_handling_command(
+    def _build_liquid_handling(
         self,
         command: Union[
             legacy_command_types.AspirateMessage, legacy_command_types.DispenseMessage
         ],
         command_id: str,
         now: datetime,
-    ) -> pe_commands.Command:
+    ) -> Tuple[pe_commands.CommandCreate, pe_commands.Command]:
         pipette: LegacyPipetteContext = command["payload"]["instrument"]
         location = command["payload"]["location"]
         volume = command["payload"]["volume"]
         # TODO:(jr, 15.08.2022): aspirate and dispense commands with no specified labware
         # get filtered into custom. Refactor this in followup legacy command mapping
         if location.labware.is_well:
             well = location.labware.as_well()
@@ -400,29 +441,37 @@
             pipette_id = self._pipette_id_by_mount[mount]
 
             if volume == 0:
                 # In edge cases, it's possible for a Python protocol to do dispense()
                 # or aspirate() with a volume of 0, which behaves roughly like
                 # move_to(). Protocol Engine aspirate and dispense commands must have
                 # volume > 0, so we can't map into those.
-                return pe_commands.MoveToWell.construct(
+                #
+                # TODO(mm, 2024-03-22): I don't think this has been true since
+                # https://github.com/Opentrons/opentrons/pull/14211. Can we just use
+                # aspirate and dispense commands now?
+                move_to_well_running = pe_commands.MoveToWell.construct(
                     id=command_id,
                     key=command_id,
                     status=pe_commands.CommandStatus.RUNNING,
                     createdAt=now,
                     startedAt=now,
                     params=pe_commands.MoveToWellParams.construct(
                         pipetteId=pipette_id,
                         labwareId=labware_id,
                         wellName=well_name,
                     ),
                 )
+                move_to_well_create = pe_commands.MoveToWellCreate.construct(
+                    key=move_to_well_running.key, params=move_to_well_running.params
+                )
+                return move_to_well_create, move_to_well_running
             elif command["name"] == legacy_command_types.ASPIRATE:
                 flow_rate = command["payload"]["rate"] * pipette.flow_rate.aspirate
-                return pe_commands.Aspirate.construct(
+                aspirate_running = pe_commands.Aspirate.construct(
                     id=command_id,
                     key=command_id,
                     status=pe_commands.CommandStatus.RUNNING,
                     createdAt=now,
                     startedAt=now,
                     # Don't .construct() params, because we want to validate
                     # volume and flowRate.
@@ -430,17 +479,21 @@
                         pipetteId=pipette_id,
                         labwareId=labware_id,
                         wellName=well_name,
                         volume=volume,
                         flowRate=flow_rate,
                     ),
                 )
+                aspirate_create = pe_commands.AspirateCreate.construct(
+                    key=aspirate_running.key, params=aspirate_running.params
+                )
+                return aspirate_create, aspirate_running
             else:
                 flow_rate = command["payload"]["rate"] * pipette.flow_rate.dispense
-                return pe_commands.Dispense.construct(
+                dispense_running = pe_commands.Dispense.construct(
                     id=command_id,
                     key=command_id,
                     status=pe_commands.CommandStatus.RUNNING,
                     createdAt=now,
                     startedAt=now,
                     # Don't .construct params, because we want to validate
                     # volume and flowRate.
@@ -448,33 +501,42 @@
                         pipetteId=pipette_id,
                         labwareId=labware_id,
                         wellName=well_name,
                         volume=volume,
                         flowRate=flow_rate,
                     ),
                 )
+                dispense_create = pe_commands.DispenseCreate.construct(
+                    key=dispense_running.key, params=dispense_running.params
+                )
+                return dispense_create, dispense_running
+
         else:
-            return pe_commands.Custom.construct(
+            running = pe_commands.Custom.construct(
                 id=command_id,
                 key=command_id,
                 status=pe_commands.CommandStatus.RUNNING,
                 createdAt=now,
                 startedAt=now,
                 params=LegacyCommandParams.construct(
                     legacyCommandType=command["name"],
                     legacyCommandText=command["payload"]["text"],
                 ),
             )
+            create = pe_commands.CustomCreate.construct(
+                key=running.key, params=running.params
+            )
+            return create, running
 
-    def _build_blow_out_command(
+    def _build_blow_out(
         self,
         command: legacy_command_types.BlowOutMessage,
         command_id: str,
         now: datetime,
-    ) -> pe_commands.Command:
+    ) -> Tuple[pe_commands.CommandCreate, pe_commands.Command]:
         pipette: LegacyPipetteContext = command["payload"]["instrument"]
         location = command["payload"]["location"]
         flow_rate = pipette.flow_rate.blow_out
         #   TODO:(jr, 15.08.2022): blow_out commands with no specified labware get filtered
         #   into custom. Remove location.labware.is_empty is False when refactor is complete
         if isinstance(location, Location) and location.labware.is_well:
             well = location.labware.as_well()
@@ -484,46 +546,56 @@
                 self._labware_id_by_module_id[parent_module_id]
                 if parent_module_id is not None
                 else self._labware_id_by_slot[slot]
             )
             mount = MountType(pipette.mount)
             well_name = well.well_name
             pipette_id = self._pipette_id_by_mount[mount]
-            return pe_commands.BlowOut.construct(
+
+            blow_out_running = pe_commands.BlowOut.construct(
                 id=command_id,
                 key=command_id,
                 status=pe_commands.CommandStatus.RUNNING,
                 createdAt=now,
                 startedAt=now,
                 # Don't .construct() params, because we want to validate flowRate.
                 params=pe_commands.BlowOutParams(
                     pipetteId=pipette_id,
                     labwareId=labware_id,
                     wellName=well_name,
                     flowRate=flow_rate,
                 ),
             )
+            blow_out_create = pe_commands.BlowOutCreate.construct(
+                key=blow_out_running.key, params=blow_out_running.params
+            )
+            return blow_out_create, blow_out_running
+
         #   TODO:(jr, 15.08.2022): blow_out commands with no specified labware get filtered
         #   into custom. Refactor this in followup legacy command mapping
         else:
-            return pe_commands.Custom.construct(
+            custom_running = pe_commands.Custom.construct(
                 id=command_id,
                 key=command_id,
                 status=pe_commands.CommandStatus.RUNNING,
                 createdAt=now,
                 startedAt=now,
                 params=LegacyCommandParams.construct(
                     legacyCommandType=command["name"],
                     legacyCommandText=command["payload"]["text"],
                 ),
             )
+            custom_create = pe_commands.CustomCreate.construct(
+                key=custom_running.key, params=custom_running.params
+            )
+            return custom_create, custom_running
 
     def _map_labware_load(
         self, labware_load_info: LegacyLabwareLoadInfo
-    ) -> pe_commands.Command:
+    ) -> List[pe_actions.Action]:
         """Map a legacy labware load to a ProtocolEngine command."""
         now = ModelUtils.get_timestamp()
         count = self._command_count["LOAD_LABWARE"]
         slot = labware_load_info.deck_slot
         location: pe_types.LabwareLocation
         if labware_load_info.on_module:
             location = pe_types.ModuleLocation.construct(
@@ -531,89 +603,126 @@
             )
         else:
             location = pe_types.DeckSlotLocation.construct(slotName=slot)
 
         command_id = f"commands.LOAD_LABWARE-{count}"
         labware_id = f"labware-{count}"
 
-        load_labware_command = pe_commands.LoadLabware.construct(
+        succeeded_command = pe_commands.LoadLabware.construct(
             id=command_id,
             key=command_id,
             status=pe_commands.CommandStatus.SUCCEEDED,
             createdAt=now,
             startedAt=now,
             completedAt=now,
             params=pe_commands.LoadLabwareParams.construct(
                 location=location,
                 loadName=labware_load_info.labware_load_name,
                 namespace=labware_load_info.labware_namespace,
                 version=labware_load_info.labware_version,
                 displayName=labware_load_info.labware_display_name,
             ),
+            notes=[],
             result=pe_commands.LoadLabwareResult.construct(
                 labwareId=labware_id,
                 definition=LabwareDefinition.parse_obj(
                     labware_load_info.labware_definition
                 ),
                 offsetId=labware_load_info.offset_id,
             ),
         )
+        queue_action = pe_actions.QueueCommandAction(
+            command_id=succeeded_command.id,
+            created_at=succeeded_command.createdAt,
+            request=pe_commands.LoadLabwareCreate.construct(
+                key=succeeded_command.key, params=succeeded_command.params
+            ),
+            request_hash=None,
+        )
+        run_action = pe_actions.RunCommandAction(
+            command_id=succeeded_command.id,
+            # We just set this above, so we know it's not None.
+            started_at=succeeded_command.startedAt,  # type: ignore[arg-type]
+        )
+        succeed_action = pe_actions.SucceedCommandAction(
+            command=succeeded_command,
+            private_result=None,
+        )
 
         self._command_count["LOAD_LABWARE"] = count + 1
         if isinstance(location, pe_types.DeckSlotLocation):
             self._labware_id_by_slot[location.slotName] = labware_id
         elif isinstance(location, pe_types.ModuleLocation):
             self._labware_id_by_module_id[location.moduleId] = labware_id
-        return load_labware_command
+
+        return [queue_action, run_action, succeed_action]
 
     def _map_instrument_load(
         self,
         instrument_load_info: LegacyInstrumentLoadInfo,
-    ) -> Tuple[pe_commands.Command, pe_commands.CommandPrivateResult]:
+    ) -> List[pe_actions.Action]:
         """Map a legacy instrument (pipette) load to a ProtocolEngine command.
 
         Also creates a `AddPipetteConfigAction`, which is not necessary for the run,
         but is needed for stop so tip geometry is in state for the HardwareStopper.
         """
         now = ModelUtils.get_timestamp()
         count = self._command_count["LOAD_PIPETTE"]
         command_id = f"commands.LOAD_PIPETTE-{count}"
         pipette_id = f"pipette-{count}"
         mount = MountType(str(instrument_load_info.mount).lower())
 
-        load_pipette_command = pe_commands.LoadPipette.construct(
+        succeeded_command = pe_commands.LoadPipette.construct(
             id=command_id,
             key=command_id,
             status=pe_commands.CommandStatus.SUCCEEDED,
             createdAt=now,
             startedAt=now,
             completedAt=now,
             params=pe_commands.LoadPipetteParams.construct(
                 pipetteName=PipetteNameType(instrument_load_info.instrument_load_name),
                 mount=mount,
             ),
+            notes=[],
             result=pe_commands.LoadPipetteResult.construct(pipetteId=pipette_id),
         )
         serial = instrument_load_info.pipette_dict.get("pipette_id", None) or ""
         pipette_config_result = pe_commands.LoadPipettePrivateResult(
             pipette_id=pipette_id,
             serial_number=serial,
             config=pipette_data_provider.get_pipette_static_config(
                 instrument_load_info.pipette_dict
             ),
         )
+        queue_action = pe_actions.QueueCommandAction(
+            command_id=succeeded_command.id,
+            created_at=succeeded_command.createdAt,
+            request=pe_commands.LoadPipetteCreate.construct(
+                key=succeeded_command.key, params=succeeded_command.params
+            ),
+            request_hash=None,
+        )
+        run_action = pe_actions.RunCommandAction(
+            command_id=succeeded_command.id,
+            # We just set this above, so we know it's not None.
+            started_at=succeeded_command.startedAt,  # type: ignore[arg-type]
+        )
+        succeed_action = pe_actions.SucceedCommandAction(
+            command=succeeded_command,
+            private_result=pipette_config_result,
+        )
 
         self._command_count["LOAD_PIPETTE"] = count + 1
         self._pipette_id_by_mount[mount] = pipette_id
 
-        return (load_pipette_command, pipette_config_result)
+        return [queue_action, run_action, succeed_action]
 
     def _map_module_load(
         self, module_load_info: LegacyModuleLoadInfo
-    ) -> pe_commands.Command:
+    ) -> List[pe_actions.Action]:
         """Map a legacy module load to a Protocol Engine command."""
         now = ModelUtils.get_timestamp()
 
         count = self._command_count["LOAD_MODULE"]
         command_id = f"commands.LOAD_MODULE-{count}"
         module_id = f"module-{count}"
         requested_model = _LEGACY_TO_PE_MODULE[module_load_info.requested_model]
@@ -624,32 +733,52 @@
         # during analysis+LPC (V2) and protocol execution (V1).
         # But this shouldn't result in any problems since V2 and V1 definitions
         # have similar info, with V2 having additional info fields.
         loaded_definition = self._module_definition_by_model.get(
             loaded_model
         ) or self._module_data_provider.get_definition(loaded_model)
 
-        load_module_command = pe_commands.LoadModule.construct(
+        succeeded_command = pe_commands.LoadModule.construct(
             id=command_id,
             key=command_id,
             status=pe_commands.CommandStatus.SUCCEEDED,
             createdAt=now,
             startedAt=now,
             completedAt=now,
             params=pe_commands.LoadModuleParams.construct(
                 model=requested_model,
                 location=pe_types.DeckSlotLocation(
                     slotName=module_load_info.deck_slot,
                 ),
                 moduleId=module_id,
             ),
+            notes=[],
             result=pe_commands.LoadModuleResult.construct(
                 moduleId=module_id,
                 serialNumber=module_load_info.module_serial,
                 definition=loaded_definition,
                 model=loaded_model,
             ),
         )
+        queue_action = pe_actions.QueueCommandAction(
+            command_id=succeeded_command.id,
+            created_at=succeeded_command.createdAt,
+            request=pe_commands.LoadModuleCreate.construct(
+                key=succeeded_command.key, params=succeeded_command.params
+            ),
+            request_hash=None,
+        )
+        run_action = pe_actions.RunCommandAction(
+            command_id=succeeded_command.id,
+            # We just set this above, so we know it's not None.
+            started_at=succeeded_command.startedAt,  # type: ignore[arg-type]
+        )
+        succeed_action = pe_actions.SucceedCommandAction(
+            command=succeeded_command,
+            private_result=None,
+        )
+
         self._command_count["LOAD_MODULE"] = count + 1
         self._module_id_by_slot[module_load_info.deck_slot] = module_id
         self._module_definition_by_model[loaded_model] = loaded_definition
-        return load_module_command
+
+        return [queue_action, run_action, succeed_action]
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_runner/legacy_context_plugin.py` & `opentrons-7.3.0a0/src/opentrons/protocol_runner/legacy_context_plugin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Customize the ProtocolEngine to monitor and control legacy (APIv2) protocols."""
 from __future__ import annotations
 
 from asyncio import create_task, Task
 from contextlib import ExitStack
-from typing import Optional
+from typing import List, Optional
 
-from opentrons.commands.types import CommandMessage as LegacyCommand
+from opentrons.legacy_commands.types import CommandMessage as LegacyCommand
 from opentrons.legacy_broker import LegacyBroker
 from opentrons.protocol_engine import AbstractPlugin, actions as pe_actions
 from opentrons.util.broker import ReadOnlyBroker
 
 from .legacy_wrappers import LegacyLoadInfo
 from .legacy_command_mapper import LegacyCommandMapper
 from .thread_async_queue import ThreadAsyncQueue
@@ -51,15 +51,23 @@
         #
         # The queue being non-blocking lets the protocol communicate its activity
         # instantly *even if the event loop is currently occupied by something else.*
         # Various things can accidentally occupy the event loop for too long.
         # So if the protocol had to wait for the event loop to be free
         # every time it reported some activity,
         # it could visibly stall for a moment, making its motion jittery.
-        self._actions_to_dispatch = ThreadAsyncQueue[pe_actions.Action]()
+        #
+        # TODO(mm, 2024-03-22): See if we can remove this non-blockingness now.
+        # It was one of several band-aids introduced in ~v5.0.0 to mitigate performance
+        # problems. v6.3.0 started running some Python protocols directly through
+        # Protocol Engine, without this plugin, and without any non-blocking queue.
+        # If performance is sufficient for those, that probably means the
+        # performance problems have been resolved in better ways elsewhere
+        # and we don't need this anymore.
+        self._actions_to_dispatch = ThreadAsyncQueue[List[pe_actions.Action]]()
         self._action_dispatching_task: Optional[Task[None]] = None
 
         self._subscription_exit_stack: Optional[ExitStack] = None
 
     def setup(self) -> None:
         """Set up the plugin.
 
@@ -115,30 +123,38 @@
 
     def _handle_legacy_command(self, command: LegacyCommand) -> None:
         """Handle a command reported by the APIv2 protocol.
 
         Used as a broker callback, so this will run in the APIv2 protocol's thread.
         """
         pe_actions = self._legacy_command_mapper.map_command(command=command)
-        for pe_action in pe_actions:
-            self._actions_to_dispatch.put(pe_action)
+        self._actions_to_dispatch.put(pe_actions)
 
     def _handle_equipment_loaded(self, load_info: LegacyLoadInfo) -> None:
-        (
-            pe_command,
-            pe_private_result,
-        ) = self._legacy_command_mapper.map_equipment_load(load_info=load_info)
-
-        self._actions_to_dispatch.put(
-            pe_actions.UpdateCommandAction(
-                command=pe_command, private_result=pe_private_result
-            )
-        )
+        """Handle an equipment load reported by the APIv2 protocol.
+
+        Used as a broker callback, so this will run in the APIv2 protocol's thread.
+        """
+        pe_actions = self._legacy_command_mapper.map_equipment_load(load_info=load_info)
+        self._actions_to_dispatch.put(pe_actions)
 
     async def _dispatch_all_actions(self) -> None:
         """Dispatch all actions to the `ProtocolEngine`.
 
         Exits only when `self._actions_to_dispatch` is closed
         (or an unexpected exception is raised).
         """
-        async for action in self._actions_to_dispatch.get_async_until_closed():
-            self.dispatch(action)
+        async for action_batch in self._actions_to_dispatch.get_async_until_closed():
+            # It's critical that we dispatch this batch of actions as one atomic
+            # sequence, without yielding to the event loop.
+            # Although this plugin only means to use the ProtocolEngine as a way of
+            # passively exposing the protocol's progress, the ProtocolEngine is still
+            # theoretically active, which means it's constantly watching in the
+            # background to execute any commands that it finds `queued`.
+            #
+            # For example, one of these action batches will often want to
+            # instantaneously create a running command by having a queue action
+            # immediately followed by a run action. We cannot let the
+            # ProtocolEngine's background task see the command in the `queued` state,
+            # or it will try to execute it, which the legacy protocol is already doing.
+            for action in action_batch:
+                self.dispatch(action)
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_runner/legacy_wrappers.py` & `opentrons-7.3.0a0/src/opentrons/protocol_runner/legacy_wrappers.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,23 +16,25 @@
     TemperatureModuleModel as LegacyTemperatureModuleModel,
     MagneticModuleModel as LegacyMagneticModuleModel,
     ThermocyclerModuleModel as LegacyThermocyclerModuleModel,
     HeaterShakerModuleModel as LegacyHeaterShakerModuleModel,
 )
 from opentrons.legacy_broker import LegacyBroker
 from opentrons.protocol_engine import ProtocolEngine
+from opentrons.protocol_engine.types import RunTimeParamValuesType
 from opentrons.protocol_reader import ProtocolSource, ProtocolFileRole
 from opentrons.util.broker import Broker
 
 from opentrons.protocol_api import (
     ProtocolContext as LegacyProtocolContext,
     InstrumentContext as LegacyPipetteContext,
     ModuleContext as LegacyModuleContext,
     Labware as LegacyLabware,
     Well as LegacyWell,
+    ParameterContext,
     create_protocol_context,
 )
 from opentrons.protocol_api.core.engine import ENGINE_CORE_API_VERSION
 from opentrons.protocol_api.core.legacy.load_info import (
     LoadInfo as LegacyLoadInfo,
     InstrumentLoadInfo as LegacyInstrumentLoadInfo,
     LabwareLoadInfo as LegacyLabwareLoadInfo,
@@ -164,17 +166,24 @@
     _USE_SIMULATING_CORE = True
 
 
 class LegacyExecutor:
     """Interface to execute Protocol API v2 protocols in a child thread."""
 
     @staticmethod
-    async def execute(protocol: LegacyProtocol, context: LegacyProtocolContext) -> None:
+    async def execute(
+        protocol: LegacyProtocol,
+        context: LegacyProtocolContext,
+        parameter_context: Optional[ParameterContext],
+        run_time_param_values: Optional[RunTimeParamValuesType],
+    ) -> None:
         """Execute a PAPIv2 protocol with a given ProtocolContext in a child thread."""
-        await to_thread.run_sync(run_protocol, protocol, context)
+        await to_thread.run_sync(
+            run_protocol, protocol, context, parameter_context, run_time_param_values
+        )
 
 
 __all__ = [
     # Re-exports of user-facing Python Protocol APIv2 stuff:
     # TODO(mc, 2022-08-22): remove, no longer "legacy", so re-exports unnecessary
     "LegacyProtocolContext",
     "LegacyLabware",
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_runner/protocol_runner.py` & `opentrons-7.3.0a0/src/opentrons/protocol_runner/protocol_runner.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from abc import ABC, abstractmethod
 
 import anyio
 
 from opentrons.hardware_control import HardwareControlAPI
 from opentrons import protocol_reader
 from opentrons.legacy_broker import LegacyBroker
+from opentrons.protocol_api import ParameterContext
 from opentrons.protocol_reader import (
     ProtocolSource,
     JsonProtocolConfig,
     PythonProtocolConfig,
 )
 from opentrons.protocol_engine import (
     ProtocolEngine,
@@ -31,22 +32,29 @@
     LEGACY_PYTHON_API_VERSION_CUTOFF,
     LEGACY_JSON_SCHEMA_VERSION_CUTOFF,
     LegacyFileReader,
     LegacyContextCreator,
     LegacyExecutor,
     LegacyLoadInfo,
 )
-from ..protocol_engine.types import PostRunHardwareState, DeckConfigurationType
+from ..protocol_engine.errors import ProtocolCommandFailedError
+from ..protocol_engine.types import (
+    PostRunHardwareState,
+    DeckConfigurationType,
+    RunTimeParameter,
+    RunTimeParamValuesType,
+)
 
 
 class RunResult(NamedTuple):
     """Result data from a run, pulled from the ProtocolEngine."""
 
     commands: List[Command]
     state_summary: StateSummary
+    parameters: List[RunTimeParameter]
 
 
 class AbstractRunner(ABC):
     """An interface to manage and control a protocol run.
 
     A Runner is primarily responsible for feeding a ProtocolEngine
     with commands and control signals. These commands and signals are
@@ -71,45 +79,55 @@
         """Return a broker that you can subscribe to in order to monitor protocol progress.
 
         Currently, this only returns messages for `PythonAndLegacyRunner`.
         Otherwise, it's a no-op.
         """
         return self._broker
 
+    @property
+    def run_time_parameters(self) -> List[RunTimeParameter]:
+        """Parameter definitions defined by protocol, if any. Currently only for python protocols."""
+        return []
+
     def was_started(self) -> bool:
         """Whether the run has been started.
 
         This value is latched; once it is True, it will never become False.
         """
         return self._protocol_engine.state_view.commands.has_been_played()
 
     def play(self, deck_configuration: Optional[DeckConfigurationType] = None) -> None:
         """Start or resume the run."""
         self._protocol_engine.play(deck_configuration=deck_configuration)
 
     def pause(self) -> None:
         """Pause the run."""
-        self._protocol_engine.pause()
+        self._protocol_engine.request_pause()
 
     async def stop(self) -> None:
         """Stop (cancel) the run."""
         if self.was_started():
-            await self._protocol_engine.stop()
+            await self._protocol_engine.request_stop()
         else:
             await self._protocol_engine.finish(
                 drop_tips_after_run=False,
                 set_run_status=False,
                 post_run_hardware_state=PostRunHardwareState.STAY_ENGAGED_IN_PLACE,
             )
 
+    def resume_from_recovery(self) -> None:
+        """See `ProtocolEngine.resume_from_recovery()`."""
+        self._protocol_engine.resume_from_recovery()
+
     @abstractmethod
     async def run(
         self,
         deck_configuration: DeckConfigurationType,
         protocol_source: Optional[ProtocolSource] = None,
+        run_time_param_values: Optional[RunTimeParamValuesType] = None,
     ) -> RunResult:
         """Run a given protocol to completion."""
 
 
 class PythonAndLegacyRunner(AbstractRunner):
     """Protocol runner implementation for Python protocols, and JSON protocols ≤v5."""
 
@@ -131,25 +149,34 @@
         self._legacy_context_creator = legacy_context_creator or LegacyContextCreator(
             hardware_api=hardware_api,
             protocol_engine=protocol_engine,
         )
         self._legacy_executor = legacy_executor or LegacyExecutor()
         # TODO(mc, 2022-01-11): replace task queue with specific implementations
         # of runner interface
-        self._task_queue = (
-            task_queue or TaskQueue()
-        )  # cleanup_func=protocol_engine.finish))
+        self._task_queue = task_queue or TaskQueue()
         self._task_queue.set_cleanup_func(
             func=protocol_engine.finish,
             drop_tips_after_run=drop_tips_after_run,
             post_run_hardware_state=post_run_hardware_state,
         )
+        self._parameter_context: Optional[ParameterContext] = None
+
+    @property
+    def run_time_parameters(self) -> List[RunTimeParameter]:
+        """Parameter definitions defined by protocol, if any. Will always be empty before execution."""
+        if self._parameter_context is not None:
+            return self._parameter_context.export_parameters_for_analysis()
+        return []
 
     async def load(
-        self, protocol_source: ProtocolSource, python_parse_mode: PythonParseMode
+        self,
+        protocol_source: ProtocolSource,
+        python_parse_mode: PythonParseMode,
+        run_time_param_values: Optional[RunTimeParamValuesType],
     ) -> None:
         """Load a Python or JSONv5(& older) ProtocolSource into managed ProtocolEngine."""
         labware_definitions = await protocol_reader.extract_labware_definitions(
             protocol_source=protocol_source
         )
         for definition in labware_definitions:
             # Assume adding a labware definition is fast and there are not many labware
@@ -157,14 +184,15 @@
             self._protocol_engine.add_labware_definition(definition)
 
         # fixme(mm, 2022-12-23): This does I/O and compute-bound parsing that will block
         # the event loop. Jira RSS-165.
         protocol = self._legacy_file_reader.read(
             protocol_source, labware_definitions, python_parse_mode
         )
+        self._parameter_context = ParameterContext(api_version=protocol.api_level)
         equipment_broker = None
 
         if protocol.api_level < LEGACY_PYTHON_API_VERSION_CUTOFF:
             equipment_broker = Broker[LegacyLoadInfo]()
             self._protocol_engine.add_plugin(
                 LegacyContextPlugin(
                     broker=self._broker, equipment_broker=equipment_broker
@@ -176,45 +204,57 @@
 
         context = self._legacy_context_creator.create(
             protocol=protocol,
             broker=self._broker,
             equipment_broker=equipment_broker,
         )
         initial_home_command = pe_commands.HomeCreate(
+            # this command homes all axes, including pipette plunger and gripper jaw
             params=pe_commands.HomeParams(axes=None)
         )
-        # this command homes all axes, including pipette plugner and gripper jaw
-        self._protocol_engine.add_command(request=initial_home_command)
 
-        self._task_queue.set_run_func(
-            func=self._legacy_executor.execute,
-            protocol=protocol,
-            context=context,
-        )
+        async def run_func() -> None:
+            await self._protocol_engine.add_and_execute_command(
+                request=initial_home_command
+            )
+            await self._legacy_executor.execute(
+                protocol=protocol,
+                context=context,
+                parameter_context=self._parameter_context,
+                run_time_param_values=run_time_param_values,
+            )
+
+        self._task_queue.set_run_func(run_func)
 
     async def run(  # noqa: D102
         self,
         deck_configuration: DeckConfigurationType,
         protocol_source: Optional[ProtocolSource] = None,
+        run_time_param_values: Optional[RunTimeParamValuesType] = None,
         python_parse_mode: PythonParseMode = PythonParseMode.NORMAL,
     ) -> RunResult:
         # TODO(mc, 2022-01-11): move load to runner creation, remove from `run`
-        # currently `protocol_source` arg is only used by tests
+        # currently `protocol_source` arg is only used by tests & protocol analyzer
         if protocol_source:
             await self.load(
-                protocol_source=protocol_source, python_parse_mode=python_parse_mode
+                protocol_source=protocol_source,
+                python_parse_mode=python_parse_mode,
+                run_time_param_values=run_time_param_values,
             )
 
         self.play(deck_configuration=deck_configuration)
         self._task_queue.start()
         await self._task_queue.join()
 
         run_data = self._protocol_engine.state_view.get_summary()
         commands = self._protocol_engine.state_view.commands.get_all()
-        return RunResult(commands=commands, state_summary=run_data)
+        parameters = self.run_time_parameters
+        return RunResult(
+            commands=commands, state_summary=run_data, parameters=parameters
+        )
 
 
 class JsonRunner(AbstractRunner):
     """Protocol runner implementation for json protocols."""
 
     def __init__(
         self,
@@ -240,14 +280,15 @@
         self._task_queue.set_cleanup_func(
             func=protocol_engine.finish,
             drop_tips_after_run=drop_tips_after_run,
             post_run_hardware_state=post_run_hardware_state,
         )
 
         self._hardware_api.should_taskify_movement_execution(taskify=False)
+        self._queued_commands: List[pe_commands.CommandCreate] = []
 
     async def load(self, protocol_source: ProtocolSource) -> None:
         """Load a JSONv6+ ProtocolSource into managed ProtocolEngine."""
         labware_definitions = await protocol_reader.extract_labware_definitions(
             protocol_source=protocol_source
         )
         for definition in labware_definitions:
@@ -281,43 +322,52 @@
             self._protocol_engine.add_liquid(
                 id=liquid.id,
                 name=liquid.displayName,
                 description=liquid.description,
                 color=liquid.displayColor,
             )
             await _yield()
+
         initial_home_command = pe_commands.HomeCreate(
             params=pe_commands.HomeParams(axes=None)
         )
         # this command homes all axes, including pipette plugner and gripper jaw
         self._protocol_engine.add_command(request=initial_home_command)
 
-        for command in commands:
-            self._protocol_engine.add_command(request=command)
-            await _yield()
+        self._queued_commands = commands
 
-        self._task_queue.set_run_func(func=self._protocol_engine.wait_until_complete)
+        self._task_queue.set_run_func(func=self._add_command_and_execute)
 
     async def run(  # noqa: D102
         self,
         deck_configuration: DeckConfigurationType,
         protocol_source: Optional[ProtocolSource] = None,
+        run_time_param_values: Optional[RunTimeParamValuesType] = None,
     ) -> RunResult:
         # TODO(mc, 2022-01-11): move load to runner creation, remove from `run`
         # currently `protocol_source` arg is only used by tests
         if protocol_source:
             await self.load(protocol_source)
 
         self.play(deck_configuration=deck_configuration)
         self._task_queue.start()
         await self._task_queue.join()
 
         run_data = self._protocol_engine.state_view.get_summary()
         commands = self._protocol_engine.state_view.commands.get_all()
-        return RunResult(commands=commands, state_summary=run_data)
+        return RunResult(commands=commands, state_summary=run_data, parameters=[])
+
+    async def _add_command_and_execute(self) -> None:
+        for command in self._queued_commands:
+            result = await self._protocol_engine.add_and_execute_command(command)
+            if result and result.error:
+                raise ProtocolCommandFailedError(
+                    original_error=result.error,
+                    message=f"{result.error.errorType}: {result.error.detail}",
+                )
 
 
 class LiveRunner(AbstractRunner):
     """Protocol runner implementation for live http protocols."""
 
     def __init__(
         self,
@@ -340,24 +390,25 @@
         """Set the task queue to wait until all commands are executed."""
         self._task_queue.set_run_func(func=self._protocol_engine.wait_until_complete)
 
     async def run(  # noqa: D102
         self,
         deck_configuration: DeckConfigurationType,
         protocol_source: Optional[ProtocolSource] = None,
+        run_time_param_values: Optional[RunTimeParamValuesType] = None,
     ) -> RunResult:
         assert protocol_source is None
         await self._hardware_api.home()
         self.play(deck_configuration=deck_configuration)
         self._task_queue.start()
         await self._task_queue.join()
 
         run_data = self._protocol_engine.state_view.get_summary()
         commands = self._protocol_engine.state_view.commands.get_all()
-        return RunResult(commands=commands, state_summary=run_data)
+        return RunResult(commands=commands, state_summary=run_data, parameters=[])
 
 
 AnyRunner = Union[PythonAndLegacyRunner, JsonRunner, LiveRunner]
 
 
 def create_protocol_runner(
     protocol_config: Optional[Union[JsonProtocolConfig, PythonProtocolConfig]],
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_runner/task_queue.py` & `opentrons-7.3.0a0/src/opentrons/protocol_runner/task_queue.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,76 +1,70 @@
 """Asynchronous task queue to accomplish a protocol run."""
 import asyncio
 import logging
-from functools import partial
-from typing import Any, Awaitable, Callable, Optional
-from typing_extensions import Protocol as Callback
+from typing import Any, Awaitable, Callable, Optional, ParamSpec, Concatenate
 
 log = logging.getLogger(__name__)
 
-
-class CleanupFunc(Callback):
-    """Expected cleanup function signature."""
-
-    def __call__(
-        self,
-        error: Optional[Exception],
-    ) -> Any:
-        """Cleanup, optionally taking an error thrown.
-
-        Return value will not be used.
-        """
-        ...
+CleanupFuncInput = ParamSpec("CleanupFuncInput")
+RunFuncInput = ParamSpec("RunFuncInput")
 
 
 class TaskQueue:
     """A queue of async tasks to run.
 
     Once started, a TaskQueue may not be re-used.
     """
 
     def __init__(
         self,
         # cleanup_func: CleanupFunc,
     ) -> None:
-        """Initialize the TaskQueue.
-
-        Args:
-            cleanup_func: A function to call at run function completion
-                with any error raised by the run function.
-        """
+        """Initialize the TaskQueue."""
         self._cleanup_func: Optional[
-            Callable[[Optional[Exception]], Any]
-        ] = None  # CleanupFunc = cleanup_func
+            Callable[[Optional[Exception]], Awaitable[Any]]
+        ] = None
 
         self._run_func: Optional[Callable[[], Any]] = None
         self._run_task: Optional["asyncio.Task[None]"] = None
         self._ok_to_join_event: asyncio.Event = asyncio.Event()
 
     def set_cleanup_func(
         self,
-        func: Callable[..., Awaitable[Any]],
-        **kwargs: Any,
+        func: Callable[
+            Concatenate[Optional[Exception], CleanupFuncInput], Awaitable[Any]
+        ],
+        *args: CleanupFuncInput.args,
+        **kwargs: CleanupFuncInput.kwargs,
     ) -> None:
         """Add the protocol cleanup task to the queue.
 
         The "cleanup" task will be run after the "run" task.
         """
-        self._cleanup_func = partial(func, **kwargs)
+
+        async def _do_cleanup(error: Optional[Exception]) -> None:
+            await func(error, *args, **kwargs)
+
+        self._cleanup_func = _do_cleanup
 
     def set_run_func(
         self,
-        func: Callable[..., Awaitable[Any]],
-        **kwargs: Any,
+        func: Callable[RunFuncInput, Awaitable[Any]],
+        *args: RunFuncInput.args,
+        **kwargs: RunFuncInput.kwargs,
     ) -> None:
         """Add the protocol run task to the queue.
 
         The "run" task will be run first, before the "cleanup" task.
         """
-        self._run_func = partial(func, **kwargs)
+
+        async def _do_run() -> None:
+            await func(*args, **kwargs)
+
+        self._run_func = _do_run
 
     def start(self) -> None:
         """Start running tasks in the queue."""
         self._ok_to_join_event.set()
 
         if self._run_task is None:
             self._run_task = asyncio.create_task(self._run())
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocol_runner/thread_async_queue.py` & `opentrons-7.3.0a0/src/opentrons/protocol_runner/thread_async_queue.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/advanced_control/mix.py` & `opentrons-7.3.0a0/src/opentrons/protocols/advanced_control/mix.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/advanced_control/transfers.py` & `opentrons-7.3.0a0/src/opentrons/protocols/advanced_control/transfers.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/api_support/deck_type.py` & `opentrons-7.3.0a0/src/opentrons/protocols/api_support/deck_type.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/api_support/definitions.py` & `opentrons-7.3.0a0/src/opentrons/protocols/api_support/definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .types import APIVersion
 
-MAX_SUPPORTED_VERSION = APIVersion(2, 17)
+MAX_SUPPORTED_VERSION = APIVersion(2, 18)
 """The maximum supported protocol API version in this release."""
 
 MIN_SUPPORTED_VERSION = APIVersion(2, 0)
 """The minimum supported protocol API version in this release, across all robot types."""
 
 MIN_SUPPORTED_VERSION_FOR_FLEX = APIVersion(2, 15)
 """The minimum protocol API version supported by the Opentrons Flex.
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/api_support/instrument.py` & `opentrons-7.3.0a0/src/opentrons/protocols/api_support/instrument.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,34 +69,41 @@
             pipette["tip_overlap"]["default"],
         )
         tip_length = tip_rack_definition["parameters"]["tipLength"]
         return tip_length - tip_overlap
 
 
 VALID_PIP_TIPRACK_VOL = {
-    "p10": [10, 20],
-    "p20": [10, 20],
-    "p50": [50, 200, 300],
-    "p300": [200, 300],
-    "p1000": [1000],
+    "FLEX": {"p50": [50], "p1000": [50, 200, 1000]},
+    "OT2": {
+        "p10": [10, 20],
+        "p20": [10, 20],
+        "p50": [50, 200, 300],
+        "p300": [200, 300],
+        "p1000": [1000],
+    },
 }
 
 
 def validate_tiprack(
     instrument_name: str, tip_rack: Labware, log: logging.Logger
 ) -> None:
     """Validate a tiprack logging a warning message."""
     if not tip_rack.is_tiprack:
         raise ValueError(f"Labware {tip_rack.load_name} is not a tip rack.")
 
     # TODO AA 2020-06-24 - we should instead add the acceptable Opentrons
     #  tipracks to the pipette as a refactor
     if tip_rack.uri.startswith("opentrons/"):
         tiprack_vol = tip_rack.wells()[0].max_volume
-        valid_vols = VALID_PIP_TIPRACK_VOL[instrument_name.split("_")[0]]
+        instr_metadata = instrument_name.split("_")
+        gen_lookup = (
+            "FLEX" if ("flex" in instr_metadata or "96" in instr_metadata) else "OT2"
+        )
+        valid_vols = VALID_PIP_TIPRACK_VOL[gen_lookup][instrument_name.split("_")[0]]
         if tiprack_vol not in valid_vols:
             log.warning(
                 f"The pipette {instrument_name} and its tip rack {tip_rack.load_name}"
                 " appear to be mismatched. Please check your protocol."
             )
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/api_support/labware_like.py` & `opentrons-7.3.0a0/src/opentrons/protocols/api_support/labware_like.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/api_support/tip_tracker.py` & `opentrons-7.3.0a0/src/opentrons/protocols/api_support/tip_tracker.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/api_support/util.py` & `opentrons-7.3.0a0/src/opentrons/protocols/api_support/util.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/bundle.py` & `opentrons-7.3.0a0/src/opentrons/protocols/bundle.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/duration/estimator.py` & `opentrons-7.3.0a0/src/opentrons/protocols/duration/estimator.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing_extensions import Final
 
 import math
 import functools
 
 from dataclasses import dataclass
 
-from opentrons.commands import types
+from opentrons.legacy_commands import types
 from opentrons.protocols.api_support.deck_type import (
     guess_from_global_config as guess_deck_type_from_global_config,
 )
 from opentrons.protocols.api_support.labware_like import LabwareLike
 from opentrons.protocols.duration.errors import DurationEstimatorException
 from opentrons.protocol_api.core.legacy.deck import Deck
 from opentrons.types import Location
```

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/execution/dev_types.py` & `opentrons-7.3.0a0/src/opentrons/protocols/execution/dev_types.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/execution/errors.py` & `opentrons-7.3.0a0/src/opentrons/protocols/execution/errors.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/execution/execute_json_v3.py` & `opentrons-7.3.0a0/src/opentrons/protocols/execution/execute_json_v3.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/execution/execute_json_v4.py` & `opentrons-7.3.0a0/src/opentrons/protocols/execution/execute_json_v4.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/execution/execute_json_v5.py` & `opentrons-7.3.0a0/src/opentrons/protocols/execution/execute_json_v5.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/execution/json_dispatchers.py` & `opentrons-7.3.0a0/src/opentrons/protocols/execution/json_dispatchers.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/geometry/labware_geometry.py` & `opentrons-7.3.0a0/src/opentrons/protocols/geometry/labware_geometry.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/geometry/planning.py` & `opentrons-7.3.0a0/src/opentrons/protocols/geometry/planning.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/labware.py` & `opentrons-7.3.0a0/src/opentrons/protocols/labware.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/models/__init__.py` & `opentrons-7.3.0a0/src/opentrons/protocols/models/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/models/json_protocol.py` & `opentrons-7.3.0a0/src/opentrons/protocols/models/json_protocol.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/parse.py` & `opentrons-7.3.0a0/src/opentrons/protocols/parse.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/protocols/types.py` & `opentrons-7.3.0a0/src/opentrons/protocols/types.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/resources/scripts/lpc21isp` & `opentrons-7.3.0a0/src/opentrons/resources/scripts/lpc21isp`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/resources/smoothie-edge-8414642.hex` & `opentrons-7.3.0a0/src/opentrons/resources/smoothie-edge-8414642.hex`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/simulate.py` & `opentrons-7.3.0a0/src/opentrons/simulate.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 from opentrons.protocol_reader.protocol_source import ProtocolSource
 from opentrons.protocol_runner.protocol_runner import create_protocol_runner
 from opentrons.protocols.duration import DurationEstimator
 from opentrons.protocols.execution import execute
 from opentrons.legacy_broker import LegacyBroker
 from opentrons.config import IS_ROBOT
 from opentrons import protocol_api
-from opentrons.commands import types as command_types
+from opentrons.legacy_commands import types as command_types
 
 from opentrons.protocols import parse, bundle
 from opentrons.protocols.types import (
     ApiDeprecationError,
     Protocol,
     PythonProtocol,
     BundleContents,
@@ -110,15 +110,15 @@
 """The user-facing robot type specifier.
 
 This should match what `opentrons.protocols.parse()` accepts in a protocol's `requirements` dict.
 """
 
 
 # TODO(mm, 2023-10-05): Type _SimulateResultRunLog more precisely by using TypedDicts from
-# opentrons.commands.
+# opentrons.legacy_commands.
 _SimulateResultRunLog = List[Mapping[str, Any]]
 _SimulateResult = Tuple[_SimulateResultRunLog, Optional[BundleContents]]
 
 
 class _AccumulatingHandler(logging.Handler):
     def __init__(
         self,
@@ -219,14 +219,15 @@
     bundled_data: Optional[Dict[str, bytes]] = None,
     extra_labware: Optional[Dict[str, "LabwareDefinitionDict"]] = None,
     hardware_simulator: Optional[ThreadManagedHardware] = None,
     # Additional arguments are kw-only to make mistakes harder in environments without
     # type checking, like Jupyter Notebook.
     *,
     robot_type: Optional[_UserSpecifiedRobotType] = None,
+    use_virtual_hardware: bool = True,
 ) -> protocol_api.ProtocolContext:
     """
     Build and return a ``protocol_api.ProtocolContext``
     connected to Virtual Smoothie.
 
     This can be used to run protocols from interactive Python sessions
     such as Jupyter or an interpreter on the command line:
@@ -256,14 +257,15 @@
                           If this is ``None`` (the default), and this function is called on a robot,
                           it will look for labware in the ``labware`` subdirectory of the Jupyter
                           data directory.
     :param hardware_simulator: If specified, a hardware simulator instance.
     :param robot_type: The type of robot to simulate: either ``"Flex"`` or ``"OT-2"``.
                        If you're running this function on a robot, the default is the type of that
                        robot. Otherwise, the default is ``"OT-2"``, for backwards compatibility.
+    :param use_virtual_hardware: If true, use the protocol engines virtual hardware, if false use the lower level hardware simulator.
     :return: The protocol context.
     """
     if isinstance(version, str):
         checked_version = parse.version_from_string(version)
     elif not isinstance(version, APIVersion):
         raise TypeError("version must be either a string or an APIVersion")
     else:
@@ -313,14 +315,15 @@
         context = _create_live_context_pe(
             api_version=checked_version,
             robot_type=parsed_robot_type,
             deck_type=deck_type,
             hardware_api=checked_hardware,
             bundled_data=bundled_data,
             extra_labware=extra_labware,
+            use_virtual_hardware=use_virtual_hardware,
         )
 
     # Intentional difference from execute.get_protocol_api():
     # For the caller's convenience, we home the virtual hardware so they don't get MustHomeErrors.
     # Since this hardware is virtual, there's no harm in commanding this "movement" implicitly.
     context.home()
 
@@ -449,15 +452,15 @@
     Each dict element in the run log has the following keys:
 
         - ``level``: The depth at which this command is nested. If this an
           aspirate inside a mix inside a transfer, for instance, it would be 3.
 
         - ``payload``: The command. The human-readable run log text is available at
           ``payload["text"]``. The other keys of ``payload`` are command-dependent;
-          see ``opentrons.commands``.
+          see ``opentrons.legacy_commands``.
 
           .. note::
             In older software versions, ``payload["text"]`` was a
             `format string <https://docs.python.org/3/library/string.html#formatstrings>`_.
             To get human-readable text, you had to do ``payload["text"].format(**payload)``.
             Don't do that anymore. If ``payload["text"]`` happens to contain any
             ``{`` or ``}`` characters, it can confuse ``.format()`` and cause it to raise a
@@ -786,23 +789,26 @@
 def _create_live_context_pe(
     api_version: APIVersion,
     hardware_api: ThreadManagedHardware,
     robot_type: RobotType,
     deck_type: str,
     extra_labware: Dict[str, "LabwareDefinitionDict"],
     bundled_data: Optional[Dict[str, bytes]],
+    use_virtual_hardware: bool = True,
 ) -> ProtocolContext:
     """Return a live ProtocolContext that controls the robot through ProtocolEngine."""
     assert api_version >= ENGINE_CORE_API_VERSION
 
     global _LIVE_PROTOCOL_ENGINE_CONTEXTS
     pe, loop = _LIVE_PROTOCOL_ENGINE_CONTEXTS.enter_context(
         create_protocol_engine_in_thread(
             hardware_api=hardware_api.wrapped(),
-            config=_get_protocol_engine_config(robot_type),
+            config=_get_protocol_engine_config(
+                robot_type, virtual=use_virtual_hardware
+            ),
             drop_tips_after_run=False,
             post_run_hardware_state=PostRunHardwareState.STAY_ENGAGED_IN_PLACE,
             load_fixed_trash=should_load_fixed_trash_labware_for_python_protocol(
                 api_version
             ),
         )
     )
@@ -862,15 +868,17 @@
     scraper = _CommandScraper(logger=logger, level=level, broker=context.broker)
     if duration_estimator:
         context.broker.subscribe(command_types.COMMAND, duration_estimator.on_message)
 
     context.home()
     with scraper.scrape():
         try:
-            execute.run_protocol(protocol, context)
+            # TODO (spp, 2024-03-18): use true run-time param overrides once enabled
+            #  for cli protocol simulation/ execution
+            execute.run_protocol(protocol, context, run_time_param_overrides=None)
             if (
                 isinstance(protocol, PythonProtocol)
                 and protocol.api_level >= APIVersion(2, 0)
                 and protocol.bundled_labware is None
                 and allow_bundle()
             ):
                 bundle_contents: Optional[BundleContents] = bundle_from_sim(
@@ -893,15 +901,15 @@
     log_level: str,
 ) -> _SimulateResult:
     """Run a protocol file with Protocol Engine."""
 
     async def run(protocol_source: ProtocolSource) -> _SimulateResult:
         protocol_engine = await create_protocol_engine(
             hardware_api=hardware_api.wrapped(),
-            config=_get_protocol_engine_config(robot_type),
+            config=_get_protocol_engine_config(robot_type, virtual=True),
             load_fixed_trash=should_load_fixed_trash(protocol_source.config),
         )
 
         protocol_runner = create_protocol_runner(
             protocol_config=protocol_source.config,
             protocol_engine=protocol_engine,
             hardware_api=hardware_api.wrapped(),
@@ -928,23 +936,23 @@
 
         return scraper.commands, bundle_contents
 
     with entrypoint_util.adapt_protocol_source(protocol) as protocol_source:
         return asyncio.run(run(protocol_source))
 
 
-def _get_protocol_engine_config(robot_type: RobotType) -> Config:
+def _get_protocol_engine_config(robot_type: RobotType, virtual: bool) -> Config:
     """Return a Protocol Engine config to execute protocols on this device."""
     return Config(
         robot_type=robot_type,
         deck_type=DeckType(deck_type_for_simulation(robot_type)),
         ignore_pause=True,
-        use_virtual_pipettes=True,
-        use_virtual_modules=True,
-        use_virtual_gripper=True,
+        use_virtual_pipettes=virtual,
+        use_virtual_modules=virtual,
+        use_virtual_gripper=virtual,
         use_simulated_deck_config=True,
     )
 
 
 @atexit.register
 def _clear_live_protocol_engine_contexts() -> None:
     global _LIVE_PROTOCOL_ENGINE_CONTEXTS
```

### Comparing `opentrons-7.2.2a3/src/opentrons/system/camera.py` & `opentrons-7.3.0a0/src/opentrons/system/camera.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/system/log_control.py` & `opentrons-7.3.0a0/src/opentrons/system/log_control.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/system/nmcli.py` & `opentrons-7.3.0a0/src/opentrons/system/nmcli.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/system/resin.py` & `opentrons-7.3.0a0/src/opentrons/system/resin.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/system/smoothie_update.py` & `opentrons-7.3.0a0/src/opentrons/system/smoothie_update.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/system/wifi.py` & `opentrons-7.3.0a0/src/opentrons/system/wifi.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/tools/args_handler.py` & `opentrons-7.3.0a0/src/opentrons/tools/args_handler.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/tools/write_pipette_memory.py` & `opentrons-7.3.0a0/src/opentrons/tools/write_pipette_memory.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/types.py` & `opentrons-7.3.0a0/src/opentrons/types.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/util/async_helpers.py` & `opentrons-7.3.0a0/src/opentrons/util/async_helpers.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/util/broker.py` & `opentrons-7.3.0a0/src/opentrons/util/broker.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/util/entrypoint_util.py` & `opentrons-7.3.0a0/src/opentrons/util/entrypoint_util.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/util/linal.py` & `opentrons-7.3.0a0/src/opentrons/util/linal.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons/util/logging_config.py` & `opentrons-7.3.0a0/src/opentrons/util/logging_config.py`

 * *Files identical despite different names*

### Comparing `opentrons-7.2.2a3/src/opentrons.egg-info/PKG-INFO` & `opentrons-7.3.0a0/src/opentrons.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentrons
-Version: 7.2.2a3
+Version: 7.3.0a0
 Summary: The Opentrons API is a simple framework designed to make writing automated biology lab protocols easy.
 Author: Opentrons
 Author-email: engineering@opentrons.com
 Maintainer: Opentrons
 Maintainer-email: engineering@opentrons.com
 License: Apache 2.0
 Project-URL: opentrons.com, https://www.opentrons.com
@@ -13,34 +13,32 @@
 Keywords: robots,protocols,synbio,pcr,automation,lab
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 License-File: ../LICENSE
-Requires-Dist: opentrons-shared-data==7.2.2a3
+Requires-Dist: opentrons-shared-data==7.3.0a0
 Requires-Dist: aionotify==0.2.0
 Requires-Dist: anyio<4.0.0,>=3.6.1
 Requires-Dist: jsonschema<4.18.0,>=3.0.1
 Requires-Dist: numpy<2,>=1.20.0
 Requires-Dist: pydantic<2.0.0,>=1.10.9
 Requires-Dist: pyserial>=3.5
 Requires-Dist: typing-extensions<5,>=4.0.0
 Requires-Dist: click<9,>=8.0.0
 Requires-Dist: importlib-metadata>=1.0; python_version < "3.8"
 Provides-Extra: ot2-hardware
-Requires-Dist: opentrons-hardware==7.2.2a3; extra == "ot2-hardware"
+Requires-Dist: opentrons-hardware==7.3.0a0; extra == "ot2-hardware"
 Provides-Extra: flex-hardware
-Requires-Dist: opentrons-hardware[FLEX]==7.2.2a3; extra == "flex-hardware"
+Requires-Dist: opentrons-hardware[FLEX]==7.3.0a0; extra == "flex-hardware"
 
 .. _Full API Documentation: http://docs.opentrons.com
 
 The Opentrons API is a simple framework designed to make it easy to write automated biology lab protocols for Opentrons robots.
 
 This package can be used to simulate protocols on your computer without connecting to a robot. Please refer to our `Full API Documentation`_ for detailed instructions on how to write and simulate your first protocol.
```

### Comparing `opentrons-7.2.2a3/src/opentrons.egg-info/SOURCES.txt` & `opentrons-7.3.0a0/src/opentrons.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,21 +39,14 @@
 src/opentrons/calibration_storage/ot3/pipette_offset.py
 src/opentrons/calibration_storage/ot3/models/__init__.py
 src/opentrons/calibration_storage/ot3/models/defaults.py
 src/opentrons/calibration_storage/ot3/models/v1.py
 src/opentrons/cli/__init__.py
 src/opentrons/cli/__main__.py
 src/opentrons/cli/analyze.py
-src/opentrons/commands/__init__.py
-src/opentrons/commands/commands.py
-src/opentrons/commands/helpers.py
-src/opentrons/commands/module_commands.py
-src/opentrons/commands/protocol_commands.py
-src/opentrons/commands/publisher.py
-src/opentrons/commands/types.py
 src/opentrons/config/__init__.py
 src/opentrons/config/advanced_settings.py
 src/opentrons/config/defaults_ot2.py
 src/opentrons/config/defaults_ot3.py
 src/opentrons/config/feature_flags.py
 src/opentrons/config/gripper_config.py
 src/opentrons/config/reset.py
@@ -158,15 +151,14 @@
 src/opentrons/hardware_control/emulation/module_server/server.py
 src/opentrons/hardware_control/emulation/scripts/__init__.py
 src/opentrons/hardware_control/emulation/scripts/run_app.py
 src/opentrons/hardware_control/emulation/scripts/run_module_emulator.py
 src/opentrons/hardware_control/emulation/scripts/run_smoothie.py
 src/opentrons/hardware_control/instruments/__init__.py
 src/opentrons/hardware_control/instruments/instrument_abc.py
-src/opentrons/hardware_control/instruments/instrument_helpers.py
 src/opentrons/hardware_control/instruments/ot2/__init__.py
 src/opentrons/hardware_control/instruments/ot2/instrument_calibration.py
 src/opentrons/hardware_control/instruments/ot2/pipette.py
 src/opentrons/hardware_control/instruments/ot2/pipette_handler.py
 src/opentrons/hardware_control/instruments/ot3/__init__.py
 src/opentrons/hardware_control/instruments/ot3/gripper.py
 src/opentrons/hardware_control/instruments/ot3/gripper_handler.py
@@ -203,29 +195,37 @@
 src/opentrons/hardware_control/protocols/motion_controller.py
 src/opentrons/hardware_control/protocols/simulatable.py
 src/opentrons/hardware_control/protocols/stoppable.py
 src/opentrons/hardware_control/protocols/types.py
 src/opentrons/hardware_control/scripts/__init__.py
 src/opentrons/hardware_control/scripts/gripper_control.py
 src/opentrons/hardware_control/scripts/repl.py
+src/opentrons/legacy_commands/__init__.py
+src/opentrons/legacy_commands/commands.py
+src/opentrons/legacy_commands/helpers.py
+src/opentrons/legacy_commands/module_commands.py
+src/opentrons/legacy_commands/protocol_commands.py
+src/opentrons/legacy_commands/publisher.py
+src/opentrons/legacy_commands/types.py
 src/opentrons/motion_planning/__init__.py
 src/opentrons/motion_planning/adjacent_slots_getters.py
 src/opentrons/motion_planning/deck_conflict.py
 src/opentrons/motion_planning/errors.py
 src/opentrons/motion_planning/types.py
 src/opentrons/motion_planning/waypoints.py
 src/opentrons/protocol_api/__init__.py
 src/opentrons/protocol_api/_liquid.py
 src/opentrons/protocol_api/_nozzle_layout.py
-src/opentrons/protocol_api/_trash_bin.py
+src/opentrons/protocol_api/_parameter_context.py
+src/opentrons/protocol_api/_parameters.py
 src/opentrons/protocol_api/_types.py
-src/opentrons/protocol_api/_waste_chute.py
 src/opentrons/protocol_api/config.py
 src/opentrons/protocol_api/create_protocol_context.py
 src/opentrons/protocol_api/deck.py
+src/opentrons/protocol_api/disposal_locations.py
 src/opentrons/protocol_api/instrument_context.py
 src/opentrons/protocol_api/labware.py
 src/opentrons/protocol_api/module_contexts.py
 src/opentrons/protocol_api/module_validation_and_errors.py
 src/opentrons/protocol_api/protocol_context.py
 src/opentrons/protocol_api/validation.py
 src/opentrons/protocol_api/core/__init__.py
@@ -260,14 +260,15 @@
 src/opentrons/protocol_api/core/legacy/module_geometry.py
 src/opentrons/protocol_api/core/legacy/well_geometry.py
 src/opentrons/protocol_api/core/legacy_simulator/__init__.py
 src/opentrons/protocol_api/core/legacy_simulator/legacy_instrument_core.py
 src/opentrons/protocol_api/core/legacy_simulator/legacy_protocol_core.py
 src/opentrons/protocol_engine/__init__.py
 src/opentrons/protocol_engine/create_protocol_engine.py
+src/opentrons/protocol_engine/error_recovery_policy.py
 src/opentrons/protocol_engine/plugins.py
 src/opentrons/protocol_engine/protocol_engine.py
 src/opentrons/protocol_engine/slot_standardization.py
 src/opentrons/protocol_engine/types.py
 src/opentrons/protocol_engine/actions/__init__.py
 src/opentrons/protocol_engine/actions/action_dispatcher.py
 src/opentrons/protocol_engine/actions/action_handler.py
@@ -304,14 +305,15 @@
 src/opentrons/protocol_engine/commands/move_to_addressable_area.py
 src/opentrons/protocol_engine/commands/move_to_addressable_area_for_drop_tip.py
 src/opentrons/protocol_engine/commands/move_to_coordinates.py
 src/opentrons/protocol_engine/commands/move_to_well.py
 src/opentrons/protocol_engine/commands/pick_up_tip.py
 src/opentrons/protocol_engine/commands/pipetting_common.py
 src/opentrons/protocol_engine/commands/prepare_to_aspirate.py
+src/opentrons/protocol_engine/commands/reload_labware.py
 src/opentrons/protocol_engine/commands/retract_axis.py
 src/opentrons/protocol_engine/commands/save_position.py
 src/opentrons/protocol_engine/commands/set_rail_lights.py
 src/opentrons/protocol_engine/commands/set_status_bar.py
 src/opentrons/protocol_engine/commands/touch_tip.py
 src/opentrons/protocol_engine/commands/verify_tip_presence.py
 src/opentrons/protocol_engine/commands/wait_for_duration.py
@@ -363,28 +365,31 @@
 src/opentrons/protocol_engine/execution/queue_worker.py
 src/opentrons/protocol_engine/execution/rail_lights.py
 src/opentrons/protocol_engine/execution/run_control.py
 src/opentrons/protocol_engine/execution/status_bar.py
 src/opentrons/protocol_engine/execution/thermocycler_movement_flagger.py
 src/opentrons/protocol_engine/execution/thermocycler_plate_lifter.py
 src/opentrons/protocol_engine/execution/tip_handler.py
+src/opentrons/protocol_engine/notes/__init__.py
+src/opentrons/protocol_engine/notes/notes.py
 src/opentrons/protocol_engine/resources/__init__.py
 src/opentrons/protocol_engine/resources/deck_configuration_provider.py
 src/opentrons/protocol_engine/resources/deck_data_provider.py
 src/opentrons/protocol_engine/resources/fixture_validation.py
 src/opentrons/protocol_engine/resources/labware_data_provider.py
 src/opentrons/protocol_engine/resources/labware_validation.py
 src/opentrons/protocol_engine/resources/model_utils.py
 src/opentrons/protocol_engine/resources/module_data_provider.py
 src/opentrons/protocol_engine/resources/ot3_validation.py
 src/opentrons/protocol_engine/resources/pipette_data_provider.py
 src/opentrons/protocol_engine/state/__init__.py
 src/opentrons/protocol_engine/state/abstract_store.py
 src/opentrons/protocol_engine/state/addressable_areas.py
 src/opentrons/protocol_engine/state/change_notifier.py
+src/opentrons/protocol_engine/state/command_history.py
 src/opentrons/protocol_engine/state/commands.py
 src/opentrons/protocol_engine/state/config.py
 src/opentrons/protocol_engine/state/geometry.py
 src/opentrons/protocol_engine/state/labware.py
 src/opentrons/protocol_engine/state/liquids.py
 src/opentrons/protocol_engine/state/modules.py
 src/opentrons/protocol_engine/state/motion.py
@@ -451,14 +456,18 @@
 src/opentrons/protocols/execution/json_dispatchers.py
 src/opentrons/protocols/execution/types.py
 src/opentrons/protocols/geometry/__init__.py
 src/opentrons/protocols/geometry/labware_geometry.py
 src/opentrons/protocols/geometry/planning.py
 src/opentrons/protocols/models/__init__.py
 src/opentrons/protocols/models/json_protocol.py
+src/opentrons/protocols/parameters/__init__.py
+src/opentrons/protocols/parameters/parameter_definition.py
+src/opentrons/protocols/parameters/types.py
+src/opentrons/protocols/parameters/validation.py
 src/opentrons/resources/smoothie-edge-8414642.hex
 src/opentrons/resources/scripts/lpc21isp
 src/opentrons/system/__init__.py
 src/opentrons/system/camera.py
 src/opentrons/system/log_control.py
 src/opentrons/system/nmcli.py
 src/opentrons/system/resin.py
@@ -469,8 +478,9 @@
 src/opentrons/tools/write_pipette_memory.py
 src/opentrons/util/__init__.py
 src/opentrons/util/async_helpers.py
 src/opentrons/util/broker.py
 src/opentrons/util/entrypoint_util.py
 src/opentrons/util/helpers.py
 src/opentrons/util/linal.py
-src/opentrons/util/logging_config.py
+src/opentrons/util/logging_config.py
+src/opentrons/util/performance_helpers.py
```

