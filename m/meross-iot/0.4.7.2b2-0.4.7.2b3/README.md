# Comparing `tmp/meross_iot-0.4.7.2b2.tar.gz` & `tmp/meross_iot-0.4.7.2b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meross_iot-0.4.7.2b2.tar", last modified: Wed May  1 10:18:02 2024, max compression
+gzip compressed data, was "meross_iot-0.4.7.2b3.tar", last modified: Thu May  2 18:05:04 2024, max compression
```

## Comparing `meross_iot-0.4.7.2b2.tar` & `meross_iot-0.4.7.2b3.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:18:02.428065 meross_iot-0.4.7.2b2/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/.version
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19314 2024-05-01 10:18:02.428065 meross_iot-0.4.7.2b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18020 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:18:02.412065 meross_iot-0.4.7.2b2/meross_iot/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:18:02.416065 meross_iot-0.4.7.2b2/meross_iot/controller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21400 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/controller/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:18:02.420065 meross_iot-0.4.7.2b2/meross_iot/controller/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/controller/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/controller/mixins/consumption.py
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/controller/mixins/diffuser_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/controller/mixins/diffuser_spray.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/controller/mixins/dnd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/controller/mixins/electricity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/controller/mixins/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/controller/mixins/garage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/controller/mixins/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/controller/mixins/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     9288 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/controller/mixins/roller_shutter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/controller/mixins/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/controller/mixins/spray.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/controller/mixins/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     9564 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/controller/mixins/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/controller/mixins/toggle.py
--rw-r--r--   0 runner    (1001) docker     (127)    18079 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/controller/subdevice.py
--rw-r--r--   0 runner    (1001) docker     (127)    10889 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/device_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/error_budget.py
--rw-r--r--   0 runner    (1001) docker     (127)    31385 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/http_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    54928 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:18:02.420065 meross_iot-0.4.7.2b2/meross_iot/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:18:02.420065 meross_iot-0.4.7.2b2/meross_iot/model/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/http/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/http/error_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/http/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/http/subdevice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:18:02.420065 meross_iot-0.4.7.2b2/meross_iot/model/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/plugin/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/plugin/light.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/plugin/power.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:18:02.424065 meross_iot-0.4.7.2b2/meross_iot/model/push/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/push/bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/push/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/push/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/push/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/push/online.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/push/unbind.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/model/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:18:02.424065 meross_iot-0.4.7.2b2/meross_iot/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/utilities/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/utilities/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/utilities/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/utilities/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    12305 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/meross_iot/utilities/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:18:02.428065 meross_iot-0.4.7.2b2/meross_iot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19314 2024-05-01 10:18:02.000000 meross_iot-0.4.7.2b2/meross_iot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-01 10:18:02.000000 meross_iot-0.4.7.2b2/meross_iot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 10:18:02.000000 meross_iot-0.4.7.2b2/meross_iot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-01 10:18:02.000000 meross_iot-0.4.7.2b2/meross_iot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-01 10:18:02.000000 meross_iot-0.4.7.2b2/meross_iot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 10:18:02.000000 meross_iot-0.4.7.2b2/meross_iot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 10:18:02.428065 meross_iot-0.4.7.2b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:18:02.428065 meross_iot-0.4.7.2b2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_consumptionx.py
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_diffuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_disconnection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_dnd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_electricity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_garage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_push_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_roller_shutter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_spray.py
--rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_thermostat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_toggle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_togglex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_transport_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/tests/test_valve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:18:02.428065 meross_iot-0.4.7.2b2/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/utilities/meross_fake_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/utilities/meross_fake_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/utilities/meross_sniffer.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-01 10:17:47.000000 meross_iot-0.4.7.2b2/utilities/mixedqueue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:05:04.714771 meross_iot-0.4.7.2b3/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/.version
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19376 2024-05-02 18:05:04.714771 meross_iot-0.4.7.2b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18082 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:05:04.702771 meross_iot-0.4.7.2b3/meross_iot/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:05:04.702771 meross_iot-0.4.7.2b3/meross_iot/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21400 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/controller/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:05:04.706771 meross_iot-0.4.7.2b3/meross_iot/controller/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/controller/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/controller/mixins/consumption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/controller/mixins/diffuser_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/controller/mixins/diffuser_spray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/controller/mixins/dnd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/controller/mixins/electricity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/controller/mixins/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/controller/mixins/garage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/controller/mixins/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/controller/mixins/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9288 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/controller/mixins/roller_shutter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/controller/mixins/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/controller/mixins/spray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/controller/mixins/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9564 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/controller/mixins/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/controller/mixins/toggle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18079 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/controller/subdevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11003 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/device_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/error_budget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31385 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/http_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54928 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:05:04.706771 meross_iot-0.4.7.2b3/meross_iot/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:05:04.706771 meross_iot-0.4.7.2b3/meross_iot/model/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/http/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/http/error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/http/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/http/subdevice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:05:04.706771 meross_iot-0.4.7.2b3/meross_iot/model/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/plugin/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/plugin/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/plugin/power.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:05:04.710771 meross_iot-0.4.7.2b3/meross_iot/model/push/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/push/bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/push/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/push/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/push/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/push/online.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/push/unbind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/model/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:05:04.710771 meross_iot-0.4.7.2b3/meross_iot/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/utilities/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/utilities/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/utilities/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/utilities/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12305 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/meross_iot/utilities/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:05:04.714771 meross_iot-0.4.7.2b3/meross_iot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19376 2024-05-02 18:05:04.000000 meross_iot-0.4.7.2b3/meross_iot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-02 18:05:04.000000 meross_iot-0.4.7.2b3/meross_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 18:05:04.000000 meross_iot-0.4.7.2b3/meross_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-02 18:05:04.000000 meross_iot-0.4.7.2b3/meross_iot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-02 18:05:04.000000 meross_iot-0.4.7.2b3/meross_iot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 18:05:04.000000 meross_iot-0.4.7.2b3/meross_iot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 18:05:04.714771 meross_iot-0.4.7.2b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:05:04.714771 meross_iot-0.4.7.2b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_consumptionx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_diffuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_disconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_dnd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_electricity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_garage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_push_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_roller_shutter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_spray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_toggle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_togglex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_transport_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/tests/test_valve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:05:04.714771 meross_iot-0.4.7.2b3/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/utilities/meross_fake_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/utilities/meross_fake_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/utilities/meross_sniffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-02 18:04:49.000000 meross_iot-0.4.7.2b3/utilities/mixedqueue.py
```

### Comparing `meross_iot-0.4.7.2b2/LICENSE` & `meross_iot-0.4.7.2b3/LICENSE`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/PKG-INFO` & `meross_iot-0.4.7.2b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meross_iot
-Version: 0.4.7.2b2
+Version: 0.4.7.2b3
 Summary: A simple library to deal with Meross devices. At the moment MSS110, MSS210, MSS310, MSS310H smart plugs and the MSS425E power strip. Other meross device might work out of the box with limited functionality. Give it a try and, in case of problems, let the developer know by opening an issue on Github.
 Home-page: https://github.com/albertogeniola/MerossIot
 Author: Alberto Geniola
 Author-email: albertogeniola@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/albertogeniola/MerossIot
 Project-URL: Funding, https://donate.pypi.org
@@ -133,15 +133,17 @@
 - MSS310 (Smart plug with power consumption)
 - MSS310h (Smart plug with power consumption)
 - MSS425E/MSS425F (Smart strip)
 - MSS530H (Wall-mount switches)
 - MSG100 (Garage opener)
 - MSG200 (3-doors Garage opener)
 - MSH300 (Smart hub + valve thermostat)
+- MSH300HK (Smart Hub)
 - MS100 (Smart hub + temperature/humidity sensor)
+- MS100F (temperature/humidity sensor)
 - MSS710
 - MSXH0 (Smart Humidifier)
 
 I'd like to thank all the people who contributed to the early stage of library development,
 who stimulated me to continue the development and making this library support more devices.
 
 Thanks to [DanoneKiD](https://github.com/DanoneKiD),
```

### Comparing `meross_iot-0.4.7.2b2/README.md` & `meross_iot-0.4.7.2b3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,17 @@
 - MSS310 (Smart plug with power consumption)
 - MSS310h (Smart plug with power consumption)
 - MSS425E/MSS425F (Smart strip)
 - MSS530H (Wall-mount switches)
 - MSG100 (Garage opener)
 - MSG200 (3-doors Garage opener)
 - MSH300 (Smart hub + valve thermostat)
+- MSH300HK (Smart Hub)
 - MS100 (Smart hub + temperature/humidity sensor)
+- MS100F (temperature/humidity sensor)
 - MSS710
 - MSXH0 (Smart Humidifier)
 
 I'd like to thank all the people who contributed to the early stage of library development,
 who stimulated me to continue the development and making this library support more devices.
 
 Thanks to [DanoneKiD](https://github.com/DanoneKiD),
```

### Comparing `meross_iot-0.4.7.2b2/meross_iot/controller/device.py` & `meross_iot-0.4.7.2b3/meross_iot/controller/device.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/controller/mixins/consumption.py` & `meross_iot-0.4.7.2b3/meross_iot/controller/mixins/consumption.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/controller/mixins/diffuser_light.py` & `meross_iot-0.4.7.2b3/meross_iot/controller/mixins/diffuser_light.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/controller/mixins/diffuser_spray.py` & `meross_iot-0.4.7.2b3/meross_iot/controller/mixins/diffuser_spray.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/controller/mixins/dnd.py` & `meross_iot-0.4.7.2b3/meross_iot/controller/mixins/dnd.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/controller/mixins/electricity.py` & `meross_iot-0.4.7.2b3/meross_iot/controller/mixins/electricity.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/controller/mixins/encryption.py` & `meross_iot-0.4.7.2b3/meross_iot/controller/mixins/encryption.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/controller/mixins/garage.py` & `meross_iot-0.4.7.2b3/meross_iot/controller/mixins/garage.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/controller/mixins/hub.py` & `meross_iot-0.4.7.2b3/meross_iot/controller/mixins/hub.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/controller/mixins/light.py` & `meross_iot-0.4.7.2b3/meross_iot/controller/mixins/light.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/controller/mixins/roller_shutter.py` & `meross_iot-0.4.7.2b3/meross_iot/controller/mixins/roller_shutter.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/controller/mixins/runtime.py` & `meross_iot-0.4.7.2b3/meross_iot/controller/mixins/runtime.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/controller/mixins/spray.py` & `meross_iot-0.4.7.2b3/meross_iot/controller/mixins/spray.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/controller/mixins/system.py` & `meross_iot-0.4.7.2b3/meross_iot/controller/mixins/system.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/controller/mixins/thermostat.py` & `meross_iot-0.4.7.2b3/meross_iot/controller/mixins/thermostat.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/controller/mixins/toggle.py` & `meross_iot-0.4.7.2b3/meross_iot/controller/mixins/toggle.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/controller/subdevice.py` & `meross_iot-0.4.7.2b3/meross_iot/controller/subdevice.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/device_factory.py` & `meross_iot-0.4.7.2b3/meross_iot/device_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 from meross_iot.model.http.device import HttpDeviceInfo
 from meross_iot.model.http.subdevice import HttpSubdeviceInfo
 
 _LOGGER = logging.getLogger(__name__)
 
 _KNOWN_DEV_TYPES_CLASSES = {
     "mts100v3": Mts100v3Valve,
-    "ms100": Ms100Sensor
+    "ms100": Ms100Sensor,
+    "ms100f": Ms100Sensor
 }
 
 _ABILITY_MATRIX = {
     # Power plugs abilities
     Namespace.CONTROL_TOGGLEX.value: ToggleXMixin,
     Namespace.CONTROL_TOGGLE.value: ToggleMixin,
     Namespace.CONTROL_CONSUMPTIONX.value: ConsumptionXMixin,
@@ -81,15 +82,16 @@
     Namespace.CONTROL_THERMOSTAT_MODE.value: ThermostatModeMixin,
 
     # TODO: BIND, UNBIND, ONLINE, WIFI, ETC!
 }
 
 _SUBDEVICE_MAPPING = {
     "mts100v3": Mts100v3Valve,
-    "ms100": Ms100Sensor
+    "ms100": Ms100Sensor,
+    "ms100f": Ms100Sensor
 }
 
 _dynamic_types = {}
 
 
 def _caclulate_device_type_name(device_type: str, hardware_version: str, firmware_version: str) -> str:
     """
@@ -183,20 +185,20 @@
 
         # Let's now pick the base class where to attach all the mixin.
         # We basically offer two possible base implementations:
         # - BaseMerossDevice: suitable for all non-hub devices
         # - HubMerossDevice: to be used when dealing with Hubs.
         # Unfortunately, it's not clear how we should discriminate an hub from a non-hub.
         # The current implementation decides which base class to use by looking at the presence
-        # of 'Appliance.Digest.Hub' namespace within the exposed abilities.
-        discriminating_ability = Namespace.SYSTEM_DIGEST_HUB.value
+        # of 'Appliance.Hub.SubdeviceList': if exposed, we assume the device is a fully featured hub.
+        discriminating_abilities = [Namespace.HUB_SUBDEVICELIST.value]
         base_class = BaseDevice
-        if discriminating_ability in device_abilities:
+        if any (da in device_abilities for da in discriminating_abilities):
             _LOGGER.warning(f"Device {http_device_info.dev_name} ({http_device_info.device_type}, "
-                            f"uuid {http_device_info.uuid}) reported ability {discriminating_ability}. "
+                            f"uuid {http_device_info.uuid}) reported one ability of {discriminating_abilities}. "
                             f"Assuming this is a full-featured HUB.")
             base_class = HubDevice
 
         cached_type = _build_cached_type(type_string=device_type_name,
                                          device_abilities=device_abilities,
                                          base_class=base_class)
         _dynamic_types[device_type_name] = cached_type
```

### Comparing `meross_iot-0.4.7.2b2/meross_iot/error_budget.py` & `meross_iot-0.4.7.2b3/meross_iot/error_budget.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/http_api.py` & `meross_iot-0.4.7.2b3/meross_iot/http_api.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/manager.py` & `meross_iot-0.4.7.2b3/meross_iot/manager.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/model/credentials.py` & `meross_iot-0.4.7.2b3/meross_iot/model/credentials.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/model/enums.py` & `meross_iot-0.4.7.2b3/meross_iot/model/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,15 @@
     DIFFUSER_SPRAY = "Appliance.Control.Diffuser.Spray"
 
     # HUB
     HUB_EXCEPTION = 'Appliance.Hub.Exception'
     HUB_BATTERY = 'Appliance.Hub.Battery'
     HUB_TOGGLEX = 'Appliance.Hub.ToggleX'
     HUB_ONLINE = 'Appliance.Hub.Online'
+    HUB_SUBDEVICELIST = 'Appliance.Hub.SubdeviceList'
 
     # SENSORS
     HUB_SENSOR_ALL = 'Appliance.Hub.Sensor.All'
     HUB_SENSOR_TEMPHUM = 'Appliance.Hub.Sensor.TempHum'
     HUB_SENSOR_ALERT = 'Appliance.Hub.Sensor.Alert'
 
     # MTS100
```

### Comparing `meross_iot-0.4.7.2b2/meross_iot/model/exception.py` & `meross_iot-0.4.7.2b3/meross_iot/model/exception.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/model/http/device.py` & `meross_iot-0.4.7.2b3/meross_iot/model/http/device.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/model/http/error_codes.py` & `meross_iot-0.4.7.2b3/meross_iot/model/http/error_codes.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/model/http/exception.py` & `meross_iot-0.4.7.2b3/meross_iot/model/http/exception.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/model/http/subdevice.py` & `meross_iot-0.4.7.2b3/meross_iot/model/http/subdevice.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/model/plugin/hub.py` & `meross_iot-0.4.7.2b3/meross_iot/model/plugin/hub.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/model/plugin/light.py` & `meross_iot-0.4.7.2b3/meross_iot/model/plugin/light.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/model/plugin/power.py` & `meross_iot-0.4.7.2b3/meross_iot/model/plugin/power.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/model/push/bind.py` & `meross_iot-0.4.7.2b3/meross_iot/model/push/bind.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/model/push/common.py` & `meross_iot-0.4.7.2b3/meross_iot/model/push/common.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/model/push/factory.py` & `meross_iot-0.4.7.2b3/meross_iot/model/push/factory.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/model/push/online.py` & `meross_iot-0.4.7.2b3/meross_iot/model/push/online.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/model/shared.py` & `meross_iot-0.4.7.2b3/meross_iot/model/shared.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/utilities/conversion.py` & `meross_iot-0.4.7.2b3/meross_iot/utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/utilities/mqtt.py` & `meross_iot-0.4.7.2b3/meross_iot/utilities/mqtt.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot/utilities/stats.py` & `meross_iot-0.4.7.2b3/meross_iot/utilities/stats.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/meross_iot.egg-info/PKG-INFO` & `meross_iot-0.4.7.2b3/meross_iot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meross_iot
-Version: 0.4.7.2b2
+Version: 0.4.7.2b3
 Summary: A simple library to deal with Meross devices. At the moment MSS110, MSS210, MSS310, MSS310H smart plugs and the MSS425E power strip. Other meross device might work out of the box with limited functionality. Give it a try and, in case of problems, let the developer know by opening an issue on Github.
 Home-page: https://github.com/albertogeniola/MerossIot
 Author: Alberto Geniola
 Author-email: albertogeniola@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/albertogeniola/MerossIot
 Project-URL: Funding, https://donate.pypi.org
@@ -133,15 +133,17 @@
 - MSS310 (Smart plug with power consumption)
 - MSS310h (Smart plug with power consumption)
 - MSS425E/MSS425F (Smart strip)
 - MSS530H (Wall-mount switches)
 - MSG100 (Garage opener)
 - MSG200 (3-doors Garage opener)
 - MSH300 (Smart hub + valve thermostat)
+- MSH300HK (Smart Hub)
 - MS100 (Smart hub + temperature/humidity sensor)
+- MS100F (temperature/humidity sensor)
 - MSS710
 - MSXH0 (Smart Humidifier)
 
 I'd like to thank all the people who contributed to the early stage of library development,
 who stimulated me to continue the development and making this library support more devices.
 
 Thanks to [DanoneKiD](https://github.com/DanoneKiD),
```

### Comparing `meross_iot-0.4.7.2b2/meross_iot.egg-info/SOURCES.txt` & `meross_iot-0.4.7.2b3/meross_iot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/setup.py` & `meross_iot-0.4.7.2b3/setup.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_consumptionx.py` & `meross_iot-0.4.7.2b3/tests/test_consumptionx.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_diffuser.py` & `meross_iot-0.4.7.2b3/tests/test_diffuser.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_disconnection.py` & `meross_iot-0.4.7.2b3/tests/test_disconnection.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_dnd.py` & `meross_iot-0.4.7.2b3/tests/test_dnd.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_electricity.py` & `meross_iot-0.4.7.2b3/tests/test_electricity.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_error.py` & `meross_iot-0.4.7.2b3/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_garage.py` & `meross_iot-0.4.7.2b3/tests/test_garage.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_http.py` & `meross_iot-0.4.7.2b3/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_hub.py` & `meross_iot-0.4.7.2b3/tests/test_hub.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_light.py` & `meross_iot-0.4.7.2b3/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_push_handler.py` & `meross_iot-0.4.7.2b3/tests/test_push_handler.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_roller_shutter.py` & `meross_iot-0.4.7.2b3/tests/test_roller_shutter.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_runtime.py` & `meross_iot-0.4.7.2b3/tests/test_runtime.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_sensor.py` & `meross_iot-0.4.7.2b3/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_spray.py` & `meross_iot-0.4.7.2b3/tests/test_spray.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_thermostat.py` & `meross_iot-0.4.7.2b3/tests/test_thermostat.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_timeout.py` & `meross_iot-0.4.7.2b3/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_toggle.py` & `meross_iot-0.4.7.2b3/tests/test_toggle.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_togglex.py` & `meross_iot-0.4.7.2b3/tests/test_togglex.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_transport_mode.py` & `meross_iot-0.4.7.2b3/tests/test_transport_mode.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_update.py` & `meross_iot-0.4.7.2b3/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/tests/test_valve.py` & `meross_iot-0.4.7.2b3/tests/test_valve.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/utilities/meross_fake_app.py` & `meross_iot-0.4.7.2b3/utilities/meross_fake_app.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/utilities/meross_fake_device.py` & `meross_iot-0.4.7.2b3/utilities/meross_fake_device.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/utilities/meross_sniffer.py` & `meross_iot-0.4.7.2b3/utilities/meross_sniffer.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.2b2/utilities/mixedqueue.py` & `meross_iot-0.4.7.2b3/utilities/mixedqueue.py`

 * *Files identical despite different names*

