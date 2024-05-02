# Comparing `tmp/hhd-2.6.4.tar.gz` & `tmp/hhd-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhd-2.6.4.tar", last modified: Mon Apr 15 15:46:17 2024, max compression
+gzip compressed data, was "hhd-2.6.5.tar", last modified: Thu May  2 19:52:42 2024, max compression
```

## Comparing `hhd-2.6.4.tar` & `hhd-2.6.5.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.696524 hhd-2.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-15 15:46:10.000000 hhd-2.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-15 15:46:10.000000 hhd-2.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    22812 2024-04-15 15:46:17.692524 hhd-2.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-15 15:46:10.000000 hhd-2.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)    22000 2024-04-15 15:46:10.000000 hhd-2.6.4/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:46:17.696524 hhd-2.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.668524 hhd-2.6.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.676524 hhd-2.6.4/src/hhd/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26086 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.676524 hhd-2.6.4/src/hhd/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/contrib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/contrib/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/contrib/gs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/contrib/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/contrib/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.680524 hhd-2.6.4/src/hhd/controller/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37040 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/controller/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/controller/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.680524 hhd-2.6.4/src/hhd/controller/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/controller/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/controller/lib/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/controller/lib/hid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/controller/lib/hide.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/controller/lib/ioctl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7958 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/controller/lib/uhid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.680524 hhd-2.6.4/src/hhd/controller/physical/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/controller/physical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21658 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/controller/physical/evdev.py
--rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/controller/physical/hidraw.py
--rw-r--r--   0 runner    (1001) docker     (127)    20696 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/controller/physical/imu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/controller/physical/rgb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.680524 hhd-2.6.4/src/hhd/controller/virtual/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/controller/virtual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.680524 hhd-2.6.4/src/hhd/controller/virtual/dualsense/
--rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/controller/virtual/dualsense/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29110 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/controller/virtual/dualsense/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.680524 hhd-2.6.4/src/hhd/controller/virtual/sd/
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/controller/virtual/sd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/controller/virtual/sd/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.680524 hhd-2.6.4/src/hhd/controller/virtual/uinput/
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/controller/virtual/uinput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/controller/virtual/uinput/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.672524 hhd-2.6.4/src/hhd/device/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.684524 hhd-2.6.4/src/hhd/device/generic/
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/generic/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/generic/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/generic/controllers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.668524 hhd-2.6.4/src/hhd/device/gpd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.684524 hhd-2.6.4/src/hhd/device/gpd/win/
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/gpd/win/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/gpd/win/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/gpd/win/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/gpd/win/controllers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.684524 hhd-2.6.4/src/hhd/device/legion_go/
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/legion_go/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17892 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/legion_go/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/legion_go/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/legion_go/controllers.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/legion_go/gyro_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/legion_go/hid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.684524 hhd-2.6.4/src/hhd/device/orange_pi/
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/orange_pi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/orange_pi/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/orange_pi/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/orange_pi/controllers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.688524 hhd-2.6.4/src/hhd/device/rog_ally/
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/rog_ally/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10604 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/rog_ally/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/rog_ally/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/rog_ally/controllers.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/device/rog_ally/hid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.688524 hhd-2.6.4/src/hhd/http/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/http/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/http/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/http/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.688524 hhd-2.6.4/src/hhd/http/static/
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/http/static/index.js
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/http/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.688524 hhd-2.6.4/src/hhd/i18n/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/i18n/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.672524 hhd-2.6.4/src/hhd/i18n/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.688524 hhd-2.6.4/src/hhd/i18n/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-04-15 15:46:15.000000 hhd-2.6.4/src/hhd/i18n/pt/LC_MESSAGES/adjustor.mo
--rw-r--r--   0 runner    (1001) docker     (127)    22062 2024-04-15 15:46:15.000000 hhd-2.6.4/src/hhd/i18n/pt/LC_MESSAGES/hhd.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.672524 hhd-2.6.4/src/hhd/i18n/zh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.688524 hhd-2.6.4/src/hhd/i18n/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-04-15 15:46:15.000000 hhd-2.6.4/src/hhd/i18n/zh/LC_MESSAGES/adjustor.mo
--rw-r--r--   0 runner    (1001) docker     (127)    16357 2024-04-15 15:46:15.000000 hhd-2.6.4/src/hhd/i18n/zh/LC_MESSAGES/hhd.mo
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.688524 hhd-2.6.4/src/hhd/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.692524 hhd-2.6.4/src/hhd/plugins/display/
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/display/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/gyro.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/outputs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.692524 hhd-2.6.4/src/hhd/plugins/overlay/
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/overlay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/overlay/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/overlay/controllers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/overlay/overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/overlay/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/overlay/x11.py
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.692524 hhd-2.6.4/src/hhd/plugins/powerbutton/
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/powerbutton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/powerbutton/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/powerbutton/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/powerbutton/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)    22188 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/touchpad.yml
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/plugins/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/sections.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-15 15:46:10.000000 hhd-2.6.4/src/hhd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.692524 hhd-2.6.4/src/hhd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22812 2024-04-15 15:46:17.000000 hhd-2.6.4/src/hhd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-15 15:46:17.000000 hhd-2.6.4/src/hhd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:46:17.000000 hhd-2.6.4/src/hhd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-15 15:46:17.000000 hhd-2.6.4/src/hhd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-15 15:46:17.000000 hhd-2.6.4/src/hhd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-15 15:46:17.000000 hhd-2.6.4/src/hhd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.672524 hhd-2.6.4/usr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.672524 hhd-2.6.4/usr/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.692524 hhd-2.6.4/usr/lib/modules-load.d/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-15 15:46:10.000000 hhd-2.6.4/usr/lib/modules-load.d/hhd-user.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.672524 hhd-2.6.4/usr/lib/systemd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.692524 hhd-2.6.4/usr/lib/systemd/system/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-15 15:46:10.000000 hhd-2.6.4/usr/lib/systemd/system/hhd@.service
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-15 15:46:10.000000 hhd-2.6.4/usr/lib/systemd/system/hhd_local@.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.692524 hhd-2.6.4/usr/lib/systemd/user/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-15 15:46:10.000000 hhd-2.6.4/usr/lib/systemd/user/hhd-user.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.672524 hhd-2.6.4/usr/lib/udev/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.692524 hhd-2.6.4/usr/lib/udev/hwdb.d/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-15 15:46:10.000000 hhd-2.6.4/usr/lib/udev/hwdb.d/83-hhd.hwdb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:17.692524 hhd-2.6.4/usr/lib/udev/rules.d/
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-15 15:46:10.000000 hhd-2.6.4/usr/lib/udev/rules.d/83-hhd-user.rules
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-15 15:46:10.000000 hhd-2.6.4/usr/lib/udev/rules.d/83-hhd.rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.631867 hhd-2.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-02 19:52:31.000000 hhd-2.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-02 19:52:31.000000 hhd-2.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    22812 2024-05-02 19:52:42.631867 hhd-2.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-02 19:52:31.000000 hhd-2.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    22000 2024-05-02 19:52:31.000000 hhd-2.6.5/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:52:42.631867 hhd-2.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.611867 hhd-2.6.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.615867 hhd-2.6.5/src/hhd/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26086 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.619867 hhd-2.6.5/src/hhd/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/contrib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/contrib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/contrib/gs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/contrib/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/contrib/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.619867 hhd-2.6.5/src/hhd/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37047 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.619867 hhd-2.6.5/src/hhd/controller/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/lib/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/lib/hid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/lib/hide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/lib/ioctl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7958 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/lib/uhid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.619867 hhd-2.6.5/src/hhd/controller/physical/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/physical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21658 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/physical/evdev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/physical/hidraw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20696 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/physical/imu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/physical/rgb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.619867 hhd-2.6.5/src/hhd/controller/virtual/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/virtual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.619867 hhd-2.6.5/src/hhd/controller/virtual/dualsense/
+-rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/virtual/dualsense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29110 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/virtual/dualsense/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.619867 hhd-2.6.5/src/hhd/controller/virtual/sd/
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/virtual/sd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/virtual/sd/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.619867 hhd-2.6.5/src/hhd/controller/virtual/uinput/
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/virtual/uinput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/virtual/uinput/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.611867 hhd-2.6.5/src/hhd/device/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.623867 hhd-2.6.5/src/hhd/device/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/generic/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/generic/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/generic/controllers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.611867 hhd-2.6.5/src/hhd/device/gpd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.623867 hhd-2.6.5/src/hhd/device/gpd/win/
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/gpd/win/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/gpd/win/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/gpd/win/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/gpd/win/controllers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.623867 hhd-2.6.5/src/hhd/device/legion_go/
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/legion_go/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17892 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/legion_go/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/legion_go/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/legion_go/controllers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/legion_go/gyro_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/legion_go/hid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.623867 hhd-2.6.5/src/hhd/device/orange_pi/
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/orange_pi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/orange_pi/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/orange_pi/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/orange_pi/controllers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.623867 hhd-2.6.5/src/hhd/device/rog_ally/
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/rog_ally/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10604 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/rog_ally/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/rog_ally/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/rog_ally/controllers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/rog_ally/hid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.623867 hhd-2.6.5/src/hhd/http/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/http/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/http/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/http/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.627867 hhd-2.6.5/src/hhd/http/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/http/static/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/http/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.627867 hhd-2.6.5/src/hhd/i18n/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/i18n/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.611867 hhd-2.6.5/src/hhd/i18n/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.627867 hhd-2.6.5/src/hhd/i18n/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-05-02 19:52:39.000000 hhd-2.6.5/src/hhd/i18n/pt/LC_MESSAGES/adjustor.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    22062 2024-05-02 19:52:39.000000 hhd-2.6.5/src/hhd/i18n/pt/LC_MESSAGES/hhd.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.611867 hhd-2.6.5/src/hhd/i18n/zh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.627867 hhd-2.6.5/src/hhd/i18n/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-05-02 19:52:39.000000 hhd-2.6.5/src/hhd/i18n/zh/LC_MESSAGES/adjustor.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    16357 2024-05-02 19:52:39.000000 hhd-2.6.5/src/hhd/i18n/zh/LC_MESSAGES/hhd.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.627867 hhd-2.6.5/src/hhd/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.627867 hhd-2.6.5/src/hhd/plugins/display/
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/display/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/gyro.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/outputs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.631867 hhd-2.6.5/src/hhd/plugins/overlay/
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/overlay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/overlay/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/overlay/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/overlay/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/overlay/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    13232 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/overlay/x11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.631867 hhd-2.6.5/src/hhd/plugins/powerbutton/
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/powerbutton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/powerbutton/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/powerbutton/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/powerbutton/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    22188 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/touchpad.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/sections.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.631867 hhd-2.6.5/src/hhd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22812 2024-05-02 19:52:42.000000 hhd-2.6.5/src/hhd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-02 19:52:42.000000 hhd-2.6.5/src/hhd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:52:42.000000 hhd-2.6.5/src/hhd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-02 19:52:42.000000 hhd-2.6.5/src/hhd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-02 19:52:42.000000 hhd-2.6.5/src/hhd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 19:52:42.000000 hhd-2.6.5/src/hhd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.611867 hhd-2.6.5/usr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.615867 hhd-2.6.5/usr/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.631867 hhd-2.6.5/usr/lib/modules-load.d/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 19:52:31.000000 hhd-2.6.5/usr/lib/modules-load.d/hhd-user.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.615867 hhd-2.6.5/usr/lib/systemd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.631867 hhd-2.6.5/usr/lib/systemd/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-02 19:52:31.000000 hhd-2.6.5/usr/lib/systemd/system/hhd@.service
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 19:52:31.000000 hhd-2.6.5/usr/lib/systemd/system/hhd_local@.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.631867 hhd-2.6.5/usr/lib/systemd/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-02 19:52:31.000000 hhd-2.6.5/usr/lib/systemd/user/hhd-user.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.615867 hhd-2.6.5/usr/lib/udev/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.631867 hhd-2.6.5/usr/lib/udev/hwdb.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-02 19:52:31.000000 hhd-2.6.5/usr/lib/udev/hwdb.d/83-hhd.hwdb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.631867 hhd-2.6.5/usr/lib/udev/rules.d/
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-02 19:52:31.000000 hhd-2.6.5/usr/lib/udev/rules.d/83-hhd-user.rules
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-02 19:52:31.000000 hhd-2.6.5/usr/lib/udev/rules.d/83-hhd.rules
```

### Comparing `hhd-2.6.4/LICENSE` & `hhd-2.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/PKG-INFO` & `hhd-2.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhd
-Version: 2.6.4
+Version: 2.6.5
 Summary: Handheld Daemon, a tool for configuring handheld devices.
 Author-email: Kapenekakis Antheas <pypi@antheas.dev>
 Project-URL: Homepage, https://github.com/hhd-dev/hhd
 Project-URL: Bug Tracker, https://github.com/hhd-dev/hhd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `hhd-2.6.4/pyproject.toml` & `hhd-2.6.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hhd"
-version = "2.6.4"
+version = "2.6.5"
 authors = [
   { name="Kapenekakis Antheas", email="pypi@antheas.dev" },
 ]
 description = "Handheld Daemon, a tool for configuring handheld devices."
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `hhd-2.6.4/readme.md` & `hhd-2.6.5/readme.md`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/__main__.py` & `hhd-2.6.5/src/hhd/__main__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/contrib/dev.py` & `hhd-2.6.5/src/hhd/contrib/dev.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/contrib/gs.py` & `hhd-2.6.5/src/hhd/contrib/gs.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/contrib/i18n.py` & `hhd-2.6.5/src/hhd/contrib/i18n.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/contrib/main.py` & `hhd-2.6.5/src/hhd/contrib/main.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/controller/__init__.py` & `hhd-2.6.5/src/hhd/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/controller/base.py` & `hhd-2.6.5/src/hhd/controller/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
     def __init__(self, ctx=None) -> None:
         self.intercept_lock = RLock()
         self._intercept = None
         self._controller_cb = None
         self._qam_cb = None
         self.ctx = ctx
-        self.use_legacy_qam = bool(os.environ.get("HHD_QAM_LEGACY", None))
+        self.use_legacy_qam = not bool(os.environ.get("HHD_QAM_GAMESCOPE", None))
 
     def send_qam(self):
         with self.intercept_lock:
             if self.use_legacy_qam:
                 return False
             if self._qam_cb:
                 return self._qam_cb()
```

### Comparing `hhd-2.6.4/src/hhd/controller/const.py` & `hhd-2.6.5/src/hhd/controller/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/controller/lib/common.py` & `hhd-2.6.5/src/hhd/controller/lib/common.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/controller/lib/hid.py` & `hhd-2.6.5/src/hhd/controller/lib/hid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/controller/lib/hide.py` & `hhd-2.6.5/src/hhd/controller/lib/hide.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/controller/lib/ioctl.py` & `hhd-2.6.5/src/hhd/controller/lib/ioctl.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/controller/lib/uhid.py` & `hhd-2.6.5/src/hhd/controller/lib/uhid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/controller/physical/evdev.py` & `hhd-2.6.5/src/hhd/controller/physical/evdev.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/controller/physical/hidraw.py` & `hhd-2.6.5/src/hhd/controller/physical/hidraw.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/controller/physical/imu.py` & `hhd-2.6.5/src/hhd/controller/physical/imu.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/controller/physical/rgb.py` & `hhd-2.6.5/src/hhd/controller/physical/rgb.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/controller/virtual/dualsense/__init__.py` & `hhd-2.6.5/src/hhd/controller/virtual/dualsense/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/controller/virtual/dualsense/const.py` & `hhd-2.6.5/src/hhd/controller/virtual/dualsense/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/controller/virtual/sd/__init__.py` & `hhd-2.6.5/src/hhd/controller/virtual/sd/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/controller/virtual/sd/const.py` & `hhd-2.6.5/src/hhd/controller/virtual/sd/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/controller/virtual/uinput/__init__.py` & `hhd-2.6.5/src/hhd/controller/virtual/uinput/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/controller/virtual/uinput/const.py` & `hhd-2.6.5/src/hhd/controller/virtual/uinput/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/device/generic/__init__.py` & `hhd-2.6.5/src/hhd/device/generic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,16 +123,16 @@
         if vendor == "ayn":
             return [GenericControllersPlugin(dmi, get_default_config(dmi, "AYN"))]
     except Exception:
         pass
 
     # Fallback to chassis vendor for aya
     try:
-        with open("/sys/class/dmi/id/board_vendor") as f:
+        with open("/sys/devices/virtual/dmi/id/sys_vendor") as f:
             vendor = f.read().lower().strip()
 
-        if "ayaneo" in vendor:
+        if "aya" in vendor:
             return [GenericControllersPlugin(dmi, get_default_config(dmi, "AYA"))]
     except Exception:
         return []
 
     return []
```

### Comparing `hhd-2.6.4/src/hhd/device/generic/base.py` & `hhd-2.6.5/src/hhd/device/generic/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/device/generic/const.py` & `hhd-2.6.5/src/hhd/device/generic/const.py`

 * *Files 20% similar despite different names*

```diff
@@ -123,14 +123,19 @@
     "NEXT Pro": {"name": "AYANEO NEXT Pro", **AYA_DEFAULT_CONF},
     "NEXT": {"name": "AYANEO NEXT", **AYA_DEFAULT_CONF},
     "SLIDE": {
         "name": "AYANEO SLIDE",
         **AYA_DEFAULT_CONF,
         "mapping": gen_gyro_state("z", False, "x", False, "y", False),
     },
+    "AYA NEO FOUNDER": {"name": "AYA NEO FOUNDER", **AYA_DEFAULT_CONF},
+    "AYA NEO 2021": {"name": "AYA NEO 2021", **AYA_DEFAULT_CONF},
+    "AYANEO 2021": {"name": "AYANEO 2021", **AYA_DEFAULT_CONF},
+    "AYANEO 2021 Pro": {"name": "AYANEO 2021 Pro", **AYA_DEFAULT_CONF},
+    "AYANEO 2021 Pro Retro Power": {"name": "AYANEO 2021 Pro Retro Power", **AYA_DEFAULT_CONF},
 }
 
 
 def get_default_config(product_name: str, manufacturer: str):
     out = {
         "name": product_name,
         "manufacturer": manufacturer,
```

### Comparing `hhd-2.6.4/src/hhd/device/generic/controllers.yml` & `hhd-2.6.5/src/hhd/device/generic/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/device/gpd/win/__init__.py` & `hhd-2.6.5/src/hhd/device/gpd/win/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from hhd.controller.lib.hid import enumerate_unique
 
 from .const import GPD_WIN_MAX_2_2023_MAPPINGS, GPD_WIN_DEFAULT_MAPPINGS
 
 GPD_CONFS = {
     "G1618-04": {"name": "GPD Win 4", "hrtimer": True},
     "G1617-01": {"name": "GPD Win Mini", "touchpad": True},
-    # TODO: GPD Win Max has multiple product names, switch to partial match
     "G1619-04": {
         "name": "GPD Win Max 2 2023 (04)",
         "hrtimer": True,
         "touchpad": True,
         "mapping": GPD_WIN_MAX_2_2023_MAPPINGS,
     },
     "G1619-05": {
@@ -140,16 +139,16 @@
     # Match just product number, should be enough for now
     with open("/sys/devices/virtual/dmi/id/product_name") as f:
         dmi = f.read().strip()
         dconf = GPD_CONFS.get(dmi, None)
         if dconf:
             return [GpdWinControllersPlugin(dmi, dconf)]
 
-    # Perform dmi agnostic detection
-    GPD_WIN_VID = 0x2F24
-    GPD_WIN_PID = 0x0135
     try:
-        if len(enumerate_unique(GPD_WIN_VID, GPD_WIN_PID)):
+        with open("/sys/devices/virtual/dmi/id/sys_vendor") as f:
+            vendor = f.read().strip().lower()
+        if vendor == "gpd":
             return [GpdWinControllersPlugin(dmi, get_default_config(dmi))]
     except Exception:
         pass
+
     return []
```

### Comparing `hhd-2.6.4/src/hhd/device/gpd/win/base.py` & `hhd-2.6.5/src/hhd/device/gpd/win/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/device/gpd/win/const.py` & `hhd-2.6.5/src/hhd/device/gpd/win/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/device/gpd/win/controllers.yml` & `hhd-2.6.5/src/hhd/device/gpd/win/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/device/legion_go/__init__.py` & `hhd-2.6.5/src/hhd/device/legion_go/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/device/legion_go/base.py` & `hhd-2.6.5/src/hhd/device/legion_go/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/device/legion_go/const.py` & `hhd-2.6.5/src/hhd/device/legion_go/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/device/legion_go/controllers.yml` & `hhd-2.6.5/src/hhd/device/legion_go/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/device/legion_go/gyro_fix.py` & `hhd-2.6.5/src/hhd/device/legion_go/gyro_fix.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/device/legion_go/hid.py` & `hhd-2.6.5/src/hhd/device/legion_go/hid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/device/orange_pi/__init__.py` & `hhd-2.6.5/src/hhd/device/orange_pi/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/device/orange_pi/base.py` & `hhd-2.6.5/src/hhd/device/orange_pi/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/device/orange_pi/const.py` & `hhd-2.6.5/src/hhd/device/orange_pi/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/device/orange_pi/controllers.yml` & `hhd-2.6.5/src/hhd/device/orange_pi/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/device/rog_ally/__init__.py` & `hhd-2.6.5/src/hhd/device/rog_ally/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/device/rog_ally/base.py` & `hhd-2.6.5/src/hhd/device/rog_ally/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/device/rog_ally/const.py` & `hhd-2.6.5/src/hhd/device/rog_ally/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/device/rog_ally/controllers.yml` & `hhd-2.6.5/src/hhd/device/rog_ally/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/device/rog_ally/hid.py` & `hhd-2.6.5/src/hhd/device/rog_ally/hid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/http/api.py` & `hhd-2.6.5/src/hhd/http/api.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/http/i18n.py` & `hhd-2.6.5/src/hhd/http/i18n.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/http/index.html` & `hhd-2.6.5/src/hhd/http/index.html`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/http/static/index.js` & `hhd-2.6.5/src/hhd/http/static/index.js`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/i18n/pt/LC_MESSAGES/adjustor.mo` & `hhd-2.6.5/src/hhd/i18n/pt/LC_MESSAGES/adjustor.mo`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/i18n/pt/LC_MESSAGES/hhd.mo` & `hhd-2.6.5/src/hhd/i18n/pt/LC_MESSAGES/hhd.mo`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/i18n/zh/LC_MESSAGES/adjustor.mo` & `hhd-2.6.5/src/hhd/i18n/zh/LC_MESSAGES/adjustor.mo`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/i18n/zh/LC_MESSAGES/hhd.mo` & `hhd-2.6.5/src/hhd/i18n/zh/LC_MESSAGES/hhd.mo`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/logging.py` & `hhd-2.6.5/src/hhd/logging.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/plugins/__init__.py` & `hhd-2.6.5/src/hhd/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/plugins/conf.py` & `hhd-2.6.5/src/hhd/plugins/conf.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/plugins/display/__init__.py` & `hhd-2.6.5/src/hhd/plugins/display/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/plugins/gyro.yml` & `hhd-2.6.5/src/hhd/plugins/gyro.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/plugins/inputs.py` & `hhd-2.6.5/src/hhd/plugins/inputs.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/plugins/outputs.py` & `hhd-2.6.5/src/hhd/plugins/outputs.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/plugins/outputs.yml` & `hhd-2.6.5/src/hhd/plugins/outputs.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/plugins/overlay/__init__.py` & `hhd-2.6.5/src/hhd/plugins/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/plugins/overlay/base.py` & `hhd-2.6.5/src/hhd/plugins/overlay/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/plugins/overlay/controllers.py` & `hhd-2.6.5/src/hhd/plugins/overlay/controllers.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/plugins/overlay/overlay.py` & `hhd-2.6.5/src/hhd/plugins/overlay/overlay.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/plugins/overlay/x11.py` & `hhd-2.6.5/src/hhd/plugins/overlay/x11.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 class CachedValues(NamedTuple):
     overlay: bool
     focus: bool
     notify: bool
     touch: int | None
 
 
+QAM_DELAY = 0.35
+
+
 class QamHandler:
 
     def __init__(
         self, ctx=None, force_disp: str | None = None, compat_send: bool = True
     ) -> None:
         self.disp = None
         self.ctx = ctx
@@ -69,14 +72,15 @@
             # if not steam:
             #     logger.info(f"Could not find Steam (?). Sending compatibility QAM.")
             #     return False
 
             fake_input(disp, X.KeyPress, KCTRL)  # , root=steam)
             fake_input(disp, X.KeyPress, KEY)  # , root=steam)
             disp.sync()
+            time.sleep(QAM_DELAY)
             fake_input(disp, X.KeyRelease, KCTRL)  # , root=steam)
             fake_input(disp, X.KeyRelease, KEY)  # , root=steam)
             disp.sync()
             logger.info(f"Sent QAM event directly to gamescope.")
             return True
         except Exception as e:
             logger.warning(
@@ -146,18 +150,19 @@
             except Exception:
                 pass
     finally:
         if old:
             restore_priviledge(old)
 
 
-def find_win(display: display.Display, win: list[str], atoms: list[str] = []):
+def find_wins(display: display.Display, win: list[str], atoms: list[str] = []):
     n = display.get_atom("WM_CLASS")
     a_ids = [display.get_atom(a, only_if_exists=True) for a in atoms]
 
+    wins = []
     for w in display.screen().root.query_tree().children:
         # Check the window has the proper class
         v = w.get_property(n, Xatom.STRING, 0, 50)
         if not v:
             continue
         if not v.value:
             continue
@@ -170,15 +175,21 @@
         classes = [c.decode() for c in v.value.split(b"\00") if c]
         found = True
         for val in win:
             if val not in classes:
                 found = False
 
         if found:
-            return w
+            wins.append(w)
+    return wins
+
+
+def find_win(display: display.Display, win: list[str], atoms: list[str] = []):
+    out = find_wins(display, win, atoms)
+    return out[0] if out else None
 
 
 def register_changes(display, win):
     win.change_attributes(event_mask=Xlib.X.PropertyChangeMask)
     display.flush()
     display.sync()
```

### Comparing `hhd-2.6.4/src/hhd/plugins/plugin.py` & `hhd-2.6.5/src/hhd/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/plugins/powerbutton/__init__.py` & `hhd-2.6.5/src/hhd/plugins/powerbutton/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/plugins/powerbutton/base.py` & `hhd-2.6.5/src/hhd/plugins/powerbutton/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/plugins/powerbutton/const.py` & `hhd-2.6.5/src/hhd/plugins/powerbutton/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/plugins/settings.py` & `hhd-2.6.5/src/hhd/plugins/settings.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/plugins/touchpad.yml` & `hhd-2.6.5/src/hhd/plugins/touchpad.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/plugins/utils.py` & `hhd-2.6.5/src/hhd/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/settings.yml` & `hhd-2.6.5/src/hhd/settings.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd/utils.py` & `hhd-2.6.5/src/hhd/utils.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/src/hhd.egg-info/PKG-INFO` & `hhd-2.6.5/src/hhd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhd
-Version: 2.6.4
+Version: 2.6.5
 Summary: Handheld Daemon, a tool for configuring handheld devices.
 Author-email: Kapenekakis Antheas <pypi@antheas.dev>
 Project-URL: Homepage, https://github.com/hhd-dev/hhd
 Project-URL: Bug Tracker, https://github.com/hhd-dev/hhd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `hhd-2.6.4/src/hhd.egg-info/SOURCES.txt` & `hhd-2.6.5/src/hhd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/usr/lib/udev/hwdb.d/83-hhd.hwdb` & `hhd-2.6.5/usr/lib/udev/hwdb.d/83-hhd.hwdb`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/usr/lib/udev/rules.d/83-hhd-user.rules` & `hhd-2.6.5/usr/lib/udev/rules.d/83-hhd-user.rules`

 * *Files identical despite different names*

### Comparing `hhd-2.6.4/usr/lib/udev/rules.d/83-hhd.rules` & `hhd-2.6.5/usr/lib/udev/rules.d/83-hhd.rules`

 * *Files identical despite different names*

