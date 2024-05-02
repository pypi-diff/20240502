# Comparing `tmp/ophyd_devices-0.9.1.tar.gz` & `tmp/ophyd_devices-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ophyd_devices-0.9.1.tar", last modified: Thu Nov  2 12:02:20 2023, max compression
+gzip compressed data, was "ophyd_devices-0.9.2.tar", last modified: Wed Nov  8 18:24:40 2023, max compression
```

## Comparing `ophyd_devices-0.9.1.tar` & `ophyd_devices-0.9.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 12:02:20.539377 ophyd_devices-0.9.1/
--rw-rw-rw-   0 root         (0) root         (0)     1511 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2890 2023-11-02 12:02:20.539377 ophyd_devices-0.9.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2345 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 12:02:20.533377 ophyd_devices-0.9.1/ophyd_devices/
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 12:02:20.533377 ophyd_devices-0.9.1/ophyd_devices/epics/
--rw-rw-rw-   0 root         (0) root         (0)     1898 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/epics/DeviceFactory.py
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/epics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 12:02:20.535377 ophyd_devices-0.9.1/ophyd_devices/epics/devices/
--rw-r--r--   0 root         (0) root         (0)    23601 2023-11-02 12:02:12.000000 ophyd_devices-0.9.1/ophyd_devices/epics/devices/DelayGeneratorDG645.py
--rw-rw-rw-   0 root         (0) root         (0)     1104 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/epics/devices/InsertionDevice.py
--rw-rw-rw-   0 root         (0) root         (0)     3809 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/epics/devices/SpmBase.py
--rw-r--r--   0 root         (0) root         (0)      301 2023-11-02 12:02:12.000000 ophyd_devices-0.9.1/ophyd_devices/epics/devices/Test.py
--rw-r--r--   0 root         (0) root         (0)    12420 2023-11-02 12:02:12.000000 ophyd_devices-0.9.1/ophyd_devices/epics/devices/X07MADevices.py
--rw-rw-rw-   0 root         (0) root         (0)     5233 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/epics/devices/XbpmBase.py
--rw-r--r--   0 root         (0) root         (0)      860 2023-11-02 12:02:12.000000 ophyd_devices-0.9.1/ophyd_devices/epics/devices/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2537 2023-11-02 12:02:12.000000 ophyd_devices-0.9.1/ophyd_devices/epics/devices/bec_scaninfo_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)      832 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/epics/devices/cSaxsVirtualMotors.py
--rw-r--r--   0 root         (0) root         (0)    17742 2023-11-02 12:02:12.000000 ophyd_devices-0.9.1/ophyd_devices/epics/devices/eiger9m_csaxs.py
--rw-r--r--   0 root         (0) root         (0)     1934 2023-11-02 12:02:12.000000 ophyd_devices-0.9.1/ophyd_devices/epics/devices/epics_motor_ex.py
--rw-r--r--   0 root         (0) root         (0)    14813 2023-11-02 12:02:12.000000 ophyd_devices-0.9.1/ophyd_devices/epics/devices/falcon_csaxs.py
--rw-r--r--   0 root         (0) root         (0)    14650 2023-11-02 12:02:12.000000 ophyd_devices-0.9.1/ophyd_devices/epics/devices/mcs_csaxs.py
--rw-rw-rw-   0 root         (0) root         (0)     4440 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/epics/devices/mono_dccm.py
--rw-r--r--   0 root         (0) root         (0)    17255 2023-11-02 12:02:12.000000 ophyd_devices-0.9.1/ophyd_devices/epics/devices/pilatus_csaxs.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-11-02 12:02:12.000000 ophyd_devices-0.9.1/ophyd_devices/epics/devices/sequencer_x12sa.py
--rw-rw-rw-   0 root         (0) root         (0)     2173 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/epics/devices/slits.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/epics/devices/slsDetector.py
--rw-r--r--   0 root         (0) root         (0)     9183 2023-11-02 12:02:12.000000 ophyd_devices-0.9.1/ophyd_devices/epics/devices/specMotors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 12:02:20.536377 ophyd_devices-0.9.1/ophyd_devices/galil/
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/galil/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19024 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/galil/galil_ophyd.py
--rw-r--r--   0 root         (0) root         (0)    25525 2023-11-02 12:02:12.000000 ophyd_devices-0.9.1/ophyd_devices/galil/sgalil_ophyd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 12:02:20.536377 ophyd_devices-0.9.1/ophyd_devices/npoint/
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/npoint/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16790 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/npoint/npoint.py
--rw-rw-rw-   0 root         (0) root         (0)    13172 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/npoint/npoint_ophyd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 12:02:20.536377 ophyd_devices-0.9.1/ophyd_devices/rt_lamni/
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/rt_lamni/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    31617 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/rt_lamni/rt_lamni_ophyd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 12:02:20.537377 ophyd_devices-0.9.1/ophyd_devices/sim/
--rw-rw-rw-   0 root         (0) root         (0)      122 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/sim/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    28937 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/sim/sim.py
--rw-r--r--   0 root         (0) root         (0)    13683 2023-11-02 12:02:12.000000 ophyd_devices-0.9.1/ophyd_devices/sim/sim_xtreme.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 12:02:20.538377 ophyd_devices-0.9.1/ophyd_devices/smaract/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/smaract/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/smaract/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)    19903 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/smaract/smaract_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     5212 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/smaract/smaract_errors.py
--rw-rw-rw-   0 root         (0) root         (0)    10338 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/smaract/smaract_ophyd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 12:02:20.538377 ophyd_devices-0.9.1/ophyd_devices/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-02 12:01:57.000000 ophyd_devices-0.9.1/ophyd_devices/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3845 2023-11-02 12:02:12.000000 ophyd_devices-0.9.1/ophyd_devices/utils/bec_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3269 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/utils/controller.py
--rw-rw-rw-   0 root         (0) root         (0)      457 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/utils/re_test.py
--rw-rw-rw-   0 root         (0) root         (0)     7014 2023-08-14 01:04:07.000000 ophyd_devices-0.9.1/ophyd_devices/utils/socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 12:02:20.539377 ophyd_devices-0.9.1/ophyd_devices.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2890 2023-11-02 12:02:20.000000 ophyd_devices-0.9.1/ophyd_devices.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1949 2023-11-02 12:02:20.000000 ophyd_devices-0.9.1/ophyd_devices.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-02 12:02:20.000000 ophyd_devices-0.9.1/ophyd_devices.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-11-02 12:02:20.000000 ophyd_devices-0.9.1/ophyd_devices.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-11-02 12:02:20.000000 ophyd_devices-0.9.1/ophyd_devices.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      651 2023-11-02 12:02:20.540377 ophyd_devices-0.9.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      432 2023-11-02 12:02:18.000000 ophyd_devices-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 18:24:40.705129 ophyd_devices-0.9.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1511 2023-08-14 01:03:25.000000 ophyd_devices-0.9.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-11-08 18:24:40.705129 ophyd_devices-0.9.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2023-08-14 01:03:25.000000 ophyd_devices-0.9.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 18:24:40.702128 ophyd_devices-0.9.2/ophyd_devices/
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-08-14 01:03:25.000000 ophyd_devices-0.9.2/ophyd_devices/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 18:24:40.702128 ophyd_devices-0.9.2/ophyd_devices/epics/
+-rw-rw-rw-   0 root         (0) root         (0)     1898 2023-08-14 01:03:25.000000 ophyd_devices-0.9.2/ophyd_devices/epics/DeviceFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-08-14 01:03:25.000000 ophyd_devices-0.9.2/ophyd_devices/epics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 18:24:40.703128 ophyd_devices-0.9.2/ophyd_devices/epics/devices/
+-rw-r--r--   0 root         (0) root         (0)    23601 2023-10-31 18:01:12.000000 ophyd_devices-0.9.2/ophyd_devices/epics/devices/DelayGeneratorDG645.py
+-rw-rw-rw-   0 root         (0) root         (0)     1104 2023-08-14 01:03:25.000000 ophyd_devices-0.9.2/ophyd_devices/epics/devices/InsertionDevice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3809 2023-08-14 01:03:25.000000 ophyd_devices-0.9.2/ophyd_devices/epics/devices/SpmBase.py
+-rw-r--r--   0 root         (0) root         (0)      301 2023-10-31 18:01:12.000000 ophyd_devices-0.9.2/ophyd_devices/epics/devices/Test.py
+-rw-rw-rw-   0 root         (0) root         (0)    12420 2023-10-24 01:04:36.000000 ophyd_devices-0.9.2/ophyd_devices/epics/devices/X07MADevices.py
+-rw-rw-rw-   0 root         (0) root         (0)     5233 2023-08-14 01:03:25.000000 ophyd_devices-0.9.2/ophyd_devices/epics/devices/XbpmBase.py
+-rw-r--r--   0 root         (0) root         (0)      860 2023-11-08 18:24:31.000000 ophyd_devices-0.9.2/ophyd_devices/epics/devices/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4397 2023-11-08 18:24:31.000000 ophyd_devices-0.9.2/ophyd_devices/epics/devices/bec_scaninfo_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      832 2023-08-14 01:03:25.000000 ophyd_devices-0.9.2/ophyd_devices/epics/devices/cSaxsVirtualMotors.py
+-rw-r--r--   0 root         (0) root         (0)    19759 2023-11-08 18:24:31.000000 ophyd_devices-0.9.2/ophyd_devices/epics/devices/eiger9m_csaxs.py
+-rw-r--r--   0 root         (0) root         (0)     1934 2023-10-31 18:01:12.000000 ophyd_devices-0.9.2/ophyd_devices/epics/devices/epics_motor_ex.py
+-rw-rw-rw-   0 root         (0) root         (0)    14813 2023-11-08 01:03:35.000000 ophyd_devices-0.9.2/ophyd_devices/epics/devices/falcon_csaxs.py
+-rw-r--r--   0 root         (0) root         (0)    14650 2023-10-31 18:01:12.000000 ophyd_devices-0.9.2/ophyd_devices/epics/devices/mcs_csaxs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4440 2023-08-14 01:03:25.000000 ophyd_devices-0.9.2/ophyd_devices/epics/devices/mono_dccm.py
+-rw-r--r--   0 root         (0) root         (0)    19266 2023-11-08 18:24:31.000000 ophyd_devices-0.9.2/ophyd_devices/epics/devices/pilatus_csaxs.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-10-31 18:01:12.000000 ophyd_devices-0.9.2/ophyd_devices/epics/devices/sequencer_x12sa.py
+-rw-rw-rw-   0 root         (0) root         (0)     2173 2023-08-14 01:03:25.000000 ophyd_devices-0.9.2/ophyd_devices/epics/devices/slits.py
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2023-08-14 01:03:25.000000 ophyd_devices-0.9.2/ophyd_devices/epics/devices/slsDetector.py
+-rw-r--r--   0 root         (0) root         (0)     9183 2023-10-31 18:01:12.000000 ophyd_devices-0.9.2/ophyd_devices/epics/devices/specMotors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 18:24:40.704128 ophyd_devices-0.9.2/ophyd_devices/galil/
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-11-08 18:22:38.000000 ophyd_devices-0.9.2/ophyd_devices/galil/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19024 2023-11-08 18:22:38.000000 ophyd_devices-0.9.2/ophyd_devices/galil/galil_ophyd.py
+-rw-r--r--   0 root         (0) root         (0)    25525 2023-10-31 18:01:12.000000 ophyd_devices-0.9.2/ophyd_devices/galil/sgalil_ophyd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 18:24:40.704128 ophyd_devices-0.9.2/ophyd_devices/npoint/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-08-14 01:03:25.000000 ophyd_devices-0.9.2/ophyd_devices/npoint/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16790 2023-11-08 18:22:38.000000 ophyd_devices-0.9.2/ophyd_devices/npoint/npoint.py
+-rw-rw-rw-   0 root         (0) root         (0)    13172 2023-11-08 18:22:38.000000 ophyd_devices-0.9.2/ophyd_devices/npoint/npoint_ophyd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 18:24:40.704128 ophyd_devices-0.9.2/ophyd_devices/rt_lamni/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-08-14 01:03:25.000000 ophyd_devices-0.9.2/ophyd_devices/rt_lamni/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    31617 2023-08-14 01:03:25.000000 ophyd_devices-0.9.2/ophyd_devices/rt_lamni/rt_lamni_ophyd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 18:24:40.704128 ophyd_devices-0.9.2/ophyd_devices/sim/
+-rw-rw-rw-   0 root         (0) root         (0)      122 2023-08-14 01:03:25.000000 ophyd_devices-0.9.2/ophyd_devices/sim/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    28937 2023-08-14 01:03:25.000000 ophyd_devices-0.9.2/ophyd_devices/sim/sim.py
+-rw-rw-rw-   0 root         (0) root         (0)    13683 2023-11-08 01:03:35.000000 ophyd_devices-0.9.2/ophyd_devices/sim/sim_xtreme.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 18:24:40.705129 ophyd_devices-0.9.2/ophyd_devices/smaract/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-08-14 01:03:25.000000 ophyd_devices-0.9.2/ophyd_devices/smaract/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-08-14 01:03:25.000000 ophyd_devices-0.9.2/ophyd_devices/smaract/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)    19903 2023-11-08 18:22:38.000000 ophyd_devices-0.9.2/ophyd_devices/smaract/smaract_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     5212 2023-08-14 01:03:25.000000 ophyd_devices-0.9.2/ophyd_devices/smaract/smaract_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    10338 2023-11-08 18:22:38.000000 ophyd_devices-0.9.2/ophyd_devices/smaract/smaract_ophyd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 18:24:40.705129 ophyd_devices-0.9.2/ophyd_devices/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-08 18:24:17.000000 ophyd_devices-0.9.2/ophyd_devices/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5306 2023-11-08 18:24:31.000000 ophyd_devices-0.9.2/ophyd_devices/utils/bec_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3269 2023-11-08 18:22:38.000000 ophyd_devices-0.9.2/ophyd_devices/utils/controller.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-11-08 18:24:31.000000 ophyd_devices-0.9.2/ophyd_devices/utils/re_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     7014 2023-08-14 01:03:25.000000 ophyd_devices-0.9.2/ophyd_devices/utils/socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 18:24:40.705129 ophyd_devices-0.9.2/ophyd_devices.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-11-08 18:24:40.000000 ophyd_devices-0.9.2/ophyd_devices.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1949 2023-11-08 18:24:40.000000 ophyd_devices-0.9.2/ophyd_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-11-08 18:24:40.000000 ophyd_devices-0.9.2/ophyd_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-11-08 18:24:40.000000 ophyd_devices-0.9.2/ophyd_devices.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-11-08 18:24:40.000000 ophyd_devices-0.9.2/ophyd_devices.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      651 2023-11-08 18:24:40.706128 ophyd_devices-0.9.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-11-08 18:24:39.000000 ophyd_devices-0.9.2/setup.py
```

### Comparing `ophyd_devices-0.9.1/LICENSE` & `ophyd_devices-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/PKG-INFO` & `ophyd_devices-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ophyd_devices
-Version: 0.9.1
+Version: 0.9.2
 Summary: Custom device implementations based on the ophyd hardware abstraction layer
 Home-page: https://gitlab.psi.ch/bec/ophyd_devices
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/ophyd_devices/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ophyd_devices-0.9.1/README.md` & `ophyd_devices-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/epics/DeviceFactory.py` & `ophyd_devices-0.9.2/ophyd_devices/epics/DeviceFactory.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/epics/__init__.py` & `ophyd_devices-0.9.2/ophyd_devices/epics/__init__.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/epics/devices/DelayGeneratorDG645.py` & `ophyd_devices-0.9.2/ophyd_devices/epics/devices/DelayGeneratorDG645.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/epics/devices/InsertionDevice.py` & `ophyd_devices-0.9.2/ophyd_devices/epics/devices/InsertionDevice.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/epics/devices/SpmBase.py` & `ophyd_devices-0.9.2/ophyd_devices/epics/devices/SpmBase.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/epics/devices/X07MADevices.py` & `ophyd_devices-0.9.2/ophyd_devices/epics/devices/X07MADevices.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/epics/devices/XbpmBase.py` & `ophyd_devices-0.9.2/ophyd_devices/epics/devices/XbpmBase.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/epics/devices/__init__.py` & `ophyd_devices-0.9.2/ophyd_devices/epics/devices/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,11 +21,11 @@
 from ophyd import EpicsSignal, EpicsSignalRO, EpicsMotor
 from ophyd.sim import SynAxis, SynSignal, SynPeriodicSignal
 from ophyd.quadem import QuadEM
 
 # cSAXS
 from .epics_motor_ex import EpicsMotorEx
 from .mcs_csaxs import McsCsaxs
-from .eiger9m_csaxs import Eiger9mCsaxs
-from .pilatus_csaxs import PilatusCsaxs
+from .eiger9m_csaxs import Eiger9McSAXS
+from .pilatus_csaxs import PilatuscSAXS
 from .falcon_csaxs import FalconCsaxs
 from .DelayGeneratorDG645 import DelayGeneratorDG645
```

### Comparing `ophyd_devices-0.9.1/ophyd_devices/epics/devices/bec_scaninfo_mixin.py` & `ophyd_devices-0.9.2/ophyd_devices/epics/devices/bec_scaninfo_mixin.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,56 +2,118 @@
 
 from bec_lib.core import DeviceManagerBase, BECMessage, MessageEndpoints
 from bec_lib.core import bec_logger
 
 logger = bec_logger.logger
 
 
+class BECInfoMsgMock:
+    """Mock BECInfoMsg class
+
+    This class is used for mocking BECInfoMsg for testing purposes
+    """
+
+    def __init__(
+        self,
+        mockrid: str = "mockrid1111",
+        mockqueueid: str = "mockqueueID111",
+        scan_number: int = 1,
+        exp_time: float = 12e-3,
+        num_points: int = 500,
+        readout_time: float = 3e-3,
+        scan_type: str = "fly",
+        num_lines: int = 1,
+        frames_per_trigger: int = 1,
+    ) -> None:
+        self.mockrid = mockrid
+        self.mockqueueid = mockqueueid
+        self.scan_number = scan_number
+        self.exp_time = exp_time
+        self.num_points = num_points
+        self.readout_time = readout_time
+        self.scan_type = scan_type
+        self.num_lines = num_lines
+        self.frames_per_trigger = frames_per_trigger
+
+    def get_bec_info_msg(self) -> dict:
+        info_msg = {
+            "RID": self.mockrid,
+            "queueID": self.mockqueueid,
+            "scan_number": self.scan_number,
+            "exp_time": self.exp_time,
+            "num_points": self.num_points,
+            "readout_time": self.readout_time,
+            "scan_type": self.scan_type,
+            "num_lines": self.exp_time,
+            "frames_per_trigger": self.frames_per_trigger,
+        }
+
+        return info_msg
+
+
 class BecScaninfoMixin:
-    def __init__(self, device_manager: DeviceManagerBase = None, sim_mode=False) -> None:
+    """BecScaninfoMixin class
+
+    Args:
+        device_manager (DeviceManagerBase): DeviceManagerBase object
+        sim_mode (bool): Simulation mode flag
+        bec_info_msg (dict): BECInfoMsg object
+    Returns:
+        BecScaninfoMixin: BecScaninfoMixin object
+    """
+
+    def __init__(
+        self, device_manager: DeviceManagerBase = None, sim_mode: bool = False, bec_info_msg=None
+    ) -> None:
         self.device_manager = device_manager
         self.sim_mode = sim_mode
         self.scan_msg = None
         self.scanID = None
-        self.bec_info_msg = {
-            "RID": "mockrid",
-            "queueID": "mockqueuid",
-            "scan_number": 1,
-            "exp_time": 12e-3,
-            "num_points": 500,
-            "readout_time": 3e-3,
-            "scan_type": "fly",
-            "num_lines": 1,
-            "frames_per_trigger": 1,
-        }
+        if bec_info_msg is None:
+            infomsgmock = BECInfoMsgMock()
+            self.bec_info_msg = infomsgmock.get_bec_info_msg()
+        else:
+            self.bec_info_msg = bec_info_msg
 
     def get_bec_info_msg(self) -> None:
+        """Get BECInfoMsg object"""
         return self.bec_info_msg
 
     def change_config(self, bec_info_msg: dict) -> None:
+        """Change BECInfoMsg object"""
         self.bec_info_msg = bec_info_msg
 
     def _get_current_scan_msg(self) -> BECMessage.ScanStatusMessage:
+        """Get current scan message
+
+        Returns:
+            BECMessage.ScanStatusMessage: BECMessage.ScanStatusMessage object
+        """
         if not self.sim_mode:
             # TODO what if no scan info is there yet!
             msg = self.device_manager.producer.get(MessageEndpoints.scan_status())
             return BECMessage.ScanStatusMessage.loads(msg)
 
         return BECMessage.ScanStatusMessage(
             scanID="1",
             status={},
             info=self.bec_info_msg,
         )
 
     def get_username(self) -> str:
+        """Get username"""
         if not self.sim_mode:
             return self.device_manager.producer.get(MessageEndpoints.account()).decode()
         return os.getlogin()
 
     def load_scan_metadata(self) -> None:
+        """Load scan metadata
+
+        This function loads scan metadata from the current scan message
+        """
         self.scan_msg = scan_msg = self._get_current_scan_msg()
         logger.info(f"{self.scan_msg}")
         try:
             self.metadata = {
                 "scanID": scan_msg.content["scanID"],
                 "RID": scan_msg.content["info"]["RID"],
                 "queueID": scan_msg.content["info"]["queueID"],
```

### Comparing `ophyd_devices-0.9.1/ophyd_devices/epics/devices/cSaxsVirtualMotors.py` & `ophyd_devices-0.9.2/ophyd_devices/epics/devices/cSaxsVirtualMotors.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/epics/devices/eiger9m_csaxs.py` & `ophyd_devices-0.9.2/ophyd_devices/epics/devices/eiger9m_csaxs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import enum
-import threading
 import time
+import threading
 from bec_lib.core.devicemanager import DeviceStatus
 import numpy as np
 import os
 
 from typing import Any, List
 
 from ophyd import EpicsSignal, EpicsSignalRO, EpicsSignalWithRBV
@@ -12,34 +12,44 @@
 from ophyd import ADComponent as ADCpt
 
 from std_daq_client import StdDaqClient
 
 from bec_lib.core import BECMessage, MessageEndpoints, threadlocked
 from bec_lib.core.file_utils import FileWriterMixin
 from bec_lib.core import bec_logger
+from bec_lib.core.bec_service import SERVICE_CONFIG
 
 from ophyd_devices.epics.devices.bec_scaninfo_mixin import BecScaninfoMixin
 from ophyd_devices.utils import bec_utils
 
 logger = bec_logger.logger
 
+EIGER9M_MIN_READOUT = 3e-3
+
 
 class EigerError(Exception):
     """Base class for exceptions in this module."""
 
     pass
 
 
-class EigerTimeoutError(Exception):
+class EigerTimeoutError(EigerError):
     """Raised when the Eiger does not respond in time during unstage."""
 
     pass
 
 
-class SlsDetectorCam(Device):
+class DeviceClassInitError(EigerError):
+    """Raised when initiation of the device class fails,
+    due to missing device manager or not started in sim_mode."""
+
+    pass
+
+
+class SLSDetectorCam(Device):
     """SLS Detector Camera - Eiger 9M
 
     Base class to map EPICS PVs to ophyd signals.
     """
 
     threshold_energy = ADCpt(EpicsSignalWithRBV, "ThresholdEnergy")
     beam_energy = ADCpt(EpicsSignalWithRBV, "BeamEnergy")
@@ -48,24 +58,24 @@
     num_frames = ADCpt(EpicsSignalWithRBV, "NumFrames")
     trigger_mode = ADCpt(EpicsSignalWithRBV, "TimingMode")
     trigger_software = ADCpt(EpicsSignal, "TriggerSoftware")
     acquire = ADCpt(EpicsSignal, "Acquire")
     detector_state = ADCpt(EpicsSignalRO, "DetectorState_RBV")
 
 
-class TriggerSource(int, enum.Enum):
+class TriggerSource(enum.IntEnum):
     """Trigger signals for Eiger9M detector"""
 
     AUTO = 0
     TRIGGER = 1
     GATING = 2
     BURST_TRIGGER = 3
 
 
-class DetectorState(int, enum.Enum):
+class DetectorState(enum.IntEnum):
     """Detector states for Eiger9M detector"""
 
     IDLE = 0
     ERROR = 1
     WAITING = 2
     FINISHED = 3
     TRANSMITTING = 4
@@ -73,15 +83,15 @@
     STOPPED = 6
     STILL_WAITING = 7
     INITIALIZING = 8
     DISCONNECTED = 9
     ABORTED = 10
 
 
-class Eiger9mCsaxs(DetectorBase):
+class Eiger9McSAXS(DetectorBase):
     """Eiger 9M detector for CSAXS
 
     Parent class: DetectorBase
     Device class: SlsDetectorCam
 
     Attributes:
         name str: 'eiger'
@@ -90,15 +100,15 @@
     """
 
     # Specify which functions are revealed to the user in BEC client
     USER_ACCESS = [
         "describe",
     ]
 
-    cam = ADCpt(SlsDetectorCam, "cam1:")
+    cam = ADCpt(SLSDetectorCam, "cam1:")
 
     def __init__(
         self,
         prefix="",
         *,
         name,
         kind=None,
@@ -127,55 +137,78 @@
             kind=kind,
             read_attrs=read_attrs,
             configuration_attrs=configuration_attrs,
             parent=parent,
             **kwargs,
         )
         if device_manager is None and not sim_mode:
-            raise EigerError("Add DeviceManager to initialization or init with sim_mode=True")
-
-        # Not sure if this is needed, comment it for now!
-        # self._lock = threading.RLock()
+            raise DeviceClassInitError(
+                f"No device manager for device: {name}, and not started sim_mode: {sim_mode}. Add DeviceManager to initialization or init with sim_mode=True"
+            )
+        self.sim_mode = sim_mode
+        # TODO check if threadlock is needed for unstage
+        self._lock = threading.RLock()
         self._stopped = False
         self.name = name
-        self.wait_for_connection()
-        # Spin up connections for simulation or BEC mode
-        # TODO check if sim_mode still works. Is it needed? I believe filewriting might be handled properly
+        self.service_cfg = None
+        self.std_client = None
+        self.scaninfo = None
+        self.filewriter = None
+        self.readout_time_min = EIGER9M_MIN_READOUT
+        self.std_rest_server_url = (
+            kwargs["file_writer_url"] if "file_writer_url" in kwargs else "http://xbl-daq-29:5000"
+        )
+        self.wait_for_connection(all_signals=True)
         if not sim_mode:
-            from bec_lib.core.bec_service import SERVICE_CONFIG
-
+            self._update_service_config()
             self.device_manager = device_manager
-            self._producer = self.device_manager.producer
-            self.service_cfg = SERVICE_CONFIG.config["service_config"]["file_writer"]
         else:
-            base_path = f"/sls/X12SA/data/{self.scaninfo.username}/Data10/"
-            self._producer = bec_utils.MockProducer()
-            self.device_manager = bec_utils.MockDeviceManager()
-            self.scaninfo = BecScaninfoMixin(device_manager, sim_mode)
-            self.scaninfo.load_scan_metadata()
-            self.service_cfg = {"base_path": base_path}
+            self.device_manager = bec_utils.DMMock()
+            base_path = kwargs["basepath"] if "basepath" in kwargs else "~/Data10/"
+            self.service_cfg = {"base_path": os.path.expanduser(base_path)}
+        self._producer = self.device_manager.producer
+        self._update_scaninfo()
+        self._update_filewriter()
+        self._init()
 
-        self.scaninfo = BecScaninfoMixin(device_manager, sim_mode)
-        self.scaninfo.load_scan_metadata()
+    def _update_filewriter(self) -> None:
+        """Update filewriter with service config"""
         self.filewriter = FileWriterMixin(self.service_cfg)
-        self._init()
+
+    def _update_scaninfo(self) -> None:
+        """Update scaninfo from BecScaninfoMixing
+        This depends on device manager and operation/sim_mode
+        """
+        self.scaninfo = BecScaninfoMixin(self.device_manager, self.sim_mode)
+        self.scaninfo.load_scan_metadata()
+
+    def _update_service_config(self) -> None:
+        """Update service config from BEC service config"""
+        self.service_cfg = SERVICE_CONFIG.config["service_config"]["file_writer"]
 
     # TODO function for abstract class?
     def _init(self) -> None:
         """Initialize detector, filewriter and set default parameters"""
         self._default_parameter()
         self._init_detector()
         self._init_filewriter()
 
-    # TODO function for abstract class?
     def _default_parameter(self) -> None:
-        """Set default parameters for Eiger 9M
-        readout (float) : readout time in seconds
+        """Set default parameters for Pilatus300k detector
+        readout (float): readout time in seconds
         """
-        self.reduce_readout = 1e-3
+        self._update_readout_time()
+
+    def _update_readout_time(self) -> None:
+        readout_time = (
+            self.scaninfo.readout_time
+            if hasattr(self.scaninfo, "readout_time")
+            else self.readout_time_min
+        )
+        self.readout_time = max(readout_time, self.readout_time_min)
 
     # TODO function for abstract class?
     def _init_detector(self) -> None:
         """Init parameters for Eiger 9m.
         Depends on hardware configuration and delay generators.
         At this point it is set up for gating mode (09/2023).
         """
@@ -184,28 +217,27 @@
 
     # TODO function for abstract class?
     def _init_filewriter(self) -> None:
         """Init parameters for filewriter.
         For the Eiger9M, the data backend is std_daq client.
         Setting up these parameters depends on the backend, and would need to change upon changes in the backend.
         """
-        self.std_rest_server_url = "http://xbl-daq-29:5000"
         self.std_client = StdDaqClient(url_base=self.std_rest_server_url)
         self.std_client.stop_writer()
         timeout = 0
-        # TODO changing e-account was not possible during beamtimes.
-        # self._update_std_cfg("writer_user_id", int(self.scaninfo.username.strip(" e")))
-        # time.sleep(5)
-        # TODO is this the only state to wait for or should we wait for more from the std_daq client?
+        # TODO put back change of e-account! and check with Leo which status to wait for
+        eacc = self.scaninfo.username
+        self._update_std_cfg("writer_user_id", int(eacc.strip(" e")))
+        time.sleep(5)
         while not self.std_client.get_status()["state"] == "READY":
             time.sleep(0.1)
             timeout = timeout + 0.1
             logger.info("Waiting for std_daq init.")
             if timeout > 5:
-                if not self.std_client.get_status()["state"]:
+                if not self.std_client.get_status()["state"] == "READY":
                     raise EigerError(
                         f"Std client not in READY state, returns: {self.std_client.get_status()}"
                     )
                 else:
                     return
 
     def _update_std_cfg(self, cfg_key: str, value: Any) -> None:
@@ -248,34 +280,40 @@
         self.mokev = self.device_manager.devices.mokev.obj.read()[
             self.device_manager.devices.mokev.name
         ]["value"]
         # TODO refactor logger.info to DEBUG mode?
         self._prep_file_writer()
         self._prep_det()
         state = False
-        self._publish_file_location(done=state, successful=state)
+        self._publish_file_location(done=state)
         self._arm_acquisition()
         # TODO Fix should take place in EPICS or directly on the hardware!
         # We observed that the detector missed triggers in the beginning in case BEC was to fast. Adding 50ms delay solved this
         time.sleep(0.05)
         return super().stage()
 
+    def _filepath_exists(self, filepath: str) -> None:
+        timer = 0
+        while not os.path.exists(os.path.dirname(self.filepath)):
+            timer = time + 0.1
+            time.sleep(0.1)
+            if timer > 3:
+                raise EigerError(f"Timeout of 3s reached for filepath {self.filepath}")
+
     # TODO function for abstract class?
     def _prep_file_writer(self) -> None:
         """Prepare file writer for scan
 
         self.filewriter is a FileWriterMixin object that hosts logic for compiling the filepath
         """
+        timer = 0
         self.filepath = self.filewriter.compile_full_filename(
             self.scaninfo.scan_number, f"{self.name}.h5", 1000, 5, True
         )
-        # TODO needed, should be checked from the filerwriter mixin right?
-        while not os.path.exists(os.path.dirname(self.filepath)):
-            time.sleep(0.1)
-
+        self._filepath_exists(self.filepath)
         self._stop_file_writer()
         logger.info(f" std_daq output filepath {self.filepath}")
         # TODO Discuss with Leo if this is needed, or how to start the async writing best
         try:
             self.std_client.start_writer_async(
                 {
                     "output_file": self.filepath,
@@ -284,86 +322,113 @@
             )
         except Exception as exc:
             time.sleep(5)
             if self.std_client.get_status()["state"] == "READY":
                 raise EigerError(f"Timeout of start_writer_async with {exc}")
 
         while True:
+            timer = timer + 0.01
             det_ctrl = self.std_client.get_status()["acquisition"]["state"]
             if det_ctrl == "WAITING_IMAGES":
                 break
-            time.sleep(0.005)
+            time.sleep(0.01)
+            if timer > 5:
+                self._close_file_writer()
+                raise EigerError(
+                    f"Timeout of 5s reached for std_daq start_writer_async with std_daq client status {det_ctrl}"
+                )
 
     # TODO function for abstract class?
     def _stop_file_writer(self) -> None:
         """Close file writer"""
         self.std_client.stop_writer()
-        # TODO can I wait for a status message here maybe? To ensure writer returned
+        # TODO can I wait for a status message here maybe? To ensure writer stopped and returned
 
     # TODO function for abstract class?
     def _prep_det(self) -> None:
         """Prepare detector for scan.
         Includes checking the detector threshold, setting the acquisition parameters and setting the trigger source
         """
         self._set_det_threshold()
         self._set_acquisition_params()
         self._set_trigger(TriggerSource.GATING)
 
     def _set_det_threshold(self) -> None:
         """Set correct detector threshold to 1/2 of current X-ray energy, allow 5% tolerance"""
         # threshold energy might be in eV or keV
         factor = 1
-        if self.cam.threshold_energy._metadata["units"] == "eV":
+        unit = getattr(self.cam.threshold_energy, "units", None)
+        if unit != None and unit == "eV":
             factor = 1000
         setpoint = int(self.mokev * factor)
         energy = self.cam.beam_energy.read()[self.cam.beam_energy.name]["value"]
         if setpoint != energy:
             self.cam.beam_energy.set(setpoint)
         threshold = self.cam.threshold_energy.read()[self.cam.threshold_energy.name]["value"]
         if not np.isclose(setpoint / 2, threshold, rtol=0.05):
             self.cam.threshold_energy.set(setpoint / 2)
 
     def _set_acquisition_params(self) -> None:
         """Set acquisition parameters for the detector"""
         self.cam.num_images.put(int(self.scaninfo.num_points * self.scaninfo.frames_per_trigger))
         self.cam.num_frames.put(1)
+        self._update_readout_time()
 
     # TODO function for abstract class? + call it for each scan??
     def _set_trigger(self, trigger_source: TriggerSource) -> None:
         """Set trigger source for the detector.
         Check the TriggerSource enum for possible values
+
+        Args:
+            trigger_source (TriggerSource): Trigger source for the detector
+
         """
-        value = int(trigger_source)
+        value = trigger_source
         self.cam.trigger_mode.put(value)
 
-    def _publish_file_location(self, done=False, successful=False) -> None:
-        """Publish the filepath to REDIS
-        First msg for file writer and the second one for other listeners (e.g. radial integ)
+    def _publish_file_location(self, done: bool = False, successful: bool = None) -> None:
+        """Publish the filepath to REDIS.
+        We publish two events here:
+        - file_event: event for the filewriter
+        - public_file: event for any secondary service (e.g. radial integ code)
+
+        Args:
+            done (bool): True if scan is finished
+            successful (bool): True if scan was successful
+
         """
         pipe = self._producer.pipeline()
-        msg = BECMessage.FileMessage(file_path=self.filepath, done=done, successful=successful)
+        if successful is None:
+            msg = BECMessage.FileMessage(file_path=self.filepath, done=done)
+        else:
+            msg = BECMessage.FileMessage(file_path=self.filepath, done=done, successful=successful)
         self._producer.set_and_publish(
             MessageEndpoints.public_file(self.scaninfo.scanID, self.name), msg.dumps(), pipe=pipe
         )
         self._producer.set_and_publish(
-            MessageEndpoints.file_event(self.name), msg.dumps(), pip=pipe
+            MessageEndpoints.file_event(self.name), msg.dumps(), pipe=pipe
         )
         pipe.execute()
 
     # TODO function for abstract class?
     def _arm_acquisition(self) -> None:
         """Arm Eiger detector for acquisition"""
+        timer = 0
         self.cam.acquire.put(1)
         while True:
             det_ctrl = self.cam.detector_state.read()[self.cam.detector_state.name]["value"]
-            if det_ctrl == int(DetectorState.RUNNING):
+            if det_ctrl == DetectorState.RUNNING:
                 break
             if self._stopped == True:
                 break
-            time.sleep(0.005)
+            time.sleep(0.01)
+            timer += 0.01
+            if timer > 5:
+                self.stop()
+                raise EigerTimeoutError("Failed to arm the acquisition. IOC did not update.")
 
     # TODO function for abstract class?
     def trigger(self) -> DeviceStatus:
         """Trigger the detector, called from BEC."""
         self._on_trigger()
         return super().trigger()
 
@@ -415,23 +480,21 @@
         """
         sleep_time = 0.1
         timeout = 5
         timer = 0
         # Check status with timeout, break out if _stopped=True
         while True:
             det_ctrl = self.cam.acquire.read()[self.cam.acquire.name]["value"]
-            std_ctrl = self.std_client.get_status()["acquisition"]["state"]
             status = self.std_client.get_status()
+            std_ctrl = status["acquisition"]["state"]
             received_frames = status["acquisition"]["stats"]["n_write_completed"]
             total_frames = int(self.scaninfo.num_points * self.scaninfo.frames_per_trigger)
             if det_ctrl == 0 and std_ctrl == "FINISHED" and total_frames == received_frames:
                 break
             if self._stopped == True:
-                self._stop_det()
-                self._stop_file_writer()
                 break
             time.sleep(sleep_time)
             timer += sleep_time
             if timer > timeout:
                 self._stopped == True
                 self._stop_det()
                 self._stop_file_writer()
@@ -448,15 +511,15 @@
         timeout = 5
         # Stop acquisition
         self.cam.acquire.put(0)
         retry = False
         # Check status
         while True:
             det_ctrl = self.cam.detector_state.read()[self.cam.detector_state.name]["value"]
-            if det_ctrl == int(DetectorState.IDLE):
+            if det_ctrl == DetectorState.IDLE:
                 break
             if self._stopped == True:
                 break
             time.sleep(sleep_time)
             elapsed_time += sleep_time
             if elapsed_time > timeout // 2 and not retry:
                 retry = True
@@ -470,8 +533,8 @@
         self._stop_det()
         self._stop_file_writer()
         super().stop(success=success)
         self._stopped = True
 
 
 if __name__ == "__main__":
-    eiger = Eiger9mCsaxs(name="eiger", prefix="X12SA-ES-EIGER9M:", sim_mode=True)
+    eiger = Eiger9McSAXS(name="eiger", prefix="X12SA-ES-EIGER9M:", sim_mode=True)
```

### Comparing `ophyd_devices-0.9.1/ophyd_devices/epics/devices/epics_motor_ex.py` & `ophyd_devices-0.9.2/ophyd_devices/epics/devices/epics_motor_ex.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/epics/devices/falcon_csaxs.py` & `ophyd_devices-0.9.2/ophyd_devices/epics/devices/falcon_csaxs.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/epics/devices/mcs_csaxs.py` & `ophyd_devices-0.9.2/ophyd_devices/epics/devices/mcs_csaxs.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/epics/devices/mono_dccm.py` & `ophyd_devices-0.9.2/ophyd_devices/epics/devices/mono_dccm.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/epics/devices/pilatus_csaxs.py` & `ophyd_devices-0.9.2/ophyd_devices/epics/devices/pilatus_csaxs.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,50 +10,60 @@
 
 from ophyd import EpicsSignal, EpicsSignalRO, EpicsSignalWithRBV
 from ophyd import DetectorBase, Device, Staged
 from ophyd import ADComponent as ADCpt
 
 from bec_lib.core import BECMessage, MessageEndpoints
 from bec_lib.core.file_utils import FileWriterMixin
+from bec_lib.core.bec_service import SERVICE_CONFIG
 from bec_lib.core import bec_logger
 
 from ophyd_devices.utils import bec_utils as bec_utils
 from ophyd_devices.epics.devices.bec_scaninfo_mixin import BecScaninfoMixin
 
 logger = bec_logger.logger
 
+PILATUS_MIN_READOUT = 3e-3
+
 
 class PilatusError(Exception):
     """Base class for exceptions in this module."""
 
     pass
 
 
-class PilatusTimeoutError(Exception):
+class PilatusTimeoutError(PilatusError):
     """Raised when the Pilatus does not respond in time during unstage."""
 
     pass
 
 
-class TriggerSource(int, enum.Enum):
+class DeviceClassInitError(PilatusError):
+    """Raised when initiation of the device class fails,
+    due to missing device manager or not started in sim_mode."""
+
+    pass
+
+
+class TriggerSource(enum.IntEnum):
     INTERNAL = 0
     EXT_ENABLE = 1
     EXT_TRIGGER = 2
     MULTI_TRIGGER = 3
     ALGINMENT = 4
 
 
-class SlsDetectorCam(Device):
+class SLSDetectorCam(Device):
     """SLS Detector Camera - Pilatus
 
     Base class to map EPICS PVs to ophyd signals.
     """
 
     num_images = ADCpt(EpicsSignalWithRBV, "NumImages")
-    num_exposures = ADCpt(EpicsSignalWithRBV, "NumExposures")
+    num_frames = ADCpt(EpicsSignalWithRBV, "NumExposures")
     delay_time = ADCpt(EpicsSignalWithRBV, "NumExposures")
     trigger_mode = ADCpt(EpicsSignalWithRBV, "TriggerMode")
     acquire = ADCpt(EpicsSignal, "Acquire")
     armed = ADCpt(EpicsSignalRO, "Armed")
 
     read_file_timeout = ADCpt(EpicsSignal, "ImageFileTmot")
     detector_state = ADCpt(EpicsSignalRO, "StatusMessage_RBV")
@@ -66,15 +76,15 @@
     file_number = ADCpt(EpicsSignalWithRBV, "FileNumber")
     auto_increment = ADCpt(EpicsSignalWithRBV, "AutoIncrement")
     file_template = ADCpt(EpicsSignalWithRBV, "FileTemplate")
     file_format = ADCpt(EpicsSignalWithRBV, "FileNumber")
     gap_fill = ADCpt(EpicsSignalWithRBV, "GapFill")
 
 
-class PilatusCsaxs(DetectorBase):
+class PilatuscSAXS(DetectorBase):
     """Pilatus_2 300k detector for CSAXS
 
     Parent class: DetectorBase
     Device class: PilatusDetectorCamEx
 
     Attributes:
         name str: 'pilatus_2'
@@ -83,15 +93,15 @@
     """
 
     # Specify which functions are revealed to the user in BEC client
     USER_ACCESS = [
         "describe",
     ]
 
-    cam = ADCpt(SlsDetectorCam, "cam1:")
+    cam = ADCpt(SLSDetectorCam, "cam1:")
 
     def __init__(
         self,
         prefix="",
         *,
         name,
         kind=None,
@@ -120,104 +130,134 @@
             kind=kind,
             read_attrs=read_attrs,
             configuration_attrs=configuration_attrs,
             parent=parent,
             **kwargs,
         )
         if device_manager is None and not sim_mode:
-            raise PilatusError("Add DeviceManager to initialization or init with sim_mode=True")
-
+            raise DeviceClassInitError(
+                f"No device manager for device: {name}, and not started sim_mode: {sim_mode}. Add DeviceManager to initialization or init with sim_mode=True"
+            )
+        self.sim_mode = sim_mode
+        self._stopped = False
         self.name = name
-        self.wait_for_connection()
-        # Spin up connections for simulation or BEC mode
+        self.service_cfg = None
+        self.std_client = None
+        self.scaninfo = None
+        self.filewriter = None
+        self.readout_time_min = PILATUS_MIN_READOUT
+        # TODO move url from data backend up here?
+        self.wait_for_connection(all_signals=True)
         if not sim_mode:
-            from bec_lib.core.bec_service import SERVICE_CONFIG
-
+            self._update_service_config()
             self.device_manager = device_manager
-            self._producer = self.device_manager.producer
-            self.service_cfg = SERVICE_CONFIG.config["service_config"]["file_writer"]
         else:
-            base_path = f"/sls/X12SA/data/{self.scaninfo.username}/Data10/"
-            self._producer = bec_utils.MockProducer()
-            self.device_manager = bec_utils.MockDeviceManager()
-            self.scaninfo = BecScaninfoMixin(device_manager, sim_mode)
-            self.scaninfo.load_scan_metadata()
-            self.service_cfg = {"base_path": base_path}
+            self.device_manager = bec_utils.DMMock()
+            base_path = kwargs["basepath"] if "basepath" in kwargs else "~/Data10/"
+            self.service_cfg = {"base_path": os.path.expanduser(base_path)}
+        self._producer = self.device_manager.producer
+        self._update_scaninfo()
+        self._update_filewriter()
+        self._init()
 
-        self.scaninfo = BecScaninfoMixin(device_manager, sim_mode)
-        self.scaninfo.load_scan_metadata()
+    def _update_filewriter(self) -> None:
+        """Update filewriter with service config"""
         self.filewriter = FileWriterMixin(self.service_cfg)
-        self._init()
+
+    def _update_scaninfo(self) -> None:
+        """Update scaninfo from BecScaninfoMixing
+        This depends on device manager and operation/sim_mode
+        """
+        self.scaninfo = BecScaninfoMixin(self.device_manager, self.sim_mode)
+        self.scaninfo.load_scan_metadata()
+
+    def _update_service_config(self) -> None:
+        """Update service config from BEC service config"""
+        self.service_cfg = SERVICE_CONFIG.config["service_config"]["file_writer"]
 
     def _init(self) -> None:
         """Initialize detector, filewriter and set default parameters"""
         self._default_parameter()
         self._init_detector()
         self._init_filewriter()
 
     def _default_parameter(self) -> None:
         """Set default parameters for Pilatus300k detector
         readout (float): readout time in seconds
         """
-        self.reduce_readout = 1e-3
+        self._update_readout_time()
+
+    def _update_readout_time(self) -> None:
+        readout_time = (
+            self.scaninfo.readout_time
+            if hasattr(self.scaninfo, "readout_time")
+            else self.readout_time_min
+        )
+        self.readout_time = max(readout_time, self.readout_time_min)
 
     def _init_detector(self) -> None:
         """Initialize the detector"""
         # TODO add check if detector is running
-        pass
+        self._stop_det()
+        self._set_trigger(TriggerSource.EXT_ENABLE)
 
     def _init_filewriter(self) -> None:
         """Initialize the file writer"""
         # TODO in case the data backend is rewritten, add check if it is ready!
         pass
 
     def _prep_det(self) -> None:
         # TODO slow reaction, seemed to have timeout.
         self._set_det_threshold()
         self._set_acquisition_params()
+        self._set_trigger(TriggerSource.EXT_ENABLE)
 
     def _set_det_threshold(self) -> None:
         # threshold_energy PV exists on Eiger 9M?
         factor = 1
-        if self.cam.threshold_energy._metadata["units"] == "eV":
+        unit = getattr(self.cam.threshold_energy, "units", None)
+        if unit != None and unit == "eV":
             factor = 1000
         setpoint = int(self.mokev * factor)
         threshold = self.cam.threshold_energy.read()[self.cam.threshold_energy.name]["value"]
         if not np.isclose(setpoint / 2, threshold, rtol=0.05):
-            self.cam.threshold_energy.set(setpoint / 2)
+            self.cam.threshold_energy.put(setpoint / 2)
 
     def _set_acquisition_params(self) -> None:
         """set acquisition parameters on the detector"""
         # self.cam.acquire_time.set(self.exp_time)
         # self.cam.acquire_period.set(self.exp_time + self.readout)
-        self.cam.num_images.set(int(self.scaninfo.num_points * self.scaninfo.frames_per_trigger))
-        self.cam.num_exposures.set(1)
-        self._set_trigger(TriggerSource.EXT_ENABLE)  # EXT_TRIGGER)
+        self.cam.num_images.put(int(self.scaninfo.num_points * self.scaninfo.frames_per_trigger))
+        self.cam.num_frames.put(1)
+        self._update_readout_time()
 
-    def _set_trigger(self, trigger_source: TriggerSource) -> None:
+    def _set_trigger(self, trigger_source: int) -> None:
         """Set trigger source for the detector, either directly to value or TriggerSource.* with
         INTERNAL = 0
         EXT_ENABLE = 1
         EXT_TRIGGER = 2
         MULTI_TRIGGER = 3
         ALGINMENT = 4
         """
-        value = int(trigger_source)
-        self.cam.trigger_mode.set(value)
+        value = trigger_source
+        self.cam.trigger_mode.put(value)
+
+    def _create_directory(filepath: str) -> None:
+        """Create directory if it does not exist"""
+        os.makedirs(filepath, exist_ok=True)
 
     def _prep_file_writer(self) -> None:
-        """Prepare the file writer for pilatus_2
-        a zmq service is running on xbl-daq-34 that is waiting
+        """
+        Prepare the file writer for pilatus_2
+
+        A zmq service is running on xbl-daq-34 that is waiting
         for a zmq message to start the writer for the pilatus_2 x12sa-pd-2
+
         """
-        # TODO worked reliable with time.sleep(2)
-        # self._close_file_writer()
-        # time.sleep(2)
-        # self._stop_file_writer()
-        # time.sleep(2)
+        # TODO explore required sleep time here
         self._close_file_writer()
         time.sleep(0.1)
         self._stop_file_writer()
         time.sleep(0.1)
 
         self.filepath_raw = self.filewriter.compile_full_filename(
             self.scaninfo.scan_number, "pilatus_2.h5", 1000, 5, True
@@ -225,119 +265,135 @@
         self.cam.file_path.put(f"/dev/shm/zmq/")
         self.cam.file_name.put(f"{self.scaninfo.username}_2_{self.scaninfo.scan_number:05d}")
         self.cam.auto_increment.put(1)  # auto increment
         self.cam.file_number.put(0)  # first iter
         self.cam.file_format.put(0)  # 0: TIFF
         self.cam.file_template.put("%s%s_%5.5d.cbf")
 
+        # TODO remove hardcoded filepath here
         # compile filename
         basepath = f"/sls/X12SA/data/{self.scaninfo.username}/Data10/pilatus_2/"
         self.filepath = os.path.join(
             basepath,
             self.filewriter.get_scan_directory(self.scaninfo.scan_number, 1000, 5),
         )
         # Make directory if needed
-        os.makedirs(self.filepath, exist_ok=True)
+        self._create_directory(self.filepath)
 
+        headers = {"Content-Type": "application/json", "Accept": "application/json"}
+        # start the stream on x12sa-pd-2
+        url = "http://x12sa-pd-2:8080/stream/pilatus_2"
         data_msg = {
             "source": [
                 {
                     "searchPath": "/",
                     "searchPattern": "glob:*.cbf",
                     "destinationPath": self.filepath,
                 }
             ]
         }
-
-        logger.info(data_msg)
-        headers = {"Content-Type": "application/json", "Accept": "application/json"}
-
-        res = requests.put(
-            url="http://x12sa-pd-2:8080/stream/pilatus_2",
-            data=json.dumps(data_msg),
-            headers=headers,
-        )
+        res = self._send_requests_put(url=url, data=data_msg, headers=headers)
         logger.info(f"{res.status_code} -  {res.text} - {res.content}")
 
         if not res.ok:
             res.raise_for_status()
 
-        # prepare writer
+        # start the data receiver on xbl-daq-34
+        url = "http://xbl-daq-34:8091/pilatus_2/run"
         data_msg = [
             "zmqWriter",
             self.scaninfo.username,
             {
                 "addr": "tcp://x12sa-pd-2:8888",
                 "dst": ["file"],
                 "numFrm": int(self.scaninfo.num_points * self.scaninfo.frames_per_trigger),
                 "timeout": 2000,
                 "ifType": "PULL",
                 "user": self.scaninfo.username,
             },
         ]
-
-        res = requests.put(
-            url="http://xbl-daq-34:8091/pilatus_2/run",
-            data=json.dumps(data_msg),
-            headers=headers,
-        )
-        # subprocess.run("curl -i -s -X PUT http://xbl-daq-34:8091/pilatus_2/run -d '[\"zmqWriter\",\"e20636\",{\"addr\":\"tcp://x12sa-pd-2:8888\",\"dst\":[\"file\"],\"numFrm\":10,\"timeout\":2000,\"ifType\":\"PULL\",\"user\":\"e20636\"}]'", shell=True)
-
+        res = self._send_requests_put(url=url, data=data_msg, headers=headers)
         logger.info(f"{res.status_code}  - {res.text} - {res.content}")
 
         if not res.ok:
             res.raise_for_status()
 
         # Wait for server to become available again
         time.sleep(0.1)
+        logger.info(f"{res.status_code} -{res.text} - {res.content}")
 
-        headers = {"Content-Type": "application/json", "Accept": "application/json"}
+        # Sent requests.put to xbl-daq-34 to wait for data
+        url = "http://xbl-daq-34:8091/pilatus_2/wait"
         data_msg = [
             "zmqWriter",
             self.scaninfo.username,
             {
                 "frmCnt": int(self.scaninfo.num_points * self.scaninfo.frames_per_trigger),
                 "timeout": 2000,
             },
         ]
-        logger.info(f"{res.status_code} -{res.text} - {res.content}")
-
         try:
-            res = requests.put(
-                url="http://xbl-daq-34:8091/pilatus_2/wait",
-                data=json.dumps(data_msg),
-                #            headers=headers,
-            )
-
+            res = self._send_requests_put(url=url, data=data_msg, headers=headers)
             logger.info(f"{res}")
 
             if not res.ok:
                 res.raise_for_status()
         except Exception as exc:
             logger.info(f"Pilatus2 wait threw Exception: {exc}")
 
+    def _send_requests_put(self, url: str, data_msg: list = None, headers: dict = None) -> object:
+        """
+        Send a put request to the given url
+
+        Args:
+            url (str): url to send the request to
+            data (dict): data to be sent with the request (optional)
+            headers (dict): headers to be sent with the request (optional)
+
+        Returns:
+            status code of the request
+        """
+        return requests.put(url=url, data=json.dumps(data_msg), headers=headers)
+
+    def _send_requests_delete(self, url: str, headers: dict = None) -> object:
+        """
+        Send a delete request to the given url
+
+        Args:
+            url (str): url to send the request to
+            headers (dict): headers to be sent with the request (optional)
+
+        Returns:
+            status code of the request
+        """
+        return requests.delete(url=url, headers=headers)
+
     def _close_file_writer(self) -> None:
-        """Close the file writer for pilatus_2
-        a zmq service is running on xbl-daq-34 that is waiting
-        for a zmq message to stop the writer for the pilatus_2 x12sa-pd-2
         """
+        Close the file writer for pilatus_2
+
+        Delete the data from x12sa-pd-2
+
+        """
+        url = "http://x12sa-pd-2:8080/stream/pilatus_2"
         try:
-            res = requests.delete(url="http://x12sa-pd-2:8080/stream/pilatus_2")
+            res = self._send_requests_delete(url=url)
             if not res.ok:
                 res.raise_for_status()
         except Exception as exc:
-            logger.info(f"Pilatus2 delete threw Exception: {exc}")
+            logger.info(f"Pilatus2 close threw Exception: {exc}")
 
     def _stop_file_writer(self) -> None:
-        res = requests.put(
-            url="http://xbl-daq-34:8091/pilatus_2/stop",
-            # data=json.dumps(data_msg),
-            #            headers=headers,
-        )
+        """
+        Stop the file writer for pilatus_2
 
+        Runs on xbl-daq-34
+        """
+        url = "http://xbl-daq-34:8091/pilatus_2/stop"
+        res = self._send_requests_put(url=url)
         if not res.ok:
             res.raise_for_status()
 
     def stage(self) -> List[object]:
         """Stage command, called from BEC in preparation of a scan.
         This will iniate the preparation of detector and file writer.
         The following functuions are called:
@@ -358,36 +414,52 @@
         self.mokev = self.device_manager.devices.mokev.obj.read()[
             self.device_manager.devices.mokev.name
         ]["value"]
         # TODO refactor logger.info to DEBUG mode?
         self._prep_file_writer()
         self._prep_det()
         state = False
-        self._publish_file_location(done=state, successful=state)
+        self._publish_file_location(done=state)
         return super().stage()
 
     # TODO might be useful for base class
     def pre_scan(self) -> None:
-        """ " Pre_scan gets executed right before"""
+        """Pre_scan is an (optional) function that is executed by BEC just before the scan core
+
+        For the pilatus detector, it is used to arm the detector for the acquisition,
+        because the detector times out after ˜7-8seconds without seeing a trigger.
+        """
         self._arm_acquisition()
 
     def _arm_acquisition(self) -> None:
-        self.acquire()
+        self.cam.acquire.put(1)
+        # TODO check if sleep of 1s is needed, could be that less is enough
+        time.sleep(1)
+
+    def _publish_file_location(self, done: bool = False, successful: bool = None) -> None:
+        """Publish the filepath to REDIS.
+        We publish two events here:
+        - file_event: event for the filewriter
+        - public_file: event for any secondary service (e.g. radial integ code)
+
+        Args:
+            done (bool): True if scan is finished
+            successful (bool): True if scan was successful
 
-    def _publish_file_location(self, done=False, successful=False) -> None:
-        """Publish the filepath to REDIS
-        First msg for file writer and the second one for other listeners (e.g. radial integ)
         """
         pipe = self._producer.pipeline()
-        msg = BECMessage.FileMessage(file_path=self.filepath, done=done, successful=successful)
+        if successful is None:
+            msg = BECMessage.FileMessage(file_path=self.filepath, done=done)
+        else:
+            msg = BECMessage.FileMessage(file_path=self.filepath, done=done, successful=successful)
         self._producer.set_and_publish(
             MessageEndpoints.public_file(self.scaninfo.scanID, self.name), msg.dumps(), pipe=pipe
         )
         self._producer.set_and_publish(
-            MessageEndpoints.file_event(self.name), msg.dumps(), pip=pipe
+            MessageEndpoints.file_event(self.name), msg.dumps(), pipe=pipe
         )
         pipe.execute()
 
     # TODO function for abstract class?
     def trigger(self) -> DeviceStatus:
         """Trigger the detector, called from BEC."""
         self._on_trigger()
@@ -437,52 +509,39 @@
         and will check detector and file backend status.
         Timeouts after given time
 
         Functions called:
             - _stop_det
             - _stop_file_writer
         """
+        timer = 0
+        sleep_time = 0.1
+        # TODO this is a workaround at the moment which relies on the status of the mcs device
         while True:
             if self.device_manager.devices.mcs.obj._staged != Staged.yes:
                 break
-            time.sleep(0.1)
-        # TODO implement a waiting function or not
-        # time.sleep(2)
-        # timer = 0
-        # while True:
-        #     # rtr = self.cam.status_message_camserver.get()
-        #     #if self.cam.acquire.get() == 0 and rtr == "Camserver returned OK":
-        #     # if rtr == "Camserver returned OK":
-        #     #     break
-        #     if self._stopped == True:
-        #         break
-        #     time.sleep(0.1)
-        #     timer += 0.1
-        #     if timer > 5:
-        #         self._close_file_writer()
-        #         self._stop_file_writer()
-        #         self._stopped == True
-        #         # raise PilatusTimeoutError(
-        #         #     f"Pilatus timeout with detector state {self.cam.acquire.get()} and camserver return status: {rtr} "
-        #         # )
+            if self._stopped == True:
+                break
+            time.sleep(sleep_time)
+            timer = timer + sleep_time
+            if timer > 5:
+                self._stopped == True
+                self._stop_det()
+                self._stop_file_writer()
+                # TODO explore if sleep is needed
+                time.sleep(0.5)
+                self._close_file_writer()
+                raise PilatusTimeoutError(f"Timeout waiting for mcs device to unstage")
 
         self._stop_det()
         self._stop_file_writer()
-        # TODO explore if sleep is needed
+        # TODO explore if sleep time  is needed
         time.sleep(0.5)
         self._close_file_writer()
 
-    def acquire(self) -> None:
-        """Start acquisition in software trigger mode,
-        or arm the detector in hardware of the detector
-        """
-        self.cam.acquire.put(1)
-        # TODO check if sleep of 1s is needed, could be that less is enough
-        time.sleep(1)
-
     def _stop_det(self) -> None:
         """Stop the detector"""
         self.cam.acquire.put(0)
 
     def stop(self, *, success=False) -> None:
         """Stop the scan, with camera and file writer"""
         self._stop_det()
@@ -490,8 +549,8 @@
         self._close_file_writer()
         super().stop(success=success)
         self._stopped = True
 
 
 # Automatically connect to test environmenr if directly invoked
 if __name__ == "__main__":
-    pilatus_2 = PilatusCsaxs(name="pilatus_2", prefix="X12SA-ES-PILATUS300K:", sim_mode=True)
+    pilatus_2 = PilatuscSAXS(name="pilatus_2", prefix="X12SA-ES-PILATUS300K:", sim_mode=True)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ophyd_devices-0.9.1/ophyd_devices/epics/devices/sequencer_x12sa.py` & `ophyd_devices-0.9.2/ophyd_devices/epics/devices/sequencer_x12sa.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/epics/devices/slits.py` & `ophyd_devices-0.9.2/ophyd_devices/epics/devices/slits.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/epics/devices/slsDetector.py` & `ophyd_devices-0.9.2/ophyd_devices/epics/devices/slsDetector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/epics/devices/specMotors.py` & `ophyd_devices-0.9.2/ophyd_devices/epics/devices/specMotors.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/galil/galil_ophyd.py` & `ophyd_devices-0.9.2/ophyd_devices/galil/galil_ophyd.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/galil/sgalil_ophyd.py` & `ophyd_devices-0.9.2/ophyd_devices/galil/sgalil_ophyd.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/npoint/npoint.py` & `ophyd_devices-0.9.2/ophyd_devices/npoint/npoint.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/npoint/npoint_ophyd.py` & `ophyd_devices-0.9.2/ophyd_devices/npoint/npoint_ophyd.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/rt_lamni/rt_lamni_ophyd.py` & `ophyd_devices-0.9.2/ophyd_devices/rt_lamni/rt_lamni_ophyd.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/sim/sim.py` & `ophyd_devices-0.9.2/ophyd_devices/sim/sim.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/sim/sim_xtreme.py` & `ophyd_devices-0.9.2/ophyd_devices/sim/sim_xtreme.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/smaract/serializer.py` & `ophyd_devices-0.9.2/ophyd_devices/smaract/serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/smaract/smaract_controller.py` & `ophyd_devices-0.9.2/ophyd_devices/smaract/smaract_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/smaract/smaract_errors.py` & `ophyd_devices-0.9.2/ophyd_devices/smaract/smaract_errors.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/smaract/smaract_ophyd.py` & `ophyd_devices-0.9.2/ophyd_devices/smaract/smaract_ophyd.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/utils/controller.py` & `ophyd_devices-0.9.2/ophyd_devices/utils/controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices/utils/socket.py` & `ophyd_devices-0.9.2/ophyd_devices/utils/socket.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/ophyd_devices.egg-info/PKG-INFO` & `ophyd_devices-0.9.2/ophyd_devices.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ophyd-devices
-Version: 0.9.1
+Version: 0.9.2
 Summary: Custom device implementations based on the ophyd hardware abstraction layer
 Home-page: https://gitlab.psi.ch/bec/ophyd_devices
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/ophyd_devices/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ophyd_devices-0.9.1/ophyd_devices.egg-info/SOURCES.txt` & `ophyd_devices-0.9.2/ophyd_devices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.9.1/setup.cfg` & `ophyd_devices-0.9.2/setup.cfg`

 * *Files identical despite different names*

