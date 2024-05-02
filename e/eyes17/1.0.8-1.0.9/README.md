# Comparing `tmp/eyes17-1.0.8.tar.gz` & `tmp/eyes17-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eyes17-1.0.8.tar", last modified: Thu Jan 23 18:58:29 2020, max compression
+gzip compressed data, was "dist/eyes17-1.0.9.tar", last modified: Fri Jan 24 04:57:12 2020, max compression
```

## Comparing `eyes17-1.0.8.tar` & `eyes17-1.0.9.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 jithin    (1000) jithin    (1000)        0 2020-01-23 18:58:29.000000 eyes17-1.0.8/
-drwxr-xr-x   0 jithin    (1000) jithin    (1000)        0 2020-01-23 18:58:29.000000 eyes17-1.0.8/eyes17/
--rw-r--r--   0 jithin    (1000) jithin    (1000)   116048 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/eyes.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)    14795 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/Peripherals.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     7413 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/achan.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)    12938 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/eyeplot17.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     7458 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/packet_handler.py
-drwxr-xr-x   0 jithin    (1000) jithin    (1000)        0 2020-01-23 18:58:29.000000 eyes17-1.0.8/eyes17/SENSORS/
--rw-r--r--   0 jithin    (1000) jithin    (1000)     2557 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/SENSORS/ADS1248.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     2836 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/SENSORS/AD9833.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     2745 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/SENSORS/HMC5883L.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     5204 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/SENSORS/MPU925x.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     5491 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/SENSORS/MPU6050.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)    22457 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/SENSORS/MF522.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)      981 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/SENSORS/Kalman.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     3253 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/SENSORS/BMP180.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     6453 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/SENSORS/AD7718_class.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     7304 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/SENSORS/ADS1115.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     1486 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/SENSORS/MLX90614.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)      611 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/SENSORS/ComplementaryFilter.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     2349 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/SENSORS/SHT21.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     1597 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/SENSORS/BH1750.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)      661 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/SENSORS/supported.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     3102 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/SENSORS/TSL2561.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)    23659 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/SENSORS/SSD1306.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)        0 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/SENSORS/__init__.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     1169 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/sensorlist.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     5585 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/eyemath17.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     6211 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/commands_proto.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)        0 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17/__init__.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)      854 2020-01-23 18:58:29.000000 eyes17-1.0.8/PKG-INFO
-drwxr-xr-x   0 jithin    (1000) jithin    (1000)        0 2020-01-23 18:58:29.000000 eyes17-1.0.8/eyes17GUI/
--rw-r--r--   0 jithin    (1000) jithin    (1000)     6624 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/RCtransient.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     5220 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/induction.py
-drwxr-xr-x   0 jithin    (1000) jithin    (1000)        0 2020-01-23 18:58:29.000000 eyes17-1.0.8/eyes17GUI/eyes17/
--rw-r--r--   0 jithin    (1000) jithin    (1000)   116048 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/eyes.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)    14795 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/Peripherals.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     7413 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/achan.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)    12938 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/eyeplot17.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     7458 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/packet_handler.py
-drwxr-xr-x   0 jithin    (1000) jithin    (1000)        0 2020-01-23 18:58:29.000000 eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/
--rw-r--r--   0 jithin    (1000) jithin    (1000)     2557 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/ADS1248.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     2836 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/AD9833.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     2745 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/HMC5883L.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     5204 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/MPU925x.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     5491 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/MPU6050.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)    22457 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/MF522.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)      981 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/Kalman.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     3253 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/BMP180.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     6453 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/AD7718_class.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     7304 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/ADS1115.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     1486 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/MLX90614.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)      611 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/ComplementaryFilter.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     2349 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/SHT21.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     1597 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/BH1750.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)      661 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/supported.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     3102 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/TSL2561.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)    23659 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/SSD1306.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)        0 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/__init__.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     1169 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/sensorlist.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     5585 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/eyemath17.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     6211 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/commands_proto.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)        0 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/eyes17/__init__.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     7713 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/sr04dist_fft.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)    13622 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/RLCsteadystate.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     7233 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/plotIV.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     8460 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/pt100.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     5325 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/npnCEout.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     2443 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/tof.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     7713 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/sr04dist.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     6399 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/logger.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     6428 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/MPU6050.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     7398 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/drivenRodPendulum.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     1015 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/terminal.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     6070 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/pendulumVelocity.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)    17351 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/main.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     7626 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/soundBeats.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     6265 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/XYplot.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     4223 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/advanced_logger.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     4027 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/dust_sensor.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     6111 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/RLCtransient.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     8403 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/numpy_help.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     7638 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/utils.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     4931 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/BHCurve.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     6672 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/lightsensorlogger.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)       74 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/generateBC.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     1979 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/driven-pendulum.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     6910 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/RLtransient.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)    36360 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/i2cLogger.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     2470 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/QtVersion.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     5355 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/pnpCEout.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     7379 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/soundFreqResp.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     7113 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/XYplot2.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     6607 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/rodPendulum.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     5341 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/diodeIV.py
-drwxr-xr-x   0 jithin    (1000) jithin    (1000)        0 2020-01-23 18:58:29.000000 eyes17-1.0.8/eyes17GUI/layouts/
--rw-r--r--   0 jithin    (1000) jithin    (1000)    12680 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/layouts/oscilloscope_widget.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     4174 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/layouts/ui_dio_robot.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)    22433 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/layouts/advancedLoggerTools.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)    14643 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/layouts/ui_scope.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     4761 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/layouts/ui_dio_pwm.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     7496 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/layouts/ui_newtonslaws.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)   376652 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/layouts/res_rc.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     6424 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/layouts/ui_advancedLogger.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     4850 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/layouts/ui_dio_sensor.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     2653 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/layouts/ui_dio_control.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)    29782 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/layouts/ui_scope_layout.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)    23774 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/layouts/gauge.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     7165 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/layouts/ui_miniScope.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     5008 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/layouts/ui_inputSelector.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)        0 2020-01-23 18:58:27.000000 eyes17-1.0.8/eyes17GUI/layouts/__init__.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)      216 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/test.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     6516 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/soundVelocity.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     7747 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/pythonSyntax.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)    11293 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/scope2.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     2628 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/editor.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     7539 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/filterCircuit.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)    20023 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/scope.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     9406 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/newtons_laws.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)        0 2020-01-23 18:58:28.000000 eyes17-1.0.8/eyes17GUI/__init__.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)       38 2020-01-23 18:58:29.000000 eyes17-1.0.8/setup.cfg
-drwxr-xr-x   0 jithin    (1000) jithin    (1000)        0 2020-01-23 18:58:29.000000 eyes17-1.0.8/resources/
--rw-r--r--   0 jithin    (1000) jithin    (1000)      883 2019-10-27 06:56:48.000000 eyes17-1.0.8/resources/sispmctl.conf
--rw-r--r--   0 jithin    (1000) jithin    (1000)      636 2019-10-27 06:52:13.000000 eyes17-1.0.8/resources/99-eyes17-pip.rules
--rw-r--r--   0 jithin    (1000) jithin    (1000)        0 2019-10-27 06:59:21.000000 eyes17-1.0.8/resources/__init__.py
--rw-r--r--   0 jithin    (1000) jithin    (1000)     3043 2020-01-23 18:53:16.000000 eyes17-1.0.8/setup.py
--rwxrwxr-x   0 jithin    (1000) jithin    (1000)       24 2020-01-23 17:15:23.000000 eyes17-1.0.8/README.md
-drwxr-xr-x   0 jithin    (1000) jithin    (1000)        0 2020-01-23 18:58:29.000000 eyes17-1.0.8/eyes17.egg-info/
--rw-r--r--   0 jithin    (1000) jithin    (1000)        1 2020-01-23 18:58:29.000000 eyes17-1.0.8/eyes17.egg-info/dependency_links.txt
--rw-r--r--   0 jithin    (1000) jithin    (1000)      854 2020-01-23 18:58:29.000000 eyes17-1.0.8/eyes17.egg-info/PKG-INFO
--rw-r--r--   0 jithin    (1000) jithin    (1000)       62 2020-01-23 18:58:29.000000 eyes17-1.0.8/eyes17.egg-info/requires.txt
--rw-r--r--   0 jithin    (1000) jithin    (1000)       27 2020-01-23 18:58:29.000000 eyes17-1.0.8/eyes17.egg-info/top_level.txt
--rw-r--r--   0 jithin    (1000) jithin    (1000)     3402 2020-01-23 18:58:29.000000 eyes17-1.0.8/eyes17.egg-info/SOURCES.txt
--rw-r--r--   0 jithin    (1000) jithin    (1000)       47 2020-01-23 18:58:29.000000 eyes17-1.0.8/eyes17.egg-info/entry_points.txt
+drwxr-xr-x   0 jithin    (1000) jithin    (1000)        0 2020-01-24 04:57:12.000000 eyes17-1.0.9/
+drwxr-xr-x   0 jithin    (1000) jithin    (1000)        0 2020-01-24 04:57:12.000000 eyes17-1.0.9/eyes17/
+-rw-r--r--   0 jithin    (1000) jithin    (1000)   116048 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17/eyes.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)    14795 2020-01-24 04:57:05.000000 eyes17-1.0.9/eyes17/Peripherals.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     7413 2020-01-24 04:57:05.000000 eyes17-1.0.9/eyes17/achan.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)    12938 2020-01-24 04:57:05.000000 eyes17-1.0.9/eyes17/eyeplot17.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     7458 2020-01-24 04:57:05.000000 eyes17-1.0.9/eyes17/packet_handler.py
+drwxr-xr-x   0 jithin    (1000) jithin    (1000)        0 2020-01-24 04:57:12.000000 eyes17-1.0.9/eyes17/SENSORS/
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     2557 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17/SENSORS/ADS1248.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     2836 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17/SENSORS/AD9833.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     2745 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17/SENSORS/HMC5883L.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     5204 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17/SENSORS/MPU925x.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     5491 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17/SENSORS/MPU6050.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)    22457 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17/SENSORS/MF522.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)      981 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17/SENSORS/Kalman.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     3253 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17/SENSORS/BMP180.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     6453 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17/SENSORS/AD7718_class.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     7304 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17/SENSORS/ADS1115.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     1486 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17/SENSORS/MLX90614.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)      611 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17/SENSORS/ComplementaryFilter.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     2349 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17/SENSORS/SHT21.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     1597 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17/SENSORS/BH1750.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)      661 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17/SENSORS/supported.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     3102 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17/SENSORS/TSL2561.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)    23659 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17/SENSORS/SSD1306.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)        0 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17/SENSORS/__init__.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     1169 2020-01-24 04:57:05.000000 eyes17-1.0.9/eyes17/sensorlist.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     5585 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17/eyemath17.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     6211 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17/commands_proto.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)        0 2020-01-24 04:57:05.000000 eyes17-1.0.9/eyes17/__init__.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)      854 2020-01-24 04:57:12.000000 eyes17-1.0.9/PKG-INFO
+drwxr-xr-x   0 jithin    (1000) jithin    (1000)        0 2020-01-24 04:57:12.000000 eyes17-1.0.9/eyes17GUI/
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     6624 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/RCtransient.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     5220 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/induction.py
+drwxr-xr-x   0 jithin    (1000) jithin    (1000)        0 2020-01-24 04:57:12.000000 eyes17-1.0.9/eyes17GUI/eyes17/
+-rw-r--r--   0 jithin    (1000) jithin    (1000)   116048 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/eyes.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)    14795 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/Peripherals.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     7413 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/achan.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)    12938 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/eyeplot17.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     7458 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/packet_handler.py
+drwxr-xr-x   0 jithin    (1000) jithin    (1000)        0 2020-01-24 04:57:12.000000 eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     2557 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/ADS1248.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     2836 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/AD9833.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     2745 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/HMC5883L.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     5204 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/MPU925x.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     5491 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/MPU6050.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)    22457 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/MF522.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)      981 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/Kalman.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     3253 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/BMP180.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     6453 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/AD7718_class.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     7304 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/ADS1115.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     1486 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/MLX90614.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)      611 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/ComplementaryFilter.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     2349 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/SHT21.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     1597 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/BH1750.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)      661 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/supported.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     3102 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/TSL2561.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)    23659 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/SSD1306.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)        0 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/__init__.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     1169 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/sensorlist.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     5585 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/eyemath17.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     6211 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/commands_proto.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)        0 2020-01-24 04:57:06.000000 eyes17-1.0.9/eyes17GUI/eyes17/__init__.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     7713 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/sr04dist_fft.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)    13615 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/RLCsteadystate.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     7233 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/plotIV.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     8460 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/pt100.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     5325 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/npnCEout.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     2443 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/tof.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     7713 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/sr04dist.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     6399 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/logger.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     6428 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/MPU6050.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     7398 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/drivenRodPendulum.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     1015 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/terminal.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     6070 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/pendulumVelocity.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)    17351 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/main.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     7626 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/soundBeats.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     6265 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/XYplot.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     4223 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/advanced_logger.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     4027 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/dust_sensor.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     6111 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/RLCtransient.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     8403 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/numpy_help.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     7638 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/utils.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     4931 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/BHCurve.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     6672 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/lightsensorlogger.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)       74 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/generateBC.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     1979 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/driven-pendulum.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     6910 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/RLtransient.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)    36360 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/i2cLogger.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     2470 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/QtVersion.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     5355 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/pnpCEout.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     7379 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/soundFreqResp.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     7113 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/XYplot2.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     6607 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/rodPendulum.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     5341 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/diodeIV.py
+drwxr-xr-x   0 jithin    (1000) jithin    (1000)        0 2020-01-24 04:57:12.000000 eyes17-1.0.9/eyes17GUI/layouts/
+-rw-r--r--   0 jithin    (1000) jithin    (1000)    12680 2020-01-24 04:57:07.000000 eyes17-1.0.9/eyes17GUI/layouts/oscilloscope_widget.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     4174 2020-01-24 04:57:07.000000 eyes17-1.0.9/eyes17GUI/layouts/ui_dio_robot.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)    22433 2020-01-24 04:57:07.000000 eyes17-1.0.9/eyes17GUI/layouts/advancedLoggerTools.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)    14643 2020-01-24 04:57:07.000000 eyes17-1.0.9/eyes17GUI/layouts/ui_scope.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     4761 2020-01-24 04:57:07.000000 eyes17-1.0.9/eyes17GUI/layouts/ui_dio_pwm.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     7496 2020-01-24 04:57:07.000000 eyes17-1.0.9/eyes17GUI/layouts/ui_newtonslaws.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)   376652 2020-01-24 04:57:07.000000 eyes17-1.0.9/eyes17GUI/layouts/res_rc.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     6424 2020-01-24 04:57:07.000000 eyes17-1.0.9/eyes17GUI/layouts/ui_advancedLogger.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     4850 2020-01-24 04:57:07.000000 eyes17-1.0.9/eyes17GUI/layouts/ui_dio_sensor.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     2653 2020-01-24 04:57:07.000000 eyes17-1.0.9/eyes17GUI/layouts/ui_dio_control.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)    29782 2020-01-24 04:57:07.000000 eyes17-1.0.9/eyes17GUI/layouts/ui_scope_layout.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)    23774 2020-01-24 04:57:07.000000 eyes17-1.0.9/eyes17GUI/layouts/gauge.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     7165 2020-01-24 04:57:07.000000 eyes17-1.0.9/eyes17GUI/layouts/ui_miniScope.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     5008 2020-01-24 04:57:07.000000 eyes17-1.0.9/eyes17GUI/layouts/ui_inputSelector.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)        0 2020-01-24 04:57:07.000000 eyes17-1.0.9/eyes17GUI/layouts/__init__.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)      216 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/test.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     6516 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/soundVelocity.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     7747 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/pythonSyntax.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)    11293 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/scope2.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     2628 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/editor.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     7539 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/filterCircuit.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)    20023 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/scope.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     9406 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/newtons_laws.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)        0 2020-01-24 04:57:08.000000 eyes17-1.0.9/eyes17GUI/__init__.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)       38 2020-01-24 04:57:12.000000 eyes17-1.0.9/setup.cfg
+drwxr-xr-x   0 jithin    (1000) jithin    (1000)        0 2020-01-24 04:57:12.000000 eyes17-1.0.9/resources/
+-rw-r--r--   0 jithin    (1000) jithin    (1000)      883 2019-10-27 06:56:48.000000 eyes17-1.0.9/resources/sispmctl.conf
+-rw-r--r--   0 jithin    (1000) jithin    (1000)      636 2019-10-27 06:52:13.000000 eyes17-1.0.9/resources/99-eyes17-pip.rules
+-rw-r--r--   0 jithin    (1000) jithin    (1000)        0 2019-10-27 06:59:21.000000 eyes17-1.0.9/resources/__init__.py
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     3043 2020-01-24 10:24:04.000000 eyes17-1.0.9/setup.py
+-rwxrwxr-x   0 jithin    (1000) jithin    (1000)       24 2020-01-23 17:15:23.000000 eyes17-1.0.9/README.md
+drwxr-xr-x   0 jithin    (1000) jithin    (1000)        0 2020-01-24 04:57:12.000000 eyes17-1.0.9/eyes17.egg-info/
+-rw-r--r--   0 jithin    (1000) jithin    (1000)        1 2020-01-24 04:57:10.000000 eyes17-1.0.9/eyes17.egg-info/dependency_links.txt
+-rw-r--r--   0 jithin    (1000) jithin    (1000)      854 2020-01-24 04:57:10.000000 eyes17-1.0.9/eyes17.egg-info/PKG-INFO
+-rw-r--r--   0 jithin    (1000) jithin    (1000)       62 2020-01-24 04:57:10.000000 eyes17-1.0.9/eyes17.egg-info/requires.txt
+-rw-r--r--   0 jithin    (1000) jithin    (1000)       27 2020-01-24 04:57:10.000000 eyes17-1.0.9/eyes17.egg-info/top_level.txt
+-rw-r--r--   0 jithin    (1000) jithin    (1000)     3402 2020-01-24 04:57:11.000000 eyes17-1.0.9/eyes17.egg-info/SOURCES.txt
+-rw-r--r--   0 jithin    (1000) jithin    (1000)       47 2020-01-24 04:57:10.000000 eyes17-1.0.9/eyes17.egg-info/entry_points.txt
```

### Comparing `eyes17-1.0.8/eyes17/eyes.py` & `eyes17-1.0.9/eyes17/eyes.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/Peripherals.py` & `eyes17-1.0.9/eyes17/Peripherals.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/achan.py` & `eyes17-1.0.9/eyes17/achan.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/eyeplot17.py` & `eyes17-1.0.9/eyes17/eyeplot17.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/packet_handler.py` & `eyes17-1.0.9/eyes17/packet_handler.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/SENSORS/ADS1248.py` & `eyes17-1.0.9/eyes17/SENSORS/ADS1248.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/SENSORS/AD9833.py` & `eyes17-1.0.9/eyes17/SENSORS/AD9833.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/SENSORS/HMC5883L.py` & `eyes17-1.0.9/eyes17/SENSORS/HMC5883L.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/SENSORS/MPU925x.py` & `eyes17-1.0.9/eyes17/SENSORS/MPU925x.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/SENSORS/MPU6050.py` & `eyes17-1.0.9/eyes17/SENSORS/MPU6050.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/SENSORS/MF522.py` & `eyes17-1.0.9/eyes17/SENSORS/MF522.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/SENSORS/Kalman.py` & `eyes17-1.0.9/eyes17/SENSORS/Kalman.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/SENSORS/BMP180.py` & `eyes17-1.0.9/eyes17/SENSORS/BMP180.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/SENSORS/AD7718_class.py` & `eyes17-1.0.9/eyes17/SENSORS/AD7718_class.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/SENSORS/ADS1115.py` & `eyes17-1.0.9/eyes17/SENSORS/ADS1115.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/SENSORS/MLX90614.py` & `eyes17-1.0.9/eyes17/SENSORS/MLX90614.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/SENSORS/ComplementaryFilter.py` & `eyes17-1.0.9/eyes17/SENSORS/ComplementaryFilter.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/SENSORS/SHT21.py` & `eyes17-1.0.9/eyes17/SENSORS/SHT21.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/SENSORS/BH1750.py` & `eyes17-1.0.9/eyes17/SENSORS/BH1750.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/SENSORS/supported.py` & `eyes17-1.0.9/eyes17/SENSORS/supported.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/SENSORS/TSL2561.py` & `eyes17-1.0.9/eyes17/SENSORS/TSL2561.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/SENSORS/SSD1306.py` & `eyes17-1.0.9/eyes17/SENSORS/SSD1306.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/sensorlist.py` & `eyes17-1.0.9/eyes17/sensorlist.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/eyemath17.py` & `eyes17-1.0.9/eyes17/eyemath17.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17/commands_proto.py` & `eyes17-1.0.9/eyes17/commands_proto.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/PKG-INFO` & `eyes17-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyes17
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python package for ExpEYES17
 Home-page: https://github.com/csparkresearch/expeyes17
 Author: Jithin B.P
 Author-email: jithinbp@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/expeyes/expeyes-programs
 Project-URL: Read The Docs, https://expeyes.in
```

### Comparing `eyes17-1.0.8/eyes17GUI/RCtransient.py` & `eyes17-1.0.9/eyes17GUI/RCtransient.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/induction.py` & `eyes17-1.0.9/eyes17GUI/induction.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/eyes.py` & `eyes17-1.0.9/eyes17GUI/eyes17/eyes.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/Peripherals.py` & `eyes17-1.0.9/eyes17GUI/eyes17/Peripherals.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/achan.py` & `eyes17-1.0.9/eyes17GUI/eyes17/achan.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/eyeplot17.py` & `eyes17-1.0.9/eyes17GUI/eyes17/eyeplot17.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/packet_handler.py` & `eyes17-1.0.9/eyes17GUI/eyes17/packet_handler.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/ADS1248.py` & `eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/ADS1248.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/AD9833.py` & `eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/AD9833.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/HMC5883L.py` & `eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/HMC5883L.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/MPU925x.py` & `eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/MPU925x.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/MPU6050.py` & `eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/MPU6050.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/MF522.py` & `eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/MF522.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/Kalman.py` & `eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/Kalman.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/BMP180.py` & `eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/BMP180.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/AD7718_class.py` & `eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/AD7718_class.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/ADS1115.py` & `eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/ADS1115.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/MLX90614.py` & `eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/MLX90614.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/ComplementaryFilter.py` & `eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/ComplementaryFilter.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/SHT21.py` & `eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/SHT21.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/BH1750.py` & `eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/BH1750.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/supported.py` & `eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/supported.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/TSL2561.py` & `eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/TSL2561.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/SENSORS/SSD1306.py` & `eyes17-1.0.9/eyes17GUI/eyes17/SENSORS/SSD1306.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/sensorlist.py` & `eyes17-1.0.9/eyes17GUI/eyes17/sensorlist.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/eyemath17.py` & `eyes17-1.0.9/eyes17GUI/eyes17/eyemath17.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/eyes17/commands_proto.py` & `eyes17-1.0.9/eyes17GUI/eyes17/commands_proto.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/sr04dist_fft.py` & `eyes17-1.0.9/eyes17GUI/sr04dist_fft.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/RLCsteadystate.py` & `eyes17-1.0.9/eyes17GUI/RLCsteadystate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8; mode: python; indent-tabs-mode: t; tab-width:4 -*-
 import sys, time, math, os.path
 from . import utils
 
 from .QtVersion import *
 
-import sys, time, utils, math
+import sys, time, math
 import pyqtgraph as pg
 import numpy as np
 from . eyes17 import eyemath17 as em
 
 
 class Expt(QWidget):
 	TIMER = 50
```

### Comparing `eyes17-1.0.8/eyes17GUI/plotIV.py` & `eyes17-1.0.9/eyes17GUI/plotIV.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/pt100.py` & `eyes17-1.0.9/eyes17GUI/pt100.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/npnCEout.py` & `eyes17-1.0.9/eyes17GUI/npnCEout.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/tof.py` & `eyes17-1.0.9/eyes17GUI/tof.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/sr04dist.py` & `eyes17-1.0.9/eyes17GUI/sr04dist.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/logger.py` & `eyes17-1.0.9/eyes17GUI/logger.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/MPU6050.py` & `eyes17-1.0.9/eyes17GUI/MPU6050.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/drivenRodPendulum.py` & `eyes17-1.0.9/eyes17GUI/drivenRodPendulum.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/terminal.py` & `eyes17-1.0.9/eyes17GUI/terminal.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/pendulumVelocity.py` & `eyes17-1.0.9/eyes17GUI/pendulumVelocity.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/main.py` & `eyes17-1.0.9/eyes17GUI/main.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/soundBeats.py` & `eyes17-1.0.9/eyes17GUI/soundBeats.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/XYplot.py` & `eyes17-1.0.9/eyes17GUI/XYplot.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/advanced_logger.py` & `eyes17-1.0.9/eyes17GUI/advanced_logger.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/dust_sensor.py` & `eyes17-1.0.9/eyes17GUI/dust_sensor.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/RLCtransient.py` & `eyes17-1.0.9/eyes17GUI/RLCtransient.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/numpy_help.py` & `eyes17-1.0.9/eyes17GUI/numpy_help.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/utils.py` & `eyes17-1.0.9/eyes17GUI/utils.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/BHCurve.py` & `eyes17-1.0.9/eyes17GUI/BHCurve.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/lightsensorlogger.py` & `eyes17-1.0.9/eyes17GUI/lightsensorlogger.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/driven-pendulum.py` & `eyes17-1.0.9/eyes17GUI/driven-pendulum.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/RLtransient.py` & `eyes17-1.0.9/eyes17GUI/RLtransient.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/i2cLogger.py` & `eyes17-1.0.9/eyes17GUI/i2cLogger.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/QtVersion.py` & `eyes17-1.0.9/eyes17GUI/QtVersion.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/pnpCEout.py` & `eyes17-1.0.9/eyes17GUI/pnpCEout.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/soundFreqResp.py` & `eyes17-1.0.9/eyes17GUI/soundFreqResp.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/XYplot2.py` & `eyes17-1.0.9/eyes17GUI/XYplot2.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/rodPendulum.py` & `eyes17-1.0.9/eyes17GUI/rodPendulum.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/diodeIV.py` & `eyes17-1.0.9/eyes17GUI/diodeIV.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/layouts/oscilloscope_widget.py` & `eyes17-1.0.9/eyes17GUI/layouts/oscilloscope_widget.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/layouts/ui_dio_robot.py` & `eyes17-1.0.9/eyes17GUI/layouts/ui_dio_robot.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/layouts/advancedLoggerTools.py` & `eyes17-1.0.9/eyes17GUI/layouts/advancedLoggerTools.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/layouts/ui_scope.py` & `eyes17-1.0.9/eyes17GUI/layouts/ui_scope.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/layouts/ui_dio_pwm.py` & `eyes17-1.0.9/eyes17GUI/layouts/ui_dio_pwm.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/layouts/ui_newtonslaws.py` & `eyes17-1.0.9/eyes17GUI/layouts/ui_newtonslaws.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/layouts/res_rc.py` & `eyes17-1.0.9/eyes17GUI/layouts/res_rc.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/layouts/ui_advancedLogger.py` & `eyes17-1.0.9/eyes17GUI/layouts/ui_advancedLogger.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/layouts/ui_dio_sensor.py` & `eyes17-1.0.9/eyes17GUI/layouts/ui_dio_sensor.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/layouts/ui_dio_control.py` & `eyes17-1.0.9/eyes17GUI/layouts/ui_dio_control.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/layouts/ui_scope_layout.py` & `eyes17-1.0.9/eyes17GUI/layouts/ui_scope_layout.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/layouts/gauge.py` & `eyes17-1.0.9/eyes17GUI/layouts/gauge.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/layouts/ui_miniScope.py` & `eyes17-1.0.9/eyes17GUI/layouts/ui_miniScope.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/layouts/ui_inputSelector.py` & `eyes17-1.0.9/eyes17GUI/layouts/ui_inputSelector.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/soundVelocity.py` & `eyes17-1.0.9/eyes17GUI/soundVelocity.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/pythonSyntax.py` & `eyes17-1.0.9/eyes17GUI/pythonSyntax.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/scope2.py` & `eyes17-1.0.9/eyes17GUI/scope2.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/editor.py` & `eyes17-1.0.9/eyes17GUI/editor.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/filterCircuit.py` & `eyes17-1.0.9/eyes17GUI/filterCircuit.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/scope.py` & `eyes17-1.0.9/eyes17GUI/scope.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/eyes17GUI/newtons_laws.py` & `eyes17-1.0.9/eyes17GUI/newtons_laws.py`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/resources/sispmctl.conf` & `eyes17-1.0.9/resources/sispmctl.conf`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/resources/99-eyes17-pip.rules` & `eyes17-1.0.9/resources/99-eyes17-pip.rules`

 * *Files identical despite different names*

### Comparing `eyes17-1.0.8/setup.py` & `eyes17-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 		make_rules()
 
 #if 'sdist' not in sys.argv:
 atexit.register(make_rules)
 
 setuptools.setup(
     name="eyes17",
-    version="1.0.8",
+    version="1.0.9",
     install_requires=requirements,
     author="Jithin B.P",
     author_email="jithinbp@gmail.com",
     description="Python package for ExpEYES17",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/csparkresearch/expeyes17",
```

### Comparing `eyes17-1.0.8/eyes17.egg-info/PKG-INFO` & `eyes17-1.0.9/eyes17.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyes17
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python package for ExpEYES17
 Home-page: https://github.com/csparkresearch/expeyes17
 Author: Jithin B.P
 Author-email: jithinbp@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/expeyes/expeyes-programs
 Project-URL: Read The Docs, https://expeyes.in
```

### Comparing `eyes17-1.0.8/eyes17.egg-info/SOURCES.txt` & `eyes17-1.0.9/eyes17.egg-info/SOURCES.txt`

 * *Files identical despite different names*

