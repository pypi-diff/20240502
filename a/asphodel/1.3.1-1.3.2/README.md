# Comparing `tmp/asphodel-1.3.1.tar.gz` & `tmp/asphodel-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asphodel-1.3.1.tar", last modified: Fri Mar 10 20:17:40 2023, max compression
+gzip compressed data, was "asphodel-1.3.2.tar", last modified: Thu May  2 17:41:07 2024, max compression
```

## Comparing `asphodel-1.3.1.tar` & `asphodel-1.3.2.tar`

### file list

```diff
@@ -1,180 +1,185 @@
-drwxrwxrwx   0        0        0        0 2023-03-10 20:17:40.625675 asphodel-1.3.1/
--rw-rw-rw-   0        0        0       89 2023-03-10 20:16:38.000000 asphodel-1.3.1/.gitmodules
--rw-rw-rw-   0        0        0     1593 2023-03-10 20:16:38.000000 asphodel-1.3.1/CMakeLists.txt
--rw-rw-rw-   0        0        0      757 2023-03-10 20:16:38.000000 asphodel-1.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0      387 2023-03-10 20:16:38.000000 asphodel-1.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1082 2023-03-10 20:17:40.625675 asphodel-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      522 2023-03-10 20:16:38.000000 asphodel-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-10 20:17:40.406921 asphodel-1.3.1/asphodel/
--rw-rw-rw-   0        0        0   178028 2023-03-10 20:16:38.000000 asphodel-1.3.1/asphodel/__init__.py
--rw-rw-rw-   0        0        0    23136 2023-03-10 20:16:38.000000 asphodel-1.3.1/asphodel/__init__.pyi
--rw-rw-rw-   0        0        0     7548 2023-03-10 20:16:38.000000 asphodel-1.3.1/asphodel/apdparse.py
--rw-rw-rw-   0        0        0    14483 2023-03-10 20:16:38.000000 asphodel-1.3.1/asphodel/nvmeditor.py
--rw-rw-rw-   0        0        0     9113 2023-03-10 20:16:38.000000 asphodel-1.3.1/asphodel/streamutil.py
--rw-rw-rw-   0        0        0      147 2023-03-10 20:17:39.000000 asphodel-1.3.1/asphodel/version.py
-drwxrwxrwx   0        0        0        0 2023-03-10 20:17:40.406921 asphodel-1.3.1/asphodel.egg-info/
--rw-rw-rw-   0        0        0     1082 2023-03-10 20:17:39.000000 asphodel-1.3.1/asphodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5532 2023-03-10 20:17:39.000000 asphodel-1.3.1/asphodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-10 20:17:39.000000 asphodel-1.3.1/asphodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-03-10 20:17:39.000000 asphodel-1.3.1/asphodel.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-03-10 20:17:39.000000 asphodel-1.3.1/asphodel.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-03-10 20:17:39.000000 asphodel-1.3.1/asphodel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-10 20:17:39.000000 asphodel-1.3.1/asphodel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-10 20:17:40.000717 asphodel-1.3.1/lib/
-drwxrwxrwx   0        0        0        0 2023-03-10 20:17:40.422646 asphodel-1.3.1/lib/asphodel/
--rw-rw-rw-   0        0        0     6356 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/CMakeLists.txt
--rw-rw-rw-   0        0        0     2629 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/GitHeader.cmake
--rw-rw-rw-   0        0        0      757 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/LICENSE.txt
--rw-rw-rw-   0        0        0     3660 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/OVERVIEW.md
--rw-rw-rw-   0        0        0     4331 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/README.md
--rw-rw-rw-   0        0        0      111 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/asphodel-usb.rules
--rw-rw-rw-   0        0        0     1543 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/buildspec.yml
-drwxrwxrwx   0        0        0        0 2023-03-10 20:17:40.422646 asphodel-1.3.1/lib/asphodel/ci-scripts/
--rw-rw-rw-   0        0        0     5042 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/ci-scripts/build.py
-drwxrwxrwx   0        0        0        0 2023-03-10 20:17:40.000717 asphodel-1.3.1/lib/asphodel/cmake/
-drwxrwxrwx   0        0        0        0 2023-03-10 20:17:40.422646 asphodel-1.3.1/lib/asphodel/cmake/modules/
--rw-rw-rw-   0        0        0     1839 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/cmake/modules/FindLIBUSB.cmake
-drwxrwxrwx   0        0        0        0 2023-03-10 20:17:40.422646 asphodel-1.3.1/lib/asphodel/documentation/
--rw-rw-rw-   0        0        0    45888 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/documentation/Base Protocol.docx
--rw-rw-rw-   0        0        0    28998 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/documentation/Bootloader Protocol.docx
--rw-rw-rw-   0        0        0    29229 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/documentation/Channel Types.docx
--rw-rw-rw-   0        0        0    34793 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/documentation/Low Level Interface.docx
--rw-rw-rw-   0        0        0    28240 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/documentation/RF Power Protocol.docx
--rw-rw-rw-   0        0        0    26728 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/documentation/Unit Types.docx
-drwxrwxrwx   0        0        0        0 2023-03-10 20:17:40.422646 asphodel-1.3.1/lib/asphodel/examples/
--rw-rw-rw-   0        0        0      132 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/examples/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2023-03-10 20:17:40.438213 asphodel-1.3.1/lib/asphodel/examples/enumeration/
--rw-rw-rw-   0        0        0      323 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/examples/enumeration/CMakeLists.txt
--rw-rw-rw-   0        0        0    63240 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/examples/enumeration/asphodel_enumeration.c
--rw-rw-rw-   0        0        0     2920 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/examples/enumeration/serialize.h
-drwxrwxrwx   0        0        0        0 2023-03-10 20:17:40.438213 asphodel-1.3.1/lib/asphodel/examples/reconnect_manual/
--rw-rw-rw-   0        0        0      543 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/examples/reconnect_manual/CMakeLists.txt
--rw-rw-rw-   0        0        0    16941 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/examples/reconnect_manual/asphodel_reconnect_manual.c
--rw-rw-rw-   0        0        0     8272 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/examples/reconnect_manual/inttypes.h
--rw-rw-rw-   0        0        0      815 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/examples/reconnect_manual/snprintf.h
-drwxrwxrwx   0        0        0        0 2023-03-10 20:17:40.438213 asphodel-1.3.1/lib/asphodel/examples/streaming/
--rw-rw-rw-   0        0        0      473 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/examples/streaming/CMakeLists.txt
--rw-rw-rw-   0        0        0    22616 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/examples/streaming/asphodel_streaming.c
--rw-rw-rw-   0        0        0     8272 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/examples/streaming/inttypes.h
--rw-rw-rw-   0        0        0      815 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/examples/streaming/snprintf.h
-drwxrwxrwx   0        0        0        0 2023-03-10 20:17:40.438213 asphodel-1.3.1/lib/asphodel/examples/unpack_benchmark/
--rw-rw-rw-   0        0        0      356 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/examples/unpack_benchmark/CMakeLists.txt
--rw-rw-rw-   0        0        0     2735 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/examples/unpack_benchmark/unpack_benchmark.c
-drwxrwxrwx   0        0        0        0 2023-03-10 20:17:40.469459 asphodel-1.3.1/lib/asphodel/inc/
--rw-rw-rw-   0        0        0     1469 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/inc/asphodel.h
--rw-rw-rw-   0        0        0     6859 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/inc/asphodel_api.h
--rw-rw-rw-   0        0        0     5573 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/inc/asphodel_bootloader.h
--rw-rw-rw-   0        0        0     6423 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/inc/asphodel_channel_specific.h
--rw-rw-rw-   0        0        0     3245 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/inc/asphodel_ctrl_var.h
--rw-rw-rw-   0        0        0     6737 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/inc/asphodel_decode.h
--rw-rw-rw-   0        0        0    22659 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/inc/asphodel_device.h
--rw-rw-rw-   0        0        0     1766 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/inc/asphodel_device_type.h
--rw-rw-rw-   0        0        0    10733 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/inc/asphodel_low_level.h
--rw-rw-rw-   0        0        0     1669 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/inc/asphodel_mem_test.h
--rw-rw-rw-   0        0        0    13867 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/inc/asphodel_protocol.h
--rw-rw-rw-   0        0        0    10192 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/inc/asphodel_radio.h
--rw-rw-rw-   0        0        0     2851 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/inc/asphodel_rf_power.h
--rw-rw-rw-   0        0        0     8392 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/inc/asphodel_setting.h
--rw-rw-rw-   0        0        0    10409 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/inc/asphodel_stream.h
--rw-rw-rw-   0        0        0     3112 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/inc/asphodel_supply.h
--rw-rw-rw-   0        0        0     4447 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/inc/asphodel_tcp.h
--rw-rw-rw-   0        0        0     4083 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/inc/asphodel_unit_format.h
--rw-rw-rw-   0        0        0     2611 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/inc/asphodel_usb.h
--rw-rw-rw-   0        0        0     1577 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/inc/asphodel_version.h
-drwxrwxrwx   0        0        0        0 2023-03-10 20:17:40.485187 asphodel-1.3.1/lib/asphodel/src/
--rw-rw-rw-   0        0        0     8095 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/src/asphodel_api.c
--rw-rw-rw-   0        0        0    63960 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/src/asphodel_decode.c
--rw-rw-rw-   0        0        0   225661 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/src/asphodel_device.c
--rw-rw-rw-   0        0        0     1750 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/src/asphodel_device_type.c
--rw-rw-rw-   0        0        0     1892 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/src/asphodel_mem_test.c
--rw-rw-rw-   0        0        0    84340 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/src/asphodel_tcp.c
--rw-rw-rw-   0        0        0    22166 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/src/asphodel_unit_format.c
--rw-rw-rw-   0        0        0    92634 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/src/asphodel_usb.c
--rw-rw-rw-   0        0        0     2118 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/src/asphodel_version.c
--rw-rw-rw-   0        0        0     5619 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/src/clock.c
--rw-rw-rw-   0        0        0     1965 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/src/clock.h
--rw-rw-rw-   0        0        0     3024 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/src/mutex.h
--rw-rw-rw-   0        0        0     2958 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/src/serialize.h
--rw-rw-rw-   0        0        0      815 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/src/snprintf.h
--rw-rw-rw-   0        0        0      249 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/src/version_autogen.h.in
-drwxrwxrwx   0        0        0        0 2023-03-10 20:17:40.485187 asphodel-1.3.1/lib/asphodel/unpack/
--rw-rw-rw-   0        0        0     1815 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2023-03-10 20:17:40.500687 asphodel-1.3.1/lib/asphodel/unpack/inc/
--rw-rw-rw-   0        0        0     1923 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/inc/unpack.h
-drwxrwxrwx   0        0        0        0 2023-03-10 20:17:40.625675 asphodel-1.3.1/lib/asphodel/unpack/src/
--rw-rw-rw-   0        0        0     9234 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack.c
--rw-rw-rw-   0        0        0     7087 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack0.c
--rw-rw-rw-   0        0        0      236 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack0.h
--rw-rw-rw-   0        0        0    59873 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack1.c
--rw-rw-rw-   0        0        0      236 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack1.h
--rw-rw-rw-   0        0        0  3969841 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack10.c
--rw-rw-rw-   0        0        0      243 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack10.h
--rw-rw-rw-   0        0        0   146190 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack11.c
--rw-rw-rw-   0        0        0      242 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack11.h
--rw-rw-rw-   0        0        0  2865578 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack12.c
--rw-rw-rw-   0        0        0      243 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack12.h
--rw-rw-rw-   0        0        0   151084 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack13.c
--rw-rw-rw-   0        0        0      242 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack13.h
--rw-rw-rw-   0        0        0  2231612 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack14.c
--rw-rw-rw-   0        0        0      243 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack14.h
--rw-rw-rw-   0        0        0   156024 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack15.c
--rw-rw-rw-   0        0        0      242 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack15.h
--rw-rw-rw-   0        0        0  7004428 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack16.c
--rw-rw-rw-   0        0        0      243 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack16.h
--rw-rw-rw-   0        0        0   160868 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack17.c
--rw-rw-rw-   0        0        0      242 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack17.h
--rw-rw-rw-   0        0        0  1501336 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack18.c
--rw-rw-rw-   0        0        0      243 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack18.h
--rw-rw-rw-   0        0        0   165654 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack19.c
--rw-rw-rw-   0        0        0      242 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack19.h
--rw-rw-rw-   0        0        0   120471 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack2.c
--rw-rw-rw-   0        0        0      236 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack2.h
--rw-rw-rw-   0        0        0  1259299 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack20.c
--rw-rw-rw-   0        0        0      243 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack20.h
--rw-rw-rw-   0        0        0   170508 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack21.c
--rw-rw-rw-   0        0        0      242 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack21.h
--rw-rw-rw-   0        0        0  1115323 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack22.c
--rw-rw-rw-   0        0        0      243 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack22.h
--rw-rw-rw-   0        0        0   174668 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack23.c
--rw-rw-rw-   0        0        0      242 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack23.h
--rw-rw-rw-   0        0        0  3580668 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack24.c
--rw-rw-rw-   0        0        0      243 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack24.h
--rw-rw-rw-   0        0        0   179218 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack25.c
--rw-rw-rw-   0        0        0      242 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack25.h
--rw-rw-rw-   0        0        0   830623 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack26.c
--rw-rw-rw-   0        0        0      243 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack26.h
--rw-rw-rw-   0        0        0   184018 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack27.c
--rw-rw-rw-   0        0        0      242 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack27.h
--rw-rw-rw-   0        0        0   775042 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack28.c
--rw-rw-rw-   0        0        0      243 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack28.h
--rw-rw-rw-   0        0        0   188758 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack29.c
--rw-rw-rw-   0        0        0      242 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack29.h
--rw-rw-rw-   0        0        0   123697 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack3.c
--rw-rw-rw-   0        0        0      236 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack3.h
--rw-rw-rw-   0        0        0   718485 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack30.c
--rw-rw-rw-   0        0        0      243 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack30.h
--rw-rw-rw-   0        0        0   193508 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack31.c
--rw-rw-rw-   0        0        0      242 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack31.h
--rw-rw-rw-   0        0        0  2349576 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack32.c
--rw-rw-rw-   0        0        0      243 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack32.h
--rw-rw-rw-   0        0        0   126853 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack4.c
--rw-rw-rw-   0        0        0      236 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack4.h
--rw-rw-rw-   0        0        0   129975 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack5.c
--rw-rw-rw-   0        0        0      236 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack5.h
--rw-rw-rw-   0        0        0   133043 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack6.c
--rw-rw-rw-   0        0        0      236 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack6.h
--rw-rw-rw-   0        0        0   136097 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack7.c
--rw-rw-rw-   0        0        0      236 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack7.h
--rw-rw-rw-   0        0        0  5853499 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack8.c
--rw-rw-rw-   0        0        0      237 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack8.h
--rw-rw-rw-   0        0        0   140923 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack9.c
--rw-rw-rw-   0        0        0      236 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack9.h
--rw-rw-rw-   0        0        0      890 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack_all_sizes.h
--rw-rw-rw-   0        0        0    15838 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack_id.c
--rw-rw-rw-   0        0        0      295 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unpack_id.h
--rw-rw-rw-   0        0        0   115609 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unwrap.c
--rw-rw-rw-   0        0        0      269 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/src/unwrap.h
--rw-rw-rw-   0        0        0    25234 2023-03-10 20:16:49.000000 asphodel-1.3.1/lib/asphodel/unpack/unpack_generator.py
--rw-rw-rw-   0        0        0      550 2023-03-10 20:16:38.000000 asphodel-1.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       85 2023-03-10 20:17:40.625675 asphodel-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2788 2023-03-10 20:16:38.000000 asphodel-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 17:41:07.122768 asphodel-1.3.2/
+-rw-rw-rw-   0        0        0       89 2024-05-02 17:40:03.000000 asphodel-1.3.2/.gitmodules
+drwxrwxrwx   0        0        0        0 2024-05-02 17:41:06.982129 asphodel-1.3.2/.vscode/
+-rw-rw-rw-   0        0        0      127 2024-05-02 17:40:03.000000 asphodel-1.3.2/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1593 2024-05-02 17:40:03.000000 asphodel-1.3.2/CMakeLists.txt
+-rw-rw-rw-   0        0        0      757 2024-05-02 17:40:03.000000 asphodel-1.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      387 2024-05-02 17:40:03.000000 asphodel-1.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1082 2024-05-02 17:41:07.122768 asphodel-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      522 2024-05-02 17:40:03.000000 asphodel-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 17:41:06.982129 asphodel-1.3.2/asphodel/
+-rw-rw-rw-   0        0        0   178087 2024-05-02 17:40:03.000000 asphodel-1.3.2/asphodel/__init__.py
+-rw-rw-rw-   0        0        0    23521 2024-05-02 17:40:03.000000 asphodel-1.3.2/asphodel/__init__.pyi
+-rw-rw-rw-   0        0        0     7548 2024-05-02 17:40:03.000000 asphodel-1.3.2/asphodel/apdparse.py
+-rw-rw-rw-   0        0        0    10067 2024-05-02 17:40:03.000000 asphodel-1.3.2/asphodel/device_config.py
+-rw-rw-rw-   0        0        0    28639 2024-05-02 17:40:03.000000 asphodel-1.3.2/asphodel/device_info.py
+-rw-rw-rw-   0        0        0    14483 2024-05-02 17:40:03.000000 asphodel-1.3.2/asphodel/nvmeditor.py
+-rw-rw-rw-   0        0        0        0 2024-05-02 17:40:03.000000 asphodel-1.3.2/asphodel/py.typed
+-rw-rw-rw-   0        0        0     9113 2024-05-02 17:40:03.000000 asphodel-1.3.2/asphodel/streamutil.py
+-rw-rw-rw-   0        0        0      147 2024-05-02 17:41:06.000000 asphodel-1.3.2/asphodel/version.py
+drwxrwxrwx   0        0        0        0 2024-05-02 17:41:06.982129 asphodel-1.3.2/asphodel.egg-info/
+-rw-rw-rw-   0        0        0     1082 2024-05-02 17:41:06.000000 asphodel-1.3.2/asphodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5622 2024-05-02 17:41:06.000000 asphodel-1.3.2/asphodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 17:41:06.000000 asphodel-1.3.2/asphodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-02 17:41:06.000000 asphodel-1.3.2/asphodel.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-02 17:41:06.000000 asphodel-1.3.2/asphodel.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2024-05-02 17:41:06.000000 asphodel-1.3.2/asphodel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 17:41:06.000000 asphodel-1.3.2/asphodel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 17:41:06.966509 asphodel-1.3.2/lib/
+drwxrwxrwx   0        0        0        0 2024-05-02 17:41:06.982129 asphodel-1.3.2/lib/asphodel/
+-rw-rw-rw-   0        0        0     6356 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/CMakeLists.txt
+-rw-rw-rw-   0        0        0     2629 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/GitHeader.cmake
+-rw-rw-rw-   0        0        0      757 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/LICENSE.txt
+-rw-rw-rw-   0        0        0     3660 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/OVERVIEW.md
+-rw-rw-rw-   0        0        0     4503 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/README.md
+-rw-rw-rw-   0        0        0      111 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/asphodel-usb.rules
+-rw-rw-rw-   0        0        0     1543 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/buildspec.yml
+drwxrwxrwx   0        0        0        0 2024-05-02 17:41:06.997756 asphodel-1.3.2/lib/asphodel/ci-scripts/
+-rw-rw-rw-   0        0        0     5042 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/ci-scripts/build.py
+drwxrwxrwx   0        0        0        0 2024-05-02 17:41:06.966509 asphodel-1.3.2/lib/asphodel/cmake/
+drwxrwxrwx   0        0        0        0 2024-05-02 17:41:06.997756 asphodel-1.3.2/lib/asphodel/cmake/modules/
+-rw-rw-rw-   0        0        0     1839 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/cmake/modules/FindLIBUSB.cmake
+drwxrwxrwx   0        0        0        0 2024-05-02 17:41:06.997756 asphodel-1.3.2/lib/asphodel/documentation/
+-rw-rw-rw-   0        0        0    45888 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/documentation/Base Protocol.docx
+-rw-rw-rw-   0        0        0    28998 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/documentation/Bootloader Protocol.docx
+-rw-rw-rw-   0        0        0    29229 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/documentation/Channel Types.docx
+-rw-rw-rw-   0        0        0    34793 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/documentation/Low Level Interface.docx
+-rw-rw-rw-   0        0        0    28240 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/documentation/RF Power Protocol.docx
+-rw-rw-rw-   0        0        0    26728 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/documentation/Unit Types.docx
+drwxrwxrwx   0        0        0        0 2024-05-02 17:41:06.997756 asphodel-1.3.2/lib/asphodel/examples/
+-rw-rw-rw-   0        0        0      132 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/examples/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 17:41:06.997756 asphodel-1.3.2/lib/asphodel/examples/enumeration/
+-rw-rw-rw-   0        0        0      323 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/examples/enumeration/CMakeLists.txt
+-rw-rw-rw-   0        0        0    63240 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/examples/enumeration/asphodel_enumeration.c
+-rw-rw-rw-   0        0        0     2920 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/examples/enumeration/serialize.h
+drwxrwxrwx   0        0        0        0 2024-05-02 17:41:06.997756 asphodel-1.3.2/lib/asphodel/examples/reconnect_manual/
+-rw-rw-rw-   0        0        0      543 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/examples/reconnect_manual/CMakeLists.txt
+-rw-rw-rw-   0        0        0    16941 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/examples/reconnect_manual/asphodel_reconnect_manual.c
+-rw-rw-rw-   0        0        0     8272 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/examples/reconnect_manual/inttypes.h
+-rw-rw-rw-   0        0        0      815 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/examples/reconnect_manual/snprintf.h
+drwxrwxrwx   0        0        0        0 2024-05-02 17:41:07.013452 asphodel-1.3.2/lib/asphodel/examples/streaming/
+-rw-rw-rw-   0        0        0      473 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/examples/streaming/CMakeLists.txt
+-rw-rw-rw-   0        0        0    22616 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/examples/streaming/asphodel_streaming.c
+-rw-rw-rw-   0        0        0     8272 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/examples/streaming/inttypes.h
+-rw-rw-rw-   0        0        0      815 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/examples/streaming/snprintf.h
+drwxrwxrwx   0        0        0        0 2024-05-02 17:41:07.013452 asphodel-1.3.2/lib/asphodel/examples/unpack_benchmark/
+-rw-rw-rw-   0        0        0      356 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/examples/unpack_benchmark/CMakeLists.txt
+-rw-rw-rw-   0        0        0     2735 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/examples/unpack_benchmark/unpack_benchmark.c
+drwxrwxrwx   0        0        0        0 2024-05-02 17:41:07.013452 asphodel-1.3.2/lib/asphodel/inc/
+-rw-rw-rw-   0        0        0     1469 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/inc/asphodel.h
+-rw-rw-rw-   0        0        0     6859 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/inc/asphodel_api.h
+-rw-rw-rw-   0        0        0     5573 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/inc/asphodel_bootloader.h
+-rw-rw-rw-   0        0        0     6423 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/inc/asphodel_channel_specific.h
+-rw-rw-rw-   0        0        0     3245 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/inc/asphodel_ctrl_var.h
+-rw-rw-rw-   0        0        0     6737 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/inc/asphodel_decode.h
+-rw-rw-rw-   0        0        0    22659 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/inc/asphodel_device.h
+-rw-rw-rw-   0        0        0     1766 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/inc/asphodel_device_type.h
+-rw-rw-rw-   0        0        0    10733 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/inc/asphodel_low_level.h
+-rw-rw-rw-   0        0        0     1669 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/inc/asphodel_mem_test.h
+-rw-rw-rw-   0        0        0    13867 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/inc/asphodel_protocol.h
+-rw-rw-rw-   0        0        0    10192 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/inc/asphodel_radio.h
+-rw-rw-rw-   0        0        0     2851 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/inc/asphodel_rf_power.h
+-rw-rw-rw-   0        0        0     8392 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/inc/asphodel_setting.h
+-rw-rw-rw-   0        0        0    10409 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/inc/asphodel_stream.h
+-rw-rw-rw-   0        0        0     3112 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/inc/asphodel_supply.h
+-rw-rw-rw-   0        0        0     4447 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/inc/asphodel_tcp.h
+-rw-rw-rw-   0        0        0     4083 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/inc/asphodel_unit_format.h
+-rw-rw-rw-   0        0        0     2611 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/inc/asphodel_usb.h
+-rw-rw-rw-   0        0        0     1577 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/inc/asphodel_version.h
+drwxrwxrwx   0        0        0        0 2024-05-02 17:41:07.029008 asphodel-1.3.2/lib/asphodel/src/
+-rw-rw-rw-   0        0        0     8095 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/src/asphodel_api.c
+-rw-rw-rw-   0        0        0    63960 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/src/asphodel_decode.c
+-rw-rw-rw-   0        0        0   225661 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/src/asphodel_device.c
+-rw-rw-rw-   0        0        0     1750 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/src/asphodel_device_type.c
+-rw-rw-rw-   0        0        0     1892 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/src/asphodel_mem_test.c
+-rw-rw-rw-   0        0        0    84340 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/src/asphodel_tcp.c
+-rw-rw-rw-   0        0        0    22166 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/src/asphodel_unit_format.c
+-rw-rw-rw-   0        0        0    92974 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/src/asphodel_usb.c
+-rw-rw-rw-   0        0        0     2118 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/src/asphodel_version.c
+-rw-rw-rw-   0        0        0     5619 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/src/clock.c
+-rw-rw-rw-   0        0        0     1965 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/src/clock.h
+-rw-rw-rw-   0        0        0     3024 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/src/mutex.h
+-rw-rw-rw-   0        0        0     2958 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/src/serialize.h
+-rw-rw-rw-   0        0        0      815 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/src/snprintf.h
+-rw-rw-rw-   0        0        0      249 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/src/version_autogen.h.in
+drwxrwxrwx   0        0        0        0 2024-05-02 17:41:07.029008 asphodel-1.3.2/lib/asphodel/unpack/
+-rw-rw-rw-   0        0        0     1815 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 17:41:07.029008 asphodel-1.3.2/lib/asphodel/unpack/inc/
+-rw-rw-rw-   0        0        0     1923 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/inc/unpack.h
+drwxrwxrwx   0        0        0        0 2024-05-02 17:41:07.122768 asphodel-1.3.2/lib/asphodel/unpack/src/
+-rw-rw-rw-   0        0        0     9234 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack.c
+-rw-rw-rw-   0        0        0     7087 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack0.c
+-rw-rw-rw-   0        0        0      236 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack0.h
+-rw-rw-rw-   0        0        0    59873 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack1.c
+-rw-rw-rw-   0        0        0      236 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack1.h
+-rw-rw-rw-   0        0        0  3969841 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack10.c
+-rw-rw-rw-   0        0        0      243 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack10.h
+-rw-rw-rw-   0        0        0   146190 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack11.c
+-rw-rw-rw-   0        0        0      242 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack11.h
+-rw-rw-rw-   0        0        0  2865578 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack12.c
+-rw-rw-rw-   0        0        0      243 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack12.h
+-rw-rw-rw-   0        0        0   151084 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack13.c
+-rw-rw-rw-   0        0        0      242 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack13.h
+-rw-rw-rw-   0        0        0  2231612 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack14.c
+-rw-rw-rw-   0        0        0      243 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack14.h
+-rw-rw-rw-   0        0        0   156024 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack15.c
+-rw-rw-rw-   0        0        0      242 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack15.h
+-rw-rw-rw-   0        0        0  7004428 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack16.c
+-rw-rw-rw-   0        0        0      243 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack16.h
+-rw-rw-rw-   0        0        0   160868 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack17.c
+-rw-rw-rw-   0        0        0      242 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack17.h
+-rw-rw-rw-   0        0        0  1501336 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack18.c
+-rw-rw-rw-   0        0        0      243 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack18.h
+-rw-rw-rw-   0        0        0   165654 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack19.c
+-rw-rw-rw-   0        0        0      242 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack19.h
+-rw-rw-rw-   0        0        0   120471 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack2.c
+-rw-rw-rw-   0        0        0      236 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack2.h
+-rw-rw-rw-   0        0        0  1259299 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack20.c
+-rw-rw-rw-   0        0        0      243 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack20.h
+-rw-rw-rw-   0        0        0   170508 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack21.c
+-rw-rw-rw-   0        0        0      242 2024-05-02 17:40:14.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack21.h
+-rw-rw-rw-   0        0        0  1115323 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack22.c
+-rw-rw-rw-   0        0        0      243 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack22.h
+-rw-rw-rw-   0        0        0   174668 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack23.c
+-rw-rw-rw-   0        0        0      242 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack23.h
+-rw-rw-rw-   0        0        0  3580668 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack24.c
+-rw-rw-rw-   0        0        0      243 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack24.h
+-rw-rw-rw-   0        0        0   179218 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack25.c
+-rw-rw-rw-   0        0        0      242 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack25.h
+-rw-rw-rw-   0        0        0   830623 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack26.c
+-rw-rw-rw-   0        0        0      243 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack26.h
+-rw-rw-rw-   0        0        0   184018 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack27.c
+-rw-rw-rw-   0        0        0      242 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack27.h
+-rw-rw-rw-   0        0        0   775042 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack28.c
+-rw-rw-rw-   0        0        0      243 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack28.h
+-rw-rw-rw-   0        0        0   188758 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack29.c
+-rw-rw-rw-   0        0        0      242 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack29.h
+-rw-rw-rw-   0        0        0   123697 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack3.c
+-rw-rw-rw-   0        0        0      236 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack3.h
+-rw-rw-rw-   0        0        0   718485 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack30.c
+-rw-rw-rw-   0        0        0      243 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack30.h
+-rw-rw-rw-   0        0        0   193508 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack31.c
+-rw-rw-rw-   0        0        0      242 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack31.h
+-rw-rw-rw-   0        0        0  2349576 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack32.c
+-rw-rw-rw-   0        0        0      243 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack32.h
+-rw-rw-rw-   0        0        0   126853 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack4.c
+-rw-rw-rw-   0        0        0      236 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack4.h
+-rw-rw-rw-   0        0        0   129975 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack5.c
+-rw-rw-rw-   0        0        0      236 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack5.h
+-rw-rw-rw-   0        0        0   133043 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack6.c
+-rw-rw-rw-   0        0        0      236 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack6.h
+-rw-rw-rw-   0        0        0   136097 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack7.c
+-rw-rw-rw-   0        0        0      236 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack7.h
+-rw-rw-rw-   0        0        0  5853499 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack8.c
+-rw-rw-rw-   0        0        0      237 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack8.h
+-rw-rw-rw-   0        0        0   140923 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack9.c
+-rw-rw-rw-   0        0        0      236 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack9.h
+-rw-rw-rw-   0        0        0      890 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack_all_sizes.h
+-rw-rw-rw-   0        0        0    15838 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack_id.c
+-rw-rw-rw-   0        0        0      295 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unpack_id.h
+-rw-rw-rw-   0        0        0   115609 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unwrap.c
+-rw-rw-rw-   0        0        0      269 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/src/unwrap.h
+-rw-rw-rw-   0        0        0    25234 2024-05-02 17:40:15.000000 asphodel-1.3.2/lib/asphodel/unpack/unpack_generator.py
+-rw-rw-rw-   0        0        0      549 2024-05-02 17:40:03.000000 asphodel-1.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2024-05-02 17:41:07.122768 asphodel-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2799 2024-05-02 17:40:03.000000 asphodel-1.3.2/setup.py
```

### Comparing `asphodel-1.3.1/CMakeLists.txt` & `asphodel-1.3.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/LICENSE.txt` & `asphodel-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/PKG-INFO` & `asphodel-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: asphodel
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python wrapper for the Asphodel C library
 Home-page: https://bitbucket.org/suprocktech/asphodel_py
 Author: Suprock Technologies, LLC
 Author-email: inquiries@suprocktech.com
 Keywords: asphodel suprock
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: System :: Hardware
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Asphodel Python Library
 
 ## About
 The Asphodel Python Library wraps the Asphodel C Library, which supports communicating with USB and TCP devices communicating through the Asphodel communication protocol.
```

### Comparing `asphodel-1.3.1/README.md` & `asphodel-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/asphodel/__init__.py` & `asphodel-1.3.2/asphodel/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4009,14 +4009,16 @@
             device.close()
 
     return None
 
 
 nativelib = AsphodelNative()
 
+asphodel_error_name = nativelib.lib.asphodel_error_name
+
 protocol_version = nativelib.protocol_version
 protocol_version_string = nativelib.protocol_version_string
 build_info = nativelib.build_info
 build_date = nativelib.build_date
 usb_backend_version = nativelib.usb_backend_version
 
 find_usb_devices = nativelib.find_usb_devices
```

### Comparing `asphodel-1.3.1/asphodel/__init__.pyi` & `asphodel-1.3.2/asphodel/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ctypes import Structure, Union as CTUnion
 from _typeshed import Incomplete
-from typing import Any, Iterable, List, NamedTuple, Optional, Set, Tuple, Union
+from typing import Any, Callable, Iterable, List, NamedTuple, Optional, Set, Tuple, Union
 
 ASPHODEL_PROTOCOL_TYPE_BASIC: int
 ASPHODEL_PROTOCOL_TYPE_RF_POWER: int
 ASPHODEL_PROTOCOL_TYPE_RADIO: int
 ASPHODEL_PROTOCOL_TYPE_REMOTE: int
 ASPHODEL_PROTOCOL_TYPE_BOOTLOADER: int
 GPIO_PIN_MODE_HI_Z: int
@@ -154,19 +154,19 @@
 
     def to_json_obj(self) -> Any: ...
     @classmethod
     def from_json_obj(cls, obj: Any) -> "AsphodelChannelInfo": ...
 
 class SettingStructure(Structure): ...
 
-class AsphodelByteSetting(SettingStructure): 
+class AsphodelByteSetting(SettingStructure):
     nvm_word: int
     nvm_word_byte: int
 
-class AsphodelByteArraySetting(SettingStructure): 
+class AsphodelByteArraySetting(SettingStructure):
     nvm_word: int
     maximum_length: int
     length_nvm_word: int
     length_nvm_word_byte: int
 
 class AsphodelStringSetting(SettingStructure):
     nvm_word: int
@@ -216,15 +216,15 @@
     int32_setting: AsphodelInt32Setting
     int32_scaled_setting: AsphodelInt32ScaledSetting
     float_setting: AsphodelFloatSetting
     float_array_setting: AsphodelFloatArraySetting
     custom_enum_setting: AsphodelCustomEnumSetting
 
 class AsphodelSettingInfo(Structure):
-    name: str
+    name: Incomplete
     name_length: int
     default_bytes: Incomplete
     default_bytes_length: int
     setting_type: int
     u: AsphodelSettingUnion
 
     @classmethod
@@ -267,35 +267,35 @@
     def open(self) -> None: ...
     def close(self) -> None: ...
     def free(self) -> None: ...
     def __del__(self) -> None: ...
     def get_location_string(self) -> str: ...
     def get_transport_type(self) -> str: ...
     def get_serial_number(self) -> str: ...
-    def do_transfer(self, cmd: int, params: bytes, callback) -> None: ...
-    def do_transfer_reset(self, cmd: int, params: bytes, callback) -> None: ...
-    def start_streaming_packets(self, packet_count: int, transfer_count: int, timeout: int, callback) -> None: ...
+    def do_transfer(self, cmd: int, params: bytes, callback: Callable[[int, Optional[bytes]], None]) -> None: ...
+    def do_transfer_reset(self, cmd: int, params: bytes, callback: Callable[[int], None]) -> None: ...
+    def start_streaming_packets(self, packet_count: int, transfer_count: int, timeout: int, callback: Optional[Callable[[int, list[bytes]], None]]) -> None: ...
     def stop_streaming_packets(self) -> None: ...
     def get_stream_packets_blocking(self, byte_count: int, timeout: int) -> bytes: ...
     def get_max_incoming_param_length(self) -> int: ...
     def get_max_outgoing_param_length(self) -> int: ...
     def get_stream_packet_length(self) -> int: ...
     def poll_device(self, milliseconds: int) -> None: ...
-    def set_connect_callback(self, callback) -> None: ...
+    def set_connect_callback(self, callback: Optional[Callable[[int, int], None]]) -> None: ...
     def wait_for_connect(self, timeout: int) -> None: ...
     def get_remote_device(self) -> AsphodelNativeDevice: ...
     def reconnect(self, bootloader: bool = False, application: bool = False, serial_number: Optional[str] = None) -> None: ...
     def reconnect_device(self, reopen: bool = False) -> None: ...
     def reconnect_device_bootloader(self, reopen: bool = False) -> None: ...
     def reconnect_device_application(self, reopen: bool = False) -> None: ...
     def supports_rf_power_commands(self) -> bool: ...
     def supports_radio_commands(self) -> bool: ...
     def supports_remote_commands(self) -> bool: ...
     def supports_bootloader_commands(self) -> bool: ...
-    def set_error_callback(self, callback) -> None: ...
+    def set_error_callback(self, callback: Optional[Callable[[AsphodelNativeDevice, int], None]]) -> None: ...
     def tcp_get_advertisement(self) -> TCPAdvInfo: ...
     def get_protocol_version(self) -> int: ...
     def get_protocol_version_string(self) -> str: ...
     def get_board_info(self) -> Tuple[str, int]: ...
     def get_user_tag_locations(self) -> Tuple[Tuple[int, int], Tuple[int, int], Tuple[int, int]]: ...
     def get_build_info(self) -> str: ...
     def get_build_date(self) -> str: ...
@@ -327,15 +327,15 @@
     def set_rgb_values(self, index: int, values: Tuple[int, int, int], instant: bool = ...) -> None: ...
     def set_rgb_values_hex(self, index: int, hex_color: int, instant: bool = ...) -> None: ...
     def get_led_count(self) -> int: ...
     def get_led_value(self, index: int) -> int: ...
     def set_led_value(self, index: int, value: int, instant: bool = ...) -> None: ...
     def set_device_mode(self, mode) -> None: ...
     def get_device_mode(self) -> int: ...
-    def get_stream_count(self) -> int: ...
+    def get_stream_count(self) -> Tuple[int, int, int]: ...
     def get_stream(self, index: int) -> AsphodelStreamInfo: ...
     def get_stream_channels(self, index: int) -> Tuple[int, ...]: ...
     def get_stream_format(self, index: int) -> StreamFormat: ...
     def enable_stream(self, index: int, enable: bool = ...) -> None: ...
     def warm_up_stream(self, index: int, enable: bool = ...) -> None: ...
     def get_stream_status(self, index: int) -> Tuple[bool, bool]: ...
     def get_stream_rate_info(self, index: int) -> StreamRateInfo: ...
@@ -442,15 +442,15 @@
     subchannels: int
     subchannel_names: List[str]
 
     def free(self) -> None: ...
     def reset(self) -> None: ...
     def decode(self, counter: int, buffer: bytes) -> None: ...
     def set_conversion_factor(self, scale: float, offset: float) -> None: ...
-    def set_callback(self, cb) -> None: ...
+    def set_callback(self, cb: Callable[[int, list[float], int, int], None]) -> None: ...
 
 class AsphodelNativeStreamDecoder:
     lib: AsphodelNative
     stream_info: AsphodelStreamInfo
     bit_offset: int
     device_decoder: AsphodelNativeDeviceDecoder
     counter_byte_offset: int
@@ -458,28 +458,28 @@
     channels: int
     decoders: List[AsphodelNativeChannelDecoder]
     last_count: int
 
     def free(self) -> None: ...
     def reset(self) -> None: ...
     def decode(self, buffer: bytes) -> None: ...
-    def set_lost_packet_callback(self, cb) -> None: ...
+    def set_lost_packet_callback(self, cb: Callable[[int, int], None]) -> None: ...
 
 class AsphodelNativeDeviceDecoder:
     lib: AsphodelNative
     id_byte_offset: int
     used_bits: int
     streams: int
     stream_ids: List[int]
     decoders: List[AsphodelNativeStreamDecoder]
 
     def free(self) -> None: ...
     def reset(self) -> None: ...
     def decode(self, buffer: bytes) -> None: ...
-    def set_unknown_id_callback(self, cb) -> None: ...
+    def set_unknown_id_callback(self, cb: Callable[[int], None]) -> None: ...
 
 class AsphodelNativeUnitFormatter:
     lib: AsphodelNative
     unit_ascii: str
     unit_utf8: str
     unit_html: str
     conversion_scale: float
@@ -492,14 +492,15 @@
     def format_html(self, value: float) -> str: ...
 
 def format_nvm_data(data, size: int = ...) -> List[str]: ...
 def find_devices() -> List[AsphodelNativeDevice]: ...
 def find_device_by_serial(serial: str) -> Optional[AsphodelNativeDevice]: ...
 
 nativelib: AsphodelNative
+def asphodel_error_name(error_code: int) -> str: ...
 protocol_version: int
 protocol_version_string: str
 build_info: str
 build_date: str
 usb_backend_version: str
 def find_usb_devices() -> List[AsphodelNativeDevice]: ...
 def find_tcp_devices(flags: Optional[int]=None) -> List[AsphodelNativeDevice]: ...
```

### Comparing `asphodel-1.3.1/asphodel/apdparse.py` & `asphodel-1.3.2/asphodel/apdparse.py`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/asphodel/nvmeditor.py` & `asphodel-1.3.2/asphodel/nvmeditor.py`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/asphodel/streamutil.py` & `asphodel-1.3.2/asphodel/streamutil.py`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/asphodel.egg-info/PKG-INFO` & `asphodel-1.3.2/asphodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: asphodel
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python wrapper for the Asphodel C library
 Home-page: https://bitbucket.org/suprocktech/asphodel_py
 Author: Suprock Technologies, LLC
 Author-email: inquiries@suprocktech.com
 Keywords: asphodel suprock
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: System :: Hardware
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Asphodel Python Library
 
 ## About
 The Asphodel Python Library wraps the Asphodel C Library, which supports communicating with USB and TCP devices communicating through the Asphodel communication protocol.
```

### Comparing `asphodel-1.3.1/asphodel.egg-info/SOURCES.txt` & `asphodel-1.3.2/asphodel.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 CMakeLists.txt
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+.vscode/settings.json
 asphodel/__init__.py
 asphodel/__init__.pyi
 asphodel/apdparse.py
+asphodel/device_config.py
+asphodel/device_info.py
 asphodel/nvmeditor.py
+asphodel/py.typed
 asphodel/streamutil.py
 asphodel/version.py
 asphodel.egg-info/PKG-INFO
 asphodel.egg-info/SOURCES.txt
 asphodel.egg-info/dependency_links.txt
 asphodel.egg-info/entry_points.txt
 asphodel.egg-info/not-zip-safe
```

### Comparing `asphodel-1.3.1/lib/asphodel/CMakeLists.txt` & `asphodel-1.3.2/lib/asphodel/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/GitHeader.cmake` & `asphodel-1.3.2/lib/asphodel/GitHeader.cmake`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/LICENSE.txt` & `asphodel-1.3.2/lib/asphodel/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/OVERVIEW.md` & `asphodel-1.3.2/lib/asphodel/OVERVIEW.md`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/README.md` & `asphodel-1.3.2/lib/asphodel/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ## License
 The Apshodel Library is licensed under the ISC license.
 
 The ISC license is a streamlined version of the BSD license, and permits usage in both open source and propretary projects.
 
 ## Dependencies
 ### libusb-1.0
-libusb-1.0: http://libusb.info/ 
+libusb-1.0: http://libusb.info/
 
 libusb-1.0 is the only runtime dependency.
 
 Asphodel has been tested with libusb-1.0 version 1.0.20.
 
 ### CMake
 CMake: http://www.cmake.org/
@@ -62,15 +62,15 @@
 Other compilers can be used with CMake by setting the CC flag while calling CMake. For example, to configure the build to use Clang:
 
     $ mkdir build_clang
     $ cd build_clang
     $ CC=/usr/bin/clang cmake -DCMAKE_BUILD_TYPE=Release ..
 
 ## Building From Source (Windows)
-CMake supports generating Visual Studio projects directly. 
+CMake supports generating Visual Studio projects directly.
 
 CMake can only generate visual studio solutions for one architecture at a time. The preferred solution is to create two seperate build directories; one for x86 and one for x86_64. From a command line in the asphodel source folder:
 
     $ mkdir build32
     $ cd build32
     $ cmake -G"Visual Studio 14 2015" ..
 
@@ -94,7 +94,10 @@
 
     $ cmake -DSTATIC_LIB=ON ..
 
 ## Asphodel Devices and udev
 By default on most Linux distributions, USB devices require root priveledges to access. The included udev rule file "asphodel-usb.rules" can be placed in /etc/udev/rules.d/ (or similar) to allow unpriveledged access to any Asphodel USB devices.
 
 udev may need to be restarted after adding the rule file, and additionally any attached Asphodel compatible devices should be unplugged and then reattached.
+
+## Pronunciation
+Commonly pronounced "AS-fuh-del" in English. In Greek mythology the Asphodel Fields are a part of the underworld, situated between Elysium and Tartarus.
```

### Comparing `asphodel-1.3.1/lib/asphodel/buildspec.yml` & `asphodel-1.3.2/lib/asphodel/buildspec.yml`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/ci-scripts/build.py` & `asphodel-1.3.2/lib/asphodel/ci-scripts/build.py`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/cmake/modules/FindLIBUSB.cmake` & `asphodel-1.3.2/lib/asphodel/cmake/modules/FindLIBUSB.cmake`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/documentation/Base Protocol.docx` & `asphodel-1.3.2/lib/asphodel/documentation/Base Protocol.docx`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/documentation/Bootloader Protocol.docx` & `asphodel-1.3.2/lib/asphodel/documentation/Bootloader Protocol.docx`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/documentation/Channel Types.docx` & `asphodel-1.3.2/lib/asphodel/documentation/Channel Types.docx`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/documentation/Low Level Interface.docx` & `asphodel-1.3.2/lib/asphodel/documentation/Low Level Interface.docx`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/documentation/RF Power Protocol.docx` & `asphodel-1.3.2/lib/asphodel/documentation/RF Power Protocol.docx`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/documentation/Unit Types.docx` & `asphodel-1.3.2/lib/asphodel/documentation/Unit Types.docx`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/examples/enumeration/asphodel_enumeration.c` & `asphodel-1.3.2/lib/asphodel/examples/enumeration/asphodel_enumeration.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/examples/enumeration/serialize.h` & `asphodel-1.3.2/lib/asphodel/examples/enumeration/serialize.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/examples/reconnect_manual/CMakeLists.txt` & `asphodel-1.3.2/lib/asphodel/examples/reconnect_manual/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/examples/reconnect_manual/asphodel_reconnect_manual.c` & `asphodel-1.3.2/lib/asphodel/examples/reconnect_manual/asphodel_reconnect_manual.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/examples/reconnect_manual/inttypes.h` & `asphodel-1.3.2/lib/asphodel/examples/reconnect_manual/inttypes.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/examples/reconnect_manual/snprintf.h` & `asphodel-1.3.2/lib/asphodel/examples/reconnect_manual/snprintf.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/examples/streaming/asphodel_streaming.c` & `asphodel-1.3.2/lib/asphodel/examples/streaming/asphodel_streaming.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/examples/streaming/inttypes.h` & `asphodel-1.3.2/lib/asphodel/examples/streaming/inttypes.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/examples/streaming/snprintf.h` & `asphodel-1.3.2/lib/asphodel/examples/streaming/snprintf.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/examples/unpack_benchmark/unpack_benchmark.c` & `asphodel-1.3.2/lib/asphodel/examples/unpack_benchmark/unpack_benchmark.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/inc/asphodel.h` & `asphodel-1.3.2/lib/asphodel/inc/asphodel.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/inc/asphodel_api.h` & `asphodel-1.3.2/lib/asphodel/inc/asphodel_api.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/inc/asphodel_bootloader.h` & `asphodel-1.3.2/lib/asphodel/inc/asphodel_bootloader.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/inc/asphodel_channel_specific.h` & `asphodel-1.3.2/lib/asphodel/inc/asphodel_channel_specific.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/inc/asphodel_ctrl_var.h` & `asphodel-1.3.2/lib/asphodel/inc/asphodel_ctrl_var.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/inc/asphodel_decode.h` & `asphodel-1.3.2/lib/asphodel/inc/asphodel_decode.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/inc/asphodel_device.h` & `asphodel-1.3.2/lib/asphodel/inc/asphodel_device.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/inc/asphodel_device_type.h` & `asphodel-1.3.2/lib/asphodel/inc/asphodel_device_type.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/inc/asphodel_low_level.h` & `asphodel-1.3.2/lib/asphodel/inc/asphodel_low_level.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/inc/asphodel_mem_test.h` & `asphodel-1.3.2/lib/asphodel/inc/asphodel_mem_test.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/inc/asphodel_protocol.h` & `asphodel-1.3.2/lib/asphodel/inc/asphodel_protocol.h`

 * *Files 0% similar despite different names*

```diff
@@ -13,19 +13,19 @@
  * OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN
  * CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
  */
 
 #ifndef ASPHODEL_PROTOCOL_H_
 #define ASPHODEL_PROTOCOL_H_
 
-// Asphodel protocol version 2.3.1
+// Asphodel protocol version 2.3.2
 // NOTE: use the functions in asphodel_version.h to access the protocol version
 #define ASPHODEL_PROTOCOL_VERSION_MAJOR      0x02
 #define ASPHODEL_PROTOCOL_VERSION_MINOR      0x03
-#define ASPHODEL_PROTOCOL_VERSION_SUBMINOR   0x01
+#define ASPHODEL_PROTOCOL_VERSION_SUBMINOR   0x02
 
 // USB class/subclass defines
 // use one ASPHODEL_PROTOCOL_TYPE_* as the USB protocol definition
 #define ASPHODEL_USB_CLASS                   0xFF // 0xFF: vendor specific USB class
 #define ASPHODEL_USB_SUBCLASS                0x01 // 0x01: Generic Sensor
 
 // protocol types to define various implementations
```

### Comparing `asphodel-1.3.1/lib/asphodel/inc/asphodel_radio.h` & `asphodel-1.3.2/lib/asphodel/inc/asphodel_radio.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/inc/asphodel_rf_power.h` & `asphodel-1.3.2/lib/asphodel/inc/asphodel_rf_power.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/inc/asphodel_setting.h` & `asphodel-1.3.2/lib/asphodel/inc/asphodel_setting.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/inc/asphodel_stream.h` & `asphodel-1.3.2/lib/asphodel/inc/asphodel_stream.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/inc/asphodel_supply.h` & `asphodel-1.3.2/lib/asphodel/inc/asphodel_supply.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/inc/asphodel_tcp.h` & `asphodel-1.3.2/lib/asphodel/inc/asphodel_tcp.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/inc/asphodel_unit_format.h` & `asphodel-1.3.2/lib/asphodel/inc/asphodel_unit_format.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/inc/asphodel_usb.h` & `asphodel-1.3.2/lib/asphodel/inc/asphodel_usb.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/inc/asphodel_version.h` & `asphodel-1.3.2/lib/asphodel/inc/asphodel_version.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/src/asphodel_api.c` & `asphodel-1.3.2/lib/asphodel/src/asphodel_api.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/src/asphodel_decode.c` & `asphodel-1.3.2/lib/asphodel/src/asphodel_decode.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/src/asphodel_device.c` & `asphodel-1.3.2/lib/asphodel/src/asphodel_device.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/src/asphodel_device_type.c` & `asphodel-1.3.2/lib/asphodel/src/asphodel_device_type.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/src/asphodel_mem_test.c` & `asphodel-1.3.2/lib/asphodel/src/asphodel_mem_test.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/src/asphodel_tcp.c` & `asphodel-1.3.2/lib/asphodel/src/asphodel_tcp.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/src/asphodel_unit_format.c` & `asphodel-1.3.2/lib/asphodel/src/asphodel_unit_format.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/src/asphodel_usb.c` & `asphodel-1.3.2/lib/asphodel/src/asphodel_usb.c`

 * *Files 0% similar despite different names*

```diff
@@ -1292,15 +1292,30 @@
 					}
 				}
 
 				free(c);
 			}
 			else
 			{
+				int ret;
+
 				usb_error_report(device, ASPHODEL_MISMATCHED_TRANSACTION);
+
+				// resubmit and hope for the actual response
+				ret = libusb_submit_transfer(transfer);
+				if (ret == 0)
+				{
+					// success, leave early so nothing gets freed
+					mutex_unlock(usb_info->mutex);
+					return;
+				}
+				else
+				{
+					usb_error_report(device, usb_libusb_error_to_asphodel(ret));
+				}
 			}
 		}
 	}
 	else if (transfer->status != LIBUSB_TRANSFER_TIMED_OUT)
 	{
 		// error
 		usb_error_report(device, ASPHODEL_TRANSFER_ERROR);
@@ -2340,15 +2355,15 @@
 
 	remote_usb_info->opened = 0;
 	remote_usb_info->streaming = 0;
 	remote_usb_info->connected = 0;
 	remote_usb_info->devh = NULL;
 	remote_usb_info->config_desc = NULL; // unneeded, not worth copying over
 	remote_usb_info->serial_number = NULL;
-	remote_usb_info->cmd_timeout = 200; // 2x default timeout
+	remote_usb_info->cmd_timeout = 300; // 3x default timeout
 	memset(remote_usb_info->transaction_table, 0, sizeof(remote_usb_info->transaction_table));
 	remote_usb_info->last_transaction_id = 0;
 	remote_usb_info->ctrl_list_head = NULL;
 	remote_usb_info->status_transfer = NULL;
 	remote_usb_info->connect_callback = NULL;
 	remote_usb_info->connect_closure = NULL;
 	remote_usb_info->remote_same_interface = 0; // not applicable
```

### Comparing `asphodel-1.3.1/lib/asphodel/src/asphodel_version.c` & `asphodel-1.3.2/lib/asphodel/src/asphodel_version.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/src/clock.c` & `asphodel-1.3.2/lib/asphodel/src/clock.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/src/clock.h` & `asphodel-1.3.2/lib/asphodel/src/clock.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/src/mutex.h` & `asphodel-1.3.2/lib/asphodel/src/mutex.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/src/serialize.h` & `asphodel-1.3.2/lib/asphodel/src/serialize.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/src/snprintf.h` & `asphodel-1.3.2/lib/asphodel/src/snprintf.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/CMakeLists.txt` & `asphodel-1.3.2/lib/asphodel/unpack/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/inc/unpack.h` & `asphodel-1.3.2/lib/asphodel/unpack/inc/unpack.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack0.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack0.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack1.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack1.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack10.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack10.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack11.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack11.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack12.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack12.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack13.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack13.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack14.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack14.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack15.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack15.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack16.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack16.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack17.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack17.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack18.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack18.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack19.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack19.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack2.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack2.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack20.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack20.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack21.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack21.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack22.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack22.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack23.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack23.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack24.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack24.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack25.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack25.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack26.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack26.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack27.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack27.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack28.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack28.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack29.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack29.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack3.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack3.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack30.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack30.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack31.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack31.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack32.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack32.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack4.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack4.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack5.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack5.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack6.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack6.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack7.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack7.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack8.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack8.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack9.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack9.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack_all_sizes.h` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack_all_sizes.h`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unpack_id.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unpack_id.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/src/unwrap.c` & `asphodel-1.3.2/lib/asphodel/unpack/src/unwrap.c`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/lib/asphodel/unpack/unpack_generator.py` & `asphodel-1.3.2/lib/asphodel/unpack/unpack_generator.py`

 * *Files identical despite different names*

### Comparing `asphodel-1.3.1/setup.py` & `asphodel-1.3.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 try:
     from skbuild.command.bdist_wheel import bdist_wheel
 
     class CustomBdistWheel(bdist_wheel):
         def get_tag(self):
             rv = bdist_wheel.get_tag(self)
-            l = [self.python_tag, 'none']
-            l.extend(rv[2:])
-            return tuple(l)
+            tag = ["py39", 'none']  # python 3.9
+            tag.extend(rv[2:])
+            return tuple(tag)
 except ImportError:
     CustomBdistWheel = None
 
 
 if sys.platform == "win32":
     # download libusb zip, and force use of msvc
     cmake_args = ['-DCMAKE_C_COMPILER=cl.exe', '-DCMAKE_CXX_COMPILER=cl.exe']
@@ -64,15 +64,15 @@
     keywords="asphodel suprock",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: ISC License (ISCL)",
         "Operating System :: OS Independent",
         "Topic :: System :: Hardware",
     ],
-    python_requires=">=3.8",
+    python_requires=">=3.9",
     install_requires=[
         "numpy",
     ],
     entry_points={
         'console_scripts': [
             'nvmeditor = asphodel.nvmeditor:main',
         ],
```

